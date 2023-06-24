# Comparing `tmp/timeplus-1.3.0b0.tar.gz` & `tmp/timeplus-1.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeplus-1.3.0b0.tar", last modified: Thu Jun 22 17:23:32 2023, max compression
+gzip compressed data, was "timeplus-1.3.0b1.tar", last modified: Fri Jun 23 23:57:17 2023, max compression
```

## Comparing `timeplus-1.3.0b0.tar` & `timeplus-1.3.0b1.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-22 17:23:32.877306 timeplus-1.3.0b0/
--rw-r--r--   0 gangtao    (502) staff       (20)     4899 2023-06-22 17:23:32.877476 timeplus-1.3.0b0/PKG-INFO
--rw-r--r--   0 gangtao    (502) staff       (20)     4455 2023-06-20 17:23:51.000000 timeplus-1.3.0b0/README.md
--rw-r--r--   0 gangtao    (502) staff       (20)      633 2023-06-22 17:23:32.878333 timeplus-1.3.0b0/setup.cfg
--rw-r--r--   0 gangtao    (502) staff       (20)     1273 2023-06-22 17:15:02.000000 timeplus-1.3.0b0/setup.py
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-22 17:23:32.781214 timeplus-1.3.0b0/swagger_client/
--rw-r--r--   0 gangtao    (502) staff       (20)     5204 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/__init__.py
--rw-r--r--   0 gangtao    (502) staff       (20)    25043 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/api_client.py
--rw-r--r--   0 gangtao    (502) staff       (20)     8229 2023-02-14 06:04:34.000000 timeplus-1.3.0b0/swagger_client/configuration.py
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-22 17:23:32.816650 timeplus-1.3.0b0/swagger_client/models/
--rw-r--r--   0 gangtao    (502) staff       (20)     4099 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/models/__init__.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3010 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/analyze_sql_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6294 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/api_key.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3907 2023-02-14 06:04:34.000000 timeplus-1.3.0b0/swagger_client/models/batching_policy.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3495 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/column.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6897 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/column_def.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4844 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/models/columns_resp.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5165 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/create_api_key_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     7665 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/create_api_key_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4618 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/create_dashboard_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6083 2023-02-14 06:04:34.000000 timeplus-1.3.0b0/swagger_client/models/create_query_request_v1_beta2.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5948 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/create_sink_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6899 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/models/create_source_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6447 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/models/create_view_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     8467 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/dashboard_dashboard.py
--rw-r--r--   0 gangtao    (502) staff       (20)     7960 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/dashboard_panel.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3551 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/edge.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3639 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/error_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)     2623 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/event.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3056 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/event_infer_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4271 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/event_infer_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5147 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/external_stream_def.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3038 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/file_upload_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3018 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/format_query_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3026 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/format_query_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5084 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/models/global_metrics_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3565 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/graph.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3666 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/ingest_data.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3880 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/models/metrics_query_throughput.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5334 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/node.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3443 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/owner.py
--rw-r--r--   0 gangtao    (502) staff       (20)    15636 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/query.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3739 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/query_pipeline.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3606 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/query_pipeline_edge.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4921 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/query_pipeline_node.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4199 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/query_pipeline_node_metric.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3752 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/query_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5782 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/models/resource_metrics_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)    10676 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/models/sink.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3879 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/sink_stat.py
--rw-r--r--   0 gangtao    (502) staff       (20)    12051 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/models/source.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5811 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/models/source_preview_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3189 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/source_upload_body.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5737 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/sql_analyze_column.py
--rw-r--r--   0 gangtao    (502) staff       (20)    11019 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/sql_analyze_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)    13632 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/models/stream.py
--rw-r--r--   0 gangtao    (502) staff       (20)    15463 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/models/stream_def.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3102 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/stream_match_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3579 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/stream_setting.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6394 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/models/stream_stats.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4794 2023-02-14 06:04:34.000000 timeplus-1.3.0b0/swagger_client/models/time_columns.py
--rw-r--r--   0 gangtao    (502) staff       (20)    15879 2023-02-14 06:04:34.000000 timeplus-1.3.0b0/swagger_client/models/udf.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3555 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/udf_argument.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3771 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/udf_auth_context.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4618 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/models/update_dashboard_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5961 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/models/update_source_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6279 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/models/update_stream_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6856 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/models/update_view_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)    11854 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/models/view.py
--rw-r--r--   0 gangtao    (502) staff       (20)    12995 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/rest.py
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-22 17:23:32.825971 timeplus-1.3.0b0/swagger_client/timeplus/
--rw-r--r--   0 gangtao    (502) staff       (20)     1040 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/timeplus/__init__.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4723 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/timeplus/alerts_internal_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4385 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/timeplus/alerts_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    11402 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/timeplus/api_keys_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    19476 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/timeplus/dashboards_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)     9044 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/timeplus/metrics_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    31463 2023-06-07 00:11:27.000000 timeplus-1.3.0b0/swagger_client/timeplus/queries_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4703 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/timeplus/sinks_internal_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    18309 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/timeplus/sinks_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    42086 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/timeplus/sources_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    33693 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/timeplus/streams_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3866 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_client/timeplus/topology_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    18450 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/timeplus/udfs_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    22977 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_client/timeplus/views_v1beta2_api.py
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-22 17:23:32.864007 timeplus-1.3.0b0/swagger_test/
--rw-r--r--   0 gangtao    (502) staff       (20)       15 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_test/__init__.py
--rw-r--r--   0 gangtao    (502) staff       (20)      920 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_test/test_alerts_internal_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      872 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_test/test_alerts_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_analyze_sql_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      842 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_api_key.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1215 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_test/test_api_keys_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      906 2023-02-14 06:04:34.000000 timeplus-1.3.0b0/swagger_test/test_batching_policy.py
--rw-r--r--   0 gangtao    (502) staff       (20)      840 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_column.py
--rw-r--r--   0 gangtao    (502) staff       (20)      866 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_column_def.py
--rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_columns_resp.py
--rw-r--r--   0 gangtao    (502) staff       (20)      950 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_create_api_key_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      958 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_create_api_key_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)      972 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_create_dashboard_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1000 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_create_query_request_v1_beta2.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_create_sink_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_create_source_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_test/test_create_view_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      938 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_dashboard_dashboard.py
--rw-r--r--   0 gangtao    (502) staff       (20)      906 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_dashboard_panel.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1547 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_dashboards_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_edge.py
--rw-r--r--   0 gangtao    (502) staff       (20)      898 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_error_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_event.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_event_infer_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_event_infer_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_external_stream_def.py
--rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_file_upload_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_format_query_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_format_query_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_global_metrics_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_graph.py
--rw-r--r--   0 gangtao    (502) staff       (20)      874 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_ingest_data.py
--rw-r--r--   0 gangtao    (502) staff       (20)      972 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_test/test_metrics_query_throughput.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1058 2023-02-14 06:04:34.000000 timeplus-1.3.0b0/swagger_test/test_metrics_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_node.py
--rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_owner.py
--rw-r--r--   0 gangtao    (502) staff       (20)     2014 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_test/test_queries_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_query.py
--rw-r--r--   0 gangtao    (502) staff       (20)      898 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_query_pipeline.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_query_pipeline_edge.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_query_pipeline_node.py
--rw-r--r--   0 gangtao    (502) staff       (20)      982 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_query_pipeline_node_metric.py
--rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_query_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)      964 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_resource_metrics_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_sink.py
--rw-r--r--   0 gangtao    (502) staff       (20)      858 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_sink_stat.py
--rw-r--r--   0 gangtao    (502) staff       (20)      911 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_test/test_sinks_internal_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1456 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_test/test_sinks_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      840 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_source.py
--rw-r--r--   0 gangtao    (502) staff       (20)      956 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_source_preview_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      924 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_source_upload_body.py
--rw-r--r--   0 gangtao    (502) staff       (20)     2519 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_test/test_sources_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      924 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_sql_analyze_column.py
--rw-r--r--   0 gangtao    (502) staff       (20)      924 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_sql_analyze_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)      840 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_stream.py
--rw-r--r--   0 gangtao    (502) staff       (20)      866 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_stream_def.py
--rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_stream_match_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      898 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_stream_setting.py
--rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_stream_stats.py
--rw-r--r--   0 gangtao    (502) staff       (20)     2036 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_test/test_streams_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_time_columns.py
--rw-r--r--   0 gangtao    (502) staff       (20)      873 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_topology_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      816 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_udf.py
--rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_udf_argument.py
--rw-r--r--   0 gangtao    (502) staff       (20)      908 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_udf_auth_context.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1438 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_test/test_udfs_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      972 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_update_dashboard_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_update_source_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_update_stream_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_update_view_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.3.0b0/swagger_test/test_view.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1636 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/swagger_test/test_views_v1beta2_api.py
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-22 17:23:32.872809 timeplus-1.3.0b0/test/
--rw-r--r--   0 gangtao    (502) staff       (20)      624 2022-12-29 02:29:17.000000 timeplus-1.3.0b0/test/test_stream.py
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-22 17:23:32.872301 timeplus-1.3.0b0/timeplus/
--rw-r--r--   0 gangtao    (502) staff       (20)      899 2023-06-22 17:15:02.000000 timeplus-1.3.0b0/timeplus/__init__.py
--rw-r--r--   0 gangtao    (502) staff       (20)     7530 2023-06-22 17:15:02.000000 timeplus-1.3.0b0/timeplus/dbapi.py
--rw-r--r--   0 gangtao    (502) staff       (20)      931 2023-06-06 23:40:05.000000 timeplus-1.3.0b0/timeplus/env.py
--rw-r--r--   0 gangtao    (502) staff       (20)      903 2023-06-22 17:15:02.000000 timeplus-1.3.0b0/timeplus/error.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3730 2023-06-22 17:15:02.000000 timeplus-1.3.0b0/timeplus/query.py
--rw-r--r--   0 gangtao    (502) staff       (20)     7390 2023-06-22 17:15:02.000000 timeplus-1.3.0b0/timeplus/sqlalchemy.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4886 2023-06-22 17:15:02.000000 timeplus-1.3.0b0/timeplus/stream.py
--rw-r--r--   0 gangtao    (502) staff       (20)      527 2022-12-28 18:52:21.000000 timeplus-1.3.0b0/timeplus/type.py
--rw-r--r--   0 gangtao    (502) staff       (20)       39 2023-06-22 17:23:27.000000 timeplus-1.3.0b0/timeplus/version.py
--rw-r--r--   0 gangtao    (502) staff       (20)     2613 2023-06-22 17:15:02.000000 timeplus-1.3.0b0/timeplus/view.py
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-22 17:23:32.876863 timeplus-1.3.0b0/timeplus.egg-info/
--rw-r--r--   0 gangtao    (502) staff       (20)     4899 2023-06-22 17:23:32.000000 timeplus-1.3.0b0/timeplus.egg-info/PKG-INFO
--rw-r--r--   0 gangtao    (502) staff       (20)     6596 2023-06-22 17:23:32.000000 timeplus-1.3.0b0/timeplus.egg-info/SOURCES.txt
--rw-r--r--   0 gangtao    (502) staff       (20)        1 2023-06-22 17:23:32.000000 timeplus-1.3.0b0/timeplus.egg-info/dependency_links.txt
--rw-r--r--   0 gangtao    (502) staff       (20)      101 2023-06-22 17:23:32.000000 timeplus-1.3.0b0/timeplus.egg-info/requires.txt
--rw-r--r--   0 gangtao    (502) staff       (20)       37 2023-06-22 17:23:32.000000 timeplus-1.3.0b0/timeplus.egg-info/top_level.txt
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-23 23:57:17.835053 timeplus-1.3.0b1/
+-rw-r--r--   0 gangtao    (502) staff       (20)     4899 2023-06-23 23:57:17.835246 timeplus-1.3.0b1/PKG-INFO
+-rw-r--r--   0 gangtao    (502) staff       (20)     4455 2023-06-20 17:23:51.000000 timeplus-1.3.0b1/README.md
+-rw-r--r--   0 gangtao    (502) staff       (20)      633 2023-06-23 23:57:17.836076 timeplus-1.3.0b1/setup.cfg
+-rw-r--r--   0 gangtao    (502) staff       (20)     1273 2023-06-22 17:15:02.000000 timeplus-1.3.0b1/setup.py
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-23 23:57:17.711055 timeplus-1.3.0b1/swagger_client/
+-rw-r--r--   0 gangtao    (502) staff       (20)     5204 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/__init__.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    25043 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/api_client.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     8229 2023-02-14 06:04:34.000000 timeplus-1.3.0b1/swagger_client/configuration.py
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-23 23:57:17.758662 timeplus-1.3.0b1/swagger_client/models/
+-rw-r--r--   0 gangtao    (502) staff       (20)     4099 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/models/__init__.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3010 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/analyze_sql_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6294 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/api_key.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3907 2023-02-14 06:04:34.000000 timeplus-1.3.0b1/swagger_client/models/batching_policy.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3495 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/column.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6897 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/column_def.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4844 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/models/columns_resp.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5165 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/create_api_key_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     7665 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/create_api_key_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4618 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/create_dashboard_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6083 2023-02-14 06:04:34.000000 timeplus-1.3.0b1/swagger_client/models/create_query_request_v1_beta2.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5948 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/create_sink_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6899 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/models/create_source_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6447 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/models/create_view_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     8467 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/dashboard_dashboard.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     7960 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/dashboard_panel.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3551 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/edge.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3639 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/error_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     2623 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/event.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3056 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/event_infer_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4271 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/event_infer_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5147 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/external_stream_def.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3038 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/file_upload_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3018 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/format_query_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3026 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/format_query_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5084 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/models/global_metrics_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3565 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/graph.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3666 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/ingest_data.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3880 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/models/metrics_query_throughput.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5334 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/node.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3443 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/owner.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    15636 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/query.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3739 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/query_pipeline.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3606 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/query_pipeline_edge.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4921 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/query_pipeline_node.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4199 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/query_pipeline_node_metric.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3752 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/query_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5782 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/models/resource_metrics_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    10676 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/models/sink.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3879 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/sink_stat.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    12051 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/models/source.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5811 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/models/source_preview_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3189 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/source_upload_body.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5737 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/sql_analyze_column.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    11019 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/sql_analyze_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    13632 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/models/stream.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    15463 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/models/stream_def.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3102 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/stream_match_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3579 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/stream_setting.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6394 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/models/stream_stats.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4794 2023-02-14 06:04:34.000000 timeplus-1.3.0b1/swagger_client/models/time_columns.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    15879 2023-02-14 06:04:34.000000 timeplus-1.3.0b1/swagger_client/models/udf.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3555 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/udf_argument.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3771 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/udf_auth_context.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4618 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/models/update_dashboard_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5961 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/models/update_source_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6279 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/models/update_stream_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6856 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/models/update_view_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    11854 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/models/view.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    12995 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/rest.py
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-23 23:57:17.771381 timeplus-1.3.0b1/swagger_client/timeplus/
+-rw-r--r--   0 gangtao    (502) staff       (20)     1040 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/timeplus/__init__.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4723 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/timeplus/alerts_internal_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4385 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/timeplus/alerts_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    11402 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/timeplus/api_keys_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    19476 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/timeplus/dashboards_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     9044 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/timeplus/metrics_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    31463 2023-06-07 00:11:27.000000 timeplus-1.3.0b1/swagger_client/timeplus/queries_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4703 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/timeplus/sinks_internal_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    18309 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/timeplus/sinks_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    42086 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/timeplus/sources_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    33693 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/timeplus/streams_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3866 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_client/timeplus/topology_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    18450 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/timeplus/udfs_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    22977 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_client/timeplus/views_v1beta2_api.py
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-23 23:57:17.822180 timeplus-1.3.0b1/swagger_test/
+-rw-r--r--   0 gangtao    (502) staff       (20)       15 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_test/__init__.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      920 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_test/test_alerts_internal_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      872 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_test/test_alerts_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_analyze_sql_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      842 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_api_key.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     1215 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_test/test_api_keys_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      906 2023-02-14 06:04:34.000000 timeplus-1.3.0b1/swagger_test/test_batching_policy.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      840 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_column.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      866 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_column_def.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_columns_resp.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      950 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_create_api_key_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      958 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_create_api_key_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      972 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_create_dashboard_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     1000 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_create_query_request_v1_beta2.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_create_sink_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_create_source_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_test/test_create_view_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      938 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_dashboard_dashboard.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      906 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_dashboard_panel.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     1547 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_dashboards_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_edge.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      898 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_error_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_event.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_event_infer_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_event_infer_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_external_stream_def.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_file_upload_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_format_query_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_format_query_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_global_metrics_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_graph.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      874 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_ingest_data.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      972 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_test/test_metrics_query_throughput.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     1058 2023-02-14 06:04:34.000000 timeplus-1.3.0b1/swagger_test/test_metrics_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_node.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_owner.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     2014 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_test/test_queries_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_query.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      898 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_query_pipeline.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_query_pipeline_edge.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_query_pipeline_node.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      982 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_query_pipeline_node_metric.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_query_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      964 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_resource_metrics_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_sink.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      858 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_sink_stat.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      911 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_test/test_sinks_internal_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     1456 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_test/test_sinks_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      840 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_source.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      956 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_source_preview_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      924 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_source_upload_body.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     2519 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_test/test_sources_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      924 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_sql_analyze_column.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      924 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_sql_analyze_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      840 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_stream.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      866 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_stream_def.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_stream_match_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      898 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_stream_setting.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_stream_stats.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     2036 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_test/test_streams_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_time_columns.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      873 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_topology_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      816 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_udf.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_udf_argument.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      908 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_udf_auth_context.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     1438 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_test/test_udfs_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      972 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_update_dashboard_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_update_source_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_update_stream_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_update_view_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.3.0b1/swagger_test/test_view.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     1636 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/swagger_test/test_views_v1beta2_api.py
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-23 23:57:17.830719 timeplus-1.3.0b1/test/
+-rw-r--r--   0 gangtao    (502) staff       (20)      624 2022-12-29 02:29:17.000000 timeplus-1.3.0b1/test/test_stream.py
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-23 23:57:17.830022 timeplus-1.3.0b1/timeplus/
+-rw-r--r--   0 gangtao    (502) staff       (20)      899 2023-06-22 17:15:02.000000 timeplus-1.3.0b1/timeplus/__init__.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     7569 2023-06-23 23:56:57.000000 timeplus-1.3.0b1/timeplus/dbapi.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      931 2023-06-06 23:40:05.000000 timeplus-1.3.0b1/timeplus/env.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      903 2023-06-22 17:15:02.000000 timeplus-1.3.0b1/timeplus/error.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3730 2023-06-22 17:15:02.000000 timeplus-1.3.0b1/timeplus/query.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     7314 2023-06-23 23:56:57.000000 timeplus-1.3.0b1/timeplus/sqlalchemy.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4886 2023-06-22 17:15:02.000000 timeplus-1.3.0b1/timeplus/stream.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      527 2022-12-28 18:52:21.000000 timeplus-1.3.0b1/timeplus/type.py
+-rw-r--r--   0 gangtao    (502) staff       (20)       39 2023-06-23 23:57:09.000000 timeplus-1.3.0b1/timeplus/version.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     2613 2023-06-22 17:15:02.000000 timeplus-1.3.0b1/timeplus/view.py
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-23 23:57:17.834486 timeplus-1.3.0b1/timeplus.egg-info/
+-rw-r--r--   0 gangtao    (502) staff       (20)     4899 2023-06-23 23:57:17.000000 timeplus-1.3.0b1/timeplus.egg-info/PKG-INFO
+-rw-r--r--   0 gangtao    (502) staff       (20)     6596 2023-06-23 23:57:17.000000 timeplus-1.3.0b1/timeplus.egg-info/SOURCES.txt
+-rw-r--r--   0 gangtao    (502) staff       (20)        1 2023-06-23 23:57:17.000000 timeplus-1.3.0b1/timeplus.egg-info/dependency_links.txt
+-rw-r--r--   0 gangtao    (502) staff       (20)      101 2023-06-23 23:57:17.000000 timeplus-1.3.0b1/timeplus.egg-info/requires.txt
+-rw-r--r--   0 gangtao    (502) staff       (20)       37 2023-06-23 23:57:17.000000 timeplus-1.3.0b1/timeplus.egg-info/top_level.txt
```

### Comparing `timeplus-1.3.0b0/PKG-INFO` & `timeplus-1.3.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeplus
-Version: 1.3.0b0
+Version: 1.3.0b1
 Summary: Timeplus python SDK
 Home-page: https://github.com/timeplus-io/gluon/tree/develop/python
 Author: Gang Tao
 Author-email: gang@timeplus.io
 Project-URL: Bug Tracker, https://github.com/timeplus-io/gluon/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `timeplus-1.3.0b0/README.md` & `timeplus-1.3.0b1/README.md`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/setup.cfg` & `timeplus-1.3.0b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/setup.py` & `timeplus-1.3.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/__init__.py` & `timeplus-1.3.0b1/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/api_client.py` & `timeplus-1.3.0b1/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/configuration.py` & `timeplus-1.3.0b1/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/__init__.py` & `timeplus-1.3.0b1/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/analyze_sql_request.py` & `timeplus-1.3.0b1/swagger_client/models/analyze_sql_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/api_key.py` & `timeplus-1.3.0b1/swagger_client/models/api_key.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/batching_policy.py` & `timeplus-1.3.0b1/swagger_client/models/batching_policy.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/column.py` & `timeplus-1.3.0b1/swagger_client/models/column.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/column_def.py` & `timeplus-1.3.0b1/swagger_client/models/column_def.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/columns_resp.py` & `timeplus-1.3.0b1/swagger_client/models/columns_resp.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/create_api_key_request.py` & `timeplus-1.3.0b1/swagger_client/models/create_api_key_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/create_api_key_response.py` & `timeplus-1.3.0b1/swagger_client/models/create_api_key_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/create_dashboard_request.py` & `timeplus-1.3.0b1/swagger_client/models/create_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/create_query_request_v1_beta2.py` & `timeplus-1.3.0b1/swagger_client/models/create_query_request_v1_beta2.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/create_sink_request.py` & `timeplus-1.3.0b1/swagger_client/models/create_sink_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/create_source_request.py` & `timeplus-1.3.0b1/swagger_client/models/create_source_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/create_view_request.py` & `timeplus-1.3.0b1/swagger_client/models/create_view_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/dashboard_dashboard.py` & `timeplus-1.3.0b1/swagger_client/models/dashboard_dashboard.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/dashboard_panel.py` & `timeplus-1.3.0b1/swagger_client/models/dashboard_panel.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/edge.py` & `timeplus-1.3.0b1/swagger_client/models/edge.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/error_response.py` & `timeplus-1.3.0b1/swagger_client/models/error_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/event.py` & `timeplus-1.3.0b1/swagger_client/models/event.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/event_infer_request.py` & `timeplus-1.3.0b1/swagger_client/models/event_infer_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/event_infer_response.py` & `timeplus-1.3.0b1/swagger_client/models/event_infer_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/external_stream_def.py` & `timeplus-1.3.0b1/swagger_client/models/external_stream_def.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/file_upload_response.py` & `timeplus-1.3.0b1/swagger_client/models/file_upload_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/format_query_request.py` & `timeplus-1.3.0b1/swagger_client/models/format_query_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/format_query_response.py` & `timeplus-1.3.0b1/swagger_client/models/format_query_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/global_metrics_result.py` & `timeplus-1.3.0b1/swagger_client/models/global_metrics_result.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/graph.py` & `timeplus-1.3.0b1/swagger_client/models/graph.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/ingest_data.py` & `timeplus-1.3.0b1/swagger_client/models/ingest_data.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/metrics_query_throughput.py` & `timeplus-1.3.0b1/swagger_client/models/metrics_query_throughput.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/node.py` & `timeplus-1.3.0b1/swagger_client/models/node.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/owner.py` & `timeplus-1.3.0b1/swagger_client/models/owner.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/query.py` & `timeplus-1.3.0b1/swagger_client/models/query.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/query_pipeline.py` & `timeplus-1.3.0b1/swagger_client/models/query_pipeline.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/query_pipeline_edge.py` & `timeplus-1.3.0b1/swagger_client/models/query_pipeline_edge.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/query_pipeline_node.py` & `timeplus-1.3.0b1/swagger_client/models/query_pipeline_node.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/query_pipeline_node_metric.py` & `timeplus-1.3.0b1/swagger_client/models/query_pipeline_node_metric.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/query_result.py` & `timeplus-1.3.0b1/swagger_client/models/query_result.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/resource_metrics_result.py` & `timeplus-1.3.0b1/swagger_client/models/resource_metrics_result.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/sink.py` & `timeplus-1.3.0b1/swagger_client/models/sink.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/sink_stat.py` & `timeplus-1.3.0b1/swagger_client/models/sink_stat.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/source.py` & `timeplus-1.3.0b1/swagger_client/models/source.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/source_preview_request.py` & `timeplus-1.3.0b1/swagger_client/models/source_preview_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/source_upload_body.py` & `timeplus-1.3.0b1/swagger_client/models/source_upload_body.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/sql_analyze_column.py` & `timeplus-1.3.0b1/swagger_client/models/sql_analyze_column.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/sql_analyze_result.py` & `timeplus-1.3.0b1/swagger_client/models/sql_analyze_result.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/stream.py` & `timeplus-1.3.0b1/swagger_client/models/stream.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/stream_def.py` & `timeplus-1.3.0b1/swagger_client/models/stream_def.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/stream_match_request.py` & `timeplus-1.3.0b1/swagger_client/models/stream_match_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/stream_setting.py` & `timeplus-1.3.0b1/swagger_client/models/stream_setting.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/stream_stats.py` & `timeplus-1.3.0b1/swagger_client/models/stream_stats.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/time_columns.py` & `timeplus-1.3.0b1/swagger_client/models/time_columns.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/udf.py` & `timeplus-1.3.0b1/swagger_client/models/udf.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/udf_argument.py` & `timeplus-1.3.0b1/swagger_client/models/udf_argument.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/udf_auth_context.py` & `timeplus-1.3.0b1/swagger_client/models/udf_auth_context.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/update_dashboard_request.py` & `timeplus-1.3.0b1/swagger_client/models/update_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/update_source_request.py` & `timeplus-1.3.0b1/swagger_client/models/update_source_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/update_stream_request.py` & `timeplus-1.3.0b1/swagger_client/models/update_stream_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/update_view_request.py` & `timeplus-1.3.0b1/swagger_client/models/update_view_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/models/view.py` & `timeplus-1.3.0b1/swagger_client/models/view.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/rest.py` & `timeplus-1.3.0b1/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/timeplus/__init__.py` & `timeplus-1.3.0b1/swagger_client/timeplus/__init__.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/timeplus/alerts_internal_api.py` & `timeplus-1.3.0b1/swagger_client/timeplus/alerts_internal_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/timeplus/alerts_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_client/timeplus/alerts_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/timeplus/api_keys_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_client/timeplus/api_keys_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/timeplus/dashboards_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_client/timeplus/dashboards_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/timeplus/metrics_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_client/timeplus/metrics_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/timeplus/queries_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_client/timeplus/queries_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/timeplus/sinks_internal_api.py` & `timeplus-1.3.0b1/swagger_client/timeplus/sinks_internal_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/timeplus/sinks_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_client/timeplus/sinks_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/timeplus/sources_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_client/timeplus/sources_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/timeplus/streams_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_client/timeplus/streams_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/timeplus/topology_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_client/timeplus/topology_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/timeplus/udfs_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_client/timeplus/udfs_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_client/timeplus/views_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_client/timeplus/views_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_alerts_internal_api.py` & `timeplus-1.3.0b1/swagger_test/test_alerts_internal_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_alerts_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_test/test_alerts_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_analyze_sql_request.py` & `timeplus-1.3.0b1/swagger_test/test_analyze_sql_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_api_key.py` & `timeplus-1.3.0b1/swagger_test/test_api_key.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_api_keys_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_test/test_api_keys_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_batching_policy.py` & `timeplus-1.3.0b1/swagger_test/test_batching_policy.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_column.py` & `timeplus-1.3.0b1/swagger_test/test_column.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_column_def.py` & `timeplus-1.3.0b1/swagger_test/test_column_def.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_columns_resp.py` & `timeplus-1.3.0b1/swagger_test/test_columns_resp.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_create_api_key_request.py` & `timeplus-1.3.0b1/swagger_test/test_create_api_key_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_create_api_key_response.py` & `timeplus-1.3.0b1/swagger_test/test_create_api_key_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_create_dashboard_request.py` & `timeplus-1.3.0b1/swagger_test/test_create_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_create_query_request_v1_beta2.py` & `timeplus-1.3.0b1/swagger_test/test_create_query_request_v1_beta2.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_create_sink_request.py` & `timeplus-1.3.0b1/swagger_test/test_create_sink_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_create_source_request.py` & `timeplus-1.3.0b1/swagger_test/test_create_source_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_create_view_request.py` & `timeplus-1.3.0b1/swagger_test/test_create_view_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_dashboard_dashboard.py` & `timeplus-1.3.0b1/swagger_test/test_dashboard_dashboard.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_dashboard_panel.py` & `timeplus-1.3.0b1/swagger_test/test_dashboard_panel.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_dashboards_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_test/test_dashboards_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_edge.py` & `timeplus-1.3.0b1/swagger_test/test_edge.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_error_response.py` & `timeplus-1.3.0b1/swagger_test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_event.py` & `timeplus-1.3.0b1/swagger_test/test_event.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_event_infer_request.py` & `timeplus-1.3.0b1/swagger_test/test_event_infer_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_event_infer_response.py` & `timeplus-1.3.0b1/swagger_test/test_event_infer_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_external_stream_def.py` & `timeplus-1.3.0b1/swagger_test/test_external_stream_def.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_file_upload_response.py` & `timeplus-1.3.0b1/swagger_test/test_file_upload_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_format_query_request.py` & `timeplus-1.3.0b1/swagger_test/test_format_query_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_format_query_response.py` & `timeplus-1.3.0b1/swagger_test/test_format_query_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_global_metrics_result.py` & `timeplus-1.3.0b1/swagger_test/test_global_metrics_result.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_graph.py` & `timeplus-1.3.0b1/swagger_test/test_graph.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_ingest_data.py` & `timeplus-1.3.0b1/swagger_test/test_ingest_data.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_metrics_query_throughput.py` & `timeplus-1.3.0b1/swagger_test/test_metrics_query_throughput.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_metrics_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_test/test_metrics_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_node.py` & `timeplus-1.3.0b1/swagger_test/test_node.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_owner.py` & `timeplus-1.3.0b1/swagger_test/test_owner.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_queries_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_test/test_queries_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_query.py` & `timeplus-1.3.0b1/swagger_test/test_query.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_query_pipeline.py` & `timeplus-1.3.0b1/swagger_test/test_query_pipeline.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_query_pipeline_edge.py` & `timeplus-1.3.0b1/swagger_test/test_query_pipeline_edge.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_query_pipeline_node.py` & `timeplus-1.3.0b1/swagger_test/test_query_pipeline_node.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_query_pipeline_node_metric.py` & `timeplus-1.3.0b1/swagger_test/test_query_pipeline_node_metric.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_query_result.py` & `timeplus-1.3.0b1/swagger_test/test_query_result.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_resource_metrics_result.py` & `timeplus-1.3.0b1/swagger_test/test_resource_metrics_result.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_sink.py` & `timeplus-1.3.0b1/swagger_test/test_sink.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_sink_stat.py` & `timeplus-1.3.0b1/swagger_test/test_sink_stat.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_sinks_internal_api.py` & `timeplus-1.3.0b1/swagger_test/test_sinks_internal_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_sinks_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_test/test_sinks_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_source.py` & `timeplus-1.3.0b1/swagger_test/test_source.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_source_preview_request.py` & `timeplus-1.3.0b1/swagger_test/test_source_preview_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_source_upload_body.py` & `timeplus-1.3.0b1/swagger_test/test_source_upload_body.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_sources_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_test/test_sources_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_sql_analyze_column.py` & `timeplus-1.3.0b1/swagger_test/test_sql_analyze_column.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_sql_analyze_result.py` & `timeplus-1.3.0b1/swagger_test/test_sql_analyze_result.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_stream.py` & `timeplus-1.3.0b1/swagger_test/test_stream.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_stream_def.py` & `timeplus-1.3.0b1/swagger_test/test_stream_def.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_stream_match_request.py` & `timeplus-1.3.0b1/swagger_test/test_stream_match_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_stream_setting.py` & `timeplus-1.3.0b1/swagger_test/test_stream_setting.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_stream_stats.py` & `timeplus-1.3.0b1/swagger_test/test_stream_stats.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_streams_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_test/test_streams_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_time_columns.py` & `timeplus-1.3.0b1/swagger_test/test_time_columns.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_topology_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_test/test_topology_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_udf.py` & `timeplus-1.3.0b1/swagger_test/test_udf.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_udf_argument.py` & `timeplus-1.3.0b1/swagger_test/test_udf_argument.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_udf_auth_context.py` & `timeplus-1.3.0b1/swagger_test/test_udf_auth_context.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_udfs_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_test/test_udfs_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_update_dashboard_request.py` & `timeplus-1.3.0b1/swagger_test/test_update_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_update_source_request.py` & `timeplus-1.3.0b1/swagger_test/test_update_source_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_update_stream_request.py` & `timeplus-1.3.0b1/swagger_test/test_update_stream_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_update_view_request.py` & `timeplus-1.3.0b1/swagger_test/test_update_view_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_view.py` & `timeplus-1.3.0b1/swagger_test/test_view.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/swagger_test/test_views_v1beta2_api.py` & `timeplus-1.3.0b1/swagger_test/test_views_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/test/test_stream.py` & `timeplus-1.3.0b1/test/test_stream.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/timeplus/__init__.py` & `timeplus-1.3.0b1/timeplus/__init__.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/timeplus/dbapi.py` & `timeplus-1.3.0b1/timeplus/dbapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import re
 import itertools
 from collections import namedtuple
 
 from timeplus import Environment, Query, Stream, View
 from timeplus.error import Error
 
 
@@ -245,15 +246,15 @@
                 False,  # [null_ok]
             )
             for field in self.header
         ]
         return
 
     def _stream_query_iter(self):
-        field_names = [field["name"] for field in self.header]
+        field_names = [re.sub(r'[^a-zA-Z0-9]', '', field["name"]) for field in self.header]
         keys = " ".join(field_names)
         for event in self.query.result():
             if event.event == "message":
                 data = json.loads(event.data)
                 for row in data:
                     Row = namedtuple(
                         "Row", keys, rename=True
```

### Comparing `timeplus-1.3.0b0/timeplus/env.py` & `timeplus-1.3.0b1/timeplus/env.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/timeplus/error.py` & `timeplus-1.3.0b1/timeplus/error.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/timeplus/query.py` & `timeplus-1.3.0b1/timeplus/query.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/timeplus/sqlalchemy.py` & `timeplus-1.3.0b1/timeplus/sqlalchemy.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,59 +2,58 @@
 from sqlalchemy import types, util
 from sqlalchemy.sql import compiler
 from timeplus.error import Error
 
 
 # TODO : need a better type mapping here
 type_map = {
-    "uint32": types.BigInteger,
-    "int32": types.BigInteger,
-    "int64": types.BigInteger,
+    "uint": types.BigInteger,
     "int": types.BigInteger,
-    "float32": types.Float,
-    "float64": types.Float,
     "float": types.Float,
-    "decimal(10, 2)": types.Float,
+    "decimal": types.Float,
     "string": types.String,
     "bool": types.Boolean,
-    "datetime64(3)": types.DateTime,
-    "datetime64(3, 'UTC')": types.DateTime,
     "datetime": types.DateTime,
+    "uuid": types.String,
 }
 
 
 class TimeplusSQLCompiler(compiler.SQLCompiler):
     pass
 
 
 class TimeplusTypeCompiler(compiler.GenericTypeCompiler):
     def visit_REAL(self, type_, **kwargs):
         return "float"
 
     def visit_NUMERIC(self, type_, **kwargs):
         return "integer"
 
-    visit_DECIMAL = visit_NUMERIC
+    visit_DECIMAL = visit_REAL
     visit_INTEGER = visit_NUMERIC
     visit_SMALLINT = visit_NUMERIC
     visit_BIGINT = visit_NUMERIC
-    visit_BOOLEAN = visit_NUMERIC
     visit_TIMESTAMP = visit_NUMERIC
-    visit_DATE = visit_NUMERIC
+
+    def visit_BOOLEAN(self, type_, **kwargs):
+        return "bool"
 
     def visit_CHAR(self, type_, **kwargs):
         return "string"
 
     visit_NCHAR = visit_CHAR
     visit_VARCHAR = visit_CHAR
     visit_NVARCHAR = visit_CHAR
     visit_TEXT = visit_CHAR
 
+    def visit_DATE(self, type_, **kwargs):
+        return "date"
+
     def visit_DATETIME(self, type_, **kwargs):
-        return "datetime64"
+        return "datetime"
 
     def visit_BLOB(self, type_, **kwargs):
         return "string"
 
     visit_CLOB = visit_BLOB
     visit_NCLOB = visit_BLOB
     visit_VARBINARY = visit_BLOB
@@ -235,14 +234,15 @@
     def get_view_definition(self, connection, view_name, schema=None, **kwargs):
         pass
 
     def do_rollback(self, dbapi_connection):
         pass
 
     def _map_type(self, col):
-        if col.type in type_map:
-            return type_map[col.type]
+        for key in type_map.keys():
+            if col.type.startswith(key):
+                return type_map[key]
         util.warn(
             "Failed to map column {col.name} with raw type {col.type}".format(
                 col=col)
         )
-        return types.NullType
+        return types.String
```

### Comparing `timeplus-1.3.0b0/timeplus/stream.py` & `timeplus-1.3.0b1/timeplus/stream.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/timeplus/type.py` & `timeplus-1.3.0b1/timeplus/type.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/timeplus/view.py` & `timeplus-1.3.0b1/timeplus/view.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.3.0b0/timeplus.egg-info/PKG-INFO` & `timeplus-1.3.0b1/timeplus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeplus
-Version: 1.3.0b0
+Version: 1.3.0b1
 Summary: Timeplus python SDK
 Home-page: https://github.com/timeplus-io/gluon/tree/develop/python
 Author: Gang Tao
 Author-email: gang@timeplus.io
 Project-URL: Bug Tracker, https://github.com/timeplus-io/gluon/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `timeplus-1.3.0b0/timeplus.egg-info/SOURCES.txt` & `timeplus-1.3.0b1/timeplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

