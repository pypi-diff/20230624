# Comparing `tmp/modular_rl-0.3.3.tar.gz` & `tmp/modular_rl-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modular_rl-0.3.3.tar", last modified: Thu Jun 15 14:19:25 2023, max compression
+gzip compressed data, was "modular_rl-0.4.0.tar", last modified: Sat Jun 24 06:50:27 2023, max compression
```

## Comparing `modular_rl-0.3.3.tar` & `modular_rl-0.4.0.tar`

### file list

```diff
@@ -1,54 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 14:19:25.982962 modular_rl-0.3.3/
--rw-rw-rw-   0        0        0     1089 2023-05-04 06:13:20.000000 modular_rl-0.3.3/LICENSE
--rw-rw-rw-   0        0        0     5688 2023-06-15 14:19:25.982962 modular_rl-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     4182 2023-06-08 11:09:02.000000 modular_rl-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 14:19:25.925107 modular_rl-0.3.3/modular_rl/
--rw-rw-rw-   0        0        0       37 2023-05-07 14:51:41.000000 modular_rl-0.3.3/modular_rl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:19:25.944071 modular_rl-0.3.3/modular_rl/agents/
--rw-rw-rw-   0        0        0      108 2023-06-06 21:28:14.000000 modular_rl-0.3.3/modular_rl/agents/__init__.py
--rw-rw-rw-   0        0        0    10939 2023-06-15 13:13:29.000000 modular_rl-0.3.3/modular_rl/agents/_agent.py
--rw-rw-rw-   0        0        0     4838 2023-06-06 21:35:21.000000 modular_rl-0.3.3/modular_rl/agents/_custom.py
--rw-rw-rw-   0        0        0    11741 2023-06-08 11:22:46.000000 modular_rl-0.3.3/modular_rl/agents/mcis.py
--rw-rw-rw-   0        0        0    12162 2023-06-15 13:13:37.000000 modular_rl-0.3.3/modular_rl/agents/mcts.py
--rw-rw-rw-   0        0        0    22611 2023-06-14 12:35:48.000000 modular_rl-0.3.3/modular_rl/agents/mim.py
--rw-rw-rw-   0        0        0    14958 2023-06-06 21:36:06.000000 modular_rl-0.3.3/modular_rl/agents/ppo.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:19:25.947262 modular_rl-0.3.3/modular_rl/envs/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:09:01.000000 modular_rl-0.3.3/modular_rl/envs/__init__.py
--rw-rw-rw-   0        0        0      133 2023-06-04 21:09:01.000000 modular_rl-0.3.3/modular_rl/envs/_custom.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:19:25.951690 modular_rl-0.3.3/modular_rl/envs/mim/
--rw-rw-rw-   0        0        0       25 2023-06-04 21:09:01.000000 modular_rl-0.3.3/modular_rl/envs/mim/__init__.py
--rw-rw-rw-   0        0        0    15402 2023-06-04 21:09:01.000000 modular_rl-0.3.3/modular_rl/envs/mim/card_evaluator.py
--rw-rw-rw-   0        0        0     4413 2023-06-14 12:37:11.000000 modular_rl-0.3.3/modular_rl/envs/mim/mim.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:19:25.958218 modular_rl-0.3.3/modular_rl/networks/
--rw-rw-rw-   0        0        0       68 2023-05-07 14:51:41.000000 modular_rl-0.3.3/modular_rl/networks/__init__.py
--rw-rw-rw-   0        0        0     2174 2023-05-07 14:51:41.000000 modular_rl-0.3.3/modular_rl/networks/actor_critic.py
--rw-rw-rw-   0        0        0     2878 2023-05-04 23:35:18.000000 modular_rl-0.3.3/modular_rl/networks/policy.py
--rw-rw-rw-   0        0        0     2688 2023-05-04 23:33:52.000000 modular_rl-0.3.3/modular_rl/networks/value.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:19:25.965168 modular_rl-0.3.3/modular_rl/params/
--rw-rw-rw-   0        0        0       85 2023-06-04 21:09:01.000000 modular_rl-0.3.3/modular_rl/params/__init__.py
--rw-rw-rw-   0        0        0     2161 2023-06-04 21:09:01.000000 modular_rl-0.3.3/modular_rl/params/mcis.py
--rw-rw-rw-   0        0        0     2294 2023-06-08 11:07:34.000000 modular_rl-0.3.3/modular_rl/params/mcts.py
--rw-rw-rw-   0        0        0     2933 2023-06-13 11:17:09.000000 modular_rl-0.3.3/modular_rl/params/mim.py
--rw-rw-rw-   0        0        0     2053 2023-05-07 14:51:41.000000 modular_rl-0.3.3/modular_rl/params/ppo.py
--rw-rw-rw-   0        0        0     1377 2023-06-06 22:36:03.000000 modular_rl-0.3.3/modular_rl/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:19:25.968433 modular_rl-0.3.3/modular_rl/util/
--rw-rw-rw-   0        0        0        0 2023-05-04 23:35:52.000000 modular_rl-0.3.3/modular_rl/util/__init__.py
--rw-rw-rw-   0        0        0     2533 2023-06-04 21:09:01.000000 modular_rl-0.3.3/modular_rl/util/node.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:19:25.933520 modular_rl-0.3.3/modular_rl.egg-info/
--rw-rw-rw-   0        0        0     5688 2023-06-15 14:19:25.000000 modular_rl-0.3.3/modular_rl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1088 2023-06-15 14:19:25.000000 modular_rl-0.3.3/modular_rl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 14:19:25.000000 modular_rl-0.3.3/modular_rl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-15 14:19:25.000000 modular_rl-0.3.3/modular_rl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-15 14:19:25.000000 modular_rl-0.3.3/modular_rl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1414 2023-06-12 13:39:56.000000 modular_rl-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-15 14:19:25.983983 modular_rl-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      937 2023-06-12 13:39:35.000000 modular_rl-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:19:25.980433 modular_rl-0.3.3/tests/
--rw-rw-rw-   0        0        0      383 2023-06-11 10:42:57.000000 modular_rl-0.3.3/tests/test_mcis.py
--rw-rw-rw-   0        0        0      725 2023-06-11 10:42:57.000000 modular_rl-0.3.3/tests/test_mcis_modular.py
--rw-rw-rw-   0        0        0      383 2023-06-11 10:42:57.000000 modular_rl-0.3.3/tests/test_mcts.py
--rw-rw-rw-   0        0        0     1077 2023-06-11 10:42:57.000000 modular_rl-0.3.3/tests/test_mcts_modular.py
--rw-rw-rw-   0        0        0      342 2023-06-11 10:42:57.000000 modular_rl-0.3.3/tests/test_mim.py
--rw-rw-rw-   0        0        0      567 2023-06-11 10:42:57.000000 modular_rl-0.3.3/tests/test_mim_modular.py
--rw-rw-rw-   0        0        0      912 2023-06-11 10:42:57.000000 modular_rl-0.3.3/tests/test_ppo.py
--rw-rw-rw-   0        0        0     1470 2023-06-11 10:42:57.000000 modular_rl-0.3.3/tests/test_ppo_modular.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:50:27.264692 modular_rl-0.4.0/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 06:13:20.000000 modular_rl-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0      781 2023-06-24 06:50:27.263692 modular_rl-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4322 2023-06-10 03:09:21.000000 modular_rl-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 06:50:27.054542 modular_rl-0.4.0/modular_rl/
+-rw-rw-rw-   0        0        0       36 2023-05-07 02:39:54.000000 modular_rl-0.4.0/modular_rl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:50:27.126082 modular_rl-0.4.0/modular_rl/agents/
+-rw-rw-rw-   0        0        0      112 2023-06-10 03:09:21.000000 modular_rl-0.4.0/modular_rl/agents/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:50:27.145774 modular_rl-0.4.0/modular_rl/agents/_common/
+-rw-rw-rw-   0        0        0       35 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/agents/_common/__init__.py
+-rw-rw-rw-   0        0        0     7265 2023-06-24 05:46:15.000000 modular_rl-0.4.0/modular_rl/agents/_common/_agents.py
+-rw-rw-rw-   0        0        0     5252 2023-06-24 05:54:50.000000 modular_rl-0.4.0/modular_rl/agents/_custom.py
+-rw-rw-rw-   0        0        0     2251 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/agents/mcis.py
+-rw-rw-rw-   0        0        0     2251 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/agents/mcts.py
+-rw-rw-rw-   0        0        0    23135 2023-06-24 05:35:24.000000 modular_rl-0.4.0/modular_rl/agents/mim.py
+-rw-rw-rw-   0        0        0     2819 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/agents/ppo.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:50:27.155779 modular_rl-0.4.0/modular_rl/agents/pytorch/
+-rw-rw-rw-   0        0        0      106 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/agents/pytorch/__init__.py
+-rw-rw-rw-   0        0        0     6913 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/agents/pytorch/_agent.py
+-rw-rw-rw-   0        0        0    12241 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/agents/pytorch/mcis.py
+-rw-rw-rw-   0        0        0    12545 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/agents/pytorch/mcts.py
+-rw-rw-rw-   0        0        0    15558 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/agents/pytorch/ppo.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:50:27.219696 modular_rl-0.4.0/modular_rl/agents/tensorflow/
+-rw-rw-rw-   0        0        0      115 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/agents/tensorflow/__init__.py
+-rw-rw-rw-   0        0        0     6053 2023-06-24 05:53:23.000000 modular_rl-0.4.0/modular_rl/agents/tensorflow/_agent.py
+-rw-rw-rw-   0        0        0    13196 2023-06-24 05:56:47.000000 modular_rl-0.4.0/modular_rl/agents/tensorflow/mcis.py
+-rw-rw-rw-   0        0        0    11894 2023-06-24 05:52:02.000000 modular_rl-0.4.0/modular_rl/agents/tensorflow/mcts.py
+-rw-rw-rw-   0        0        0    11937 2023-06-24 05:52:29.000000 modular_rl-0.4.0/modular_rl/agents/tensorflow/ppo.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:50:27.223698 modular_rl-0.4.0/modular_rl/envs/
+-rw-rw-rw-   0        0        0        0 2023-06-03 00:27:02.000000 modular_rl-0.4.0/modular_rl/envs/__init__.py
+-rw-rw-rw-   0        0        0      133 2023-06-03 00:27:02.000000 modular_rl-0.4.0/modular_rl/envs/_custom.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:50:27.228698 modular_rl-0.4.0/modular_rl/envs/mim/
+-rw-rw-rw-   0        0        0       25 2023-06-03 00:27:02.000000 modular_rl-0.4.0/modular_rl/envs/mim/__init__.py
+-rw-rw-rw-   0        0        0    15402 2023-06-03 00:27:02.000000 modular_rl-0.4.0/modular_rl/envs/mim/card_evaluator.py
+-rw-rw-rw-   0        0        0     4555 2023-06-24 05:35:24.000000 modular_rl-0.4.0/modular_rl/envs/mim/mim.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:50:27.230687 modular_rl-0.4.0/modular_rl/networks/
+-rw-rw-rw-   0        0        0        0 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/networks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:50:27.238686 modular_rl-0.4.0/modular_rl/networks/pytorch/
+-rw-rw-rw-   0        0        0      135 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/networks/pytorch/__init__.py
+-rw-rw-rw-   0        0        0     2188 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/networks/pytorch/actor_critic.py
+-rw-rw-rw-   0        0        0     2888 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/networks/pytorch/policy.py
+-rw-rw-rw-   0        0        0     2698 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/networks/pytorch/value.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:50:27.247692 modular_rl-0.4.0/modular_rl/networks/tensorflow/
+-rw-rw-rw-   0        0        0      114 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/networks/tensorflow/__init__.py
+-rw-rw-rw-   0        0        0      849 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/networks/tensorflow/actor_critic.py
+-rw-rw-rw-   0        0        0     1119 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/networks/tensorflow/policy.py
+-rw-rw-rw-   0        0        0     1022 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/networks/tensorflow/value.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:50:27.257692 modular_rl-0.4.0/modular_rl/params/
+-rw-rw-rw-   0        0        0       85 2023-06-03 00:27:02.000000 modular_rl-0.4.0/modular_rl/params/__init__.py
+-rw-rw-rw-   0        0        0     2198 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/params/mcis.py
+-rw-rw-rw-   0        0        0     2412 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/params/mcts.py
+-rw-rw-rw-   0        0        0     2975 2023-06-24 05:35:24.000000 modular_rl-0.4.0/modular_rl/params/mim.py
+-rw-rw-rw-   0        0        0     2131 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/params/ppo.py
+-rw-rw-rw-   0        0        0     1406 2023-06-10 03:09:21.000000 modular_rl-0.4.0/modular_rl/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:50:27.261690 modular_rl-0.4.0/modular_rl/util/
+-rw-rw-rw-   0        0        0        0 2023-05-04 23:35:52.000000 modular_rl-0.4.0/modular_rl/util/__init__.py
+-rw-rw-rw-   0        0        0     2626 2023-06-24 05:45:12.000000 modular_rl-0.4.0/modular_rl/util/node.py
+drwxrwxrwx   0        0        0        0 2023-06-24 06:50:27.100552 modular_rl-0.4.0/modular_rl.egg-info/
+-rw-rw-rw-   0        0        0      781 2023-06-24 06:50:26.000000 modular_rl-0.4.0/modular_rl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1555 2023-06-24 06:50:26.000000 modular_rl-0.4.0/modular_rl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 06:50:26.000000 modular_rl-0.4.0/modular_rl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-06-24 06:50:26.000000 modular_rl-0.4.0/modular_rl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-24 06:50:26.000000 modular_rl-0.4.0/modular_rl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1495 2023-06-24 05:45:12.000000 modular_rl-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-24 06:50:27.264692 modular_rl-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      999 2023-06-24 05:45:12.000000 modular_rl-0.4.0/setup.py
```

### Comparing `modular_rl-0.3.3/LICENSE` & `modular_rl-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.3/README.md` & `modular_rl-0.4.0/README.md`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-# ModularRL
-
-ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
-
-## Installation
-
-```powershell
-pip install modular_rl
-```
-
-## Features
-
--   Implementations of various reinforcement learning algorithms,
-    such as Proximal Policy Optimization (PPO), Monte Carlo Tree Search (MCTS), Monte Carlo Information Set (MCIS), and Modular's sIMulator (MIM)
--   Customizable agent settings and network architectures
--   Modular structure for easy adaptation and extension across different algorithms
--   Model saving and loading functionality for easy reuse of trained models
-
-## Supported Algorithms
-
--   Proximal Policy Optimization (PPO)
--   Monte Carlo Tree Search (MCTS)
--   Monte Carlo Information Set (MCIS)
--   Modular's sIMulator (MIM)
-
-Refer to the respective agent classes for each algorithm:
-
--   AgentPPO (+ Modular)
--   AgentMCTS (+ Modular)
--   AgentMCIS (+ Modular)
--   AgentMIM (+ Modular)
-
-## Example Usage
-
-You can use the tester.py script provided in the library to create and train an instance of an agent with default or modified settings:
-
-```python
-import modular_rl.tester as tester
-
-tester.init_ppo()
-# or
-tester.init_ppo_modular()
-
-tester.init_mcts()
-```
-
-As more algorithms are added, the tester functions will follow the naming convention init*[algorithm_name] or init*[algorithm_name]\_modular.
-
-Please note that not all algorithms support modular training due to the nature of their design.
-For such algorithms, you will need to use the non-modular training method provided by the respective agent class.
-You can refer to the list of supported algorithms to determine which training method is appropriate.
-
-Alternatively, you can create and train an instance of the AgentPPO(example) class directly in your code:
-
-```python
-from modular_rl.agents.agent_ppo import AgentPPO
-from modular_rl.settings import AgentSettings
-
-def init():
-    env = AgentPPO(env=None, setting=AgentSettings.default)
-    env.learn()
-
-init()
-```
-
-To create and train an instance of the AgentPPO(example) class with modified settings, use the following code:
-
-```python
-from modular_rl.agents.agent_ppo import AgentPPO
-from modular_rl.settings import AgentSettings
-
-def init_modular():
-    # Semi-automatic (defined record usage)
-    # Implement your environment and pass it to 'env' parameter.
-    env = AgentPPO(env=None, setting=AgentSettings.default_modular)
-    env.reset()
-    env.learn_reset()
-    action, reward, is_done = env.learn_next()
-    env.learn_check()
-    env.update()
-
-    # Proceed with the learning manually.
-    env.reset()
-    # Implement the 'reset' method in your environment.
-    '''
-    def reset(self):
-        ...
-        return initial_state
-    '''
-    env.learn_reset()
-    initial_state = env.learn_reset()
-    action, dist = env.select_action(initial_state)
-
-    '''
-    Note:
-    Please implement the resulting state of update_step in the step function of your environment.
-
-    For example:
-
-    def step(self, action):
-        ...
-        return next_state, reward, is_done, _
-    '''
-
-    env.update_step(initial_state, dist, action, -1)
-
-    env.learn_check()
-    env.update()
-
-    env.learn_close()
-
-init_modular()
-```
-
-## Saving and Loading Models
-
-Agents can save and load their models using the save_model(file_name) and load_model(file_name) methods.
-The file_name parameter should be the name of the file to save or load the model to/from.
-
-Example:
-
-```python
-agent = AgentPPO(env, setting)
-agent.train()
-
-agent.save_model("my_saved_model.pth")
-
-loaded_agent = AgentPPO(env, setting)
-loaded_agent.load_model("my_saved_model.pth")
-```
-
-## Key Classes
-
--   AgentPPO, AgentMCTS, AgentMCIS, AgentMIM: The main agent classes implementing various reinforcement learning algorithms.
--   PolicyNetwork, ValueNetwork, ActorCriticNetwork: Customizable neural networks for the agent's policy and value functions.
--   AgentSettings: A configuration class for setting up the agents.
-
-## License
-
-MIT License
+# ModularRL
+
+ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
+
+## Installation
+
+```powershell
+pip install modular_rl
+```
+
+## Features
+
+-   Implementations of various reinforcement learning algorithms,
+    such as Proximal Policy Optimization (PPO), Monte Carlo Tree Search (MCTS), Monte Carlo Information Set (MCIS), and Modular's sIMulator (MIM)
+-   Customizable agent settings and network architectures
+-   Modular structure for easy adaptation and extension across different algorithms
+-   Model saving and loading functionality for easy reuse of trained models
+
+## Supported Algorithms
+
+-   Proximal Policy Optimization (PPO)
+-   Monte Carlo Tree Search (MCTS)
+-   Monte Carlo Information Set (MCIS)
+-   Modular's sIMulator (MIM)
+
+Refer to the respective agent classes for each algorithm:
+
+-   AgentPPO (+ Modular)
+-   AgentMCTS (+ Modular)
+-   AgentMCIS (+ Modular)
+-   AgentMIM (+ Modular)
+
+## Example Usage
+
+You can use the tester.py script provided in the library to create and train an instance of an agent with default or modified settings:
+
+```python
+import modular_rl.tester as tester
+
+tester.init_ppo()
+# or
+tester.init_ppo_modular()
+
+tester.init_mcts()
+```
+
+As more algorithms are added, the tester functions will follow the naming convention init*[algorithm_name] or init*[algorithm_name]\_modular.
+
+Please note that not all algorithms support modular training due to the nature of their design.
+For such algorithms, you will need to use the non-modular training method provided by the respective agent class.
+You can refer to the list of supported algorithms to determine which training method is appropriate.
+
+Alternatively, you can create and train an instance of the AgentPPO(example) class directly in your code:
+
+```python
+from modular_rl.agents.agent_ppo import AgentPPO
+from modular_rl.settings import AgentSettings
+
+def init():
+    env = AgentPPO(env=None, setting=AgentSettings.default)
+    env.learn()
+
+init()
+```
+
+To create and train an instance of the AgentPPO(example) class with modified settings, use the following code:
+
+```python
+from modular_rl.agents.agent_ppo import AgentPPO
+from modular_rl.settings import AgentSettings
+
+def init_modular():
+    # Semi-automatic (defined record usage)
+    # Implement your environment and pass it to 'env' parameter.
+    env = AgentPPO(env=None, setting=AgentSettings.default_modular)
+    env.reset()
+    env.learn_reset()
+    action, reward, is_done = env.learn_next()
+    env.learn_check()
+    env.update()
+
+    # Proceed with the learning manually.
+    env.reset()
+    # Implement the 'reset' method in your environment.
+    '''
+    def reset(self):
+        ...
+        return initial_state
+    '''
+    env.learn_reset()
+    initial_state = env.learn_reset()
+    action, dist = env.select_action(initial_state)
+
+    '''
+    Note:
+    Please implement the resulting state of update_step in the step function of your environment.
+
+    For example:
+
+    def step(self, action):
+        ...
+        return next_state, reward, is_done, _
+    '''
+
+    env.update_step(initial_state, dist, action, -1)
+
+    env.learn_check()
+    env.update()
+
+    env.learn_close()
+
+init_modular()
+```
+
+## Saving and Loading Models
+
+Agents can save and load their models using the save_model(file_name) and load_model(file_name) methods.
+The file_name parameter should be the name of the file to save or load the model to/from.
+
+Example:
+
+```python
+agent = AgentPPO(env, setting)
+agent.train()
+
+agent.save_model("my_saved_model.pth")
+
+loaded_agent = AgentPPO(env, setting)
+loaded_agent.load_model("my_saved_model.pth")
+```
+
+## Key Classes
+
+-   AgentPPO, AgentMCTS, AgentMCIS, AgentMIM: The main agent classes implementing various reinforcement learning algorithms.
+-   PolicyNetwork, ValueNetwork, ActorCriticNetwork: Customizable neural networks for the agent's policy and value functions.
+-   AgentSettings: A configuration class for setting up the agents.
+
+## License
+
+MIT License
```

### Comparing `modular_rl-0.3.3/modular_rl/agents/_agent.py` & `modular_rl-0.4.0/modular_rl/agents/tensorflow/ppo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,297 +1,305 @@
+
 # -*- coding: utf-8 -*-
 """
 ModularRL project
 
 Copyright (c) 2023 horrible-gh
 
-ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms.
-The library is designed to be easily customizable and modular,
-allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
+Class AgentPPO is an implementation of the Proximal Policy Optimization (PPO) algorithm.
+It takes an environment and a setting configuration as inputs, initializes neural network instances and optimizers,
+and sets various learning parameters.
+It has methods to predict an action given a state, perform a learning step, update the neural network parameters,
+save and load a checkpoint, and reset learning parameters.
+The class also has instance variables to keep track of episode and total rewards, previous reward, and average reward.
 
 This software includes the following third-party libraries:
 Gym (MIT License): https://github.com/openai/gym - Copyright (c) OpenAI.
 NumPy (BSD License): https://numpy.org - Copyright (c) NumPy Developers.
-PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
+TensorFlow (Apache License 2.0): https://www.tensorflow.org/ - Copyright (c) TensorFlow Developers.
 """
 
-import gym
+import tensorflow as tf
+import tensorflow_probability as tfp
+import numpy as np
 from LogAssist.log import Logger
-import torch
-import torch.optim as optim
-from modular_rl.networks.policy import PolicyNetwork
-from modular_rl.networks.value import ValueNetwork
-from modular_rl.networks.actor_critic import ActorCriticNetwork
+from modular_rl.agents.tensorflow._agent import Agent
 
 
-class Agent:
+class TensorFlowAgentPPO(Agent):
     def __init__(self, env, setting):
-        '''
-        :param env: The environment for the agent to interact with, if not provided, CartPole-v0 will be used.
-        :param setting: A dictionary containing the settings and hyperparameters for the agent's training process.
-        '''
+        super(TensorFlowAgentPPO, self).__init__(env, setting)
+        super(TensorFlowAgentPPO, self).init_policy_value()
 
-        # Environment preparation
-        self.env = env if env else gym.make('CartPole-v0')
-        self.setting = setting
-        self.state_dim = self.env.observation_space.shape[0]
-        self.action_dim = self.env.action_space.n
-
-        # Defination networks and optimizers
-        self.policy_net = None
-        self.value_net = None
-        self.policy_optimizer = None
-        self.value_optimizer = None
-
-        self.actor_critic_net = None
-        self.actor_critic_optimizer = None
-
-        # Training parameters(Common)
-        self.max_episodes = setting.get('max_episodes', 30)
-        self.max_timesteps = setting.get('max_timesteps', 100)
-        self.update_timestep = setting.get('update_timestep', 200)
-        self.gamma = setting.get('gamma', 0.99)
-        self.early_stop_threshold = setting.get('early_stop_threshold', -1)
-        self.done_loop_end = setting.get('done_loop_end', False)
-
-        # Set learn episode parameters
-        self.episode_reward = 0
-        self.total_reward = 0
-        self.prev_reward = 0
-        self.episode = 0
-        self.avg_reward = 0
+        # Set learning parameters
+        self.ppo_epochs = setting.get('ppo_epochs', 4)
+        self.mini_batch_size = setting.get('mini_batch_size', 64)
+        self.lam = setting.get('lam', 0.95)
+        self.clip_param = setting.get('clip_param', 0.2)
 
-        # Set learn parameters (If necessary)
+        # Set learn modular parameters
         self.state = None
-        self.action = None
-        self.reward = None
-        self.done = None
-        self.reset()
+        self.dist = None
+
+        # Create optimizers
+        self.value_optimizer = tf.keras.optimizers.Adam()
 
-        # Logger initialize
-        self.log_level = setting.get('log_level', 'debug')
-        self.log_init_pass = setting.get('log_init_pass', False)
-        if self.log_init_pass == False:
-            Logger.init(
-                dir_name=None,
-                file_name=None,
-                log_level=self.log_level,
-                out_console=True,
-                out_file=None,
-                prev_log_remove=None
-            )
+    def learn_reset(self):
+        return super(TensorFlowAgentPPO, self).learn_reset()
 
     def reset(self):
-        """
-        Reset the lists that contain information about the states, actions, rewards, and other values for the agent.
-        """
+        super(TensorFlowAgentPPO, self).reset()
 
-        self.states = []
-        self.actions = []
-        self.rewards = []
-        self.next_states = []
-        self.dones = []
-        self.log_probs = []
+    def check_tensor(self, state):
+        '''
+        This function checks if the provided object is a TensorFlow tensor, and if not, converts it to a tensor.
 
-    def init_policy_value(self):
-        """
-        Initializes policy and value networks, and their respective optimizers.
-        """
+        :param state: The object to check/convert to a TensorFlow tensor.
+        :return: The input object as a TensorFlow tensor.
+        '''
+        Logger.verb('_agent:check_tensor', f'state={state}')
+        if not isinstance(state[0], tf.Tensor):
+            state = (tf.convert_to_tensor(
+                state[0], dtype=tf.float32), state[1])
+        return state
 
-        # Create neural network instances and optimizer
-        networks_size = self.setting.get('networks', 'middle')
-        Logger.verb('_agent:init_policy_value',
-                    f'Initialize policy and value networks to {networks_size}')
-        self.policy_net = PolicyNetwork(
-            self.state_dim, self.action_dim, networks_size)
-        self.value_net = ValueNetwork(
-            self.state_dim, networks_size)
-        self.policy_optimizer = optim.Adam(
-            self.policy_net.parameters(), lr=self.setting.get('optimizer_speed', 3e-4))
-        self.value_optimizer = optim.Adam(
-            self.value_net.parameters(), lr=self.setting.get('optimizer_speed', 3e-4))
+    def compute_advantages(self, rewards, values, dones, gamma=0.99, lam=0.95):
+        advantages = np.zeros_like(rewards)
+        last_advantage = 0
+        for t in reversed(range(len(rewards))):
+            delta = rewards[t] + gamma * \
+                values[t + 1] * (1 - dones[t]) - values[t]
+            advantages[t] = delta + gamma * lam * \
+                last_advantage * (1 - dones[t])
+            last_advantage = advantages[t]
+        return advantages
 
-    def init_actor_critic(self):
-        """
-        Initializes the actor-critic network and its optimizer.
-        """
+    def select_action(self, state):
+        state = self._check_state(self.state)
+        state_tensor = tf.convert_to_tensor(state, dtype=tf.float32)
+        action_probs = self.policy_net(state_tensor)
+        dist = tfp.distributions.Categorical(probs=action_probs)
+        self.dist = dist
+        action = dist.sample()
+        return action, dist
+
+    def learn_step(self, state, timestep):
+        action, dist = self.select_action(state)
+        return self.update_step(state, dist, action, timestep)
+
+    def update_step(self, state, dist, action, timestep, auto_step=True, is_done=False, reward=0, next_state=None):
+        if dist is None and self.dist:
+            dist = self.dist
+        if auto_step:
+            step_output = self.env.step(int(action.numpy()[0]))
+            next_state, reward, is_done = self.step_unpack(step_output)
+        else:
+            if next_state is None:
+                next_state = state
+        self.update_reward(reward)
+        state = self._check_state(state)
+        # Note: we use Python lists here, as TensorFlow has a better support for Pythonic operations
+        self.states.append(state)
+        self.actions.append(action)
+        self.rewards.append(reward)
+        self.next_states.append(next_state)
+        self.dones.append(is_done)
+        self.log_probs.append(dist.log_prob(action))
+        self.state = next_state
+        if timestep > 0:
+            timestep += 1
+        if self.update_timestep > 0 and timestep > 0 and (timestep % self.update_timestep == 0):
+            self.update()
+        return action, reward, is_done, timestep
 
-        # Neural Network
-        self.actor_critic_net = ActorCriticNetwork(
-            self.state_dim, self.action_dim)
-        self.actor_critic_optimizer = optim.Adam(
-            self.actor_critic_net.parameters(), lr=self.setting.get('optimizer_speed', 3e-4))
+    def update(self):
+        # convert lists to tensors
+        states_tensor = tf.convert_to_tensor(self.states, dtype=tf.float32)
+        actions_tensor = tf.convert_to_tensor(self.actions, dtype=tf.int32)
+        rewards_tensor = tf.convert_to_tensor(self.rewards, dtype=tf.float32)
+        next_states_tensor = tf.convert_to_tensor(
+            self.next_states, dtype=tf.float32)
+        done_tensor = tf.convert_to_tensor(self.dones, dtype=tf.float32)
+        log_probs_tensor = tf.stack(self.log_probs)
 
-    def _check_state(self, state):
-        '''
-        This function takes a state parameter and returns the first element of a tuple if state has a length of 2, otherwise it simply returns the state parameter.
+        values = self.value_net(states_tensor).numpy().squeeze(1)
+        next_values = self.value_net(next_states_tensor).numpy().squeeze(1)
 
-        :param state: The state data to be checked.
-        :return: The checked state data.
-        '''
+        if len(next_states_tensor) > 0:
+            last_value = next_values[-1]
+        else:
+            last_value = 0
 
-        state_num = len(state)
-        if state_num == 2:
-            state, _ = state  # Unpack the tuple
-        return state
+        advantages = self.compute_advantages(rewards_tensor.numpy(), np.append(
+            values, last_value), done_tensor.numpy(), self.gamma, self.lam)
+        advantages = (advantages - advantages.mean()) / \
+            (advantages.std() + 1e-5)
+        advantages_tensor = tf.convert_to_tensor(advantages, dtype=tf.float32)
 
-    def learn_reset(self):
-        """
-        Reset the agent's state and episode reward.
-        """
+        if len(advantages) > 1:
+            returns = np.add(advantages[:-1], values[:-1])
+        else:
+            returns = np.add(advantages, values)
 
-        self.state = self.env.reset()
-        return self._check_state(self.state)
+        self.ppo_update(self.ppo_epochs, self.mini_batch_size, states_tensor,
+                        actions_tensor, log_probs_tensor, returns, advantages_tensor)
 
-    def learn_close(self):
-        """
-        Close the environment and reset the agent's total reward, episode count, and episode reward.
-        """
+        self.reset()
+        self.update_episode()
 
-        self.env.close()
-        self.total_reward = 0
-        self.episode = 0
-        self.episode_reward = 0
+    def ppo_update(self, ppo_epochs, mini_batch_size, states, actions, log_probs, returns, advantages, clip_param=0.2):
+        batch_size = states.shape[0]
+        returns = tf.convert_to_tensor(returns, dtype=tf.float32)
+        for _ in range(ppo_epochs):
+            for idx in range(batch_size // mini_batch_size):
+                # Extract mini-batch
+                minibatch_indices = tf.range(
+                    idx * mini_batch_size, (idx + 1) * mini_batch_size)
+                states_minibatch = tf.gather(states, minibatch_indices)
+                actions_minibatch = tf.gather(actions, minibatch_indices)
+                old_log_probs_minibatch = tf.gather(
+                    log_probs, minibatch_indices)
+                returns_minibatch = tf.gather(returns, minibatch_indices)
+                advantages_minibatch = tf.gather(advantages, minibatch_indices)
+
+                # Calculate policy loss
+                with tf.GradientTape() as tape:
+                    new_probs = self.policy_net(states_minibatch)
+                    new_dist = tfp.distributions.Categorical(probs=new_probs)
+                    new_log_probs = new_dist.log_prob(actions_minibatch)
+                    ratio = tf.exp(new_log_probs - old_log_probs_minibatch)
+                    surr1 = ratio * advantages_minibatch
+                    surr2 = tf.clip_by_value(
+                        ratio, 1.0 - clip_param, 1.0 + clip_param) * advantages_minibatch
+                    policy_loss = -tf.reduce_mean(tf.minimum(surr1, surr2))
+
+                # Calculate gradients
+                policy_gradients = tape.gradient(
+                    policy_loss, self.policy_net.trainable_variables)
+                # Apply gradients
+                self.policy_optimizer.apply_gradients(
+                    zip(policy_gradients, self.policy_net.trainable_variables))
+
+                # Calculate value loss
+                with tf.GradientTape() as tape:
+                    current_value_estimate = self.value_net(states_minibatch)
+                    value_loss = tf.reduce_mean(
+                        (returns_minibatch - current_value_estimate) ** 2)
+
+                # Calculate gradients
+                value_gradients = tape.gradient(
+                    value_loss, self.value_net.trainable_variables)
+                # Apply gradients
+                self.value_optimizer.apply_gradients(
+                    zip(value_gradients, self.value_net.trainable_variables))
+
+    def train(self):
+        """
+        Execute the learning loop, where the PPO algorithm is used to train the agent on the specified environment.
+        """
+        self.learn()
 
-    def learn_check(self):
+    def learn(self):
         """
-        Print the episode count, previous reward, episode reward, total reward, and average episode reward.
+        Execute the learning loop, where the PPO algorithm is used to train the agent on the specified environment.
         """
 
-        avg_reward = self.total_reward / (self.episode + 1)
-        Logger.debug(
-            f'Episode: {self.episode}, Previous Reward: {self.prev_reward},  Episode Reward: {self.episode_reward}, Total Reward: {self.total_reward}, Average Episode Reward: {avg_reward}')
-
-    def select_action(self, state):
-        '''
-        These functions are placeholders and must be implemented by the child class that extends this Agent class.
-
-        select_action() function is a placeholder that needs to be implemented in the child class that extends the Agent class. This function takes the current state of the environment and returns the selected action for the agent to take.
-
-        :param state: The current state of the environment.
-        :return: The selected action for the agent to take.
-        '''
-        pass
+        timestep = 0
+        test = 0
+        self.total_reward = 0
 
-    def update(self):
-        '''
-        This function is a placeholder and must be implemented by the child class that extends this Agent class.
+        if self.max_episodes > 0 and self.max_timesteps > 0:
+            is_done = False
+            for episode in range(self.max_episodes):
+                self.episode = episode
+                self.reset()
+                self.learn_reset()
+                self.episode_reward = 0
+                reward = 0
+
+                for t in range(self.max_timesteps):
+                    state_tensor = self.check_tensor(self.state)
+                    action, reward, is_done, timestep = self.learn_step(
+                        state_tensor, timestep)
+                    if is_done:
+                        break
+
+                self.learn_check()
+                avg_reward = self.total_reward / (self.episode + 1)
+
+                if avg_reward >= self.early_stop_threshold > 0:
+                    Logger.info(
+                        f'Early stopping: Average reward has reached the threshold ({self.early_stop_threshold}) at episode {self.episode}')
+                    break
+                if is_done and self.done_loop_end:
+                    break
 
-        update() function is a placeholder that needs to be implemented in the child class that extends the Agent class. This function is responsible for updating the agent's state, action, and policy based on the new state and reward received from the environment.
+                if self.episode + 1 >= self.max_episodes:
+                    break
 
-        No parameters are passed into this function and it does not return anything.
-        '''
-        pass
+            self.env.close()
+        else:
+            self.reset()
 
-    def update_step(self, state, action, reward, done, next_state):
+    def learn_next(self):
         """
-        Updates the provided state, action, reward, done, and next_state.
+        Perform a single learning step and update the episode and total rewards.
 
-        :param state: The current state of the environment.
-        :type state: numpy.ndarray
-        :param action: The action taken by the agent.
-        :type action: int
-        :param reward: The reward for the current step.
-        :type reward: float
-        :param done: Flag to mark if the episode is done or not.
-        :type done: bool
-        :param next_state: The next state after the current action.
-        :type next_state: numpy.ndarray
+        :return: The action taken, the resulting reward, and whether the episode is done or not.
+        :rtype: tuple(torch.Tensor, float, bool)
         """
 
-        self.update_reward(reward)
-
-        self.states.append(state)
-        self.actions.append(action)
-        self.rewards.append(reward)
-        self.dones.append(done)
-        self.next_states.append(next_state)
+        action, reward, is_done, timestep = self.learn_step(self.state, -1)
 
-        if done:
-            self.update()
+        return action, reward, is_done, timestep
 
-    def save_policy_value(self, file_name):
+    def learn_close(self):
         """
-        Save the policy and value networks and their optimizer states in a file.
-
-        :param file_name: The name of the file to save the networks and optimizer states.
-        :type file_name: str
+        Close the environment and reset the agent's total reward, episode count, and episode reward.
         """
 
-        torch.save({
-            'policy_net_state_dict': self.policy_net.state_dict(),
-            'value_net_state_dict': self.value_net.state_dict(),
-            'policy_optimizer_state_dict': self.policy_optimizer.state_dict(),
-            'value_optimizer_state_dict': self.value_optimizer.state_dict(),
-        }, file_name)
+        super().learn_close()
 
-    def load_policy_value(self, file_name):
+    def learn_check(self):
         """
-        Load the policy and value networks and their optimizer states from a file.
-
-        :param file_name: The name of the file to load the networks and optimizer states from.
-        :type file_name: str
+        Print the episode count, previous reward, episode reward, total reward, and average episode reward.
         """
 
-        checkpoint = torch.load(file_name)
-        self.policy_net.load_state_dict(checkpoint['policy_net_state_dict'])
-        self.value_net.load_state_dict(checkpoint['value_net_state_dict'])
-        self.policy_optimizer.load_state_dict(
-            checkpoint['policy_optimizer_state_dict'])
-        self.value_optimizer.load_state_dict(
-            checkpoint['value_optimizer_state_dict'])
+        super().learn_check()
 
-    def save_actor_critic(self, file_name):
+    def save_model(self, file_name):
         """
-        Save the actor-critic network and its optimizer state in a file.
+        This function saves the model to the specified file.
 
-        :param file_name: The name of the file to save the network and optimizer state.
-        :type file_name: str
+        :param file_name: The name of the file to save the model to.
+        :return: None
         """
+        self.save(file_name)
 
-        torch.save({
-            'actor_critic_net_state_dict': self.actor_critic_net.state_dict(),
-            'optimizer_state_dict': self.actor_critic_optimizer.state_dict(),
-        }, file_name)
-
-    def load_actor_critic(self, file_name):
+    def save(self, file_name):
         """
-        Load the actor-critic network and its optimizer state from a file.
+        This function saves the policy and value networks to the specified file.
 
-        :param file_name: The name of the file to load the network and optimizer state from.
-        :type file_name: str
+        :param file_name: The name of the file to save the policy and value networks to.
+        :return: None
         """
 
-        checkpoint = torch.load(file_name)
-        self.actor_critic_net.load_state_dict(
-            checkpoint['actor_critic_net_state_dict'])
-        self.actor_critic_optimizer.load_state_dict(
-            checkpoint['optimizer_state_dict'])
+        self.save_policy_value(file_name)
 
-    def step_unpack(self, step_output):
-        step_output_num = len(step_output)
-        if step_output_num == 4:
-            next_state, reward, is_done, _ = step_output
-        elif step_output_num == 5:
-            next_state, reward, is_done, _, _ = step_output
-        return next_state, reward, is_done
+    def load_model(self, file_name):
+        """
+        This function loads the model from the specified file.
 
-    def update_reward(self, reward):
-        self.episode_reward += reward
-        self.total_reward += reward
-        self.prev_reward = reward
+        :param file_name: The name of the file to load the model from.
+        :return: None
+        """
+        self.load(file_name)
 
-    def update_episode(self):
-        self.episode += 1
-        self.episode_reward = 0
+    def load(self, file_name):
+        """
+        This function loads the policy and value networks from the specified file.
 
-    def convert_float_to_double(self, input_tensor):
-        if input_tensor.dtype == torch.float32:
-            return input_tensor.double()
-        else:
-            return input_tensor
+        :param file_name: The name of the file to load the policy and value networks from.
+        :return: None
+        """
 
-    def ensure_float(self, input_tensor):
-        if input_tensor.dtype == torch.float64:
-            return input_tensor.float()
-        else:
-            return input_tensor
+        self.load_policy_value(file_name)
```

### Comparing `modular_rl-0.3.3/modular_rl/agents/_custom.py` & `modular_rl-0.4.0/modular_rl/agents/_custom.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,22 @@
 
 from LogAssist.log import Logger
 from modular_rl.envs._custom import CustomEnv
 
 
 class AgentCustom:
     def __init__(self, env, setting):
+        """
+        :param env: The environment for the agent to interact with. It should be an instance of a compatible environment class. If None is provided, a default CustomEnv environment will be used.
+        :type env: object
+        :param setting: The setting configuration for the agent, specifying various learning parameters and settings.
+        :type setting: dict
+        :return: None
+        """
+
         self.env = env if env else CustomEnv()
         self.setting = setting
 
         # Set learn episode parameters
         self.episode_reward = 0
         self.total_reward = 0
         self.prev_reward = 0
```

### Comparing `modular_rl-0.3.3/modular_rl/agents/mcis.py` & `modular_rl-0.4.0/modular_rl/agents/tensorflow/mcis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 """
 ModularRL project
 
 Copyright (c) 2023 horrible-gh
 
 Class AgentMCIS is an implementation of the Monte Carlo Importance Sampling (MCIS) algorithm.
 The algorithm is used for solving problems of sequential decision making under uncertainty.
@@ -14,26 +13,26 @@
 
 Importance Sampling is used to estimate the properties of a particular target distribution, given some observed data and a proposal distribution.
 This implementation makes use of Monte Carlo methods, which rely on repeated random sampling to obtain numerical results.
 
 This software includes the following third-party libraries:
 Gym (MIT License): https://github.com/openai/gym - Copyright (c) OpenAI.
 NumPy (BSD License): https://numpy.org - Copyright (c) NumPy Developers.
-PyTorch (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
+TensorFlow (Apache License 2.0): https://www.tensorflow.org/ - Copyright (c) TensorFlow Developers.
 """
 
-import torch
-from torch.distributions import Categorical
-import torch.nn.functional as F
-from modular_rl.util.node import Node
-from modular_rl.agents._agent import Agent
+import tensorflow as tf
+import tensorflow_probability as tfp
 import numpy as np
+from LogAssist.log import Logger
+from modular_rl.agents.tensorflow._agent import Agent
+from modular_rl.util.node import Node
 
 
-class AgentMCIS(Agent):
+class TensorFlowAgentMCIS(Agent):
     def __init__(self, env, setting):
         """
         Initialize the AgentMCIS class with the specified environment and settings.
 
         :param env: The environment to use for training.
         :type env: gym.Env or None
         :param setting: The settings for the MCIS algorithm.
@@ -46,54 +45,91 @@
         # mcis parameters
         self.num_simulations = setting.get('num_simulations', 800)
         self.cpuct = setting.get('cpuct', 1.0)
         self.temperature = setting.get('temperature', 1.0)
 
         self.device = setting.get('device', None)
         if self.device == None:
-            self.device = torch.device(
-                "cuda" if torch.cuda.is_available() else "cpu")
+            # TensorFlow automatically uses the GPU if one is available, otherwise it uses the CPU.
+            # Therefore, there is no need to manually set the device as in PyTorch.
+            pass
 
-    def select_action(self, state):
+    def update_step(self, state, action, reward, done, next_state):
         """
-        Select an action using mcis.
+        Updates the provided state, action, reward, done, and next_state.
 
-        :param state: The current state.
+        :param state: The current state of the environment.
         :type state: numpy.ndarray
-        :return: The selected action.
-        :rtype: int
+        :param action: The action taken by the agent.
+        :type action: int
+        :param reward: The reward for the current step.
+        :type reward: float
+        :param done: Flag to mark if the episode is done or not.
+        :type done: bool
+        :param next_state: The next state after the current action.
+        :type next_state: numpy.ndarray
         """
 
-        state_tensor = self.check_tensor(state).to(self.device)
+        self.update_reward(reward)
+
+        self.states.append(tf.squeeze(state))  # change here
+        self.actions.append(action)
+        self.rewards.append(reward)
+        self.dones.append(done)
+        self.next_states.append(tf.squeeze(next_state))  # change here
+
+        if done:
+            self.update()
+
+    def select_action(self, state):
+        state_tensor = tf.convert_to_tensor(
+            self.check_tensor(state), dtype=tf.float32)
         action_probs, _ = self.actor_critic_net(state_tensor)
-        action_probs = action_probs.detach().numpy().flatten()
+        action_probs = action_probs.numpy().flatten()
         root = Node(state, action_probs)
         for _ in range(self.num_simulations):
             node = root
             search_path = [node]
             while node.expanded():
-                action, node = node.select_child(self.cpuct)
-                search_path.append(node)
+                best_score = -np.inf
+                best_action = -1
+                for action, child in node.children.items():
+                    uct_score = child.get_score(self.cpuct)
+                    if np.any(uct_score > best_score):
+                        best_score = uct_score
+                        best_action = action
+
+                if best_action != -1:
+                    action = best_action
+                    node = node.children[action]
+                    search_path.append(node)
+                else:
+                    break
+
             if len(search_path) > 1:
                 parent, action = search_path[-2], search_path[-1].action
             else:
                 parent, action = search_path[0], None
             if True not in self.dones:  # Check if the game is not over
-                state_tensor = self.check_tensor(node.state).to(self.device)
+                state_tensor = tf.convert_to_tensor(
+                    self.check_tensor(node.state), dtype=tf.float32)
                 action_probs, value = self.actor_critic_net(state_tensor)
                 action_space = self.env.action_space.n
                 node.expand(action_space, action_probs, False)
-            state_tensor = self.check_tensor(node.state).to(self.device)
+            state_tensor = tf.convert_to_tensor(
+                self.check_tensor(node.state), dtype=tf.float32)
             _, value = self.actor_critic_net(state_tensor)
-            self.backpropagate(search_path, value.item(), node.done)
-        root_state_tensor = self.check_tensor(
-            root.state).to(self.device)  # This line is added
+            self.backpropagate(search_path, value.numpy(), node.done)
+        root_state_tensor = tf.convert_to_tensor(
+            self.check_tensor(root.state), dtype=tf.float32)
         action_probs, _ = self.actor_critic_net(root_state_tensor)
+        action_probs = action_probs.numpy().flatten()  # make sure it is a flat array
+        Logger.verb('mcis:select_action:action_probs', f'{action_probs}')
         chosen_action = np.random.choice(
-            range(len(action_probs)), p=action_probs.detach().numpy())
+            range(len(action_probs)), p=action_probs)  # choosing from the range of all possible actions
         return chosen_action
 
     def backpropagate(self, search_path, reward, done):
         """
         Backpropagate the value estimates back to the root node.
 
         :param search_path: The nodes visited during the search.
@@ -103,62 +139,23 @@
         :param done: Whether the episode has ended.
         :type done: bool
         """
         for node in reversed(search_path):
             node.update_stats(reward)
             if not done:
                 if isinstance(node.state, np.ndarray):
-                    state_tensor = torch.from_numpy(
-                        node.state).float().to(self.device)
-                elif torch.is_tensor(node.state):
-                    state_tensor = node.state.float().to(self.device)
+                    state_tensor = tf.convert_to_tensor(
+                        node.state, dtype=tf.float32)
+                elif tf.is_tensor(node.state):
+                    state_tensor = node.state
                 else:
                     raise ValueError(
-                        "node.state must be a numpy array or torch tensor")
+                        "node.state must be a numpy array or tensorflow tensor")
                 _, reward = self.actor_critic_net(state_tensor)
-                reward = reward.item()
-
-    def learn(self):
-        """
-        Train the agent.
-        """
-        self.train()
-
-    def train(self):
-        """
-        Train the agent.
-        """
-        self.total_reward = 0
-        for episode in range(self.max_episodes):
-            self.episode = episode
-            state = self.learn_reset()
-
-            for t in range(self.max_timesteps):
-                state = self._check_state(state)
-                self.state_tensor = self.check_tensor(state).squeeze(0)
-
-                # Select an action
-                action = self.select_action(self.state_tensor)
-
-                # Take a step in the environment
-                step_out = self.env.step(action)
-                next_state, reward, done = self.step_unpack(step_out)
-
-                # Update the agent's experience
-                self.update_step(state, action, reward, done, next_state)
-
-                # Update the network parameters at the end of the episode
-                if done:
-                    self.update()
-                    self.learn_check()
-                    break
-
-                state = next_state
-
-            self.episode += 1
+                reward = reward.numpy()
 
     def compute_loss(self, state, action, reward, next_state, done):
         '''
         This function computes the actor and critic loss using the provided state, action, reward, next_state, and done variables.
         The actor loss is computed based on the policy gradient algorithm,
         and the critic loss is computed as the mean squared error between the estimated value of the current state and the target value of the next state.
 
@@ -177,85 +174,119 @@
         :param done: A flag indicating whether the episode has ended.
         :return: The computed actor and critic loss values.
         '''
 
         # Predict action probabilities and values
         action_probs, values = self.actor_critic_net(state)
 
-        # Logger.verb('agents:mcis:compute_loss',f'{self.actor_critic_net(next_state)}')
-
         # Compute the value loss
         actor_output, critic_output = self.actor_critic_net(next_state)
         target_values = reward + self.gamma * \
-            torch.mean(critic_output) * (1 - done)
-        target_values = target_values.unsqueeze(1)
-        critic_loss = F.mse_loss(values, target_values.detach())
+            tf.reduce_mean(critic_output) * (1 - done)
+        target_values = tf.expand_dims(target_values, 1)
+        critic_loss = tf.keras.losses.MSE(
+            values, tf.stop_gradient(target_values))
 
         # Compute the policy loss
-        m = Categorical(action_probs)
+        m = tfp.distributions.Categorical(probs=action_probs)
         logprobs = m.log_prob(self.check_tensor(action))
-        actor_loss = -logprobs * (target_values - values).detach()
+        actor_loss = -logprobs * tf.stop_gradient(target_values - values)
 
         # Take mean of actor_loss and critic_loss
-        actor_loss = actor_loss.mean()
-        critic_loss = critic_loss.mean()
+        actor_loss = tf.reduce_mean(actor_loss)
+        critic_loss = tf.reduce_mean(critic_loss)
 
         return actor_loss, critic_loss
 
     def update(self):
         """
         This function updates the network parameters using the optimizer and computed loss values.
         """
 
         if not self.states:  # Check if the states list is empty
             return
 
-        # Logger.verb('agents:mcis:update',f'states={self.states},actions={self.actions},rewards={self.rewards},dones={self.dones}')
-
         # Prepare data
-        states_tensor = torch.stack(
-            [self.check_tensor(state) for state in self.states]).to(self.device)
-        actions_tensor = torch.Tensor(self.actions).to(self.device)
-        rewards_tensor = torch.Tensor(self.rewards).to(self.device)
-        next_states_tensor = torch.stack(
-            [self.check_tensor(state) for state in self.next_states]).to(self.device)
-        dones_tensor = torch.Tensor(self.dones).to(self.device)
-
-        # Compute loss
-        actor_loss, critic_loss = self.compute_loss(
-            states_tensor, actions_tensor, rewards_tensor, next_states_tensor, dones_tensor)
+        states_tensor = tf.stack(
+            [self.check_tensor(state) for state in self.states])
+        actions_tensor = tf.convert_to_tensor(self.actions, dtype=tf.float32)
+        rewards_tensor = tf.convert_to_tensor(self.rewards, dtype=tf.float32)
+        next_states_tensor = tf.stack(
+            [self.check_tensor(state) for state in self.next_states])
+        dones_tensor = tf.convert_to_tensor(self.dones, dtype=tf.float32)
 
         # Compute gradients and update network parameters
-        self.actor_critic_optimizer.zero_grad()
-        loss = actor_loss + critic_loss
-        loss.backward()
-        self.actor_critic_optimizer.step()
+        with tf.GradientTape() as tape:
+            # Compute loss
+            actor_loss, critic_loss = self.compute_loss(
+                states_tensor, actions_tensor, rewards_tensor, next_states_tensor, dones_tensor)
+            loss = actor_loss + critic_loss
+
+        # Calculate gradients
+        gradients = tape.gradient(
+            loss, self.actor_critic_net.trainable_variables)
+
+        # Apply gradients
+        self.actor_critic_optimizer.apply_gradients(
+            zip(gradients, self.actor_critic_net.trainable_variables))
 
         # Reset the lists for the next episode
         self.reset()
         self.update_episode()
 
-    def check_tensor(self, state):
-        '''
-        This function checks if the provided object is a PyTorch tensor, and if not, converts it to a tensor.
+    def learn(self):
+        """
+        Train the agent.
+        """
+        self.train()
+
+    def train(self):
+        """
+        Train the agent.
+        """
+        self.total_reward = 0
+        for episode in range(self.max_episodes):
+            self.episode = episode
+            state = self.learn_reset()
+
+            for t in range(self.max_timesteps):
+                state = self._check_state(state)
+                Logger.verb('mcis:train', f'{state.shape}')
+                self.state_tensor = self.check_tensor(state).numpy()
 
-        check_tensor() function checks if the provided obj parameter is a PyTorch tensor.
-        If it is not a tensor, it converts it to a tensor using torch.FloatTensor().
-        If it is already a tensor, it simply returns the tensor.
+                # Select an action
+                action = self.select_action(self.state_tensor)
 
-        The obj parameter is the object to check/convert to a PyTorch tensor.
+                # Take a step in the environment
+                step_out = self.env.step(action)
+                next_state, reward, done = self.step_unpack(step_out)
 
-        The function returns the input object as a PyTorch tensor.
+                # Update the agent's experience
+                self.update_step(state, action, reward, done, next_state)
 
-        :param obj: The object to check/convert to a PyTorch tensor.
-        :return: The input object as a PyTorch tensor.
+                # Update the network parameters at the end of the episode
+                if done:
+                    self.update()
+                    self.learn_check()
+                    break
+
+                state = next_state
+
+            self.episode += 1
+
+    def check_tensor(self, state):
         '''
+        This function checks if the provided object is a TensorFlow tensor, and if not, converts it to a tensor.
 
-        if not isinstance(state, torch.Tensor):
-            state = torch.tensor(state, dtype=torch.float32)
+        :param state: The object to check/convert to a TensorFlow tensor.
+        :return: The input object as a TensorFlow tensor.
+        '''
+        Logger.verb('_agent:check_tensor', f'state={state}')
+        if not isinstance(state, tf.Tensor):
+            state = tf.convert_to_tensor(state, dtype=tf.float32)
         return state
 
     def save_model(self, file_name):
         """
         This function saves the model to the specified file.
 
         :param file_name: The name of the file to save the model to.
```

### Comparing `modular_rl-0.3.3/modular_rl/agents/mcts.py` & `modular_rl-0.4.0/modular_rl/agents/tensorflow/mcts.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,52 +11,49 @@
 It has methods to predict an action given a state, perform a learning step, update the neural network parameters,
 save and load a checkpoint, and reset learning parameters.
 The class also has instance variables to keep track of episode and total rewards, previous reward, and average reward.
 
 This software includes the following third-party libraries:
 Gym (MIT License): https://github.com/openai/gym - Copyright (c) OpenAI.
 NumPy (BSD License): https://numpy.org - Copyright (c) NumPy Developers.
-PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
+TensorFlow (Apache License 2.0): https://www.tensorflow.org/ - Copyright (c) TensorFlow Developers.
 """
 
-import torch
+import tensorflow as tf
+import tensorflow_probability as tfp
 import numpy as np
-from torch.distributions import Categorical
-import torch.nn.functional as F
-from modular_rl.util.node import Node
-from modular_rl.agents._agent import Agent
 from LogAssist.log import Logger
+from modular_rl.agents.tensorflow._agent import Agent
+from modular_rl.util.node import Node
 
 
-class AgentMCTS(Agent):
+class TensorFlowAgentMCTS(Agent):
     def __init__(self, env, setting):
         """
-        Initialize the AgentMCTS class with the specified environment and settings.
+        Initialize the AgentMCIS class with the specified environment and settings.
 
         :param env: The environment to use for training.
         :type env: gym.Env or None
-        :param setting: The settings for the MCTS algorithm.
+        :param setting: The settings for the MCIS algorithm.
         :type setting: AgentSettings
         """
 
         super().__init__(env, setting)
         super().init_actor_critic()
 
-        # MCTS parameters
+        # mcis parameters
         self.num_simulations = setting.get('num_simulations', 800)
         self.cpuct = setting.get('cpuct', 1.0)
         self.temperature = setting.get('temperature', 1.0)
-        self.gamma = 0.95
-        self.total_value = 0
 
         self.device = setting.get('device', None)
         if self.device == None:
-            self.device = torch.device(
-                "cuda" if torch.cuda.is_available() else "cpu")
-        self.reset()
+            # TensorFlow automatically uses the GPU if one is available, otherwise it uses the CPU.
+            # Therefore, there is no need to manually set the device as in PyTorch.
+            pass
 
     def reset(self):
         self.state = None
         self.action = None
         self.reward = None
         self.done = None
         self.total_reward = 0
@@ -66,20 +63,20 @@
         Select an action using MCTS.
 
         :param state: The current state.
         :type state: numpy.ndarray
         :return: The selected action.
         :rtype: int
         """
-
-        state_tensor = self.check_tensor(self._check_state(state))
+        state = self._check_state(state)
+        state_tensor = self.check_tensor(state)
         action_probs, _ = self.actor_critic_net(state_tensor)
-        action_probs = action_probs.detach()
-        m = Categorical(action_probs)
-        chosen_action = m.sample().item()
+        action_probs = tf.stop_gradient(action_probs)
+        m = tfp.distributions.Categorical(probs=action_probs)
+        chosen_action = m.sample().numpy().item()
 
         # Use uniform prior for root node.
         root = Node(state, [1 / self.env.action_space.n]
                     * self.env.action_space.n)
 
         for _ in range(self.num_simulations):
             node, search_path = root, [root]
@@ -94,18 +91,18 @@
                 search_path) > 1 else (search_path[0], None)
             step_output = self.env.step(action) if action is not None else (
                 parent.state, 0, False, None)
             state, reward, done, *_ = step_output
             Logger.verb('mcts:select_action', f"Step Output Reward: {reward}")
 
             if not done:
-                state_tensor = self.check_tensor(state).to(self.device)
+                state_tensor = self.check_tensor(state)
                 action_probs, _ = self.actor_critic_net(state_tensor)
                 node.expand(self.env.action_space.n,
-                            action_probs.detach().cpu().numpy().flatten(), False)
+                            action_probs.numpy().flatten(), False)
 
             self.backpropagate(search_path, reward, done)
 
         chosen_action_node = root.children[chosen_action]
 
         self.state = chosen_action_node.state
         self.action = chosen_action
@@ -128,153 +125,165 @@
         :type done: bool
         """
         for node in reversed(search_path):
             # Logger.verb('mcts:backpropagate',
             #            f"Node Reward({reward}) after Update Stats: {node.total_value}")
             node.update_stats(reward)
 
-    def learn(self):
-        """
-        Train the agent.
-        """
-        self.train()
-
-    def train(self):
-        """
-        Train the agent.
-        """
-        self.total_reward = 0
-        for episode in range(self.max_episodes):
-            self.episode = episode
-            state = self.learn_reset()
-            # state = self.env.reset()
-
-            for t in range(self.max_timesteps):
-                state = self._check_state(state)
-                self.state_tensor = self.check_tensor(state).squeeze(0)
-                self.next_state, self.action, self.reward, self.done = self.select_action(
-                    self.state_tensor)
-
-                self.learn_check()
-
-                if self.done:
-                    # self.update()
-                    break
-
-                self.update()
-
-                state = self.next_state
-
-            self.episode += 1
-            # print(f"Episode: {self.episode}, Reward: {self.total_reward}")
-
     def compute_loss(self, state, action, reward, done):
         '''
-        This function computes the actor and critic loss using the provided state, action, reward, next_state, and done variables.
+        This function computes the actor and critic loss using the provided state, action, reward, and done variables.
         The actor loss is computed based on the policy gradient algorithm,
         and the critic loss is computed as the mean squared error between the estimated value of the current state and the target value of the next state.
 
-        compute_loss() function computes the actor and critic loss values for the provided state, action, reward, next_state, and done variables.
-
-        The state parameter is the current state of the environment.
-        The action parameter is the action taken in the current state.
-        The reward parameter is the reward received for taking the action in the current state.
-        The next_state parameter is the state resulting from taking the action in the current state.
-        The done parameter is a flag indicating whether the episode has ended.
-
         :param state: The current state of the environment.
         :param action: The action taken in the current state.
         :param reward: The reward received for taking the action in the current state.
-        :param next_state: The state resulting from taking the action in the current state.
         :param done: A flag indicating whether the episode has ended.
         :return: The computed actor and critic loss values.
         '''
         # Predict action probabilities and values
         state = self.ensure_float(state)
         action_probs, values = self.actor_critic_net(state)
 
-        # Compute the value loss
         # Convert reward to tensor
-        reward = torch.tensor(reward, device=self.device)
-        # Convert total_value to tensor
-        total_value = torch.tensor(self.total_value, device=self.device)
-        target_values = reward + self.gamma * total_value * (1 - done)
-        target_values = target_values.unsqueeze(0)
-        critic_loss = F.mse_loss(values, target_values.detach())
+        reward = tf.convert_to_tensor(reward, dtype=tf.float32)
+        # Compute the value loss
+        target_values = reward + self.gamma * self.total_value * (1 - done)
+        target_values = tf.expand_dims(target_values, axis=0)
+        critic_loss = tf.keras.losses.MSE(values, target_values)
 
         # If action is not a list or tuple or its length is zero, initialize it with zeros
         if not isinstance(action, (list, tuple)) or len(action) == 0:
-            action = torch.zeros_like(action_probs)
+            action = tf.zeros_like(action_probs)
 
         # Compute the policy loss
-        m = Categorical(action_probs)
+        m = tfp.distributions.Categorical(probs=action_probs)
         logprobs = m.log_prob(self.check_tensor(action))
-        actor_loss = -logprobs * (target_values - values).detach()
+        actor_loss = -logprobs * (target_values - values)
 
         # Average the actor and critic loss
-        loss = (actor_loss.mean() + critic_loss.mean()) / 2
+        loss = (tf.reduce_mean(actor_loss) + tf.reduce_mean(critic_loss)) / 2
 
         return loss
 
+    def ensure_float(self, tensor):
+        if tensor.dtype != tf.float32:
+            return tf.cast(tensor, tf.float32)
+        return tensor
+
     def update(self):
         '''
         This function updates the network parameters using the optimizer and computed loss values.
 
         update() function updates the network parameters using the optimizer and computed loss values.
         It uses the compute_loss() function to compute the loss and the optimizer object to perform the optimization step.
 
         This function does not take any parameters and does not return anything.
 
         :return: None
         '''
 
-        # Update the network
         # Convert state to tensor
-        state_tensor = torch.tensor(self.state, device=self.device)
+        state_tensor = self.check_tensor(self.state)
 
-        # Update the network
-        self.actor_critic_optimizer.zero_grad()
-        loss = self.compute_loss(
-            state_tensor, self.action, self.reward, self.done)
-        Logger.verb('mcts:update',
-                    f"Loss: {loss.item()}, Reward: {self.reward}")
-        loss.backward()
-        self.actor_critic_optimizer.step()
+        # Compute loss and update network parameters
+        with tf.GradientTape() as tape:
+            loss = self.compute_loss(
+                state_tensor, self.action, self.reward, self.done)
+            Logger.verb('mcts:update',
+                        f"Loss: {loss.numpy()}, Reward: {self.reward}")
+
+        # Calculate gradients
+        gradients = tape.gradient(
+            loss, self.actor_critic_net.trainable_variables)
+
+        # Apply gradients
+        self.actor_critic_optimizer.apply_gradients(
+            zip(gradients, self.actor_critic_net.trainable_variables))
 
         self.reset()
 
     def check_tensor(self, obj):
         '''
-        This function checks if the provided object is a PyTorch tensor, and if not, converts it to a tensor.
+        This function checks if the provided object is a TensorFlow tensor, and if not, converts it to a tensor.
 
-        check_tensor() function checks if the provided obj parameter is a PyTorch tensor.
-        If it is not a tensor, it converts it to a tensor using torch.FloatTensor().
+        check_tensor() function checks if the provided obj parameter is a TensorFlow tensor.
+        If it is not a tensor, it converts it to a tensor using tf.convert_to_tensor().
         If it is already a tensor, it simply returns the tensor.
 
-        The obj parameter is the object to check/convert to a PyTorch tensor.
+        The obj parameter is the object to check/convert to a TensorFlow tensor.
 
-        The function returns the input object as a PyTorch tensor.
+        The function returns the input object as a TensorFlow tensor.
 
-        :param obj: The object to check/convert to a PyTorch tensor.
-        :return: The input object as a PyTorch tensor.
+        :param obj: The object to check/convert to a TensorFlow tensor.
+        :return: The input object as a TensorFlow tensor.
         '''
 
-        if not torch.is_tensor(obj):
-            obj_tensor = torch.FloatTensor(obj)
+        if not tf.is_tensor(obj):
+            obj_tensor = tf.convert_to_tensor(obj, dtype=tf.float32)
         else:
             obj_tensor = obj
 
         Logger.verb('mcts:check_tensor', f"Before remapping: {obj_tensor}")
         obj_tensor = obj_tensor % self.env.action_space.n
-        obj_tensor = torch.where(
+        obj_tensor = tf.where(
             obj_tensor >= self.env.action_space.n, self.env.action_space.n - 1, obj_tensor)
-        obj_tensor = torch.round(obj_tensor)
+        obj_tensor = self._check_state(tf.round(obj_tensor))
         Logger.verb('mcts:check_tensor', f"After remapping: {obj_tensor}")
         return obj_tensor
 
+    def learn(self):
+        """
+        Train the agent.
+        """
+        self.train()
+
+    def train(self):
+        """
+        Train the agent.
+        """
+        self.total_reward = 0
+        for episode in range(self.max_episodes):
+            self.episode = episode
+            state = self.learn_reset()
+
+            for t in range(self.max_timesteps):
+                state = self._check_state(state)
+                self.state_tensor = self.check_tensor(state).numpy()
+                self.state_tensor = tf.squeeze(self.state_tensor, axis=0)
+                self.next_state, self.action, self.reward, self.done = self.select_action(
+                    self.state_tensor)
+
+                self.learn_check()
+
+                if self.done:
+                    break
+
+                self.update()
+
+                state = self.next_state
+
+            self.episode += 1
+            # print(f"Episode: {self.episode}, Reward: {self.total_reward}")
+
+    def update_step(self, state, action, reward, done, next_state):
+        """
+        In MCTS, update_step is not necessary as the agent is updated
+        after every simulation (or a batch of simulations), each of which
+        represents an entire episode. Thus, this method can be left blank or removed.
+        """
+        self.state = state
+        self.action = action
+        self.reward = reward
+        self.done = done
+        self.next_state = next_state
+        self.update_reward(reward)
+        self.update_episode()
+
     def save_model(self, file_name):
         """
         This function saves the model to the specified file.
 
         :param file_name: The name of the file to save the model to.
         :return: None
         """
@@ -304,21 +313,7 @@
         This function loads the actor critic network from the specified file.
 
         :param file_name: The name of the file to load the actor critic network from.
         :return: None
         """
 
         self.load_actor_critic(file_name)
-
-    def update_step(self, state, action, reward, done, next_state):
-        """
-        In MCTS, update_step is not necessary as the agent is updated
-        after every simulation (or a batch of simulations), each of which
-        represents an entire episode. Thus, this method can be left blank or removed.
-        """
-        self.state = state
-        self.action = action
-        self.reward = reward
-        self.done = done
-        self.next_state = next_state
-        self.update_reward(reward)
-        self.update_episode()
```

### Comparing `modular_rl-0.3.3/modular_rl/agents/mim.py` & `modular_rl-0.4.0/modular_rl/agents/mim.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,524 +1,524 @@
-"""
-ModularRL project
-
-Copyright (c) 2023 horrible-gh
-
-Class AgentMIM is an implementation of the Modular's sIMulator (MIM) algorithm.
-It takes an environment and a setting configuration as inputs, initializes various simulation parameters,
-and sets various simulation elements such as fixed states, unknown spaces, simulation states, excluded states, score calculation method, and simulation number.
-
-It has methods to perform a simulation given a state, calculate skewness and kurtosis of the simulation result, rank the simulation result array, and adjust weights based on the simulation result.
-The class also keeps track of the simulation iteration count, average standard deviations, skews, and kurtosises of the simulation results.
-
-This software includes the following third-party libraries:
-NumPy (BSD License): https://numpy.org - Copyright (c) NumPy Developers.
-"""
-
-import random
-import numpy as np
-from LogAssist.log import Logger
-from modular_rl.agents._custom import AgentCustom
-from modular_rl.params.mim import ParamMIM
-
-
-class AgentMIM(AgentCustom):
-    def __init__(self, env, setting):
-        """
-        Initialize the AgentMIM class with the specified environment and settings.
-
-        :param env: The environment to use for training.
-        :type env: gym.Env or None
-        :param setting: The settings for the MIM algorithm.
-        :type setting: AgentSettings
-        """
-        super().__init__(env, setting)
-        # The name to use for the fixed states in the simulation.
-        self.fixed_states_name = 'fixed_states'
-        # The name to use for the unknown spaces in the simulation.
-        self.unknown_spaces_name = 'unknown_spaces'
-        # The name to use for the simulation states.
-        self.simulation_states_name = 'simulation_states'
-        # The name to use for the excluded states in the simulation.
-        self.excluded_states_name = 'excluded_states'
-        # The name to use for the simulation number.
-        self.my_simulation_number_name = 'my_simulation_number'
-        # The name to use for the score table.
-        self.score_table_name = 'score_table'
-        # The name to use for the score calculation callback function.
-        self.score_calculation_callback_name = 'score_calculation_callback'
-        self.score_column = setting.get(  # The name of the score column in the score table.
-            'score_column', ParamMIM.default['score_column'])
-        self.simulation_iterations = setting.get(  # The number of iterations for each simulation.
-            'simulation_iterations', ParamMIM.default['simulation_iterations'])
-        self.superior_rank_adjustment_factor = setting.get(  # The adjustment factor applied to actions that are ranked superior.
-            'superior_rank_adjustment_factor', ParamMIM.default['superior_rank_adjustment_factor'])
-        self.inferior_rank_adjustment_factor = setting.get(  # The adjustment factor applied to actions that are ranked inferior.
-            'inferior_rank_adjustment_factor', ParamMIM.default['inferior_rank_adjustment_factor'])
-        self.std_deviation_factor = setting.get(
-            'std_deviation_factor', ParamMIM.default['std_deviation_factor'])
-        self.skewness_factor = setting.get(
-            'skewness_factor', ParamMIM.default['skewness_factor'])
-        self.kurtosis_factor = setting.get(
-            'kurtosis_factor', ParamMIM.default['kurtosis_factor'])
-
-        # Counter for the number of simulation iterations.
-        self.simulation_iteration_indexes_count = 0
-        # Average of standard deviations for all simulations.
-        self.standard_deviations_avg = 0
-        self.skews_avg = 0  # Average skewness for all simulations.
-        self.kurtosises_avg = 0  # Average kurtosis for all simulations.
-        self.reset()  # Reset the simulation results.
-
-    def simulate(self, state):
-        """
-        Simulates the given state with various conditions and adjustments.
-        It extracts the required elements from the state, performs multiple simulations,
-        calculates the score, and records the statistics of each simulation.
-
-        :param state: The state to be simulated.
-        :type state: dict
-        """
-
-        required_state_elements = {
-            self.fixed_states_name: 'fixed_state',
-            self.unknown_spaces_name: 'unknown_spaces',
-            self.simulation_states_name: 'simulation_states',
-            self.excluded_states_name: 'excluded_states',
-            self.score_calculation_callback_name: 'score_calculation_callback',
-            self.my_simulation_number_name: 'my_simulation_number',
-            self.score_table_name: 'score_table',
-        }
-
-        for element_key, error_obj in required_state_elements.items():
-            if state.get(element_key) is None:
-                raise Exception(
-                    f"'{error_obj}' not found in the provided state for simulation.")
-
-        fixed_states = state[self.fixed_states_name]
-        unknown_spaces = state[self.unknown_spaces_name]
-        simulation_states = state[self.simulation_states_name]
-        excluded_states = state[self.excluded_states_name]
-        score_calculation_callback = state[self.score_calculation_callback_name]
-        self.my_simulation_number = state[self.my_simulation_number_name]
-        score_table = state[self.score_table_name]
-        self.risk_table = state.get('risk_table', None)
-        remaining_states = set(simulation_states) - set(excluded_states)
-        simulation_table = []
-
-        Logger.verb(
-            'mim:simulate', f'{self.simulation_states_name},{list(remaining_states)}, {simulation_states}')
-
-        self.reset()
-
-        if len(fixed_states) != len(unknown_spaces):
-            return simulation_table
-
-        for fixed_state in fixed_states:
-            remaining_states -= set(fixed_state)
-
-        for i, fixed_state in enumerate(fixed_states):
-            simulation_table.append([0 for _ in score_table])
-            self.simulation_iteration_indexes.append(0)
-            for _ in range(self.simulation_iterations):
-                self.simulation_iteration_indexes[i] += 1
-                # Logger.verb('mim:simulate:fixed_states,unkonwn_spaces,remaining_states ',f'{fixed_states}, {unknown_spaces}, {list(remaining_states)}, {i}')
-                sample_states = random.sample(
-                    list(remaining_states), unknown_spaces[i])
-                simulated_result = fixed_state + sample_states
-                # Logger.verb('mim:simulate',simulated_result)
-                score_obj = score_calculation_callback(simulated_result)
-                score = score_obj[self.score_column] if self.score_column else score_obj
-                for idx in range(len(score_table)-1):
-                    # Logger.verb('mim:simulate',f'{score}, {score_table}')
-                    if score_table[idx] <= score <= score_table[idx+1]:
-                        simulation_table[i][idx] += 1
-                        break
-                if unknown_spaces[i] == 0:
-                    break
-
-        Logger.verb('mim:simulation_table', simulation_table)
-        for index in range(len(simulation_table)):
-            sim_result = 0
-            for sub_index in range(len(simulation_table[index])):
-                sim_result += simulation_table[index][sub_index] * \
-                    sub_index + 0.0001
-            self.simulation_totals.append(sim_result)
-            self.simulation_averages.append(
-                sim_result / self.simulation_iteration_indexes[index])
-            self.standard_deviations.append(np.std(simulation_table[index]))
-            skewness, kurtosis = self.calc_skewness_kurtosis(
-                simulation_table[index])
-            self.skews.append(skewness)
-            self.kurtosises.append(kurtosis)
-
-        Logger.verb('simulator:simulation_totals', self.simulation_totals)
-        Logger.verb('simulator:simulation_averages', self.simulation_averages)
-        Logger.verb('simulator:standard_deviations', self.standard_deviations)
-        Logger.verb('simulator:skews', self.skews)
-        Logger.verb('simulator:kurtosises', self.kurtosises)
-
-    def calc_skewness_kurtosis(self, data):
-        """
-        Calculates the skewness and kurtosis of the given data.
-
-        :param data: The data for which to calculate skewness and kurtosis.
-        :type data: list or array-like
-        :return: The skewness and kurtosis of the data.
-        :rtype: tuple
-        """
-
-        n = len(data)
-        mean = np.mean(data)
-        std_dev = np.std(data)
-
-        skewness = (1/n) * sum((x - mean)**3 for x in data) / (std_dev**3)
-        kurtosis = (1/n) * sum((x - mean)**4 for x in data) / (std_dev**4) - 3
-
-        return skewness, kurtosis
-
-    def rank_array(self, array):
-        """
-        Ranks the elements in the array in descending order.
-
-        :param array: The array to be ranked.
-        :type array: list or array-like
-        :return: The ranks of the elements in the array.
-        :rtype: numpy.ndarray
-        """
-
-        temp = array.argsort()
-        ranks = np.empty_like(temp)
-        ranks[temp] = len(array) - (np.arange(len(array)))
-
-        return ranks
-
-    def calculate_weight_adjustment_factors(self, simulation_size):
-        """
-        Calculates the adjustment factors for the weights of the simulations.
-
-        :param simulation_size: The size of the simulation.
-        :type simulation_size: int
-        :return: The adjustment factors for the weights of the simulations.
-        :rtype: list
-        """
-
-        weight_adjustment_factors = [1] * simulation_size
-        factors = [
-            self.std_deviation_factor,
-            self.skewness_factor,
-            self.kurtosis_factor,
-        ]
-        averages = [self.standard_deviations_avg,
-                    self.skews_avg, self.kurtosises_avg]
-        values = [self.standard_deviations, self.skews, self.kurtosises]
-
-        for index in range(simulation_size):
-            for factor, average, value in zip(factors, averages, values):
-                if average < value[index]:
-                    weight_adjustment_factor = factor * average / value[index]
-                    weight_adjustment_factors[index] += weight_adjustment_factor - factor
-        return weight_adjustment_factors
-
-    def update_averages(self, total_size):
-        """
-        Updates the averages of standard deviations, skews, and kurtosises.
-
-        :param total_size: The total size of the simulations.
-        :type total_size: int
-        """
-
-        factors = [self.standard_deviations_avg,
-                   self.skews_avg, self.kurtosises_avg]
-        values = [self.standard_deviations, self.skews, self.kurtosises]
-        for factor, value in zip(factors, values):
-            factor = (
-                factor * self.simulation_iteration_indexes_count + sum(value)) / total_size
-        self.simulation_iteration_indexes_count = total_size
-
-    def calculate_action_weights(self, adjusted_averages, skip_myself):
-        """
-        Calculates the weights for each action.
-
-        :param adjusted_averages: The adjusted averages from the simulations.
-        :type adjusted_averages: list
-        :param skip_myself: Whether to skip the current instance in the calculation.
-        :type skip_myself: bool
-        :return: The weights for each action.
-        :rtype: list
-        """
-
-        Logger.verb('mim:calculate_action_weights:adjusted_averages',
-                    adjusted_averages)
-        Logger.verb('mim:calculate_action_weights:my_simulation_average',
-                    self.my_simulation_average)
-        averages_table = []
-        if skip_myself:
-            averages_table.insert(0, self.my_simulation_average)
-        averages_table.extend(adjusted_averages)
-        Logger.verb('mim:calculate_action_weights:averages_table',
-                    averages_table)
-        ranks = self.rank_array(np.array(averages_table))
-        Logger.verb('mim:calculate_action_weights:ranks', f'{ranks}')
-
-        base_weight = int(1 / self.env.action_space * 100)
-        action_scale = self.env.action_space / len(ranks)
-        action_weights = [base_weight for _ in range(self.env.action_space)]
-        check_weights = [False for _ in range(self.env.action_space)]
-
-        Logger.verb('mim:calculate_action_weights:check_base_weight',
-                    f'{base_weight},{action_scale},{action_weights}')
-
-        my_rank = ranks[0]
-        my_average = self.my_simulation_average
-        my_action_rank = my_rank
-        my_action_rank = self.env.action_space - \
-            round(my_rank * action_scale)
-        if my_rank == 1 and action_scale >= 1.5:
-            my_action_rank = self.env.action_space - 1
-        if my_action_rank < 0:
-            my_action_rank = 0
-
-        for rank_idx in range(len(ranks)):
-            Logger.verb('mim:calculate_action_weights:rank_idx',
-                        rank_idx)
-            if rank_idx != 0:
-                rank_diff = abs(my_rank - ranks[rank_idx])
-                Logger.verb('mim:calculate_action_weights:rank_diff',
-                            rank_diff)
-                if my_rank < ranks[rank_idx]:
-                    average_weight = (averages_table[rank_idx] /
-                                      my_average) * (self.superior_rank_adjustment_factor ** rank_diff)
-                else:
-                    average_weight = (my_average /
-                                      averages_table[rank_idx]) * (self.inferior_rank_adjustment_factor ** rank_diff)
-
-                Logger.verb('mim:calculate_action_weights:scale,num',
-                            f'{action_scale}, {rank_idx}, {average_weight}')
-
-                action_num = self.env.action_space - \
-                    round(ranks[rank_idx] * action_scale)
-                if ranks[rank_idx] == 1 and action_scale >= 1.5:
-                    action_num = self.env.action_space - 1
-                if action_num < 0:
-                    action_num = 0
-                Logger.verb('mim:calculate_action_weights:action_num',
-                            action_num)
-
-                if check_weights[action_num] == False:
-                    check_weights[action_num] = True
-                    expect_weight = action_weights[action_num] * \
-                        average_weight
-                    weight_diff = action_weights[action_num] - expect_weight
-                    Logger.verb('mim:calculate_action_weights:weight_diff',
-                                f'{weight_diff}, {expect_weight}')
-                    action_weights[action_num] -= weight_diff
-                    if action_weights[action_num] < 1:
-                        action_weights[action_num] = 1
-                    action_weights[my_action_rank] += weight_diff
-                    Logger.verb('mim:calculate_action_weights:scale,num',
-                                f'{action_num}, {action_weights[action_num]}, {my_action_rank}, {action_weights[my_action_rank]}, {average_weight}')
-
-        for action_num in range(len(action_weights)):
-            if action_weights[action_num] in (0, int(1 / self.env.action_space * 100)):
-                prev_action_weights = action_weights[action_num-1]
-                next_action_weights = action_weights[action_num+1]
-                middle_weight = (prev_action_weights + next_action_weights) / 2
-                action_weights[action_num] = round(middle_weight)
-
-        if self.risk_table:
-            risk_total = sum(self.risk_table)
-            if risk_total != 0:
-                action_weight_total = 0
-                action_weight = 0
-                for risk_num in range(len(self.risk_table)):
-                    action_weight += action_weights[risk_num] * \
-                        self.risk_table[risk_num]
-                    action_weights[risk_num] -= action_weight
-                    action_weight_total += action_weight
-
-                risk_weight = [risk_total-self.risk_table[risk_num]
-                               for risk_num in range(len(self.risk_table))]
-                risk_total = sum(risk_weight)
-
-                Logger.verb('mim:calculate_action_weights:risk_weight,risk_total',
-                            f'{risk_weight},{risk_total}')
-
-                for risk_num in range(len(risk_weight)):
-                    if risk_total != 0:
-                        action_weights[risk_num] += action_weight_total * \
-                            risk_weight[risk_num] / risk_total
-
-        Logger.verb('mim:calculate_action_weights:action_weights',
-                    action_weights)
-        return action_weights
-
-    def calculate_weights(self):
-        """
-        Calculates the weights for the actions based on the simulation results.
-
-        :return: The calculated weights for each action.
-        :rtype: list
-        """
-
-        skip_myself = False
-        skip_count = 0
-
-        if self.simulation_iteration_indexes[self.my_simulation_number] <= 1:
-            skip_myself = True
-            skip_count = 1
-
-        self.my_simulation_average = self.simulation_averages[self.my_simulation_number]
-
-        if skip_myself:
-            del self.simulation_iteration_indexes[self.my_simulation_number]
-            del self.simulation_averages[self.my_simulation_number]
-            del self.standard_deviations[self.my_simulation_number]
-            del self.skews[self.my_simulation_number]
-            del self.kurtosises[self.my_simulation_number]
-
-        simulation_size = len(self.simulation_averages)
-        simulation_total_size = self.simulation_iteration_indexes_count + simulation_size
-
-        self.update_averages(simulation_total_size)
-        weight_adjustment_factors = self.calculate_weight_adjustment_factors(
-            simulation_size)
-
-        adjusted_averages = [average * factor for average,
-                             factor in zip(self.simulation_averages, weight_adjustment_factors)]
-        action_weights = self.calculate_action_weights(
-            adjusted_averages, skip_myself)
-
-        return action_weights
-
-    def select_action(self, state):
-        action_list = []
-        if isinstance(self.env.action_space, int) != True:
-            raise Exception("action space be not an integer")
-        else:
-            action_table = list(range(self.env.action_space))
-        self.simulate(state)
-        action_weights = self.calculate_weights()
-        Logger.verb('mim:select_action', action_weights)
-        for action_index in range(len(action_weights)):
-            for _ in range(int(action_weights[action_index])):
-                action_list.append(action_index)
-
-        random.shuffle(action_list)
-        choice = random.choice(action_list)
-        return action_table[choice]
-
-    def update_step(self, reward, done):
-        """
-        This method updates the agent at each step in the environment.
-        It takes as input the reward from the last action and a boolean indicating if the episode has ended.
-
-        :param reward: The reward received after executing an action
-        :type reward: int/float
-        :param done: Indicates if the episode has ended
-        :type done: bool
-        """
-        self.update_reward(reward)
-        # self.states.append(state)
-        # self.actions.append(action)
-        # self.rewards.append(reward)
-        # self.dones.append(done)
-        # self.next_states.append(next_state)
-        if done:
-            self.update()
-
-    def update(self):
-        """
-        This method is intended to update the internal model or values based on the collected rewards or experiences.
-        Currently, it's just a placeholder and does nothing. Further implementation is needed.
-        """
-        pass
-
-    def reset(self):
-        """
-        This method resets the agent's internal data. It's typically called at the end of each episode.
-        It clears out various lists that store information about the simulations.
-        """
-        self.simulation_totals = []
-        self.simulation_iteration_indexes = []
-        self.simulation_averages = []
-        self.standard_deviations = []
-        self.skews = []
-        self.kurtosises = []
-
-    def train(self):
-        """
-        Train the agent.
-        """
-        self.learn()
-
-    def learn(self):
-        """
-        Train the agent.
-        """
-        self.total_reward = 0
-        for episode in range(self.max_episodes):
-            self.episode = episode
-            state = self.learn_reset()
-            for t in range(self.max_timesteps):
-                state = self._check_state(state)
-
-                # Select an action
-                action = self.select_action(state)
-                Logger.verb('agents:mim:learn:action', action)
-                # Take a step in the environment
-                next_state, reward, done = self.env.step(action)
-                # Update the agent's experience
-                self.update_step(reward, done)
-                # Update the network parameters at the end of the episode
-                if done:
-                    self.update()
-                    self.learn_check()
-                    break
-                state = next_state
-            self.episode += 1
-
-    def load(self, file_name):
-        """
-        Loads the simulation statistics from the given file.
-
-        :param file_name: The name of the file from which to load the statistics.
-        :type file_name: str
-        """
-        self.load_model(file_name)
-
-    def load_model(self, file_name):
-        """
-        Loads the simulation statistics from the given file.
-
-        :param file_name: The name of the file from which to load the statistics.
-        :type file_name: str
-        """
-        data_arr = np.load(file_name)
-        self.simulation_iteration_indexes_count = data_arr[0]
-        self.standard_deviations_avg = data_arr[1]
-        self.skews_avg = data_arr[2]
-        self.kurtosises_avg = data_arr[3]
-
-    def save(self, file_name):
-        """
-        Saves the simulation statistics to the given file.
-
-        :param file_name: The name of the file to which to save the statistics.
-        :type file_name: str
-        """
-        self.save_model(file_name)
-
-    def save_model(self, file_name):
-        """
-        Saves the simulation statistics to the given file.
-
-        :param file_name: The name of the file to which to save the statistics.
-        :type file_name: str
-        """
-        data_arr = [
-            self.simulation_iteration_indexes_count,
-            self.standard_deviations_avg,
-            self.skews_avg,
-            self.kurtosises_avg,
-        ]
-        np.save(file_name, data_arr)
+"""
+ModularRL project
+
+Copyright (c) 2023 horrible-gh
+
+Class AgentMIM is an implementation of the Modular's sIMulator (MIM) algorithm.
+It takes an environment and a setting configuration as inputs, initializes various simulation parameters,
+and sets various simulation elements such as fixed states, unknown spaces, simulation states, excluded states, score calculation method, and simulation number.
+
+It has methods to perform a simulation given a state, calculate skewness and kurtosis of the simulation result, rank the simulation result array, and adjust weights based on the simulation result.
+The class also keeps track of the simulation iteration count, average standard deviations, skews, and kurtosises of the simulation results.
+
+This software includes the following third-party libraries:
+NumPy (BSD License): https://numpy.org - Copyright (c) NumPy Developers.
+"""
+
+import random
+import numpy as np
+from LogAssist.log import Logger
+from modular_rl.agents._custom import AgentCustom
+from modular_rl.params.mim import ParamMIM
+
+
+class AgentMIM(AgentCustom):
+    def __init__(self, env, setting):
+        """
+        Initialize the AgentMIM class with the specified environment and settings.
+
+        :param env: The environment to use for training.
+        :type env: gym.Env or None
+        :param setting: The settings for the MIM algorithm.
+        :type setting: AgentSettings
+        """
+        super().__init__(env, setting)
+        # The name to use for the fixed states in the simulation.
+        self.fixed_states_name = 'fixed_states'
+        # The name to use for the unknown spaces in the simulation.
+        self.unknown_spaces_name = 'unknown_spaces'
+        # The name to use for the simulation states.
+        self.simulation_states_name = 'simulation_states'
+        # The name to use for the excluded states in the simulation.
+        self.excluded_states_name = 'excluded_states'
+        # The name to use for the simulation number.
+        self.my_simulation_number_name = 'my_simulation_number'
+        # The name to use for the score table.
+        self.score_table_name = 'score_table'
+        # The name to use for the score calculation callback function.
+        self.score_calculation_callback_name = 'score_calculation_callback'
+        self.score_column = setting.get(  # The name of the score column in the score table.
+            'score_column', ParamMIM.default['score_column'])
+        self.simulation_iterations = setting.get(  # The number of iterations for each simulation.
+            'simulation_iterations', ParamMIM.default['simulation_iterations'])
+        self.superior_rank_adjustment_factor = setting.get(  # The adjustment factor applied to actions that are ranked superior.
+            'superior_rank_adjustment_factor', ParamMIM.default['superior_rank_adjustment_factor'])
+        self.inferior_rank_adjustment_factor = setting.get(  # The adjustment factor applied to actions that are ranked inferior.
+            'inferior_rank_adjustment_factor', ParamMIM.default['inferior_rank_adjustment_factor'])
+        self.std_deviation_factor = setting.get(
+            'std_deviation_factor', ParamMIM.default['std_deviation_factor'])
+        self.skewness_factor = setting.get(
+            'skewness_factor', ParamMIM.default['skewness_factor'])
+        self.kurtosis_factor = setting.get(
+            'kurtosis_factor', ParamMIM.default['kurtosis_factor'])
+
+        # Counter for the number of simulation iterations.
+        self.simulation_iteration_indexes_count = 0
+        # Average of standard deviations for all simulations.
+        self.standard_deviations_avg = 0
+        self.skews_avg = 0  # Average skewness for all simulations.
+        self.kurtosises_avg = 0  # Average kurtosis for all simulations.
+        self.reset()  # Reset the simulation results.
+
+    def simulate(self, state):
+        """
+        Simulates the given state with various conditions and adjustments.
+        It extracts the required elements from the state, performs multiple simulations,
+        calculates the score, and records the statistics of each simulation.
+
+        :param state: The state to be simulated.
+        :type state: dict
+        """
+
+        required_state_elements = {
+            self.fixed_states_name: 'fixed_state',
+            self.unknown_spaces_name: 'unknown_spaces',
+            self.simulation_states_name: 'simulation_states',
+            self.excluded_states_name: 'excluded_states',
+            self.score_calculation_callback_name: 'score_calculation_callback',
+            self.my_simulation_number_name: 'my_simulation_number',
+            self.score_table_name: 'score_table',
+        }
+
+        for element_key, error_obj in required_state_elements.items():
+            if state.get(element_key) is None:
+                raise Exception(
+                    f"'{error_obj}' not found in the provided state for simulation.")
+
+        fixed_states = state[self.fixed_states_name]
+        unknown_spaces = state[self.unknown_spaces_name]
+        simulation_states = state[self.simulation_states_name]
+        excluded_states = state[self.excluded_states_name]
+        score_calculation_callback = state[self.score_calculation_callback_name]
+        self.my_simulation_number = state[self.my_simulation_number_name]
+        score_table = state[self.score_table_name]
+        self.risk_table = state.get('risk_table', None)
+        remaining_states = set(simulation_states) - set(excluded_states)
+        simulation_table = []
+
+        Logger.verb(
+            'mim:simulate', f'{self.simulation_states_name},{list(remaining_states)}, {simulation_states}')
+
+        self.reset()
+
+        if len(fixed_states) != len(unknown_spaces):
+            return simulation_table
+
+        for fixed_state in fixed_states:
+            remaining_states -= set(fixed_state)
+
+        for i, fixed_state in enumerate(fixed_states):
+            simulation_table.append([0 for _ in score_table])
+            self.simulation_iteration_indexes.append(0)
+            for _ in range(self.simulation_iterations):
+                self.simulation_iteration_indexes[i] += 1
+                # Logger.verb('mim:simulate:fixed_states,unkonwn_spaces,remaining_states ',f'{fixed_states}, {unknown_spaces}, {list(remaining_states)}, {i}')
+                sample_states = random.sample(
+                    list(remaining_states), unknown_spaces[i])
+                simulated_result = fixed_state + sample_states
+                # Logger.verb('mim:simulate',simulated_result)
+                score_obj = score_calculation_callback(simulated_result)
+                score = score_obj[self.score_column] if self.score_column else score_obj
+                for idx in range(len(score_table)-1):
+                    # Logger.verb('mim:simulate',f'{score}, {score_table}')
+                    if score_table[idx] <= score <= score_table[idx+1]:
+                        simulation_table[i][idx] += 1
+                        break
+                if unknown_spaces[i] == 0:
+                    break
+
+        Logger.verb('mim:simulation_table', simulation_table)
+        for index in range(len(simulation_table)):
+            sim_result = 0
+            for sub_index in range(len(simulation_table[index])):
+                sim_result += simulation_table[index][sub_index] * \
+                    sub_index + 0.0001
+            self.simulation_totals.append(sim_result)
+            self.simulation_averages.append(
+                sim_result / self.simulation_iteration_indexes[index])
+            self.standard_deviations.append(np.std(simulation_table[index]))
+            skewness, kurtosis = self.calc_skewness_kurtosis(
+                simulation_table[index])
+            self.skews.append(skewness)
+            self.kurtosises.append(kurtosis)
+
+        Logger.verb('simulator:simulation_totals', self.simulation_totals)
+        Logger.verb('simulator:simulation_averages', self.simulation_averages)
+        Logger.verb('simulator:standard_deviations', self.standard_deviations)
+        Logger.verb('simulator:skews', self.skews)
+        Logger.verb('simulator:kurtosises', self.kurtosises)
+
+    def calc_skewness_kurtosis(self, data):
+        """
+        Calculates the skewness and kurtosis of the given data.
+
+        :param data: The data for which to calculate skewness and kurtosis.
+        :type data: list or array-like
+        :return: The skewness and kurtosis of the data.
+        :rtype: tuple
+        """
+
+        n = len(data)
+        mean = np.mean(data)
+        std_dev = np.std(data)
+
+        skewness = (1/n) * sum((x - mean)**3 for x in data) / (std_dev**3)
+        kurtosis = (1/n) * sum((x - mean)**4 for x in data) / (std_dev**4) - 3
+
+        return skewness, kurtosis
+
+    def rank_array(self, array):
+        """
+        Ranks the elements in the array in descending order.
+
+        :param array: The array to be ranked.
+        :type array: list or array-like
+        :return: The ranks of the elements in the array.
+        :rtype: numpy.ndarray
+        """
+
+        temp = array.argsort()
+        ranks = np.empty_like(temp)
+        ranks[temp] = len(array) - (np.arange(len(array)))
+
+        return ranks
+
+    def calculate_weight_adjustment_factors(self, simulation_size):
+        """
+        Calculates the adjustment factors for the weights of the simulations.
+
+        :param simulation_size: The size of the simulation.
+        :type simulation_size: int
+        :return: The adjustment factors for the weights of the simulations.
+        :rtype: list
+        """
+
+        weight_adjustment_factors = [1] * simulation_size
+        factors = [
+            self.std_deviation_factor,
+            self.skewness_factor,
+            self.kurtosis_factor,
+        ]
+        averages = [self.standard_deviations_avg,
+                    self.skews_avg, self.kurtosises_avg]
+        values = [self.standard_deviations, self.skews, self.kurtosises]
+
+        for index in range(simulation_size):
+            for factor, average, value in zip(factors, averages, values):
+                if average < value[index]:
+                    weight_adjustment_factor = factor * average / value[index]
+                    weight_adjustment_factors[index] += weight_adjustment_factor - factor
+        return weight_adjustment_factors
+
+    def update_averages(self, total_size):
+        """
+        Updates the averages of standard deviations, skews, and kurtosises.
+
+        :param total_size: The total size of the simulations.
+        :type total_size: int
+        """
+
+        factors = [self.standard_deviations_avg,
+                   self.skews_avg, self.kurtosises_avg]
+        values = [self.standard_deviations, self.skews, self.kurtosises]
+        for factor, value in zip(factors, values):
+            factor = (
+                factor * self.simulation_iteration_indexes_count + sum(value)) / total_size
+        self.simulation_iteration_indexes_count = total_size
+
+    def calculate_action_weights(self, adjusted_averages, skip_myself):
+        """
+        Calculates the weights for each action.
+
+        :param adjusted_averages: The adjusted averages from the simulations.
+        :type adjusted_averages: list
+        :param skip_myself: Whether to skip the current instance in the calculation.
+        :type skip_myself: bool
+        :return: The weights for each action.
+        :rtype: list
+        """
+
+        Logger.verb('mim:calculate_action_weights:adjusted_averages',
+                    adjusted_averages)
+        Logger.verb('mim:calculate_action_weights:my_simulation_average',
+                    self.my_simulation_average)
+        averages_table = []
+        if skip_myself:
+            averages_table.insert(0, self.my_simulation_average)
+        averages_table.extend(adjusted_averages)
+        Logger.verb('mim:calculate_action_weights:averages_table',
+                    averages_table)
+        ranks = self.rank_array(np.array(averages_table))
+        Logger.verb('mim:calculate_action_weights:ranks', f'{ranks}')
+
+        base_weight = int(1 / self.env.action_space * 100)
+        action_scale = self.env.action_space / len(ranks)
+        action_weights = [base_weight for _ in range(self.env.action_space)]
+        check_weights = [False for _ in range(self.env.action_space)]
+
+        Logger.verb('mim:calculate_action_weights:check_base_weight',
+                    f'{base_weight},{action_scale},{action_weights}')
+
+        my_rank = ranks[0]
+        my_average = self.my_simulation_average
+        my_action_rank = my_rank
+        my_action_rank = self.env.action_space - \
+            round(my_rank * action_scale)
+        if my_rank == 1 and action_scale >= 1.5:
+            my_action_rank = self.env.action_space - 1
+        if my_action_rank < 0:
+            my_action_rank = 0
+
+        for rank_idx in range(len(ranks)):
+            Logger.verb('mim:calculate_action_weights:rank_idx',
+                        rank_idx)
+            if rank_idx != 0:
+                rank_diff = abs(my_rank - ranks[rank_idx])
+                Logger.verb('mim:calculate_action_weights:rank_diff',
+                            rank_diff)
+                if my_rank < ranks[rank_idx]:
+                    average_weight = (averages_table[rank_idx] /
+                                      my_average) * (self.superior_rank_adjustment_factor ** rank_diff)
+                else:
+                    average_weight = (my_average /
+                                      averages_table[rank_idx]) * (self.inferior_rank_adjustment_factor ** rank_diff)
+
+                Logger.verb('mim:calculate_action_weights:scale,num',
+                            f'{action_scale}, {rank_idx}, {average_weight}')
+
+                action_num = self.env.action_space - \
+                    round(ranks[rank_idx] * action_scale)
+                if ranks[rank_idx] == 1 and action_scale >= 1.5:
+                    action_num = self.env.action_space - 1
+                if action_num < 0:
+                    action_num = 0
+                Logger.verb('mim:calculate_action_weights:action_num',
+                            action_num)
+
+                if check_weights[action_num] == False:
+                    check_weights[action_num] = True
+                    expect_weight = action_weights[action_num] * \
+                        average_weight
+                    weight_diff = action_weights[action_num] - expect_weight
+                    Logger.verb('mim:calculate_action_weights:weight_diff',
+                                f'{weight_diff}, {expect_weight}')
+                    action_weights[action_num] -= weight_diff
+                    if action_weights[action_num] < 1:
+                        action_weights[action_num] = 1
+                    action_weights[my_action_rank] += weight_diff
+                    Logger.verb('mim:calculate_action_weights:scale,num',
+                                f'{action_num}, {action_weights[action_num]}, {my_action_rank}, {action_weights[my_action_rank]}, {average_weight}')
+
+        for action_num in range(len(action_weights)):
+            if action_weights[action_num] in (0, int(1 / self.env.action_space * 100)):
+                prev_action_weights = action_weights[action_num-1]
+                next_action_weights = action_weights[action_num+1]
+                middle_weight = (prev_action_weights + next_action_weights) / 2
+                action_weights[action_num] = round(middle_weight)
+
+        if self.risk_table:
+            risk_total = sum(self.risk_table)
+            if risk_total != 0:
+                action_weight_total = 0
+                action_weight = 0
+                for risk_num in range(len(self.risk_table)):
+                    action_weight += action_weights[risk_num] * \
+                        self.risk_table[risk_num]
+                    action_weights[risk_num] -= action_weight
+                    action_weight_total += action_weight
+
+                risk_weight = [risk_total-self.risk_table[risk_num]
+                               for risk_num in range(len(self.risk_table))]
+                risk_total = sum(risk_weight)
+
+                Logger.verb('mim:calculate_action_weights:risk_weight,risk_total',
+                            f'{risk_weight},{risk_total}')
+
+                for risk_num in range(len(risk_weight)):
+                    if risk_total != 0:
+                        action_weights[risk_num] += action_weight_total * \
+                            risk_weight[risk_num] / risk_total
+
+        Logger.verb('mim:calculate_action_weights:action_weights',
+                    action_weights)
+        return action_weights
+
+    def calculate_weights(self):
+        """
+        Calculates the weights for the actions based on the simulation results.
+
+        :return: The calculated weights for each action.
+        :rtype: list
+        """
+
+        skip_myself = False
+        skip_count = 0
+
+        if self.simulation_iteration_indexes[self.my_simulation_number] <= 1:
+            skip_myself = True
+            skip_count = 1
+
+        self.my_simulation_average = self.simulation_averages[self.my_simulation_number]
+
+        if skip_myself:
+            del self.simulation_iteration_indexes[self.my_simulation_number]
+            del self.simulation_averages[self.my_simulation_number]
+            del self.standard_deviations[self.my_simulation_number]
+            del self.skews[self.my_simulation_number]
+            del self.kurtosises[self.my_simulation_number]
+
+        simulation_size = len(self.simulation_averages)
+        simulation_total_size = self.simulation_iteration_indexes_count + simulation_size
+
+        self.update_averages(simulation_total_size)
+        weight_adjustment_factors = self.calculate_weight_adjustment_factors(
+            simulation_size)
+
+        adjusted_averages = [average * factor for average,
+                             factor in zip(self.simulation_averages, weight_adjustment_factors)]
+        action_weights = self.calculate_action_weights(
+            adjusted_averages, skip_myself)
+
+        return action_weights
+
+    def select_action(self, state):
+        action_list = []
+        if isinstance(self.env.action_space, int) != True:
+            raise Exception("action space be not an integer")
+        else:
+            action_table = list(range(self.env.action_space))
+        self.simulate(state)
+        action_weights = self.calculate_weights()
+        Logger.verb('mim:select_action', action_weights)
+        for action_index in range(len(action_weights)):
+            for _ in range(int(action_weights[action_index])):
+                action_list.append(action_index)
+
+        random.shuffle(action_list)
+        choice = random.choice(action_list)
+        return action_table[choice]
+
+    def update_step(self, reward, done):
+        """
+        This method updates the agent at each step in the environment.
+        It takes as input the reward from the last action and a boolean indicating if the episode has ended.
+
+        :param reward: The reward received after executing an action
+        :type reward: int/float
+        :param done: Indicates if the episode has ended
+        :type done: bool
+        """
+        self.update_reward(reward)
+        # self.states.append(state)
+        # self.actions.append(action)
+        # self.rewards.append(reward)
+        # self.dones.append(done)
+        # self.next_states.append(next_state)
+        if done:
+            self.update()
+
+    def update(self):
+        """
+        This method is intended to update the internal model or values based on the collected rewards or experiences.
+        Currently, it's just a placeholder and does nothing. Further implementation is needed.
+        """
+        pass
+
+    def reset(self):
+        """
+        This method resets the agent's internal data. It's typically called at the end of each episode.
+        It clears out various lists that store information about the simulations.
+        """
+        self.simulation_totals = []
+        self.simulation_iteration_indexes = []
+        self.simulation_averages = []
+        self.standard_deviations = []
+        self.skews = []
+        self.kurtosises = []
+
+    def train(self):
+        """
+        Train the agent.
+        """
+        self.learn()
+
+    def learn(self):
+        """
+        Train the agent.
+        """
+        self.total_reward = 0
+        for episode in range(self.max_episodes):
+            self.episode = episode
+            state = self.learn_reset()
+            for t in range(self.max_timesteps):
+                state = self._check_state(state)
+
+                # Select an action
+                action = self.select_action(state)
+                Logger.verb('agents:mim:learn:action', action)
+                # Take a step in the environment
+                next_state, reward, done = self.env.step(action)
+                # Update the agent's experience
+                self.update_step(reward, done)
+                # Update the network parameters at the end of the episode
+                if done:
+                    self.update()
+                    self.learn_check()
+                    break
+                state = next_state
+            self.episode += 1
+
+    def load(self, file_name):
+        """
+        Loads the simulation statistics from the given file.
+
+        :param file_name: The name of the file from which to load the statistics.
+        :type file_name: str
+        """
+        self.load_model(file_name)
+
+    def load_model(self, file_name):
+        """
+        Loads the simulation statistics from the given file.
+
+        :param file_name: The name of the file from which to load the statistics.
+        :type file_name: str
+        """
+        data_arr = np.load(file_name)
+        self.simulation_iteration_indexes_count = data_arr[0]
+        self.standard_deviations_avg = data_arr[1]
+        self.skews_avg = data_arr[2]
+        self.kurtosises_avg = data_arr[3]
+
+    def save(self, file_name):
+        """
+        Saves the simulation statistics to the given file.
+
+        :param file_name: The name of the file to which to save the statistics.
+        :type file_name: str
+        """
+        self.save_model(file_name)
+
+    def save_model(self, file_name):
+        """
+        Saves the simulation statistics to the given file.
+
+        :param file_name: The name of the file to which to save the statistics.
+        :type file_name: str
+        """
+        data_arr = [
+            self.simulation_iteration_indexes_count,
+            self.standard_deviations_avg,
+            self.skews_avg,
+            self.kurtosises_avg,
+        ]
+        np.save(file_name, data_arr)
```

### Comparing `modular_rl-0.3.3/modular_rl/agents/ppo.py` & `modular_rl-0.4.0/modular_rl/agents/pytorch/ppo.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,384 +1,390 @@
-
-# -*- coding: utf-8 -*-
-"""
-ModularRL project
-
-Copyright (c) 2023 horrible-gh
-
-Class AgentPPO is an implementation of the Proximal Policy Optimization (PPO) algorithm.
-It takes an environment and a setting configuration as inputs, initializes neural network instances and optimizers,
-and sets various learning parameters.
-It has methods to predict an action given a state, perform a learning step, update the neural network parameters,
-save and load a checkpoint, and reset learning parameters.
-The class also has instance variables to keep track of episode and total rewards, previous reward, and average reward.
-
-This software includes the following third-party libraries:
-Gym (MIT License): https://github.com/openai/gym - Copyright (c) OpenAI.
-NumPy (BSD License): https://numpy.org - Copyright (c) NumPy Developers.
-PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
-"""
-
-import torch
-from torch.distributions import Categorical
-import numpy as np
-from modular_rl.agents._agent import Agent
-from LogAssist.log import Logger
-
-
-class AgentPPO(Agent):
-    def __init__(self, env, setting):
-        """
-        Initialize the AgentPPO class with the specified environment and settings.
-
-        :param env: The environment to use for training.
-        :type env: gym.Env or None
-        :param setting: The settings for the PPO algorithm.
-        :type setting: AgentSettings
-        """
-
-        super().__init__(env, setting)
-        super().init_policy_value()
-
-        # Set learning parameters
-        self.ppo_epochs = setting.get('ppo_epochs', 4)
-        self.mini_batch_size = setting.get('mini_batch_size', 64)
-        self.lam = setting.get('lam', 0.95)
-        self.clip_param = setting.get('clip_param', 0.2)
-
-        # Set learn modular parameters
-        self.state = None
-        self.dist = None
-
-    # Implement PPO algorithm
-
-    def compute_advantages(self, rewards, values, dones, gamma=0.99, lam=0.95):
-        """
-        Compute advantages given the rewards, values, done flags, and discount factors.
-
-        :param rewards: The rewards obtained from the environment.
-        :type rewards: numpy.ndarray
-        :param values: The predicted state-value from the critic network.
-        :type values: numpy.ndarray
-        :param done: The done flags obtained from the environment.
-        :type done: numpy.ndarray
-        :param gamma: The discount factor.
-        :type gamma: float
-        :param lam: The GAE lambda value.
-        :type lam: float
-        :return: The calculated advantages.
-        :rtype: numpy.ndarray
-        """
-
-        advantages = np.zeros_like(rewards)
-        last_advantage = 0
-        for t in reversed(range(len(rewards))):
-            delta = rewards[t] + gamma * \
-                values[t + 1] * (1 - dones[t]) - values[t]
-            advantages[t] = delta + gamma * lam * \
-                last_advantage * (1 - dones[t])
-            last_advantage = advantages[t]
-        return advantages
-
-    def ppo_iter(self, mini_batch_size, states, actions, log_probs, returns, advantages):
-        """
-        Generate random mini-batches of data for PPO algorithm.
-
-        :param mini_batch_size: The size of each mini-batch.
-        :type mini_batch_size: int
-        :param states: The states from the environment.
-        :type states: torch.Tensor
-        :param actions: The actions taken in the environment.
-        :type actions: torch.Tensor
-        :param log_probs: The logarithmic probabilities of the actions.
-        :type log_probs: torch.Tensor
-        :param returns: The calculated returns.
-        :type returns: torch.Tensor
-        :param advantages: The calculated advantages.
-        :type advantages: torch.Tensor
-        :yield: A mini-batch of data.
-        """
-
-        batch_size = states.size(0)
-        for _ in range(batch_size // mini_batch_size):
-            rand_ids = np.random.randint(0, batch_size - 1, mini_batch_size)
-            yield states[rand_ids, :], actions[rand_ids], log_probs[rand_ids], returns[rand_ids], advantages[rand_ids]
-
-    def ppo_update(self, ppo_epochs, mini_batch_size, states, actions, log_probs, returns, advantages, clip_param=0.2):
-        """
-        Perform PPO algorithm for the specified number of epochs.
-
-        :param ppo_epochs: The number of epochs to run PPO algorithm.
-        :type ppo_epochs: int
-        :param mini_batch_size: The size of each mini-batch.
-        :type mini_batch_size: int
-        :param states: The states from the environment.
-        :type states: torch.Tensor
-        :param actions: The actions taken in the environment.
-        :type actions: torch.Tensor
-        :param log_probs: The logarithmic probabilities of the actions.
-        :type log_probs: torch.Tensor
-        :param returns: The calculated returns.
-        :type returns: torch.Tensor
-        :param advantages: The calculated advantages.
-        :type advantages: torch.Tensor
-        :param clip_param: The PPO clipping parameter.
-        :type clip_param: float
-        """
-
-        for _ in range(ppo_epochs):
-            for state, action, old_log_probs, return_, advantage in self.ppo_iter(mini_batch_size, states, actions, log_probs, returns, advantages):
-                dist = Categorical(self.policy_net(state))
-                new_log_probs = dist.log_prob(action)
-
-                ratio = (new_log_probs - old_log_probs).exp()
-                surr1 = ratio * advantage
-                surr2 = torch.clamp(ratio, 1.0 - clip_param,
-                                    1.0 + clip_param) * advantage
-                policy_loss = -torch.min(surr1, surr2).mean()
-
-                value_loss = (return_ - self.value_net(state)).pow(2).mean()
-                self.value_optimizer.zero_grad()
-                value_loss.backward()
-                self.value_optimizer.step()
-
-    def select_action(self, state):
-        """
-        Selects an action based on the given state and the current policy.
-
-        :param state: The state to use for selecting an action.
-        :type state: numpy.ndarray
-        :return: The selected action and its corresponding probability distribution.
-        :rtype: tuple(torch.Tensor, torch.distributions.Categorical)
-        """
-
-        state = self._check_state(self.state)
-        state_tensor = torch.tensor(state, dtype=torch.float32)
-        with torch.no_grad():
-            action_probs = self.policy_net(state_tensor)
-        dist = Categorical(action_probs)
-        self.dist = dist
-        action = dist.sample()
-        return action, dist
-
-    def learn_step(self, state, timestep):
-        """
-        Takes a step in the environment and updates the PPO algorithm with the resulting state, reward, and action.
-
-        :param state: The current state of the environment.
-        :type state: numpy.ndarray
-        :param timestep: The current timestep of the training process.
-        :type timestep: int
-        :return: The action taken, the resulting reward, and whether the episode is done or not.
-        :rtype: tuple(torch.Tensor, float, bool)
-        """
-
-        action, dist = self.select_action(state)
-
-        return self.update_step(state, dist, action, timestep)
-
-    def update_step(self, state, dist, action, timestep, auto_step=True, is_done=False, reward=0, next_state=None):
-        """
-        Updates the Proximal Policy Optimization (PPO) algorithm with the provided state, action, and timestep. This function can either take an environment step based on the given action (auto_step=True) or manually handle state transitions (auto_step=False).
-
-        :param state: The current state of the environment.
-        :type state: numpy.ndarray
-        :param dist: The corresponding probability distribution of the action space.
-        :type dist: torch.distributions.Categorical
-        :param action: The action taken by the agent.
-        :type action: int
-        :param timestep: The current timestep of the training process.
-        :type timestep: int
-        :param auto_step: Flag to determine whether to take an environment step or not. If False, is_done, reward, and next_state should be provided.
-        :type auto_step: bool, optional
-        :param is_done: Flag to mark if the episode is done or not. Should be provided if auto_step is False.
-        :type is_done: bool, optional
-        :param reward: The reward for the current step. Should be provided if auto_step is False.
-        :type reward: float, optional
-        :param next_state: The next state after the current action. If not provided and auto_step is False, it will be assumed to be the same as the current state.
-        :type next_state: numpy.ndarray, optional
-        :return: The action taken, the resulting reward, whether the episode is done or not, and the updated timestep.
-        :rtype: tuple(int, float, bool, int)
-        """
-
-        if dist == None and self.dist:
-            dist = self.dist
-
-        if auto_step:
-            step_output = self.env.step(action.item())
-            next_state, reward, is_done = self.step_unpack(step_output)
-
-        else:
-            if next_state is None:
-                next_state = state
-
-        self.update_reward(reward)
-
-        state = self._check_state(state)
-
-        self.states.append(state)
-        self.actions.append(action)
-        self.rewards.append(reward)
-        self.next_states.append(next_state)
-        self.dones.append(is_done)
-        self.log_probs.append(dist.log_prob(action))
-
-        self.state = next_state
-
-        if timestep > 0:
-            timestep += 1
-
-        if self.update_timestep > 0 and timestep > 0 and (timestep % self.update_timestep == 0):
-            self.update()
-
-        return action, reward, is_done, timestep
-
-    def update(self):
-        """
-        Perform an update of the PPO algorithm, using the stored information about the environment from the previous learning iterations.
-        """
-
-        Logger.verb('agents:ppo:update',
-                    f'states={self.states}, next_states={self.next_states}, actions={self.actions}, rewards={self.rewards}, dones={self.dones}')
-        states_tensor = torch.tensor(np.array(self.states, dtype=np.float32))
-        actions_tensor = torch.tensor(np.array(self.actions))
-        rewards_tensor = torch.tensor(np.array(self.rewards, dtype=np.float32))
-        next_states_tensor = torch.tensor(
-            np.array(self.next_states, dtype=np.float32))
-        done_tensor = torch.tensor(np.array(self.dones, dtype=np.float32))
-        log_probs_tensor = torch.stack(self.log_probs)
-
-        values = self.value_net(states_tensor).detach().squeeze(1)
-        next_values = self.value_net(next_states_tensor).detach().squeeze(1)
-
-        if len(next_states_tensor) > 0:
-            last_value = next_values[-1].item()
-        else:
-            last_value = 0
-
-        advantages = self.compute_advantages(rewards_tensor.numpy(), np.append(
-            values.numpy(), last_value), done_tensor.numpy(), self.gamma, self.lam)
-        advantages = (advantages - advantages.mean()) / \
-            (advantages.std() + 1e-5)
-        advantages_tensor = torch.tensor(advantages, dtype=torch.float32)
-
-        if len(advantages) > 1:
-            returns = np.add(advantages[:-1], values[:-1])
-        else:
-            returns = np.add(advantages, values)
-
-        self.ppo_update(self.ppo_epochs, self.mini_batch_size, states_tensor,
-                        actions_tensor, log_probs_tensor, returns, advantages_tensor)
-
-        self.reset()
-        self.update_episode()
-
-    def train(self):
-        """
-        Execute the learning loop, where the PPO algorithm is used to train the agent on the specified environment.
-        """
-        self.learn()
-
-    def learn(self):
-        """
-        Execute the learning loop, where the PPO algorithm is used to train the agent on the specified environment.
-        """
-
-        timestep = 0
-        test = 0
-        self.total_reward = 0
-
-        if self.max_episodes > 0 and self.max_timesteps > 0:
-            is_done = False
-            for episode in range(self.max_episodes):
-                self.episode = episode
-                self.reset()
-                self.learn_reset()
-                self.episode_reward = 0
-                reward = 0
-
-                for t in range(self.max_timesteps):
-                    action, reward, is_done, timestep = self.learn_step(
-                        self.state, timestep)
-                    if is_done:
-                        break
-
-                self.learn_check()
-                avg_reward = self.total_reward / (self.episode + 1)
-
-                if avg_reward >= self.early_stop_threshold > 0:
-                    Logger.info(
-                        f'Early stopping: Average reward has reached the threshold ({self.early_stop_threshold}) at episode {self.episode}')
-                    break
-                if is_done and self.done_loop_end:
-                    break
-
-                if self.episode + 1 >= self.max_episodes:
-                    break
-
-            self.env.close()
-        else:
-            self.reset()
-
-    def learn_next(self):
-        """
-        Perform a single learning step and update the episode and total rewards.
-
-        :return: The action taken, the resulting reward, and whether the episode is done or not.
-        :rtype: tuple(torch.Tensor, float, bool)
-        """
-
-        action, reward, is_done, timestep = self.learn_step(self.state, -1)
-
-        return action, reward, is_done, timestep
-
-    def learn_close(self):
-        """
-        Close the environment and reset the agent's total reward, episode count, and episode reward.
-        """
-
-        super().learn_close()
-
-    def learn_check(self):
-        """
-        Print the episode count, previous reward, episode reward, total reward, and average episode reward.
-        """
-
-        super().learn_check()
-
-    def save_model(self, file_name):
-        """
-        This function saves the model to the specified file.
-
-        :param file_name: The name of the file to save the model to.
-        :return: None
-        """
-        self.save(file_name)
-
-    def save(self, file_name):
-        """
-        This function saves the policy and value networks to the specified file.
-
-        :param file_name: The name of the file to save the policy and value networks to.
-        :return: None
-        """
-
-        self.save_policy_value(file_name)
-
-    def load_model(self, file_name):
-        """
-        This function loads the model from the specified file.
-
-        :param file_name: The name of the file to load the model from.
-        :return: None
-        """
-        self.load(file_name)
-
-    def load(self, file_name):
-        """
-        This function loads the policy and value networks from the specified file.
-
-        :param file_name: The name of the file to load the policy and value networks from.
-        :return: None
-        """
-
-        self.load_policy_value(file_name)
+
+# -*- coding: utf-8 -*-
+"""
+ModularRL project
+
+Copyright (c) 2023 horrible-gh
+
+Class AgentPPO is an implementation of the Proximal Policy Optimization (PPO) algorithm.
+It takes an environment and a setting configuration as inputs, initializes neural network instances and optimizers,
+and sets various learning parameters.
+It has methods to predict an action given a state, perform a learning step, update the neural network parameters,
+save and load a checkpoint, and reset learning parameters.
+The class also has instance variables to keep track of episode and total rewards, previous reward, and average reward.
+
+This software includes the following third-party libraries:
+Gym (MIT License): https://github.com/openai/gym - Copyright (c) OpenAI.
+NumPy (BSD License): https://numpy.org - Copyright (c) NumPy Developers.
+PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
+"""
+
+import torch
+from torch.distributions import Categorical
+import numpy as np
+from modular_rl.agents.pytorch._agent import Agent
+from LogAssist.log import Logger
+
+
+class PyTorchAgentPPO(Agent):
+    def __init__(self, env, setting):
+        """
+        Initialize the AgentPPO class with the specified environment and settings.
+
+        :param env: The environment to use for training.
+        :type env: gym.Env or None
+        :param setting: The settings for the PPO algorithm.
+        :type setting: AgentSettings
+        """
+
+        super(PyTorchAgentPPO, self).__init__(env, setting)
+        super(PyTorchAgentPPO, self).init_policy_value()
+
+        # Set learning parameters
+        self.ppo_epochs = setting.get('ppo_epochs', 4)
+        self.mini_batch_size = setting.get('mini_batch_size', 64)
+        self.lam = setting.get('lam', 0.95)
+        self.clip_param = setting.get('clip_param', 0.2)
+
+        # Set learn modular parameters
+        self.state = None
+        self.dist = None
+
+    # Implement PPO algorithm
+
+    def learn_reset(self):
+        return super(PyTorchAgentPPO, self).learn_reset()
+
+    def reset(self):
+        super(PyTorchAgentPPO, self).reset()
+
+    def compute_advantages(self, rewards, values, dones, gamma=0.99, lam=0.95):
+        """
+        Compute advantages given the rewards, values, done flags, and discount factors.
+
+        :param rewards: The rewards obtained from the environment.
+        :type rewards: numpy.ndarray
+        :param values: The predicted state-value from the critic network.
+        :type values: numpy.ndarray
+        :param done: The done flags obtained from the environment.
+        :type done: numpy.ndarray
+        :param gamma: The discount factor.
+        :type gamma: float
+        :param lam: The GAE lambda value.
+        :type lam: float
+        :return: The calculated advantages.
+        :rtype: numpy.ndarray
+        """
+
+        advantages = np.zeros_like(rewards)
+        last_advantage = 0
+        for t in reversed(range(len(rewards))):
+            delta = rewards[t] + gamma * \
+                values[t + 1] * (1 - dones[t]) - values[t]
+            advantages[t] = delta + gamma * lam * \
+                last_advantage * (1 - dones[t])
+            last_advantage = advantages[t]
+        return advantages
+
+    def ppo_iter(self, mini_batch_size, states, actions, log_probs, returns, advantages):
+        """
+        Generate random mini-batches of data for PPO algorithm.
+
+        :param mini_batch_size: The size of each mini-batch.
+        :type mini_batch_size: int
+        :param states: The states from the environment.
+        :type states: torch.Tensor
+        :param actions: The actions taken in the environment.
+        :type actions: torch.Tensor
+        :param log_probs: The logarithmic probabilities of the actions.
+        :type log_probs: torch.Tensor
+        :param returns: The calculated returns.
+        :type returns: torch.Tensor
+        :param advantages: The calculated advantages.
+        :type advantages: torch.Tensor
+        :yield: A mini-batch of data.
+        """
+
+        batch_size = states.size(0)
+        for _ in range(batch_size // mini_batch_size):
+            rand_ids = np.random.randint(0, batch_size - 1, mini_batch_size)
+            yield states[rand_ids, :], actions[rand_ids], log_probs[rand_ids], returns[rand_ids], advantages[rand_ids]
+
+    def ppo_update(self, ppo_epochs, mini_batch_size, states, actions, log_probs, returns, advantages, clip_param=0.2):
+        """
+        Perform PPO algorithm for the specified number of epochs.
+
+        :param ppo_epochs: The number of epochs to run PPO algorithm.
+        :type ppo_epochs: int
+        :param mini_batch_size: The size of each mini-batch.
+        :type mini_batch_size: int
+        :param states: The states from the environment.
+        :type states: torch.Tensor
+        :param actions: The actions taken in the environment.
+        :type actions: torch.Tensor
+        :param log_probs: The logarithmic probabilities of the actions.
+        :type log_probs: torch.Tensor
+        :param returns: The calculated returns.
+        :type returns: torch.Tensor
+        :param advantages: The calculated advantages.
+        :type advantages: torch.Tensor
+        :param clip_param: The PPO clipping parameter.
+        :type clip_param: float
+        """
+
+        for _ in range(ppo_epochs):
+            for state, action, old_log_probs, return_, advantage in self.ppo_iter(mini_batch_size, states, actions, log_probs, returns, advantages):
+                dist = Categorical(self.policy_net(state))
+                new_log_probs = dist.log_prob(action)
+
+                ratio = (new_log_probs - old_log_probs).exp()
+                surr1 = ratio * advantage
+                surr2 = torch.clamp(ratio, 1.0 - clip_param,
+                                    1.0 + clip_param) * advantage
+                policy_loss = -torch.min(surr1, surr2).mean()
+
+                value_loss = (return_ - self.value_net(state)).pow(2).mean()
+                self.value_optimizer.zero_grad()
+                value_loss.backward()
+                self.value_optimizer.step()
+
+    def select_action(self, state):
+        """
+        Selects an action based on the given state and the current policy.
+
+        :param state: The state to use for selecting an action.
+        :type state: numpy.ndarray
+        :return: The selected action and its corresponding probability distribution.
+        :rtype: tuple(torch.Tensor, torch.distributions.Categorical)
+        """
+
+        state = self._check_state(self.state)
+        state_tensor = torch.tensor(state, dtype=torch.float32)
+        with torch.no_grad():
+            action_probs = self.policy_net(state_tensor)
+        dist = Categorical(action_probs)
+        self.dist = dist
+        action = dist.sample()
+        return action, dist
+
+    def learn_step(self, state, timestep):
+        """
+        Takes a step in the environment and updates the PPO algorithm with the resulting state, reward, and action.
+
+        :param state: The current state of the environment.
+        :type state: numpy.ndarray
+        :param timestep: The current timestep of the training process.
+        :type timestep: int
+        :return: The action taken, the resulting reward, and whether the episode is done or not.
+        :rtype: tuple(torch.Tensor, float, bool)
+        """
+
+        action, dist = self.select_action(state)
+
+        return self.update_step(state, dist, action, timestep)
+
+    def update_step(self, state, dist, action, timestep, auto_step=True, is_done=False, reward=0, next_state=None):
+        """
+        Updates the Proximal Policy Optimization (PPO) algorithm with the provided state, action, and timestep. This function can either take an environment step based on the given action (auto_step=True) or manually handle state transitions (auto_step=False).
+
+        :param state: The current state of the environment.
+        :type state: numpy.ndarray
+        :param dist: The corresponding probability distribution of the action space.
+        :type dist: torch.distributions.Categorical
+        :param action: The action taken by the agent.
+        :type action: int
+        :param timestep: The current timestep of the training process.
+        :type timestep: int
+        :param auto_step: Flag to determine whether to take an environment step or not. If False, is_done, reward, and next_state should be provided.
+        :type auto_step: bool, optional
+        :param is_done: Flag to mark if the episode is done or not. Should be provided if auto_step is False.
+        :type is_done: bool, optional
+        :param reward: The reward for the current step. Should be provided if auto_step is False.
+        :type reward: float, optional
+        :param next_state: The next state after the current action. If not provided and auto_step is False, it will be assumed to be the same as the current state.
+        :type next_state: numpy.ndarray, optional
+        :return: The action taken, the resulting reward, whether the episode is done or not, and the updated timestep.
+        :rtype: tuple(int, float, bool, int)
+        """
+
+        if dist == None and self.dist:
+            dist = self.dist
+
+        if auto_step:
+            step_output = self.env.step(action.item())
+            next_state, reward, is_done = self.step_unpack(step_output)
+
+        else:
+            if next_state is None:
+                next_state = state
+
+        self.update_reward(reward)
+
+        state = self._check_state(state)
+
+        self.states.append(state)
+        self.actions.append(action)
+        self.rewards.append(reward)
+        self.next_states.append(next_state)
+        self.dones.append(is_done)
+        self.log_probs.append(dist.log_prob(action))
+
+        self.state = next_state
+
+        if timestep > 0:
+            timestep += 1
+
+        if self.update_timestep > 0 and timestep > 0 and (timestep % self.update_timestep == 0):
+            self.update()
+
+        return action, reward, is_done, timestep
+
+    def update(self):
+        """
+        Perform an update of the PPO algorithm, using the stored information about the environment from the previous learning iterations.
+        """
+
+        Logger.verb('agents:ppo:update',
+                    f'states={self.states}, next_states={self.next_states}, actions={self.actions}, rewards={self.rewards}, dones={self.dones}')
+        states_tensor = torch.tensor(np.array(self.states, dtype=np.float32))
+        actions_tensor = torch.tensor(np.array(self.actions))
+        rewards_tensor = torch.tensor(np.array(self.rewards, dtype=np.float32))
+        next_states_tensor = torch.tensor(
+            np.array(self.next_states, dtype=np.float32))
+        done_tensor = torch.tensor(np.array(self.dones, dtype=np.float32))
+        log_probs_tensor = torch.stack(self.log_probs)
+
+        values = self.value_net(states_tensor).detach().squeeze(1)
+        next_values = self.value_net(next_states_tensor).detach().squeeze(1)
+
+        if len(next_states_tensor) > 0:
+            last_value = next_values[-1].item()
+        else:
+            last_value = 0
+
+        advantages = self.compute_advantages(rewards_tensor.numpy(), np.append(
+            values.numpy(), last_value), done_tensor.numpy(), self.gamma, self.lam)
+        advantages = (advantages - advantages.mean()) / \
+            (advantages.std() + 1e-5)
+        advantages_tensor = torch.tensor(advantages, dtype=torch.float32)
+
+        if len(advantages) > 1:
+            returns = np.add(advantages[:-1], values[:-1])
+        else:
+            returns = np.add(advantages, values)
+
+        self.ppo_update(self.ppo_epochs, self.mini_batch_size, states_tensor,
+                        actions_tensor, log_probs_tensor, returns, advantages_tensor)
+
+        self.reset()
+        self.update_episode()
+
+    def train(self):
+        """
+        Execute the learning loop, where the PPO algorithm is used to train the agent on the specified environment.
+        """
+        self.learn()
+
+    def learn(self):
+        """
+        Execute the learning loop, where the PPO algorithm is used to train the agent on the specified environment.
+        """
+
+        timestep = 0
+        test = 0
+        self.total_reward = 0
+
+        if self.max_episodes > 0 and self.max_timesteps > 0:
+            is_done = False
+            for episode in range(self.max_episodes):
+                self.episode = episode
+                self.reset()
+                self.learn_reset()
+                self.episode_reward = 0
+                reward = 0
+
+                for t in range(self.max_timesteps):
+                    action, reward, is_done, timestep = self.learn_step(
+                        self.state, timestep)
+                    if is_done:
+                        break
+
+                self.learn_check()
+                avg_reward = self.total_reward / (self.episode + 1)
+
+                if avg_reward >= self.early_stop_threshold > 0:
+                    Logger.info(
+                        f'Early stopping: Average reward has reached the threshold ({self.early_stop_threshold}) at episode {self.episode}')
+                    break
+                if is_done and self.done_loop_end:
+                    break
+
+                if self.episode + 1 >= self.max_episodes:
+                    break
+
+            self.env.close()
+        else:
+            self.reset()
+
+    def learn_next(self):
+        """
+        Perform a single learning step and update the episode and total rewards.
+
+        :return: The action taken, the resulting reward, and whether the episode is done or not.
+        :rtype: tuple(torch.Tensor, float, bool)
+        """
+
+        action, reward, is_done, timestep = self.learn_step(self.state, -1)
+
+        return action, reward, is_done, timestep
+
+    def learn_close(self):
+        """
+        Close the environment and reset the agent's total reward, episode count, and episode reward.
+        """
+
+        super().learn_close()
+
+    def learn_check(self):
+        """
+        Print the episode count, previous reward, episode reward, total reward, and average episode reward.
+        """
+
+        super().learn_check()
+
+    def save_model(self, file_name):
+        """
+        This function saves the model to the specified file.
+
+        :param file_name: The name of the file to save the model to.
+        :return: None
+        """
+        self.save(file_name)
+
+    def save(self, file_name):
+        """
+        This function saves the policy and value networks to the specified file.
+
+        :param file_name: The name of the file to save the policy and value networks to.
+        :return: None
+        """
+
+        self.save_policy_value(file_name)
+
+    def load_model(self, file_name):
+        """
+        This function loads the model from the specified file.
+
+        :param file_name: The name of the file to load the model from.
+        :return: None
+        """
+        self.load(file_name)
+
+    def load(self, file_name):
+        """
+        This function loads the policy and value networks from the specified file.
+
+        :param file_name: The name of the file to load the policy and value networks from.
+        :return: None
+        """
+
+        self.load_policy_value(file_name)
```

### Comparing `modular_rl-0.3.3/modular_rl/envs/mim/card_evaluator.py` & `modular_rl-0.4.0/modular_rl/envs/mim/card_evaluator.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.3/modular_rl/networks/actor_critic.py` & `modular_rl-0.4.0/modular_rl/networks/pytorch/actor_critic.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 This software includes the following third-party libraries:
 PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
 
 """
 import torch.nn as nn
 
 
-class ActorCriticNetwork(nn.Module):
+class PyTorchActorCriticNetwork(nn.Module):
     def __init__(self, state_dim, action_dim, hidden_size=256):
         '''
         This code defines a class ActorCriticNetwork that implements an actor-critic network using PyTorch.
         The actor-critic algorithm is a popular reinforcement learning algorithm that is used to learn how to maximize rewards in an environment by having an agent interact with the environment.
         This network takes as input the state and action dimensions, and the number of neurons in the hidden layers of both the actor and critic networks.
         It then predicts state-value and action-value for the given input.
 
         :param state_dim: (int) The dimensionality of the state space.
         :param action_dim: (int) The dimensionality of the action space.
         :param hidden_size: (int) The number of neurons in the hidden layers of both the actor and critic networks.
         '''
 
-        super(ActorCriticNetwork, self).__init__()
+        super(PyTorchActorCriticNetwork, self).__init__()
 
         # Actor network
         self.actor = nn.Sequential(
             nn.Linear(state_dim, hidden_size),
             nn.ReLU(),
             nn.Linear(hidden_size, action_dim),
             nn.Softmax(dim=-1)
```

### Comparing `modular_rl-0.3.3/modular_rl/networks/policy.py` & `modular_rl-0.4.0/modular_rl/networks/pytorch/policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 # -*- coding: utf-8 -*-
 """
 ModularRL project
 
 Copyright (c) 2023 horrible
 
-PolicyNetwork is a neural network that takes in the current state of the environment as input and outputs a probability distribution over the available actions. 
+PolicyNetwork is a neural network that takes in the current state of the environment as input and outputs a probability distribution over the available actions.
 The purpose of this network is to determine the best action to take in the current state.
 
-ValueNetwork, on the other hand, 
-is a neural network that takes in the current state of the environment as input and outputs a value that represents the expected future reward that can be obtained from that state. 
+ValueNetwork, on the other hand,
+is a neural network that takes in the current state of the environment as input and outputs a value that represents the expected future reward that can be obtained from that state.
 The purpose of this network is to estimate the value of a given state so that the agent can make decisions that lead to the most reward in the long term.
 
-Both networks are important components of the Proximal Policy Optimization (PPO) algorithm, 
+Both networks are important components of the Proximal Policy Optimization (PPO) algorithm,
 which is a type of reinforcement learning algorithm used for training agents to perform tasks in an environment.
 
 This software includes the following third-party libraries:
 PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
 
 """
 import torch.nn as nn
 import torch
 
 
-class PolicyNetwork(nn.Module):
+class PyTorchPolicyNetwork(nn.Module):
     def __init__(self, input_dim, output_dim, hidden_option='medium', num_layers=2):
         """
         Initialize the PolicyNetwork class with the specified input dimension, output dimension, and network settings.
 
         :param input_dim: The dimension of the input layer.
         :type input_dim: int
         :param output_dim: The dimension of the output layer.
         :type output_dim: int
         :param hidden_option: The size of the hidden layers (options are 'small', 'medium', 'large', 'huge', or 'exhuge').
         :type hidden_option: str
         :param num_layers: The number of hidden layers.
         :type num_layers: int
         """
 
-        super(PolicyNetwork, self).__init__()
+        super(PyTorchPolicyNetwork, self).__init__()
 
         hidden_dim_map = {
             'small': 32,
             'medium': 64,
             'large': 128,
             'huge': 256,
             'exhuge': 512
```

### Comparing `modular_rl-0.3.3/modular_rl/networks/value.py` & `modular_rl-0.4.0/modular_rl/networks/pytorch/value.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # -*- coding: utf-8 -*-
 """
 ModularRL project
 
 Copyright (c) 2023 horrible
 
-PolicyNetwork is a neural network that takes in the current state of the environment as input and outputs a probability distribution over the available actions. 
+PolicyNetwork is a neural network that takes in the current state of the environment as input and outputs a probability distribution over the available actions.
 The purpose of this network is to determine the best action to take in the current state.
 
-ValueNetwork, on the other hand, 
-is a neural network that takes in the current state of the environment as input and outputs a value that represents the expected future reward that can be obtained from that state. 
+ValueNetwork, on the other hand,
+is a neural network that takes in the current state of the environment as input and outputs a value that represents the expected future reward that can be obtained from that state.
 The purpose of this network is to estimate the value of a given state so that the agent can make decisions that lead to the most reward in the long term.
 
-Both networks are important components of the Proximal Policy Optimization (PPO) algorithm, 
+Both networks are important components of the Proximal Policy Optimization (PPO) algorithm,
 which is a type of reinforcement learning algorithm used for training agents to perform tasks in an environment.
 
 This software includes the following third-party libraries:
 PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
 
 """
 import torch.nn as nn
 
 
-class ValueNetwork(nn.Module):
+class PyTorchValueNetwork(nn.Module):
     def __init__(self, input_dim, hidden_option='medium', num_layers=2):
         """
         Initialize the ValueNetwork class with the specified input dimension and network settings.
 
         :param input_dim: The dimension of the input layer.
         :type input_dim: int
         :param hidden_option: The size of the hidden layers (options are 'small', 'medium', 'large', 'huge', or 'exhuge').
         :type hidden_option: str
         :param num_layers: The number of hidden layers.
         :type num_layers: int
         """
 
-        super(ValueNetwork, self).__init__()
+        super(PyTorchValueNetwork, self).__init__()
 
         hidden_dim_map = {
             'small': 32,
             'medium': 64,
             'large': 128,
             'huge': 256,
             'exhuge': 512
```

### Comparing `modular_rl-0.3.3/modular_rl/params/mcis.py` & `modular_rl-0.4.0/modular_rl/params/mcts.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,41 @@
-class ParamMCIS:
+class ParamMCTS:
     default = {
+        'learn_framework': 'pytorch',
         'max_episodes': 10,  # Maximum number of episodes for training
         'max_timesteps': 200,  # Maximum number of timesteps for each episode
+        'update_timestep': 2000,  # Update the policy every specified timestep
+        'num_simulations': 10,  # Number of MCTS simulations per move
         'networks': 'medium',  # Size of the hidden layer in neural networks
         'optimizer_speed': 3e-4,  # Learning rate for the optimizer
-        'num_simulations': 10,  # Number of MCIS simulations per move
-        'cpuct': 1.0,  # Exploration constant for MCIS
-        'temperature': 1.0,  # Temperature for action selection during MCIS
+        'cpuct': 1.0,  # Exploration constant for MCTS
+        'temperature': 1.0,  # Temperature for action selection during MCTS
         'gamma': 0.99,  # Discount factor
         # If the average reward is greater than or equal to this value, training is stopped early
         'early_stop_threshold': -1,
         'done_loop_end': False,  # If True, end the episode when the done flag is set
         'reward_print': True,  # If True, print the reward during training
         'device': None,  # Device to run the model on, None for automatic selection
         'log_level': 'debug',  # Log level for the logger
         'log_init_pass': False,  # If True, skip logger initialization
     }
 
     default_modular = {
-        # Maximum number of episodes for training (-1 for no limit)
-        'max_episodes': -1,
-        # Maximum number of timesteps for each episode (-1 for no limit)
-        'max_timesteps': -1,
+        'learn_framework': 'pytorch',
+        # Maximum number of episodes for training (1 for modular)
+        'max_episodes': 1,
+        # Maximum number of timesteps for each episode (1 for modular)
+        'max_timesteps': 1,
+        # Update the policy every specified timestep (1 for modular)
+        'update_timestep': 1,
+        'num_simulations': 1,  # Number of MCTS simulations per move
         'networks': 'medium',  # Size of the hidden layer in neural networks
         'optimizer_speed': 3e-4,  # Learning rate for the optimizer
-        'num_simulations': 800,  # Number of MCIS simulations per move
-        'cpuct': 1.0,  # Exploration constant for MCIS
-        'temperature': 1.0,  # Temperature for action selection during MCIS
+        'cpuct': 1.0,  # Exploration constant for MCTS
+        'temperature': 1.0,  # Temperature for action selection during MCTS
         'gamma': 0.99,  # Discount factor
         # If the average reward is greater than or equal to this value, training is stopped early
         'early_stop_threshold': -1,
         'reward_print': True,  # If True, print the reward during training
         'device': None,  # Device to run the model on, None for automatic selection
         'log_level': 'debug',  # Log level for the logger
         'log_init_pass': False,  # If True, skip logger initialization
```

### Comparing `modular_rl-0.3.3/modular_rl/params/mcts.py` & `modular_rl-0.4.0/modular_rl/params/mcis.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-class ParamMCTS:
-    default = {
-        'max_episodes': 10,  # Maximum number of episodes for training
-        'max_timesteps': 200,  # Maximum number of timesteps for each episode
-        'update_timestep': 2000,  # Update the policy every specified timestep
-        'num_simulations': 10,  # Number of MCTS simulations per move
-        'networks': 'medium',  # Size of the hidden layer in neural networks
-        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
-        'cpuct': 1.0,  # Exploration constant for MCTS
-        'temperature': 1.0,  # Temperature for action selection during MCTS
-        'gamma': 0.99,  # Discount factor
-        # If the average reward is greater than or equal to this value, training is stopped early
-        'early_stop_threshold': -1,
-        'done_loop_end': False,  # If True, end the episode when the done flag is set
-        'reward_print': True,  # If True, print the reward during training
-        'device': None,  # Device to run the model on, None for automatic selection
-        'log_level': 'debug',  # Log level for the logger
-        'log_init_pass': False,  # If True, skip logger initialization
-    }
-
-    default_modular = {
-        # Maximum number of episodes for training (1 for modular)
-        'max_episodes': 1,
-        # Maximum number of timesteps for each episode (1 for modular)
-        'max_timesteps': 1,
-        # Update the policy every specified timestep (1 for modular)
-        'update_timestep': 1,
-        'num_simulations': 1,  # Number of MCTS simulations per move
-        'networks': 'medium',  # Size of the hidden layer in neural networks
-        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
-        'cpuct': 1.0,  # Exploration constant for MCTS
-        'temperature': 1.0,  # Temperature for action selection during MCTS
-        'gamma': 0.99,  # Discount factor
-        # If the average reward is greater than or equal to this value, training is stopped early
-        'early_stop_threshold': -1,
-        'reward_print': True,  # If True, print the reward during training
-        'device': None,  # Device to run the model on, None for automatic selection
-        'log_level': 'debug',  # Log level for the logger
-        'log_init_pass': False,  # If True, skip logger initialization
-    }
+class ParamMCIS:
+    default = {
+        'learn_framework': 'pytorch',
+        'max_episodes': 10,  # Maximum number of episodes for training
+        'max_timesteps': 50,  # Maximum number of timesteps for each episode
+        'networks': 'medium',  # Size of the hidden layer in neural networks
+        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
+        'num_simulations': 10,  # Number of MCIS simulations per move
+        'cpuct': 1.0,  # Exploration constant for MCIS
+        'temperature': 1.0,  # Temperature for action selection during MCIS
+        'gamma': 0.99,  # Discount factor
+        # If the average reward is greater than or equal to this value, training is stopped early
+        'early_stop_threshold': -1,
+        'done_loop_end': False,  # If True, end the episode when the done flag is set
+        'reward_print': True,  # If True, print the reward during training
+        'device': None,  # Device to run the model on, None for automatic selection
+        'log_level': 'debug',  # Log level for the logger
+        'log_init_pass': False,  # If True, skip logger initialization
+    }
+
+    default_modular = {
+        'learn_framework': 'pytorch',
+        # Maximum number of episodes for training
+        'max_episodes': 1,
+        # Maximum number of timesteps for each episode
+        'max_timesteps': 1,
+        'networks': 'medium',  # Size of the hidden layer in neural networks
+        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
+        'num_simulations': 1,  # Number of MCIS simulations per move
+        'cpuct': 1.0,  # Exploration constant for MCIS
+        'temperature': 1.0,  # Temperature for action selection during MCIS
+        'gamma': 0.99,  # Discount factor
+        # If the average reward is greater than or equal to this value, training is stopped early
+        'early_stop_threshold': -1,
+        'reward_print': True,  # If True, print the reward during training
+        'device': None,  # Device to run the model on, None for automatic selection
+        'log_level': 'debug',  # Log level for the logger
+        'log_init_pass': False,  # If True, skip logger initialization
+    }
```

### Comparing `modular_rl-0.3.3/modular_rl/params/ppo.py` & `modular_rl-0.4.0/modular_rl/params/ppo.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 class ParamPPO:
     default = {
+        'learn_framework': 'pytorch',
         'max_episodes': 30,  # Maximum number of episodes for training
         'max_timesteps': 200,  # Maximum number of timesteps for each episode
         'update_timestep': 2000,  # Update the policy every specified timestep
         'ppo_epochs': 4,  # Number of PPO epochs
         'mini_batch_size': 64,  # Batch size for PPO updates
         'networks': 'medium',  # Size of the hidden layer in neural networks
         'optimizer_speed': 3e-4,  # Learning rate for the optimizer
@@ -14,14 +15,15 @@
         'early_stop_threshold': -1,
         'done_loop_end': False,  # If True, end the episode when the done flag is set
         'log_level': 'debug',  # Log level for the logger
         'log_init_pass': False,  # If True, skip logger initialization
     }
 
     default_modular = {
+        'learn_framework': 'pytorch',
         # Maximum number of episodes for training (-1 for no limit)
         'max_episodes': -1,
         # Maximum number of timesteps for each episode (-1 for no limit)
         'max_timesteps': -1,
         # Update the policy every specified timestep (-1 for no limit)
         'update_timestep': -1,
         'ppo_epochs': 4,  # Number of PPO epochs
```

### Comparing `modular_rl-0.3.3/modular_rl/settings.py` & `modular_rl-0.4.0/modular_rl/settings.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-'''
-The AgentSettings class is a configuration class used for setting up various reinforcement learning agents.
-
-It provides default values for various parameters used in the agents, such as the maximum number of episodes,
-maximum number of timesteps per episode, update timestep, network architecture, learning rate,
-discount factor, early stopping threshold, and whether to end training when the environment is done.
-
-The class currently supports PPO and MCTS algorithms, but it can be extended to include other algorithms in the future.
-The default dictionary provides default values for all parameters, while the modular version provides default values
-with more flexibility for specific use cases. These default values can be modified by passing in a dictionary of
-key-value pairs to the AgentSettings constructor.
-
-'''
-
-from modular_rl.params.ppo import ParamPPO
-from modular_rl.params.mcts import ParamMCTS
-from modular_rl.params.mcis import ParamMCIS
-from modular_rl.params.mim import ParamMIM
-
-
-class AgentSettings:
-    default_ppo = ParamPPO.default
-    default_ppo_modular = ParamPPO.default_modular
-    default_mcts = ParamMCTS.default
-    default_mcts_modular = ParamMCTS.default_modular
-    default_mcis = ParamMCIS.default
-    default_mcis_modular = ParamMCIS.default_modular
-    default_mim = ParamMIM.default
-    default_mim_modular = ParamMIM.default_modular
+'''
+The AgentSettings class is a configuration class used for setting up various reinforcement learning agents.
+
+It provides default values for various parameters used in the agents, such as the maximum number of episodes,
+maximum number of timesteps per episode, update timestep, network architecture, learning rate,
+discount factor, early stopping threshold, and whether to end training when the environment is done.
+
+The class currently supports PPO and MCTS algorithms, but it can be extended to include other algorithms in the future.
+The default dictionary provides default values for all parameters, while the modular version provides default values
+with more flexibility for specific use cases. These default values can be modified by passing in a dictionary of
+key-value pairs to the AgentSettings constructor.
+
+'''
+
+from modular_rl.params.ppo import ParamPPO
+from modular_rl.params.mcts import ParamMCTS
+from modular_rl.params.mcis import ParamMCIS
+from modular_rl.params.mim import ParamMIM
+
+
+class AgentSettings:
+    default_ppo = ParamPPO.default
+    default_ppo_modular = ParamPPO.default_modular
+    default_mcts = ParamMCTS.default
+    default_mcts_modular = ParamMCTS.default_modular
+    default_mcis = ParamMCIS.default
+    default_mcis_modular = ParamMCIS.default_modular
+    default_mim = ParamMIM.default
+    default_mim_modular = ParamMIM.default_modular
```

### Comparing `modular_rl-0.3.3/modular_rl/util/node.py` & `modular_rl-0.4.0/modular_rl/util/node.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,32 +3,37 @@
 import numpy as np
 
 
 class Node:
     def __init__(self, state, prior, action=None, done=False):
         self.state = state
         self.prior = prior
-        self.action = action  # 액션 정보를 저장하는 속성 추가
+        self.action = action
         self.visit_count = 0
         self.value_sum = 0
         self.children = {}
         self.total_value = 0
         self.done = done  # Assign the done attribute
 
-
     def __repr__(self):
         return f'Node(state={self.state}, total_value={self.total_value}, visit_count={self.visit_count}, is_expanded={self.expanded()}, action_probs={self.action}, children={self.children})'
 
     def expanded(self):
         return len(self.children) > 0
 
     def value(self):
         if self.visit_count == 0:
             return 0
-        return self.total_value / self.visit_count  # 총 보상을 방문 횟수로 나누어 평균 보상을 반환
+        return self.total_value / self.visit_count
+
+    def get_score(self, cpuct):
+        """
+        Calculate and return the UCT value of the node.
+        """
+        return self.value() + cpuct * self.prior * math.sqrt(self.visit_count) / (1 + self.visit_count)
 
     def select_child(self, cpuct):
         best_score = -math.inf
         best_action = -1
         best_child = None
 
         for action, child in self.children.items():
@@ -40,19 +45,21 @@
                 best_child = child
 
         return best_action, best_child
 
     def expand(self, action_space, child_priors, child_done):  # Add a child_done parameter
         for action, prior in zip(range(action_space), child_priors):
             if action not in self.children:
-                self.children[action] = Node(self.state, prior, action, child_done)  # Pass the child_done to the new Node
+                # Pass the child_done to the new Node
+                self.children[action] = Node(
+                    self.state, prior, action, child_done)
 
     def update_stats(self, reward):
-        self.total_value += reward  # 총 보상 업데이트
-        self.visit_count += 1  # 방문 횟수 증가
+        self.total_value += reward
+        self.visit_count += 1
 
     def select_action(self, temperature=1):
         visit_counts = np.array(
             [child.visit_count for child in self.children.values()])
         actions = [action for action in self.children.keys()]
         if temperature == 0:
             action = actions[np.argmax(visit_counts)]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `modular_rl-0.3.3/pyproject.toml` & `modular_rl-0.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "modular_rl"
-version = "0.3.3"
-authors = [
-  { name="horrible", email="shinjpn1@gmail.com" },
-]
-description = "ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm."
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
-    'Programming Language :: Python :: 3.11',
-]
-keywords=['ModularRL', 'Modular-RL', 'Modular_RL', 'Modular RL',  'modularrl',  'modular_rl', 'modular-rl', 'modular rl', 'mrl', 'modular', 'learn', 'learning', 'pytorch learn', 'pytorch learning']
-dependencies=['gym', 'numpy', 'torch', 'LogAssist']
-
-
-[project.urls]
-"Homepage" = "https://github.com/horrible-gh/ModularRL"
-"Bug Tracker" = "https://github.com/horrible-gh/ModularRL/issues"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "modular_rl"
+version = "0.4.0"
+authors = [
+  { name="horrible", email="shinjpn1@gmail.com" },
+]
+description = "ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm."
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.6',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+]
+keywords=['ModularRL', 'Modular-RL', 'Modular_RL', 'Modular RL',  'modularrl',  'modular_rl', 'modular-rl', 'modular rl', 'mrl', 'modular', 'learn', 'learning', 'pytorch learn', 'pytorch learning', 'tensorflow learn', 'tensorflow learning', 'ai']
+dependencies=['gym', 'numpy', 'torch', 'LogAssist']
+
+
+[project.urls]
+"Homepage" = "https://github.com/horrible-gh/ModularRL"
+"Bug Tracker" = "https://github.com/horrible-gh/ModularRL/issues"
```

