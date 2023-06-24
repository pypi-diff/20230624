# Comparing `tmp/fedml-0.8.4a9.tar.gz` & `tmp/fedml-0.8.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fedml-0.8.4a9.tar", last modified: Sun Apr 30 05:33:28 2023, max compression
+gzip compressed data, was "dist/fedml-0.8.5a1.tar", last modified: Sat Jun 24 12:02:55 2023, max compression
```

## Comparing `fedml-0.8.4a9.tar` & `fedml-0.8.5a1.tar`

### file list

```diff
@@ -1,1164 +1,1187 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/
--rw-r--r--   0 runner     (501) staff       (20)     3806 2023-04-30 05:33:28.000000 fedml-0.8.4a9/PKG-INFO
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/tests/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/tests/security/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/tests/security/attack/
--rw-r--r--   0 runner     (501) staff       (20)     1218 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/attack/test_label_flipping_attack.py
--rw-r--r--   0 runner     (501) staff       (20)      730 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/attack/test_backdoor.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/attack/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1159 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/attack/test_model_replacement_backdoor_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     5147 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/attack/test_invertgradient.py
--rw-r--r--   0 runner     (501) staff       (20)     1586 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/attack/test_byzantine_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     5519 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/attack/utils.py
--rw-r--r--   0 runner     (501) staff       (20)      955 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/attack/test_edge_case_backdoor_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     1466 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/attack/test_dlg.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/tests/security/defense/
--rw-r--r--   0 runner     (501) staff       (20)      376 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/defense/test_rfa.py
--rw-r--r--   0 runner     (501) staff       (20)     1942 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/defense/test_residual_based_reweighting.py
--rw-r--r--   0 runner     (501) staff       (20)     1139 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/defense/test_wbc.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/defense/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1099 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/defense/test_crfl.py
--rw-r--r--   0 runner     (501) staff       (20)     1871 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/defense/test_geometric_median.py
--rw-r--r--   0 runner     (501) staff       (20)     2682 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/defense/test_slsgd_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     1327 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/defense/test_weak_dp.py
--rw-r--r--   0 runner     (501) staff       (20)     1525 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/defense/test_norm_diff_clipping.py
--rw-r--r--   0 runner     (501) staff       (20)     5913 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/defense/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     1555 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/defense/test_bulyan.py
--rw-r--r--   0 runner     (501) staff       (20)      805 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/defense/test_robust_learning_rate_defense.py
--rw-r--r--   0 runner     (501) staff       (20)      999 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/defense/test_coordinate_wise_trimmed_mean.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1206 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/defense/test_krum.py
--rwxr-xr-x   0 runner     (501) staff       (20)      987 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/defense/test_cclip.py
--rw-r--r--   0 runner     (501) staff       (20)      390 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/defense/test_coordinate_median.py
--rw-r--r--   0 runner     (501) staff       (20)      902 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/defense/test_foolsgold_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     2208 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/security/defense/test_soteria.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/tests/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2326 2023-04-30 05:33:15.000000 fedml-0.8.4a9/README.md
--rw-r--r--   0 runner     (501) staff       (20)     4574 2023-04-30 05:33:16.000000 fedml-0.8.4a9/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_attack_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_attack_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_attack_mnist_lr_example/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_attack_mnist_lr_example/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/torch_server.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)     2026 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       89 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)       89 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/torch_server.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/
--rw-r--r--   0 runner     (501) staff       (20)      404 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/main_fedml_cross_silo_hi.py
--rw-r--r--   0 runner     (501) staff       (20)      196 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/mlops_client_launcher.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2003 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2024 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/torch_server.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)     4403 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_trainer_classification.py
--rw-r--r--   0 runner     (501) staff       (20)     5218 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2033 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_server.py
--rw-r--r--   0 runner     (501) staff       (20)     2020 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_client.py
--rw-r--r--   0 runner     (501) staff       (20)     1435 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      757 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      757 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/
--rw-r--r--   0 runner     (501) staff       (20)     1689 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2119 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_trainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      827 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      965 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_mpi.py
--rw-r--r--   0 runner     (501) staff       (20)      827 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)     4098 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_trainer_classification.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1739 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model.py
--rw-r--r--   0 runner     (501) staff       (20)     5323 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1999 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_client.py
--rw-r--r--   0 runner     (501) staff       (20)     2013 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_cdp_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_cdp_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_cdp_mnist_lr_example/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_cdp_mnist_lr_example/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/trpc_fedavg_mnist_lr_example/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/torch_server.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/trpc_fedavg_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2003 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1993 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_client.py
--rw-r--r--   0 runner     (501) staff       (20)     3354 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1387 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_trainer_classification.py
--rw-r--r--   0 runner     (501) staff       (20)     2007 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_server.py
--rw-r--r--   0 runner     (501) staff       (20)      699 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_ldp_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_ldp_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_ldp_mnist_lr_example/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      395 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_ldp_mnist_lr_example/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/mqtt_s3_intersection_and_cardinality_fake_data_example/
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/mqtt_s3_intersection_and_cardinality_fake_data_example/server.py
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/mqtt_s3_intersection_and_cardinality_fake_data_example/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/mqtt_s3_intersection_and_cardinality_fake_data_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/mqtt_s3_k_percentile_fake_data_example/
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/mqtt_s3_k_percentile_fake_data_example/server.py
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/mqtt_s3_k_percentile_fake_data_example/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/mqtt_s3_k_percentile_fake_data_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/mqtt_s3_union_fake_data_example/
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/mqtt_s3_union_fake_data_example/server.py
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/mqtt_s3_union_fake_data_example/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/mqtt_s3_union_fake_data_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/mqtt_s3_frequency_estimation_fake_data_example/
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/mqtt_s3_frequency_estimation_fake_data_example/server.py
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/mqtt_s3_frequency_estimation_fake_data_example/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/mqtt_s3_frequency_estimation_fake_data_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/mqtt_s3_avg_fake_data_example/
--rw-r--r--   0 runner     (501) staff       (20)      391 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/mqtt_s3_avg_fake_data_example/server.py
--rw-r--r--   0 runner     (501) staff       (20)      282 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/mqtt_s3_avg_fake_data_example/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/FA_examples/mqtt_s3_avg_fake_data_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      968 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/torch_client.py
--rw-r--r--   0 runner     (501) staff       (20)      968 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/torch_mpi.py
--rw-r--r--   0 runner     (501) staff       (20)      968 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_hierarchical_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      404 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_hierarchical_mnist_lr_example/main_fedml_cross_silo_hi.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_hierarchical_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_device/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/
--rw-r--r--   0 runner     (501) staff       (20)     1214 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/my_dataset.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      801 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/torch_server.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_device/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/
--rw-r--r--   0 runner     (501) staff       (20)     1170 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/my_dataset.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      809 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/centralized/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/centralized/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    20282 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/centralized/main.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/mpi_fedopt_datasets_and_models_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_fedopt_datasets_and_models_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_fedopt_datasets_and_models_example/torch_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/sp_vertical_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_vertical_mnist_lr_example/torch_vertical_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_vertical_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/sp_fedopt_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_fedopt_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_fedopt_mnist_lr_example/torch_fedopt_mnist_lr_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/mpi_decentralized_fl_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_decentralized_fl_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      222 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_decentralized_fl_example/mpi_decentralized_fl_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/sp_decentralized_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_decentralized_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_decentralized_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedgkt_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedgkt_mnist_lr_example/torch_fedgkt_cifar10_resnet56.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedgkt_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg/
--rw-r--r--   0 runner     (501) staff       (20)     5590 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg/reddit_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     4816 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg/reddit_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6461 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg/main.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/sp_hierarchicalfl_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_hierarchicalfl_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_hierarchicalfl_mnist_lr_example/torch_hierarchicalfl_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedopt_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedopt_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedopt_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedgan_mnist_gan_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedgan_mnist_gan_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedgan_mnist_gan_example/torch_fedgan_mnist_gan_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/mpi_fedavg_datasets_and_models_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_fedavg_datasets_and_models_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_fedavg_datasets_and_models_example/torch_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_seq/
--rw-r--r--   0 runner     (501) staff       (20)      762 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_seq/torch_fedavg.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_seq/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/mpi_fedprox_datasets_and_models_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_fedprox_datasets_and_models_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_fedprox_datasets_and_models_example/torch_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/sp_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)       69 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_one_line_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_fedavg_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      423 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fednas_cifar10_dart_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fednas_cifar10_dart_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fednas_cifar10_dart_example/torch_fednas_cifar10_dart_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
--rw-r--r--   0 runner     (501) staff       (20)       82 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_splitnn_cifar10_resnet56_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_splitnn_cifar10_resnet56_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_splitnn_cifar10_resnet56_example/torch_splitnn_mnist_lr_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/sp_fednova_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_fednova_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_fednova_mnist_lr_example/torch_fednova_mnist_lr_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
--rw-r--r--   0 runner     (501) staff       (20)       82 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
--rw-r--r--   0 runner     (501) staff       (20)       82 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/mpi_base_framework_example/
--rw-r--r--   0 runner     (501) staff       (20)      222 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_base_framework_example/mpi_base_framework_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_base_framework_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/sp_fedavg_mnist_cnn_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_fedavg_mnist_cnn_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_fedavg_mnist_cnn_example/torch_fedavg_mnist_cnn_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
--rw-r--r--   0 runner     (501) staff       (20)       82 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)       82 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_one_line_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)     1990 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedprox_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedprox_mnist_lr_example/torch_fedprox_mnist_lr_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_fedprox_mnist_lr_example/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/sp_turboaggregate_mnist_lr_example/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_turboaggregate_mnist_lr_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_turboaggregate_mnist_lr_example/torch_turboaggregate_mnist_lr_step_by_step_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_async_fedavg/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_async_fedavg/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1042 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/mpi_torch_async_fedavg/torch_fedavg_mnist_lr_custum_data_and_model_example.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/examples/simulation/sp_fedavg_datasets_and_models_example/
--rw-r--r--   0 runner     (501) staff       (20)      422 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_fedavg_datasets_and_models_example/torch_fedavg_step_by_step_example.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/simulation/sp_fedavg_datasets_and_models_example/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/examples/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-04-30 05:33:28.000000 fedml-0.8.4a9/setup.cfg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/
--rw-r--r--   0 runner     (501) staff       (20)     1061 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/launch_serving.py
--rw-r--r--   0 runner     (501) staff       (20)     1078 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/launch_cross_silo_hi.py
--rw-r--r--   0 runner     (501) staff       (20)     6907 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/runner.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cross_silo/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cross_silo/lightsecagg/
--rw-r--r--   0 runner     (501) staff       (20)     3009 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/lightsecagg/lsa_message_define.py
--rw-r--r--   0 runner     (501) staff       (20)    11077 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/lightsecagg/lsa_fedml_client_manager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/lightsecagg/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    13517 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/lightsecagg/lsa_fedml_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)    12846 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/lightsecagg/lsa_fedml_server_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     3467 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/lightsecagg/lsa_fedml_api.py
--rw-r--r--   0 runner     (501) staff       (20)      157 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cross_silo/server/
--rw-r--r--   0 runner     (501) staff       (20)     2212 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/server/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/server/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    15312 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/server/fedml_server_manager.py
--rw-r--r--   0 runner     (501) staff       (20)    11613 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/server/fedml_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1056 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/server/server_initializer.py
--rw-r--r--   0 runner     (501) staff       (20)     1917 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/fedml_client.py
--rw-r--r--   0 runner     (501) staff       (20)     2025 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/fedml_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cross_silo/client/
--rw-r--r--   0 runner     (501) staff       (20)     2266 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/client/client_initializer.py
--rw-r--r--   0 runner     (501) staff       (20)     5161 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/client/client_launcher.py
--rw-r--r--   0 runner     (501) staff       (20)     2673 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/client/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     2680 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/client/fedml_trainer_dist_adapter.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/client/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1655 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/client/fedml_client_slave_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     1258 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/client/process_group_manager.py
--rw-r--r--   0 runner     (501) staff       (20)      677 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/client/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     7549 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/client/fedml_client_master_manager.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3563 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_silo/client/fedml_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     1079 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/launch_cross_silo_horizontal.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/serving/
--rw-r--r--   0 runner     (501) staff       (20)      163 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/serving/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/serving/server/
--rw-r--r--   0 runner     (501) staff       (20)     2212 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/serving/server/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/serving/server/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    15366 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/serving/server/fedml_server_manager.py
--rw-r--r--   0 runner     (501) staff       (20)    11613 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/serving/server/fedml_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1056 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/serving/server/server_initializer.py
--rw-r--r--   0 runner     (501) staff       (20)     1340 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/serving/fedml_client.py
--rw-r--r--   0 runner     (501) staff       (20)     1456 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/serving/fedml_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/serving/client/
--rw-r--r--   0 runner     (501) staff       (20)     2266 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/serving/client/client_initializer.py
--rw-r--r--   0 runner     (501) staff       (20)     5161 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/serving/client/client_launcher.py
--rw-r--r--   0 runner     (501) staff       (20)     2673 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/serving/client/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     2680 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/serving/client/fedml_trainer_dist_adapter.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/serving/client/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1655 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/serving/client/fedml_client_slave_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     1258 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/serving/client/process_group_manager.py
--rw-r--r--   0 runner     (501) staff       (20)      677 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/serving/client/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     7549 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/serving/client/fedml_client_master_manager.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3563 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/serving/client/fedml_trainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/schedule/
--rw-r--r--   0 runner     (501) staff       (20)     5761 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/schedule/runtime_estimate.py
--rw-r--r--   0 runner     (501) staff       (20)     9840 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/schedule/seq_train_scheduler.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/schedule/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/alg_frame/
--rw-r--r--   0 runner     (501) staff       (20)      795 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/alg_frame/params.py
--rw-r--r--   0 runner     (501) staff       (20)     1855 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/alg_frame/client_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/alg_frame/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      894 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/alg_frame/context.py
--rw-r--r--   0 runner     (501) staff       (20)     5737 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/alg_frame/server_aggregator.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/distributed/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/distributed/topology/
--rw-r--r--   0 runner     (501) staff       (20)     5001 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/topology/asymmetric_topology_manager.py
--rw-r--r--   0 runner     (501) staff       (20)      479 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/topology/base_topology_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     3853 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/topology/symmetric_topology_manager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/topology/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/distributed/crypto/
--rw-r--r--   0 runner     (501) staff       (20)     2167 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/crypto/crypto_api.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/crypto/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     8764 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/fedml_comm_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/distributed/communication/
--rw-r--r--   0 runner     (501) staff       (20)      153 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/observer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/distributed/communication/s3/
--rw-r--r--   0 runner     (501) staff       (20)     1680 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/s3/remote_storage_mnn.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/s3/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    21800 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/s3/remote_storage.py
--rw-r--r--   0 runner     (501) staff       (20)     2792 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/s3/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/distributed/communication/mpi/
--rw-r--r--   0 runner     (501) staff       (20)     1648 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/mpi/mpi_send_thread.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/mpi/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4977 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/mpi/com_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     1603 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/mpi/mpi_receive_thread.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/distributed/communication/grpc/
--rw-r--r--   0 runner     (501) staff       (20)     1255 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/grpc/grpc_server.py
--rw-r--r--   0 runner     (501) staff       (20)     6381 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/grpc/grpc_comm_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/distributed/communication/grpc/proto/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/grpc/proto/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/grpc/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4236 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2_grpc.py
--rw-r--r--   0 runner     (501) staff       (20)      346 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/grpc/ip_config_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     6272 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/distributed/communication/trpc/
--rw-r--r--   0 runner     (501) staff       (20)     1614 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/trpc/trpc_server.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/trpc/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4807 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/trpc/trpc_comm_manager.py
--rw-r--r--   0 runner     (501) staff       (20)      437 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/trpc/utils.py
--rw-r--r--   0 runner     (501) staff       (20)      377 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/constants.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2612 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/message.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/distributed/communication/mqtt_web3/
--rwxr-xr-x   0 runner     (501) staff       (20)       91 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/mqtt_web3/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)    14594 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/mqtt_web3/mqtt_web3_comm_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/distributed/communication/mqtt_thetastore/
--rwxr-xr-x   0 runner     (501) staff       (20)      109 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/mqtt_thetastore/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)    14669 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/mqtt_thetastore/mqtt_thetastore_comm_manager.py
--rwxr-xr-x   0 runner     (501) staff       (20)      869 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/utils.py
--rw-r--r--   0 runner     (501) staff       (20)      518 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/base_com_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/distributed/communication/mqtt_s3/
--rwxr-xr-x   0 runner     (501) staff       (20)      123 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/mqtt_s3/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)    15504 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/mqtt_s3/mqtt_s3_multi_clients_comm_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/distributed/communication/mqtt/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/mqtt/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    13754 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/mqtt/mqtt_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/distributed/communication/mqtt_s3_mnn/
--rwxr-xr-x   0 runner     (501) staff       (20)       91 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/mqtt_s3_mnn/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)    12233 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/communication/mqtt_s3_mnn/mqtt_s3_comm_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/distributed/distributed_storage/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/distributed/distributed_storage/web3_storage/
--rw-r--r--   0 runner     (501) staff       (20)     3604 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/distributed_storage/web3_storage/web3_storage.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/distributed_storage/web3_storage/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/distributed/distributed_storage/theta_storage/
--rw-r--r--   0 runner     (501) staff       (20)     6834 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/distributed_storage/theta_storage/theta_storage.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/distributed_storage/theta_storage/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/distributed_storage/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/distributed/flow/
--rw-r--r--   0 runner     (501) staff       (20)    12684 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/flow/fedml_flow.py
--rw-r--r--   0 runner     (501) staff       (20)      728 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/flow/fedml_executor.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/flow/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      338 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/flow/fedml_flow_constants.py
--rw-r--r--   0 runner     (501) staff       (20)     3248 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/distributed/flow/test_fedml_flow.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/security/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/security/attack/
--rw-r--r--   0 runner     (501) staff       (20)     4005 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/attack/model_replacement_backdoor_attack.py
--rw-r--r--   0 runner     (501) staff       (20)      440 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/attack/attack_base.py
--rw-r--r--   0 runner     (501) staff       (20)     3424 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/attack/edge_case_backdoor_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     3607 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/attack/byzantine_attack.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/attack/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6102 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/attack/lazy_worker.py
--rw-r--r--   0 runner     (501) staff       (20)    27345 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/attack/invert_gradient_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     6066 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/attack/dlg_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     4712 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/attack/revealing_labels_from_gradients_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     2551 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/attack/label_flipping_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     5286 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/attack/backdoor_attack.py
--rw-r--r--   0 runner     (501) staff       (20)     3738 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/fedml_attacker.py
--rw-r--r--   0 runner     (501) staff       (20)     1208 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/constants.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     7568 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/fedml_defender.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/security/common/
--rw-r--r--   0 runner     (501) staff       (20)     1973 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/common/bucket.py
--rw-r--r--   0 runner     (501) staff       (20)      734 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/common/net.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/common/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1856 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/common/attack_defense_data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)     7488 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/common/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/security/defense/
--rw-r--r--   0 runner     (501) staff       (20)     8885 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/three_sigma_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     2172 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/norm_diff_clipping_defense.py
--rw-r--r--   0 runner     (501) staff       (20)    10320 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/residual_based_reweighting_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     8375 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/three_sigma_krum_defense.py
--rw-r--r--   0 runner     (501) staff       (20)      994 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/coordinate_wise_trimmed_mean_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     2849 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/slsgd_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     1610 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/coordinate_wise_median_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     3640 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/wbc_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     2675 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/robust_learning_rate_defense.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1071 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/RFA_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     1682 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/defense_base.py
--rw-r--r--   0 runner     (501) staff       (20)     3568 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/foolsgold_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     3709 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/soteria_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     5462 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/bulyan_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     4636 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/cross_round_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     6525 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/three_sigma_geomedian_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     1988 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/geometric_median_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     3054 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/crfl_defense.py
--rw-r--r--   0 runner     (501) staff       (20)     1173 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/outlier_detection.py
--rw-r--r--   0 runner     (501) staff       (20)     1008 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/weak_dp_defense.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2650 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/cclip_defense.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2564 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/security/defense/krum_defense.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/mlops/
--rw-r--r--   0 runner     (501) staff       (20)     8983 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/mlops/mlops_configs.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/mlops/ssl/
--rw-r--r--   0 runner     (501) staff       (20)     4089 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/mlops/ssl/open-dev.fedml.ai_bundle.crt
--rw-r--r--   0 runner     (501) staff       (20)     4085 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/mlops/ssl/open-release.fedml.ai_bundle.crt
--rw-r--r--   0 runner     (501) staff       (20)     1947 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/mlops/ssl/open-root-ca.crt
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/mlops/ssl/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4093 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/mlops/ssl/open-test.fedml.ai_bundle.crt
--rw-r--r--   0 runner     (501) staff       (20)    21213 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/mlops/mlops_metrics.py
--rw-r--r--   0 runner     (501) staff       (20)     4891 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/mlops/mlops_profiler_event.py
--rw-r--r--   0 runner     (501) staff       (20)     1377 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/mlops/mlops_status.py
--rw-r--r--   0 runner     (501) staff       (20)    33177 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/mlops/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    11124 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/mlops/stats_impl.py
--rw-r--r--   0 runner     (501) staff       (20)     1410 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/mlops/mlops_utils.py
--rw-r--r--   0 runner     (501) staff       (20)    17257 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/mlops/mlops_runtime_log_daemon.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3906 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/mlops/system_stats.py
--rw-r--r--   0 runner     (501) staff       (20)     8097 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/mlops/mlops_runtime_log.py
--rw-r--r--   0 runner     (501) staff       (20)     1117 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/common/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/common/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      298 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/common/ml_engine_backend.py
--rw-r--r--   0 runner     (501) staff       (20)      231 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/common/singleton.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/mpc/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/mpc/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6017 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/mpc/lightsecagg.py
--rw-r--r--   0 runner     (501) staff       (20)    12340 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/mpc/secagg.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/dp/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/dp/mechanisms/
--rw-r--r--   0 runner     (501) staff       (20)     1443 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/dp/mechanisms/dp_mechanism.py
--rw-r--r--   0 runner     (501) staff       (20)      659 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/dp/mechanisms/laplace.py
--rw-r--r--   0 runner     (501) staff       (20)       83 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/dp/mechanisms/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      177 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/dp/mechanisms/base_dp_mechanism.py
--rw-r--r--   0 runner     (501) staff       (20)     1037 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/dp/mechanisms/gaussian.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/dp/test/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/dp/test/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2532 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/dp/test/test_fed_privacy_mechanism.py
--rw-r--r--   0 runner     (501) staff       (20)     4178 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/dp/fedml_differential_privacy.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/dp/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/dp/frames/
--rw-r--r--   0 runner     (501) staff       (20)     3293 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/dp/frames/NbAFL.py
--rw-r--r--   0 runner     (501) staff       (20)     2444 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/dp/frames/dp_clip.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/dp/frames/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1101 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/dp/frames/cdp.py
--rw-r--r--   0 runner     (501) staff       (20)      470 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/dp/frames/ldp.py
--rw-r--r--   0 runner     (501) staff       (20)     2118 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/dp/frames/base_dp_solution.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/dp/budget_accountant/
--rw-r--r--   0 runner     (501) staff       (20)     6747 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/dp/budget_accountant/rdp_analysis.py
--rw-r--r--   0 runner     (501) staff       (20)     1141 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/dp/budget_accountant/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6915 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/dp/budget_accountant/rdp_accountant.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/dp/common/
--rw-r--r--   0 runner     (501) staff       (20)       69 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/dp/common/constants.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/dp/common/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2411 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/dp/common/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/contribution/
--rw-r--r--   0 runner     (501) staff       (20)     5603 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/contribution/gtg_shapley_value.py
--rw-r--r--   0 runner     (501) staff       (20)     3197 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/contribution/mr_shapley_value.py
--rw-r--r--   0 runner     (501) staff       (20)     1665 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/contribution/base_contribution_assessor.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/contribution/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4930 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/contribution/leave_one_out.py
--rw-r--r--   0 runner     (501) staff       (20)     1922 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/contribution/contribution_assessor_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/core/data/
--rw-r--r--   0 runner     (501) staff       (20)      158 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/data/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4937 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/core/data/noniid_partition.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/distributed/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/distributed/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/config/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/config/simulaton_mpi/
--rw-r--r--   0 runner     (501) staff       (20)      964 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/config/simulaton_mpi/fedml_config.yaml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/config/simulation_sp/
--rw-r--r--   0 runner     (501) staff       (20)     1091 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/config/simulation_sp/fedml_config.yaml
--rwxr-xr-x   0 runner     (501) staff       (20)     8022 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/arguments.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/mlops/
--rw-r--r--   0 runner     (501) staff       (20)     2354 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/mlops/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1037 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/launch_cheeath.py
--rw-r--r--   0 runner     (501) staff       (20)     2198 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/constants.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cross_device/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cross_device/server_mnn/
--rw-r--r--   0 runner     (501) staff       (20)     2190 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_device/server_mnn/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_device/server_mnn/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    18567 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_device/server_mnn/fedml_server_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     2772 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_device/server_mnn/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     7827 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_device/server_mnn/fedml_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1264 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_device/server_mnn/server_mnn_api.py
--rw-r--r--   0 runner     (501) staff       (20)       66 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_device/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      579 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cross_device/mnn_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/centralized/
--rw-r--r--   0 runner     (501) staff       (20)     6588 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/centralized/centralized_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/centralized/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      685 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/launch_simulation.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/sp/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/sp/fedavg/
--rw-r--r--   0 runner     (501) staff       (20)     1401 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/fedavg/client.py
--rw-r--r--   0 runner     (501) staff       (20)       34 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/fedavg/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    12457 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/fedavg/fedavg_api.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/sp/fedprox/
--rw-r--r--   0 runner     (501) staff       (20)     1401 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/fedprox/client.py
--rw-r--r--   0 runner     (501) staff       (20)       44 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/fedprox/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    11535 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/fedprox/fedprox_trainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/sp/turboaggregate/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/turboaggregate/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     7850 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/turboaggregate/TA_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     7880 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/turboaggregate/mpc_function.py
--rw-r--r--   0 runner     (501) staff       (20)      818 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/turboaggregate/TA_client.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/sp/feddyn/
--rw-r--r--   0 runner     (501) staff       (20)     1916 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/feddyn/client copy.py
--rw-r--r--   0 runner     (501) staff       (20)     1941 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/feddyn/client.py
--rw-r--r--   0 runner     (501) staff       (20)       42 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/feddyn/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    16395 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/feddyn/feddyn_trainer copy.py
--rw-r--r--   0 runner     (501) staff       (20)    15943 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/feddyn/feddyn_trainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/sp/classical_vertical_fl/
--rw-r--r--   0 runner     (501) staff       (20)     1355 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/classical_vertical_fl/client.py
--rw-r--r--   0 runner     (501) staff       (20)     3625 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/classical_vertical_fl/party_models.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/classical_vertical_fl/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2241 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/classical_vertical_fl/vfl.py
--rw-r--r--   0 runner     (501) staff       (20)    10964 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/classical_vertical_fl/vfl_api.py
--rw-r--r--   0 runner     (501) staff       (20)     3887 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/classical_vertical_fl/vfl_fixture.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/sp/fednova/
--rw-r--r--   0 runner     (501) staff       (20)     8207 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/fednova/fednova.py
--rw-r--r--   0 runner     (501) staff       (20)    12457 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/fednova/fednova_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)    10932 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/fednova/fednova_api.py
--rw-r--r--   0 runner     (501) staff       (20)     6496 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/fednova/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/fednova/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2258 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/fednova/comm_helpers.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/sp/fedopt/
--rw-r--r--   0 runner     (501) staff       (20)    12255 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/fedopt/fedopt_api.py
--rw-r--r--   0 runner     (501) staff       (20)     1456 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/fedopt/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/fedopt/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1830 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/fedopt/optrepo.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/sp/hierarchical_fl/
--rw-r--r--   0 runner     (501) staff       (20)     2133 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/hierarchical_fl/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/hierarchical_fl/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2391 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/hierarchical_fl/group.py
--rw-r--r--   0 runner     (501) staff       (20)     4644 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/hierarchical_fl/trainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/sp/mime/
--rw-r--r--   0 runner     (501) staff       (20)     1494 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/mime/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/mime/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3192 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/mime/opt_utils.py
--rw-r--r--   0 runner     (501) staff       (20)    13370 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/mime/mime_trainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/sp/scaffold/
--rw-r--r--   0 runner     (501) staff       (20)    13084 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/scaffold/scaffold_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     2677 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/scaffold/client.py
--rw-r--r--   0 runner     (501) staff       (20)       46 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/scaffold/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/sp/decentralized/
--rw-r--r--   0 runner     (501) staff       (20)     4187 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/decentralized/decentralized_fl_api.py
--rw-r--r--   0 runner     (501) staff       (20)     4328 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/decentralized/client_dsgd.py
--rw-r--r--   0 runner     (501) staff       (20)     5514 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/decentralized/client_pushsum.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/decentralized/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5741 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/sp/decentralized/topology_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/mpi/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedavg/
--rw-r--r--   0 runner     (501) staff       (20)     2689 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedavg/FedAvgClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)      852 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedavg/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedavg/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6818 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedavg/FedAVGAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     3602 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedavg/FedAvgAPI.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedavg/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2542 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedavg/FedAVGTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     4462 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedavg/FedAvgServerManager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/mpi/split_nn/
--rw-r--r--   0 runner     (501) staff       (20)     2589 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/split_nn/server.py
--rw-r--r--   0 runner     (501) staff       (20)     2338 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/split_nn/SplitNNAPI.py
--rw-r--r--   0 runner     (501) staff       (20)      591 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/split_nn/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     1733 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/split_nn/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/split_nn/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3996 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/split_nn/client_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     2043 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/split_nn/server_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedprox/
--rw-r--r--   0 runner     (501) staff       (20)      852 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedprox/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     2438 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedprox/FedProxTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedprox/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2804 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedprox/FedProxClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)     7365 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedprox/FedProxAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedprox/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     4607 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedprox/FedProxServerManager.py
--rw-r--r--   0 runner     (501) staff       (20)     3460 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedprox/FedProxAPI.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedgan/
--rw-r--r--   0 runner     (501) staff       (20)     4494 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedgan/FedGanServerManager.py
--rw-r--r--   0 runner     (501) staff       (20)     3809 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedgan/FedGanAPI.py
--rw-r--r--   0 runner     (501) staff       (20)      852 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedgan/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedgan/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3633 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedgan/gan_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)      880 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedgan/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2218 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedgan/FedGANTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     7774 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedgan/FedGANAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     2625 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedgan/FedGanClientManager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedgkt/
--rw-r--r--   0 runner     (501) staff       (20)    15801 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedgkt/GKTServerTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     2120 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedgkt/FedGKTAPI.py
--rw-r--r--   0 runner     (501) staff       (20)     3165 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedgkt/GKTServerManager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedgkt/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4940 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedgkt/utils.py
--rw-r--r--   0 runner     (501) staff       (20)      671 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedgkt/message_def.py
--rw-r--r--   0 runner     (501) staff       (20)     2925 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedgkt/GKTClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)     6492 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedgkt/GKTClientTrainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/mpi/base_framework/
--rw-r--r--   0 runner     (501) staff       (20)      428 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/base_framework/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/base_framework/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1858 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/base_framework/client_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     1123 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/base_framework/central_worker.py
--rw-r--r--   0 runner     (501) staff       (20)     1147 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/base_framework/algorithm_api.py
--rw-r--r--   0 runner     (501) staff       (20)      438 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/base_framework/client_worker.py
--rw-r--r--   0 runner     (501) staff       (20)     2266 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/base_framework/central_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/
--rw-r--r--   0 runner     (501) staff       (20)     1015 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     3409 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/MyModelTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4903 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/AsyncFedAvgServerManager.py
--rw-r--r--   0 runner     (501) staff       (20)     3324 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/my_model_trainer_nwp.py
--rw-r--r--   0 runner     (501) staff       (20)     3531 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/AsyncFedAvgClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2222 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/AsyncFedAVGTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     3863 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/AsyncFedAvgSeqAPI.py
--rw-r--r--   0 runner     (501) staff       (20)     7993 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/AsyncFedAVGAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     4779 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/my_model_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     4164 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/my_model_trainer_tag_prediction.py
--rw-r--r--   0 runner     (501) staff       (20)     3274 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/my_model_trainer_classification.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedavg_seq/
--rw-r--r--   0 runner     (501) staff       (20)     5488 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedavg_seq/FedAvgClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)     1015 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedavg_seq/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedavg_seq/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3489 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedavg_seq/FedAvgSeqAPI.py
--rw-r--r--   0 runner     (501) staff       (20)    13844 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedavg_seq/FedAVGAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedavg_seq/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     3079 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedavg_seq/FedAVGTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     5954 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedavg_seq/FedAvgServerManager.py
--rw-r--r--   0 runner     (501) staff       (20)     3284 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedavg_seq/my_model_trainer_classification.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/mpi/decentralized_framework/
--rw-r--r--   0 runner     (501) staff       (20)      386 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/decentralized_framework/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/decentralized_framework/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1112 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/decentralized_framework/decentralized_worker.py
--rw-r--r--   0 runner     (501) staff       (20)     2374 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/decentralized_framework/decentralized_worker_manager.py
--rw-r--r--   0 runner     (501) staff       (20)      738 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/decentralized_framework/algorithm_api.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/mpi/classical_vertical_fl/
--rw-r--r--   0 runner     (501) staff       (20)      504 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/classical_vertical_fl/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     7074 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/classical_vertical_fl/guest_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/classical_vertical_fl/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2198 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/classical_vertical_fl/guest_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     1801 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/classical_vertical_fl/vfl_api.py
--rw-r--r--   0 runner     (501) staff       (20)     3470 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/classical_vertical_fl/host_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     1842 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/classical_vertical_fl/host_manager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/mpi/fednas/
--rw-r--r--   0 runner     (501) staff       (20)    11022 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fednas/FedNASAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     3767 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fednas/FedNASClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)     2295 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fednas/FedNASAPI.py
--rw-r--r--   0 runner     (501) staff       (20)    10792 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fednas/FedNASTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)      693 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fednas/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fednas/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4146 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fednas/FedNASServerManager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/mpi/fednova/
--rw-r--r--   0 runner     (501) staff       (20)     3490 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fednova/FedNovaAPI.py
--rw-r--r--   0 runner     (501) staff       (20)     1015 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fednova/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     5687 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fednova/FedNovaServerManager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fednova/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3309 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fednova/FedNovaTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fednova/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     4893 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fednova/FedNovaClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)    10695 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fednova/FedNovaAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     3306 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fednova/my_model_trainer_classification.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedopt/
--rw-r--r--   0 runner     (501) staff       (20)     8893 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedopt/FedOptAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)      578 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedopt/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     2663 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedopt/FedOptClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedopt/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1830 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedopt/optrepo.py
--rw-r--r--   0 runner     (501) staff       (20)     3297 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedopt/FedOptAPI.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedopt/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     1307 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedopt/FedOptTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     4470 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedopt/FedOptServerManager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedopt_seq/
--rw-r--r--   0 runner     (501) staff       (20)     3300 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedopt_seq/FedOptSeqAPI.py
--rw-r--r--   0 runner     (501) staff       (20)    12025 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedopt_seq/FedOptAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1009 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedopt_seq/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     4464 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedopt_seq/FedOptClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedopt_seq/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1830 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedopt_seq/optrepo.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedopt_seq/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     1307 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedopt_seq/FedOptTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     5535 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedopt_seq/FedOptServerManager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedseg/
--rw-r--r--   0 runner     (501) staff       (20)     3507 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedseg/FedSegClientManager.py
--rw-r--r--   0 runner     (501) staff       (20)      716 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedseg/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     1927 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedseg/FedSegTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)     6138 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedseg/MyModelTrainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedseg/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    12406 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedseg/FedSegAggregator.py
--rw-r--r--   0 runner     (501) staff       (20)    10700 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedseg/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2448 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedseg/FedSegAPI.py
--rw-r--r--   0 runner     (501) staff       (20)     4172 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/mpi/fedseg/FedSegServerManager.py
--rw-r--r--   0 runner     (501) staff       (20)      205 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     9847 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/simulation/simulator.py
--rw-r--r--   0 runner     (501) staff       (20)    14566 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/utils/
--rw-r--r--   0 runner     (501) staff       (20)    10317 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/utils/model_utils.py
--rw-r--r--   0 runner     (501) staff       (20)      735 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/utils/logging.py
--rw-r--r--   0 runner     (501) staff       (20)    10524 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/utils/compression.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/utils/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      809 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/utils/context.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cli/
--rwxr-xr-x   0 runner     (501) staff       (20)      313 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/cli_utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cli/edge_deployment/
--rwxr-xr-x   0 runner     (501) staff       (20)    14236 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/edge_deployment/client_data_interface.py
--rwxr-xr-x   0 runner     (501) staff       (20)    11063 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/edge_deployment/client_login.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2266 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/edge_deployment/client_daemon.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/edge_deployment/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)     5658 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/edge_deployment/docker_login.py
--rwxr-xr-x   0 runner     (501) staff       (20)    52330 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/edge_deployment/client_runner.py
--rw-r--r--   0 runner     (501) staff       (20)    15185 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/edge_deployment/client_constants.py
--rw-r--r--   0 runner     (501) staff       (20)    10779 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/edge_deployment/client_diagnosis.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1969 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/edge_deployment/client_api.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3126 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/edge_deployment/simulator_daemon.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cli/model_deployment/
--rwxr-xr-x   0 runner     (501) staff       (20)     5427 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_model_inference.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2320 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_client_daemon.py
--rw-r--r--   0 runner     (501) staff       (20)     7935 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/modelops_configs.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1983 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_server_api.py
--rwxr-xr-x   0 runner     (501) staff       (20)    73881 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_server_runner.py
--rwxr-xr-x   0 runner     (501) staff       (20)    25696 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_model_cards.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1983 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_client_api.py
--rwxr-xr-x   0 runner     (501) staff       (20)     5426 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/docker_client_login.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)    16417 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_server_login.py
--rwxr-xr-x   0 runner     (501) staff       (20)    16754 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_model_cache.py
--rwxr-xr-x   0 runner     (501) staff       (20)    34262 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_model_deployment.py
--rwxr-xr-x   0 runner     (501) staff       (20)      816 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_server_data_interface.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1766 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_model_object.py
--rwxr-xr-x   0 runner     (501) staff       (20)    26434 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_model_db.py
--rwxr-xr-x   0 runner     (501) staff       (20)     6554 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_login_entry.py
--rwxr-xr-x   0 runner     (501) staff       (20)    14992 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_client_data_interface.py
--rw-r--r--   0 runner     (501) staff       (20)    19913 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_server_constants.py
--rwxr-xr-x   0 runner     (501) staff       (20)     8168 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_model_monitor.py
--rw-r--r--   0 runner     (501) staff       (20)    25461 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_client_constants.py
--rwxr-xr-x   0 runner     (501) staff       (20)    46421 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_client_runner.py
--rwxr-xr-x   0 runner     (501) staff       (20)     5460 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/docker_server_login.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2986 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_server_daemon.py
--rwxr-xr-x   0 runner     (501) staff       (20)     6819 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_client_login.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2759 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_model_msg_object.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2906 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/model_deployment/device_model_inference_entry.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cli/env/
--rw-r--r--   0 runner     (501) staff       (20)     3453 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/env/collect_env.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/env/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)    45366 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/cli.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cli/build-package/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/build-package/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-server/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1253 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/fedml_config.yaml
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/torch_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      629 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/fedml.yaml
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-server/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-client/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1253 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/fedml_config.yaml
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/torch_client.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      650 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/fedml.yaml
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-client/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cli/comm_utils/
--rw-r--r--   0 runner     (501) staff       (20)    24852 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/comm_utils/sys_utils.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/comm_utils/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      295 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/comm_utils/yaml_utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cli/server_deployment/
--rwxr-xr-x   0 runner     (501) staff       (20)      749 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/server_deployment/server_data_interface.py
--rwxr-xr-x   0 runner     (501) staff       (20)    71491 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/server_deployment/server_runner.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/server_deployment/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2848 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/server_deployment/job_manager.py
--rwxr-xr-x   0 runner     (501) staff       (20)     5692 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/server_deployment/docker_login.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1971 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/server_deployment/server_api.py
--rwxr-xr-x   0 runner     (501) staff       (20)    10533 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/server_deployment/app_manager.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2522 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/server_deployment/server_daemon.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cli/server_deployment/templates/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/server_deployment/templates/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      404 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/server_deployment/templates/fedml-aggregator-data-pv.yaml
--rw-r--r--   0 runner     (501) staff       (20)      279 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/server_deployment/templates/fedml-aggregator-data-pvc.yaml
--rw-r--r--   0 runner     (501) staff       (20)      275 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/server_deployment/templates/fedml-server-svc.yaml
--rw-r--r--   0 runner     (501) staff       (20)     1370 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/server_deployment/templates/fedml-server-deployment.yaml
--rwxr-xr-x   0 runner     (501) staff       (20)    13814 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/server_deployment/server_login.py
--rw-r--r--   0 runner     (501) staff       (20)    14281 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cli/server_deployment/server_constants.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cheetah/
--rw-r--r--   0 runner     (501) staff       (20)      153 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cheetah/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cheetah/server/
--rw-r--r--   0 runner     (501) staff       (20)     2212 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cheetah/server/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cheetah/server/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    15366 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cheetah/server/fedml_server_manager.py
--rw-r--r--   0 runner     (501) staff       (20)    11613 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cheetah/server/fedml_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1056 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cheetah/server/server_initializer.py
--rw-r--r--   0 runner     (501) staff       (20)     1939 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cheetah/fedml_client.py
--rw-r--r--   0 runner     (501) staff       (20)     2047 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cheetah/fedml_server.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/cheetah/client/
--rw-r--r--   0 runner     (501) staff       (20)     2266 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cheetah/client/client_initializer.py
--rw-r--r--   0 runner     (501) staff       (20)     5161 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cheetah/client/client_launcher.py
--rw-r--r--   0 runner     (501) staff       (20)     2673 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cheetah/client/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)     2680 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cheetah/client/fedml_trainer_dist_adapter.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cheetah/client/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1655 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cheetah/client/fedml_client_slave_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     1258 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cheetah/client/process_group_manager.py
--rw-r--r--   0 runner     (501) staff       (20)      677 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cheetah/client/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     7549 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cheetah/client/fedml_client_master_manager.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3563 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/cheetah/client/fedml_trainer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/ml/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/ml/aggregator/
--rw-r--r--   0 runner     (501) staff       (20)      548 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/aggregator/aggregator_creator.py
--rw-r--r--   0 runner     (501) staff       (20)     2488 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/aggregator/my_server_aggregator_nwp.py
--rw-r--r--   0 runner     (501) staff       (20)     4187 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/aggregator/default_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/aggregator/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5621 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/aggregator/my_server_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     2408 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/aggregator/my_server_aggregator_classification.py
--rw-r--r--   0 runner     (501) staff       (20)    10546 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/aggregator/agg_operator.py
--rw-r--r--   0 runner     (501) staff       (20)     3388 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/aggregator/my_server_aggregator_prediction.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/ml/engine/
--rw-r--r--   0 runner     (501) staff       (20)    11333 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/engine/ml_engine_adapter.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/engine/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1345 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/engine/torch_process_group_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/ml/trainer/
--rw-r--r--   0 runner     (501) staff       (20)     3953 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/trainer/scaffold_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)      580 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/trainer/trainer_creator.py
--rw-r--r--   0 runner     (501) staff       (20)     9496 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/trainer/fednova_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/trainer/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/trainer/local_optimizer.py
--rw-r--r--   0 runner     (501) staff       (20)     5923 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/trainer/fedprox_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     3578 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/trainer/my_model_trainer_nwp.py
--rw-r--r--   0 runner     (501) staff       (20)     6857 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/trainer/feddyn_trainer copy.py
--rw-r--r--   0 runner     (501) staff       (20)     5180 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/trainer/feddyn_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     5063 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/trainer/my_model_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     6274 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/trainer/mime_trainer.py
--rw-r--r--   0 runner     (501) staff       (20)     4026 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/trainer/my_model_trainer_tag_prediction.py
--rw-r--r--   0 runner     (501) staff       (20)     5805 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/ml/trainer/my_model_trainer_classification.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/model/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/model/linear/
--rw-r--r--   0 runner     (501) staff       (20)      433 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/linear/lr.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/linear/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      544 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/linear/lr_cifar10.py
--rw-r--r--   0 runner     (501) staff       (20)       52 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4549 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/model_hub.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/model/mobile/
--rw-r--r--   0 runner     (501) staff       (20)      988 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/mobile/mnn_lenet.py
--rw-r--r--   0 runner     (501) staff       (20)     3860 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/mobile/mnn_resnet.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/mobile/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      774 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/mobile/torch_lenet.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/model/nlp/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/nlp/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6272 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/nlp/model_args.py
--rw-r--r--   0 runner     (501) staff       (20)     4687 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/nlp/rnn.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/model/finance/
--rw-r--r--   0 runner     (501) staff       (20)      458 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/finance/vfl_feature_extractor.py
--rw-r--r--   0 runner     (501) staff       (20)     2385 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/finance/vfl_models_standalone.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/finance/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      354 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/finance/vfl_classifier.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/model/cv/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/model/cv/resnet56/
--rw-r--r--   0 runner     (501) staff       (20)     9541 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/resnet56/resnet_pretrained.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/resnet56/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     8241 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/resnet56/resnet_server.py
--rw-r--r--   0 runner     (501) staff       (20)     9507 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/resnet56/resnet_client.py
--rw-r--r--   0 runner     (501) staff       (20)     6216 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/vgg.py
--rw-r--r--   0 runner     (501) staff       (20)      455 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/test_cnn.py
--rw-r--r--   0 runner     (501) staff       (20)    16186 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/resnet_torch.py
--rw-r--r--   0 runner     (501) staff       (20)    25891 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/efficientnet_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     7751 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/resnet_cifar.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    10352 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/mobilenet_v3.py
--rw-r--r--   0 runner     (501) staff       (20)    19954 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/batchnorm_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     7629 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/cnn.py
--rw-r--r--   0 runner     (501) staff       (20)     1590 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/mnist_gan.py
--rw-r--r--   0 runner     (501) staff       (20)    17984 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/efficientnet.py
--rw-r--r--   0 runner     (501) staff       (20)    25096 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/resnet_all.py
--rw-r--r--   0 runner     (501) staff       (20)     4593 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/mobilenet.py
--rw-r--r--   0 runner     (501) staff       (20)    74592 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/common.py
--rw-r--r--   0 runner     (501) staff       (20)    10274 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/resnet.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/model/cv/darts/
--rw-r--r--   0 runner     (501) staff       (20)     7088 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/darts/model_search_gdas.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/darts/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1713 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/darts/visualize.py
--rw-r--r--   0 runner     (501) staff       (20)    18693 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/darts/architect.py
--rw-r--r--   0 runner     (501) staff       (20)     7681 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/darts/model.py
--rw-r--r--   0 runner     (501) staff       (20)     4504 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/darts/operations.py
--rw-r--r--   0 runner     (501) staff       (20)     3268 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/darts/utils.py
--rw-r--r--   0 runner     (501) staff       (20)    12302 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/darts/model_search.py
--rw-r--r--   0 runner     (501) staff       (20)     8673 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/darts/train.py
--rw-r--r--   0 runner     (501) staff       (20)     3486 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/darts/genotypes.py
--rw-r--r--   0 runner     (501) staff       (20)    14555 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/darts/train_search.py
--rw-r--r--   0 runner     (501) staff       (20)     7625 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/resnet_gn.py
--rw-r--r--   0 runner     (501) staff       (20)     5343 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/model/cv/group_normalization.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/device/
--rw-r--r--   0 runner     (501) staff       (20)     2833 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/device/gpu_mapping_cross_silo.py
--rw-r--r--   0 runner     (501) staff       (20)     3632 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/device/gpu_mapping_mpi.py
--rw-r--r--   0 runner     (501) staff       (20)     5611 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/device/device.py
--rw-r--r--   0 runner     (501) staff       (20)      112 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/device/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      346 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/device/ip_config_utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/fa/
--rw-r--r--   0 runner     (501) staff       (20)     1817 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/runner.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/fa/cross_silo/
--rw-r--r--   0 runner     (501) staff       (20)      674 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/cross_silo/fa_server.py
--rw-r--r--   0 runner     (501) staff       (20)      645 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/cross_silo/fa_client.py
--rw-r--r--   0 runner     (501) staff       (20)      186 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/cross_silo/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/fa/cross_silo/server/
--rw-r--r--   0 runner     (501) staff       (20)     2182 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/cross_silo/server/message_define.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/cross_silo/server/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    11137 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/cross_silo/server/fedml_server_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     5135 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/cross_silo/server/fedml_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)      879 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/cross_silo/server/server_initializer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/fa/cross_silo/client/
--rw-r--r--   0 runner     (501) staff       (20)     1526 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/cross_silo/client/client_initializer.py
--rw-r--r--   0 runner     (501) staff       (20)      809 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/cross_silo/client/client_launcher.py
--rw-r--r--   0 runner     (501) staff       (20)     2673 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/cross_silo/client/message_define.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1853 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/cross_silo/client/fa_local_analyzer.py
--rw-r--r--   0 runner     (501) staff       (20)     1960 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/cross_silo/client/fedml_trainer_dist_adapter.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/cross_silo/client/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1655 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/cross_silo/client/fedml_client_slave_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     1258 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/cross_silo/client/process_group_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     5993 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/cross_silo/client/fedml_client_master_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/fa/aggregator/
--rw-r--r--   0 runner     (501) staff       (20)     1903 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/aggregator/frequency_estimation_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1885 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/aggregator/intersection_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     1559 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/aggregator/union_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     2114 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/aggregator/avg_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)     3908 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/aggregator/k_percentile_element_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/aggregator/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1163 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/aggregator/global_analyzer_creator.py
--rw-r--r--   0 runner     (501) staff       (20)      414 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/constants.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/fa/simulation/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/fa/simulation/sp/
--rw-r--r--   0 runner     (501) staff       (20)     1192 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/simulation/sp/client.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/simulation/sp/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3316 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/simulation/sp/simulator.py
--rw-r--r--   0 runner     (501) staff       (20)      119 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/simulation/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      606 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/simulation/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2832 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/fa/local_analyzer/
--rw-r--r--   0 runner     (501) staff       (20)     4574 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/local_analyzer/heavy_hitter_triehh.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/local_analyzer/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      453 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/local_analyzer/frequency_estimation.py
--rw-r--r--   0 runner     (501) staff       (20)     1245 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/local_analyzer/client_analyzer_creator.py
--rw-r--r--   0 runner     (501) staff       (20)      392 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/local_analyzer/k_percentage_element.py
--rw-r--r--   0 runner     (501) staff       (20)      223 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/local_analyzer/intersection.py
--rw-r--r--   0 runner     (501) staff       (20)      217 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/local_analyzer/union.py
--rw-r--r--   0 runner     (501) staff       (20)      348 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/local_analyzer/avg.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/fa/base_frame/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/base_frame/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      527 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/base_frame/server_aggregator.py
--rw-r--r--   0 runner     (501) staff       (20)      911 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/base_frame/client_analyzer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/fa/data/
--rw-r--r--   0 runner     (501) staff       (20)     2564 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/data/data_loader.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/fa/data/twitter_Sentiment140/
--rw-r--r--   0 runner     (501) staff       (20)      932 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/data/twitter_Sentiment140/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/data/twitter_Sentiment140/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       75 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/data/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      927 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/data/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/fa/data/fake_numeric_data/
--rw-r--r--   0 runner     (501) staff       (20)      526 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/data/fake_numeric_data/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/fa/data/fake_numeric_data/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      545 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/launch_cross_device.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/MNIST/
--rw-r--r--   0 runner     (501) staff       (20)     5448 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/MNIST/mnist_mobile_preprocessor.py
--rwxr-xr-x   0 runner     (501) staff       (20)     4826 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/MNIST/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/MNIST/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2942 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/MNIST/stats.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/lending_club_loan/
--rw-r--r--   0 runner     (501) staff       (20)     7729 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/lending_club_loan/lending_club_dataset.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/lending_club_loan/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2291 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/lending_club_loan/lending_club_feature_group.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/fed_cifar100/
--rw-r--r--   0 runner     (501) staff       (20)     6320 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/fed_cifar100/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/fed_cifar100/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      517 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/fed_cifar100/dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     2631 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/fed_cifar100/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/FederatedEMNIST/
--rw-r--r--   0 runner     (501) staff       (20)     6737 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/FederatedEMNIST/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/FederatedEMNIST/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      426 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/FederatedEMNIST/dataset.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/cifar100/
--rw-r--r--   0 runner     (501) staff       (20)    11837 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/cifar100/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)     2077 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/cifar100/datasets.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/cifar100/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    21968 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)      156 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4146 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/file_operation.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/shakespeare/
--rwxr-xr-x   0 runner     (501) staff       (20)     3431 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/shakespeare/language_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     4135 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/shakespeare/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/shakespeare/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      335 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/shakespeare/dataset.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2942 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/shakespeare/stats.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/synthetic_1_1/
--rw-r--r--   0 runner     (501) staff       (20)     4562 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/synthetic_1_1/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/synthetic_1_1/__init__.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3210 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/synthetic_1_1/stats.py
--rw-r--r--   0 runner     (501) staff       (20)     2749 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/synthetic_1_1/generate_synthetic.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/Landmarks/
--rw-r--r--   0 runner     (501) staff       (20)      375 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/Landmarks/download_with_tff.py
--rw-r--r--   0 runner     (501) staff       (20)    14871 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/Landmarks/download_without_tff.py
--rw-r--r--   0 runner     (501) staff       (20)    11159 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/Landmarks/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)     2191 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/Landmarks/datasets.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/Landmarks/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    14342 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/Landmarks/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2090 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/Landmarks/check_download.py
--rw-r--r--   0 runner     (501) staff       (20)     7872 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/Landmarks/download_without_tf.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/fednlp/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/fednlp/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/fednlp/base/
--rw-r--r--   0 runner     (501) staff       (20)      169 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/fednlp/base/globals.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/fednlp/base/preprocess/
--rw-r--r--   0 runner     (501) staff       (20)     4794 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/fednlp/base/preprocess/base_example.py
--rw-r--r--   0 runner     (501) staff       (20)      363 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/fednlp/base/preprocess/base_data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/fednlp/base/preprocess/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      224 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/fednlp/base/preprocess/base_preprocessor.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/fednlp/base/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/fednlp/base/raw_data/
--rw-r--r--   0 runner     (501) staff       (20)     1428 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/fednlp/base/raw_data/partition.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/fednlp/base/raw_data/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3636 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/fednlp/base/raw_data/base_raw_data_loader.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/fednlp/base/data_manager/
--rw-r--r--   0 runner     (501) staff       (20)    16505 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/fednlp/base/data_manager/base_data_manager.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/fednlp/base/data_manager/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     8248 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/fednlp/base/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/NUS_WIDE/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/NUS_WIDE/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    11281 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/NUS_WIDE/nus_wide_dataset.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/stackoverflow_lr/
--rw-r--r--   0 runner     (501) staff       (20)     8487 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/stackoverflow_lr/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/stackoverflow_lr/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2841 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/stackoverflow_lr/dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     4272 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/stackoverflow_lr/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/fed_shakespeare/
--rw-r--r--   0 runner     (501) staff       (20)     6100 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/fed_shakespeare/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/fed_shakespeare/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3633 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/fed_shakespeare/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/ImageNet/
--rw-r--r--   0 runner     (501) staff       (20)    11416 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/ImageNet/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)     6718 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/ImageNet/datasets.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/ImageNet/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5874 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/ImageNet/datasets_hdf5.py
--rw-r--r--   0 runner     (501) staff       (20)     1429 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/data_loader_cross_silo.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/cinic10/
--rw-r--r--   0 runner     (501) staff       (20)    13807 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/cinic10/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)     3071 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/cinic10/datasets.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/cinic10/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/stackoverflow_nwp/
--rw-r--r--   0 runner     (501) staff       (20)     7023 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/stackoverflow_nwp/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/stackoverflow_nwp/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2171 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/stackoverflow_nwp/dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     2508 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/stackoverflow_nwp/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/UCI/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/UCI/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6215 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/UCI/data_loader_for_susy_and_ro.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/edge_case_examples/
--rw-r--r--   0 runner     (501) staff       (20)    44697 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/edge_case_examples/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)    20285 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/edge_case_examples/datasets.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/edge_case_examples/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml/data/cifar10/
--rw-r--r--   0 runner     (501) staff       (20)    13825 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/cifar10/efficient_loader.py
--rw-r--r--   0 runner     (501) staff       (20)    11902 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/cifar10/data_loader.py
--rw-r--r--   0 runner     (501) staff       (20)     2378 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/cifar10/datasets.py
--rw-r--r--   0 runner     (501) staff       (20)     3972 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/cifar10/without_reload.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-30 05:33:16.000000 fedml-0.8.4a9/fedml/data/cifar10/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     3806 2023-04-30 05:33:27.000000 fedml-0.8.4a9/fedml.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    47479 2023-04-30 05:33:28.000000 fedml-0.8.4a9/fedml.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)       45 2023-04-30 05:33:27.000000 fedml-0.8.4a9/fedml.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)      588 2023-04-30 05:33:27.000000 fedml-0.8.4a9/fedml.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       21 2023-04-30 05:33:27.000000 fedml-0.8.4a9/fedml.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-30 05:33:27.000000 fedml-0.8.4a9/fedml.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/
+-rw-r--r--   0 runner     (501) staff       (20)     3806 2023-06-24 12:02:55.000000 fedml-0.8.5a1/PKG-INFO
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/tests/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/tests/security/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/tests/security/attack/
+-rw-r--r--   0 runner     (501) staff       (20)     2718 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/attack/test_label_flipping_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)      730 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/attack/test_backdoor.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/attack/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1159 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/attack/test_model_replacement_backdoor_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     5147 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/attack/test_invertgradient.py
+-rw-r--r--   0 runner     (501) staff       (20)     1586 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/attack/test_byzantine_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     5519 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/attack/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     1091 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/attack/test_edge_case_backdoor_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     1466 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/attack/test_dlg.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/tests/security/defense/
+-rw-r--r--   0 runner     (501) staff       (20)      376 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/defense/test_rfa.py
+-rw-r--r--   0 runner     (501) staff       (20)     1942 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/defense/test_residual_based_reweighting.py
+-rw-r--r--   0 runner     (501) staff       (20)     1139 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/defense/test_wbc.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/defense/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1099 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/defense/test_crfl.py
+-rw-r--r--   0 runner     (501) staff       (20)     1889 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/defense/test_geometric_median.py
+-rw-r--r--   0 runner     (501) staff       (20)     2682 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/defense/test_slsgd_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     1327 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/defense/test_weak_dp.py
+-rw-r--r--   0 runner     (501) staff       (20)     1525 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/defense/test_norm_diff_clipping.py
+-rw-r--r--   0 runner     (501) staff       (20)     5913 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/defense/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     1555 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/defense/test_bulyan.py
+-rw-r--r--   0 runner     (501) staff       (20)      805 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/defense/test_robust_learning_rate_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)      999 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/defense/test_coordinate_wise_trimmed_mean.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1206 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/defense/test_krum.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1276 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/defense/test_cclip.py
+-rw-r--r--   0 runner     (501) staff       (20)      408 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/defense/test_coordinate_median.py
+-rw-r--r--   0 runner     (501) staff       (20)      902 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/defense/test_foolsgold_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     2208 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/security/defense/test_soteria.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/tests/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2326 2023-06-24 12:02:34.000000 fedml-0.8.5a1/README.md
+-rw-r--r--   0 runner     (501) staff       (20)     4554 2023-06-24 12:02:36.000000 fedml-0.8.5a1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/one_line/torch_server.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     2026 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       89 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)       89 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/torch_server.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/
+-rw-r--r--   0 runner     (501) staff       (20)      404 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/main_fedml_cross_silo_hi.py
+-rw-r--r--   0 runner     (501) staff       (20)      196 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/mlops_client_launcher.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2003 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/step_by_step/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2024 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/torch_server.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)     4403 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_trainer_classification.py
+-rw-r--r--   0 runner     (501) staff       (20)     5218 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2033 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_server.py
+-rw-r--r--   0 runner     (501) staff       (20)     2020 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     1435 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      757 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      757 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/
+-rw-r--r--   0 runner     (501) staff       (20)     1689 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2119 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_trainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)     4098 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_trainer_classification.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1739 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model.py
+-rw-r--r--   0 runner     (501) staff       (20)     5323 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1999 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     2013 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/trpc_fedavg_mnist_lr_example/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/torch_server.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/trpc_fedavg_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2003 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/step_by_step/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1993 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     3354 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1387 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_trainer_classification.py
+-rw-r--r--   0 runner     (501) staff       (20)     2007 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_server.py
+-rw-r--r--   0 runner     (501) staff       (20)      699 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_hierarchical_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      404 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_hierarchical_mnist_lr_example/main_fedml_cross_silo_hi.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_hierarchical_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/privacy/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/privacy/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/privacy/mqtt_s3_fedavg_cdp_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/privacy/mqtt_s3_fedavg_cdp_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/privacy/mqtt_s3_fedavg_cdp_mnist_lr_example/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/privacy/mqtt_s3_fedavg_cdp_mnist_lr_example/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/privacy/mpi_fedavg_dp_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/privacy/mpi_fedavg_dp_mnist_lr_example/cross_silo_with_mpi.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/privacy/mpi_fedavg_dp_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/privacy/mqtt_s3_fedavg_ldp_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/privacy/mqtt_s3_fedavg_ldp_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/privacy/mqtt_s3_fedavg_ldp_mnist_lr_example/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/privacy/mqtt_s3_fedavg_ldp_mnist_lr_example/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/security/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/security/mqtt_s3_fedavg_attack_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/security/mqtt_s3_fedavg_attack_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/security/mqtt_s3_fedavg_attack_mnist_lr_example/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      395 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/security/mqtt_s3_fedavg_attack_mnist_lr_example/torch_server.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/security/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      827 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      965 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_mpi.py
+-rw-r--r--   0 runner     (501) staff       (20)      827 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      966 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/torch_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      966 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/torch_mpi.py
+-rw-r--r--   0 runner     (501) staff       (20)      966 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_device/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/
+-rw-r--r--   0 runner     (501) staff       (20)     1214 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/my_dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      801 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/torch_server.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_device/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/
+-rw-r--r--   0 runner     (501) staff       (20)     1178 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/my_dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3268 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/centralized/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/centralized/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    20282 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/centralized/main.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/mpi_fedopt_datasets_and_models_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_fedopt_datasets_and_models_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_fedopt_datasets_and_models_example/torch_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/examples/simulation/sp_vertical_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_vertical_mnist_lr_example/torch_vertical_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_vertical_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/examples/simulation/sp_fedopt_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_fedopt_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_fedopt_mnist_lr_example/torch_fedopt_mnist_lr_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/mpi_decentralized_fl_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_decentralized_fl_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      222 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_decentralized_fl_example/mpi_decentralized_fl_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/sp_decentralized_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_decentralized_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_decentralized_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedgkt_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedgkt_mnist_lr_example/torch_fedgkt_cifar10_resnet56.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedgkt_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg/
+-rw-r--r--   0 runner     (501) staff       (20)     5590 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg/reddit_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     4816 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg/reddit_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6461 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg/main.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/examples/simulation/sp_hierarchicalfl_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_hierarchicalfl_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_hierarchicalfl_mnist_lr_example/torch_hierarchicalfl_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedopt_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedopt_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedopt_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedgan_mnist_gan_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedgan_mnist_gan_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedgan_mnist_gan_example/torch_fedgan_mnist_gan_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/mpi_fedavg_datasets_and_models_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_fedavg_datasets_and_models_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_fedavg_datasets_and_models_example/torch_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_seq/
+-rw-r--r--   0 runner     (501) staff       (20)      762 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_seq/torch_fedavg.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_seq/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/mpi_fedprox_datasets_and_models_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_fedprox_datasets_and_models_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_fedprox_datasets_and_models_example/torch_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/examples/simulation/sp_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)       69 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_one_line_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_fedavg_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      423 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fednas_cifar10_dart_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fednas_cifar10_dart_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fednas_cifar10_dart_example/torch_fednas_cifar10_dart_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
+-rw-r--r--   0 runner     (501) staff       (20)       82 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_splitnn_cifar10_resnet56_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_splitnn_cifar10_resnet56_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_splitnn_cifar10_resnet56_example/torch_splitnn_mnist_lr_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/examples/simulation/sp_fednova_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_fednova_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_fednova_mnist_lr_example/torch_fednova_mnist_lr_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
+-rw-r--r--   0 runner     (501) staff       (20)       82 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
+-rw-r--r--   0 runner     (501) staff       (20)       82 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/mpi_base_framework_example/
+-rw-r--r--   0 runner     (501) staff       (20)      222 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_base_framework_example/mpi_base_framework_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_base_framework_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/sp_fedavg_mnist_cnn_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_fedavg_mnist_cnn_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_fedavg_mnist_cnn_example/torch_fedavg_mnist_cnn_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py
+-rw-r--r--   0 runner     (501) staff       (20)       82 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_one_line_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)       82 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_one_line_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)     1990 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedprox_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedprox_mnist_lr_example/torch_fedprox_mnist_lr_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_fedprox_mnist_lr_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/examples/simulation/sp_turboaggregate_mnist_lr_example/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_turboaggregate_mnist_lr_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_turboaggregate_mnist_lr_example/torch_turboaggregate_mnist_lr_step_by_step_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_async_fedavg/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_async_fedavg/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1042 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/mpi_torch_async_fedavg/torch_fedavg_mnist_lr_custum_data_and_model_example.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/simulation/sp_fedavg_datasets_and_models_example/
+-rw-r--r--   0 runner     (501) staff       (20)      422 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_fedavg_datasets_and_models_example/torch_fedavg_step_by_step_example.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/examples/simulation/sp_fedavg_datasets_and_models_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/federated_analytics/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/federated_analytics/intersection_and_cardinality_fake_data_example/
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/intersection_and_cardinality_fake_data_example/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/intersection_and_cardinality_fake_data_example/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/intersection_and_cardinality_fake_data_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/federated_analytics/heavy_hitter_twitter_data_example/
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/heavy_hitter_twitter_data_example/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/heavy_hitter_twitter_data_example/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/heavy_hitter_twitter_data_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/federated_analytics/frequency_estimation_fake_data_example/
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/frequency_estimation_fake_data_example/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/frequency_estimation_fake_data_example/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/frequency_estimation_fake_data_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/federated_analytics/avg_self_defined_data_example/
+-rw-r--r--   0 runner     (501) staff       (20)      316 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/avg_self_defined_data_example/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      280 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/avg_self_defined_data_example/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/avg_self_defined_data_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/federated_analytics/avg_fake_data_example/
+-rw-r--r--   0 runner     (501) staff       (20)      316 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/avg_fake_data_example/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/avg_fake_data_example/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/avg_fake_data_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/federated_analytics/k_percentile_fake_data_example/
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/k_percentile_fake_data_example/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/k_percentile_fake_data_example/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/k_percentile_fake_data_example/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/examples/federated_analytics/union_fake_data_example/
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/union_fake_data_example/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      282 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/union_fake_data_example/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:35.000000 fedml-0.8.5a1/examples/federated_analytics/union_fake_data_example/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-06-24 12:02:55.000000 fedml-0.8.5a1/setup.cfg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/
+-rw-r--r--   0 runner     (501) staff       (20)     1061 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/launch_serving.py
+-rw-r--r--   0 runner     (501) staff       (20)     1078 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/launch_cross_silo_hi.py
+-rw-r--r--   0 runner     (501) staff       (20)     7392 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/runner.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cross_silo/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cross_silo/lightsecagg/
+-rw-r--r--   0 runner     (501) staff       (20)     3009 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/lightsecagg/lsa_message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)    11077 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/lightsecagg/lsa_fedml_client_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/lightsecagg/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    13517 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/lightsecagg/lsa_fedml_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)    12846 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/lightsecagg/lsa_fedml_server_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     3467 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/lightsecagg/lsa_fedml_api.py
+-rw-r--r--   0 runner     (501) staff       (20)      157 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cross_silo/server/
+-rw-r--r--   0 runner     (501) staff       (20)     2212 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/server/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/server/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    15649 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/server/fedml_server_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)    11720 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/server/fedml_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1056 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/server/server_initializer.py
+-rw-r--r--   0 runner     (501) staff       (20)     1917 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/fedml_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     2025 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/fedml_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cross_silo/client/
+-rw-r--r--   0 runner     (501) staff       (20)     2266 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/client/client_initializer.py
+-rw-r--r--   0 runner     (501) staff       (20)     5161 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/client/client_launcher.py
+-rw-r--r--   0 runner     (501) staff       (20)     2673 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/client/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     2680 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/client/fedml_trainer_dist_adapter.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/client/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1655 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/client/fedml_client_slave_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1258 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/client/process_group_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)      677 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/client/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     8064 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/client/fedml_client_master_manager.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3563 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_silo/client/fedml_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     1079 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/launch_cross_silo_horizontal.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/serving/
+-rw-r--r--   0 runner     (501) staff       (20)      163 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/serving/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/serving/server/
+-rw-r--r--   0 runner     (501) staff       (20)     2212 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/serving/server/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/serving/server/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    15366 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/serving/server/fedml_server_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)    11613 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/serving/server/fedml_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1056 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/serving/server/server_initializer.py
+-rw-r--r--   0 runner     (501) staff       (20)     1340 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/serving/fedml_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     1456 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/serving/fedml_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/serving/client/
+-rw-r--r--   0 runner     (501) staff       (20)     2266 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/serving/client/client_initializer.py
+-rw-r--r--   0 runner     (501) staff       (20)     5161 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/serving/client/client_launcher.py
+-rw-r--r--   0 runner     (501) staff       (20)     2673 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/serving/client/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     2680 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/serving/client/fedml_trainer_dist_adapter.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/serving/client/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1655 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/serving/client/fedml_client_slave_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1258 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/serving/client/process_group_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)      677 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/serving/client/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     7549 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/serving/client/fedml_client_master_manager.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3563 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/serving/client/fedml_trainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/schedule/
+-rw-r--r--   0 runner     (501) staff       (20)     5761 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/schedule/runtime_estimate.py
+-rw-r--r--   0 runner     (501) staff       (20)     9840 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/schedule/seq_train_scheduler.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/schedule/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/alg_frame/
+-rw-r--r--   0 runner     (501) staff       (20)      795 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/alg_frame/params.py
+-rw-r--r--   0 runner     (501) staff       (20)     2349 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/alg_frame/client_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/alg_frame/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      894 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/alg_frame/context.py
+-rw-r--r--   0 runner     (501) staff       (20)     5792 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/alg_frame/server_aggregator.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/distributed/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/distributed/topology/
+-rw-r--r--   0 runner     (501) staff       (20)     5001 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/topology/asymmetric_topology_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)      479 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/topology/base_topology_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     3853 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/topology/symmetric_topology_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/topology/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/distributed/crypto/
+-rw-r--r--   0 runner     (501) staff       (20)     2167 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/crypto/crypto_api.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/crypto/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     8764 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/fedml_comm_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/distributed/communication/
+-rw-r--r--   0 runner     (501) staff       (20)      153 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/observer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/distributed/communication/s3/
+-rw-r--r--   0 runner     (501) staff       (20)     1680 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/s3/remote_storage_mnn.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/s3/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    22460 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/s3/remote_storage.py
+-rw-r--r--   0 runner     (501) staff       (20)     2792 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/s3/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/distributed/communication/mpi/
+-rw-r--r--   0 runner     (501) staff       (20)     1648 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/mpi/mpi_send_thread.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/mpi/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4977 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/mpi/com_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1603 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/mpi/mpi_receive_thread.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/distributed/communication/grpc/
+-rw-r--r--   0 runner     (501) staff       (20)     1255 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/grpc/grpc_server.py
+-rw-r--r--   0 runner     (501) staff       (20)     6381 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/grpc/grpc_comm_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/distributed/communication/grpc/proto/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/grpc/proto/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/grpc/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4236 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2_grpc.py
+-rw-r--r--   0 runner     (501) staff       (20)      346 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/grpc/ip_config_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     6272 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/distributed/communication/trpc/
+-rw-r--r--   0 runner     (501) staff       (20)     1614 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/trpc/trpc_server.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/trpc/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4807 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/trpc/trpc_comm_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)      437 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/trpc/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)      377 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/constants.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2612 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/message.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/distributed/communication/mqtt_web3/
+-rwxr-xr-x   0 runner     (501) staff       (20)       91 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/mqtt_web3/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    14594 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/mqtt_web3/mqtt_web3_comm_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/distributed/communication/mqtt_thetastore/
+-rwxr-xr-x   0 runner     (501) staff       (20)      109 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/mqtt_thetastore/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    14669 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/mqtt_thetastore/mqtt_thetastore_comm_manager.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      869 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)      518 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/base_com_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/distributed/communication/mqtt_s3/
+-rwxr-xr-x   0 runner     (501) staff       (20)      123 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/mqtt_s3/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    15504 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/mqtt_s3/mqtt_s3_multi_clients_comm_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/distributed/communication/mqtt/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/mqtt/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    14081 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/mqtt/mqtt_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/distributed/communication/mqtt_s3_mnn/
+-rwxr-xr-x   0 runner     (501) staff       (20)       91 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/mqtt_s3_mnn/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    12233 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/communication/mqtt_s3_mnn/mqtt_s3_comm_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/distributed/distributed_storage/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/distributed/distributed_storage/web3_storage/
+-rw-r--r--   0 runner     (501) staff       (20)     3604 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/distributed_storage/web3_storage/web3_storage.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/distributed_storage/web3_storage/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/distributed/distributed_storage/theta_storage/
+-rw-r--r--   0 runner     (501) staff       (20)     6834 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/distributed_storage/theta_storage/theta_storage.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/distributed_storage/theta_storage/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/distributed_storage/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/distributed/flow/
+-rw-r--r--   0 runner     (501) staff       (20)    12684 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/flow/fedml_flow.py
+-rw-r--r--   0 runner     (501) staff       (20)      728 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/flow/fedml_executor.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/flow/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      338 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/flow/fedml_flow_constants.py
+-rw-r--r--   0 runner     (501) staff       (20)     3248 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/distributed/flow/test_fedml_flow.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/security/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/security/attack/
+-rw-r--r--   0 runner     (501) staff       (20)     4005 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/attack/model_replacement_backdoor_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)      696 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/attack/attack_base.py
+-rw-r--r--   0 runner     (501) staff       (20)     3424 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/attack/edge_case_backdoor_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     3607 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/attack/byzantine_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/attack/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6102 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/attack/lazy_worker.py
+-rw-r--r--   0 runner     (501) staff       (20)    27345 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/attack/invert_gradient_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     6112 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/attack/dlg_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     4712 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/attack/revealing_labels_from_gradients_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     3928 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/attack/label_flipping_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     5286 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/attack/backdoor_attack.py
+-rw-r--r--   0 runner     (501) staff       (20)     4414 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/fedml_attacker.py
+-rw-r--r--   0 runner     (501) staff       (20)     1278 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/constants.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     7879 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/fedml_defender.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/security/common/
+-rw-r--r--   0 runner     (501) staff       (20)     2016 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/common/bucket.py
+-rw-r--r--   0 runner     (501) staff       (20)      734 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/common/net.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/common/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1875 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/common/attack_defense_data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     8805 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/common/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/security/defense/
+-rw-r--r--   0 runner     (501) staff       (20)     8885 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/three_sigma_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     2148 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/norm_diff_clipping_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)    10054 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/residual_based_reweighting_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     8375 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/three_sigma_krum_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)      994 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/coordinate_wise_trimmed_mean_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     2849 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/slsgd_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     1629 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/coordinate_wise_median_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     3640 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/wbc_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     2675 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/robust_learning_rate_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1071 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/RFA_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     1682 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/defense_base.py
+-rw-r--r--   0 runner     (501) staff       (20)     3568 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/foolsgold_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     3709 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/soteria_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     5462 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/bulyan_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     4636 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/cross_round_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     6525 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/three_sigma_geomedian_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     2022 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/geometric_median_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     3320 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/crfl_defense.py
+-rw-r--r--   0 runner     (501) staff       (20)     1173 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/outlier_detection.py
+-rw-r--r--   0 runner     (501) staff       (20)     1008 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/weak_dp_defense.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2876 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/cclip_defense.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2564 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/security/defense/krum_defense.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/mlops/
+-rw-r--r--   0 runner     (501) staff       (20)    10089 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/mlops/mlops_configs.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/mlops/ssl/
+-rw-r--r--   0 runner     (501) staff       (20)     4089 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/mlops/ssl/open-dev.fedml.ai_bundle.crt
+-rw-r--r--   0 runner     (501) staff       (20)     4085 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/mlops/ssl/open-release.fedml.ai_bundle.crt
+-rw-r--r--   0 runner     (501) staff       (20)     1947 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/mlops/ssl/open-root-ca.crt
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/mlops/ssl/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4093 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/mlops/ssl/open-test.fedml.ai_bundle.crt
+-rw-r--r--   0 runner     (501) staff       (20)    20693 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/mlops/mlops_metrics.py
+-rw-r--r--   0 runner     (501) staff       (20)     4693 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/mlops/mlops_profiler_event.py
+-rw-r--r--   0 runner     (501) staff       (20)     1377 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/mlops/mlops_status.py
+-rw-r--r--   0 runner     (501) staff       (20)    33486 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/mlops/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    11124 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/mlops/stats_impl.py
+-rw-r--r--   0 runner     (501) staff       (20)     1747 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/mlops/mlops_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)    18085 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/mlops/mlops_runtime_log_daemon.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     4121 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/mlops/system_stats.py
+-rw-r--r--   0 runner     (501) staff       (20)     8514 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/mlops/mlops_runtime_log.py
+-rw-r--r--   0 runner     (501) staff       (20)     1117 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/common/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/common/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      298 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/common/ml_engine_backend.py
+-rw-r--r--   0 runner     (501) staff       (20)      231 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/common/singleton.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/mpc/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/mpc/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6017 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/mpc/lightsecagg.py
+-rw-r--r--   0 runner     (501) staff       (20)    12340 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/mpc/secagg.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/dp/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/dp/mechanisms/
+-rw-r--r--   0 runner     (501) staff       (20)     1443 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/dp/mechanisms/dp_mechanism.py
+-rw-r--r--   0 runner     (501) staff       (20)      659 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/dp/mechanisms/laplace.py
+-rw-r--r--   0 runner     (501) staff       (20)       83 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/dp/mechanisms/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      177 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/dp/mechanisms/base_dp_mechanism.py
+-rw-r--r--   0 runner     (501) staff       (20)     1037 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/dp/mechanisms/gaussian.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/dp/test/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/dp/test/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2532 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/dp/test/test_fed_privacy_mechanism.py
+-rw-r--r--   0 runner     (501) staff       (20)     4178 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/dp/fedml_differential_privacy.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/dp/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/dp/frames/
+-rw-r--r--   0 runner     (501) staff       (20)     3293 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/dp/frames/NbAFL.py
+-rw-r--r--   0 runner     (501) staff       (20)     2444 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/dp/frames/dp_clip.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/dp/frames/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1101 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/dp/frames/cdp.py
+-rw-r--r--   0 runner     (501) staff       (20)      470 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/dp/frames/ldp.py
+-rw-r--r--   0 runner     (501) staff       (20)     2118 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/dp/frames/base_dp_solution.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/dp/budget_accountant/
+-rw-r--r--   0 runner     (501) staff       (20)     6747 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/dp/budget_accountant/rdp_analysis.py
+-rw-r--r--   0 runner     (501) staff       (20)     1141 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/dp/budget_accountant/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6915 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/dp/budget_accountant/rdp_accountant.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/dp/common/
+-rw-r--r--   0 runner     (501) staff       (20)       69 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/dp/common/constants.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/dp/common/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2411 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/dp/common/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/contribution/
+-rw-r--r--   0 runner     (501) staff       (20)     5603 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/contribution/gtg_shapley_value.py
+-rw-r--r--   0 runner     (501) staff       (20)     3197 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/contribution/mr_shapley_value.py
+-rw-r--r--   0 runner     (501) staff       (20)     1665 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/contribution/base_contribution_assessor.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/contribution/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4930 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/contribution/leave_one_out.py
+-rw-r--r--   0 runner     (501) staff       (20)     1922 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/contribution/contribution_assessor_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/core/data/
+-rw-r--r--   0 runner     (501) staff       (20)      158 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/data/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4937 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/core/data/noniid_partition.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/distributed/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/distributed/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:54.000000 fedml-0.8.5a1/fedml/config/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/config/simulaton_mpi/
+-rw-r--r--   0 runner     (501) staff       (20)      964 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/config/simulaton_mpi/fedml_config.yaml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/config/simulation_sp/
+-rw-r--r--   0 runner     (501) staff       (20)     1091 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/config/simulation_sp/fedml_config.yaml
+-rwxr-xr-x   0 runner     (501) staff       (20)     8022 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/arguments.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/mlops/
+-rw-r--r--   0 runner     (501) staff       (20)     2648 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/mlops/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1037 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/launch_cheeath.py
+-rw-r--r--   0 runner     (501) staff       (20)     2198 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/constants.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cross_device/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cross_device/server_mnn/
+-rw-r--r--   0 runner     (501) staff       (20)     2190 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_device/server_mnn/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_device/server_mnn/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    18860 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_device/server_mnn/fedml_server_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     2772 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_device/server_mnn/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)    11252 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_device/server_mnn/fedml_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1264 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_device/server_mnn/server_mnn_api.py
+-rw-r--r--   0 runner     (501) staff       (20)       66 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_device/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      579 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cross_device/mnn_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/centralized/
+-rw-r--r--   0 runner     (501) staff       (20)     6588 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/centralized/centralized_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/centralized/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      685 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/launch_simulation.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/sp/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/sp/fedavg/
+-rw-r--r--   0 runner     (501) staff       (20)     1401 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/fedavg/client.py
+-rw-r--r--   0 runner     (501) staff       (20)       34 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/fedavg/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    12457 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/fedavg/fedavg_api.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/sp/fedprox/
+-rw-r--r--   0 runner     (501) staff       (20)     1401 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/fedprox/client.py
+-rw-r--r--   0 runner     (501) staff       (20)       44 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/fedprox/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    11535 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/fedprox/fedprox_trainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/sp/turboaggregate/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/turboaggregate/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     7850 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/turboaggregate/TA_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     7880 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/turboaggregate/mpc_function.py
+-rw-r--r--   0 runner     (501) staff       (20)      818 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/turboaggregate/TA_client.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/sp/feddyn/
+-rw-r--r--   0 runner     (501) staff       (20)     1916 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/feddyn/client copy.py
+-rw-r--r--   0 runner     (501) staff       (20)     1941 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/feddyn/client.py
+-rw-r--r--   0 runner     (501) staff       (20)       42 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/feddyn/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    16395 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/feddyn/feddyn_trainer copy.py
+-rw-r--r--   0 runner     (501) staff       (20)    15943 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/feddyn/feddyn_trainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/sp/classical_vertical_fl/
+-rw-r--r--   0 runner     (501) staff       (20)     1355 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/classical_vertical_fl/client.py
+-rw-r--r--   0 runner     (501) staff       (20)     3625 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/classical_vertical_fl/party_models.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/classical_vertical_fl/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2241 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/classical_vertical_fl/vfl.py
+-rw-r--r--   0 runner     (501) staff       (20)    10964 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/classical_vertical_fl/vfl_api.py
+-rw-r--r--   0 runner     (501) staff       (20)     3887 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/classical_vertical_fl/vfl_fixture.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/sp/fednova/
+-rw-r--r--   0 runner     (501) staff       (20)     8207 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/fednova/fednova.py
+-rw-r--r--   0 runner     (501) staff       (20)    12457 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/fednova/fednova_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)    10932 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/fednova/fednova_api.py
+-rw-r--r--   0 runner     (501) staff       (20)     6496 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/fednova/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/fednova/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2258 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/fednova/comm_helpers.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/sp/fedopt/
+-rw-r--r--   0 runner     (501) staff       (20)    12255 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/fedopt/fedopt_api.py
+-rw-r--r--   0 runner     (501) staff       (20)     1456 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/fedopt/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/fedopt/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1830 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/fedopt/optrepo.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/sp/hierarchical_fl/
+-rw-r--r--   0 runner     (501) staff       (20)     2133 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/hierarchical_fl/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/hierarchical_fl/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2391 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/hierarchical_fl/group.py
+-rw-r--r--   0 runner     (501) staff       (20)     4644 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/hierarchical_fl/trainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/sp/mime/
+-rw-r--r--   0 runner     (501) staff       (20)     1494 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/mime/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/mime/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3192 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/mime/opt_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)    13370 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/mime/mime_trainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/sp/scaffold/
+-rw-r--r--   0 runner     (501) staff       (20)    13466 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/scaffold/scaffold_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     2677 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/scaffold/client.py
+-rw-r--r--   0 runner     (501) staff       (20)       46 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/scaffold/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/sp/decentralized/
+-rw-r--r--   0 runner     (501) staff       (20)     4187 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/decentralized/decentralized_fl_api.py
+-rw-r--r--   0 runner     (501) staff       (20)     4328 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/decentralized/client_dsgd.py
+-rw-r--r--   0 runner     (501) staff       (20)     5514 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/decentralized/client_pushsum.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/decentralized/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5741 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/sp/decentralized/topology_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/mpi/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedavg/
+-rw-r--r--   0 runner     (501) staff       (20)     2689 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedavg/FedAvgClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)      852 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedavg/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedavg/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6818 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedavg/FedAVGAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     3602 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedavg/FedAvgAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedavg/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2542 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedavg/FedAVGTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     4462 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedavg/FedAvgServerManager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/mpi/split_nn/
+-rw-r--r--   0 runner     (501) staff       (20)     2589 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/split_nn/server.py
+-rw-r--r--   0 runner     (501) staff       (20)     2338 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/split_nn/SplitNNAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)      591 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/split_nn/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     1733 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/split_nn/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/split_nn/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3996 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/split_nn/client_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     2043 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/split_nn/server_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedprox/
+-rw-r--r--   0 runner     (501) staff       (20)      852 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedprox/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     2438 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedprox/FedProxTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedprox/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2804 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedprox/FedProxClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     7365 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedprox/FedProxAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedprox/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     4607 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedprox/FedProxServerManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     3460 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedprox/FedProxAPI.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedgan/
+-rw-r--r--   0 runner     (501) staff       (20)     4494 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedgan/FedGanServerManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     3809 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedgan/FedGanAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)      852 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedgan/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedgan/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3633 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedgan/gan_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)      880 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedgan/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2218 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedgan/FedGANTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     7774 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedgan/FedGANAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     2625 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedgan/FedGanClientManager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedgkt/
+-rw-r--r--   0 runner     (501) staff       (20)    15801 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedgkt/GKTServerTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     2120 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedgkt/FedGKTAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)     3165 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedgkt/GKTServerManager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedgkt/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4940 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedgkt/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)      671 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedgkt/message_def.py
+-rw-r--r--   0 runner     (501) staff       (20)     2925 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedgkt/GKTClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     6492 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedgkt/GKTClientTrainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/mpi/base_framework/
+-rw-r--r--   0 runner     (501) staff       (20)      428 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/base_framework/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/base_framework/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1858 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/base_framework/client_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1123 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/base_framework/central_worker.py
+-rw-r--r--   0 runner     (501) staff       (20)     1147 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/base_framework/algorithm_api.py
+-rw-r--r--   0 runner     (501) staff       (20)      438 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/base_framework/client_worker.py
+-rw-r--r--   0 runner     (501) staff       (20)     2266 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/base_framework/central_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/
+-rw-r--r--   0 runner     (501) staff       (20)     1015 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     3409 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/MyModelTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4903 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/AsyncFedAvgServerManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     3324 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/my_model_trainer_nwp.py
+-rw-r--r--   0 runner     (501) staff       (20)     3531 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/AsyncFedAvgClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2222 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/AsyncFedAVGTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     3863 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/AsyncFedAvgSeqAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)     7993 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/AsyncFedAVGAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     4779 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/my_model_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     4164 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/my_model_trainer_tag_prediction.py
+-rw-r--r--   0 runner     (501) staff       (20)     3274 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/my_model_trainer_classification.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedavg_seq/
+-rw-r--r--   0 runner     (501) staff       (20)     5488 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedavg_seq/FedAvgClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1015 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedavg_seq/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedavg_seq/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3489 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedavg_seq/FedAvgSeqAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)    13844 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedavg_seq/FedAVGAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedavg_seq/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     3079 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedavg_seq/FedAVGTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     5954 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedavg_seq/FedAvgServerManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     3284 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedavg_seq/my_model_trainer_classification.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/mpi/decentralized_framework/
+-rw-r--r--   0 runner     (501) staff       (20)      386 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/decentralized_framework/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/decentralized_framework/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1112 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/decentralized_framework/decentralized_worker.py
+-rw-r--r--   0 runner     (501) staff       (20)     2374 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/decentralized_framework/decentralized_worker_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)      738 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/decentralized_framework/algorithm_api.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/mpi/classical_vertical_fl/
+-rw-r--r--   0 runner     (501) staff       (20)      504 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/classical_vertical_fl/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     7074 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/classical_vertical_fl/guest_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/classical_vertical_fl/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2198 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/classical_vertical_fl/guest_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1801 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/classical_vertical_fl/vfl_api.py
+-rw-r--r--   0 runner     (501) staff       (20)     3470 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/classical_vertical_fl/host_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     1842 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/classical_vertical_fl/host_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/mpi/fednas/
+-rw-r--r--   0 runner     (501) staff       (20)    11022 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fednas/FedNASAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     3767 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fednas/FedNASClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)     2295 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fednas/FedNASAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)    10792 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fednas/FedNASTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)      693 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fednas/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fednas/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4146 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fednas/FedNASServerManager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/mpi/fednova/
+-rw-r--r--   0 runner     (501) staff       (20)     3490 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fednova/FedNovaAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)     1015 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fednova/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     5687 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fednova/FedNovaServerManager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fednova/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3309 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fednova/FedNovaTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fednova/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     4893 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fednova/FedNovaClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)    10695 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fednova/FedNovaAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     3306 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fednova/my_model_trainer_classification.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedopt/
+-rw-r--r--   0 runner     (501) staff       (20)     8893 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedopt/FedOptAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)      578 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedopt/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     2663 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedopt/FedOptClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedopt/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1830 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedopt/optrepo.py
+-rw-r--r--   0 runner     (501) staff       (20)     3297 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedopt/FedOptAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedopt/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     1307 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedopt/FedOptTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     4470 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedopt/FedOptServerManager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedopt_seq/
+-rw-r--r--   0 runner     (501) staff       (20)     3300 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedopt_seq/FedOptSeqAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)    12025 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedopt_seq/FedOptAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1009 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedopt_seq/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     4464 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedopt_seq/FedOptClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedopt_seq/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1830 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedopt_seq/optrepo.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedopt_seq/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     1307 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedopt_seq/FedOptTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     5535 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedopt_seq/FedOptServerManager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedseg/
+-rw-r--r--   0 runner     (501) staff       (20)     3507 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedseg/FedSegClientManager.py
+-rw-r--r--   0 runner     (501) staff       (20)      716 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedseg/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     1927 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedseg/FedSegTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     6138 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedseg/MyModelTrainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedseg/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    12406 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedseg/FedSegAggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)    10700 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedseg/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2448 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedseg/FedSegAPI.py
+-rw-r--r--   0 runner     (501) staff       (20)     4172 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/mpi/fedseg/FedSegServerManager.py
+-rw-r--r--   0 runner     (501) staff       (20)      205 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     9847 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/simulation/simulator.py
+-rw-r--r--   0 runner     (501) staff       (20)    14960 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/utils/
+-rw-r--r--   0 runner     (501) staff       (20)    10317 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/utils/model_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)      735 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/utils/logging.py
+-rw-r--r--   0 runner     (501) staff       (20)    10524 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/utils/compression.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/utils/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      809 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/utils/context.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cli/
+-rwxr-xr-x   0 runner     (501) staff       (20)      313 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/cli_utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cli/edge_deployment/
+-rwxr-xr-x   0 runner     (501) staff       (20)    17332 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/edge_deployment/client_data_interface.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    11014 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/edge_deployment/client_login.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2263 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/edge_deployment/client_daemon.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/edge_deployment/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     5644 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/edge_deployment/docker_login.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    53261 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/edge_deployment/client_runner.py
+-rw-r--r--   0 runner     (501) staff       (20)    19884 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/edge_deployment/client_constants.py
+-rw-r--r--   0 runner     (501) staff       (20)    10779 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/edge_deployment/client_diagnosis.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2846 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/edge_deployment/client_api.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3126 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/edge_deployment/simulator_daemon.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cli/model_deployment/
+-rwxr-xr-x   0 runner     (501) staff       (20)     5828 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_model_inference.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2317 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_client_daemon.py
+-rw-r--r--   0 runner     (501) staff       (20)     8771 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/modelops_configs.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1983 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_server_api.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    75936 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_server_runner.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    25678 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_model_cards.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1983 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_client_api.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     5417 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/docker_client_login.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    16456 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_server_login.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    18262 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_model_cache.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    40907 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_model_deployment.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      816 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_server_data_interface.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1766 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_model_object.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    26762 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_model_db.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     6311 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_login_entry.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    14992 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_client_data_interface.py
+-rw-r--r--   0 runner     (501) staff       (20)    22536 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_server_constants.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     8362 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_model_monitor.py
+-rw-r--r--   0 runner     (501) staff       (20)    28986 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_client_constants.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    47255 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_client_runner.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     5442 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/docker_server_login.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2979 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_server_daemon.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     6722 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_client_login.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2766 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_model_msg_object.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2906 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/model_deployment/device_model_inference_entry.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cli/env/
+-rw-r--r--   0 runner     (501) staff       (20)     3453 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/env/collect_env.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/env/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    45651 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/cli.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cli/build-package/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/build-package/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-server/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1253 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/fedml_config.yaml
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/torch_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      629 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/fedml.yaml
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-server/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-client/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1253 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/fedml_config.yaml
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       76 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/torch_client.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      650 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/fedml.yaml
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-client/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cli/comm_utils/
+-rw-r--r--   0 runner     (501) staff       (20)    25267 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/comm_utils/sys_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/comm_utils/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      295 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/comm_utils/yaml_utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cli/server_deployment/
+-rwxr-xr-x   0 runner     (501) staff       (20)      749 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/server_deployment/server_data_interface.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    71302 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/server_deployment/server_runner.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/server_deployment/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2848 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/server_deployment/job_manager.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     5677 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/server_deployment/docker_login.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1971 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/server_deployment/server_api.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    10533 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/server_deployment/app_manager.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2519 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/server_deployment/server_daemon.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cli/server_deployment/templates/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/server_deployment/templates/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      404 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/server_deployment/templates/fedml-aggregator-data-pv.yaml
+-rw-r--r--   0 runner     (501) staff       (20)      279 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/server_deployment/templates/fedml-aggregator-data-pvc.yaml
+-rw-r--r--   0 runner     (501) staff       (20)      275 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/server_deployment/templates/fedml-server-svc.yaml
+-rw-r--r--   0 runner     (501) staff       (20)     1370 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/server_deployment/templates/fedml-server-deployment.yaml
+-rwxr-xr-x   0 runner     (501) staff       (20)    13871 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/server_deployment/server_login.py
+-rw-r--r--   0 runner     (501) staff       (20)    18216 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cli/server_deployment/server_constants.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cheetah/
+-rw-r--r--   0 runner     (501) staff       (20)      153 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cheetah/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cheetah/server/
+-rw-r--r--   0 runner     (501) staff       (20)     2212 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cheetah/server/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cheetah/server/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    15366 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cheetah/server/fedml_server_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)    11613 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cheetah/server/fedml_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1056 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cheetah/server/server_initializer.py
+-rw-r--r--   0 runner     (501) staff       (20)     1939 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cheetah/fedml_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     2047 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cheetah/fedml_server.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/cheetah/client/
+-rw-r--r--   0 runner     (501) staff       (20)     2266 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cheetah/client/client_initializer.py
+-rw-r--r--   0 runner     (501) staff       (20)     5161 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cheetah/client/client_launcher.py
+-rw-r--r--   0 runner     (501) staff       (20)     2673 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cheetah/client/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)     2680 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cheetah/client/fedml_trainer_dist_adapter.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cheetah/client/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1655 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cheetah/client/fedml_client_slave_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1258 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cheetah/client/process_group_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)      677 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cheetah/client/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     7549 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cheetah/client/fedml_client_master_manager.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3563 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/cheetah/client/fedml_trainer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/ml/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/ml/aggregator/
+-rw-r--r--   0 runner     (501) staff       (20)      548 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/aggregator/aggregator_creator.py
+-rw-r--r--   0 runner     (501) staff       (20)     2488 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/aggregator/my_server_aggregator_nwp.py
+-rw-r--r--   0 runner     (501) staff       (20)     4187 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/aggregator/default_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/aggregator/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5621 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/aggregator/my_server_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     2408 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/aggregator/my_server_aggregator_classification.py
+-rw-r--r--   0 runner     (501) staff       (20)    10546 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/aggregator/agg_operator.py
+-rw-r--r--   0 runner     (501) staff       (20)     3388 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/aggregator/my_server_aggregator_prediction.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/ml/engine/
+-rw-r--r--   0 runner     (501) staff       (20)    11333 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/engine/ml_engine_adapter.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/engine/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1345 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/engine/torch_process_group_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/ml/trainer/
+-rw-r--r--   0 runner     (501) staff       (20)     3953 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/trainer/scaffold_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)      580 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/trainer/trainer_creator.py
+-rw-r--r--   0 runner     (501) staff       (20)     9496 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/trainer/fednova_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/trainer/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/trainer/local_optimizer.py
+-rw-r--r--   0 runner     (501) staff       (20)     5923 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/trainer/fedprox_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     3578 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/trainer/my_model_trainer_nwp.py
+-rw-r--r--   0 runner     (501) staff       (20)     6857 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/trainer/feddyn_trainer copy.py
+-rw-r--r--   0 runner     (501) staff       (20)     5180 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/trainer/feddyn_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     5063 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/trainer/my_model_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     6274 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/trainer/mime_trainer.py
+-rw-r--r--   0 runner     (501) staff       (20)     4026 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/trainer/my_model_trainer_tag_prediction.py
+-rw-r--r--   0 runner     (501) staff       (20)     5805 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/ml/trainer/my_model_trainer_classification.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/model/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/model/linear/
+-rw-r--r--   0 runner     (501) staff       (20)      433 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/linear/lr.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/linear/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      544 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/linear/lr_cifar10.py
+-rw-r--r--   0 runner     (501) staff       (20)       52 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4549 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/model_hub.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/model/mobile/
+-rw-r--r--   0 runner     (501) staff       (20)      988 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/mobile/mnn_lenet.py
+-rw-r--r--   0 runner     (501) staff       (20)     3860 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/mobile/mnn_resnet.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/mobile/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      774 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/mobile/torch_lenet.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/model/nlp/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/nlp/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6272 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/nlp/model_args.py
+-rw-r--r--   0 runner     (501) staff       (20)     4687 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/nlp/rnn.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/model/finance/
+-rw-r--r--   0 runner     (501) staff       (20)      458 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/finance/vfl_feature_extractor.py
+-rw-r--r--   0 runner     (501) staff       (20)     2385 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/finance/vfl_models_standalone.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/finance/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      354 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/finance/vfl_classifier.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/model/cv/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/model/cv/resnet56/
+-rw-r--r--   0 runner     (501) staff       (20)     9541 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/resnet56/resnet_pretrained.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/resnet56/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     8241 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/resnet56/resnet_server.py
+-rw-r--r--   0 runner     (501) staff       (20)     9507 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/resnet56/resnet_client.py
+-rw-r--r--   0 runner     (501) staff       (20)     6216 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/vgg.py
+-rw-r--r--   0 runner     (501) staff       (20)      455 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/test_cnn.py
+-rw-r--r--   0 runner     (501) staff       (20)    16186 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/resnet_torch.py
+-rw-r--r--   0 runner     (501) staff       (20)    25891 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/efficientnet_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     7751 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/resnet_cifar.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    10352 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/mobilenet_v3.py
+-rw-r--r--   0 runner     (501) staff       (20)    19954 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/batchnorm_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     7629 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/cnn.py
+-rw-r--r--   0 runner     (501) staff       (20)     1590 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/mnist_gan.py
+-rw-r--r--   0 runner     (501) staff       (20)    17984 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/efficientnet.py
+-rw-r--r--   0 runner     (501) staff       (20)    25096 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/resnet_all.py
+-rw-r--r--   0 runner     (501) staff       (20)     4593 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/mobilenet.py
+-rw-r--r--   0 runner     (501) staff       (20)    74592 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/common.py
+-rw-r--r--   0 runner     (501) staff       (20)    10274 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/resnet.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/model/cv/darts/
+-rw-r--r--   0 runner     (501) staff       (20)     7088 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/darts/model_search_gdas.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/darts/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1713 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/darts/visualize.py
+-rw-r--r--   0 runner     (501) staff       (20)    18693 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/darts/architect.py
+-rw-r--r--   0 runner     (501) staff       (20)     7681 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/darts/model.py
+-rw-r--r--   0 runner     (501) staff       (20)     4504 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/darts/operations.py
+-rw-r--r--   0 runner     (501) staff       (20)     3268 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/darts/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)    12302 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/darts/model_search.py
+-rw-r--r--   0 runner     (501) staff       (20)     8673 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/darts/train.py
+-rw-r--r--   0 runner     (501) staff       (20)     3486 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/darts/genotypes.py
+-rw-r--r--   0 runner     (501) staff       (20)    14555 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/darts/train_search.py
+-rw-r--r--   0 runner     (501) staff       (20)     7625 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/resnet_gn.py
+-rw-r--r--   0 runner     (501) staff       (20)     5343 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/model/cv/group_normalization.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/device/
+-rw-r--r--   0 runner     (501) staff       (20)     2833 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/device/gpu_mapping_cross_silo.py
+-rw-r--r--   0 runner     (501) staff       (20)     3632 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/device/gpu_mapping_mpi.py
+-rw-r--r--   0 runner     (501) staff       (20)     5611 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/device/device.py
+-rw-r--r--   0 runner     (501) staff       (20)      112 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/device/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      346 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/device/ip_config_utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/fa/
+-rw-r--r--   0 runner     (501) staff       (20)     1737 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/runner.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/fa/cross_silo/
+-rw-r--r--   0 runner     (501) staff       (20)      673 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/cross_silo/fa_server.py
+-rw-r--r--   0 runner     (501) staff       (20)      644 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/cross_silo/fa_client.py
+-rw-r--r--   0 runner     (501) staff       (20)      186 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/cross_silo/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/fa/cross_silo/server/
+-rw-r--r--   0 runner     (501) staff       (20)     2224 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/cross_silo/server/message_define.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/cross_silo/server/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    11189 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/cross_silo/server/fedml_server_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     5262 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/cross_silo/server/fedml_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)      879 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/cross_silo/server/server_initializer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/fa/cross_silo/client/
+-rw-r--r--   0 runner     (501) staff       (20)     1526 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/cross_silo/client/client_initializer.py
+-rw-r--r--   0 runner     (501) staff       (20)      809 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/cross_silo/client/client_launcher.py
+-rw-r--r--   0 runner     (501) staff       (20)     2714 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/cross_silo/client/message_define.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2051 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/cross_silo/client/fa_local_analyzer.py
+-rw-r--r--   0 runner     (501) staff       (20)     2050 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/cross_silo/client/fedml_trainer_dist_adapter.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/cross_silo/client/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1655 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/cross_silo/client/fedml_client_slave_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     1258 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/cross_silo/client/process_group_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     6118 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/cross_silo/client/fedml_client_master_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/fa/aggregator/
+-rw-r--r--   0 runner     (501) staff       (20)     1903 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/aggregator/frequency_estimation_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1885 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/aggregator/intersection_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1559 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/aggregator/union_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     2114 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/aggregator/avg_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     3908 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/aggregator/k_percentile_element_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/aggregator/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4005 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/aggregator/heavy_hitter_triehh_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1401 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/aggregator/global_analyzer_creator.py
+-rw-r--r--   0 runner     (501) staff       (20)      414 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/constants.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/fa/simulation/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/fa/simulation/sp/
+-rw-r--r--   0 runner     (501) staff       (20)     1192 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/simulation/sp/client.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/simulation/sp/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3449 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/simulation/sp/simulator.py
+-rw-r--r--   0 runner     (501) staff       (20)      119 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/simulation/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      606 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/simulation/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2832 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/fa/utils/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/utils/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     7789 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/utils/trie.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/fa/local_analyzer/
+-rw-r--r--   0 runner     (501) staff       (20)     1599 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/local_analyzer/heavy_hitter_triehh.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/local_analyzer/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      453 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/local_analyzer/frequency_estimation.py
+-rw-r--r--   0 runner     (501) staff       (20)     1413 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/local_analyzer/client_analyzer_creator.py
+-rw-r--r--   0 runner     (501) staff       (20)      392 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/local_analyzer/k_percentage_element.py
+-rw-r--r--   0 runner     (501) staff       (20)      223 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/local_analyzer/intersection.py
+-rw-r--r--   0 runner     (501) staff       (20)      217 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/local_analyzer/union.py
+-rw-r--r--   0 runner     (501) staff       (20)      362 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/local_analyzer/avg.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/fa/base_frame/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/base_frame/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      716 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/base_frame/server_aggregator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1049 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/base_frame/client_analyzer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/fa/data/
+-rw-r--r--   0 runner     (501) staff       (20)     4487 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/data/data_loader.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/fa/data/twitter_Sentiment140/
+-rw-r--r--   0 runner     (501) staff       (20)     3223 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/data/twitter_Sentiment140/twitter_data_processing.py
+-rw-r--r--   0 runner     (501) staff       (20)     1693 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/data/twitter_Sentiment140/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/data/twitter_Sentiment140/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       75 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/data/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2374 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/data/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/fa/data/self_defined_data/
+-rw-r--r--   0 runner     (501) staff       (20)      856 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/data/self_defined_data/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/data/self_defined_data/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/fa/data/fake_numeric_data/
+-rw-r--r--   0 runner     (501) staff       (20)      526 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/data/fake_numeric_data/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/fa/data/fake_numeric_data/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      545 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/launch_cross_device.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/MNIST/
+-rw-r--r--   0 runner     (501) staff       (20)     5448 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/MNIST/mnist_mobile_preprocessor.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     4945 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/MNIST/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/MNIST/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2942 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/MNIST/stats.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/lending_club_loan/
+-rw-r--r--   0 runner     (501) staff       (20)     7729 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/lending_club_loan/lending_club_dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/lending_club_loan/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2291 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/lending_club_loan/lending_club_feature_group.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/fed_cifar100/
+-rw-r--r--   0 runner     (501) staff       (20)     6320 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/fed_cifar100/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/fed_cifar100/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      517 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/fed_cifar100/dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     2631 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/fed_cifar100/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/FederatedEMNIST/
+-rw-r--r--   0 runner     (501) staff       (20)     6737 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/FederatedEMNIST/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/FederatedEMNIST/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      426 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/FederatedEMNIST/dataset.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/cifar100/
+-rw-r--r--   0 runner     (501) staff       (20)    11837 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/cifar100/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     2077 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/cifar100/datasets.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/cifar100/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    21968 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)      156 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4146 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/file_operation.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/shakespeare/
+-rwxr-xr-x   0 runner     (501) staff       (20)     3431 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/shakespeare/language_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     4135 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/shakespeare/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/shakespeare/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      335 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/shakespeare/dataset.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2942 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/shakespeare/stats.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/synthetic_1_1/
+-rw-r--r--   0 runner     (501) staff       (20)     4562 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/synthetic_1_1/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/synthetic_1_1/__init__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3210 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/synthetic_1_1/stats.py
+-rw-r--r--   0 runner     (501) staff       (20)     2749 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/synthetic_1_1/generate_synthetic.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/Landmarks/
+-rw-r--r--   0 runner     (501) staff       (20)      375 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/Landmarks/download_with_tff.py
+-rw-r--r--   0 runner     (501) staff       (20)    14871 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/Landmarks/download_without_tff.py
+-rw-r--r--   0 runner     (501) staff       (20)    11159 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/Landmarks/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     2191 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/Landmarks/datasets.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/Landmarks/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    14342 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/Landmarks/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2090 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/Landmarks/check_download.py
+-rw-r--r--   0 runner     (501) staff       (20)     7872 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/Landmarks/download_without_tf.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/fednlp/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/fednlp/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/fednlp/base/
+-rw-r--r--   0 runner     (501) staff       (20)      169 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/fednlp/base/globals.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/fednlp/base/preprocess/
+-rw-r--r--   0 runner     (501) staff       (20)     4794 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/fednlp/base/preprocess/base_example.py
+-rw-r--r--   0 runner     (501) staff       (20)      363 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/fednlp/base/preprocess/base_data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/fednlp/base/preprocess/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      224 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/fednlp/base/preprocess/base_preprocessor.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/fednlp/base/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/fednlp/base/raw_data/
+-rw-r--r--   0 runner     (501) staff       (20)     1428 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/fednlp/base/raw_data/partition.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/fednlp/base/raw_data/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3636 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/fednlp/base/raw_data/base_raw_data_loader.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/fednlp/base/data_manager/
+-rw-r--r--   0 runner     (501) staff       (20)    16505 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/fednlp/base/data_manager/base_data_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/fednlp/base/data_manager/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     8248 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/fednlp/base/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/NUS_WIDE/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/NUS_WIDE/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    11281 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/NUS_WIDE/nus_wide_dataset.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/stackoverflow_lr/
+-rw-r--r--   0 runner     (501) staff       (20)     8487 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/stackoverflow_lr/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/stackoverflow_lr/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2841 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/stackoverflow_lr/dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     4272 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/stackoverflow_lr/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/fed_shakespeare/
+-rw-r--r--   0 runner     (501) staff       (20)     6100 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/fed_shakespeare/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/fed_shakespeare/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3633 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/fed_shakespeare/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/ImageNet/
+-rw-r--r--   0 runner     (501) staff       (20)    11416 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/ImageNet/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     6718 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/ImageNet/datasets.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/ImageNet/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5874 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/ImageNet/datasets_hdf5.py
+-rw-r--r--   0 runner     (501) staff       (20)     1429 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/data_loader_cross_silo.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/cinic10/
+-rw-r--r--   0 runner     (501) staff       (20)    13807 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/cinic10/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     3071 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/cinic10/datasets.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/cinic10/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/stackoverflow_nwp/
+-rw-r--r--   0 runner     (501) staff       (20)     7023 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/stackoverflow_nwp/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/stackoverflow_nwp/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2171 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/stackoverflow_nwp/dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     2508 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/stackoverflow_nwp/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/UCI/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/UCI/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6215 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/UCI/data_loader_for_susy_and_ro.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/edge_case_examples/
+-rw-r--r--   0 runner     (501) staff       (20)    44697 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/edge_case_examples/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)    20285 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/edge_case_examples/datasets.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/edge_case_examples/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml/data/cifar10/
+-rw-r--r--   0 runner     (501) staff       (20)    13696 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/cifar10/efficient_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)    11902 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/cifar10/data_loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     2378 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/cifar10/datasets.py
+-rw-r--r--   0 runner     (501) staff       (20)     3972 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/cifar10/without_reload.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-24 12:02:36.000000 fedml-0.8.5a1/fedml/data/cifar10/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-24 12:02:55.000000 fedml-0.8.5a1/fedml.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     3806 2023-06-24 12:02:54.000000 fedml-0.8.5a1/fedml.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    48148 2023-06-24 12:02:54.000000 fedml-0.8.5a1/fedml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)       45 2023-06-24 12:02:54.000000 fedml-0.8.5a1/fedml.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)      546 2023-06-24 12:02:54.000000 fedml-0.8.5a1/fedml.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       21 2023-06-24 12:02:54.000000 fedml-0.8.5a1/fedml.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-06-24 12:02:54.000000 fedml-0.8.5a1/fedml.egg-info/dependency_links.txt
```

### Comparing `fedml-0.8.4a9/PKG-INFO` & `fedml-0.8.5a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedml
-Version: 0.8.4a9
+Version: 0.8.5a1
 Summary: A research and production integrated edge-cloud library for federated/distributed machine learning at anywhere at any scale.
 Home-page: https://github.com/FedML-AI/FedML
 Author: FedML Team
 Author-email: ch@fedml.ai
 License: Apache 2.0
 Description: # FedML - The community building and connecting AI anywhere at any scale
```

### Comparing `fedml-0.8.4a9/tests/security/attack/test_backdoor.py` & `fedml-0.8.5a1/tests/security/attack/test_backdoor.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/tests/security/attack/test_model_replacement_backdoor_attack.py` & `fedml-0.8.5a1/tests/security/attack/test_model_replacement_backdoor_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/tests/security/attack/test_invertgradient.py` & `fedml-0.8.5a1/tests/security/attack/test_invertgradient.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/tests/security/attack/test_byzantine_attack.py` & `fedml-0.8.5a1/tests/security/attack/test_byzantine_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/tests/security/attack/utils.py` & `fedml-0.8.5a1/tests/security/attack/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/tests/security/attack/test_edge_case_backdoor_attack.py` & `fedml-0.8.5a1/tests/security/attack/test_edge_case_backdoor_attack.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+import os.path
+from os.path import expanduser
+
 import torch
 from torch.utils.data import TensorDataset
 from fedml.core.security.attack.edge_case_backdoor_attack import EdgeCaseBackdoorAttack
 from fedml.core.security.common.attack_defense_data_loader import AttackDefenseDataLoader
 
 
 def test_attack_cifar10():
     client_num = 10
     attack_client_num = 5
     batch_size = 32
-    dataset = AttackDefenseDataLoader.load_cifar10_data(client_num=client_num, batch_size=batch_size)
+    data_dir = os.path.join(expanduser("~"), "fedml_data", "cifar10")
+    dataset = AttackDefenseDataLoader.load_cifar10_data(data_dir=data_dir, client_num=client_num, batch_size=batch_size)
     backdoor_data = torch.rand(784, 3, 32, 32)
     backdoor_target = torch.randint(10, (784,))
     backdoor_dataset = TensorDataset(backdoor_data, backdoor_target)
     edge_case_backdoor_attack = EdgeCaseBackdoorAttack(
         client_num=client_num,
         poisoned_client_num=attack_client_num,
         backdoor_sample_percentage=0.1,
```

### Comparing `fedml-0.8.4a9/tests/security/attack/test_dlg.py` & `fedml-0.8.5a1/tests/security/attack/test_dlg.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/tests/security/defense/test_residual_based_reweighting.py` & `fedml-0.8.5a1/tests/security/defense/test_residual_based_reweighting.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/tests/security/defense/test_wbc.py` & `fedml-0.8.5a1/tests/security/defense/test_wbc.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/tests/security/defense/test_crfl.py` & `fedml-0.8.5a1/tests/security/defense/test_crfl.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/tests/security/defense/test_geometric_median.py` & `fedml-0.8.5a1/tests/security/defense/test_geometric_median.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     return GeometricMedianDefense(config)
 
 
 def test_defense():
     print("-----test defense-----")
     gm = _get_geometric_median_obj()
     model_list = create_fake_model_list(gm.client_num_per_round)
-    res = gm.run(model_list)
+    res = gm.defend_on_aggregation(model_list)
     print(f"aggregation result = {res}")
 
 
 def test__compute_middle_point():
     alphas = [0.5, 0.5]
     batch_w = [
         torch.FloatTensor([[1, 0, 1], [2, 2, 2], [1, 1, 1]]),
```

### Comparing `fedml-0.8.4a9/tests/security/defense/test_slsgd_defense.py` & `fedml-0.8.5a1/tests/security/defense/test_slsgd_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/tests/security/defense/test_weak_dp.py` & `fedml-0.8.5a1/tests/security/defense/test_weak_dp.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/tests/security/defense/test_norm_diff_clipping.py` & `fedml-0.8.5a1/tests/security/defense/test_norm_diff_clipping.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/tests/security/defense/utils.py` & `fedml-0.8.5a1/tests/security/defense/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/tests/security/defense/test_bulyan.py` & `fedml-0.8.5a1/tests/security/defense/test_bulyan.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/tests/security/defense/test_robust_learning_rate_defense.py` & `fedml-0.8.5a1/tests/security/defense/test_robust_learning_rate_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/tests/security/defense/test_coordinate_wise_trimmed_mean.py` & `fedml-0.8.5a1/tests/security/defense/test_coordinate_wise_trimmed_mean.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/tests/security/defense/test_krum.py` & `fedml-0.8.5a1/tests/security/defense/test_krum.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/tests/security/defense/test_cclip.py` & `fedml-0.8.5a1/tests/security/defense/test_foolsgold_defense.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import argparse
-from fedml.core.security.defense.cclip_defense import CClipDefense
-from fedml.ml.aggregator.agg_operator import FedMLAggOperator
-from tests.security.defense.utils import create_fake_model_list
+import torch
+from fedml.core.security.defense.foolsgold_defense import FoolsGoldDefense
 
 
 def add_args():
     parser = argparse.ArgumentParser(description="FedML")
     parser.add_argument(
-        "--yaml_config_file", "--cf", help="yaml configuration file", type=str, default="",
+        "--yaml_config_file",
+        "--cf",
+        help="yaml configuration file",
+        type=str,
+        default="",
     )
-
-    # default arguments
     parser.add_argument("--federated_optimizer", type=str, default="FedAvg")
-    parser.add_argument("--tau", type=int, default=10)
-    parser.add_argument("--bucket_size", type=int, default=3)
     args, unknown = parser.parse_known_args()
     return args
 
 
 def test_defense():
     config = add_args()
-    client_grad_list = create_fake_model_list(20)
-    defense = CClipDefense(config)
-    result = defense.run(client_grad_list, base_aggregation_func=FedMLAggOperator.agg)
-    print(f"result = {result}")
+    model = torch.hub.load("pytorch/vision:v0.10.0", "vgg11", pretrained=True).state_dict()
+    model_list = [(100, model) for i in range(4)]
+
+    print(f"model_list len = {len(model_list)}")
+    defense = FoolsGoldDefense(config)
+    aggr_result = defense.defend_before_aggregation(model_list)
+    # print(f"result = {aggr_result}")
 
 
 if __name__ == "__main__":
     test_defense()
```

### Comparing `fedml-0.8.4a9/tests/security/defense/test_soteria.py` & `fedml-0.8.5a1/tests/security/defense/test_soteria.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/README.md` & `fedml-0.8.5a1/README.md`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/setup.py` & `fedml-0.8.5a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,29 +25,27 @@
     "h5py",
     "tqdm",
     "wget",
     "paho-mqtt",
     "boto3",
     "pynvml",
     "scikit-learn",
-    "networkx",
+    "networkx<3.0",
     "click",
     "torch>=1.13.1",
     "torchvision>=0.14.1",
     "spacy",
     "gensim",
     "multiprocess",
     "smart-open==6.3.0",
     "nvidia-ml-py3",
     "matplotlib",
     "dill",
     "pandas",
     "wandb==0.13.2",
-    "eciespy",
-    "PyNaCl",
     "httpx",
     "attrs",
     "fastapi==0.92.0",
     "uvicorn",
     "geventhttpclient>=1.4.4,<=2.0.9",
     "aiohttp>=3.8.1",
     "python-rapidjson>=0.9.1",
@@ -68,32 +66,35 @@
 requirements_extra_tf = [
     "tensorflow",
     "tensorflow_datasets",
     "tensorflow_federated",
 ]
 
 requirements_extra_jax = [
-    "jax[cpu]",
-    "dm-haiku",
-    "optax",
-    "jaxlib"
+
+
 ]
 
 # https://github.com/apache/incubator-mxnet/issues/18329
 requirements_extra_mxnet = [
     "mxnet==2.0.0b1"
 ]
 
+requirements_extra_crypto = [
+    "eciespy",
+    "PyNaCl"
+]
+
 
 # if platform.machine() == "x86_64":
 #    requirements.append("MNN==1.1.6")
 
 setup(
     name="fedml",
-    version="0.8.4a9",
+    version="0.8.5a1",
     author="FedML Team",
     author_email="ch@fedml.ai",
     description="A research and production integrated edge-cloud library for "
                 "federated/distributed machine learning at anywhere at any scale.",
     long_description=io.open(os.path.join("README.md"), "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/FedML-AI/FedML",
```

### Comparing `fedml-0.8.4a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py` & `fedml-0.8.5a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py` & `fedml-0.8.5a1/examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py` & `fedml-0.8.5a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py` & `fedml-0.8.5a1/examples/cross_silo/mqtt_web3storage_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py` & `fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py` & `fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_trainer_classification.py` & `fedml-0.8.5a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_trainer_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_aggregator.py` & `fedml-0.8.5a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_server.py` & `fedml-0.8.5a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_client.py` & `fedml-0.8.5a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model.py` & `fedml-0.8.5a1/examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_client.py` & `fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_server.py` & `fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_aggregator.py` & `fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_trainer.py` & `fedml-0.8.5a1/examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_client.py` & `fedml-0.8.5a1/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_mpi.py` & `fedml-0.8.5a1/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_mpi.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_server.py` & `fedml-0.8.5a1/examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_trainer_classification.py` & `fedml-0.8.5a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_trainer_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model.py` & `fedml-0.8.5a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_aggregator.py` & `fedml-0.8.5a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_model_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_client.py` & `fedml-0.8.5a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_server.py` & `fedml-0.8.5a1/examples/cross_silo/mxnet_mqtt_s3_fedavg_mnist_lr_example/mxnet_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py` & `fedml-0.8.5a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py` & `fedml-0.8.5a1/examples/cross_silo/mqtt_thetastore_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_client.py` & `fedml-0.8.5a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_aggregator.py` & `fedml-0.8.5a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_trainer_classification.py` & `fedml-0.8.5a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_trainer_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_server.py` & `fedml-0.8.5a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model.py` & `fedml-0.8.5a1/examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/torch_client.py` & `fedml-0.8.5a1/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/torch_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def create_model():
     """
     loading pretrained model...
     please download the pre-trained weight file from
     https://github.com/FedML-AI/FedML/blob/fedml_v0.6_before_fundraising/fedml_api/model/cv/pretrained/CIFAR10/resnet56/best.pth
     and rename the file to ``resnet56_on_cifar10.pth''
     """
-    pre_trained_model_path = "./config/resnet56_on_cifar10.pth"
+    pre_trained_model_path = "config/resnet56_on_cifar10.pth"
     model = resnet56(10, pretrained=True, path=pre_trained_model_path)
     logging.info("load pretrained model successfully")
     return model
 
 
 if __name__ == "__main__":
     args = fedml.init()
```

### Comparing `fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/torch_mpi.py` & `fedml-0.8.5a1/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/torch_mpi.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def create_model():
     """
     loading pretrained model...
     please download the pre-trained weight file from
     https://github.com/FedML-AI/FedML/blob/fedml_v0.6_before_fundraising/fedml_api/model/cv/pretrained/CIFAR10/resnet56/best.pth
     and rename the file to ``resnet56_on_cifar10.pth''
     """
-    pre_trained_model_path = "./config/resnet56_on_cifar10.pth"
+    pre_trained_model_path = "config/resnet56_on_cifar10.pth"
     model = resnet56(10, pretrained=True, path=pre_trained_model_path)
     logging.info("load pretrained model successfully")
     return model
 
 
 if __name__ == "__main__":
     args = fedml.init()
```

### Comparing `fedml-0.8.4a9/examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/torch_server.py` & `fedml-0.8.5a1/examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/torch_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def create_model():
     """
     loading pretrained model...
     please download the pre-trained weight file from
     https://github.com/FedML-AI/FedML/blob/fedml_v0.6_before_fundraising/fedml_api/model/cv/pretrained/CIFAR10/resnet56/best.pth
     and rename the file to ``resnet56_on_cifar10.pth''
     """
-    pre_trained_model_path = "./config/resnet56_on_cifar10.pth"
+    pre_trained_model_path = "config/resnet56_on_cifar10.pth"
     model = resnet56(10, pretrained=True, path=pre_trained_model_path)
     logging.info("load pretrained model successfully")
     return model
 
 
 if __name__ == "__main__":
     args = fedml.init()
```

### Comparing `fedml-0.8.4a9/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/my_dataset.py` & `fedml-0.8.5a1/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/my_dataset.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/torch_server.py` & `fedml-0.8.5a1/examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/torch_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/my_dataset.py` & `fedml-0.8.5a1/examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/my_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 F = MNN.expr
 
 
 class MnistDataset(MNN.data.Dataset):
     def __init__(self, datapath, training_dataset=True):
         super(MnistDataset, self).__init__()
         self.is_training_dataset = training_dataset
-        trainset = MNIST(root=datapath, train=True, download=True)
-        testset = MNIST(root=datapath, train=False, download=True)
         if self.is_training_dataset:
+            trainset = MNIST(root=datapath, train=True, download=True)
             self.data = trainset.data / 255.0
             self.labels = trainset.targets
         else:
+            testset = MNIST(root=datapath, train=False, download=True)
             self.data = testset.data / 255.0
             self.labels = testset.targets
 
     def __getitem__(self, index):
         dv = F.const(
             self.data[index].flatten().tolist(), [1, 28, 28], F.data_format.NCHW
         )
```

### Comparing `fedml-0.8.4a9/examples/centralized/main.py` & `fedml-0.8.5a1/examples/centralized/main.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg/reddit_aggregator.py` & `fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg/reddit_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg/reddit_trainer.py` & `fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg/reddit_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg/main.py` & `fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg/main.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_seq/torch_fedavg.py` & `fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_seq/torch_fedavg.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py` & `fedml-0.8.5a1/examples/simulation/sp_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py` & `fedml-0.8.5a1/examples/simulation/sp_torch_dpfedavg_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py` & `fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_defense_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py` & `fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_attack_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py` & `fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_dp_mnist_lr_example/torch_fedavg_defense_mnist_lr_custum_data_and_model_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py` & `fedml-0.8.5a1/examples/simulation/mpi_torch_fedavg_mnist_lr_example/torch_fedavg_mnist_lr_custum_data_and_model_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/examples/simulation/mpi_torch_async_fedavg/torch_fedavg_mnist_lr_custum_data_and_model_example.py` & `fedml-0.8.5a1/examples/simulation/mpi_torch_async_fedavg/torch_fedavg_mnist_lr_custum_data_and_model_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/launch_serving.py` & `fedml-0.8.5a1/fedml/launch_serving.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/launch_cross_silo_hi.py` & `fedml-0.8.5a1/fedml/launch_cross_silo_hi.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/runner.py` & `fedml-0.8.5a1/fedml/runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import os
+from os.path import expanduser
+
 from torch import nn
 
 from .constants import (
     FEDML_TRAINING_PLATFORM_SIMULATION,
     FEDML_SIMULATION_TYPE_NCCL,
     FEDML_TRAINING_PLATFORM_CROSS_SILO,
     FEDML_TRAINING_PLATFORM_CROSS_DEVICE,
@@ -198,9 +201,21 @@
             )
         else:
             raise Exception(
                 "Wrong program path: Python package only supports mobile server!"
             )
         return runner
 
+    @staticmethod
+    def log_runner_result():
+        log_runner_result_dir = os.path.join(expanduser("~"), "fedml_trace")
+        if not os.path.exists(log_runner_result_dir):
+            os.makedirs(log_runner_result_dir)
+
+        log_file_obj = open(os.path.join(log_runner_result_dir, str(os.getpid())), "w")
+        log_file_obj.write("{}".format(str(os.getpid())))
+        log_file_obj.close()
+
     def run(self):
         self.runner.run()
+        FedMLRunner.log_runner_result()
+
```

### Comparing `fedml-0.8.4a9/fedml/cross_silo/lightsecagg/lsa_message_define.py` & `fedml-0.8.5a1/fedml/cross_silo/lightsecagg/lsa_message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_silo/lightsecagg/lsa_fedml_client_manager.py` & `fedml-0.8.5a1/fedml/cross_silo/lightsecagg/lsa_fedml_client_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_silo/lightsecagg/lsa_fedml_aggregator.py` & `fedml-0.8.5a1/fedml/cross_silo/lightsecagg/lsa_fedml_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_silo/lightsecagg/lsa_fedml_server_manager.py` & `fedml-0.8.5a1/fedml/cross_silo/lightsecagg/lsa_fedml_server_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_silo/lightsecagg/lsa_fedml_api.py` & `fedml-0.8.5a1/fedml/cross_silo/lightsecagg/lsa_fedml_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_silo/server/message_define.py` & `fedml-0.8.5a1/fedml/cross_silo/server/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_silo/server/fedml_server_manager.py` & `fedml-0.8.5a1/fedml/serving/server/fedml_server_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,16 @@
             logging.info(f"input shape: {input_shape}")  # [torch.Size([1, 24]), torch.Size([1, 2])]
             logging.info(f"input type: {input_type}")    # [torch.int64, torch.float32]
 
             # Send output input size and type (saved as json) to s3,
             # and transfer when click "Create Model Card"
             model_input_url = mlops.log_training_model_input_info(list(input_shape), list(input_type))
         except Exception as e:
-            logging.info("Cannot get dummy input size or shape for model serving")
+            logging.info("exception when processing model net and model input info: {}".format(
+                traceback.format_exc()))
 
     def register_message_receive_handlers(self):
         logging.info("register_message_receive_handlers------")
         self.register_message_receive_handler(
             MyMessage.MSG_TYPE_CONNECTION_IS_READY, self.handle_message_connection_ready
         )
```

### Comparing `fedml-0.8.4a9/fedml/cross_silo/server/fedml_aggregator.py` & `fedml-0.8.5a1/fedml/serving/server/fedml_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_silo/server/server_initializer.py` & `fedml-0.8.5a1/fedml/cross_silo/server/server_initializer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_silo/fedml_client.py` & `fedml-0.8.5a1/fedml/cross_silo/fedml_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_silo/fedml_server.py` & `fedml-0.8.5a1/fedml/cross_silo/fedml_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_silo/client/client_initializer.py` & `fedml-0.8.5a1/fedml/cross_silo/client/client_initializer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_silo/client/client_launcher.py` & `fedml-0.8.5a1/fedml/cross_silo/client/client_launcher.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_silo/client/message_define.py` & `fedml-0.8.5a1/fedml/cross_silo/client/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_silo/client/fedml_trainer_dist_adapter.py` & `fedml-0.8.5a1/fedml/cross_silo/client/fedml_trainer_dist_adapter.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_silo/client/fedml_client_slave_manager.py` & `fedml-0.8.5a1/fedml/cross_silo/client/fedml_client_slave_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_silo/client/process_group_manager.py` & `fedml-0.8.5a1/fedml/cross_silo/client/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_silo/client/utils.py` & `fedml-0.8.5a1/fedml/cross_silo/client/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_silo/client/fedml_client_master_manager.py` & `fedml-0.8.5a1/fedml/serving/client/fedml_client_master_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_silo/client/fedml_trainer.py` & `fedml-0.8.5a1/fedml/cross_silo/client/fedml_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/launch_cross_silo_horizontal.py` & `fedml-0.8.5a1/fedml/launch_cross_silo_horizontal.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/serving/server/message_define.py` & `fedml-0.8.5a1/fedml/serving/server/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/serving/server/fedml_server_manager.py` & `fedml-0.8.5a1/fedml/cheetah/server/fedml_server_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/serving/server/fedml_aggregator.py` & `fedml-0.8.5a1/fedml/cheetah/server/fedml_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/serving/server/server_initializer.py` & `fedml-0.8.5a1/fedml/serving/server/server_initializer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/serving/fedml_client.py` & `fedml-0.8.5a1/fedml/serving/fedml_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/serving/fedml_server.py` & `fedml-0.8.5a1/fedml/serving/fedml_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/serving/client/client_initializer.py` & `fedml-0.8.5a1/fedml/serving/client/client_initializer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/serving/client/client_launcher.py` & `fedml-0.8.5a1/fedml/serving/client/client_launcher.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/serving/client/message_define.py` & `fedml-0.8.5a1/fedml/serving/client/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/serving/client/fedml_trainer_dist_adapter.py` & `fedml-0.8.5a1/fedml/serving/client/fedml_trainer_dist_adapter.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/serving/client/fedml_client_slave_manager.py` & `fedml-0.8.5a1/fedml/serving/client/fedml_client_slave_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/serving/client/process_group_manager.py` & `fedml-0.8.5a1/fedml/serving/client/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/serving/client/utils.py` & `fedml-0.8.5a1/fedml/serving/client/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/serving/client/fedml_client_master_manager.py` & `fedml-0.8.5a1/fedml/cheetah/client/fedml_client_master_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/serving/client/fedml_trainer.py` & `fedml-0.8.5a1/fedml/serving/client/fedml_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/schedule/runtime_estimate.py` & `fedml-0.8.5a1/fedml/core/schedule/runtime_estimate.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/schedule/seq_train_scheduler.py` & `fedml-0.8.5a1/fedml/core/schedule/seq_train_scheduler.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/alg_frame/params.py` & `fedml-0.8.5a1/fedml/core/alg_frame/params.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/alg_frame/client_trainer.py` & `fedml-0.8.5a1/fedml/core/alg_frame/client_trainer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from abc import ABC, abstractmethod
-
+from ..security.fedml_attacker import FedMLAttacker
 from ...core.dp.fedml_differential_privacy import FedMLDifferentialPrivacy
 
 
 class ClientTrainer(ABC):
     """Abstract base class for federated learning trainer.
     1. The goal of this abstract class is to be compatible to
     any deep learning frameworks such as PyTorch, TensorFlow, Keras, MXNET, etc.
@@ -16,21 +16,29 @@
         self.model = model
         self.id = 0
         self.args = args
         self.local_train_dataset = None
         self.local_test_dataset = None
         self.local_sample_number = 0
         FedMLDifferentialPrivacy.get_instance().init(args)
+        FedMLAttacker.get_instance().init(args)
 
     def set_id(self, trainer_id):
         self.id = trainer_id
 
+    def is_main_process(self):
+        return True
+
     def update_dataset(self, local_train_dataset, local_test_dataset, local_sample_number):
-        self.local_train_dataset = local_train_dataset
-        self.local_test_dataset = local_test_dataset
+        if FedMLAttacker.get_instance().is_data_poisoning_attack() and FedMLAttacker.get_instance().is_to_poison_data():
+            self.local_train_dataset = FedMLAttacker.get_instance().poison_data(local_train_dataset)
+            self.local_test_dataset = FedMLAttacker.get_instance().poison_data(local_test_dataset)
+        else:
+            self.local_train_dataset = local_train_dataset
+            self.local_test_dataset = local_test_dataset
         self.local_sample_number = local_sample_number
 
     @abstractmethod
     def get_model_params(self):
         pass
 
     @abstractmethod
```

### Comparing `fedml-0.8.4a9/fedml/core/alg_frame/context.py` & `fedml-0.8.5a1/fedml/core/alg_frame/context.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/alg_frame/server_aggregator.py` & `fedml-0.8.5a1/fedml/core/alg_frame/server_aggregator.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,17 @@
         FedMLDefender.get_instance().init(args)
         FedMLDifferentialPrivacy.get_instance().init(args)
         self.contribution_assessor_mgr = ContributionAssessorManager(args)
         self.final_contribution_assigment_dict = dict()
 
         self.eval_data = None
 
+    def is_main_process(self):
+        return True
+
     def set_id(self, aggregator_id):
         self.id = aggregator_id
 
     @abstractmethod
     def get_model_params(self):
         pass
 
@@ -37,15 +40,15 @@
         pass
 
     def on_before_aggregation(
             self, raw_client_model_or_grad_list: List[Tuple[float, OrderedDict]]
     ):
         if FedMLDifferentialPrivacy.get_instance().is_global_dp_enabled() and FedMLDifferentialPrivacy.get_instance().is_clipping():
             raw_client_model_or_grad_list = FedMLDifferentialPrivacy.get_instance().global_clip(raw_client_model_or_grad_list)
-        if FedMLAttacker.get_instance().is_reconstruct_data_attack():
+        if FedMLAttacker.get_instance().is_data_reconstruction_attack():
             FedMLAttacker.get_instance().reconstruct_data(
                 raw_client_grad_list=raw_client_model_or_grad_list,
                 extra_auxiliary_info=self.get_model_params(),
             )
         if FedMLAttacker.get_instance().is_model_attack():
             raw_client_model_or_grad_list = FedMLAttacker.get_instance().attack_model(
                 raw_client_grad_list=raw_client_model_or_grad_list,
```

### Comparing `fedml-0.8.4a9/fedml/core/distributed/topology/asymmetric_topology_manager.py` & `fedml-0.8.5a1/fedml/core/distributed/topology/asymmetric_topology_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/topology/symmetric_topology_manager.py` & `fedml-0.8.5a1/fedml/core/distributed/topology/symmetric_topology_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/crypto/crypto_api.py` & `fedml-0.8.5a1/fedml/core/distributed/crypto/crypto_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/fedml_comm_manager.py` & `fedml-0.8.5a1/fedml/core/distributed/fedml_comm_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/communication/s3/remote_storage_mnn.py` & `fedml-0.8.5a1/fedml/core/distributed/communication/s3/remote_storage_mnn.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/communication/s3/remote_storage.py` & `fedml-0.8.5a1/fedml/core/distributed/communication/s3/remote_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import io
 import json
 import logging
 import os
 import pickle
 import time
+import uuid
+from os.path import expanduser
 
 import boto3
 # for multi-processing, we need to create a global variable for AWS S3 client:
 # https://www.pythonforthelab.com/blog/differences-between-multiprocessing-windows-and-linux/
 # https://stackoverflow.com/questions/72313845/multiprocessing-picklingerror-cant-pickle-class-botocore-client-s3-attr
 import dill
 import torch
@@ -90,15 +92,18 @@
         global aws_s3_client
         pickle_dump_start_time = time.time()
         MLOpsProfilerEvent.log_to_wandb(
             {"PickleDumpsTime": time.time() - pickle_dump_start_time}
         )
 
         if not os.path.exists(local_model_cache_path):
-            os.makedirs(local_model_cache_path)
+            try:
+                os.makedirs(local_model_cache_path)
+            except Exception as e:
+                pass
         write_model_path = os.path.join(local_model_cache_path, message_key)
         try:
             model.eval()
             jit_model = torch.jit.trace(model, dummy_input_tensor)
             jit_model.save(write_model_path)
         except Exception as e:
             logging.info("jit.save failed")
@@ -140,15 +145,18 @@
         )
         return model_url
 
     def write_model_input(self, message_key, input_size, input_type, local_model_cache_path):
         global aws_s3_client
 
         if not os.path.exists(local_model_cache_path):
-            os.makedirs(local_model_cache_path)
+            try:
+                os.makedirs(local_model_cache_path)
+            except Exception as e:
+                pass
         model_input_path = os.path.join(local_model_cache_path, message_key)
         model_input_dict = {"input_size": input_size, "input_type": input_type}
         with open(model_input_path, "w") as f:
             json.dump(model_input_dict, f)
 
         with open(model_input_path, 'rb') as f:
             aws_s3_client.upload_fileobj(f, Bucket=self.bucket_name, Key=message_key)
@@ -184,17 +192,27 @@
 
     def read_model(self, message_key):
         global aws_s3_client
         message_handler_start_time = time.time()
 
         kwargs = {"Bucket": self.bucket_name, "Key": message_key}
         object_size = aws_s3_client.head_object(**kwargs)["ContentLength"]
-        temp_base_file_path = './cache/S3_DOWNLOADED_MODEL' + "_P" + str(os.getpid())
+        cache_dir = os.path.join(expanduser("~"), "fedml_cache")
+        if not os.path.exists(cache_dir):
+            try:
+                os.makedirs(cache_dir)
+            except Exception as e:
+                pass
+        temp_base_file_path = os.path.join(cache_dir, str(os.getpid()) + "@" + str(uuid.uuid4()))
         if not os.path.exists(temp_base_file_path):
-            os.makedirs(temp_base_file_path)
+            try:
+                os.makedirs(temp_base_file_path)
+            except Exception as e:
+                pass
+
         temp_file_path = temp_base_file_path + "/" + str(message_key)
         logging.info("temp_file_path = {}".format(temp_file_path))
         model_file_transfered = 0
         prev_progress = 0
         def read_model_progress(bytes_transferred):
             nonlocal model_file_transfered
             nonlocal object_size
@@ -229,15 +247,18 @@
         global aws_s3_client
         message_handler_start_time = time.time()
 
         kwargs = {"Bucket": self.bucket_name, "Key": message_key}
         object_size = aws_s3_client.head_object(**kwargs)["ContentLength"]
         temp_base_file_path = local_model_cache_path
         if not os.path.exists(temp_base_file_path):
-            os.makedirs(temp_base_file_path)
+            try:
+                os.makedirs(temp_base_file_path)
+            except Exception as e:
+                pass
         temp_file_path = os.path.join(temp_base_file_path, str(message_key))
         if os.path.exists(temp_file_path):
             os.remove(temp_file_path)
         logging.info("temp_file_path = {}".format(temp_file_path))
         model_file_transfered = 0
         prev_progress = 0
         def read_model_net_progress(bytes_transferred):
@@ -272,15 +293,18 @@
         return model
 
     def read_model_input(self, message_key, local_model_cache_path):
         global aws_s3_client
 
         temp_base_file_path = local_model_cache_path
         if not os.path.exists(temp_base_file_path):
-            os.makedirs(temp_base_file_path)
+            try:
+                os.makedirs(temp_base_file_path)
+            except Exception as e:
+                pass
         temp_file_path = os.path.join(temp_base_file_path, str(message_key))
         if os.path.exists(temp_file_path):
             os.remove(temp_file_path)
         logging.info("temp_file_path = {}".format(temp_file_path))
         with open(temp_file_path, 'wb') as f:
             aws_s3_client.download_fileobj(Bucket=self.bucket_name, Key=message_key, Fileobj=f)
```

### Comparing `fedml-0.8.4a9/fedml/core/distributed/communication/s3/utils.py` & `fedml-0.8.5a1/fedml/core/distributed/communication/s3/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/communication/mpi/mpi_send_thread.py` & `fedml-0.8.5a1/fedml/core/distributed/communication/mpi/mpi_send_thread.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/communication/mpi/com_manager.py` & `fedml-0.8.5a1/fedml/core/distributed/communication/mpi/com_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/communication/mpi/mpi_receive_thread.py` & `fedml-0.8.5a1/fedml/core/distributed/communication/mpi/mpi_receive_thread.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/communication/grpc/grpc_server.py` & `fedml-0.8.5a1/fedml/core/distributed/communication/grpc/grpc_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/communication/grpc/grpc_comm_manager.py` & `fedml-0.8.5a1/fedml/core/distributed/communication/grpc/grpc_comm_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2_grpc.py` & `fedml-0.8.5a1/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2.py` & `fedml-0.8.5a1/fedml/core/distributed/communication/grpc/grpc_comm_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/communication/trpc/trpc_server.py` & `fedml-0.8.5a1/fedml/core/distributed/communication/trpc/trpc_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/communication/trpc/trpc_comm_manager.py` & `fedml-0.8.5a1/fedml/core/distributed/communication/trpc/trpc_comm_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/communication/message.py` & `fedml-0.8.5a1/fedml/core/distributed/communication/message.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/communication/mqtt_web3/mqtt_web3_comm_manager.py` & `fedml-0.8.5a1/fedml/core/distributed/communication/mqtt_web3/mqtt_web3_comm_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/communication/mqtt_thetastore/mqtt_thetastore_comm_manager.py` & `fedml-0.8.5a1/fedml/core/distributed/communication/mqtt_thetastore/mqtt_thetastore_comm_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/communication/utils.py` & `fedml-0.8.5a1/fedml/core/distributed/communication/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/communication/base_com_manager.py` & `fedml-0.8.5a1/fedml/core/distributed/communication/base_com_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/communication/mqtt_s3/mqtt_s3_multi_clients_comm_manager.py` & `fedml-0.8.5a1/fedml/core/distributed/communication/mqtt_s3/mqtt_s3_multi_clients_comm_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/communication/mqtt/mqtt_manager.py` & `fedml-0.8.5a1/fedml/core/distributed/communication/mqtt/mqtt_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,16 @@
         self._client.on_disconnect = self.on_disconnect
         self._client.on_message = self.on_message
         self._client.on_subscribe = self._on_subscribe
         # self._client.on_log = self._on_log
         self._client.disable_logger()
         self._client.username_pw_set(self.user, self.pwd)
         self._client._connect_timeout = 15
-        logging.info("MQTT Connection timeout: {}, client id {}.".format(
-            self._client._connect_timeout, self.mqtt_connection_id))
+        # logging.info("MQTT Connection timeout: {}, client id {}.".format(
+        #     self._client._connect_timeout, self.mqtt_connection_id))
 
     def connect(self):
         if self.last_will_topic is not None:
             if self.last_will_msg is None:
                 self.last_will_msg = json.dumps({"ID": f"{self._client_id}", "status": "OFFLINE"})
             self._client.will_set(self.last_will_topic,
                                   payload=self.last_will_msg,
@@ -86,14 +86,17 @@
     def loop_stop(self):
         self._client.loop_stop()
 
     def loop_forever(self):
         self._client.loop_forever(retry_first_connection=True)
 
     def send_message(self, topic, message, publish_single_message=False):
+        logging.info(
+            f"FedMLDebug - Send: topic ({topic}), message ({message})"
+        )
         self.check_connection()
 
         mqtt_send_start_time = time.time()
         if publish_single_message:
             connection_id = "FEDML_SINGLE_CONN_{}_{}".format(self._client_id,
                                                              str(mqtt.base62(uuid.uuid4().int, padding=22)))
             mqtt_publish.single(topic, payload=message, qos=2,
@@ -103,14 +106,17 @@
         else:
             ret_info = self._client.publish(topic, payload=message, qos=2, retain=True)
             return ret_info.is_published()
         MLOpsProfilerEvent.log_to_wandb({"Comm/send_delay_mqtt": time.time() - mqtt_send_start_time})
         return True
 
     def send_message_json(self, topic, message, publish_single_message=False):
+        logging.info(
+            f"FedMLDebug - Send: topic ({topic}), message ({message})"
+        )
         self.check_connection()
 
         if publish_single_message:
             connection_id = "FEDML_SINGLE_CONN_{}_{}".format(self._client_id,
                                                              str(mqtt.base62(uuid.uuid4().int, padding=22)))
             mqtt_publish.single(topic, payload=message, qos=2,
                                 hostname=self._host, port=self._port,
@@ -121,15 +127,15 @@
             return ret_info.is_published()
         return True
 
     def on_connect(self, client, userdata, flags, rc):
         if rc == 0:
             client.connected_flag = True
             client.bad_conn_flag = False
-            logging.info("MQTT Connection is OK, client id {}.".format(self.mqtt_connection_id))
+            # logging.info("MQTT Connection is OK, client id {}.".format(self.mqtt_connection_id))
 
             # Callback connected listeners
             self.callback_connected_listener(client)
         else:
             client.connected_flag = False
             client.bad_conn_flag = True
 
@@ -178,15 +184,17 @@
         for passthrough_listener in self._passthrough_listeners:
             passthrough_listener(msg)
 
         _listener = self._listeners.get(msg.topic, None)
         if _listener is not None and callable(_listener):
             payload_obj = json.loads(msg.payload)
             payload_obj["is_retain"] = msg.retain
-            _listener(msg.topic, json.dumps(payload_obj))
+            payload = json.dumps(payload_obj)
+            _listener(msg.topic, payload)
+
         MLOpsProfilerEvent.log_to_wandb({"BusyTime": time.time() - message_handler_start_time})
 
     def on_publish(self, client, obj, mid):
         self.callback_published_listener(client)
 
     def on_disconnect(self, client, userdata, rc):
         client.connected_flag = False
@@ -275,25 +283,26 @@
                 listener(client)
 
     def subscribe_msg(self, topic):
         self._client.subscribe(topic, qos=2)
 
     def check_connection(self):
         count = 0
-        while not self._client.connected_flag and not self._client.bad_conn_flag:
+        while not self._client.connected_flag and self._client.bad_conn_flag:
             if count >= 30:
                 raise Exception("MQTT Connection timeout, please check your network connection!")
             logging.info("MQTT client id {}, waiting to connect to MQTT server...".format(self.mqtt_connection_id))
             time.sleep(1)
             count += 1
 
-        if self._client.bad_conn_flag:
-            logging.info("Failed to connect to MQTT server! {}".format(traceback.format_exc()))
-            self._client.loop_stop()
-            raise Exception("MQTT Connection failed, please check your network connection!")
+        if self._client.bad_conn_flag and not self.connected_flag:
+            if not self._client.is_connected():
+                logging.info("Failed to connect to MQTT server! {}".format(traceback.format_exc()))
+                self._client.loop_stop()
+                raise Exception("MQTT Connection failed, please check your network connection!")
 
 
 global received_msg_count
 received_msg_count = 0
 
 
 def test_msg_callback(topic, payload):
```

### Comparing `fedml-0.8.4a9/fedml/core/distributed/communication/mqtt_s3_mnn/mqtt_s3_comm_manager.py` & `fedml-0.8.5a1/fedml/core/distributed/communication/mqtt_s3_mnn/mqtt_s3_comm_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/distributed_storage/web3_storage/web3_storage.py` & `fedml-0.8.5a1/fedml/core/distributed/distributed_storage/web3_storage/web3_storage.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/distributed_storage/theta_storage/theta_storage.py` & `fedml-0.8.5a1/fedml/core/distributed/distributed_storage/theta_storage/theta_storage.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/flow/fedml_flow.py` & `fedml-0.8.5a1/fedml/core/distributed/flow/fedml_flow.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/flow/fedml_executor.py` & `fedml-0.8.5a1/fedml/core/distributed/flow/fedml_executor.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/distributed/flow/test_fedml_flow.py` & `fedml-0.8.5a1/fedml/core/distributed/flow/test_fedml_flow.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/attack/model_replacement_backdoor_attack.py` & `fedml-0.8.5a1/fedml/core/security/attack/model_replacement_backdoor_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/attack/edge_case_backdoor_attack.py` & `fedml-0.8.5a1/fedml/core/security/attack/edge_case_backdoor_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/attack/byzantine_attack.py` & `fedml-0.8.5a1/fedml/core/security/attack/byzantine_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/attack/lazy_worker.py` & `fedml-0.8.5a1/fedml/core/security/attack/lazy_worker.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/attack/invert_gradient_attack.py` & `fedml-0.8.5a1/fedml/core/security/attack/invert_gradient_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/attack/dlg_attack.py` & `fedml-0.8.5a1/fedml/core/security/attack/dlg_attack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import OrderedDict
-import time
+# import time
 import numpy as np
 import torch
 import torch.nn.functional as F
-from matplotlib import pyplot as plt
+# from matplotlib import pyplot as plt
 from torchvision import transforms
 from typing import List, Tuple, Any
 import fedml
 from fedml.model.cv.resnet import resnet56, resnet20
 from .attack_base import BaseAttackMethod
 from ..common.net import LeNet
 from ..common.utils import cross_entropy_for_onehot
@@ -120,18 +120,19 @@
             # print(f"dummy_data = {dummy_data}")
             # print(f"dummy_label = {dummy_label}")
             if iters % 50 == 0:
                 current_loss = closure()
                 print(iters, "%.4f" % current_loss.item())
                 history.append(tt(dummy_data[0].cpu()))
 
-        plt.figure(figsize=(12, 8))
-        for i in range(len(history)):
-            plt.subplot(3, 10, i + 1)
-            plt.imshow(history[i])
-            plt.title("iter=%d" % (i * 50))
-            plt.axis('off')
-        # plt.show()
-        filename = str(self.iteration_num) + '_' + str(round(time.time()*1000)) + '.png'
-        plt.savefig(filename)
+        # plot figures:
+        # plt.figure(figsize=(12, 8))
+        # for i in range(len(history)):
+        #     plt.subplot(3, 10, i + 1)
+        #     plt.imshow(history[i])
+        #     plt.title("iter=%d" % (i * 50))
+        #     plt.axis('off')
+        # # plt.show()
+        # filename = str(self.iteration_num) + '_' + str(round(time.time()*1000)) + '.png'
+        # plt.savefig(filename)
 
         return dummy_data, dummy_label
```

### Comparing `fedml-0.8.4a9/fedml/core/security/attack/revealing_labels_from_gradients_attack.py` & `fedml-0.8.5a1/fedml/core/security/attack/revealing_labels_from_gradients_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/attack/label_flipping_attack.py` & `fedml-0.8.5a1/fedml/fa/simulation/sp/simulator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,79 @@
-import torch
-from torch.utils.data import DataLoader
-from torch.utils.data import TensorDataset
-
-from ..common.utils import (
-    get_malicious_client_id_list,
-    replace_original_class_with_target_class,
-    log_client_data_statistics,
-)
-
-"""
-ref: Tolpegin, Vale, Truex,  "Data Poisoning Attacks Against Federated Learning Systems."  (2021).
-attack @client, added by Yuhui, 07/08/2022
-"""
-
-
-class LabelFlippingAttack:
-    def __init__(
-        self, args):
-        self.original_class_list = args.original_class_list
-        self.target_class_list = args.target_class_list
-        self.client_num = args.client_num
-        self.attack_epoch = 0
-        self.poisoned_client_num = args.poisoned_client_num
-        self.batch_size = args.batch_size
-        self.poisoned_client_list = []
+import logging
+import random
+from fedml.fa.aggregator.global_analyzer_creator import create_global_analyzer
+from fedml.fa.local_analyzer.client_analyzer_creator import create_local_analyzer
+from fedml.fa.simulation.sp.client import Client
+from fedml.fa.simulation.utils import client_sampling
 
-    def poison_data(self, dataset):
+
+class FASimulatorSingleProcess:
+    def __init__(self, args, dataset):
+        self.args = args
         [
             train_data_num,
-            test_data_num,
-            train_data_global,
-            test_data_global,
-            train_data_local_num_dict,
+            local_datasize_dict,
             train_data_local_dict,
-            test_data_local_dict,
-            class_num,
         ] = dataset
-        self.poisoned_client_list = get_malicious_client_id_list(
-            random_seed=self.attack_epoch, client_num=self.client_num, malicious_client_num=self.poisoned_client_num,
+
+        self.train_data_num_in_total = train_data_num
+        self.client_list = []
+        self.local_datasize_dict = local_datasize_dict
+        self.train_data_local_dict = train_data_local_dict
+        self.local_analyzer = create_local_analyzer(args)
+        self.aggregator = create_global_analyzer(args, train_data_num)
+        if self.aggregator.get_init_msg() is not None:
+            self.local_analyzer.set_init_msg(self.aggregator.get_init_msg())
+        self._setup_clients(
+            local_datasize_dict, train_data_local_dict, self.local_analyzer,
         )
-        self.attack_epoch += 1
-        poisoned_dataset = []
-        for client_idx in range(self.client_num):
-            if client_idx in self.poisoned_client_list:
-                tmp_local_dataset_X = torch.Tensor([])
-                tmp_local_dataset_Y = torch.Tensor([])
-                for batch_idx, (data, target) in enumerate(train_data_local_dict[client_idx]):
-                    tmp_local_dataset_X = torch.cat((tmp_local_dataset_X, data))
-                    tmp_local_dataset_Y = torch.cat((tmp_local_dataset_Y, target))
-                tmp_Y = replace_original_class_with_target_class(
-                    data_labels=tmp_local_dataset_Y,
-                    original_class_list=self.original_class_list,
-                    target_class_list=self.target_class_list,
+
+    def _setup_clients(
+            self, local_datasize_dict, train_data_local_dict, local_analyzer,
+    ):
+        logging.info("############setup_clients (START)#############")
+        for client_idx in range(self.args.client_num_per_round):
+            c = Client(
+                client_idx,
+                train_data_local_dict[client_idx],
+                local_datasize_dict[client_idx],
+                self.args,
+                local_analyzer,
+            )
+            self.client_list.append(c)
+        logging.info("############setup_clients (END)#############")
+
+    def analyze(self):
+        logging.info("self.local_analyzer = {}".format(self.local_analyzer))
+        local_sample_num = dict()
+        for round_idx in range(self.args.comm_round):
+            logging.info("################Communication round : {}".format(round_idx))
+            client_submission_list = []
+
+            """
+            for scalability: following the original FedAvg algorithm, we uniformly sample a fraction of clients in each round.
+            Instead of changing the 'Client' instances, our implementation keeps the 'Client' instances and then updates their local dataset 
+            """
+            client_indexes = client_sampling(
+                round_idx, self.args.client_num_in_total, self.args.client_num_per_round
+            )
+            print(f"self.local_datasize_dict={self.local_datasize_dict}, local_sample_num={local_sample_num}")
+            for i in client_indexes:
+                local_sample_num[i] = random.randint(1, self.local_datasize_dict[i])
+                #     todo: add sample mode
+
+            for idx, client in enumerate(self.client_list):
+                # update dataset
+                client_idx = client_indexes[idx]
+                client.update_local_dataset(
+                    client_idx,
+                    self.train_data_local_dict[client_idx],
+                    local_sample_num[client_idx]
                 )
-                dataset = TensorDataset(tmp_local_dataset_X, tmp_Y)
-                data_loader = DataLoader(dataset, batch_size=self.batch_size)
-                poisoned_dataset.append(data_loader)
-            else:
-                poisoned_dataset.append(train_data_local_dict[client_idx])
-        log_client_data_statistics(self.poisoned_client_list, poisoned_dataset)
-        self.attack_epoch = self.attack_epoch + 1
-        return poisoned_dataset
+
+                client_submission = client.local_analyze(w_global=self.aggregator.get_server_data())
+                client_submission_list.append((client.get_sample_number(), client_submission))
+            result = self.aggregator.aggregate(client_submission_list)
+            print(f"round_idx={round_idx}, aggregation result = {result}")
+
+    def run(self):
+        self.analyze()
```

### Comparing `fedml-0.8.4a9/fedml/core/security/attack/backdoor_attack.py` & `fedml-0.8.5a1/fedml/core/security/attack/backdoor_attack.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/fedml_attacker.py` & `fedml-0.8.5a1/fedml/core/security/fedml_attacker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .attack.byzantine_attack import ByzantineAttack
 from .attack.dlg_attack import DLGAttack
+from .attack.label_flipping_attack import LabelFlippingAttack
 from .attack.model_replacement_backdoor_attack import ModelReplacementBackdoorAttack
 from .constants import ATTACK_METHOD_BYZANTINE_ATTACK, ATTACK_LABEL_FLIPPING, BACKDOOR_ATTACK_MODEL_REPLACEMENT, \
     ATTACK_METHOD_DLG
 import logging
 from ..common.ml_engine_backend import MLEngineBackend
 from typing import List, Tuple, Any
 from collections import OrderedDict
@@ -28,16 +29,16 @@
         if hasattr(args, "enable_attack") and args.enable_attack:
             logging.info("------init attack..." + args.attack_type.strip())
             self.is_enabled = True
             self.attack_type = args.attack_type.strip()
             self.attacker = None
             if self.attack_type == ATTACK_METHOD_BYZANTINE_ATTACK:
                 self.attacker = ByzantineAttack(args)
-            # elif self.attack_type == ATTACK_LABEL_FLIPPING:
-            #     self.attacker = LabelFlippingAttack(args)
+            elif self.attack_type == ATTACK_LABEL_FLIPPING:
+                self.attacker = LabelFlippingAttack(args)
             elif self.attack_type == BACKDOOR_ATTACK_MODEL_REPLACEMENT:
                 self.attacker = ModelReplacementBackdoorAttack(args)
             elif self.attack_type == ATTACK_METHOD_DLG:
                 self.attacker = DLGAttack(args=args)
         else:
             self.is_enabled = False
 
@@ -56,38 +57,49 @@
 
     def is_attack_enabled(self):
         return self.is_enabled
 
     def get_attack_types(self):
         return self.attack_type
 
+    # --------------- for model poisoning attacks --------------- #
     def is_model_attack(self):
         if self.is_attack_enabled() and self.attack_type in [
             ATTACK_METHOD_BYZANTINE_ATTACK, BACKDOOR_ATTACK_MODEL_REPLACEMENT
         ]:
             return True
         return False
 
-    def is_poison_data_attack(self):
-        if self.is_attack_enabled() and self.attack_type in []:
-            return True
-        return False
+    def attack_model(self, raw_client_grad_list: List[Tuple[float, OrderedDict]], extra_auxiliary_info: Any = None):
+        if self.attacker is None:
+            raise Exception("attacker is not initialized!")
+        return self.attacker.attack_model(raw_client_grad_list, extra_auxiliary_info)
+    # --------------- for model poisoning attacks --------------- #
 
-    def is_reconstruct_data_attack(self):
-        if self.is_attack_enabled() and self.attack_type in [ATTACK_METHOD_DLG]:
+    # --------------- for data poisoning attacks --------------- #
+    def is_data_poisoning_attack(self):
+        if self.is_attack_enabled() and self.attack_type in [ATTACK_LABEL_FLIPPING]:
             return True
         return False
 
-    def attack_model(self, raw_client_grad_list: List[Tuple[float, OrderedDict]], extra_auxiliary_info: Any = None):
+    def is_to_poison_data(self):
         if self.attacker is None:
             raise Exception("attacker is not initialized!")
-        return self.attacker.attack_model(raw_client_grad_list, extra_auxiliary_info)
+        return self.attacker.is_to_poison_data()
 
     def poison_data(self, dataset):
         if self.attacker is None:
             raise Exception("attacker is not initialized!")
         return self.attacker.poison_data(dataset)
+    # --------------- for data poisoning attacks --------------- #
+
+    # --------------- for data reconstructing attacks --------------- #
+    def is_data_reconstruction_attack(self):
+        if self.is_attack_enabled() and self.attack_type in [ATTACK_METHOD_DLG]:
+            return True
+        return False
 
     def reconstruct_data(self, raw_client_grad_list: List[Tuple[float, OrderedDict]], extra_auxiliary_info: Any = None):
         if self.attacker is None:
             raise Exception("attacker is not initialized!")
         self.attacker.reconstruct_data(raw_client_grad_list, extra_auxiliary_info=extra_auxiliary_info)
+    # --------------- for data reconstructing attacks --------------- #
```

### Comparing `fedml-0.8.4a9/fedml/core/security/constants.py` & `fedml-0.8.5a1/fedml/core/security/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 DEFENSE_NORM_DIFF_CLIPPING = "norm_diff_clipping"
 DEFENSE_ROBUST_LEARNING_RATE = "robust_learning_rate"
 DEFENSE_KRUM = "krum"
 DEFENSE_SLSGD = "slsgd"
-DEFENSE_GEO_MEDIAN = "geometric_median"
+DEFENSE_GEO_MEDIAN = "geo_median"
 DEFENSE_CCLIP = "cclip"
 DEFENSE_WEAK_DP = "weak_dp"
 DEFENSE_DP = "dp"
 DEFENSE_RFA = "rfa"
 DEFENSE_FOOLSGOLD = "foolsgold"
 DEFENSE_CRFL = "crfl"
 DEFENSE_THREESIGMA = "3sigma"
 DEFENSE_THREESIGMA_KRUM = "3sigma_krum"
 DEFENSE_THREESIGMA_GEOMEDIAN = "3sigma_geo"
 DEFENSE_MULTIKRUM = "multikrum"
 DEFENSE_TRIMMED_MEAN = "trimmed_mean"
+DEFENSE_DIFF_CLIPPING = "diff_clipping"
+DEFENSE_WISE_MEDIAN = "wise_median"
 ANOMALY_DETECTION = "anomaly_detection"
 
 ATTACK_METHOD_BYZANTINE_ATTACK = "byzantine"
 ATTACK_METHOD_DLG = "dlg"
 ATTACK_LABEL_FLIPPING = "label_flipping"
 BACKDOOR_ATTACK_MODEL_REPLACEMENT = "model_replacement"
```

### Comparing `fedml-0.8.4a9/fedml/core/security/fedml_defender.py` & `fedml-0.8.5a1/fedml/core/security/fedml_defender.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from collections import OrderedDict
 from typing import List, Tuple, Any, Callable
 from .defense.RFA_defense import RFADefense
+from .defense.coordinate_wise_median_defense import CoordinateWiseMedianDefense
 from .defense.coordinate_wise_trimmed_mean_defense import CoordinateWiseTrimmedMeanDefense
 from .defense.crfl_defense import CRFLDefense
 from .defense.outlier_detection import OutlierDetection
 from .defense.three_sigma_defense import ThreeSigmaDefense
 from .defense.three_sigma_geomedian_defense import ThreeSigmaGeoMedianDefense
 from .defense.three_sigma_krum_defense import ThreeSigmaKrumDefense
 from ..common.ml_engine_backend import MLEngineBackend
@@ -28,15 +29,15 @@
     DEFENSE_RFA,
     DEFENSE_FOOLSGOLD,
     DEFENSE_THREESIGMA,
     DEFENSE_CRFL,
     DEFENSE_MULTIKRUM,
     DEFENSE_TRIMMED_MEAN,
     DEFENSE_THREESIGMA_GEOMEDIAN,
-    DEFENSE_THREESIGMA_KRUM, ANOMALY_DETECTION,
+    DEFENSE_THREESIGMA_KRUM, ANOMALY_DETECTION, DEFENSE_WISE_MEDIAN, DEFENSE_DIFF_CLIPPING,
 )
 
 
 class FedMLDefender:
     _defender_instance = None
 
     @staticmethod
@@ -69,14 +70,16 @@
                 self.defender = SLSGDDefense(args)
             elif self.defense_type == DEFENSE_GEO_MEDIAN:
                 self.defender = GeometricMedianDefense(args)
             elif self.defense_type == DEFENSE_WEAK_DP:
                 self.defender = WeakDPDefense(args)
             elif self.defense_type == DEFENSE_CCLIP:
                 self.defender = CClipDefense(args)
+            elif self.defense_type == DEFENSE_WISE_MEDIAN:
+                self.defender = CoordinateWiseMedianDefense(args)
             elif self.defense_type == DEFENSE_RFA:
                 self.defender = RFADefense(args)
             elif self.defense_type == DEFENSE_FOOLSGOLD:
                 self.defender = FoolsGoldDefense(args)
             elif self.defense_type == DEFENSE_THREESIGMA:
                 self.defender = ThreeSigmaDefense(args)
             elif self.defense_type == DEFENSE_THREESIGMA_GEOMEDIAN:
@@ -122,35 +125,33 @@
         if self.defender is None:
             raise Exception("defender is not initialized!")
         return self.defender.run(
             raw_client_grad_list, base_aggregation_func, extra_auxiliary_info
         )
 
     def is_defense_on_aggregation(self):
-        return self.is_defense_enabled() and self.defense_type in [
-            DEFENSE_SLSGD,
-            DEFENSE_CRFL,
-            DEFENSE_RFA,
-        ]
+        return self.is_defense_enabled() and self.defense_type in [DEFENSE_SLSGD, DEFENSE_RFA, DEFENSE_WISE_MEDIAN, DEFENSE_GEO_MEDIAN]
 
     def is_defense_before_aggregation(self):
         return self.is_defense_enabled() and self.defense_type in [
             DEFENSE_SLSGD,
             DEFENSE_FOOLSGOLD,
             DEFENSE_THREESIGMA,
             DEFENSE_THREESIGMA_GEOMEDIAN,
             DEFENSE_THREESIGMA_KRUM,
             DEFENSE_KRUM,
+            DEFENSE_CCLIP,
             DEFENSE_MULTIKRUM,
             DEFENSE_TRIMMED_MEAN,
-            ANOMALY_DETECTION
+            ANOMALY_DETECTION,
+            DEFENSE_NORM_DIFF_CLIPPING
         ]
 
     def is_defense_after_aggregation(self):
-        return self.is_defense_enabled() and self.defense_type in [DEFENSE_CRFL]
+        return self.is_defense_enabled() and self.defense_type in [DEFENSE_CRFL, DEFENSE_CCLIP]
 
     def defend_before_aggregation(
         self,
         raw_client_grad_list: List[Tuple[float, OrderedDict]],
         extra_auxiliary_info: Any = None,
     ):
         if self.defender is None:
```

### Comparing `fedml-0.8.4a9/fedml/core/security/common/bucket.py` & `fedml-0.8.5a1/fedml/core/security/common/bucket.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import math
+from collections import OrderedDict
 
 
 class Bucket:
     @classmethod
     def bucketization(cls, client_grad_list, batch_size):
         (num0, averaged_params) = client_grad_list[0]
         batch_grad_list = []
         for batch_idx in range(0, math.ceil(len(client_grad_list) / batch_size)):
             client_num = cls._get_client_num_current_batch(
                 batch_size, batch_idx, client_grad_list
             )
             sample_num = cls._get_total_sample_num_for_current_batch(
                 batch_idx * batch_size, client_num, client_grad_list
             )
-            batch_weight = dict()
+            batch_weight = OrderedDict()
             for i in range(0, client_num):
                 local_sample_num, local_model_params = client_grad_list[
                     batch_idx * batch_size + i
                 ]
                 w = local_sample_num / sample_num
                 for k in averaged_params.keys():
                     if i == 0:
```

### Comparing `fedml-0.8.4a9/fedml/core/security/common/net.py` & `fedml-0.8.5a1/fedml/core/security/common/net.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/common/attack_defense_data_loader.py` & `fedml-0.8.5a1/fedml/core/security/common/attack_defense_data_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from torch.utils.data import DataLoader
 import pickle
 
 
 class AttackDefenseDataLoader:
     @classmethod
     def load_cifar10_data(
-        cls, client_num, batch_size, partition_method="homo", partition_alpha=None
+        cls, client_num, batch_size, data_dir="../../../../../data/cifar10", partition_method="homo", partition_alpha=None
     ):
         return load_partition_data_cifar10(
             "cifar10",
-            data_dir="../../../../../data/cifar10",
+            data_dir=data_dir,
             partition_method=partition_method,
             partition_alpha=partition_alpha,
             client_number=client_num,
             batch_size=batch_size,
         )
 
     @classmethod
```

### Comparing `fedml-0.8.4a9/fedml/core/security/common/utils.py` & `fedml-0.8.5a1/fedml/core/security/common/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -100,27 +100,26 @@
         client_indexes = [client_index for client_index in range(client_num)]
     else:
         num_clients = min(malicious_client_num, client_num)
         np.random.seed(
             random_seed
         )  # make sure for each comparison, we are selecting the same clients each round
         client_indexes = np.random.choice(range(client_num), num_clients, replace=False)
-    print("client_indexes = %s" % str(client_indexes))
+    print("malicious client_indexes = %s" % str(client_indexes))
     return client_indexes
 
 
 def replace_original_class_with_target_class(
         data_labels, original_class_list=None, target_class_list=None
 ):
     """
     :param targets: Target class IDs
     :type targets: list
     :return: new class IDs
     """
-
     if (
             len(original_class_list) == 0
             or len(target_class_list) == 0
             or original_class_list is None
             or target_class_list is None
     ):
         return data_labels
@@ -159,14 +158,51 @@
                     else:
                         targets_set[target] += 1
             print("Client #{} has data distribution:".format(client_idx))
             for item in targets_set.items():
                 print("target:{} num:{}".format(item[0], item[1]))
 
 
+def get_client_data_stat(local_dataset):
+    print("-==========================")
+    targets_set = {}
+    for batch_idx, (data, targets) in enumerate(local_dataset):
+        for t in targets.tolist():
+            if t in targets_set.keys():
+                targets_set[t] += 1
+            else:
+                targets_set[t] = 1
+            # if t not in targets_set.keys():
+            #     targets_set[t] = 1
+            # else:
+            #     targets_set[t] += 1
+    total_counter = 0
+    # for item in targets_set.items():
+    #     print("------target:{} num:{}".format(item[0], item[1]))
+    #     total_counter += item[1]
+    # print(f"total counter = {total_counter}")
+    #
+    # targets_set = {}
+    # for batch_idx, (data, targets) in enumerate(local_dataset):
+    #     for t in targets.tolist():
+    #         if t in targets_set.keys():
+    #             targets_set[t] += 1
+    #         else:
+    #             targets_set[t] = 1
+    #         # if t not in targets_set.keys():
+    #         #     targets_set[t] = 1
+    #         # else:
+    #         #     targets_set[t] += 1
+    # total_counter = 0
+    for item in targets_set.items():
+        print("------target:{} num:{}".format(item[0], item[1]))
+        total_counter += item[1]
+    print(f"total counter = {total_counter}")
+
+
 def cross_entropy_for_onehot(pred, target):
     return torch.mean(torch.sum(-target * F.log_softmax(pred, dim=-1), 1))
 
 
 def label_to_onehot(target, num_classes=100):
     target = torch.unsqueeze(target, 1)
     onehot_target = torch.zeros(target.size(0), num_classes, device=target.device)
```

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/three_sigma_defense.py` & `fedml-0.8.5a1/fedml/core/security/defense/three_sigma_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/norm_diff_clipping_defense.py` & `fedml-0.8.5a1/fedml/core/security/defense/norm_diff_clipping_defense.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,48 +10,47 @@
 https://arxiv.org/pdf/1911.07963.pdf 
 """
 
 
 class NormDiffClippingDefense(BaseDefenseMethod):
     def __init__(self, config):
         self.config = config
-        self.norm_bound = config.norm_bound  # for norm diff clipping and weak DP defenses
+        self.norm_bound = config.norm_bound  # for norm diff clipping; in the paper, they set it to 0.1, 0.17, and 0.33.
 
-    def run(
-        self,
-        raw_client_grad_list: List[Tuple[float, OrderedDict]],
-        base_aggregation_func: Callable = None,
-        extra_auxiliary_info: Any = None,
+    def defend_before_aggregation(
+            self,
+            raw_client_grad_list: List[Tuple[float, OrderedDict]],
+            extra_auxiliary_info: Any = None,
     ):
         global_model = extra_auxiliary_info
         vec_global_w = utils.vectorize_weight(global_model)
         new_grad_list = []
         for (sample_num, local_w) in raw_client_grad_list:
             vec_local_w = utils.vectorize_weight(local_w)
             clipped_weight_diff = self._get_clipped_norm_diff(vec_local_w, vec_global_w)
             clipped_w = self._get_clipped_weights(
                 local_w, global_model, clipped_weight_diff
             )
             new_grad_list.append((sample_num, clipped_w))
-        return base_aggregation_func(self.config, new_grad_list)  # avg_params
+        return new_grad_list
 
     def _get_clipped_norm_diff(self, vec_local_w, vec_global_w):
         vec_diff = vec_local_w - vec_global_w
         weight_diff_norm = torch.norm(vec_diff).item()
         clipped_weight_diff = vec_diff / max(1, weight_diff_norm / self.norm_bound)
         return clipped_weight_diff
 
     @staticmethod
     def _get_clipped_weights(local_w, global_w, weight_diff):
         #  rule: global_w + clipped(local_w - global_w)
-        recons_local_w = {}
+        recons_local_w = OrderedDict()
         index_bias = 0
         for item_index, (k, v) in enumerate(local_w.items()):
             if utils.is_weight_param(k):
                 recons_local_w[k] = (
-                    weight_diff[index_bias : index_bias + v.numel()].view(v.size())
+                    weight_diff[index_bias: index_bias + v.numel()].view(v.size())
                     + global_w[k]
                 )
                 index_bias += v.numel()
             else:
                 recons_local_w[k] = v
         return recons_local_w
```

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/residual_based_reweighting_defense.py` & `fedml-0.8.5a1/fedml/core/security/defense/residual_based_reweighting_defense.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,23 +29,14 @@
     def defend_before_aggregation(
         self,
         raw_client_grad_list: List[Tuple[float, OrderedDict]],
         extra_auxiliary_info: Any = None,
     ):
         return self.IRLS_other_split_restricted(raw_client_grad_list)
 
-    def defend_on_aggregation(
-        self,
-        raw_client_grad_list: List[Tuple[float, OrderedDict]],
-        base_aggregation_func: Callable = None,
-        extra_auxiliary_info: Any = None,
-    ):
-
-        return base_aggregation_func(raw_client_grad_list)
-
     def IRLS_other_split_restricted(self, raw_client_grad_list):
         reweight_algorithm = median_reweight_algorithm_restricted
         if self.mode == "median":
             reweight_algorithm = median_reweight_algorithm_restricted
         elif self.mode == "theilsen":
             reweight_algorithm = theilsen_reweight_algorithm_restricted
         elif self.mode == "gaussian":
```

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/three_sigma_krum_defense.py` & `fedml-0.8.5a1/fedml/core/security/defense/three_sigma_krum_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/coordinate_wise_trimmed_mean_defense.py` & `fedml-0.8.5a1/fedml/core/security/defense/coordinate_wise_trimmed_mean_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/slsgd_defense.py` & `fedml-0.8.5a1/fedml/core/security/defense/slsgd_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/coordinate_wise_median_defense.py` & `fedml-0.8.5a1/fedml/core/security/defense/coordinate_wise_median_defense.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 from collections import OrderedDict
-
 import torch
-from typing import Callable, List, Tuple, Dict, Any
+from typing import Callable, List, Tuple, Any
 from .defense_base import BaseDefenseMethod
 from ..common.utils import vectorize_weight
 
 """
 Coordinate-wise Median from "Byzantine-Robust Distributed Learning: Towards Optimal Statistical Rates".
 This can be called at aggregate() of an Aggregator inplace of parameter averaging after \
 model_list has been created
  """
 
 
 class CoordinateWiseMedianDefense(BaseDefenseMethod):
     def __init__(self, config):
         pass
 
-    def run(
-        self,
-        raw_client_grad_list: List[Tuple[float, OrderedDict]],
-        base_aggregation_func: Callable = None,
-        extra_auxiliary_info: Any = None,
-    ) -> Dict:
-        (num0, averaged_params) = raw_client_grad_list[0]
+    def defend_on_aggregation(
+            self,
+            raw_client_grad_list: List[Tuple[float, OrderedDict]],
+            base_aggregation_func: Callable = None,
+            extra_auxiliary_info: Any = None,
+    ):
         vectorized_params = []
 
         for i in range(0, len(raw_client_grad_list)):
             local_sample_number, local_model_params = raw_client_grad_list[i]
             vectorized_weight = vectorize_weight(local_model_params)
             vectorized_params.append(vectorized_weight.unsqueeze(-1))
 
         # concatenate all weights by the last dimension (number of clients)
         vectorized_params = torch.cat(vectorized_params, dim=-1)
         vec_median_params = torch.median(vectorized_params, dim=-1).values
 
         index = 0
+        (num0, averaged_params) = raw_client_grad_list[0]
         for k, params in averaged_params.items():
             median_params = vec_median_params[index : index + params.numel()].view(
                 params.size()
             )
             index += params.numel()
             averaged_params[k] = median_params
```

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/wbc_defense.py` & `fedml-0.8.5a1/fedml/core/security/defense/wbc_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/robust_learning_rate_defense.py` & `fedml-0.8.5a1/fedml/core/security/defense/robust_learning_rate_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/RFA_defense.py` & `fedml-0.8.5a1/fedml/core/security/defense/RFA_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/defense_base.py` & `fedml-0.8.5a1/fedml/core/security/defense/defense_base.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/foolsgold_defense.py` & `fedml-0.8.5a1/fedml/core/security/defense/foolsgold_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/soteria_defense.py` & `fedml-0.8.5a1/fedml/core/security/defense/soteria_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/bulyan_defense.py` & `fedml-0.8.5a1/fedml/core/security/defense/bulyan_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/cross_round_defense.py` & `fedml-0.8.5a1/fedml/core/security/defense/cross_round_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/three_sigma_geomedian_defense.py` & `fedml-0.8.5a1/fedml/core/security/defense/three_sigma_geomedian_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/geometric_median_defense.py` & `fedml-0.8.5a1/fedml/core/security/defense/geometric_median_defense.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,19 +27,19 @@
         # trade-off between accuracy & robustness:
         #       larger batch_num --> more Byzantine robustness, larger estimation error.
         self.batch_num = config.batch_num
         if self.byzantine_client_num == 0:
             self.batch_num = 1
         self.batch_size = math.ceil(self.client_num_per_round / self.batch_num)
 
-    def run(
-        self,
-        raw_client_grad_list: List[Tuple[float, OrderedDict]],
-        base_aggregation_func: Callable = None,
-        extra_auxiliary_info: Any = None,
+    def defend_on_aggregation(
+            self,
+            raw_client_grad_list: List[Tuple[float, OrderedDict]],
+            base_aggregation_func: Callable = None,
+            extra_auxiliary_info: Any = None,
     ):
         batch_grad_list = Bucket.bucketization(raw_client_grad_list, self.batch_size)
         (num0, avg_params) = batch_grad_list[0]
         alphas = {alpha for (alpha, params) in batch_grad_list}
         alphas = {alpha / sum(alphas, 0.0) for alpha in alphas}
         for k in avg_params.keys():
             batch_grads = [params[k] for (alpha, params) in batch_grad_list]
```

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/crfl_defense.py` & `fedml-0.8.5a1/fedml/core/dp/frames/dp_clip.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,61 @@
 from collections import OrderedDict
-from .defense_base import BaseDefenseMethod
-from typing import Callable, List, Tuple, Any
-from ..common import utils
-from ...dp.mechanisms import Gaussian
+import torch
+from fedml.core.dp.frames.base_dp_solution import BaseDPFrame
+from typing import List, Tuple, Dict, Any
 
 """
-CRFL: Certifiably Robust Federated Learning against Backdoor Attacks (ICML 2021)
-http://proceedings.mlr.press/v139/xie21a/xie21a.pdf
+(ICLR 2018) Learning Differentially Private Recurrent Language Models
+
+1. (todo: Need to change sampling process) each user is selected independently with probability q, rather than always selecting a fixed number of users
+2. enforce clipping of per-user updates so the total update has bounded L2 norm.
+3. use different estimators for the average update (introduced next).
+4. add Gaussian noise to the final average update.
 """
 
+class DP_Clip(BaseDPFrame):
+    def __init__(self, args):
+        super().__init__(args)
+        self.clipping_norm = args.clipping_norm
+        self.train_data_num_in_total = args.train_data_num_in_total
+        self._scale = args.clipping_norm * args.noise_multiplier
+
+    def clip_local_update(self, local_grad, norm_type: float = 2.0):
+        total_norm = torch.norm(torch.stack([torch.norm(local_grad[k], norm_type) for k in local_grad.keys()]), norm_type)
+        clip_coef = self.clipping_norm / (total_norm + 1e-6)
+        clip_coef_clamped = torch.clamp(clip_coef, max=1.0)
+        for k in local_grad.keys():
+            local_grad[k].mul_(clip_coef_clamped)
+        return local_grad
+
+    def add_local_noise(self, local_grad: OrderedDict, extra_auxiliary_info: Any = None,):
+        global_model_params = extra_auxiliary_info
+        for k in global_model_params.keys():
+            local_grad[k] = local_grad[k] - global_model_params[k]
+        return self.clip_local_update(local_grad, self.clipping_norm)
 
-class CRFLDefense(BaseDefenseMethod):
-    def __init__(self, config):
-        self.config = config
-        self.epoch = 1
-        if hasattr(config, "clip_threshold"):
-            self.clip_threshold = config.clip_threshold
-        else:
-            self.clip_threshold = None
-        if hasattr(config, "sigma") and isinstance(config.sigma, float):
-            self.sigma = config.sigma
-        else:
-            self.sigma = 0.01  # in the code of CRFL, the author set sigma to 0.01
-
-    def defend_before_aggregation(
-            self,
-            raw_client_grad_list: List[Tuple[float, OrderedDict]],
-            extra_auxiliary_info: Any = None,
-    ):
-        return raw_client_grad_list
-
-    def defend_on_aggregation(
-            self,
-            raw_client_grad_list: List[Tuple[float, OrderedDict]],
-            base_aggregation_func: Callable = None,
-            extra_auxiliary_info: Any = None,
-    ):
-        avg_params = base_aggregation_func(args=self.config, raw_grad_list=raw_client_grad_list)
-        """
-        clip the global model; dynamic threshold is adjusted according to the dataset;
-        in the experiment, the authors set the dynamic threshold as follows:
-            dataset == MNIST: dynamic_thres = epoch * 0.1 + 2
-            dataseet == LOAN: dynamic_thres = epoch * 0.025 + 2
-            datset == EMNIST: dynamic_thres = epoch * 0.25 + 4
-        """
-        dynamic_threshold = self.epoch * 0.1 + 2
-        if self.clip_threshold is None or self.clip_threshold > dynamic_threshold:
-            self.clip_threshold = dynamic_threshold
-        self.epoch += 1
-
-        new_model = self.clip_weight_norm(avg_params, self.clip_threshold)
-        # the output model is new model; later the algo adds dp noise to the global model
-        return new_model
-
-    def defend_after_aggregation(self, global_model):
-        # todo: to discuss with chaoyang: the output is the clipped model (real model);
-        # add dp noise to the real model and sent the permuted model to clients; how to get the last iteration?
-        new_global_model = OrderedDict()
+    def add_global_noise(self, global_model: OrderedDict):
+        qw = self.train_data_num_in_total * (self.args.client_num_per_round / self.args.client_num_in_total)
         for k in global_model.keys():
-            new_global_model[k] = global_model[k] + Gaussian.compute_noise_using_sigma(self.sigma, global_model[k].shape)
-        return new_global_model
+            global_model[k] = global_model[k] / qw
+        w_global = self.add_noise(
+            global_model, qw
+        )
+        for k in w_global.keys():
+            w_global[k] = w_global[k] + global_model[k]
+
+    def get_global_params(self):
+        pass
+
+    def compute_noise(self, size, qw):
+        self._scale = self._scale / qw
+        return torch.normal(mean=0, std=self._scale, size=size)
+
+    def add_noise(self, w_global, qw):
+        new_params = OrderedDict()
+        for k in w_global.keys():
+            new_params[k] = self.compute_noise(w_global[k].shape, qw) + w_global[k]
+        return new_params
+
+
+
 
-    @staticmethod
-    def clip_weight_norm(model, clip_threshold):
-        total_norm = utils.compute_model_norm(model)
-        print(f"total_norm = {total_norm}")
-        if total_norm > clip_threshold:
-            clip_coef = clip_threshold / (total_norm + 1e-6)
-            new_model = OrderedDict()
-            for k in model.keys():
-                new_model[k] = model[k] * clip_coef
-            return new_model
-        return model
```

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/outlier_detection.py` & `fedml-0.8.5a1/fedml/core/security/defense/outlier_detection.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/weak_dp_defense.py` & `fedml-0.8.5a1/fedml/core/security/defense/weak_dp_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/cclip_defense.py` & `fedml-0.8.5a1/fedml/core/security/defense/cclip_defense.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import OrderedDict
-from typing import Callable, List, Tuple, Any
+from typing import List, Tuple, Any
 import numpy as np
 from .defense_base import BaseDefenseMethod
 from ..common import utils
 from ..common.bucket import Bucket
 
 """
 defense @ server, added by Xiaoyang, 07/10/2022
@@ -11,51 +11,54 @@
 https://arxiv.org/pdf/2006.09365.pdf
 """
 
 
 class CClipDefense(BaseDefenseMethod):
     def __init__(self, config):
         self.config = config
-        self.tau = config.tau  # clipping raduis
+        if hasattr(config, "tau") and type(config.tau) in [int, float] and config.tau > 0:
+            self.tau = config.tau  # clipping raduis; tau = 10 / (1-beta), beta is the coefficient of momentum
+        else:
+            self.tau = 10  # default: no momentum, beta = 0
         # element # in each bucket; a grad_list is partitioned into floor(len(grad_list)/bucket_size) buckets
         self.bucket_size = config.bucket_size
+        self.initial_guess = None
 
-    def run(
-        self,
-        raw_client_grad_list: List[Tuple[float, OrderedDict]],
-        base_aggregation_func: Callable = None,
-        extra_auxiliary_info: Any = None,
-    ) -> OrderedDict:
+    def defend_before_aggregation(
+            self,
+            raw_client_grad_list: List[Tuple[float, OrderedDict]],
+            extra_auxiliary_info: Any = None,
+    ):
         client_grad_buckets = Bucket.bucketization(
             raw_client_grad_list, self.bucket_size
         )
-        initial_guess = self._compute_an_initial_guess(client_grad_buckets)
+        self.initial_guess = self._compute_an_initial_guess(client_grad_buckets)
         bucket_num = len(client_grad_buckets)
         vec_local_w = [
             (
                 client_grad_buckets[i][0],
                 utils.vectorize_weight(client_grad_buckets[i][1]),
             )
             for i in range(bucket_num)
         ]
-        vec_refs = utils.vectorize_weight(initial_guess)
+        vec_refs = utils.vectorize_weight(self.initial_guess)
         cclip_score = self._compute_cclip_score(vec_local_w, vec_refs)
         new_grad_list = []
         for i in range(bucket_num):
-            tuple = dict()
+            tuple = OrderedDict()
             sample_num, bucket_params = client_grad_buckets[i]
             for k in bucket_params.keys():
-                tuple[k] = (bucket_params[k] - initial_guess[k]) * cclip_score[i]
+                tuple[k] = (bucket_params[k] - self.initial_guess[k]) * cclip_score[i]
             new_grad_list.append((sample_num, tuple))
-        print(f"cclip_score = {cclip_score}")
+        return new_grad_list
 
-        avg_params = base_aggregation_func(self.config, new_grad_list)
-        for k in avg_params.keys():
-            avg_params[k] = initial_guess[k] + avg_params[k]
-        return avg_params
+    def defend_after_aggregation(self, global_model):
+        for k in global_model.keys():
+            global_model[k] = self.initial_guess[k] + global_model[k]
+        return global_model
 
     @staticmethod
     def _compute_an_initial_guess(client_grad_list):
         # randomly select a gradient as the initial guess
         return client_grad_list[np.random.randint(0, len(client_grad_list))][1]
 
     def _compute_cclip_score(self, local_w, refs):
```

### Comparing `fedml-0.8.4a9/fedml/core/security/defense/krum_defense.py` & `fedml-0.8.5a1/fedml/core/security/defense/krum_defense.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/mlops/mlops_configs.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/modelops_configs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,215 +1,201 @@
 
 import os
+import time
+
 import certifi
 import requests
+from fedml.core.mlops import MLOpsUtils
 
 
 class Singleton(object):
     def __new__(cls):
         if not hasattr(cls, "_instance"):
             orig = super(Singleton, cls)
             cls._instance = orig.__new__(cls)
         return cls._instance
 
 
-class MLOpsConfigs(Singleton):
+class ModelOpsConfigs(Singleton):
     _config_instance = None
 
     def __init__(self):
         self.args = None
 
     @staticmethod
     def get_instance(args):
-        if MLOpsConfigs._config_instance is None:
-            MLOpsConfigs._config_instance = MLOpsConfigs()
-            MLOpsConfigs._config_instance.args = args
+        if ModelOpsConfigs._config_instance is None:
+            ModelOpsConfigs._config_instance = ModelOpsConfigs()
+            ModelOpsConfigs._config_instance.args = args
 
-        return MLOpsConfigs._config_instance
+        return ModelOpsConfigs._config_instance
 
-    def get_request_params(self):
+    def get_request_params(self, in_config_version="release"):
         url = "https://open.fedml.ai/fedmlOpsServer/configs/fetch"
         config_version = "release"
-        if (
-                hasattr(self.args, "config_version")
-                and self.args.config_version is not None
-        ):
+        if in_config_version is not None and in_config_version != "":
             # Setup config url based on selected version.
-            config_version = self.args.config_version
-            if self.args.config_version == "release":
+            config_version = in_config_version
+            if config_version == "release":
                 url = "https://open.fedml.ai/fedmlOpsServer/configs/fetch"
-            elif self.args.config_version == "test":
+            elif config_version == "test":
                 url = "https://open-test.fedml.ai/fedmlOpsServer/configs/fetch"
-            elif self.args.config_version == "dev":
+            elif config_version == "dev":
                 url = "https://open-dev.fedml.ai/fedmlOpsServer/configs/fetch"
-            elif self.args.config_version == "local":
+            elif config_version == "local":
                 if hasattr(self.args, "local_server") and self.args.local_server is not None:
                     url = "http://{}:9000/fedmlOpsServer/configs/fetch".format(self.args.local_server)
                 else:
                     url = "http://localhost:9000/fedmlOpsServer/configs/fetch"
 
         cert_path = None
         if str(url).startswith("https://"):
             cur_source_dir = os.path.dirname(__file__)
             cert_path = os.path.join(
-                cur_source_dir, "ssl", "open-" + config_version + ".fedml.ai_bundle.crt"
-            )
-
-        return url, cert_path
-
-    def get_request_params_with_version(self, version):
-        url = "https://open.fedml.ai/fedmlOpsServer/configs/fetch"
-        if version == "release":
-            url = "https://open.fedml.ai/fedmlOpsServer/configs/fetch"
-        elif version == "test":
-            url = "https://open-test.fedml.ai/fedmlOpsServer/configs/fetch"
-        elif version == "dev":
-            url = "https://open-dev.fedml.ai/fedmlOpsServer/configs/fetch"
-        elif version == "local":
-            if hasattr(self.args, "local_server") and self.args.local_server is not None:
-                url = "http://{}:9000/fedmlOpsServer/configs/fetch".format(self.args.local_server)
-            else:
-                url = "http://localhost:9000/fedmlOpsServer/configs/fetch"
-
-        cert_path = None
-        if str(url).startswith("https://"):
-            cur_source_dir = os.path.dirname(__file__)
-            cert_path = os.path.join(
-                cur_source_dir, "ssl", "open-" + version + ".fedml.ai_bundle.crt"
+                cur_source_dir, "ssl", "model-" + config_version + ".fedml.ai_bundle.crt"
             )
 
         return url, cert_path
 
     @staticmethod
     def get_root_ca_path():
         cur_source_dir = os.path.dirname(__file__)
-        cert_path = os.path.join(
-            cur_source_dir, "ssl", "open-root-ca.crt"
-        )
+        cert_path = os.path.join(cur_source_dir, "..", "..", "core", "mlops", "ssl", "open-root-ca.crt")
         return cert_path
 
     @staticmethod
     def install_root_ca_file():
         ca_file = certifi.where()
-        open_root_ca_path = MLOpsConfigs.get_root_ca_path()
+        open_root_ca_path = ModelOpsConfigs.get_root_ca_path()
         with open(open_root_ca_path, 'rb') as infile:
             open_root_ca_file = infile.read()
         with open(ca_file, 'ab') as outfile:
             outfile.write(open_root_ca_file)
 
-    def fetch_configs(self):
-        url, cert_path = self.get_request_params()
-        json_params = {"config_name": ["mqtt_config", "s3_config"]}
+    def fetch_configs(self, config_version="release"):
+        url, cert_path = self.get_request_params(config_version)
+        json_params = {"config_name": ["mqtt_config", "s3_config", "ml_ops_config"],
+                       "device_send_time": int(time.time() * 1000)}
 
         if cert_path is not None:
             try:
                 requests.session().verify = cert_path
                 response = requests.post(
                     url, json=json_params, verify=True, headers={"content-type": "application/json", "Connection": "close"}
                 )
             except requests.exceptions.SSLError as err:
-                MLOpsConfigs.install_root_ca_file()
+                ModelOpsConfigs.install_root_ca_file()
                 response = requests.post(
                     url, json=json_params, verify=True, headers={"content-type": "application/json", "Connection": "close"}
                 )
         else:
             response = requests.post(
                 url, json=json_params, headers={"content-type": "application/json", "Connection": "close"}
             )
 
         status_code = response.json().get("code")
         if status_code == "SUCCESS":
             mqtt_config = response.json().get("data").get("mqtt_config")
             s3_config = response.json().get("data").get("s3_config")
+            mlops_config = response.json().get("data").get("ml_ops_config")
+            MLOpsUtils.calc_ntp_from_config(mlops_config)
         else:
             raise Exception("failed to fetch device configurations!")
         return mqtt_config, s3_config
 
     def fetch_web3_configs(self):
         url, cert_path = self.get_request_params()
-        json_params = {"config_name": ["mqtt_config", "web3_config"]}
+        json_params = {"config_name": ["mqtt_config", "web3_config", "ml_ops_config"],
+                       "device_send_time": int(time.time() * 1000)}
 
         if cert_path is not None:
             try:
                 requests.session().verify = cert_path
                 response = requests.post(
                     url, json=json_params, verify=True, headers={"content-type": "application/json", "Connection": "close"}
                 )
             except requests.exceptions.SSLError as err:
-                MLOpsConfigs.install_root_ca_file()
+                ModelOpsConfigs.install_root_ca_file()
                 response = requests.post(
                     url, json=json_params, verify=True, headers={"content-type": "application/json", "Connection": "close"}
                 )
         else:
             response = requests.post(
                 url, json=json_params, headers={"content-type": "application/json", "Connection": "close"}
             )
 
         status_code = response.json().get("code")
         if status_code == "SUCCESS":
             mqtt_config = response.json().get("data").get("mqtt_config")
             web3_config = response.json().get("data").get("web3_config")
+            mlops_config = response.json().get("data").get("ml_ops_config")
+            MLOpsUtils.calc_ntp_from_config(mlops_config)
         else:
             raise Exception("failed to fetch device configurations!")
         return mqtt_config, web3_config
 
     def fetch_thetastore_configs(self):
         url, cert_path = self.get_request_params()
-        json_params = {"config_name": ["mqtt_config", "thetastore_config"]}
+        json_params = {"config_name": ["mqtt_config", "thetastore_config", "ml_ops_config"],
+                       "device_send_time": int(time.time() * 1000)}
 
         if cert_path is not None:
             try:
                 requests.session().verify = cert_path
                 response = requests.post(
                     url, json=json_params, verify=True, headers={"content-type": "application/json", "Connection": "close"}
                 )
             except requests.exceptions.SSLError as err:
-                MLOpsConfigs.install_root_ca_file()
+                ModelOpsConfigs.install_root_ca_file()
                 response = requests.post(
                     url, json=json_params, verify=True, headers={"content-type": "application/json", "Connection": "close"}
                 )
         else:
             response = requests.post(
                 url, json=json_params, headers={"content-type": "application/json", "Connection": "close"}
             )
 
         status_code = response.json().get("code")
         if status_code == "SUCCESS":
             mqtt_config = response.json().get("data").get("mqtt_config")
             thetastore_config = response.json().get("data").get("thetastore_config")
+            mlops_config = response.json().get("data").get("ml_ops_config")
+            MLOpsUtils.calc_ntp_from_config(mlops_config)
         else:
             raise Exception("failed to fetch device configurations!")
         return mqtt_config, thetastore_config
 
     def fetch_all_configs(self):
         url, cert_path = self.get_request_params()
-        json_params = {"config_name": ["mqtt_config", "s3_config", "ml_ops_config", "docker_config"]}
+        json_params = {"config_name": ["mqtt_config", "s3_config", "ml_ops_config", "docker_config"],
+                       "device_send_time": int(time.time() * 1000)}
 
         if cert_path is not None:
             try:
                 requests.session().verify = cert_path
                 response = requests.post(
                     url, json=json_params, verify=True, headers={"content-type": "application/json", "Connection": "close"}
                 )
             except requests.exceptions.SSLError as err:
-                MLOpsConfigs.install_root_ca_file()
+                ModelOpsConfigs.install_root_ca_file()
                 response = requests.post(
                     url, json=json_params, verify=True, headers={"content-type": "application/json", "Connection": "close"}
                 )
         else:
             response = requests.post(
                 url, json=json_params, headers={"content-type": "application/json", "Connection": "close"}
             )
 
         status_code = response.json().get("code")
         if status_code == "SUCCESS":
             mqtt_config = response.json().get("data").get("mqtt_config")
             s3_config = response.json().get("data").get("s3_config")
             mlops_config = response.json().get("data").get("ml_ops_config")
             docker_config = response.json().get("data").get("docker_config")
+            MLOpsUtils.calc_ntp_from_config(mlops_config)
         else:
             raise Exception("failed to fetch device configurations!")
 
         return mqtt_config, s3_config, mlops_config, docker_config
 
 
 if __name__ == "__main__":
```

### Comparing `fedml-0.8.4a9/fedml/core/mlops/ssl/open-dev.fedml.ai_bundle.crt` & `fedml-0.8.5a1/fedml/core/mlops/ssl/open-dev.fedml.ai_bundle.crt`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/mlops/ssl/open-release.fedml.ai_bundle.crt` & `fedml-0.8.5a1/fedml/core/mlops/ssl/open-release.fedml.ai_bundle.crt`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/mlops/ssl/open-root-ca.crt` & `fedml-0.8.5a1/fedml/core/mlops/ssl/open-root-ca.crt`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/mlops/ssl/open-test.fedml.ai_bundle.crt` & `fedml-0.8.5a1/fedml/core/mlops/ssl/open-test.fedml.ai_bundle.crt`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/mlops/mlops_metrics.py` & `fedml-0.8.5a1/fedml/core/mlops/mlops_metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 import argparse
 import json
 import logging
 import os
 import time
+import traceback
 import uuid
 
 import multiprocess as multiprocessing
 
-from ..common.singleton import Singleton
 from ...cli.edge_deployment.client_constants import ClientConstants
 from ...cli.server_deployment.server_constants import ServerConstants
 from ...core.distributed.communication.mqtt.mqtt_manager import MqttManager
 from ...core.mlops.mlops_status import MLOpsStatus
 from ...core.mlops.system_stats import SysStats
 
 
-class MLOpsMetrics(Singleton):
+class MLOpsMetrics(object):
     FEDML_SYS_PERF_RUNNING_FILE_NAME = "sys_perf.id"
 
+    def __new__(cls, *args, **kw):
+        if not hasattr(cls, "_instance"):
+            orig = super(MLOpsMetrics, cls)
+            cls._instance = orig.__new__(cls, *args, **kw)
+            cls._instance.init()
+        return cls._instance
+
     def __init__(self):
+        pass
+
+    def init(self):
+        self.sys_stats_process = None
         self.messenger = None
         self.args = None
         self.run_id = None
         self.edge_id = None
         self.server_agent_id = None
         self.sys_performances = None
-        self.is_sys_perf_reporting = False
+        self.sys_perf_event = None
         self.current_device_status = ClientConstants.MSG_MLOPS_CLIENT_STATUS_OFFLINE
         self.current_run_status = ServerConstants.MSG_MLOPS_SERVER_STATUS_FAILED
-        self.sys_perf_running_file = os.path.join(
-            ClientConstants.get_data_dir(),
-            ClientConstants.LOCAL_RUNNER_INFO_DIR_NAME,
-            MLOpsMetrics.FEDML_SYS_PERF_RUNNING_FILE_NAME,
-        )
 
     def set_messenger(self, msg_messenger, args=None):
         self.messenger = msg_messenger
         if args is not None:
             self.args = args
             self.run_id = args.run_id
-            if args.rank == 0:
+            if args.role == "server":
                 if hasattr(args, "server_id"):
                     self.edge_id = args.server_id
                 else:
                     self.edge_id = 0
 
                 self.sys_perf_running_file = os.path.join(
                     ServerConstants.get_data_dir(),
@@ -127,15 +133,15 @@
         """
         run_id = 0
         if self.run_id is not None:
             run_id = self.run_id
         topic_name = "fl_run/fl_client/mlops/status"
         msg = {"edge_id": edge_id, "run_id": run_id, "status": status}
         message_json = json.dumps(msg)
-        logging.info("report_client_training_status. message_json = %s" % message_json)
+        # logging.info("report_client_training_status. message_json = %s" % message_json)
         MLOpsStatus.get_instance().set_client_status(edge_id, status)
         self.messenger.send_message_json(topic_name, message_json)
 
     def broadcast_client_training_status(self, edge_id, status, is_from_model=False):
         # if not self.comm_sanity_check():
         #     return
         """
@@ -166,17 +172,17 @@
             run_id = self.run_id
         topic_name = "fl_run/fl_client/mlops/status"
         msg = {"edge_id": edge_id, "run_id": run_id, "status": status}
         message_json = json.dumps(msg)
         logging.info("report_client_training_status. message_json = %s" % message_json)
         self.messenger.send_message_json(topic_name, message_json)
 
-    def client_send_exit_train_msg(self, run_id, edge_id, status):
+    def client_send_exit_train_msg(self, run_id, edge_id, status, msg=None):
         topic_exit_train_with_exception = "flserver_agent/" + str(run_id) + "/client_exit_train_with_exception"
-        msg = {"run_id": run_id, "edge_id": edge_id, "status": status}
+        msg = {"run_id": run_id, "edge_id": edge_id, "status": status, "msg": msg if msg is not None else ""}
         message_json = json.dumps(msg)
         logging.info("client_send_exit_train_msg.")
         self.messenger.send_message_json(topic_exit_train_with_exception, message_json)
 
     def report_client_id_status(self, run_id, edge_id, status, running_json=None, is_from_model=False):
         # if not self.comm_sanity_check():
         #     return
@@ -199,15 +205,15 @@
         #     return
         """
         this is used for communication between client agent (FedML cli module) and client
         """
         topic_name = "fl_client/flclient_agent_" + str(edge_id) + "/status"
         msg = {"run_id": run_id, "edge_id": edge_id, "status": status}
         message_json = json.dumps(msg)
-        logging.info("report_client_id_status. message_json = %s" % message_json)
+        # logging.info("report_client_id_status. message_json = %s" % message_json)
         self.messenger.send_message_json(topic_name, message_json)
 
     def report_server_training_status(self, run_id, status, role=None, running_json=None, is_from_model=False):
         # if not self.comm_sanity_check():
         #     return
         self.common_report_server_training_status(run_id, status, role)
 
@@ -250,15 +256,15 @@
             role = "normal"
         msg = {
             "run_id": run_id,
             "edge_id": self.edge_id,
             "status": status,
             "role": role,
         }
-        logging.info("report_server_training_status. msg = %s" % msg)
+        # logging.info("report_server_training_status. msg = %s" % msg)
         message_json = json.dumps(msg)
         MLOpsStatus.get_instance().set_server_status(self.edge_id, status)
         self.messenger.send_message_json(topic_name, message_json)
         self.report_server_id_status(run_id, status)
 
     def broadcast_server_training_status(self, run_id, status, role=None, is_from_model=False):
         if self.messenger is None:
@@ -402,53 +408,37 @@
         #     return
         topic_name = "mlops/runtime_logs/" + str(run_id)
         msg = {"time": time.time()}
         message_json = json.dumps(msg)
         logging.info("report_logs_updated. message_json = %s" % message_json)
         self.messenger.send_message_json(topic_name, message_json)
 
-    def set_sys_reporting_status(self, enable, is_client=True):
-        if is_client:
-            self.sys_perf_running_file = os.path.join(
-                ClientConstants.get_data_dir(),
-                ClientConstants.LOCAL_RUNNER_INFO_DIR_NAME,
-                MLOpsMetrics.FEDML_SYS_PERF_RUNNING_FILE_NAME,
-            )
-        else:
-            self.sys_perf_running_file = os.path.join(
-                ServerConstants.get_data_dir(),
-                ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME,
-                MLOpsMetrics.FEDML_SYS_PERF_RUNNING_FILE_NAME,
-            )
-        self.is_sys_perf_reporting = enable
-        sys_perf_file_handle = open(self.sys_perf_running_file, "w")
-        if sys_perf_file_handle is not None:
-            sys_perf_file_handle.writelines([str(self.is_sys_perf_reporting)])
-            sys_perf_file_handle.flush()
-            sys_perf_file_handle.close()
-
-    def is_system_perf_reporting(self):
-        sys_perf_file_handle = open(self.sys_perf_running_file, "r")
-        if sys_perf_file_handle is not None:
-            self.is_sys_perf_reporting = eval(sys_perf_file_handle.readline())
-            sys_perf_file_handle.close()
-        return self.is_sys_perf_reporting
+    def stop_sys_perf(self):
+        if self.sys_perf_event is not None:
+            self.sys_perf_event.set()
+
+    def setup_sys_perf_process(self, sys_args):
+        self.stop_sys_perf()
+
+        self.args = sys_args
+        if self.sys_perf_event is None:
+            self.sys_perf_event = multiprocessing.Event()
+        self.sys_perf_event.clear()
+
+        self.sys_stats_process = multiprocessing.Process(target=self.report_sys_performances,
+                                                         args=(self.sys_perf_event,))
+        self.sys_stats_process.start()
 
     @staticmethod
-    def report_sys_perf(sys_args, is_client=True):
-        sys_metrics = MLOpsMetrics()
-        sys_metrics.args = sys_args
-        sys_metrics.set_sys_reporting_status(True, is_client)
-        sys_metrics.is_system_perf_reporting()
-        sys_metrics.sys_stats_process = multiprocessing.Process(
-            target=sys_metrics.report_sys_performances
-        )
-        sys_metrics.sys_stats_process.start()
+    def report_sys_perf(sys_args):
+        metrics = MLOpsMetrics()
+        metrics.setup_sys_perf_process(sys_args)
 
-    def report_sys_performances(self):
+    def report_sys_performances(self, sys_event):
+        self.sys_perf_event = sys_event
         self.set_messenger(None, self.args)
         mqtt_mgr = MqttManager(
             self.args.mqtt_config_path["BROKER_HOST"],
             self.args.mqtt_config_path["BROKER_PORT"],
             self.args.mqtt_config_path["MQTT_USER"],
             self.args.mqtt_config_path["MQTT_PWD"],
             180,
@@ -456,29 +446,36 @@
         )
 
         self.set_messenger(mqtt_mgr, self.args)
         mqtt_mgr.connect()
         mqtt_mgr.loop_start()
 
         # Notify MLOps with system information.
-        while self.is_system_perf_reporting() is True:
+        while not self.should_stop_sys_perf():
             try:
                 self.report_system_metric()
             except Exception as e:
+                logging.debug("exception when reporting system pref: {}.".format(traceback.format_exc()))
                 pass
 
             time.sleep(10)
 
         logging.info("System metrics process is about to exit.")
         mqtt_mgr.loop_stop()
         mqtt_mgr.disconnect()
 
     def report_json_message(self, topic, payload):
         self.messenger.send_message_json(topic, payload)
 
+    def should_stop_sys_perf(self):
+        if self.sys_perf_event is not None and self.sys_perf_event.is_set():
+            return True
+
+        return False
+
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter
     )
     parser.add_argument("--run_id", "-r", help="run id")
     parser.add_argument("--client_id", "-c", help="client id")
@@ -495,10 +492,10 @@
     else:
         setattr(args, "rank", 0)
 
     MLOpsMetrics.report_sys_perf(args)
     while True:
         time.sleep(5)
         sys_metrics = MLOpsMetrics()
-        sys_metrics.set_sys_reporting_status(False)
+        sys_metrics.stop_sys_perf()
         break
     pass
```

### Comparing `fedml-0.8.4a9/fedml/core/mlops/mlops_profiler_event.py` & `fedml-0.8.5a1/fedml/core/mlops/mlops_profiler_event.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import json
 import logging
 import threading
 import time
 
 import wandb
 from .mlops_utils import MLOpsUtils
-import datetime
 
 
 class MLOpsProfilerEvent:
     EVENT_TYPE_STARTED = 0
     EVENT_TYPE_ENDED = 1
 
     _instance_lock = threading.Lock()
     _sys_perf_profiling = False
     _enable_wandb = False
-    _ntp_offset = None
 
     def __new__(cls, *args, **kwargs):
         if not hasattr(MLOpsProfilerEvent, "_instance"):
             with MLOpsProfilerEvent._instance_lock:
                 if not hasattr(MLOpsProfilerEvent, "_instance"):
                     MLOpsProfilerEvent._instance = object.__new__(cls)
         return MLOpsProfilerEvent._instance
@@ -71,14 +69,15 @@
             event_value_passed = event_value
 
         if event_edge_id is not None:
             edge_id = event_edge_id
         else:
             edge_id = self.edge_id
 
+        time.sleep(0.1)
         event_topic, event_msg = self.__build_event_mqtt_msg(
             self.args.run_id,
             edge_id,
             MLOpsProfilerEvent.EVENT_TYPE_STARTED,
             event_name,
             event_value_passed,
         )
@@ -93,56 +92,50 @@
             event_value_passed = event_value
 
         if event_edge_id is not None:
             edge_id = event_edge_id
         else:
             edge_id = self.edge_id
 
+        time.sleep(0.1)
         event_topic, event_msg = self.__build_event_mqtt_msg(
             self.args.run_id,
             edge_id,
             MLOpsProfilerEvent.EVENT_TYPE_ENDED,
             event_name,
             event_value_passed,
         )
         event_msg_str = json.dumps(event_msg)
         logging.info("Event ended, {}".format(event_msg_str))
         self.com_manager.send_message_json(event_topic, event_msg_str)
         self.com_manager.send_message_json(event_topic, event_msg_str)
 
     @staticmethod
-    def get_ntp_time():
-        if MLOpsProfilerEvent._ntp_offset is None:
-            MLOpsProfilerEvent._ntp_offset = MLOpsUtils.get_ntp_offset()
-
-        if MLOpsProfilerEvent._ntp_offset is not None:
-            ntp_time_seconds = time.time() + MLOpsProfilerEvent._ntp_offset
-            return ntp_time_seconds
-
-        return time.time()
-
-    @staticmethod
     def __build_event_mqtt_msg(run_id, edge_id, event_type, event_name, event_value):
         event_topic = "mlops/events"
         event_msg = {}
         if event_type == MLOpsProfilerEvent.EVENT_TYPE_STARTED:
-            current_time = MLOpsProfilerEvent.get_ntp_time()
-            if current_time is None:
-                current_time = time.time()
+            current_time_ms = MLOpsUtils.get_ntp_time()
+            if current_time_ms is None:
+                current_time = int(time.time()*1000)
+            else:
+                current_time = int(current_time_ms)
             event_msg = {
                 "run_id": run_id,
                 "edge_id": edge_id,
                 "event_name": event_name,
                 "event_value": event_value,
                 "started_time": int(current_time),
             }
         elif event_type == MLOpsProfilerEvent.EVENT_TYPE_ENDED:
-            current_time = MLOpsProfilerEvent.get_ntp_time()
-            if current_time is None:
-                current_time = time.time()
+            current_time_ms = MLOpsUtils.get_ntp_time()
+            if current_time_ms is None:
+                current_time = int(time.time()*1000)
+            else:
+                current_time = int(current_time_ms)
             event_msg = {
                 "run_id": run_id,
                 "edge_id": edge_id,
                 "event_name": event_name,
                 "event_value": event_value,
                 "ended_time": int(current_time),
             }
```

### Comparing `fedml-0.8.4a9/fedml/core/mlops/mlops_status.py` & `fedml-0.8.5a1/fedml/core/mlops/mlops_status.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/mlops/__init__.py` & `fedml-0.8.5a1/fedml/core/mlops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 from .mlops_profiler_event import MLOpsProfilerEvent
 from .system_stats import SysStats
 from .mlops_status import MLOpsStatus
 from .mlops_runtime_log import MLOpsRuntimeLog
 from .mlops_runtime_log_daemon import MLOpsRuntimeLogProcessor
 from .mlops_runtime_log_daemon import MLOpsRuntimeLogDaemon
 from ...cli.edge_deployment.client_data_interface import FedMLClientDataInterface
+from .mlops_utils import MLOpsUtils
+
 
 FEDML_MLOPS_API_RESPONSE_SUCCESS_CODE = "SUCCESS"
 
 __all__ = [
     "MLOpsMetrics",
     "MLOpsProfilerEvent",
     "SysStats",
@@ -261,14 +263,15 @@
     setup_log_mqtt_mgr()
     MLOpsStore.mlops_metrics.broadcast_client_training_status(MLOpsStore.mlops_edge_id,
                                                               ClientConstants.MSG_MLOPS_CLIENT_STATUS_FINISHED)
     MLOpsStore.mlops_metrics.report_client_id_status(MLOpsStore.mlops_run_id,
                                                      MLOpsStore.mlops_edge_id,
                                                      ClientConstants.MSG_MLOPS_CLIENT_STATUS_FINISHED)
 
+
 def send_exit_train_msg(run_id=None):
     if not mlops_enabled(MLOpsStore.mlops_args):
         return
 
     set_realtime_params()
 
     if not MLOpsStore.mlops_bind_result:
@@ -473,14 +476,19 @@
 
     if sys_args is not None:
         MLOpsStore.mlops_args = sys_args
 
     MLOpsMetrics.report_sys_perf(MLOpsStore.mlops_args)
 
 
+def stop_sys_perf():
+    metrics = MLOpsMetrics()
+    metrics.stop_sys_perf()
+
+
 def log_server_payload(run_id, edge_id, payload):
     if not mlops_enabled(MLOpsStore.mlops_args):
         return
 
     set_realtime_params()
 
     if not mlops_enabled(MLOpsStore.mlops_args):
@@ -704,15 +712,21 @@
     MLOpsStore.mlops_log_mqtt_lock.release()
 
 
 def init_logs(args, edge_id):
     # Init runtime logs
     args.log_file_dir = ClientConstants.get_log_file_dir()
     args.run_id = MLOpsStore.mlops_run_id
-    args.rank = 1
+    if hasattr(args, "rank") and args.rank is not None:
+        if str(args.rank) == "0":
+            args.role = "server"
+        else:
+            args.role = "client"
+    else:
+        args.role = "client"
     client_ids = list()
     client_ids.append(edge_id)
     args.client_id_list = json.dumps(client_ids)
     MLOpsRuntimeLog.get_instance(args).init_logs()
 
     # Start log processor for current run
     MLOpsRuntimeLogDaemon.get_instance(args).start_log_processor(MLOpsStore.mlops_run_id, MLOpsStore.mlops_edge_id)
```

### Comparing `fedml-0.8.4a9/fedml/core/mlops/stats_impl.py` & `fedml-0.8.5a1/fedml/core/mlops/stats_impl.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/mlops/mlops_runtime_log_daemon.py` & `fedml-0.8.5a1/fedml/core/mlops/mlops_runtime_log_daemon.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import argparse
 import json
+
 import multiprocess as multiprocessing
 import os
 import shutil
 import threading
 import time
 
 import requests
 import yaml
 from ...core.mlops.mlops_configs import MLOpsConfigs
 
 
 class MLOpsRuntimeLogProcessor:
     FED_LOG_LINE_NUMS_PER_UPLOADING = 1000
-    FED_LOG_UPLOAD_FREQUENCY = 1
+    FED_LOG_UPLOAD_FREQUENCY = 3
     FEDML_LOG_REPORTING_STATUS_FILE_NAME = "log_status"
     FEDML_RUN_LOG_STATUS_DIR = "run_log_status"
 
     def __init__(self, using_mlops, log_run_id, log_device_id, log_file_dir, log_server_url, in_args=None):
         self.args = in_args
         self.is_log_reporting = False
         self.log_reporting_status_file = os.path.join(log_file_dir,
@@ -48,14 +49,15 @@
         self.log_file_path = os.path.join(self.args.log_file_dir, "fedml-run-"
                                           + str(self.run_id)
                                           + "-edge-"
                                           + str(self.device_id)
                                           + "-upload.log")
         self.run_list = list()
         self.log_source = None
+        self.log_process_event = None
 
     def set_log_source(self, source):
         self.log_source = source
         if source is not None:
             self.log_source = str(self.log_source).replace(' ', '')
 
     @staticmethod
@@ -169,24 +171,31 @@
             log_headers = {'Content-Type': 'application/json', 'Connection': 'close'}
 
             # send log data to the log server
             _, cert_path = MLOpsConfigs.get_instance(self.args).get_request_params()
             if cert_path is not None:
                 try:
                     requests.session().verify = cert_path
+                    # logging.info(f"FedMLDebug POST log to server. run_id {run_id}, device_id {device_id}")
                     response = requests.post(
                         self.log_server_url, json=log_upload_request, verify=True, headers=log_headers
                     )
+                    # logging.info(f"FedMLDebug POST log to server run_id {run_id}, device_id {device_id}. response.status_code: {response.status_code}")
+
                 except requests.exceptions.SSLError as err:
                     MLOpsConfigs.install_root_ca_file()
+                    # logging.info(f"FedMLDebug POST log to server. run_id {run_id}, device_id {device_id}")
                     response = requests.post(
                         self.log_server_url, json=log_upload_request, verify=True, headers=log_headers
                     )
+                    # logging.info(f"FedMLDebug POST log to server run_id {run_id}, device_id {device_id}. response.status_code: {response.status_code}")
             else:
+                # logging.info(f"FedMLDebug POST log to server. run_id {run_id}, device_id {device_id}")
                 response = requests.post(self.log_server_url, headers=log_headers, json=log_upload_request)
+                # logging.info(f"FedMLDebug POST log to server. run_id {run_id}, device_id {device_id}. response.status_code: {response.status_code}")
             if response.status_code != 200:
                 pass
             else:
                 self.log_line_index += (line_end_req - line_start_req)
                 self.log_uploaded_line_index += len(upload_lines)
                 line_count += (line_end_req - line_start_req)
                 line_start_req = line_end_req
@@ -204,23 +213,27 @@
         cur_line_list = str(log_line).split(']')
         if str(log_line).startswith('[FedML-') and \
                 len(cur_line_list) == 5 and (cur_line_list[4] == ' \n'):
             return True
 
         return False
 
-    def log_process(self):
-        self.set_log_reporting_status(True)
-        while self.is_log_reporting_enabled():
+    def log_process(self, process_event):
+        self.log_process_event = process_event
+
+        while not self.should_stop():
             try:
                 time.sleep(MLOpsRuntimeLogProcessor.FED_LOG_UPLOAD_FREQUENCY)
                 self.log_upload(self.run_id, self.device_id)
             except Exception as e:
                 pass
 
+        self.log_upload(self.run_id, self.device_id)
+        print("FedDebug log_process STOPPED")
+
     def log_relocation(self):
         log_line_count = self.log_line_index
         self.log_uploaded_line_index = self.log_line_index
         while log_line_count > 0:
             line = self.log_file.readline()
             if line is None:
                 break
@@ -291,42 +304,19 @@
         try:
             log_config_key = "log_config_{}_{}".format(self.run_id, self.device_id)
             self.log_config = self.__load_yaml_config(self.log_config_file)
             self.log_line_index = self.log_config[log_config_key]["log_line_index"]
         except Exception as e:
             pass
 
-    def set_log_reporting_status(self, enable):
-        self.is_log_reporting = enable
-        log_reporting_status_handle = open(self.log_reporting_status_file, "w")
-        if log_reporting_status_handle is not None:
-            log_reporting_status_handle.writelines([str(self.is_log_reporting)])
-            log_reporting_status_handle.flush()
-            log_reporting_status_handle.close()
-
-    def is_log_reporting_enabled(self):
-        report_status_from_file = False
-        log_reporting_status_handle = open(self.log_reporting_status_file, "r")
-        if log_reporting_status_handle is not None:
-            report_status_from_file = eval(log_reporting_status_handle.readline())
-            log_reporting_status_handle.close()
-
-        origin_log_file_line_num = 0
-        try:
-            for index, line in enumerate(open(self.origin_log_file_path, 'r')):
-                origin_log_file_line_num += 1
-        except Exception as ex:
-            pass
-
-        if report_status_from_file is False and self.log_line_index >= origin_log_file_line_num:
-            self.is_log_reporting = False
-        else:
-            self.is_log_reporting = True
+    def should_stop(self):
+        if self.log_process_event is not None and self.log_process_event.is_set():
+            return True
 
-        return self.is_log_reporting
+        return False
 
 
 class MLOpsRuntimeLogDaemon:
     _log_sdk_instance = None
     _instance_lock = threading.Lock()
 
     def __new__(cls, *args, **kwargs):
@@ -335,15 +325,15 @@
                 if not hasattr(MLOpsRuntimeLogDaemon, "_instance"):
                     MLOpsRuntimeLogDaemon._instance = object.__new__(cls)
         return MLOpsRuntimeLogDaemon._instance
 
     def __init__(self, in_args):
         self.args = in_args
 
-        if in_args.rank == 0:
+        if in_args.role == "server":
             if hasattr(in_args, "server_id"):
                 self.edge_id = in_args.server_id
             else:
                 if hasattr(in_args, "edge_id"):
                     self.edge_id = in_args.edge_id
                 else:
                     self.edge_id = 0
@@ -367,15 +357,17 @@
                 self.log_server_url = "https://open.fedml.ai/fedmlLogsServer/logs/update"
             else:
                 self.log_server_url = self.args.log_server_url
         except Exception as e:
             self.log_server_url = "https://open.fedml.ai/fedmlLogsServer/logs/update"
 
         self.log_file_dir = self.args.log_file_dir
-        self.log_processor_list = list()
+        self.log_child_process_list = list()
+        self.log_child_process = None
+        self.log_process_event = None
 
     @staticmethod
     def get_instance(args):
         if MLOpsRuntimeLogDaemon._log_sdk_instance is None:
             MLOpsRuntimeLogDaemon._log_sdk_instance = MLOpsRuntimeLogDaemon(args)
             MLOpsRuntimeLogDaemon._log_sdk_instance.log_source = None
 
@@ -386,33 +378,47 @@
 
     def start_log_processor(self, log_run_id, log_device_id):
         log_processor = MLOpsRuntimeLogProcessor(self.args.using_mlops, log_run_id,
                                                  log_device_id, self.log_file_dir,
                                                  self.log_server_url,
                                                  in_args=self.args)
         log_processor.set_log_source(self.log_source)
-        process = multiprocessing.Process(target=log_processor.log_process)
+        if self.log_process_event is None:
+            self.log_process_event = multiprocessing.Event()
+        self.log_process_event.clear()
+        log_processor.log_process_event = self.log_process_event
+        self.log_child_process = multiprocessing.Process(target=log_processor.log_process,
+                                                         args=(self.log_process_event,))
         # process = threading.Thread(target=log_processor.log_process)
-        if process is not None:
-            process.start()
-
+        if self.log_child_process is not None:
+            self.log_child_process.start()
             try:
-                self.log_processor_list.index(log_processor)
+                self.log_child_process_list.index((self.log_child_process, log_run_id, log_device_id))
             except ValueError as ex:
-                self.log_processor_list.append(log_processor)
+                self.log_child_process_list.append((self.log_child_process, log_run_id, log_device_id))
 
     def stop_log_processor(self, log_run_id, log_device_id):
-        for log_processor in self.log_processor_list:
-            if str(log_processor.run_id) == str(log_run_id) and str(log_processor.device_id) == str(log_device_id):
-                log_processor.set_log_reporting_status(False)
+        if log_run_id is None or log_device_id is None:
+            return
+
+        # logging.info(f"FedMLDebug. stop log processor. log_run_id = {log_run_id}, log_device_id = {log_device_id}")
+        for (log_child_process, run_id, device_id) in self.log_child_process_list:
+            if str(run_id) == str(log_run_id) and str(device_id) == str(log_device_id):
+                if self.log_process_event is not None:
+                    self.log_process_event.set()
+                else:
+                    log_child_process.terminate()
                 break
 
     def stop_all_log_processor(self):
-        for log_processor in self.log_processor_list:
-            log_processor.set_log_reporting_status(False)
+        for (log_child_process, _, _) in self.log_child_process_list:
+            if self.log_process_event is not None:
+                self.log_process_event.set()
+            else:
+                log_child_process.terminate()
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument("--log_file_dir", "-log", help="log file dir")
     parser.add_argument("--rank", "-r", type=str, default="1")
     parser.add_argument("--client_id_list", "-cil", type=str, default="[]")
```

### Comparing `fedml-0.8.4a9/fedml/core/mlops/system_stats.py` & `fedml-0.8.5a1/fedml/core/mlops/system_stats.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,40 +21,44 @@
         self.process_memory_in_use_size = 0.0
         self.system_memory_utilization = 0.0
         self.cpu_utilization = 0.0
 
     def produce_info(self):
         stats = self.sys_stats_impl.stats()
 
-        self.cpu_utilization = stats["cpu"]
-        self.system_memory_utilization = stats["memory"]
-        self.process_memory_in_use_size = stats["proc.memory.percent"]
-        self.process_memory_in_use = stats["proc.memory.rssMB"]
-        self.process_memory_available = stats["proc.memory.availableMB"]
-        self.process_cpu_threads_in_use = stats["proc.cpu.threads"]
-        self.disk_utilization = stats["disk"]
-        self.network_traffic = stats["network"]["sent"] + stats["network"]["recv"]
+        self.cpu_utilization = stats.get("cpu", 0.0)
+        self.system_memory_utilization = stats.get("memory", 0.0)
+        self.process_memory_in_use_size = stats.get("proc.memory.percent", 0.0)
+        self.process_memory_in_use = stats.get("proc.memory.rssMB", 0.0)
+        self.process_memory_available = stats.get("proc.memory.availableMB", 0.0)
+        self.process_cpu_threads_in_use = stats.get("proc.cpu.threads", 0.0)
+        self.disk_utilization = stats.get("disk", 0.0)
+        network = stats.get("network", None)
+        if network is not None:
+            self.network_traffic = network.get("sent", 0.0) + network.get("recv", 0.0)
 
         for stat_key, stat_value in stats.items():
             if str(stat_key).find("gpu.0.gpu") != -1:
                 if self.sys_stats_impl.gpu_count == 0:
                     self.sys_stats_impl.gpu_count = 1
 
         gpu_mem_used = 0.0
         gpu_usage_total = 0.0
         gpu_mem_allocated = 0.0
         gpu_temperature_total = 0.0
         gpu_power_usage_total = 0.0
-        for i in range(self.sys_stats_impl.gpu_count):
-            gpu_mem_used += stats["gpu.{}.{}".format(i, "memory")]
-            gpu_usage_total += stats["gpu.{}.{}".format(i, "gpu")]
-            gpu_mem_allocated += stats["gpu.{}.{}".format(i, "memoryAllocated")]
-            gpu_temperature_total += stats["gpu.{}.{}".format(i, "temp")]
-            gpu_power_usage_total += stats["gpu.{}.{}".format(i, "powerPercent")]
+
         if self.sys_stats_impl.gpu_count >= 1:
+            for i in range(self.sys_stats_impl.gpu_count):
+                gpu_mem_used += stats.get("gpu.{}.{}".format(i, "memory"), 0.0)
+                gpu_usage_total += stats.get("gpu.{}.{}".format(i, "gpu"), 0.0)
+                gpu_mem_allocated += stats.get("gpu.{}.{}".format(i, "memoryAllocated"), 0.0)
+                gpu_temperature_total += stats.get("gpu.{}.{}".format(i, "temp"), 0.0)
+                gpu_power_usage_total += stats.get("gpu.{}.{}".format(i, "powerPercent"), 0.0)
+
             self.gpu_utilization = round(
                 gpu_usage_total / self.sys_stats_impl.gpu_count, 2
             )
             self.gpu_memory_allocated = round(
                 gpu_mem_allocated / self.sys_stats_impl.gpu_count
             )
             self.gpu_temp = round(gpu_temperature_total / self.sys_stats_impl.gpu_count)
```

### Comparing `fedml-0.8.4a9/fedml/core/mlops/mlops_runtime_log.py` & `fedml-0.8.5a1/fedml/core/mlops/mlops_runtime_log.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import argparse
 import json
 import logging
 import os
 import sys
 import threading
 import time
-import traceback
-
-import ntplib
 import datetime
-from datetime import timezone
 from logging import handlers
 
 from fedml import mlops
 from .mlops_utils import MLOpsUtils
 
 
 class MLOpsRuntimeLog:
@@ -57,15 +53,15 @@
         if hasattr(args, "using_mlops"):
             self.should_write_log_file = args.using_mlops
         else:
             self.should_write_log_file = False
         self.log_file_dir = args.log_file_dir
         self.log_file = None
         self.run_id = args.run_id
-        if args.rank == 0:
+        if args.role == "server":
             if hasattr(args, "server_id"):
                 self.edge_id = args.server_id
             else:
                 if hasattr(args, "edge_id"):
                     self.edge_id = args.edge_id
                 else:
                     self.edge_id = 0
@@ -88,42 +84,58 @@
                     self.edge_id = 0
 
         self.origin_log_file_path = os.path.join(self.log_file_dir, "fedml-run-"
                                                  + str(self.run_id)
                                                  + "-edge-"
                                                  + str(self.edge_id)
                                                  + ".log")
-        self.ntp_offset = None
         sys.excepthook = MLOpsRuntimeLog.handle_exception
 
     @staticmethod
     def get_instance(args):
         if MLOpsRuntimeLog._log_sdk_instance is None:
             MLOpsRuntimeLog._log_sdk_instance = MLOpsRuntimeLog(args)
 
         return MLOpsRuntimeLog._log_sdk_instance
 
     def init_logs(self, show_stdout_log=True):
         log_file_path, program_prefix = MLOpsRuntimeLog.build_log_file_path(self.args)
         logging.raiseExceptions = True
         self.logger = logging.getLogger(log_file_path)
-        format_str = logging.Formatter(fmt="[" + program_prefix + "] [%(asctime)s] [%(levelname)s] "
-                                                                  "[%(filename)s:%(lineno)d:%(funcName)s] %("
-                                                                  "message)s",
-                                       datefmt="%a, %d %b %Y %H:%M:%S")
-        if self.ntp_offset is None:
-            self.ntp_offset = MLOpsUtils.get_ntp_offset()
-        def log_ntp_time(sec, what):
-            if self.ntp_offset is not None:
-                ntp_time_seconds = time.time() + self.ntp_offset
-            else:
-                ntp_time_seconds = time.time()
-            ntp_time = datetime.datetime.fromtimestamp(ntp_time_seconds)
-            return ntp_time.timetuple()
-        logging.Formatter.converter = log_ntp_time
+
+        class MLOpsFormatter(logging.Formatter):
+            converter = datetime.datetime.utcfromtimestamp
+
+            def __init__(self, fmt=None, datefmt=None, style='%', validate=True):
+                super().__init__(fmt, datefmt, style, validate)
+                self.ntp_offset = 0.0
+
+            # Here the `record` is a LogRecord object
+            def formatTime(self, record, datefmt=None):
+                log_time = record.created
+                if record.created is None:
+                    log_time = time.time()
+
+                if self.ntp_offset is None:
+                    self.ntp_offset = 0.0
+
+                log_ntp_time = int((log_time * 1000 + self.ntp_offset) / 1000.0)
+                ct = self.converter(log_ntp_time)
+                if datefmt:
+                    s = ct.strftime(datefmt)
+                else:
+                    s = ct.strftime("%a, %d %b %Y %H:%M:%S")
+                return s
+
+        format_str = MLOpsFormatter(fmt="[" + program_prefix + "] [%(asctime)s] [%(levelname)s] "
+                                                               "[%(filename)s:%(lineno)d:%(funcName)s] %("
+                                                               "message)s",
+                                    datefmt="%a, %d %b %Y %H:%M:%S")
+        format_str.ntp_offset = MLOpsUtils.get_ntp_offset()
+
         stdout_handle = logging.StreamHandler()
         stdout_handle.setFormatter(format_str)
         if show_stdout_log:
             stdout_handle.setLevel(logging.INFO)
             self.logger.setLevel(logging.INFO)
         else:
             stdout_handle.setLevel(logging.CRITICAL)
@@ -140,23 +152,23 @@
             self.logger.addHandler(file_handle)
         logging.root = self.logger
         # Rewrite sys.stdout to redirect stdout (i.e print()) to Logger
         sys.stdout.write = self.logger.info
 
     @staticmethod
     def build_log_file_path(in_args):
-        if in_args.rank == 0:
+        if in_args.role == "server":
             if hasattr(in_args, "server_id"):
                 edge_id = in_args.server_id
             else:
                 if hasattr(in_args, "edge_id"):
                     edge_id = in_args.edge_id
                 else:
                     edge_id = 0
-            program_prefix = "FedML-Server({}) @device-id-{}".format(in_args.rank, edge_id)
+            program_prefix = "FedML-Server @device-id-{}".format(edge_id)
         else:
             if hasattr(in_args, "client_id"):
                 edge_id = in_args.client_id
             elif hasattr(in_args, "client_id_list"):
                 if in_args.client_id_list is None:
                     edge_id = 0
                 else:
```

### Comparing `fedml-0.8.4a9/fedml/core/__init__.py` & `fedml-0.8.5a1/fedml/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/mpc/lightsecagg.py` & `fedml-0.8.5a1/fedml/core/mpc/lightsecagg.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/mpc/secagg.py` & `fedml-0.8.5a1/fedml/core/mpc/secagg.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/dp/mechanisms/dp_mechanism.py` & `fedml-0.8.5a1/fedml/core/dp/mechanisms/dp_mechanism.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/dp/mechanisms/laplace.py` & `fedml-0.8.5a1/fedml/core/dp/mechanisms/laplace.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/dp/mechanisms/gaussian.py` & `fedml-0.8.5a1/fedml/core/dp/mechanisms/gaussian.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/dp/test/test_fed_privacy_mechanism.py` & `fedml-0.8.5a1/fedml/core/dp/test/test_fed_privacy_mechanism.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/dp/fedml_differential_privacy.py` & `fedml-0.8.5a1/fedml/core/dp/fedml_differential_privacy.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/dp/frames/NbAFL.py` & `fedml-0.8.5a1/fedml/core/dp/frames/NbAFL.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/dp/frames/cdp.py` & `fedml-0.8.5a1/fedml/core/dp/frames/cdp.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/dp/frames/base_dp_solution.py` & `fedml-0.8.5a1/fedml/core/dp/frames/base_dp_solution.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/dp/budget_accountant/rdp_analysis.py` & `fedml-0.8.5a1/fedml/core/dp/budget_accountant/rdp_analysis.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/dp/budget_accountant/__init__.py` & `fedml-0.8.5a1/fedml/core/dp/budget_accountant/__init__.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/dp/budget_accountant/rdp_accountant.py` & `fedml-0.8.5a1/fedml/core/dp/budget_accountant/rdp_accountant.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/dp/common/utils.py` & `fedml-0.8.5a1/fedml/core/dp/common/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/contribution/gtg_shapley_value.py` & `fedml-0.8.5a1/fedml/core/contribution/gtg_shapley_value.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/contribution/mr_shapley_value.py` & `fedml-0.8.5a1/fedml/core/contribution/mr_shapley_value.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/contribution/base_contribution_assessor.py` & `fedml-0.8.5a1/fedml/core/contribution/base_contribution_assessor.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/contribution/leave_one_out.py` & `fedml-0.8.5a1/fedml/core/contribution/leave_one_out.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/contribution/contribution_assessor_manager.py` & `fedml-0.8.5a1/fedml/core/contribution/contribution_assessor_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/core/data/noniid_partition.py` & `fedml-0.8.5a1/fedml/core/data/noniid_partition.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/config/simulaton_mpi/fedml_config.yaml` & `fedml-0.8.5a1/fedml/config/simulaton_mpi/fedml_config.yaml`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/config/simulation_sp/fedml_config.yaml` & `fedml-0.8.5a1/fedml/config/simulation_sp/fedml_config.yaml`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/arguments.py` & `fedml-0.8.5a1/fedml/arguments.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/mlops/__init__.py` & `fedml-0.8.5a1/fedml/mlops/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 def init(args):
     mlops.init(args)
 
 
 def event(event_name, event_started=True, event_value=None, event_edge_id=None):
+    logging.info(f"FedMLDebug edge_id = {event_edge_id}, event_name = {event_name}, START = {event_started}")
     mlops.event(event_name, event_started, event_value, event_edge_id)
 
 
 def log(metrics):
     mlops.log(metrics)
 
 
@@ -74,15 +75,22 @@
     mlops.log_client_model_info(round_index, total_rounds, model_url)
 
 
 def log_sys_perf(sys_args=None):
     try:
         mlops.log_sys_perf(sys_args)
     except Exception as e:
-        logging.info("excpetions when logging sys perf: {}".format(traceback.format_exc()))
+        logging.debug("excpetions when logging sys perf: {}".format(traceback.format_exc()))
+
+
+def stop_sys_perf():
+    try:
+        mlops.stop_sys_perf()
+    except Exception as e:
+        logging.debug("excpetions when stopping sys perf: {}".format(traceback.format_exc()))
 
 
 def log_server_payload(run_id, edge_id, payload):
     mlops.log_server_payload(run_id, edge_id, payload)
 
 
 from ..cli.edge_deployment.client_constants import ClientConstants
```

### Comparing `fedml-0.8.4a9/fedml/launch_cheeath.py` & `fedml-0.8.5a1/fedml/launch_cheeath.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/constants.py` & `fedml-0.8.5a1/fedml/constants.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_device/server_mnn/message_define.py` & `fedml-0.8.5a1/fedml/cross_device/server_mnn/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_device/server_mnn/fedml_server_manager.py` & `fedml-0.8.5a1/fedml/cross_device/server_mnn/fedml_server_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,14 +170,15 @@
         for receiver_id in self.client_id_list_in_this_round:
             global_model_url, global_model_key = self.send_message_init_config(
                 receiver_id,
                 self.global_model_file_path,
                 self.data_silo_index_list[client_idx_in_this_round],
                 global_model_url, global_model_key
             )
+            logging.info(f"global_model_url = {global_model_url}, global_model_key = {global_model_key}")
             client_idx_in_this_round += 1
 
         mlops.event("server.wait", event_started=True, event_value=str(self.args.round_idx))
 
         # Todo: for serving the cross-device model,
         #       how to transform it to pytorch and upload the model network to ModelOps
         # mlops.log_training_model_net_info(self.aggregator.aggregator.model)
@@ -298,21 +299,26 @@
             logging.info("=================================================")
 
             mlops.event("server.wait", event_started=False, event_value=str(self.args.round_idx))
 
             mlops.event("server.agg_and_eval", event_started=True, event_value=str(self.args.round_idx))
 
             global_model_params = self.aggregator.aggregate()
+            
+            # self.aggregator.test_on_server_for_all_clients(
+            #     self.args.round_idx, self.global_model_file_path
+            # )
+            
             write_tensor_dict_to_mnn(self.global_model_file_path, global_model_params)
-
-            mlops.event("server.agg_and_eval", event_started=False, event_value=str(self.args.round_idx))
-
-            self.aggregator.test_on_server_for_all_clients(
+            self.aggregator.test_on_server_for_all_clients_mnn(
                 self.global_model_file_path, self.args.round_idx
             )
+            
+            mlops.event("server.agg_and_eval", event_started=False, event_value=str(self.args.round_idx))
+
 
             # send round info to the MQTT backend
             mlops.log_round_info(self.round_num, self.args.round_idx)
 
             self.client_id_list_in_this_round = self.aggregator.client_selection(
                 self.args.round_idx, self.client_real_ids, self.args.client_num_per_round
             )
```

### Comparing `fedml-0.8.4a9/fedml/cross_device/server_mnn/utils.py` & `fedml-0.8.5a1/fedml/cross_device/server_mnn/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_device/server_mnn/fedml_aggregator.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedopt/FedOptAggregator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,188 +1,220 @@
+import copy
+import logging
+import random
 import time
 
-import MNN
 import numpy as np
+import torch
 import wandb
 
-import fedml
-from fedml import mlops
-
-F = MNN.expr
-nn = MNN.nn
+from .optrepo import OptRepo
+from .utils import transform_list_to_tensor
 
-from .utils import read_mnn_as_tensor_dict
-import logging
 
-
-class FedMLAggregator(object):
+class FedOptAggregator(object):
     def __init__(
-        self, test_dataloader, worker_num, device, args, aggregator,
+        self,
+        train_global,
+        test_global,
+        all_train_data_num,
+        train_data_local_dict,
+        test_data_local_dict,
+        train_data_local_num_dict,
+        worker_num,
+        device,
+        args,
+        server_aggregator,
     ):
-        self.aggregator = aggregator
+        self.aggregator = server_aggregator
 
         self.args = args
-        self.test_global = test_dataloader
+        self.train_global = train_global
+        self.test_global = test_global
+        self.val_global = self._generate_validation_set()
+        self.all_train_data_num = all_train_data_num
+
+        self.train_data_local_dict = train_data_local_dict
+        self.test_data_local_dict = test_data_local_dict
+        self.train_data_local_num_dict = train_data_local_num_dict
 
         self.worker_num = worker_num
         self.device = device
         self.model_dict = dict()
         self.sample_num_dict = dict()
         self.flag_client_model_uploaded_dict = dict()
+        self.opt = self._instantiate_opt()
         for idx in range(self.worker_num):
             self.flag_client_model_uploaded_dict[idx] = False
 
+    def _instantiate_opt(self):
+        return OptRepo.name2cls(self.args.server_optimizer)(
+            filter(lambda p: p.requires_grad, self.get_model_params()),
+            lr=self.args.server_lr,
+            momentum=self.args.server_momentum,
+        )
+
+    def get_model_params(self):
+        # return model parameters in type of generator
+        return self.aggregator.model.parameters()
+
     def get_global_model_params(self):
+        # return model parameters in type of ordered_dict
         return self.aggregator.get_model_params()
 
-    # TODO: refactor MNN-related file processing
-    def get_global_model_params_file(self):
-        return self.aggregator.get_model_params_file()
-
     def set_global_model_params(self, model_parameters):
         self.aggregator.set_model_params(model_parameters)
 
     def add_local_trained_result(self, index, model_params, sample_num):
         logging.info("add_model. index = %d" % index)
         self.model_dict[index] = model_params
         self.sample_num_dict[index] = sample_num
         self.flag_client_model_uploaded_dict[index] = True
 
     def check_whether_all_receive(self):
-        logging.info("worker_num = {}".format(self.worker_num))
         for idx in range(self.worker_num):
             if not self.flag_client_model_uploaded_dict[idx]:
                 return False
         for idx in range(self.worker_num):
             self.flag_client_model_uploaded_dict[idx] = False
         return True
 
     def aggregate(self):
         start_time = time.time()
         model_list = []
         training_num = 0
 
         for idx in range(self.worker_num):
-            logging.info("self.model_dict[idx] = {}".format(self.model_dict[idx]))
-            mnn_file_path = self.model_dict[idx]
-            tensor_params_dict = read_mnn_as_tensor_dict(mnn_file_path)
-            model_list.append((self.sample_num_dict[idx], tensor_params_dict))
+            model_list.append((self.sample_num_dict[idx], self.model_dict[idx]))
             training_num += self.sample_num_dict[idx]
-        logging.info("training_num = {}".format(training_num))
+
         logging.info("len of self.model_dict[idx] = " + str(len(self.model_dict)))
 
         # logging.info("################aggregate: %d" % len(model_list))
         (num0, averaged_params) = model_list[0]
         for k in averaged_params.keys():
             for i in range(0, len(model_list)):
                 local_sample_number, local_model_params = model_list[i]
                 w = local_sample_number / training_num
                 if i == 0:
                     averaged_params[k] = local_model_params[k] * w
                 else:
                     averaged_params[k] += local_model_params[k] * w
 
+        # server optimizer
+        # save optimizer state
+        self.opt.zero_grad()
+        opt_state = self.opt.state_dict()
+        # set new aggregated grad
+        self.set_model_global_grads(averaged_params)
+        self.opt = self._instantiate_opt()
+        # load optimizer state
+        self.opt.load_state_dict(opt_state)
+        self.opt.step()
+
         end_time = time.time()
         logging.info("aggregate time cost: %d" % (end_time - start_time))
-        return averaged_params
-
-    def data_silo_selection(self, round_idx, data_silo_num_in_total, client_num_in_total):
-        """
+        return self.get_global_model_params()
 
-        Args:
-            round_idx: round index, starting from 0
-            data_silo_num_in_total: this is equal to the users in a synthetic data,
-                                    e.g., in synthetic_1_1, this value is 30
-            client_num_in_total: the number of edge devices that can train
-
-        Returns:
-            data_silo_index_list: e.g., when data_silo_num_in_total = 30, client_num_in_total = 3,
-                                        this value is the form of [0, 11, 20]
-
-        """
-        logging.info(
-            "data_silo_num_in_total = %d, client_num_in_total = %d" % (data_silo_num_in_total, client_num_in_total)
-        )
-        assert data_silo_num_in_total >= client_num_in_total
-        if client_num_in_total == data_silo_num_in_total:
-            return [i for i in range(data_silo_num_in_total)]
-        else:
-            np.random.seed(round_idx)  # make sure for each comparison, we are selecting the same clients each round
-            data_silo_index_list = np.random.choice(range(data_silo_num_in_total), client_num_in_total, replace=False)
-        return data_silo_index_list
-
-    def client_selection(self, round_idx, client_id_list_in_total, client_num_per_round):
-        """
-        Args:
-            round_idx: round index, starting from 0
-            client_id_list_in_total: this is the real edge IDs.
-                                    In MLOps, its element is real edge ID, e.g., [64, 65, 66, 67];
-                                    in simulated mode, its element is client index starting from 0, e.g., [0, 1, 2, 3]
-            client_num_per_round:
-
-        Returns:
-            client_id_list_in_this_round: sampled real edge ID list, e.g., [64, 66]
-        """
-        if client_num_per_round == len(client_id_list_in_total) or len(client_id_list_in_total) == 1:  # for debugging
-            return client_id_list_in_total
-        np.random.seed(round_idx)  # make sure for each comparison, we are selecting the same clients each round
-        client_id_list_in_this_round = np.random.choice(client_id_list_in_total, client_num_per_round, replace=False)
-        return client_id_list_in_this_round
+    def set_model_global_grads(self, new_state):
+        new_model = copy.deepcopy(self.aggregator.model)
+        new_model.load_state_dict(new_state)
+        with torch.no_grad():
+            for parameter, new_parameter in zip(self.aggregator.model.parameters(), new_model.parameters()):
+                parameter.grad = parameter.data - new_parameter.data
+                # because we go to the opposite direction of the gradient
+        model_state_dict = self.aggregator.model.state_dict()
+        new_model_state_dict = new_model.state_dict()
+        for k in dict(self.aggregator.model.named_parameters()).keys():
+            new_model_state_dict[k] = model_state_dict[k]
+        # self.trainer.model.load_state_dict(new_model_state_dict)
+        self.set_global_model_params(new_model_state_dict)
 
     def client_sampling(self, round_idx, client_num_in_total, client_num_per_round):
         if client_num_in_total == client_num_per_round:
             client_indexes = [client_index for client_index in range(client_num_in_total)]
         else:
             num_clients = min(client_num_per_round, client_num_in_total)
             np.random.seed(round_idx)  # make sure for each comparison, we are selecting the same clients each round
             client_indexes = np.random.choice(range(client_num_in_total), num_clients, replace=False)
         logging.info("client_indexes = %s" % str(client_indexes))
         return client_indexes
 
-    def test_on_server_for_all_clients(self, mnn_file_path, round_idx):
-        # load global model from MNN
-        var_map = F.load_as_dict(mnn_file_path)
-        input_dicts, output_dicts = F.get_inputs_and_outputs(var_map)
-        input_names = [n for n in input_dicts.keys()]
-        output_names = [n for n in output_dicts.keys()]
-        input_vars = [input_dicts[n] for n in input_names]
-        output_vars = [output_dicts[n] for n in output_names]
-        module = MNN.nn.load_module(input_vars, output_vars, False)
-
-        module.train(False)
-        self.test_global.reset()
-
-        correct = 0
-        for i in range(self.test_global.iter_number):
-            example = self.test_global.next()
-            input_data = example[0]
-            output_target = example[1]
-            data = input_data[0]  # which input, model may have more than one inputs
-            label = output_target[0]  # also, model may have more than one outputs
-
-            result = module.forward(data)
-            predict = F.argmax(result, 1)
-            predict = np.array(predict.read())
-
-            label_test = np.array(label.read())
-            correct += np.sum(label_test == predict)
-
-            target = F.one_hot(F.cast(label, F.int), 10, 1, 0)
-            loss = nn.loss.cross_entropy(result, target)
-
-        test_accuracy = correct * 100.0 / self.test_global.size
-        test_loss = loss.read()
-        fedml.logging.info("test acc = {}".format(test_accuracy))
-        fedml.logging.info("test loss = {}".format(test_loss))
-
-        mlops.log(
-            {
-                "round_idx": round_idx,
-                "accuracy": round(np.round(test_accuracy, 4), 4),
-                "loss": round(np.round(test_loss, 4)),
-            }
-        )
+    def _generate_validation_set(self, num_samples=10000):
+        if self.args.dataset.startswith("stackoverflow"):
+            test_data_num = len(self.test_global.dataset)
+            sample_indices = random.sample(range(test_data_num), min(num_samples, test_data_num))
+            subset = torch.utils.data.Subset(self.test_global.dataset, sample_indices)
+            sample_testset = torch.utils.data.DataLoader(subset, batch_size=self.args.batch_size)
+            return sample_testset
+        else:
+            return self.test_global
 
-        if self.args.enable_wandb:
-            wandb.log(
-                {"round idx": round_idx, "test acc": test_accuracy, "test loss": test_loss,}
+    def test_on_server_for_all_clients(self, round_idx):
+        if self.aggregator.test_all(
+            self.train_data_local_dict,
+            self.test_data_local_dict,
+            self.device,
+            self.args,
+        ):
+            return
+
+        if (
+            round_idx % self.args.frequency_of_the_test == 0
+            or round_idx == self.args.comm_round - 1
+        ):
+            logging.info(
+                "################test_on_server_for_all_clients : {}".format(round_idx)
+            )
+            train_num_samples = []
+            train_tot_corrects = []
+            train_losses = []
+            for client_idx in range(self.args.client_num_in_total):
+                # train data
+                metrics = self.aggregator.test(
+                    self.train_data_local_dict[client_idx], self.device, self.args
+                )
+                train_tot_correct, train_num_sample, train_loss = (
+                    metrics["test_correct"],
+                    metrics["test_total"],
+                    metrics["test_loss"],
+                )
+                train_tot_corrects.append(copy.deepcopy(train_tot_correct))
+                train_num_samples.append(copy.deepcopy(train_num_sample))
+                train_losses.append(copy.deepcopy(train_loss))
+
+            # test on training dataset
+            train_acc = sum(train_tot_corrects) / sum(train_num_samples)
+            train_loss = sum(train_losses) / sum(train_num_samples)
+            if self.args.enable_wandb:
+                wandb.log({"Train/Acc": train_acc, "round": round_idx})
+                wandb.log({"Train/Loss": train_loss, "round": round_idx})
+            stats = {"training_acc": train_acc, "training_loss": train_loss}
+            logging.info(stats)
+
+            # test data
+            test_num_samples = []
+            test_tot_corrects = []
+            test_losses = []
+
+            if round_idx == self.args.comm_round - 1:
+                metrics = self.aggregator.test(self.test_global, self.device, self.args)
+            else:
+                metrics = self.aggregator.test(self.val_global, self.device, self.args)
+
+            test_tot_correct, test_num_sample, test_loss = (
+                metrics["test_correct"],
+                metrics["test_total"],
+                metrics["test_loss"],
             )
+            test_tot_corrects.append(copy.deepcopy(test_tot_correct))
+            test_num_samples.append(copy.deepcopy(test_num_sample))
+            test_losses.append(copy.deepcopy(test_loss))
+
+            # test on test dataset
+            test_acc = sum(test_tot_corrects) / sum(test_num_samples)
+            test_loss = sum(test_losses) / sum(test_num_samples)
+            if self.args.enable_wandb:
+                wandb.log({"Test/Acc": test_acc, "round": round_idx})
+                wandb.log({"Test/Loss": test_loss, "round": round_idx})
+            stats = {"test_acc": test_acc, "test_loss": test_loss}
+            logging.info(stats)
```

### Comparing `fedml-0.8.4a9/fedml/cross_device/server_mnn/server_mnn_api.py` & `fedml-0.8.5a1/fedml/cross_device/server_mnn/server_mnn_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cross_device/mnn_server.py` & `fedml-0.8.5a1/fedml/cross_device/mnn_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/centralized/centralized_trainer.py` & `fedml-0.8.5a1/fedml/centralized/centralized_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/launch_simulation.py` & `fedml-0.8.5a1/fedml/launch_simulation.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/fedavg/client.py` & `fedml-0.8.5a1/fedml/simulation/sp/fedavg/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/fedavg/fedavg_api.py` & `fedml-0.8.5a1/fedml/simulation/sp/fedavg/fedavg_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/fedprox/client.py` & `fedml-0.8.5a1/fedml/simulation/sp/fedprox/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/fedprox/fedprox_trainer.py` & `fedml-0.8.5a1/fedml/simulation/sp/fedprox/fedprox_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/turboaggregate/TA_trainer.py` & `fedml-0.8.5a1/fedml/simulation/sp/turboaggregate/TA_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/turboaggregate/mpc_function.py` & `fedml-0.8.5a1/fedml/simulation/sp/turboaggregate/mpc_function.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/turboaggregate/TA_client.py` & `fedml-0.8.5a1/fedml/simulation/sp/turboaggregate/TA_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/feddyn/client copy.py` & `fedml-0.8.5a1/fedml/simulation/sp/feddyn/client copy.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/feddyn/client.py` & `fedml-0.8.5a1/fedml/simulation/sp/feddyn/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/feddyn/feddyn_trainer copy.py` & `fedml-0.8.5a1/fedml/simulation/sp/feddyn/feddyn_trainer copy.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/feddyn/feddyn_trainer.py` & `fedml-0.8.5a1/fedml/simulation/sp/feddyn/feddyn_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/classical_vertical_fl/client.py` & `fedml-0.8.5a1/fedml/simulation/sp/classical_vertical_fl/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/classical_vertical_fl/party_models.py` & `fedml-0.8.5a1/fedml/simulation/sp/classical_vertical_fl/party_models.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/classical_vertical_fl/vfl.py` & `fedml-0.8.5a1/fedml/simulation/sp/classical_vertical_fl/vfl.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/classical_vertical_fl/vfl_api.py` & `fedml-0.8.5a1/fedml/simulation/sp/classical_vertical_fl/vfl_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/classical_vertical_fl/vfl_fixture.py` & `fedml-0.8.5a1/fedml/simulation/sp/classical_vertical_fl/vfl_fixture.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/fednova/fednova.py` & `fedml-0.8.5a1/fedml/simulation/sp/fednova/fednova.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/fednova/fednova_trainer.py` & `fedml-0.8.5a1/fedml/simulation/sp/fednova/fednova_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/fednova/fednova_api.py` & `fedml-0.8.5a1/fedml/simulation/sp/fednova/fednova_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/fednova/client.py` & `fedml-0.8.5a1/fedml/simulation/sp/fednova/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/fednova/comm_helpers.py` & `fedml-0.8.5a1/fedml/simulation/sp/fednova/comm_helpers.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/fedopt/fedopt_api.py` & `fedml-0.8.5a1/fedml/simulation/sp/fedopt/fedopt_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/fedopt/client.py` & `fedml-0.8.5a1/fedml/simulation/sp/fedopt/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/fedopt/optrepo.py` & `fedml-0.8.5a1/fedml/simulation/sp/fedopt/optrepo.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/hierarchical_fl/client.py` & `fedml-0.8.5a1/fedml/simulation/sp/hierarchical_fl/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/hierarchical_fl/group.py` & `fedml-0.8.5a1/fedml/simulation/sp/hierarchical_fl/group.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/hierarchical_fl/trainer.py` & `fedml-0.8.5a1/fedml/simulation/sp/hierarchical_fl/trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/mime/client.py` & `fedml-0.8.5a1/fedml/simulation/sp/mime/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/mime/opt_utils.py` & `fedml-0.8.5a1/fedml/simulation/sp/mime/opt_utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/mime/mime_trainer.py` & `fedml-0.8.5a1/fedml/simulation/sp/mime/mime_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/scaffold/scaffold_trainer.py` & `fedml-0.8.5a1/fedml/simulation/sp/scaffold/scaffold_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,20 @@
                 elif c_global_para[key].type() == 'torch.cuda.LongTensor':
                     c_global_para[key] += total_c_delta_para[key].type(torch.cuda.LongTensor)
                 else:
                     c_global_para[key] += total_c_delta_para[key]
             self.c_model_global.load_state_dict(c_global_para)
 
             for key in w_global.keys():
-                w_global[key] += total_weights_delta[key] * self.args.server_lr
+                if w_global[key].type() == 'torch.LongTensor':
+                    w_global[key] += (total_weights_delta[key] * self.args.server_lr).type(torch.LongTensor)
+                elif w_global[key].type() == 'torch.cuda.LongTensor':
+                    w_global[key] += (total_weights_delta[key] * self.args.server_lr).type(torch.cuda.LongTensor)
+                else:
+                    w_global[key] += total_weights_delta[key] * self.args.server_lr
 
             self.model_trainer.set_model_params(w_global)
             mlops.event("agg", event_started=False, event_value=str(round_idx))
 
             # test results
             # at last round
             if round_idx == self.args.comm_round - 1:
```

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/scaffold/client.py` & `fedml-0.8.5a1/fedml/simulation/sp/scaffold/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/decentralized/decentralized_fl_api.py` & `fedml-0.8.5a1/fedml/simulation/sp/decentralized/decentralized_fl_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/decentralized/client_dsgd.py` & `fedml-0.8.5a1/fedml/simulation/sp/decentralized/client_dsgd.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/decentralized/client_pushsum.py` & `fedml-0.8.5a1/fedml/simulation/sp/decentralized/client_pushsum.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/sp/decentralized/topology_manager.py` & `fedml-0.8.5a1/fedml/simulation/sp/decentralized/topology_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedavg/FedAvgClientManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedavg/FedAvgClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedavg/message_define.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedavg/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedavg/FedAVGAggregator.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedavg/FedAVGAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedavg/FedAvgAPI.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedavg/FedAvgAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedavg/utils.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedavg/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedavg/FedAVGTrainer.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedavg/FedAVGTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedavg/FedAvgServerManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedavg/FedAvgServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/split_nn/server.py` & `fedml-0.8.5a1/fedml/simulation/mpi/split_nn/server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/split_nn/SplitNNAPI.py` & `fedml-0.8.5a1/fedml/simulation/mpi/split_nn/SplitNNAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/split_nn/message_define.py` & `fedml-0.8.5a1/fedml/simulation/mpi/split_nn/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/split_nn/client.py` & `fedml-0.8.5a1/fedml/simulation/mpi/split_nn/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/split_nn/client_manager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/split_nn/client_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/split_nn/server_manager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/split_nn/server_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedprox/message_define.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedprox/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedprox/FedProxTrainer.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedprox/FedProxTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedprox/FedProxClientManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedprox/FedProxClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedprox/FedProxAggregator.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedprox/FedProxAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedprox/utils.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedprox/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedprox/FedProxServerManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedprox/FedProxServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedprox/FedProxAPI.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedprox/FedProxAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedgan/FedGanServerManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedgan/FedGanServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedgan/FedGanAPI.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedgan/FedGanAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedgan/message_define.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedgan/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedgan/gan_trainer.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedgan/gan_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedgan/utils.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedgan/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedgan/FedGANTrainer.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedgan/FedGANTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedgan/FedGANAggregator.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedgan/FedGANAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedgan/FedGanClientManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedgan/FedGanClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedgkt/GKTServerTrainer.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedgkt/GKTServerTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedgkt/FedGKTAPI.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedgkt/FedGKTAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedgkt/GKTServerManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedgkt/GKTServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedgkt/utils.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedgkt/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedgkt/message_def.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedgkt/message_def.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedgkt/GKTClientManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedgkt/GKTClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedgkt/GKTClientTrainer.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedgkt/GKTClientTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/base_framework/client_manager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/base_framework/client_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/base_framework/central_worker.py` & `fedml-0.8.5a1/fedml/simulation/mpi/base_framework/central_worker.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/base_framework/algorithm_api.py` & `fedml-0.8.5a1/fedml/simulation/mpi/base_framework/algorithm_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/base_framework/central_manager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/base_framework/central_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/message_define.py` & `fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/MyModelTrainer.py` & `fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/MyModelTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/AsyncFedAvgServerManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/AsyncFedAvgServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/my_model_trainer_nwp.py` & `fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/my_model_trainer_nwp.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/AsyncFedAvgClientManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/AsyncFedAvgClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/utils.py` & `fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/AsyncFedAVGTrainer.py` & `fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/AsyncFedAVGTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/AsyncFedAvgSeqAPI.py` & `fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/AsyncFedAvgSeqAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/AsyncFedAVGAggregator.py` & `fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/AsyncFedAVGAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/my_model_trainer.py` & `fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/my_model_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/my_model_trainer_tag_prediction.py` & `fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/my_model_trainer_tag_prediction.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/async_fedavg/my_model_trainer_classification.py` & `fedml-0.8.5a1/fedml/simulation/mpi/async_fedavg/my_model_trainer_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedavg_seq/FedAvgClientManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedavg_seq/FedAvgClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedavg_seq/message_define.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedavg_seq/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedavg_seq/FedAvgSeqAPI.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedavg_seq/FedAvgSeqAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedavg_seq/FedAVGAggregator.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedavg_seq/FedAVGAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedavg_seq/utils.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedavg_seq/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedavg_seq/FedAVGTrainer.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedavg_seq/FedAVGTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedavg_seq/FedAvgServerManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedavg_seq/FedAvgServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedavg_seq/my_model_trainer_classification.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedavg_seq/my_model_trainer_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/decentralized_framework/decentralized_worker.py` & `fedml-0.8.5a1/fedml/simulation/mpi/decentralized_framework/decentralized_worker.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/decentralized_framework/decentralized_worker_manager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/decentralized_framework/decentralized_worker_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/decentralized_framework/algorithm_api.py` & `fedml-0.8.5a1/fedml/simulation/mpi/decentralized_framework/algorithm_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/classical_vertical_fl/guest_trainer.py` & `fedml-0.8.5a1/fedml/simulation/mpi/classical_vertical_fl/guest_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/classical_vertical_fl/guest_manager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/classical_vertical_fl/guest_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/classical_vertical_fl/vfl_api.py` & `fedml-0.8.5a1/fedml/simulation/mpi/classical_vertical_fl/vfl_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/classical_vertical_fl/host_trainer.py` & `fedml-0.8.5a1/fedml/simulation/mpi/classical_vertical_fl/host_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/classical_vertical_fl/host_manager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/classical_vertical_fl/host_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fednas/FedNASAggregator.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fednas/FedNASAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fednas/FedNASClientManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fednas/FedNASClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fednas/FedNASAPI.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fednas/FedNASAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fednas/FedNASTrainer.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fednas/FedNASTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fednas/message_define.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fednas/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fednas/FedNASServerManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fednas/FedNASServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fednova/FedNovaAPI.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fednova/FedNovaAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fednova/message_define.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fednova/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fednova/FedNovaServerManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fednova/FedNovaServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fednova/FedNovaTrainer.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fednova/FedNovaTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fednova/utils.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fednova/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fednova/FedNovaClientManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fednova/FedNovaClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fednova/FedNovaAggregator.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fednova/FedNovaAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fednova/my_model_trainer_classification.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fednova/my_model_trainer_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedopt/FedOptAggregator.py` & `fedml-0.8.5a1/fedml/cross_silo/client/fedml_client_master_manager.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,220 +1,187 @@
-import copy
+import json
 import logging
-import random
+import platform
 import time
 
-import numpy as np
-import torch
-import wandb
-
-from .optrepo import OptRepo
-from .utils import transform_list_to_tensor
-
-
-class FedOptAggregator(object):
-    def __init__(
-        self,
-        train_global,
-        test_global,
-        all_train_data_num,
-        train_data_local_dict,
-        test_data_local_dict,
-        train_data_local_num_dict,
-        worker_num,
-        device,
-        args,
-        server_aggregator,
-    ):
-        self.aggregator = server_aggregator
+import torch.distributed as dist
 
+from fedml import mlops
+from fedml.constants import FEDML_CROSS_SILO_SCENARIO_HIERARCHICAL
+from .message_define import MyMessage
+from .utils import convert_model_params_from_ddp, convert_model_params_to_ddp
+from ...core.distributed.fedml_comm_manager import FedMLCommManager
+from ...core.distributed.communication.message import Message
+from ...core.mlops.mlops_profiler_event import MLOpsProfilerEvent
+
+
+class ClientMasterManager(FedMLCommManager):
+    ONLINE_STATUS_FLAG = "ONLINE"
+    RUN_FINISHED_STATUS_FLAG = "FINISHED"
+
+    def __init__(self, args, trainer_dist_adapter, comm=None, rank=0, size=0, backend="MPI"):
+        super().__init__(args, comm, rank, size, backend)
+        self.trainer_dist_adapter = trainer_dist_adapter
         self.args = args
-        self.train_global = train_global
-        self.test_global = test_global
-        self.val_global = self._generate_validation_set()
-        self.all_train_data_num = all_train_data_num
-
-        self.train_data_local_dict = train_data_local_dict
-        self.test_data_local_dict = test_data_local_dict
-        self.train_data_local_num_dict = train_data_local_num_dict
-
-        self.worker_num = worker_num
-        self.device = device
-        self.model_dict = dict()
-        self.sample_num_dict = dict()
-        self.flag_client_model_uploaded_dict = dict()
-        self.opt = self._instantiate_opt()
-        for idx in range(self.worker_num):
-            self.flag_client_model_uploaded_dict[idx] = False
-
-    def _instantiate_opt(self):
-        return OptRepo.name2cls(self.args.server_optimizer)(
-            filter(lambda p: p.requires_grad, self.get_model_params()),
-            lr=self.args.server_lr,
-            momentum=self.args.server_momentum,
+
+        self.num_rounds = args.comm_round
+        self.round_idx = 0
+        self.rank = rank
+        self.client_real_ids = json.loads(args.client_id_list)
+        logging.info("self.client_real_ids = {}".format(self.client_real_ids))
+        # for the client, len(self.client_real_ids)==1: we only specify its client id in the list, not including others.
+        self.client_real_id = self.client_real_ids[0]
+
+        self.has_sent_online_msg = False
+        self.is_inited = False
+
+    def is_main_process(self):
+        return getattr(self.trainer_dist_adapter, "trainer", None) is None or \
+            getattr(self.trainer_dist_adapter.trainer, "trainer", None) is None or \
+            self.trainer_dist_adapter.trainer.trainer.is_main_process()
+
+    def register_message_receive_handlers(self):
+        self.register_message_receive_handler(
+            MyMessage.MSG_TYPE_CONNECTION_IS_READY, self.handle_message_connection_ready
         )
 
-    def get_model_params(self):
-        # return model parameters in type of generator
-        return self.aggregator.model.parameters()
-
-    def get_global_model_params(self):
-        # return model parameters in type of ordered_dict
-        return self.aggregator.get_model_params()
-
-    def set_global_model_params(self, model_parameters):
-        self.aggregator.set_model_params(model_parameters)
-
-    def add_local_trained_result(self, index, model_params, sample_num):
-        logging.info("add_model. index = %d" % index)
-        self.model_dict[index] = model_params
-        self.sample_num_dict[index] = sample_num
-        self.flag_client_model_uploaded_dict[index] = True
-
-    def check_whether_all_receive(self):
-        for idx in range(self.worker_num):
-            if not self.flag_client_model_uploaded_dict[idx]:
-                return False
-        for idx in range(self.worker_num):
-            self.flag_client_model_uploaded_dict[idx] = False
-        return True
-
-    def aggregate(self):
-        start_time = time.time()
-        model_list = []
-        training_num = 0
-
-        for idx in range(self.worker_num):
-            model_list.append((self.sample_num_dict[idx], self.model_dict[idx]))
-            training_num += self.sample_num_dict[idx]
-
-        logging.info("len of self.model_dict[idx] = " + str(len(self.model_dict)))
-
-        # logging.info("################aggregate: %d" % len(model_list))
-        (num0, averaged_params) = model_list[0]
-        for k in averaged_params.keys():
-            for i in range(0, len(model_list)):
-                local_sample_number, local_model_params = model_list[i]
-                w = local_sample_number / training_num
-                if i == 0:
-                    averaged_params[k] = local_model_params[k] * w
-                else:
-                    averaged_params[k] += local_model_params[k] * w
-
-        # server optimizer
-        # save optimizer state
-        self.opt.zero_grad()
-        opt_state = self.opt.state_dict()
-        # set new aggregated grad
-        self.set_model_global_grads(averaged_params)
-        self.opt = self._instantiate_opt()
-        # load optimizer state
-        self.opt.load_state_dict(opt_state)
-        self.opt.step()
-
-        end_time = time.time()
-        logging.info("aggregate time cost: %d" % (end_time - start_time))
-        return self.get_global_model_params()
-
-    def set_model_global_grads(self, new_state):
-        new_model = copy.deepcopy(self.aggregator.model)
-        new_model.load_state_dict(new_state)
-        with torch.no_grad():
-            for parameter, new_parameter in zip(self.aggregator.model.parameters(), new_model.parameters()):
-                parameter.grad = parameter.data - new_parameter.data
-                # because we go to the opposite direction of the gradient
-        model_state_dict = self.aggregator.model.state_dict()
-        new_model_state_dict = new_model.state_dict()
-        for k in dict(self.aggregator.model.named_parameters()).keys():
-            new_model_state_dict[k] = model_state_dict[k]
-        # self.trainer.model.load_state_dict(new_model_state_dict)
-        self.set_global_model_params(new_model_state_dict)
-
-    def client_sampling(self, round_idx, client_num_in_total, client_num_per_round):
-        if client_num_in_total == client_num_per_round:
-            client_indexes = [client_index for client_index in range(client_num_in_total)]
-        else:
-            num_clients = min(client_num_per_round, client_num_in_total)
-            np.random.seed(round_idx)  # make sure for each comparison, we are selecting the same clients each round
-            client_indexes = np.random.choice(range(client_num_in_total), num_clients, replace=False)
-        logging.info("client_indexes = %s" % str(client_indexes))
-        return client_indexes
-
-    def _generate_validation_set(self, num_samples=10000):
-        if self.args.dataset.startswith("stackoverflow"):
-            test_data_num = len(self.test_global.dataset)
-            sample_indices = random.sample(range(test_data_num), min(num_samples, test_data_num))
-            subset = torch.utils.data.Subset(self.test_global.dataset, sample_indices)
-            sample_testset = torch.utils.data.DataLoader(subset, batch_size=self.args.batch_size)
-            return sample_testset
-        else:
-            return self.test_global
+        self.register_message_receive_handler(
+            MyMessage.MSG_TYPE_S2C_CHECK_CLIENT_STATUS, self.handle_message_check_status
+        )
+
+        self.register_message_receive_handler(MyMessage.MSG_TYPE_S2C_INIT_CONFIG, self.handle_message_init)
+        self.register_message_receive_handler(
+            MyMessage.MSG_TYPE_S2C_SYNC_MODEL_TO_CLIENT, self.handle_message_receive_model_from_server,
+        )
+
+        self.register_message_receive_handler(
+            MyMessage.MSG_TYPE_S2C_FINISH, self.handle_message_finish,
+        )
+
+    def handle_message_connection_ready(self, msg_params):
+        if not self.has_sent_online_msg:
+            self.has_sent_online_msg = True
+            self.send_client_status(0)
+
+            mlops.log_sys_perf(self.args)
+
+    def handle_message_check_status(self, msg_params):
+        self.send_client_status(0)
 
-    def test_on_server_for_all_clients(self, round_idx):
-        if self.aggregator.test_all(
-            self.train_data_local_dict,
-            self.test_data_local_dict,
-            self.device,
-            self.args,
-        ):
+    def handle_message_init(self, msg_params):
+        if self.is_inited:
             return
 
-        if (
-            round_idx % self.args.frequency_of_the_test == 0
-            or round_idx == self.args.comm_round - 1
-        ):
-            logging.info(
-                "################test_on_server_for_all_clients : {}".format(round_idx)
+        self.is_inited = True
+
+        global_model_params = msg_params.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS)
+        data_silo_index = msg_params.get(MyMessage.MSG_ARG_KEY_CLIENT_INDEX)
+
+        logging.info("data_silo_index = %s" % str(data_silo_index))
+
+        # Notify MLOps with training status.
+        self.report_training_status(MyMessage.MSG_MLOPS_CLIENT_STATUS_TRAINING)
+
+        if self.args.scenario == FEDML_CROSS_SILO_SCENARIO_HIERARCHICAL:
+            global_model_params = convert_model_params_to_ddp(global_model_params)
+            self.sync_process_group(0, global_model_params, data_silo_index)
+
+        self.trainer_dist_adapter.update_dataset(int(data_silo_index))
+        self.trainer_dist_adapter.update_model(global_model_params)
+        self.round_idx = 0
+
+        self.__train()
+        self.round_idx += 1
+
+    def handle_message_receive_model_from_server(self, msg_params):
+        logging.info("handle_message_receive_model_from_server.")
+        model_params = msg_params.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS)
+        client_index = msg_params.get(MyMessage.MSG_ARG_KEY_CLIENT_INDEX)
+
+        if self.args.scenario == FEDML_CROSS_SILO_SCENARIO_HIERARCHICAL:
+            model_params = convert_model_params_to_ddp(model_params)
+            self.sync_process_group(self.round_idx, model_params, client_index)
+
+        self.trainer_dist_adapter.update_dataset(int(client_index))
+        logging.info("current round index {}, total rounds {}".format(self.round_idx, self.num_rounds))
+        self.trainer_dist_adapter.update_model(model_params)
+        if self.round_idx < self.num_rounds:
+            self.__train()
+            self.round_idx += 1
+        else:
+            mlops.stop_sys_perf()
+            self.send_client_status(0, ClientMasterManager.RUN_FINISHED_STATUS_FLAG)
+            if self.is_main_process():
+                mlops.log_training_finished_status()
+            self.finish()
+
+    def handle_message_finish(self, msg_params):
+        logging.info(" ====================cleanup ====================")
+        self.cleanup()
+
+    def cleanup(self):
+        self.send_client_status(0, ClientMasterManager.RUN_FINISHED_STATUS_FLAG)
+        if self.is_main_process():
+            mlops.log_training_finished_status()
+        self.finish()
+
+    def send_model_to_server(self, receive_id, weights, local_sample_num):
+        if self.is_main_process():
+            tick = time.time()
+            mlops.event("comm_c2s", event_started=True, event_value=str(self.round_idx))
+            message = Message(MyMessage.MSG_TYPE_C2S_SEND_MODEL_TO_SERVER, self.client_real_id, receive_id)
+            message.add_params(MyMessage.MSG_ARG_KEY_MODEL_PARAMS, weights)
+            message.add_params(MyMessage.MSG_ARG_KEY_NUM_SAMPLES, local_sample_num)
+            self.send_message(message)
+
+            MLOpsProfilerEvent.log_to_wandb({"Communication/Send_Total": time.time() - tick})
+            mlops.log_client_model_info(
+                self.round_idx + 1, self.num_rounds, model_url=message.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_URL),
             )
-            train_num_samples = []
-            train_tot_corrects = []
-            train_losses = []
-            for client_idx in range(self.args.client_num_in_total):
-                # train data
-                metrics = self.aggregator.test(
-                    self.train_data_local_dict[client_idx], self.device, self.args
-                )
-                train_tot_correct, train_num_sample, train_loss = (
-                    metrics["test_correct"],
-                    metrics["test_total"],
-                    metrics["test_loss"],
-                )
-                train_tot_corrects.append(copy.deepcopy(train_tot_correct))
-                train_num_samples.append(copy.deepcopy(train_num_sample))
-                train_losses.append(copy.deepcopy(train_loss))
-
-            # test on training dataset
-            train_acc = sum(train_tot_corrects) / sum(train_num_samples)
-            train_loss = sum(train_losses) / sum(train_num_samples)
-            if self.args.enable_wandb:
-                wandb.log({"Train/Acc": train_acc, "round": round_idx})
-                wandb.log({"Train/Loss": train_loss, "round": round_idx})
-            stats = {"training_acc": train_acc, "training_loss": train_loss}
-            logging.info(stats)
-
-            # test data
-            test_num_samples = []
-            test_tot_corrects = []
-            test_losses = []
 
-            if round_idx == self.args.comm_round - 1:
-                metrics = self.aggregator.test(self.test_global, self.device, self.args)
+    def send_client_status(self, receive_id, status=ONLINE_STATUS_FLAG):
+        if self.is_main_process():
+            logging.info("send_client_status")
+            logging.info("self.client_real_id = {}".format(self.client_real_id))
+            message = Message(MyMessage.MSG_TYPE_C2S_CLIENT_STATUS, self.client_real_id, receive_id)
+            sys_name = platform.system()
+            if sys_name == "Darwin":
+                sys_name = "Mac"
+            # Debug for simulation mobile system
+            # sys_name = MyMessage.MSG_CLIENT_OS_ANDROID
+
+            message.add_params(MyMessage.MSG_ARG_KEY_CLIENT_STATUS, status)
+            message.add_params(MyMessage.MSG_ARG_KEY_CLIENT_OS, sys_name)
+
+            if getattr(self.args, "using_mlops", False) and status == ClientMasterManager.RUN_FINISHED_STATUS_FLAG:
+                mlops.log_server_payload(self.args.run_id, self.client_real_id, json.dumps(message.get_params()))
             else:
-                metrics = self.aggregator.test(self.val_global, self.device, self.args)
+                self.send_message(message)
 
-            test_tot_correct, test_num_sample, test_loss = (
-                metrics["test_correct"],
-                metrics["test_total"],
-                metrics["test_loss"],
-            )
-            test_tot_corrects.append(copy.deepcopy(test_tot_correct))
-            test_num_samples.append(copy.deepcopy(test_num_sample))
-            test_losses.append(copy.deepcopy(test_loss))
-
-            # test on test dataset
-            test_acc = sum(test_tot_corrects) / sum(test_num_samples)
-            test_loss = sum(test_losses) / sum(test_num_samples)
-            if self.args.enable_wandb:
-                wandb.log({"Test/Acc": test_acc, "round": round_idx})
-                wandb.log({"Test/Loss": test_loss, "round": round_idx})
-            stats = {"test_acc": test_acc, "test_loss": test_loss}
-            logging.info(stats)
+    def report_training_status(self, status):
+        mlops.log_training_status(status)
+
+    def sync_process_group(self, round_idx, model_params=None, client_index=None, src=0):
+        logging.info("sending round number to pg")
+        round_number = [round_idx, model_params, client_index]
+        dist.broadcast_object_list(
+            round_number, src=src, group=self.trainer_dist_adapter.process_group_manager.get_process_group(),
+        )
+        logging.info("round number %d broadcast to process group" % round_number[0])
+
+    def __train(self):
+        logging.info("#######training########### round_id = %d" % self.round_idx)
+
+        mlops.event("train", event_started=True, event_value=str(self.round_idx))
+
+        weights, local_sample_num = self.trainer_dist_adapter.train(self.round_idx)
+
+        mlops.event("train", event_started=False, event_value=str(self.round_idx))
+
+        # the current model is still DDP-wrapped under cross-silo-hi setting
+        if self.args.scenario == FEDML_CROSS_SILO_SCENARIO_HIERARCHICAL:
+            weights = convert_model_params_from_ddp(weights)
+
+        self.send_model_to_server(0, weights, local_sample_num)
+
+    def run(self):
+        super().run()
```

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedopt/message_define.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedopt/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedopt/FedOptClientManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedopt/FedOptClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedopt/optrepo.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedopt/optrepo.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedopt/FedOptAPI.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedopt/FedOptAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedopt/utils.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedopt/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedopt/FedOptTrainer.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedopt/FedOptTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedopt/FedOptServerManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedopt/FedOptServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedopt_seq/FedOptSeqAPI.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedopt_seq/FedOptSeqAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedopt_seq/FedOptAggregator.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedopt_seq/FedOptAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedopt_seq/message_define.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedopt_seq/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedopt_seq/FedOptClientManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedopt_seq/FedOptClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedopt_seq/optrepo.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedopt_seq/optrepo.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedopt_seq/utils.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedopt_seq/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedopt_seq/FedOptTrainer.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedopt_seq/FedOptTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedopt_seq/FedOptServerManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedopt_seq/FedOptServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedseg/FedSegClientManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedseg/FedSegClientManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedseg/message_define.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedseg/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedseg/FedSegTrainer.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedseg/FedSegTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedseg/MyModelTrainer.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedseg/MyModelTrainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedseg/FedSegAggregator.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedseg/FedSegAggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedseg/utils.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedseg/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedseg/FedSegAPI.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedseg/FedSegAPI.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/mpi/fedseg/FedSegServerManager.py` & `fedml-0.8.5a1/fedml/simulation/mpi/fedseg/FedSegServerManager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/simulation/simulator.py` & `fedml-0.8.5a1/fedml/simulation/simulator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/__init__.py` & `fedml-0.8.5a1/fedml/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     FEDML_TRAINING_PLATFORM_SERVING,
 )
 from .core.common.ml_engine_backend import MLEngineBackend
 
 _global_training_type = None
 _global_comm_backend = None
 
-__version__ = "0.8.4a9"
+__version__ = "0.8.5a1"
 
 
 def init(args=None):
     if args is None:
         args = load_arguments(fedml._global_training_type, fedml._global_comm_backend)
 
     """Initialize FedML Engine."""
@@ -311,23 +311,28 @@
             args.launcher_rdzv_port = 29400
 
         if not hasattr(args, "n_node_in_silo"):
             args.n_node_in_silo = 1
         if not (hasattr(args, "n_proc_per_node") and args.n_proc_per_node):
             if args.n_node_in_silo == 1 and torch.cuda.is_available():
                 gpu_count = torch.cuda.device_count()
-                # Checking if launcher is has spawned enoug processes.
+                # Checking if launcher is has spawned enough processes.
                 if gpu_count == args.n_proc_in_silo:
                     print(f"Auto assigning GPU to processes.")
                     args.gpu_id = args.proc_rank_in_silo
                 else:
                     args.n_proc_per_node = 1
             else:
                 args.n_proc_per_node = 1
 
+    print("\nargs.rank = {}, args.n_proc_in_silo: {}".format(args.rank, args.n_proc_in_silo))
+    print("args.rank = {}, n_proc_in_silo: {}".format(args.rank, args.n_proc_in_silo))
+    print("args.rank = {}, rank_in_node: {}".format(args.rank, args.rank_in_node))
+    print("args.rank = {}, proc_rank_in_silo: {}".format(args.rank, args.proc_rank_in_silo))
+    exit()
     return args
 
 
 def init_cheetah(args):
     args.n_proc_in_silo = 1
     args.proc_rank_in_silo = 0
     manage_mpi_args(args)
@@ -376,14 +381,15 @@
             print("args.client_id_list is not None")
     else:
         print("using_mlops = true")
 
 
 def init_cross_device(args):
     args.rank = 0  # only server runs on Python package
+    args.role = "server"
     return args
 
 
 def run_distributed():
     pass
```

### Comparing `fedml-0.8.4a9/fedml/utils/model_utils.py` & `fedml-0.8.5a1/fedml/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/utils/logging.py` & `fedml-0.8.5a1/fedml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/utils/compression.py` & `fedml-0.8.5a1/fedml/utils/compression.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/utils/context.py` & `fedml-0.8.5a1/fedml/utils/context.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cli/edge_deployment/client_data_interface.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_client_data_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import logging
 import os
 import sqlite3
 import time
 import traceback
 
-from fedml.cli.edge_deployment.client_constants import ClientConstants
+from fedml.cli.model_deployment.device_client_constants import ClientConstants
 from fedml.core.common.singleton import Singleton
-from fedml.cli.server_deployment.server_constants import ServerConstants
+from fedml.cli.model_deployment.device_server_constants import ServerConstants
 
 
 class FedMLClientDataInterface(Singleton):
     MAX_JOB_LIST_SIZE = 50000
     ERRCODE_JOB_FAILED = 1
     ERRCODE_JOB_KILLED = 2
+    JOBS_DB = "model-jobs.db"
 
     def __init__(self):
         pass
 
     @staticmethod
     def get_instance():
         return FedMLClientDataInterface()
@@ -109,18 +110,27 @@
                                 status,
                                 status)
         else:
             self.save_job_status(run_id, edge_id,
                                  status,
                                  status)
 
+    def save_job_result(self, job_id, edge_id, deployment_result=None):
+        self.create_job_table()
+
+        job_obj = FedMLClientJobModel()
+        job_obj.job_id = job_id
+        job_obj.edge_id = edge_id
+        job_obj.deployment_result = deployment_result
+        self.update_job_to_db(job_obj)
+
     def open_job_db(self):
         if not os.path.exists(ClientConstants.get_database_dir()):
             os.makedirs(ClientConstants.get_database_dir())
-        job_db_path = os.path.join(ClientConstants.get_database_dir(), "jobs.db")
+        job_db_path = os.path.join(ClientConstants.get_database_dir(), FedMLClientDataInterface.JOBS_DB)
         self.db_connection = sqlite3.connect(job_db_path)
 
     def close_job_db(self):
         if self.db_connection is not None:
             self.db_connection.close()
 
     def create_job_table(self):
@@ -139,15 +149,16 @@
                    status TEXT,
                    failed_time TEXT,
                    error_code INT,
                    msg TEXT,
                    updated_time TEXT,
                    round_index INT,
                    total_rounds INT,
-                   running_json TEXT);''')
+                   running_json TEXT,
+                   deployment_result TEXT);''')
             self.db_connection.commit()
         except Exception as e:
             pass
         self.db_connection.close()
 
     def drop_job_table(self):
         self.open_job_db()
@@ -179,14 +190,15 @@
             job_obj.round_index = row[11]
             job_obj.total_rounds = row[12]
             job_obj.progress = (0 if job_obj.total_rounds == 0 else job_obj.round_index / job_obj.total_rounds)
             total_time = (0 if job_obj.progress == 0 else (float(job_obj.updated_time) - float(job_obj.started_time))
                                                           / job_obj.progress)
             job_obj.eta = total_time * (1.0 - job_obj.progress)
             job_obj.running_json = row[13]
+            job_obj.deployment_result = row[14]
             # job_obj.show()
             break
 
         self.db_connection.close()
         return job_obj
 
     def get_jobs_from_db(self):
@@ -209,26 +221,26 @@
             job_obj.round_index = row[11]
             job_obj.total_rounds = row[12]
             job_obj.progress = (0 if job_obj.total_rounds == 0 else job_obj.round_index / job_obj.total_rounds)
             total_time = (0 if job_obj.progress == 0 else (float(job_obj.updated_time) - float(job_obj.started_time))
                                                           / job_obj.progress)
             job_obj.eta = total_time * (1.0 - job_obj.progress)
             job_obj.running_json = row[13]
+            job_obj.deployment_result = row[14]
             job_list_obj.job_list.append(job_obj)
 
             if len(job_list_obj.job_list) > FedMLClientDataInterface.MAX_JOB_LIST_SIZE:
                 break
 
         self.db_connection.close()
         return job_list_obj
 
     def get_job_by_id(self, job_id):
         if job_id is None:
             return None
-
         job_obj = None
 
         self.open_job_db()
         current_cursor = self.db_connection.cursor()
         results = current_cursor.execute("SELECT *  from jobs where job_id={};".format(job_id))
         for row in results:
             job_obj = FedMLClientJobModel()
@@ -244,14 +256,15 @@
             job_obj.round_index = row[11]
             job_obj.total_rounds = row[12]
             job_obj.progress = (0 if job_obj.total_rounds == 0 else job_obj.round_index / job_obj.total_rounds)
             total_time = (0 if job_obj.progress == 0 else (float(job_obj.updated_time) - float(job_obj.started_time))
                                                           / job_obj.progress)
             job_obj.eta = total_time * (1.0 - job_obj.progress)
             job_obj.running_json = row[13]
+            job_obj.deployment_result = row[14]
             # job_obj.show()
             break
 
         self.db_connection.close()
         return job_obj
 
     def insert_job_to_db(self, job):
@@ -262,61 +275,62 @@
             self.db_connection.close()
             self.update_job_to_db(job)
             return
 
         try:
             current_cursor.execute("INSERT INTO jobs (\
                 job_id, edge_id, started_time, ended_time, progress, ETA, status, failed_time, error_code, msg, \
-                updated_time, round_index, total_rounds, running_json) \
-                VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)",
+                updated_time, round_index, total_rounds, running_json, deployment_result) \
+                VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)",
                                    (job.job_id, job.edge_id, job.started_time, job.ended_time,
                                     job.progress, job.eta, job.status, job.failed_time,
                                     job.error_code, job.msg, str(time.time()),
-                                    job.round_index, job.total_rounds, job.running_json))
+                                    job.round_index, job.total_rounds, job.running_json, job.deployment_result))
         except Exception as e:
             logging.info("Process jobs insertion {}.".format(traceback.format_exc()))
         self.db_connection.commit()
         self.db_connection.close()
 
     def update_job_to_db(self, job):
         self.open_job_db()
         current_cursor = self.db_connection.cursor()
         try:
-            update_statement = "UPDATE jobs set {} {} {} {} {} {} {} {} {} {} {} {} where job_id={}".format(
+            update_statement = "UPDATE jobs set {} {} {} {} {} {} {} {} {} {} {} {} {} where job_id={}".format(
                 f"edge_id={job.edge_id}" if job.edge_id != 0 else "",
                 f",started_time='{job.started_time}'" if job.started_time != "" else "",
                 f",ended_time='{job.ended_time}'" if job.ended_time != "" else "",
                 f",progress={job.progress}" if job.progress != 0 else "",
                 f",eta={job.eta}" if job.eta != 0 else "",
                 f",status='{job.status}'" if job.status != "" else "",
                 f",failed_time='{job.failed_time}'" if job.failed_time != "" else "",
                 f",error_code={job.error_code}" if job.error_code != -1 else "",
                 f",msg='{job.msg}'" if job.msg != "" else "",
                 ",updated_time='" + str(time.time()) + "'",
                 f",round_index={job.round_index}" if job.round_index != 0 else "",
                 f",total_rounds={job.total_rounds}" if job.total_rounds != 0 else "",
+                f",deployment_result='{job.deployment_result}'" if job.deployment_result != "" else "",
                 job.job_id)
             current_cursor.execute(update_statement)
             self.db_connection.commit()
         except Exception as e:
             pass
         self.db_connection.close()
 
     def handle_database_compatibility(self):
         self.open_job_db()
         should_alter_old_table = False
         current_cursor = self.db_connection.cursor()
         results = current_cursor.execute("select * from sqlite_master where type='table' and name='jobs';")
         for row in results:
             table_statement = str(row[4])
-            if table_statement.find("running_json") == -1:
+            if table_statement.find("deployment_result") == -1:
                 should_alter_old_table = True
 
         if should_alter_old_table:
-            current_cursor.execute("ALTER TABLE jobs ADD running_json TEXT;")
+            current_cursor.execute("ALTER TABLE jobs ADD deployment_result TEXT;")
             self.db_connection.commit()
             logging.info("Process compatibility on the local db.")
 
         self.close_job_db()
 
 
 class FedMLClientJobModel(object):
@@ -332,14 +346,15 @@
         self.error_code = -1
         self.msg = ""
         self.updated_time = ""
         self.round_index = 0
         self.total_rounds = 0
         self.status = ""
         self.running_json = ""
+        self.deployment_result = ""
 
     def show(self):
         logging.info("Job object, job id {}, edge id {}, started time {},"
                      "ended time {}, progress {}, eta {}, status {},"
                      "failed time {}, error code {}, msg {},"
                      "updated time {}, round index {}, total rounds {}".format(
             self.job_id, self.edge_id, self.started_time,
```

### Comparing `fedml-0.8.4a9/fedml/cli/edge_deployment/client_login.py` & `fedml-0.8.5a1/fedml/cli/edge_deployment/client_login.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,36 +2,33 @@
 import argparse
 import json
 import logging
 import os
 import platform
 import subprocess
 import time
-from os.path import expanduser
 
 import click
 from fedml.cli.comm_utils import sys_utils
-from fedml.cli.edge_deployment.client_data_interface import FedMLClientDataInterface
-from fedml.core.mlops import MLOpsProfilerEvent
-from fedml.core.mlops.mlops_runtime_log import MLOpsRuntimeLog
 from fedml.cli.edge_deployment.client_runner import FedMLClientRunner
 from fedml.cli.edge_deployment.client_constants import ClientConstants
+from fedml.core.mlops.mlops_utils import MLOpsUtils
 
 
 def init_logs(args, edge_id):
     # Init runtime logs
     args.log_file_dir = ClientConstants.get_log_file_dir()
     args.run_id = 0
-    args.rank = 1
+    args.role = "client"
     client_ids = list()
     client_ids.append(edge_id)
     args.client_id_list = json.dumps(client_ids)
     setattr(args, "using_mlops", True)
-    MLOpsRuntimeLog.get_instance(args).init_logs(show_stdout_log=True)
-    logging.info("client ids:{}".format(args.client_id_list))
+    # MLOpsRuntimeLog.get_instance(args).init_logs(show_stdout_log=True)
+    # logging.info("client ids:{}".format(args.client_id_list))
 
 
 def __login_as_client(args, userid, version):
     setattr(args, "account_id", userid)
     setattr(args, "current_running_dir", ClientConstants.get_fedml_home_dir())
 
     sys_name = platform.system()
@@ -63,27 +60,28 @@
         try:
             mqtt_config, s3_config, mlops_config, docker_config = runner.fetch_configs()
             service_config["mqtt_config"] = mqtt_config
             service_config["s3_config"] = s3_config
             service_config["ml_ops_config"] = mlops_config
             service_config["docker_config"] = docker_config
             runner.agent_config = service_config
+            # click.echo("service_config = {}".format(service_config))
             log_server_url = mlops_config.get("LOG_SERVER_URL", None)
             if log_server_url is not None:
                 setattr(args, "log_server_url", log_server_url)
                 setattr(runner.args, "log_server_url", log_server_url)
             break
         except Exception as e:
             config_try_count += 1
             time.sleep(3)
             continue
 
     if config_try_count >= 5:
         click.echo("")
-        click.echo("Oops, you failed to login the FedML MLOps platform.")
+        click.echo("[1] Oops, you failed to login the FedML MLOps platform.")
         click.echo("Please check whether your network is normal!")
         return
 
     # Judge whether running from fedml docker hub
     is_from_fedml_docker_hub = False
     dock_loc_file = ClientConstants.get_docker_location_file()
     if os.path.exists(dock_loc_file):
@@ -111,27 +109,27 @@
         except Exception as e:
             register_try_count += 1
             time.sleep(3)
             continue
 
     if edge_id <= 0:
         click.echo("")
-        click.echo("Oops, you failed to login the FedML MLOps platform.")
+        click.echo("[2] Oops, you failed to login the FedML MLOps platform.")
         click.echo("Please check whether your network is normal!")
         return
 
     # Init runtime logs
     setattr(args, "client_id", edge_id)
     runner.args = args
     init_logs(args, edge_id)
-    logging.info("args {}".format(args))
+    # logging.info("args {}".format(args))
 
     # Log arguments and binding results.
-    logging.info("login: unique_device_id = %s" % str(unique_device_id))
-    logging.info("login: edge_id = %s" % str(edge_id))
+    # logging.info("login: unique_device_id = %s" % str(unique_device_id))
+    # logging.info("login: edge_id = %s" % str(edge_id))
     runner.unique_device_id = unique_device_id
     ClientConstants.save_runner_infos(args.current_device_id + "." + args.os_name, edge_id, run_id=0)
 
     # Setup MQTT connection for communication with the FedML server.
     runner.setup_agent_mqtt_connection(service_config)
 
     # Start mqtt looper
@@ -177,15 +175,15 @@
         except Exception as e:
             config_try_count += 1
             time.sleep(3)
             continue
 
     if config_try_count >= 5:
         click.echo("")
-        click.echo("Oops, you failed to login the FedML MLOps platform.")
+        click.echo("[3] Oops, you failed to login the FedML MLOps platform.")
         click.echo("Please check whether your network is normal!")
         return False, edge_id, args
 
     # Build unique device id
     if args.device_id is not None and len(str(args.device_id)) > 0:
         unique_device_id = args.device_id + "@" + args.os_name + ".Edge.Simulator"
 
@@ -204,15 +202,15 @@
         except Exception as e:
             register_try_count += 1
             time.sleep(3)
             continue
 
     if edge_id <= 0:
         click.echo("")
-        click.echo("Oops, you failed to login the FedML MLOps platform.")
+        click.echo("[4] Oops, you failed to login the FedML MLOps platform.")
         click.echo("Please check whether your network is normal!")
         return False, edge_id, args
 
     # Init runtime logs
     setattr(args, "client_id", edge_id)
     runner.args = args
     #init_logs(args, edge_id)
@@ -230,15 +228,15 @@
         try:
             runner.setup_agent_mqtt_connection(service_config)
         except Exception as e:
             pass
 
         # Open simulator daemon process to process run status.
         simulator_daemon_cmd = os.path.join(os.path.dirname(__file__), "simulator_daemon.py")
-        simulator_daemon_process = subprocess.Popen(
+        simulator_daemon_process = sys_utils.run_subprocess_open(
             [
                 sys_utils.get_python_program(),
                 simulator_daemon_cmd,
                 "-t",
                 "login",
                 "-u",
                 str(args.user),
@@ -273,15 +271,15 @@
     if args.role == ClientConstants.login_role_list[ClientConstants.LOGIN_MODE_CLIEN_INDEX]:
         __login_as_client(args, args.user, args.version)
     elif args.role == ClientConstants.login_role_list[ClientConstants.LOGIN_MODE_EDGE_SIMULATOR_INDEX]:
         __login_as_simulator(args, args.user, args.version)
 
 
 def logout():
-    ClientConstants.cleanup_run_process()
+    ClientConstants.cleanup_run_process(None)
     sys_utils.cleanup_all_fedml_client_api_processes()
 
 
 if __name__ == "__main__":
     os.environ['PYTHONWARNINGS'] = 'ignore:semaphore_tracker:UserWarning'
     os.environ.setdefault('PYTHONWARNINGS', 'ignore:semaphore_tracker:UserWarning')
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
@@ -290,14 +288,15 @@
                         help='account id at MLOps platform')
     parser.add_argument("--version", "-v", type=str, default="release")
     parser.add_argument("--local_server", "-ls", type=str, default="127.0.0.1")
     parser.add_argument("--role", "-r", type=str, default="client")
     parser.add_argument("--device_id", "-id", type=str, default="0")
     parser.add_argument("--os_name", "-os", type=str, default="")
     args = parser.parse_args()
+    
     args.user = args.user
     if args.type == 'login':
         login(args)
     else:
         logout()
```

### Comparing `fedml-0.8.4a9/fedml/cli/edge_deployment/client_daemon.py` & `fedml-0.8.5a1/fedml/cli/edge_deployment/client_daemon.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 
 import argparse
 import os
 import time
-import sys
 
 from fedml.cli.comm_utils.sys_utils import cleanup_all_fedml_client_api_processes, \
     cleanup_all_fedml_client_learning_processes, cleanup_all_fedml_client_login_processes, get_python_program, \
     daemon_ota_upgrade
 from fedml.cli.edge_deployment.client_constants import ClientConstants
 
 
@@ -23,17 +22,17 @@
     args = parser.parse_args()
     args.user = args.user
 
     pip_source_dir = os.path.dirname(__file__)
     login_cmd = os.path.join(pip_source_dir, "client_login.py")
     while True:
         try:
-            ClientConstants.cleanup_run_process()
+            ClientConstants.cleanup_run_process(None)
             cleanup_all_fedml_client_api_processes()
-            cleanup_all_fedml_client_learning_processes()
+            cleanup_all_fedml_client_learning_processes(None)
             cleanup_all_fedml_client_login_processes("client_login.py", clean_process_group=False)
         except Exception as e:
             pass
 
         daemon_ota_upgrade(args)
 
         login_pid = ClientConstants.exec_console_with_shell_script_list(
```

### Comparing `fedml-0.8.4a9/fedml/cli/edge_deployment/docker_login.py` & `fedml-0.8.5a1/fedml/cli/edge_deployment/docker_login.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,17 +93,20 @@
             is_deployment_ok = True
     if err is not None:
         err_str = err.decode(encoding="utf-8")
         if str(err_str).find(fedml_docker_name) != -1 and str(err_str).find("Up") != -1:
             is_deployment_ok = True
 
     if is_deployment_ok:
-        click.echo("Congratulations, you have deployed the FedML client agent successfully!")
-        click.echo("Your device id is " + env_current_device_id + ".")
-        click.echo("You may review the device in the MLOps edge device list.")
+        print("\n\nCongratulations, your device is connected to the FedML MLOps platform successfully!")
+        print(
+            "Your unique device ID is "
+            + str(env_current_device_id)
+            + "\n"
+        )
 
         logs_with_docker_mode(docker_rank)
     else:
         click.echo("Oops, you failed to deploy the FedML client agent.")
         click.echo("Please check whether your Docker Application is installed and running normally!")
```

### Comparing `fedml-0.8.4a9/fedml/cli/edge_deployment/client_runner.py` & `fedml-0.8.5a1/fedml/cli/edge_deployment/client_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 import time
 import traceback
 import urllib
 import uuid
 import zipfile
 
-import click
 import requests
 from ...core.mlops.mlops_runtime_log import MLOpsRuntimeLog
 
 from ...core.distributed.communication.mqtt.mqtt_manager import MqttManager
 from ...cli.comm_utils.yaml_utils import load_yaml_config
 from ...cli.edge_deployment.client_constants import ClientConstants
 
@@ -29,26 +28,28 @@
 
 from ...core.mlops.mlops_configs import MLOpsConfigs
 from ...core.mlops.mlops_runtime_log_daemon import MLOpsRuntimeLogDaemon
 from ...core.mlops.mlops_status import MLOpsStatus
 from ..comm_utils.sys_utils import get_sys_runner_info, get_python_program
 from .client_data_interface import FedMLClientDataInterface
 from ..comm_utils import sys_utils
+from ...core.mlops.mlops_utils import MLOpsUtils
 
 
 class RunnerError(Exception):
     """ Runner failed. """
     pass
 
 
 class FedMLClientRunner:
 
     def __init__(self, args, edge_id=0, request_json=None, agent_config=None, run_id=0):
         self.run_process_event = None
         self.run_process = None
+        self.local_api_process = None
         self.start_request_json = None
         self.device_status = None
         self.current_training_status = None
         self.mqtt_mgr = None
         self.client_mqtt_mgr = None
         self.client_mqtt_is_connected = False
         self.client_mqtt_lock = None
@@ -83,14 +84,15 @@
             "${FEDSYS.CLIENT_INDEX}": "",
             "${FEDSYS.CLIENT_OBJECT_LIST}": "",
             "${FEDSYS.LOG_SERVER_URL}": "",
         }
 
         self.mlops_metrics = None
         self.client_active_list = dict()
+        self.ntp_offset = MLOpsUtils.get_ntp_offset()
         # logging.info("Current directory of client agent: " + self.cur_dir)
 
     def build_dynamic_constrain_variables(self, run_id, run_config):
         data_config = run_config["data_config"]
         server_edge_id_list = self.request_json["edgeids"]
         local_edge_id_list = [1]
         local_edge_id_list[0] = self.edge_id
@@ -224,20 +226,20 @@
         package_conf_object["dynamic_args"]["log_file_dir"] = log_file_dir
 
         # Save new config dictionary to local file
         fedml_updated_config_file = os.path.join(unzip_package_path, "conf", "fedml.yaml")
         ClientConstants.generate_yaml_doc(package_conf_object, fedml_updated_config_file)
 
         # Build dynamic arguments and set arguments to fedml config object
-        if not self.build_dynamic_args(run_config, package_conf_object, unzip_package_path):
+        if not self.build_dynamic_args(run_id, run_config, package_conf_object, unzip_package_path):
             return None, None
 
         return unzip_package_path, package_conf_object
 
-    def build_dynamic_args(self, run_config, package_conf_object, base_dir):
+    def build_dynamic_args(self, run_id, run_config, package_conf_object, base_dir):
         fedml_conf_file = package_conf_object["entry_config"]["conf_file"]
         fedml_conf_file_processed = str(fedml_conf_file).replace('\\', os.sep).replace('/', os.sep)
         fedml_conf_path = os.path.join(base_dir, "fedml", "config",
                                        os.path.basename(fedml_conf_file_processed))
         fedml_conf_object = load_yaml_config(fedml_conf_path)
 
         # Replace local fedml config objects with parameters from MLOps web
@@ -257,22 +259,27 @@
         fedml_conf_object["train_args"]["server_id"] = self.request_json.get("server_id", "0")
         fedml_conf_object["device_args"]["worker_num"] = int(package_dynamic_args["client_num_in_total"])
         # fedml_conf_object["data_args"]["data_cache_dir"] = package_dynamic_args["data_cache_dir"]
         fedml_conf_object["tracking_args"]["log_file_dir"] = package_dynamic_args["log_file_dir"]
         fedml_conf_object["tracking_args"]["log_server_url"] = package_dynamic_args["log_server_url"]
         if hasattr(self.args, "local_server") and self.args.local_server is not None:
             fedml_conf_object["comm_args"]["local_server"] = self.args.local_server
-        bootstrap_script_file = fedml_conf_object["environment_args"]["bootstrap"]
-        bootstrap_script_file = str(bootstrap_script_file).replace('\\', os.sep).replace('/', os.sep)
-        if platform.system() == 'Windows':
-            bootstrap_script_file = bootstrap_script_file.replace('.sh', '.bat')
-        bootstrap_script_dir = os.path.join(base_dir, "fedml", os.path.dirname(bootstrap_script_file))
-        bootstrap_script_path = os.path.join(
-            bootstrap_script_dir, bootstrap_script_dir, os.path.basename(bootstrap_script_file)
-        )
+        bootstrap_script_path = None
+        env_args = fedml_conf_object.get("environment_args", None)
+        if env_args is not None:
+            bootstrap_script_file = env_args.get("bootstrap", None)
+            if bootstrap_script_file is not None:
+                bootstrap_script_file = str(bootstrap_script_file).replace('\\', os.sep).replace('/', os.sep)
+                if platform.system() == 'Windows':
+                    bootstrap_script_file = bootstrap_script_file.replace('.sh', '.bat')
+                if bootstrap_script_file is not None:
+                    bootstrap_script_dir = os.path.join(base_dir, "fedml", os.path.dirname(bootstrap_script_file))
+                    bootstrap_script_path = os.path.join(
+                        bootstrap_script_dir, bootstrap_script_dir, os.path.basename(bootstrap_script_file)
+                    )
         # try:
         #     os.makedirs(package_dynamic_args["data_cache_dir"])
         # except Exception as e:
         #     pass
         fedml_conf_object["dynamic_args"] = package_dynamic_args
 
         ClientConstants.generate_yaml_doc(fedml_conf_object, fedml_conf_path)
@@ -291,14 +298,15 @@
                                  bootstrap_stat.st_mode | stat.S_IXUSR | stat.S_IXGRP | stat.S_IXOTH)
                         bootstrap_scripts = "cd {}; ./{}".format(bootstrap_script_dir,
                                                                  os.path.basename(bootstrap_script_file))
                     bootstrap_scripts = str(bootstrap_scripts).replace('\\', os.sep).replace('/', os.sep)
                     logging.info("Bootstrap scripts are being executed...")
                     process = ClientConstants.exec_console_with_script(bootstrap_scripts, should_capture_stdout=True,
                                                                        should_capture_stderr=True)
+                    ClientConstants.save_bootstrap_process(run_id, process.pid)
                     ret_code, out, err = ClientConstants.get_console_pipe_out_err_results(process)
                     if ret_code is None or ret_code <= 0:
                         if out is not None:
                             out_str = out.decode(encoding="utf-8")
                             if out_str != "":
                                 logging.info("{}".format(out_str))
 
@@ -322,26 +330,31 @@
 
     def run(self, process_event):
         os.environ['PYTHONWARNINGS'] = 'ignore:semaphore_tracker:UserWarning'
         os.environ.setdefault('PYTHONWARNINGS', 'ignore:semaphore_tracker:UserWarning')
 
         self.run_process_event = process_event
         try:
+            MLOpsUtils.set_ntp_offset(self.ntp_offset)
             self.setup_client_mqtt_mgr()
             self.run_impl()
         except RunnerError:
             logging.info("Runner stopped.")
             self.reset_devices_status(self.edge_id, ClientConstants.MSG_MLOPS_CLIENT_STATUS_KILLED)
         except Exception as e:
-            logging.info("Runner exits with exceptions.")
-            sys_utils.cleanup_all_fedml_client_login_processes(ClientConstants.CLIENT_LOGIN_PROGRAM,
-                                                               clean_process_group=False)
-            sys.exit(1)
+            logging.error("Runner exits with exceptions. {}".format(traceback.format_exc()))
+            self.reset_devices_status(self.edge_id, ClientConstants.MSG_MLOPS_CLIENT_STATUS_FAILED)
         finally:
             logging.info("Release resources.")
+            MLOpsRuntimeLogDaemon.get_instance(self.args).stop_log_processor(self.run_id, self.edge_id)
+            if self.mlops_metrics is not None:
+                self.mlops_metrics.stop_sys_perf()
+            time.sleep(3)
+            ClientConstants.cleanup_learning_process(self.run_id)
+            ClientConstants.cleanup_run_process(self.run_id)
             self.release_client_mqtt_mgr()
 
     def check_runner_stop_event(self):
         if self.run_process_event.is_set():
             logging.info("Received stopping event.")
             raise RunnerError("Runner stopped")
 
@@ -353,15 +366,16 @@
 
         self.check_runner_stop_event()
 
         MLOpsRuntimeLog.get_instance(self.args).init_logs(show_stdout_log=True)
 
         self.mlops_metrics.report_client_training_status(self.edge_id,
                                                          ClientConstants.MSG_MLOPS_CLIENT_STATUS_INITIALIZING,
-                                                         self.start_request_json)
+                                                         self.start_request_json,
+                                                         in_run_id=run_id)
 
         # get training params
         private_local_data_dir = data_config.get("privateLocalData", "")
         is_using_local_data = 0
         # if private_local_data_dir is not None and len(str(private_local_data_dir).strip(' ')) > 0:
         #     is_using_local_data = 1
 
@@ -391,18 +405,16 @@
 
         entry_file_config = fedml_config_object["entry_config"]
         dynamic_args_config = fedml_config_object["dynamic_args"]
         entry_file = str(entry_file_config["entry_file"]).replace('\\', os.sep).replace('/', os.sep)
         entry_file = os.path.basename(entry_file)
         conf_file = entry_file_config["conf_file"]
         conf_file = str(conf_file).replace('\\', os.sep).replace('/', os.sep)
-        ClientConstants.cleanup_learning_process()
-        sys_utils.cleanup_all_bootstrap_processes(
-            ClientConstants.CLIENT_BOOTSTRAP_WIN_PROGRAM if platform.system() == "Windows" else
-            ClientConstants.CLIENT_BOOTSTRAP_LINUX_PROGRAM, clean_process_group=False)
+        ClientConstants.cleanup_learning_process(run_id)
+        ClientConstants.cleanup_bootstrap_process(run_id)
         if not os.path.exists(unzip_package_path):
             logging.info("failed to unzip file.")
             self.check_runner_stop_event()
             self.cleanup_run_when_starting_failed()
             self.mlops_metrics.client_send_exit_train_msg(run_id, self.edge_id,
                                                           ClientConstants.MSG_MLOPS_CLIENT_STATUS_FAILED)
             return
@@ -422,30 +434,36 @@
                 python_program,
                 entry_fill_full_path,
                 "--cf",
                 conf_file_full_path,
                 "--rank",
                 str(dynamic_args_config["rank"]),
                 "--role",
-                "client",
+                "client"
             ],
             should_capture_stdout=False,
             should_capture_stderr=True
         )
         logging.info("waiting the learning process to train models...")
-        ClientConstants.save_learning_process(process.pid)
+        ClientConstants.save_learning_process(run_id, process.pid)
+
         ret_code, out, err = ClientConstants.get_console_pipe_out_err_results(process)
+        is_run_ok = sys_utils.is_runner_finished_normally(process.pid)
         if ret_code is None or ret_code <= 0:
-            if out is not None:
-                out_str = out.decode(encoding="utf-8")
-                if out_str != "":
-                    logging.info("{}".format(out_str))
+            if is_run_ok:
+                if out is not None:
+                    out_str = out.decode(encoding="utf-8")
+                    if out_str != "":
+                        logging.info("{}".format(out_str))
 
-            sys_utils.log_return_info(entry_file, 0)
+                sys_utils.log_return_info(entry_file, 0)
         else:
+            is_run_ok = False
+
+        if not is_run_ok:
             # If the run status is killed or finished, then return with the normal state.
             current_job = FedMLClientDataInterface.get_instance().get_job_by_id(run_id)
             if current_job is not None and (current_job.status == ClientConstants.MSG_MLOPS_CLIENT_STATUS_FINISHED or
                                             current_job.status == ClientConstants.MSG_MLOPS_CLIENT_STATUS_KILLED):
                 return
 
             self.check_runner_stop_event()
@@ -472,114 +490,100 @@
 
     def stop_run(self):
         logging.info("Stop run successfully.")
 
         self.reset_devices_status(self.edge_id, ClientConstants.MSG_MLOPS_CLIENT_STATUS_FINISHED)
 
         try:
-            ClientConstants.cleanup_learning_process()
-            sys_utils.cleanup_all_bootstrap_processes(
-                ClientConstants.CLIENT_BOOTSTRAP_WIN_PROGRAM if platform.system() == "Windows" else
-                ClientConstants.CLIENT_BOOTSTRAP_LINUX_PROGRAM, clean_process_group=False)
+            ClientConstants.cleanup_learning_process(self.run_id)
+            ClientConstants.cleanup_bootstrap_process(self.run_id)
+            ClientConstants.cleanup_run_process(self.run_id)
         except Exception as e:
             pass
 
     def stop_run_entry(self):
         try:
             if self.run_process_event is not None:
                 self.run_process_event.set()
             self.stop_run_with_killed_status()
             # if self.run_process is not None:
             #     logging.info("Run will be stopped, waiting...")
             #     self.run_process.join()
         except Exception as e:
-            sys_utils.cleanup_all_fedml_client_login_processes(
-                ClientConstants.CLIENT_LOGIN_PROGRAM, clean_process_group=False)
-            sys.exit(1)
+            ClientConstants.cleanup_run_process(self.run_id)
 
     def stop_run_with_killed_status(self, report_status=True):
         # logging.info("Stop run successfully.")
         try:
-            ClientConstants.cleanup_learning_process()
-            sys_utils.cleanup_all_bootstrap_processes(
-                ClientConstants.CLIENT_BOOTSTRAP_WIN_PROGRAM if platform.system() == "Windows" else
-                ClientConstants.CLIENT_BOOTSTRAP_LINUX_PROGRAM, clean_process_group=False)
+            ClientConstants.cleanup_learning_process(self.run_id)
+            ClientConstants.cleanup_bootstrap_process(self.run_id)
         except Exception as e:
             pass
 
         if report_status:
             self.reset_devices_status(self.edge_id, ClientConstants.MSG_MLOPS_CLIENT_STATUS_KILLED)
 
     def exit_run_with_exception_entry(self):
         try:
             self.setup_client_mqtt_mgr()
             self.exit_run_with_exception()
         except Exception as e:
             self.release_client_mqtt_mgr()
-            sys_utils.cleanup_all_fedml_client_login_processes(
-                ClientConstants.CLIENT_LOGIN_PROGRAM, clean_process_group=False)
-            sys.exit(1)
         finally:
             self.release_client_mqtt_mgr()
 
     def exit_run_with_exception(self):
         logging.info("Exit run successfully.")
 
-        ClientConstants.cleanup_learning_process()
-        ClientConstants.cleanup_run_process()
-        sys_utils.cleanup_all_bootstrap_processes(
-            ClientConstants.CLIENT_BOOTSTRAP_WIN_PROGRAM if platform.system() == "Windows" else
-            ClientConstants.CLIENT_BOOTSTRAP_LINUX_PROGRAM, clean_process_group=False)
+        ClientConstants.cleanup_learning_process(self.run_id)
+        ClientConstants.cleanup_run_process(self.run_id)
+        ClientConstants.cleanup_bootstrap_process(self.run_id)
 
         self.mlops_metrics.report_client_id_status(self.run_id, self.edge_id,
                                                    ClientConstants.MSG_MLOPS_CLIENT_STATUS_FAILED)
 
         time.sleep(1)
 
     def cleanup_run_when_starting_failed(self):
-        logging.info("Cleanup run successfully when starting failed.")
+        logging.error("Cleanup run successfully when starting failed.")
 
         self.reset_devices_status(self.edge_id, ClientConstants.MSG_MLOPS_CLIENT_STATUS_FAILED)
 
         time.sleep(2)
 
         try:
-            self.mlops_metrics.set_sys_reporting_status(False)
+            self.mlops_metrics.stop_sys_perf()
         except Exception as ex:
             pass
 
         time.sleep(1)
 
         try:
-            ClientConstants.cleanup_learning_process()
-            sys_utils.cleanup_all_bootstrap_processes(
-                ClientConstants.CLIENT_BOOTSTRAP_WIN_PROGRAM if platform.system() == "Windows" else
-                ClientConstants.CLIENT_BOOTSTRAP_LINUX_PROGRAM, clean_process_group=False)
+            ClientConstants.cleanup_learning_process(self.run_id)
+            ClientConstants.cleanup_bootstrap_process(self.run_id)
         except Exception as e:
             pass
 
     def cleanup_run_when_finished(self):
         logging.info("Cleanup run successfully when finished.")
 
         self.reset_devices_status(self.edge_id, ClientConstants.MSG_MLOPS_CLIENT_STATUS_FINISHED)
 
         time.sleep(2)
 
         try:
-            self.mlops_metrics.set_sys_reporting_status(False)
+            self.mlops_metrics.stop_sys_perf()
         except Exception as ex:
             pass
 
         time.sleep(1)
 
         try:
-            ClientConstants.cleanup_learning_process()
-            sys_utils.cleanup_all_bootstrap_processes(
-                ClientConstants.CLIENT_BOOTSTRAP_WIN_PROGRAM if platform.system() == "Windows" else
-                ClientConstants.CLIENT_BOOTSTRAP_LINUX_PROGRAM, clean_process_group=False)
+            ClientConstants.cleanup_learning_process(self.run_id)
+            ClientConstants.cleanup_bootstrap_process(self.run_id)
         except Exception as e:
             pass
 
     def on_client_mqtt_disconnected(self, mqtt_client_object):
         if self.client_mqtt_lock is None:
             self.client_mqtt_lock = threading.Lock()
 
@@ -686,42 +690,52 @@
             logging.info(f"Upgrade to version {upgrade_version} ...")
 
             sys_utils.do_upgrade(self.version, upgrade_version)
 
             raise Exception("Restarting after upgraded...")
 
     def callback_start_train(self, topic, payload):
+        try:
+            _, _ = MLOpsConfigs.get_instance(self.args).fetch_configs()
+        except Exception as e:
+            pass
+
+        if not FedMLClientDataInterface.get_instance().get_agent_status():
+            request_json = json.loads(payload)
+            run_id = request_json["runId"]
+            logging.error(
+                "FedMLDebug - Receive: topic ({}), payload ({}), but the client agent is disabled. {}".format(
+                    topic, payload, traceback.format_exc()
+                )
+            )
+            self.mlops_metrics.client_send_exit_train_msg(run_id, self.edge_id,
+                                                          ClientConstants.MSG_MLOPS_CLIENT_STATUS_FAILED,
+                                                          msg=f"the client agent {self.edge_id} is disabled")
+            self.mlops_metrics.report_client_training_status(self.edge_id,
+                                                             ClientConstants.MSG_MLOPS_CLIENT_STATUS_FAILED,
+                                                             in_run_id=run_id)
+            return
+
+        logging.info(
+            f"FedMLDebug - Receive: topic ({topic}), payload ({payload})"
+        )
+
         # Get training params
         request_json = json.loads(payload)
         is_retain = request_json.get("is_retain", False)
         if is_retain:
             return
         self.start_request_json = payload
         run_id = request_json["runId"]
 
-        if self.run_process is not None and \
-                sys_utils.get_process_running_count(ClientConstants.CLIENT_LOGIN_PROGRAM) >= 2:
-            logging.info("There is a running job {}.".format(
-                self.run_process.pid
-            ))
-            try:
-                if self.run_process_event is not None:
-                    self.run_process_event.set()
-                self.stop_run_with_killed_status()
-                sys_utils.cleanup_all_fedml_client_login_processes(
-                    ClientConstants.CLIENT_LOGIN_PROGRAM, clean_process_group=False)
-            except Exception as e:
-                pass
-
         logging.info("cleanup and save runner information")
 
         # Terminate previous process about starting or stopping run command
         server_agent_id = request_json["cloud_agent_id"]
-        ClientConstants.exit_process(self.run_process)
-        ClientConstants.cleanup_run_process()
+        ClientConstants.cleanup_run_process(run_id)
         ClientConstants.save_runner_infos(self.args.device_id + "." + self.args.os_name, self.edge_id, run_id=run_id)
 
         # Start log processor for current run
         self.args.run_id = run_id
         self.args.edge_id = self.edge_id
         MLOpsRuntimeLog.get_instance(self.args).init_logs(show_stdout_log=True)
         logging.info("start the log processor")
@@ -738,18 +752,21 @@
         if self.run_process_event is None:
             self.run_process_event = multiprocessing.Event()
         self.run_process_event.clear()
         client_runner.run_process_event = self.run_process_event
         logging.info("start the runner process.")
         self.run_process = Process(target=client_runner.run, args=(self.run_process_event,))
         self.run_process.start()
-        ClientConstants.save_run_process(self.run_process.pid)
+        ClientConstants.save_run_process(run_id, self.run_process.pid)
 
     def callback_stop_train(self, topic, payload):
         # logging.info("callback_stop_train: topic = %s, payload = %s" % (topic, payload))
+        logging.info(
+            f"FedMLDebug - Receive: topic ({topic}), payload ({payload})"
+        )
 
         request_json = json.loads(payload)
         is_retain = request_json.get("is_retain", False)
         if is_retain:
             return
         run_id = request_json.get("runId", None)
         if run_id is None:
@@ -768,14 +785,18 @@
         client_runner.mlops_metrics = self.mlops_metrics
         client_runner.stop_run_entry()
 
         # Stop log processor for current run
         MLOpsRuntimeLogDaemon.get_instance(self.args).stop_log_processor(run_id, self.edge_id)
 
     def callback_exit_train_with_exception(self, topic, payload):
+        logging.info(
+            f"FedMLDebug - Receive: topic ({topic}), payload ({payload})"
+        )
+
         request_json = json.loads(payload)
         is_retain = request_json.get("is_retain", False)
         if is_retain:
             return
         run_id = request_json.get("runId", None)
         if run_id is None:
             run_id = request_json.get("run_id", None)
@@ -796,19 +817,22 @@
             pass
 
     def cleanup_client_with_status(self):
         if self.device_status == ClientConstants.MSG_MLOPS_CLIENT_STATUS_FINISHED:
             logging.info("received to finished status.")
             self.cleanup_run_when_finished()
         elif self.device_status == ClientConstants.MSG_MLOPS_CLIENT_STATUS_FAILED:
-            logging.info("received to failed status.")
+            logging.error("received to failed status from the server agent")
             self.cleanup_run_when_starting_failed()
 
     def callback_runner_id_status(self, topic, payload):
         # logging.info("callback_runner_id_status: topic = %s, payload = %s" % (topic, payload))
+        logging.info(
+            f"FedMLDebug - Receive: topic ({topic}), payload ({payload})"
+        )
 
         request_json = json.loads(payload)
         is_retain = request_json.get("is_retain", False)
         if is_retain:
             return
         run_id = request_json["run_id"]
         edge_id = request_json["edge_id"]
@@ -832,21 +856,29 @@
             client_runner.mlops_metrics = self.mlops_metrics
             client_runner.cleanup_client_with_status()
 
             # Stop log processor for current run
             MLOpsRuntimeLogDaemon.get_instance(self.args).stop_log_processor(run_id, edge_id)
 
     def callback_report_current_status(self, topic, payload):
+        logging.info(
+            f"FedMLDebug - Receive: topic ({topic}), payload ({payload})"
+        )
+
         self.send_agent_active_msg()
 
     @staticmethod
     def process_ota_upgrade_msg():
         os.system("pip install -U fedml")
 
     def callback_client_ota_msg(self, topic, payload):
+        logging.info(
+            f"FedMLDebug - Receive: topic ({topic}), payload ({payload})"
+        )
+
         request_json = json.loads(payload)
         cmd = request_json["cmd"]
 
         if cmd == ClientConstants.FEDML_OTA_CMD_UPGRADE:
             FedMLClientRunner.process_ota_upgrade_msg()
             # Process(target=FedMLClientRunner.process_ota_upgrade_msg).start()
             raise Exception("After upgraded, restart runner...")
@@ -896,15 +928,15 @@
                 device_id = str(get_uuid())
                 logging.info(device_id)
             elif "posix" in os.name:
                 device_id = sys_utils.get_device_id_in_docker()
                 if device_id is None:
                     device_id = hex(uuid.getnode())
             else:
-                device_id = subprocess.Popen(
+                device_id = sys_utils.run_subprocess_open(
                     "hal-get-property --udi /org/freedesktop/Hal/devices/computer --key system.hardware.uuid".split()
                 )
                 device_id = hex(device_id)
 
         if device_id is not None and device_id != "":
             with open(file_for_device_id, 'w', encoding='utf-8') as f:
                 f.write(device_id)
@@ -961,14 +993,15 @@
                 MLOpsConfigs.install_root_ca_file()
                 response = requests.post(
                     url, json=json_params, verify=True,
                     headers={"content-type": "application/json", "Connection": "close"}
                 )
         else:
             response = requests.post(url, json=json_params, headers={"Connection": "close"})
+        # print("url = {}, response = {}".format(url, response))
         status_code = response.json().get("code")
         if status_code == "SUCCESS":
             edge_id = response.json().get("data").get("id")
         else:
             return 0
         return edge_id
 
@@ -1041,26 +1074,24 @@
         # Subscribe topics for starting train, stopping train and fetching client status.
         mqtt_client_object.subscribe(topic_start_train, qos=2)
         mqtt_client_object.subscribe(topic_stop_train, qos=2)
         mqtt_client_object.subscribe(topic_client_status, qos=2)
         mqtt_client_object.subscribe(topic_report_status, qos=2)
         mqtt_client_object.subscribe(topic_exit_train_with_exception, qos=2)
         mqtt_client_object.subscribe(topic_ota_msg, qos=2)
-        mqtt_client_object.subscribe(topic_exit_train_with_exception, qos=2)
 
         # Broadcast the first active message.
         self.send_agent_active_msg()
 
         # Echo results
-        click.echo("")
-        click.echo("Congratulations, you have logged into the FedML MLOps platform successfully!")
-        click.echo(
-            "Your device id is "
+        print("\n\nCongratulations, your device is connected to the FedML MLOps platform successfully!")
+        print(
+            "Your FedML Edge ID is " + str(self.edge_id) + ", unique device ID is "
             + str(self.unique_device_id)
-            + ". You may review the device in the MLOps edge device list."
+            + "\n"
         )
 
     def on_agent_mqtt_disconnected(self, mqtt_client_object):
         MLOpsStatus.get_instance().set_client_agent_status(
             self.edge_id, ClientConstants.MSG_MLOPS_CLIENT_STATUS_OFFLINE
         )
         pass
@@ -1080,18 +1111,18 @@
         self.agent_config = service_config
 
         # Init local database
         FedMLClientDataInterface.get_instance().create_job_table()
 
         # Start local API services
         python_program = get_python_program()
-        local_api_process = ClientConstants.exec_console_with_script(
+        self.local_api_process = ClientConstants.exec_console_with_script(
             "{} -m uvicorn fedml.cli.edge_deployment.client_api:api --host 0.0.0.0 --port {} "
             "--log-level critical".format(python_program,
-                                                   ClientConstants.LOCAL_CLIENT_API_PORT),
+                                          ClientConstants.LOCAL_CLIENT_API_PORT),
             should_capture_stdout=False,
             should_capture_stderr=False
         )
 
         # Setup MQTT connected listener
         self.mqtt_mgr.add_connected_listener(self.on_agent_mqtt_connected)
         self.mqtt_mgr.add_disconnected_listener(self.on_agent_mqtt_disconnected)
```

### Comparing `fedml-0.8.4a9/fedml/cli/edge_deployment/client_constants.py` & `fedml-0.8.5a1/fedml/cli/edge_deployment/client_constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -64,62 +64,84 @@
     LOGIN_MODE_EDGE_SIMULATOR_INDEX = 1
     login_role_list = ["client", "edge_simulator"]
 
     @staticmethod
     def get_fedml_home_dir():
         home_dir = expanduser("~")
         fedml_home_dir = os.path.join(home_dir, ClientConstants.LOCAL_HOME_RUNNER_DIR_NAME)
+        if not os.path.exists(fedml_home_dir):
+            os.makedirs(fedml_home_dir)
         return fedml_home_dir
 
     @staticmethod
     def get_log_file_dir():
         log_file_dir = os.path.join(ClientConstants.get_fedml_home_dir(), "fedml", "logs")
+        if not os.path.exists(log_file_dir):
+            os.makedirs(log_file_dir)
         return log_file_dir
 
     @staticmethod
     def get_data_dir():
         data_dir = os.path.join(ClientConstants.get_fedml_home_dir(), "fedml", "data")
+        if not os.path.exists(data_dir):
+            os.makedirs(data_dir)
         return data_dir
 
     @staticmethod
     def get_package_download_dir():
         package_download_dir = os.path.join(ClientConstants.get_fedml_home_dir(),
                                             ClientConstants.LOCAL_PACKAGE_HOME_DIR_NAME)
+        if not os.path.exists(package_download_dir):
+            os.makedirs(package_download_dir)
         return package_download_dir
 
     @staticmethod
     def get_package_unzip_dir():
         package_unzip_dir = ClientConstants.get_package_download_dir()
+        if not os.path.exists(package_unzip_dir):
+            os.makedirs(package_unzip_dir)
         return package_unzip_dir
 
     @staticmethod
     def get_package_run_dir(package_name):
         package_file_no_extension = str(package_name).split('.')[0]
         package_run_dir = os.path.join(ClientConstants.get_package_unzip_dir(),
                                        package_file_no_extension)
+        if not os.path.exists(package_run_dir):
+            os.makedirs(package_run_dir)
         return package_run_dir
 
     @staticmethod
     def get_model_cache_dir():
         model_cache_dir = os.path.join(ClientConstants.get_fedml_home_dir(), "fedml", "model_cache")
+        if not os.path.exists(model_cache_dir):
+            os.makedirs(model_cache_dir)
         return model_cache_dir
 
     @staticmethod
     def get_database_dir():
         database_dir = os.path.join(ClientConstants.get_data_dir(), "database")
+        if not os.path.exists(database_dir):
+            os.makedirs(database_dir)
         return database_dir
 
     @staticmethod
-    def cleanup_run_process():
+    def cleanup_run_process(run_id):
         try:
             local_pkg_data_dir = ClientConstants.get_data_dir()
             process_id_file = os.path.join(local_pkg_data_dir, ClientConstants.LOCAL_RUNNER_INFO_DIR_NAME,
-                                           "runner-sub-process.id")
+                                           "runner-sub-process-v2.id")
+            if not os.path.exists(process_id_file):
+                return
             process_info = load_yaml_config(process_id_file)
-            process_id = process_info.get('process_id', None)
+            if run_id is None:
+                for run_id_key, process_id_value in process_info.items():
+                    ClientConstants.cleanup_run_process(run_id_key)
+                return
+            process_id = process_info.get(str(run_id), None)
             if process_id is not None:
                 try:
                     process = psutil.Process(process_id)
                     for sub_process in process.children():
                         if platform.system() == 'Windows':
                             os.system("taskkill /PID {} /T /F".format(sub_process.pid))
                         else:
@@ -128,71 +150,134 @@
                     if process is not None:
                         if platform.system() == 'Windows':
                             os.system("taskkill /PID {} /T /F".format(process.pid))
                         else:
                             os.kill(process.pid, signal.SIGKILL)
                 except Exception as e:
                     pass
-            yaml_object = {}
-            yaml_object['process_id'] = -1
-            ClientConstants.generate_yaml_doc(yaml_object, process_id_file)
+
+                process_info.pop(str(run_id))
+                ClientConstants.generate_yaml_doc(process_info, process_id_file)
         except Exception as e:
             pass
 
     @staticmethod
-    def save_run_process(process_id):
+    def save_run_process(run_id, process_id):
         try:
             local_pkg_data_dir = ClientConstants.get_data_dir()
             process_id_file = os.path.join(local_pkg_data_dir, ClientConstants.LOCAL_RUNNER_INFO_DIR_NAME,
-                                           "runner-sub-process.id")
-            yaml_object = {}
-            yaml_object['process_id'] = process_id
-            ClientConstants.generate_yaml_doc(yaml_object, process_id_file)
+                                           "runner-sub-process-v2.id")
+            if os.path.exists(process_id_file):
+                process_info = load_yaml_config(process_id_file)
+            else:
+                process_info = dict()
+            process_info[str(run_id)] = process_id
+            ClientConstants.generate_yaml_doc(process_info, process_id_file)
         except Exception as e:
             pass
 
     @staticmethod
-    def cleanup_learning_process():
+    def cleanup_learning_process(run_id):
         try:
             local_pkg_data_dir = ClientConstants.get_data_dir()
             process_id_file = os.path.join(local_pkg_data_dir, ClientConstants.LOCAL_RUNNER_INFO_DIR_NAME,
-                                           "runner-learning-process.id")
+                                           "runner-learning-process-v2.id")
+            if not os.path.exists(process_id_file):
+                return
             process_info = load_yaml_config(process_id_file)
-            process_id = process_info.get('process_id', None)
+            if run_id is None:
+                for run_id_key, process_id_value in process_info.items():
+                    ClientConstants.cleanup_learning_process(run_id_key)
+                return
+            process_id = process_info.get(str(run_id), None)
             if process_id is not None:
                 try:
                     process = psutil.Process(process_id)
                     for sub_process in process.children():
                         if platform.system() == 'Windows':
                             os.system("taskkill /PID {} /T /F".format(sub_process.pid))
                         else:
-                            os.kill(sub_process.pid, signal.SIGKILL)
+                            os.kill(sub_process.pid, signal.SIGTERM)
 
                     if process is not None:
                         if platform.system() == 'Windows':
                             os.system("taskkill /PID {} /T /F".format(process.pid))
                         else:
-                            os.kill(process.pid, signal.SIGKILL)
+                            os.kill(process.pid, signal.SIGTERM)
+                except Exception as e:
+                    pass
+
+                process_info.pop(str(run_id))
+                ClientConstants.generate_yaml_doc(process_info, process_id_file)
+        except Exception as e:
+            pass
+
+    @staticmethod
+    def save_learning_process(run_id, learning_id):
+        try:
+            local_pkg_data_dir = ClientConstants.get_data_dir()
+            process_id_file = os.path.join(local_pkg_data_dir, ClientConstants.LOCAL_RUNNER_INFO_DIR_NAME,
+                                           "runner-learning-process-v2.id")
+            if os.path.exists(process_id_file):
+                process_info = load_yaml_config(process_id_file)
+            else:
+                process_info = dict()
+            process_info[str(run_id)] = learning_id
+            ClientConstants.generate_yaml_doc(process_info, process_id_file)
+        except Exception as e:
+            pass
+
+    @staticmethod
+    def cleanup_bootstrap_process(run_id):
+        try:
+            local_pkg_data_dir = ClientConstants.get_data_dir()
+            process_id_file = os.path.join(local_pkg_data_dir, ClientConstants.LOCAL_RUNNER_INFO_DIR_NAME,
+                                           "runner-bootstrap-process-v2.id")
+            if not os.path.exists(process_id_file):
+                return
+            process_info = load_yaml_config(process_id_file)
+            if run_id is None:
+                for run_id_key, process_id_value in process_info.items():
+                    ClientConstants.cleanup_bootstrap_process(run_id_key)
+                return
+            process_id = process_info.get(str(run_id), None)
+            if process_id is not None:
+                try:
+                    process = psutil.Process(process_id)
+                    for sub_process in process.children():
+                        if platform.system() == 'Windows':
+                            os.system("taskkill /PID {} /T /F".format(sub_process.pid))
+                        else:
+                            os.kill(sub_process.pid, signal.SIGTERM)
+
+                    if process is not None:
+                        if platform.system() == 'Windows':
+                            os.system("taskkill /PID {} /T /F".format(process.pid))
+                        else:
+                            os.kill(process.pid, signal.SIGTERM)
                 except Exception as e:
                     pass
-            yaml_object = {}
-            yaml_object['process_id'] = -1
-            ClientConstants.generate_yaml_doc(yaml_object, process_id_file)
+
+                process_info.pop(str(run_id))
+                ClientConstants.generate_yaml_doc(process_info, process_id_file)
         except Exception as e:
             pass
 
     @staticmethod
-    def save_learning_process(learning_id):
+    def save_bootstrap_process(run_id, process_id):
         try:
             local_pkg_data_dir = ClientConstants.get_data_dir()
             process_id_file = os.path.join(local_pkg_data_dir, ClientConstants.LOCAL_RUNNER_INFO_DIR_NAME,
-                                           "runner-learning-process.id")
-            yaml_object = {}
-            yaml_object['process_id'] = learning_id
-            ClientConstants.generate_yaml_doc(yaml_object, process_id_file)
+                                           "runner-bootstrap-process-v2.id")
+            if os.path.exists(process_id_file):
+                process_info = load_yaml_config(process_id_file)
+            else:
+                process_info = dict()
+            process_info[str(run_id)] = process_id
+            ClientConstants.generate_yaml_doc(process_info, process_id_file)
         except Exception as e:
             pass
 
     @staticmethod
     def save_runner_infos(unique_device_id, edge_id, run_id=None):
         local_pkg_data_dir = ClientConstants.get_data_dir()
         try:
@@ -273,36 +358,48 @@
 
     @staticmethod
     def exec_console_with_script(script_path, should_capture_stdout=False, should_capture_stderr=False):
         stdout_flag = subprocess.PIPE if should_capture_stdout else sys.stdout
         stderr_flag = subprocess.PIPE if should_capture_stderr else sys.stderr
 
         if platform.system() == 'Windows':
-            script_process = subprocess.Popen(script_path, stdout=stdout_flag, stderr=stderr_flag)
+            script_process = subprocess.Popen(script_path, stdout=stdout_flag, stderr=stderr_flag,
+                                              creationflags=subprocess.CREATE_NEW_PROCESS_GROUP)
         else:
-            script_process = subprocess.Popen(['bash', '-c', script_path], stdout=stdout_flag, stderr=stderr_flag)
+            script_process = subprocess.Popen(['bash', '-c', script_path], stdout=stdout_flag, stderr=stderr_flag,
+                                              preexec_fn=os.setsid)
 
         return script_process
 
     @staticmethod
     def exec_console_with_shell(shell, script_path, should_capture_stdout=False, should_capture_stderr=False):
         stdout_flag = subprocess.PIPE if should_capture_stdout else sys.stdout
         stderr_flag = subprocess.PIPE if should_capture_stderr else sys.stderr
 
-        script_process = subprocess.Popen([shell, script_path], stdout=stdout_flag, stderr=stderr_flag)
+        if platform.system() == 'Windows':
+            script_process = subprocess.Popen([shell, script_path], stdout=stdout_flag, stderr=stderr_flag,
+                                              creationflags=subprocess.CREATE_NEW_PROCESS_GROUP)
+        else:
+            script_process = subprocess.Popen([shell, script_path], stdout=stdout_flag, stderr=stderr_flag,
+                                              preexec_fn=os.setsid)
 
         return script_process
 
     @staticmethod
     def exec_console_with_shell_script_list(shell_script_list, should_capture_stdout=False,
                                             should_capture_stderr=False):
         stdout_flag = subprocess.PIPE if should_capture_stdout else sys.stdout
         stderr_flag = subprocess.PIPE if should_capture_stderr else sys.stderr
 
-        script_process = subprocess.Popen(shell_script_list, stdout=stdout_flag, stderr=stderr_flag)
+        if platform.system() == 'Windows':
+            script_process = subprocess.Popen(shell_script_list, stdout=stdout_flag, stderr=stderr_flag,
+                                              creationflags=subprocess.CREATE_NEW_PROCESS_GROUP)
+        else:
+            script_process = subprocess.Popen(shell_script_list, stdout=stdout_flag, stderr=stderr_flag,
+                                              preexec_fn=os.setsid)
 
         return script_process
 
     @staticmethod
     def get_console_pipe_out_err_results(script_process):
         exec_out, exec_err = script_process.communicate()
         return script_process.returncode, exec_out, exec_err
```

### Comparing `fedml-0.8.4a9/fedml/cli/edge_deployment/client_diagnosis.py` & `fedml-0.8.5a1/fedml/cli/edge_deployment/client_diagnosis.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cli/edge_deployment/client_api.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_client_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from fastapi import FastAPI, Request
-from fedml.cli.edge_deployment.client_data_interface import FedMLClientDataInterface
+from fedml.cli.model_deployment.device_client_data_interface import FedMLClientDataInterface
 
 
 api = FastAPI()
 
 
 @api.get('/')
 def root():
-    return {'message': 'FedML Client Local API Service!'}
+    return {'message': 'FedML Model Client Local API Service!'}
 
 
 @api.post('/fedml/api/v2/currentJobStatus')
 async def get_current_job_status(request: Request):
     # Get json data
     input_json = await request.json()
```

### Comparing `fedml-0.8.4a9/fedml/cli/edge_deployment/simulator_daemon.py` & `fedml-0.8.5a1/fedml/cli/edge_deployment/simulator_daemon.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_model_inference.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_model_inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,17 +67,21 @@
         print("inference url {}.".format(inference_output_url))
         if inference_output_url != "":
             input_list = input_json["inputs"]
             output_list = input_json["outputs"]
             inference_response = send_inference_request(inference_output_url, input_list, output_list)
 
         # Calculate model metrics
-        model_metrics.calc_metrics(end_point_id, in_end_point_name,
-                                   model_id, model_name, model_version,
-                                   inference_output_url)
+        try:
+            model_metrics.calc_metrics(end_point_id, in_end_point_name,
+                                        model_id, model_name, model_version,
+                                        inference_output_url, idle_device)
+        except Exception as e:
+            print("Calculate Inference Metrics Exception: {}".format(traceback.format_exc()))
+            pass
 
         logging_inference_request(input_json, inference_response)
 
         return inference_response
 
     else:
         inference_response = {"error": True, "message": "token is not valid."}
@@ -133,11 +137,17 @@
     if cached_token is not None and cached_token == token:
         return True
 
     return False
 
 
 def logging_inference_request(request, response):
-    inference_log_file = os.path.join(ServerConstants.get_log_file_dir(), "inference.log")
-    with open(inference_log_file, "a") as f:
-        f.writelines([f"request: {request}, response: {response}\n"])
+    try:
+        log_dir = ServerConstants.get_log_file_dir()
+        if not os.path.exists(log_dir):
+            os.makedirs(log_dir)
+        inference_log_file = os.path.join(log_dir, "inference.log")
+        with open(inference_log_file, "a") as f:
+            f.writelines([f"request: {request}, response: {response}\n"])
+    except Exception as ex:
+        print("failed to log inference request and response to file.")
```

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_client_daemon.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_client_daemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 
 import argparse
 import os
 import time
-import sys
 
 from fedml.cli.comm_utils import sys_utils
 from fedml.cli.model_deployment.device_client_constants import ClientConstants
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
@@ -22,17 +21,17 @@
     args = parser.parse_args()
     args.user = args.user
 
     pip_source_dir = os.path.dirname(__file__)
     login_cmd = os.path.join(pip_source_dir, "device_client_login.py")
     while True:
         try:
-            ClientConstants.cleanup_run_process()
+            ClientConstants.cleanup_run_process(None)
             sys_utils.cleanup_all_fedml_client_api_processes(is_model_device=True)
-            sys_utils.cleanup_all_fedml_client_learning_processes()
+            sys_utils.cleanup_all_fedml_client_learning_processes(None)
             sys_utils.cleanup_all_fedml_client_login_processes("device_client_login.py", clean_process_group=False)
         except Exception as e:
             pass
 
         sys_utils.daemon_ota_upgrade(args)
 
         login_pid = ClientConstants.exec_console_with_shell_script_list(
```

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/modelops_configs.py` & `fedml-0.8.5a1/fedml/core/mlops/mlops_configs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,187 +1,240 @@
 
 import os
+import time
 import certifi
 import requests
+from fedml.core.mlops.mlops_utils import MLOpsUtils
 
 
 class Singleton(object):
     def __new__(cls):
         if not hasattr(cls, "_instance"):
             orig = super(Singleton, cls)
             cls._instance = orig.__new__(cls)
         return cls._instance
 
 
-class ModelOpsConfigs(Singleton):
+class MLOpsConfigs(object):
     _config_instance = None
 
+    def __new__(cls):
+        if not hasattr(cls, "_instance"):
+            orig = super(MLOpsConfigs, cls)
+            cls._instance = orig.__new__(cls)
+            cls._instance.init()
+        return cls._instance
+
     def __init__(self):
+        pass
+
+    def init(self):
         self.args = None
 
     @staticmethod
     def get_instance(args):
-        if ModelOpsConfigs._config_instance is None:
-            ModelOpsConfigs._config_instance = ModelOpsConfigs()
-            ModelOpsConfigs._config_instance.args = args
+        if MLOpsConfigs._config_instance is None:
+            MLOpsConfigs._config_instance = MLOpsConfigs()
+            MLOpsConfigs._config_instance.args = args
 
-        return ModelOpsConfigs._config_instance
+        return MLOpsConfigs._config_instance
 
-    def get_request_params(self, in_config_version="release"):
+    def get_request_params(self):
         url = "https://open.fedml.ai/fedmlOpsServer/configs/fetch"
         config_version = "release"
-        if in_config_version is not None and in_config_version != "":
+        if (
+                hasattr(self.args, "config_version")
+                and self.args.config_version is not None
+        ):
             # Setup config url based on selected version.
-            config_version = in_config_version
-            if config_version == "release":
+            config_version = self.args.config_version
+            if self.args.config_version == "release":
                 url = "https://open.fedml.ai/fedmlOpsServer/configs/fetch"
-            elif config_version == "test":
+            elif self.args.config_version == "test":
                 url = "https://open-test.fedml.ai/fedmlOpsServer/configs/fetch"
-            elif config_version == "dev":
+            elif self.args.config_version == "dev":
                 url = "https://open-dev.fedml.ai/fedmlOpsServer/configs/fetch"
-            elif config_version == "local":
+            elif self.args.config_version == "local":
                 if hasattr(self.args, "local_server") and self.args.local_server is not None:
                     url = "http://{}:9000/fedmlOpsServer/configs/fetch".format(self.args.local_server)
                 else:
                     url = "http://localhost:9000/fedmlOpsServer/configs/fetch"
 
         cert_path = None
         if str(url).startswith("https://"):
             cur_source_dir = os.path.dirname(__file__)
             cert_path = os.path.join(
-                cur_source_dir, "ssl", "model-" + config_version + ".fedml.ai_bundle.crt"
+                cur_source_dir, "ssl", "open-" + config_version + ".fedml.ai_bundle.crt"
+            )
+
+        return url, cert_path
+
+    def get_request_params_with_version(self, version):
+        url = "https://open.fedml.ai/fedmlOpsServer/configs/fetch"
+        if version == "release":
+            url = "https://open.fedml.ai/fedmlOpsServer/configs/fetch"
+        elif version == "test":
+            url = "https://open-test.fedml.ai/fedmlOpsServer/configs/fetch"
+        elif version == "dev":
+            url = "https://open-dev.fedml.ai/fedmlOpsServer/configs/fetch"
+        elif version == "local":
+            if hasattr(self.args, "local_server") and self.args.local_server is not None:
+                url = "http://{}:9000/fedmlOpsServer/configs/fetch".format(self.args.local_server)
+            else:
+                url = "http://localhost:9000/fedmlOpsServer/configs/fetch"
+
+        cert_path = None
+        if str(url).startswith("https://"):
+            cur_source_dir = os.path.dirname(__file__)
+            cert_path = os.path.join(
+                cur_source_dir, "ssl", "open-" + version + ".fedml.ai_bundle.crt"
             )
 
         return url, cert_path
 
     @staticmethod
     def get_root_ca_path():
         cur_source_dir = os.path.dirname(__file__)
-        cert_path = os.path.join(cur_source_dir, "..", "..", "core", "mlops", "ssl", "open-root-ca.crt")
+        cert_path = os.path.join(
+            cur_source_dir, "ssl", "open-root-ca.crt"
+        )
         return cert_path
 
     @staticmethod
     def install_root_ca_file():
         ca_file = certifi.where()
-        open_root_ca_path = ModelOpsConfigs.get_root_ca_path()
+        open_root_ca_path = MLOpsConfigs.get_root_ca_path()
         with open(open_root_ca_path, 'rb') as infile:
             open_root_ca_file = infile.read()
         with open(ca_file, 'ab') as outfile:
             outfile.write(open_root_ca_file)
 
-    def fetch_configs(self, config_version="release"):
-        url, cert_path = self.get_request_params(config_version)
-        json_params = {"config_name": ["mqtt_config", "s3_config"]}
+    def fetch_configs(self):
+        url, cert_path = self.get_request_params()
+        json_params = {"config_name": ["mqtt_config", "s3_config", "ml_ops_config"],
+                       "device_send_time": int(time.time() * 1000)}
 
         if cert_path is not None:
             try:
                 requests.session().verify = cert_path
                 response = requests.post(
                     url, json=json_params, verify=True, headers={"content-type": "application/json", "Connection": "close"}
                 )
             except requests.exceptions.SSLError as err:
-                ModelOpsConfigs.install_root_ca_file()
+                MLOpsConfigs.install_root_ca_file()
                 response = requests.post(
                     url, json=json_params, verify=True, headers={"content-type": "application/json", "Connection": "close"}
                 )
         else:
             response = requests.post(
                 url, json=json_params, headers={"content-type": "application/json", "Connection": "close"}
             )
 
         status_code = response.json().get("code")
         if status_code == "SUCCESS":
             mqtt_config = response.json().get("data").get("mqtt_config")
             s3_config = response.json().get("data").get("s3_config")
+            mlops_config = response.json().get("data").get("ml_ops_config")
+            MLOpsUtils.calc_ntp_from_config(mlops_config)
         else:
             raise Exception("failed to fetch device configurations!")
         return mqtt_config, s3_config
 
     def fetch_web3_configs(self):
         url, cert_path = self.get_request_params()
-        json_params = {"config_name": ["mqtt_config", "web3_config"]}
+        json_params = {"config_name": ["mqtt_config", "web3_config", "ml_ops_config"],
+                       "device_send_time": int(time.time() * 1000)}
 
         if cert_path is not None:
             try:
                 requests.session().verify = cert_path
                 response = requests.post(
                     url, json=json_params, verify=True, headers={"content-type": "application/json", "Connection": "close"}
                 )
             except requests.exceptions.SSLError as err:
-                ModelOpsConfigs.install_root_ca_file()
+                MLOpsConfigs.install_root_ca_file()
                 response = requests.post(
                     url, json=json_params, verify=True, headers={"content-type": "application/json", "Connection": "close"}
                 )
         else:
             response = requests.post(
                 url, json=json_params, headers={"content-type": "application/json", "Connection": "close"}
             )
 
         status_code = response.json().get("code")
         if status_code == "SUCCESS":
             mqtt_config = response.json().get("data").get("mqtt_config")
             web3_config = response.json().get("data").get("web3_config")
+            mlops_config = response.json().get("data").get("ml_ops_config")
+            MLOpsUtils.calc_ntp_from_config(mlops_config)
         else:
             raise Exception("failed to fetch device configurations!")
         return mqtt_config, web3_config
 
     def fetch_thetastore_configs(self):
         url, cert_path = self.get_request_params()
-        json_params = {"config_name": ["mqtt_config", "thetastore_config"]}
+        json_params = {"config_name": ["mqtt_config", "thetastore_config", "ml_ops_config"],
+                       "device_send_time": int(time.time() * 1000)}
 
         if cert_path is not None:
             try:
                 requests.session().verify = cert_path
                 response = requests.post(
                     url, json=json_params, verify=True, headers={"content-type": "application/json", "Connection": "close"}
                 )
             except requests.exceptions.SSLError as err:
-                ModelOpsConfigs.install_root_ca_file()
+                MLOpsConfigs.install_root_ca_file()
                 response = requests.post(
                     url, json=json_params, verify=True, headers={"content-type": "application/json", "Connection": "close"}
                 )
         else:
             response = requests.post(
                 url, json=json_params, headers={"content-type": "application/json", "Connection": "close"}
             )
 
         status_code = response.json().get("code")
         if status_code == "SUCCESS":
             mqtt_config = response.json().get("data").get("mqtt_config")
             thetastore_config = response.json().get("data").get("thetastore_config")
+            mlops_config = response.json().get("data").get("ml_ops_config")
+            MLOpsUtils.calc_ntp_from_config(mlops_config)
         else:
             raise Exception("failed to fetch device configurations!")
         return mqtt_config, thetastore_config
 
     def fetch_all_configs(self):
         url, cert_path = self.get_request_params()
-        json_params = {"config_name": ["mqtt_config", "s3_config", "ml_ops_config", "docker_config"]}
+        json_params = {
+            "config_name": ["mqtt_config", "s3_config", "ml_ops_config", "docker_config"],
+            "device_send_time": int(time.time() * 1000)
+        }
 
         if cert_path is not None:
             try:
                 requests.session().verify = cert_path
                 response = requests.post(
                     url, json=json_params, verify=True, headers={"content-type": "application/json", "Connection": "close"}
                 )
             except requests.exceptions.SSLError as err:
-                ModelOpsConfigs.install_root_ca_file()
+                MLOpsConfigs.install_root_ca_file()
                 response = requests.post(
                     url, json=json_params, verify=True, headers={"content-type": "application/json", "Connection": "close"}
                 )
         else:
             response = requests.post(
                 url, json=json_params, headers={"content-type": "application/json", "Connection": "close"}
             )
 
         status_code = response.json().get("code")
         if status_code == "SUCCESS":
             mqtt_config = response.json().get("data").get("mqtt_config")
             s3_config = response.json().get("data").get("s3_config")
             mlops_config = response.json().get("data").get("ml_ops_config")
             docker_config = response.json().get("data").get("docker_config")
+            MLOpsUtils.calc_ntp_from_config(mlops_config)
         else:
             raise Exception("failed to fetch device configurations!")
 
         return mqtt_config, s3_config, mlops_config, docker_config
 
 
 if __name__ == "__main__":
```

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_server_api.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_server_api.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_server_runner.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_server_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import copy
 import json
 import logging
 import multiprocessing
 import platform
-import random
 import sys
 
 from multiprocessing import Process
 import os
 import shutil
 import subprocess
 import threading
@@ -15,15 +14,14 @@
 import time
 import traceback
 import urllib
 import uuid
 import zipfile
 from os import listdir
 
-import click
 import requests
 import torch
 
 from ..comm_utils import sys_utils
 from .device_server_data_interface import FedMLServerDataInterface
 from ...core.mlops.mlops_runtime_log import MLOpsRuntimeLog
 
@@ -37,14 +35,15 @@
 from ...core.mlops.mlops_configs import MLOpsConfigs
 from ...core.mlops.mlops_runtime_log_daemon import MLOpsRuntimeLogDaemon
 from ...core.mlops.mlops_status import MLOpsStatus
 from ..comm_utils.sys_utils import get_sys_runner_info, get_python_program
 from .device_model_cache import FedMLModelCache
 from .device_model_msg_object import FedMLModelMsgObject
 from ...serving.fedml_server import FedMLModelServingServer
+from ...core.mlops.mlops_utils import MLOpsUtils
 
 
 class RunnerError(BaseException):
     """ Runner failed. """
     pass
 
 
@@ -94,14 +93,15 @@
         self.redis_port = "6379"
         self.redis_password = "fedml_default"
 
         self.slave_deployment_statuses_mapping = {}
         self.slave_deployment_results_mapping = {}
 
         self.model_runner_mapping = dict()
+        self.ntp_offset = MLOpsUtils.get_ntp_offset()
 
     def build_dynamic_constrain_variables(self, run_id, run_config):
         pass
 
     def unzip_file(self, zip_file, unzip_file_path):
         result = False
         if zipfile.is_zipfile(zip_file):
@@ -151,15 +151,15 @@
 
     def update_local_fedml_config(self, run_id, run_config):
         model_config = run_config
         model_name = model_config["model_name"]
         model_storage_url = model_config["model_storage_url"]
         scale_min = model_config["instance_scale_min"]
         scale_max = model_config["instance_scale_max"]
-        inference_engine = model_config["inference_engine"]
+        inference_engine = model_config.get("inference_engine", 0)
         inference_end_point_id = run_id
 
         # Copy config file from the client
         unzip_package_path = self.retrieve_and_unzip_package(
             model_name, model_storage_url
         )
         fedml_local_config_file = os.path.join(unzip_package_path, "fedml_model_config.yaml")
@@ -176,29 +176,43 @@
 
     def run(self, process_event):
         os.environ['PYTHONWARNINGS'] = 'ignore:semaphore_tracker:UserWarning'
         os.environ.setdefault('PYTHONWARNINGS', 'ignore:semaphore_tracker:UserWarning')
 
         self.run_process_event = process_event
         try:
+            MLOpsUtils.set_ntp_offset(self.ntp_offset)
+
             self.setup_client_mqtt_mgr()
 
             self.run_impl()
         except RunnerError:
             logging.info("Runner stopped.")
             self.mlops_metrics.report_server_training_status(self.run_id,
                                                              ServerConstants.MSG_MLOPS_SERVER_STATUS_KILLED,
                                                              is_from_model=True)
         except Exception as e:
-            logging.info("Runner exits with exceptions.")
+            logging.error("Runner exits with exceptions.")
+            self.mlops_metrics.report_server_training_status(self.run_id,
+                                                             ServerConstants.MSG_MLOPS_SERVER_STATUS_FAILED,
+                                                             is_from_model=True)
+            MLOpsRuntimeLogDaemon.get_instance(self.args).stop_log_processor(self.run_id, self.edge_id)
+            if self.mlops_metrics is not None:
+                self.mlops_metrics.stop_sys_perf()
+            time.sleep(3)
+            time.sleep(3)
             sys_utils.cleanup_all_fedml_server_login_processes(ServerConstants.SERVER_LOGIN_PROGRAM,
                                                                clean_process_group=False)
             sys.exit(1)
         finally:
             logging.info("Release resources.")
+            MLOpsRuntimeLogDaemon.get_instance(self.args).stop_log_processor(self.run_id, self.edge_id)
+            if self.mlops_metrics is not None:
+                self.mlops_metrics.stop_sys_perf()
+            time.sleep(3)
             if not self.run_as_cloud_server:
                 self.release_client_mqtt_mgr()
 
     def parse_model_run_params(self, running_json):
         run_id = running_json["end_point_id"]
         end_point_name = running_json["end_point_name"]
         token = running_json["token"]
@@ -209,15 +223,15 @@
 
         model_config = running_json["model_config"]
         model_name = model_config["model_name"]
         model_id = model_config["model_id"]
         model_storage_url = model_config["model_storage_url"]
         scale_min = model_config["instance_scale_min"]
         scale_max = model_config["instance_scale_max"]
-        inference_engine = model_config["inference_engine"]
+        inference_engine = model_config.get("inference_engine", 0)
         model_is_from_open = model_config["is_from_open"]
         inference_end_point_id = run_id
         use_gpu = "gpu"  # TODO: Get GPU from device infos
         memory_size = "256m"  # TODO: Get Memory size for each instance
         model_version = model_config["model_version"]
 
         return run_id, end_point_name, token, user_id, user_name, device_ids, device_objs, model_config, model_name, \
@@ -372,15 +386,15 @@
 
         self.mlops_metrics.broadcast_server_training_status(
             self.run_id, ServerConstants.MSG_MLOPS_SERVER_STATUS_FINISHED,
             is_from_model=True
         )
 
         try:
-            self.mlops_metrics.set_sys_reporting_status(False)
+            self.mlops_metrics.stop_sys_perf()
         except Exception as ex:
             pass
 
         time.sleep(1)
 
         try:
             local_package_path = ServerConstants.get_package_download_dir()
@@ -394,15 +408,15 @@
         logging.info("Cleanup run successfully when starting failed.")
 
         self.mlops_metrics.broadcast_server_training_status(self.run_id,
                                                             ServerConstants.MSG_MLOPS_SERVER_STATUS_FAILED,
                                                             is_from_model=True)
 
         try:
-            self.mlops_metrics.set_sys_reporting_status(False)
+            self.mlops_metrics.stop_sys_perf()
         except Exception as ex:
             pass
 
         time.sleep(1)
 
         try:
             local_package_path = ServerConstants.get_package_download_dir()
@@ -494,37 +508,44 @@
             payload_json["port"] = model_inference_port
             token = FedMLModelCache.get_instance(self.redis_addr, self.redis_port). \
                 get_end_point_token(end_point_name, model_name)
 
             model_metadata = payload_json["model_metadata"]
             model_inputs = model_metadata["inputs"]
             ret_inputs = list()
-
-            for input_item in model_inputs:
-                ret_item = input_item
-                shape = ret_item["shape"]
-                data_type = ret_item["datatype"]
-                if ServerConstants.MODEL_DATA_TYPE_MAPPING[data_type] == ServerConstants.MODEL_DATA_TYPE_INT:
-                    for i in range(len(shape)):
-                        if shape[i] == -1:  # if input shape is dynamic, we set a default value 1
-                            shape[i] = 1
-                    ret_item["data"] = torch.randint(0, 1, shape).tolist()
-                else:
-                    for i in range(len(shape)):
-                        if shape[i] == -1:  # if input shape is dynamic, we set a default value 1
-                            shape[i] = 1
-                    ret_item["data"] = torch.zeros(shape).tolist()
-                ret_inputs.append(ret_item)
-
-            payload_json["input_json"] = {"end_point_name": end_point_name,
-                                          "model_name": model_name,
-                                          "token": str(token),
-                                          "inputs": ret_inputs,
-                                          "outputs": model_metadata["outputs"]}
-            payload_json["output_json"] = model_metadata["outputs"]
+            if "type" in model_metadata and model_metadata["type"] == "llm":
+                payload_json["input_json"] = {"end_point_name": end_point_name,
+                                            "model_name": model_name,
+                                            "token": str(token),
+                                            "inputs": model_inputs,
+                                            "outputs": []}
+                payload_json["output_json"] = model_metadata["outputs"]
+            else:
+                for input_item in model_inputs:
+                    ret_item = input_item
+                    shape = ret_item["shape"]
+                    data_type = ret_item["datatype"]
+                    if ServerConstants.MODEL_DATA_TYPE_MAPPING[data_type] == ServerConstants.MODEL_DATA_TYPE_INT:
+                        for i in range(len(shape)):
+                            if shape[i] == -1:  # if input shape is dynamic, we set a default value 1
+                                shape[i] = 1
+                        ret_item["data"] = torch.randint(0, 1, shape).tolist()
+                    else:
+                        for i in range(len(shape)):
+                            if shape[i] == -1:  # if input shape is dynamic, we set a default value 1
+                                shape[i] = 1
+                        ret_item["data"] = torch.zeros(shape).tolist()
+                    ret_inputs.append(ret_item)
+                
+                payload_json["input_json"] = {"end_point_name": end_point_name,
+                                            "model_name": model_name,
+                                            "token": str(token),
+                                            "inputs": ret_inputs,
+                                            "outputs": model_metadata["outputs"]}
+                payload_json["output_json"] = model_metadata["outputs"]
             FedMLModelCache.get_instance(self.redis_addr, self.redis_port). \
                 set_deployment_result(end_point_id, end_point_name,
                                       model_name, model_version,
                                       self.edge_id, json.dumps(payload_json))
             FedMLModelCache.get_instance(self.redis_addr, self.redis_port). \
                 set_end_point_activation(end_point_id, end_point_name, True)
             self.send_deployment_results_with_payload(self.run_id, end_point_name, payload_json)
@@ -673,14 +694,19 @@
             raise Exception("Restarting after upgraded...")
 
     def callback_start_deployment(self, topic, payload):
         """
         topic: model_ops/model_device/start_deployment/model-agent-device-id
         payload: {"timestamp": 1671440005119, "end_point_id": 4325, "token": "FCpWU", "state": "STARTING","user_id": "105", "user_name": "alex.liang2", "device_ids": [693], "device_objs": [{"device_id": "0xT3630FW2YM@MacOS.Edge.Device", "os_type": "MacOS", "id": 693, "ip": "1.1.1.1", "memory": 1024, "cpu": "1.7", "gpu": "Nvidia", "extra_infos":{}}], "model_config": {"model_name": "image-model", "model_id": 111, "model_version": "v1", 'is_from_open": 0, "model_storage_url": "https://fedml.s3.us-west-1.amazonaws.com/1666239314792client-package.zip", "instance_scale_min": 1, "instance_scale_max": 3, "inference_engine": "onnx"}, "parameters": {"hidden_size": 128, "hidden_act": "gelu", "initializer_range": 0.02, "vocab_size": 30522, "hidden_dropout_prob": 0.1, "num_attention_heads": 2, "type_vocab_size": 2, "max_position_embeddings": 512, "num_hidden_layers": 2, "intermediate_size": 512, "attention_probs_dropout_prob": 0.1}}
         """
+        try:
+            _, _ = MLOpsConfigs.get_instance(self.args).fetch_configs()
+        except Exception as e:
+            pass
+
         logging.info("callback_start_deployment {}".format(payload))
 
         # get deployment params
         request_json = json.loads(payload)
         run_id = request_json["end_point_id"]
         end_point_name = request_json["end_point_name"]
         token = request_json["token"]
@@ -691,15 +717,15 @@
 
         model_config = request_json["model_config"]
         model_name = model_config["model_name"]
         model_id = model_config["model_id"]
         model_storage_url = model_config["model_storage_url"]
         scale_min = model_config["instance_scale_min"]
         scale_max = model_config["instance_scale_max"]
-        inference_engine = model_config["inference_engine"]
+        inference_engine = model_config.get("inference_engine", 0)
         inference_end_point_id = run_id
 
         # Start log processor for current run
         self.args.run_id = run_id
         self.args.edge_id = self.edge_id
         MLOpsRuntimeLog.get_instance(self.args).init_logs(show_stdout_log=True)
         MLOpsRuntimeLogDaemon.get_instance(self.args).set_log_source(
@@ -756,15 +782,15 @@
                 self.run_process_event = multiprocessing.Event()
             # server_runner.run(self.run_process_event)
             self.run_process_event.clear()
             server_runner.run_process_event = self.run_process_event
             self.model_runner_mapping[run_id] = server_runner
             server_process = Process(target=server_runner.run, args=(self.run_process_event,))
             server_process.start()
-            ServerConstants.save_run_process(server_process.pid)
+            ServerConstants.save_run_process(run_id, server_process.pid)
 
             # Send stage: MODEL_DEPLOYMENT_STAGE3 = "StartRunner"
             self.send_deployment_stages(self.run_id, model_name, model_id,
                                         "",
                                         ServerConstants.MODEL_DEPLOYMENT_STAGE3["index"],
                                         ServerConstants.MODEL_DEPLOYMENT_STAGE3["text"],
                                         ServerConstants.MODEL_DEPLOYMENT_STAGE3["text"])
@@ -838,14 +864,16 @@
         model_msg_object = FedMLModelMsgObject(topic, payload)
 
         # Set end point as deactivated status
         FedMLModelCache.get_instance().set_redis_params(self.redis_addr, self.redis_port, self.redis_password)
         FedMLModelCache.get_instance(self.redis_addr, self.redis_port). \
             set_end_point_activation(model_msg_object.inference_end_point_id,
                                      model_msg_object.end_point_name, False)
+        FedMLModelCache.get_instance(self.redis_addr, self.redis_port). \
+            delete_end_point(model_msg_object.end_point_name, model_msg_object.model_name, model_msg_object.model_version)                                     
 
         self.send_deployment_delete_request_to_edges(payload, model_msg_object)
 
         self.set_runner_stopped_event(model_msg_object.run_id)
 
         self.stop_device_inference_monitor(model_msg_object.run_id, model_msg_object.end_point_name,
                                            model_msg_object.model_id, model_msg_object.model_name,
@@ -941,19 +969,19 @@
     def setup_client_mqtt_mgr(self):
         if self.client_mqtt_mgr is not None:
             return
 
         if self.client_mqtt_lock is None:
             self.client_mqtt_lock = threading.Lock()
 
-        logging.info(
-            "server agent config: {},{}".format(
-                self.agent_config["mqtt_config"]["BROKER_HOST"], self.agent_config["mqtt_config"]["BROKER_PORT"]
-            )
-        )
+        # logging.info(
+        #     "server agent config: {},{}".format(
+        #         self.agent_config["mqtt_config"]["BROKER_HOST"], self.agent_config["mqtt_config"]["BROKER_PORT"]
+        #     )
+        # )
 
         self.client_mqtt_mgr = MqttManager(
             self.agent_config["mqtt_config"]["BROKER_HOST"],
             self.agent_config["mqtt_config"]["BROKER_PORT"],
             self.agent_config["mqtt_config"]["MQTT_USER"],
             self.agent_config["mqtt_config"]["MQTT_PWD"],
             self.agent_config["mqtt_config"]["MQTT_KEEPALIVE"],
@@ -1010,16 +1038,16 @@
             sys.exit(1)
         finally:
             self.release_client_mqtt_mgr()
 
     def exit_run_with_exception(self):
         logging.info("Exit run successfully.")
 
-        ServerConstants.cleanup_learning_process()
-        ServerConstants.cleanup_run_process()
+        ServerConstants.cleanup_learning_process(self.run_id)
+        ServerConstants.cleanup_run_process(self.run_id)
 
         self.mlops_metrics.report_server_id_status(self.run_id,
                                                    ServerConstants.MSG_MLOPS_SERVER_STATUS_FAILED)
 
         time.sleep(1)
 
     def callback_exit_train_with_exception(self, topic, payload):
@@ -1184,15 +1212,15 @@
 
                 device_id = str(get_uuid())
             elif "posix" in os.name:
                 device_id = sys_utils.get_device_id_in_docker()
                 if device_id is None:
                     device_id = hex(uuid.getnode())
             else:
-                device_id = subprocess.Popen(
+                device_id = sys_utils.run_subprocess_open(
                     "hal-get-property --udi /org/freedesktop/Hal/devices/computer --key system.hardware.uuid".split()
                 )
                 device_id = hex(device_id)
 
         if device_id is not None and device_id != "":
             with open(file_for_device_id, 'w', encoding='utf-8') as f:
                 f.write(device_id)
@@ -1348,17 +1376,22 @@
         mqtt_client_object.subscribe(topic_report_status, qos=2)
         mqtt_client_object.subscribe(topic_ota_msg, qos=2)
 
         # Broadcast the first active message.
         self.send_agent_active_msg()
 
         # Echo results
-        click.echo("")
-        click.echo("Congratulations, you have logged into the FedML ModelOps platform successfully!")
-        click.echo("Your server unique device id is " + str(self.unique_device_id))
+        print("\n\nCongratulations, your device is connected to the FedML MLOps platform successfully!")
+        print(
+            "Your FedML Edge ID is " + str(self.edge_id) + ", unique device ID is "
+            + str(self.unique_device_id)
+            + "\n"
+        )
+
+        MLOpsRuntimeLog.get_instance(self.args).init_logs(show_stdout_log=True)
 
     def on_agent_mqtt_disconnected(self, mqtt_client_object):
         MLOpsStatus.get_instance().set_server_agent_status(
             self.edge_id, ServerConstants.MSG_MLOPS_SERVER_STATUS_OFFLINE
         )
 
     def recover_inference_and_monitor(self):
@@ -1372,14 +1405,15 @@
                     continue
 
                 run_id, end_point_name, token, user_id, user_name, device_ids, device_objs, model_config, model_name, \
                     model_id, model_storage_url, scale_min, scale_max, inference_engine, model_is_from_open, \
                     inference_end_point_id, use_gpu, memory_size, model_version = \
                     self.parse_model_run_params(json.loads(job.running_json))
 
+                FedMLModelCache.get_instance().set_redis_params(self.redis_addr, self.redis_port, self.redis_password)
                 is_activated = FedMLModelCache.get_instance(self.redis_addr, self.redis_port). \
                     get_end_point_activation(run_id)
                 if not is_activated:
                     continue
 
                 self.start_device_inference_gateway(run_id, end_point_name, model_id, model_name, model_version)
 
@@ -1440,17 +1474,16 @@
         self.setup_client_mqtt_mgr()
         self.mlops_metrics.report_server_training_status(self.run_id,
                                                          ServerConstants.MSG_MLOPS_SERVER_STATUS_IDLE,
                                                          is_from_model=True)
         MLOpsStatus.get_instance().set_server_agent_status(
             self.edge_id, ServerConstants.MSG_MLOPS_SERVER_STATUS_IDLE
         )
-        self.mlops_metrics.set_sys_reporting_status(enable=True, is_client=False)
         setattr(self.args, "mqtt_config_path", service_config["mqtt_config"])
-        self.mlops_metrics.report_sys_perf(self.args, is_client=False)
+        self.mlops_metrics.report_sys_perf(self.args)
 
         self.recover_start_deployment_msg_after_upgrading()
 
     def start_agent_mqtt_loop(self):
         # Start MQTT message loop
         try:
             self.mqtt_mgr.loop_forever()
```

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_model_cards.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_model_cards.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from ...core.distributed.communication.s3.remote_storage import S3Storage
 
 from .device_client_constants import ClientConstants
 from ...core.common.singleton import Singleton
 from .modelops_configs import ModelOpsConfigs
 from .device_model_deployment import get_model_info
 from .device_server_constants import ServerConstants
-from .device_model_object import FedMLModelList, FedMLModelObject
+from .device_model_object import FedMLModelList
 
 
 class FedMLModelCards(Singleton):
 
     def __init__(self):
         self.current_model_name = None
         self.local_deployment_end_point_id = None
```

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_client_api.py` & `fedml-0.8.5a1/fedml/cli/server_deployment/server_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from fastapi import FastAPI, Request
-from fedml.cli.model_deployment.device_client_data_interface import FedMLClientDataInterface
+from fedml.cli.server_deployment.server_data_interface import FedMLServerDataInterface
 
 
 api = FastAPI()
 
 
 @api.get('/')
 def root():
-    return {'message': 'FedML Model Client Local API Service!'}
+    return {'message': 'FedML Server Local API Service!'}
 
 
 @api.post('/fedml/api/v2/currentJobStatus')
 async def get_current_job_status(request: Request):
     # Get json data
     input_json = await request.json()
 
-    current_job = FedMLClientDataInterface.get_instance().get_current_job()
+    current_job = FedMLServerDataInterface.get_instance().get_current_job()
     if current_job is None:
         return {}
     response = {"jobId": current_job.job_id,
                 "edgeId": current_job.edge_id,
                 "startedTime": int(float(current_job.started_time)) if current_job.started_time != "" else 0,
                 "endedTime": int(float(current_job.ended_time)) if current_job.ended_time != "" else 0,
                 "progress": current_job.progress, "ETA": int(current_job.eta),
@@ -32,15 +32,15 @@
 
 @api.post('/fedml/api/v2/historyJobStatus')
 async def get_history_job_status(request: Request):
     # Get json data
     input_json = await request.json()
 
     responses = list()
-    history_jobs = FedMLClientDataInterface.get_instance().get_history_jobs()
+    history_jobs = FedMLServerDataInterface.get_instance().get_history_jobs()
     for job_item in history_jobs.job_list:
         response = {"jobId": job_item.job_id,
                     "edgeId": job_item.edge_id,
                     "startedTime": int(float(job_item.started_time)) if job_item.started_time != "" else 0,
                     "endedTime": int(float(job_item.ended_time)) if job_item.ended_time != "" else 0,
                     "failedTime": int(float(job_item.failed_time))if job_item.ended_time != "" else 0,
                     "errorCode": job_item.error_code,
```

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/docker_client_login.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/docker_client_login.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,18 +91,21 @@
             is_deployment_ok = True
     if err is not None:
         err_str = err.decode(encoding="utf-8")
         if str(err_str).find(fedml_docker_name) != -1 and str(err_str).find("Up") != -1:
             is_deployment_ok = True
 
     if is_deployment_ok:
-        click.echo("Congratulations, you have deployed the FedML client agent successfully!")
-        click.echo("Your device id is " + env_current_device_id + ".")
-        click.echo("You may review the device in the ModelOps edge device list.")
-
+        print("\n\nCongratulations, your device is connected to the FedML MLOps platform successfully!")
+        print(
+            "Your unique device ID is "
+            + str(env_current_device_id)
+            + "\n"
+        )
+        
         logs_with_docker_mode(docker_rank)
     else:
         click.echo("Oops, you failed to deploy the FedML client agent.")
         click.echo("Please check whether your Docker Application is installed and running normally!")
 
 
 def logout_with_docker_mode(docker_rank):
```

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_server_login.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_server_login.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import argparse
 import logging
 import os
 import platform
 import time
 
 import click
-from fedml.core.mlops.mlops_runtime_log import MLOpsRuntimeLog
 from fedml.cli.model_deployment.device_server_runner import FedMLServerRunner
 from fedml.cli.model_deployment.device_server_constants import ServerConstants
+from fedml.core.mlops.mlops_utils import MLOpsUtils
 
 
 def __login_as_edge_server_and_agent(args, userid, version):
     setattr(args, "account_id", userid)
     setattr(args, "current_running_dir", ServerConstants.get_fedml_home_dir())
 
     sys_name = platform.system()
@@ -119,16 +119,16 @@
     runner.infer_host = args.infer_host
     runner.redis_addr = args.redis_addr
     runner.redis_port = args.redis_port
     runner.redis_password = args.redis_password
     init_logs(edge_id)
 
     # Log arguments and binding results.
-    logging.info("login: unique_device_id = %s" % str(unique_device_id))
-    logging.info("login: server_id = %s" % str(edge_id))
+    # logging.info("login: unique_device_id = %s" % str(unique_device_id))
+    # logging.info("login: server_id = %s" % str(edge_id))
     runner.unique_device_id = unique_device_id
     ServerConstants.save_runner_infos(args.current_device_id + "." + args.os_name, edge_id)
 
     # Setup MQTT connection for communication with the FedML server.
     runner.setup_agent_mqtt_connection(service_config)
 
     # Start mqtt looper
@@ -307,14 +307,15 @@
             continue
 
     if edge_id <= 0:
         click.echo("")
         click.echo("Oops, you failed to login the FedML ModelOps platform.")
         click.echo("Please check whether your network is normal!")
         return
+
     setattr(args, "server_id", edge_id)
     runner.args = args
     runner.edge_id = edge_id
     runner.infer_host = args.infer_host
     runner.redis_addr = args.redis_addr
     runner.redis_port = args.redis_port
     runner.redis_password = args.redis_password
@@ -322,30 +323,34 @@
 
     # Log arguments and binding results.
     logging.info("login: unique_device_id = %s" % str(unique_device_id))
     logging.info("login: server_id = %s" % str(edge_id))
     ServerConstants.save_runner_infos(args.current_device_id + "." + args.os_name, edge_id)
 
     # Echo results
-    logging.info("Congratulations, you have logged into the FedML ModelOps platform successfully!")
-    logging.info("Your server unique device id is " + str(unique_device_id))
-
+    print("\n\nCongratulations, your device is connected to the FedML MLOps platform successfully!")
+    print(
+        "Your unique device ID is "
+        + str(unique_device_id)
+        + "\n"
+    )
+        
     # Start the FedML server
     runner.callback_start_train(payload=args.runner_cmd)
 
 
 def init_logs(edge_id):
     # Init runtime logs
     args.log_file_dir = ServerConstants.get_log_file_dir()
     args.run_id = 0
-    args.rank = 0
+    args.role = "server"
     args.edge_id = edge_id
     setattr(args, "using_mlops", True)
     setattr(args, "server_agent_id", edge_id)
-    MLOpsRuntimeLog.get_instance(args).init_logs(show_stdout_log=True)
+    # MLOpsRuntimeLog.get_instance(args).init_logs(show_stdout_log=True)
 
 
 def login(args):
     # Install redis server
     if not hasattr(args, "redis_addr") or args.redis_addr is None or args.redis_addr == "local":
         sys_name = platform.system()
         if sys_name == "Linux":
@@ -361,15 +366,15 @@
     elif args.role == ServerConstants.login_role_list[ServerConstants.LOGIN_MODE_PUBLIC_CLOUD_MASTER_INDEX]:
         __login_as_cloud_agent(args, args.user, args.version)
     elif args.role == ServerConstants.login_role_list[ServerConstants.LOGIN_MODE_INFERENCE_INSTANCE_INDEX]:
         __login_as_cloud_server(args, args.user, args.version)
 
 
 def logout():
-    ServerConstants.cleanup_run_process()
+    ServerConstants.cleanup_run_process(None)
 
 
 if __name__ == "__main__":
     os.environ['PYTHONWARNINGS'] = 'ignore:semaphore_tracker:UserWarning'
     os.environ.setdefault('PYTHONWARNINGS', 'ignore:semaphore_tracker:UserWarning')
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument("--type", "-t", help="Login or logout to ModelOps platform")
```

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_model_cache.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_model_cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import json
 import redis
-from random import shuffle
 from fedml.cli.model_deployment.device_server_constants import ServerConstants
-from fedml.cli.model_deployment.device_server_data_interface import FedMLServerDataInterface
 from .device_model_db import FedMLModelDatabase
 
 
 class FedMLModelCache(object):
     FEDML_MODEL_DEPLOYMENT_RESULT_TAG = "FEDML_MODEL_DEPLOYMENT_RESULT-"
     FEDML_MODEL_DEPLOYMENT_STATUS_TAG = "FEDML_MODEL_DEPLOYMENT_STATUS-"
     FEDML_MODEL_DEPLOYMENT_MONITOR_TAG = "FEDML_MODEL_DEPLOYMENT_MONITOR-"
     FEDML_MODEL_END_POINT_ACTIVATION_TAG = "FEDML_MODEL_END_POINT_ACTIVATION-"
     FEDML_MODEL_END_POINT_STATUS_TAG = "FEDML_MODEL_END_POINT_STATUS-"
     FEDML_MODEL_DEVICE_INFO_TAG = "FEDML_MODEL_DEVICE_INFO_TAG-"
     FEDML_MODEL_END_POINT_TOKEN_TAG = "FEDML_MODEL_END_POINT_TOKEN_TAG-"
+    FEDML_MODEL_ROUND_ROBIN_PREVIOUS_DEVICE_TAG = "FEDML_MODEL_ROUND_ROBIN_PREVIOUS_DEVICE_TAG-"
     FEDML_KEY_COUNT_PER_SCAN = 1000
 
     def __init__(self):
         pass
 
     def __new__(cls, *args, **kw):
         if not hasattr(cls, "_instance"):
@@ -105,60 +104,83 @@
         result_payload = json.loads(result_item_json["result"])
         return device_id, result_payload
 
     def get_idle_device(self, end_point_name,
                         model_name, model_version,
                         check_end_point_status=True):
         # Find all deployed devices
-        status_list = self.get_deployment_status_list(end_point_name, model_name)
+        status_list = self.get_deployment_status_list(end_point_name, model_name)   # get from redis
         if len(status_list) == 0:
             return None, None
 
         idle_device_list = list()
         if model_version == "latest":
-            device_id, status_payload = self.get_status_item_info(status_list[-1])
-            model_status = status_payload["model_status"]
-            end_point_id_cache = status_payload["end_point_id"]
-            if model_status != ServerConstants.MSG_MODELOPS_DEPLOYMENT_STATUS_DEPLOYED:
-                return None, None
-            idle_device_list.append({"device_id": device_id, "end_point_id": end_point_id_cache})
-        else:
+            _, status_payload = self.get_status_item_info(status_list[-1])
+            model_version = status_payload["model_version"]
+
+        # find all devices
+        try:
             for status_item in status_list:
                 device_id, status_payload = self.get_status_item_info(status_item)
                 print(f"status_payload {status_payload}")
                 model_status = status_payload["model_status"]
                 model_version_cache = status_payload["model_version"]
                 end_point_id_cache = status_payload["end_point_id"]
                 print(f"model_version {model_version}, model_version_cache {model_version_cache}")
                 if model_version == model_version_cache and \
                         model_status == ServerConstants.MSG_MODELOPS_DEPLOYMENT_STATUS_DEPLOYED:
                     idle_device_list.append({"device_id": device_id, "end_point_id": end_point_id_cache})
-
+        except Exception as e:
+            print("Get idel device list Failed:")
+            print(e)
         print(f"idle device list {idle_device_list}")
-        # Randomly shuffle the list of deployed devices and get the first one as the target idle device.
-        if len(idle_device_list) <= 0:
-            return None, None
-        shuffle(idle_device_list)
-        idle_device_dict = idle_device_list[0]
+        # Randomly shuffle 
+        # shuffle the list of deployed devices and get the first one as the target idle device.
+        # if len(idle_device_list) <= 0:
+        #     return None, None
+        # shuffle(idle_device_list)
+        # idle_device_dict = idle_device_list[0]
+
+        # Round Robin
+        total_device_num = len(idle_device_list)
+        redis_round_robin_key = self.get_round_robin_prev_device(end_point_name, model_name, model_version)
+
+        try:
+            if self.redis_connection.exists(redis_round_robin_key):
+                selected_device_index = int(self.redis_connection.get(redis_round_robin_key))
+                selected_device_index %= total_device_num
+            else:
+                selected_device_index = 0
+            next_selected_device_index = (selected_device_index + 1) % total_device_num
+            self.redis_connection.set(redis_round_robin_key, str(next_selected_device_index))
+        except Exception as e:
+            print("Inference Device selection Failed:")
+            print(str(e))
 
+        print(f"Using Round Robin, the device index is {selected_device_index}")
+        idle_device_dict = idle_device_list[selected_device_index]
         # Find deployment result from the target idle device.
-        result_list = self.get_deployment_result_list(end_point_name, model_name)
-        for result_item in result_list:
-            device_id, result_payload = self.get_result_item_info(result_item)
-            found_end_point_id = result_payload["end_point_id"]
-            found_end_point_name = result_payload["end_point_name"]
-            # Check whether the end point is activated.
-            if check_end_point_status:
-                end_point_activated = self.get_end_point_activation(found_end_point_id)
-                if not end_point_activated:
-                    continue
-
-            if found_end_point_id == idle_device_dict["end_point_id"] \
-                    and device_id == idle_device_dict["device_id"]:
-                return result_payload, device_id
+        try:
+            result_list = self.get_deployment_result_list(end_point_name, model_name)
+            for result_item in result_list:
+                device_id, result_payload = self.get_result_item_info(result_item)
+                found_end_point_id = result_payload["end_point_id"]
+                found_end_point_name = result_payload["end_point_name"]
+                # Check whether the end point is activated.
+                if check_end_point_status:
+                    end_point_activated = self.get_end_point_activation(found_end_point_id)
+                    if not end_point_activated:
+                        continue
+
+                if found_end_point_id == idle_device_dict["end_point_id"] \
+                        and device_id == idle_device_dict["device_id"]:
+                    print(f"The chosen device is {device_id}")
+                    return result_payload, device_id
+        except Exception as e:
+            print(e)
 
         return None, None
 
     def set_end_point_status(self, end_point_id, end_point_name, status):
         self.redis_connection.set(self.get_end_point_status_key(end_point_id), status)
         self.model_deployment_db.set_end_point_status(end_point_id, end_point_name, status)
 
@@ -172,14 +194,18 @@
         status = self.redis_connection.get(self.get_end_point_status_key(end_point_id))
         return status
 
     def set_end_point_activation(self, end_point_id, end_point_name, activate_status):
         status = 1 if activate_status else 0
         self.redis_connection.set(self.get_end_point_activation_key(end_point_id), status)
         self.model_deployment_db.set_end_point_activation(end_point_id, end_point_name, status)
+        
+    def delete_end_point(self, end_point_name, model_name, model_version):
+        self.redis_connection.delete(self.get_deployment_status_key(end_point_name, model_name))
+        # TODO: Delete related KV Pair        
 
     def get_end_point_activation(self, end_point_id):
         if not self.redis_connection.exists(self.get_end_point_activation_key(end_point_id)):
             activated = self.model_deployment_db.get_end_point_activation(end_point_id)
             self.redis_connection.set(self.get_end_point_activation_key(end_point_id), activated)
             status = True if int(activated) == 1 else False
             return status
@@ -232,29 +258,32 @@
 
     def get_deployment_device_info_key(self, end_point_id):
         return "{}{}".format(FedMLModelCache.FEDML_MODEL_DEVICE_INFO_TAG, end_point_id)
 
     def get_deployment_token_key(self, end_point_name, model_name):
         return "{}{}-{}".format(FedMLModelCache.FEDML_MODEL_END_POINT_TOKEN_TAG, end_point_name, model_name)
 
+    def get_round_robin_prev_device(self, end_point_name, model_name, version):
+        return "{}{}-{}-{}".format(FedMLModelCache.FEDML_MODEL_ROUND_ROBIN_PREVIOUS_DEVICE_TAG, end_point_name, model_name, version)
+
     def set_monitor_metrics(self, end_point_id, end_point_name,
                             model_name, model_version,
                             total_latency, avg_latency,
                             total_request_num, current_qps,
-                            avg_qps, timestamp):
+                            avg_qps, timestamp, device_id):
         metrics_dict = {"total_latency": total_latency, "avg_latency": avg_latency,
                         "total_request_num": total_request_num, "current_qps": current_qps,
-                        "avg_qps": avg_qps, "timestamp": timestamp}
+                        "avg_qps": avg_qps, "timestamp": timestamp, "device_id": device_id}
         self.redis_connection.rpush(self.get_monitor_metrics_key(end_point_name, model_name, model_version),
                                     json.dumps(metrics_dict))
         self.model_deployment_db.set_monitor_metrics(end_point_id, end_point_name,
                                                      model_name, model_version,
                                                      total_latency, avg_latency,
                                                      total_request_num, current_qps,
-                                                     avg_qps, timestamp)
+                                                     avg_qps, timestamp, device_id)
 
     def get_latest_monitor_metrics(self, end_point_name, model_name, model_version):
         if not self.redis_connection.exists(self.get_monitor_metrics_key(end_point_name, model_name, model_version)):
             metrics_dict = self.model_deployment_db.get_latest_monitor_metrics(end_point_name, model_name, model_version)
             if metrics_dict is not None:
                 self.redis_connection.rpush(self.get_monitor_metrics_key(end_point_name, model_name, model_version),
                                             metrics_dict)
@@ -279,15 +308,16 @@
         metrics_item_json = json.loads(metrics_item)
         total_latency = metrics_item_json["total_latency"]
         avg_latency = metrics_item_json["avg_latency"]
         total_request_num = metrics_item_json["total_request_num"]
         current_qps = metrics_item_json["current_qps"]
         avg_qps = metrics_item_json["avg_qps"]
         timestamp = metrics_item_json["timestamp"]
-        return total_latency, avg_latency, total_request_num, current_qps, avg_qps, timestamp
+        device_id = metrics_item_json["device_id"]
+        return total_latency, avg_latency, total_request_num, current_qps, avg_qps, timestamp, device_id
 
     def get_monitor_metrics_key(self, end_point_name, model_name, model_version):
         return "{}{}-{}-{}".format(FedMLModelCache.FEDML_MODEL_DEPLOYMENT_MONITOR_TAG,
                                    end_point_name, model_name, model_version)
 
 
 if __name__ == "__main__":
```

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_model_deployment.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_model_deployment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import io
 import logging
 import os
 import pickle
 import platform
 import shutil
 import time
 import traceback
@@ -14,14 +13,23 @@
 
 import collections.abc
 
 for type_name in collections.abc.__all__:
     setattr(collections, type_name, getattr(collections.abc, type_name))
 
 from fedml.cli.model_deployment.device_client_constants import ClientConstants
+import io
+
+
+class CPUUnpickler(pickle.Unpickler):
+    def find_class(self, module, name):
+        if module == 'torch.storage' and name == '_load_from_bytes':
+            return lambda b: torch.load(io.BytesIO(b), map_location='cpu')
+        else:
+            return super().find_class(module, name)
 
 
 def start_deployment(end_point_id, end_point_name, model_id, model_version,
                      model_storage_local_path, model_bin_file, inference_model_name, inference_engine,
                      inference_http_port, inference_grpc_port, inference_metric_port,
                      inference_use_gpu, inference_memory_size,
                      inference_convertor_image, inference_server_image,
@@ -52,16 +60,17 @@
                 "name": "output",
                 "data_type": "TYPE_FP32",
                 "dims": []
             }
         ]
     }
 
-    gpu_attach_cmd = ""
-    if inference_use_gpu is not None and inference_use_gpu != "":
+    if not torch.cuda.is_available():
+        gpu_attach_cmd = ""
+    else:
         gpu_attach_cmd = "--gpus all"
 
     logging.info("Update docker environments...")
 
     sudo_prefix = "sudo "
     sys_name = platform.system()
     if sys_name == "Darwin":
@@ -97,99 +106,106 @@
                   && curl -s -L https://nvidia.github.io/libnvidia-container/experimental/$distribution/libnvidia-container.list | \
                      sed 's#deb https://#deb [signed-by=/usr/share/keyrings/nvidia-container-toolkit-keyring.gpg] https://#g' | \
                      sudo tee /etc/apt/sources.list.d/nvidia-container-toolkit.list")
                     os.system(sudo_prefix + "apt-get update")
                     os.system(sudo_prefix + "apt-get install -y nvidia-docker2")
                     os.system(sudo_prefix + "systemctl restart docker")
 
+    test_llm = False
     # Convert models from pytorch to onnx format
     if model_is_from_open:
-        logging.info("convert the onnx model when the mode is from the MLOps platform...")
-
-        logging.info("Input size {}, input types {}".format(model_params["input_size"],
-                                                            model_params["input_types"]))
-
         running_model_name = ClientConstants.get_running_model_name(end_point_name,
                                                                     inference_model_name,
                                                                     model_version, end_point_id, model_id)
         if model_from_open is None:
             return running_model_name, "", model_version, {}, {}
 
+        logging.info("model binary file: {}".format(model_bin_file))
         with open(model_bin_file, 'rb') as model_pkl_file:
             if not torch.cuda.is_available():
                 try:
-                    open_model_params = pickle.load(model_pkl_file)
-                except Exception as e:
-                    logging.info("load model exceptions, try to use torch.load(f,map_location=torch.device('cpu')), "
-                                 "details: {}".format(traceback.format_exc()))
-                    try:
-                        open_model_params = torch.load(model_pkl_file, map_location=torch.device('cpu'))
-                    except Exception as ex:
-                        logging.info("load model exceptions when using torch.load: {}".format(traceback.format_exc()))
-                        return "", "", model_version, model_metadata, model_config
+                    open_model_params = CPUUnpickler(model_pkl_file).load()
+                except Exception as ex:
+                    logging.info("load model exceptions when using CPU_Unpickler: {}".format(traceback.format_exc()))
+                    return "", "", model_version, model_metadata, model_config
             else:
                 open_model_params = pickle.load(model_pkl_file)
             model_from_open.load_state_dict(open_model_params)
             model_from_open.eval()
 
-        input_size = model_params["input_size"]
-        input_types = model_params["input_types"]
-
-        dummy_input_list = []
-        for index, input_i in enumerate(input_size):
-            if input_types[index] == "int":
-                this_input = torch.randint(0, 1, input_i).clone().detach()
-            else:
-                this_input = torch.zeros(input_i).clone().detach()
-            dummy_input_list.append(this_input)
-
-        onnx_model_path = os.path.join(model_storage_local_path,
-                                       ClientConstants.FEDML_CONVERTED_MODEL_DIR_NAME,
-                                       running_model_name, ClientConstants.INFERENCE_MODEL_VERSION)
-        if not os.path.exists(onnx_model_path):
-            os.makedirs(onnx_model_path)
-        onnx_model_path = os.path.join(onnx_model_path, "model.onnx")
-
-        convert_model_to_onnx(model_from_open, onnx_model_path, dummy_input_list, input_size)
+        if not test_llm:
+            logging.info("convert the onnx model when the mode is from the MLOps platform...")
+            logging.info("Input size {}, input types {}".format(model_params["input_size"],
+                                                                model_params["input_types"]))
+            input_size = model_params["input_size"]
+            input_types = model_params["input_types"]
+
+            dummy_input_list = []
+            for index, input_i in enumerate(input_size):
+                if input_types[index] == "int":
+                    this_input = torch.randint(0, 1, input_i).clone().detach()
+                else:
+                    this_input = torch.zeros(input_i).clone().detach()
+                dummy_input_list.append(this_input)
+
+            onnx_model_path = os.path.join(model_storage_local_path,
+                                           ClientConstants.FEDML_CONVERTED_MODEL_DIR_NAME,
+                                           running_model_name, ClientConstants.INFERENCE_MODEL_VERSION)
+            if not os.path.exists(onnx_model_path):
+                os.makedirs(onnx_model_path)
+            onnx_model_path = os.path.join(onnx_model_path, "model.onnx")
+
+            convert_model_to_onnx(model_from_open, onnx_model_path, dummy_input_list, input_size)
+        else:  # we do not convert the model to onnx in llm
+            logging.info("LLM model loaded from the open")
     else:
-        logging.info("convert the onnx model when the mode is from the general PyTorch...")
-        logging.info("Input size {}, input types {}".format(model_params["input_size"],
-                                                            model_params["input_types"]))
-
+        # not from open
         running_model_name = ClientConstants.get_running_model_name(end_point_name,
                                                                     inference_model_name,
                                                                     model_version, end_point_id, model_id)
-        # configuration passed by user in the Cli
         model_location = os.path.join(model_storage_local_path, "fedml_model.bin")
-        input_size = model_params["input_size"]
-        input_types = model_params["input_types"]
-
-        model = torch.jit.load(model_location)  # model def + params
         try:
+            model = torch.jit.load(model_location)  # model def + params
             model.eval()
         except Exception as e:
-            pass
+            logging.info(
+                "Cannot locate the .bin file, will read it from the fedml_model_cofig.yaml with the key [local_model_dir] ")
+            import yaml
+            local_model_location = os.path.join(model_storage_local_path, "fedml_model_config.yaml")
+
+            with open(local_model_location, 'r') as file:
+                config = yaml.safe_load(file)
+                local_model_dir = config.get('local_model_dir')
+
+            local_model_dir_from_config = local_model_dir
+
+        if not test_llm:
+            # configuration passed by user in the Cli
+            input_size = model_params["input_size"]
+            input_types = model_params["input_types"]
+            logging.info("convert the onnx model when the mode is from the general PyTorch...")
+            logging.info("Input size {}, input types {}".format(model_params["input_size"],
+                                                                model_params["input_types"]))
+            dummy_input_list = []
+            for index, input_i in enumerate(input_size):
+                if input_types[index] == "int":
+                    this_input = torch.randint(0, 1, input_i).clone().detach()
+                else:
+                    this_input = torch.zeros(input_i).clone().detach()
+                dummy_input_list.append(this_input)
+
+            onnx_model_path = os.path.join(model_storage_local_path,
+                                           ClientConstants.FEDML_CONVERTED_MODEL_DIR_NAME,
+                                           running_model_name, ClientConstants.INFERENCE_MODEL_VERSION)
+            logging.info("converted onnx model path: {}".format(onnx_model_path))
+            if not os.path.exists(onnx_model_path):
+                os.makedirs(onnx_model_path)
+            onnx_model_path = os.path.join(onnx_model_path, "model.onnx")
 
-        dummy_input_list = []
-        for index, input_i in enumerate(input_size):
-            if input_types[index] == "int":
-                this_input = torch.randint(0, 1, input_i).clone().detach()
-            else:
-                this_input = torch.zeros(input_i).clone().detach()
-            dummy_input_list.append(this_input)
-
-        onnx_model_path = os.path.join(model_storage_local_path,
-                                       ClientConstants.FEDML_CONVERTED_MODEL_DIR_NAME,
-                                       running_model_name, ClientConstants.INFERENCE_MODEL_VERSION)
-        logging.info("converted onnx model path: {}".format(onnx_model_path))
-        if not os.path.exists(onnx_model_path):
-            os.makedirs(onnx_model_path)
-        onnx_model_path = os.path.join(onnx_model_path, "model.onnx")
-
-        convert_model_to_onnx(model, onnx_model_path, dummy_input_list, input_size)
+            convert_model_to_onnx(model, onnx_model_path, dummy_input_list, input_size)
 
         # convert_model_container_name = "{}_{}_{}".format(ClientConstants.FEDML_CONVERT_MODEL_CONTAINER_NAME_PREFIX,
         #                                                  str(end_point_id),
         #                                                  str(model_id))
         # running_model_name = ClientConstants.get_running_model_name(end_point_name,
         #                                                             inference_model_name,
         #                                                             model_version, end_point_id, model_id)
@@ -228,64 +244,109 @@
                 if not os.path.exists(dst_model_file):
                     shutil.copytree(src_model_file, dst_model_file, copy_function=shutil.copy,
                                     ignore_dangling_symlinks=True)
             else:
                 if not os.path.exists(dst_model_file):
                     shutil.copyfile(src_model_file, dst_model_file)
 
-    # Run triton server
-    logging.info("prepare to run triton server...")
-    if not use_simulation_test_without_triton:
-        if not triton_server_is_running and not ClientConstants.is_running_on_k8s():
-            triton_server_cmd = "{}docker stop {}; {}docker rm {}; {}docker run --name {} {} -p{}:8000 " \
-                                "-p{}:8001 -p{}:8002 " \
-                                "--shm-size {} " \
-                                "-v {}:/models {} " \
-                                "bash -c \"pip install transformers && tritonserver --strict-model-config=false " \
-                                "--model-control-mode=poll --repository-poll-secs={} " \
-                                "--model-repository=/models\" ".format(sudo_prefix, triton_server_container_name,
-                                                                       sudo_prefix, triton_server_container_name,
-                                                                       sudo_prefix, triton_server_container_name,
-                                                                       gpu_attach_cmd,
-                                                                       inference_http_port,
-                                                                       inference_grpc_port,
-                                                                       inference_metric_port,
-                                                                       inference_memory_size,
-                                                                       model_serving_dir,
-                                                                       inference_server_image,
-                                                                       ClientConstants.FEDML_MODEL_SERVING_REPO_SCAN_INTERVAL)
-            logging.info("Run triton inference server: {}".format(triton_server_cmd))
-            triton_server_process = ClientConstants.exec_console_with_script(triton_server_cmd,
-                                                                             should_capture_stdout=False,
-                                                                             should_capture_stderr=False,
-                                                                             no_sys_out_err=True)
-            log_deployment_result(end_point_id, model_id, triton_server_container_name,
-                                  ClientConstants.CMD_TYPE_RUN_TRITON_SERVER, triton_server_process.pid,
-                                  running_model_name, inference_engine, inference_http_port)
-
+    if test_llm:
+        logging.info(f"local_model_dir: {local_model_dir_from_config}")
+        inference_server_image = "myimage"  # TODO:download from dockerhub
+        inference_http_port = 2345
+        local_model_dir = local_model_dir_from_config
+        llm_server_container_name = "{}".format(ClientConstants.FEDML_LLM_SERVER_CONTAINER_NAME_PREFIX)
+        volume_dst_loc = "code/model_and_config"
+        llm_server_cmd = "{}docker stop {}; {}docker rm {}; {}docker run --gpus all --name {} -p{}:2345 " \
+                         "-v {}:/{} {}".format(sudo_prefix, llm_server_container_name,
+                                               sudo_prefix, llm_server_container_name,
+                                               sudo_prefix, llm_server_container_name,
+                                               inference_http_port,
+                                               local_model_dir,
+                                               volume_dst_loc,
+                                               inference_server_image)
+        logging.info("Run llm inference server: {}".format(llm_server_cmd))
+        llm_server = ClientConstants.exec_console_with_script(llm_server_cmd,
+                                                              should_capture_stdout=False,
+                                                              should_capture_stderr=False,
+                                                              no_sys_out_err=True)
+        # report the status
+        log_deployment_result(end_point_id, model_id, llm_server_container_name,
+                              ClientConstants.CMD_TYPE_RUN_TRITON_SERVER, llm_server.pid,
+                              running_model_name, inference_engine, inference_http_port, inference_type="llm")
         inference_output_url, running_model_version, ret_model_metadata, ret_model_config = \
-            get_model_info(running_model_name, inference_engine, inference_http_port, infer_host)
+            get_model_info(running_model_name, inference_engine, inference_http_port, infer_host, inference_type="llm")
+
+        # testing
+        test_input = {"inputs": {"text": "What is a good cure for hiccups?"}}
         if inference_output_url != "":
-            # Send the test request to the inference backend and check if the response is normal
-            input_json, output_json = build_inference_req(end_point_name, inference_model_name,
-                                                          token, ret_model_metadata)
             try:
-                inference_response = run_http_inference_with_curl_request(inference_output_url, input_json["inputs"], input_json["outputs"])
+                inference_response = run_http_inference_with_curl_request(inference_output_url, test_input, [],
+                                                                          inference_type="llm")
                 logging.info("Tested the inference backend, the response is {}".format(inference_response))
             except Exception as e:
                 logging.info("Tested the inference backend, exceptions occurred: {}".format(traceback.format_exc()))
                 inference_output_url = ""
+        model_metadata = ret_model_metadata
 
-            if inference_output_url != "":
-                logging.info("Deploy model successfully, inference url: {}, model metadata: {}, model config: {}".format(
-                    inference_output_url, model_metadata, model_config))
-                model_metadata = ret_model_metadata
-                model_config = ret_model_config
+        # metadata to report
+        logging.info(model_metadata)
     else:
-        inference_output_url = f"http://localhost:{inference_http_port}/v2/models/{running_model_name}/versions/1/infer"
+        # Run triton server
+        logging.info("prepare to run triton server...")
+        if not use_simulation_test_without_triton:
+            if not triton_server_is_running and not ClientConstants.is_running_on_k8s():
+                triton_server_cmd = "{}docker stop {}; {}docker rm {}; {}docker run --name {} {} -p{}:8000 " \
+                                    "-p{}:8001 -p{}:8002 " \
+                                    "--shm-size {} " \
+                                    "-v {}:/models {} " \
+                                    "bash -c \"pip install transformers && tritonserver --strict-model-config=false " \
+                                    "--model-control-mode=poll --repository-poll-secs={} " \
+                                    "--model-repository=/models\" ".format(sudo_prefix, triton_server_container_name,
+                                                                           sudo_prefix, triton_server_container_name,
+                                                                           sudo_prefix, triton_server_container_name,
+                                                                           gpu_attach_cmd,
+                                                                           inference_http_port,
+                                                                           inference_grpc_port,
+                                                                           inference_metric_port,
+                                                                           inference_memory_size,
+                                                                           model_serving_dir,
+                                                                           inference_server_image,
+                                                                           ClientConstants.FEDML_MODEL_SERVING_REPO_SCAN_INTERVAL)
+                logging.info("Run triton inference server: {}".format(triton_server_cmd))
+                triton_server_process = ClientConstants.exec_console_with_script(triton_server_cmd,
+                                                                                 should_capture_stdout=False,
+                                                                                 should_capture_stderr=False,
+                                                                                 no_sys_out_err=True)
+                log_deployment_result(end_point_id, model_id, triton_server_container_name,
+                                      ClientConstants.CMD_TYPE_RUN_TRITON_SERVER, triton_server_process.pid,
+                                      running_model_name, inference_engine, inference_http_port)
+
+            inference_output_url, running_model_version, ret_model_metadata, ret_model_config = \
+                get_model_info(running_model_name, inference_engine, inference_http_port, infer_host)
+            if inference_output_url != "":
+                # Send the test request to the inference backend and check if the response is normal
+                input_json, output_json = build_inference_req(end_point_name, inference_model_name,
+                                                              token, ret_model_metadata)
+                try:
+                    inference_response = run_http_inference_with_curl_request(inference_output_url,
+                                                                              input_json["inputs"],
+                                                                              input_json["outputs"])
+                    logging.info("Tested the inference backend, the response is {}".format(inference_response))
+                except Exception as e:
+                    logging.info("Tested the inference backend, exceptions occurred: {}".format(traceback.format_exc()))
+                    inference_output_url = ""
+
+                if inference_output_url != "":
+                    logging.info(
+                        "Deploy model successfully, inference url: {}, model metadata: {}, model config: {}".format(
+                            inference_output_url, model_metadata, model_config))
+                    model_metadata = ret_model_metadata
+                    model_config = ret_model_config
+        else:
+            inference_output_url = f"http://localhost:{inference_http_port}/v2/models/{running_model_name}/versions/1/infer"
 
     return running_model_name, inference_output_url, model_version, model_metadata, model_config
 
 
 def build_inference_req(end_point_name, model_name, token, in_model_metadata):
     model_inputs = in_model_metadata["inputs"]
     ret_inputs = list()
@@ -312,15 +373,16 @@
                   "inputs": ret_inputs,
                   "outputs": in_model_metadata["outputs"]}
     output_json = in_model_metadata["outputs"]
 
     return input_json, output_json
 
 
-def should_exit_logs(end_point_id, model_id, cmd_type, cmd_process_id, model_name, inference_engine, inference_port):
+def should_exit_logs(end_point_id, model_id, cmd_type, cmd_process_id, model_name, inference_engine, inference_port,
+                     inference_type=None):
     sudo_prefix = "sudo "
     sys_name = platform.system()
     if sys_name == "Darwin":
         sudo_prefix = ""
 
     if cmd_type == ClientConstants.CMD_TYPE_CONVERT_MODEL:
         convert_model_container_name = "{}_{}_{}".format(ClientConstants.FEDML_CONVERT_MODEL_CONTAINER_NAME_PREFIX,
@@ -338,28 +400,28 @@
             else:
                 return False
         else:
             return True
     elif cmd_type == ClientConstants.CMD_TYPE_RUN_TRITON_SERVER:
         try:
             inference_output_url, model_version, model_metadata, model_config = \
-                get_model_info(model_name, inference_engine, inference_port)
+                get_model_info(model_name, inference_engine, inference_port, inference_type=inference_type)
             logging.info("Log test for deploying model successfully, inference url: {}, "
                          "model metadata: {}, model config: {}".
                          format(inference_output_url, model_metadata, model_config))
             if inference_output_url != "":
                 return True
         except Exception as e:
             pass
         return False
 
 
 def log_deployment_result(end_point_id, model_id, cmd_container_name, cmd_type,
                           cmd_process_id, inference_model_name, inference_engine,
-                          inference_http_port):
+                          inference_http_port, inference_type=None):
     sudo_prefix = "sudo "
     sys_name = platform.system()
     if sys_name == "Darwin":
         sudo_prefix = ""
 
     last_out_logs = ""
     last_err_logs = ""
@@ -386,24 +448,48 @@
 
         time.sleep(3)
         deployment_count += 1
         if deployment_count >= 5:
             break
 
         if should_exit_logs(end_point_id, model_id, cmd_type, cmd_process_id,
-                            inference_model_name, inference_engine, inference_http_port):
+                            inference_model_name, inference_engine, inference_http_port, inference_type):
             break
 
 
-def get_model_info(model_name, inference_engine, inference_http_port, infer_host=None, is_hg_model=False):
+def get_model_info(model_name, inference_engine, inference_http_port, infer_host=None, is_hg_model=False,
+                   inference_type=None):
     local_ip = ClientConstants.get_local_ip()
     if infer_host is not None and infer_host != "127.0.0.1":
         infer_url_host = infer_host
     else:
         infer_url_host = local_ip
+    logging.info(f"The infer_url_host is {infer_url_host}")
+    if inference_type == "llm":
+        llm_server_test_ready_url = "http://{}:{}/ready".format(infer_url_host, inference_http_port)
+        wait_count = 0
+        while True:
+            response = None
+            try:
+                response = requests.get(llm_server_test_ready_url)
+            except:
+                pass
+            if not response or response.status_code != 200:
+                logging.info(f"model {model_name} not yet ready")
+                time.sleep(10)
+                wait_count += 1
+                if wait_count >= 15:
+                    return "", model_version, {}, {}
+            else:
+                break
+        model_metadata = {}
+        model_metadata["inputs"] = {"text": "What is a good cure for hiccups?"}
+        model_metadata["outputs"] = []
+        model_metadata["type"] = "llm"
+        return "http://{}:{}/predict".format(infer_url_host, inference_http_port), None, model_metadata, None
     local_infer_url = "{}:{}".format(infer_url_host, inference_http_port)
     model_version = ""
     logging.info("triton infer url: {}.".format(local_infer_url))
     if is_hg_model:
         inference_model_name = "{}_{}_inference".format(model_name, inference_engine)
     else:
         inference_model_name = model_name
@@ -434,25 +520,34 @@
                                                                                 ClientConstants.INFERENCE_INFERENCE_SERVER_VERSION,
                                                                                 inference_model_name,
                                                                                 model_version)
 
     return inference_output_url, model_version, model_metadata, model_config
 
 
-def run_http_inference_with_curl_request(inference_url, inference_input_list, inference_output_list):
+def run_http_inference_with_curl_request(inference_url, inference_input_list, inference_output_list,
+                                         inference_type=None):
     model_inference_result = {}
     model_api_headers = {'Content-Type': 'application/json', 'Connection': 'close'}
-    model_inference_json = {
-        "inputs": inference_input_list,
-        "outputs": inference_output_list
-    }
-
-    response = requests.post(inference_url, headers=model_api_headers, json=model_inference_json)
-    if response.status_code == 200:
-        model_inference_result = response.json()
+    print("inference_url: {}".format(inference_url))
+    print("inference_input_list: {}".format(inference_input_list))
+    if inference_output_list == []:
+        model_inference_json = inference_input_list
+    else:  # triton
+        model_inference_json = {
+            "inputs": inference_input_list,
+            "outputs": inference_output_list
+        }
+
+    try:
+        response = requests.post(inference_url, headers=model_api_headers, json=model_inference_json)
+        if response.status_code == 200:
+            model_inference_result = response.json()
+    except Exception as e:
+        print("Error in running inference: {}".format(e))
 
     return model_inference_result
 
 
 def convert_model_to_onnx(
         torch_model, output_path: str, dummy_input_list, input_size: int, input_is_tensor=True
 ) -> None:
@@ -539,15 +634,48 @@
                           input_is_tensor=True)
 
     model_serving_dir = os.path.join(ClientConstants.get_model_cache_dir(),
                                      ClientConstants.FEDML_CONVERTED_MODEL_DIR_NAME)
     return model_serving_dir
 
 
+def start_gpu_model_load_process():
+    from multiprocessing import Process
+    import time
+    process = Process(target=load_gpu_model_to_cpu_device)
+    process.start()
+    while True:
+        time.sleep(1)
+
+
+def load_gpu_model_to_cpu_device():
+    import pickle
+    import io
+    import torch
+
+    class CPU_Unpickler(pickle.Unpickler):
+        def find_class(self, module, name):
+            if module == 'torch.storage' and name == '_load_from_bytes':
+                return lambda b: torch.load(io.BytesIO(b), map_location='cpu')
+            else:
+                return super().find_class(module, name)
+
+    model_file = "/home/fedml/fedml-client/fedml/models/theta_rec_auc_81_single_label/theta_rec_auc_81_single_label"
+    with open(model_file, "rb") as model_pkl_file:
+        if not torch.cuda.is_available():
+            model = CPU_Unpickler(model_pkl_file).load()
+            if model is None:
+                print("Failed to load gpu model to cpu device")
+            else:
+                print("Succeeded to load gpu model to cpu device")
+
+
 if __name__ == "__main__":
+    start_gpu_model_load_process()
+
     model_serving_dir = test_convert_pytorch_model_to_onnx("./sample-open-training-model-net",
                                                            "./sample-open-training-model",
                                                            "rec-model",
                                                            {"input_size": [[1, 24], [1, 2]],
                                                             "input_types": ["int", "float"]})
 
     test_start_triton_server(model_serving_dir)
```

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_server_data_interface.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_server_data_interface.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_model_object.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_model_object.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_model_db.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_model_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-import logging
 import os
 import time
 
 from fedml.cli.model_deployment.device_server_constants import ServerConstants
 from sqlalchemy import Column, String, TEXT, Integer, Float, create_engine, and_
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.ext.declarative import declarative_base
@@ -96,39 +95,41 @@
             return auth_info.token
         return None
 
     def set_monitor_metrics(self, end_point_id, end_point_name,
                             model_name, model_version,
                             total_latency, avg_latency,
                             total_request_num, current_qps,
-                            avg_qps, timestamp):
+                            avg_qps, timestamp, device_id):
         self.set_end_point_metrics(end_point_id, end_point_name,
                                    model_name, model_version,
                                    total_latency=total_latency, avg_latency=avg_latency,
                                    total_request_num=total_request_num, current_qps=current_qps,
-                                   avg_qps=avg_qps, timestamp=timestamp)
+                                   avg_qps=avg_qps, timestamp=timestamp, device_id=device_id)
 
     def get_latest_monitor_metrics(self, end_point_name, model_name, model_version):
         endpoint_metrics = self.get_latest_end_point_metrics(end_point_name, model_name, model_version)
         if endpoint_metrics is None:
             return None
         metrics_dict = {"total_latency": endpoint_metrics.total_latency, "avg_latency": endpoint_metrics.avg_latency,
                         "total_request_num": endpoint_metrics.total_request_num,
                         "current_qps": endpoint_metrics.current_qps,
-                        "avg_qps": endpoint_metrics.avg_qps, "timestamp": endpoint_metrics.timestamp}
+                        "avg_qps": endpoint_metrics.avg_qps, "timestamp": endpoint_metrics.timestamp,
+                        "device_id": endpoint_metrics.device_id}
         return json.dumps(metrics_dict)
 
     def get_monitor_metrics_item(self, end_point_name, model_name, model_version, index):
         endpoint_metrics = self.get_end_point_metrics_by_index(end_point_name, model_name, model_version, index)
         if endpoint_metrics is None:
             return None
         metrics_dict = {"total_latency": endpoint_metrics.total_latency, "avg_latency": endpoint_metrics.avg_latency,
                         "total_request_num": endpoint_metrics.total_request_num,
                         "current_qps": endpoint_metrics.current_qps,
-                        "avg_qps": endpoint_metrics.avg_qps, "timestamp": endpoint_metrics.timestamp}
+                        "avg_qps": endpoint_metrics.avg_qps, "timestamp": endpoint_metrics.timestamp,
+                        "device_id": endpoint_metrics.device_id}
         return json.dumps(metrics_dict)
 
     def open_job_db(self):
         if self.db_connection is not None:
             return
 
         if not os.path.exists(ServerConstants.get_database_dir()):
@@ -268,27 +269,27 @@
             offset(index).limit(1).first()
         return endpoint_metric
 
     def set_end_point_metrics(self, end_point_id, end_point_name,
                               model_name, model_version,
                               total_latency=None, avg_latency=None,
                               total_request_num=None, current_qps=None,
-                              avg_qps=None, timestamp=None):
+                              avg_qps=None, timestamp=None, device_id=None):
         self.open_job_db()
         endpoint_metric = self.db_connection.query(FedMLEndPointMetricsModel). \
             filter(and_(FedMLEndPointMetricsModel.end_point_name == f'{end_point_name}',
                         FedMLEndPointMetricsModel.model_name == f'{model_name}',
                         FedMLEndPointMetricsModel.model_version == f'{model_version}')).first()
         if endpoint_metric is None:
             endpoint_metric = FedMLEndPointMetricsModel(end_point_id=end_point_id,
                                                         end_point_name=end_point_name,
                                                         model_name=model_name, model_version=model_version,
                                                         total_latency=total_latency, avg_latency=avg_latency,
                                                         total_request_num=total_request_num, current_qps=current_qps,
-                                                        avg_qps=avg_qps, timestamp=timestamp)
+                                                        avg_qps=avg_qps, timestamp=timestamp, device_id=device_id)
             self.db_connection.add(endpoint_metric)
             self.db_connection.commit()
             return
 
         if total_latency is not None:
             endpoint_metric.total_latency = total_latency
         if avg_latency is not None:
@@ -297,14 +298,16 @@
             endpoint_metric.total_request_num = total_request_num
         if current_qps is not None:
             endpoint_metric.current_qps = current_qps
         if avg_qps is not None:
             endpoint_metric.avg_qps = avg_qps
         if timestamp is not None:
             endpoint_metric.timestamp = timestamp
+        if device_id is not None:
+            endpoint_metric.device_id = device_id
 
         self.db_connection.commit()
 
 
 class FedMLDeploymentResultInfoModel(Base):
     __tablename__ = 'deployment_result_info'
 
@@ -350,14 +353,15 @@
     model_version = Column(TEXT)
     total_latency = Column(Float)
     avg_latency = Column(Float)
     total_request_num = Column(Integer)
     current_qps = Column(Float)
     avg_qps = Column(Float)
     timestamp = Column(Integer)
+    device_id = Column(TEXT)
 
 
 def test_deployment_result():
     test_end_point_id = "545"
     test_end_point_name = "EndPoint-98f9f598-5ac7-40a4-b780-54c20f19acaa"
     test_model_name = "alex-test-model"
     test_model_version = "v0-Mon Apr 10 12:30:55 CST 2023"
@@ -483,21 +487,22 @@
     test_model_version = "v0-Mon Apr 10 12:30:55 CST 2023"
     total_latency = 1.0
     avg_latency = 1.0
     total_request_num = 1
     current_qps = 1
     avg_qps = 1
     timestamp = time.time()
+    device_id = 100
     FedMLModelDatabase.get_instance().set_monitor_metrics(test_end_point_id,
                                                           test_end_point_name,
                                                           test_model_name,
                                                           test_model_version,
                                                           total_latency, avg_latency,
                                                           total_request_num, current_qps,
-                                                          avg_qps, timestamp)
+                                                          avg_qps, timestamp, device_id)
 
     ret_latest_metrics = FedMLModelDatabase.get_instance().get_latest_monitor_metrics(test_end_point_name,
                                                                                       test_model_name,
                                                                                       test_model_version)
     if ret_latest_metrics is None:
         print("Failed to test for setting and getting end point monitoring metrics")
     else:
```

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_login_entry.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_login_entry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 import os
-import shutil
 import subprocess
-from os.path import expanduser
 
 import click
 
-import fedml
-
 from ...cli.model_deployment.device_client_constants import ClientConstants
 from ...cli.model_deployment.device_server_constants import ServerConstants
 from ...cli.model_deployment.device_client_login import logout as client_logout
-from ...cli.env.collect_env import collect_env
 from ...cli.model_deployment.device_server_login import logout as server_logout
 from ...cli.model_deployment.docker_client_login import login_with_docker_mode
 from ...cli.model_deployment.docker_client_login import logout_with_docker_mode
-from ...cli.model_deployment.docker_client_login import logs_with_docker_mode
 from ...cli.model_deployment.docker_server_login import login_with_server_docker_mode
 from ...cli.model_deployment.docker_server_login import logout_with_server_docker_mode
-from ...cli.model_deployment.docker_server_login import logs_with_server_docker_mode
 from ...cli.comm_utils import sys_utils
 
 
 def login_as_model_device_agent(
     userid, cloud, on_premise, master, infer_host, version, local_server,
     runner_cmd, device_id, os_name, docker, docker_rank, redis_addr, redis_port, redis_password
 ):
@@ -71,15 +64,15 @@
 
         if is_on_premise is True:
             role = ClientConstants.login_role_list[ClientConstants.LOGIN_MODE_ON_PREMISE_INDEX]
 
         if is_cloud is True:
             role = ClientConstants.login_role_list[ClientConstants.LOGIN_MODE_FEDML_CLOUD_INDEX]
 
-        login_pid = subprocess.Popen(
+        login_pid = sys_utils.run_subprocess_open(
             [
                 sys_utils.get_python_program(),
                 login_cmd,
                 "-t",
                 "login",
                 "-u",
                 str(account_id),
@@ -113,15 +106,15 @@
 
         pip_source_dir = os.path.dirname(__file__)
         login_cmd = os.path.join(pip_source_dir, "device_server_daemon.py")
         server_logout()
         sys_utils.cleanup_login_process(ServerConstants.LOCAL_HOME_RUNNER_DIR_NAME, ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME)
         sys_utils.cleanup_all_fedml_server_learning_processes()
         sys_utils.cleanup_all_fedml_server_login_processes("device_server_login.py")
-        login_pid = subprocess.Popen(
+        login_pid = sys_utils.run_subprocess_open(
             [
                 sys_utils.get_python_program(),
                 login_cmd,
                 "-t",
                 "login",
                 "-u",
                 str(account_id),
```

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_client_data_interface.py` & `fedml-0.8.5a1/fedml/cli/edge_deployment/client_data_interface.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import logging
 import os
 import sqlite3
 import time
 import traceback
 
-from fedml.cli.model_deployment.device_client_constants import ClientConstants
+from fedml.cli.edge_deployment.client_constants import ClientConstants
 from fedml.core.common.singleton import Singleton
-from fedml.cli.model_deployment.device_server_constants import ServerConstants
+from fedml.cli.server_deployment.server_constants import ServerConstants
 
 
 class FedMLClientDataInterface(Singleton):
     MAX_JOB_LIST_SIZE = 50000
     ERRCODE_JOB_FAILED = 1
     ERRCODE_JOB_KILLED = 2
-    JOBS_DB = "model-jobs.db"
 
     def __init__(self):
         pass
 
     @staticmethod
     def get_instance():
         return FedMLClientDataInterface()
@@ -110,27 +109,18 @@
                                 status,
                                 status)
         else:
             self.save_job_status(run_id, edge_id,
                                  status,
                                  status)
 
-    def save_job_result(self, job_id, edge_id, deployment_result=None):
-        self.create_job_table()
-
-        job_obj = FedMLClientJobModel()
-        job_obj.job_id = job_id
-        job_obj.edge_id = edge_id
-        job_obj.deployment_result = deployment_result
-        self.update_job_to_db(job_obj)
-
     def open_job_db(self):
         if not os.path.exists(ClientConstants.get_database_dir()):
             os.makedirs(ClientConstants.get_database_dir())
-        job_db_path = os.path.join(ClientConstants.get_database_dir(), FedMLClientDataInterface.JOBS_DB)
+        job_db_path = os.path.join(ClientConstants.get_database_dir(), "jobs.db")
         self.db_connection = sqlite3.connect(job_db_path)
 
     def close_job_db(self):
         if self.db_connection is not None:
             self.db_connection.close()
 
     def create_job_table(self):
@@ -149,16 +139,15 @@
                    status TEXT,
                    failed_time TEXT,
                    error_code INT,
                    msg TEXT,
                    updated_time TEXT,
                    round_index INT,
                    total_rounds INT,
-                   running_json TEXT,
-                   deployment_result TEXT);''')
+                   running_json TEXT);''')
             self.db_connection.commit()
         except Exception as e:
             pass
         self.db_connection.close()
 
     def drop_job_table(self):
         self.open_job_db()
@@ -166,14 +155,39 @@
         try:
             current_cursor.execute('''DROP TABLE IF EXISTS jobs;''')
             self.db_connection.commit()
         except Exception as e:
             logging.info("Process compatibility on the local db.")
         self.db_connection.close()
 
+    def create_agent_status_table(self):
+        self.handle_database_compatibility()
+
+        self.open_job_db()
+        current_cursor = self.db_connection.cursor()
+        try:
+            current_cursor.execute('''CREATE TABLE IF NOT EXISTS agent_status
+                   (edge_id INT NOT NULL,
+                   enabled INT,
+                   updated_time TEXT);''')
+            self.db_connection.commit()
+        except Exception as e:
+            pass
+        self.db_connection.close()
+
+    def drop_agent_status_table(self):
+        self.open_job_db()
+        current_cursor = self.db_connection.cursor()
+        try:
+            current_cursor.execute('''DROP TABLE IF EXISTS agent_status;''')
+            self.db_connection.commit()
+        except Exception as e:
+            logging.info("Process compatibility on the local db.")
+        self.db_connection.close()
+
     def get_current_job_from_db(self):
         job_obj = None
 
         self.open_job_db()
         current_cursor = self.db_connection.cursor()
         results = current_cursor.execute("SELECT *  from jobs order by updated_time desc limit(1)")
         for row in results:
@@ -190,15 +204,14 @@
             job_obj.round_index = row[11]
             job_obj.total_rounds = row[12]
             job_obj.progress = (0 if job_obj.total_rounds == 0 else job_obj.round_index / job_obj.total_rounds)
             total_time = (0 if job_obj.progress == 0 else (float(job_obj.updated_time) - float(job_obj.started_time))
                                                           / job_obj.progress)
             job_obj.eta = total_time * (1.0 - job_obj.progress)
             job_obj.running_json = row[13]
-            job_obj.deployment_result = row[14]
             # job_obj.show()
             break
 
         self.db_connection.close()
         return job_obj
 
     def get_jobs_from_db(self):
@@ -221,26 +234,26 @@
             job_obj.round_index = row[11]
             job_obj.total_rounds = row[12]
             job_obj.progress = (0 if job_obj.total_rounds == 0 else job_obj.round_index / job_obj.total_rounds)
             total_time = (0 if job_obj.progress == 0 else (float(job_obj.updated_time) - float(job_obj.started_time))
                                                           / job_obj.progress)
             job_obj.eta = total_time * (1.0 - job_obj.progress)
             job_obj.running_json = row[13]
-            job_obj.deployment_result = row[14]
             job_list_obj.job_list.append(job_obj)
 
             if len(job_list_obj.job_list) > FedMLClientDataInterface.MAX_JOB_LIST_SIZE:
                 break
 
         self.db_connection.close()
         return job_list_obj
 
     def get_job_by_id(self, job_id):
         if job_id is None:
             return None
+
         job_obj = None
 
         self.open_job_db()
         current_cursor = self.db_connection.cursor()
         results = current_cursor.execute("SELECT *  from jobs where job_id={};".format(job_id))
         for row in results:
             job_obj = FedMLClientJobModel()
@@ -256,15 +269,14 @@
             job_obj.round_index = row[11]
             job_obj.total_rounds = row[12]
             job_obj.progress = (0 if job_obj.total_rounds == 0 else job_obj.round_index / job_obj.total_rounds)
             total_time = (0 if job_obj.progress == 0 else (float(job_obj.updated_time) - float(job_obj.started_time))
                                                           / job_obj.progress)
             job_obj.eta = total_time * (1.0 - job_obj.progress)
             job_obj.running_json = row[13]
-            job_obj.deployment_result = row[14]
             # job_obj.show()
             break
 
         self.db_connection.close()
         return job_obj
 
     def insert_job_to_db(self, job):
@@ -275,67 +287,122 @@
             self.db_connection.close()
             self.update_job_to_db(job)
             return
 
         try:
             current_cursor.execute("INSERT INTO jobs (\
                 job_id, edge_id, started_time, ended_time, progress, ETA, status, failed_time, error_code, msg, \
-                updated_time, round_index, total_rounds, running_json, deployment_result) \
-                VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)",
+                updated_time, round_index, total_rounds, running_json) \
+                VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)",
                                    (job.job_id, job.edge_id, job.started_time, job.ended_time,
                                     job.progress, job.eta, job.status, job.failed_time,
                                     job.error_code, job.msg, str(time.time()),
-                                    job.round_index, job.total_rounds, job.running_json, job.deployment_result))
+                                    job.round_index, job.total_rounds, job.running_json))
         except Exception as e:
             logging.info("Process jobs insertion {}.".format(traceback.format_exc()))
         self.db_connection.commit()
         self.db_connection.close()
 
     def update_job_to_db(self, job):
         self.open_job_db()
         current_cursor = self.db_connection.cursor()
         try:
-            update_statement = "UPDATE jobs set {} {} {} {} {} {} {} {} {} {} {} {} {} where job_id={}".format(
+            update_statement = "UPDATE jobs set {} {} {} {} {} {} {} {} {} {} {} {} where job_id={}".format(
                 f"edge_id={job.edge_id}" if job.edge_id != 0 else "",
                 f",started_time='{job.started_time}'" if job.started_time != "" else "",
                 f",ended_time='{job.ended_time}'" if job.ended_time != "" else "",
                 f",progress={job.progress}" if job.progress != 0 else "",
                 f",eta={job.eta}" if job.eta != 0 else "",
                 f",status='{job.status}'" if job.status != "" else "",
                 f",failed_time='{job.failed_time}'" if job.failed_time != "" else "",
                 f",error_code={job.error_code}" if job.error_code != -1 else "",
                 f",msg='{job.msg}'" if job.msg != "" else "",
                 ",updated_time='" + str(time.time()) + "'",
                 f",round_index={job.round_index}" if job.round_index != 0 else "",
                 f",total_rounds={job.total_rounds}" if job.total_rounds != 0 else "",
-                f",deployment_result='{job.deployment_result}'" if job.deployment_result != "" else "",
                 job.job_id)
             current_cursor.execute(update_statement)
             self.db_connection.commit()
         except Exception as e:
             pass
         self.db_connection.close()
 
     def handle_database_compatibility(self):
         self.open_job_db()
         should_alter_old_table = False
         current_cursor = self.db_connection.cursor()
         results = current_cursor.execute("select * from sqlite_master where type='table' and name='jobs';")
         for row in results:
             table_statement = str(row[4])
-            if table_statement.find("deployment_result") == -1:
+            if table_statement.find("running_json") == -1:
                 should_alter_old_table = True
 
         if should_alter_old_table:
-            current_cursor.execute("ALTER TABLE jobs ADD deployment_result TEXT;")
+            current_cursor.execute("ALTER TABLE jobs ADD running_json TEXT;")
             self.db_connection.commit()
             logging.info("Process compatibility on the local db.")
 
         self.close_job_db()
 
+    def get_agent_status(self, edge_id=0):
+        self.open_job_db()
+        enabled = 1
+        current_cursor = self.db_connection.cursor()
+        try:
+            results = current_cursor.execute("SELECT *  from agent_status where edge_id={};".format(edge_id))
+            for row in results:
+                out_edge_id = row[0]
+                enabled = row[1] > 0
+                update_time = row[2]
+                break
+        except Exception as e:
+            pass
+
+        self.db_connection.close()
+        return enabled
+
+    def insert_agent_status_to_db(self, agent_status, edge_id=0):
+        self.create_agent_status_table()
+        self.open_job_db()
+        current_cursor = self.db_connection.cursor()
+        query_results = current_cursor.execute("SELECT * from agent_status where edge_id={};".format(edge_id))
+        for row in query_results:
+            self.db_connection.close()
+            self.update_agent_status_to_db(agent_status, edge_id)
+            return
+
+        try:
+            current_cursor.execute("INSERT INTO agent_status (\
+                edge_id, enabled, \
+                updated_time) \
+                VALUES (?, ?, ?)",
+                                   (edge_id, agent_status,
+                                    str(time.time())))
+        except Exception as e:
+            logging.info("Process agent status insertion {}.".format(traceback.format_exc()))
+        self.db_connection.commit()
+        self.db_connection.close()
+
+    def update_agent_status_to_db(self, agent_status, edge_id=0):
+        self.create_agent_status_table()
+        self.open_job_db()
+        current_cursor = self.db_connection.cursor()
+        try:
+            update_statement = "UPDATE agent_status set {} {} {} where edge_id={}".format(
+                f"edge_id={edge_id}",
+                f",enabled={agent_status}",
+                ",updated_time='" + str(time.time()) + "'",
+                edge_id)
+            current_cursor.execute(update_statement)
+            self.db_connection.commit()
+        except Exception as e:
+            logging.info("update agent status exception {}".format(traceback.format_exc()))
+            pass
+        self.db_connection.close()
+
 
 class FedMLClientJobModel(object):
 
     def __init__(self):
         self.job_id = 0
         self.edge_id = 0
         self.started_time = ""
@@ -346,15 +413,14 @@
         self.error_code = -1
         self.msg = ""
         self.updated_time = ""
         self.round_index = 0
         self.total_rounds = 0
         self.status = ""
         self.running_json = ""
-        self.deployment_result = ""
 
     def show(self):
         logging.info("Job object, job id {}, edge id {}, started time {},"
                      "ended time {}, progress {}, eta {}, status {},"
                      "failed time {}, error code {}, msg {},"
                      "updated time {}, round index {}, total rounds {}".format(
             self.job_id, self.edge_id, self.started_time,
```

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_server_constants.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_server_constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import json
+
 import os
 import platform
 import signal
 import subprocess
 import sys
 from os.path import expanduser
 
@@ -34,15 +34,15 @@
     MSG_MLOPS_RUN_STATUS_STARTING = "STARTING"
     MSG_MLOPS_RUN_STATUS_RUNNING = "RUNNING"
     MSG_MLOPS_RUN_STATUS_STOPPING = "STOPPING"
     MSG_MLOPS_RUN_STATUS_KILLED = "KILLED"
     MSG_MLOPS_RUN_STATUS_FAILED = "FAILED"
     MSG_MLOPS_RUN_STATUS_FINISHED = "FINISHED"
 
-    LOCAL_HOME_RUNNER_DIR_NAME = 'fedml-server'
+    LOCAL_HOME_RUNNER_DIR_NAME = 'fedml-model-server'
     LOCAL_RUNNER_INFO_DIR_NAME = 'runner_infos'
     LOCAL_PACKAGE_HOME_DIR_NAME = "fedml_packages"
 
     FEDML_OTA_CMD_UPGRADE = "upgrade"
     FEDML_OTA_CMD_RESTART = "restart"
 
     LOCAL_SERVER_API_PORT = 40806
@@ -128,60 +128,78 @@
                                "FP32": MODEL_DATA_TYPE_FLOAT, "FP64": MODEL_DATA_TYPE_FLOAT,
                                "STRING": MODEL_DATA_TYPE_STR, "BF16": MODEL_DATA_TYPE_INT}
 
     @staticmethod
     def get_fedml_home_dir():
         home_dir = expanduser("~")
         fedml_home_dir = os.path.join(home_dir, ServerConstants.LOCAL_HOME_RUNNER_DIR_NAME)
+        if not os.path.exists(fedml_home_dir):
+            os.makedirs(fedml_home_dir)
         return fedml_home_dir
 
     @staticmethod
     def get_log_file_dir():
         log_file_dir = os.path.join(ServerConstants.get_fedml_home_dir(), "fedml", "logs")
+        if not os.path.exists(log_file_dir):
+            os.makedirs(log_file_dir)
         return log_file_dir
 
     @staticmethod
     def get_data_dir():
         data_dir = os.path.join(ServerConstants.get_fedml_home_dir(), "fedml", "data")
+        if not os.path.exists(data_dir):
+            os.makedirs(data_dir)
         return data_dir
 
     @staticmethod
     def get_package_download_dir():
         package_download_dir = os.path.join(ServerConstants.get_fedml_home_dir(),
                                             ServerConstants.LOCAL_PACKAGE_HOME_DIR_NAME)
+        if not os.path.exists(package_download_dir):
+            os.makedirs(package_download_dir)
         return package_download_dir
 
     @staticmethod
     def get_package_unzip_dir(run_id, package_url):
         package_unzip_dir_name = "run_{}_{}".format(str(run_id),
                                                     str(os.path.basename(package_url)).split('.')[0])
         package_unzip_dir = os.path.join(ServerConstants.get_package_download_dir(),
                                          package_unzip_dir_name)
+        if not os.path.exists(package_unzip_dir):
+            os.makedirs(package_unzip_dir)
         return package_unzip_dir
 
     @staticmethod
     def get_package_run_dir(run_id, package_url, package_name):
         package_file_no_extension = str(package_name).split('.')[0]
         package_run_dir = os.path.join(ServerConstants.get_package_unzip_dir(run_id, package_url),
                                        package_file_no_extension)
+        if not os.path.exists(package_run_dir):
+            os.makedirs(package_run_dir)
         return package_run_dir
 
     @staticmethod
     def get_database_dir():
         database_dir = os.path.join(ServerConstants.get_data_dir(), "database")
+        if not os.path.exists(database_dir):
+            os.makedirs(database_dir)
         return database_dir
 
     @staticmethod
     def get_model_dir():
         model_file_dir = os.path.join(ServerConstants.get_fedml_home_dir(), "fedml", "models")
+        if not os.path.exists(model_file_dir):
+            os.makedirs(model_file_dir)
         return model_file_dir
 
     @staticmethod
     def get_model_package_dir():
         model_packages_dir = os.path.join(ServerConstants.get_fedml_home_dir(), "fedml", "model_packages")
+        if not os.path.exists(model_packages_dir):
+            os.makedirs(model_packages_dir)
         return model_packages_dir
 
     @staticmethod
     def get_k8s_master_host_dir(current_dir):
         if not ServerConstants.is_running_on_k8s():
             return current_dir
 
@@ -206,14 +224,16 @@
         if running_source is not None and running_source == ServerConstants.FEDML_RUNNING_SOURCE_ENV_VALUE_K8S:
             return True
         return False
 
     @staticmethod
     def get_model_serving_dir():
         model_file_dir = os.path.join(ServerConstants.get_fedml_home_dir(), "fedml", "models_serving")
+        if not os.path.exists(model_file_dir):
+            os.makedirs(model_file_dir)
         return model_file_dir
 
     @staticmethod
     def get_model_ops_list_url(config_version="release"):
         model_ops_url = "{}/api/v1/model/listFromCli".format(ServerConstants.get_model_ops_url(config_version))
         return model_ops_url
 
@@ -245,94 +265,110 @@
         s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         conn = s.connect(('8.8.8.8', 53))
         ip = s.getsockname()[0]
         s.close()
         return ip
 
     @staticmethod
-    def cleanup_run_process():
+    def cleanup_run_process(run_id):
         try:
-            home_dir = expanduser("~")
             local_pkg_data_dir = ServerConstants.get_data_dir()
             process_id_file = os.path.join(local_pkg_data_dir, ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME,
-                                           "runner-sub-process.id")
+                                           "runner-sub-process-v2.id")
+            if not os.path.exists(process_id_file):
+                return
             process_info = load_yaml_config(process_id_file)
-            process_ids_str = process_info.get('process_id', '[]')
-            process_ids = json.loads(process_ids_str)
-            for process_id in process_ids:
+            if run_id is None:
+                for run_id_key, process_id_value in process_info.items():
+                    ServerConstants.cleanup_run_process(run_id_key)
+                return
+            process_id = process_info.get(str(run_id), None)
+            if process_id is not None:
                 try:
                     process = psutil.Process(process_id)
                     for sub_process in process.children():
-                        os.kill(sub_process.pid, signal.SIGTERM)
+                        if platform.system() == 'Windows':
+                            os.system("taskkill /PID {} /T /F".format(sub_process.pid))
+                        else:
+                            os.kill(sub_process.pid, signal.SIGTERM)
 
                     if process is not None:
-                        os.kill(process.pid, signal.SIGTERM)
+                        if platform.system() == 'Windows':
+                            os.system("taskkill /PID {} /T /F".format(process.pid))
+                        else:
+                            os.kill(process.pid, signal.SIGTERM)
                 except Exception as e:
                     pass
 
-            yaml_object = {}
-            yaml_object['process_id'] = '[]'
-            ServerConstants.generate_yaml_doc(yaml_object, process_id_file)
+                process_info.pop(str(run_id))
+                ServerConstants.generate_yaml_doc(process_info, process_id_file)
         except Exception as e:
             pass
 
     @staticmethod
-    def save_run_process(process_id):
+    def save_run_process(run_id, process_id):
         try:
-            home_dir = expanduser("~")
             local_pkg_data_dir = ServerConstants.get_data_dir()
             process_id_file = os.path.join(local_pkg_data_dir, ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME,
-                                           "runner-sub-process.id")
-            process_ids = []
-            if os.path.exists(process_id_file) is True:
-                yaml_object = load_yaml_config(process_id_file)
-                process_ids_str = yaml_object.get('process_id', '[]')
-                process_ids = json.loads(process_ids_str)
-            process_ids.append(process_id)
-            yaml_object = {}
-            yaml_object['process_id'] = str(process_ids)
-            ServerConstants.generate_yaml_doc(yaml_object, process_id_file)
+                                           "runner-sub-process-v2.id")
+            if os.path.exists(process_id_file):
+                process_info = load_yaml_config(process_id_file)
+            else:
+                process_info = dict()
+            process_info[str(run_id)] = process_id
+            ServerConstants.generate_yaml_doc(process_info, process_id_file)
         except Exception as e:
             pass
 
     @staticmethod
-    def cleanup_learning_process():
+    def cleanup_learning_process(run_id):
         try:
-            home_dir = expanduser("~")
             local_pkg_data_dir = ServerConstants.get_data_dir()
             process_id_file = os.path.join(local_pkg_data_dir, ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME,
-                                           "runner-learning-process.id")
+                                           "runner-learning-process-v2.id")
             process_info = load_yaml_config(process_id_file)
-            process_id = process_info.get('process_id', None)
+            if run_id is None:
+                for run_id_key, process_id_value in process_info.items():
+                    ServerConstants.cleanup_learning_process(run_id_key)
+                return
+            process_id = process_info.get(str(run_id), None)
             if process_id is not None:
                 try:
                     process = psutil.Process(process_id)
                     for sub_process in process.children():
-                        os.kill(sub_process.pid, signal.SIGTERM)
+                        if platform.system() == 'Windows':
+                            os.system("taskkill /PID {} /T /F".format(sub_process.pid))
+                        else:
+                            os.kill(sub_process.pid, signal.SIGTERM)
 
                     if process is not None:
-                        os.kill(process.pid, signal.SIGTERM)
+                        if platform.system() == 'Windows':
+                            os.system("taskkill /PID {} /T /F".format(process.pid))
+                        else:
+                            os.kill(process.pid, signal.SIGTERM)
                 except Exception as e:
                     pass
-            yaml_object = {}
-            yaml_object['process_id'] = -1
-            ServerConstants.generate_yaml_doc(yaml_object, process_id_file)
+
+                process_info.pop(str(run_id))
+                ServerConstants.generate_yaml_doc(process_info, process_id_file)
         except Exception as e:
             pass
 
     @staticmethod
-    def save_learning_process(learning_id):
+    def save_learning_process(run_id, learning_id):
         try:
-            home_dir = expanduser("~")
             local_pkg_data_dir = ServerConstants.get_data_dir()
             process_id_file = os.path.join(local_pkg_data_dir, ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME,
-                                           "runner-learning-process.id")
-            yaml_object = {}
-            yaml_object['process_id'] = learning_id
-            ServerConstants.generate_yaml_doc(yaml_object, process_id_file)
+                                           "runner-learning-process-v2.id")
+            if os.path.exists(process_id_file):
+                process_info = load_yaml_config(process_id_file)
+            else:
+                process_info = dict()
+            process_info[str(run_id)] = learning_id
+            ServerConstants.generate_yaml_doc(process_info, process_id_file)
         except Exception as e:
             pass
 
     @staticmethod
     def save_runner_infos(unique_device_id, edge_id, run_id=None):
         home_dir = expanduser("~")
         local_pkg_data_dir = ServerConstants.get_data_dir()
@@ -381,36 +417,48 @@
 
     @staticmethod
     def exec_console_with_script(script_path, should_capture_stdout=False, should_capture_stderr=False):
         stdout_flag = subprocess.PIPE if should_capture_stdout else sys.stdout
         stderr_flag = subprocess.PIPE if should_capture_stderr else sys.stderr
 
         if platform.system() == 'Windows':
-            script_process = subprocess.Popen(script_path, stdout=stdout_flag, stderr=stderr_flag)
+            script_process = subprocess.Popen(script_path, stdout=stdout_flag, stderr=stderr_flag,
+                                              creationflags=subprocess.CREATE_NEW_PROCESS_GROUP)
         else:
-            script_process = subprocess.Popen(['bash', '-c', script_path], stdout=stdout_flag, stderr=stderr_flag)
+            script_process = subprocess.Popen(['bash', '-c', script_path], stdout=stdout_flag, stderr=stderr_flag,
+                                              preexec_fn=os.setsid)
 
         return script_process
 
     @staticmethod
     def exec_console_with_shell(shell, script_path, should_capture_stdout=False, should_capture_stderr=False):
         stdout_flag = subprocess.PIPE if should_capture_stdout else sys.stdout
         stderr_flag = subprocess.PIPE if should_capture_stderr else sys.stderr
 
-        script_process = subprocess.Popen([shell, script_path], stdout=stdout_flag, stderr=stderr_flag)
+        if platform.system() == 'Windows':
+            script_process = subprocess.Popen([shell, script_path], stdout=stdout_flag, stderr=stderr_flag,
+                                              creationflags=subprocess.CREATE_NEW_PROCESS_GROUP)
+        else:
+            script_process = subprocess.Popen([shell, script_path], stdout=stdout_flag, stderr=stderr_flag,
+                                              preexec_fn=os.setsid)
 
         return script_process
 
     @staticmethod
     def exec_console_with_shell_script_list(shell_script_list, should_capture_stdout=False,
                                             should_capture_stderr=False):
         stdout_flag = subprocess.PIPE if should_capture_stdout else sys.stdout
         stderr_flag = subprocess.PIPE if should_capture_stderr else sys.stderr
 
-        script_process = subprocess.Popen(shell_script_list, stdout=stdout_flag, stderr=stderr_flag)
+        if platform.system() == 'Windows':
+            script_process = subprocess.Popen(shell_script_list, stdout=stdout_flag, stderr=stderr_flag,
+                                              creationflags=subprocess.CREATE_NEW_PROCESS_GROUP)
+        else:
+            script_process = subprocess.Popen(shell_script_list, stdout=stdout_flag, stderr=stderr_flag,
+                                              preexec_fn=os.setsid)
 
         return script_process
 
     @staticmethod
     def get_console_pipe_out_err_results(script_process):
         exec_out, exec_err = script_process.communicate()
         return script_process.returncode, exec_out, exec_err
```

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_model_monitor.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_model_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,22 +31,22 @@
         if start_time is None:
             self.start_time = time.time_ns()
         else:
             self.start_time = start_time
 
     def calc_metrics(self, end_point_id, end_point_name,
                      model_id, model_name, model_version,
-                     inference_output_url):
+                     inference_output_url, device_id):
         total_latency, avg_latency, total_request_num, current_qps, timestamp = 0, 0, 0, 0, 0
         FedMLModelCache.get_instance().set_redis_params(self.redis_addr, self.redis_port, self.redis_password)
         metrics_item = FedMLModelCache.get_instance(self.redis_addr, self.redis_port).\
             get_latest_monitor_metrics(end_point_name, model_name, model_version)
         print(f"calc metrics_item {metrics_item}")
         if metrics_item is not None:
-            total_latency, avg_latency, total_request_num, current_qps, avg_qps, timestamp = \
+            total_latency, avg_latency, total_request_num, current_qps, avg_qps, timestamp, _ = \
                 FedMLModelCache.get_instance(self.redis_addr, self.redis_port).get_metrics_item_info(metrics_item)
         cost_time = (time.time_ns() - self.start_time) / self.ns_per_ms
         total_latency += cost_time
         total_request_num += 1
         current_qps = 1 / (cost_time / self.ms_per_sec)
         current_qps = format(current_qps, '.0f')
         avg_qps = total_request_num / (total_latency / self.ms_per_sec)
@@ -58,15 +58,16 @@
                                                                                            end_point_name,
                                                                                            model_name,
                                                                                            model_version,
                                                                                            total_latency,
                                                                                            avg_latency,
                                                                                            total_request_num,
                                                                                            current_qps, avg_qps,
-                                                                                           timestamp)
+                                                                                           timestamp,
+                                                                                           str(device_id))
 
     def start_monitoring_metrics_center(self):
         self.build_metrics_report_channel()
 
     def build_metrics_report_channel(self):
         args = {"config_version": "release"}
         mqtt_config, _ = ModelOpsConfigs.get_instance(args).fetch_configs(self.config_version)
@@ -97,26 +98,27 @@
     def send_monitoring_metrics(self, index):
         FedMLModelCache.get_instance().set_redis_params(self.redis_addr, self.redis_port, self.redis_password)
         metrics_item, inc_index = FedMLModelCache.get_instance(self.redis_addr, self.redis_port).\
             get_monitor_metrics_item(self.current_end_point_name, self.current_model_name,
                                      self.current_model_version, index)
         if metrics_item is None:
             return index
-        total_latency, avg_latency, total_request_num, current_qps, avg_qps, timestamp = \
+        total_latency, avg_latency, total_request_num, current_qps, avg_qps, timestamp, device_id = \
             FedMLModelCache.get_instance(self.redis_addr, self.redis_port).get_metrics_item_info(metrics_item)
         deployment_monitoring_topic_prefix = "model_ops/model_device/return_inference_monitoring"
         deployment_monitoring_topic = "{}/{}".format(deployment_monitoring_topic_prefix, self.current_end_point_id)
         deployment_monitoring_payload = {"model_name": self.current_model_name,
                                          "model_id": self.current_model_id,
                                          "model_url": self.current_infer_url,
                                          "end_point_id": self.current_end_point_id,
                                          "latency": float(avg_latency),
                                          "qps": int(avg_qps),
                                          "total_request_num": int(total_request_num),
-                                         "timestamp": timestamp}
+                                         "timestamp": timestamp,
+                                         "edgeId": device_id}
         # print("send monitor metrics {}".format(json.dumps(deployment_monitoring_payload)))
 
         self.monitor_mqtt_mgr.send_message_json(deployment_monitoring_topic, json.dumps(deployment_monitoring_payload))
         self.monitor_mqtt_mgr.send_message_json(deployment_monitoring_topic_prefix,
                                                 json.dumps(deployment_monitoring_payload))
         return inc_index
```

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_client_constants.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_client_constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     MSG_MLOPS_RUN_STATUS_STARTING = "STARTING"
     MSG_MLOPS_RUN_STATUS_RUNNING = "RUNNING"
     MSG_MLOPS_RUN_STATUS_STOPPING = "STOPPING"
     MSG_MLOPS_RUN_STATUS_KILLED = "KILLED"
     MSG_MLOPS_RUN_STATUS_FAILED = "FAILED"
     MSG_MLOPS_RUN_STATUS_FINISHED = "FINISHED"
 
-    LOCAL_HOME_RUNNER_DIR_NAME = 'fedml-client'
+    LOCAL_HOME_RUNNER_DIR_NAME = 'fedml-model-client'
     LOCAL_RUNNER_INFO_DIR_NAME = 'runner_infos'
     LOCAL_PACKAGE_HOME_DIR_NAME = "fedml_packages"
 
     CLIENT_LOGIN_PROGRAM = "device_client_login.py"
 
     # Constants for models
     K8S_DEPLOYMENT_MASTER_HOST_HOME_DIR = "/home/fedml-server"
@@ -94,14 +94,15 @@
     MODEL_REQUIRED_MODEL_BIN_FILE = "fedml_model.bin"
     MODEL_REQUIRED_MODEL_README_FILE = "README.md"
 
     CMD_TYPE_CONVERT_MODEL = "convert_model"
     CMD_TYPE_RUN_TRITON_SERVER = "run_triton_server"
     FEDML_CONVERT_MODEL_CONTAINER_NAME_PREFIX = "fedml_convert_model_container"
     FEDML_TRITON_SERVER_CONTAINER_NAME_PREFIX = "fedml_triton_server_container"
+    FEDML_LLM_SERVER_CONTAINER_NAME_PREFIX = "fedml_llm_server_container"
     FEDML_CONVERTED_MODEL_DIR_NAME = "triton_models"
     FEDML_MODEL_SERVING_REPO_SCAN_INTERVAL = 3
 
     FEDML_RUNNING_SOURCE_ENV_NAME = "FEDML_RUNNING_SOURCE"
     FEDML_RUNNING_SOURCE_ENV_VALUE_K8S = "k8s"
 
     MODEL_INFERENCE_DEFAULT_PORT = 5001
@@ -132,62 +133,82 @@
                                "FP32": MODEL_DATA_TYPE_FLOAT, "FP64": MODEL_DATA_TYPE_FLOAT,
                                "STRING": MODEL_DATA_TYPE_STR, "BF16": MODEL_DATA_TYPE_INT}
 
     @staticmethod
     def get_fedml_home_dir():
         home_dir = expanduser("~")
         fedml_home_dir = os.path.join(home_dir, ClientConstants.LOCAL_HOME_RUNNER_DIR_NAME)
+        if not os.path.exists(fedml_home_dir):
+            os.makedirs(fedml_home_dir)
         return fedml_home_dir
 
     @staticmethod
     def get_log_file_dir():
         log_file_dir = os.path.join(ClientConstants.get_fedml_home_dir(), "fedml", "logs")
+        if not os.path.exists(log_file_dir):
+            os.makedirs(log_file_dir)
         return log_file_dir
 
     @staticmethod
     def get_data_dir():
         data_dir = os.path.join(ClientConstants.get_fedml_home_dir(), "fedml", "data")
+        if not os.path.exists(data_dir):
+            os.makedirs(data_dir)
         return data_dir
 
     @staticmethod
     def get_package_download_dir():
         package_download_dir = os.path.join(ClientConstants.get_fedml_home_dir(),
                                             ClientConstants.LOCAL_PACKAGE_HOME_DIR_NAME)
+        if not os.path.exists(package_download_dir):
+            os.makedirs(package_download_dir)
         return package_download_dir
 
     @staticmethod
     def get_package_unzip_dir():
         package_unzip_dir = ClientConstants.get_package_download_dir()
+        if not os.path.exists(package_unzip_dir):
+            os.makedirs(package_unzip_dir)
         return package_unzip_dir
 
     @staticmethod
     def get_package_run_dir(package_name):
         package_file_no_extension = str(package_name).split('.')[0]
         package_run_dir = os.path.join(ClientConstants.get_package_unzip_dir(),
                                        package_file_no_extension)
+        if not os.path.exists(package_run_dir):
+            os.makedirs(package_run_dir)
         return package_run_dir
 
     @staticmethod
     def get_model_dir():
         model_file_dir = os.path.join(ClientConstants.get_fedml_home_dir(), "fedml", "models")
+        if not os.path.exists(model_file_dir):
+            os.makedirs(model_file_dir)
         return model_file_dir
 
     @staticmethod
     def get_model_package_dir():
         model_packages_dir = os.path.join(ClientConstants.get_fedml_home_dir(), "fedml", "model_packages")
+        if not os.path.exists(model_packages_dir):
+            os.makedirs(model_packages_dir)
         return model_packages_dir
 
     @staticmethod
     def get_model_cache_dir():
         model_cache_dir = os.path.join(ClientConstants.get_fedml_home_dir(), "fedml", "model_cache")
+        if not os.path.exists(model_cache_dir):
+            os.makedirs(model_cache_dir)
         return model_cache_dir
 
     @staticmethod
     def get_database_dir():
         database_dir = os.path.join(ClientConstants.get_data_dir(), "database")
+        if not os.path.exists(database_dir):
+            os.makedirs(database_dir)
         return database_dir
 
     @staticmethod
     def get_k8s_master_host_dir(current_dir):
         if not ClientConstants.is_running_on_k8s():
             return current_dir
 
@@ -212,19 +233,23 @@
         if running_source is not None and running_source == ClientConstants.FEDML_RUNNING_SOURCE_ENV_VALUE_K8S:
             return True
         return False
 
     @staticmethod
     def get_model_serving_dir():
         model_file_dir = os.path.join(ClientConstants.get_fedml_home_dir(), "fedml", "models_serving")
+        if not os.path.exists(model_file_dir):
+            os.makedirs(model_file_dir)
         return model_file_dir
 
     @staticmethod
     def get_model_infer_data_dir():
         model_infer_data_dir = os.path.join(ClientConstants.get_fedml_home_dir(), "fedml", "models_infer_data")
+        if not os.path.exists(model_infer_data_dir):
+            os.makedirs(model_infer_data_dir)
         return model_infer_data_dir
 
     @staticmethod
     def get_model_ops_list_url(config_version="release", local_server=None):
         model_ops_url = "{}/api/v1/model/listFromCli".format(
             ClientConstants.get_model_ops_url(config_version, local_server))
         return model_ops_url
@@ -338,82 +363,110 @@
         except Exception as e:
             pass
         ClientConstants.unzip_file(local_package_file, unzip_package_path)
         unzip_package_path = os.path.join(unzip_package_path, package_name)
         return unzip_package_path
 
     @staticmethod
-    def cleanup_run_process():
+    def cleanup_run_process(run_id):
         try:
             local_pkg_data_dir = ClientConstants.get_data_dir()
             process_id_file = os.path.join(local_pkg_data_dir, ClientConstants.LOCAL_RUNNER_INFO_DIR_NAME,
-                                           "runner-sub-process.id")
+                                           "runner-sub-process-v2.id")
+            if not os.path.exists(process_id_file):
+                return
             process_info = load_yaml_config(process_id_file)
-            process_id = process_info.get('process_id', None)
+            if run_id is None:
+                for run_id_key, process_id_value in process_info.items():
+                    ClientConstants.cleanup_run_process(run_id_key)
+                return
+            process_id = process_info.get(str(run_id), None)
             if process_id is not None:
                 try:
                     process = psutil.Process(process_id)
                     for sub_process in process.children():
-                        os.kill(sub_process.pid, signal.SIGTERM)
+                        if platform.system() == 'Windows':
+                            os.system("taskkill /PID {} /T /F".format(sub_process.pid))
+                        else:
+                            os.kill(sub_process.pid, signal.SIGKILL)
 
                     if process is not None:
-                        os.kill(process.pid, signal.SIGTERM)
+                        if platform.system() == 'Windows':
+                            os.system("taskkill /PID {} /T /F".format(process.pid))
+                        else:
+                            os.kill(process.pid, signal.SIGKILL)
                 except Exception as e:
                     pass
-            yaml_object = {}
-            yaml_object['process_id'] = -1
-            ClientConstants.generate_yaml_doc(yaml_object, process_id_file)
+
+                process_info.pop(str(run_id))
+                ClientConstants.generate_yaml_doc(process_info, process_id_file)
         except Exception as e:
             pass
 
     @staticmethod
-    def save_run_process(process_id):
+    def save_run_process(run_id, process_id):
         try:
             local_pkg_data_dir = ClientConstants.get_data_dir()
             process_id_file = os.path.join(local_pkg_data_dir, ClientConstants.LOCAL_RUNNER_INFO_DIR_NAME,
-                                           "runner-sub-process.id")
-            yaml_object = {}
-            yaml_object['process_id'] = process_id
-            ClientConstants.generate_yaml_doc(yaml_object, process_id_file)
+                                           "runner-sub-process-v2.id")
+            if os.path.exists(process_id_file):
+                process_info = load_yaml_config(process_id_file)
+            else:
+                process_info = dict()
+            process_info[str(run_id)] = process_id
+            ClientConstants.generate_yaml_doc(process_info, process_id_file)
         except Exception as e:
             pass
 
     @staticmethod
-    def cleanup_learning_process():
+    def cleanup_learning_process(run_id):
         try:
             local_pkg_data_dir = ClientConstants.get_data_dir()
             process_id_file = os.path.join(local_pkg_data_dir, ClientConstants.LOCAL_RUNNER_INFO_DIR_NAME,
-                                           "runner-learning-process.id")
+                                           "runner-learning-process-v2.id")
             process_info = load_yaml_config(process_id_file)
-            process_id = process_info.get('process_id', None)
+            if run_id is None:
+                for run_id_key, process_id_value in process_info.items():
+                    ClientConstants.cleanup_learning_process(run_id_key)
+                return
+            process_id = process_info.get(str(run_id), None)
             if process_id is not None:
                 try:
                     process = psutil.Process(process_id)
                     for sub_process in process.children():
-                        os.kill(sub_process.pid, signal.SIGTERM)
+                        if platform.system() == 'Windows':
+                            os.system("taskkill /PID {} /T /F".format(sub_process.pid))
+                        else:
+                            os.kill(sub_process.pid, signal.SIGTERM)
 
                     if process is not None:
-                        os.kill(process.pid, signal.SIGTERM)
+                        if platform.system() == 'Windows':
+                            os.system("taskkill /PID {} /T /F".format(process.pid))
+                        else:
+                            os.kill(process.pid, signal.SIGTERM)
                 except Exception as e:
                     pass
-            yaml_object = {}
-            yaml_object['process_id'] = -1
-            ClientConstants.generate_yaml_doc(yaml_object, process_id_file)
+
+                process_info.pop(str(run_id))
+                ClientConstants.generate_yaml_doc(process_info, process_id_file)
         except Exception as e:
             pass
 
     @staticmethod
-    def save_learning_process(learning_id):
+    def save_learning_process(run_id, learning_id):
         try:
             local_pkg_data_dir = ClientConstants.get_data_dir()
             process_id_file = os.path.join(local_pkg_data_dir, ClientConstants.LOCAL_RUNNER_INFO_DIR_NAME,
-                                           "runner-learning-process.id")
-            yaml_object = {}
-            yaml_object['process_id'] = learning_id
-            ClientConstants.generate_yaml_doc(yaml_object, process_id_file)
+                                           "runner-learning-process-v2.id")
+            if os.path.exists(process_id_file):
+                process_info = load_yaml_config(process_id_file)
+            else:
+                process_info = dict()
+            process_info[str(run_id)] = learning_id
+            ClientConstants.generate_yaml_doc(process_info, process_id_file)
         except Exception as e:
             pass
 
     @staticmethod
     def save_runner_infos(unique_device_id, edge_id, run_id=None):
         local_pkg_data_dir = ClientConstants.get_data_dir()
         try:
@@ -496,41 +549,53 @@
     def exec_console_with_script(script_path, should_capture_stdout=False, should_capture_stderr=False,
                                  no_sys_out_err=False):
         stdout_flag = subprocess.PIPE if should_capture_stdout else sys.stdout
         stderr_flag = subprocess.PIPE if should_capture_stderr else sys.stderr
 
         if platform.system() == 'Windows':
             if no_sys_out_err:
-                script_process = subprocess.Popen(script_path)
+                script_process = subprocess.Popen(script_path, creationflags=subprocess.CREATE_NEW_PROCESS_GROUP)
             else:
-                script_process = subprocess.Popen(script_path, stdout=stdout_flag, stderr=stderr_flag)
+                script_process = subprocess.Popen(script_path, stdout=stdout_flag, stderr=stderr_flag,
+                                                  creationflags=subprocess.CREATE_NEW_PROCESS_GROUP)
         else:
             if no_sys_out_err:
-                script_process = subprocess.Popen(['bash', '-c', script_path])
+                script_process = subprocess.Popen(['bash', '-c', script_path], preexec_fn=os.setsid)
             else:
-                script_process = subprocess.Popen(['bash', '-c', script_path], stdout=stdout_flag, stderr=stderr_flag)
+                script_process = subprocess.Popen(['bash', '-c', script_path], stdout=stdout_flag, stderr=stderr_flag,
+                                                  preexec_fn=os.setsid)
 
         return script_process
 
     @staticmethod
     def exec_console_with_shell(shell, script_path, should_capture_stdout=False, should_capture_stderr=False):
         stdout_flag = subprocess.PIPE if should_capture_stdout else sys.stdout
         stderr_flag = subprocess.PIPE if should_capture_stderr else sys.stderr
 
-        script_process = subprocess.Popen([shell, script_path], stdout=stdout_flag, stderr=stderr_flag)
+        if platform.system() == 'Windows':
+            script_process = subprocess.Popen([shell, script_path], stdout=stdout_flag, stderr=stderr_flag,
+                                              creationflags=subprocess.CREATE_NEW_PROCESS_GROUP)
+        else:
+            script_process = subprocess.Popen([shell, script_path], stdout=stdout_flag, stderr=stderr_flag,
+                                              preexec_fn=os.setsid)
 
         return script_process
 
     @staticmethod
     def exec_console_with_shell_script_list(shell_script_list, should_capture_stdout=False,
                                             should_capture_stderr=False):
         stdout_flag = subprocess.PIPE if should_capture_stdout else sys.stdout
         stderr_flag = subprocess.PIPE if should_capture_stderr else sys.stderr
 
-        script_process = subprocess.Popen(shell_script_list, stdout=stdout_flag, stderr=stderr_flag)
+        if platform.system() == 'Windows':
+            script_process = subprocess.Popen(shell_script_list, stdout=stdout_flag, stderr=stderr_flag,
+                                              creationflags=subprocess.CREATE_NEW_PROCESS_GROUP)
+        else:
+            script_process = subprocess.Popen(shell_script_list, stdout=stdout_flag, stderr=stderr_flag,
+                                              preexec_fn=os.setsid)
 
         return script_process
 
     @staticmethod
     def get_console_pipe_out_err_results(script_process):
         exec_out, exec_err = script_process.communicate()
         return script_process.returncode, exec_out, exec_err
```

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_client_runner.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_client_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import time
 import traceback
 import urllib
 import uuid
 import zipfile
 from urllib.parse import urlparse
 
-import click
 import requests
 from fedml import mlops
 from fedml.cli.model_deployment.device_model_msg_object import FedMLModelMsgObject
 from fedml.core.distributed.communication.s3.remote_storage import S3Storage
 from ..comm_utils import sys_utils
 
 from ...core.mlops.mlops_runtime_log import MLOpsRuntimeLog
@@ -35,14 +34,15 @@
 from ...core.mlops.mlops_configs import MLOpsConfigs
 from ...core.mlops.mlops_runtime_log_daemon import MLOpsRuntimeLogDaemon
 from ...core.mlops.mlops_status import MLOpsStatus
 from ..comm_utils.sys_utils import get_sys_runner_info, get_python_program
 from .device_model_deployment import start_deployment
 from .device_client_data_interface import FedMLClientDataInterface
 from ...serving.fedml_client import FedMLModelServingClient
+from ...core.mlops.mlops_utils import MLOpsUtils
 
 
 class RunnerError(Exception):
     """ Runner failed. """
     pass
 
 
@@ -83,14 +83,15 @@
 
         self.mlops_metrics = None
         self.client_active_list = dict()
         self.infer_host = "127.0.0.1"
         self.model_is_from_open = False
 
         self.model_runner_mapping = dict()
+        self.ntp_offset = MLOpsUtils.get_ntp_offset()
 
     def unzip_file(self, zip_file, unzip_file_path):
         result = False
         if zipfile.is_zipfile(zip_file):
             with zipfile.ZipFile(zip_file, "r") as zipf:
                 zipf.extractall(unzip_file_path)
                 result = True
@@ -159,15 +160,15 @@
         pass
 
     def update_local_fedml_config(self, run_id, model_config, model_config_parameters):
         model_name = model_config["model_name"]
         model_storage_url = model_config["model_storage_url"]
         scale_min = model_config["instance_scale_min"]
         scale_max = model_config["instance_scale_max"]
-        inference_engine = model_config["inference_engine"]
+        inference_engine = model_config.get("inference_engine", 0)
         inference_end_point_id = run_id
 
         # Retrieve model package or model binary file.
         if self.model_is_from_open:
             unzip_package_path, model_bin_file = self.retrieve_binary_model_file(model_name, model_storage_url)
         else:
             unzip_package_path, model_bin_file = self.retrieve_and_unzip_package(model_name, model_storage_url)
@@ -198,26 +199,36 @@
 
     def run(self, process_event):
         os.environ['PYTHONWARNINGS'] = 'ignore:semaphore_tracker:UserWarning'
         os.environ.setdefault('PYTHONWARNINGS', 'ignore:semaphore_tracker:UserWarning')
 
         self.run_process_event = process_event
         try:
+            MLOpsUtils.set_ntp_offset(self.ntp_offset)
             self.setup_client_mqtt_mgr()
             self.run_impl()
         except RunnerError:
             logging.info("Runner stopped.")
             self.reset_devices_status(self.edge_id, ClientConstants.MSG_MLOPS_CLIENT_STATUS_KILLED)
         except Exception as e:
-            logging.info("Runner exits with exceptions. {}".format(traceback.format_exc()))
+            logging.error("Runner exits with exceptions. {}".format(traceback.format_exc()))
+            self.reset_devices_status(self.edge_id, ClientConstants.MSG_MLOPS_CLIENT_STATUS_FAILED)
+            MLOpsRuntimeLogDaemon.get_instance(self.args).stop_log_processor(self.run_id, self.edge_id)
+            if self.mlops_metrics is not None:
+                self.mlops_metrics.stop_sys_perf()
+            time.sleep(3)
             sys_utils.cleanup_all_fedml_client_login_processes(ClientConstants.CLIENT_LOGIN_PROGRAM,
                                                                clean_process_group=False)
             sys.exit(1)
         finally:
             logging.info("Release resources.")
+            MLOpsRuntimeLogDaemon.get_instance(self.args).stop_log_processor(self.run_id, self.edge_id)
+            if self.mlops_metrics is not None:
+                self.mlops_metrics.stop_sys_perf()
+            time.sleep(3)
             self.release_client_mqtt_mgr()
 
     def check_runner_stop_event(self):
         if self.run_process_event.is_set():
             logging.info("Received stopping event.")
             raise RunnerError("Runner stopped")
 
@@ -245,15 +256,15 @@
         model_config = self.request_json["model_config"]
         model_name = model_config["model_name"]
         model_id = model_config["model_id"]
         model_version = model_config["model_version"]
         model_storage_url = model_config["model_storage_url"]
         scale_min = model_config["instance_scale_min"]
         scale_max = model_config["instance_scale_max"]
-        inference_engine = model_config["inference_engine"]
+        inference_engine = model_config.get("inference_engine", 0)
         self.model_is_from_open = True if model_config.get("is_from_open", 0) == 1 else False
         if self.model_is_from_open:
             model_net_url = model_config["model_net_url"]
         model_config_parameters = self.request_json["parameters"]
         inference_end_point_id = run_id
         use_gpu = "gpu"  # TODO: Get GPU from device infos
         memory_size = "4096m"  # TODO: Get Memory size for each instance
@@ -339,15 +350,15 @@
                 ClientConstants.INFERENCE_CONVERTOR_IMAGE,
                 ClientConstants.INFERENCE_SERVER_IMAGE,
                 self.infer_host,
                 self.model_is_from_open, model_config_parameters,
                 model_from_open,
                 token)
         if inference_output_url == "":
-            logging.info("failed to deploy the model...")
+            logging.error("failed to deploy the model...")
             self.send_deployment_status(end_point_name, self.edge_id,
                                         model_id, model_name, model_version,
                                         inference_output_url,
                                         ClientConstants.MSG_MODELOPS_DEPLOYMENT_STATUS_FAILED)
             self.send_deployment_results(end_point_name, self.edge_id,
                                          ClientConstants.MSG_MODELOPS_DEPLOYMENT_STATUS_FAILED,
                                          model_id, model_name, inference_output_url,
@@ -418,29 +429,29 @@
         logging.info("Cleanup run successfully when starting failed.")
 
         self.reset_devices_status(self.edge_id, ClientConstants.MSG_MLOPS_CLIENT_STATUS_FAILED)
 
         time.sleep(2)
 
         try:
-            self.mlops_metrics.set_sys_reporting_status(False)
+            self.mlops_metrics.stop_sys_perf()
         except Exception as ex:
             pass
 
         time.sleep(1)
 
     def cleanup_run_when_finished(self):
         logging.info("Cleanup run successfully when finished.")
 
         self.reset_devices_status(self.edge_id, ClientConstants.MSG_MLOPS_CLIENT_STATUS_FINISHED)
 
         time.sleep(2)
 
         try:
-            self.mlops_metrics.set_sys_reporting_status(False)
+            self.mlops_metrics.stop_sys_perf()
         except Exception as ex:
             pass
 
         time.sleep(1)
 
     def on_client_mqtt_disconnected(self, mqtt_client_object):
         if self.client_mqtt_lock is None:
@@ -562,20 +573,24 @@
         device_objs = request_json["device_objs"]
 
         model_config = request_json["model_config"]
         model_name = model_config["model_name"]
         model_storage_url = model_config["model_storage_url"]
         scale_min = model_config["instance_scale_min"]
         scale_max = model_config["instance_scale_max"]
-        inference_engine = model_config["inference_engine"]
+        inference_engine = model_config.get("inference_engine", 0)
         inference_end_point_id = run_id
 
+        try:
+            _, _ = MLOpsConfigs.get_instance(self.args).fetch_configs()
+        except Exception as e:
+            pass
+
         # Terminate previous process about starting or stopping run command
-        ClientConstants.exit_process(self.process)
-        ClientConstants.cleanup_run_process()
+        ClientConstants.cleanup_run_process(run_id)
         ClientConstants.save_runner_infos(self.args.device_id + "." + self.args.os_name, self.edge_id, run_id=run_id)
 
         # Start log processor for current run
         run_id = inference_end_point_id
         self.args.run_id = run_id
         self.args.edge_id = self.edge_id
         MLOpsRuntimeLog.get_instance(self.args).init_logs(show_stdout_log=True)
@@ -597,15 +612,15 @@
         self.run_process_event.clear()
         client_runner.run_process_event = self.run_process_event
         self.model_runner_mapping[run_id] = client_runner
         self.run_id = run_id
         self.process = Process(target=client_runner.run, args=(self.run_process_event,))
         # client_runner.run()
         self.process.start()
-        ClientConstants.save_run_process(self.process.pid)
+        ClientConstants.save_run_process(run_id, self.process.pid)
 
     def set_runner_stopped_event(self, run_id):
         client_runner = self.model_runner_mapping.get(run_id, None)
         if client_runner is not None:
             if client_runner.run_process_event is not None:
                 client_runner.run_process_event.set()
             self.model_runner_mapping.pop(run_id)
@@ -632,16 +647,16 @@
             sys.exit(1)
         finally:
             self.release_client_mqtt_mgr()
 
     def exit_run_with_exception(self):
         logging.info("Exit run successfully.")
 
-        ClientConstants.cleanup_learning_process()
-        ClientConstants.cleanup_run_process()
+        ClientConstants.cleanup_learning_process(self.run_id)
+        ClientConstants.cleanup_run_process(self.run_id)
 
         self.mlops_metrics.report_client_id_status(self.run_id, self.edge_id,
                                                    ClientConstants.MSG_MLOPS_CLIENT_STATUS_FAILED,
                                                    is_from_model=True)
 
         time.sleep(1)
 
@@ -765,15 +780,15 @@
                 device_id = str(get_uuid())
                 logging.info(device_id)
             elif "posix" in os.name:
                 device_id = sys_utils.get_device_id_in_docker()
                 if device_id is None:
                     device_id = hex(uuid.getnode())
             else:
-                device_id = subprocess.Popen(
+                device_id = sys_utils.run_subprocess_open(
                     "hal-get-property --udi /org/freedesktop/Hal/devices/computer --key system.hardware.uuid".split()
                 )
                 device_id = hex(device_id)
 
         if device_id is not None and device_id != "":
             with open(file_for_device_id, 'w', encoding='utf-8') as f:
                 f.write(device_id)
@@ -914,22 +929,23 @@
         mqtt_client_object.subscribe(topic_exit_train_with_exception, qos=2)
         mqtt_client_object.subscribe(topic_ota_msg, qos=2)
 
         # Broadcast the first active message.
         self.send_agent_active_msg()
 
         # Echo results
-        click.echo("")
-        click.echo("Congratulations, you have logged into the FedML ModelOps platform successfully!")
-        click.echo(
-            "Your device id is "
+        print("\n\nCongratulations, your device is connected to the FedML MLOps platform successfully!")
+        print(
+            "Your FedML Edge ID is " + str(self.edge_id) + ", unique device ID is "
             + str(self.unique_device_id)
-            + ". You may review the device in the ModelOps edge device list."
+            + "\n"
         )
 
+        MLOpsRuntimeLog.get_instance(self.args).init_logs(show_stdout_log=True)
+
     def on_agent_mqtt_disconnected(self, mqtt_client_object):
         MLOpsStatus.get_instance().set_client_agent_status(
             self.edge_id, ClientConstants.MSG_MLOPS_CLIENT_STATUS_OFFLINE
         )
         pass
 
     def setup_agent_mqtt_connection(self, service_config):
@@ -967,15 +983,15 @@
         self.mqtt_mgr.connect()
 
         self.setup_client_mqtt_mgr()
         self.mlops_metrics.report_client_training_status(self.edge_id,
                                                          ClientConstants.MSG_MLOPS_CLIENT_STATUS_IDLE,
                                                          is_from_model=True)
         MLOpsStatus.get_instance().set_client_agent_status(self.edge_id, ClientConstants.MSG_MLOPS_CLIENT_STATUS_IDLE)
-        self.mlops_metrics.set_sys_reporting_status(enable=True, is_client=True)
+        self.mlops_metrics.stop_sys_perf()
         setattr(self.args, "mqtt_config_path", service_config["mqtt_config"])
         self.mlops_metrics.report_sys_perf(self.args)
 
         self.recover_start_deployment_msg_after_upgrading()
 
     def start_agent_mqtt_loop(self):
         # Start MQTT message loop
```

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/docker_server_login.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/docker_server_login.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,18 +91,20 @@
             is_deployment_ok = True
     if err is not None:
         err_str = err.decode(encoding="utf-8")
         if str(err_str).find(fedml_docker_name) != -1 and str(err_str).find("Up") != -1:
             is_deployment_ok = True
 
     if is_deployment_ok:
-        click.echo("Congratulations, you have deployed the FedML client agent successfully!")
-        click.echo("Your device id is " + env_current_device_id + ".")
-        click.echo("You may review the device in the ModelOps edge device list.")
-
+        print("\n\nCongratulations, your device is connected to the FedML MLOps platform successfully!")
+        print(
+            "Your unique device ID is "
+            + str(env_current_device_id)
+            + "\n"
+        )
         logs_with_server_docker_mode(docker_rank)
     else:
         click.echo("Oops, you failed to deploy the FedML client agent.")
         click.echo("Please check whether your Docker Application is installed and running normally!")
 
 
 def logout_with_server_docker_mode(docker_rank):
```

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_server_daemon.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_server_daemon.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 
 import argparse
 import os
 import time
-import sys
 
 from fedml.cli.comm_utils.sys_utils import cleanup_all_fedml_server_api_processes, \
     cleanup_all_fedml_server_learning_processes, cleanup_all_fedml_server_login_processes, get_python_program, \
     daemon_ota_upgrade
 from fedml.cli.model_deployment.device_server_constants import ServerConstants
 
 
@@ -28,15 +27,15 @@
     args = parser.parse_args()
     args.user = args.user
 
     pip_source_dir = os.path.dirname(__file__)
     login_cmd = os.path.join(pip_source_dir, "device_server_login.py")
     while True:
         try:
-            ServerConstants.cleanup_run_process()
+            ServerConstants.cleanup_run_process(None)
             cleanup_all_fedml_server_api_processes(is_model_device=True)
             cleanup_all_fedml_server_learning_processes()
             cleanup_all_fedml_server_login_processes("device_server_login.py", clean_process_group=False)
         except Exception as e:
             pass
 
         daemon_ota_upgrade(args)
```

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_client_login.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_client_login.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 
 import argparse
 import json
-import logging
 import os
 import platform
-import subprocess
 import time
-from os.path import expanduser
 
 import click
-from fedml.cli.comm_utils import sys_utils
-from fedml.core.mlops.mlops_runtime_log import MLOpsRuntimeLog
 from fedml.cli.model_deployment.device_client_runner import FedMLClientRunner
 from fedml.cli.model_deployment.device_client_constants import ClientConstants
+from fedml.core.mlops.mlops_utils import MLOpsUtils
 
 
 def init_logs(args, edge_id):
     # Init runtime logs
     args.log_file_dir = ClientConstants.get_log_file_dir()
     args.run_id = 0
-    args.rank = 1
+    args.role = "client"
     client_ids = list()
     client_ids.append(edge_id)
     args.client_id_list = json.dumps(client_ids)
     setattr(args, "using_mlops", True)
-    MLOpsRuntimeLog.get_instance(args).init_logs(show_stdout_log=True)
-    logging.info("client ids:{}".format(args.client_id_list))
+    # MLOpsRuntimeLog.get_instance(args).init_logs(show_stdout_log=True)
+    # logging.info("client ids:{}".format(args.client_id_list))
 
 
 def __login_as_client(args, userid, version):
     setattr(args, "account_id", userid)
     setattr(args, "current_running_dir", ClientConstants.get_fedml_home_dir())
 
     sys_name = platform.system()
@@ -128,19 +124,19 @@
         click.echo("Please check whether your network is normal!")
         return
 
     # Init runtime logs
     setattr(args, "client_id", edge_id)
     runner.args = args
     init_logs(args, edge_id)
-    logging.info("args {}".format(args))
+    # logging.info("args {}".format(args))
 
     # Log arguments and binding results.
-    logging.info("login: unique_device_id = %s" % str(unique_device_id))
-    logging.info("login: edge_id = %s" % str(edge_id))
+    # logging.info("login: unique_device_id = %s" % str(unique_device_id))
+    # logging.info("login: edge_id = %s" % str(edge_id))
     runner.unique_device_id = unique_device_id
     ClientConstants.save_runner_infos(args.current_device_id + "." + args.os_name, edge_id, run_id=0)
 
     # Setup MQTT connection for communication with the FedML server.
     runner.infer_host = args.infer_host
     runner.setup_agent_mqtt_connection(service_config)
 
@@ -149,15 +145,15 @@
 
 
 def login(args):
     __login_as_client(args, args.user, args.version)
 
 
 def logout():
-    ClientConstants.cleanup_run_process()
+    ClientConstants.cleanup_run_process(None)
 
 
 if __name__ == "__main__":
     os.environ['PYTHONWARNINGS'] = 'ignore:semaphore_tracker:UserWarning'
     os.environ.setdefault('PYTHONWARNINGS', 'ignore:semaphore_tracker:UserWarning')
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument("--type", "-t", help="Login or logout to ModelOps platform")
```

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_model_msg_object.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_model_msg_object.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         self.model_config = request_json["model_config"]
         self.model_name = self.model_config["model_name"]
         self.model_id = self.model_config["model_id"]
         self.model_version = self.model_config["model_version"]
         self.model_storage_url = self.model_config["model_storage_url"]
         self.scale_min = self.model_config["instance_scale_min"]
         self.scale_max = self.model_config["instance_scale_max"]
-        self.inference_engine = self.model_config["inference_engine"]
+        self.inference_engine = self.model_config.get("inference_engine", 0)
         self.inference_end_point_id = self.run_id
 
         self. request_json["run_id"] = self.run_id
 
     def show(self, prefix=""):
         print("{}end point id: {}, model name: {}, model id: {},"
               " model version: {}, model url: {}".format(prefix,
```

### Comparing `fedml-0.8.4a9/fedml/cli/model_deployment/device_model_inference_entry.py` & `fedml-0.8.5a1/fedml/cli/model_deployment/device_model_inference_entry.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cli/env/collect_env.py` & `fedml-0.8.5a1/fedml/cli/env/collect_env.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cli/cli.py` & `fedml-0.8.5a1/fedml/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,33 +90,36 @@
 def display_client_logs():
     run_id, edge_id = sys_utils.get_running_info(ClientConstants.LOCAL_HOME_RUNNER_DIR_NAME,
                                                  ClientConstants.LOCAL_RUNNER_INFO_DIR_NAME)
     home_dir = expanduser("~")
     log_file = "{}/{}/fedml/logs/fedml-run-{}-edge-{}.log".format(
         home_dir, ClientConstants.LOCAL_HOME_RUNNER_DIR_NAME, str(run_id), str(edge_id)
     )
+
     if os.path.exists(log_file):
         with open(log_file) as file_handle:
             log_lines = file_handle.readlines()
         for log_line in log_lines:
-            click.echo(log_line)
+            click.echo(log_line, nl=False)
+    print("\nconsole log file path = {}".format(log_file))
 
 
 def display_server_logs():
     run_id, edge_id = sys_utils.get_running_info(ServerConstants.LOCAL_HOME_RUNNER_DIR_NAME,
                                                  ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME)
     home_dir = expanduser("~")
     log_file = "{}/{}/fedml/logs/fedml-run-{}-edge-{}.log".format(
         home_dir, ServerConstants.LOCAL_HOME_RUNNER_DIR_NAME, str(run_id), str(edge_id)
     )
     if os.path.exists(log_file):
         with open(log_file) as file_handle:
             log_lines = file_handle.readlines()
         for log_line in log_lines:
             click.echo(log_line)
+    print("\nconsole log file path = {}".format(log_file))
 
 
 @cli.command("login", help="Login to MLOps platform")
 @click.argument("userid", nargs=-1)
 @click.option(
     "--version",
     "-v",
@@ -162,14 +165,15 @@
 )
 @click.option(
     "--docker-rank", "-dr", default="1", help="docker client rank index (from 1 to n).",
 )
 def mlops_login(
         userid, version, client, server, local_server, role, runner_cmd, device_id, os_name, docker, docker_rank
 ):
+    print("\n Welcome to FedML.ai! \n Start to login the current device to the MLOps (https://open.fedml.ai)...\n")
     if userid is None or len(userid) <= 0:
         click.echo("Please specify your account id, usage: fedml login $your_account_id")
         return
     account_id = userid[0]
     platform_url = "open.fedml.ai"
     if version != "release":
         platform_url = "open-{}.fedml.ai".format(version)
@@ -178,47 +182,45 @@
     if userid == "":
         click.echo(
             "Please provide your account id in the MLOps platform ({}).".format(
                 platform_url
             )
         )
         return
-
     # click.echo("client {}, server {}".format(client, server))
     # Set client as default entity.
     is_client = client
     is_server = server
     if client is None and server is None:
         is_client = True
 
     # Check docker mode.
     is_docker = docker
     if docker is None:
         is_docker = False
 
-    # click.echo("login as client: {}, as server: {}".format(is_client, is_server))
     if is_client is True:
         if is_docker:
             login_with_docker_mode(account_id, version, docker_rank)
             return
         pip_source_dir = os.path.dirname(__file__)
         login_cmd = os.path.join(pip_source_dir, "edge_deployment", "client_daemon.py")
+
         client_logout()
         sys_utils.cleanup_login_process(ClientConstants.LOCAL_HOME_RUNNER_DIR_NAME,
                                         ClientConstants.LOCAL_RUNNER_INFO_DIR_NAME)
         sys_utils.cleanup_all_fedml_client_learning_processes()
         sys_utils.cleanup_all_fedml_client_login_processes("client_login.py")
         sys_utils.cleanup_all_fedml_client_api_processes(kill_all=True)
-
         try:
             ClientConstants.login_role_list.index(role)
         except ValueError as e:
             role = ClientConstants.login_role_list[ClientConstants.LOGIN_MODE_CLIEN_INDEX]
 
-        login_pid = subprocess.Popen(
+        login_pid = sys_utils.run_subprocess_open(
             [
                 sys_utils.get_python_program(),
                 "-W",
                 "ignore",
                 login_cmd,
                 "-t",
                 "login",
@@ -234,15 +236,14 @@
                 device_id,
                 "-os",
                 os_name
             ]
         ).pid
         sys_utils.save_login_process(ClientConstants.LOCAL_HOME_RUNNER_DIR_NAME,
                                      ClientConstants.LOCAL_RUNNER_INFO_DIR_NAME, login_pid)
-
     if is_server is True:
         # Check login mode.
         try:
             ServerConstants.login_role_list.index(role)
         except ValueError as e:
             click.echo(
                 "Please specify login mode as follows ({}).".format(
@@ -259,15 +260,15 @@
         login_cmd = os.path.join(pip_source_dir, "server_deployment", "server_daemon.py")
         server_logout()
         sys_utils.cleanup_login_process(ServerConstants.LOCAL_HOME_RUNNER_DIR_NAME,
                                         ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME)
         sys_utils.cleanup_all_fedml_server_learning_processes()
         sys_utils.cleanup_all_fedml_server_login_processes("server_login.py")
         sys_utils.cleanup_all_fedml_server_api_processes(kill_all=True)
-        login_pid = subprocess.Popen(
+        login_pid = sys_utils.run_subprocess_open(
             [
                 sys_utils.get_python_program(),
                 "-W",
                 "ignore",
                 login_cmd,
                 "-t",
                 "login",
@@ -335,15 +336,15 @@
         server_logout()
         sys_utils.cleanup_login_process(ServerConstants.LOCAL_HOME_RUNNER_DIR_NAME,
                                         ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME)
         sys_utils.cleanup_all_fedml_server_learning_processes()
         sys_utils.cleanup_all_fedml_server_login_processes("server_login.py")
         sys_utils.cleanup_all_fedml_server_api_processes(kill_all=True)
         sys_utils.cleanup_all_fedml_server_login_processes("server_daemon.py")
-
+    print("\nlogout successfully!\n")
 
 @cli.command("build", help="Build packages for MLOps platform (open.fedml.ai)")
 @click.option(
     "--platform",
     "-pf",
     type=str,
     default="octopus",
@@ -666,28 +667,28 @@
     if check_mqtt_daemon:
         ClientDiagnosis.check_mqtt_connection_with_daemon_mode()
 
     sys_utils.cleanup_all_fedml_client_diagnosis_processes()
     if check_mqtt_s3_backend_server:
         pip_source_dir = os.path.dirname(__file__)
         server_diagnosis_cmd = os.path.join(pip_source_dir, "edge_deployment", "client_diagnosis.py")
-        backend_server_process = subprocess.Popen([
+        backend_server_process = sys_utils.run_subprocess_open([
             sys_utils.get_python_program(),
             server_diagnosis_cmd,
             "-t",
             "server",
             "-r",
             run_id
         ]
         ).pid
 
     if check_mqtt_s3_backend_client:
         pip_source_dir = os.path.dirname(__file__)
         client_diagnosis_cmd = os.path.join(pip_source_dir, "edge_deployment", "client_diagnosis.py")
-        backend_client_process = subprocess.Popen([
+        backend_client_process = sys_utils.run_subprocess_open([
             sys_utils.get_python_program(),
             client_diagnosis_cmd,
             "-t",
             "client",
             "-r",
             run_id
         ]
@@ -986,15 +987,15 @@
     "--docker", "-d", default=None, is_flag=True, help="logout from docker mode at the model device agent.",
 )
 @click.option(
     "--docker-rank", "-dr", default=None, help="docker client rank index (from 1 to n).",
 )
 def logout_from_model_ops(slave, master, docker, docker_rank):
     device_login_entry.logout_from_model_ops(slave, master, docker, docker_rank)
-
+    print("\nlogout successfully!\n")
 
 @model.command("create", help="Create local model repository.")
 @click.option(
     "--name", "-n", type=str, help="model name.",
 )
 def create_model(name):
     if FedMLModelCards.get_instance().create_model(name):
```

### Comparing `fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/fedml_config.yaml` & `fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/fedml/config/fedml_config.yaml`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/fedml.yaml` & `fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-server/server-package/conf/fedml.yaml`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/fedml_config.yaml` & `fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/fedml/config/fedml_config.yaml`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/fedml.yaml` & `fedml-0.8.5a1/fedml/cli/build-package/mlops-core/fedml-client/client-package/conf/fedml.yaml`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cli/comm_utils/sys_utils.py` & `fedml-0.8.5a1/fedml/cli/comm_utils/sys_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 import logging
 import os
 import platform
 import signal
-import traceback
 import uuid
 from os.path import expanduser
 
-import click
 import psutil
 import yaml
-from psutil import NoSuchProcess, STATUS_ZOMBIE
 
 from fedml.cli.comm_utils.yaml_utils import load_yaml_config
 import json
 from urllib import request
 from pkg_resources import parse_version
 import fedml
 from packaging import version
 import sys
+import subprocess
 
 from fedml.cli.edge_deployment.client_constants import ClientConstants
-import importlib
 
 
 FETAL_ERROR_START_CODE = 128
 
 SYS_ERR_CODE_MAP = {"0": "Successful exit without errors.",
                     "1": "One or more generic errors encountered upon exit.",
                     "2": "Incorrect usage, such as invalid options or missing arguments.",
@@ -503,26 +500,25 @@
 
 def get_device_id_in_docker():
     docker_env_file = "/.dockerenv"
     cgroup_file = "/proc/1/cgroup"
     product_uuid_file = "/sys/class/dmi/id/product_uuid"
 
     if os.path.exists(docker_env_file) or os.path.exists(cgroup_file):
-        if os.path.exists(product_uuid_file):
-            try:
-                with open(product_uuid_file, 'r') as f:
-                    sys_device_id = f.readline().rstrip("\n").strip(" ")
-                    if sys_device_id is None or sys_device_id == "":
-                        device_id = str(uuid.uuid4())
-                    else:
-                        device_id = "{}-@-{}".format(sys_device_id, str(uuid.uuid4()))
-                    return f"{device_id}-docker"
-            except Exception as e:
-                device_id = str(uuid.uuid4())
+        try:
+            with open(product_uuid_file, 'r') as f:
+                sys_device_id = f.readline().rstrip("\n").strip(" ")
+                if sys_device_id is None or sys_device_id == "":
+                    device_id = str(uuid.uuid4())
+                else:
+                    device_id = "{}-@-{}".format(sys_device_id, str(uuid.uuid4()))
                 return f"{device_id}-docker"
+        except Exception as e:
+            device_id = str(uuid.uuid4())
+            return f"{device_id}-docker"
     return None
 
 
 def versions(configuration_env, pkg_name):
     if configuration_env == "release":
         url = f'https://pypi.python.org/pypi/{pkg_name}/json'
     else:
@@ -651,12 +647,30 @@
         logging.info("Upgrade successfully")
     else:
         logging.info("Upgrade error")
 
     return upgrade_result
 
 
+def is_runner_finished_normally(process_id):
+    log_runner_result_file = os.path.join(expanduser("~"), "fedml_trace", str(process_id))
+    if os.path.exists(log_runner_result_file):
+        os.remove(log_runner_result_file)
+        return True
+
+    return False
+
+
+def run_subprocess_open(shell_script_list):
+    if platform.system() == 'Windows':
+        script_process = subprocess.Popen(shell_script_list, creationflags=subprocess.CREATE_NEW_PROCESS_GROUP)
+    else:
+        script_process = subprocess.Popen(shell_script_list, preexec_fn=os.setsid)
+
+    return script_process
+
+
 if __name__ == '__main__':
     fedml_is_latest_version, local_ver, remote_ver = check_fedml_is_latest_version("dev")
     print("FedML is latest version: {}, local version {}, remote version {}".format(
         fedml_is_latest_version, local_ver, remote_ver))
     do_upgrade("release", remote_ver)
```

### Comparing `fedml-0.8.4a9/fedml/cli/server_deployment/server_data_interface.py` & `fedml-0.8.5a1/fedml/cli/server_deployment/server_data_interface.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cli/server_deployment/server_runner.py` & `fedml-0.8.5a1/fedml/cli/server_deployment/server_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import time
 import traceback
 import urllib
 import uuid
 import zipfile
 from os import listdir
 
-import click
 import requests
 from ...core.mlops.mlops_runtime_log import MLOpsRuntimeLog
 
 from ...core.distributed.communication.mqtt.mqtt_manager import MqttManager
 from ...cli.comm_utils.yaml_utils import load_yaml_config
 from ...cli.edge_deployment.client_constants import ClientConstants
 from ...cli.server_deployment.server_constants import ServerConstants
@@ -33,16 +32,15 @@
 
 from ...core.mlops.mlops_configs import MLOpsConfigs
 from ...core.mlops.mlops_runtime_log_daemon import MLOpsRuntimeLogDaemon
 from ...core.mlops.mlops_status import MLOpsStatus
 from ..comm_utils.sys_utils import get_sys_runner_info, get_python_program
 from ..comm_utils import sys_utils
 from .server_data_interface import FedMLServerDataInterface
-
-import tqdm
+from ...core.mlops.mlops_utils import MLOpsUtils
 
 
 class RunnerError(BaseException):
     """ Runner failed. """
     pass
 
 
@@ -104,14 +102,15 @@
             "${FEDSYS.LOG_SERVER_URL}": "",
         }
 
         self.mlops_metrics = None
         self.client_agent_active_list = dict()
         self.server_active_list = dict()
         self.run_status = None
+        self.ntp_offset = MLOpsUtils.get_ntp_offset()
 
     def build_dynamic_constrain_variables(self, run_id, run_config):
         data_config = run_config["data_config"]
         server_edge_id_list = self.request_json["edgeids"]
         is_using_local_data = 0
         private_data_dir = data_config["privateLocalData"]
         synthetic_data_url = data_config["syntheticDataUrl"]
@@ -243,20 +242,20 @@
         package_conf_object["dynamic_args"]["log_file_dir"] = log_file_dir
 
         # Save new config dictionary to local file
         fedml_updated_config_file = os.path.join(unzip_package_path, "conf", "fedml.yaml")
         ServerConstants.generate_yaml_doc(package_conf_object, fedml_updated_config_file)
 
         # Build dynamic arguments and set arguments to fedml config object
-        if not self.build_dynamic_args(run_config, package_conf_object, unzip_package_path):
+        if not self.build_dynamic_args(run_id, run_config, package_conf_object, unzip_package_path):
             return None, None
 
         return unzip_package_path, package_conf_object
 
-    def build_dynamic_args(self, run_config, package_conf_object, base_dir):
+    def build_dynamic_args(self, run_id, run_config, package_conf_object, base_dir):
         fedml_conf_file = package_conf_object["entry_config"]["conf_file"]
         fedml_conf_file_processed = str(fedml_conf_file).replace('\\', os.sep).replace('/', os.sep)
         fedml_conf_path = os.path.join(base_dir, "fedml", "config",
                                        os.path.basename(fedml_conf_file_processed))
         fedml_conf_object = load_yaml_config(fedml_conf_path)
 
         # Replace local fedml config objects with parameters from MLOps web
@@ -281,22 +280,23 @@
         fedml_conf_object["tracking_args"]["log_server_url"] = package_dynamic_args["log_server_url"]
         if hasattr(self.args, "local_server") and self.args.local_server is not None:
             fedml_conf_object["comm_args"]["local_server"] = self.args.local_server
         bootstrap_script_path = None
         env_args = fedml_conf_object.get("environment_args", None)
         if env_args is not None:
             bootstrap_script_file = env_args.get("bootstrap", None)
-            bootstrap_script_file = str(bootstrap_script_file).replace('\\', os.sep).replace('/', os.sep)
-            if platform.system() == 'Windows':
-                bootstrap_script_file = bootstrap_script_file.replace('.sh', '.bat')
             if bootstrap_script_file is not None:
-                bootstrap_script_dir = os.path.join(base_dir, "fedml", os.path.dirname(bootstrap_script_file))
-                bootstrap_script_path = os.path.join(
-                    bootstrap_script_dir, bootstrap_script_dir, os.path.basename(bootstrap_script_file)
-                )
+                bootstrap_script_file = str(bootstrap_script_file).replace('\\', os.sep).replace('/', os.sep)
+                if platform.system() == 'Windows':
+                    bootstrap_script_file = bootstrap_script_file.replace('.sh', '.bat')
+                if bootstrap_script_file is not None:
+                    bootstrap_script_dir = os.path.join(base_dir, "fedml", os.path.dirname(bootstrap_script_file))
+                    bootstrap_script_path = os.path.join(
+                        bootstrap_script_dir, bootstrap_script_dir, os.path.basename(bootstrap_script_file)
+                    )
         # try:
         #     os.makedirs(package_dynamic_args["data_cache_dir"])
         # except Exception as e:
         #     pass
         fedml_conf_object["dynamic_args"] = package_dynamic_args
 
         ServerConstants.generate_yaml_doc(fedml_conf_object, fedml_conf_path)
@@ -316,14 +316,15 @@
                         bootstrap_scripts = "cd {}; ./{}".format(bootstrap_script_dir,
                                                                  os.path.basename(bootstrap_script_file))
                     bootstrap_scripts = str(bootstrap_scripts).replace('\\', os.sep).replace('/', os.sep)
                     logging.info("Bootstrap scripts are being executed...")
                     process = ServerConstants.exec_console_with_script(bootstrap_scripts,
                                                                        should_capture_stdout=True,
                                                                        should_capture_stderr=True)
+                    ServerConstants.save_bootstrap_process(run_id, process.pid)
                     ret_code, out, err = ServerConstants.get_console_pipe_out_err_results(process)
                     if ret_code is None or ret_code <= 0:
                         if out is not None:
                             out_str = out.decode(encoding="utf-8")
                             if out_str != "":
                                 logging.info("{}".format(out_str))
 
@@ -348,14 +349,16 @@
 
     def run(self, process_event):
         os.environ['PYTHONWARNINGS'] = 'ignore:semaphore_tracker:UserWarning'
         os.environ.setdefault('PYTHONWARNINGS', 'ignore:semaphore_tracker:UserWarning')
 
         self.run_process_event = process_event
         try:
+            MLOpsUtils.set_ntp_offset(self.ntp_offset)
+
             self.setup_client_mqtt_mgr()
 
             if self.run_as_cloud_server:
                 topic_client_exit_train_with_exception = "flserver_agent/" + str(self.run_id) \
                                                          + "/client_exit_train_with_exception"
                 self.client_mqtt_mgr.add_message_listener(topic_client_exit_train_with_exception,
                                                           self.callback_client_exit_train_with_exception)
@@ -363,20 +366,26 @@
 
             self.run_impl()
         except RunnerError:
             logging.info("Runner stopped.")
             self.mlops_metrics.report_server_training_status(self.run_id,
                                                              ServerConstants.MSG_MLOPS_SERVER_STATUS_KILLED)
         except Exception as e:
-            logging.info("Runner exits with exceptions.")
-            sys_utils.cleanup_all_fedml_server_login_processes(ServerConstants.SERVER_LOGIN_PROGRAM,
-                                                               clean_process_group=False)
-            sys.exit(1)
+            logging.error("Runner exits with exceptions. {}".format(traceback.format_exc()))
+            self.mlops_metrics.report_server_training_status(self.run_id,
+                                                             ServerConstants.MSG_MLOPS_SERVER_STATUS_FAILED)
         finally:
             logging.info("Release resources.")
+            MLOpsRuntimeLogDaemon.get_instance(self.args).stop_log_processor(self.run_id, self.edge_id)
+            if self.mlops_metrics is not None:
+                self.mlops_metrics.stop_sys_perf()
+            time.sleep(3)
+            ServerConstants.cleanup_run_process(self.run_id)
+            ServerConstants.cleanup_learning_process(self.run_id)
+            ServerConstants.cleanup_bootstrap_process(self.run_id)
             if not self.run_as_cloud_server:
                 self.release_client_mqtt_mgr()
 
     def check_runner_stop_event(self):
         if self.run_process_event.is_set():
             logging.info("Received stopping event.")
             raise RunnerError("Runner stopped")
@@ -434,15 +443,15 @@
 
         entry_file_config = fedml_config_object["entry_config"]
         dynamic_args_config = fedml_config_object["dynamic_args"]
         entry_file = str(entry_file_config["entry_file"]).replace('\\', os.sep).replace('/', os.sep)
         entry_file = os.path.basename(entry_file)
         conf_file = entry_file_config["conf_file"]
         conf_file = str(conf_file).replace('\\', os.sep).replace('/', os.sep)
-        ServerConstants.cleanup_learning_process()
+        ServerConstants.cleanup_learning_process(run_id)
         self.check_runner_stop_event()
         if not os.path.exists(unzip_package_path):
             logging.info("failed to unzip file.")
             self.check_runner_stop_event()
             self.cleanup_run_when_starting_failed()
             self.send_exit_train_with_exception_request_to_edges(edge_ids, self.start_request_json)
             return
@@ -468,24 +477,29 @@
                 "--role",
                 "server"
             ],
             should_capture_stdout=False,
             should_capture_stderr=True
         )
         logging.info("waiting the aggregation process to aggregate models...")
-        ServerConstants.save_learning_process(process.pid)
+        ServerConstants.save_learning_process(run_id, process.pid)
         ret_code, out, err = ServerConstants.get_console_pipe_out_err_results(process)
+        is_run_ok = sys_utils.is_runner_finished_normally(process.pid)
         if ret_code is None or ret_code <= 0:
-            if out is not None:
-                out_str = out.decode(encoding="utf-8")
-                if out_str != "":
-                    logging.info("{}".format(out_str))
+            if is_run_ok:
+                if out is not None:
+                    out_str = out.decode(encoding="utf-8")
+                    if out_str != "":
+                        logging.info("{}".format(out_str))
 
-            sys_utils.log_return_info(entry_file, 0)
+                sys_utils.log_return_info(entry_file, 0)
         else:
+            is_run_ok = False
+
+        if not is_run_ok:
             # If the run status is killed or finished, then return with the normal state.
             current_job = FedMLServerDataInterface.get_instance().get_job_by_id(run_id)
             if current_job is not None and (current_job.status == ServerConstants.MSG_MLOPS_SERVER_STATUS_FINISHED or
                                             current_job.status == ServerConstants.MSG_MLOPS_SERVER_STATUS_KILLED):
                 return
 
             self.check_runner_stop_event()
@@ -517,25 +531,22 @@
             if self.run_process_event is not None:
                 self.run_process_event.set()
             self.stop_run()
             # if self.run_process is not None:
             #     logging.info("Run will be stopped, waiting...")
             #     self.run_process.join()
         except Exception as e:
-            sys_utils.cleanup_all_fedml_server_login_processes(
-                ServerConstants.SERVER_LOGIN_PROGRAM, clean_process_group=False)
-            sys.exit(1)
+            pass
 
     def stop_run(self):
         edge_id_list = self.request_json["edgeids"]
 
-        ServerConstants.cleanup_learning_process()
-        sys_utils.cleanup_all_bootstrap_processes(
-            ServerConstants.SERVER_BOOTSTRAP_WIN_PROGRAM if platform.system() == "Windows" else
-            ServerConstants.SERVER_BOOTSTRAP_LINUX_PROGRAM, clean_process_group=False)
+        ServerConstants.cleanup_learning_process(self.run_id)
+        ServerConstants.cleanup_bootstrap_process(self.run_id)
+        ServerConstants.cleanup_run_process(self.run_id)
 
         self.send_training_stop_request_to_edges(edge_id_list, json.dumps(self.request_json))
         self.mlops_metrics.report_server_training_status(self.run_id, ServerConstants.MSG_MLOPS_SERVER_STATUS_KILLED)
 
         logging.info("stop run successfully.")
 
         try:
@@ -544,15 +555,15 @@
                 if os.path.basename(package_file).startswith("run_" + str(self.run_id)):
                     shutil.rmtree(os.path.join(local_package_path, package_file), ignore_errors=True)
         except Exception as e:
             pass
 
     def stop_run_when_starting_failed(self):
         edge_id_list = self.request_json["edgeids"]
-        logging.info("edge ids {}".format(str(edge_id_list)))
+        logging.error("edge ids {}".format(str(edge_id_list)))
         self.send_exit_train_with_exception_request_to_edges(edge_id_list, json.dumps(self.request_json))
 
         # logging.info("Stop run successfully when starting failed.")
 
         self.mlops_metrics.report_server_id_status(self.run_id, ServerConstants.MSG_MLOPS_SERVER_STATUS_FAILED)
 
         self.set_all_devices_status(ClientConstants.MSG_MLOPS_CLIENT_STATUS_FAILED)
@@ -564,24 +575,22 @@
         logging.info("Cleanup run successfully when finished.")
 
         self.mlops_metrics.broadcast_server_training_status(
             self.run_id, ServerConstants.MSG_MLOPS_SERVER_STATUS_FINISHED
         )
 
         try:
-            self.mlops_metrics.set_sys_reporting_status(False)
+            self.mlops_metrics.stop_sys_perf()
         except Exception as ex:
             pass
 
         time.sleep(1)
 
-        ServerConstants.cleanup_learning_process()
-        sys_utils.cleanup_all_bootstrap_processes(
-            ServerConstants.SERVER_BOOTSTRAP_WIN_PROGRAM if platform.system() == "Windows" else
-            ServerConstants.SERVER_BOOTSTRAP_LINUX_PROGRAM, clean_process_group=False)
+        ServerConstants.cleanup_learning_process(self.run_id)
+        ServerConstants.cleanup_bootstrap_process(self.run_id)
 
         try:
             local_package_path = ServerConstants.get_package_download_dir()
             for package_file in listdir(local_package_path):
                 if os.path.basename(package_file).startswith("run_" + str(self.run_id)):
                     shutil.rmtree(os.path.join(local_package_path, package_file), ignore_errors=True)
         except Exception as e:
@@ -592,24 +601,22 @@
             self.stop_cloud_server()
 
         logging.info("Cleanup run successfully when starting failed.")
 
         self.mlops_metrics.broadcast_server_training_status(self.run_id, ServerConstants.MSG_MLOPS_SERVER_STATUS_FAILED)
 
         try:
-            self.mlops_metrics.set_sys_reporting_status(False)
+            self.mlops_metrics.stop_sys_perf()
         except Exception as ex:
             pass
 
         time.sleep(1)
 
-        ServerConstants.cleanup_learning_process()
-        sys_utils.cleanup_all_bootstrap_processes(
-            ServerConstants.SERVER_BOOTSTRAP_WIN_PROGRAM if platform.system() == "Windows" else
-            ServerConstants.SERVER_BOOTSTRAP_LINUX_PROGRAM, clean_process_group=False)
+        ServerConstants.cleanup_learning_process(self.run_id)
+        ServerConstants.cleanup_bootstrap_process(self.run_id)
 
         try:
             local_package_path = ServerConstants.get_package_download_dir()
             for package_file in listdir(local_package_path):
                 if os.path.basename(package_file).startswith("run_" + str(self.run_id)):
                     shutil.rmtree(os.path.join(local_package_path, package_file), ignore_errors=True)
         except Exception as e:
@@ -666,15 +673,23 @@
             logging.info(f"Upgrade to version {upgrade_version} ...")
 
             sys_utils.do_upgrade(self.version, upgrade_version)
 
             raise Exception("Restarting after upgraded...")
 
     def callback_start_train(self, topic=None, payload=None):
+        try:
+            _, _ = MLOpsConfigs.get_instance(self.args).fetch_configs()
+        except Exception as e:
+            pass
+
         logging.info("callback_start_train payload: {}".format(payload))
+        logging.info(
+            f"FedMLDebug - Receive: topic ({topic}), payload ({payload})"
+        )
 
         # get training params
         if self.run_as_cloud_server:
             message_bytes = payload.encode("ascii")
             base64_bytes = base64.b64decode(message_bytes)
             payload = base64_bytes.decode("ascii")
             logging.info("decoded payload: {}".format(payload))
@@ -693,30 +708,14 @@
             MLOpsRuntimeLog.get_instance(self.args).init_logs(show_stdout_log=True)
             MLOpsRuntimeLogDaemon.get_instance(self.args).start_log_processor(run_id, self.edge_id)
 
         if not self.run_as_cloud_agent and not self.run_as_cloud_server:
             self.ota_upgrade(payload, request_json)
 
         self.start_request_json = payload
-        if self.run_as_edge_server_and_agent:
-            if self.run_process is not None and \
-                    sys_utils.get_process_running_count(ServerConstants.SERVER_LOGIN_PROGRAM) >= 2:
-                logging.info("There is a running job {}.".format(
-                    self.run_process.pid
-                ))
-                try:
-                    if self.run_process_event is not None:
-                        self.run_process_event.set()
-                    ClientConstants.cleanup_run_process()
-                    self.stop_run()
-                    sys_utils.cleanup_all_fedml_server_login_processes(
-                        ServerConstants.SERVER_LOGIN_PROGRAM, clean_process_group=False)
-                except Exception as e:
-                    logging.info("Error for cleanup the previous run.")
-                    pass
 
         logging.info("save runner information")
 
         self.run_id = run_id
         ServerConstants.save_runner_infos(self.args.device_id + "." + self.args.os_name, self.edge_id, run_id=run_id)
 
         # Start server with multiprocessing mode
@@ -745,15 +744,15 @@
             if self.run_process_event is None:
                 self.run_process_event = multiprocessing.Event()
             self.run_process_event.clear()
             server_runner.run_process_event = self.run_process_event
             logging.info("start the runner process.")
             self.run_process = Process(target=server_runner.run, args=(self.run_process_event,))
             self.run_process.start()
-            ServerConstants.save_run_process(self.run_process.pid)
+            ServerConstants.save_run_process(run_id, self.run_process.pid)
         elif self.run_as_cloud_agent:
             # Start log processor for current run
             MLOpsRuntimeLogDaemon.get_instance(self.args).start_log_processor(
                 run_id, self.request_json.get("cloudServerDeviceId", "0")
             )
 
             server_runner = FedMLServerRunner(
@@ -762,15 +761,15 @@
             server_runner.run_as_cloud_agent = self.run_as_cloud_agent
             server_runner.start_request_json = self.start_request_json
             if self.run_process_event is None:
                 self.run_process_event = multiprocessing.Event()
             server_runner.run_process_event = self.run_process_event
             self.run_process = Process(target=server_runner.start_cloud_server_process_entry)
             self.run_process.start()
-            ServerConstants.save_run_process(self.run_process.pid)
+            ServerConstants.save_run_process(run_id, self.run_process.pid)
         elif self.run_as_cloud_server:
             self.server_agent_id = self.request_json.get("cloud_agent_id", self.edge_id)
             self.start_request_json = json.dumps(self.request_json)
             run_id = self.request_json["runId"]
 
             # Init local database
             FedMLServerDataInterface.get_instance().create_job_table()
@@ -783,17 +782,15 @@
             self.run_process_event.clear()
             self.run(self.run_process_event)
 
     def start_cloud_server_process_entry(self):
         try:
             self.start_cloud_server_process()
         except Exception as e:
-            sys_utils.cleanup_all_fedml_server_login_processes(
-                ServerConstants.SERVER_LOGIN_PROGRAM, clean_process_group=False)
-            sys.exit(1)
+            pass
 
     def start_cloud_server_process(self):
         run_config = self.request_json["run_config"]
         packages_config = run_config["packages_config"]
         self.start_cloud_server(packages_config)
 
     def start_cloud_server(self, packages_config):
@@ -959,19 +956,19 @@
     def setup_client_mqtt_mgr(self):
         if self.client_mqtt_mgr is not None:
             return
 
         if self.client_mqtt_lock is None:
             self.client_mqtt_lock = threading.Lock()
 
-        logging.info(
-            "server agent config: {},{}".format(
-                self.agent_config["mqtt_config"]["BROKER_HOST"], self.agent_config["mqtt_config"]["BROKER_PORT"]
-            )
-        )
+        # logging.info(
+        #     "server agent config: {},{}".format(
+        #         self.agent_config["mqtt_config"]["BROKER_HOST"], self.agent_config["mqtt_config"]["BROKER_PORT"]
+        #     )
+        # )
 
         self.client_mqtt_mgr = MqttManager(
             self.agent_config["mqtt_config"]["BROKER_HOST"],
             self.agent_config["mqtt_config"]["BROKER_PORT"],
             self.agent_config["mqtt_config"]["MQTT_USER"],
             self.agent_config["mqtt_config"]["MQTT_PWD"],
             self.agent_config["mqtt_config"]["MQTT_KEEPALIVE"],
@@ -1012,29 +1009,33 @@
             self.client_mqtt_mgr.send_message(topic_stop_train, payload)
             self.mlops_metrics.common_broadcast_client_training_status(edge_id,
                                                                        ClientConstants.MSG_MLOPS_CLIENT_STATUS_KILLED)
 
     def send_exit_train_with_exception_request_to_edges(self, edge_id_list, payload):
         for edge_id in edge_id_list:
             topic_exit_train = "flserver_agent/" + str(edge_id) + "/exit_train_with_exception"
-            logging.info("exit_train_with_exception: send topic " + topic_exit_train)
+            logging.error("exit_train_with_exception: send topic " + topic_exit_train)
             self.client_mqtt_mgr.send_message(topic_exit_train, payload)
             self.mlops_metrics.common_broadcast_client_training_status(edge_id,
                                                                        ClientConstants.MSG_MLOPS_CLIENT_STATUS_FAILED)
 
     def callback_stop_train(self, topic, payload):
         # logging.info("callback_stop_train: topic = %s, payload = %s" % (topic, payload))
+        logging.info(
+            f"FedMLDebug - Receive: topic ({topic}), payload ({payload})"
+        )
 
         request_json = json.loads(payload)
         is_retain = request_json.get("is_retain", False)
         if is_retain:
             return
         run_id = request_json.get("runId", None)
         if run_id is None:
             run_id = request_json.get("id", None)
+
         edge_id_list = request_json["edgeids"]
         server_id = request_json.get("serverId", None)
         if server_id is None:
             server_id = request_json.get("server_id", None)
 
         if run_id is None or server_id is None:
             logging("Json format is not correct!")
@@ -1082,36 +1083,35 @@
 
     def exit_run_with_exception_entry(self):
         try:
             self.setup_client_mqtt_mgr()
             self.exit_run_with_exception()
         except Exception as e:
             self.release_client_mqtt_mgr()
-            sys_utils.cleanup_all_fedml_server_login_processes(
-                ServerConstants.SERVER_LOGIN_PROGRAM, clean_process_group=False)
-            sys.exit(1)
+
         finally:
             self.release_client_mqtt_mgr()
 
     def exit_run_with_exception(self):
-        logging.info("Exit run successfully.")
+        logging.error("Exit run successfully.")
 
-        ServerConstants.cleanup_learning_process()
-        ServerConstants.cleanup_run_process()
-        sys_utils.cleanup_all_bootstrap_processes(
-            ServerConstants.SERVER_BOOTSTRAP_WIN_PROGRAM if platform.system() == "Windows" else
-            ServerConstants.SERVER_BOOTSTRAP_LINUX_PROGRAM, clean_process_group=False)
+        ServerConstants.cleanup_learning_process(self.run_id)
+        ServerConstants.cleanup_run_process(self.run_id)
+        ServerConstants.cleanup_bootstrap_process(self.run_id)
 
         self.mlops_metrics.report_server_id_status(self.run_id,
                                                    ServerConstants.MSG_MLOPS_SERVER_STATUS_FAILED)
 
         time.sleep(1)
 
     def callback_exit_train_with_exception(self, topic, payload):
         # logging.info("callback_exit_train_with_exception: topic = %s, payload = %s" % (topic, payload))
+        logging.info(
+            f"FedMLDebug - Receive: topic ({topic}), payload ({payload})"
+        )
 
         request_json = json.loads(payload)
         is_retain = request_json.get("is_retain", False)
         if is_retain:
             return
         run_id = request_json.get("runId", None)
         if run_id is None:
@@ -1138,35 +1138,38 @@
 
     def callback_client_exit_train_with_exception(self, topic, payload):
         # logging.info("callback_client_exit_train_with_exception: topic = %s, payload = %s" % (topic, payload))
 
         request_json = json.loads(payload)
         run_id = request_json.get("run_id", None)
         edge_id = request_json.get("edge_id", None)
+        msg = request_json.get("msg", None)
         if run_id is None:
             logging.info("callback_client_exit_train_with_exception run id is none")
             return
 
         job = FedMLServerDataInterface.get_instance().get_job_by_id(run_id)
         if job is not None and job.running_json is not None and job.running_json != "":
             job_json_obj = json.loads(job.running_json)
             edge_ids = job_json_obj.get("edgeids", None)
 
+            if msg is not None:
+                logging.error(f"{msg}")
+
             self.mlops_metrics.broadcast_server_training_status(run_id, ServerConstants.MSG_MLOPS_SERVER_STATUS_FAILED)
 
             self.send_exit_train_with_exception_request_to_edges(edge_ids, job.running_json)
 
             self.exit_run_with_exception()
 
-            if not self.run_as_cloud_server:
-                sys_utils.cleanup_all_fedml_server_login_processes(
-                    ServerConstants.SERVER_LOGIN_PROGRAM, clean_process_group=False)
-
     def callback_runner_id_status(self, topic, payload):
         # logging.info("callback_runner_id_status: topic = %s, payload = %s" % (topic, payload))
+        logging.info(
+            f"FedMLDebug - Receive: topic ({topic}), payload ({payload})"
+        )
 
         request_json = json.loads(payload)
         is_retain = request_json.get("is_retain", False)
         if is_retain:
             return
         run_id = request_json["run_id"]
         status = request_json["status"]
@@ -1216,27 +1219,35 @@
             logging.info("received to finished status.")
             self.cleanup_run_when_finished()
         elif self.run_status == ServerConstants.MSG_MLOPS_SERVER_STATUS_FAILED:
             logging.info("received to failed status.")
             self.cleanup_run_when_starting_failed()
 
     def callback_report_current_status(self, topic, payload):
+        logging.info(
+            f"FedMLDebug - Receive: topic ({topic}), payload ({payload})"
+        )
+
         request_json = json.loads(payload)
         if self.run_as_edge_server_and_agent:
             self.send_agent_active_msg()
         elif self.run_as_cloud_agent:
             self.send_agent_active_msg()
         elif self.run_as_cloud_server:
             pass
 
     @staticmethod
     def process_ota_upgrade_msg():
         os.system("pip install -U fedml")
 
     def callback_server_ota_msg(self, topic, payload):
+        logging.info(
+            f"FedMLDebug - Receive: topic ({topic}), payload ({payload})"
+        )
+
         request_json = json.loads(payload)
         cmd = request_json["cmd"]
 
         if cmd == ServerConstants.FEDML_OTA_CMD_UPGRADE:
             try:
                 self.process_ota_upgrade_msg()
                 # Process(target=FedMLServerRunner.process_ota_upgrade_msg).start()
@@ -1283,15 +1294,15 @@
 
                 device_id = str(get_uuid())
             elif "posix" in os.name:
                 device_id = sys_utils.get_device_id_in_docker()
                 if device_id is None:
                     device_id = hex(uuid.getnode())
             else:
-                device_id = subprocess.Popen(
+                device_id = sys_utils.run_subprocess_open(
                     "hal-get-property --udi /org/freedesktop/Hal/devices/computer --key system.hardware.uuid".split()
                 )
                 device_id = hex(device_id)
 
         if device_id is not None and device_id != "":
             with open(file_for_device_id, 'w', encoding='utf-8') as f:
                 f.write(device_id)
@@ -1446,18 +1457,21 @@
         mqtt_client_object.subscribe(topic_ota_msg, qos=2)
         mqtt_client_object.subscribe(topic_exit_train_with_exception, qos=2)
 
         # Broadcast the first active message.
         self.send_agent_active_msg()
 
         # Echo results
-        click.echo("")
-        click.echo("Congratulations, you have logged into the FedML MLOps platform successfully!")
-        click.echo("Your server unique device id is " + str(self.unique_device_id))
-
+        print("\n\nCongratulations, your device is connected to the FedML MLOps platform successfully!")
+        print(
+            "Your FedML Edge ID is " + str(self.edge_id) + ", unique device ID is "
+            + str(self.unique_device_id)
+            + "\n"
+        )
+        
     def on_agent_mqtt_disconnected(self, mqtt_client_object):
         MLOpsStatus.get_instance().set_server_agent_status(
             self.edge_id, ServerConstants.MSG_MLOPS_SERVER_STATUS_OFFLINE
         )
 
     def setup_agent_mqtt_connection(self, service_config):
         # Setup MQTT connection
```

### Comparing `fedml-0.8.4a9/fedml/cli/server_deployment/job_manager.py` & `fedml-0.8.5a1/fedml/cli/server_deployment/job_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cli/server_deployment/docker_login.py` & `fedml-0.8.5a1/fedml/cli/server_deployment/docker_login.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,18 +93,20 @@
             is_deployment_ok = True
     if err is not None:
         err_str = err.decode(encoding="utf-8")
         if str(err_str).find(fedml_docker_name) != -1 and str(err_str).find("Up") != -1:
             is_deployment_ok = True
 
     if is_deployment_ok:
-        click.echo("Congratulations, you have deployed the FedML client agent successfully!")
-        click.echo("Your device id is " + env_current_device_id + ".")
-        click.echo("You may review the device in the MLOps edge device list.")
-
+        print("\n\nCongratulations, your device is connected to the FedML MLOps platform successfully!")
+        print(
+            "Your unique device ID is "
+            + str(env_current_device_id)
+            + "\n"
+        )
         logs_with_server_docker_mode(docker_rank)
     else:
         click.echo("Oops, you failed to deploy the FedML client agent.")
         click.echo("Please check whether your Docker Application is installed and running normally!")
 
 
 def logout_with_server_docker_mode(docker_rank):
```

### Comparing `fedml-0.8.4a9/fedml/cli/server_deployment/app_manager.py` & `fedml-0.8.5a1/fedml/cli/server_deployment/app_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cli/server_deployment/server_daemon.py` & `fedml-0.8.5a1/fedml/cli/server_deployment/server_daemon.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 
 import argparse
 import os
 import time
-import sys
 
 from fedml.cli.comm_utils.sys_utils import cleanup_all_fedml_server_api_processes,\
     cleanup_all_fedml_server_learning_processes,cleanup_all_fedml_server_login_processes, get_python_program, \
     daemon_ota_upgrade
 from fedml.cli.server_deployment.server_constants import ServerConstants
 
 
@@ -25,17 +24,17 @@
     args.user = args.user
 
     pip_source_dir = os.path.dirname(__file__)
     login_cmd = os.path.join(pip_source_dir, "server_login.py")
 
     while True:
         try:
-            ServerConstants.cleanup_run_process()
+            ServerConstants.cleanup_run_process(None)
             cleanup_all_fedml_server_api_processes()
-            cleanup_all_fedml_server_learning_processes()
+            cleanup_all_fedml_server_learning_processes(None)
             cleanup_all_fedml_server_login_processes("server_login.py", clean_process_group=False)
         except Exception as e:
             pass
 
         daemon_ota_upgrade(args)
 
         login_pid = ServerConstants.exec_console_with_shell_script_list(
```

### Comparing `fedml-0.8.4a9/fedml/cli/server_deployment/templates/fedml-server-deployment.yaml` & `fedml-0.8.5a1/fedml/cli/server_deployment/templates/fedml-server-deployment.yaml`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cli/server_deployment/server_login.py` & `fedml-0.8.5a1/fedml/cli/server_deployment/server_login.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import logging
 import os
 import platform
 import time
 
 import click
 from fedml.cli.comm_utils import sys_utils
-from fedml.core.mlops.mlops_runtime_log import MLOpsRuntimeLog
 from fedml.cli.server_deployment.server_runner import FedMLServerRunner
 from fedml.cli.server_deployment.server_constants import ServerConstants
+from fedml.core.mlops.mlops_utils import MLOpsUtils
 
 
 def __login_as_edge_server_and_agent(args, userid, version):
     setattr(args, "account_id", userid)
     setattr(args, "current_running_dir", ServerConstants.get_fedml_home_dir())
 
     sys_name = platform.system()
@@ -57,15 +57,15 @@
         except Exception as e:
             config_try_count += 1
             time.sleep(3)
             continue
 
     if config_try_count >= 5:
         click.echo("")
-        click.echo("Oops, you failed to login the FedML MLOps platform.")
+        click.echo("[5] Oops, you failed to login the FedML MLOps platform.")
         click.echo("Please check whether your network is normal!")
         return
 
     # Judge whether running from fedml docker hub
     is_from_fedml_docker_hub = False
     dock_loc_file = ServerConstants.get_docker_location_file()
     if os.path.exists(dock_loc_file):
@@ -94,25 +94,25 @@
         except Exception as e:
             register_try_count += 1
             time.sleep(3)
             continue
 
     if edge_id <= 0:
         click.echo("")
-        click.echo("Oops, you failed to login the FedML MLOps platform.")
+        click.echo("[6] Oops, you failed to login the FedML MLOps platform.")
         click.echo("Please check whether your network is normal!")
         return
     setattr(args, "server_id", edge_id)
     runner.args = args
     runner.edge_id = edge_id
     init_logs(edge_id)
 
     # Log arguments and binding results.
-    logging.info("login: unique_device_id = %s" % str(unique_device_id))
-    logging.info("login: server_id = %s" % str(edge_id))
+    # logging.info("login: unique_device_id = %s" % str(unique_device_id))
+    # logging.info("login: server_id = %s" % str(edge_id))
     runner.unique_device_id = unique_device_id
     ServerConstants.save_runner_infos(args.current_device_id + "." + args.os_name, edge_id)
 
     # Setup MQTT connection for communication with the FedML server.
     runner.setup_agent_mqtt_connection(service_config)
 
     # Start mqtt looper
@@ -160,15 +160,15 @@
         except Exception as e:
             config_try_count += 1
             time.sleep(3)
             continue
 
     if config_try_count >= 5:
         click.echo("")
-        click.echo("Oops, you failed to login the FedML MLOps platform.")
+        click.echo("[7] Oops, you failed to login the FedML MLOps platform.")
         click.echo("Please check whether your network is normal!")
         return
 
     # Build unique device id
     if args.current_device_id is not None and len(str(args.current_device_id)) > 0:
         unique_device_id = args.current_device_id + "@" + args.os_name + ".Public.Cloud"
 
@@ -189,15 +189,15 @@
         except Exception as e:
             register_try_count += 1
             time.sleep(3)
             continue
 
     if edge_id <= 0:
         click.echo("")
-        click.echo("Oops, you failed to login the FedML MLOps platform.")
+        click.echo("[8] Oops, you failed to login the FedML MLOps platform.")
         click.echo("Please check whether your network is normal!")
         return
     setattr(args, "server_id", edge_id)
     runner.args = args
     runner.edge_id = edge_id
     init_logs(edge_id)
     logging.info("args {}".format(args))
@@ -256,15 +256,15 @@
         except Exception as e:
             config_try_count += 1
             time.sleep(3)
             continue
 
     if config_try_count >= 5:
         click.echo("")
-        click.echo("Oops, you failed to login the FedML MLOps platform.")
+        click.echo("[9] Oops, you failed to login the FedML MLOps platform.")
         click.echo("Please check whether your network is normal!")
         return
 
     # Build unique device id
     if hasattr(args, "device_id") and args.device_id is not None and args.device_id != "0":
         unique_device_id = args.current_device_id
     else:
@@ -284,57 +284,60 @@
         except Exception as e:
             register_try_count += 1
             time.sleep(3)
             continue
 
     if edge_id <= 0:
         click.echo("")
-        click.echo("Oops, you failed to login the FedML MLOps platform.")
+        click.echo("[10] Oops, you failed to login the FedML MLOps platform.")
         click.echo("Please check whether your network is normal!")
         return
     setattr(args, "server_id", edge_id)
     runner.args = args
     runner.edge_id = edge_id
     init_logs(edge_id)
 
     # Log arguments and binding results.
     logging.info("login: unique_device_id = %s" % str(unique_device_id))
     logging.info("login: server_id = %s" % str(edge_id))
     ServerConstants.save_runner_infos(args.current_device_id + "." + args.os_name, edge_id)
 
     # Echo results
-    logging.info("Congratulations, you have logged into the FedML MLOps platform successfully!")
-    logging.info("Your server unique device id is " + str(unique_device_id))
-
+    print("\n\nCongratulations, your device is connected to the FedML MLOps platform successfully!")
+    print(
+        "Your unique device ID is "
+        + str(unique_device_id)
+        + "\n"
+    )
     # Start the FedML server
     runner.callback_start_train(payload=args.runner_cmd)
 
 
 def init_logs(edge_id):
     # Init runtime logs
     args.log_file_dir = ServerConstants.get_log_file_dir()
     args.run_id = 0
-    args.rank = 0
+    args.role = "server"
     args.edge_id = edge_id
     setattr(args, "using_mlops", True)
     setattr(args, "server_agent_id", edge_id)
-    MLOpsRuntimeLog.get_instance(args).init_logs(show_stdout_log=True)
+    # MLOpsRuntimeLog.get_instance(args).init_logs(show_stdout_log=True)
 
 
 def login(args):
     if args.role == ServerConstants.login_role_list[ServerConstants.LOGIN_MODE_LOCAL_INDEX]:
         __login_as_edge_server_and_agent(args, args.user, args.version)
     elif args.role == ServerConstants.login_role_list[ServerConstants.LOGIN_MODE_CLOUD_AGENT_INDEX]:
         __login_as_cloud_agent(args, args.user, args.version)
     elif args.role == ServerConstants.login_role_list[ServerConstants.LOGIN_MODE_CLOUD_SERVER_INDEX]:
         __login_as_cloud_server(args, args.user, args.version)
 
 
 def logout():
-    ServerConstants.cleanup_run_process()
+    ServerConstants.cleanup_run_process(None)
     sys_utils.cleanup_all_fedml_server_api_processes()
 
 
 if __name__ == "__main__":
     os.environ['PYTHONWARNINGS'] = 'ignore:semaphore_tracker:UserWarning'
     os.environ.setdefault('PYTHONWARNINGS', 'ignore:semaphore_tracker:UserWarning')
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
```

### Comparing `fedml-0.8.4a9/fedml/cli/server_deployment/server_constants.py` & `fedml-0.8.5a1/fedml/cli/server_deployment/server_constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import json
+
 import os
 import platform
 import signal
 import subprocess
 import sys
 from os.path import expanduser
 
@@ -56,50 +56,64 @@
     LOGIN_MODE_CLOUD_SERVER_INDEX = 2
     login_role_list = ["edge_server", "cloud_agent", "cloud_server"]
 
     @staticmethod
     def get_fedml_home_dir():
         home_dir = expanduser("~")
         fedml_home_dir = os.path.join(home_dir, ServerConstants.LOCAL_HOME_RUNNER_DIR_NAME)
+        if not os.path.exists(fedml_home_dir):
+            os.makedirs(fedml_home_dir)
         return fedml_home_dir
 
     @staticmethod
     def get_log_file_dir():
         log_file_dir = os.path.join(ServerConstants.get_fedml_home_dir(), "fedml", "logs")
+        if not os.path.exists(log_file_dir):
+            os.makedirs(log_file_dir)
         return log_file_dir
 
     @staticmethod
     def get_data_dir():
         data_dir = os.path.join(ServerConstants.get_fedml_home_dir(), "fedml", "data")
+        if not os.path.exists(data_dir):
+            os.makedirs(data_dir)
         return data_dir
 
     @staticmethod
     def get_package_download_dir():
         package_download_dir = os.path.join(ServerConstants.get_fedml_home_dir(),
                                             ServerConstants.LOCAL_PACKAGE_HOME_DIR_NAME)
+        if not os.path.exists(package_download_dir):
+            os.makedirs(package_download_dir)
         return package_download_dir
 
     @staticmethod
     def get_package_unzip_dir(run_id, package_url):
         package_unzip_dir_name = "run_{}_{}".format(str(run_id),
                                                     str(os.path.basename(package_url)).split('.')[0])
         package_unzip_dir = os.path.join(ServerConstants.get_package_download_dir(),
                                          package_unzip_dir_name)
+        if not os.path.exists(package_unzip_dir):
+            os.makedirs(package_unzip_dir)
         return package_unzip_dir
 
     @staticmethod
     def get_package_run_dir(run_id, package_url, package_name):
         package_file_no_extension = str(package_name).split('.')[0]
         package_run_dir = os.path.join(ServerConstants.get_package_unzip_dir(run_id, package_url),
                                        package_file_no_extension)
+        if not os.path.exists(package_run_dir):
+            os.makedirs(package_run_dir)
         return package_run_dir
 
     @staticmethod
     def get_database_dir():
         database_dir = os.path.join(ServerConstants.get_data_dir(), "database")
+        if not os.path.exists(database_dir):
+            os.makedirs(database_dir)
         return database_dir
 
     @staticmethod
     def get_mlops_url(config_version="release"):
         return "https://open{}.fedml.ai".format(
             "" if config_version == "release" else "-" + config_version)
 
@@ -118,24 +132,77 @@
     @staticmethod
     def get_app_update_url(config_version="release"):
         app_url = "{}/fedmlOpsServer/api/v1/application/updateApplicationFromCli".format(
             ServerConstants.get_mlops_url(config_version))
         return app_url
 
     @staticmethod
-    def cleanup_run_process():
+    def cleanup_run_process(run_id):
+        try:
+            local_pkg_data_dir = ServerConstants.get_data_dir()
+            process_id_file = os.path.join(local_pkg_data_dir, ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME,
+                                           "runner-sub-process-v2.id")
+            if not os.path.exists(process_id_file):
+                return
+            process_info = load_yaml_config(process_id_file)
+            if run_id is None:
+                for run_id_key, process_id_value in process_info.items():
+                    ServerConstants.cleanup_run_process(run_id_key)
+                return
+            process_id = process_info.get(str(run_id), None)
+            if process_id is not None:
+                try:
+                    process = psutil.Process(process_id)
+                    for sub_process in process.children():
+                        if platform.system() == 'Windows':
+                            os.system("taskkill /PID {} /T /F".format(sub_process.pid))
+                        else:
+                            os.kill(sub_process.pid, signal.SIGTERM)
+
+                    if process is not None:
+                        if platform.system() == 'Windows':
+                            os.system("taskkill /PID {} /T /F".format(process.pid))
+                        else:
+                            os.kill(process.pid, signal.SIGTERM)
+                except Exception as e:
+                    pass
+
+                process_info.pop(str(run_id))
+                ServerConstants.generate_yaml_doc(process_info, process_id_file)
+        except Exception as e:
+            pass
+
+    @staticmethod
+    def save_run_process(run_id, process_id):
+        try:
+            local_pkg_data_dir = ServerConstants.get_data_dir()
+            process_id_file = os.path.join(local_pkg_data_dir, ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME,
+                                           "runner-sub-process-v2.id")
+            if os.path.exists(process_id_file):
+                process_info = load_yaml_config(process_id_file)
+            else:
+                process_info = dict()
+            process_info[str(run_id)] = process_id
+            ServerConstants.generate_yaml_doc(process_info, process_id_file)
+        except Exception as e:
+            pass
+
+    @staticmethod
+    def cleanup_learning_process(run_id):
         try:
-            home_dir = expanduser("~")
             local_pkg_data_dir = ServerConstants.get_data_dir()
             process_id_file = os.path.join(local_pkg_data_dir, ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME,
-                                           "runner-sub-process.id")
+                                           "runner-learning-process-v2.id")
             process_info = load_yaml_config(process_id_file)
-            process_ids_str = process_info.get('process_id', '[]')
-            process_ids = json.loads(process_ids_str)
-            for process_id in process_ids:
+            if run_id is None:
+                for run_id_key, process_id_value in process_info.items():
+                    ServerConstants.cleanup_learning_process(run_id_key)
+                return
+            process_id = process_info.get(str(run_id), None)
+            if process_id is not None:
                 try:
                     process = psutil.Process(process_id)
                     for sub_process in process.children():
                         if platform.system() == 'Windows':
                             os.system("taskkill /PID {} /T /F".format(sub_process.pid))
                         else:
                             os.kill(sub_process.pid, signal.SIGTERM)
@@ -144,48 +211,48 @@
                         if platform.system() == 'Windows':
                             os.system("taskkill /PID {} /T /F".format(process.pid))
                         else:
                             os.kill(process.pid, signal.SIGTERM)
                 except Exception as e:
                     pass
 
-            yaml_object = {}
-            yaml_object['process_id'] = '[]'
-            ServerConstants.generate_yaml_doc(yaml_object, process_id_file)
+                process_info.pop(str(run_id))
+                ServerConstants.generate_yaml_doc(process_info, process_id_file)
         except Exception as e:
             pass
 
     @staticmethod
-    def save_run_process(process_id):
+    def save_learning_process(run_id, learning_id):
         try:
-            home_dir = expanduser("~")
             local_pkg_data_dir = ServerConstants.get_data_dir()
             process_id_file = os.path.join(local_pkg_data_dir, ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME,
-                                           "runner-sub-process.id")
-            process_ids = []
-            if os.path.exists(process_id_file) is True:
-                yaml_object = load_yaml_config(process_id_file)
-                process_ids_str = yaml_object.get('process_id', '[]')
-                process_ids = json.loads(process_ids_str)
-            process_ids.append(process_id)
-            yaml_object = {}
-            yaml_object['process_id'] = str(process_ids)
-            ServerConstants.generate_yaml_doc(yaml_object, process_id_file)
+                                           "runner-learning-process-v2.id")
+            if os.path.exists(process_id_file):
+                process_info = load_yaml_config(process_id_file)
+            else:
+                process_info = dict()
+            process_info[str(run_id)] = learning_id
+            ServerConstants.generate_yaml_doc(process_info, process_id_file)
         except Exception as e:
             pass
 
     @staticmethod
-    def cleanup_learning_process():
+    def cleanup_bootstrap_process(run_id):
         try:
-            home_dir = expanduser("~")
             local_pkg_data_dir = ServerConstants.get_data_dir()
             process_id_file = os.path.join(local_pkg_data_dir, ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME,
-                                           "runner-learning-process.id")
+                                           "runner-bootstrap-process-v2.id")
+            if not os.path.exists(process_id_file):
+                return
             process_info = load_yaml_config(process_id_file)
-            process_id = process_info.get('process_id', None)
+            if run_id is None:
+                for run_id_key, process_id_value in process_info.items():
+                    ServerConstants.cleanup_bootstrap_process(run_id_key)
+                return
+            process_id = process_info.get(str(run_id), None)
             if process_id is not None:
                 try:
                     process = psutil.Process(process_id)
                     for sub_process in process.children():
                         if platform.system() == 'Windows':
                             os.system("taskkill /PID {} /T /F".format(sub_process.pid))
                         else:
@@ -194,36 +261,37 @@
                     if process is not None:
                         if platform.system() == 'Windows':
                             os.system("taskkill /PID {} /T /F".format(process.pid))
                         else:
                             os.kill(process.pid, signal.SIGTERM)
                 except Exception as e:
                     pass
-            yaml_object = {}
-            yaml_object['process_id'] = -1
-            ServerConstants.generate_yaml_doc(yaml_object, process_id_file)
+
+                process_info.pop(str(run_id))
+                ServerConstants.generate_yaml_doc(process_info, process_id_file)
         except Exception as e:
             pass
 
     @staticmethod
-    def save_learning_process(learning_id):
+    def save_bootstrap_process(run_id, process_id):
         try:
-            home_dir = expanduser("~")
             local_pkg_data_dir = ServerConstants.get_data_dir()
             process_id_file = os.path.join(local_pkg_data_dir, ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME,
-                                           "runner-learning-process.id")
-            yaml_object = {}
-            yaml_object['process_id'] = learning_id
-            ServerConstants.generate_yaml_doc(yaml_object, process_id_file)
+                                           "runner-bootstrap-process-v2.id")
+            if os.path.exists(process_id_file):
+                process_info = load_yaml_config(process_id_file)
+            else:
+                process_info = dict()
+            process_info[str(run_id)] = process_id
+            ServerConstants.generate_yaml_doc(process_info, process_id_file)
         except Exception as e:
             pass
 
     @staticmethod
     def save_runner_infos(unique_device_id, edge_id, run_id=None):
-        home_dir = expanduser("~")
         local_pkg_data_dir = ServerConstants.get_data_dir()
         try:
             os.makedirs(local_pkg_data_dir)
         except Exception as e:
             pass
         try:
             os.makedirs(os.path.join(local_pkg_data_dir, ServerConstants.LOCAL_RUNNER_INFO_DIR_NAME))
@@ -266,36 +334,48 @@
 
     @staticmethod
     def exec_console_with_script(script_path, should_capture_stdout=False, should_capture_stderr=False):
         stdout_flag = subprocess.PIPE if should_capture_stdout else sys.stdout
         stderr_flag = subprocess.PIPE if should_capture_stderr else sys.stderr
 
         if platform.system() == 'Windows':
-            script_process = subprocess.Popen(script_path, stdout=stdout_flag, stderr=stderr_flag)
+            script_process = subprocess.Popen("dir", stdout=stdout_flag, stderr=stderr_flag,
+                                              creationflags=subprocess.CREATE_NEW_PROCESS_GROUP)
         else:
-            script_process = subprocess.Popen(['bash', '-c', script_path], stdout=stdout_flag, stderr=stderr_flag)
+            script_process = subprocess.Popen(['bash', '-c', script_path], stdout=stdout_flag, stderr=stderr_flag,
+                                              preexec_fn=os.setsid)
 
         return script_process
 
     @staticmethod
     def exec_console_with_shell(shell, script_path, should_capture_stdout=False, should_capture_stderr=False):
         stdout_flag = subprocess.PIPE if should_capture_stdout else sys.stdout
         stderr_flag = subprocess.PIPE if should_capture_stderr else sys.stderr
 
-        script_process = subprocess.Popen([shell, script_path], stdout=stdout_flag, stderr=stderr_flag)
+        if platform.system() == 'Windows':
+            script_process = subprocess.Popen([shell, script_path], stdout=stdout_flag, stderr=stderr_flag,
+                                              creationflags=subprocess.CREATE_NEW_PROCESS_GROUP)
+        else:
+            script_process = subprocess.Popen([shell, script_path], stdout=stdout_flag, stderr=stderr_flag,
+                                              preexec_fn=os.setsid)
 
         return script_process
 
     @staticmethod
     def exec_console_with_shell_script_list(shell_script_list, should_capture_stdout=False,
                                             should_capture_stderr=False):
         stdout_flag = subprocess.PIPE if should_capture_stdout else sys.stdout
         stderr_flag = subprocess.PIPE if should_capture_stderr else sys.stderr
 
-        script_process = subprocess.Popen(shell_script_list, stdout=stdout_flag, stderr=stderr_flag)
+        if platform.system() == 'Windows':
+            script_process = subprocess.Popen(shell_script_list, stdout=stdout_flag, stderr=stderr_flag,
+                                              creationflags=subprocess.CREATE_NEW_PROCESS_GROUP)
+        else:
+            script_process = subprocess.Popen(shell_script_list, stdout=stdout_flag, stderr=stderr_flag,
+                                              preexec_fn=os.setsid)
 
         return script_process
 
     @staticmethod
     def get_console_pipe_out_err_results(script_process):
         exec_out, exec_err = script_process.communicate()
         return script_process.returncode, exec_out, exec_err
```

### Comparing `fedml-0.8.4a9/fedml/cheetah/server/message_define.py` & `fedml-0.8.5a1/fedml/cheetah/server/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cheetah/server/fedml_server_manager.py` & `fedml-0.8.5a1/fedml/cross_silo/server/fedml_server_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 
         self.client_finished_mapping = {}
 
         self.is_initialized = False
         self.client_id_list_in_this_round = None
         self.data_silo_index_list = None
 
+    def is_main_process(self):
+        return getattr(self.aggregator, "aggregator", None) is None or self.aggregator.aggregator.is_main_process()
+
     def run(self):
         super().run()
 
     def send_init_msg(self):
         global_model_params = self.aggregator.get_global_model_params()
 
         global_model_url = None
@@ -52,29 +55,25 @@
             client_idx_in_this_round += 1
 
         mlops.event("server.wait", event_started=True, event_value=str(self.args.round_idx))
 
         try:
             # get input type and shape for inference
             dummy_input_tensor = self.aggregator.get_dummy_input_tensor()
-            logging.info(f"dummy tensor: {dummy_input_tensor}")  # sample tensor for ONNX
 
             model_net_url = mlops.log_training_model_net_info(self.aggregator.aggregator.model, dummy_input_tensor)
 
             # type and shape for later configuration
             input_shape, input_type = self.aggregator.get_input_shape_type()
-            logging.info(f"input shape: {input_shape}")  # [torch.Size([1, 24]), torch.Size([1, 2])]
-            logging.info(f"input type: {input_type}")    # [torch.int64, torch.float32]
 
             # Send output input size and type (saved as json) to s3,
             # and transfer when click "Create Model Card"
             model_input_url = mlops.log_training_model_input_info(list(input_shape), list(input_type))
         except Exception as e:
-            logging.info("exception when processing model net and model input info: {}".format(
-                traceback.format_exc()))
+            logging.info("Cannot get dummy input size or shape for model serving")
 
     def register_message_receive_handlers(self):
         logging.info("register_message_receive_handlers------")
         self.register_message_receive_handler(
             MyMessage.MSG_TYPE_CONNECTION_IS_READY, self.handle_message_connection_ready
         )
 
@@ -141,15 +140,17 @@
                 break
 
         logging.info(
             "sender_id = %d, all_client_is_finished = %s" % (msg_params.get_sender_id(), str(all_client_is_finished))
         )
 
         if all_client_is_finished:
-            mlops.log_aggregation_finished_status()
+            mlops.stop_sys_perf()
+            if self.is_main_process():
+                mlops.log_aggregation_finished_status()
             time.sleep(5)
             self.finish()
 
     def handle_message_client_status_update(self, msg_params):
         client_status = msg_params.get(MyMessage.MSG_ARG_KEY_CLIENT_STATUS)
         logging.info(f"received client status {client_status}")
         if client_status == FedMLServerManager.ONLINE_STATUS_FLAG:
@@ -178,15 +179,16 @@
             logging.info("self.client_id_list_in_this_round = {}".format(self.client_id_list_in_this_round))
             new_client_id_list_in_this_round = []
             for client_idx in model_list_idxes:
                 new_client_id_list_in_this_round.append(self.client_id_list_in_this_round[client_idx])
             logging.info("new_client_id_list_in_this_round = {}".format(new_client_id_list_in_this_round))
             Context().add(Context.KEY_CLIENT_ID_LIST_IN_THIS_ROUND, new_client_id_list_in_this_round)
 
-            MLOpsProfilerEvent.log_to_wandb({"AggregationTime": time.time() - tick, "round": self.args.round_idx})
+            if self.is_main_process():
+                MLOpsProfilerEvent.log_to_wandb({"AggregationTime": time.time() - tick, "round": self.args.round_idx})
 
             self.aggregator.test_on_server_for_all_clients(self.args.round_idx)
 
             self.aggregator.assess_contribution()
 
             mlops.event("server.agg_and_eval", event_started=False, event_value=str(self.args.round_idx))
 
@@ -197,43 +199,42 @@
                 self.args.round_idx, self.client_real_ids, self.args.client_num_per_round
             )
             self.data_silo_index_list = self.aggregator.data_silo_selection(
                 self.args.round_idx, self.args.client_num_in_total, len(self.client_id_list_in_this_round),
             )
             Context().add(Context.KEY_CLIENT_ID_LIST_IN_THIS_ROUND, self.client_id_list_in_this_round)
 
-            if self.args.round_idx == 0:
+            if self.args.round_idx == 0 and self.is_main_process():
                 MLOpsProfilerEvent.log_to_wandb({"BenchmarkStart": time.time()})
 
             client_idx_in_this_round = 0
             global_model_url = None
             global_model_key = None
             for receiver_id in self.client_id_list_in_this_round:
                 client_index = self.data_silo_index_list[client_idx_in_this_round]
                 if type(global_model_params) is dict:
-                    # compatible with the old version that, user did not give {-1 : global_parms_dict}
+                    # compatible with the old version that, user did not give {-1 : global_params_dict}
                     global_model_url, global_model_key = self.send_message_diff_sync_model_to_client(
                         receiver_id, global_model_params[client_index], client_index
                     )
                 else:
                     global_model_url, global_model_key = self.send_message_sync_model_to_client(
                         receiver_id, global_model_params, client_index, global_model_url, global_model_key
                     )
                 client_idx_in_this_round += 1
 
-            # if user give {-1 : global_parms_dict}, then record global_model url separately
+            # if user give {-1 : global_params_dict}, then record global_model url separately
             if type(global_model_params) is dict and (-1 in global_model_params.keys()):
                 global_model_url, global_model_key = self.send_message_diff_sync_model_to_client(
                     -1, global_model_params[-1], -1
                 )
 
             self.args.round_idx += 1
-            mlops.log_aggregated_model_info(
-                self.args.round_idx, model_url=global_model_url,
-                )
+            if self.is_main_process():
+                mlops.log_aggregated_model_info(self.args.round_idx, model_url=global_model_url)
 
             logging.info("\n\n==========end {}-th round training===========\n".format(self.args.round_idx))
             if self.args.round_idx < self.round_num:
                 mlops.event("server.wait", event_started=True, event_value=str(self.args.round_idx))
 
     def cleanup(self):
         client_idx_in_this_round = 0
@@ -241,27 +242,28 @@
             self.send_message_finish(
                 client_id, self.data_silo_index_list[client_idx_in_this_round],
             )
             client_idx_in_this_round += 1
 
     def send_message_init_config(self, receive_id, global_model_params, datasilo_index,
                                  global_model_url=None, global_model_key=None):
-        tick = time.time()
-        message = Message(MyMessage.MSG_TYPE_S2C_INIT_CONFIG, self.get_sender_id(), receive_id)
-        if global_model_url is not None:
-            message.add_params(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_URL, global_model_url)
-        if global_model_key is not None:
-            message.add_params(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_KEY, global_model_key)
-        message.add_params(MyMessage.MSG_ARG_KEY_MODEL_PARAMS, global_model_params)
-        message.add_params(MyMessage.MSG_ARG_KEY_CLIENT_INDEX, str(datasilo_index))
-        message.add_params(MyMessage.MSG_ARG_KEY_CLIENT_OS, "PythonClient")
-        self.send_message(message)
-        global_model_url = message.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_URL)
-        global_model_key = message.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_KEY)
-        MLOpsProfilerEvent.log_to_wandb({"Communiaction/Send_Total": time.time() - tick})
+        if self.is_main_process():
+            tick = time.time()
+            message = Message(MyMessage.MSG_TYPE_S2C_INIT_CONFIG, self.get_sender_id(), receive_id)
+            if global_model_url is not None:
+                message.add_params(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_URL, global_model_url)
+            if global_model_key is not None:
+                message.add_params(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_KEY, global_model_key)
+            message.add_params(MyMessage.MSG_ARG_KEY_MODEL_PARAMS, global_model_params)
+            message.add_params(MyMessage.MSG_ARG_KEY_CLIENT_INDEX, str(datasilo_index))
+            message.add_params(MyMessage.MSG_ARG_KEY_CLIENT_OS, "PythonClient")
+            self.send_message(message)
+            global_model_url = message.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_URL)
+            global_model_key = message.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_KEY)
+            MLOpsProfilerEvent.log_to_wandb({"Communiaction/Send_Total": time.time() - tick})
         return global_model_url, global_model_key
 
     def send_message_check_client_status(self, receive_id, datasilo_index):
         message = Message(MyMessage.MSG_TYPE_S2C_CHECK_CLIENT_STATUS, self.get_sender_id(), receive_id)
         message.add_params(MyMessage.MSG_ARG_KEY_CLIENT_INDEX, str(datasilo_index))
         self.send_message(message)
 
@@ -271,41 +273,46 @@
         self.send_message(message)
         logging.info(
             "finish from send id {} to receive id {}.".format(message.get_sender_id(), message.get_receiver_id()))
         logging.info(" ====================send cleanup message to {}====================".format(str(datasilo_index)))
 
     def send_message_sync_model_to_client(self, receive_id, global_model_params, client_index,
                                           global_model_url=None, global_model_key=None):
-        tick = time.time()
-        logging.info("send_message_sync_model_to_client. receive_id = %d" % receive_id)
-        message = Message(MyMessage.MSG_TYPE_S2C_SYNC_MODEL_TO_CLIENT, self.get_sender_id(), receive_id, )
-        message.add_params(MyMessage.MSG_ARG_KEY_MODEL_PARAMS, global_model_params)
-        if global_model_url is not None:
-            message.add_params(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_URL, global_model_url)
-        if global_model_key is not None:
-            message.add_params(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_KEY, global_model_key)
-        message.add_params(MyMessage.MSG_ARG_KEY_CLIENT_INDEX, str(client_index))
-        message.add_params(MyMessage.MSG_ARG_KEY_CLIENT_OS, "PythonClient")
-        self.send_message(message)
+        if self.is_main_process():
+            tick = time.time()
+            logging.info("send_message_sync_model_to_client. receive_id = %d" % receive_id)
+            message = Message(MyMessage.MSG_TYPE_S2C_SYNC_MODEL_TO_CLIENT, self.get_sender_id(), receive_id, )
+            message.add_params(MyMessage.MSG_ARG_KEY_MODEL_PARAMS, global_model_params)
+            if global_model_url is not None:
+                message.add_params(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_URL, global_model_url)
+            if global_model_key is not None:
+                message.add_params(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_KEY, global_model_key)
+            message.add_params(MyMessage.MSG_ARG_KEY_CLIENT_INDEX, str(client_index))
+            message.add_params(MyMessage.MSG_ARG_KEY_CLIENT_OS, "PythonClient")
+            self.send_message(message)
 
-        MLOpsProfilerEvent.log_to_wandb({"Communiaction/Send_Total": time.time() - tick})
+            MLOpsProfilerEvent.log_to_wandb({"Communiaction/Send_Total": time.time() - tick})
 
-        global_model_url = message.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_URL)
-        global_model_key = message.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_KEY)
+            global_model_url = message.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_URL)
+            global_model_key = message.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_KEY)
 
         return global_model_url, global_model_key
 
     def send_message_diff_sync_model_to_client(self, receive_id, client_model_params, client_index):
-        tick = time.time()
-        logging.info("send_message_sync_model_to_client. receive_id = %d" % receive_id)
-        message = Message(MyMessage.MSG_TYPE_S2C_SYNC_MODEL_TO_CLIENT, self.get_sender_id(), receive_id, )
-        message.add_params(MyMessage.MSG_ARG_KEY_MODEL_PARAMS, client_model_params)
-        message.add_params(MyMessage.MSG_ARG_KEY_CLIENT_INDEX, str(client_index))
-        message.add_params(MyMessage.MSG_ARG_KEY_CLIENT_OS, "PythonClient")
-        self.send_message(message)
+        global_model_url = None
+        global_model_key = None
 
-        MLOpsProfilerEvent.log_to_wandb({"Communiaction/Send_Total": time.time() - tick})
+        if self.is_main_process():
+            tick = time.time()
+            logging.info("send_message_sync_model_to_client. receive_id = %d" % receive_id)
+            message = Message(MyMessage.MSG_TYPE_S2C_SYNC_MODEL_TO_CLIENT, self.get_sender_id(), receive_id, )
+            message.add_params(MyMessage.MSG_ARG_KEY_MODEL_PARAMS, client_model_params)
+            message.add_params(MyMessage.MSG_ARG_KEY_CLIENT_INDEX, str(client_index))
+            message.add_params(MyMessage.MSG_ARG_KEY_CLIENT_OS, "PythonClient")
+            self.send_message(message)
 
-        global_model_url = message.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_URL)
-        global_model_key = message.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_KEY)
-        
-        return global_model_url, global_model_key
+            MLOpsProfilerEvent.log_to_wandb({"Communiaction/Send_Total": time.time() - tick})
+
+            global_model_url = message.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_URL)
+            global_model_key = message.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_KEY)
+
+        return global_model_url, global_model_key
```

### Comparing `fedml-0.8.4a9/fedml/cheetah/server/fedml_aggregator.py` & `fedml-0.8.5a1/fedml/cross_silo/server/fedml_aggregator.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,17 @@
             Context().add(Context.KEY_METRICS_ON_AGGREGATED_MODEL, metric_result_in_current_round)
             if metric_results_in_the_last_round is not None:
                 Context().add(Context.KEY_METRICS_ON_LAST_ROUND, metric_results_in_the_last_round)
             else:
                 Context().add(Context.KEY_METRICS_ON_LAST_ROUND, metric_result_in_current_round)
             key_metrics_on_last_round = Context().get(Context.KEY_METRICS_ON_LAST_ROUND)
             logging.info("key_metrics_on_last_round = {}".format(key_metrics_on_last_round))
+
+            if round_idx == self.args.comm_round - 1:
+                mlops.log({"round_idx": round_idx})
         else:
             mlops.log({"round_idx": round_idx})
     
     def get_dummy_input_tensor(self):
         test_data = None
         if self.test_global:
             test_data = self.test_global
```

### Comparing `fedml-0.8.4a9/fedml/cheetah/server/server_initializer.py` & `fedml-0.8.5a1/fedml/cheetah/server/server_initializer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cheetah/fedml_client.py` & `fedml-0.8.5a1/fedml/cheetah/fedml_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cheetah/fedml_server.py` & `fedml-0.8.5a1/fedml/cheetah/fedml_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cheetah/client/client_initializer.py` & `fedml-0.8.5a1/fedml/cheetah/client/client_initializer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cheetah/client/client_launcher.py` & `fedml-0.8.5a1/fedml/cheetah/client/client_launcher.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cheetah/client/message_define.py` & `fedml-0.8.5a1/fedml/cheetah/client/message_define.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cheetah/client/fedml_trainer_dist_adapter.py` & `fedml-0.8.5a1/fedml/cheetah/client/fedml_trainer_dist_adapter.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cheetah/client/fedml_client_slave_manager.py` & `fedml-0.8.5a1/fedml/cheetah/client/fedml_client_slave_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cheetah/client/process_group_manager.py` & `fedml-0.8.5a1/fedml/cheetah/client/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cheetah/client/utils.py` & `fedml-0.8.5a1/fedml/cheetah/client/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/cheetah/client/fedml_client_master_manager.py` & `fedml-0.8.5a1/fedml/fa/cross_silo/client/fedml_client_master_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,32 @@
 import json
 import logging
 import platform
 import time
-
-import torch.distributed as dist
-
 from fedml import mlops
-from fedml.constants import FEDML_CROSS_SILO_SCENARIO_HIERARCHICAL
+from fedml.core import FedMLCommManager
+from fedml.core.distributed.communication.message import Message
+from fedml.core.mlops import MLOpsProfilerEvent
 from .message_define import MyMessage
-from .utils import convert_model_params_from_ddp, convert_model_params_to_ddp
-from ...core.distributed.fedml_comm_manager import FedMLCommManager
-from ...core.distributed.communication.message import Message
-from ...core.mlops.mlops_profiler_event import MLOpsProfilerEvent
+import torch.distributed as dist
 
 
 class ClientMasterManager(FedMLCommManager):
-    ONLINE_STATUS_FLAG = "ONLINE"
-    RUN_FINISHED_STATUS_FLAG = "FINISHED"
-
     def __init__(self, args, trainer_dist_adapter, comm=None, rank=0, size=0, backend="MPI"):
         super().__init__(args, comm, rank, size, backend)
         self.trainer_dist_adapter = trainer_dist_adapter
         self.args = args
-
         self.num_rounds = args.comm_round
         self.round_idx = 0
         self.rank = rank
         self.client_real_ids = json.loads(args.client_id_list)
         logging.info("self.client_real_ids = {}".format(self.client_real_ids))
         # for the client, len(self.client_real_ids)==1: we only specify its client id in the list, not including others.
         self.client_real_id = self.client_real_ids[0]
-
         self.has_sent_online_msg = False
-        self.is_inited = False
 
     def register_message_receive_handlers(self):
         self.register_message_receive_handler(
             MyMessage.MSG_TYPE_CONNECTION_IS_READY, self.handle_message_connection_ready
         )
 
         self.register_message_receive_handler(
@@ -59,98 +49,76 @@
 
             mlops.log_sys_perf(self.args)
 
     def handle_message_check_status(self, msg_params):
         self.send_client_status(0)
 
     def handle_message_init(self, msg_params):
-        if self.is_inited:
-            return
-
-        self.is_inited = True
-
         global_model_params = msg_params.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS)
         data_silo_index = msg_params.get(MyMessage.MSG_ARG_KEY_CLIENT_INDEX)
-
+        init_msg = msg_params.get(MyMessage.MSG_INIT_MSG_TO_CLIENTS)
         logging.info("data_silo_index = %s" % str(data_silo_index))
 
         # Notify MLOps with training status.
         self.report_training_status(MyMessage.MSG_MLOPS_CLIENT_STATUS_TRAINING)
 
-        if self.args.scenario == FEDML_CROSS_SILO_SCENARIO_HIERARCHICAL:
-            global_model_params = convert_model_params_to_ddp(global_model_params)
-            self.sync_process_group(0, global_model_params, data_silo_index)
-
         self.trainer_dist_adapter.update_dataset(int(data_silo_index))
-        self.trainer_dist_adapter.update_model(global_model_params)
+        self.trainer_dist_adapter.set_server_data(global_model_params)
+        self.trainer_dist_adapter.set_init_msg(init_msg)
         self.round_idx = 0
 
         self.__train()
         self.round_idx += 1
 
     def handle_message_receive_model_from_server(self, msg_params):
         logging.info("handle_message_receive_model_from_server.")
         model_params = msg_params.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS)
         client_index = msg_params.get(MyMessage.MSG_ARG_KEY_CLIENT_INDEX)
 
-        if self.args.scenario == FEDML_CROSS_SILO_SCENARIO_HIERARCHICAL:
-            model_params = convert_model_params_to_ddp(model_params)
-            self.sync_process_group(self.round_idx, model_params, client_index)
-
         self.trainer_dist_adapter.update_dataset(int(client_index))
         logging.info("current round index {}, total rounds {}".format(self.round_idx, self.num_rounds))
-        self.trainer_dist_adapter.update_model(model_params)
+        self.trainer_dist_adapter.set_server_data(model_params)
         if self.round_idx < self.num_rounds:
             self.__train()
             self.round_idx += 1
-        else:
-            self.send_client_status(0, ClientMasterManager.RUN_FINISHED_STATUS_FLAG)
-            mlops.log_training_finished_status()
-            self.finish()
 
     def handle_message_finish(self, msg_params):
         logging.info(" ====================cleanup ====================")
         self.cleanup()
 
     def cleanup(self):
-        self.send_client_status(0, ClientMasterManager.RUN_FINISHED_STATUS_FLAG)
-        mlops.log_training_finished_status()
         self.finish()
+        mlops.log_training_finished_status()
 
     def send_model_to_server(self, receive_id, weights, local_sample_num):
         tick = time.time()
         mlops.event("comm_c2s", event_started=True, event_value=str(self.round_idx))
         message = Message(MyMessage.MSG_TYPE_C2S_SEND_MODEL_TO_SERVER, self.client_real_id, receive_id,)
         message.add_params(MyMessage.MSG_ARG_KEY_MODEL_PARAMS, weights)
         message.add_params(MyMessage.MSG_ARG_KEY_NUM_SAMPLES, local_sample_num)
         self.send_message(message)
 
         MLOpsProfilerEvent.log_to_wandb({"Communication/Send_Total": time.time() - tick})
         mlops.log_client_model_info(
             self.round_idx+1, self.num_rounds, model_url=message.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_URL),
         )
 
-    def send_client_status(self, receive_id, status=ONLINE_STATUS_FLAG):
+    def send_client_status(self, receive_id, status="ONLINE"):
         logging.info("send_client_status")
         logging.info("self.client_real_id = {}".format(self.client_real_id))
         message = Message(MyMessage.MSG_TYPE_C2S_CLIENT_STATUS, self.client_real_id, receive_id)
         sys_name = platform.system()
         if sys_name == "Darwin":
             sys_name = "Mac"
         # Debug for simulation mobile system
         # sys_name = MyMessage.MSG_CLIENT_OS_ANDROID
 
         message.add_params(MyMessage.MSG_ARG_KEY_CLIENT_STATUS, status)
         message.add_params(MyMessage.MSG_ARG_KEY_CLIENT_OS, sys_name)
-
-        if hasattr(self.args, "using_mlops") and self.args.using_mlops and \
-                status == ClientMasterManager.RUN_FINISHED_STATUS_FLAG:
-            mlops.log_server_payload(self.args.run_id, self.client_real_id, json.dumps(message.get_params()))
-        else:
-            self.send_message(message)
+        self.send_message(message)
 
     def report_training_status(self, status):
         mlops.log_training_status(status)
 
     def sync_process_group(self, round_idx, model_params=None, client_index=None, src=0):
         logging.info("sending round number to pg")
         round_number = [round_idx, model_params, client_index]
@@ -160,19 +128,15 @@
         logging.info("round number %d broadcast to process group" % round_number[0])
 
     def __train(self):
         logging.info("#######training########### round_id = %d" % self.round_idx)
 
         mlops.event("train", event_started=True, event_value=str(self.round_idx))
 
-        weights, local_sample_num = self.trainer_dist_adapter.train(self.round_idx)
+        client_submission, local_sample_num = self.trainer_dist_adapter.local_analyze(self.round_idx)
 
         mlops.event("train", event_started=False, event_value=str(self.round_idx))
 
-        # the current model is still DDP-wrapped under cross-silo-hi setting
-        if self.args.scenario == FEDML_CROSS_SILO_SCENARIO_HIERARCHICAL:
-            weights = convert_model_params_from_ddp(weights)
-
-        self.send_model_to_server(0, weights, local_sample_num)
+        self.send_model_to_server(0, client_submission, local_sample_num)
 
     def run(self):
         super().run()
```

### Comparing `fedml-0.8.4a9/fedml/cheetah/client/fedml_trainer.py` & `fedml-0.8.5a1/fedml/cheetah/client/fedml_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/ml/aggregator/aggregator_creator.py` & `fedml-0.8.5a1/fedml/ml/aggregator/aggregator_creator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/ml/aggregator/my_server_aggregator_nwp.py` & `fedml-0.8.5a1/fedml/ml/aggregator/my_server_aggregator_nwp.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/ml/aggregator/default_aggregator.py` & `fedml-0.8.5a1/fedml/ml/aggregator/default_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/ml/aggregator/my_server_aggregator.py` & `fedml-0.8.5a1/fedml/ml/aggregator/my_server_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/ml/aggregator/my_server_aggregator_classification.py` & `fedml-0.8.5a1/fedml/ml/aggregator/my_server_aggregator_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/ml/aggregator/agg_operator.py` & `fedml-0.8.5a1/fedml/ml/aggregator/agg_operator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/ml/aggregator/my_server_aggregator_prediction.py` & `fedml-0.8.5a1/fedml/ml/aggregator/my_server_aggregator_prediction.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/ml/engine/ml_engine_adapter.py` & `fedml-0.8.5a1/fedml/ml/engine/ml_engine_adapter.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/ml/engine/torch_process_group_manager.py` & `fedml-0.8.5a1/fedml/ml/engine/torch_process_group_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/ml/trainer/scaffold_trainer.py` & `fedml-0.8.5a1/fedml/ml/trainer/scaffold_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/ml/trainer/trainer_creator.py` & `fedml-0.8.5a1/fedml/ml/trainer/trainer_creator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/ml/trainer/fednova_trainer.py` & `fedml-0.8.5a1/fedml/ml/trainer/fednova_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/ml/trainer/fedprox_trainer.py` & `fedml-0.8.5a1/fedml/ml/trainer/fedprox_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/ml/trainer/my_model_trainer_nwp.py` & `fedml-0.8.5a1/fedml/ml/trainer/my_model_trainer_nwp.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/ml/trainer/feddyn_trainer copy.py` & `fedml-0.8.5a1/fedml/ml/trainer/feddyn_trainer copy.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/ml/trainer/feddyn_trainer.py` & `fedml-0.8.5a1/fedml/ml/trainer/feddyn_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/ml/trainer/my_model_trainer.py` & `fedml-0.8.5a1/fedml/ml/trainer/my_model_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/ml/trainer/mime_trainer.py` & `fedml-0.8.5a1/fedml/ml/trainer/mime_trainer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/ml/trainer/my_model_trainer_tag_prediction.py` & `fedml-0.8.5a1/fedml/ml/trainer/my_model_trainer_tag_prediction.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/ml/trainer/my_model_trainer_classification.py` & `fedml-0.8.5a1/fedml/ml/trainer/my_model_trainer_classification.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/linear/lr_cifar10.py` & `fedml-0.8.5a1/fedml/model/linear/lr_cifar10.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/model_hub.py` & `fedml-0.8.5a1/fedml/model/model_hub.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/mobile/mnn_lenet.py` & `fedml-0.8.5a1/fedml/model/mobile/mnn_lenet.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/mobile/mnn_resnet.py` & `fedml-0.8.5a1/fedml/model/mobile/mnn_resnet.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/mobile/torch_lenet.py` & `fedml-0.8.5a1/fedml/model/mobile/torch_lenet.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/nlp/model_args.py` & `fedml-0.8.5a1/fedml/model/nlp/model_args.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/nlp/rnn.py` & `fedml-0.8.5a1/fedml/model/nlp/rnn.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/finance/vfl_models_standalone.py` & `fedml-0.8.5a1/fedml/model/finance/vfl_models_standalone.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/resnet56/resnet_pretrained.py` & `fedml-0.8.5a1/fedml/model/cv/resnet56/resnet_pretrained.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/resnet56/resnet_server.py` & `fedml-0.8.5a1/fedml/model/cv/resnet56/resnet_server.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/resnet56/resnet_client.py` & `fedml-0.8.5a1/fedml/model/cv/resnet56/resnet_client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/vgg.py` & `fedml-0.8.5a1/fedml/model/cv/vgg.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/resnet_torch.py` & `fedml-0.8.5a1/fedml/model/cv/resnet_torch.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/efficientnet_utils.py` & `fedml-0.8.5a1/fedml/model/cv/efficientnet_utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/resnet_cifar.py` & `fedml-0.8.5a1/fedml/model/cv/resnet_cifar.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/mobilenet_v3.py` & `fedml-0.8.5a1/fedml/model/cv/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/batchnorm_utils.py` & `fedml-0.8.5a1/fedml/model/cv/batchnorm_utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/cnn.py` & `fedml-0.8.5a1/fedml/model/cv/cnn.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/mnist_gan.py` & `fedml-0.8.5a1/fedml/model/cv/mnist_gan.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/efficientnet.py` & `fedml-0.8.5a1/fedml/model/cv/efficientnet.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/resnet_all.py` & `fedml-0.8.5a1/fedml/model/cv/resnet_all.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/mobilenet.py` & `fedml-0.8.5a1/fedml/model/cv/mobilenet.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/common.py` & `fedml-0.8.5a1/fedml/model/cv/common.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/resnet.py` & `fedml-0.8.5a1/fedml/model/cv/resnet.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/darts/model_search_gdas.py` & `fedml-0.8.5a1/fedml/model/cv/darts/model_search_gdas.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/darts/visualize.py` & `fedml-0.8.5a1/fedml/model/cv/darts/visualize.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/darts/architect.py` & `fedml-0.8.5a1/fedml/model/cv/darts/architect.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/darts/model.py` & `fedml-0.8.5a1/fedml/model/cv/darts/model.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/darts/operations.py` & `fedml-0.8.5a1/fedml/model/cv/darts/operations.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/darts/utils.py` & `fedml-0.8.5a1/fedml/model/cv/darts/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/darts/model_search.py` & `fedml-0.8.5a1/fedml/model/cv/darts/model_search.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/darts/train.py` & `fedml-0.8.5a1/fedml/model/cv/darts/train.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/darts/genotypes.py` & `fedml-0.8.5a1/fedml/model/cv/darts/genotypes.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/darts/train_search.py` & `fedml-0.8.5a1/fedml/model/cv/darts/train_search.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/resnet_gn.py` & `fedml-0.8.5a1/fedml/model/cv/resnet_gn.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/model/cv/group_normalization.py` & `fedml-0.8.5a1/fedml/model/cv/group_normalization.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/device/gpu_mapping_cross_silo.py` & `fedml-0.8.5a1/fedml/device/gpu_mapping_cross_silo.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/device/gpu_mapping_mpi.py` & `fedml-0.8.5a1/fedml/device/gpu_mapping_mpi.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/device/device.py` & `fedml-0.8.5a1/fedml/device/device.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/fa/runner.py` & `fedml-0.8.5a1/fedml/fa/runner.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,29 +28,21 @@
         if hasattr(args, "backend") and args.backend == FEDML_SIMULATION_TYPE_SP:
             runner = FASimulatorSingleProcess(args, dataset)
         else:
             raise Exception("not such backend {}".format(args.backend))
 
         return runner
 
-    def _init_cross_silo_runner(
-            self, args, dataset, client_analyzer=None, server_analyzer=None
-    ):
+    def _init_cross_silo_runner(self, args, dataset, client_analyzer=None, server_analyzer=None):
         if args.role == "client":
             from fedml.fa.cross_silo.fa_client import FACrossSiloClient as Client
-
-            runner = Client(
-                args, dataset, client_analyzer
-            )
+            runner = Client(args, dataset, client_analyzer)
         elif args.role == "server":
             from fedml.fa.cross_silo.fa_server import FACrossSiloServer as Server
-
-            runner = Server(
-                args, dataset, server_analyzer
-            )
+            runner = Server(args, dataset, server_analyzer)
         else:
             raise Exception("no such role")
 
         return runner
 
     def run(self):
         self.runner.run()
```

### Comparing `fedml-0.8.4a9/fedml/fa/cross_silo/fa_server.py` & `fedml-0.8.5a1/fedml/fa/cross_silo/fa_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,10 +16,9 @@
             args.worker_num,
             train_data_num,
             train_data_local_dict,
             train_data_local_num_dict,
             server_aggregator,
         )
 
-
     def run(self):
         pass
```

### Comparing `fedml-0.8.4a9/fedml/fa/cross_silo/fa_client.py` & `fedml-0.8.5a1/fedml/fa/cross_silo/fa_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,10 +16,9 @@
             args.worker_num,
             train_data_num,
             train_data_local_num_dict,
             train_data_local_dict,
             client_analyzer,
         )
 
-
     def run(self):
         pass
```

### Comparing `fedml-0.8.4a9/fedml/fa/cross_silo/server/message_define.py` & `fedml-0.8.5a1/fedml/fa/cross_silo/server/message_define.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     MSG_TYPE_CONNECTION_IS_READY = 0
 
     # server to client
     MSG_TYPE_S2C_INIT_CONFIG = 1
     MSG_TYPE_S2C_SYNC_MODEL_TO_CLIENT = 2
     MSG_TYPE_S2C_CHECK_CLIENT_STATUS = 6
     MSG_TYPE_S2C_FINISH = 7
+    MSG_INIT_MSG_TO_CLIENTS = "init_msg"
 
     # client to server
     MSG_TYPE_C2S_SEND_MODEL_TO_SERVER = 3
     MSG_TYPE_C2S_SEND_STATS_TO_SERVER = 4
     MSG_TYPE_C2S_CLIENT_STATUS = 5
 
     MSG_ARG_KEY_TYPE = "msg_type"
@@ -26,14 +27,15 @@
     """
     MSG_ARG_KEY_NUM_SAMPLES = "num_samples"
     MSG_ARG_KEY_MODEL_PARAMS = "model_params"
     MSG_ARG_KEY_MODEL_PARAMS_URL = "model_params_url"
     MSG_ARG_KEY_MODEL_PARAMS_KEY = "model_params_key"
     MSG_ARG_KEY_CLIENT_INDEX = "client_idx"
 
+
     MSG_ARG_KEY_TRAIN_CORRECT = "train_correct"
     MSG_ARG_KEY_TRAIN_ERROR = "train_error"
     MSG_ARG_KEY_TRAIN_NUM = "train_num_sample"
 
     MSG_ARG_KEY_TEST_CORRECT = "test_correct"
     MSG_ARG_KEY_TEST_ERROR = "test_error"
     MSG_ARG_KEY_TEST_NUM = "test_num_sample"
```

### Comparing `fedml-0.8.4a9/fedml/fa/cross_silo/server/fedml_server_manager.py` & `fedml-0.8.5a1/fedml/fa/cross_silo/server/fedml_server_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,36 +13,34 @@
             self, args, aggregator, comm=None, client_rank=0, client_num=0, backend="MQTT_S3",
     ):
         super().__init__(args, comm, client_rank, client_num, backend)
         self.args = args
         self.aggregator = aggregator
         self.round_num = args.comm_round
         self.args.round_idx = 0
-
         self.client_online_mapping = {}
         self.client_real_ids = json.loads(args.client_id_list)
-
         self.is_initialized = False
         self.client_id_list_in_this_round = None
         self.data_silo_index_list = None
 
     def run(self):
         super().run()
 
     def send_init_msg(self):
-        global_model_params = self.aggregator.get_server_data()
+        global_result = self.aggregator.get_server_data()
 
-        global_model_url = None
-        global_model_key = None
+        global_result_url = None
+        global_result_key = None
 
         client_idx_in_this_round = 0
         for client_id in self.client_id_list_in_this_round:
-            global_model_url, global_model_key = self.send_message_init_config(
-                client_id, global_model_params, self.data_silo_index_list[client_idx_in_this_round],
-                global_model_url, global_model_key
+            global_result_url, global_result_key = self.send_message_init_config(
+                client_id, global_result, self.data_silo_index_list[client_idx_in_this_round],
+                global_result_url, global_result_key
             )
             client_idx_in_this_round += 1
 
         mlops.event("server.wait", event_started=True, event_value=str(self.args.round_idx))
 
     def register_message_receive_handlers(self):
         logging.info("register_message_receive_handlers------")
@@ -66,34 +64,30 @@
             self.data_silo_index_list = self.aggregator.data_silo_selection(
                 self.args.round_idx, self.args.client_num_in_total, len(self.client_id_list_in_this_round),
             )
 
             mlops.log_round_info(self.round_num, -1)
 
             # check client status in case that some clients start earlier than the server
-            client_idx_in_this_round = 0
+            client_idx_this_round = 0
             for client_id in self.client_id_list_in_this_round:
                 try:
-                    self.send_message_check_client_status(
-                        client_id, self.data_silo_index_list[client_idx_in_this_round],
-                    )
+                    self.send_message_check_client_status(client_id, self.data_silo_index_list[client_idx_this_round])
                     logging.info("Connection ready for client" + str(client_id))
                 except Exception as e:
                     logging.info("Connection not ready for client" + str(client_id))
-                client_idx_in_this_round += 1
+                client_idx_this_round += 1
 
     def handle_message_client_status_update(self, msg_params):
         client_status = msg_params.get(MyMessage.MSG_ARG_KEY_CLIENT_STATUS)
         if client_status == "ONLINE":
             self.client_online_mapping[str(msg_params.get_sender_id())] = True
-
             logging.info("self.client_online_mapping = {}".format(self.client_online_mapping))
 
         mlops.log_aggregation_status(MyMessage.MSG_MLOPS_SERVER_STATUS_RUNNING)
-
         all_client_is_online = True
         for client_id in self.client_id_list_in_this_round:
             if not self.client_online_mapping.get(str(client_id), False):
                 all_client_is_online = False
                 break
 
         logging.info(
@@ -104,33 +98,30 @@
             # send initialization message to all clients to start training
             self.send_init_msg()
             self.is_initialized = True
 
     def handle_message_receive_model_from_client(self, msg_params):
         sender_id = msg_params.get(MyMessage.MSG_ARG_KEY_SENDER)
         mlops.event("comm_c2s", event_started=False, event_value=str(self.args.round_idx), event_edge_id=sender_id)
-
-        model_params = msg_params.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS)
+        local_results = msg_params.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS)
         local_sample_number = msg_params.get(MyMessage.MSG_ARG_KEY_NUM_SAMPLES)
 
         self.aggregator.add_local_trained_result(
-            self.client_real_ids.index(sender_id), model_params, local_sample_number
+            self.client_real_ids.index(sender_id), local_results, local_sample_number
         )
         b_all_received = self.aggregator.check_whether_all_receive()
         logging.info("b_all_received = " + str(b_all_received))
         if b_all_received:
             mlops.event("server.wait", event_started=False, event_value=str(self.args.round_idx))
             mlops.event("server.agg_and_eval", event_started=True, event_value=str(self.args.round_idx))
             tick = time.time()
-            global_model_params, model_list = self.aggregator.aggregate()
+            global_result, _ = self.aggregator.aggregate()
 
             logging.info("self.client_id_list_in_this_round = {}".format(self.client_id_list_in_this_round))
-
             MLOpsProfilerEvent.log_to_wandb({"AggregationTime": time.time() - tick, "round": self.args.round_idx})
-
             mlops.event("server.agg_and_eval", event_started=False, event_value=str(self.args.round_idx))
 
             # send round info to the MQTT backend
             mlops.log_round_info(self.round_num, self.args.round_idx)
 
             self.client_id_list_in_this_round = self.aggregator.client_selection(
                 self.args.round_idx, self.client_real_ids, self.args.client_num_per_round
@@ -141,36 +132,33 @@
 
             Context().add(Context.KEY_CLIENT_ID_LIST_IN_THIS_ROUND, self.client_id_list_in_this_round)
 
             if self.args.round_idx == 0:
                 MLOpsProfilerEvent.log_to_wandb({"BenchmarkStart": time.time()})
 
             client_idx_in_this_round = 0
-            global_model_url = None
-            global_model_key = None
-            # todo: add cases when no need to send global model with clients
+            global_result_url = None
+            global_result_key = None
             for receiver_id in self.client_id_list_in_this_round:
                 client_index = self.data_silo_index_list[client_idx_in_this_round]
-                global_model_url, global_model_key = self.send_message_sync_model_to_client(
-                    receiver_id, global_model_params, client_index, global_model_url,
-                    global_model_key
+                global_result_url, global_result_key = self.send_message_sync_model_to_client(
+                    receiver_id, global_result, client_index, global_result_url, global_result_key
                 )
                 client_idx_in_this_round += 1
 
             self.args.round_idx += 1
-            mlops.log_aggregated_model_info(
-                self.args.round_idx, model_url=global_model_url,
-                )
-
-            logging.info("\n\n==========end {}-th round training===========\n".format(self.args.round_idx))
+            mlops.log_aggregated_model_info(self.args.round_idx, model_url=global_result_url)
+            logging.info("\n\n==========end {}-th round analyzing===========\n".format(self.args.round_idx))
             mlops.event("server.wait", event_started=True, event_value=str(self.args.round_idx))
 
             if self.args.round_idx == self.round_num:
-                logging.info("=============training is finished. Cleanup...============")
+                logging.info("=============analyzing is finished. Cleanup...============")
                 self.cleanup()
+        if self.aggregator.get_init_msg() is not None:
+            self.aggregator.set_init_msg(init_msg=None)
 
     def cleanup(self):
         client_idx_in_this_round = 0
         for client_id in self.client_id_list_in_this_round:
             self.send_message_finish(
                 client_id, self.data_silo_index_list[client_idx_in_this_round],
             )
@@ -183,14 +171,16 @@
                                  global_model_url=None, global_model_key=None):
         tick = time.time()
         message = Message(MyMessage.MSG_TYPE_S2C_INIT_CONFIG, self.get_sender_id(), receive_id)
         if global_model_url is not None:
             message.add_params(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_URL, global_model_url)
         if global_model_key is not None:
             message.add_params(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_KEY, global_model_key)
+        if self.aggregator.get_init_msg() is not None:
+            message.add_params(MyMessage.MSG_INIT_MSG_TO_CLIENTS, self.aggregator.get_init_msg())
         message.add_params(MyMessage.MSG_ARG_KEY_MODEL_PARAMS, global_model_params)
         message.add_params(MyMessage.MSG_ARG_KEY_CLIENT_INDEX, str(datasilo_index))
         message.add_params(MyMessage.MSG_ARG_KEY_CLIENT_OS, "PythonClient")
         self.send_message(message)
         global_model_url = message.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_URL)
         global_model_key = message.get(MyMessage.MSG_ARG_KEY_MODEL_PARAMS_KEY)
         MLOpsProfilerEvent.log_to_wandb({"Communiaction/Send_Total": time.time() - tick})
```

### Comparing `fedml-0.8.4a9/fedml/fa/cross_silo/server/fedml_aggregator.py` & `fedml-0.8.5a1/fedml/fa/cross_silo/server/fedml_aggregator.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,27 +11,31 @@
         train_data_local_dict,
         train_data_local_num_dict,
         client_num,
         args,
         server_aggregator,
     ):
         self.aggregator = server_aggregator
-
         self.args = args
         self.all_train_data_num = all_train_data_num
         self.train_data_local_dict = train_data_local_dict
         self.train_data_local_num_dict = train_data_local_num_dict
-
         self.client_num = client_num
         self.model_dict = dict()
         self.sample_num_dict = dict()
         self.flag_client_model_uploaded_dict = dict()
         for idx in range(self.client_num):
             self.flag_client_model_uploaded_dict[idx] = False
 
+    def get_init_msg(self):
+        return self.aggregator.get_init_msg()
+
+    def set_init_msg(self, init_msg):
+        self.aggregator.set_init_msg(init_msg)
+
     def get_server_data(self):
         return self.aggregator.get_server_data()
 
     def set_server_data(self, server_data):
         self.aggregator.set_server_data(server_data)
 
     def add_local_trained_result(self, index, model_params, sample_num):
@@ -48,33 +52,28 @@
         for idx in range(self.client_num):
             self.flag_client_model_uploaded_dict[idx] = False
         return True
 
     def aggregate(self):
         start_time = time.time()
 
-        model_list = []
+        local_result_list = []
         for idx in range(self.client_num):
-            model_list.append((self.sample_num_dict[idx], self.model_dict[idx]))
-        # model_list is the list after outlier removal
-        Context().add(Context.KEY_CLIENT_MODEL_LIST, model_list)
-
-        averaged_params = self.aggregator.aggregate(model_list)
-
-        self.set_server_data(averaged_params)
+            local_result_list.append((self.sample_num_dict[idx], self.model_dict[idx]))
+        Context().add(Context.KEY_CLIENT_MODEL_LIST, local_result_list)
+        global_result = self.aggregator.aggregate(local_result_list)
+        self.set_server_data(global_result)
 
         end_time = time.time()
-        logging.info(f"aggregation result = {averaged_params}")
+        logging.info(f"aggregation result = {global_result}")
         logging.info("aggregate time cost: %d" % (end_time - start_time))
-        return averaged_params, model_list
-
+        return global_result, local_result_list
 
     def data_silo_selection(self, round_idx, client_num_in_total, client_num_per_round):
         """
-
         Args:
             round_idx: round index, starting from 0
             client_num_in_total: this is equal to the users in a synthetic data,
                                     e.g., in synthetic_1_1, this value is 30
             client_num_per_round: the number of edge devices that can train
 
         Returns:
```

### Comparing `fedml-0.8.4a9/fedml/fa/cross_silo/server/server_initializer.py` & `fedml-0.8.5a1/fedml/fa/cross_silo/server/server_initializer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/fa/cross_silo/client/client_initializer.py` & `fedml-0.8.5a1/fedml/fa/cross_silo/client/client_initializer.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/fa/cross_silo/client/client_launcher.py` & `fedml-0.8.5a1/fedml/fa/cross_silo/client/client_launcher.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/fa/cross_silo/client/message_define.py` & `fedml-0.8.5a1/fedml/fa/cross_silo/client/message_define.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     MSG_TYPE_CONNECTION_IS_READY = 0
 
     # server to client
     MSG_TYPE_S2C_INIT_CONFIG = 1
     MSG_TYPE_S2C_SYNC_MODEL_TO_CLIENT = 2
     MSG_TYPE_S2C_CHECK_CLIENT_STATUS = 6
     MSG_TYPE_S2C_FINISH = 7
+    MSG_INIT_MSG_TO_CLIENTS = "init_msg"
 
     # client to server
     MSG_TYPE_C2S_SEND_MODEL_TO_SERVER = 3
     MSG_TYPE_C2S_SEND_STATS_TO_SERVER = 4
     MSG_TYPE_C2S_CLIENT_STATUS = 5
 
     MSG_ARG_KEY_TYPE = "msg_type"
```

### Comparing `fedml-0.8.4a9/fedml/fa/cross_silo/client/fa_local_analyzer.py` & `fedml-0.8.5a1/fedml/fa/cross_silo/client/fa_local_analyzer.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,14 +17,21 @@
         self.train_data_local_dict = train_data_local_dict
         self.train_data_local_num_dict = train_data_local_num_dict
         self.all_train_data_num = train_data_num
         self.train_local = None
         self.local_sample_number = None
         self.test_local = None
         self.args = args
+        self.init_msg = None
+
+    def set_init_msg(self, init_msg):
+        self.local_analyzer.set_init_msg(init_msg)
+
+    def get_init_msg(self):
+        return self.local_analyzer.get_init_msg()
 
     def set_server_data(self, server_data):
         self.local_analyzer.set_server_data(server_data)
 
     def set_client_submission(self, client_submission):
         self.local_analyzer.set_client_submission(client_submission)
```

### Comparing `fedml-0.8.4a9/fedml/fa/cross_silo/client/fedml_trainer_dist_adapter.py` & `fedml-0.8.5a1/fedml/fa/cross_silo/client/fedml_trainer_dist_adapter.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,13 +54,16 @@
     def local_analyze(self, round_idx):
         client_submission, local_sample_num = self.local_analyzer.local_analyze(round_idx)
         return client_submission, local_sample_num
 
     def set_server_data(self, server_data):
         self.local_analyzer.set_server_data(server_data)
 
+    def set_init_msg(self, init_msg):
+        self.local_analyzer.set_init_msg(init_msg)
+
     def set_client_submission(self, client_submission):
         self.local_analyzer.set_client_submission(client_submission)
 
     def update_dataset(self, client_index=None):
         _client_index = client_index or self.client_index
         self.local_analyzer.update_dataset(int(_client_index))
```

### Comparing `fedml-0.8.4a9/fedml/fa/cross_silo/client/fedml_client_slave_manager.py` & `fedml-0.8.5a1/fedml/fa/cross_silo/client/fedml_client_slave_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/fa/cross_silo/client/process_group_manager.py` & `fedml-0.8.5a1/fedml/fa/cross_silo/client/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/fa/aggregator/frequency_estimation_aggregator.py` & `fedml-0.8.5a1/fedml/fa/aggregator/frequency_estimation_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/fa/aggregator/intersection_aggregator.py` & `fedml-0.8.5a1/fedml/fa/aggregator/intersection_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/fa/aggregator/union_aggregator.py` & `fedml-0.8.5a1/fedml/fa/aggregator/union_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/fa/aggregator/avg_aggregator.py` & `fedml-0.8.5a1/fedml/fa/aggregator/avg_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/fa/aggregator/k_percentile_element_aggregator.py` & `fedml-0.8.5a1/fedml/fa/aggregator/k_percentile_element_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/fa/aggregator/global_analyzer_creator.py` & `fedml-0.8.5a1/fedml/fa/aggregator/global_analyzer_creator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from fedml.fa.aggregator.avg_aggregator import AVGAggregatorFA
 from fedml.fa.aggregator.frequency_estimation_aggregator import FrequencyEstimationAggregatorFA
+from fedml.fa.aggregator.heavy_hitter_triehh_aggregator import HeavyHitterTriehhAggregatorFA
 from fedml.fa.aggregator.intersection_aggregator import IntersectionAggregatorFA
 from fedml.fa.aggregator.k_percentile_element_aggregator import KPercentileElementAggregatorFA
 from fedml.fa.aggregator.union_aggregator import UnionAggregatorFA
 from fedml.fa.constants import FA_TASK_AVG, FA_TASK_INTERSECTION, FA_TASK_CARDINALITY, FA_TASK_HISTOGRAM, FA_TASK_FREQ, \
-    FA_TASK_UNION, FA_TASK_K_PERCENTILE_ELEMENT
+    FA_TASK_UNION, FA_TASK_K_PERCENTILE_ELEMENT, FA_TASK_HEAVY_HITTER_TRIEHH
 
 
 def create_global_analyzer(args, train_data_num):
     task_type = args.fa_task
     if task_type == FA_TASK_AVG:
         return AVGAggregatorFA(args)
     if task_type == FA_TASK_INTERSECTION or task_type == FA_TASK_CARDINALITY:
         return IntersectionAggregatorFA(args)
     if task_type == FA_TASK_FREQ or task_type == FA_TASK_HISTOGRAM:
         return FrequencyEstimationAggregatorFA(args)
     if task_type == FA_TASK_UNION:
         return UnionAggregatorFA(args)
     if task_type == FA_TASK_K_PERCENTILE_ELEMENT:
         return KPercentileElementAggregatorFA(args, train_data_num)
+    if task_type == FA_TASK_HEAVY_HITTER_TRIEHH:
+        return HeavyHitterTriehhAggregatorFA(args, train_data_num)
```

### Comparing `fedml-0.8.4a9/fedml/fa/simulation/sp/client.py` & `fedml-0.8.5a1/fedml/fa/simulation/sp/client.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/fa/simulation/utils.py` & `fedml-0.8.5a1/fedml/fa/simulation/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/fa/__init__.py` & `fedml-0.8.5a1/fedml/fa/__init__.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/fa/local_analyzer/heavy_hitter_triehh.py` & `fedml-0.8.5a1/fedml/fa/data/twitter_Sentiment140/twitter_data_processing.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,67 +3,26 @@
 """
 import collections
 import csv
 import operator
 import os
 import pickle
 import re
-import numpy as np
 
 
 def is_valid(word):
     if len(word) < 3 or (word[-1] in [
         '?', '!', '.', ';', ','
     ]) or word.startswith('http') or word.startswith('www'):
         return False
     if re.match(r'^[a-z_\@\#\-\;\(\)\*\:\.\'\/]+$', word):
         return True
     return False
 
 
-def get_clients(filename, dictionary):
-    # import dict_trie
-    """Returns a dictionary of dictionaries containing per client word frequencies."""
-
-    # read dictionary file
-    vocab = Trie()
-    # with open(dictionary, 'r') as f:
-    #     content = f.readlines()
-    #     for x in content:
-    #         vocab.add(x.strip().lower())
-
-    clients = {}
-    with open(filename, encoding='ISO-8859-1') as csv_file:
-        csv_reader = csv.reader(csv_file, delimiter=',')
-        for row in csv_reader:
-            client = row[4]
-            comment = row[5]
-
-            raw_words = comment.lower().split()
-            raw_words = [word.strip(',.;?!') for word in raw_words]
-            raw_words = [x for x in raw_words if is_valid(x)]
-            words = [x for x in raw_words if not vocab.has_prefix(x)]
-
-            # don't create client if he/she has no valid words
-            word_len = len(words)
-            if word_len > 0 and client not in clients:
-                clients[client] = {}
-            for word in words:
-                if word not in clients[client]:
-                    clients[client][word] = 1
-                else:
-                    clients[client][word] += 1
-    # change word counts to percentages
-    for client in clients:
-        num_words = sum(clients[client].values())
-        for word in clients[client]:
-            clients[client][word] = clients[client][word] * 1.0 / num_words
-    return clients
-
-
 def truncate_or_extend(word, max_word_len):
     if len(word) > max_word_len:
         word = word[:max_word_len]
     else:
         word += '$' * (max_word_len - len(word))
     return word
 
@@ -80,63 +39,60 @@
         word_freq[word] += 1
     word_freq = dict(word_freq)
     file_path = os.path.join(path, 'clients_triehh.txt')
     with open(file_path, 'wb') as fp:
         pickle.dump(triehh_clients, fp)
 
 
-def generate_sfp_clients(clients, max_word_len):
-    """Generate sfp clients.
-  Args:
-    clients: input clients.
-    max_word_len: maximum word length.
-  """
-    clients_num = len(clients)
-    sfp_clients = [
-        truncate_or_extend(clients[i], max_word_len) for i in range(clients_num)
-    ]
-    word_freq = collections.defaultdict(lambda: 0)
-    for word in sfp_clients:
-        word_freq[word] += 1
-    word_freq = dict(word_freq)
-    with open('clients_sfp.txt', 'wb') as fp:
-        pickle.dump(sfp_clients, fp)
+def preprocess_twitter_data(path):
+    filename = os.path.join(path, 'training.1600000.processed.noemoticon.csv')
+    dataset = {}
+    with open(filename, encoding='ISO-8859-1') as csv_file:
+        csv_reader = csv.reader(csv_file, delimiter=',')
+        for row in csv_reader:
+            if len(row) >= 6:
+                client = row[4]
+                comment = row[5]
+
+                raw_words = comment.lower().split()
+                raw_words = [word.strip(',.;?!') for word in raw_words]
+                words = [x for x in raw_words if is_valid(x)]
+
+                word_len = len(words)
+                if word_len > 0:
+                    if client not in dataset:
+                        dataset[client] = list()
+                    dataset[client].extend(words)
+    return dataset
 
 
-def preprocess_twitter_data(path):  # todo: remove @ at the beginning of the words
+def preprocess_twitter_data_heavy_hitter(path):
     # load dataset from csv file
     filename = os.path.join(path, 'training.1600000.processed.noemoticon.csv')
+    clients = {}
+    with open(filename, encoding='ISO-8859-1') as csv_file:
+        csv_reader = csv.reader(csv_file, delimiter=',')
+        for row in csv_reader:
+            if len(row) >= 6:
+                client = row[4]
+                comment = row[5]
+
+                raw_words = comment.lower().split()
+                raw_words = [word.strip(',.;?!') for word in raw_words]
+                words = [x for x in raw_words if is_valid(x)]
+
+                # don't create client if he/she has no valid words
+                word_len = len(words)
+                if word_len > 0 and client not in clients:
+                    clients[client] = {}
+                for word in words:
+                    if word not in clients[client]:
+                        clients[client][word] = 1
+                    else:
+                        clients[client][word] += 1
 
-    # load dictionary
-    # please provide your own dictionary if you would like to
-    # run out-of-vocabulary experiments
-    dictionary = os.path.join(path, 'dictionary.txt')
-    max_word_len = 10 # maximum word length
-    clients = get_clients(filename, dictionary)
-
-    clients_top_word = []
-    top_word_counts = {}
     # get the top word for every client
+    local_datasets_top_word = {}
     for client in clients:
         top_word = max(clients[client].items(), key=operator.itemgetter(1))[0]
-        clients_top_word.append(top_word)
-        if top_word not in top_word_counts:
-            top_word_counts[top_word] = 1
-        else:
-            top_word_counts[top_word] += 1
-
-    # compute frequencies of top words
-    top_word_frequencies = {}
-    sum_num = sum(top_word_counts.values())
-    for word in top_word_counts:
-        top_word_frequencies[word] = top_word_counts[word] * 1.0 / sum_num
-
-    clients_top_word = np.array(clients_top_word)
-    freq_file = path + 'word_frequencies.txt'
-    with open(freq_file, 'wb') as fp:
-        pickle.dump(top_word_frequencies, fp)
-
-    generate_sfp_clients(clients_top_word, max_word_len)
-    generate_triehh_clients(clients_top_word, path=path)
-
-    print('client count:', len(clients_top_word))
-    print('top word count:', len(top_word_counts))
+        local_datasets_top_word[client] = add_end_symbol(top_word)
+    return local_datasets_top_word
```

### Comparing `fedml-0.8.4a9/fedml/fa/local_analyzer/client_analyzer_creator.py` & `fedml-0.8.5a1/fedml/fa/local_analyzer/client_analyzer_creator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from fedml.fa.constants import FA_TASK_AVG, FA_TASK_HEAVY_HITTER_TRIEHH, FA_TASK_UNION, FA_TASK_K_PERCENTILE_ELEMENT, \
     FA_TASK_INTERSECTION, FA_TASK_CARDINALITY, FA_TASK_HISTOGRAM, FA_TASK_FREQ
 from fedml.fa.local_analyzer.avg import AverageClientAnalyzer
 from fedml.fa.local_analyzer.frequency_estimation import FrequencyEstimationClientAnalyzer
+from fedml.fa.local_analyzer.heavy_hitter_triehh import TrieHHClientAnalyzer
 from fedml.fa.local_analyzer.intersection import IntersectionClientAnalyzer
 from fedml.fa.local_analyzer.k_percentage_element import KPercentileElementClientAnalyzer
 from fedml.fa.local_analyzer.union import UnionClientAnalyzer
 
 
 def create_local_analyzer(args):
     task_type = args.fa_task
@@ -17,8 +18,10 @@
         return UnionClientAnalyzer(args)
     if task_type == FA_TASK_K_PERCENTILE_ELEMENT:
         return KPercentileElementClientAnalyzer(args)
     if task_type == FA_TASK_INTERSECTION or task_type == FA_TASK_CARDINALITY:
         return IntersectionClientAnalyzer(args)
     if task_type == FA_TASK_FREQ or task_type == FA_TASK_HISTOGRAM:
         return FrequencyEstimationClientAnalyzer(args)
+    if task_type == FA_TASK_HEAVY_HITTER_TRIEHH:
+        return TrieHHClientAnalyzer(args)
```

### Comparing `fedml-0.8.4a9/fedml/fa/base_frame/server_aggregator.py` & `fedml-0.8.5a1/fedml/fa/base_frame/server_aggregator.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 
 class FAServerAggregator(ABC):
     def __init__(self, args):
         self.id = 0
         self.args = args
         self.eval_data = None
         self.server_data = None
+        self.init_msg = None
+
+    def get_init_msg(self):
+        # return self.init_msg
+        pass
+
+    def set_init_msg(self, init_msg):
+        # self.init_msg = init_msg
+        pass
 
     def set_id(self, aggregator_id):
         self.id = aggregator_id
 
     def get_server_data(self):
         return self.server_data
```

### Comparing `fedml-0.8.4a9/fedml/fa/base_frame/client_analyzer.py` & `fedml-0.8.5a1/fedml/fa/base_frame/client_analyzer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,25 @@
+import logging
 from abc import ABC, abstractmethod
 
 
 class FAClientAnalyzer(ABC):
     def __init__(self, args):
         self.client_submission = 0
         self.id = 0
         self.args = args
         self.local_train_dataset = None
         self.server_data = None
+        self.init_msg = None
+
+    def set_init_msg(self, init_msg):
+        pass
+
+    def get_init_msg(self):
+        pass
 
     def set_id(self, analyzer_id):
         self.id = analyzer_id
 
     def get_client_submission(self):
         return self.client_submission
```

### Comparing `fedml-0.8.4a9/fedml/fa/data/data_loader.py` & `fedml-0.8.5a1/fedml/fa/data/data_loader.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import argparse
 import logging
 import os
-
+from fedml.fa.constants import FA_TASK_HEAVY_HITTER_TRIEHH
 from fedml.fa.data.fake_numeric_data.data_loader import generate_fake_data, load_partition_data_fake
+from fedml.fa.data.self_defined_data.data_loader import load_partition_self_defined_data
 from fedml.fa.data.twitter_Sentiment140.data_loader import download_twitter_Sentiment140, \
-    load_partition_data_twitter_sentiment140
+    load_partition_data_twitter_sentiment140, load_partition_data_twitter_sentiment140_heavy_hitter
+from fedml.fa.data.twitter_Sentiment140.twitter_data_processing import preprocess_twitter_data, \
+    preprocess_twitter_data_heavy_hitter
 
 
 def fa_load_data(args):
     return load_synthetic_data(args)
 
 
 def load_synthetic_data(args):
     dataset_name = args.dataset
     if dataset_name == "fake":
         data_cache_dir = os.path.join(args.data_cache_dir, "fake_numeric_data")
         if not os.path.exists(data_cache_dir):
             os.makedirs(data_cache_dir)
-        print(f"---data_cache_dir={data_cache_dir}")
         generate_fake_data(data_cache_dir)
         logging.info("load_data. dataset_name = %s" % dataset_name)
         (
             datasize,
             train_data_local_num_dict,
             local_data_dict,
         ) = load_partition_data_fake(data_dir=data_cache_dir, client_num=int(args.client_num_in_total))
@@ -31,27 +33,64 @@
             train_data_local_num_dict,
             local_data_dict,
         ]
         # print(f"datasize, train_data_local_num_dict, local_data_dict,{dataset}")
     elif dataset_name == "twitter":
         path = os.path.join(args.data_cache_dir, "twitter_Sentiment140")
         download_twitter_Sentiment140(data_cache_dir=path)
-        # preprocess_twitter_data(path=path)
-        (
-            datasize,
-            train_data_local_num_dict,
-            local_data_dict,
-        ) = load_partition_data_twitter_sentiment140(data_dir=path, client_num_in_total=int(args.client_num_in_total))
+        if args.fa_task != FA_TASK_HEAVY_HITTER_TRIEHH:
+            local_datasets = preprocess_twitter_data(path=path)
+            (
+                datasize,
+                train_data_local_num_dict,
+                local_data_dict,
+            ) = load_partition_data_twitter_sentiment140(local_datasets, client_num_in_total=int(args.client_num_in_total))
+
+            dataset = [
+                datasize,
+                train_data_local_num_dict,
+                local_data_dict,
+            ]
+        else:
+            local_datasets = preprocess_twitter_data_heavy_hitter(path=path)
+            (
+                datasize,
+                train_data_local_num_dict,
+                local_data_dict,
+            ) = load_partition_data_twitter_sentiment140_heavy_hitter(local_datasets, int(args.client_num_in_total))
+            dataset = [
+                datasize,
+                train_data_local_num_dict,
+                local_data_dict,
+            ]
+    elif dataset_name == "self_defined":
+        data_cache_dir = args.data_cache_dir
+        if not os.path.exists(data_cache_dir):
+            os.makedirs(data_cache_dir)
+        if hasattr(args, "data_col_idx") and isinstance(args.data_col_idx, int) and args.data_col_idx >= 0:
+            if hasattr(args, "seperator"):
+                separator = args.seperator
+            else:
+                separator = ","  # default seperator = ","
+            (
+                datasize,
+                train_data_local_num_dict,
+                local_data_dict,
+            ) = load_partition_self_defined_data(file_folder_path=data_cache_dir,
+                                                 client_num=int(args.client_num_in_total),
+                                                 data_col_idx=int(args.data_col_idx),
+                                                 separator=separator)
+            dataset = [
+                datasize,
+                train_data_local_num_dict,
+                local_data_dict,
+            ]
 
-        dataset = [
-            datasize,
-            train_data_local_num_dict,
-            local_data_dict,
-        ]
-        print(f"datasize, train_data_local_num_dict, local_data_dict,{dataset}")
+        else:
+            raise Exception("illegal data column index (data_col_idx) in the data file(s)")
     else:
         raise "Not Implemented Error"
     return dataset
 
 
 def load_synthetic_data_test():
     parser = argparse.ArgumentParser(description="FedML")
```

### Comparing `fedml-0.8.4a9/fedml/fa/data/utils.py` & `fedml-0.8.5a1/fedml/fa/data/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import math
 import os
 
 
 def equally_partition_a_dataset(client_num_in_total, dataset):
     client_data_num = int(len(dataset) / client_num_in_total)
     local_data_dict = dict()
     train_data_local_num_dict = dict()
@@ -14,17 +15,55 @@
     return (
         datasize,
         train_data_local_num_dict,
         local_data_dict,
     )
 
 
+def equally_partition_a_dataset_according_to_users(client_num_in_total, dataset):
+    user_num_for_one_client = int(math.ceil(len(dataset) / client_num_in_total))
+    local_data_dict = dict()
+    train_data_local_num_dict = dict()
+    datasize = 0
+    user_list = list(dataset.keys())
+    user_list_counter = 0
+    for i in range(client_num_in_total):
+        local_data_dict[i] = list()
+        client_data_num = 0
+        for j in range(user_num_for_one_client):
+            if user_list_counter >= len(user_list):
+                break
+            local_data_dict[i].extend(dataset[user_list[user_list_counter]])
+            client_data_num += len(dataset[user_list[user_list_counter]])
+            user_list_counter += 1
+        train_data_local_num_dict[i] = client_data_num
+        datasize += train_data_local_num_dict[i]
+    return (
+        datasize,
+        train_data_local_num_dict,
+        local_data_dict,
+    )
+
+
 def read_data(data_dir):
     train_files = os.listdir(data_dir)
     train_files = [f for f in train_files if f.endswith(".txt")]
     dataset = []
     for f in train_files:
         file_path = os.path.join(data_dir, f)
         f2 = open(file_path, "r")
         lines = [int(line.strip()) for line in f2]
         dataset.extend(lines)
     return dataset
+
+
+def read_data_with_column_idx(file_folder_path, column_idx, seperator=","):
+    train_files = os.listdir(file_folder_path)
+    train_files = [f for f in train_files if not f.startswith(".")]
+    dataset = []
+    for f in train_files:
+        file_path = os.path.join(file_folder_path, f)
+        f2 = open(file_path, "r")
+        for line in f2:
+            if len(line.split(seperator)[column_idx].strip()) > 0:
+                dataset.append(line.split(seperator)[column_idx].strip())
+    return dataset
```

### Comparing `fedml-0.8.4a9/fedml/fa/data/fake_numeric_data/data_loader.py` & `fedml-0.8.5a1/fedml/fa/data/fake_numeric_data/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/launch_cross_device.py` & `fedml-0.8.5a1/fedml/launch_cross_device.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/MNIST/mnist_mobile_preprocessor.py` & `fedml-0.8.5a1/fedml/data/MNIST/mnist_mobile_preprocessor.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/MNIST/data_loader.py` & `fedml-0.8.5a1/fedml/data/MNIST/data_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,18 @@
     file_path = os.path.join(data_cache_dir, "MNIST.zip")
     logging.info(file_path)
 
     # Download the file (if we haven't already)
     if not os.path.exists(file_path):
         wget.download(FEDML_DATA_MNIST_URL, out=file_path)
 
-    with zipfile.ZipFile(file_path, "r") as zip_ref:
-        zip_ref.extractall(data_cache_dir)
-
+    file_extracted_path = os.path.join(data_cache_dir, "MNIST")
+    if not os.path.exists(file_extracted_path):
+        with zipfile.ZipFile(file_path, "r") as zip_ref:
+            zip_ref.extractall(data_cache_dir)
 
 def read_data(train_data_dir, test_data_dir):
     """parses data in given train and test data directories
 
     assumes:
     - the data in the input directories are .json files with
         keys 'users' and 'user_data'
```

### Comparing `fedml-0.8.4a9/fedml/data/MNIST/stats.py` & `fedml-0.8.5a1/fedml/data/MNIST/stats.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/lending_club_loan/lending_club_dataset.py` & `fedml-0.8.5a1/fedml/data/lending_club_loan/lending_club_dataset.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/lending_club_loan/lending_club_feature_group.py` & `fedml-0.8.5a1/fedml/data/lending_club_loan/lending_club_feature_group.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/fed_cifar100/data_loader.py` & `fedml-0.8.5a1/fedml/data/fed_cifar100/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/fed_cifar100/dataset.py` & `fedml-0.8.5a1/fedml/data/fed_cifar100/dataset.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/fed_cifar100/utils.py` & `fedml-0.8.5a1/fedml/data/fed_cifar100/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/FederatedEMNIST/data_loader.py` & `fedml-0.8.5a1/fedml/data/FederatedEMNIST/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/cifar100/data_loader.py` & `fedml-0.8.5a1/fedml/data/cifar100/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/cifar100/datasets.py` & `fedml-0.8.5a1/fedml/data/cifar100/datasets.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/data_loader.py` & `fedml-0.8.5a1/fedml/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/file_operation.py` & `fedml-0.8.5a1/fedml/data/file_operation.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/shakespeare/language_utils.py` & `fedml-0.8.5a1/fedml/data/shakespeare/language_utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/shakespeare/data_loader.py` & `fedml-0.8.5a1/fedml/data/shakespeare/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/shakespeare/stats.py` & `fedml-0.8.5a1/fedml/data/shakespeare/stats.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/synthetic_1_1/data_loader.py` & `fedml-0.8.5a1/fedml/data/synthetic_1_1/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/synthetic_1_1/stats.py` & `fedml-0.8.5a1/fedml/data/synthetic_1_1/stats.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/synthetic_1_1/generate_synthetic.py` & `fedml-0.8.5a1/fedml/data/synthetic_1_1/generate_synthetic.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/Landmarks/download_without_tff.py` & `fedml-0.8.5a1/fedml/data/Landmarks/download_without_tff.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/Landmarks/data_loader.py` & `fedml-0.8.5a1/fedml/data/Landmarks/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/Landmarks/datasets.py` & `fedml-0.8.5a1/fedml/data/Landmarks/datasets.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/Landmarks/utils.py` & `fedml-0.8.5a1/fedml/data/Landmarks/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/Landmarks/check_download.py` & `fedml-0.8.5a1/fedml/data/Landmarks/check_download.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/Landmarks/download_without_tf.py` & `fedml-0.8.5a1/fedml/data/Landmarks/download_without_tf.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/fednlp/base/preprocess/base_example.py` & `fedml-0.8.5a1/fedml/data/fednlp/base/preprocess/base_example.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/fednlp/base/raw_data/partition.py` & `fedml-0.8.5a1/fedml/data/fednlp/base/raw_data/partition.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/fednlp/base/raw_data/base_raw_data_loader.py` & `fedml-0.8.5a1/fedml/data/fednlp/base/raw_data/base_raw_data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/fednlp/base/data_manager/base_data_manager.py` & `fedml-0.8.5a1/fedml/data/fednlp/base/data_manager/base_data_manager.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/fednlp/base/utils.py` & `fedml-0.8.5a1/fedml/data/fednlp/base/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/NUS_WIDE/nus_wide_dataset.py` & `fedml-0.8.5a1/fedml/data/NUS_WIDE/nus_wide_dataset.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/stackoverflow_lr/data_loader.py` & `fedml-0.8.5a1/fedml/data/stackoverflow_lr/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/stackoverflow_lr/dataset.py` & `fedml-0.8.5a1/fedml/data/stackoverflow_lr/dataset.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/stackoverflow_lr/utils.py` & `fedml-0.8.5a1/fedml/data/stackoverflow_lr/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/fed_shakespeare/data_loader.py` & `fedml-0.8.5a1/fedml/data/fed_shakespeare/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/fed_shakespeare/utils.py` & `fedml-0.8.5a1/fedml/data/fed_shakespeare/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/ImageNet/data_loader.py` & `fedml-0.8.5a1/fedml/data/ImageNet/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/ImageNet/datasets.py` & `fedml-0.8.5a1/fedml/data/ImageNet/datasets.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/ImageNet/datasets_hdf5.py` & `fedml-0.8.5a1/fedml/data/ImageNet/datasets_hdf5.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/data_loader_cross_silo.py` & `fedml-0.8.5a1/fedml/data/data_loader_cross_silo.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/cinic10/data_loader.py` & `fedml-0.8.5a1/fedml/data/cinic10/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/cinic10/datasets.py` & `fedml-0.8.5a1/fedml/data/cinic10/datasets.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/stackoverflow_nwp/data_loader.py` & `fedml-0.8.5a1/fedml/data/stackoverflow_nwp/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/stackoverflow_nwp/dataset.py` & `fedml-0.8.5a1/fedml/data/stackoverflow_nwp/dataset.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/stackoverflow_nwp/utils.py` & `fedml-0.8.5a1/fedml/data/stackoverflow_nwp/utils.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/UCI/data_loader_for_susy_and_ro.py` & `fedml-0.8.5a1/fedml/data/UCI/data_loader_for_susy_and_ro.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/edge_case_examples/data_loader.py` & `fedml-0.8.5a1/fedml/data/edge_case_examples/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/edge_case_examples/datasets.py` & `fedml-0.8.5a1/fedml/data/edge_case_examples/datasets.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/cifar10/efficient_loader.py` & `fedml-0.8.5a1/fedml/data/cifar10/efficient_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,16 +94,14 @@
     return train_transform, valid_transform
 
 
 def load_cifar10_data(datadir, process_id, synthetic_data_url, private_local_data, resize=32, augmentation=True, data_efficient_load=False):
     train_transform, test_transform = _data_transforms_cifar10()
 
     is_download = True;
-    if process_id != 0:
-        is_download = False if (len(synthetic_data_url) != 0 or len(private_local_data) != 0) else True;
 
     if data_efficient_load:
         cifar10_train_ds = CIFAR10(datadir, train=True, download=True, transform=train_transform)
         cifar10_test_ds = CIFAR10(datadir, train=False, download=True, transform=test_transform)
     else:
         cifar10_train_ds = CIFAR10_truncated(datadir, train=True, download=is_download, transform=train_transform)
         cifar10_test_ds = CIFAR10_truncated(datadir, train=False, download=is_download, transform=test_transform)
```

### Comparing `fedml-0.8.4a9/fedml/data/cifar10/data_loader.py` & `fedml-0.8.5a1/fedml/data/cifar10/data_loader.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/cifar10/datasets.py` & `fedml-0.8.5a1/fedml/data/cifar10/datasets.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml/data/cifar10/without_reload.py` & `fedml-0.8.5a1/fedml/data/cifar10/without_reload.py`

 * *Files identical despite different names*

### Comparing `fedml-0.8.4a9/fedml.egg-info/PKG-INFO` & `fedml-0.8.5a1/fedml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedml
-Version: 0.8.4a9
+Version: 0.8.5a1
 Summary: A research and production integrated edge-cloud library for federated/distributed machine learning at anywhere at any scale.
 Home-page: https://github.com/FedML-AI/FedML
 Author: FedML Team
 Author-email: ch@fedml.ai
 License: Apache 2.0
 Description: # FedML - The community building and connecting AI anywhere at any scale
```

### Comparing `fedml-0.8.4a9/fedml.egg-info/SOURCES.txt` & `fedml-0.8.5a1/fedml.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,14 @@
 examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/__init__.py
 examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/my_dataset.py
 examples/cross_device/mqtt_s3_fedavg_cifar10_resnet20_example/torch_server.py
 examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/__init__.py
 examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/my_dataset.py
 examples/cross_device/mqtt_s3_fedavg_mnist_lenet_example/torch_server.py
 examples/cross_silo/__init__.py
-examples/cross_silo/FA_examples/__init__.py
-examples/cross_silo/FA_examples/mqtt_s3_avg_fake_data_example/__init__.py
-examples/cross_silo/FA_examples/mqtt_s3_avg_fake_data_example/client.py
-examples/cross_silo/FA_examples/mqtt_s3_avg_fake_data_example/server.py
-examples/cross_silo/FA_examples/mqtt_s3_frequency_estimation_fake_data_example/__init__.py
-examples/cross_silo/FA_examples/mqtt_s3_frequency_estimation_fake_data_example/client.py
-examples/cross_silo/FA_examples/mqtt_s3_frequency_estimation_fake_data_example/server.py
-examples/cross_silo/FA_examples/mqtt_s3_intersection_and_cardinality_fake_data_example/__init__.py
-examples/cross_silo/FA_examples/mqtt_s3_intersection_and_cardinality_fake_data_example/client.py
-examples/cross_silo/FA_examples/mqtt_s3_intersection_and_cardinality_fake_data_example/server.py
-examples/cross_silo/FA_examples/mqtt_s3_k_percentile_fake_data_example/__init__.py
-examples/cross_silo/FA_examples/mqtt_s3_k_percentile_fake_data_example/client.py
-examples/cross_silo/FA_examples/mqtt_s3_k_percentile_fake_data_example/server.py
-examples/cross_silo/FA_examples/mqtt_s3_union_fake_data_example/__init__.py
-examples/cross_silo/FA_examples/mqtt_s3_union_fake_data_example/client.py
-examples/cross_silo/FA_examples/mqtt_s3_union_fake_data_example/server.py
 examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/__init__.py
 examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/__init__.py
 examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/torch_client.py
 examples/cross_silo/cuda_rpc_fedavg_mnist_lr_example/one_line/torch_server.py
 examples/cross_silo/grpc_fedavg_mnist_lr_example/__init__.py
 examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
 examples/cross_silo/grpc_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
@@ -43,47 +27,30 @@
 examples/cross_silo/grpc_fedavg_mnist_lr_example/step_by_step/torch_server.py
 examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/__init__.py
 examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_client.py
 examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model.py
 examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_aggregator.py
 examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_model_trainer_classification.py
 examples/cross_silo/jax_haiku_mqtt_s3_fedavg_mnist_lr_example/jax_haiku_server.py
-examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/__init__.py
-examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_client.py
-examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_mpi.py
-examples/cross_silo/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_server.py
-examples/cross_silo/mqtt_s3_fedavg_attack_mnist_lr_example/__init__.py
-examples/cross_silo/mqtt_s3_fedavg_attack_mnist_lr_example/torch_client.py
-examples/cross_silo/mqtt_s3_fedavg_attack_mnist_lr_example/torch_server.py
-examples/cross_silo/mqtt_s3_fedavg_cdp_mnist_lr_example/__init__.py
-examples/cross_silo/mqtt_s3_fedavg_cdp_mnist_lr_example/torch_client.py
-examples/cross_silo/mqtt_s3_fedavg_cdp_mnist_lr_example/torch_server.py
 examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/__init__.py
 examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_client.py
 examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/torch_server.py
 examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/__init__.py
 examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_aggregator.py
 examples/cross_silo/mqtt_s3_fedavg_cifar10_lr_example/trainer/classification_trainer.py
-examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/__init__.py
-examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/torch_client.py
-examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/torch_mpi.py
-examples/cross_silo/mqtt_s3_fedavg_defense_mnist_lr_example/torch_server.py
 examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/__init__.py
 examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/__init__.py
 examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/main_fedml_cross_silo_hi.py
 examples/cross_silo/mqtt_s3_fedavg_hierarchical_manual_mnist_lr_example/one_line/mlops_client_launcher.py
 examples/cross_silo/mqtt_s3_fedavg_hierarchical_mnist_lr_example/__init__.py
 examples/cross_silo/mqtt_s3_fedavg_hierarchical_mnist_lr_example/main_fedml_cross_silo_hi.py
 examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/__init__.py
 examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/__init__.py
 examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/torch_client.py
 examples/cross_silo/mqtt_s3_fedavg_horizontal_mnist_lr_example/one_line/torch_server.py
-examples/cross_silo/mqtt_s3_fedavg_ldp_mnist_lr_example/__init__.py
-examples/cross_silo/mqtt_s3_fedavg_ldp_mnist_lr_example/torch_client.py
-examples/cross_silo/mqtt_s3_fedavg_ldp_mnist_lr_example/torch_server.py
 examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/__init__.py
 examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/__init__.py
 examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_client.py
 examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/custom_data_and_model/torch_server.py
 examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/__init__.py
 examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/torch_client.py
 examples/cross_silo/mqtt_s3_fedavg_mnist_lr_example/step_by_step/torch_server.py
@@ -113,14 +80,57 @@
 examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_aggregator.py
 examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_model_trainer_classification.py
 examples/cross_silo/tf_mqtt_s3_fedavg_mnist_lr_example/tf_server.py
 examples/cross_silo/trpc_fedavg_mnist_lr_example/__init__.py
 examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/__init__.py
 examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/torch_client.py
 examples/cross_silo/trpc_fedavg_mnist_lr_example/one_line/torch_server.py
+examples/federated_analytics/__init__.py
+examples/federated_analytics/avg_fake_data_example/__init__.py
+examples/federated_analytics/avg_fake_data_example/client.py
+examples/federated_analytics/avg_fake_data_example/server.py
+examples/federated_analytics/avg_self_defined_data_example/__init__.py
+examples/federated_analytics/avg_self_defined_data_example/client.py
+examples/federated_analytics/avg_self_defined_data_example/server.py
+examples/federated_analytics/frequency_estimation_fake_data_example/__init__.py
+examples/federated_analytics/frequency_estimation_fake_data_example/client.py
+examples/federated_analytics/frequency_estimation_fake_data_example/server.py
+examples/federated_analytics/heavy_hitter_twitter_data_example/__init__.py
+examples/federated_analytics/heavy_hitter_twitter_data_example/client.py
+examples/federated_analytics/heavy_hitter_twitter_data_example/server.py
+examples/federated_analytics/intersection_and_cardinality_fake_data_example/__init__.py
+examples/federated_analytics/intersection_and_cardinality_fake_data_example/client.py
+examples/federated_analytics/intersection_and_cardinality_fake_data_example/server.py
+examples/federated_analytics/k_percentile_fake_data_example/__init__.py
+examples/federated_analytics/k_percentile_fake_data_example/client.py
+examples/federated_analytics/k_percentile_fake_data_example/server.py
+examples/federated_analytics/union_fake_data_example/__init__.py
+examples/federated_analytics/union_fake_data_example/client.py
+examples/federated_analytics/union_fake_data_example/server.py
+examples/privacy/__init__.py
+examples/privacy/mpi_fedavg_dp_mnist_lr_example/__init__.py
+examples/privacy/mpi_fedavg_dp_mnist_lr_example/cross_silo_with_mpi.py
+examples/privacy/mqtt_s3_fedavg_cdp_mnist_lr_example/__init__.py
+examples/privacy/mqtt_s3_fedavg_cdp_mnist_lr_example/torch_client.py
+examples/privacy/mqtt_s3_fedavg_cdp_mnist_lr_example/torch_server.py
+examples/privacy/mqtt_s3_fedavg_ldp_mnist_lr_example/__init__.py
+examples/privacy/mqtt_s3_fedavg_ldp_mnist_lr_example/torch_client.py
+examples/privacy/mqtt_s3_fedavg_ldp_mnist_lr_example/torch_server.py
+examples/security/__init__.py
+examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/__init__.py
+examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_client.py
+examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_mpi.py
+examples/security/mqtt_s3_fedavg_attack_defense_cifar10_resnet56_example/torch_server.py
+examples/security/mqtt_s3_fedavg_attack_mnist_lr_example/__init__.py
+examples/security/mqtt_s3_fedavg_attack_mnist_lr_example/torch_client.py
+examples/security/mqtt_s3_fedavg_attack_mnist_lr_example/torch_server.py
+examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/__init__.py
+examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/torch_client.py
+examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/torch_mpi.py
+examples/security/mqtt_s3_fedavg_defense_mnist_lr_example/torch_server.py
 examples/simulation/__init__.py
 examples/simulation/mpi_base_framework_example/__init__.py
 examples/simulation/mpi_base_framework_example/mpi_base_framework_example.py
 examples/simulation/mpi_decentralized_fl_example/__init__.py
 examples/simulation/mpi_decentralized_fl_example/mpi_decentralized_fl_example.py
 examples/simulation/mpi_fedavg_datasets_and_models_example/__init__.py
 examples/simulation/mpi_fedavg_datasets_and_models_example/torch_step_by_step_example.py
@@ -580,14 +590,15 @@
 fedml/fa/__init__.py
 fedml/fa/constants.py
 fedml/fa/runner.py
 fedml/fa/aggregator/__init__.py
 fedml/fa/aggregator/avg_aggregator.py
 fedml/fa/aggregator/frequency_estimation_aggregator.py
 fedml/fa/aggregator/global_analyzer_creator.py
+fedml/fa/aggregator/heavy_hitter_triehh_aggregator.py
 fedml/fa/aggregator/intersection_aggregator.py
 fedml/fa/aggregator/k_percentile_element_aggregator.py
 fedml/fa/aggregator/union_aggregator.py
 fedml/fa/base_frame/__init__.py
 fedml/fa/base_frame/client_analyzer.py
 fedml/fa/base_frame/server_aggregator.py
 fedml/fa/cross_silo/__init__.py
@@ -608,29 +619,34 @@
 fedml/fa/cross_silo/server/message_define.py
 fedml/fa/cross_silo/server/server_initializer.py
 fedml/fa/data/__init__.py
 fedml/fa/data/data_loader.py
 fedml/fa/data/utils.py
 fedml/fa/data/fake_numeric_data/__init__.py
 fedml/fa/data/fake_numeric_data/data_loader.py
+fedml/fa/data/self_defined_data/__init__.py
+fedml/fa/data/self_defined_data/data_loader.py
 fedml/fa/data/twitter_Sentiment140/__init__.py
 fedml/fa/data/twitter_Sentiment140/data_loader.py
+fedml/fa/data/twitter_Sentiment140/twitter_data_processing.py
 fedml/fa/local_analyzer/__init__.py
 fedml/fa/local_analyzer/avg.py
 fedml/fa/local_analyzer/client_analyzer_creator.py
 fedml/fa/local_analyzer/frequency_estimation.py
 fedml/fa/local_analyzer/heavy_hitter_triehh.py
 fedml/fa/local_analyzer/intersection.py
 fedml/fa/local_analyzer/k_percentage_element.py
 fedml/fa/local_analyzer/union.py
 fedml/fa/simulation/__init__.py
 fedml/fa/simulation/utils.py
 fedml/fa/simulation/sp/__init__.py
 fedml/fa/simulation/sp/client.py
 fedml/fa/simulation/sp/simulator.py
+fedml/fa/utils/__init__.py
+fedml/fa/utils/trie.py
 fedml/ml/__init__.py
 fedml/ml/aggregator/__init__.py
 fedml/ml/aggregator/agg_operator.py
 fedml/ml/aggregator/aggregator_creator.py
 fedml/ml/aggregator/default_aggregator.py
 fedml/ml/aggregator/my_server_aggregator.py
 fedml/ml/aggregator/my_server_aggregator_classification.py
```

