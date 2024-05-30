# Comparing `tmp/agilerl-0.1.8.tar.gz` & `tmp/agilerl-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agilerl-0.1.8.tar", max compression
+gzip compressed data, was "agilerl-0.1.9.tar", max compression
```

## Comparing `agilerl-0.1.8.tar` & `agilerl-0.1.9.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0    11357 2023-08-22 10:25:16.267840 agilerl-0.1.8/LICENSE
--rw-r--r--   0        0        0    43374 2023-08-23 11:52:48.184325 agilerl-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-07-14 09:37:02.389508 agilerl-0.1.8/agilerl/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 09:37:02.390330 agilerl-0.1.8/agilerl/algorithms/__init__.py
--rw-r--r--   0        0        0    22132 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/algorithms/bc_lm.py
--rw-r--r--   0        0        0    15180 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/algorithms/cqn.py
--rw-r--r--   0        0        0    21864 2023-07-19 10:40:38.170157 agilerl-0.1.8/agilerl/algorithms/ddpg.py
--rw-r--r--   0        0        0    15220 2023-08-23 10:50:27.835848 agilerl-0.1.8/agilerl/algorithms/dqn.py
--rw-r--r--   0        0        0    72436 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/algorithms/ilql.py
--rw-r--r--   0        0        0    30648 2023-08-31 15:40:29.887853 agilerl-0.1.8/agilerl/algorithms/maddpg.py
--rw-r--r--   0        0        0    38430 2023-08-31 15:40:29.887853 agilerl-0.1.8/agilerl/algorithms/matd3.py
--rw-r--r--   0        0        0    27745 2023-08-31 15:40:29.887853 agilerl-0.1.8/agilerl/algorithms/td3.py
--rw-r--r--   0        0        0        0 2023-07-14 09:37:02.392857 agilerl-0.1.8/agilerl/components/__init__.py
--rw-r--r--   0        0        0     3846 2023-08-31 15:40:29.887853 agilerl-0.1.8/agilerl/components/multi_agent_replay_buffer.py
--rw-r--r--   0        0        0     4072 2023-07-19 10:40:38.171156 agilerl-0.1.8/agilerl/components/replay_buffer.py
--rw-r--r--   0        0        0      631 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/components/replay_data.py
--rw-r--r--   0        0        0      687 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/components/sampler.py
--rw-r--r--   0        0        0        0 2023-07-14 09:37:02.392857 agilerl-0.1.8/agilerl/data/__init__.py
--rw-r--r--   0        0        0     1624 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/data/language_environment.py
--rw-r--r--   0        0        0     7824 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/data/rl_data.py
--rw-r--r--   0        0        0     1259 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/data/tokenizer.py
--rw-r--r--   0        0        0     1133 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/data/torch_datasets.py
--rw-r--r--   0        0        0        0 2023-07-31 15:51:32.685783 agilerl-0.1.8/agilerl/hpo/__init__.py
--rw-r--r--   0        0        0    40085 2023-08-31 15:40:29.887853 agilerl-0.1.8/agilerl/hpo/mutation.py
--rw-r--r--   0        0        0     2193 2023-07-14 09:37:02.396404 agilerl-0.1.8/agilerl/hpo/tournament.py
--rw-r--r--   0        0        0        0 2023-07-14 09:37:02.396404 agilerl-0.1.8/agilerl/networks/__init__.py
--rw-r--r--   0        0        0      853 2023-08-31 15:40:29.887853 agilerl-0.1.8/agilerl/networks/custom_architecture.py
--rw-r--r--   0        0        0    36712 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/networks/evolvable_bert.py
--rw-r--r--   0        0        0    28941 2023-08-31 15:40:29.887853 agilerl-0.1.8/agilerl/networks/evolvable_cnn.py
--rw-r--r--   0        0        0    37084 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/networks/evolvable_gpt.py
--rw-r--r--   0        0        0    15344 2023-08-31 15:40:29.887853 agilerl-0.1.8/agilerl/networks/evolvable_mlp.py
--rw-r--r--   0        0        0        0 2023-07-14 09:37:02.398842 agilerl-0.1.8/agilerl/training/__init__.py
--rw-r--r--   0        0        0    13777 2023-08-31 15:40:29.887853 agilerl-0.1.8/agilerl/training/train.py
--rw-r--r--   0        0        0     8654 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/training/train_bc_lm.py
--rw-r--r--   0        0        0     9198 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/training/train_ilql.py
--rw-r--r--   0        0        0    14519 2023-08-31 15:41:13.967857 agilerl-0.1.8/agilerl/training/train_multi_agent.py
--rw-r--r--   0        0        0    13677 2023-08-31 15:40:29.887853 agilerl-0.1.8/agilerl/training/train_offline.py
--rw-r--r--   0        0        0        0 2023-07-14 09:37:02.400716 agilerl-0.1.8/agilerl/utils/__init__.py
--rw-r--r--   0        0        0     1574 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/utils/cache.py
--rw-r--r--   0        0        0     3992 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/utils/ilql_utils.py
--rw-r--r--   0        0        0    10171 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/utils/load_objects.py
--rw-r--r--   0        0        0     2380 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/utils/log_utils.py
--rw-r--r--   0        0        0     3344 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/utils/minari_utils.py
--rw-r--r--   0        0        0      116 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/utils/mp_cache.py
--rw-r--r--   0        0        0     2183 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/utils/sampling_utils.py
--rw-r--r--   0        0        0     3346 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/utils/serve_queue.py
--rw-r--r--   0        0        0     1475 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/utils/torch_utils.py
--rw-r--r--   0        0        0     6906 2023-08-31 15:40:29.887853 agilerl-0.1.8/agilerl/utils/utils.py
--rw-r--r--   0        0        0        0 2023-07-14 09:37:02.402768 agilerl-0.1.8/agilerl/wordle/__init__.py
--rw-r--r--   0        0        0     6859 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/wordle/policy.py
--rw-r--r--   0        0        0     5888 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/wordle/wordle_dataset.py
--rw-r--r--   0        0        0     1089 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/wordle/wordle_env.py
--rw-r--r--   0        0        0     9909 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/wordle/wordle_evaluators.py
--rw-r--r--   0        0        0    10924 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/wordle/wordle_game.py
--rw-r--r--   0        0        0     2689 2023-08-22 10:25:16.267840 agilerl-0.1.8/agilerl/wordle/wordle_tokenizer.py
--rw-r--r--   0        0        0      796 2023-08-31 15:40:29.897853 agilerl-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    44809 1970-01-01 00:00:00.000000 agilerl-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-22 10:25:16.267840 agilerl-0.1.9/LICENSE
+-rw-r--r--   0        0        0    52430 2023-09-07 16:35:05.397876 agilerl-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-07-14 09:37:02.389508 agilerl-0.1.9/agilerl/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 09:37:02.390330 agilerl-0.1.9/agilerl/algorithms/__init__.py
+-rw-r--r--   0        0        0    22874 2023-09-07 16:33:44.497869 agilerl-0.1.9/agilerl/algorithms/bc_lm.py
+-rw-r--r--   0        0        0    15197 2023-09-07 16:33:44.497869 agilerl-0.1.9/agilerl/algorithms/cqn.py
+-rw-r--r--   0        0        0    21552 2023-09-07 16:33:44.497869 agilerl-0.1.9/agilerl/algorithms/ddpg.py
+-rw-r--r--   0        0        0    14893 2023-09-07 16:33:44.497869 agilerl-0.1.9/agilerl/algorithms/dqn.py
+-rw-r--r--   0        0        0    79029 2023-09-07 16:33:44.497869 agilerl-0.1.9/agilerl/algorithms/ilql.py
+-rw-r--r--   0        0        0    32964 2023-09-07 16:33:44.497869 agilerl-0.1.9/agilerl/algorithms/maddpg.py
+-rw-r--r--   0        0        0    42406 2023-09-07 16:33:44.497869 agilerl-0.1.9/agilerl/algorithms/matd3.py
+-rw-r--r--   0        0        0    22139 2023-09-07 16:33:44.497869 agilerl-0.1.9/agilerl/algorithms/ppo.py
+-rw-r--r--   0        0        0    27822 2023-09-07 16:33:44.497869 agilerl-0.1.9/agilerl/algorithms/td3.py
+-rw-r--r--   0        0        0        0 2023-07-14 09:37:02.392857 agilerl-0.1.9/agilerl/components/__init__.py
+-rw-r--r--   0        0        0     4761 2023-09-07 16:33:44.497869 agilerl-0.1.9/agilerl/components/multi_agent_replay_buffer.py
+-rw-r--r--   0        0        0     4072 2023-09-07 16:33:44.497869 agilerl-0.1.9/agilerl/components/replay_buffer.py
+-rw-r--r--   0        0        0      632 2023-09-07 16:33:44.497869 agilerl-0.1.9/agilerl/components/replay_data.py
+-rw-r--r--   0        0        0      679 2023-09-07 16:33:44.497869 agilerl-0.1.9/agilerl/components/sampler.py
+-rw-r--r--   0        0        0        0 2023-07-14 09:37:02.392857 agilerl-0.1.9/agilerl/data/__init__.py
+-rw-r--r--   0        0        0     1578 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/data/language_environment.py
+-rw-r--r--   0        0        0     8113 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/data/rl_data.py
+-rw-r--r--   0        0        0     1147 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/data/tokenizer.py
+-rw-r--r--   0        0        0     1115 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/data/torch_datasets.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:51:32.685783 agilerl-0.1.9/agilerl/hpo/__init__.py
+-rw-r--r--   0        0        0    41238 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/hpo/mutation.py
+-rw-r--r--   0        0        0     2096 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/hpo/tournament.py
+-rw-r--r--   0        0        0        0 2023-07-14 09:37:02.396404 agilerl-0.1.9/agilerl/networks/__init__.py
+-rw-r--r--   0        0        0      843 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/networks/custom_architecture.py
+-rw-r--r--   0        0        0    36859 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/networks/evolvable_bert.py
+-rw-r--r--   0        0        0    28881 2023-09-07 16:43:06.107912 agilerl-0.1.9/agilerl/networks/evolvable_cnn.py
+-rw-r--r--   0        0        0    37435 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/networks/evolvable_gpt.py
+-rw-r--r--   0        0        0    14920 2023-09-07 16:43:06.107912 agilerl-0.1.9/agilerl/networks/evolvable_mlp.py
+-rw-r--r--   0        0        0        0 2023-07-14 09:37:02.398842 agilerl-0.1.9/agilerl/training/__init__.py
+-rw-r--r--   0        0        0    13899 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/training/train.py
+-rw-r--r--   0        0        0     9348 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/training/train_bc_lm.py
+-rw-r--r--   0        0        0     9962 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/training/train_ilql.py
+-rw-r--r--   0        0        0    15262 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/training/train_multi_agent.py
+-rw-r--r--   0        0        0    14072 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/training/train_offline.py
+-rw-r--r--   0        0        0        0 2023-07-14 09:37:02.400716 agilerl-0.1.9/agilerl/utils/__init__.py
+-rw-r--r--   0        0        0     1515 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/utils/cache.py
+-rw-r--r--   0        0        0     4123 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/utils/ilql_utils.py
+-rw-r--r--   0        0        0    10492 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/utils/load_objects.py
+-rw-r--r--   0        0        0     2401 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/utils/log_utils.py
+-rw-r--r--   0        0        0     3317 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/utils/minari_utils.py
+-rw-r--r--   0        0        0      116 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/utils/mp_cache.py
+-rw-r--r--   0        0        0     2336 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/utils/sampling_utils.py
+-rw-r--r--   0        0        0     3681 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/utils/serve_queue.py
+-rw-r--r--   0        0        0     1531 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/utils/torch_utils.py
+-rw-r--r--   0        0        0     6936 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/utils/utils.py
+-rw-r--r--   0        0        0        0 2023-07-14 09:37:02.402768 agilerl-0.1.9/agilerl/wordle/__init__.py
+-rw-r--r--   0        0        0     7371 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/wordle/policy.py
+-rw-r--r--   0        0        0     6216 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/wordle/wordle_dataset.py
+-rw-r--r--   0        0        0     1088 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/wordle/wordle_env.py
+-rw-r--r--   0        0        0    12490 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/wordle/wordle_evaluators.py
+-rw-r--r--   0        0        0    12276 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/wordle/wordle_game.py
+-rw-r--r--   0        0        0     2670 2023-09-07 16:33:44.507869 agilerl-0.1.9/agilerl/wordle/wordle_tokenizer.py
+-rw-r--r--   0        0        0      818 2023-09-07 16:43:59.837916 agilerl-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    53908 1970-01-01 00:00:00.000000 agilerl-0.1.9/PKG-INFO
```

### Comparing `agilerl-0.1.8/LICENSE` & `agilerl-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.8/README.md` & `agilerl-0.1.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 **_NEW: AgileRL now supports distributed training with HuggingFace Accelerate!<br>
 Train even faster by taking full advantage of your entire compute stack._**
 
 </div>
 
 This is a Deep Reinforcement Learning library focused on improving development by introducing RLOps - MLOps for reinforcement learning.
-  
+
 This library is initially focused on reducing the time taken for training models and hyperparameter optimization (HPO) by pioneering evolutionary HPO techniques for reinforcement learning.<br>
 Evolutionary HPO has been shown to drastically reduce overall training times by automatically converging on optimal hyperparameters, without requiring numerous training runs.<br>
 We are constantly adding more algorithms, with a view to add hierarchical and multi-agent algorithms soon.
 
 <p align="center">
   <img src=https://user-images.githubusercontent.com/47857277/236407686-21363eb3-ffcf-419f-b019-0be4ddf1ed4a.gif height="250">
 </p>
@@ -33,37 +33,44 @@
   * [Algorithms implemented](#algorithms-implemented-more-coming-soon)
   * [Train an agent on a Gym environment (Online)](#train-an-agent-on-a-gym-environment-online)
     + [Custom Online Training Loop](#custom-online-training-loop)
   * [Train an agent on data (Offline)](#train-an-agent-on-data-offline)
     + [Custom Offline Training Loop](#custom-offline-training-loop)
   * [Train an agent on a language environment (RLHF)](#train-an-agent-on-a-language-environment-rlhf)
   * [Distributed training](#distributed-training)
+  * [Multi-agent training](#multi-agent-training)
 
 ## Benchmarks
 
 Reinforcement learning algorithms and libraries are usually benchmarked once the optimal hyperparameters for training are known, but it often takes hundreds or thousands of experiments to discover these. This is unrealistic and does not reflect the true, total time taken for training. What if we could remove the need to conduct all these prior experiments?
 
 In the charts below, a single AgileRL run, which automatically tunes hyperparameters, is benchmarked against Optuna's multiple training runs traditionally required for hyperparameter optimization, demonstrating the real time savings possible. Global steps is the sum of every step taken by any agent in the environment, including across an entire population.
 
 <p align="center">
   <img src=https://user-images.githubusercontent.com/47857277/227481592-27a9688f-7c0a-4655-ab32-90d659a71c69.png height="500">
 </p>
 <p align="center">AgileRL offers an order of magnitude speed up in hyperparameter optimization vs popular reinforcement learning training frameworks combined with Optuna. Remove the need for multiple training runs and save yourself hours.</p>
 
+AgileRL also supports multi-agent reinforcement learning using the Petting Zoo-style (parallel API). The charts below highlight the performance of our MADDPG and MATD3 algorithms with evolutionary hyper-parameter optimisation (HPO), benchmarked against epymarl's MADDPG algorithm with grid-search HPO for the simple speaker listener and simple spread environments.
+
+<p align="center">
+  <img src=https://github-production-user-asset-6210df.s3.amazonaws.com/118982716/264712154-4965ea5f-b777-423c-989b-e4db86eda3bd.png>
+</p>
+
 ## Get Started
-Install as a package with pip: 
+Install as a package with pip:
 ```bash
 pip install agilerl
 ```
 Or install in development mode: (Recommended due to nascent nature of this library)
 ```bash
 git clone https://github.com/AgileRL/AgileRL.git && cd AgileRL
 pip install -r requirements.txt
 ```
-If using ILQL on Wordle, download and unzip data.zip <a href="https://drive.google.com/drive/folders/13LFspsFQ-7XIlFjnsZttKf4nfVDlnmW2?usp=sharing">here</a>. 
+If using ILQL on Wordle, download and unzip data.zip <a href="https://drive.google.com/drive/folders/13LFspsFQ-7XIlFjnsZttKf4nfVDlnmW2?usp=sharing">here</a>.
 
 Demo:
 ```bash
 python demo_online.py
 ```
 or to demo distributed training:
 ```bash
@@ -72,14 +79,16 @@
 
 ## Algorithms implemented (more coming soon!)
   * DQN
   * DDPG
   * CQL
   * ILQL
   * TD3
+  * MADDPG
+  * MATD3
 
 ## Train an agent on a Gym environment (Online)
 Before starting training, there are some meta-hyperparameters and settings that must be set. These are defined in <code>INIT_HP</code>, for general parameters, and <code>MUTATION_PARAMS</code>, which define the evolutionary probabilities, and <code>NET_CONFIG</code>, which defines the network architecture. For example:
 ```python
 INIT_HP = {
     'ENV_NAME': 'LunarLander-v2',   # Gym environment name
     'ALGO': 'DQN',                  # Algorithm
@@ -297,36 +306,36 @@
         state = env.reset()[0]  # Reset environment at start of episode
         score = 0
         for idx_step in range(max_steps):
             if INIT_HP['CHANNELS_LAST']:
                 state = np.moveaxis(state, [3], [1])
             action = agent.getAction(state, epsilon)    # Get next action from agent
             next_state, reward, done, _, _ = env.step(action)   # Act in environment
-            
+
             # Save experience to replay buffer
             if INIT_HP['CHANNELS_LAST']:
                 memory.save2memoryVectEnvs(
                     state, action, reward, np.moveaxis(next_state, [3], [1]), done)
             else:
                 memory.save2memoryVectEnvs(
                     state, action, reward, next_state, done)
 
             # Learn according to learning frequency
             if memory.counter % agent.learn_step == 0 and len(memory) >= agent.batch_size:
                 experiences = memory.sample(agent.batch_size) # Sample replay buffer
                 agent.learn(experiences)    # Learn according to agent's RL algorithm
-            
+
             state = next_state
             score += reward
 
     epsilon = max(eps_end, epsilon*eps_decay) # Update epsilon for exploration
 
     # Now evolve population if necessary
     if (idx_epi+1) % evo_epochs == 0:
-        
+
         # Evaluate population
         fitnesses = [agent.test(env, swap_channels=INIT_HP['CHANNELS_LAST'], max_steps=max_steps, loop=evo_loop) for agent in pop]
 
         print(f'Episode {idx_epi+1}/{max_episodes}')
         print(f'Fitnesses: {["%.2f"%fitness for fitness in fitnesses]}')
         print(f'100 fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:]) for agent in pop]}')
 
@@ -576,15 +585,15 @@
         for idx_step in range(max_steps):
             experiences = memory.sample(agent.batch_size)   # Sample replay buffer
             # Learn according to agent's RL algorithm
             agent.learn(experiences)
 
     # Now evolve population if necessary
     if (idx_epi+1) % evo_epochs == 0:
-        
+
         # Evaluate population
         fitnesses = [agent.test(env, swap_channels=False, max_steps=max_steps, loop=evo_loop) for agent in pop]
 
         print(f'Episode {idx_epi+1}/{max_episodes}')
         print(f'Fitnesses: {["%.2f"%fitness for fitness in fitnesses]}')
         print(f'100 fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:]) for agent in pop]}')
 
@@ -592,38 +601,38 @@
         elite, pop = tournament.select(pop)
         pop = mutations.mutation(pop)
 
 env.close()
 ```
 
 ## Train an agent on a language environment (RLHF)
-We implement RLHF on Wordle, and use <a href="https://arxiv.org/pdf/2206.11871.pdf">ILQL</a> to finetune our model. To create your own language environment, 
+We implement RLHF on Wordle, and use <a href="https://arxiv.org/pdf/2206.11871.pdf">ILQL</a> to finetune our model. To create your own language environment,
 see https://github.com/Sea-Snell/Implicit-Language-Q-Learning.
-The <code>EvolvableGPT</code> class allows us to combine LLMs and transformer architectures with evolvable HPO, which can massively reduce the time taken to finetune 
-these expensive models. Due to the vast number of parameters and settings involved in training a Large Language Model (LLM) on human feedback, these are defined in 
-<code>configs</code>. 
+The <code>EvolvableGPT</code> class allows us to combine LLMs and transformer architectures with evolvable HPO, which can massively reduce the time taken to finetune
+these expensive models. Due to the vast number of parameters and settings involved in training a Large Language Model (LLM) on human feedback, these are defined in
+<code>configs</code>.
 
-In order to finetune a model with RLHF, we need a trained model as a starting point. We can use behavioural cloning (BC, supervised learning) to build this first version of 
+In order to finetune a model with RLHF, we need a trained model as a starting point. We can use behavioural cloning (BC, supervised learning) to build this first version of
 the model. To train your own model from scratch:
 ```bash
 python run_bc_lm.py
 ```
 If you want to use pretrained model weights, these can be defined in <code>configs/wordle/train_bc.yaml</code> in <code>model: load:</code>.
 
 Similarly, to then run ILQL and perform RLHF on the BC model:
 ```bash
 python run_ilql.py
 ```
 
 ## Distributed training
-AgileRL can also be used for distributed training if you have multiple devices you want to take advantage of. We use the HuggingFace 
-<a href="https://github.com/huggingface/accelerate">Accelerate</a> library to implement this in an open manner, without hiding behind too many layers of abstraction. 
+AgileRL can also be used for distributed training if you have multiple devices you want to take advantage of. We use the HuggingFace
+<a href="https://github.com/huggingface/accelerate">Accelerate</a> library to implement this in an open manner, without hiding behind too many layers of abstraction.
 This should make implementations simple, but also highly customisable, by continuing to expose the PyTorch training loop beneath it all.
 
-To launch distributed training scripts in bash, use <code>accelerate launch</code>. To customise the distributed training properties, specify the key <code>--config_file</code>. An example 
+To launch distributed training scripts in bash, use <code>accelerate launch</code>. To customise the distributed training properties, specify the key <code>--config_file</code>. An example
 config file has been provided at <code>configs/accelerate/accelerate.yaml</code>.
 
 Putting this all together, launching a distributed training script can be done as follows:
 ```bash
 accelerate_launch --config_file configs/accelerate/accelerate.yaml demo_online_distributed.py
 ```
 
@@ -695,16 +704,16 @@
     field_names = ["state", "action", "reward", "next_state", "done"]
     memory = ReplayBuffer(action_dim=action_dim,    # Number of agent actions
                         memory_size=10000,        # Max replay buffer size
                         field_names=field_names)  # Field names to store in memory
     replay_dataset = ReplayDataset(memory, INIT_HP['BATCH_SIZE'])
     replay_dataloader = DataLoader(replay_dataset, batch_size=None)
     replay_dataloader = accelerator.prepare(replay_dataloader)
-    sampler = Sampler(distributed=True, 
-                    dataset=replay_dataset, 
+    sampler = Sampler(distributed=True,
+                    dataset=replay_dataset,
                     dataloader=replay_dataloader)
 
     tournament = TournamentSelection(tournament_size=2,  # Tournament selection size
                                     elitism=True,      # Elitism in tournament selection
                                     population_size=INIT_HP['POPULATION_SIZE'],  # Population size
                                     evo_step=1)        # Evaluate using last N fitness scores
 
@@ -803,8 +812,162 @@
             accelerator.wait_for_everyone()
             for model in pop:
                 model.wrap_models()
 
     env.close()
 ```
 
+## Multi-agent training
+
+As in previous examples, before starting training, meta-hyperparameters ```INIT_HP```, ```MUTATION_PARAMS```, and ```NET_CONFIG``` must first be defined.
+
+```python
+NET_CONFIG = {
+        'arch': 'mlp',          # Network architecture
+        'h_size': [32, 32],     # Actor hidden size
+    }
+
+    INIT_HP = {
+        'ALGO': 'MADDPG',               # Algorithm
+        'BATCH_SIZE': 512,              # Batch size
+        'LR': 0.01,                     # Learning rate
+        'EPISODES': 10_000,             # Max no. episodes
+        'GAMMA': 0.95,                  # Discount factor
+        'MEMORY_SIZE': 1_000_000,       # Max memory buffer size
+        'LEARN_STEP': 5,                # Learning frequency
+        'TAU': 0.01,                    # For soft update of target parameters
+        # Swap image channels dimension from last to first [H, W, C] -> [C, H, W]
+        'CHANNELS_LAST': False,
+        "WANDB": False                  # Start run with Weights&Biases
+    }
+
+    MUTATION_PARAMS = {
+        "NO_MUT": 0.4,                              # No mutation
+        "ARCH_MUT": 0.2,                            # Architecture mutation
+        "NEW_LAYER": 0.2,                           # New layer mutation
+        "PARAMS_MUT": 0.2,                           # Network parameters mutation
+        "ACT_MUT": 0,                               # Activation layer mutation
+        "RL_HP_MUT": 0.2,                           # Learning HP mutation
+        # Learning HPs to choose from
+        "RL_HP_SELECTION": ["lr", "batch_size", "learn_step"],
+        "MUT_SD": 0.1,                              # Mutation strength
+        "RAND_SEED": 42,                            # Random seed
+        "MIN_LR": 0.0001,                           # Define max and min limits for mutating RL hyperparams
+        "MAX_LR": 0.01,
+        "MIN_LEARN_STEP": 1,
+        "MAX_LEARN_STEP": 200,
+        "MIN_BATCH_SIZE": 8,
+        "MAX_BATCH_SIZE": 1024
+    }
+```
+Use ```utils.utils.initialPopulation``` to create a list of agents - our population that will evolve and mutate to the optimal hyperparameters.
+```python
+    from agilerl.utils.utils import initialPopulation
+    from pettingzoo.mpe import simple_speaker_listener_v4
+    import torch
+
+    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+    env = simple_speaker_listener_v4.parallel_env(continuous_actions=True)
+    env.reset()
+
+    # Configure the multi-agent algo input arguments
+    try:
+        state_dim = [env.observation_space(agent).n for agent in env.agents]
+        one_hot = True
+    except Exception:
+        state_dim = [env.observation_space(agent).shape for agent in env.agents]
+        one_hot = False
+    try:
+        action_dim = [env.action_space(agent).n for agent in env.agents]
+        INIT_HP['DISCRETE_ACTIONS'] = True
+        INIT_HP['MAX_ACTION'] = None
+        INIT_HP['MIN_ACTION'] = None
+    except Exception:
+        action_dim = [env.action_space(agent).shape[0] for agent in env.agents]
+        INIT_HP['DISCRETE_ACTIONS'] = False
+        INIT_HP['MAX_ACTION'] = [env.action_space(agent).high for agent in env.agents]
+        INIT_HP['MIN_ACTION'] = [env.action_space(agent).low for agent in env.agents]
+
+    if INIT_HP['CHANNELS_LAST']:
+        state_dim = [(state_dim[2], state_dim[0], state_dim[1]) for state_dim in state_dim]
+
+    INIT_HP['N_AGENTS'] = env.num_agents
+    INIT_HP['AGENT_IDS'] = [agent_id for agent_id in env.agents]
+
+    agent_pop = initialPopulation(algo=INIT_HP['ALGO'],
+                                  state_dim=state_dim,
+                                  action_dim=action_dim,
+                                  one_hot=one_hot,
+                                  net_config=NET_CONFIG,
+                                  INIT_HP=INIT_HP,
+                                  population_size=6,
+                                  device=device)
+
+```
+
+Next, create the tournament, mutations and experience replay buffer objects that allow agents to share memory and efficiently perform evolutionary HPO.
+
+```python
+    from agilerl.components.multi_agent_replay_buffer import MultiAgentReplayBuffer
+    from agilerl.hpo.tournament import TournamentSelection
+    from agilerl.hpo.mutation import Mutations
+
+    field_names = ["state", "action", "reward", "next_state", "done"]
+
+    memory = MultiAgentReplayBuffer(memory_size=1_000_000,        # Max replay buffer size
+                                    field_names=field_names,  # Field names to store in memory
+                                    agent_ids=INIT_HP['AGENT_IDS'],
+                                    device=torch.device("cuda"))
+
+    tournament = TournamentSelection(tournament_size=2, # Tournament selection size
+                                     elitism=True,      # Elitism in tournament selection
+                                     population_size=6, # Population size
+                                     evo_step=1)        # Evaluate using last N fitness scores
+
+    mutations = Mutations(algo=INIT_HP['ALGO'],
+                          no_mutation=MUTATION_PARAMS['NO_MUT'],
+                          architecture=MUTATION_PARAMS['ARCH_MUT'],
+                          new_layer_prob=MUTATION_PARAMS['NEW_LAYER'],
+                          parameters=MUTATION_PARAMS['PARAMS_MUT'],
+                          activation=MUTATION_PARAMS['ACT_MUT'],
+                          rl_hp=MUTATION_PARAMS['RL_HP_MUT'],
+                          rl_hp_selection=MUTATION_PARAMS['RL_HP_SELECTION'],
+                          mutation_sd=MUTATION_PARAMS['MUT_SD'],
+                          min_lr=MUTATION_PARAMS['MIN_LR'],
+                          max_lr=MUTATION_PARAMS['MAX_LR'],
+                          min_learn_step=MUTATION_PARAMS['MIN_LEARN_STEP'],
+                          max_learn_step=MUTATION_PARAMS['MAX_LEARN_STEP'],
+                          min_batch_size=MUTATION_PARAMS['MIN_BATCH_SIZE'],
+                          max_batch_size=MUTATION_PARAMS['MAX_BATCH_SIZE'],
+                          agent_ids=INIT_HP['AGENT_IDS'],
+                          arch=NET_CONFIG['arch'],
+                          rand_seed=MUTATION_PARAMS['RAND_SEED'],
+                          device=device)
+
+```
+The easiest training loop implementation is to use our ```training.train_multi_agent.train_multi_agent()``` function. It requires the agent have functions ```getAction()``` and ```learn()```.
+
+```python
+
+    from agilerl.training.train_multi_agent import train_multi_agent
+    import torch
+
+    trained_pop, pop_fitnesses = train_multi_agent(env=env,                              # Pettingzoo-style environment
+                                                env_name='simple_speaker_listener_v4',   # Environment name
+                                                algo=INIT_HP['ALGO'],                    # Algorithm
+                                                pop=agent_pop,                           # Population of agents
+                                                memory=memory,                           # Replay buffer
+                                                INIT_HP=INIT_HP,                         # IINIT_HP dictionary
+                                                MUT_P=MUTATION_PARAMS,                   # MUTATION_PARAMS dictionary
+                                                net_config=NET_CONFIG,                   # Network configuration
+                                                swap_channels=INIT_HP['CHANNELS_LAST'],  # Swap image channel from last to first
+                                                n_episodes=INIT_HP['EPISODES'],          # Max number of training episodes
+                                                evo_epochs=20,                           # Evolution frequency
+                                                evo_loop=1,                              # Number of evaluation episodes per agent
+                                                max_steps=900,                           # Max steps to take in the environment
+                                                target=200.,                             # Target score for early stopping
+                                                tournament=tournament,                   # Tournament selection object
+                                                mutation=mutations,                      # Mutations object
+                                                wb=INIT_HP["WANDB"])                     # Weights and Biases tracking
+
+```
 View <a href="https://agilerl.readthedocs.io/en/latest/">documentation</a>.
```

#### html2text {}

```diff
@@ -33,61 +33,68 @@
 ## Table of Contents * [Benchmarks](#benchmarks) * [Get Started](#get-started)
 * [Algorithms implemented](#algorithms-implemented-more-coming-soon) * [Train
 an agent on a Gym environment (Online)](#train-an-agent-on-a-gym-environment-
 online) + [Custom Online Training Loop](#custom-online-training-loop) * [Train
 an agent on data (Offline)](#train-an-agent-on-data-offline) + [Custom Offline
 Training Loop](#custom-offline-training-loop) * [Train an agent on a language
 environment (RLHF)](#train-an-agent-on-a-language-environment-rlhf) *
-[Distributed training](#distributed-training) ## Benchmarks Reinforcement
-learning algorithms and libraries are usually benchmarked once the optimal
-hyperparameters for training are known, but it often takes hundreds or
-thousands of experiments to discover these. This is unrealistic and does not
-reflect the true, total time taken for training. What if we could remove the
-need to conduct all these prior experiments? In the charts below, a single
-AgileRL run, which automatically tunes hyperparameters, is benchmarked against
-Optuna's multiple training runs traditionally required for hyperparameter
-optimization, demonstrating the real time savings possible. Global steps is the
-sum of every step taken by any agent in the environment, including across an
-entire population.
+[Distributed training](#distributed-training) * [Multi-agent training](#multi-
+agent-training) ## Benchmarks Reinforcement learning algorithms and libraries
+are usually benchmarked once the optimal hyperparameters for training are
+known, but it often takes hundreds or thousands of experiments to discover
+these. This is unrealistic and does not reflect the true, total time taken for
+training. What if we could remove the need to conduct all these prior
+experiments? In the charts below, a single AgileRL run, which automatically
+tunes hyperparameters, is benchmarked against Optuna's multiple training runs
+traditionally required for hyperparameter optimization, demonstrating the real
+time savings possible. Global steps is the sum of every step taken by any agent
+in the environment, including across an entire population.
  [https://user-images.githubusercontent.com/47857277/227481592-27a9688f-7c0a-
                           4655-ab32-90d659a71c69.png]
 AgileRL offers an order of magnitude speed up in hyperparameter optimization vs
 popular reinforcement learning training frameworks combined with Optuna. Remove
          the need for multiple training runs and save yourself hours.
+AgileRL also supports multi-agent reinforcement learning using the Petting Zoo-
+style (parallel API). The charts below highlight the performance of our MADDPG
+and MATD3 algorithms with evolutionary hyper-parameter optimisation (HPO),
+benchmarked against epymarl's MADDPG algorithm with grid-search HPO for the
+simple speaker listener and simple spread environments.
+   [https://github-production-user-asset-6210df.s3.amazonaws.com/118982716/
+              264712154-4965ea5f-b777-423c-989b-e4db86eda3bd.png]
 ## Get Started Install as a package with pip: ```bash pip install agilerl ```
 Or install in development mode: (Recommended due to nascent nature of this
 library) ```bash git clone https://github.com/AgileRL/AgileRL.git && cd AgileRL
 pip install -r requirements.txt ``` If using ILQL on Wordle, download and unzip
 data.zip _h_e_r_e. Demo: ```bash python demo_online.py ``` or to demo distributed
 training: ```bash accelerate launch --config_file configs/accelerate/
 accelerate.yaml demo_online_distributed.py ``` ## Algorithms implemented (more
-coming soon!) * DQN * DDPG * CQL * ILQL * TD3 ## Train an agent on a Gym
-environment (Online) Before starting training, there are some meta-
-hyperparameters and settings that must be set. These are defined in INIT_HP,
-for general parameters, and MUTATION_PARAMS, which define the evolutionary
-probabilities, and NET_CONFIG, which defines the network architecture. For
-example: ```python INIT_HP = { 'ENV_NAME': 'LunarLander-v2', # Gym environment
-name 'ALGO': 'DQN', # Algorithm 'DOUBLE': True, # Use double Q-learning
-'CHANNELS_LAST': False, # Swap image channels dimension from last to first [H,
-W, C] -> [C, H, W] 'BATCH_SIZE': 256, # Batch size 'LR': 1e-3, # Learning rate
-'EPISODES': 2000, # Max no. episodes 'TARGET_SCORE': 200., # Early training
-stop at avg score of last 100 episodes 'GAMMA': 0.99, # Discount factor
-'MEMORY_SIZE': 10000, # Max memory buffer size 'LEARN_STEP': 1, # Learning
-frequency 'TAU': 1e-3, # For soft update of target parameters 'TOURN_SIZE': 2,
-# Tournament size 'ELITISM': True, # Elitism in tournament selection
-'POP_SIZE': 6, # Population size 'EVO_EPOCHS': 20, # Evolution frequency
-'POLICY_FREQ': 2, # Policy network update frequency 'WANDB': True # Log with
-Weights and Biases } ``` ```python MUTATION_PARAMS = { # Relative probabilities
-'NO_MUT': 0.4, # No mutation 'ARCH_MUT': 0.2, # Architecture mutation
-'NEW_LAYER': 0.2, # New layer mutation 'PARAMS_MUT': 0.2, # Network parameters
-mutation 'ACT_MUT': 0, # Activation layer mutation 'RL_HP_MUT': 0.2, # Learning
-HP mutation 'RL_HP_SELECTION': ['lr', 'batch_size'], # Learning HPs to choose
-from 'MUT_SD': 0.1, # Mutation strength 'RAND_SEED': 1, # Random seed } ```
-```python NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size': [32,
-32], # Actor hidden size } ``` First, use utils.utils.initialPopulation to
+coming soon!) * DQN * DDPG * CQL * ILQL * TD3 * MADDPG * MATD3 ## Train an
+agent on a Gym environment (Online) Before starting training, there are some
+meta-hyperparameters and settings that must be set. These are defined in
+INIT_HP, for general parameters, and MUTATION_PARAMS, which define the
+evolutionary probabilities, and NET_CONFIG, which defines the network
+architecture. For example: ```python INIT_HP = { 'ENV_NAME': 'LunarLander-v2',
+# Gym environment name 'ALGO': 'DQN', # Algorithm 'DOUBLE': True, # Use double
+Q-learning 'CHANNELS_LAST': False, # Swap image channels dimension from last to
+first [H, W, C] -> [C, H, W] 'BATCH_SIZE': 256, # Batch size 'LR': 1e-3, #
+Learning rate 'EPISODES': 2000, # Max no. episodes 'TARGET_SCORE': 200., #
+Early training stop at avg score of last 100 episodes 'GAMMA': 0.99, # Discount
+factor 'MEMORY_SIZE': 10000, # Max memory buffer size 'LEARN_STEP': 1, #
+Learning frequency 'TAU': 1e-3, # For soft update of target parameters
+'TOURN_SIZE': 2, # Tournament size 'ELITISM': True, # Elitism in tournament
+selection 'POP_SIZE': 6, # Population size 'EVO_EPOCHS': 20, # Evolution
+frequency 'POLICY_FREQ': 2, # Policy network update frequency 'WANDB': True #
+Log with Weights and Biases } ``` ```python MUTATION_PARAMS = { # Relative
+probabilities 'NO_MUT': 0.4, # No mutation 'ARCH_MUT': 0.2, # Architecture
+mutation 'NEW_LAYER': 0.2, # New layer mutation 'PARAMS_MUT': 0.2, # Network
+parameters mutation 'ACT_MUT': 0, # Activation layer mutation 'RL_HP_MUT': 0.2,
+# Learning HP mutation 'RL_HP_SELECTION': ['lr', 'batch_size'], # Learning HPs
+to choose from 'MUT_SD': 0.1, # Mutation strength 'RAND_SEED': 1, # Random seed
+} ``` ```python NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size':
+[32, 32], # Actor hidden size } ``` First, use utils.utils.initialPopulation to
 create a list of agents - our population that will evolve and mutate to the
 optimal hyperparameters. ```python from agilerl.utils.utils import
 makeVectEnvs, initialPopulation import torch device = torch.device("cuda" if
 torch.cuda.is_available() else "cpu") env = makeVectEnvs(env_name=INIT_HP
 ['ENV_NAME'], num_envs=16) try: state_dim = env.single_observation_space.n #
 Discrete observation space one_hot = True # Requires one-hot encoding except
 Exception: state_dim = env.single_observation_space.shape # Continuous
@@ -437,8 +444,86 @@
 pop: model.unwrap_models() accelerator.wait_for_everyone() if
 accelerator.is_main_process: elite, pop = tournament.select(pop) pop =
 mutations.mutation(pop) for pop_i, model in enumerate(pop):
 model.saveCheckpoint(f'{accel_temp_models_path}/DQN_{pop_i}.pt')
 accelerator.wait_for_everyone() if not accelerator.is_main_process: for pop_i,
 model in enumerate(pop): model.loadCheckpoint(f'{accel_temp_models_path}/DQN_
 {pop_i}.pt') accelerator.wait_for_everyone() for model in pop:
-model.wrap_models() env.close() ``` View _d_o_c_u_m_e_n_t_a_t_i_o_n.
+model.wrap_models() env.close() ``` ## Multi-agent training As in previous
+examples, before starting training, meta-hyperparameters ```INIT_HP```,
+```MUTATION_PARAMS```, and ```NET_CONFIG``` must first be defined. ```python
+NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size': [32, 32], #
+Actor hidden size } INIT_HP = { 'ALGO': 'MADDPG', # Algorithm 'BATCH_SIZE':
+512, # Batch size 'LR': 0.01, # Learning rate 'EPISODES': 10_000, # Max no.
+episodes 'GAMMA': 0.95, # Discount factor 'MEMORY_SIZE': 1_000_000, # Max
+memory buffer size 'LEARN_STEP': 5, # Learning frequency 'TAU': 0.01, # For
+soft update of target parameters # Swap image channels dimension from last to
+first [H, W, C] -> [C, H, W] 'CHANNELS_LAST': False, "WANDB": False # Start run
+with Weights&Biases } MUTATION_PARAMS = { "NO_MUT": 0.4, # No mutation
+"ARCH_MUT": 0.2, # Architecture mutation "NEW_LAYER": 0.2, # New layer mutation
+"PARAMS_MUT": 0.2, # Network parameters mutation "ACT_MUT": 0, # Activation
+layer mutation "RL_HP_MUT": 0.2, # Learning HP mutation # Learning HPs to
+choose from "RL_HP_SELECTION": ["lr", "batch_size", "learn_step"], "MUT_SD":
+0.1, # Mutation strength "RAND_SEED": 42, # Random seed "MIN_LR": 0.0001, #
+Define max and min limits for mutating RL hyperparams "MAX_LR": 0.01,
+"MIN_LEARN_STEP": 1, "MAX_LEARN_STEP": 200, "MIN_BATCH_SIZE": 8,
+"MAX_BATCH_SIZE": 1024 } ``` Use ```utils.utils.initialPopulation``` to create
+a list of agents - our population that will evolve and mutate to the optimal
+hyperparameters. ```python from agilerl.utils.utils import initialPopulation
+from pettingzoo.mpe import simple_speaker_listener_v4 import torch device =
+torch.device("cuda" if torch.cuda.is_available() else "cpu") env =
+simple_speaker_listener_v4.parallel_env(continuous_actions=True) env.reset() #
+Configure the multi-agent algo input arguments try: state_dim =
+[env.observation_space(agent).n for agent in env.agents] one_hot = True except
+Exception: state_dim = [env.observation_space(agent).shape for agent in
+env.agents] one_hot = False try: action_dim = [env.action_space(agent).n for
+agent in env.agents] INIT_HP['DISCRETE_ACTIONS'] = True INIT_HP['MAX_ACTION'] =
+None INIT_HP['MIN_ACTION'] = None except Exception: action_dim =
+[env.action_space(agent).shape[0] for agent in env.agents] INIT_HP
+['DISCRETE_ACTIONS'] = False INIT_HP['MAX_ACTION'] = [env.action_space
+(agent).high for agent in env.agents] INIT_HP['MIN_ACTION'] = [env.action_space
+(agent).low for agent in env.agents] if INIT_HP['CHANNELS_LAST']: state_dim = [
+(state_dim[2], state_dim[0], state_dim[1]) for state_dim in state_dim] INIT_HP
+['N_AGENTS'] = env.num_agents INIT_HP['AGENT_IDS'] = [agent_id for agent_id in
+env.agents] agent_pop = initialPopulation(algo=INIT_HP['ALGO'],
+state_dim=state_dim, action_dim=action_dim, one_hot=one_hot,
+net_config=NET_CONFIG, INIT_HP=INIT_HP, population_size=6, device=device) ```
+Next, create the tournament, mutations and experience replay buffer objects
+that allow agents to share memory and efficiently perform evolutionary HPO.
+```python from agilerl.components.multi_agent_replay_buffer import
+MultiAgentReplayBuffer from agilerl.hpo.tournament import TournamentSelection
+from agilerl.hpo.mutation import Mutations field_names = ["state", "action",
+"reward", "next_state", "done"] memory = MultiAgentReplayBuffer
+(memory_size=1_000_000, # Max replay buffer size field_names=field_names, #
+Field names to store in memory agent_ids=INIT_HP['AGENT_IDS'],
+device=torch.device("cuda")) tournament = TournamentSelection
+(tournament_size=2, # Tournament selection size elitism=True, # Elitism in
+tournament selection population_size=6, # Population size evo_step=1) #
+Evaluate using last N fitness scores mutations = Mutations(algo=INIT_HP
+['ALGO'], no_mutation=MUTATION_PARAMS['NO_MUT'], architecture=MUTATION_PARAMS
+['ARCH_MUT'], new_layer_prob=MUTATION_PARAMS['NEW_LAYER'],
+parameters=MUTATION_PARAMS['PARAMS_MUT'], activation=MUTATION_PARAMS
+['ACT_MUT'], rl_hp=MUTATION_PARAMS['RL_HP_MUT'],
+rl_hp_selection=MUTATION_PARAMS['RL_HP_SELECTION'], mutation_sd=MUTATION_PARAMS
+['MUT_SD'], min_lr=MUTATION_PARAMS['MIN_LR'], max_lr=MUTATION_PARAMS['MAX_LR'],
+min_learn_step=MUTATION_PARAMS['MIN_LEARN_STEP'],
+max_learn_step=MUTATION_PARAMS['MAX_LEARN_STEP'],
+min_batch_size=MUTATION_PARAMS['MIN_BATCH_SIZE'],
+max_batch_size=MUTATION_PARAMS['MAX_BATCH_SIZE'], agent_ids=INIT_HP
+['AGENT_IDS'], arch=NET_CONFIG['arch'], rand_seed=MUTATION_PARAMS['RAND_SEED'],
+device=device) ``` The easiest training loop implementation is to use our
+```training.train_multi_agent.train_multi_agent()``` function. It requires the
+agent have functions ```getAction()``` and ```learn()```. ```python from
+agilerl.training.train_multi_agent import train_multi_agent import torch
+trained_pop, pop_fitnesses = train_multi_agent(env=env, # Pettingzoo-style
+environment env_name='simple_speaker_listener_v4', # Environment name
+algo=INIT_HP['ALGO'], # Algorithm pop=agent_pop, # Population of agents
+memory=memory, # Replay buffer INIT_HP=INIT_HP, # IINIT_HP dictionary
+MUT_P=MUTATION_PARAMS, # MUTATION_PARAMS dictionary net_config=NET_CONFIG, #
+Network configuration swap_channels=INIT_HP['CHANNELS_LAST'], # Swap image
+channel from last to first n_episodes=INIT_HP['EPISODES'], # Max number of
+training episodes evo_epochs=20, # Evolution frequency evo_loop=1, # Number of
+evaluation episodes per agent max_steps=900, # Max steps to take in the
+environment target=200., # Target score for early stopping
+tournament=tournament, # Tournament selection object mutation=mutations, #
+Mutations object wb=INIT_HP["WANDB"]) # Weights and Biases tracking ``` View
+_d_o_c_u_m_e_n_t_a_t_i_o_n.
```

### Comparing `agilerl-0.1.8/agilerl/algorithms/bc_lm.py` & `agilerl-0.1.9/agilerl/algorithms/bc_lm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,429 +1,612 @@
+from typing import Any, Callable, Optional, Tuple, Union
+
+import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from typing import Any, Callable, Optional, Tuple, Union
-import numpy as np
-from agilerl.networks.evolvable_gpt import EvolvableGPT
-from agilerl.data.rl_data import DataPoint, RL_Dataset
+
 from agilerl.data.language_environment import Language_Observation, interact_environment
-from agilerl.utils.sampling_utils import process_logits, pad_sequence, map_all_kvs, \
-    update_kvs, always_terminate
+from agilerl.data.rl_data import DataPoint, RL_Dataset
+from agilerl.networks.evolvable_gpt import EvolvableGPT
+from agilerl.utils.sampling_utils import (
+    always_terminate,
+    map_all_kvs,
+    pad_sequence,
+    process_logits,
+    update_kvs,
+)
+
 
 class BC_LM(nn.Module):
-    def __init__(self, 
-                 dataset: RL_Dataset, 
-                 net_config,
-                 device: Union[torch.device, str] = "cuda", 
-                 transition_weight: float=0.0, 
-                ):
-        super(BC_LM, self).__init__()
+    def __init__(
+        self,
+        dataset: RL_Dataset,
+        net_config,
+        device: Union[torch.device, str] = "cuda",
+        transition_weight: float = 0.0,
+    ):
+        super().__init__()
 
         self.dataset = dataset
         self.device = device
         self.model = EvolvableGPT(
-            n_layer=net_config['n_layer'],
-            vocab_size=net_config['vocab_size'],
-            n_embd=net_config['n_embd'],
-            n_head=net_config['n_head'],
-            dim_feedfwd=net_config['dim_feedfwd'],
-            block_size=net_config['block_size'],
-            dropout=net_config['dropout'],
-            activation=net_config['activation'],
-            layer_norm_eps=net_config['layer_norm_eps'],
-            min_layers=net_config['min_layers'],
-            max_layers=net_config['max_layers'],
-            bias=net_config['bias'],
-            device=self.device).to(
-            self.device)
+            n_layer=net_config["n_layer"],
+            vocab_size=net_config["vocab_size"],
+            n_embd=net_config["n_embd"],
+            n_head=net_config["n_head"],
+            dim_feedfwd=net_config["dim_feedfwd"],
+            block_size=net_config["block_size"],
+            dropout=net_config["dropout"],
+            activation=net_config["activation"],
+            layer_norm_eps=net_config["layer_norm_eps"],
+            min_layers=net_config["min_layers"],
+            max_layers=net_config["max_layers"],
+            bias=net_config["bias"],
+            device=self.device,
+        ).to(self.device)
         self.max_len = self.dataset.max_len
-        self.h_dim  = net_config['n_embd']
+        self.h_dim = net_config["n_embd"]
         self.transition_weight = transition_weight
 
-    def forward(self, 
-                tokens: torch.Tensor, 
-                attn_mask: Optional[torch.Tensor], 
-                prefix_embs: Optional[torch.Tensor]=None, 
-                prefix_attn_mask: Optional[torch.Tensor]=None, 
-                remove_prefix_position_embs: bool=False, 
-                **kwargs):
+    def forward(
+        self,
+        tokens: torch.Tensor,
+        attn_mask: Optional[torch.Tensor],
+        prefix_embs: Optional[torch.Tensor] = None,
+        prefix_attn_mask: Optional[torch.Tensor] = None,
+        remove_prefix_position_embs: bool = False,
+        **kwargs
+    ):
         # tokens – b,t
         # attn_mask – b,t
         # prefix_embs – b,t',d
         # prefix_attn_mask - b, t'
         if prefix_embs is None:
             prefix_embs = torch.empty((tokens.shape[0], 0, self.h_dim)).to(self.device)
         set_pos_ids = prefix_attn_mask is not None
         if prefix_attn_mask is not None and attn_mask is not None:
             input_attn_mask = torch.cat((prefix_attn_mask, attn_mask), dim=1)
         else:
             input_attn_mask = None
-        position_ids = torch.cumsum(input_attn_mask, dim=1)-1 if set_pos_ids else None
+        position_ids = torch.cumsum(input_attn_mask, dim=1) - 1 if set_pos_ids else None
         if remove_prefix_position_embs:
             prefix_embs -= self.model.transformer.wpe(
-                position_ids[:, :prefix_embs.shape[1]])
-        input_embeddings = torch.cat((prefix_embs, self.model.transformer.wte(tokens)), 
-                                     dim=1)
-        
+                position_ids[:, : prefix_embs.shape[1]]
+            )
+        input_embeddings = torch.cat(
+            (prefix_embs, self.model.transformer.wte(tokens)), dim=1
+        )
+
         model_outputs, _, model_past_key_values, _ = self.model(
-                                   tok_emb=input_embeddings, 
-                                   attn_mask=input_attn_mask, 
-                                   pos=position_ids, 
-                                   **kwargs)
+            tok_emb=input_embeddings,
+            attn_mask=input_attn_mask,
+            pos=position_ids,
+            **kwargs
+        )
         return model_outputs, model_past_key_values
-    
-    def get_weights(self, 
-                    tokens: torch.Tensor, 
-                    action_idxs: torch.Tensor):
+
+    def get_weights(self, tokens: torch.Tensor, action_idxs: torch.Tensor):
         weights = torch.full(tokens.shape, self.transition_weight).to(self.device)
         if action_idxs.shape[1] == 0:
             n = torch.zeros((tokens.shape[0],)).long().to(self.device)
         else:
-            n = torch.argmax(action_idxs, dim=1)+1
+            n = torch.argmax(action_idxs, dim=1) + 1
         for i in range(tokens.shape[0]):
-            weights[i] = torch.scatter(weights[i], 
-                                       dim=0, 
-                                       index=action_idxs[i, :n[i]], 
-                                       src=torch.full((n[i].item(),), 
-                                                      1.0).to(self.device))
+            weights[i] = torch.scatter(
+                weights[i],
+                dim=0,
+                index=action_idxs[i, : n[i]],
+                src=torch.full((n[i].item(),), 1.0).to(self.device),
+            )
         return weights
-    
+
     def awac_loss(self, tokens, attn_mask, logits, w):
         w = w.detach()
-        losses = F.cross_entropy(logits[:, :-1, :].reshape(-1, logits.shape[-1]), 
-                                 tokens[:, 1:].reshape(-1), reduction='none')
-        losses = losses.reshape(tokens.shape[0], tokens.shape[1]-1)
+        losses = F.cross_entropy(
+            logits[:, :-1, :].reshape(-1, logits.shape[-1]),
+            tokens[:, 1:].reshape(-1),
+            reduction="none",
+        )
+        losses = losses.reshape(tokens.shape[0], tokens.shape[1] - 1)
         return (losses * w[:, :-1] * attn_mask[:, 1:]).sum() / attn_mask[:, 1:].sum()
 
     def get_loss(self, items):
         prepared_inputs = self.prepare_inputs(items)
-        tokens, attn_mask = prepared_inputs['tokens'], prepared_inputs['attn_mask']
-        a_idx = prepared_inputs['action_idxs']
+        tokens, attn_mask = prepared_inputs["tokens"], prepared_inputs["attn_mask"]
+        a_idx = prepared_inputs["action_idxs"]
         logits, _ = self(tokens, attn_mask)
         logs = {}
         n = attn_mask.sum().item()
         weights = self.get_weights(tokens, a_idx)
         token_loss = self.awac_loss(tokens, attn_mask, logits, weights)
-        logs['loss'] = (token_loss.item(), n)
+        logs["loss"] = (token_loss.item(), n)
         return token_loss, logs, []
-    
+
     def prepare_inputs(self, items):
         if isinstance(items, dict):
             return items
         return to(self.dataset.collate(items, self.device), self.device)
-    
-    def score(self, model_args, model_kwargs, 
-              temp: float=1.0, 
-              top_k: Optional[int]=None, 
-              top_p: Optional[float]=None):
+
+    def score(
+        self,
+        model_args,
+        model_kwargs,
+        temp: float = 1.0,
+        top_k: Optional[int] = None,
+        top_p: Optional[float] = None,
+    ):
         logits, _ = self(*model_args, **model_kwargs)
         logits = process_logits(logits, temp=temp, top_k=top_k, top_p=top_p)
         return torch.log(F.softmax(logits, dim=-1)), logits
-    
-    def get_scores(self, 
-                   items, 
-                   temp: float=1.0, 
-                   top_k: Optional[int]=None, 
-                   top_p: Optional[float]=None) -> torch.Tensor:
+
+    def get_scores(
+        self,
+        items,
+        temp: float = 1.0,
+        top_k: Optional[int] = None,
+        top_p: Optional[float] = None,
+    ) -> torch.Tensor:
         prepared_inputs = self.prepare_inputs(items)
-        tokens, attn_mask = prepared_inputs['tokens'], prepared_inputs['attn_mask']
-        return self.score((tokens, attn_mask,), {}, 
-                          temp=temp, top_k=top_k, top_p=top_p)[0]
-
-    def initial_score(self, 
-                      items, 
-                      temp: float=1.0, 
-                      top_k: Optional[int]=None, 
-                      top_p: Optional[float]=None) -> Tuple[torch.Tensor, Any]:
+        tokens, attn_mask = prepared_inputs["tokens"], prepared_inputs["attn_mask"]
+        return self.score(
+            (
+                tokens,
+                attn_mask,
+            ),
+            {},
+            temp=temp,
+            top_k=top_k,
+            top_p=top_p,
+        )[0]
+
+    def initial_score(
+        self,
+        items,
+        temp: float = 1.0,
+        top_k: Optional[int] = None,
+        top_p: Optional[float] = None,
+    ) -> Tuple[torch.Tensor, Any]:
         prepared_inputs = self.prepare_inputs(items)
-        tokens = prepared_inputs['tokens']
-        scores, model_outputs = self.score((tokens, None,), {}, 
-                                           temp=temp, top_k=top_k, top_p=top_p)
+        tokens = prepared_inputs["tokens"]
+        scores, model_outputs = self.score(
+            (
+                tokens,
+                None,
+            ),
+            {},
+            temp=temp,
+            top_k=top_k,
+            top_p=top_p,
+        )
         return scores[:, -1, :], model_outputs.past_key_values
-    
-    def next_score(self, 
-                   tokens: torch.Tensor, 
-                   state: Any, 
-                   temp: float=1.0, 
-                   top_k: Optional[int]=None, 
-                   top_p: Optional[float]=None) -> Tuple[torch.Tensor, Any]:
-        scores, model_outputs = self.score((tokens.unsqueeze(1), None,), 
-                                            {'past_key_values': state}, 
-                                           temp=temp, top_k=top_k, top_p=top_p)
+
+    def next_score(
+        self,
+        tokens: torch.Tensor,
+        state: Any,
+        temp: float = 1.0,
+        top_k: Optional[int] = None,
+        top_p: Optional[float] = None,
+    ) -> Tuple[torch.Tensor, Any]:
+        scores, model_outputs = self.score(
+            (
+                tokens.unsqueeze(1),
+                None,
+            ),
+            {"past_key_values": state},
+            temp=temp,
+            top_k=top_k,
+            top_p=top_p,
+        )
         return scores.squeeze(1), model_outputs.past_key_values
 
-class BC_Policy():
-    def __init__(self, bc_lm: BC_LM, 
-                 kind: str, **generation_kwargs) -> None:
+
+class BC_Policy:
+    def __init__(self, bc_lm: BC_LM, kind: str, **generation_kwargs) -> None:
         super().__init__()
         self.bc_lm = bc_lm
-        assert kind in {'sample', 'beam'}
+        assert kind in {"sample", "beam"}
         self.kind = kind
         self.generation_kwargs = generation_kwargs
-    
-    def sample_raw(self, 
-                   tokens: torch.Tensor, attn_mask: torch.Tensor, 
-                   termination_condition: Callable[[np.ndarray], bool], 
-                   num_generations=1, max_generation_len=None, 
-                   temp=1.0, top_k=None, top_p=None, 
-                   prefix_embs: Optional[torch.Tensor]=None, 
-                   prefix_attn_mask: Optional[torch.Tensor]=None, 
-                   remove_prefix_position_embs: bool=False):
+
+    def sample_raw(
+        self,
+        tokens: torch.Tensor,
+        attn_mask: torch.Tensor,
+        termination_condition: Callable[[np.ndarray], bool],
+        num_generations=1,
+        max_generation_len=None,
+        temp=1.0,
+        top_k=None,
+        top_p=None,
+        prefix_embs: Optional[torch.Tensor] = None,
+        prefix_attn_mask: Optional[torch.Tensor] = None,
+        remove_prefix_position_embs: bool = False,
+    ):
         tokenizer = self.bc_lm.dataset.tokenizer
         max_length = self.bc_lm.dataset.max_len
         if max_length is None:
             max_length = self.bc_lm.model.block_size
         max_length = min(max_length, self.bc_lm.model.block_size)
         device = self.bc_lm.device
         bsize = tokens.shape[0]
         n = bsize * num_generations
         if max_generation_len is None:
-            max_generation_len = max_length+1
-        input_strs = [tokenizer.decode(
-            tokens[i, :][:attn_mask[i, :].sum().long()].tolist(), 
-            clean_up_tokenization_spaces=False) for i in range(len(tokens))]
+            max_generation_len = max_length + 1
+        input_strs = [
+            tokenizer.decode(
+                tokens[i, :][: attn_mask[i, :].sum().long()].tolist(),
+                clean_up_tokenization_spaces=False,
+            )
+            for i in range(len(tokens))
+        ]
         prefix_t = 0 if prefix_embs is None else prefix_embs.shape[1]
-        logits, past_key_values = self.bc_lm(tokens=tokens, 
-                                   attn_mask=attn_mask, 
-                                   prefix_embs=prefix_embs, 
-                                   prefix_attn_mask=prefix_attn_mask, 
-                                   remove_prefix_position_embs=remove_prefix_position_embs,
-                                   is_causal=False)
+        logits, past_key_values = self.bc_lm(
+            tokens=tokens,
+            attn_mask=attn_mask,
+            prefix_embs=prefix_embs,
+            prefix_attn_mask=prefix_attn_mask,
+            remove_prefix_position_embs=remove_prefix_position_embs,
+            is_causal=False,
+        )
         dialogue_kvs = past_key_values
         dialogue_lens = attn_mask.sum(dim=1)
-        tokens = pad_sequence(torch.repeat_interleave(tokens, num_generations, dim=0), 
-                              max_length, tokenizer.pad_token_id, device, 1)
+        tokens = pad_sequence(
+            torch.repeat_interleave(tokens, num_generations, dim=0),
+            max_length,
+            tokenizer.pad_token_id,
+            device,
+            1,
+        )
         dialogue_lens = torch.repeat_interleave(dialogue_lens, num_generations, dim=0)
-        dialogue_kvs = map_all_kvs(lambda x: pad_sequence(
-            torch.repeat_interleave(x, num_generations, dim=0), 
-            max_length, 0.0, device, 2), dialogue_kvs)
+        dialogue_kvs = map_all_kvs(
+            lambda x: pad_sequence(
+                torch.repeat_interleave(x, num_generations, dim=0),
+                max_length,
+                0.0,
+                device,
+                2,
+            ),
+            dialogue_kvs,
+        )
         log_probs = torch.full((dialogue_lens.shape[0],), 0.0).to(device)
         termination_mask = torch.full((dialogue_lens.shape[0],), 1).to(device)
         t = torch.min(dialogue_lens).int()
-        while termination_mask.sum() > 0 and (t+prefix_t) < max_length:
-            curr_token = tokens[:, t-1].unsqueeze(1)
-            curr_dialogue_kvs = map_all_kvs(lambda x: x[:,:,:(t+prefix_t)-1,:], 
-                                            dialogue_kvs)
-            logits, past_key_values = self.bc_lm(curr_token, None, 
-                                                 past_key_values=curr_dialogue_kvs, 
-                                                 is_causal=False)
-            logits[:, 0, tokenizer.pad_token_id] = torch.where(termination_mask == 1, 
-                                                               float('-inf'), 1e7)
-            logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(device), 
-                   tokens[:, t]] = logits[torch.arange(0, n).to(device), 
-                                          torch.full((n,), 0).to(device), 
-                                          tokens[:, t]].masked_fill_(t < dialogue_lens, 
-                                                                     1e7)
+        while termination_mask.sum() > 0 and (t + prefix_t) < max_length:
+            curr_token = tokens[:, t - 1].unsqueeze(1)
+            curr_dialogue_kvs = map_all_kvs(
+                lambda x: x[:, :, : (t + prefix_t) - 1, :], dialogue_kvs
+            )
+            logits, past_key_values = self.bc_lm(
+                curr_token, None, past_key_values=curr_dialogue_kvs, is_causal=False
+            )
+            logits[:, 0, tokenizer.pad_token_id] = torch.where(
+                termination_mask == 1, float("-inf"), 1e7
+            )
+            logits[
+                torch.arange(0, n).to(device),
+                torch.full((n,), 0).to(device),
+                tokens[:, t],
+            ] = logits[
+                torch.arange(0, n).to(device),
+                torch.full((n,), 0).to(device),
+                tokens[:, t],
+            ].masked_fill_(
+                t < dialogue_lens, 1e7
+            )
             logits = process_logits(logits, temp=temp, top_k=top_k, top_p=top_p)
             cat_dist = torch.distributions.categorical.Categorical(logits=logits[:, 0])
             new_tokens = cat_dist.sample()
             log_probs += cat_dist.log_prob(new_tokens)
             tokens[:, t] = new_tokens
-            dialogue_kvs = update_kvs(dialogue_kvs, past_key_values, 
-                                      torch.arange(0, n).to(device), (t+prefix_t)-1)
+            dialogue_kvs = update_kvs(
+                dialogue_kvs,
+                past_key_values,
+                torch.arange(0, n).to(device),
+                (t + prefix_t) - 1,
+            )
             for idx in range(n):
                 if tokens[idx, t] == tokenizer.eoa_token_id and t >= dialogue_lens[idx]:
-                    termination_mask[idx] *= (1 - int(termination_condition(
-                        tokenizer.decode(tokens[idx, :].tolist(), 
-                                         clean_up_tokenization_spaces=False))))
+                    termination_mask[idx] *= 1 - int(
+                        termination_condition(
+                            tokenizer.decode(
+                                tokens[idx, :].tolist(),
+                                clean_up_tokenization_spaces=False,
+                            )
+                        )
+                    )
             t += 1
-            termination_mask *= ((t-dialogue_lens) < max_generation_len).int()
-    
-        output_strs = [tokenizer.decode(
-            tokens[i, :].tolist(),
-            clean_up_tokenization_spaces=False) for i in range(len(tokens))]
+            termination_mask *= ((t - dialogue_lens) < max_generation_len).int()
+
+        output_strs = [
+            tokenizer.decode(tokens[i, :].tolist(), clean_up_tokenization_spaces=False)
+            for i in range(len(tokens))
+        ]
         processed_outputs = []
         for i in range(len(input_strs)):
             temp_outputs = []
             for x in range(num_generations):
-                processed_str = output_strs[i*num_generations+x][len(
-                    input_strs[i]):].strip()
+                processed_str = output_strs[i * num_generations + x][
+                    len(input_strs[i]) :
+                ].strip()
                 if tokenizer.id_to_token(tokenizer.pad_token_id) in processed_str:
-                    processed_str = processed_str[:processed_str.find(
-                        tokenizer.id_to_token(tokenizer.pad_token_id))].strip()
+                    processed_str = processed_str[
+                        : processed_str.find(
+                            tokenizer.id_to_token(tokenizer.pad_token_id)
+                        )
+                    ].strip()
                 if tokenizer.id_to_token(tokenizer.eoa_token_id) in processed_str:
-                    processed_str = processed_str[:processed_str.find(
-                        tokenizer.id_to_token(tokenizer.eoa_token_id))].strip()
+                    processed_str = processed_str[
+                        : processed_str.find(
+                            tokenizer.id_to_token(tokenizer.eoa_token_id)
+                        )
+                    ].strip()
                 temp_outputs.append(processed_str)
             processed_outputs.append(temp_outputs)
-        return list(zip(input_strs, processed_outputs)), log_probs.reshape(-1, 
-                                                                           num_generations)
-    
-    def beam_raw(self, 
-                 tokens: torch.Tensor, attn_mask: torch.Tensor, 
-                 termination_condition: Callable[[np.ndarray], bool], 
-                 beam_width=1, max_generation_len=None, 
-                 prefix_embs: Optional[torch.Tensor]=None, 
-                 prefix_attn_mask: Optional[torch.Tensor]=None, 
-                 remove_prefix_position_embs: bool=False):
+        return list(zip(input_strs, processed_outputs)), log_probs.reshape(
+            -1, num_generations
+        )
+
+    def beam_raw(
+        self,
+        tokens: torch.Tensor,
+        attn_mask: torch.Tensor,
+        termination_condition: Callable[[np.ndarray], bool],
+        beam_width=1,
+        max_generation_len=None,
+        prefix_embs: Optional[torch.Tensor] = None,
+        prefix_attn_mask: Optional[torch.Tensor] = None,
+        remove_prefix_position_embs: bool = False,
+    ):
         tokenizer = self.bc_lm.dataset.tokenizer
         max_length = self.bc_lm.dataset.max_len
         if max_length is None:
             max_length = self.bc_lm.model.block_size
         max_length = min(max_length, self.bc_lm.model.block_size)
         device = self.bc_lm.device
         bsize, vocab_size = tokens.shape[0], tokenizer.num_tokens()
         n = bsize * beam_width
         if max_generation_len is None:
-            max_generation_len = max_length+1
-        input_strs = [tokenizer.decode(
-            tokens[i, :][:attn_mask[i, :].sum().long()].tolist(), 
-            clean_up_tokenization_spaces=False) for i in range(len(tokens))]
+            max_generation_len = max_length + 1
+        input_strs = [
+            tokenizer.decode(
+                tokens[i, :][: attn_mask[i, :].sum().long()].tolist(),
+                clean_up_tokenization_spaces=False,
+            )
+            for i in range(len(tokens))
+        ]
         prefix_t = 0 if prefix_embs is None else prefix_embs.shape[1]
-        logits, past_key_values = self.bc_lm(tokens, attn_mask, 
-                                             prefix_embs=prefix_embs, 
-                                   prefix_attn_mask=prefix_attn_mask, 
-                                   remove_prefix_position_embs=remove_prefix_position_embs,
-                                   is_causal=False)
+        logits, past_key_values = self.bc_lm(
+            tokens,
+            attn_mask,
+            prefix_embs=prefix_embs,
+            prefix_attn_mask=prefix_attn_mask,
+            remove_prefix_position_embs=remove_prefix_position_embs,
+            is_causal=False,
+        )
         dialogue_kvs = past_key_values
         original_dialogue_lens = attn_mask.sum(dim=1)
-        batch_indicator = torch.stack(beam_width*[torch.arange(0, bsize).to(device)], 
-                                      dim=1)
-        tokens = pad_sequence(torch.repeat_interleave(tokens, beam_width, dim=0), 
-                              max_length, tokenizer.pad_token_id, device, 1)
-        dialogue_lens = torch.repeat_interleave(original_dialogue_lens, beam_width, 
-                                                dim=0)
+        batch_indicator = torch.stack(
+            beam_width * [torch.arange(0, bsize).to(device)], dim=1
+        )
+        tokens = pad_sequence(
+            torch.repeat_interleave(tokens, beam_width, dim=0),
+            max_length,
+            tokenizer.pad_token_id,
+            device,
+            1,
+        )
+        dialogue_lens = torch.repeat_interleave(
+            original_dialogue_lens, beam_width, dim=0
+        )
         dialogue_kvs = map_all_kvs(
             lambda x: pad_sequence(
-            torch.repeat_interleave(x, beam_width, dim=0), max_length, 
-            0.0, device, 2), dialogue_kvs)
+                torch.repeat_interleave(x, beam_width, dim=0),
+                max_length,
+                0.0,
+                device,
+                2,
+            ),
+            dialogue_kvs,
+        )
         curr_scores = torch.zeros(bsize, beam_width).to(device)  # (batch, k)
         termination_mask = torch.full((n,), 1).to(device)
         t = torch.min(dialogue_lens).int()
-        while termination_mask.sum() > 0 and (t+prefix_t) < max_length:
-            curr_token = tokens[:, t-1].unsqueeze(1)
-            curr_dialogue_kvs = map_all_kvs(lambda x: x[:,:,:(t+prefix_t)-1,:], 
-                                            dialogue_kvs)
+        while termination_mask.sum() > 0 and (t + prefix_t) < max_length:
+            curr_token = tokens[:, t - 1].unsqueeze(1)
+            curr_dialogue_kvs = map_all_kvs(
+                lambda x: x[:, :, : (t + prefix_t) - 1, :], dialogue_kvs
+            )
             logits, past_key_values = self.bc_lm(
-                curr_token, None, past_key_values=curr_dialogue_kvs, is_causal=False)
-            logits[:, 0, tokenizer.pad_token_id] = torch.where(termination_mask == 1, 
-                                                               float('-inf'), 1e7)
-            logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(device), 
-                   tokens[:, t]] = logits[torch.arange(0, n).to(device), 
-                                          torch.full((n,), 0).to(
-                device), tokens[:, t]].masked_fill_(t < dialogue_lens, 1e7)
-            scores = (torch.log(F.softmax(logits, dim=-1)).reshape(
-                1, bsize, beam_width, -1).permute(
-                3, 0, 1, 2) + curr_scores).permute(1, 2, 3, 0).reshape(
-                1, bsize, -1)  # (time, batch, k*vocab)
+                curr_token, None, past_key_values=curr_dialogue_kvs, is_causal=False
+            )
+            logits[:, 0, tokenizer.pad_token_id] = torch.where(
+                termination_mask == 1, float("-inf"), 1e7
+            )
+            logits[
+                torch.arange(0, n).to(device),
+                torch.full((n,), 0).to(device),
+                tokens[:, t],
+            ] = logits[
+                torch.arange(0, n).to(device),
+                torch.full((n,), 0).to(device),
+                tokens[:, t],
+            ].masked_fill_(
+                t < dialogue_lens, 1e7
+            )
+            scores = (
+                (
+                    torch.log(F.softmax(logits, dim=-1))
+                    .reshape(1, bsize, beam_width, -1)
+                    .permute(3, 0, 1, 2)
+                    + curr_scores
+                )
+                .permute(1, 2, 3, 0)
+                .reshape(1, bsize, -1)
+            )  # (time, batch, k*vocab)
             scores[0, :, vocab_size:] = scores[0, :, vocab_size:].masked_fill_(
-                (t == original_dialogue_lens).unsqueeze(1).repeat(
-                1, scores.shape[2]-vocab_size), float('-inf'))
+                (t == original_dialogue_lens)
+                .unsqueeze(1)
+                .repeat(1, scores.shape[2] - vocab_size),
+                float("-inf"),
+            )
             curr_scores, top_k = torch.topk(
-                scores[0, :, :], k=beam_width, dim=1)  # (batch, k), (batch, k)
-            tokens = tokens[(
-                batch_indicator * beam_width + (top_k // vocab_size)).reshape(-1), :]
+                scores[0, :, :], k=beam_width, dim=1
+            )  # (batch, k), (batch, k)
+            tokens = tokens[
+                (batch_indicator * beam_width + (top_k // vocab_size)).reshape(-1), :
+            ]
             tokens[:, t] = top_k.reshape(-1) % vocab_size  # (batch*k,)
             fixed_dialogue_kvs = map_all_kvs(
-                lambda x: x[(
-                batch_indicator * beam_width + (top_k // vocab_size)).reshape(
-                -1), :, :, :], past_key_values)
-            dialogue_kvs = map_all_kvs(lambda x: x[(batch_indicator * beam_width + (
-                top_k // vocab_size)).reshape(-1), :, :, :], dialogue_kvs)
+                lambda x: x[
+                    (batch_indicator * beam_width + (top_k // vocab_size)).reshape(-1),
+                    :,
+                    :,
+                    :,
+                ],
+                past_key_values,
+            )
+            dialogue_kvs = map_all_kvs(
+                lambda x: x[
+                    (batch_indicator * beam_width + (top_k // vocab_size)).reshape(-1),
+                    :,
+                    :,
+                    :,
+                ],
+                dialogue_kvs,
+            )
             dialogue_kvs = update_kvs(
-                dialogue_kvs, fixed_dialogue_kvs, torch.arange(0, n).to(
-                device), (t+prefix_t)-1)
-            dialogue_lens = dialogue_lens[(
-                batch_indicator * beam_width + (top_k // vocab_size)).reshape(-1)]
-            termination_mask = termination_mask[(
-                batch_indicator * beam_width + (top_k // vocab_size)).reshape(-1)]
+                dialogue_kvs,
+                fixed_dialogue_kvs,
+                torch.arange(0, n).to(device),
+                (t + prefix_t) - 1,
+            )
+            dialogue_lens = dialogue_lens[
+                (batch_indicator * beam_width + (top_k // vocab_size)).reshape(-1)
+            ]
+            termination_mask = termination_mask[
+                (batch_indicator * beam_width + (top_k // vocab_size)).reshape(-1)
+            ]
             for idx in range(n):
                 if tokens[idx, t] == tokenizer.eoa_token_id and t >= dialogue_lens[idx]:
-                    termination_mask[idx] *= (1 - int(termination_condition(
-                        tokenizer.decode(tokens[idx, :].tolist(), 
-                                         clean_up_tokenization_spaces=False))))
+                    termination_mask[idx] *= 1 - int(
+                        termination_condition(
+                            tokenizer.decode(
+                                tokens[idx, :].tolist(),
+                                clean_up_tokenization_spaces=False,
+                            )
+                        )
+                    )
             t += 1
-            termination_mask *= ((t-dialogue_lens) < max_generation_len).int()
-        output_strs = [tokenizer.decode(tokens[i, :].tolist(),
-                                 clean_up_tokenization_spaces=False) for i in range(n)]
+            termination_mask *= ((t - dialogue_lens) < max_generation_len).int()
+        output_strs = [
+            tokenizer.decode(tokens[i, :].tolist(), clean_up_tokenization_spaces=False)
+            for i in range(n)
+        ]
         processed_outputs = []
         for i in range(len(input_strs)):
             temp_outputs = []
             for x in range(beam_width):
-                processed_str = output_strs[i*beam_width+x][len(input_strs[i]):].strip()
+                processed_str = output_strs[i * beam_width + x][
+                    len(input_strs[i]) :
+                ].strip()
                 if tokenizer.id_to_token(tokenizer.pad_token_id) in processed_str:
-                    processed_str = processed_str[:processed_str.find(
-                        tokenizer.id_to_token(tokenizer.pad_token_id))].strip()
+                    processed_str = processed_str[
+                        : processed_str.find(
+                            tokenizer.id_to_token(tokenizer.pad_token_id)
+                        )
+                    ].strip()
                 if tokenizer.id_to_token(tokenizer.eoa_token_id) in processed_str:
-                    processed_str = processed_str[:processed_str.find(
-                        tokenizer.id_to_token(tokenizer.eoa_token_id))].strip()
+                    processed_str = processed_str[
+                        : processed_str.find(
+                            tokenizer.id_to_token(tokenizer.eoa_token_id)
+                        )
+                    ].strip()
                 temp_outputs.append(processed_str)
             processed_outputs.append(temp_outputs)
         return list(zip(input_strs, processed_outputs)), curr_scores
-    
-    def generate(self, items, 
-                 termination_condition: Callable[[np.ndarray], bool], **kwargs):
+
+    def generate(
+        self, items, termination_condition: Callable[[np.ndarray], bool], **kwargs
+    ):
         prepared_inputs = self.bc_lm.prepare_inputs(items)
-        tokens, attn_mask = prepared_inputs['tokens'], prepared_inputs['attn_mask']
-        if self.kind == 'beam':
+        tokens, attn_mask = prepared_inputs["tokens"], prepared_inputs["attn_mask"]
+        if self.kind == "beam":
             method = self.beam_raw
-        elif self.kind == 'sample':
+        elif self.kind == "sample":
             method = self.sample_raw
         else:
             raise NotImplementedError
-        generations, probs = method(tokens, attn_mask, 
-                                    termination_condition, 
-                                    **kwargs)
+        generations, probs = method(tokens, attn_mask, termination_condition, **kwargs)
         return generations, probs
-    
+
     def act(self, obs: Language_Observation) -> str:
-        item = DataPoint.from_obs(obs, 
-                                  self.bc_lm.dataset.tokenizer, 
-                                  self.bc_lm.dataset.token_reward)
-        generations, probs = self.generate([item], always_terminate, 
-                                           **self.generation_kwargs)
-        sorted_outputs = list(zip(*sorted(zip(
-            generations[0][1], probs[0]), key=lambda x: -x[1])))[0]
+        item = DataPoint.from_obs(
+            obs, self.bc_lm.dataset.tokenizer, self.bc_lm.dataset.token_reward
+        )
+        generations, probs = self.generate(
+            [item], always_terminate, **self.generation_kwargs
+        )
+        sorted_outputs = list(
+            zip(*sorted(zip(generations[0][1], probs[0]), key=lambda x: -x[1]))
+        )[0]
         return sorted_outputs[0]
-    
+
     def train(self):
         self.bc_lm.train()
-    
+
     def eval(self):
         self.bc_lm.eval()
 
-class BC_Evaluator():
+
+class BC_Evaluator:
     def __init__(self, env, verbose: bool, kind: str, **generation_kwargs) -> None:
         super().__init__()
         self.env = env
         self.verbose = verbose
         self.kind = kind
         self.generation_kwargs = generation_kwargs
-    
+
     def evaluate(self, model: BC_LM, items):
         policy = BC_Policy(model, self.kind, **self.generation_kwargs)
-        tokens = model.prepare_inputs(items)['tokens']
+        tokens = model.prepare_inputs(items)["tokens"]
         n = tokens.shape[0]
         total_token_reward = 0
         total_env_reward = 0
         for i in range(n):
             result, sequence = interact_environment(self.env, policy, None)
             env_reward = sum(map(lambda x: x[2], sequence))
-            token_reward = sum(DataPoint.get_token_reward(result, 
-                                                          model.dataset.tokenizer, 
-                                                          model.dataset.token_reward))
+            token_reward = sum(
+                DataPoint.get_token_reward(
+                    result, model.dataset.tokenizer, model.dataset.token_reward
+                )
+            )
             total_env_reward += env_reward
             total_token_reward += token_reward
             if self.verbose:
                 print(result)
-                print('='*25)
-                print('token reward:', token_reward)
-                print('env reward:', env_reward)
-                print('avg token reward:', total_token_reward / (i + 1))
-                print('avg env reward:', total_env_reward / (i + 1))
-                print('='*25)
-        return {'token_reward':(total_token_reward/n,n),
-                'env_reward':(total_env_reward/n,n)}
+                print("=" * 25)
+                print("token reward:", token_reward)
+                print("env reward:", env_reward)
+                print("avg token reward:", total_token_reward / (i + 1))
+                print("avg env reward:", total_env_reward / (i + 1))
+                print("=" * 25)
+        return {
+            "token_reward": (total_token_reward / n, n),
+            "env_reward": (total_env_reward / n, n),
+        }
+
 
 def to(item: Any, device: torch.device):
     return map_pytree(lambda x: torch.tensor(x).to(device), item)
 
-def map_pytree(f: Callable[[Union[np.ndarray, torch.Tensor]], Any],
-               item: Any):
+
+def map_pytree(f: Callable[[Union[np.ndarray, torch.Tensor]], Any], item: Any):
     if isinstance(item, dict):
         return {k: map_pytree(f, v) for k, v in item.items()}
     elif isinstance(item, list) or isinstance(item, set) or isinstance(item, tuple):
         return [map_pytree(f, v) for v in item]
     elif isinstance(item, np.ndarray) or isinstance(item, torch.Tensor):
         return f(item)
     else:
-        return item
+        return item
```

### Comparing `agilerl-0.1.8/agilerl/algorithms/cqn.py` & `agilerl-0.1.9/agilerl/algorithms/cqn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-import random
 import copy
+import random
+
 import dill
 import numpy as np
 import torch
 import torch.nn as nn
-from torch.nn.utils import clip_grad_norm_
 import torch.optim as optim
-from agilerl.networks.evolvable_mlp import EvolvableMLP
+from torch.nn.utils import clip_grad_norm_
+
 from agilerl.networks.evolvable_cnn import EvolvableCNN
+from agilerl.networks.evolvable_mlp import EvolvableMLP
 
 
-class CQN():
+class CQN:
     """The CQN algorithm class. CQN paper: https://arxiv.org/abs/2006.04779
 
     :param state_dim: State observation dimension
     :type state_dim: int
     :param action_dim: Action dimension
     :type action_dim: int
     :param one_hot: One-hot encoding, used with discrete observation spaces
@@ -41,19 +43,33 @@
     :type device: str, optional
     :param accelerator: Accelerator for distributed computing, defaults to None
     :type accelerator: Hugging Face accelerate.Accelerator(), optional
     :param wrap: Wrap models for distributed training upon creation, defaults to True
     :type wrap: bool, optional
     """
 
-    def __init__(self, state_dim, action_dim, one_hot, index=0, 
-                 net_config={'arch': 'mlp', 'h_size':[64, 64]}, batch_size=64, lr=1e-4,
-                 learn_step=5, gamma=0.99, tau=1e-3, mutation=None, double=False,
-                 device='cpu', accelerator=None, wrap=True):
-        self.algo = 'CQN'
+    def __init__(
+        self,
+        state_dim,
+        action_dim,
+        one_hot,
+        index=0,
+        net_config={"arch": "mlp", "h_size": [64, 64]},
+        batch_size=64,
+        lr=1e-4,
+        learn_step=5,
+        gamma=0.99,
+        tau=1e-3,
+        mutation=None,
+        double=False,
+        device="cpu",
+        accelerator=None,
+        wrap=True,
+    ):
+        self.algo = "CQN"
         self.state_dim = state_dim
         self.action_dim = action_dim
         self.one_hot = one_hot
         self.net_config = net_config
         self.batch_size = batch_size
         self.lr = lr
         self.learn_step = learn_step
@@ -67,50 +83,54 @@
         self.scores = []
         self.fitness = []
         self.steps = [0]
 
         self.double = double
 
         # model
-        if self.net_config['arch'] == 'mlp':      # Multi-layer Perceptron
+        if self.net_config["arch"] == "mlp":  # Multi-layer Perceptron
             self.actor = EvolvableMLP(
                 num_inputs=state_dim[0],
                 num_outputs=action_dim,
-                hidden_size=self.net_config['h_size'],
+                hidden_size=self.net_config["h_size"],
                 device=self.device,
-                accelerator=self.accelerator)
+                accelerator=self.accelerator,
+            )
             self.actor_target = EvolvableMLP(
                 num_inputs=state_dim[0],
                 num_outputs=action_dim,
-                hidden_size=self.net_config['h_size'],
+                hidden_size=self.net_config["h_size"],
                 device=self.device,
-                accelerator=self.accelerator)
+                accelerator=self.accelerator,
+            )
             self.actor_target.load_state_dict(self.actor.state_dict())
 
-        elif self.net_config['arch'] == 'cnn':    # Convolutional Neural Network
+        elif self.net_config["arch"] == "cnn":  # Convolutional Neural Network
             self.actor = EvolvableCNN(
                 input_shape=state_dim,
                 num_actions=action_dim,
-                channel_size=self.net_config['c_size'],
-                kernal_size=self.net_config['k_size'],
-                stride_size=self.net_config['s_size'],
-                hidden_size=self.net_config['h_size'],
-                normalize=self.net_config['normalize'],
+                channel_size=self.net_config["c_size"],
+                kernal_size=self.net_config["k_size"],
+                stride_size=self.net_config["s_size"],
+                hidden_size=self.net_config["h_size"],
+                normalize=self.net_config["normalize"],
                 device=self.device,
-                accelerator=self.accelerator)
+                accelerator=self.accelerator,
+            )
             self.actor_target = EvolvableCNN(
                 input_shape=state_dim,
                 num_actions=action_dim,
-                channel_size=self.net_config['c_size'],
-                kernal_size=self.net_config['k_size'],
-                stride_size=self.net_config['s_size'],
-                hidden_size=self.net_config['h_size'],
-                normalize=self.net_config['normalize'],
+                channel_size=self.net_config["c_size"],
+                kernal_size=self.net_config["k_size"],
+                stride_size=self.net_config["s_size"],
+                hidden_size=self.net_config["h_size"],
+                normalize=self.net_config["normalize"],
                 device=self.device,
-                accelerator=self.accelerator)
+                accelerator=self.accelerator,
+            )
             self.actor_target.load_state_dict(self.actor.state_dict())
 
         self.optimizer_type = optim.Adam(self.actor.parameters(), lr=self.lr)
 
         if self.accelerator is not None:
             self.optimizer = self.optimizer_type
             if wrap:
@@ -119,48 +139,51 @@
             self.actor = self.actor.to(self.device)
             self.actor_target = self.actor_target.to(self.device)
             self.optimizer = self.optimizer_type
 
         self.criterion = nn.MSELoss()
 
     def getAction(self, state, epsilon=0):
-        """Returns the next action to take in the environment. Epsilon is the 
+        """Returns the next action to take in the environment. Epsilon is the
         probability of taking a random action, used for exploration.
         For epsilon-greedy behaviour, set epsilon to 0.
 
         :param state: State observation, or multiple observations in a batch
         :type state: float or List[float]
         :param epsilon: Probablilty of taking a random action for exploration, defaults to 0
         :type epsilon: float, optional
         """
         state = torch.from_numpy(state).float()
         if self.accelerator is None:
             state = state.to(self.device)
 
         if self.one_hot:
-            state = nn.functional.one_hot(
-                state.long(), num_classes=self.state_dim[0]).float().squeeze()
+            state = (
+                nn.functional.one_hot(state.long(), num_classes=self.state_dim[0])
+                .float()
+                .squeeze()
+            )
 
         if len(state.size()) < 2:
             state = state.unsqueeze(0)
 
         # epsilon-greedy
         if random.random() < epsilon:
             action = np.random.randint(0, self.action_dim, size=state.size()[0])
         else:
             self.actor.eval()
             with torch.no_grad():
                 action_values = self.actor(state)
             self.actor.train()
             action = np.argmax(action_values.cpu().data.numpy(), axis=1)
         return action
-    
+
     def _squeeze_exp(self, experiences):
         """Remove first dim created by dataloader.
-        
+
         :param experiences: List of batched states, actions, rewards, next_states, dones in that order.
         :type state: List[torch.Tensor[float]]
         """
         st, ac, re, ne, do = experiences
         return st.squeeze(0), ac.squeeze(0), re.squeeze(0), ne.squeeze(0), do.squeeze(0)
 
     def learn(self, experiences):
@@ -168,24 +191,32 @@
 
         :param experiences: List of batched states, actions, rewards, next_states, dones in that order.
         :type state: List[torch.Tensor[float]]
         """
         states, actions, rewards, next_states, dones = experiences
 
         if self.one_hot:
-            states = nn.functional.one_hot(
-                states.long(), num_classes=self.state_dim[0]).float().squeeze()
-            next_states = nn.functional.one_hot(
-                next_states.long(), num_classes=self.state_dim[0]).float().squeeze()
+            states = (
+                nn.functional.one_hot(states.long(), num_classes=self.state_dim[0])
+                .float()
+                .squeeze()
+            )
+            next_states = (
+                nn.functional.one_hot(next_states.long(), num_classes=self.state_dim[0])
+                .float()
+                .squeeze()
+            )
 
-        if self.double: # Double Q-learning
+        if self.double:  # Double Q-learning
             q_idx = self.actor_target(next_states).argmax(dim=1).unsqueeze(1)
             q_target_next = self.actor(next_states).gather(dim=1, index=q_idx).detach()
         else:
-            q_target_next = self.actor_target(next_states).detach().max(axis=1)[0].unsqueeze(1)
+            q_target_next = (
+                self.actor_target(next_states).detach().max(axis=1)[0].unsqueeze(1)
+            )
 
         # target, if terminal then y_j = rewards
         q_target = rewards + self.gamma * q_target_next * (1 - dones)
         q_a_s = self.actor(states)
         q_eval = q_a_s.gather(1, actions.long())
 
         # loss backprop
@@ -200,20 +231,21 @@
         clip_grad_norm_(self.actor.parameters(), 1)
         self.optimizer.step()
 
         # soft update target network
         self.softUpdate()
 
     def softUpdate(self):
-        """Soft updates target network.
-        """
+        """Soft updates target network."""
         for eval_param, target_param in zip(
-                self.actor.parameters(), self.actor_target.parameters()):
+            self.actor.parameters(), self.actor_target.parameters()
+        ):
             target_param.data.copy_(
-                self.tau * eval_param.data + (1.0 - self.tau) * target_param.data)
+                self.tau * eval_param.data + (1.0 - self.tau) * target_param.data
+            )
 
     def test(self, env, swap_channels=False, max_steps=500, loop=3):
         """Returns mean test score of agent in environment with epsilon-greedy policy.
 
         :param env: The environment to be tested in
         :type env: Gym-style environment
         :param swap_channels: Swap image channels dimension from last to first [H, W, C] -> [C, H, W], defaults to False
@@ -246,109 +278,120 @@
 
         :param index: Index to keep track of agent for tournament selection and mutation, defaults to None
         :type index: int, optional
         """
         if index is None:
             index = self.index
 
-        clone = type(self)(state_dim=self.state_dim,
-                           action_dim=self.action_dim,
-                           one_hot=self.one_hot,
-                           index=index,
-                           net_config=self.net_config,
-                           batch_size=self.batch_size,
-                           lr=self.lr,
-                           learn_step=self.learn_step,
-                           gamma=self.gamma,
-                           tau=self.tau,
-                           mutation=self.mut,
-                           device=self.device,
-                           accelerator=self.accelerator,
-                           wrap=wrap)
+        clone = type(self)(
+            state_dim=self.state_dim,
+            action_dim=self.action_dim,
+            one_hot=self.one_hot,
+            index=index,
+            net_config=self.net_config,
+            batch_size=self.batch_size,
+            lr=self.lr,
+            learn_step=self.learn_step,
+            gamma=self.gamma,
+            tau=self.tau,
+            mutation=self.mut,
+            device=self.device,
+            accelerator=self.accelerator,
+            wrap=wrap,
+        )
 
         actor = self.actor.clone()
         actor_target = self.actor_target.clone()
         optimizer = optim.Adam(actor.parameters(), lr=clone.lr)
         clone.optimizer_type = optimizer
         if self.accelerator is not None:
             if wrap:
-                clone.actor, clone.actor_target, clone.optimizer = self.accelerator.prepare(
-                                                                                        actor, 
-                                                                                        actor_target,
-                                                                                        optimizer)
+                (
+                    clone.actor,
+                    clone.actor_target,
+                    clone.optimizer,
+                ) = self.accelerator.prepare(actor, actor_target, optimizer)
             else:
-                clone.actor, clone.actor_target, clone.optimizer = actor, actor_target, optimizer
+                clone.actor, clone.actor_target, clone.optimizer = (
+                    actor,
+                    actor_target,
+                    optimizer,
+                )
         else:
             clone.actor = actor.to(self.device)
             clone.actor_target = actor_target.to(self.device)
             clone.optimizer = optimizer
         clone.fitness = copy.deepcopy(self.fitness)
         clone.steps = copy.deepcopy(self.steps)
         clone.scores = copy.deepcopy(self.scores)
 
         return clone
-    
+
     def wrap_models(self):
         if self.accelerator is not None:
-            self.actor, self.actor_target, self.optimizer = self.accelerator.prepare(self.actor, 
-                                                                            self.actor_target, 
-                                                                            self.optimizer)
-    
+            self.actor, self.actor_target, self.optimizer = self.accelerator.prepare(
+                self.actor, self.actor_target, self.optimizer
+            )
+
     def unwrap_models(self):
         if self.accelerator is not None:
             self.actor = self.accelerator.unwrap_model(self.actor)
             self.actor_target = self.accelerator.unwrap_model(self.actor_target)
             self.optimizer = self.accelerator.unwrap_model(self.optimizer)
 
     def saveCheckpoint(self, path):
         """Saves a checkpoint of agent properties and network weights to path.
 
         :param path: Location to save checkpoint at
         :type path: string
         """
-        torch.save({
-            'actor_init_dict': self.actor.init_dict,
-            'actor_state_dict': self.actor.state_dict(),
-            'actor_target_init_dict': self.actor_target.init_dict,
-            'actor_target_state_dict': self.actor_target.state_dict(),
-            'optimizer_state_dict': self.optimizer.state_dict(),
-            'net_config': self.net_config,
-            'batch_size': self.batch_size,
-            'lr': self.lr,
-            'learn_step': self.learn_step,
-            'gamma': self.gamma,
-            'tau': self.tau,
-            'mutation': self.mut,
-            'index': self.index,
-            'scores': self.scores,
-            'fitness': self.fitness,
-            'steps': self.steps,
-        }, path, pickle_module=dill)
+        torch.save(
+            {
+                "actor_init_dict": self.actor.init_dict,
+                "actor_state_dict": self.actor.state_dict(),
+                "actor_target_init_dict": self.actor_target.init_dict,
+                "actor_target_state_dict": self.actor_target.state_dict(),
+                "optimizer_state_dict": self.optimizer.state_dict(),
+                "net_config": self.net_config,
+                "batch_size": self.batch_size,
+                "lr": self.lr,
+                "learn_step": self.learn_step,
+                "gamma": self.gamma,
+                "tau": self.tau,
+                "mutation": self.mut,
+                "index": self.index,
+                "scores": self.scores,
+                "fitness": self.fitness,
+                "steps": self.steps,
+            },
+            path,
+            pickle_module=dill,
+        )
 
     def loadCheckpoint(self, path):
         """Loads saved agent properties and network weights from checkpoint.
 
         :param path: Location to load checkpoint from
         :type path: string
         """
         checkpoint = torch.load(path, pickle_module=dill)
-        self.net_config = checkpoint['net_config']
-        if self.net_config['arch'] == 'mlp':
-            self.actor = EvolvableMLP(**checkpoint['actor_init_dict'])
-            self.actor_target = EvolvableMLP(**checkpoint['actor_target_init_dict'])
-        elif self.net_config['arch'] == 'cnn':
-            self.actor = EvolvableCNN(**checkpoint['actor_init_dict'])
-            self.actor_target = EvolvableCNN(**checkpoint['actor_target_init_dict'])
-        self.lr = checkpoint['lr']
+        self.net_config = checkpoint["net_config"]
+        if self.net_config["arch"] == "mlp":
+            self.actor = EvolvableMLP(**checkpoint["actor_init_dict"])
+            self.actor_target = EvolvableMLP(**checkpoint["actor_target_init_dict"])
+        elif self.net_config["arch"] == "cnn":
+            self.actor = EvolvableCNN(**checkpoint["actor_init_dict"])
+            self.actor_target = EvolvableCNN(**checkpoint["actor_target_init_dict"])
+        self.lr = checkpoint["lr"]
         self.optimizer = optim.Adam(self.actor.parameters(), lr=self.lr)
-        self.actor.load_state_dict(checkpoint['actor_state_dict'])
-        self.actor_target.load_state_dict(checkpoint['actor_target_state_dict'])
-        self.optimizer.load_state_dict(checkpoint['optimizer_state_dict'])
-        self.batch_size = checkpoint['batch_size']
-        self.learn_step = checkpoint['learn_step']
-        self.gamma = checkpoint['gamma']
-        self.tau = checkpoint['tau']
-        self.mut = checkpoint['mutation']
-        self.index = checkpoint['index']
-        self.scores = checkpoint['scores']
-        self.fitness = checkpoint['fitness']
-        self.steps = checkpoint['steps']
+        self.actor.load_state_dict(checkpoint["actor_state_dict"])
+        self.actor_target.load_state_dict(checkpoint["actor_target_state_dict"])
+        self.optimizer.load_state_dict(checkpoint["optimizer_state_dict"])
+        self.batch_size = checkpoint["batch_size"]
+        self.learn_step = checkpoint["learn_step"]
+        self.gamma = checkpoint["gamma"]
+        self.tau = checkpoint["tau"]
+        self.mut = checkpoint["mutation"]
+        self.index = checkpoint["index"]
+        self.scores = checkpoint["scores"]
+        self.fitness = checkpoint["fitness"]
+        self.steps = checkpoint["steps"]
```

### Comparing `agilerl-0.1.8/agilerl/algorithms/ddpg.py` & `agilerl-0.1.9/agilerl/algorithms/ddpg.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,466 +1,532 @@
-import random
-import copy
-import dill
-import numpy as np
-import torch
-import torch.nn as nn
-import torch.optim as optim
-from agilerl.networks.evolvable_mlp import EvolvableMLP
-from agilerl.networks.evolvable_cnn import EvolvableCNN
-
-
-class DDPG():
-    """The DDPG algorithm class. DDPG paper: https://arxiv.org/abs/1509.02971
-
-    :param state_dim: State observation dimension
-    :type state_dim: int
-    :param action_dim: Action dimension
-    :type action_dim: int
-    :param one_hot: One-hot encoding, used with discrete observation spaces
-    :type one_hot: bool
-    :param index: Index to keep track of object instance during tournament selection and mutation, defaults to 0
-    :type index: int, optional
-    :param net_config: Network configuration, defaults to mlp with hidden size [64,64]
-    :type net_config: dict, optional
-    :param batch_size: Size of batched sample from replay buffer for learning, defaults to 64
-    :type batch_size: int, optional
-    :param lr: Learning rate for optimizer, defaults to 1e-4
-    :type lr: float, optional
-    :param learn_step: Learning frequency, defaults to 5
-    :type learn_step: int, optional
-    :param gamma: Discount factor, defaults to 0.99
-    :type gamma: float, optional
-    :param tau: For soft update of target network parameters, defaults to 1e-3
-    :type tau: float, optional
-    :param mutation: Most recent mutation to agent, defaults to None
-    :type mutation: str, optional
-    :param policy_freq: Frequency of target network updates compared to policy network, defaults to 2
-    :type policy_freq: int, optional
-    :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
-    :type device: str, optional
-    :param accelerator: Accelerator for distributed computing, defaults to None
-    :type accelerator: Hugging Face accelerate.Accelerator(), optional
-    :param wrap: Wrap models for distributed training upon creation, defaults to True
-    :type wrap: bool, optional
-    """
-
-    def __init__(self, state_dim, action_dim, one_hot, index=0, 
-                 net_config={'arch': 'mlp', 'h_size': [64,64]}, batch_size=64, lr=1e-4, 
-                 learn_step=5, gamma=0.99, tau=1e-3, mutation=None, policy_freq=2, 
-                 device='cpu', accelerator=None, wrap=True):
-        self.algo = 'DDPG'
-        self.state_dim = state_dim
-        self.action_dim = action_dim
-        self.one_hot = one_hot
-        self.net_config = net_config
-        self.batch_size = batch_size
-        self.lr = lr
-        self.learn_step = learn_step
-        self.gamma = gamma
-        self.tau = tau
-        self.mut = mutation
-        self.policy_freq = policy_freq
-        self.device = device
-        self.accelerator = accelerator
-
-        self.index = index
-        self.scores = []
-        self.fitness = []
-        self.steps = [0]
-
-        # model
-        if self.net_config['arch'] == 'mlp':      # Multi-layer Perceptron
-            self.actor = EvolvableMLP(
-                num_inputs=state_dim[0],
-                num_outputs=action_dim,
-                hidden_size=self.net_config['h_size'],
-                output_activation='tanh',
-                device=self.device,
-                accelerator=self.accelerator)
-            self.actor_target = EvolvableMLP(
-                num_inputs=state_dim[0],
-                num_outputs=action_dim,
-                hidden_size=self.net_config['h_size'],
-                output_activation='tanh',
-                device=self.device,
-                accelerator=self.accelerator)
-            self.actor_target.load_state_dict(self.actor.state_dict())
-
-            self.critic = EvolvableMLP(
-                num_inputs=state_dim[0] + action_dim,
-                num_outputs=1,
-                hidden_size=self.net_config['h_size'],
-                device=self.device,
-                accelerator=self.accelerator)
-            self.critic_target = EvolvableMLP(
-                num_inputs=state_dim[0] + action_dim,
-                num_outputs=1,
-                hidden_size=self.net_config['h_size'],
-                device=self.device,
-                accelerator=self.accelerator)
-            self.critic_target.load_state_dict(self.critic.state_dict())
-
-        elif self.net_config['arch'] == 'cnn':    # Convolutional Neural Network
-            self.actor = EvolvableCNN(
-                input_shape=state_dim,
-                num_actions=action_dim,
-                channel_size=self.net_config['c_size'],
-                kernal_size=self.net_config['k_size'],
-                stride_size=self.net_config['s_size'],
-                hidden_size=self.net_config['h_size'],
-                normalize=self.net_config['normalize'],
-                mlp_activation='tanh',
-                device=self.device,
-                accelerator=self.accelerator)
-            self.actor_target = EvolvableCNN(
-                input_shape=state_dim,
-                num_actions=action_dim,
-                channel_size=self.net_config['c_size'],
-                kernal_size=self.net_config['k_size'],
-                stride_size=self.net_config['s_size'],
-                hidden_size=self.net_config['h_size'],
-                normalize=self.net_config['normalize'],
-                mlp_activation='tanh',
-                device=self.device,
-                accelerator=self.accelerator)
-            self.actor_target.load_state_dict(self.actor.state_dict())
-
-            self.critic = EvolvableCNN(
-                input_shape=state_dim,
-                num_actions=action_dim,
-                channel_size=self.net_config['c_size'],
-                kernal_size=self.net_config['k_size'],
-                stride_size=self.net_config['s_size'],
-                hidden_size=self.net_config['h_size'],
-                normalize=self.net_config['normalize'],
-                mlp_activation='tanh',
-                critic=True,
-                device=self.device,
-                accelerator=self.accelerator)
-            self.critic_target = EvolvableCNN(
-                input_shape=state_dim,
-                num_actions=action_dim,
-                channel_size=self.net_config['c_size'],
-                kernal_size=self.net_config['k_size'],
-                stride_size=self.net_config['s_size'],
-                hidden_size=self.net_config['h_size'],
-                normalize=self.net_config['normalize'],
-                mlp_activation='tanh',
-                critic=True,
-                device=self.device,
-                accelerator=self.accelerator)
-            self.critic_target.load_state_dict(self.critic.state_dict())
-
-        self.actor_optimizer_type = optim.Adam(self.actor.parameters(), lr=self.lr)
-        self.critic_optimizer_type = optim.Adam(self.critic.parameters(), lr=self.lr)
-
-        if self.accelerator is not None:
-            self.actor_optimizer = self.actor_optimizer_type
-            self.critic_optimizer = self.critic_optimizer_type
-            if wrap:
-                self.wrap_models()          
-        else:
-            self.actor = self.actor.to(self.device)
-            self.actor_target = self.actor_target.to(self.device)
-            self.critic = self.critic.to(self.device)
-            self.critic_target = self.critic_target.to(self.device)
-            self.actor_optimizer = self.actor_optimizer_type
-            self.critic_optimizer = self.critic_optimizer_type
-
-        self.criterion = nn.MSELoss()
-
-    def getAction(self, state, epsilon=0):
-        """Returns the next action to take in the environment. 
-        Epsilon is the probability of taking a random action, used for exploration.
-        For epsilon-greedy behaviour, set epsilon to 0.
-
-        :param state: Environment observation, or multiple observations in a batch
-        :type state: float or List[float]
-        :param epsilon: Probablilty of taking a random action for exploration, defaults to 0
-        :type epsilon: float, optional
-        """
-        state = torch.from_numpy(state).float()
-        if self.accelerator is None:
-            state = state.to(self.device)
-
-        if self.one_hot:
-            state = nn.functional.one_hot(
-                state.long(), num_classes=self.state_dim[0]).float().squeeze()
-
-        if len(state.size()) < 2:
-            state = state.unsqueeze(0)       
-
-        # epsilon-greedy
-        if random.random() < epsilon:
-            action = (np.random.rand(
-                state.size()[0], self.action_dim).astype('float32') - 0.5) * 2
-        else:
-            self.actor.eval()
-            with torch.no_grad():
-                action_values = self.actor(state)
-            self.actor.train()
-
-            action = action_values.cpu().data.numpy()
-
-        return action
-    
-    def _squeeze_exp(self, experiences):
-        """Remove first dim created by dataloader.
-        
-        :param experiences: List of batched states, actions, rewards, next_states, dones in that order.
-        :type state: List[torch.Tensor[float]]
-        """
-        st, ac, re, ne, do = experiences
-        return st.squeeze(0), ac.squeeze(0), re.squeeze(0), ne.squeeze(0), do.squeeze(0)
-
-    def learn(self, experiences, noise_clip=0.5, policy_noise=0.2):
-        """Updates agent network parameters to learn from experiences.
-
-        :param experience: List of batched states, actions, rewards, next_states, dones in that order.
-        :type experience: List[torch.Tensor[float]]
-        :param noise_clip: Maximum noise limit to apply to actions, defaults to 0.5
-        :type noise_clip: float, optional
-        :param policy_noise: Standard deviation of noise applied to policy, defaults to 0.2
-        :type policy_noise: float, optional
-        """
-        states, actions, rewards, next_states, dones = experiences
-
-        if self.one_hot:
-            states = nn.functional.one_hot(
-                states.long(), num_classes=self.state_dim[0]).float().squeeze()
-            next_states = nn.functional.one_hot(
-                next_states.long(), num_classes=self.state_dim[0]).float().squeeze()
-
-        if self.net_config['arch'] == 'mlp':
-            input_combined = torch.cat([states, actions], 1)
-            q_value = self.critic(input_combined)
-        elif self.net_config['arch'] == 'cnn':
-            q_value = self.critic(states, actions)
-
-        next_actions = self.actor_target(next_states)
-        noise = actions.data.normal_(0, policy_noise)
-        noise = noise.clamp(-noise_clip, noise_clip)
-        next_actions = (next_actions + noise)
-
-        if self.net_config['arch'] == 'mlp':
-            next_input_combined = torch.cat([next_states, next_actions], 1)
-            q_value_next_state = self.critic_target(next_input_combined)
-        elif self.net_config['arch'] == 'cnn':
-            q_value_next_state = self.critic_target(next_states, next_actions)
-
-        y_j = rewards + ((1-dones)*self.gamma * q_value_next_state).detach()
-
-        critic_loss = self.criterion(q_value, y_j)
-
-        # critic loss backprop
-        self.critic_optimizer.zero_grad()
-        if self.accelerator is not None:
-            self.accelerator.backward(critic_loss)
-        else:
-            critic_loss.backward()
-        self.critic_optimizer.step()
-
-        # update actor and targets every policy_freq episodes
-        if len(self.scores) % self.policy_freq == 0:
-            if self.net_config['arch'] == 'mlp':
-                input_combined = torch.cat(
-                    [states, self.actor.forward(states)], 1)
-                actor_loss = -self.critic(input_combined).mean()
-            elif self.net_config['arch'] == 'cnn':
-                actor_loss = - \
-                    self.critic(states, self.actor.forward(states)).mean()
-
-            # actor loss backprop
-            self.actor_optimizer.zero_grad()
-            if self.accelerator is not None:
-                self.accelerator.backward(actor_loss)
-            else:
-                actor_loss.backward()
-            self.actor_optimizer.step()
-
-            self.softUpdate(self.actor, self.actor_target)
-            self.softUpdate(self.critic, self.critic_target)
-
-    def softUpdate(self, net, target):
-        """Soft updates target network.
-        """
-        for eval_param, target_param in zip(net.parameters(), target.parameters()):
-            target_param.data.copy_(
-                self.tau * eval_param.data + (1.0 - self.tau) * target_param.data)
-
-    def test(self, env, swap_channels=False, max_steps=500, loop=3):
-        """Returns mean test score of agent in environment with epsilon-greedy policy.
-
-        :param env: The environment to be tested in
-        :type env: Gym-style environment
-        :param swap_channels: Swap image channels dimension from last to first [H, W, C] -> [C, H, W], defaults to False
-        :type swap_channels: bool, optional
-        :param max_steps: Maximum number of testing steps, defaults to 500
-        :type max_steps: int, optional
-        :param loop: Number of testing loops/epsiodes to complete. The returned score is the mean. Defaults to 3
-        :type loop: int, optional
-        """
-        with torch.no_grad():
-            rewards = []
-            for i in range(loop):
-                state = env.reset()[0]
-                score = 0
-                for idx_step in range(max_steps):
-                    if swap_channels:
-                        state = np.moveaxis(state, [3], [1])
-                    action = self.getAction(state, epsilon=0)
-                    state, reward, done, trunc, info = env.step(action)
-                    score += reward
-                rewards.append(score)
-        mean_fit = np.mean(rewards)
-        self.fitness.append(mean_fit)
-        return mean_fit
-
-    def clone(self, index=None, wrap=True):
-        """Returns cloned agent identical to self.
-
-        :param index: Index to keep track of agent for tournament selection and mutation, defaults to None
-        :type index: int, optional
-        """
-        if index is None:
-            index = self.index
-
-        clone = type(self)(state_dim=self.state_dim,
-                           action_dim=self.action_dim,
-                           one_hot=self.one_hot,
-                           index=index,
-                           net_config=self.net_config,
-                           batch_size=self.batch_size,
-                           lr=self.lr,
-                           learn_step=self.learn_step,
-                           gamma=self.gamma,
-                           tau=self.tau,
-                           mutation=self.mut,
-                           policy_freq=self.policy_freq,
-                           device=self.device,
-                           accelerator=self.accelerator,
-                           wrap=wrap)
-        
-        if self.accelerator is not None:
-            self.unwrap_models()
-        actor = self.actor.clone()
-        actor_target = self.actor_target.clone()
-        critic = self.critic.clone()
-        critic_target = self.critic_target.clone()
-        actor_optimizer = optim.Adam(actor.parameters(), lr=clone.lr)
-        critic_optimizer = optim.Adam(critic.parameters(), lr=clone.lr)
-        clone.actor_optimizer_type = actor_optimizer
-        clone.critic_optimizer_type = critic_optimizer
-
-        if self.accelerator is not None:
-            if wrap:
-                clone.actor, clone.actor_target, clone.critic, clone.critic_target, \
-                clone.actor_optimizer, clone.critic_optimizer = self.accelerator.prepare(actor,
-                                                                                actor_target,
-                                                                                critic,
-                                                                                critic_target,
-                                                                                actor_optimizer,
-                                                                                critic_optimizer)
-            else:
-                clone.actor, clone.actor_target, clone.critic, clone.critic_target, \
-                clone.actor_optimizer, clone.critic_optimizer = actor, actor_target, critic, \
-                critic_target, actor_optimizer, critic_optimizer
-        else:
-            clone.actor = actor.to(self.device)
-            clone.actor_target = actor_target.to(self.device)
-            clone.critic = critic.to(self.device)
-            clone.critic_target = critic_target.to(self.device)
-            clone.actor_optimizer = actor_optimizer
-            clone.critic_optimizer = critic_optimizer
-
-        clone.fitness = copy.deepcopy(self.fitness)
-        clone.steps = copy.deepcopy(self.steps)
-        clone.scores = copy.deepcopy(self.scores)
-
-        return clone
-
-    def wrap_models(self):
-        if self.accelerator is not None:
-            self.actor, self.actor_target, self.critic, self.critic_target, \
-            self.actor_optimizer, self.critic_optimizer = self.accelerator.prepare(self.actor,
-                                                                            self.actor_target,
-                                                                            self.critic,
-                                                                            self.critic_target,
-                                                                            self.actor_optimizer_type,
-                                                                            self.critic_optimizer_type)
-    
-    def unwrap_models(self):
-        if self.accelerator is not None:
-            self.actor = self.accelerator.unwrap_model(self.actor)
-            self.actor_target = self.accelerator.unwrap_model(self.actor_target)
-            self.critic = self.accelerator.unwrap_model(self.critic)
-            self.critic_target = self.accelerator.unwrap_model(self.critic_target)
-            self.actor_optimizer = self.accelerator.unwrap_model(self.actor_optimizer)
-            self.critic_optimizer = self.accelerator.unwrap_model(self.critic_optimizer)
-
-    def saveCheckpoint(self, path):
-        """Saves a checkpoint of agent properties and network weights to path.
-
-        :param path: Location to save checkpoint at
-        :type path: string
-        """
-        torch.save({
-            'actor_init_dict': self.actor.init_dict,
-            'actor_state_dict': self.actor.state_dict(),
-            'actor_target_init_dict': self.actor_target.init_dict,
-            'actor_target_state_dict': self.actor_target.state_dict(),
-            'critic_init_dict': self.critic.init_dict,
-            'critic_state_dict': self.critic.state_dict(),
-            'critic_target_init_dict': self.critic_target.init_dict,
-            'critic_target_state_dict': self.critic_target.state_dict(),
-            'actor_optimizer_state_dict': self.actor_optimizer.state_dict(),
-            'critic_optimizer_state_dict': self.critic_optimizer.state_dict(),
-            'net_config': self.net_config,
-            'batch_size': self.batch_size,
-            'lr': self.lr,
-            'learn_step': self.learn_step,
-            'gamma': self.gamma,
-            'tau': self.tau,
-            'mutation': self.mut,
-            'index': self.index,
-            'scores': self.scores,
-            'fitness': self.fitness,
-            'steps': self.steps,
-        }, path, pickle_module=dill)
-
-    def loadCheckpoint(self, path):
-        """Loads saved agent properties and network weights from checkpoint.
-
-        :param path: Location to load checkpoint from
-        :type path: string
-        """
-        checkpoint = torch.load(path, pickle_module=dill)
-        self.net_config = checkpoint['net_config']
-        if self.net_config['arch'] == 'mlp':
-            self.actor = EvolvableMLP(**checkpoint['actor_init_dict'])
-            self.actor_target = EvolvableMLP(**checkpoint['actor_target_init_dict'])
-            self.critic = EvolvableMLP(**checkpoint['critic_init_dict'])
-            self.critic_target = EvolvableMLP(**checkpoint['critic_target_init_dict'])
-        elif self.net_config['arch'] == 'cnn':
-            self.actor = EvolvableCNN(**checkpoint['actor_init_dict'])
-            self.actor_target = EvolvableCNN(**checkpoint['actor_target_init_dict'])
-            self.critic = EvolvableCNN(**checkpoint['critic_init_dict'])
-            self.critic_target = EvolvableCNN(**checkpoint['critic_target_init_dict'])
-        self.lr = checkpoint['lr']
-        self.actor_optimizer = optim.Adam(self.actor.parameters(), lr=self.lr)
-        self.critic_optimizer = optim.Adam(self.critic.parameters(), lr=self.lr)
-        self.actor.load_state_dict(checkpoint['actor_state_dict'])
-        self.actor_target.load_state_dict(checkpoint['actor_target_state_dict'])
-        self.critic.load_state_dict(checkpoint['critic_state_dict'])
-        self.critic_target.load_state_dict(checkpoint['critic_target_state_dict'])
-        self.actor_optimizer.load_state_dict(checkpoint['actor_optimizer_state_dict'])
-        self.critic_optimizer.load_state_dict(checkpoint['critic_optimizer_state_dict'])
-        self.batch_size = checkpoint['batch_size']
-        self.learn_step = checkpoint['learn_step']
-        self.gamma = checkpoint['gamma']
-        self.tau = checkpoint['tau']
-        self.mut = checkpoint['mutation']
-        self.index = checkpoint['index']
-        self.scores = checkpoint['scores']
-        self.fitness = checkpoint['fitness']
-        self.steps = checkpoint['steps']
+import copy
+import random
+
+import dill
+import numpy as np
+import torch
+import torch.nn as nn
+import torch.optim as optim
+
+from agilerl.networks.evolvable_cnn import EvolvableCNN
+from agilerl.networks.evolvable_mlp import EvolvableMLP
+
+
+class DDPG:
+    """The DDPG algorithm class. DDPG paper: https://arxiv.org/abs/1509.02971
+
+    :param state_dim: State observation dimension
+    :type state_dim: int
+    :param action_dim: Action dimension
+    :type action_dim: int
+    :param one_hot: One-hot encoding, used with discrete observation spaces
+    :type one_hot: bool
+    :param index: Index to keep track of object instance during tournament selection and mutation, defaults to 0
+    :type index: int, optional
+    :param net_config: Network configuration, defaults to mlp with hidden size [64,64]
+    :type net_config: dict, optional
+    :param batch_size: Size of batched sample from replay buffer for learning, defaults to 64
+    :type batch_size: int, optional
+    :param lr: Learning rate for optimizer, defaults to 1e-4
+    :type lr: float, optional
+    :param learn_step: Learning frequency, defaults to 5
+    :type learn_step: int, optional
+    :param gamma: Discount factor, defaults to 0.99
+    :type gamma: float, optional
+    :param tau: For soft update of target network parameters, defaults to 1e-3
+    :type tau: float, optional
+    :param mutation: Most recent mutation to agent, defaults to None
+    :type mutation: str, optional
+    :param policy_freq: Frequency of target network updates compared to policy network, defaults to 2
+    :type policy_freq: int, optional
+    :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
+    :type device: str, optional
+    :param accelerator: Accelerator for distributed computing, defaults to None
+    :type accelerator: Hugging Face accelerate.Accelerator(), optional
+    :param wrap: Wrap models for distributed training upon creation, defaults to True
+    :type wrap: bool, optional
+    """
+
+    def __init__(
+        self,
+        state_dim,
+        action_dim,
+        one_hot,
+        index=0,
+        net_config={"arch": "mlp", "h_size": [64, 64]},
+        batch_size=64,
+        lr=1e-4,
+        learn_step=5,
+        gamma=0.99,
+        tau=1e-3,
+        mutation=None,
+        policy_freq=2,
+        device="cpu",
+        accelerator=None,
+        wrap=True,
+    ):
+        self.algo = "DDPG"
+        self.state_dim = state_dim
+        self.action_dim = action_dim
+        self.one_hot = one_hot
+        self.net_config = net_config
+        self.batch_size = batch_size
+        self.lr = lr
+        self.learn_step = learn_step
+        self.gamma = gamma
+        self.tau = tau
+        self.mut = mutation
+        self.policy_freq = policy_freq
+        self.device = device
+        self.accelerator = accelerator
+
+        self.index = index
+        self.scores = []
+        self.fitness = []
+        self.steps = [0]
+
+        # model
+        if self.net_config["arch"] == "mlp":  # Multi-layer Perceptron
+            self.actor = EvolvableMLP(
+                num_inputs=state_dim[0],
+                num_outputs=action_dim,
+                hidden_size=self.net_config["h_size"],
+                output_activation="tanh",
+                device=self.device,
+                accelerator=self.accelerator,
+            )
+            self.actor_target = EvolvableMLP(
+                num_inputs=state_dim[0],
+                num_outputs=action_dim,
+                hidden_size=self.net_config["h_size"],
+                output_activation="tanh",
+                device=self.device,
+                accelerator=self.accelerator,
+            )
+            self.actor_target.load_state_dict(self.actor.state_dict())
+
+            self.critic = EvolvableMLP(
+                num_inputs=state_dim[0] + action_dim,
+                num_outputs=1,
+                hidden_size=self.net_config["h_size"],
+                device=self.device,
+                accelerator=self.accelerator,
+            )
+            self.critic_target = EvolvableMLP(
+                num_inputs=state_dim[0] + action_dim,
+                num_outputs=1,
+                hidden_size=self.net_config["h_size"],
+                device=self.device,
+                accelerator=self.accelerator,
+            )
+            self.critic_target.load_state_dict(self.critic.state_dict())
+
+        elif self.net_config["arch"] == "cnn":  # Convolutional Neural Network
+            self.actor = EvolvableCNN(
+                input_shape=state_dim,
+                num_actions=action_dim,
+                channel_size=self.net_config["c_size"],
+                kernal_size=self.net_config["k_size"],
+                stride_size=self.net_config["s_size"],
+                hidden_size=self.net_config["h_size"],
+                normalize=self.net_config["normalize"],
+                mlp_activation="tanh",
+                device=self.device,
+                accelerator=self.accelerator,
+            )
+            self.actor_target = EvolvableCNN(
+                input_shape=state_dim,
+                num_actions=action_dim,
+                channel_size=self.net_config["c_size"],
+                kernal_size=self.net_config["k_size"],
+                stride_size=self.net_config["s_size"],
+                hidden_size=self.net_config["h_size"],
+                normalize=self.net_config["normalize"],
+                mlp_activation="tanh",
+                device=self.device,
+                accelerator=self.accelerator,
+            )
+            self.actor_target.load_state_dict(self.actor.state_dict())
+
+            self.critic = EvolvableCNN(
+                input_shape=state_dim,
+                num_actions=action_dim,
+                channel_size=self.net_config["c_size"],
+                kernal_size=self.net_config["k_size"],
+                stride_size=self.net_config["s_size"],
+                hidden_size=self.net_config["h_size"],
+                normalize=self.net_config["normalize"],
+                mlp_activation="tanh",
+                critic=True,
+                device=self.device,
+                accelerator=self.accelerator,
+            )
+            self.critic_target = EvolvableCNN(
+                input_shape=state_dim,
+                num_actions=action_dim,
+                channel_size=self.net_config["c_size"],
+                kernal_size=self.net_config["k_size"],
+                stride_size=self.net_config["s_size"],
+                hidden_size=self.net_config["h_size"],
+                normalize=self.net_config["normalize"],
+                mlp_activation="tanh",
+                critic=True,
+                device=self.device,
+                accelerator=self.accelerator,
+            )
+            self.critic_target.load_state_dict(self.critic.state_dict())
+
+        self.actor_optimizer_type = optim.Adam(self.actor.parameters(), lr=self.lr)
+        self.critic_optimizer_type = optim.Adam(self.critic.parameters(), lr=self.lr)
+
+        if self.accelerator is not None:
+            self.actor_optimizer = self.actor_optimizer_type
+            self.critic_optimizer = self.critic_optimizer_type
+            if wrap:
+                self.wrap_models()
+        else:
+            self.actor = self.actor.to(self.device)
+            self.actor_target = self.actor_target.to(self.device)
+            self.critic = self.critic.to(self.device)
+            self.critic_target = self.critic_target.to(self.device)
+            self.actor_optimizer = self.actor_optimizer_type
+            self.critic_optimizer = self.critic_optimizer_type
+
+        self.criterion = nn.MSELoss()
+
+    def getAction(self, state, epsilon=0):
+        """Returns the next action to take in the environment.
+        Epsilon is the probability of taking a random action, used for exploration.
+        For epsilon-greedy behaviour, set epsilon to 0.
+
+        :param state: Environment observation, or multiple observations in a batch
+        :type state: float or List[float]
+        :param epsilon: Probablilty of taking a random action for exploration, defaults to 0
+        :type epsilon: float, optional
+        """
+        state = torch.from_numpy(state).float()
+        if self.accelerator is None:
+            state = state.to(self.device)
+
+        if self.one_hot:
+            state = (
+                nn.functional.one_hot(state.long(), num_classes=self.state_dim[0])
+                .float()
+                .squeeze()
+            )
+
+        if len(state.size()) < 2:
+            state = state.unsqueeze(0)
+
+        # epsilon-greedy
+        if random.random() < epsilon:
+            action = (
+                np.random.rand(state.size()[0], self.action_dim).astype("float32") - 0.5
+            ) * 2
+        else:
+            self.actor.eval()
+            with torch.no_grad():
+                action_values = self.actor(state)
+            self.actor.train()
+
+            action = action_values.cpu().data.numpy()
+
+        return action
+
+    def _squeeze_exp(self, experiences):
+        """Remove first dim created by dataloader.
+
+        :param experiences: List of batched states, actions, rewards, next_states, dones in that order.
+        :type state: List[torch.Tensor[float]]
+        """
+        st, ac, re, ne, do = experiences
+        return st.squeeze(0), ac.squeeze(0), re.squeeze(0), ne.squeeze(0), do.squeeze(0)
+
+    def learn(self, experiences, noise_clip=0.5, policy_noise=0.2):
+        """Updates agent network parameters to learn from experiences.
+
+        :param experience: List of batched states, actions, rewards, next_states, dones in that order.
+        :type experience: List[torch.Tensor[float]]
+        :param noise_clip: Maximum noise limit to apply to actions, defaults to 0.5
+        :type noise_clip: float, optional
+        :param policy_noise: Standard deviation of noise applied to policy, defaults to 0.2
+        :type policy_noise: float, optional
+        """
+        states, actions, rewards, next_states, dones = experiences
+
+        if self.one_hot:
+            states = (
+                nn.functional.one_hot(states.long(), num_classes=self.state_dim[0])
+                .float()
+                .squeeze()
+            )
+            next_states = (
+                nn.functional.one_hot(next_states.long(), num_classes=self.state_dim[0])
+                .float()
+                .squeeze()
+            )
+
+        if self.net_config["arch"] == "mlp":
+            input_combined = torch.cat([states, actions], 1)
+            q_value = self.critic(input_combined)
+        elif self.net_config["arch"] == "cnn":
+            q_value = self.critic(states, actions)
+
+        next_actions = self.actor_target(next_states)
+        noise = actions.data.normal_(0, policy_noise)
+        noise = noise.clamp(-noise_clip, noise_clip)
+        next_actions = next_actions + noise
+
+        if self.net_config["arch"] == "mlp":
+            next_input_combined = torch.cat([next_states, next_actions], 1)
+            q_value_next_state = self.critic_target(next_input_combined)
+        elif self.net_config["arch"] == "cnn":
+            q_value_next_state = self.critic_target(next_states, next_actions)
+
+        y_j = rewards + ((1 - dones) * self.gamma * q_value_next_state).detach()
+
+        critic_loss = self.criterion(q_value, y_j)
+
+        # critic loss backprop
+        self.critic_optimizer.zero_grad()
+        if self.accelerator is not None:
+            self.accelerator.backward(critic_loss)
+        else:
+            critic_loss.backward()
+        self.critic_optimizer.step()
+
+        # update actor and targets every policy_freq episodes
+        if len(self.scores) % self.policy_freq == 0:
+            if self.net_config["arch"] == "mlp":
+                input_combined = torch.cat([states, self.actor.forward(states)], 1)
+                actor_loss = -self.critic(input_combined).mean()
+            elif self.net_config["arch"] == "cnn":
+                actor_loss = -self.critic(states, self.actor.forward(states)).mean()
+
+            # actor loss backprop
+            self.actor_optimizer.zero_grad()
+            if self.accelerator is not None:
+                self.accelerator.backward(actor_loss)
+            else:
+                actor_loss.backward()
+            self.actor_optimizer.step()
+
+            self.softUpdate(self.actor, self.actor_target)
+            self.softUpdate(self.critic, self.critic_target)
+
+    def softUpdate(self, net, target):
+        """Soft updates target network."""
+        for eval_param, target_param in zip(net.parameters(), target.parameters()):
+            target_param.data.copy_(
+                self.tau * eval_param.data + (1.0 - self.tau) * target_param.data
+            )
+
+    def test(self, env, swap_channels=False, max_steps=500, loop=3):
+        """Returns mean test score of agent in environment with epsilon-greedy policy.
+
+        :param env: The environment to be tested in
+        :type env: Gym-style environment
+        :param swap_channels: Swap image channels dimension from last to first [H, W, C] -> [C, H, W], defaults to False
+        :type swap_channels: bool, optional
+        :param max_steps: Maximum number of testing steps, defaults to 500
+        :type max_steps: int, optional
+        :param loop: Number of testing loops/epsiodes to complete. The returned score is the mean. Defaults to 3
+        :type loop: int, optional
+        """
+        with torch.no_grad():
+            rewards = []
+            for i in range(loop):
+                state = env.reset()[0]
+                score = 0
+                for idx_step in range(max_steps):
+                    if swap_channels:
+                        state = np.moveaxis(state, [3], [1])
+                    action = self.getAction(state, epsilon=0)
+                    state, reward, done, trunc, info = env.step(action)
+                    score += reward
+                rewards.append(score)
+        mean_fit = np.mean(rewards)
+        self.fitness.append(mean_fit)
+        return mean_fit
+
+    def clone(self, index=None, wrap=True):
+        """Returns cloned agent identical to self.
+
+        :param index: Index to keep track of agent for tournament selection and mutation, defaults to None
+        :type index: int, optional
+        """
+        if index is None:
+            index = self.index
+
+        clone = type(self)(
+            state_dim=self.state_dim,
+            action_dim=self.action_dim,
+            one_hot=self.one_hot,
+            index=index,
+            net_config=self.net_config,
+            batch_size=self.batch_size,
+            lr=self.lr,
+            learn_step=self.learn_step,
+            gamma=self.gamma,
+            tau=self.tau,
+            mutation=self.mut,
+            policy_freq=self.policy_freq,
+            device=self.device,
+            accelerator=self.accelerator,
+            wrap=wrap,
+        )
+
+        if self.accelerator is not None:
+            self.unwrap_models()
+        actor = self.actor.clone()
+        actor_target = self.actor_target.clone()
+        critic = self.critic.clone()
+        critic_target = self.critic_target.clone()
+        actor_optimizer = optim.Adam(actor.parameters(), lr=clone.lr)
+        critic_optimizer = optim.Adam(critic.parameters(), lr=clone.lr)
+        clone.actor_optimizer_type = actor_optimizer
+        clone.critic_optimizer_type = critic_optimizer
+
+        if self.accelerator is not None:
+            if wrap:
+                (
+                    clone.actor,
+                    clone.actor_target,
+                    clone.critic,
+                    clone.critic_target,
+                    clone.actor_optimizer,
+                    clone.critic_optimizer,
+                ) = self.accelerator.prepare(
+                    actor,
+                    actor_target,
+                    critic,
+                    critic_target,
+                    actor_optimizer,
+                    critic_optimizer,
+                )
+            else:
+                (
+                    clone.actor,
+                    clone.actor_target,
+                    clone.critic,
+                    clone.critic_target,
+                    clone.actor_optimizer,
+                    clone.critic_optimizer,
+                ) = (
+                    actor,
+                    actor_target,
+                    critic,
+                    critic_target,
+                    actor_optimizer,
+                    critic_optimizer,
+                )
+        else:
+            clone.actor = actor.to(self.device)
+            clone.actor_target = actor_target.to(self.device)
+            clone.critic = critic.to(self.device)
+            clone.critic_target = critic_target.to(self.device)
+            clone.actor_optimizer = actor_optimizer
+            clone.critic_optimizer = critic_optimizer
+
+        clone.fitness = copy.deepcopy(self.fitness)
+        clone.steps = copy.deepcopy(self.steps)
+        clone.scores = copy.deepcopy(self.scores)
+
+        return clone
+
+    def wrap_models(self):
+        if self.accelerator is not None:
+            (
+                self.actor,
+                self.actor_target,
+                self.critic,
+                self.critic_target,
+                self.actor_optimizer,
+                self.critic_optimizer,
+            ) = self.accelerator.prepare(
+                self.actor,
+                self.actor_target,
+                self.critic,
+                self.critic_target,
+                self.actor_optimizer_type,
+                self.critic_optimizer_type,
+            )
+
+    def unwrap_models(self):
+        if self.accelerator is not None:
+            self.actor = self.accelerator.unwrap_model(self.actor)
+            self.actor_target = self.accelerator.unwrap_model(self.actor_target)
+            self.critic = self.accelerator.unwrap_model(self.critic)
+            self.critic_target = self.accelerator.unwrap_model(self.critic_target)
+            self.actor_optimizer = self.accelerator.unwrap_model(self.actor_optimizer)
+            self.critic_optimizer = self.accelerator.unwrap_model(self.critic_optimizer)
+
+    def saveCheckpoint(self, path):
+        """Saves a checkpoint of agent properties and network weights to path.
+
+        :param path: Location to save checkpoint at
+        :type path: string
+        """
+        torch.save(
+            {
+                "actor_init_dict": self.actor.init_dict,
+                "actor_state_dict": self.actor.state_dict(),
+                "actor_target_init_dict": self.actor_target.init_dict,
+                "actor_target_state_dict": self.actor_target.state_dict(),
+                "critic_init_dict": self.critic.init_dict,
+                "critic_state_dict": self.critic.state_dict(),
+                "critic_target_init_dict": self.critic_target.init_dict,
+                "critic_target_state_dict": self.critic_target.state_dict(),
+                "actor_optimizer_state_dict": self.actor_optimizer.state_dict(),
+                "critic_optimizer_state_dict": self.critic_optimizer.state_dict(),
+                "net_config": self.net_config,
+                "batch_size": self.batch_size,
+                "lr": self.lr,
+                "learn_step": self.learn_step,
+                "gamma": self.gamma,
+                "tau": self.tau,
+                "mutation": self.mut,
+                "index": self.index,
+                "scores": self.scores,
+                "fitness": self.fitness,
+                "steps": self.steps,
+            },
+            path,
+            pickle_module=dill,
+        )
+
+    def loadCheckpoint(self, path):
+        """Loads saved agent properties and network weights from checkpoint.
+
+        :param path: Location to load checkpoint from
+        :type path: string
+        """
+        checkpoint = torch.load(path, pickle_module=dill)
+        self.net_config = checkpoint["net_config"]
+        if self.net_config["arch"] == "mlp":
+            self.actor = EvolvableMLP(**checkpoint["actor_init_dict"])
+            self.actor_target = EvolvableMLP(**checkpoint["actor_target_init_dict"])
+            self.critic = EvolvableMLP(**checkpoint["critic_init_dict"])
+            self.critic_target = EvolvableMLP(**checkpoint["critic_target_init_dict"])
+        elif self.net_config["arch"] == "cnn":
+            self.actor = EvolvableCNN(**checkpoint["actor_init_dict"])
+            self.actor_target = EvolvableCNN(**checkpoint["actor_target_init_dict"])
+            self.critic = EvolvableCNN(**checkpoint["critic_init_dict"])
+            self.critic_target = EvolvableCNN(**checkpoint["critic_target_init_dict"])
+        self.lr = checkpoint["lr"]
+        self.actor_optimizer = optim.Adam(self.actor.parameters(), lr=self.lr)
+        self.critic_optimizer = optim.Adam(self.critic.parameters(), lr=self.lr)
+        self.actor.load_state_dict(checkpoint["actor_state_dict"])
+        self.actor_target.load_state_dict(checkpoint["actor_target_state_dict"])
+        self.critic.load_state_dict(checkpoint["critic_state_dict"])
+        self.critic_target.load_state_dict(checkpoint["critic_target_state_dict"])
+        self.actor_optimizer.load_state_dict(checkpoint["actor_optimizer_state_dict"])
+        self.critic_optimizer.load_state_dict(checkpoint["critic_optimizer_state_dict"])
+        self.batch_size = checkpoint["batch_size"]
+        self.learn_step = checkpoint["learn_step"]
+        self.gamma = checkpoint["gamma"]
+        self.tau = checkpoint["tau"]
+        self.mut = checkpoint["mutation"]
+        self.index = checkpoint["index"]
+        self.scores = checkpoint["scores"]
+        self.fitness = checkpoint["fitness"]
+        self.steps = checkpoint["steps"]
```

### Comparing `agilerl-0.1.8/agilerl/algorithms/dqn.py` & `agilerl-0.1.9/agilerl/algorithms/dqn.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,347 +1,390 @@
-import random
-import copy
-import dill
-import numpy as np
-import torch
-import torch.nn as nn
-import torch.optim as optim
-from agilerl.networks.evolvable_mlp import EvolvableMLP
-from agilerl.networks.evolvable_cnn import EvolvableCNN
-
-
-class DQN():
-    """The DQN algorithm class. DQN paper: https://arxiv.org/abs/1312.5602
-
-    :param state_dim: State observation dimension
-    :type state_dim: int
-    :param action_dim: Action dimension
-    :type action_dim: int
-    :param one_hot: One-hot encoding, used with discrete observation spaces
-    :type one_hot: bool
-    :param index: Index to keep track of object instance during tournament selection and mutation, defaults to 0
-    :type index: int, optional
-    :param net_config: Network configuration, defaults to mlp with hidden size [64,64]
-    :type net_config: dict, optional
-    :param batch_size: Size of batched sample from replay buffer for learning, defaults to 64
-    :type batch_size: int, optional
-    :param lr: Learning rate for optimizer, defaults to 1e-4
-    :type lr: float, optional
-    :param learn_step: Learning frequency, defaults to 5
-    :type learn_step: int, optional
-    :param gamma: Discount factor, defaults to 0.99
-    :type gamma: float, optional
-    :param tau: For soft update of target network parameters, defaults to 1e-3
-    :type tau: float, optional
-    :param mutation: Most recent mutation to agent, defaults to None
-    :type mutation: str, optional
-    :param double: Use double Q-learning, defaults to False
-    :type double: bool, optional
-    :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
-    :type device: str, optional
-    :param accelerator: Accelerator for distributed computing, defaults to None
-    :type accelerator: Hugging Face accelerate.Accelerator(), optional
-    :param wrap: Wrap models for distributed training upon creation, defaults to True
-    :type wrap: bool, optional
-    """
-
-    def __init__(self, state_dim, action_dim, one_hot, index=0, 
-                 net_config={'arch': 'mlp', 'h_size':[64,64]}, batch_size=64, lr=1e-4, 
-                 learn_step=5, gamma=0.99, tau=1e-3, mutation=None, double=False, 
-                 device='cpu', accelerator=None, wrap=True):
-        self.algo = 'DQN'
-        self.state_dim = state_dim
-        self.action_dim = action_dim
-        self.one_hot = one_hot
-        self.net_config = net_config
-        self.batch_size = batch_size
-        self.lr = lr
-        self.learn_step = learn_step
-        self.gamma = gamma
-        self.tau = tau
-        self.mut = mutation
-        self.device = device
-        self.accelerator = accelerator
-        self.index = index
-        self.scores = []
-        self.fitness = []
-        self.steps = [0]
-        self.double = double
-
-        # model
-        if self.net_config['arch'] == 'mlp':      # Multi-layer Perceptron
-            self.actor = EvolvableMLP(
-                num_inputs=state_dim[0],
-                num_outputs=action_dim,
-                hidden_size=self.net_config['h_size'],
-                device=self.device,
-                accelerator=self.accelerator)
-            self.actor_target = EvolvableMLP(
-                num_inputs=state_dim[0],
-                num_outputs=action_dim,
-                hidden_size=self.net_config['h_size'],
-                device=self.device,
-                accelerator=self.accelerator)
-            self.actor_target.load_state_dict(self.actor.state_dict())
-
-        elif self.net_config['arch'] == 'cnn':    # Convolutional Neural Network
-            self.actor = EvolvableCNN(
-                input_shape=state_dim,
-                num_actions=action_dim,
-                channel_size=self.net_config['c_size'],
-                kernal_size=self.net_config['k_size'],
-                stride_size=self.net_config['s_size'],
-                hidden_size=self.net_config['h_size'],
-                normalize=self.net_config['normalize'],
-                device=self.device,
-                accelerator=self.accelerator)
-            self.actor_target = EvolvableCNN(
-                input_shape=state_dim,
-                num_actions=action_dim,
-                channel_size=self.net_config['c_size'],
-                kernal_size=self.net_config['k_size'],
-                stride_size=self.net_config['s_size'],
-                hidden_size=self.net_config['h_size'],
-                normalize=self.net_config['normalize'],
-                device=self.device,
-                accelerator=self.accelerator)
-            self.actor_target.load_state_dict(self.actor.state_dict())
-
-        self.optimizer_type = optim.Adam(self.actor.parameters(), lr=self.lr)
-
-        if self.accelerator is not None:
-            self.optimizer = self.optimizer_type
-            if wrap:
-                self.wrap_models()
-        else:
-            self.actor = self.actor.to(self.device)
-            self.actor_target = self.actor_target.to(self.device)
-            self.optimizer = self.optimizer_type
-
-        self.criterion = nn.MSELoss()
-
-    def getAction(self, state, epsilon=0):
-        """Returns the next action to take in the environment. 
-        Epsilon is the probability of taking a random action, used for exploration.
-        For epsilon-greedy behaviour, set epsilon to 0.
-
-        :param state: State observation, or multiple observations in a batch
-        :type state: float or List[float]
-        :param epsilon: Probablilty of taking a random action for exploration, defaults to 0
-        :type epsilon: float, optional
-        """
-        state = torch.from_numpy(state).float()
-        if self.accelerator is None:
-            state = state.to(self.device)
-
-        if self.one_hot:
-            state = nn.functional.one_hot(
-                state.long(), num_classes=self.state_dim[0]).float().squeeze()
-
-        if len(state.size()) < 2:
-            state = state.unsqueeze(0)
-
-        # epsilon-greedy
-        if random.random() < epsilon:
-            action = np.random.randint(0, self.action_dim, size=state.size()[0])
-        else:
-            self.actor.eval()
-            with torch.no_grad():
-                action_values = self.actor(state)
-            self.actor.train()
-
-            action = np.argmax(action_values.cpu().data.numpy(), axis=1)
-
-        return action
-    
-    def _squeeze_exp(self, experiences):
-        """Remove first dim created by dataloader.
-        
-        :param experiences: List of batched states, actions, rewards, next_states, dones in that order.
-        :type state: List[torch.Tensor[float]]
-        """
-        st, ac, re, ne, do = experiences
-        return st.squeeze(0), ac.squeeze(0), re.squeeze(0), ne.squeeze(0), do.squeeze(0)
-
-    def learn(self, experiences):
-        """Updates agent network parameters to learn from experiences.
-
-        :param experiences: List of batched states, actions, rewards, next_states, dones in that order.
-        :type state: List[torch.Tensor[float]]
-        """
-        states, actions, rewards, next_states, dones = experiences
-
-        if self.one_hot:
-            states = nn.functional.one_hot(
-                states.long(), num_classes=self.state_dim[0]).float().squeeze()
-            next_states = nn.functional.one_hot(
-                next_states.long(), num_classes=self.state_dim[0]).float().squeeze()
-
-        if self.double: # Double Q-learning
-            q_idx = self.actor_target(next_states).argmax(dim=1).unsqueeze(1)
-            q_target = self.actor(next_states).gather(dim=1, index=q_idx).detach()
-        else:
-            q_target = self.actor_target(next_states).detach().max(axis=1)[0].unsqueeze(1)
-
-        # target, if terminal then y_j = rewards
-        y_j = rewards + self.gamma * q_target * (1 - dones)
-        q_eval = self.actor(states).gather(1, actions.long())
-
-        # loss backprop
-        loss = self.criterion(q_eval, y_j)
-        self.optimizer.zero_grad()
-        if self.accelerator is not None:
-            self.accelerator.backward(loss)
-        else:
-            loss.backward()
-        self.optimizer.step()
-
-        # soft update target network
-        self.softUpdate()
-
-    def softUpdate(self):
-        """Soft updates target network.
-        """
-        for eval_param, target_param in zip(
-                self.actor.parameters(), self.actor_target.parameters()):
-            target_param.data.copy_(
-                self.tau * eval_param.data + (1.0 - self.tau) * target_param.data)
-
-    def test(self, env, swap_channels=False, max_steps=500, loop=3):
-        """Returns mean test score of agent in environment with epsilon-greedy policy.
-
-        :param env: The environment to be tested in
-        :type env: Gym-style environment
-        :param swap_channels: Swap image channels dimension from last to first [H, W, C] -> [C, H, W], defaults to False
-        :type swap_channels: bool, optional
-        :param max_steps: Maximum number of testing steps, defaults to 500
-        :type max_steps: int, optional
-        :param loop: Number of testing loops/epsiodes to complete. The returned score is the mean over these tests. Defaults to 3
-        :type loop: int, optional
-        """
-        with torch.no_grad():
-            rewards = []
-            for i in range(loop):
-                state = env.reset()[0]
-                score = 0
-                for idx_step in range(max_steps):
-                    if swap_channels:
-                        state = np.moveaxis(state, [3], [1])
-                    action = self.getAction(state, epsilon=0)
-                    state, reward, done, _, _ = env.step(action)
-                    score += reward
-                rewards.append(score)
-        mean_fit = np.mean(rewards)
-        self.fitness.append(mean_fit)
-        return mean_fit
-
-    def clone(self, index=None, wrap=True):
-        """Returns cloned agent identical to self.
-
-        :param index: Index to keep track of agent for tournament selection and mutation, defaults to None
-        :type index: int, optional
-        """
-        if index is None:
-            index = self.index
-
-        clone = type(self)(state_dim=self.state_dim,
-                           action_dim=self.action_dim,
-                           one_hot=self.one_hot,
-                           index=index,
-                           net_config=self.net_config,
-                           batch_size=self.batch_size,
-                           lr=self.lr,
-                           learn_step=self.learn_step,
-                           gamma=self.gamma,
-                           tau=self.tau,
-                           mutation=self.mut,
-                           device=self.device,
-                           accelerator=self.accelerator,
-                           wrap=wrap)
-
-        actor = self.actor.clone()
-        actor_target = self.actor_target.clone()
-        optimizer = optim.Adam(actor.parameters(), lr=clone.lr)
-        clone.optimizer_type = optimizer
-        if self.accelerator is not None:
-            if wrap:
-                clone.actor, clone.actor_target, clone.optimizer = self.accelerator.prepare(
-                                                                                        actor, 
-                                                                                        actor_target,
-                                                                                        optimizer)
-            else:
-                clone.actor, clone.actor_target, clone.optimizer = actor, actor_target, optimizer
-        else:
-            clone.actor = actor.to(self.device)
-            clone.actor_target = actor_target.to(self.device)
-            clone.optimizer = optimizer
-        clone.fitness = copy.deepcopy(self.fitness)
-        clone.steps = copy.deepcopy(self.steps)
-        clone.scores = copy.deepcopy(self.scores)
-
-        return clone
-
-    def wrap_models(self):
-        if self.accelerator is not None:
-            self.actor, self.actor_target, self.optimizer = self.accelerator.prepare(self.actor, 
-                                                                            self.actor_target, 
-                                                                            self.optimizer)
-    
-    def unwrap_models(self):
-        if self.accelerator is not None:
-            self.actor = self.accelerator.unwrap_model(self.actor)
-            self.actor_target = self.accelerator.unwrap_model(self.actor_target)
-            self.optimizer = self.accelerator.unwrap_model(self.optimizer)
-
-    def saveCheckpoint(self, path):
-        """Saves a checkpoint of agent properties and network weights to path.
-
-        :param path: Location to save checkpoint at
-        :type path: string
-        """
-        torch.save({
-            'actor_init_dict': self.actor.init_dict,
-            'actor_state_dict': self.actor.state_dict(),
-            'actor_target_init_dict': self.actor_target.init_dict,
-            'actor_target_state_dict': self.actor_target.state_dict(),
-            'optimizer_state_dict': self.optimizer.state_dict(),
-            'net_config': self.net_config,
-            'batch_size': self.batch_size,
-            'lr': self.lr,
-            'learn_step': self.learn_step,
-            'gamma': self.gamma,
-            'tau': self.tau,
-            'mutation': self.mut,
-            'index': self.index,
-            'scores': self.scores,
-            'fitness': self.fitness,
-            'steps': self.steps,
-        }, path, pickle_module=dill)
-
-    def loadCheckpoint(self, path):
-        """Loads saved agent properties and network weights from checkpoint.
-
-        :param path: Location to load checkpoint from
-        :type path: string
-        """
-        checkpoint = torch.load(path, pickle_module=dill)
-        self.net_config = checkpoint['net_config']
-        if self.net_config['arch'] == 'mlp':
-            self.actor = EvolvableMLP(**checkpoint['actor_init_dict'])
-            self.actor_target = EvolvableMLP(**checkpoint['actor_target_init_dict'])
-        elif self.net_config['arch'] == 'cnn':
-            self.actor = EvolvableCNN(**checkpoint['actor_init_dict'])
-            self.actor_target = EvolvableCNN(**checkpoint['actor_target_init_dict'])
-        self.lr = checkpoint['lr']
-        self.optimizer = optim.Adam(self.actor.parameters(), lr=self.lr)
-        self.actor.load_state_dict(checkpoint['actor_state_dict'])
-        self.actor_target.load_state_dict(checkpoint['actor_target_state_dict'])
-        self.optimizer.load_state_dict(checkpoint['optimizer_state_dict'])
-        self.batch_size = checkpoint['batch_size']
-        self.learn_step = checkpoint['learn_step']
-        self.gamma = checkpoint['gamma']
-        self.tau = checkpoint['tau']
-        self.mut = checkpoint['mutation']
-        self.index = checkpoint['index']
-        self.scores = checkpoint['scores']
-        self.fitness = checkpoint['fitness']
-        self.steps = checkpoint['steps']
+import copy
+import random
+
+import dill
+import numpy as np
+import torch
+import torch.nn as nn
+import torch.optim as optim
+
+from agilerl.networks.evolvable_cnn import EvolvableCNN
+from agilerl.networks.evolvable_mlp import EvolvableMLP
+
+
+class DQN:
+    """The DQN algorithm class. DQN paper: https://arxiv.org/abs/1312.5602
+
+    :param state_dim: State observation dimension
+    :type state_dim: int
+    :param action_dim: Action dimension
+    :type action_dim: int
+    :param one_hot: One-hot encoding, used with discrete observation spaces
+    :type one_hot: bool
+    :param index: Index to keep track of object instance during tournament selection and mutation, defaults to 0
+    :type index: int, optional
+    :param net_config: Network configuration, defaults to mlp with hidden size [64,64]
+    :type net_config: dict, optional
+    :param batch_size: Size of batched sample from replay buffer for learning, defaults to 64
+    :type batch_size: int, optional
+    :param lr: Learning rate for optimizer, defaults to 1e-4
+    :type lr: float, optional
+    :param learn_step: Learning frequency, defaults to 5
+    :type learn_step: int, optional
+    :param gamma: Discount factor, defaults to 0.99
+    :type gamma: float, optional
+    :param tau: For soft update of target network parameters, defaults to 1e-3
+    :type tau: float, optional
+    :param mutation: Most recent mutation to agent, defaults to None
+    :type mutation: str, optional
+    :param double: Use double Q-learning, defaults to False
+    :type double: bool, optional
+    :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
+    :type device: str, optional
+    :param accelerator: Accelerator for distributed computing, defaults to None
+    :type accelerator: Hugging Face accelerate.Accelerator(), optional
+    :param wrap: Wrap models for distributed training upon creation, defaults to True
+    :type wrap: bool, optional
+    """
+
+    def __init__(
+        self,
+        state_dim,
+        action_dim,
+        one_hot,
+        index=0,
+        net_config={"arch": "mlp", "h_size": [64, 64]},
+        batch_size=64,
+        lr=1e-4,
+        learn_step=5,
+        gamma=0.99,
+        tau=1e-3,
+        mutation=None,
+        double=False,
+        device="cpu",
+        accelerator=None,
+        wrap=True,
+    ):
+        self.algo = "DQN"
+        self.state_dim = state_dim
+        self.action_dim = action_dim
+        self.one_hot = one_hot
+        self.net_config = net_config
+        self.batch_size = batch_size
+        self.lr = lr
+        self.learn_step = learn_step
+        self.gamma = gamma
+        self.tau = tau
+        self.mut = mutation
+        self.device = device
+        self.accelerator = accelerator
+        self.index = index
+        self.scores = []
+        self.fitness = []
+        self.steps = [0]
+        self.double = double
+
+        # model
+        if self.net_config["arch"] == "mlp":  # Multi-layer Perceptron
+            self.actor = EvolvableMLP(
+                num_inputs=state_dim[0],
+                num_outputs=action_dim,
+                hidden_size=self.net_config["h_size"],
+                device=self.device,
+                accelerator=self.accelerator,
+            )
+            self.actor_target = EvolvableMLP(
+                num_inputs=state_dim[0],
+                num_outputs=action_dim,
+                hidden_size=self.net_config["h_size"],
+                device=self.device,
+                accelerator=self.accelerator,
+            )
+            self.actor_target.load_state_dict(self.actor.state_dict())
+
+        elif self.net_config["arch"] == "cnn":  # Convolutional Neural Network
+            self.actor = EvolvableCNN(
+                input_shape=state_dim,
+                num_actions=action_dim,
+                channel_size=self.net_config["c_size"],
+                kernal_size=self.net_config["k_size"],
+                stride_size=self.net_config["s_size"],
+                hidden_size=self.net_config["h_size"],
+                normalize=self.net_config["normalize"],
+                device=self.device,
+                accelerator=self.accelerator,
+            )
+            self.actor_target = EvolvableCNN(
+                input_shape=state_dim,
+                num_actions=action_dim,
+                channel_size=self.net_config["c_size"],
+                kernal_size=self.net_config["k_size"],
+                stride_size=self.net_config["s_size"],
+                hidden_size=self.net_config["h_size"],
+                normalize=self.net_config["normalize"],
+                device=self.device,
+                accelerator=self.accelerator,
+            )
+            self.actor_target.load_state_dict(self.actor.state_dict())
+
+        self.optimizer_type = optim.Adam(self.actor.parameters(), lr=self.lr)
+
+        if self.accelerator is not None:
+            self.optimizer = self.optimizer_type
+            if wrap:
+                self.wrap_models()
+        else:
+            self.actor = self.actor.to(self.device)
+            self.actor_target = self.actor_target.to(self.device)
+            self.optimizer = self.optimizer_type
+
+        self.criterion = nn.MSELoss()
+
+    def getAction(self, state, epsilon=0):
+        """Returns the next action to take in the environment.
+        Epsilon is the probability of taking a random action, used for exploration.
+        For epsilon-greedy behaviour, set epsilon to 0.
+
+        :param state: State observation, or multiple observations in a batch
+        :type state: float or List[float]
+        :param epsilon: Probablilty of taking a random action for exploration, defaults to 0
+        :type epsilon: float, optional
+        """
+        state = torch.from_numpy(state).float()
+        if self.accelerator is None:
+            state = state.to(self.device)
+
+        if self.one_hot:
+            state = (
+                nn.functional.one_hot(state.long(), num_classes=self.state_dim[0])
+                .float()
+                .squeeze()
+            )
+
+        if len(state.size()) < 2:
+            state = state.unsqueeze(0)
+
+        # epsilon-greedy
+        if random.random() < epsilon:
+            action = np.random.randint(0, self.action_dim, size=state.size()[0])
+        else:
+            self.actor.eval()
+            with torch.no_grad():
+                action_values = self.actor(state)
+            self.actor.train()
+
+            action = np.argmax(action_values.cpu().data.numpy(), axis=1)
+
+        return action
+
+    def _squeeze_exp(self, experiences):
+        """Remove first dim created by dataloader.
+
+        :param experiences: List of batched states, actions, rewards, next_states, dones in that order.
+        :type state: List[torch.Tensor[float]]
+        """
+        st, ac, re, ne, do = experiences
+        return st.squeeze(0), ac.squeeze(0), re.squeeze(0), ne.squeeze(0), do.squeeze(0)
+
+    def learn(self, experiences):
+        """Updates agent network parameters to learn from experiences.
+
+        :param experiences: List of batched states, actions, rewards, next_states, dones in that order.
+        :type state: List[torch.Tensor[float]]
+        """
+        states, actions, rewards, next_states, dones = experiences
+
+        if self.one_hot:
+            states = (
+                nn.functional.one_hot(states.long(), num_classes=self.state_dim[0])
+                .float()
+                .squeeze()
+            )
+            next_states = (
+                nn.functional.one_hot(next_states.long(), num_classes=self.state_dim[0])
+                .float()
+                .squeeze()
+            )
+
+        if self.double:  # Double Q-learning
+            q_idx = self.actor_target(next_states).argmax(dim=1).unsqueeze(1)
+            q_target = self.actor(next_states).gather(dim=1, index=q_idx).detach()
+        else:
+            q_target = (
+                self.actor_target(next_states).detach().max(axis=1)[0].unsqueeze(1)
+            )
+
+        # target, if terminal then y_j = rewards
+        y_j = rewards + self.gamma * q_target * (1 - dones)
+        q_eval = self.actor(states).gather(1, actions.long())
+
+        # loss backprop
+        loss = self.criterion(q_eval, y_j)
+        self.optimizer.zero_grad()
+        if self.accelerator is not None:
+            self.accelerator.backward(loss)
+        else:
+            loss.backward()
+        self.optimizer.step()
+
+        # soft update target network
+        self.softUpdate()
+
+    def softUpdate(self):
+        """Soft updates target network."""
+        for eval_param, target_param in zip(
+            self.actor.parameters(), self.actor_target.parameters()
+        ):
+            target_param.data.copy_(
+                self.tau * eval_param.data + (1.0 - self.tau) * target_param.data
+            )
+
+    def test(self, env, swap_channels=False, max_steps=500, loop=3):
+        """Returns mean test score of agent in environment with epsilon-greedy policy.
+
+        :param env: The environment to be tested in
+        :type env: Gym-style environment
+        :param swap_channels: Swap image channels dimension from last to first [H, W, C] -> [C, H, W], defaults to False
+        :type swap_channels: bool, optional
+        :param max_steps: Maximum number of testing steps, defaults to 500
+        :type max_steps: int, optional
+        :param loop: Number of testing loops/epsiodes to complete. The returned score is the mean over these tests. Defaults to 3
+        :type loop: int, optional
+        """
+        with torch.no_grad():
+            rewards = []
+            for i in range(loop):
+                state = env.reset()[0]
+                score = 0
+                for idx_step in range(max_steps):
+                    if swap_channels:
+                        state = np.moveaxis(state, [3], [1])
+                    action = self.getAction(state, epsilon=0)
+                    state, reward, done, _, _ = env.step(action)
+                    score += reward
+                rewards.append(score)
+        mean_fit = np.mean(rewards)
+        self.fitness.append(mean_fit)
+        return mean_fit
+
+    def clone(self, index=None, wrap=True):
+        """Returns cloned agent identical to self.
+
+        :param index: Index to keep track of agent for tournament selection and mutation, defaults to None
+        :type index: int, optional
+        """
+        if index is None:
+            index = self.index
+
+        clone = type(self)(
+            state_dim=self.state_dim,
+            action_dim=self.action_dim,
+            one_hot=self.one_hot,
+            index=index,
+            net_config=self.net_config,
+            batch_size=self.batch_size,
+            lr=self.lr,
+            learn_step=self.learn_step,
+            gamma=self.gamma,
+            tau=self.tau,
+            mutation=self.mut,
+            device=self.device,
+            accelerator=self.accelerator,
+            wrap=wrap,
+        )
+
+        actor = self.actor.clone()
+        actor_target = self.actor_target.clone()
+        optimizer = optim.Adam(actor.parameters(), lr=clone.lr)
+        clone.optimizer_type = optimizer
+        if self.accelerator is not None:
+            if wrap:
+                (
+                    clone.actor,
+                    clone.actor_target,
+                    clone.optimizer,
+                ) = self.accelerator.prepare(actor, actor_target, optimizer)
+            else:
+                clone.actor, clone.actor_target, clone.optimizer = (
+                    actor,
+                    actor_target,
+                    optimizer,
+                )
+        else:
+            clone.actor = actor.to(self.device)
+            clone.actor_target = actor_target.to(self.device)
+            clone.optimizer = optimizer
+        clone.fitness = copy.deepcopy(self.fitness)
+        clone.steps = copy.deepcopy(self.steps)
+        clone.scores = copy.deepcopy(self.scores)
+
+        return clone
+
+    def wrap_models(self):
+        if self.accelerator is not None:
+            self.actor, self.actor_target, self.optimizer = self.accelerator.prepare(
+                self.actor, self.actor_target, self.optimizer
+            )
+
+    def unwrap_models(self):
+        if self.accelerator is not None:
+            self.actor = self.accelerator.unwrap_model(self.actor)
+            self.actor_target = self.accelerator.unwrap_model(self.actor_target)
+            self.optimizer = self.accelerator.unwrap_model(self.optimizer)
+
+    def saveCheckpoint(self, path):
+        """Saves a checkpoint of agent properties and network weights to path.
+
+        :param path: Location to save checkpoint at
+        :type path: string
+        """
+        torch.save(
+            {
+                "actor_init_dict": self.actor.init_dict,
+                "actor_state_dict": self.actor.state_dict(),
+                "actor_target_init_dict": self.actor_target.init_dict,
+                "actor_target_state_dict": self.actor_target.state_dict(),
+                "optimizer_state_dict": self.optimizer.state_dict(),
+                "net_config": self.net_config,
+                "batch_size": self.batch_size,
+                "lr": self.lr,
+                "learn_step": self.learn_step,
+                "gamma": self.gamma,
+                "tau": self.tau,
+                "mutation": self.mut,
+                "index": self.index,
+                "scores": self.scores,
+                "fitness": self.fitness,
+                "steps": self.steps,
+            },
+            path,
+            pickle_module=dill,
+        )
+
+    def loadCheckpoint(self, path):
+        """Loads saved agent properties and network weights from checkpoint.
+
+        :param path: Location to load checkpoint from
+        :type path: string
+        """
+        checkpoint = torch.load(path, pickle_module=dill)
+        self.net_config = checkpoint["net_config"]
+        if self.net_config["arch"] == "mlp":
+            self.actor = EvolvableMLP(**checkpoint["actor_init_dict"])
+            self.actor_target = EvolvableMLP(**checkpoint["actor_target_init_dict"])
+        elif self.net_config["arch"] == "cnn":
+            self.actor = EvolvableCNN(**checkpoint["actor_init_dict"])
+            self.actor_target = EvolvableCNN(**checkpoint["actor_target_init_dict"])
+        self.lr = checkpoint["lr"]
+        self.optimizer = optim.Adam(self.actor.parameters(), lr=self.lr)
+        self.actor.load_state_dict(checkpoint["actor_state_dict"])
+        self.actor_target.load_state_dict(checkpoint["actor_target_state_dict"])
+        self.optimizer.load_state_dict(checkpoint["optimizer_state_dict"])
+        self.batch_size = checkpoint["batch_size"]
+        self.learn_step = checkpoint["learn_step"]
+        self.gamma = checkpoint["gamma"]
+        self.tau = checkpoint["tau"]
+        self.mut = checkpoint["mutation"]
+        self.index = checkpoint["index"]
+        self.scores = checkpoint["scores"]
+        self.fitness = checkpoint["fitness"]
+        self.steps = checkpoint["steps"]
```

### Comparing `agilerl-0.1.8/agilerl/algorithms/ilql.py` & `agilerl-0.1.9/agilerl/algorithms/ilql.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,31 @@
-from collections import defaultdict
 import copy
 import math
+from collections import defaultdict
+from typing import Any, Callable, Optional, Tuple, Union
+
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.optim as optim
 from torch.nn import functional as F
 from tqdm import tqdm
-from typing import Any, Callable, Tuple, Union, Optional
+
 import wandb
-from agilerl.networks.evolvable_mlp import EvolvableMLP
-from agilerl.networks.evolvable_gpt import EvolvableGPT
 from agilerl.data.rl_data import DataPoint
-from agilerl.utils.sampling_utils import map_all_kvs, pad_sequence, update_kvs, process_logits, always_terminate
+from agilerl.networks.evolvable_gpt import EvolvableGPT
+from agilerl.networks.evolvable_mlp import EvolvableMLP
+from agilerl.utils.sampling_utils import (
+    always_terminate,
+    map_all_kvs,
+    pad_sequence,
+    process_logits,
+    update_kvs,
+)
+
 
 class ILQL(nn.Module):
     """The Implicit Language Q Learning algorithm class. ILQL paper: https://arxiv.org/pdf/2206.11871.pdf
 
     :param dataset: Language dataset to perform ILQL on
     :type dataset: torch.utils.data.Dataset
     :param net_config: Network configuration, defaults to GPT2 configuration
@@ -64,56 +73,57 @@
     :param weight_decay: weight decay for optimizer, defaults to 0.0
     :type weight_decay: float, optional
     :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
     :type device: str, optional
     """
 
     def __init__(
-            self,
-            dataset,
-            net_config={
-                'arch': 'gpt',
-                'vocab_size': 50257,
-                'n_layer': 12,
-                'n_embd': 768,
-                'n_head': 12,
-                'dim_feedfwd': 3072,
-                'block_size': 1024,
-                'activation': 'gelu',
-                'dropout': 0.1,
-                'layer_norm_eps': 1e-5,
-                'min_layers': 8,
-                'max_layers': 16,
-                'bias': True,
-            },
-            index=0,
-            batch_size=64,
-            lr=1e-5,
-            alpha=0.005,
-            beta=0.,
-            gamma=0.99,
-            tau=0.6,
-            mutation=None,
-            transition_weight=0.,
-            clip_weight=None,
-            value_max=None,
-            value_min=None,
-            detach_v=False,
-            detach_q=False,
-            detach_pi=False,
-            double_q=True,
-            per_token=True,
-            exp_weights=True,
-            dm_margin=0.,
-            cql_temp=1.,
-            weight_decay=0.,
-            device='cpu'):
-        super(ILQL, self).__init__()
+        self,
+        dataset,
+        net_config={
+            "arch": "gpt",
+            "vocab_size": 50257,
+            "n_layer": 12,
+            "n_embd": 768,
+            "n_head": 12,
+            "dim_feedfwd": 3072,
+            "block_size": 1024,
+            "activation": "gelu",
+            "dropout": 0.1,
+            "layer_norm_eps": 1e-5,
+            "min_layers": 8,
+            "max_layers": 16,
+            "bias": True,
+        },
+        index=0,
+        batch_size=64,
+        lr=1e-5,
+        alpha=0.005,
+        beta=0.0,
+        gamma=0.99,
+        tau=0.6,
+        mutation=None,
+        transition_weight=0.0,
+        clip_weight=None,
+        value_max=None,
+        value_min=None,
+        detach_v=False,
+        detach_q=False,
+        detach_pi=False,
+        double_q=True,
+        per_token=True,
+        exp_weights=True,
+        dm_margin=0.0,
+        cql_temp=1.0,
+        weight_decay=0.0,
+        device="cpu",
+    ):
+        super().__init__()
 
-        self.algo = 'ILQL'
+        self.algo = "ILQL"
         self.dataset = dataset
         self.net_config = net_config
         self.alpha = alpha
         self.gamma = gamma
         self.beta = beta
         self.transition_weight = transition_weight
         self.clip_weight = clip_weight
@@ -137,136 +147,129 @@
         self.index = index
         self.scores = []
         self.fitness = []
         self.steps = [0]
 
         # model
         self.model = EvolvableGPT(
-            n_layer=net_config['n_layer'],
-            vocab_size=net_config['vocab_size'],
-            n_embd=net_config['n_embd'],
-            n_head=net_config['n_head'],
-            dim_feedfwd=net_config['dim_feedfwd'],
-            block_size=net_config['block_size'],
-            dropout=net_config['dropout'],
-            activation=net_config['activation'],
-            layer_norm_eps=net_config['layer_norm_eps'],
-            min_layers=net_config['min_layers'],
-            max_layers=net_config['max_layers'],
-            bias=net_config['bias'],
-            device=self.device).to(
-            self.device)
+            n_layer=net_config["n_layer"],
+            vocab_size=net_config["vocab_size"],
+            n_embd=net_config["n_embd"],
+            n_head=net_config["n_head"],
+            dim_feedfwd=net_config["dim_feedfwd"],
+            block_size=net_config["block_size"],
+            dropout=net_config["dropout"],
+            activation=net_config["activation"],
+            layer_norm_eps=net_config["layer_norm_eps"],
+            min_layers=net_config["min_layers"],
+            max_layers=net_config["max_layers"],
+            bias=net_config["bias"],
+            device=self.device,
+        ).to(self.device)
         # lm policy
         self.actor = EvolvableGPT(
-            n_layer=net_config['n_layer'],
-            vocab_size=net_config['vocab_size'],
-            n_embd=net_config['n_embd'],
-            n_head=net_config['n_head'],
-            dim_feedfwd=net_config['dim_feedfwd'],
-            block_size=net_config['block_size'],
-            dropout=net_config['dropout'],
-            activation=net_config['activation'],
-            layer_norm_eps=net_config['layer_norm_eps'],
-            min_layers=net_config['min_layers'],
-            max_layers=net_config['max_layers'],
-            bias=net_config['bias'],
-            device=self.device).to(
-            self.device)
+            n_layer=net_config["n_layer"],
+            vocab_size=net_config["vocab_size"],
+            n_embd=net_config["n_embd"],
+            n_head=net_config["n_head"],
+            dim_feedfwd=net_config["dim_feedfwd"],
+            block_size=net_config["block_size"],
+            dropout=net_config["dropout"],
+            activation=net_config["activation"],
+            layer_norm_eps=net_config["layer_norm_eps"],
+            min_layers=net_config["min_layers"],
+            max_layers=net_config["max_layers"],
+            bias=net_config["bias"],
+            device=self.device,
+        ).to(self.device)
         # lm target
         self.actor_target = EvolvableGPT(
-            n_layer=net_config['n_layer'],
-            vocab_size=net_config['vocab_size'],
-            n_embd=net_config['n_embd'],
-            n_head=net_config['n_head'],
-            dim_feedfwd=net_config['dim_feedfwd'],
-            block_size=net_config['block_size'],
-            dropout=net_config['dropout'],
-            activation=net_config['activation'],
-            layer_norm_eps=net_config['layer_norm_eps'],
-            min_layers=net_config['min_layers'],
-            max_layers=net_config['max_layers'],
-            bias=net_config['bias'],
-            device=self.device).to(
-            self.device)
+            n_layer=net_config["n_layer"],
+            vocab_size=net_config["vocab_size"],
+            n_embd=net_config["n_embd"],
+            n_head=net_config["n_head"],
+            dim_feedfwd=net_config["dim_feedfwd"],
+            block_size=net_config["block_size"],
+            dropout=net_config["dropout"],
+            activation=net_config["activation"],
+            layer_norm_eps=net_config["layer_norm_eps"],
+            min_layers=net_config["min_layers"],
+            max_layers=net_config["max_layers"],
+            bias=net_config["bias"],
+            device=self.device,
+        ).to(self.device)
 
         self.copy_model_to_actor_target()
 
         # v and q networks
         self.v = EvolvableMLP(
-            num_inputs=net_config['n_embd'],
+            num_inputs=net_config["n_embd"],
             num_outputs=1,
-            hidden_size=[
-                net_config['n_embd'] * 2,
-                net_config['n_embd'] * 2],
-            device=self.device).to(
-            self.device)
+            hidden_size=[net_config["n_embd"] * 2, net_config["n_embd"] * 2],
+            device=self.device,
+        ).to(self.device)
         self.q = EvolvableMLP(
-            num_inputs=net_config['n_embd'],
+            num_inputs=net_config["n_embd"],
             num_outputs=self.dataset.tokenizer.num_tokens(),
-            hidden_size=[
-                net_config['n_embd'] * 2,
-                net_config['n_embd'] * 2],
-            device=self.device).to(
-            self.device)
+            hidden_size=[net_config["n_embd"] * 2, net_config["n_embd"] * 2],
+            device=self.device,
+        ).to(self.device)
         self.target_q = EvolvableMLP(
-            num_inputs=net_config['n_embd'],
+            num_inputs=net_config["n_embd"],
             num_outputs=self.dataset.tokenizer.num_tokens(),
-            hidden_size=[
-                net_config['n_embd'] * 2,
-                net_config['n_embd'] * 2],
-            device=self.device).to(
-            self.device)
+            hidden_size=[net_config["n_embd"] * 2, net_config["n_embd"] * 2],
+            device=self.device,
+        ).to(self.device)
         self.target_q.load_state_dict(self.q.state_dict())
 
         if self.double_q:
             self.q2 = EvolvableMLP(
-                num_inputs=net_config['n_embd'],
+                num_inputs=net_config["n_embd"],
                 num_outputs=self.dataset.tokenizer.num_tokens(),
-                hidden_size=[
-                    net_config['n_embd'] * 2,
-                    net_config['n_embd'] * 2],
-                device=self.device).to(
-                self.device)
+                hidden_size=[net_config["n_embd"] * 2, net_config["n_embd"] * 2],
+                device=self.device,
+            ).to(self.device)
             self.target_q2 = EvolvableMLP(
-                num_inputs=net_config['n_embd'],
+                num_inputs=net_config["n_embd"],
                 num_outputs=self.dataset.tokenizer.num_tokens(),
-                hidden_size=[
-                    net_config['n_embd'] * 2,
-                    net_config['n_embd'] * 2],
-                device=self.device).to(
-                self.device)
+                hidden_size=[net_config["n_embd"] * 2, net_config["n_embd"] * 2],
+                device=self.device,
+            ).to(self.device)
             self.target_q2.load_state_dict(self.q2.state_dict())
 
         self.pi = EvolvableMLP(
-            num_inputs=net_config['n_embd'],
+            num_inputs=net_config["n_embd"],
             num_outputs=self.dataset.tokenizer.num_tokens(),
-            hidden_size=[
-                net_config['n_embd'] * 2,
-                net_config['n_embd'] * 2],
-            device=self.device).to(
-            self.device)
+            hidden_size=[net_config["n_embd"] * 2, net_config["n_embd"] * 2],
+            device=self.device,
+        ).to(self.device)
 
         self.optimizer = optim.AdamW(
-            self.parameters(), lr=self.lr, weight_decay=self.weight_decay)
-        
+            self.parameters(), lr=self.lr, weight_decay=self.weight_decay
+        )
+
     def copy_model_to_actor_target(self):
         self.actor.load_state_dict(self.model.state_dict())
         self.actor_target.load_state_dict(self.model.state_dict())
 
-    def forward(self,
-                tokens: torch.Tensor,
-                state_idxs: torch.Tensor,
-                action_idxs: torch.Tensor,
-                attn_mask: Optional[torch.Tensor] = None,
-                prefix_embs: Optional[torch.Tensor] = None,
-                prefix_attn_mask: Optional[torch.Tensor]=None,
-                remove_prefix_position_embs: bool=False,
-                qv_kwargs=None, policy_kwargs=None, target_kwargs=None,
-                skip_policy_on_train: bool = False,
-                detach_full_policy: bool = False):
+    def forward(
+        self,
+        tokens: torch.Tensor,
+        state_idxs: torch.Tensor,
+        action_idxs: torch.Tensor,
+        attn_mask: Optional[torch.Tensor] = None,
+        prefix_embs: Optional[torch.Tensor] = None,
+        prefix_attn_mask: Optional[torch.Tensor] = None,
+        remove_prefix_position_embs: bool = False,
+        qv_kwargs=None,
+        policy_kwargs=None,
+        target_kwargs=None,
+        skip_policy_on_train: bool = False,
+        detach_full_policy: bool = False,
+    ):
         """Forward pass through transformers.
 
         :param tokens: Tokens to input to model
         :type tokens: torch.Tensor
         :param state_idxs: State indexes
         :type state_idxs: torch.Tensor
         :param action_idxs: Action indexes
@@ -283,304 +286,441 @@
         if qv_kwargs is None:
             qv_kwargs = {}
         if target_kwargs is None:
             target_kwargs = {}
         if policy_kwargs is None:
             policy_kwargs = {}
         if prefix_embs is None:
-            prefix_embs = torch.empty((tokens.shape[0], 0, self.net_config['n_embd'])).to(self.device)
+            prefix_embs = torch.empty(
+                (tokens.shape[0], 0, self.net_config["n_embd"])
+            ).to(self.device)
             prefix_t = prefix_embs.shape[1]
         else:
             prefix_t = 0
         set_pos_ids = prefix_attn_mask is not None
         if prefix_attn_mask is not None and attn_mask is not None:
             input_attn_mask = torch.cat((prefix_attn_mask, attn_mask), dim=1)
         else:
             input_attn_mask = None
-        position_ids = torch.cumsum(input_attn_mask, dim=1)-1 if set_pos_ids else None
+        position_ids = torch.cumsum(input_attn_mask, dim=1) - 1 if set_pos_ids else None
 
         target_prefix_embs = prefix_embs.clone()
         policy_prefix_embs = prefix_embs.clone()
 
         if remove_prefix_position_embs:
-            prefix_embs -= self.model.transformer.wpe(position_ids[:, :prefix_embs.shape[1]])
-            target_prefix_embs -= self.actor_target.transformer.wpe(position_ids[:, :prefix_embs.shape[1]])
+            prefix_embs -= self.model.transformer.wpe(
+                position_ids[:, : prefix_embs.shape[1]]
+            )
+            target_prefix_embs -= self.actor_target.transformer.wpe(
+                position_ids[:, : prefix_embs.shape[1]]
+            )
 
-        input_embeddings = torch.cat((prefix_embs, self.model.transformer.wte(tokens)), dim=1)
-        target_input_embeddings = torch.cat((target_prefix_embs, self.actor_target.transformer.wte(tokens)), dim=1)
+        input_embeddings = torch.cat(
+            (prefix_embs, self.model.transformer.wte(tokens)), dim=1
+        )
+        target_input_embeddings = torch.cat(
+            (target_prefix_embs, self.actor_target.transformer.wte(tokens)), dim=1
+        )
 
         # Model forward passes
-        model_outputs, model_hidden_states, model_past_key_values, model_loss = self.model(
-            tok_emb=input_embeddings, attn_mask=input_attn_mask, pos=position_ids, **qv_kwargs)
+        (
+            model_outputs,
+            model_hidden_states,
+            model_past_key_values,
+            model_loss,
+        ) = self.model(
+            tok_emb=input_embeddings,
+            attn_mask=input_attn_mask,
+            pos=position_ids,
+            **qv_kwargs
+        )
         hidden_states = model_hidden_states[-1][:, prefix_t:, :]
 
         with torch.no_grad():
-            target_outputs, target_hidden_states, target_past_key_values, target_loss = self.actor_target(
-                tok_emb=target_input_embeddings, attn_mask=input_attn_mask, pos=position_ids, **target_kwargs)
+            (
+                target_outputs,
+                target_hidden_states,
+                target_past_key_values,
+                target_loss,
+            ) = self.actor_target(
+                tok_emb=target_input_embeddings,
+                attn_mask=input_attn_mask,
+                pos=position_ids,
+                **target_kwargs
+            )
         target_hidden_states = target_hidden_states[-1][:, prefix_t:, :]
 
         # Prepare policy inputs
         if skip_policy_on_train and self.training:
             policy_outputs = model_outputs
             policy_hidden_states = hidden_states
             policy_past_key_values = model_past_key_values
         else:
             if remove_prefix_position_embs:
-                policy_prefix_embs -= self.actor.transformer.wpe(position_ids[:, :prefix_embs.shape[1]])
-            policy_input_embeddings = torch.cat((policy_prefix_embs, self.actor.transformer.wte(tokens)), dim=1)
+                policy_prefix_embs -= self.actor.transformer.wpe(
+                    position_ids[:, : prefix_embs.shape[1]]
+                )
+            policy_input_embeddings = torch.cat(
+                (policy_prefix_embs, self.actor.transformer.wte(tokens)), dim=1
+            )
             if detach_full_policy:
                 with torch.no_grad():
-                    policy_outputs, policy_hidden_states, policy_past_key_values, policy_loss = self.actor(
-                        tok_emb=policy_input_embeddings, attn_mask=input_attn_mask, pos=position_ids, **policy_kwargs)
+                    (
+                        policy_outputs,
+                        policy_hidden_states,
+                        policy_past_key_values,
+                        policy_loss,
+                    ) = self.actor(
+                        tok_emb=policy_input_embeddings,
+                        attn_mask=input_attn_mask,
+                        pos=position_ids,
+                        **policy_kwargs
+                    )
             else:
-                policy_outputs, policy_hidden_states, policy_past_key_values, policy_loss = self.actor(
-                    tok_emb=policy_input_embeddings, attn_mask=input_attn_mask, pos=position_ids, **policy_kwargs)
+                (
+                    policy_outputs,
+                    policy_hidden_states,
+                    policy_past_key_values,
+                    policy_loss,
+                ) = self.actor(
+                    tok_emb=policy_input_embeddings,
+                    attn_mask=input_attn_mask,
+                    pos=position_ids,
+                    **policy_kwargs
+                )
             policy_hidden_states = policy_hidden_states[-1][:, prefix_t:, :]
 
-        all_model_outputs = {'qv_model_outputs': {'past_key_values': model_past_key_values},
-                             'policy_model_outputs': {'past_key_values': policy_past_key_values},
-                             'target_model_outputs':  {'past_key_values': target_past_key_values}}
-        all_hidden_states = {'qv_hidden_states': model_hidden_states,
-                             'policy_hidden_states': target_hidden_states,
-                             'target_hidden_states': policy_hidden_states}
+        all_model_outputs = {
+            "qv_model_outputs": {"past_key_values": model_past_key_values},
+            "policy_model_outputs": {"past_key_values": policy_past_key_values},
+            "target_model_outputs": {"past_key_values": target_past_key_values},
+        }
+        all_hidden_states = {
+            "qv_hidden_states": model_hidden_states,
+            "policy_hidden_states": target_hidden_states,
+            "target_hidden_states": policy_hidden_states,
+        }
 
         state_hidden_states = torch.gather(
-            input=hidden_states, dim=1, index=state_idxs.unsqueeze(2).repeat(
-                1, 1, self.net_config['n_embd']))
+            input=hidden_states,
+            dim=1,
+            index=state_idxs.unsqueeze(2).repeat(1, 1, self.net_config["n_embd"]),
+        )
         action_hidden_states = torch.gather(
-            input=hidden_states, dim=1, index=action_idxs.unsqueeze(2).repeat(
-                1, 1, self.net_config['n_embd']))
+            input=hidden_states,
+            dim=1,
+            index=action_idxs.unsqueeze(2).repeat(1, 1, self.net_config["n_embd"]),
+        )
         action_target_hidden_states = torch.gather(
-            input=target_hidden_states, dim=1, index=action_idxs.unsqueeze(2).repeat(
-                1, 1, self.net_config['n_embd']))
-        vs = self.v(state_hidden_states.detach()
-                    if self.detach_v else state_hidden_states).squeeze(2)
-        qs = self.q(action_hidden_states.detach()
-                    if self.detach_q else action_hidden_states)
+            input=target_hidden_states,
+            dim=1,
+            index=action_idxs.unsqueeze(2).repeat(1, 1, self.net_config["n_embd"]),
+        )
+        vs = self.v(
+            state_hidden_states.detach() if self.detach_v else state_hidden_states
+        ).squeeze(2)
+        qs = self.q(
+            action_hidden_states.detach() if self.detach_q else action_hidden_states
+        )
         if self.double_q:
-            qs2 = self.q2(action_hidden_states.detach()
-                          if self.detach_q else action_hidden_states)
+            qs2 = self.q2(
+                action_hidden_states.detach() if self.detach_q else action_hidden_states
+            )
         with torch.no_grad():
             target_qs = self.target_q(action_target_hidden_states)
             if self.double_q:
                 target_qs2 = self.target_q2(action_target_hidden_states)
         if skip_policy_on_train and self.training and self.actor is not None:
             logits = torch.zeros(
-                (policy_hidden_states.shape[0],
-                 policy_hidden_states.shape[1],
-                 self.dataset.tokenizer.num_tokens(),
-                 )).to(
-                self.device)
+                (
+                    policy_hidden_states.shape[0],
+                    policy_hidden_states.shape[1],
+                    self.dataset.tokenizer.num_tokens(),
+                )
+            ).to(self.device)
         else:
             if detach_full_policy:
                 with torch.no_grad():
-                    logits = self.pi(policy_hidden_states.detach(
-                    ) if self.detach_pi else policy_hidden_states)
+                    logits = self.pi(
+                        policy_hidden_states.detach()
+                        if self.detach_pi
+                        else policy_hidden_states
+                    )
             else:
-                logits = self.pi(policy_hidden_states.detach()
-                                 if self.detach_pi else policy_hidden_states)
+                logits = self.pi(
+                    policy_hidden_states.detach()
+                    if self.detach_pi
+                    else policy_hidden_states
+                )
         return {
-            'model_outputs': all_model_outputs,
-            'hidden_states': all_hidden_states,
-            'vs': vs,
-            'target_vs': vs,
-            'qs': (
+            "model_outputs": all_model_outputs,
+            "hidden_states": all_hidden_states,
+            "vs": vs,
+            "target_vs": vs,
+            "qs": (
                 qs,
                 qs2,
-            ) if self.double_q else qs,
-            'target_qs': self.clip_values(
-                torch.minimum(
-                    target_qs,
-                    target_qs2) if self.double_q else target_qs),
-            'logits': logits,
+            )
+            if self.double_q
+            else qs,
+            "target_qs": self.clip_values(
+                torch.minimum(target_qs, target_qs2) if self.double_q else target_qs
+            ),
+            "logits": logits,
         }
 
     def clip_values(self, values):
         if self.value_min is not None or self.value_max is not None:
             return torch.clip(values, self.value_min, self.value_max)
         return values
 
     def get_downstream_rs(self, rs, gamma):
-        gamma_row = torch.cumprod(torch.full(
-            rs.shape, gamma).to(self.device), dim=1)
-        gamma_tensor = torch.triu(
-            gamma_row.unsqueeze(1) / gamma_row.unsqueeze(2))
+        gamma_row = torch.cumprod(torch.full(rs.shape, gamma).to(self.device), dim=1)
+        gamma_tensor = torch.triu(gamma_row.unsqueeze(1) / gamma_row.unsqueeze(2))
         return (gamma_tensor * rs.unsqueeze(1)).sum(dim=2)
 
-    def get_weights(self,
-                    tokens: torch.Tensor,
-                    vs: torch.Tensor,
-                    qs: Optional[torch.Tensor],
-                    state_idxs: torch.Tensor,
-                    action_idxs: torch.Tensor,
-                    terminals: torch.Tensor):
-        weights = torch.full(
-            tokens.shape, self.transition_weight).to(self.device)
+    def get_weights(
+        self,
+        tokens: torch.Tensor,
+        vs: torch.Tensor,
+        qs: Optional[torch.Tensor],
+        state_idxs: torch.Tensor,
+        action_idxs: torch.Tensor,
+        terminals: torch.Tensor,
+    ):
+        weights = torch.full(tokens.shape, self.transition_weight).to(self.device)
         if self.exp_weights:
             w_values = torch.exp(self.beta * (qs - vs))
         else:
             # w_values = ((qs - vs) > 0.0).float()
             adv_sign = ((qs - vs) > 0.0).float()
             w_values = self.beta * adv_sign + (1 - self.beta) * (1 - adv_sign)
         if action_idxs.shape[1] == 0:
             n = torch.zeros((tokens.shape[0],)).long().to(self.device)
         else:
             n = torch.argmax(action_idxs, dim=1) + 1
         for i in range(tokens.shape[0]):
             weights[i] = torch.scatter(
-                weights[i], dim=0, index=action_idxs[i, :n[i]], src=w_values[i, :n[i]])
+                weights[i], dim=0, index=action_idxs[i, : n[i]], src=w_values[i, : n[i]]
+            )
         if self.clip_weight is not None:
             weights = torch.clip(weights, max=self.clip_weight)
         return weights
 
     def awac_loss(self, tokens, attn_mask, logits, w):
         w = w.detach()
         losses = F.cross_entropy(
-            logits[:, :-1, :].reshape(-1, logits.shape[-1]), tokens[:, 1:].reshape(-1), reduction='none')
+            logits[:, :-1, :].reshape(-1, logits.shape[-1]),
+            tokens[:, 1:].reshape(-1),
+            reduction="none",
+        )
         losses = losses.reshape(tokens.shape[0], tokens.shape[1] - 1)
         return (losses * w[:, :-1] * attn_mask[:, 1:]).sum() / attn_mask[:, 1:].sum()
 
     def get_v_loss(self, vs, target_qs, terminals):
         target_qs = target_qs.detach()
-        return (((target_qs >= vs).int() * self.tau * (target_qs - vs)**2 + (target_qs < vs).int() * (1 - self.tau)
-                * (target_qs - vs)**2) * (1 - terminals[:, :-1])).sum() / max((1 - terminals[:, :-1]).sum().item(), 1.0)
+        return (
+            (
+                (target_qs >= vs).int() * self.tau * (target_qs - vs) ** 2
+                + (target_qs < vs).int() * (1 - self.tau) * (target_qs - vs) ** 2
+            )
+            * (1 - terminals[:, :-1])
+        ).sum() / max((1 - terminals[:, :-1]).sum().item(), 1.0)
 
     def get_q_loss(self, vns, qs, rs, gamma, terminals):
         vns = vns.detach()
         if self.double_q:
             q1, q2 = qs
-            l1 = ((((1 - terminals[:, 1:]) * vns * gamma + rs - q1) ** 2) * (1 - \
-                  terminals[:, :-1])).sum() / max((1 - terminals[:, :-1]).sum().item(), 1.0)
-            l2 = ((((1 - terminals[:, 1:]) * vns * gamma + rs - q2) ** 2) * (1 - \
-                  terminals[:, :-1])).sum() / max((1 - terminals[:, :-1]).sum().item(), 1.0)
+            l1 = (
+                (((1 - terminals[:, 1:]) * vns * gamma + rs - q1) ** 2)
+                * (1 - terminals[:, :-1])
+            ).sum() / max((1 - terminals[:, :-1]).sum().item(), 1.0)
+            l2 = (
+                (((1 - terminals[:, 1:]) * vns * gamma + rs - q2) ** 2)
+                * (1 - terminals[:, :-1])
+            ).sum() / max((1 - terminals[:, :-1]).sum().item(), 1.0)
             return l1 + l2
-        return ((((1 - terminals[:, 1:]) * vns * gamma + rs - qs) ** 2) * (1 - \
-                terminals[:, :-1])).sum() / max((1 - terminals[:, :-1]).sum().item(), 1.0)
+        return (
+            (((1 - terminals[:, 1:]) * vns * gamma + rs - qs) ** 2)
+            * (1 - terminals[:, :-1])
+        ).sum() / max((1 - terminals[:, :-1]).sum().item(), 1.0)
 
     def get_cql_loss(self, qs, action_tokens, terminals):
         n = (1 - terminals[:, :-1]).sum()
         if self.double_q:
             q1, q2 = qs
             b, t, d = q1.shape
-            t1 = F.cross_entropy(q1.reshape(-1, d) / self.cql_temp,
-                                 action_tokens.reshape(-1),
-                                 reduction='none').reshape(b, t) * (1 - terminals[:,:-1])
-
-            t2 = F.cross_entropy(q2.reshape(-1, d) / self.cql_temp, 
-                                 action_tokens.reshape(-1), 
-                                 reduction='none').reshape(b, t) * (1 - terminals[:,:-1])
+            t1 = F.cross_entropy(
+                q1.reshape(-1, d) / self.cql_temp,
+                action_tokens.reshape(-1),
+                reduction="none",
+            ).reshape(b, t) * (1 - terminals[:, :-1])
+
+            t2 = F.cross_entropy(
+                q2.reshape(-1, d) / self.cql_temp,
+                action_tokens.reshape(-1),
+                reduction="none",
+            ).reshape(b, t) * (1 - terminals[:, :-1])
             return ((t1) + (t2)).sum() / max(n.item(), 1.0)
         b, t, d = qs.shape
-        return (F.cross_entropy(qs.reshape(-1, d) / self.cql_temp, action_tokens.reshape(-1),
-                reduction='none').reshape(b, t) * (1 - terminals[:, :-1])).sum() / max(n.item(), 1.0)
+        return (
+            F.cross_entropy(
+                qs.reshape(-1, d) / self.cql_temp,
+                action_tokens.reshape(-1),
+                reduction="none",
+            ).reshape(b, t)
+            * (1 - terminals[:, :-1])
+        ).sum() / max(n.item(), 1.0)
 
     def get_dm_loss(self, qs, data_qs, terminals, margin):
         n = (1 - terminals[:, :-1]).sum()
         if self.double_q:
             q1, q2 = qs
             data_q1, data_q2 = data_qs
-            return (((torch.max(q1 - data_q1.unsqueeze(-1) + margin,
-                                torch.tensor(0.0).to(self.device)) ** 2).sum(
-                dim=-1) * (1 - terminals[:,:-1])) + ((torch.max(q2 - data_q2.unsqueeze(-1) + margin, 
-                                                                torch.tensor(0.0).to(self.device)) ** 2).sum(
-                dim=-1) * (1 - terminals[:,:-1]))).sum() / max(n.item(), 1.0)
-        return ((torch.max(qs - data_qs.unsqueeze(-1) + margin, torch.tensor(0.0).to(self.device))
-                ** 2).sum(dim=-1) * (1 - terminals[:, :-1])).sum() / max(n.item(), 1.0)
+            return (
+                (
+                    (
+                        torch.max(
+                            q1 - data_q1.unsqueeze(-1) + margin,
+                            torch.tensor(0.0).to(self.device),
+                        )
+                        ** 2
+                    ).sum(dim=-1)
+                    * (1 - terminals[:, :-1])
+                )
+                + (
+                    (
+                        torch.max(
+                            q2 - data_q2.unsqueeze(-1) + margin,
+                            torch.tensor(0.0).to(self.device),
+                        )
+                        ** 2
+                    ).sum(dim=-1)
+                    * (1 - terminals[:, :-1])
+                )
+            ).sum() / max(n.item(), 1.0)
+        return (
+            (
+                torch.max(
+                    qs - data_qs.unsqueeze(-1) + margin,
+                    torch.tensor(0.0).to(self.device),
+                )
+                ** 2
+            ).sum(dim=-1)
+            * (1 - terminals[:, :-1])
+        ).sum() / max(n.item(), 1.0)
 
     def prepare_inputs(self, items):
         if isinstance(items, dict):
             return items
         return to(self.dataset.collate(items, self.device), self.device)
 
-    def get_qvs(self, items,
-                prefix_embs: Optional[torch.Tensor] = None,
-                prefix_attn_mask: Optional[torch.Tensor] = None,
-                remove_prefix_position_embs: bool = False,
-                qv_kwargs=None, policy_kwargs=None, target_kwargs=None,
-                **kwargs):
+    def get_qvs(
+        self,
+        items,
+        prefix_embs: Optional[torch.Tensor] = None,
+        prefix_attn_mask: Optional[torch.Tensor] = None,
+        remove_prefix_position_embs: bool = False,
+        qv_kwargs=None,
+        policy_kwargs=None,
+        target_kwargs=None,
+        **kwargs
+    ):
         prepared_inputs = self.prepare_inputs(items)
-        tokens, attn_mask = prepared_inputs['tokens'], prepared_inputs['attn_mask']
-        s_idx, a_idx = prepared_inputs['state_idxs'], prepared_inputs['action_idxs']
-        rs, terminals = prepared_inputs['rewards'], prepared_inputs['terminals']
-        self_outputs = self(tokens, s_idx, a_idx, attn_mask,
-                            prefix_embs,
-                            **kwargs)
-        model_outputs, vs, qs = self_outputs['model_outputs'], self_outputs['vs'], self_outputs['qs']
-        target_qs, logits = self_outputs['target_qs'], self_outputs['logits']
+        tokens, attn_mask = prepared_inputs["tokens"], prepared_inputs["attn_mask"]
+        s_idx, a_idx = prepared_inputs["state_idxs"], prepared_inputs["action_idxs"]
+        rs, terminals = prepared_inputs["rewards"], prepared_inputs["terminals"]
+        self_outputs = self(tokens, s_idx, a_idx, attn_mask, prefix_embs, **kwargs)
+        model_outputs, vs, qs = (
+            self_outputs["model_outputs"],
+            self_outputs["vs"],
+            self_outputs["qs"],
+        )
+        target_qs, logits = self_outputs["target_qs"], self_outputs["logits"]
         vt = vs[:, :-1]
         vtp1 = vs[:, 1:]
         select_tokens = torch.gather(tokens[:, 1:], dim=1, index=a_idx)
         cql_term = self.get_cql_loss(qs, select_tokens, terminals)
         full_qs = qs
         if self.double_q:
             q1, q2 = qs
-            q1 = torch.gather(
-                q1, dim=2, index=select_tokens.unsqueeze(2)).squeeze(2)
-            q2 = torch.gather(
-                q2, dim=2, index=select_tokens.unsqueeze(2)).squeeze(2)
+            q1 = torch.gather(q1, dim=2, index=select_tokens.unsqueeze(2)).squeeze(2)
+            q2 = torch.gather(q2, dim=2, index=select_tokens.unsqueeze(2)).squeeze(2)
             # tok_seq = [self.dataset.tokenizer.id_to_token(
             #   token) for token in select_tokens[0].detach().cpu().tolist()][:(1-terminals[0, :-1]).sum()]
             # max_q_seq = torch.max(q1, q2)[0, :(1-terminals[0, :-1]).sum()].detach().cpu().tolist()
-            # print(self.dataset.tokenizer.decode(tokens[0, :][:attn_mask[0, :].sum().long()].tolist(), 
+            # print(self.dataset.tokenizer.decode(tokens[0, :][:attn_mask[0, :].sum().long()].tolist(),
             #   clean_up_tokenization_spaces=False))
             # print(list(zip(tok_seq, max_q_seq)))
             # print(rs)
-            qs = (q1, q2,)
+            qs = (
+                q1,
+                q2,
+            )
         else:
-            qs = torch.gather(
-                qs, dim=2, index=select_tokens.unsqueeze(2)).squeeze(2)
+            qs = torch.gather(qs, dim=2, index=select_tokens.unsqueeze(2)).squeeze(2)
         dm_term = self.get_dm_loss(full_qs, qs, terminals, self.dm_margin)
         target_qs = torch.gather(
-            target_qs, dim=2, index=select_tokens.unsqueeze(2)).squeeze(2)
+            target_qs, dim=2, index=select_tokens.unsqueeze(2)
+        ).squeeze(2)
         with torch.no_grad():
-            weights = self.get_weights(
-                tokens, vt, target_qs, s_idx, a_idx, terminals)
+            weights = self.get_weights(tokens, vt, target_qs, s_idx, a_idx, terminals)
         return {
-            'tokens': tokens,
-            'attn_mask': attn_mask,
-            'model_outputs': model_outputs,
-            'vs': vt,
-            'qs': qs,
-            'vns': vtp1,
-            'target_vs': vt,
-            'target_qs': target_qs,
-            'target_vns': vtp1,
-            'rs': rs,
-            'terminals': terminals,
-            'logits': logits,
-            'weights': weights,
-            'cql_term': cql_term,
-            'dm_term': dm_term,
+            "tokens": tokens,
+            "attn_mask": attn_mask,
+            "model_outputs": model_outputs,
+            "vs": vt,
+            "qs": qs,
+            "vns": vtp1,
+            "target_vs": vt,
+            "target_qs": target_qs,
+            "target_vns": vtp1,
+            "rs": rs,
+            "terminals": terminals,
+            "logits": logits,
+            "weights": weights,
+            "cql_term": cql_term,
+            "dm_term": dm_term,
         }
 
-    def get_loss(self,
-                 items,
-                 awac_weight=0.0,
-                 v_loss_weight=0.0,
-                 q_loss_weight=0.0,
-                 cql_loss_weight=0.0,
-                 dm_loss_weight=0.0,
-                 mc_returns=False):
+    def get_loss(
+        self,
+        items,
+        awac_weight=0.0,
+        v_loss_weight=0.0,
+        q_loss_weight=0.0,
+        cql_loss_weight=0.0,
+        dm_loss_weight=0.0,
+        mc_returns=False,
+    ):
         prepared_inputs = self.prepare_inputs(items)
-        a_idx = prepared_inputs['action_idxs']
-        get_qvs_outputs = self.get_qvs(items,
-                                       qv_kwargs={'output_attentions': True},
-                                       policy_kwargs={
-                                           'output_attentions': True},
-                                       target_kwargs={
-                                           'output_attentions': True},
-                                       skip_policy_on_train=(
-                                           awac_weight == 0.0),
-                                       )
-        tokens, attn_mask, _ = get_qvs_outputs[
-            'tokens'], get_qvs_outputs['attn_mask'], get_qvs_outputs['model_outputs']
-        vs, qs = get_qvs_outputs['vs'], get_qvs_outputs['qs']
-        vns, target_qs, rs = get_qvs_outputs['vns'], get_qvs_outputs['target_qs'], get_qvs_outputs['rs']
-        terminals, logits, weights = get_qvs_outputs[
-            'terminals'], get_qvs_outputs['logits'], get_qvs_outputs['weights']
+        a_idx = prepared_inputs["action_idxs"]
+        get_qvs_outputs = self.get_qvs(
+            items,
+            qv_kwargs={"output_attentions": True},
+            policy_kwargs={"output_attentions": True},
+            target_kwargs={"output_attentions": True},
+            skip_policy_on_train=(awac_weight == 0.0),
+        )
+        tokens, attn_mask, _ = (
+            get_qvs_outputs["tokens"],
+            get_qvs_outputs["attn_mask"],
+            get_qvs_outputs["model_outputs"],
+        )
+        vs, qs = get_qvs_outputs["vs"], get_qvs_outputs["qs"]
+        vns, target_qs, rs = (
+            get_qvs_outputs["vns"],
+            get_qvs_outputs["target_qs"],
+            get_qvs_outputs["rs"],
+        )
+        terminals, logits, weights = (
+            get_qvs_outputs["terminals"],
+            get_qvs_outputs["logits"],
+            get_qvs_outputs["weights"],
+        )
 
         logs = {}
         transformer_logs = {}
         # transformer_logs['qv_transformer_logs'] = get_transformer_logs(
         #     model_outputs['qv_model_outputs'].attentions, self.model, attn_mask)
         # if self.actor is not None and (not (self.training and awac_weight == 0.0)):
         #     transformer_logs['policy_transformer_logs'] = get_transformer_logs(
@@ -591,232 +731,372 @@
         n = (1 - terminals[:, :-1]).sum().item()
         rs_downstream = self.get_downstream_rs(rs, self.gamma)
         if mc_returns:
             v_loss = self.get_v_loss(vs, rs_downstream, terminals)
         else:
             v_loss = self.get_v_loss(vs, target_qs, terminals)
         q_loss = self.get_q_loss(vns, qs, rs, self.gamma, terminals)
-        cql_loss = get_qvs_outputs['cql_term']
-        dm_loss = get_qvs_outputs['dm_term']
+        cql_loss = get_qvs_outputs["cql_term"]
+        dm_loss = get_qvs_outputs["dm_term"]
         token_loss = self.awac_loss(tokens, attn_mask, logits, weights)
-        logs['token_loss'] = (token_loss.item(), n)
-        loss = awac_weight * token_loss + v_loss_weight * v_loss + q_loss_weight * \
-            q_loss + cql_loss_weight * cql_loss + dm_loss_weight * dm_loss
-        logs['v_loss'] = (v_loss.item(), n)
-        logs['q_loss'] = (q_loss.item(), n)
-        logs['cql_loss'] = (cql_loss.item(), n)
-        logs['dm_loss'] = (dm_loss.item(), n)
-        advantages = sum([((target_qs[i] - vs[i])[:(1 - terminals[i, :-1]).sum().long().item()]
-                           ).detach().cpu().tolist() for i in range(tokens.shape[0])], [])
+        logs["token_loss"] = (token_loss.item(), n)
+        loss = (
+            awac_weight * token_loss
+            + v_loss_weight * v_loss
+            + q_loss_weight * q_loss
+            + cql_loss_weight * cql_loss
+            + dm_loss_weight * dm_loss
+        )
+        logs["v_loss"] = (v_loss.item(), n)
+        logs["q_loss"] = (q_loss.item(), n)
+        logs["cql_loss"] = (cql_loss.item(), n)
+        logs["dm_loss"] = (dm_loss.item(), n)
+        advantages = sum(
+            [
+                ((target_qs[i] - vs[i])[: (1 - terminals[i, :-1]).sum().long().item()])
+                .detach()
+                .cpu()
+                .tolist()
+                for i in range(tokens.shape[0])
+            ],
+            [],
+        )
         if self.double_q:
             q1, q2 = qs
-            logs['q1_avg'] = ((q1 * (1 - terminals[:, :-1])
-                               ).sum().item() / max(n, 1), n)
-            logs['q1_var'] = (((((q1 - logs['q1_avg'][0]) ** 2) *
-                              (1 - terminals[:, :-1])).sum() / max(n, 1)).item(), 1)
-            logs['q2_avg'] = ((q2 * (1 - terminals[:, :-1])
-                               ).sum().item() / max(n, 1), n)
-            logs['q2_var'] = (((((q2 - logs['q2_avg'][0]) ** 2) *
-                              (1 - terminals[:, :-1])).sum() / max(n, 1)).item(), 1)
+            logs["q1_avg"] = (
+                (q1 * (1 - terminals[:, :-1])).sum().item() / max(n, 1),
+                n,
+            )
+            logs["q1_var"] = (
+                (
+                    (((q1 - logs["q1_avg"][0]) ** 2) * (1 - terminals[:, :-1])).sum()
+                    / max(n, 1)
+                ).item(),
+                1,
+            )
+            logs["q2_avg"] = (
+                (q2 * (1 - terminals[:, :-1])).sum().item() / max(n, 1),
+                n,
+            )
+            logs["q2_var"] = (
+                (
+                    (((q2 - logs["q2_avg"][0]) ** 2) * (1 - terminals[:, :-1])).sum()
+                    / max(n, 1)
+                ).item(),
+                1,
+            )
         else:
-            logs['q_avg'] = ((qs * (1 - terminals[:, :-1])
-                              ).sum().item() / max(n, 1), n)
-            logs['q_var'] = (((((qs - logs['q_avg'][0]) ** 2) *
-                             (1 - terminals[:, :-1])).sum() / max(n, 1)).item(), 1)
-        logs['v_avg'] = ((vs * (1 - terminals[:, :-1])
-                          ).sum().item() / max(n, 1), n)
-        logs['v_var'] = (((((vs - logs['v_avg'][0]) ** 2) *
-                         (1 - terminals[:, :-1])).sum() / max(n, 1)).item(), 1)
+            logs["q_avg"] = ((qs * (1 - terminals[:, :-1])).sum().item() / max(n, 1), n)
+            logs["q_var"] = (
+                (
+                    (((qs - logs["q_avg"][0]) ** 2) * (1 - terminals[:, :-1])).sum()
+                    / max(n, 1)
+                ).item(),
+                1,
+            )
+        logs["v_avg"] = ((vs * (1 - terminals[:, :-1])).sum().item() / max(n, 1), n)
+        logs["v_var"] = (
+            (
+                (((vs - logs["v_avg"][0]) ** 2) * (1 - terminals[:, :-1])).sum()
+                / max(n, 1)
+            ).item(),
+            1,
+        )
         act_weights = torch.gather(weights, dim=1, index=a_idx)
-        logs['act_weight_avg'] = (
-            ((act_weights * (1 - terminals[:, :-1])).sum() / max(n, 1)).item(), n)
-        logs['transformer'] = transformer_logs
+        logs["act_weight_avg"] = (
+            ((act_weights * (1 - terminals[:, :-1])).sum() / max(n, 1)).item(),
+            n,
+        )
+        logs["transformer"] = transformer_logs
 
         def postproc_f(x):
-            return x.update({'loss': awac_weight * x['token_loss'] + q_loss_weight * x[
-                'q_loss'] + v_loss_weight * x['v_loss'] + cql_loss_weight * x[
-                    'cql_loss'] + dm_loss_weight * x['dm_loss']})
+            return x.update(
+                {
+                    "loss": awac_weight * x["token_loss"]
+                    + q_loss_weight * x["q_loss"]
+                    + v_loss_weight * x["v_loss"]
+                    + cql_loss_weight * x["cql_loss"]
+                    + dm_loss_weight * x["dm_loss"]
+                }
+            )
+
         def hist_f(x):
-            return x.update({'advantage_hist': wandb.Histogram(advantages)})
-        
+            return x.update({"advantage_hist": wandb.Histogram(advantages)})
+
         return loss, logs, [postproc_f, hist_f]
 
-    def score(self,
-              tokens: torch.Tensor,
-              attn_mask: Optional[torch.Tensor],
-              state_idxs: Optional[torch.Tensor],
-              action_idxs: Optional[torch.Tensor],
-              prefix_embs: Optional[torch.Tensor] = None,
-              prefix_attn_mask: Optional[torch.Tensor] = None,
-              remove_prefix_position_embs: bool = False,
-              qv_kwargs=None,
-              policy_kwargs=None,
-              target_kwargs=None,
-              beta: float = 1.0,
-              exp_weights: bool = False,
-              clip_weight: Optional[float] = None,
-              logit_temp: float = 1.0,
-              logit_top_k: Optional[int] = None,
-              logit_top_p: Optional[float] = None,
-              include_logits: bool = False,
-              include_advantage: bool = True,
-              action_mask: Optional[torch.Tensor] = None):
+    def score(
+        self,
+        tokens: torch.Tensor,
+        attn_mask: Optional[torch.Tensor],
+        state_idxs: Optional[torch.Tensor],
+        action_idxs: Optional[torch.Tensor],
+        prefix_embs: Optional[torch.Tensor] = None,
+        prefix_attn_mask: Optional[torch.Tensor] = None,
+        remove_prefix_position_embs: bool = False,
+        qv_kwargs=None,
+        policy_kwargs=None,
+        target_kwargs=None,
+        beta: float = 1.0,
+        exp_weights: bool = False,
+        clip_weight: Optional[float] = None,
+        logit_temp: float = 1.0,
+        logit_top_k: Optional[int] = None,
+        logit_top_p: Optional[float] = None,
+        include_logits: bool = False,
+        include_advantage: bool = True,
+        action_mask: Optional[torch.Tensor] = None,
+    ):
         trivial_value_query = False
         if state_idxs is None or action_idxs is None:
-            state_idxs = torch.full(
-                (tokens.shape[0], 1,), tokens.shape[1] - 1).long().to(self.device)
-            action_idxs = torch.full(
-                (tokens.shape[0], 1,), tokens.shape[1] - 1).long().to(self.device)
+            state_idxs = (
+                torch.full(
+                    (
+                        tokens.shape[0],
+                        1,
+                    ),
+                    tokens.shape[1] - 1,
+                )
+                .long()
+                .to(self.device)
+            )
+            action_idxs = (
+                torch.full(
+                    (
+                        tokens.shape[0],
+                        1,
+                    ),
+                    tokens.shape[1] - 1,
+                )
+                .long()
+                .to(self.device)
+            )
             trivial_value_query = True
-        self_outputs = self(tokens, state_idxs, action_idxs, attn_mask,
-                            prefix_embs, prefix_attn_mask,
-                            remove_prefix_position_embs,
-                            qv_kwargs, policy_kwargs, target_kwargs)
-        model_outputs = self_outputs['model_outputs']
-        weights = torch.zeros(self_outputs['logits'].shape).to(self.device)
+        self_outputs = self(
+            tokens,
+            state_idxs,
+            action_idxs,
+            attn_mask,
+            prefix_embs,
+            prefix_attn_mask,
+            remove_prefix_position_embs,
+            qv_kwargs,
+            policy_kwargs,
+            target_kwargs,
+        )
+        model_outputs = self_outputs["model_outputs"]
+        weights = torch.zeros(self_outputs["logits"].shape).to(self.device)
         if include_advantage:
             if action_mask is None:
                 action_mask = torch.ones((tokens.shape[0],)).to(self.device)
-            vs, qs = self_outputs['target_vs'], self_outputs['target_qs']
+            vs, qs = self_outputs["target_vs"], self_outputs["target_qs"]
             if not trivial_value_query:
                 vs = vs[:, :-1]
             if exp_weights:
                 w_values = beta * (qs - vs.unsqueeze(2))
             else:
                 adv_sign = ((qs - vs.unsqueeze(2)) > 0.0).float()
                 w_values = beta * adv_sign + (1 - beta) * (1 - adv_sign)
                 w_values = torch.log(w_values)
             if clip_weight is not None:
                 w_values = torch.clip(w_values, max=clip_weight)
             n = torch.argmax(action_idxs, dim=1) + 1
             for i in range(tokens.shape[0]):
-                weights[i] += torch.scatter(weights[i], dim=0,
-                                            index=action_idxs[i, :n[i]].unsqueeze(
-                                                1).repeat(1, weights.shape[2]),
-                                            src=w_values[i, :n[i], :]) * action_mask[i]
+                weights[i] += (
+                    torch.scatter(
+                        weights[i],
+                        dim=0,
+                        index=action_idxs[i, : n[i]]
+                        .unsqueeze(1)
+                        .repeat(1, weights.shape[2]),
+                        src=w_values[i, : n[i], :],
+                    )
+                    * action_mask[i]
+                )
         if include_logits:
             logits = process_logits(
-                self_outputs['logits'],
+                self_outputs["logits"],
                 temp=logit_temp,
                 top_k=logit_top_k,
-                top_p=logit_top_p)
+                top_p=logit_top_p,
+            )
             weights += torch.log(F.softmax(logits, dim=-1))
         return weights, model_outputs
 
-    def get_scores(self,
-                   items,
-                   beta: float = 1.0,
-                   exp_weights: bool = False,
-                   clip_weight: Optional[float] = None,
-                   logit_temp: float = 1.0,
-                   logit_top_k: Optional[int] = None,
-                   logit_top_p: Optional[float] = None,
-                   include_logits: bool = False,
-                   include_advantage: bool = True) -> torch.Tensor:
+    def get_scores(
+        self,
+        items,
+        beta: float = 1.0,
+        exp_weights: bool = False,
+        clip_weight: Optional[float] = None,
+        logit_temp: float = 1.0,
+        logit_top_k: Optional[int] = None,
+        logit_top_p: Optional[float] = None,
+        include_logits: bool = False,
+        include_advantage: bool = True,
+    ) -> torch.Tensor:
         prepared_inputs = self.prepare_inputs(items)
-        tokens, attn_mask = prepared_inputs['tokens'], prepared_inputs['attn_mask']
-        s_idx, a_idx = prepared_inputs['state_idxs'], prepared_inputs['action_idxs']
-        return self.score(tokens, attn_mask, s_idx, a_idx,
-                          beta=beta, exp_weights=exp_weights, clip_weight=clip_weight,
-                          logit_temp=logit_temp, logit_top_k=logit_top_k,
-                          logit_top_p=logit_top_p, include_logits=include_logits,
-                          include_advantage=include_advantage, action_mask=None)[0]
-
-    def initial_score(self,
-                      items,
-                      beta: float = 1.0,
-                      exp_weights: bool = False,
-                      clip_weight: Optional[float] = None,
-                      logit_temp: float = 1.0,
-                      logit_top_k: Optional[int] = None,
-                      logit_top_p: Optional[float] = None,
-                      include_logits: bool = False,
-                      include_advantage: bool = True) -> Tuple[torch.Tensor, Any]:
+        tokens, attn_mask = prepared_inputs["tokens"], prepared_inputs["attn_mask"]
+        s_idx, a_idx = prepared_inputs["state_idxs"], prepared_inputs["action_idxs"]
+        return self.score(
+            tokens,
+            attn_mask,
+            s_idx,
+            a_idx,
+            beta=beta,
+            exp_weights=exp_weights,
+            clip_weight=clip_weight,
+            logit_temp=logit_temp,
+            logit_top_k=logit_top_k,
+            logit_top_p=logit_top_p,
+            include_logits=include_logits,
+            include_advantage=include_advantage,
+            action_mask=None,
+        )[0]
+
+    def initial_score(
+        self,
+        items,
+        beta: float = 1.0,
+        exp_weights: bool = False,
+        clip_weight: Optional[float] = None,
+        logit_temp: float = 1.0,
+        logit_top_k: Optional[int] = None,
+        logit_top_p: Optional[float] = None,
+        include_logits: bool = False,
+        include_advantage: bool = True,
+    ) -> Tuple[torch.Tensor, Any]:
         prepared_inputs = self.prepare_inputs(items)
-        tokens = prepared_inputs['tokens']
-        is_state = ((tokens == self.dataset.tokenizer.bos_token_id).float(
-        ) + (tokens == self.dataset.tokenizer.eoa_token_id).float()) > 0
-        is_action = ((tokens == self.dataset.tokenizer.boa_token_id).float(
-        ) + (tokens == self.dataset.tokenizer.eos_token_id).float()) > 0
-        state_points = torch.where(is_state, torch.arange(tokens.shape[1]).unsqueeze(
-            0).repeat(tokens.shape[0], 1).to(self.device), -1)
-        action_points = torch.where(is_action, torch.arange(tokens.shape[1]).unsqueeze(
-            0).repeat(tokens.shape[0], 1).to(self.device), -1)
-        action_mask = (action_points.argmax(dim=1) >=
-                       state_points.argmax(dim=1)).float()
-        scores, model_outputs = self.score(tokens, None, None, None,
-                                           beta=beta, exp_weights=exp_weights,
-                                           clip_weight=clip_weight,
-                                           logit_temp=logit_temp, logit_top_k=logit_top_k,
-                                           logit_top_p=logit_top_p, include_logits=include_logits,
-                                           include_advantage=include_advantage, action_mask=action_mask)
+        tokens = prepared_inputs["tokens"]
+        is_state = (
+            (tokens == self.dataset.tokenizer.bos_token_id).float()
+            + (tokens == self.dataset.tokenizer.eoa_token_id).float()
+        ) > 0
+        is_action = (
+            (tokens == self.dataset.tokenizer.boa_token_id).float()
+            + (tokens == self.dataset.tokenizer.eos_token_id).float()
+        ) > 0
+        state_points = torch.where(
+            is_state,
+            torch.arange(tokens.shape[1])
+            .unsqueeze(0)
+            .repeat(tokens.shape[0], 1)
+            .to(self.device),
+            -1,
+        )
+        action_points = torch.where(
+            is_action,
+            torch.arange(tokens.shape[1])
+            .unsqueeze(0)
+            .repeat(tokens.shape[0], 1)
+            .to(self.device),
+            -1,
+        )
+        action_mask = (
+            action_points.argmax(dim=1) >= state_points.argmax(dim=1)
+        ).float()
+        scores, model_outputs = self.score(
+            tokens,
+            None,
+            None,
+            None,
+            beta=beta,
+            exp_weights=exp_weights,
+            clip_weight=clip_weight,
+            logit_temp=logit_temp,
+            logit_top_k=logit_top_k,
+            logit_top_p=logit_top_p,
+            include_logits=include_logits,
+            include_advantage=include_advantage,
+            action_mask=action_mask,
+        )
         return scores[:, -1, :], (
-            model_outputs['qv_model_outputs']['past_key_values'],
-            model_outputs['policy_model_outputs']['past_key_values'],
-            model_outputs['target_model_outputs']['past_key_values'],
+            model_outputs["qv_model_outputs"]["past_key_values"],
+            model_outputs["policy_model_outputs"]["past_key_values"],
+            model_outputs["target_model_outputs"]["past_key_values"],
             action_mask,
         )
 
-    def next_score(self,
-                   tokens: torch.Tensor,
-                   state: Any,
-                   beta: float = 1.0,
-                   exp_weights: bool = False,
-                   clip_weight: Optional[float] = None,
-                   logit_temp: float = 1.0,
-                   logit_top_k: Optional[int] = None,
-                   logit_top_p: Optional[float] = None,
-                   include_logits: bool = False,
-                   include_advantage: bool = True) -> Tuple[torch.Tensor, Any]:
+    def next_score(
+        self,
+        tokens: torch.Tensor,
+        state: Any,
+        beta: float = 1.0,
+        exp_weights: bool = False,
+        clip_weight: Optional[float] = None,
+        logit_temp: float = 1.0,
+        logit_top_k: Optional[int] = None,
+        logit_top_p: Optional[float] = None,
+        include_logits: bool = False,
+        include_advantage: bool = True,
+    ) -> Tuple[torch.Tensor, Any]:
         qv_kvs, policy_kvs, target_kvs, action_mask = state
         action_mask *= (tokens != self.dataset.tokenizer.eoa_token_id).float()
         action_mask += (tokens == self.dataset.tokenizer.eos_token_id).float()
         action_mask = (action_mask > 0.0).float()
-        scores, model_outputs = self.score(tokens.unsqueeze(1), None, None, None,
-                                           qv_kwargs={'past_key_values': qv_kvs},
-                                           policy_kwargs={'past_key_values': policy_kvs},
-                                           target_kwargs={'past_key_values': target_kvs},
-                                           beta=beta, exp_weights=exp_weights, clip_weight=clip_weight,
-                                           logit_temp=logit_temp, logit_top_k=logit_top_k,
-                                           logit_top_p=logit_top_p, include_logits=include_logits,
-                                           include_advantage=include_advantage, action_mask=action_mask)
+        scores, model_outputs = self.score(
+            tokens.unsqueeze(1),
+            None,
+            None,
+            None,
+            qv_kwargs={"past_key_values": qv_kvs},
+            policy_kwargs={"past_key_values": policy_kvs},
+            target_kwargs={"past_key_values": target_kvs},
+            beta=beta,
+            exp_weights=exp_weights,
+            clip_weight=clip_weight,
+            logit_temp=logit_temp,
+            logit_top_k=logit_top_k,
+            logit_top_p=logit_top_p,
+            include_logits=include_logits,
+            include_advantage=include_advantage,
+            action_mask=action_mask,
+        )
         return scores.squeeze(1), (
-            model_outputs['qv_model_outputs']['past_key_values'],
-            model_outputs['policy_model_outputs']['past_key_values'],
-            model_outputs['target_model_outputs']['past_key_values'],
+            model_outputs["qv_model_outputs"]["past_key_values"],
+            model_outputs["policy_model_outputs"]["past_key_values"],
+            model_outputs["target_model_outputs"]["past_key_values"],
             action_mask,
         )
 
     def softUpdate(self):
-        """Soft updates target networks.
-        """
+        """Soft updates target networks."""
         for target_param, local_param in zip(
-                self.target_q.parameters(), self.q.parameters()):
+            self.target_q.parameters(), self.q.parameters()
+        ):
             target_param.data.copy_(
-                self.alpha * local_param.data + (1.0 - self.alpha) * target_param.data)
+                self.alpha * local_param.data + (1.0 - self.alpha) * target_param.data
+            )
         if self.double_q:
             for target_param, local_param in zip(
-                    self.target_q2.parameters(), self.q2.parameters()):
+                self.target_q2.parameters(), self.q2.parameters()
+            ):
                 target_param.data.copy_(
-                    self.alpha * local_param.data + (1.0 - self.alpha) * target_param.data)
+                    self.alpha * local_param.data
+                    + (1.0 - self.alpha) * target_param.data
+                )
         if self.actor_target is not None:
             for target_param, local_param in zip(
-                    self.actor_target.parameters(), self.model.parameters()):
+                self.actor_target.parameters(), self.model.parameters()
+            ):
                 target_param.data.copy_(
-                    self.alpha * local_param.data + (1.0 - self.alpha) * target_param.data)
+                    self.alpha * local_param.data
+                    + (1.0 - self.alpha) * target_param.data
+                )
 
     def hardUpdate(self):
-        """Hard updates target networks.
-        """
+        """Hard updates target networks."""
         for target_param, local_param in zip(
-                self.target_q.parameters(), self.q.parameters()):
+            self.target_q.parameters(), self.q.parameters()
+        ):
             target_param.data.copy_(local_param.data)
         if self.double_q:
             for target_param, local_param in zip(
-                    self.target_q2.parameters(), self.q2.parameters()):
+                self.target_q2.parameters(), self.q2.parameters()
+            ):
                 target_param.data.copy_(local_param.data)
         if self.actor_target is not None:
             del self.actor_target
             self.actor_target = None
             self.actor_target = copy.deepcopy(self.model)
 
     def clone(self, index=None):
@@ -824,587 +1104,974 @@
 
         :param index: Index to keep track of agent for tournament selection and mutation, defaults to None
         :type index: int, optional
         """
         if index is None:
             index = self.index
 
-        clone = type(self)(dataset=self.dataset,
-                           net_config=self.net_config,
-                           index=index,
-                           batch_size=self.batch_size,
-                           lr=self.lr,
-                           alpha=self.alpha,
-                           beta=self.beta,
-                           gamma=self.gamma,
-                           tau=self.tau,
-                           mutation=self.mut,
-                           transition_weight=self.transition_weight,
-                           clip_weight=self.clip_weight,
-                           value_max=self.value_max,
-                           value_min=self.value_min,
-                           detach_v=self.detach_v,
-                           detach_q=self.detach_q,
-                           detach_pi=self.detach_pi,
-                           double_q=self.double_q,
-                           per_token=self.per_token,
-                           exp_weights=self.exp_weights,
-                           dm_margin=self.dm_margin,
-                           cql_temp=self.cql_temp,
-                           weight_decay=self.weight_decay,
-                           device=self.device,
-                           )
+        clone = type(self)(
+            dataset=self.dataset,
+            net_config=self.net_config,
+            index=index,
+            batch_size=self.batch_size,
+            lr=self.lr,
+            alpha=self.alpha,
+            beta=self.beta,
+            gamma=self.gamma,
+            tau=self.tau,
+            mutation=self.mut,
+            transition_weight=self.transition_weight,
+            clip_weight=self.clip_weight,
+            value_max=self.value_max,
+            value_min=self.value_min,
+            detach_v=self.detach_v,
+            detach_q=self.detach_q,
+            detach_pi=self.detach_pi,
+            double_q=self.double_q,
+            per_token=self.per_token,
+            exp_weights=self.exp_weights,
+            dm_margin=self.dm_margin,
+            cql_temp=self.cql_temp,
+            weight_decay=self.weight_decay,
+            device=self.device,
+        )
 
         clone.model = self.model.clone().to(self.device)
         clone.actor = self.actor.clone().to(self.device)
         clone.actor_target = self.actor_target.clone().to(self.device)
-        clone.optimizer = optim.Adam(clone.actor.parameters(
-        ), lr=clone.lr, weight_decay=clone.weight_decay)
+        clone.optimizer = optim.Adam(
+            clone.actor.parameters(), lr=clone.lr, weight_decay=clone.weight_decay
+        )
         clone.fitness = copy.deepcopy(self.fitness)
         clone.steps = copy.deepcopy(self.steps)
         clone.scores = copy.deepcopy(self.scores)
 
         return clone
 
     def saveCheckpoint(self, path):
         """Saves a checkpoint of agent properties and network weights to path.
 
         :param path: Location to save checkpoint at
         :type path: string
         """
-        torch.save({
-            'model_init_dict': self.model.init_dict,
-            'model_state_dict': self.model.state_dict(),
-            'actor_init_dict': self.actor.init_dict,
-            'actor_state_dict': self.actor.state_dict(),
-            'actor_target_init_dict': self.actor_target.init_dict,
-            'actor_target_state_dict': self.actor_target.state_dict(),
-            'optimizer_state_dict': self.optimizer.state_dict(),
-            'dataset': self.dataset,
-            'net_config': self.net_config,
-            'batch_size': self.batch_size,
-            'lr': self.lr,
-            'alpha': self.alpha,
-            'beta': self.beta,
-            'gamma': self.gamma,
-            'tau': self.tau,
-            'mutation': self.mut,
-            'transition_weight': self.transition_weight,
-            'clip_weight': self.clip_weight,
-            'value_max': self.value_max,
-            'value_min': self.value_min,
-            'detach_v': self.detach_v,
-            'detach_q': self.detach_q,
-            'detach_pi': self.detach_pi,
-            'double_q': self.double_q,
-            'per_token': self.per_token,
-            'exp_weights': self.exp_weights,
-            'dm_margin': self.dm_margin,
-            'cql_temp': self.cql_temp,
-            'weight_decay': self.weight_decay,
-            'index': self.index,
-            'scores': self.scores,
-            'fitness': self.fitness,
-            'steps': self.steps,
-        }, path)
+        torch.save(
+            {
+                "model_init_dict": self.model.init_dict,
+                "model_state_dict": self.model.state_dict(),
+                "actor_init_dict": self.actor.init_dict,
+                "actor_state_dict": self.actor.state_dict(),
+                "actor_target_init_dict": self.actor_target.init_dict,
+                "actor_target_state_dict": self.actor_target.state_dict(),
+                "optimizer_state_dict": self.optimizer.state_dict(),
+                "dataset": self.dataset,
+                "net_config": self.net_config,
+                "batch_size": self.batch_size,
+                "lr": self.lr,
+                "alpha": self.alpha,
+                "beta": self.beta,
+                "gamma": self.gamma,
+                "tau": self.tau,
+                "mutation": self.mut,
+                "transition_weight": self.transition_weight,
+                "clip_weight": self.clip_weight,
+                "value_max": self.value_max,
+                "value_min": self.value_min,
+                "detach_v": self.detach_v,
+                "detach_q": self.detach_q,
+                "detach_pi": self.detach_pi,
+                "double_q": self.double_q,
+                "per_token": self.per_token,
+                "exp_weights": self.exp_weights,
+                "dm_margin": self.dm_margin,
+                "cql_temp": self.cql_temp,
+                "weight_decay": self.weight_decay,
+                "index": self.index,
+                "scores": self.scores,
+                "fitness": self.fitness,
+                "steps": self.steps,
+            },
+            path,
+        )
 
     def loadCheckpoint(self, path):
         """Loads saved agent properties and network weights from checkpoint.
 
         :param path: Location to load checkpoint from
         :type path: string
         """
         checkpoint = torch.load(path)
-        self.net_config = checkpoint['net_config']
-        self.model = EvolvableGPT(**checkpoint['model_init_dict'])
-        self.actor = EvolvableGPT(**checkpoint['actor_init_dict'])
-        self.actor_target = EvolvableGPT(
-            **checkpoint['actor_target_init_dict'])
-        self.model.load_state_dict(checkpoint['model_state_dict'])
-        self.actor.load_state_dict(checkpoint['actor_state_dict'])
-        self.actor_target.load_state_dict(
-            checkpoint['actor_target_state_dict'])
-        self.optimizer.load_state_dict(checkpoint['optimizer_state_dict'])
-        self.batch_size = checkpoint['batch_size']
-        self.lr = checkpoint['lr']
-        self.alpha = checkpoint['alpha']
-        self.beta = checkpoint['beta']
-        self.gamma = checkpoint['gamma']
-        self.tau = checkpoint['tau']
-        self.mut = checkpoint['mutation']
-        self.transition_weight = checkpoint['transition_weight']
-        self.clip_weight = checkpoint['clip_weight']
-        self.value_max = checkpoint['value_max']
-        self.value_min = checkpoint['value_min']
-        self.detach_v = checkpoint['detach_v']
-        self.detach_q = checkpoint['detach_q']
-        self.detach_pi = checkpoint['detach_pi']
-        self.double_q = checkpoint['double_q']
-        self.per_token = checkpoint['per_token']
-        self.exp_weights = checkpoint['exp_weights']
-        self.dm_margin = checkpoint['dm_margin']
-        self.cql_temp = checkpoint['cql_temp']
-        self.weight_decay = checkpoint['weight_decay']
-        self.index = checkpoint['index']
-        self.scores = checkpoint['scores']
-        self.fitness = checkpoint['fitness']
-        self.steps = checkpoint['steps']
-
-
-class ILQL_Policy():
-    def __init__(self, iql_model: ILQL, 
-                 kind: str, **generation_kwargs) -> None:
+        self.net_config = checkpoint["net_config"]
+        self.model = EvolvableGPT(**checkpoint["model_init_dict"])
+        self.actor = EvolvableGPT(**checkpoint["actor_init_dict"])
+        self.actor_target = EvolvableGPT(**checkpoint["actor_target_init_dict"])
+        self.model.load_state_dict(checkpoint["model_state_dict"])
+        self.actor.load_state_dict(checkpoint["actor_state_dict"])
+        self.actor_target.load_state_dict(checkpoint["actor_target_state_dict"])
+        self.optimizer.load_state_dict(checkpoint["optimizer_state_dict"])
+        self.batch_size = checkpoint["batch_size"]
+        self.lr = checkpoint["lr"]
+        self.alpha = checkpoint["alpha"]
+        self.beta = checkpoint["beta"]
+        self.gamma = checkpoint["gamma"]
+        self.tau = checkpoint["tau"]
+        self.mut = checkpoint["mutation"]
+        self.transition_weight = checkpoint["transition_weight"]
+        self.clip_weight = checkpoint["clip_weight"]
+        self.value_max = checkpoint["value_max"]
+        self.value_min = checkpoint["value_min"]
+        self.detach_v = checkpoint["detach_v"]
+        self.detach_q = checkpoint["detach_q"]
+        self.detach_pi = checkpoint["detach_pi"]
+        self.double_q = checkpoint["double_q"]
+        self.per_token = checkpoint["per_token"]
+        self.exp_weights = checkpoint["exp_weights"]
+        self.dm_margin = checkpoint["dm_margin"]
+        self.cql_temp = checkpoint["cql_temp"]
+        self.weight_decay = checkpoint["weight_decay"]
+        self.index = checkpoint["index"]
+        self.scores = checkpoint["scores"]
+        self.fitness = checkpoint["fitness"]
+        self.steps = checkpoint["steps"]
+
+
+class ILQL_Policy:
+    def __init__(self, iql_model: ILQL, kind: str, **generation_kwargs) -> None:
         super().__init__()
         self.iql_model = iql_model
-        assert kind in {'beam', 'sample'}
+        assert kind in {"beam", "sample"}
         self.kind = kind
         self.generation_kwargs = generation_kwargs
         self.kls_all = []
         self.logprobs_all = []
-    
-    def sample_raw(self, 
-                   tokens: torch.Tensor, attn_mask: torch.Tensor, 
-                   state_idxs: torch.Tensor, action_idxs: torch.Tensor, 
-                   termination_condition: Callable[[np.ndarray], bool], 
-                   num_generations=1, max_generation_len=None, 
-                   temp=1.0, top_k=None, top_p=None, 
-                   exp_adv=False, adv_weight=0.0, adv_clip=None, 
-                   include_logits=True, include_adv=True, 
-                   rerank_log_prob_weight: float=0.0, 
-                   rerank_advantage_weight: float=0.0, 
-                   prefix_embs: Optional[torch.Tensor]=None, 
-                   prefix_attn_mask: Optional[torch.Tensor]=None, 
-                   remove_prefix_position_embs: bool=False):
+
+    def sample_raw(
+        self,
+        tokens: torch.Tensor,
+        attn_mask: torch.Tensor,
+        state_idxs: torch.Tensor,
+        action_idxs: torch.Tensor,
+        termination_condition: Callable[[np.ndarray], bool],
+        num_generations=1,
+        max_generation_len=None,
+        temp=1.0,
+        top_k=None,
+        top_p=None,
+        exp_adv=False,
+        adv_weight=0.0,
+        adv_clip=None,
+        include_logits=True,
+        include_adv=True,
+        rerank_log_prob_weight: float = 0.0,
+        rerank_advantage_weight: float = 0.0,
+        prefix_embs: Optional[torch.Tensor] = None,
+        prefix_attn_mask: Optional[torch.Tensor] = None,
+        remove_prefix_position_embs: bool = False,
+    ):
         assert include_logits or include_adv
-        
+
         tokenizer = self.iql_model.dataset.tokenizer
         max_length = self.iql_model.dataset.max_len
         if max_length is None:
             max_length = self.iql_model.model.block_size
         max_length = min(max_length, self.iql_model.model.block_size)
         device = self.iql_model.device
         bsize = tokens.shape[0]
         n = bsize * num_generations
         if max_generation_len is None:
-            max_generation_len = max_length+1
-        input_strs = [tokenizer.decode(tokens[i, :][:attn_mask[i, :].sum().long()].tolist(), 
-                                       clean_up_tokenization_spaces=False) for i in range(len(tokens))]
+            max_generation_len = max_length + 1
+        input_strs = [
+            tokenizer.decode(
+                tokens[i, :][: attn_mask[i, :].sum().long()].tolist(),
+                clean_up_tokenization_spaces=False,
+            )
+            for i in range(len(tokens))
+        ]
         prefix_t = 0 if prefix_embs is None else prefix_embs.shape[1]
-        model_outputs = self.iql_model(tokens, 
-                                       state_idxs, action_idxs, attn_mask,
-                                       prefix_embs=prefix_embs, 
-                                       prefix_attn_mask=prefix_attn_mask, 
-                                       remove_prefix_position_embs=remove_prefix_position_embs,
-                                       is_causal=False)['model_outputs']
-        kvs = {'qv': model_outputs['qv_model_outputs']['past_key_values']}
+        model_outputs = self.iql_model(
+            tokens,
+            state_idxs,
+            action_idxs,
+            attn_mask,
+            prefix_embs=prefix_embs,
+            prefix_attn_mask=prefix_attn_mask,
+            remove_prefix_position_embs=remove_prefix_position_embs,
+            is_causal=False,
+        )["model_outputs"]
+        kvs = {"qv": model_outputs["qv_model_outputs"]["past_key_values"]}
         if self.iql_model.actor_target is not None:
-            kvs['target'] = model_outputs['target_model_outputs']['past_key_values']
+            kvs["target"] = model_outputs["target_model_outputs"]["past_key_values"]
         if self.iql_model.actor is not None:
-            kvs['policy'] = model_outputs['policy_model_outputs']['past_key_values']
+            kvs["policy"] = model_outputs["policy_model_outputs"]["past_key_values"]
         dialogue_lens = attn_mask.sum(dim=1)
-        tokens = pad_sequence(torch.repeat_interleave(tokens, num_generations, dim=0), max_length, 
-                              tokenizer.pad_token_id, device, 1)
+        tokens = pad_sequence(
+            torch.repeat_interleave(tokens, num_generations, dim=0),
+            max_length,
+            tokenizer.pad_token_id,
+            device,
+            1,
+        )
         dialogue_lens = torch.repeat_interleave(dialogue_lens, num_generations, dim=0)
-        kvs['qv'] = map_all_kvs(lambda x: pad_sequence(torch.repeat_interleave(x, num_generations, dim=0), 
-                                                       max_length, 0.0, device, 2), kvs['qv'])
-        if 'target' in kvs:
-            kvs['target'] = map_all_kvs(lambda x: pad_sequence(torch.repeat_interleave(x, num_generations, dim=0), 
-                                                               max_length, 0.0, device, 2), kvs['target'])
-        if 'policy' in kvs:
-            kvs['policy'] = map_all_kvs(lambda x: pad_sequence(torch.repeat_interleave(x, num_generations, dim=0), 
-                                                               max_length, 0.0, device, 2), kvs['policy'])
+        kvs["qv"] = map_all_kvs(
+            lambda x: pad_sequence(
+                torch.repeat_interleave(x, num_generations, dim=0),
+                max_length,
+                0.0,
+                device,
+                2,
+            ),
+            kvs["qv"],
+        )
+        if "target" in kvs:
+            kvs["target"] = map_all_kvs(
+                lambda x: pad_sequence(
+                    torch.repeat_interleave(x, num_generations, dim=0),
+                    max_length,
+                    0.0,
+                    device,
+                    2,
+                ),
+                kvs["target"],
+            )
+        if "policy" in kvs:
+            kvs["policy"] = map_all_kvs(
+                lambda x: pad_sequence(
+                    torch.repeat_interleave(x, num_generations, dim=0),
+                    max_length,
+                    0.0,
+                    device,
+                    2,
+                ),
+                kvs["policy"],
+            )
         log_probs = torch.full((dialogue_lens.shape[0],), 0.0).to(device)
-        kls = torch.full((dialogue_lens.shape[0],), math.log(
-            num_generations)-((num_generations-1)/num_generations)).to(device)
+        kls = torch.full(
+            (dialogue_lens.shape[0],),
+            math.log(num_generations) - ((num_generations - 1) / num_generations),
+        ).to(device)
         advantages = torch.full((dialogue_lens.shape[0],), 0.0).to(device)
         termination_mask = torch.full((dialogue_lens.shape[0],), 1).to(device)
-        state_idxs_temp, action_idxs_temp = torch.zeros((dialogue_lens.shape[0], 1,)).long().to(device), \
-            torch.zeros((dialogue_lens.shape[0], 1,)).long().to(device)
+        state_idxs_temp, action_idxs_temp = torch.zeros(
+            (
+                dialogue_lens.shape[0],
+                1,
+            )
+        ).long().to(device), torch.zeros(
+            (
+                dialogue_lens.shape[0],
+                1,
+            )
+        ).long().to(
+            device
+        )
         t = torch.min(dialogue_lens).int()
         base_logits = torch.full((dialogue_lens.shape[0],), 0.0).to(device)
-        while termination_mask.sum() > 0 and (t+prefix_t) < max_length:
-            curr_token = tokens[:, t-1].unsqueeze(1)
-            curr_kvs = map_all_kvs(lambda x: x[:,:,:(t+prefix_t)-1,:], kvs['qv'])
+        while termination_mask.sum() > 0 and (t + prefix_t) < max_length:
+            curr_token = tokens[:, t - 1].unsqueeze(1)
+            curr_kvs = map_all_kvs(
+                lambda x: x[:, :, : (t + prefix_t) - 1, :], kvs["qv"]
+            )
             curr_target_kvs, curr_policy_kvs = curr_kvs, curr_kvs
-            if 'target' in kvs:
-                map_all_kvs(lambda x: x[:,:,:(t+prefix_t)-1,:], kvs['target'])
-            if 'policy' in kvs:
-                map_all_kvs(lambda x: x[:,:,:(t+prefix_t)-1,:], kvs['policy'])
-            iql_outputs = self.iql_model(curr_token, state_idxs_temp, action_idxs_temp, None,
-                                         qv_kwargs={'past_key_values': curr_kvs}, 
-                                         policy_kwargs={'past_key_values': curr_policy_kvs}, 
-                                         target_kwargs={'past_key_values': curr_target_kvs},
-                                         is_causal=False)
-            model_outputs, logits = iql_outputs['model_outputs'], iql_outputs['logits']
-            
-            logits[:, 0, tokenizer.pad_token_id] = torch.where(termination_mask == 1, float('-inf'), 1e7)
-            logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(
-                device), tokens[:, t]] = logits[torch.arange(0, n).to(device), torch.full(
-                (n,), 0).to(device), tokens[:, t]].masked_fill_(t < dialogue_lens, 1e7)
-            edited_logits = process_logits(logits.clone(), temp=temp, top_k=top_k, top_p=top_p)
+            if "target" in kvs:
+                map_all_kvs(lambda x: x[:, :, : (t + prefix_t) - 1, :], kvs["target"])
+            if "policy" in kvs:
+                map_all_kvs(lambda x: x[:, :, : (t + prefix_t) - 1, :], kvs["policy"])
+            iql_outputs = self.iql_model(
+                curr_token,
+                state_idxs_temp,
+                action_idxs_temp,
+                None,
+                qv_kwargs={"past_key_values": curr_kvs},
+                policy_kwargs={"past_key_values": curr_policy_kvs},
+                target_kwargs={"past_key_values": curr_target_kvs},
+                is_causal=False,
+            )
+            model_outputs, logits = iql_outputs["model_outputs"], iql_outputs["logits"]
+
+            logits[:, 0, tokenizer.pad_token_id] = torch.where(
+                termination_mask == 1, float("-inf"), 1e7
+            )
+            logits[
+                torch.arange(0, n).to(device),
+                torch.full((n,), 0).to(device),
+                tokens[:, t],
+            ] = logits[
+                torch.arange(0, n).to(device),
+                torch.full((n,), 0).to(device),
+                tokens[:, t],
+            ].masked_fill_(
+                t < dialogue_lens, 1e7
+            )
+            edited_logits = process_logits(
+                logits.clone(), temp=temp, top_k=top_k, top_p=top_p
+            )
 
-            vs, qs = iql_outputs['target_vs'], iql_outputs['target_qs']
+            vs, qs = iql_outputs["target_vs"], iql_outputs["target_qs"]
             if exp_adv:
                 adv_logits = adv_weight * (qs - vs.unsqueeze(2))
             else:
                 adv_sign = ((qs - vs.unsqueeze(2)) > 0.0).float()
                 adv_logits = adv_weight * adv_sign + (1 - adv_weight) * (1 - adv_sign)
                 adv_logits = torch.log(adv_logits)
             if adv_clip is not None:
                 adv_logits = torch.clip(adv_logits, max=adv_clip)
-            adv_logits[:, 0, tokenizer.pad_token_id] = torch.where(termination_mask == 1, float('-inf'), 1e7)
-            adv_logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(
-                device), tokens[:, t]] = adv_logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(
-                device), tokens[:, t]].masked_fill_(t < dialogue_lens, 1e7)
-
-            full_logits = (edited_logits if include_logits else 0.0) + (
-                adv_logits if include_adv else 0.0) + base_logits.unsqueeze(1).unsqueeze(2)
-
-            cat_dist = torch.distributions.categorical.Categorical(logits=full_logits[:, 0])
-            original_cat_dist = torch.distributions.categorical.Categorical(logits=logits[:, 0])
+            adv_logits[:, 0, tokenizer.pad_token_id] = torch.where(
+                termination_mask == 1, float("-inf"), 1e7
+            )
+            adv_logits[
+                torch.arange(0, n).to(device),
+                torch.full((n,), 0).to(device),
+                tokens[:, t],
+            ] = adv_logits[
+                torch.arange(0, n).to(device),
+                torch.full((n,), 0).to(device),
+                tokens[:, t],
+            ].masked_fill_(
+                t < dialogue_lens, 1e7
+            )
+
+            full_logits = (
+                (edited_logits if include_logits else 0.0)
+                + (adv_logits if include_adv else 0.0)
+                + base_logits.unsqueeze(1).unsqueeze(2)
+            )
+
+            cat_dist = torch.distributions.categorical.Categorical(
+                logits=full_logits[:, 0]
+            )
+            original_cat_dist = torch.distributions.categorical.Categorical(
+                logits=logits[:, 0]
+            )
 
             new_tokens = cat_dist.sample()
             log_probs += cat_dist.log_prob(new_tokens)
-            kls += (cat_dist.log_prob(new_tokens) - original_cat_dist.log_prob(new_tokens))
-            qs_chosen = torch.gather(qs.squeeze(1), dim=1, index=new_tokens.unsqueeze(1)).squeeze(1)
-            advantages += (qs_chosen - vs.squeeze(1))
+            kls += cat_dist.log_prob(new_tokens) - original_cat_dist.log_prob(
+                new_tokens
+            )
+            qs_chosen = torch.gather(
+                qs.squeeze(1), dim=1, index=new_tokens.unsqueeze(1)
+            ).squeeze(1)
+            advantages += qs_chosen - vs.squeeze(1)
             tokens[:, t] = new_tokens
-            kvs['qv'] = update_kvs(kvs['qv'], 
-                                   model_outputs['qv_model_outputs']['past_key_values'], 
-                                   torch.arange(0, n).to(device), (t+prefix_t)-1)
-            if 'target' in kvs:
-                kvs['target'] = update_kvs(kvs['target'], 
-                                           model_outputs['target_model_outputs']['past_key_values'], 
-                                           torch.arange(0, n).to(device), (t+prefix_t)-1)
-            if 'policy' in kvs:
-                kvs['policy'] = update_kvs(kvs['policy'], 
-                                           model_outputs['policy_model_outputs']['past_key_values'], 
-                                           torch.arange(0, n).to(device), (t+prefix_t)-1)
+            kvs["qv"] = update_kvs(
+                kvs["qv"],
+                model_outputs["qv_model_outputs"]["past_key_values"],
+                torch.arange(0, n).to(device),
+                (t + prefix_t) - 1,
+            )
+            if "target" in kvs:
+                kvs["target"] = update_kvs(
+                    kvs["target"],
+                    model_outputs["target_model_outputs"]["past_key_values"],
+                    torch.arange(0, n).to(device),
+                    (t + prefix_t) - 1,
+                )
+            if "policy" in kvs:
+                kvs["policy"] = update_kvs(
+                    kvs["policy"],
+                    model_outputs["policy_model_outputs"]["past_key_values"],
+                    torch.arange(0, n).to(device),
+                    (t + prefix_t) - 1,
+                )
             for idx in range(n):
                 if tokens[idx, t] == tokenizer.eoa_token_id and t >= dialogue_lens[idx]:
-                    termination_mask[idx] *= (1 - int(termination_condition(tokenizer.decode(tokens[idx, :].tolist(), 
-                                                                                             clean_up_tokenization_spaces=False))))
+                    termination_mask[idx] *= 1 - int(
+                        termination_condition(
+                            tokenizer.decode(
+                                tokens[idx, :].tolist(),
+                                clean_up_tokenization_spaces=False,
+                            )
+                        )
+                    )
             t += 1
-            termination_mask *= ((t-dialogue_lens) < max_generation_len).int()
+            termination_mask *= ((t - dialogue_lens) < max_generation_len).int()
 
-        scores = ((advantages * rerank_advantage_weight) + (
-            log_probs * rerank_log_prob_weight)).reshape(-1, num_generations)
+        scores = (
+            (advantages * rerank_advantage_weight)
+            + (log_probs * rerank_log_prob_weight)
+        ).reshape(-1, num_generations)
         order = torch.argsort(-scores, dim=1)
-        output_strs = [tokenizer.decode(tokens[i, :].tolist(), 
-                                        clean_up_tokenization_spaces=False) for i in range(len(tokens))]
+        output_strs = [
+            tokenizer.decode(tokens[i, :].tolist(), clean_up_tokenization_spaces=False)
+            for i in range(len(tokens))
+        ]
         processed_outputs = []
         for i in range(len(input_strs)):
             temp_outputs = []
             for x in range(num_generations):
-                processed_str = output_strs[i*num_generations+order[i, x]][len(input_strs[i]):].strip()
+                processed_str = output_strs[i * num_generations + order[i, x]][
+                    len(input_strs[i]) :
+                ].strip()
                 if tokenizer.id_to_token(tokenizer.pad_token_id) in processed_str:
-                    processed_str = processed_str[:processed_str.find(
-                        tokenizer.id_to_token(tokenizer.pad_token_id))].strip()
+                    processed_str = processed_str[
+                        : processed_str.find(
+                            tokenizer.id_to_token(tokenizer.pad_token_id)
+                        )
+                    ].strip()
                 if tokenizer.id_to_token(tokenizer.eoa_token_id) in processed_str:
-                    processed_str = processed_str[:processed_str.find(
-                        tokenizer.id_to_token(tokenizer.eoa_token_id))].strip()
+                    processed_str = processed_str[
+                        : processed_str.find(
+                            tokenizer.id_to_token(tokenizer.eoa_token_id)
+                        )
+                    ].strip()
                 temp_outputs.append(processed_str)
             processed_outputs.append(temp_outputs)
         scores = torch.gather(scores, dim=1, index=order)
-        log_probs = torch.gather(log_probs.reshape(-1, num_generations), dim=1, index=order)
+        log_probs = torch.gather(
+            log_probs.reshape(-1, num_generations), dim=1, index=order
+        )
         kls = torch.gather(kls.reshape(-1, num_generations), dim=1, index=order)
-        return list(zip(input_strs, processed_outputs)), log_probs.reshape(-1, num_generations), kls
-    
-    def beam_raw(self, 
-                 tokens: torch.Tensor, attn_mask: torch.Tensor, 
-                 state_idxs: torch.Tensor, action_idxs: torch.Tensor, 
-                 termination_condition: Callable[[np.ndarray], bool], 
-                 max_generation_len: Optional[int]=None, beam_width=1, 
-                 temp=1.0, top_k=None, top_p=None, 
-                 exp_adv=False, adv_weight=0.0, adv_clip=None, 
-                 include_logits=True, include_adv=True, 
-                 prefix_embs: Optional[torch.Tensor]=None, 
-                 prefix_attn_mask: Optional[torch.Tensor]=None, 
-                 remove_prefix_position_embs: bool=False):
-        
+        return (
+            list(zip(input_strs, processed_outputs)),
+            log_probs.reshape(-1, num_generations),
+            kls,
+        )
+
+    def beam_raw(
+        self,
+        tokens: torch.Tensor,
+        attn_mask: torch.Tensor,
+        state_idxs: torch.Tensor,
+        action_idxs: torch.Tensor,
+        termination_condition: Callable[[np.ndarray], bool],
+        max_generation_len: Optional[int] = None,
+        beam_width=1,
+        temp=1.0,
+        top_k=None,
+        top_p=None,
+        exp_adv=False,
+        adv_weight=0.0,
+        adv_clip=None,
+        include_logits=True,
+        include_adv=True,
+        prefix_embs: Optional[torch.Tensor] = None,
+        prefix_attn_mask: Optional[torch.Tensor] = None,
+        remove_prefix_position_embs: bool = False,
+    ):
         tokenizer = self.iql_model.dataset.tokenizer
         max_length = self.iql_model.dataset.max_len
         if max_length is None:
             max_length = self.iql_model.model.block_size
         max_length = min(max_length, self.iql_model.model.block_size)
         device = self.iql_model.device
         bsize, vocab_size = tokens.shape[0], tokenizer.num_tokens()
         n = bsize * beam_width
         if max_generation_len is None:
-            max_generation_len = max_length+1
-        input_strs = [tokenizer.decode(tokens[i, :][:attn_mask[i, :].sum().long()].tolist(), 
-                                       clean_up_tokenization_spaces=False) for i in range(len(tokens))]
+            max_generation_len = max_length + 1
+        input_strs = [
+            tokenizer.decode(
+                tokens[i, :][: attn_mask[i, :].sum().long()].tolist(),
+                clean_up_tokenization_spaces=False,
+            )
+            for i in range(len(tokens))
+        ]
         prefix_t = 0 if prefix_embs is None else prefix_embs.shape[1]
-        model_outputs = self.iql_model(tokens, state_idxs, action_idxs, attn_mask,
-                                       prefix_embs=prefix_embs, prefix_attn_mask=prefix_attn_mask,
-                                       remove_prefix_position_embs=remove_prefix_position_embs,
-                                       is_causal=False)['model_outputs']
-        kvs = {'qv': model_outputs['qv_model_outputs']['past_key_values']}
+        model_outputs = self.iql_model(
+            tokens,
+            state_idxs,
+            action_idxs,
+            attn_mask,
+            prefix_embs=prefix_embs,
+            prefix_attn_mask=prefix_attn_mask,
+            remove_prefix_position_embs=remove_prefix_position_embs,
+            is_causal=False,
+        )["model_outputs"]
+        kvs = {"qv": model_outputs["qv_model_outputs"]["past_key_values"]}
         if self.iql_model.actor_target is not None:
-            kvs['target'] = model_outputs['target_model_outputs']['past_key_values']
+            kvs["target"] = model_outputs["target_model_outputs"]["past_key_values"]
         if self.iql_model.actor is not None:
-            kvs['policy'] = model_outputs['policy_model_outputs']['past_key_values']
+            kvs["policy"] = model_outputs["policy_model_outputs"]["past_key_values"]
         original_dialogue_lens = attn_mask.sum(dim=1)
-        batch_indicator = torch.stack(beam_width*[torch.arange(0, bsize).to(device)], dim=1)
+        batch_indicator = torch.stack(
+            beam_width * [torch.arange(0, bsize).to(device)], dim=1
+        )
 
-        tokens = pad_sequence(torch.repeat_interleave(tokens, beam_width, dim=0), max_length, 
-                              tokenizer.pad_token_id, device, 1)
-        dialogue_lens = torch.repeat_interleave(original_dialogue_lens, beam_width, dim=0)
-        kvs['qv'] = map_all_kvs(lambda x: pad_sequence(torch.repeat_interleave(x, beam_width, dim=0), 
-                                                       max_length, 0.0, device, 2), kvs['qv'])
-        if 'target' in kvs:
-            kvs['target'] = map_all_kvs(lambda x: pad_sequence(torch.repeat_interleave(x, beam_width, dim=0), 
-                                                               max_length, 0.0, device, 2), kvs['target'])
-        if 'policy' in kvs:
-            kvs['policy'] = map_all_kvs(lambda x: pad_sequence(torch.repeat_interleave(x, beam_width, dim=0), 
-                                                               max_length, 0.0, device, 2), kvs['policy'])
+        tokens = pad_sequence(
+            torch.repeat_interleave(tokens, beam_width, dim=0),
+            max_length,
+            tokenizer.pad_token_id,
+            device,
+            1,
+        )
+        dialogue_lens = torch.repeat_interleave(
+            original_dialogue_lens, beam_width, dim=0
+        )
+        kvs["qv"] = map_all_kvs(
+            lambda x: pad_sequence(
+                torch.repeat_interleave(x, beam_width, dim=0),
+                max_length,
+                0.0,
+                device,
+                2,
+            ),
+            kvs["qv"],
+        )
+        if "target" in kvs:
+            kvs["target"] = map_all_kvs(
+                lambda x: pad_sequence(
+                    torch.repeat_interleave(x, beam_width, dim=0),
+                    max_length,
+                    0.0,
+                    device,
+                    2,
+                ),
+                kvs["target"],
+            )
+        if "policy" in kvs:
+            kvs["policy"] = map_all_kvs(
+                lambda x: pad_sequence(
+                    torch.repeat_interleave(x, beam_width, dim=0),
+                    max_length,
+                    0.0,
+                    device,
+                    2,
+                ),
+                kvs["policy"],
+            )
         curr_scores = torch.zeros(bsize, beam_width).to(device)  # (batch, k)
         logit_scores = torch.zeros(bsize, beam_width).to(device)  # (batch, k)
         termination_mask = torch.full((n,), 1).to(device)
-        state_idxs_temp, action_idxs_temp = torch.zeros((dialogue_lens.shape[0], 1,)).long().to(device), torch.zeros(
-            (dialogue_lens.shape[0], 1,)).long().to(device)
+        state_idxs_temp, action_idxs_temp = torch.zeros(
+            (
+                dialogue_lens.shape[0],
+                1,
+            )
+        ).long().to(device), torch.zeros(
+            (
+                dialogue_lens.shape[0],
+                1,
+            )
+        ).long().to(
+            device
+        )
         t = torch.min(dialogue_lens).int()
         base_logits = torch.full((dialogue_lens.shape[0],), 0.0).to(device)
-        while termination_mask.sum() > 0 and (t+prefix_t) < max_length:
-            curr_token = tokens[:, t-1].unsqueeze(1)
-            curr_kvs = map_all_kvs(lambda x: x[:,:,:(t+prefix_t)-1,:], kvs['qv'])
+        while termination_mask.sum() > 0 and (t + prefix_t) < max_length:
+            curr_token = tokens[:, t - 1].unsqueeze(1)
+            curr_kvs = map_all_kvs(
+                lambda x: x[:, :, : (t + prefix_t) - 1, :], kvs["qv"]
+            )
             curr_target_kvs, curr_policy_kvs = curr_kvs, curr_kvs
-            if 'target' in kvs:
-                map_all_kvs(lambda x: x[:,:,:(t+prefix_t)-1,:], kvs['target'])
-            if 'policy' in kvs:
-                map_all_kvs(lambda x: x[:,:,:(t+prefix_t)-1,:], kvs['policy'])
-            iql_outputs = self.iql_model(curr_token, 
-                                         state_idxs_temp, 
-                                         action_idxs_temp, 
-                                         None,
-                                         qv_kwargs={'past_key_values': curr_kvs}, 
-                                         policy_kwargs={'past_key_values': curr_policy_kvs}, 
-                                         target_kwargs={'past_key_values': curr_target_kvs}, 
-                                         is_causal=False)
-            model_outputs, logits = iql_outputs['model_outputs'], iql_outputs['logits']
-            
-            logits[:, 0, tokenizer.pad_token_id] = torch.where(termination_mask == 1, float('-inf'), 1e7)
-            logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(device), tokens[:, t]] = logits[torch.arange(
-                0, n).to(device), torch.full((n,), 0).to(device), tokens[:, t]].masked_fill_(t < dialogue_lens, 1e7)
-            edited_logits = process_logits(logits.clone(), temp=temp, top_k=top_k, top_p=top_p)
-            
-            vs, qs = iql_outputs['target_vs'], iql_outputs['target_qs']
+            if "target" in kvs:
+                map_all_kvs(lambda x: x[:, :, : (t + prefix_t) - 1, :], kvs["target"])
+            if "policy" in kvs:
+                map_all_kvs(lambda x: x[:, :, : (t + prefix_t) - 1, :], kvs["policy"])
+            iql_outputs = self.iql_model(
+                curr_token,
+                state_idxs_temp,
+                action_idxs_temp,
+                None,
+                qv_kwargs={"past_key_values": curr_kvs},
+                policy_kwargs={"past_key_values": curr_policy_kvs},
+                target_kwargs={"past_key_values": curr_target_kvs},
+                is_causal=False,
+            )
+            model_outputs, logits = iql_outputs["model_outputs"], iql_outputs["logits"]
+
+            logits[:, 0, tokenizer.pad_token_id] = torch.where(
+                termination_mask == 1, float("-inf"), 1e7
+            )
+            logits[
+                torch.arange(0, n).to(device),
+                torch.full((n,), 0).to(device),
+                tokens[:, t],
+            ] = logits[
+                torch.arange(0, n).to(device),
+                torch.full((n,), 0).to(device),
+                tokens[:, t],
+            ].masked_fill_(
+                t < dialogue_lens, 1e7
+            )
+            edited_logits = process_logits(
+                logits.clone(), temp=temp, top_k=top_k, top_p=top_p
+            )
+
+            vs, qs = iql_outputs["target_vs"], iql_outputs["target_qs"]
             if exp_adv:
                 adv_logits = adv_weight * (qs - vs.unsqueeze(2))
             else:
                 adv_sign = ((qs - vs.unsqueeze(2)) > 0.0).float()
                 adv_logits = adv_weight * adv_sign + (1 - adv_weight) * (1 - adv_sign)
                 adv_logits = torch.log(adv_logits)
             if adv_clip is not None:
                 adv_logits = torch.clip(adv_logits, max=adv_clip)
-            adv_logits[:, 0, tokenizer.pad_token_id] = torch.where(termination_mask == 1, float('-inf'), 1e7)
-            adv_logits[torch.arange(0, n).to(device), torch.full((n,), 0).to(device), tokens[:, t]] = adv_logits[
-                torch.arange(0, n).to(device), torch.full((n,), 0).to(device), tokens[:, t]].masked_fill_(
-                t < dialogue_lens, 1e7)
-
-            full_logits = (edited_logits if include_logits else 0.0) + (
-                adv_logits if include_adv else 0.0) + base_logits.unsqueeze(1).unsqueeze(2)
-            
-            scores = (torch.log(F.softmax(full_logits, dim=-1)).reshape(1, bsize, beam_width, -1).permute(
-                3, 0, 1, 2) + curr_scores).permute(1, 2, 3, 0).reshape(1, bsize, -1)  # (time, batch, k*vocab)
-            scores[0, :, vocab_size:] = scores[0, :, vocab_size:].masked_fill_((t == original_dialogue_lens).unsqueeze(
-                1).repeat(1, scores.shape[2]-vocab_size), float('-inf'))
-            curr_scores, top_k_ = torch.topk(scores[0, :, :], k=beam_width, dim=1)  # (batch, k), (batch, k)
-            tokens = tokens[(batch_indicator * beam_width + (top_k_ // vocab_size)).reshape(-1), :]
-            logits = logits[(batch_indicator * beam_width + (top_k_ // vocab_size)).reshape(-1), :, :]
-            logit_scores += torch.gather(torch.log(F.softmax(logits, dim=-1)).squeeze(1), dim=1, index=(top_k_.reshape(
-                -1) % vocab_size).unsqueeze(1)).squeeze(1).reshape(-1, beam_width)
+            adv_logits[:, 0, tokenizer.pad_token_id] = torch.where(
+                termination_mask == 1, float("-inf"), 1e7
+            )
+            adv_logits[
+                torch.arange(0, n).to(device),
+                torch.full((n,), 0).to(device),
+                tokens[:, t],
+            ] = adv_logits[
+                torch.arange(0, n).to(device),
+                torch.full((n,), 0).to(device),
+                tokens[:, t],
+            ].masked_fill_(
+                t < dialogue_lens, 1e7
+            )
+
+            full_logits = (
+                (edited_logits if include_logits else 0.0)
+                + (adv_logits if include_adv else 0.0)
+                + base_logits.unsqueeze(1).unsqueeze(2)
+            )
+
+            scores = (
+                (
+                    torch.log(F.softmax(full_logits, dim=-1))
+                    .reshape(1, bsize, beam_width, -1)
+                    .permute(3, 0, 1, 2)
+                    + curr_scores
+                )
+                .permute(1, 2, 3, 0)
+                .reshape(1, bsize, -1)
+            )  # (time, batch, k*vocab)
+            scores[0, :, vocab_size:] = scores[0, :, vocab_size:].masked_fill_(
+                (t == original_dialogue_lens)
+                .unsqueeze(1)
+                .repeat(1, scores.shape[2] - vocab_size),
+                float("-inf"),
+            )
+            curr_scores, top_k_ = torch.topk(
+                scores[0, :, :], k=beam_width, dim=1
+            )  # (batch, k), (batch, k)
+            tokens = tokens[
+                (batch_indicator * beam_width + (top_k_ // vocab_size)).reshape(-1), :
+            ]
+            logits = logits[
+                (batch_indicator * beam_width + (top_k_ // vocab_size)).reshape(-1),
+                :,
+                :,
+            ]
+            logit_scores += (
+                torch.gather(
+                    torch.log(F.softmax(logits, dim=-1)).squeeze(1),
+                    dim=1,
+                    index=(top_k_.reshape(-1) % vocab_size).unsqueeze(1),
+                )
+                .squeeze(1)
+                .reshape(-1, beam_width)
+            )
             tokens[:, t] = top_k_.reshape(-1) % vocab_size  # (batch*k,)
-            fixed_kvs = map_all_kvs(lambda x: x[(batch_indicator * beam_width + torch.div(
-                top_k_, vocab_size, rounding_mode='trunc')).reshape(-1), :, :, :], 
-                model_outputs['qv_model_outputs']['past_key_values'])
-            kvs['qv'] = map_all_kvs(lambda x: x[(batch_indicator * beam_width + torch.div(
-                top_k_, vocab_size, rounding_mode='trunc')).reshape(-1), :, :, :], kvs['qv'])
-            kvs['qv'] = update_kvs(kvs['qv'], fixed_kvs, torch.arange(0, n).to(device), (t+prefix_t)-1)
-            if 'target' in kvs:
-                fixed_target_kvs = map_all_kvs(lambda x: x[(batch_indicator * beam_width + torch.div(
-                    top_k_, vocab_size, rounding_mode='trunc')).reshape(-1), :, :, :], 
-                    model_outputs['target_model_outputs']['past_key_values'])
-                kvs['target'] = map_all_kvs(lambda x: x[(batch_indicator * beam_width + torch.div(
-                    top_k_, vocab_size, rounding_mode='trunc')).reshape(-1), :, :, :], kvs['target'])
-                kvs['target'] = update_kvs(kvs['target'], fixed_target_kvs, torch.arange(0, n).to(device), 
-                                           (t+prefix_t)-1)
-            if 'policy' in kvs:
-                fixed_policy_kvs = map_all_kvs(lambda x: x[(batch_indicator * beam_width + torch.div(
-                    top_k_, vocab_size, rounding_mode='trunc')).reshape(-1), :, :, :], 
-                    model_outputs['policy_model_outputs']['past_key_values'])
-                kvs['policy'] = map_all_kvs(lambda x: x[(batch_indicator * beam_width + torch.div(
-                    top_k_, vocab_size, rounding_mode='trunc')).reshape(-1), :, :, :], kvs['policy'])
-                kvs['policy'] = update_kvs(kvs['policy'], fixed_policy_kvs, torch.arange(0, n).to(device), 
-                                           (t+prefix_t)-1)
-            termination_mask = termination_mask[(batch_indicator * beam_width + (top_k_ // vocab_size)).reshape(-1)]
+            fixed_kvs = map_all_kvs(
+                lambda x: x[
+                    (
+                        batch_indicator * beam_width
+                        + torch.div(top_k_, vocab_size, rounding_mode="trunc")
+                    ).reshape(-1),
+                    :,
+                    :,
+                    :,
+                ],
+                model_outputs["qv_model_outputs"]["past_key_values"],
+            )
+            kvs["qv"] = map_all_kvs(
+                lambda x: x[
+                    (
+                        batch_indicator * beam_width
+                        + torch.div(top_k_, vocab_size, rounding_mode="trunc")
+                    ).reshape(-1),
+                    :,
+                    :,
+                    :,
+                ],
+                kvs["qv"],
+            )
+            kvs["qv"] = update_kvs(
+                kvs["qv"], fixed_kvs, torch.arange(0, n).to(device), (t + prefix_t) - 1
+            )
+            if "target" in kvs:
+                fixed_target_kvs = map_all_kvs(
+                    lambda x: x[
+                        (
+                            batch_indicator * beam_width
+                            + torch.div(top_k_, vocab_size, rounding_mode="trunc")
+                        ).reshape(-1),
+                        :,
+                        :,
+                        :,
+                    ],
+                    model_outputs["target_model_outputs"]["past_key_values"],
+                )
+                kvs["target"] = map_all_kvs(
+                    lambda x: x[
+                        (
+                            batch_indicator * beam_width
+                            + torch.div(top_k_, vocab_size, rounding_mode="trunc")
+                        ).reshape(-1),
+                        :,
+                        :,
+                        :,
+                    ],
+                    kvs["target"],
+                )
+                kvs["target"] = update_kvs(
+                    kvs["target"],
+                    fixed_target_kvs,
+                    torch.arange(0, n).to(device),
+                    (t + prefix_t) - 1,
+                )
+            if "policy" in kvs:
+                fixed_policy_kvs = map_all_kvs(
+                    lambda x: x[
+                        (
+                            batch_indicator * beam_width
+                            + torch.div(top_k_, vocab_size, rounding_mode="trunc")
+                        ).reshape(-1),
+                        :,
+                        :,
+                        :,
+                    ],
+                    model_outputs["policy_model_outputs"]["past_key_values"],
+                )
+                kvs["policy"] = map_all_kvs(
+                    lambda x: x[
+                        (
+                            batch_indicator * beam_width
+                            + torch.div(top_k_, vocab_size, rounding_mode="trunc")
+                        ).reshape(-1),
+                        :,
+                        :,
+                        :,
+                    ],
+                    kvs["policy"],
+                )
+                kvs["policy"] = update_kvs(
+                    kvs["policy"],
+                    fixed_policy_kvs,
+                    torch.arange(0, n).to(device),
+                    (t + prefix_t) - 1,
+                )
+            termination_mask = termination_mask[
+                (batch_indicator * beam_width + (top_k_ // vocab_size)).reshape(-1)
+            ]
             for idx in range(n):
                 if tokens[idx, t] == tokenizer.eoa_token_id and t >= dialogue_lens[idx]:
-                    termination_mask[idx] *= (1 - int(termination_condition(tokenizer.decode(tokens[idx, :].tolist(),
-                                                                                             clean_up_tokenization_spaces=False))))
+                    termination_mask[idx] *= 1 - int(
+                        termination_condition(
+                            tokenizer.decode(
+                                tokens[idx, :].tolist(),
+                                clean_up_tokenization_spaces=False,
+                            )
+                        )
+                    )
             t += 1
-            termination_mask *= ((t-dialogue_lens) < max_generation_len).int()
-        
-        output_strs = [tokenizer.decode(tokens[i, :].tolist(), clean_up_tokenization_spaces=False) for i in range(n)]
+            termination_mask *= ((t - dialogue_lens) < max_generation_len).int()
+
+        output_strs = [
+            tokenizer.decode(tokens[i, :].tolist(), clean_up_tokenization_spaces=False)
+            for i in range(n)
+        ]
         processed_outputs = []
         for i in range(len(input_strs)):
             temp_outputs = []
             for x in range(beam_width):
-                processed_str = output_strs[i*beam_width+x][len(input_strs[i]):].strip()
+                processed_str = output_strs[i * beam_width + x][
+                    len(input_strs[i]) :
+                ].strip()
                 if tokenizer.id_to_token(tokenizer.pad_token_id) in processed_str:
-                    processed_str = processed_str[:processed_str.find(tokenizer.id_to_token(
-                        tokenizer.pad_token_id))].strip()
+                    processed_str = processed_str[
+                        : processed_str.find(
+                            tokenizer.id_to_token(tokenizer.pad_token_id)
+                        )
+                    ].strip()
                 if tokenizer.id_to_token(tokenizer.eoa_token_id) in processed_str:
-                    processed_str = processed_str[:processed_str.find(tokenizer.id_to_token(
-                        tokenizer.eoa_token_id))].strip()
+                    processed_str = processed_str[
+                        : processed_str.find(
+                            tokenizer.id_to_token(tokenizer.eoa_token_id)
+                        )
+                    ].strip()
                 temp_outputs.append(processed_str)
             processed_outputs.append(temp_outputs)
         return list(zip(input_strs, processed_outputs)), curr_scores, -logit_scores
 
-    def generate(self, items, 
-                 termination_condition: Callable[[np.ndarray], bool], **kwargs):
+    def generate(
+        self, items, termination_condition: Callable[[np.ndarray], bool], **kwargs
+    ):
         prepared_inputs = self.iql_model.prepare_inputs(items)
-        tokens, attn_mask = prepared_inputs['tokens'], prepared_inputs['attn_mask']
-        state_idxs, action_idxs = prepared_inputs['state_idxs'], prepared_inputs['action_idxs']
-        if self.kind == 'beam':
+        tokens, attn_mask = prepared_inputs["tokens"], prepared_inputs["attn_mask"]
+        state_idxs, action_idxs = (
+            prepared_inputs["state_idxs"],
+            prepared_inputs["action_idxs"],
+        )
+        if self.kind == "beam":
             method = self.beam_raw
-        elif self.kind == 'sample':
+        elif self.kind == "sample":
             method = self.sample_raw
         else:
             raise NotImplementedError
-        generations, info, kls = method(tokens, attn_mask, 
-                                             state_idxs, action_idxs, 
-                                             termination_condition, 
-                                             **kwargs)
+        generations, info, kls = method(
+            tokens, attn_mask, state_idxs, action_idxs, termination_condition, **kwargs
+        )
         return generations, info, kls
-    
+
     def act(self, obs):
-        item = DataPoint.from_obs(obs, self.iql_model.dataset.tokenizer, self.iql_model.dataset.token_reward)
-        generations, logprobs, kls = self.generate([item], always_terminate, **self.generation_kwargs)
+        item = DataPoint.from_obs(
+            obs, self.iql_model.dataset.tokenizer, self.iql_model.dataset.token_reward
+        )
+        generations, logprobs, kls = self.generate(
+            [item], always_terminate, **self.generation_kwargs
+        )
         self.kls_all.append(kls[0, 0].item())
         self.logprobs_all.append(logprobs[0, 0].item())
         return generations[0][1][0]
-    
+
     def train(self):
         self.iql_model.train()
-    
+
     def eval(self):
         self.iql_model.eval()
 
-class ILQL_Evaluator():
+
+class ILQL_Evaluator:
     def __init__(self, env, verbose: bool, kind: str, **generation_kwargs) -> None:
         super().__init__()
         self.env = env
         self.verbose = verbose
         self.kind = kind
         self.generation_kwargs = generation_kwargs
         self.all_results = []
         self.all_entropy = []
-    
+
     def evaluate(self, model: ILQL, items):
         policy = ILQL_Policy(model, self.kind, **self.generation_kwargs)
-        tokens = model.prepare_inputs(items)['tokens']
+        tokens = model.prepare_inputs(items)["tokens"]
         total_token_reward = 0
         total_env_reward = 0
         for i in range(tokens.shape[0]):
             result, sequence = interact_environment(self.env, policy, None)
-            self.all_results.append((result, sequence,))
+            self.all_results.append(
+                (
+                    result,
+                    sequence,
+                )
+            )
             env_reward = sum(map(lambda x: x[2], sequence))
-            token_reward = sum(DataPoint.get_token_reward(result, model.dataset.tokenizer, model.dataset.token_reward))
+            token_reward = sum(
+                DataPoint.get_token_reward(
+                    result, model.dataset.tokenizer, model.dataset.token_reward
+                )
+            )
             total_env_reward += env_reward
             total_token_reward += token_reward
             if self.verbose:
                 print(result)
-                print('='*25)
-                print('token reward:', token_reward)
-                print('env reward:', env_reward)
-                print('avg token reward:', total_token_reward / (i + 1))
-                print('avg env reward:', total_env_reward / (i + 1))
-                print('='*25)
+                print("=" * 25)
+                print("token reward:", token_reward)
+                print("env reward:", env_reward)
+                print("avg token reward:", total_token_reward / (i + 1))
+                print("avg env reward:", total_env_reward / (i + 1))
+                print("=" * 25)
         kl_total = sum(policy.kls_all)
         entropy_total = -sum(policy.logprobs_all)
         self.all_entropy.extend(policy.logprobs_all)
-        return {'token_reward': (total_token_reward / tokens.shape[0], tokens.shape[0]), 'env_reward': (
-            total_env_reward / tokens.shape[0], tokens.shape[0]), 'kl': (kl_total / len(policy.kls_all), len(
-            policy.kls_all)), 
-                'entropy': (entropy_total / len(policy.logprobs_all), len(policy.logprobs_all))}
-    
+        return {
+            "token_reward": (total_token_reward / tokens.shape[0], tokens.shape[0]),
+            "env_reward": (total_env_reward / tokens.shape[0], tokens.shape[0]),
+            "kl": (kl_total / len(policy.kls_all), len(policy.kls_all)),
+            "entropy": (
+                entropy_total / len(policy.logprobs_all),
+                len(policy.logprobs_all),
+            ),
+        }
+
     def dump(self):
-        return {'results': self.all_results, 'entropies': self.all_entropy}
+        return {"results": self.all_results, "entropies": self.all_entropy}
 
 
-class TopAdvantageNGrams():
+class TopAdvantageNGrams:
     def __init__(self, data, print_every, print_k, n_gram):
         self.data = data
         self.print_every = print_every
         self.print_k = print_k
         self.n_gram = n_gram
-    
+
     def evaluate(self, model, items):
         top_actions = defaultdict(float)
         total_actions = defaultdict(int)
         for i in tqdm(range(self.data.size())):
             item = self.data.get_item(i)
             prepared_inputs = model.prepare_inputs([item])
-            tokens, a_idx = prepared_inputs['tokens'], prepared_inputs['action_idxs']
+            tokens, a_idx = prepared_inputs["tokens"], prepared_inputs["action_idxs"]
             model_outputs = model.get_qvs([item])
             select_tokens = torch.gather(tokens[0, 1:], dim=0, index=a_idx[0, :])
-            advantages = model_outputs['target_qs'][0, :] - model_outputs['target_vs'][0, :]
+            advantages = (
+                model_outputs["target_qs"][0, :] - model_outputs["target_vs"][0, :]
+            )
             curr_idx = 0
             for x, token in enumerate(select_tokens):
                 start_idx = curr_idx
                 if self.n_gram is not None:
-                    if x-self.n_gram >= 0 and a_idx[0, x-self.n_gram].item() > a_idx[0, start_idx].item():
-                        start_idx = x-self.n_gram
-                    if x-start_idx < self.n_gram:
+                    if (
+                        x - self.n_gram >= 0
+                        and a_idx[0, x - self.n_gram].item()
+                        > a_idx[0, start_idx].item()
+                    ):
+                        start_idx = x - self.n_gram
+                    if x - start_idx < self.n_gram:
                         continue
                 elif select_tokens[x].item() != self.data.tokenizer.eoa_token_id:
                     continue
                 total_advantage = advantages[start_idx:x].sum().item()
-                utterance = self.data.tokenizer.decode(tokens[0, (
-                    a_idx[0, start_idx].item()+1):(a_idx[0, x].item()+1)].detach().cpu().tolist())
+                utterance = self.data.tokenizer.decode(
+                    tokens[
+                        0, (a_idx[0, start_idx].item() + 1) : (a_idx[0, x].item() + 1)
+                    ]
+                    .detach()
+                    .cpu()
+                    .tolist()
+                )
                 top_actions[utterance] += total_advantage
                 total_actions[utterance] += 1
                 if select_tokens[x].item() == self.data.tokenizer.eoa_token_id:
-                    curr_idx = x+1
+                    curr_idx = x + 1
             if i % self.print_every == 0:
                 ranked_actions = sorted(
-                    {k: top_actions[k] / total_actions[k] for k in total_actions.keys()}.items(), key=lambda x: x[1])
-                print(ranked_actions[-self.print_k:])
-                print(ranked_actions[:self.print_k])
+                    {
+                        k: top_actions[k] / total_actions[k]
+                        for k in total_actions.keys()
+                    }.items(),
+                    key=lambda x: x[1],
+                )
+                print(ranked_actions[-self.print_k :])
+                print(ranked_actions[: self.print_k])
+
 
 def interact_environment(env, policy, obs):
     obs_sequence = []
     if obs is None:
         obs = env.reset()
     while not env.is_terminal():
         action = policy.act(obs)
         new_obs, r, t = env.step(action)
         obs_sequence.append((obs, action, r, t))
         obs = new_obs
     obs_sequence.append((obs, None, 0, True))
     return obs, obs_sequence
 
-def map_pytree(f: Callable[[Union[np.ndarray, torch.Tensor]], Any],
-               item: Any):
+
+def map_pytree(f: Callable[[Union[np.ndarray, torch.Tensor]], Any], item: Any):
     if isinstance(item, dict):
         return {k: map_pytree(f, v) for k, v in item.items()}
     elif isinstance(item, list) or isinstance(item, set) or isinstance(item, tuple):
         return [map_pytree(f, v) for v in item]
     elif isinstance(item, np.ndarray) or isinstance(item, torch.Tensor):
         return f(item)
     else:
         return item
 
+
 def to(item: Any, device: torch.device):
     return map_pytree(lambda x: torch.tensor(x).to(device), item)
 
+
 def to_decorator(f, device):
     def new_f(*args, **kwargs):
         return to(f(*args, **kwargs), device)
+
     return new_f
 
+
 def parameter_norm(model: nn.Module):
     norm = 0.0
     for param in model.parameters():
         norm += (param.norm() ** 2).item()
     return math.sqrt(norm)
```

### Comparing `agilerl-0.1.8/agilerl/algorithms/maddpg.py` & `agilerl-0.1.9/agilerl/algorithms/maddpg.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-import random
 import copy
+import random
+
 import dill
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.optim as optim
-from agilerl.networks.evolvable_mlp import EvolvableMLP
+
 from agilerl.networks.evolvable_cnn import EvolvableCNN
+from agilerl.networks.evolvable_mlp import EvolvableMLP
 
 
-class MADDPG():
+class MADDPG:
     """The MADDPG algorithm class. MADDPG paper: https://arxiv.org/abs/1706.02275
 
     :param state_dims: State observation dimensions for each agent
     :type state_dims: List[tuple]
     :param action_dims: Action dimensions for each agent
     :type action_dims: List[int]
     :param one_hot: One-hot encoding, used with discrete observation spaces
@@ -50,19 +52,38 @@
     :type device: str, optional
     :param accelerator: Accelerator for distributed computing, defaults to None
     :type accelerator: Hugging Face accelerate.Accelerator(), optional
     :param wrap: Wrap models for distributed training upon creation, defaults to True
     :type wrap: bool, optional
     """
 
-    def __init__(self, state_dims, action_dims, one_hot, n_agents, agent_ids, max_action, 
-                 min_action, discrete_actions, expl_noise=0.1, index=0,  
-                 net_config={'arch': 'mlp', 'h_size': [64,64]}, batch_size=64, lr=0.01,
-                 learn_step=5, gamma=0.95, tau=0.01, mutation=None, device="cpu", accelerator=None, wrap=True):
-        self.algo = 'MADDPG'
+    def __init__(
+        self,
+        state_dims,
+        action_dims,
+        one_hot,
+        n_agents,
+        agent_ids,
+        max_action,
+        min_action,
+        discrete_actions,
+        expl_noise=0.1,
+        index=0,
+        net_config={"arch": "mlp", "h_size": [64, 64]},
+        batch_size=64,
+        lr=0.01,
+        learn_step=5,
+        gamma=0.95,
+        tau=0.01,
+        mutation=None,
+        device="cpu",
+        accelerator=None,
+        wrap=True,
+    ):
+        self.algo = "MADDPG"
         self.state_dims = state_dims
         self.total_state_dims = sum(state_dim[0] for state_dim in self.state_dims)
         self.action_dims = action_dims
         self.one_hot = one_hot
         self.n_agents = n_agents
         self.multi = True if n_agents > 1 else False
         self.agent_ids = agent_ids
@@ -79,95 +100,123 @@
         self.scores = []
         self.fitness = []
         self.steps = [0]
         self.max_action = max_action
         self.expl_noise = expl_noise
         self.min_action = min_action
         self.discrete_actions = discrete_actions
-        self.total_actions = sum(self.action_dims) if not self.discrete_actions else len(self.action_dims)
+        self.total_actions = (
+            sum(self.action_dims)
+            if not self.discrete_actions
+            else len(self.action_dims)
+        )
 
-        if 'output_activation' in self.net_config.keys():
+        if "output_activation" in self.net_config.keys():
             pass
         else:
             if self.discrete_actions:
-                self.net_config['output_activation'] = 'gumbel_softmax'
+                self.net_config["output_activation"] = "gumbel_softmax"
             else:
-                self.net_config['output_activation'] = 'softmax'
+                self.net_config["output_activation"] = "softmax"
 
         # model
-        if self.net_config['arch'] == 'mlp':      # Multi-layer Perceptron
-            self.actors = [EvolvableMLP(
-                num_inputs=state_dim[0],
-                num_outputs=action_dim,
-                hidden_size=self.net_config['h_size'],
-                output_activation=self.net_config['output_activation'],
-                device=self.device,
-                accelerator=self.accelerator) for (action_dim, state_dim) in zip(self.action_dims, self.state_dims)]
+        if self.net_config["arch"] == "mlp":  # Multi-layer Perceptron
+            self.actors = [
+                EvolvableMLP(
+                    num_inputs=state_dim[0],
+                    num_outputs=action_dim,
+                    hidden_size=self.net_config["h_size"],
+                    output_activation=self.net_config["output_activation"],
+                    device=self.device,
+                    accelerator=self.accelerator,
+                )
+                for (action_dim, state_dim) in zip(self.action_dims, self.state_dims)
+            ]
             self.actor_targets = copy.deepcopy(self.actors)
 
-            self.critics = [EvolvableMLP(
-                num_inputs=self.total_state_dims + self.total_actions, 
-                num_outputs=1,
-                hidden_size=self.net_config['h_size'],
-                device=self.device,
-                accelerator=self.accelerator) for _ in range(self.n_agents)]
+            self.critics = [
+                EvolvableMLP(
+                    num_inputs=self.total_state_dims + self.total_actions,
+                    num_outputs=1,
+                    hidden_size=self.net_config["h_size"],
+                    device=self.device,
+                    accelerator=self.accelerator,
+                )
+                for _ in range(self.n_agents)
+            ]
             self.critic_targets = copy.deepcopy(self.critics)
 
-        elif self.net_config['arch'] == 'cnn':    # Convolutional Neural Network
-            self.actors = [EvolvableCNN(
-                input_shape=state_dim,
-                num_actions=action_dim,
-                channel_size=self.net_config['c_size'],
-                kernal_size=self.net_config['k_size'],
-                stride_size=self.net_config['s_size'],
-                hidden_size=self.net_config['h_size'],
-                normalize=self.net_config['normalize'],
-                mlp_activation=self.net_config['output_activation'],
-                multi=self.multi,
-                n_agents=self.n_agents,
-                device=self.device,
-                accelerator=self.accelerator) for (action_dim, state_dim) in zip(self.action_dims, self.state_dims)]
+        elif self.net_config["arch"] == "cnn":  # Convolutional Neural Network
+            self.actors = [
+                EvolvableCNN(
+                    input_shape=state_dim,
+                    num_actions=action_dim,
+                    channel_size=self.net_config["c_size"],
+                    kernal_size=self.net_config["k_size"],
+                    stride_size=self.net_config["s_size"],
+                    hidden_size=self.net_config["h_size"],
+                    normalize=self.net_config["normalize"],
+                    mlp_activation=self.net_config["output_activation"],
+                    multi=self.multi,
+                    n_agents=self.n_agents,
+                    device=self.device,
+                    accelerator=self.accelerator,
+                )
+                for (action_dim, state_dim) in zip(self.action_dims, self.state_dims)
+            ]
             self.actor_targets = copy.deepcopy(self.actors)
 
-            self.critics = [EvolvableCNN(
-                input_shape=state_dim, 
-                num_actions=self.total_actions,
-                channel_size=self.net_config['c_size'],
-                kernal_size=self.net_config['k_size'],
-                stride_size=self.net_config['s_size'],
-                hidden_size=self.net_config['h_size'],
-                normalize=self.net_config['normalize'],
-                mlp_activation='tanh',
-                critic=True,
-                n_agents=self.n_agents,
-                multi=self.multi,
-                device=self.device,
-                accelerator=self.accelerator) for state_dim in self.state_dims]
+            self.critics = [
+                EvolvableCNN(
+                    input_shape=state_dim,
+                    num_actions=self.total_actions,
+                    channel_size=self.net_config["c_size"],
+                    kernal_size=self.net_config["k_size"],
+                    stride_size=self.net_config["s_size"],
+                    hidden_size=self.net_config["h_size"],
+                    normalize=self.net_config["normalize"],
+                    mlp_activation="tanh",
+                    critic=True,
+                    n_agents=self.n_agents,
+                    multi=self.multi,
+                    device=self.device,
+                    accelerator=self.accelerator,
+                )
+                for state_dim in self.state_dims
+            ]
             self.critic_targets = copy.deepcopy(self.critics)
 
-        self.actor_optimizers_type = [optim.Adam(actor.parameters(), lr=self.lr) for actor in self.actors]
-        self.critic_optimizers_type = [optim.Adam(critic.parameters(), lr=self.lr) for critic in self.critics]
+        self.actor_optimizers_type = [
+            optim.Adam(actor.parameters(), lr=self.lr) for actor in self.actors
+        ]
+        self.critic_optimizers_type = [
+            optim.Adam(critic.parameters(), lr=self.lr) for critic in self.critics
+        ]
 
         if self.accelerator is not None:
             self.actor_optimizers = self.actor_optimizers_type
             self.critic_optimizers = self.critic_optimizers_type
             if wrap:
-                self.wrap_models()          
+                self.wrap_models()
         else:
             self.actors = [actor.to(self.device) for actor in self.actors]
-            self.actor_targets = [actor_target.to(self.device) for actor_target in self.actor_targets]
+            self.actor_targets = [
+                actor_target.to(self.device) for actor_target in self.actor_targets
+            ]
             self.critics = [critic.to(self.device) for critic in self.critics]
-            self.critic_targets = [critic_target.to(self.device) for critic_target in self.critic_targets]
+            self.critic_targets = [
+                critic_target.to(self.device) for critic_target in self.critic_targets
+            ]
             self.actor_optimizers = self.actor_optimizers_type
             self.critic_optimizers = self.critic_optimizers_type
 
         self.criterion = nn.MSELoss()
 
     def getAction(self, states, epsilon=0):
-        """Returns the next action to take in the environment. 
+        """Returns the next action to take in the environment.
         Epsilon is the probability of taking a random action, used for exploration.
         For epsilon-greedy behaviour, set epsilon to 0.
 
         :param state: Environment observations: {'agent_0': state_dim_0, ..., 'agent_n': state_dim_n}
         :type state: Dict[str, numpy.Array]
         :param epsilon: Probablilty of taking a random action for exploration, defaults to 0
         :type epsilon: float, optional
@@ -176,193 +225,260 @@
         states = [torch.from_numpy(state).float() for state in states.values()]
 
         # Configure accelerator
         if self.accelerator is None:
             states = [state.to(self.device) for state in states]
 
         if self.one_hot:
-            states = [nn.functional.one_hot(
-                state.long(), num_classes=state_dim[0]).float().squeeze() for state, state_dim 
-                in zip(states, self.state_dims)]
-        
+            states = [
+                nn.functional.one_hot(state.long(), num_classes=state_dim[0])
+                .float()
+                .squeeze()
+                for state, state_dim in zip(states, self.state_dims)
+            ]
+
         if self.net_config["arch"] == "mlp":
-            states = [state.unsqueeze(0) if len(state.size()) < 2 else state for state in states]   
+            states = [
+                state.unsqueeze(0) if len(state.size()) < 2 else state
+                for state in states
+            ]
         elif self.net_config["arch"] == "cnn":
             states = [state.unsqueeze(2) for state in states]
 
-        actions = {} 
-        for idx, (agent_id, state, actor) in enumerate(zip(self.agent_ids, states, self.actors)):
+        actions = {}
+        for idx, (agent_id, state, actor) in enumerate(
+            zip(self.agent_ids, states, self.actors)
+        ):
             if random.random() < epsilon:
                 if self.discrete_actions:
                     action = np.random.randint(0, self.action_dims[idx])
                 else:
-                    action = np.random.rand(state.size()[0], self.action_dims[idx]).astype('float32').squeeze()
+                    action = (
+                        np.random.rand(state.size()[0], self.action_dims[idx])
+                        .astype("float32")
+                        .squeeze()
+                    )
             else:
                 actor.eval()
                 if self.accelerator is not None:
                     with actor.no_sync():
                         action_values = actor(state)
                 else:
                     with torch.no_grad():
                         action_values = actor(state)
                 actor.train()
                 if self.discrete_actions:
                     action = action_values.squeeze(0).argmax().item()
                 else:
-                    action = action_values.cpu().data.numpy().squeeze() \
-                         + np.random.normal(0, self.max_action[idx][0] * self.expl_noise, size=self.action_dims[idx]).astype(np.float32)
-                    action = np.clip(action, self.min_action[idx][0], self.max_action[idx][0])     
+                    action = (
+                        action_values.cpu().data.numpy().squeeze()
+                        + np.random.normal(
+                            0,
+                            self.max_action[idx][0] * self.expl_noise,
+                            size=self.action_dims[idx],
+                        ).astype(np.float32)
+                    )
+                    action = np.clip(
+                        action, self.min_action[idx][0], self.max_action[idx][0]
+                    )
             actions[agent_id] = action
-        
+
         return actions
-    
+
     def _squeeze_exp(self, experiences):
         """Remove first dim created by dataloader.
-        
+
         :param experiences: List of batched states, actions, rewards, next_states, dones in that order.
         :type state: List[torch.Tensor[float]]
         """
         st, ac, re, ne, do = experiences
         return st.squeeze(0), ac.squeeze(0), re.squeeze(0), ne.squeeze(0), do.squeeze(0)
 
     def learn(self, experiences):
         """Updates agent network parameters to learn from experiences.
 
-        :param experience: Tuple of dictionaries containing batched states, actions, rewards, next_states, 
+        :param experience: Tuple of dictionaries containing batched states, actions, rewards, next_states,
         dones in that order for each individual agent.
         :type experience: Tuple[Dict[str, torch.Tensor]]
         """
 
-        for agent_id, actor, actor_target, critic, critic_target, actor_optimizer, critic_optimizer in zip(self.agent_ids,
-                                                                                                 self.actors,    
-                                                                                                 self.actor_targets,
-                                                                                                 self.critics, 
-                                                                                                 self.critic_targets,
-                                                                                                 self.actor_optimizers, 
-                                                                                                 self.critic_optimizers):
-         
+        for (
+            agent_id,
+            actor,
+            actor_target,
+            critic,
+            critic_target,
+            actor_optimizer,
+            critic_optimizer,
+        ) in zip(
+            self.agent_ids,
+            self.actors,
+            self.actor_targets,
+            self.critics,
+            self.critic_targets,
+            self.actor_optimizers,
+            self.critic_optimizers,
+        ):
             states, actions, rewards, next_states, dones = experiences
-            
-            if self.one_hot:
-                states = {agent_id: nn.functional.one_hot(state.long(), num_classes=state_dim[0]).float().squeeze() for 
-                          agent_id, state, state_dim in zip(states.items(), self.state_dims)}
 
+            if self.one_hot:
+                states = {
+                    agent_id: nn.functional.one_hot(
+                        state.long(), num_classes=state_dim[0]
+                    )
+                    .float()
+                    .squeeze()
+                    for agent_id, state, state_dim in zip(
+                        states.items(), self.state_dims
+                    )
+                }
 
-            if self.net_config['arch'] == 'mlp':
+            if self.net_config["arch"] == "mlp":
                 if self.discrete_actions:
                     action_values = [a.unsqueeze(1) for a in actions.values()]
                 else:
                     action_values = list(actions.values())
                 input_combined = torch.cat(list(states.values()) + action_values, 1)
                 if self.accelerator is not None:
                     with critic.no_sync():
                         q_value = critic(input_combined)
                 else:
                     q_value = critic(input_combined)
-                next_actions = [self.actor_targets[idx](next_states[agent_id]).detach_() for idx, agent_id in enumerate(self.agent_ids)]
-                
-            elif self.net_config['arch'] == 'cnn':
+                next_actions = [
+                    self.actor_targets[idx](next_states[agent_id]).detach_()
+                    for idx, agent_id in enumerate(self.agent_ids)
+                ]
+
+            elif self.net_config["arch"] == "cnn":
                 stacked_states = torch.stack(list(states.values()), dim=2)
                 stacked_actions = torch.stack(list(actions.values()), dim=1)
                 if self.accelerator is not None:
                     with critic.no_sync():
                         q_value = critic(stacked_states, stacked_actions)
                 else:
                     q_value = critic(stacked_states, stacked_actions)
-                next_actions = [self.actor_targets[idx](next_states[agent_id].unsqueeze(2)).detach_() for idx, agent_id in enumerate(self.agent_ids)]
-            
-            if self.discrete_actions:
-                next_actions = [torch.argmax(agent_actions, dim=1).unsqueeze(1) if  self.net_config['arch'] == 'mlp' else
-                                torch.argmax(agent_actions, dim=1) for agent_actions in next_actions]
+                next_actions = [
+                    self.actor_targets[idx](
+                        next_states[agent_id].unsqueeze(2)
+                    ).detach_()
+                    for idx, agent_id in enumerate(self.agent_ids)
+                ]
 
-            if self.net_config['arch'] == 'mlp':
-                next_input_combined = torch.cat(list(next_states.values()) + next_actions, 1)
+            if self.discrete_actions:
+                next_actions = [
+                    torch.argmax(agent_actions, dim=1).unsqueeze(1)
+                    if self.net_config["arch"] == "mlp"
+                    else torch.argmax(agent_actions, dim=1)
+                    for agent_actions in next_actions
+                ]
+
+            if self.net_config["arch"] == "mlp":
+                next_input_combined = torch.cat(
+                    list(next_states.values()) + next_actions, 1
+                )
                 if self.accelerator is not None:
                     with critic_target.no_sync():
                         q_value_next_state = critic_target(next_input_combined)
                 else:
                     q_value_next_state = critic_target(next_input_combined)
-            elif self.net_config['arch'] == 'cnn':
+            elif self.net_config["arch"] == "cnn":
                 stacked_next_states = torch.stack(list(next_states.values()), dim=2)
                 stacked_next_actions = torch.stack(next_actions, dim=1)
                 if self.accelerator is not None:
                     with critic_target.no_sync():
-                        q_value_next_state = critic_target(stacked_next_states, stacked_next_actions)
-                else:
-                    q_value_next_state = critic_target(stacked_next_states, stacked_next_actions)
-
-            y_j = rewards[agent_id] + (1 - dones[agent_id]) * self.gamma * q_value_next_state
+                        q_value_next_state = critic_target(
+                            stacked_next_states, stacked_next_actions
+                        )
+                else:
+                    q_value_next_state = critic_target(
+                        stacked_next_states, stacked_next_actions
+                    )
+
+            y_j = (
+                rewards[agent_id]
+                + (1 - dones[agent_id]) * self.gamma * q_value_next_state
+            )
 
             critic_loss = self.criterion(q_value, y_j.detach_())
 
             # critic loss backprop
             critic_optimizer.zero_grad()
             if self.accelerator is not None:
                 self.accelerator.backward(critic_loss)
             else:
                 critic_loss.backward()
             critic_optimizer.step()
 
-            # update actor and targets 
-            if self.net_config['arch'] == 'mlp':
+            # update actor and targets
+            if self.net_config["arch"] == "mlp":
                 if self.accelerator is not None:
                     with actor.no_sync():
                         action = actor(states[agent_id])
                 else:
                     action = actor(states[agent_id])
                 detached_actions = copy.deepcopy(actions)
                 if self.discrete_actions:
                     action = action.argmax(1).unsqueeze(1)
-                    detached_actions = {agent_id: d.unsqueeze(1) for agent_id, d in detached_actions.items()}
+                    detached_actions = {
+                        agent_id: d.unsqueeze(1)
+                        for agent_id, d in detached_actions.items()
+                    }
                 detached_actions[agent_id] = action
-                input_combined = torch.cat(list(states.values()) + list(detached_actions.values()), 1)
+                input_combined = torch.cat(
+                    list(states.values()) + list(detached_actions.values()), 1
+                )
                 if self.accelerator is not None:
                     with critic.no_sync():
                         actor_loss = -critic(input_combined).mean()
                 else:
                     actor_loss = -critic(input_combined).mean()
 
-            elif self.net_config['arch'] == 'cnn':
+            elif self.net_config["arch"] == "cnn":
                 if self.accelerator is not None:
                     with actor.no_sync():
                         action = actor(states[agent_id].unsqueeze(2))
                 else:
                     action = actor(states[agent_id].unsqueeze(2))
                 if self.discrete_actions:
                     action = action.argmax(1)
                 detached_actions = copy.deepcopy(actions)
                 detached_actions[agent_id] = action
-                stacked_detached_actions = torch.stack(list(detached_actions.values()), dim=1)
+                stacked_detached_actions = torch.stack(
+                    list(detached_actions.values()), dim=1
+                )
                 if self.accelerator is not None:
                     with critic.no_sync():
-                        actor_loss = - \
-                            critic(stacked_states, stacked_detached_actions).mean()
-                else:
-                    actor_loss = - \
-                            critic(stacked_states, stacked_detached_actions).mean()
+                        actor_loss = -critic(
+                            stacked_states, stacked_detached_actions
+                        ).mean()
+                else:
+                    actor_loss = -critic(
+                        stacked_states, stacked_detached_actions
+                    ).mean()
 
             # actor loss backprop
             actor_optimizer.zero_grad()
             if self.accelerator is not None:
                 self.accelerator.backward(actor_loss)
             else:
                 actor_loss.backward()
             actor_optimizer.step()
 
-        for actor, actor_target, critic, critic_target in zip(self.actors, self.actor_targets, 
-                                                                self.critics, self.critic_targets):
+        for actor, actor_target, critic, critic_target in zip(
+            self.actors, self.actor_targets, self.critics, self.critic_targets
+        ):
             self.softUpdate(actor, actor_target)
             self.softUpdate(critic, critic_target)
 
     def softUpdate(self, net, target):
-        """Soft updates target network.
-        """
+        """Soft updates target network."""
         for eval_param, target_param in zip(net.parameters(), target.parameters()):
             target_param.data.copy_(
-                self.tau * eval_param.data + (1.0 - self.tau) * target_param.data)
+                self.tau * eval_param.data + (1.0 - self.tau) * target_param.data
+            )
 
     def test(self, env, swap_channels=False, max_steps=500, loop=3):
         """Returns mean test score of agent in environment with epsilon-greedy policy.
 
         :param env: The environment to be tested in
         :type env: Gym-style environment
         :param swap_channels: Swap image channels dimension from last to first [H, W, C] -> [C, H, W], defaults to False
@@ -376,19 +492,22 @@
             rewards = []
             for i in range(loop):
                 state, _ = env.reset()
                 agent_reward = {agent_id: 0 for agent_id in self.agent_ids}
                 score = 0
                 for _ in range(max_steps):
                     if swap_channels:
-                        state = {agent_id: np.moveaxis(np.expand_dims(s, 0), [3], [1]) for agent_id, s in state.items()}
+                        state = {
+                            agent_id: np.moveaxis(np.expand_dims(s, 0), [3], [1])
+                            for agent_id, s in state.items()
+                        }
                     action = self.getAction(state, epsilon=0)
                     state, reward, done, trunc, info = env.step(action)
                     for agent_id, r in reward.items():
-                        agent_reward[agent_id] += r 
+                        agent_reward[agent_id] += r
                     score = sum(agent_reward.values())
                 rewards.append(score)
         mean_fit = np.mean(rewards)
         self.fitness.append(mean_fit)
         return mean_fit
 
     def clone(self, index=None, wrap=True):
@@ -396,188 +515,302 @@
 
         :param index: Index to keep track of agent for tournament selection and mutation, defaults to None
         :type index: int, optional
         """
         if index is None:
             index = self.index
 
-        clone = type(self)(state_dims=self.state_dims,
-                           action_dims=self.action_dims,
-                           one_hot=self.one_hot,
-                           n_agents=self.n_agents,
-                           agent_ids=self.agent_ids,
-                           max_action=self.max_action,
-                           min_action=self.min_action,
-                           expl_noise=self.expl_noise,
-                           discrete_actions=self.discrete_actions,
-                           index=index,
-                           net_config=self.net_config,
-                           batch_size=self.batch_size,
-                           lr=self.lr,
-                           learn_step=self.learn_step,
-                           gamma=self.gamma,
-                           tau=self.tau,
-                           mutation=self.mut,
-                           device=self.device,
-                           accelerator=self.accelerator,
-                           wrap=wrap)
-        
+        clone = type(self)(
+            state_dims=self.state_dims,
+            action_dims=self.action_dims,
+            one_hot=self.one_hot,
+            n_agents=self.n_agents,
+            agent_ids=self.agent_ids,
+            max_action=self.max_action,
+            min_action=self.min_action,
+            expl_noise=self.expl_noise,
+            discrete_actions=self.discrete_actions,
+            index=index,
+            net_config=self.net_config,
+            batch_size=self.batch_size,
+            lr=self.lr,
+            learn_step=self.learn_step,
+            gamma=self.gamma,
+            tau=self.tau,
+            mutation=self.mut,
+            device=self.device,
+            accelerator=self.accelerator,
+            wrap=wrap,
+        )
+
         if self.accelerator is not None:
             self.unwrap_models()
         actors = [actor.clone() for actor in self.actors]
         actor_targets = [actor_target.clone() for actor_target in self.actor_targets]
         critics = [critic.clone() for critic in self.critics]
-        critic_targets = [critic_target.clone() for critic_target in self.critic_targets]
-        actor_optimizers = [optim.Adam(actor.parameters(), lr=clone.lr) for actor in actors]
-        critic_optimizers = [optim.Adam(critic.parameters(), lr=clone.lr) for critic in critics]
+        critic_targets = [
+            critic_target.clone() for critic_target in self.critic_targets
+        ]
+        actor_optimizers = [
+            optim.Adam(actor.parameters(), lr=clone.lr) for actor in actors
+        ]
+        critic_optimizers = [
+            optim.Adam(critic.parameters(), lr=clone.lr) for critic in critics
+        ]
         clone.actor_optimizers_type = actor_optimizers
         clone.critic_optimizers_type = critic_optimizers
 
         if self.accelerator is not None:
             if wrap:
                 clone.actors = [self.accelerator.prepare(actor) for actor in actors]
-                clone.actor_targets = [self.accelerator.prepare(actor_target) for actor_target in actor_targets]
+                clone.actor_targets = [
+                    self.accelerator.prepare(actor_target)
+                    for actor_target in actor_targets
+                ]
                 clone.critics = [self.accelerator.prepare(critic) for critic in critics]
-                clone.critic_targets = [self.accelerator.prepare(critic_target) for critic_target in critic_targets]
-                clone.actor_optimizers = [self.accelerator.prepare(actor_optimizer) for actor_optimizer in actor_optimizers]
-                clone.critic_optimizers = [self.accelerator.prepare(critic_optimizer) for critic_optimizer in critic_optimizers]
+                clone.critic_targets = [
+                    self.accelerator.prepare(critic_target)
+                    for critic_target in critic_targets
+                ]
+                clone.actor_optimizers = [
+                    self.accelerator.prepare(actor_optimizer)
+                    for actor_optimizer in actor_optimizers
+                ]
+                clone.critic_optimizers = [
+                    self.accelerator.prepare(critic_optimizer)
+                    for critic_optimizer in critic_optimizers
+                ]
             else:
-                clone.actors, clone.actor_targets, clone.critics, clone.critic_targets, \
-                clone.actor_optimizer, clone.critic_optimizer = actors, actor_targets, critics, \
-                critic_targets, actor_optimizers, critic_optimizers
+                (
+                    clone.actors,
+                    clone.actor_targets,
+                    clone.critics,
+                    clone.critic_targets,
+                    clone.actor_optimizer,
+                    clone.critic_optimizer,
+                ) = (
+                    actors,
+                    actor_targets,
+                    critics,
+                    critic_targets,
+                    actor_optimizers,
+                    critic_optimizers,
+                )
         else:
             clone.actors = [actor.to(self.device) for actor in actors]
-            clone.actor_targets = [actor_target.to(self.device) for actor_target in actor_targets]
+            clone.actor_targets = [
+                actor_target.to(self.device) for actor_target in actor_targets
+            ]
             clone.critics = [critic.to(self.device) for critic in critics]
-            clone.critic_targets = [critic_target.to(self.device) for critic_target in critic_targets]
+            clone.critic_targets = [
+                critic_target.to(self.device) for critic_target in critic_targets
+            ]
             clone.actor_optimizers = actor_optimizers
             clone.critic_optimizers = critic_optimizers
 
         clone.fitness = copy.deepcopy(self.fitness)
         clone.steps = copy.deepcopy(self.steps)
         clone.scores = copy.deepcopy(self.scores)
 
         return clone
 
     def wrap_models(self):
         if self.accelerator is not None:
             self.actors = [self.accelerator.prepare(actor) for actor in self.actors]
-            self.actor_targets = [self.accelerator.prepare(actor_target) for actor_target in self.actor_targets]
+            self.actor_targets = [
+                self.accelerator.prepare(actor_target)
+                for actor_target in self.actor_targets
+            ]
             self.critics = [self.accelerator.prepare(critic) for critic in self.critics]
-            self.critic_targets = [self.accelerator.prepare(critic_target) for critic_target in self.critic_targets]
-            self.actor_optimizers = [self.accelerator.prepare(actor_optimizer) for actor_optimizer in self.actor_optimizers_type]
-            self.critic_optimizers = [self.accelerator.prepare(critic_optimizer) for critic_optimizer in self.critic_optimizers_type]
-    
+            self.critic_targets = [
+                self.accelerator.prepare(critic_target)
+                for critic_target in self.critic_targets
+            ]
+            self.actor_optimizers = [
+                self.accelerator.prepare(actor_optimizer)
+                for actor_optimizer in self.actor_optimizers_type
+            ]
+            self.critic_optimizers = [
+                self.accelerator.prepare(critic_optimizer)
+                for critic_optimizer in self.critic_optimizers_type
+            ]
+
     def unwrap_models(self):
         if self.accelerator is not None:
-            self.actors = [self.accelerator.unwrap_model(actor) for actor in self.actors]
-            self.actor_targets = [self.accelerator.unwrap_model(actor_target) for actor_target in self.actor_targets]
-            self.critics = [self.accelerator.unwrap_model(critic) for critic in self.critics]
-            self.critic_targets = [self.accelerator.unwrap_model(critic_target) for critic_target in self.critic_targets]
-            self.actor_optimizers = [self.accelerator.unwrap_model(actor_optimizer) for actor_optimizer in self.actor_optimizers]
-            self.critic_optimizers = [self.accelerator.unwrap_model(critic_optimizer) for critic_optimizer in  self.critic_optimizers]
+            self.actors = [
+                self.accelerator.unwrap_model(actor) for actor in self.actors
+            ]
+            self.actor_targets = [
+                self.accelerator.unwrap_model(actor_target)
+                for actor_target in self.actor_targets
+            ]
+            self.critics = [
+                self.accelerator.unwrap_model(critic) for critic in self.critics
+            ]
+            self.critic_targets = [
+                self.accelerator.unwrap_model(critic_target)
+                for critic_target in self.critic_targets
+            ]
+            self.actor_optimizers = [
+                self.accelerator.unwrap_model(actor_optimizer)
+                for actor_optimizer in self.actor_optimizers
+            ]
+            self.critic_optimizers = [
+                self.accelerator.unwrap_model(critic_optimizer)
+                for critic_optimizer in self.critic_optimizers
+            ]
 
     def saveCheckpoint(self, path):
         """Saves a checkpoint of agent properties and network weights to path.
 
         :param path: Location to save checkpoint at
         :type path: string
         """
-        
-        torch.save({
-            'actors_init_dict': [actor.init_dict for actor in self.actors],
-            'actors_state_dict': [actor.state_dict() for actor in self.actors],
-            'actor_targets_init_dict': [actor_target.init_dict for actor_target in self.actor_targets],
-            'actor_targets_state_dict': [actor_target.state_dict() for actor_target in self.actor_targets],
-            'critics_init_dict': [critic.init_dict for critic in self.critics],
-            'critics_state_dict': [critic.state_dict() for critic in self.critics],
-            'critic_targets_init_dict': [critic_target.init_dict for critic_target in self.critic_targets],
-            'critic_targets_state_dict': [critic_target.state_dict() for critic_target in self.critic_targets],
-            'actor_optimizers_state_dict': [actor_optimizer.state_dict() for actor_optimizer in self.actor_optimizers],
-            'critic_optimizers_state_dict': [critic_optimizer.state_dict() for critic_optimizer in self.critic_optimizers],
-            'net_config': self.net_config,
-            'batch_size': self.batch_size,
-            'lr' : self.lr,
-            'learn_step': self.learn_step,
-            'gamma': self.gamma,
-            'tau': self.tau,
-            'mutation': self.mut,
-            'index': self.index,
-            'scores': self.scores,
-            'fitness': self.fitness,
-            'steps': self.steps,
-            }, path, pickle_module=dill)
-        
+
+        torch.save(
+            {
+                "actors_init_dict": [actor.init_dict for actor in self.actors],
+                "actors_state_dict": [actor.state_dict() for actor in self.actors],
+                "actor_targets_init_dict": [
+                    actor_target.init_dict for actor_target in self.actor_targets
+                ],
+                "actor_targets_state_dict": [
+                    actor_target.state_dict() for actor_target in self.actor_targets
+                ],
+                "critics_init_dict": [critic.init_dict for critic in self.critics],
+                "critics_state_dict": [critic.state_dict() for critic in self.critics],
+                "critic_targets_init_dict": [
+                    critic_target.init_dict for critic_target in self.critic_targets
+                ],
+                "critic_targets_state_dict": [
+                    critic_target.state_dict() for critic_target in self.critic_targets
+                ],
+                "actor_optimizers_state_dict": [
+                    actor_optimizer.state_dict()
+                    for actor_optimizer in self.actor_optimizers
+                ],
+                "critic_optimizers_state_dict": [
+                    critic_optimizer.state_dict()
+                    for critic_optimizer in self.critic_optimizers
+                ],
+                "net_config": self.net_config,
+                "batch_size": self.batch_size,
+                "lr": self.lr,
+                "learn_step": self.learn_step,
+                "gamma": self.gamma,
+                "tau": self.tau,
+                "mutation": self.mut,
+                "index": self.index,
+                "scores": self.scores,
+                "fitness": self.fitness,
+                "steps": self.steps,
+            },
+            path,
+            pickle_module=dill,
+        )
 
     def loadCheckpoint(self, path):
         """Loads saved agent properties and network weights from checkpoint.
 
         :param path: Location to load checkpoint from
         :type path: string
         """
         checkpoint = torch.load(path, pickle_module=dill)
-        self.net_config = checkpoint['net_config']
-        if self.net_config['arch'] == 'mlp':
-            self.actors = [EvolvableMLP(**checkpoint['actors_init_dict'][idx]) 
-                           for idx, _ in enumerate(self.agent_ids)]
-            self.actor_targets = [EvolvableMLP(**checkpoint['actor_targets_init_dict'][idx]) 
-                           for idx, _ in enumerate(self.agent_ids)]
-            self.critics = [EvolvableMLP(**checkpoint['critics_init_dict'][idx]) 
-                           for idx, _ in enumerate(self.agent_ids)]
-            self.critic_targets = [EvolvableMLP(**checkpoint['critic_targets_init_dict'][idx]) 
-                           for idx, _ in enumerate(self.agent_ids)]
-        elif self.net_config['arch'] == 'cnn':
-            self.actors = [EvolvableCNN(**checkpoint['actors_init_dict'][idx]) 
-                           for idx, _ in enumerate(self.agent_ids)]
-            self.actor_targets = [EvolvableCNN(**checkpoint['actor_targets_init_dict'][idx]) 
-                           for idx, _ in enumerate(self.agent_ids)]
-            self.critics = [EvolvableCNN(**checkpoint['critics_init_dict'][idx]) 
-                           for idx, _ in enumerate(self.agent_ids)]
-            self.critic_targets = [EvolvableCNN(**checkpoint['critic_targets_init_dict'][idx]) 
-                           for idx, _ in enumerate(self.agent_ids)]
-            
-        self.lr = checkpoint['lr']
-        self.actor_optimizers = [optim.Adam(actor.parameters(), lr=self.lr) for actor in self.actors]
-        self.critic_optimizers = [optim.Adam(critic.parameters(), lr=self.lr) for critic in self.critics]
-        actor_list = [] 
+        self.net_config = checkpoint["net_config"]
+        if self.net_config["arch"] == "mlp":
+            self.actors = [
+                EvolvableMLP(**checkpoint["actors_init_dict"][idx])
+                for idx, _ in enumerate(self.agent_ids)
+            ]
+            self.actor_targets = [
+                EvolvableMLP(**checkpoint["actor_targets_init_dict"][idx])
+                for idx, _ in enumerate(self.agent_ids)
+            ]
+            self.critics = [
+                EvolvableMLP(**checkpoint["critics_init_dict"][idx])
+                for idx, _ in enumerate(self.agent_ids)
+            ]
+            self.critic_targets = [
+                EvolvableMLP(**checkpoint["critic_targets_init_dict"][idx])
+                for idx, _ in enumerate(self.agent_ids)
+            ]
+        elif self.net_config["arch"] == "cnn":
+            self.actors = [
+                EvolvableCNN(**checkpoint["actors_init_dict"][idx])
+                for idx, _ in enumerate(self.agent_ids)
+            ]
+            self.actor_targets = [
+                EvolvableCNN(**checkpoint["actor_targets_init_dict"][idx])
+                for idx, _ in enumerate(self.agent_ids)
+            ]
+            self.critics = [
+                EvolvableCNN(**checkpoint["critics_init_dict"][idx])
+                for idx, _ in enumerate(self.agent_ids)
+            ]
+            self.critic_targets = [
+                EvolvableCNN(**checkpoint["critic_targets_init_dict"][idx])
+                for idx, _ in enumerate(self.agent_ids)
+            ]
+
+        self.lr = checkpoint["lr"]
+        self.actor_optimizers = [
+            optim.Adam(actor.parameters(), lr=self.lr) for actor in self.actors
+        ]
+        self.critic_optimizers = [
+            optim.Adam(critic.parameters(), lr=self.lr) for critic in self.critics
+        ]
+        actor_list = []
         critic_list = []
         actor_target_list = []
         critic_target_list = []
         actor_optimizer_list = []
         critic_optimizer_list = []
-        
-        for idx, (actor, actor_target, critic, critic_target, actor_optimizer, critic_optimizer) in enumerate(zip(self.actors,
-                                                                                                                self.actor_targets,
-                                                                                                                self.critics,
-                                                                                                                self.critic_targets,
-                                                                                                                self.actor_optimizers,
-                                                                                                                self.critic_optimizers)):
-            
 
-            actor.load_state_dict(checkpoint['actors_state_dict'][idx])
+        for idx, (
+            actor,
+            actor_target,
+            critic,
+            critic_target,
+            actor_optimizer,
+            critic_optimizer,
+        ) in enumerate(
+            zip(
+                self.actors,
+                self.actor_targets,
+                self.critics,
+                self.critic_targets,
+                self.actor_optimizers,
+                self.critic_optimizers,
+            )
+        ):
+            actor.load_state_dict(checkpoint["actors_state_dict"][idx])
             actor_list.append(actor)
-            actor_target.load_state_dict(checkpoint['actor_targets_state_dict'][idx])
+            actor_target.load_state_dict(checkpoint["actor_targets_state_dict"][idx])
             actor_target_list.append(actor_target)
-            critic.load_state_dict(checkpoint['critics_state_dict'][idx])
+            critic.load_state_dict(checkpoint["critics_state_dict"][idx])
             critic_list.append(critic)
-            critic_target.load_state_dict(checkpoint['critic_targets_state_dict'][idx])
+            critic_target.load_state_dict(checkpoint["critic_targets_state_dict"][idx])
             critic_target_list.append(critic_target)
-            actor_optimizer.load_state_dict(checkpoint['actor_optimizers_state_dict'][idx])
+            actor_optimizer.load_state_dict(
+                checkpoint["actor_optimizers_state_dict"][idx]
+            )
             actor_optimizer_list.append(actor_optimizer)
-            critic_optimizer.load_state_dict(checkpoint['critic_optimizers_state_dict'][idx])
+            critic_optimizer.load_state_dict(
+                checkpoint["critic_optimizers_state_dict"][idx]
+            )
             critic_optimizer_list.append(critic_optimizer)
-        
-        self.actors = actor_list                        
-        self.actor_targets = actor_target_list          
-        self.critics = critic_list                      
-        self.critic_targets = critic_target_list        
-        self.actor_optimizers = actor_optimizer_list    
-        self.critic_optimizers =  critic_optimizer_list 
-        self.batch_size = checkpoint['batch_size']
-        self.learn_step = checkpoint['learn_step']
-        self.gamma = checkpoint['gamma']
-        self.tau = checkpoint['tau']
-        self.mut = checkpoint['mutation']
-        self.index = checkpoint['index']
-        self.scores = checkpoint['scores']
-        self.fitness = checkpoint['fitness']
-        self.steps = checkpoint['steps']
+
+        self.actors = actor_list
+        self.actor_targets = actor_target_list
+        self.critics = critic_list
+        self.critic_targets = critic_target_list
+        self.actor_optimizers = actor_optimizer_list
+        self.critic_optimizers = critic_optimizer_list
+        self.batch_size = checkpoint["batch_size"]
+        self.learn_step = checkpoint["learn_step"]
+        self.gamma = checkpoint["gamma"]
+        self.tau = checkpoint["tau"]
+        self.mut = checkpoint["mutation"]
+        self.index = checkpoint["index"]
+        self.scores = checkpoint["scores"]
+        self.fitness = checkpoint["fitness"]
+        self.steps = checkpoint["steps"]
```

### Comparing `agilerl-0.1.8/agilerl/algorithms/matd3.py` & `agilerl-0.1.9/agilerl/algorithms/matd3.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-import random
 import copy
+import random
+
 import dill
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.optim as optim
-from agilerl.networks.evolvable_mlp import EvolvableMLP
+
 from agilerl.networks.evolvable_cnn import EvolvableCNN
+from agilerl.networks.evolvable_mlp import EvolvableMLP
 
 
-class MATD3():
+class MATD3:
     """The MATD3 algorithm class. MATD3 paper: https://arxiv.org/abs/1910.01465
 
     :param state_dims: State observation dimensions for each agent
     :type state_dims: List[tuple]
     :param action_dims: Action dimensions for each agent
     :type action_dims: List[int]
     :param one_hot: One-hot encoding, used with discrete observation spaces
@@ -52,19 +54,39 @@
     :type device: str, optional
     :param accelerator: Accelerator for distributed computing, defaults to None
     :type accelerator: Hugging Face accelerate.Accelerator(), optional
     :param wrap: Wrap models for distributed training upon creation, defaults to True
     :type wrap: bool, optional
     """
 
-    def __init__(self, state_dims, action_dims, one_hot, n_agents, agent_ids, max_action, 
-                 min_action, discrete_actions, expl_noise=0.1, index=0, policy_freq=2,
-                 net_config={'arch': 'mlp', 'h_size': [64,64]}, batch_size=64, lr=0.01,
-                 learn_step=5, gamma=0.95, tau=0.01, mutation=None, device="cpu", accelerator=None, wrap=True):
-        self.algo = 'MADDPG'
+    def __init__(
+        self,
+        state_dims,
+        action_dims,
+        one_hot,
+        n_agents,
+        agent_ids,
+        max_action,
+        min_action,
+        discrete_actions,
+        expl_noise=0.1,
+        index=0,
+        policy_freq=2,
+        net_config={"arch": "mlp", "h_size": [64, 64]},
+        batch_size=64,
+        lr=0.01,
+        learn_step=5,
+        gamma=0.95,
+        tau=0.01,
+        mutation=None,
+        device="cpu",
+        accelerator=None,
+        wrap=True,
+    ):
+        self.algo = "MADDPG"
         self.state_dims = state_dims
         self.total_state_dims = sum(state_dim[0] for state_dim in self.state_dims)
         self.action_dims = action_dims
         self.one_hot = one_hot
         self.n_agents = n_agents
         self.multi = True if n_agents > 1 else False
         self.agent_ids = agent_ids
@@ -82,124 +104,164 @@
         self.scores = []
         self.fitness = []
         self.steps = [0]
         self.max_action = max_action
         self.expl_noise = expl_noise
         self.min_action = min_action
         self.discrete_actions = discrete_actions
-        self.total_actions = sum(self.action_dims) if not self.discrete_actions else len(self.action_dims)
+        self.total_actions = (
+            sum(self.action_dims)
+            if not self.discrete_actions
+            else len(self.action_dims)
+        )
 
-        if 'output_activation' in self.net_config.keys():
+        if "output_activation" in self.net_config.keys():
             pass
         else:
             if self.discrete_actions:
-                self.net_config['output_activation'] = 'gumbel_softmax'
+                self.net_config["output_activation"] = "gumbel_softmax"
             else:
-                self.net_config['output_activation'] = 'softmax'
+                self.net_config["output_activation"] = "softmax"
 
         # model
-        if self.net_config['arch'] == 'mlp':      # Multi-layer Perceptron
-            self.actors = [EvolvableMLP(
-                num_inputs=state_dim[0],
-                num_outputs=action_dim,
-                hidden_size=self.net_config['h_size'],
-                output_activation=self.net_config['output_activation'],
-                device=self.device,
-                accelerator=self.accelerator) for (action_dim, state_dim) in zip(self.action_dims, self.state_dims)]
+        if self.net_config["arch"] == "mlp":  # Multi-layer Perceptron
+            self.actors = [
+                EvolvableMLP(
+                    num_inputs=state_dim[0],
+                    num_outputs=action_dim,
+                    hidden_size=self.net_config["h_size"],
+                    output_activation=self.net_config["output_activation"],
+                    device=self.device,
+                    accelerator=self.accelerator,
+                )
+                for (action_dim, state_dim) in zip(self.action_dims, self.state_dims)
+            ]
             self.actor_targets = copy.deepcopy(self.actors)
 
-            self.critics_1 = [EvolvableMLP(
-                num_inputs=self.total_state_dims + self.total_actions, 
-                num_outputs=1,
-                hidden_size=self.net_config['h_size'],
-                device=self.device,
-                accelerator=self.accelerator) for _ in range(self.n_agents)]
+            self.critics_1 = [
+                EvolvableMLP(
+                    num_inputs=self.total_state_dims + self.total_actions,
+                    num_outputs=1,
+                    hidden_size=self.net_config["h_size"],
+                    device=self.device,
+                    accelerator=self.accelerator,
+                )
+                for _ in range(self.n_agents)
+            ]
             self.critic_targets_1 = copy.deepcopy(self.critics_1)
 
-            self.critics_2 = [EvolvableMLP(
-                num_inputs=self.total_state_dims + self.total_actions, 
-                num_outputs=1,
-                hidden_size=self.net_config['h_size'],
-                device=self.device,
-                accelerator=self.accelerator) for _ in range(self.n_agents)]
+            self.critics_2 = [
+                EvolvableMLP(
+                    num_inputs=self.total_state_dims + self.total_actions,
+                    num_outputs=1,
+                    hidden_size=self.net_config["h_size"],
+                    device=self.device,
+                    accelerator=self.accelerator,
+                )
+                for _ in range(self.n_agents)
+            ]
             self.critic_targets_2 = copy.deepcopy(self.critics_2)
 
-        elif self.net_config['arch'] == 'cnn':    # Convolutional Neural Network
-            self.actors = [EvolvableCNN(
-                input_shape=state_dim,
-                num_actions=action_dim,
-                channel_size=self.net_config['c_size'],
-                kernal_size=self.net_config['k_size'],
-                stride_size=self.net_config['s_size'],
-                hidden_size=self.net_config['h_size'],
-                normalize=self.net_config['normalize'],
-                mlp_activation=self.net_config['output_activation'],
-                multi=self.multi,
-                n_agents=self.n_agents,
-                device=self.device,
-                accelerator=self.accelerator) for (action_dim, state_dim) in zip(self.action_dims, self.state_dims)]
+        elif self.net_config["arch"] == "cnn":  # Convolutional Neural Network
+            self.actors = [
+                EvolvableCNN(
+                    input_shape=state_dim,
+                    num_actions=action_dim,
+                    channel_size=self.net_config["c_size"],
+                    kernal_size=self.net_config["k_size"],
+                    stride_size=self.net_config["s_size"],
+                    hidden_size=self.net_config["h_size"],
+                    normalize=self.net_config["normalize"],
+                    mlp_activation=self.net_config["output_activation"],
+                    multi=self.multi,
+                    n_agents=self.n_agents,
+                    device=self.device,
+                    accelerator=self.accelerator,
+                )
+                for (action_dim, state_dim) in zip(self.action_dims, self.state_dims)
+            ]
             self.actor_targets = copy.deepcopy(self.actors)
 
-            self.critics_1 = [EvolvableCNN(
-                input_shape=state_dim, 
-                num_actions=self.total_actions,
-                channel_size=self.net_config['c_size'],
-                kernal_size=self.net_config['k_size'],
-                stride_size=self.net_config['s_size'],
-                hidden_size=self.net_config['h_size'],
-                normalize=self.net_config['normalize'],
-                mlp_activation='tanh',
-                critic=True,
-                n_agents=self.n_agents,
-                multi=self.multi,
-                device=self.device,
-                accelerator=self.accelerator) for state_dim in self.state_dims]
+            self.critics_1 = [
+                EvolvableCNN(
+                    input_shape=state_dim,
+                    num_actions=self.total_actions,
+                    channel_size=self.net_config["c_size"],
+                    kernal_size=self.net_config["k_size"],
+                    stride_size=self.net_config["s_size"],
+                    hidden_size=self.net_config["h_size"],
+                    normalize=self.net_config["normalize"],
+                    mlp_activation="tanh",
+                    critic=True,
+                    n_agents=self.n_agents,
+                    multi=self.multi,
+                    device=self.device,
+                    accelerator=self.accelerator,
+                )
+                for state_dim in self.state_dims
+            ]
             self.critic_targets_1 = copy.deepcopy(self.critics_1)
 
-            self.critics_2 = [EvolvableCNN(
-                input_shape=state_dim, 
-                num_actions=self.total_actions,
-                channel_size=self.net_config['c_size'],
-                kernal_size=self.net_config['k_size'],
-                stride_size=self.net_config['s_size'],
-                hidden_size=self.net_config['h_size'],
-                normalize=self.net_config['normalize'],
-                mlp_activation='tanh',
-                critic=True,
-                n_agents=self.n_agents,
-                multi=self.multi,
-                device=self.device,
-                accelerator=self.accelerator) for state_dim in self.state_dims]
+            self.critics_2 = [
+                EvolvableCNN(
+                    input_shape=state_dim,
+                    num_actions=self.total_actions,
+                    channel_size=self.net_config["c_size"],
+                    kernal_size=self.net_config["k_size"],
+                    stride_size=self.net_config["s_size"],
+                    hidden_size=self.net_config["h_size"],
+                    normalize=self.net_config["normalize"],
+                    mlp_activation="tanh",
+                    critic=True,
+                    n_agents=self.n_agents,
+                    multi=self.multi,
+                    device=self.device,
+                    accelerator=self.accelerator,
+                )
+                for state_dim in self.state_dims
+            ]
             self.critic_targets_2 = copy.deepcopy(self.critics_2)
 
-        self.actor_optimizers_type = [optim.Adam(actor.parameters(), lr=self.lr) for actor in self.actors]
-        self.critic_1_optimizers_type = [optim.Adam(critic.parameters(), lr=self.lr) for critic in self.critics_1]
-        self.critic_2_optimizers_type = [optim.Adam(critic.parameters(), lr=self.lr) for critic in self.critics_2]
+        self.actor_optimizers_type = [
+            optim.Adam(actor.parameters(), lr=self.lr) for actor in self.actors
+        ]
+        self.critic_1_optimizers_type = [
+            optim.Adam(critic.parameters(), lr=self.lr) for critic in self.critics_1
+        ]
+        self.critic_2_optimizers_type = [
+            optim.Adam(critic.parameters(), lr=self.lr) for critic in self.critics_2
+        ]
 
         if self.accelerator is not None:
             self.actor_optimizers = self.actor_optimizers_type
             self.critic_1_optimizers = self.critic_1_optimizers_type
             self.critic_2_optimizers = self.critic_2_optimizers_type
             if wrap:
-                self.wrap_models()          
+                self.wrap_models()
         else:
             self.actors = [actor.to(self.device) for actor in self.actors]
-            self.actor_targets = [actor_target.to(self.device) for actor_target in self.actor_targets]
+            self.actor_targets = [
+                actor_target.to(self.device) for actor_target in self.actor_targets
+            ]
             self.critics_1 = [critic.to(self.device) for critic in self.critics_1]
-            self.critic_targets_1 = [critic_target.to(self.device) for critic_target in self.critic_targets_1]
+            self.critic_targets_1 = [
+                critic_target.to(self.device) for critic_target in self.critic_targets_1
+            ]
             self.critics_2 = [critic.to(self.device) for critic in self.critics_2]
-            self.critic_targets_2 = [critic_target.to(self.device) for critic_target in self.critic_targets_2]
+            self.critic_targets_2 = [
+                critic_target.to(self.device) for critic_target in self.critic_targets_2
+            ]
             self.actor_optimizers = self.actor_optimizers_type
             self.critic_1_optimizers = self.critic_1_optimizers_type
             self.critic_2_optimizers = self.critic_2_optimizers_type
 
         self.criterion = nn.MSELoss()
 
     def getAction(self, states, epsilon=0):
-        """Returns the next action to take in the environment. 
+        """Returns the next action to take in the environment.
         Epsilon is the probability of taking a random action, used for exploration.
         For epsilon-greedy behaviour, set epsilon to 0.
 
         :param state: Environment observations: {'agent_0': state_dim_0, ..., 'agent_n': state_dim_n}
         :type state: Dict[str, numpy.Array]
         :param epsilon: Probablilty of taking a random action for exploration, defaults to 0
         :type epsilon: float, optional
@@ -208,215 +270,302 @@
         states = [torch.from_numpy(state).float() for state in states.values()]
 
         # Configure accelerator
         if self.accelerator is None:
             states = [state.to(self.device) for state in states]
 
         if self.one_hot:
-            states = [nn.functional.one_hot(
-                state.long(), num_classes=state_dim[0]).float().squeeze() for state, state_dim 
-                in zip(states, self.state_dims)]
-        
+            states = [
+                nn.functional.one_hot(state.long(), num_classes=state_dim[0])
+                .float()
+                .squeeze()
+                for state, state_dim in zip(states, self.state_dims)
+            ]
+
         if self.net_config["arch"] == "mlp":
-            states = [state.unsqueeze(0) if len(state.size()) < 2 else state for state in states]   
+            states = [
+                state.unsqueeze(0) if len(state.size()) < 2 else state
+                for state in states
+            ]
         elif self.net_config["arch"] == "cnn":
             states = [state.unsqueeze(2) for state in states]
 
-        actions = {} 
-        for idx, (agent_id, state, actor) in enumerate(zip(self.agent_ids, states, self.actors)):
+        actions = {}
+        for idx, (agent_id, state, actor) in enumerate(
+            zip(self.agent_ids, states, self.actors)
+        ):
             if random.random() < epsilon:
                 if self.discrete_actions:
                     action = np.random.randint(0, self.action_dims[idx])
                 else:
-                    action = np.random.rand(state.size()[0], self.action_dims[idx]).astype('float32').squeeze()
+                    action = (
+                        np.random.rand(state.size()[0], self.action_dims[idx])
+                        .astype("float32")
+                        .squeeze()
+                    )
             else:
                 actor.eval()
                 if self.accelerator is not None:
                     with actor.no_sync():
                         action_values = actor(state)
                 else:
                     with torch.no_grad():
                         action_values = actor(state)
                 actor.train()
                 if self.discrete_actions:
                     action = action_values.squeeze(0).argmax().item()
                 else:
-                    action = action_values.cpu().data.numpy().squeeze() \
-                         + np.random.normal(0, self.max_action[idx][0] * self.expl_noise, size=self.action_dims[idx]).astype(np.float32)
-                    action = np.clip(action, self.min_action[idx][0], self.max_action[idx][0])     
+                    action = (
+                        action_values.cpu().data.numpy().squeeze()
+                        + np.random.normal(
+                            0,
+                            self.max_action[idx][0] * self.expl_noise,
+                            size=self.action_dims[idx],
+                        ).astype(np.float32)
+                    )
+                    action = np.clip(
+                        action, self.min_action[idx][0], self.max_action[idx][0]
+                    )
             actions[agent_id] = action
-        
+
         return actions
-    
+
     def _squeeze_exp(self, experiences):
         """Remove first dim created by dataloader.
-        
+
         :param experiences: List of batched states, actions, rewards, next_states, dones in that order.
         :type state: List[torch.Tensor[float]]
         """
         st, ac, re, ne, do = experiences
         return st.squeeze(0), ac.squeeze(0), re.squeeze(0), ne.squeeze(0), do.squeeze(0)
 
     def learn(self, experiences):
         """Updates agent network parameters to learn from experiences.
 
-        :param experience: Tuple of dictionaries containing batched states, actions, rewards, next_states, 
+        :param experience: Tuple of dictionaries containing batched states, actions, rewards, next_states,
         dones in that order for each individual agent.
         :type experience: Tuple[Dict[str, torch.Tensor]]
         """
 
-        for agent_id, actor, actor_target, critic_1, critic_target_1, \
-            critic_2,critic_target_2, actor_optimizer, critic_1_optimizer, critic_2_optimizer in zip(self.agent_ids,
-                                                                                self.actors,    
-                                                                                self.actor_targets,
-                                                                                self.critics_1, 
-                                                                                self.critic_targets_1,
-                                                                                self.critics_2, 
-                                                                                self.critic_targets_2,
-                                                                                self.actor_optimizers, 
-                                                                                self.critic_1_optimizers,
-                                                                                self.critic_2_optimizers):
-         
+        for (
+            agent_id,
+            actor,
+            actor_target,
+            critic_1,
+            critic_target_1,
+            critic_2,
+            critic_target_2,
+            actor_optimizer,
+            critic_1_optimizer,
+            critic_2_optimizer,
+        ) in zip(
+            self.agent_ids,
+            self.actors,
+            self.actor_targets,
+            self.critics_1,
+            self.critic_targets_1,
+            self.critics_2,
+            self.critic_targets_2,
+            self.actor_optimizers,
+            self.critic_1_optimizers,
+            self.critic_2_optimizers,
+        ):
             states, actions, rewards, next_states, dones = experiences
-            
-            if self.one_hot:
-                states = {agent_id: nn.functional.one_hot(state.long(), num_classes=state_dim[0]).float().squeeze() for 
-                          agent_id, state, state_dim in zip(states.items(), self.state_dims)}
 
+            if self.one_hot:
+                states = {
+                    agent_id: nn.functional.one_hot(
+                        state.long(), num_classes=state_dim[0]
+                    )
+                    .float()
+                    .squeeze()
+                    for agent_id, state, state_dim in zip(
+                        states.items(), self.state_dims
+                    )
+                }
 
-            if self.net_config['arch'] == 'mlp':
+            if self.net_config["arch"] == "mlp":
                 if self.discrete_actions:
                     action_values = [a.unsqueeze(1) for a in actions.values()]
                 else:
                     action_values = list(actions.values())
                 input_combined = torch.cat(list(states.values()) + action_values, 1)
                 if self.accelerator is not None:
                     with critic_1.no_sync():
                         q_value_1 = critic_1(input_combined)
                     with critic_2.no_sync():
                         q_value_2 = critic_2(input_combined)
                 else:
                     q_value_1 = critic_1(input_combined)
                     q_value_2 = critic_2(input_combined)
-                next_actions = [self.actor_targets[idx](next_states[agent_id]).detach_() for idx, agent_id in enumerate(self.agent_ids)]
-                
-            elif self.net_config['arch'] == 'cnn':
+                next_actions = [
+                    self.actor_targets[idx](next_states[agent_id]).detach_()
+                    for idx, agent_id in enumerate(self.agent_ids)
+                ]
+
+            elif self.net_config["arch"] == "cnn":
                 stacked_states = torch.stack(list(states.values()), dim=2)
                 stacked_actions = torch.stack(list(actions.values()), dim=1)
                 if self.accelerator is not None:
                     with critic_1.no_sync():
                         q_value_1 = critic_1(stacked_states, stacked_actions)
                     with critic_2.no_sync():
                         q_value_2 = critic_2(stacked_states, stacked_actions)
                 else:
                     q_value_1 = critic_1(stacked_states, stacked_actions)
                     q_value_2 = critic_2(stacked_states, stacked_actions)
-                next_actions = [self.actor_targets[idx](next_states[agent_id].unsqueeze(2)).detach_() for idx, agent_id in enumerate(self.agent_ids)]
-            
-            if self.discrete_actions:
-                next_actions = [torch.argmax(agent_actions, dim=1).unsqueeze(1) if  self.net_config['arch'] == 'mlp' else
-                                torch.argmax(agent_actions, dim=1) for agent_actions in next_actions]
+                next_actions = [
+                    self.actor_targets[idx](
+                        next_states[agent_id].unsqueeze(2)
+                    ).detach_()
+                    for idx, agent_id in enumerate(self.agent_ids)
+                ]
 
-            if self.net_config['arch'] == 'mlp':
-                next_input_combined = torch.cat(list(next_states.values()) + next_actions, 1)
+            if self.discrete_actions:
+                next_actions = [
+                    torch.argmax(agent_actions, dim=1).unsqueeze(1)
+                    if self.net_config["arch"] == "mlp"
+                    else torch.argmax(agent_actions, dim=1)
+                    for agent_actions in next_actions
+                ]
+
+            if self.net_config["arch"] == "mlp":
+                next_input_combined = torch.cat(
+                    list(next_states.values()) + next_actions, 1
+                )
                 if self.accelerator is not None:
                     with critic_target_1.no_sync():
                         q_value_next_state_1 = critic_target_1(next_input_combined)
                     with critic_target_2.no_sync():
                         q_value_next_state_2 = critic_target_2(next_input_combined)
                 else:
                     q_value_next_state_1 = critic_target_1(next_input_combined)
                     q_value_next_state_2 = critic_target_2(next_input_combined)
-            elif self.net_config['arch'] == 'cnn':
+            elif self.net_config["arch"] == "cnn":
                 stacked_next_states = torch.stack(list(next_states.values()), dim=2)
                 stacked_next_actions = torch.stack(next_actions, dim=1)
                 if self.accelerator is not None:
                     with critic_target_1.no_sync():
-                        q_value_next_state_1 = critic_target_1(stacked_next_states, stacked_next_actions)
+                        q_value_next_state_1 = critic_target_1(
+                            stacked_next_states, stacked_next_actions
+                        )
                     with critic_target_2.no_sync():
-                        q_value_next_state_2 = critic_target_2(stacked_next_states, stacked_next_actions)
+                        q_value_next_state_2 = critic_target_2(
+                            stacked_next_states, stacked_next_actions
+                        )
                 else:
-                    q_value_next_state_1 = critic_target_1(stacked_next_states, stacked_next_actions)
-                    q_value_next_state_2 = critic_target_2(stacked_next_states, stacked_next_actions)
+                    q_value_next_state_1 = critic_target_1(
+                        stacked_next_states, stacked_next_actions
+                    )
+                    q_value_next_state_2 = critic_target_2(
+                        stacked_next_states, stacked_next_actions
+                    )
             q_value_next_state = torch.min(q_value_next_state_1, q_value_next_state_2)
 
-            y_j = rewards[agent_id] + (1 - dones[agent_id]) * self.gamma * q_value_next_state
-
-            critic_loss = self.criterion(q_value_1, y_j.detach_()) + self.criterion(q_value_2, y_j.detach_())
+            y_j = (
+                rewards[agent_id]
+                + (1 - dones[agent_id]) * self.gamma * q_value_next_state
+            )
+
+            critic_loss = self.criterion(q_value_1, y_j.detach_()) + self.criterion(
+                q_value_2, y_j.detach_()
+            )
 
             # critic loss backprop
             critic_1_optimizer.zero_grad()
             critic_2_optimizer.zero_grad()
             if self.accelerator is not None:
                 self.accelerator.backward(critic_loss)
             else:
                 critic_loss.backward()
             critic_1_optimizer.step()
             critic_2_optimizer.step()
 
             # update actor and targets every policy_freq episodes
             if len(self.scores) % self.policy_freq == 0:
-                if self.net_config['arch'] == 'mlp':
+                if self.net_config["arch"] == "mlp":
                     if self.accelerator is not None:
                         with actor.no_sync():
                             action = actor(states[agent_id])
                     else:
                         action = actor(states[agent_id])
                     detached_actions = copy.deepcopy(actions)
                     if self.discrete_actions:
                         action = action.argmax(1).unsqueeze(1)
-                        detached_actions = {agent_id: d.unsqueeze(1) for agent_id, d in detached_actions.items()}
+                        detached_actions = {
+                            agent_id: d.unsqueeze(1)
+                            for agent_id, d in detached_actions.items()
+                        }
                     detached_actions[agent_id] = action
-                    input_combined = torch.cat(list(states.values()) + list(detached_actions.values()), 1)
+                    input_combined = torch.cat(
+                        list(states.values()) + list(detached_actions.values()), 1
+                    )
                     if self.accelerator is not None:
                         with critic_1.no_sync():
                             actor_loss = -critic_1(input_combined).mean()
                     else:
                         actor_loss = -critic_1(input_combined).mean()
 
-                elif self.net_config['arch'] == 'cnn':
+                elif self.net_config["arch"] == "cnn":
                     if self.accelerator is not None:
                         with actor.no_sync():
                             action = actor(states[agent_id].unsqueeze(2))
                     else:
                         action = actor(states[agent_id].unsqueeze(2))
                     if self.discrete_actions:
                         action = action.argmax(1)
                     detached_actions = copy.deepcopy(actions)
                     detached_actions[agent_id] = action
-                    stacked_detached_actions = torch.stack(list(detached_actions.values()), dim=1)
+                    stacked_detached_actions = torch.stack(
+                        list(detached_actions.values()), dim=1
+                    )
                     if self.accelerator is not None:
                         with critic_1.no_sync():
-                            actor_loss = - \
-                                critic_1(stacked_states, stacked_detached_actions).mean()
+                            actor_loss = -critic_1(
+                                stacked_states, stacked_detached_actions
+                            ).mean()
                     else:
-                        actor_loss = - \
-                        critic_1(stacked_states, stacked_detached_actions).mean()
+                        actor_loss = -critic_1(
+                            stacked_states, stacked_detached_actions
+                        ).mean()
 
                 # actor loss backprop
                 actor_optimizer.zero_grad()
                 if self.accelerator is not None:
                     self.accelerator.backward(actor_loss)
                 else:
                     actor_loss.backward()
                 actor_optimizer.step()
 
         if len(self.scores) % self.policy_freq:
-            for actor, actor_target, critic_1, critic_target_1, critic_2, critic_target_2  \
-            in zip(self.actors, self.actor_targets, self.critics_1, self.critic_targets_1, self.critics_2, self.critic_targets_2):
+            for (
+                actor,
+                actor_target,
+                critic_1,
+                critic_target_1,
+                critic_2,
+                critic_target_2,
+            ) in zip(
+                self.actors,
+                self.actor_targets,
+                self.critics_1,
+                self.critic_targets_1,
+                self.critics_2,
+                self.critic_targets_2,
+            ):
                 self.softUpdate(actor, actor_target)
                 self.softUpdate(critic_1, critic_target_1)
                 self.softUpdate(critic_2, critic_target_2)
 
     def softUpdate(self, net, target):
-        """Soft updates target network.
-        """
+        """Soft updates target network."""
         for eval_param, target_param in zip(net.parameters(), target.parameters()):
             target_param.data.copy_(
-                self.tau * eval_param.data + (1.0 - self.tau) * target_param.data)
+                self.tau * eval_param.data + (1.0 - self.tau) * target_param.data
+            )
 
     def test(self, env, swap_channels=False, max_steps=500, loop=3):
         """Returns mean test score of agent in environment with epsilon-greedy policy.
 
         :param env: The environment to be tested in
         :type env: Gym-style environment
         :param swap_channels: Swap image channels dimension from last to first [H, W, C] -> [C, H, W], defaults to False
@@ -430,19 +579,22 @@
             rewards = []
             for i in range(loop):
                 state, _ = env.reset()
                 agent_reward = {agent_id: 0 for agent_id in self.agent_ids}
                 score = 0
                 for _ in range(max_steps):
                     if swap_channels:
-                        state = {agent_id: np.moveaxis(np.expand_dims(s, 0), [3], [1]) for agent_id, s in state.items()}
+                        state = {
+                            agent_id: np.moveaxis(np.expand_dims(s, 0), [3], [1])
+                            for agent_id, s in state.items()
+                        }
                     action = self.getAction(state, epsilon=0)
                     state, reward, done, trunc, info = env.step(action)
                     for agent_id, r in reward.items():
-                        agent_reward[agent_id] += r 
+                        agent_reward[agent_id] += r
                     score = sum(agent_reward.values())
                 rewards.append(score)
         mean_fit = np.mean(rewards)
         self.fitness.append(mean_fit)
         return mean_fit
 
     def clone(self, index=None, wrap=True):
@@ -450,236 +602,424 @@
 
         :param index: Index to keep track of agent for tournament selection and mutation, defaults to None
         :type index: int, optional
         """
         if index is None:
             index = self.index
 
-        clone = type(self)(state_dims=self.state_dims,
-                           action_dims=self.action_dims,
-                           one_hot=self.one_hot,
-                           n_agents=self.n_agents,
-                           agent_ids=self.agent_ids,
-                           max_action=self.max_action,
-                           min_action=self.min_action,
-                           expl_noise=self.expl_noise,
-                           discrete_actions=self.discrete_actions,
-                           index=index,
-                           net_config=self.net_config,
-                           batch_size=self.batch_size,
-                           policy_freq=self.policy_freq,
-                           lr=self.lr,
-                           learn_step=self.learn_step,
-                           gamma=self.gamma,
-                           tau=self.tau,
-                           mutation=self.mut,
-                           device=self.device,
-                           accelerator=self.accelerator,
-                           wrap=wrap)
-        
+        clone = type(self)(
+            state_dims=self.state_dims,
+            action_dims=self.action_dims,
+            one_hot=self.one_hot,
+            n_agents=self.n_agents,
+            agent_ids=self.agent_ids,
+            max_action=self.max_action,
+            min_action=self.min_action,
+            expl_noise=self.expl_noise,
+            discrete_actions=self.discrete_actions,
+            index=index,
+            net_config=self.net_config,
+            batch_size=self.batch_size,
+            policy_freq=self.policy_freq,
+            lr=self.lr,
+            learn_step=self.learn_step,
+            gamma=self.gamma,
+            tau=self.tau,
+            mutation=self.mut,
+            device=self.device,
+            accelerator=self.accelerator,
+            wrap=wrap,
+        )
+
         if self.accelerator is not None:
             self.unwrap_models()
         actors = [actor.clone() for actor in self.actors]
         actor_targets = [actor_target.clone() for actor_target in self.actor_targets]
         critics_1 = [critic.clone() for critic in self.critics_1]
-        critic_targets_1 = [critic_target.clone() for critic_target in self.critic_targets_1]
+        critic_targets_1 = [
+            critic_target.clone() for critic_target in self.critic_targets_1
+        ]
         critics_2 = [critic.clone() for critic in self.critics_2]
-        critic_targets_2 = [critic_target.clone() for critic_target in self.critic_targets_2]
-        actor_optimizers = [optim.Adam(actor.parameters(), lr=clone.lr) for actor in actors]
-        critic_1_optimizers = [optim.Adam(critic.parameters(), lr=clone.lr) for critic in critics_1]
-        critic_2_optimizers = [optim.Adam(critic.parameters(), lr=clone.lr) for critic in critics_2]
+        critic_targets_2 = [
+            critic_target.clone() for critic_target in self.critic_targets_2
+        ]
+        actor_optimizers = [
+            optim.Adam(actor.parameters(), lr=clone.lr) for actor in actors
+        ]
+        critic_1_optimizers = [
+            optim.Adam(critic.parameters(), lr=clone.lr) for critic in critics_1
+        ]
+        critic_2_optimizers = [
+            optim.Adam(critic.parameters(), lr=clone.lr) for critic in critics_2
+        ]
         clone.actor_optimizers_type = actor_optimizers
         clone.critic_1_optimizers_type = critic_1_optimizers
         clone.critic_2_optimizers_type = critic_2_optimizers
 
         if self.accelerator is not None:
             if wrap:
                 clone.actors = [self.accelerator.prepare(actor) for actor in actors]
-                clone.actor_targets = [self.accelerator.prepare(actor_target) for actor_target in actor_targets]
-                clone.critics_1 = [self.accelerator.prepare(critic) for critic in critics_1]
-                clone.critic_targets_1 = [self.accelerator.prepare(critic_target) for critic_target in critic_targets_1]
-                clone.critics_2 = [self.accelerator.prepare(critic) for critic in critics_2]
-                clone.critic_targets_2 = [self.accelerator.prepare(critic_target) for critic_target in critic_targets_2]
-                clone.actor_optimizers = [self.accelerator.prepare(actor_optimizer) for actor_optimizer in actor_optimizers]
-                clone.critic_1_optimizers = [self.accelerator.prepare(critic_optimizer) for critic_optimizer in critic_1_optimizers]
-                clone.critic_2_optimizers = [self.accelerator.prepare(critic_optimizer) for critic_optimizer in critic_2_optimizers]
+                clone.actor_targets = [
+                    self.accelerator.prepare(actor_target)
+                    for actor_target in actor_targets
+                ]
+                clone.critics_1 = [
+                    self.accelerator.prepare(critic) for critic in critics_1
+                ]
+                clone.critic_targets_1 = [
+                    self.accelerator.prepare(critic_target)
+                    for critic_target in critic_targets_1
+                ]
+                clone.critics_2 = [
+                    self.accelerator.prepare(critic) for critic in critics_2
+                ]
+                clone.critic_targets_2 = [
+                    self.accelerator.prepare(critic_target)
+                    for critic_target in critic_targets_2
+                ]
+                clone.actor_optimizers = [
+                    self.accelerator.prepare(actor_optimizer)
+                    for actor_optimizer in actor_optimizers
+                ]
+                clone.critic_1_optimizers = [
+                    self.accelerator.prepare(critic_optimizer)
+                    for critic_optimizer in critic_1_optimizers
+                ]
+                clone.critic_2_optimizers = [
+                    self.accelerator.prepare(critic_optimizer)
+                    for critic_optimizer in critic_2_optimizers
+                ]
             else:
-                clone.actors, clone.actor_targets, clone.critics_1, clone.critic_targets_1, \
-                clone.critics_2, clone.critic_targets_2, clone.actor_optimizers, clone.critic_1_optimizers, \
-                clone.critic_2_optimizers = actors, actor_targets, critics_1, critic_targets_1, critics_2, critic_targets_2, \
-                actor_optimizers, critic_1_optimizers, critic_2_optimizers
+                (
+                    clone.actors,
+                    clone.actor_targets,
+                    clone.critics_1,
+                    clone.critic_targets_1,
+                    clone.critics_2,
+                    clone.critic_targets_2,
+                    clone.actor_optimizers,
+                    clone.critic_1_optimizers,
+                    clone.critic_2_optimizers,
+                ) = (
+                    actors,
+                    actor_targets,
+                    critics_1,
+                    critic_targets_1,
+                    critics_2,
+                    critic_targets_2,
+                    actor_optimizers,
+                    critic_1_optimizers,
+                    critic_2_optimizers,
+                )
         else:
             clone.actors = [actor.to(self.device) for actor in actors]
-            clone.actor_targets = [actor_target.to(self.device) for actor_target in actor_targets]
+            clone.actor_targets = [
+                actor_target.to(self.device) for actor_target in actor_targets
+            ]
             clone.critics_1 = [critic.to(self.device) for critic in critics_1]
-            clone.critic_targets_1 = [critic_target.to(self.device) for critic_target in critic_targets_1]
+            clone.critic_targets_1 = [
+                critic_target.to(self.device) for critic_target in critic_targets_1
+            ]
             clone.critics_2 = [critic.to(self.device) for critic in critics_2]
-            clone.critic_targets_2 = [critic_target.to(self.device) for critic_target in critic_targets_2]
+            clone.critic_targets_2 = [
+                critic_target.to(self.device) for critic_target in critic_targets_2
+            ]
             clone.actor_optimizers = actor_optimizers
             clone.critic_1_optimizers = critic_1_optimizers
             clone.critic_2_optimizers = critic_2_optimizers
 
         clone.fitness = copy.deepcopy(self.fitness)
         clone.steps = copy.deepcopy(self.steps)
         clone.scores = copy.deepcopy(self.scores)
 
         return clone
 
     def wrap_models(self):
         if self.accelerator is not None:
             self.actors = [self.accelerator.prepare(actor) for actor in self.actors]
-            self.actor_targets = [self.accelerator.prepare(actor_target) for actor_target in self.actor_targets]
-            self.critics_1 = [self.accelerator.prepare(critic) for critic in self.critics_1]
-            self.critic_targets_1 = [self.accelerator.prepare(critic_target) for critic_target in self.critic_targets_1]
-            self.critics_2 = [self.accelerator.prepare(critic) for critic in self.critics_2]
-            self.critic_targets_2 = [self.accelerator.prepare(critic_target) for critic_target in self.critic_targets_2]
-            self.actor_optimizers = [self.accelerator.prepare(actor_optimizer) for actor_optimizer in self.actor_optimizers_type]
-            self.critic_1_optimizers = [self.accelerator.prepare(critic_optimizer) for critic_optimizer in self.critic_1_optimizers_type]
-            self.critic_2_optimizers = [self.accelerator.prepare(critic_optimizer) for critic_optimizer in self.critic_2_optimizers_type]
-    
+            self.actor_targets = [
+                self.accelerator.prepare(actor_target)
+                for actor_target in self.actor_targets
+            ]
+            self.critics_1 = [
+                self.accelerator.prepare(critic) for critic in self.critics_1
+            ]
+            self.critic_targets_1 = [
+                self.accelerator.prepare(critic_target)
+                for critic_target in self.critic_targets_1
+            ]
+            self.critics_2 = [
+                self.accelerator.prepare(critic) for critic in self.critics_2
+            ]
+            self.critic_targets_2 = [
+                self.accelerator.prepare(critic_target)
+                for critic_target in self.critic_targets_2
+            ]
+            self.actor_optimizers = [
+                self.accelerator.prepare(actor_optimizer)
+                for actor_optimizer in self.actor_optimizers_type
+            ]
+            self.critic_1_optimizers = [
+                self.accelerator.prepare(critic_optimizer)
+                for critic_optimizer in self.critic_1_optimizers_type
+            ]
+            self.critic_2_optimizers = [
+                self.accelerator.prepare(critic_optimizer)
+                for critic_optimizer in self.critic_2_optimizers_type
+            ]
+
     def unwrap_models(self):
         if self.accelerator is not None:
-            self.actors = [self.accelerator.unwrap_model(actor) for actor in self.actors]
-            self.actor_targets = [self.accelerator.unwrap_model(actor_target) for actor_target in self.actor_targets]
-            self.critics_1 = [self.accelerator.unwrap_model(critic) for critic in self.critics_1]
-            self.critic_targets_1 = [self.accelerator.unwrap_model(critic_target) for critic_target in self.critic_targets_1]
-            self.critics_2 = [self.accelerator.unwrap_model(critic) for critic in self.critics_2]
-            self.critic_targets_2 = [self.accelerator.unwrap_model(critic_target) for critic_target in self.critic_targets_2]
-            self.actor_optimizers = [self.accelerator.unwrap_model(actor_optimizer) for actor_optimizer in self.actor_optimizers]
-            self.critic_1_optimizers = [self.accelerator.unwrap_model(critic_optimizer) for critic_optimizer in  self.critic_1_optimizers]
-            self.critic_2_optimizers = [self.accelerator.unwrap_model(critic_optimizer) for critic_optimizer in  self.critic_2_optimizers]
+            self.actors = [
+                self.accelerator.unwrap_model(actor) for actor in self.actors
+            ]
+            self.actor_targets = [
+                self.accelerator.unwrap_model(actor_target)
+                for actor_target in self.actor_targets
+            ]
+            self.critics_1 = [
+                self.accelerator.unwrap_model(critic) for critic in self.critics_1
+            ]
+            self.critic_targets_1 = [
+                self.accelerator.unwrap_model(critic_target)
+                for critic_target in self.critic_targets_1
+            ]
+            self.critics_2 = [
+                self.accelerator.unwrap_model(critic) for critic in self.critics_2
+            ]
+            self.critic_targets_2 = [
+                self.accelerator.unwrap_model(critic_target)
+                for critic_target in self.critic_targets_2
+            ]
+            self.actor_optimizers = [
+                self.accelerator.unwrap_model(actor_optimizer)
+                for actor_optimizer in self.actor_optimizers
+            ]
+            self.critic_1_optimizers = [
+                self.accelerator.unwrap_model(critic_optimizer)
+                for critic_optimizer in self.critic_1_optimizers
+            ]
+            self.critic_2_optimizers = [
+                self.accelerator.unwrap_model(critic_optimizer)
+                for critic_optimizer in self.critic_2_optimizers
+            ]
 
     def saveCheckpoint(self, path):
         """Saves a checkpoint of agent properties and network weights to path.
 
         :param path: Location to save checkpoint at
         :type path: string
         """
-        
-        torch.save({
-            'actors_init_dict': [actor.init_dict for actor in self.actors],
-            'actors_state_dict': [actor.state_dict() for actor in self.actors],
-            'actor_targets_init_dict': [actor_target.init_dict for actor_target in self.actor_targets],
-            'actor_targets_state_dict': [actor_target.state_dict() for actor_target in self.actor_targets],
-            'critics_1_init_dict': [critic_1.init_dict for critic_1 in self.critics_1],
-            'critics_1_state_dict': [critic_1.state_dict() for critic_1 in self.critics_1],
-            'critic_targets_1_init_dict': [critic_target_1.init_dict for critic_target_1 in self.critic_targets_1],
-            'critic_targets_1_state_dict': [critic_target_1.state_dict() for critic_target_1 in self.critic_targets_1],
-            'critics_2_init_dict': [critic_2.init_dict for critic_2 in self.critics_2],
-            'critics_2_state_dict': [critic_2.state_dict() for critic_2 in self.critics_2],
-            'critic_targets_2_init_dict': [critic_target_2.init_dict for critic_target_2 in self.critic_targets_2],
-            'critic_targets_2_state_dict': [critic_target_2.state_dict() for critic_target_2 in self.critic_targets_2],
-            'actor_optimizers_state_dict': [actor_optimizer.state_dict() for actor_optimizer in self.actor_optimizers],
-            'critic_1_optimizers_state_dict': [critic_1_optimizer.state_dict() for critic_1_optimizer in self.critic_1_optimizers],
-            'critic_2_optimizers_state_dict': [critic_2_optimizer.state_dict() for critic_2_optimizer in self.critic_2_optimizers],
-            'net_config': self.net_config,
-            'batch_size': self.batch_size,
-            'lr' : self.lr,
-            'learn_step': self.learn_step,
-            'policy_freq': self.policy_freq,
-            'gamma': self.gamma,
-            'tau': self.tau,
-            'mutation': self.mut,
-            'index': self.index,
-            'scores': self.scores,
-            'fitness': self.fitness,
-            'steps': self.steps,
-            }, path, pickle_module=dill)
 
+        torch.save(
+            {
+                "actors_init_dict": [actor.init_dict for actor in self.actors],
+                "actors_state_dict": [actor.state_dict() for actor in self.actors],
+                "actor_targets_init_dict": [
+                    actor_target.init_dict for actor_target in self.actor_targets
+                ],
+                "actor_targets_state_dict": [
+                    actor_target.state_dict() for actor_target in self.actor_targets
+                ],
+                "critics_1_init_dict": [
+                    critic_1.init_dict for critic_1 in self.critics_1
+                ],
+                "critics_1_state_dict": [
+                    critic_1.state_dict() for critic_1 in self.critics_1
+                ],
+                "critic_targets_1_init_dict": [
+                    critic_target_1.init_dict
+                    for critic_target_1 in self.critic_targets_1
+                ],
+                "critic_targets_1_state_dict": [
+                    critic_target_1.state_dict()
+                    for critic_target_1 in self.critic_targets_1
+                ],
+                "critics_2_init_dict": [
+                    critic_2.init_dict for critic_2 in self.critics_2
+                ],
+                "critics_2_state_dict": [
+                    critic_2.state_dict() for critic_2 in self.critics_2
+                ],
+                "critic_targets_2_init_dict": [
+                    critic_target_2.init_dict
+                    for critic_target_2 in self.critic_targets_2
+                ],
+                "critic_targets_2_state_dict": [
+                    critic_target_2.state_dict()
+                    for critic_target_2 in self.critic_targets_2
+                ],
+                "actor_optimizers_state_dict": [
+                    actor_optimizer.state_dict()
+                    for actor_optimizer in self.actor_optimizers
+                ],
+                "critic_1_optimizers_state_dict": [
+                    critic_1_optimizer.state_dict()
+                    for critic_1_optimizer in self.critic_1_optimizers
+                ],
+                "critic_2_optimizers_state_dict": [
+                    critic_2_optimizer.state_dict()
+                    for critic_2_optimizer in self.critic_2_optimizers
+                ],
+                "net_config": self.net_config,
+                "batch_size": self.batch_size,
+                "lr": self.lr,
+                "learn_step": self.learn_step,
+                "policy_freq": self.policy_freq,
+                "gamma": self.gamma,
+                "tau": self.tau,
+                "mutation": self.mut,
+                "index": self.index,
+                "scores": self.scores,
+                "fitness": self.fitness,
+                "steps": self.steps,
+            },
+            path,
+            pickle_module=dill,
+        )
 
     def loadCheckpoint(self, path):
         """Loads saved agent properties and network weights from checkpoint.
 
         :param path: Location to load checkpoint from
         :type path: string
         """
         checkpoint = torch.load(path, pickle_module=dill)
-        self.net_config = checkpoint['net_config']
-        if self.net_config['arch'] == 'mlp':
-            self.actors = [EvolvableMLP(**checkpoint['actors_init_dict'][idx]) 
-                           for idx, _ in enumerate(self.agent_ids)]
-            self.actor_targets = [EvolvableMLP(**checkpoint['actor_targets_init_dict'][idx]) 
-                           for idx, _ in enumerate(self.agent_ids)]
-            self.critics_1 = [EvolvableMLP(**checkpoint['critics_1_init_dict'][idx]) 
-                           for idx, _ in enumerate(self.agent_ids)]
-            self.critic_targets_1 = [EvolvableMLP(**checkpoint['critic_targets_1_init_dict'][idx]) 
-                           for idx, _ in enumerate(self.agent_ids)]
-            self.critics_2 = [EvolvableMLP(**checkpoint['critics_2_init_dict'][idx]) 
-                           for idx, _ in enumerate(self.agent_ids)]
-            self.critic_targets_2 = [EvolvableMLP(**checkpoint['critic_targets_2_init_dict'][idx]) 
-                           for idx, _ in enumerate(self.agent_ids)]
-        elif self.net_config['arch'] == 'cnn':
-            self.actors = [EvolvableCNN(**checkpoint['actors_init_dict'][idx]) 
-                           for idx, _ in enumerate(self.agent_ids)]
-            self.actor_targets = [EvolvableCNN(**checkpoint['actor_targets_init_dict'][idx]) 
-                           for idx, _ in enumerate(self.agent_ids)]
-            self.critics_1 = [EvolvableCNN(**checkpoint['critics_1_init_dict'][idx]) 
-                           for idx, _ in enumerate(self.agent_ids)]
-            self.critic_targets_1 = [EvolvableCNN(**checkpoint['critic_targets_1_init_dict'][idx]) 
-                           for idx, _ in enumerate(self.agent_ids)]
-            self.critics_2 = [EvolvableCNN(**checkpoint['critics_2_init_dict'][idx]) 
-                           for idx, _ in enumerate(self.agent_ids)]
-            self.critic_targets_2 = [EvolvableCNN(**checkpoint['critic_targets_2_init_dict'][idx]) 
-                           for idx, _ in enumerate(self.agent_ids)]
-            
-        self.lr = checkpoint['lr']
-        self.actor_optimizers = [optim.Adam(actor.parameters(), lr=self.lr) for actor in self.actors]
-        self.critic_1_optimizers = [optim.Adam(critic_1.parameters(), lr=self.lr) for critic_1 in self.critics_1]
-        self.critic_2_optimizers = [optim.Adam(critic_2.parameters(), lr=self.lr) for critic_2 in self.critics_2]
-        actor_list = [] 
+        self.net_config = checkpoint["net_config"]
+        if self.net_config["arch"] == "mlp":
+            self.actors = [
+                EvolvableMLP(**checkpoint["actors_init_dict"][idx])
+                for idx, _ in enumerate(self.agent_ids)
+            ]
+            self.actor_targets = [
+                EvolvableMLP(**checkpoint["actor_targets_init_dict"][idx])
+                for idx, _ in enumerate(self.agent_ids)
+            ]
+            self.critics_1 = [
+                EvolvableMLP(**checkpoint["critics_1_init_dict"][idx])
+                for idx, _ in enumerate(self.agent_ids)
+            ]
+            self.critic_targets_1 = [
+                EvolvableMLP(**checkpoint["critic_targets_1_init_dict"][idx])
+                for idx, _ in enumerate(self.agent_ids)
+            ]
+            self.critics_2 = [
+                EvolvableMLP(**checkpoint["critics_2_init_dict"][idx])
+                for idx, _ in enumerate(self.agent_ids)
+            ]
+            self.critic_targets_2 = [
+                EvolvableMLP(**checkpoint["critic_targets_2_init_dict"][idx])
+                for idx, _ in enumerate(self.agent_ids)
+            ]
+        elif self.net_config["arch"] == "cnn":
+            self.actors = [
+                EvolvableCNN(**checkpoint["actors_init_dict"][idx])
+                for idx, _ in enumerate(self.agent_ids)
+            ]
+            self.actor_targets = [
+                EvolvableCNN(**checkpoint["actor_targets_init_dict"][idx])
+                for idx, _ in enumerate(self.agent_ids)
+            ]
+            self.critics_1 = [
+                EvolvableCNN(**checkpoint["critics_1_init_dict"][idx])
+                for idx, _ in enumerate(self.agent_ids)
+            ]
+            self.critic_targets_1 = [
+                EvolvableCNN(**checkpoint["critic_targets_1_init_dict"][idx])
+                for idx, _ in enumerate(self.agent_ids)
+            ]
+            self.critics_2 = [
+                EvolvableCNN(**checkpoint["critics_2_init_dict"][idx])
+                for idx, _ in enumerate(self.agent_ids)
+            ]
+            self.critic_targets_2 = [
+                EvolvableCNN(**checkpoint["critic_targets_2_init_dict"][idx])
+                for idx, _ in enumerate(self.agent_ids)
+            ]
+
+        self.lr = checkpoint["lr"]
+        self.actor_optimizers = [
+            optim.Adam(actor.parameters(), lr=self.lr) for actor in self.actors
+        ]
+        self.critic_1_optimizers = [
+            optim.Adam(critic_1.parameters(), lr=self.lr) for critic_1 in self.critics_1
+        ]
+        self.critic_2_optimizers = [
+            optim.Adam(critic_2.parameters(), lr=self.lr) for critic_2 in self.critics_2
+        ]
+        actor_list = []
         critic_1_list = []
         critic_2_list = []
         actor_target_list = []
         critic_target_1_list = []
         critic_target_2_list = []
         actor_optimizer_list = []
         critic_1_optimizer_list = []
         critic_2_optimizer_list = []
 
-        for idx, (actor, actor_target, critic_1, critic_target_1, critic_2, critic_target_2, 
-                  actor_optimizer, critic_1_optimizer, critic_2_optimizer) in enumerate(zip(self.actors,
-                                                                                            self.actor_targets,
-                                                                                            self.critics_1,
-                                                                                            self.critic_targets_1,
-                                                                                            self.critics_2,
-                                                                                            self.critic_targets_2,
-                                                                                            self.actor_optimizers,
-                                                                                            self.critic_1_optimizers,
-                                                                                            self.critic_2_optimizers)):
-            
-
-            actor.load_state_dict(checkpoint['actors_state_dict'][idx])
+        for idx, (
+            actor,
+            actor_target,
+            critic_1,
+            critic_target_1,
+            critic_2,
+            critic_target_2,
+            actor_optimizer,
+            critic_1_optimizer,
+            critic_2_optimizer,
+        ) in enumerate(
+            zip(
+                self.actors,
+                self.actor_targets,
+                self.critics_1,
+                self.critic_targets_1,
+                self.critics_2,
+                self.critic_targets_2,
+                self.actor_optimizers,
+                self.critic_1_optimizers,
+                self.critic_2_optimizers,
+            )
+        ):
+            actor.load_state_dict(checkpoint["actors_state_dict"][idx])
             actor_list.append(actor)
-            actor_target.load_state_dict(checkpoint['actor_targets_state_dict'][idx])
+            actor_target.load_state_dict(checkpoint["actor_targets_state_dict"][idx])
             actor_target_list.append(actor_target)
-            critic_1.load_state_dict(checkpoint['critics_1_state_dict'][idx])
+            critic_1.load_state_dict(checkpoint["critics_1_state_dict"][idx])
             critic_1_list.append(critic_1)
-            critic_2.load_state_dict(checkpoint['critics_2_state_dict'][idx])
+            critic_2.load_state_dict(checkpoint["critics_2_state_dict"][idx])
             critic_2_list.append(critic_2)
-            critic_target_1.load_state_dict(checkpoint['critic_targets_1_state_dict'][idx])
+            critic_target_1.load_state_dict(
+                checkpoint["critic_targets_1_state_dict"][idx]
+            )
             critic_target_1_list.append(critic_target_1)
-            actor_optimizer.load_state_dict(checkpoint['actor_optimizers_state_dict'][idx])
+            actor_optimizer.load_state_dict(
+                checkpoint["actor_optimizers_state_dict"][idx]
+            )
             actor_optimizer_list.append(actor_optimizer)
-            critic_1_optimizer.load_state_dict(checkpoint['critic_1_optimizers_state_dict'][idx])
+            critic_1_optimizer.load_state_dict(
+                checkpoint["critic_1_optimizers_state_dict"][idx]
+            )
             critic_1_optimizer_list.append(critic_1_optimizer)
-            critic_2_optimizer.load_state_dict(checkpoint['critic_2_optimizers_state_dict'][idx])
+            critic_2_optimizer.load_state_dict(
+                checkpoint["critic_2_optimizers_state_dict"][idx]
+            )
             critic_2_optimizer_list.append(critic_2_optimizer)
-        
-        self.actors = actor_list                        
-        self.actor_targets = actor_target_list          
-        self.critics_1 = critic_1_list                     
+
+        self.actors = actor_list
+        self.actor_targets = actor_target_list
+        self.critics_1 = critic_1_list
         self.critic_targets_1 = critic_target_1_list
-        self.critics_2 = critic_2_list                     
-        self.critic_targets_2 = critic_target_2_list         
-        self.actor_optimizers = actor_optimizer_list    
-        self.critic_1_optimizers =  critic_1_optimizer_list 
-        self.critic_2_optimizers =  critic_2_optimizer_list 
-        self.batch_size = checkpoint['batch_size']
-        self.learn_step = checkpoint['learn_step']
-        self.policy_freq = checkpoint['policy_freq']
-        self.gamma = checkpoint['gamma']
-        self.tau = checkpoint['tau']
-        self.mut = checkpoint['mutation']
-        self.index = checkpoint['index']
-        self.scores = checkpoint['scores']
-        self.fitness = checkpoint['fitness']
-        self.steps = checkpoint['steps']
+        self.critics_2 = critic_2_list
+        self.critic_targets_2 = critic_target_2_list
+        self.actor_optimizers = actor_optimizer_list
+        self.critic_1_optimizers = critic_1_optimizer_list
+        self.critic_2_optimizers = critic_2_optimizer_list
+        self.batch_size = checkpoint["batch_size"]
+        self.learn_step = checkpoint["learn_step"]
+        self.policy_freq = checkpoint["policy_freq"]
+        self.gamma = checkpoint["gamma"]
+        self.tau = checkpoint["tau"]
+        self.mut = checkpoint["mutation"]
+        self.index = checkpoint["index"]
+        self.scores = checkpoint["scores"]
+        self.fitness = checkpoint["fitness"]
+        self.steps = checkpoint["steps"]
```

### Comparing `agilerl-0.1.8/agilerl/algorithms/td3.py` & `agilerl-0.1.9/agilerl/algorithms/td3.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-import random
 import copy
+import random
+
 import dill
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.optim as optim
-from agilerl.networks.evolvable_mlp import EvolvableMLP
+
 from agilerl.networks.evolvable_cnn import EvolvableCNN
+from agilerl.networks.evolvable_mlp import EvolvableMLP
 
-class TD3():
+
+class TD3:
     """The TD3 algorithm class. TD3 paper: https://arxiv.org/abs/1802.09477
 
     :param state_dim: State observation dimension
     :type state_dim: int
     :param action_dim: Action dimension
     :type action_dim: int
     :param one_hot: One-hot encoding, used with discrete observation spaces
@@ -43,18 +46,35 @@
     :type device: str, optional
     :param accelerator: Accelerator for distributed computing, defaults to None
     :type accelerator: Hugging Face accelerate.Accelerator(), optional
     :param wrap: Wrap models for distributed training upon creation, defaults to True
     :type wrap: bool, optional
     """
 
-    def __init__(self, state_dim, action_dim, one_hot, max_action, expl_noise=0.1, index=0, 
-                 net_config={'arch': 'mlp', 'h_size': [64,64]}, batch_size=64, lr=1e-4, learn_step=5, gamma=0.99, 
-                 tau=0.005, mutation=None, policy_freq=2, device='cpu', accelerator=None, wrap=True):
-        self.algo = 'TD3'
+    def __init__(
+        self,
+        state_dim,
+        action_dim,
+        one_hot,
+        max_action,
+        expl_noise=0.1,
+        index=0,
+        net_config={"arch": "mlp", "h_size": [64, 64]},
+        batch_size=64,
+        lr=1e-4,
+        learn_step=5,
+        gamma=0.99,
+        tau=0.005,
+        mutation=None,
+        policy_freq=2,
+        device="cpu",
+        accelerator=None,
+        wrap=True,
+    ):
+        self.algo = "TD3"
         self.state_dim = state_dim
         self.action_dim = action_dim
         self.one_hot = one_hot
         self.net_config = net_config
         self.batch_size = batch_size
         self.lr = lr
         self.learn_step = learn_step
@@ -70,261 +90,283 @@
         self.index = index
         self.scores = []
         self.fitness = []
         self.steps = [0]
 
         # model
         # TD3 employs two critic networks
-        if self.net_config['arch'] == 'mlp':      # Multi-layer Perceptron
+        if self.net_config["arch"] == "mlp":  # Multi-layer Perceptron
             self.actor = EvolvableMLP(
                 num_inputs=state_dim[0],
                 num_outputs=action_dim,
-                hidden_size=self.net_config['h_size'],
-                output_activation='tanh',
+                hidden_size=self.net_config["h_size"],
+                output_activation="tanh",
                 device=self.device,
-                accelerator=self.accelerator)
+                accelerator=self.accelerator,
+            )
             self.actor_target = EvolvableMLP(
                 num_inputs=state_dim[0],
                 num_outputs=action_dim,
-                hidden_size=self.net_config['h_size'],
-                output_activation='tanh',
+                hidden_size=self.net_config["h_size"],
+                output_activation="tanh",
                 device=self.device,
-                accelerator=self.accelerator)
+                accelerator=self.accelerator,
+            )
             self.actor_target.load_state_dict(self.actor.state_dict())
 
             self.critic_1 = EvolvableMLP(
                 num_inputs=state_dim[0] + action_dim,
                 num_outputs=1,
-                hidden_size=self.net_config['h_size'],
+                hidden_size=self.net_config["h_size"],
                 device=self.device,
-                accelerator=self.accelerator)
+                accelerator=self.accelerator,
+            )
             self.critic_target_1 = EvolvableMLP(
                 num_inputs=state_dim[0] + action_dim,
                 num_outputs=1,
-                hidden_size=self.net_config['h_size'],
+                hidden_size=self.net_config["h_size"],
                 device=self.device,
-                accelerator=self.accelerator)
+                accelerator=self.accelerator,
+            )
 
             self.critic_2 = EvolvableMLP(
                 num_inputs=state_dim[0] + action_dim,
                 num_outputs=1,
-                hidden_size=self.net_config['h_size'],
+                hidden_size=self.net_config["h_size"],
                 device=self.device,
-                accelerator=self.accelerator)
+                accelerator=self.accelerator,
+            )
             self.critic_target_2 = EvolvableMLP(
                 num_inputs=state_dim[0] + action_dim,
                 num_outputs=1,
-                hidden_size=self.net_config['h_size'],
+                hidden_size=self.net_config["h_size"],
                 device=self.device,
-                accelerator=self.accelerator)
+                accelerator=self.accelerator,
+            )
 
             self.critic_target_1.load_state_dict(self.critic_1.state_dict())
             self.critic_target_2.load_state_dict(self.critic_2.state_dict())
 
-        elif self.net_config['arch'] == 'cnn':    # Convolutional Neural Network
+        elif self.net_config["arch"] == "cnn":  # Convolutional Neural Network
             self.actor = EvolvableCNN(
                 input_shape=state_dim,
                 num_actions=action_dim,
-                channel_size=self.net_config['c_size'],
-                kernal_size=self.net_config['k_size'],
-                stride_size=self.net_config['s_size'],
-                hidden_size=self.net_config['h_size'],
-                normalize=self.net_config['normalize'],
-                mlp_activation='tanh',
+                channel_size=self.net_config["c_size"],
+                kernal_size=self.net_config["k_size"],
+                stride_size=self.net_config["s_size"],
+                hidden_size=self.net_config["h_size"],
+                normalize=self.net_config["normalize"],
+                mlp_activation="tanh",
                 device=self.device,
-                accelerator=self.accelerator)
+                accelerator=self.accelerator,
+            )
             self.actor_target = EvolvableCNN(
                 input_shape=state_dim,
                 num_actions=action_dim,
-                channel_size=self.net_config['c_size'],
-                kernal_size=self.net_config['k_size'],
-                stride_size=self.net_config['s_size'],
-                hidden_size=self.net_config['h_size'],
-                normalize=self.net_config['normalize'],
-                mlp_activation='tanh',
+                channel_size=self.net_config["c_size"],
+                kernal_size=self.net_config["k_size"],
+                stride_size=self.net_config["s_size"],
+                hidden_size=self.net_config["h_size"],
+                normalize=self.net_config["normalize"],
+                mlp_activation="tanh",
                 device=self.device,
-                accelerator=self.accelerator)
+                accelerator=self.accelerator,
+            )
             self.actor_target.load_state_dict(self.actor.state_dict())
 
             self.critic_1 = EvolvableCNN(
                 input_shape=state_dim,
                 num_actions=action_dim,
-                channel_size=self.net_config['c_size'],
-                kernal_size=self.net_config['k_size'],
-                stride_size=self.net_config['s_size'],
-                hidden_size=self.net_config['h_size'],
-                normalize=self.net_config['normalize'],
-                mlp_activation='tanh',
+                channel_size=self.net_config["c_size"],
+                kernal_size=self.net_config["k_size"],
+                stride_size=self.net_config["s_size"],
+                hidden_size=self.net_config["h_size"],
+                normalize=self.net_config["normalize"],
+                mlp_activation="tanh",
                 critic=True,
                 device=self.device,
-                accelerator=self.accelerator)
+                accelerator=self.accelerator,
+            )
             self.critic_target_1 = EvolvableCNN(
                 input_shape=state_dim,
                 num_actions=action_dim,
-                channel_size=self.net_config['c_size'],
-                kernal_size=self.net_config['k_size'],
-                stride_size=self.net_config['s_size'],
-                hidden_size=self.net_config['h_size'],
-                normalize=self.net_config['normalize'],
-                mlp_activation='tanh',
+                channel_size=self.net_config["c_size"],
+                kernal_size=self.net_config["k_size"],
+                stride_size=self.net_config["s_size"],
+                hidden_size=self.net_config["h_size"],
+                normalize=self.net_config["normalize"],
+                mlp_activation="tanh",
                 critic=True,
                 device=self.device,
-                accelerator=self.accelerator)
+                accelerator=self.accelerator,
+            )
 
             self.critic_2 = EvolvableCNN(
                 input_shape=state_dim,
                 num_actions=action_dim,
-                channel_size=self.net_config['c_size'],
-                kernal_size=self.net_config['k_size'],
-                stride_size=self.net_config['s_size'],
-                hidden_size=self.net_config['h_size'],
-                normalize=self.net_config['normalize'],
-                mlp_activation='tanh',
+                channel_size=self.net_config["c_size"],
+                kernal_size=self.net_config["k_size"],
+                stride_size=self.net_config["s_size"],
+                hidden_size=self.net_config["h_size"],
+                normalize=self.net_config["normalize"],
+                mlp_activation="tanh",
                 critic=True,
                 device=self.device,
-                accelerator=self.accelerator)
+                accelerator=self.accelerator,
+            )
             self.critic_target_2 = EvolvableCNN(
                 input_shape=state_dim,
                 num_actions=action_dim,
-                channel_size=self.net_config['c_size'],
-                kernal_size=self.net_config['k_size'],
-                stride_size=self.net_config['s_size'],
-                hidden_size=self.net_config['h_size'],
-                normalize=self.net_config['normalize'],
-                mlp_activation='tanh',
+                channel_size=self.net_config["c_size"],
+                kernal_size=self.net_config["k_size"],
+                stride_size=self.net_config["s_size"],
+                hidden_size=self.net_config["h_size"],
+                normalize=self.net_config["normalize"],
+                mlp_activation="tanh",
                 critic=True,
                 device=self.device,
-                accelerator=self.accelerator)
-        
+                accelerator=self.accelerator,
+            )
+
             self.critic_target_1.load_state_dict(self.critic_1.state_dict())
             self.critic_target_2.load_state_dict(self.critic_2.state_dict())
 
         self.actor_optimizer_type = optim.Adam(self.actor.parameters(), lr=self.lr)
-        self.critic_1_optimizer_type = optim.Adam(self.critic_1.parameters(), lr=self.lr)
-        self.critic_2_optimizer_type = optim.Adam(self.critic_2.parameters(), lr=self.lr)
-        
+        self.critic_1_optimizer_type = optim.Adam(
+            self.critic_1.parameters(), lr=self.lr
+        )
+        self.critic_2_optimizer_type = optim.Adam(
+            self.critic_2.parameters(), lr=self.lr
+        )
+
         if self.accelerator is not None:
             self.actor_optimizer = self.actor_optimizer_type
             self.critic_1_optimizer = self.critic_1_optimizer_type
             self.critic_2_optimizer = self.critic_2_optimizer_type
             if wrap:
-                self.wrap_models()          
+                self.wrap_models()
         else:
             self.actor = self.actor.to(self.device)
             self.actor_target = self.actor_target.to(self.device)
             self.critic_1 = self.critic_1.to(self.device)
             self.critic_target_1 = self.critic_target_1.to(self.device)
             self.critic_2 = self.critic_2.to(self.device)
             self.critic_target_2 = self.critic_target_2.to(self.device)
             self.actor_optimizer = self.actor_optimizer_type
             self.critic_1_optimizer = self.critic_1_optimizer_type
             self.critic_2_optimizer = self.critic_2_optimizer_type
-        
+
         self.criterion = nn.MSELoss()
 
     def getAction(self, state, epsilon=0):
-        """Returns the next action to take in the environment, noise is added to aid exploration. 
+        """Returns the next action to take in the environment, noise is added to aid exploration.
         Epsilon is the probability of taking a random action, used for exploration.
         For epsilon-greedy behaviour, set epsilon to 0.
 
         :param state: Environment observation, or multiple observations in a batch
         :type state: float or List[float]
         :param epsilon: Probablilty of taking a random action for exploration, defaults to 0
         :type epsilon: float, optional
         """
         state = torch.from_numpy(state).float().to(self.device)
 
         if self.one_hot:
-            state = nn.functional.one_hot(
-                state.long(), num_classes=self.state_dim[0]).float().squeeze()
+            state = (
+                nn.functional.one_hot(state.long(), num_classes=self.state_dim[0])
+                .float()
+                .squeeze()
+            )
 
         if len(state.size()) < 2:
-            state = state.unsqueeze(0)       
+            state = state.unsqueeze(0)
 
         # epsilon-greedy, Gaussian noise added to aid exploration
         if random.random() < epsilon:
-            action = (np.random.rand(
-                state.size()[0], self.action_dim).astype('float32') - 0.5) * 2
+            action = (
+                np.random.rand(state.size()[0], self.action_dim).astype("float32") - 0.5
+            ) * 2
         else:
             self.actor.eval()
             with torch.no_grad():
                 action_values = self.actor(state)
             self.actor.train()
 
-            action = (
-                action_values.cpu().data.numpy()
-                + np.random.normal(0, self.max_action * self.expl_noise, size=self.action_dim
+            action = action_values.cpu().data.numpy() + np.random.normal(
+                0, self.max_action * self.expl_noise, size=self.action_dim
             ).astype(np.float32).clip(-self.max_action, self.max_action)
-            )
         return action
 
     def learn(self, experiences, noise_clip=0.5, policy_noise=0.2):
         """Updates agent network parameters to learn from experiences.
 
         :param experience: List of batched states, actions, rewards, next_states, dones in that order.
         :type experience: List[torch.Tensor[float]]
         :param noise_clip: Maximum noise limit to apply to actions, defaults to 0.5
         :type noise_clip: float, optional
         :param policy_noise: Standard deviation of noise applied to policy, defaults to 0.2
         :type policy_noise: float, optional
         """
         states, actions, rewards, next_states, dones = experiences
-        
+
         if self.one_hot:
-            states = nn.functional.one_hot(
-                states.long(), num_classes=self.state_dim[0]).float().squeeze()
-            next_states = nn.functional.one_hot(
-                next_states.long(), num_classes=self.state_dim[0]).float().squeeze()
-        
-        if self.net_config['arch'] == 'mlp':
+            states = (
+                nn.functional.one_hot(states.long(), num_classes=self.state_dim[0])
+                .float()
+                .squeeze()
+            )
+            next_states = (
+                nn.functional.one_hot(next_states.long(), num_classes=self.state_dim[0])
+                .float()
+                .squeeze()
+            )
+
+        if self.net_config["arch"] == "mlp":
             input_combined = torch.cat([states, actions], 1)
             q_value_1 = self.critic_1(input_combined)
             q_value_2 = self.critic_2(input_combined)
-        elif self.net_config['arch'] == 'cnn':
+        elif self.net_config["arch"] == "cnn":
             q_value_1 = self.critic_1(states, actions)
             q_value_2 = self.critic_2(states, actions)
 
         next_actions = self.actor_target(next_states)
         noise = actions.data.normal_(0, policy_noise).to(self.device)
         noise = noise.clamp(-noise_clip, noise_clip)
-        next_actions = (next_actions + noise)
+        next_actions = next_actions + noise
 
         # Compute the target, y_j, making use of twin critic networks
-        if self.net_config['arch'] == 'mlp':
+        if self.net_config["arch"] == "mlp":
             next_input_combined = torch.cat([next_states, next_actions], 1)
             q_value_next_state_1 = self.critic_target_1(next_input_combined)
             q_value_next_state_2 = self.critic_target_2(next_input_combined)
-        elif self.net_config['arch'] == 'cnn':
+        elif self.net_config["arch"] == "cnn":
             q_value_next_state_1 = self.critic_target_1(next_states, next_actions)
             q_value_next_state_2 = self.critic_target_2(next_states, next_actions)
         q_value_next_state = torch.min(q_value_next_state_1, q_value_next_state_2)
-        y_j = rewards + ((1- dones)*self.gamma * q_value_next_state).detach()
+        y_j = rewards + ((1 - dones) * self.gamma * q_value_next_state).detach()
 
         # Loss equation needs to be updated to account for two q_values from two critics
-        critic_loss = self.criterion(q_value_1, y_j) + self.criterion(q_value_2, y_j) 
-      
+        critic_loss = self.criterion(q_value_1, y_j) + self.criterion(q_value_2, y_j)
+
         # critic loss backprop
         self.critic_1_optimizer.zero_grad()
         self.critic_2_optimizer.zero_grad()
         if self.accelerator is not None:
             self.accelerator.backward(critic_loss)
         else:
             critic_loss.backward()
         self.critic_1_optimizer.step()
         self.critic_2_optimizer.step()
 
         # update actor and targets every policy_freq episodes
         if len(self.scores) % self.policy_freq == 0:
-            if self.net_config['arch'] == 'mlp':
-                input_combined = torch.cat(
-                    [states, self.actor.forward(states)], 1)
+            if self.net_config["arch"] == "mlp":
+                input_combined = torch.cat([states, self.actor.forward(states)], 1)
                 actor_loss = -self.critic_1(input_combined).mean()
-            elif self.net_config['arch'] == 'cnn':
-                actor_loss = - \
-                    self.critic_1(states, self.actor.forward(states)).mean()
+            elif self.net_config["arch"] == "cnn":
+                actor_loss = -self.critic_1(states, self.actor.forward(states)).mean()
 
             # actor loss backprop
             self.actor_optimizer.zero_grad()
             if self.accelerator is not None:
                 self.accelerator.backward(actor_loss)
             else:
                 actor_loss.backward()
@@ -332,19 +374,19 @@
 
             # Add in a soft update for both critic_targets
             self.softUpdate(self.actor, self.actor_target)
             self.softUpdate(self.critic_1, self.critic_target_1)
             self.softUpdate(self.critic_2, self.critic_target_2)
 
     def softUpdate(self, net, target):
-        """Soft updates target network.
-        """
+        """Soft updates target network."""
         for eval_param, target_param in zip(net.parameters(), target.parameters()):
             target_param.data.copy_(
-                self.tau * eval_param.data + (1.0 - self.tau) * target_param.data)
+                self.tau * eval_param.data + (1.0 - self.tau) * target_param.data
+            )
 
     def test(self, env, swap_channels=False, max_steps=500, loop=3):
         """Returns mean test score of agent in environment with epsilon-greedy policy.
 
         :param env: The environment to be tested in
         :type env: Gym-style environment
         :param swap_channels: Swap image channels dimension from last to first [H, W, C] -> [C, H, W], defaults to False
@@ -375,31 +417,33 @@
 
         :param index: Index to keep track of agent for tournament selection and mutation, defaults to None
         :type index: int, optional
         """
         if index is None:
             index = self.index
 
-        clone = type(self)(state_dim=self.state_dim,
-                           action_dim=self.action_dim,
-                           one_hot=self.one_hot,
-                           max_action=self.max_action,
-                           expl_noise=self.expl_noise,
-                           index=index,
-                           net_config=self.net_config,
-                           batch_size=self.batch_size,
-                           lr=self.lr,
-                           learn_step=self.learn_step,
-                           gamma=self.gamma,
-                           tau=self.tau,
-                           mutation=self.mut,
-                           policy_freq=self.policy_freq,
-                           device=self.device,
-                           accelerator=self.accelerator,
-                           wrap=wrap)
+        clone = type(self)(
+            state_dim=self.state_dim,
+            action_dim=self.action_dim,
+            one_hot=self.one_hot,
+            max_action=self.max_action,
+            expl_noise=self.expl_noise,
+            index=index,
+            net_config=self.net_config,
+            batch_size=self.batch_size,
+            lr=self.lr,
+            learn_step=self.learn_step,
+            gamma=self.gamma,
+            tau=self.tau,
+            mutation=self.mut,
+            policy_freq=self.policy_freq,
+            device=self.device,
+            accelerator=self.accelerator,
+            wrap=wrap,
+        )
 
         if self.accelerator is not None:
             self.unwrap_models()
         actor = self.actor.clone()
         actor_target = self.actor_target.clone()
         critic_1 = self.critic_1.clone()
         critic_target_1 = self.critic_target_1.clone()
@@ -412,30 +456,57 @@
 
         clone.actor_optimizer_type = actor_optimizer
         clone.critic_1_optimizer_type = critic_1_optimizer
         clone.critic_2_optimizer_type = critic_2_optimizer
 
         if self.accelerator is not None:
             if wrap:
-                clone.actor, clone.actor_target, clone.critic_1, clone.critic_target_1, \
-                clone.critic_2, clone.critic_target_2, clone.actor_optimizer, \
-                clone.critic_1_optimizer, clone.critic_2_optimizer = self.accelerator.prepare(actor,
-                                                                                            actor_target,
-                                                                                            critic_1,
-                                                                                            critic_target_1,
-                                                                                            critic_2,
-                                                                                            critic_target_2,
-                                                                                            actor_optimizer,
-                                                                                            critic_1_optimizer,
-                                                                                            critic_2_optimizer)
+                (
+                    clone.actor,
+                    clone.actor_target,
+                    clone.critic_1,
+                    clone.critic_target_1,
+                    clone.critic_2,
+                    clone.critic_target_2,
+                    clone.actor_optimizer,
+                    clone.critic_1_optimizer,
+                    clone.critic_2_optimizer,
+                ) = self.accelerator.prepare(
+                    actor,
+                    actor_target,
+                    critic_1,
+                    critic_target_1,
+                    critic_2,
+                    critic_target_2,
+                    actor_optimizer,
+                    critic_1_optimizer,
+                    critic_2_optimizer,
+                )
             else:
-                clone.actor, clone.actor_target, clone.critic_1, clone.critic_target_1, clone.critic_2, \
-                clone.critic_target_2, clone.actor_optimizer, clone.critic_1_optimizer, \
-                clone.critic_1_optimizer = actor, actor_target, critic_1, critic_target_1, critic_2, \
-                critic_target_2, actor_optimizer, critic_1_optimizer, critic_2_optimizer
+                (
+                    clone.actor,
+                    clone.actor_target,
+                    clone.critic_1,
+                    clone.critic_target_1,
+                    clone.critic_2,
+                    clone.critic_target_2,
+                    clone.actor_optimizer,
+                    clone.critic_1_optimizer,
+                    clone.critic_1_optimizer,
+                ) = (
+                    actor,
+                    actor_target,
+                    critic_1,
+                    critic_target_1,
+                    critic_2,
+                    critic_target_2,
+                    actor_optimizer,
+                    critic_1_optimizer,
+                    critic_2_optimizer,
+                )
         else:
             clone.actor = actor.to(self.device)
             clone.actor_target = actor_target.to(self.device)
             clone.critic_1 = critic_1.to(self.device)
             clone.critic_target_1 = critic_target_1.to(self.device)
             clone.critic_2 = critic_2.to(self.device)
             clone.critic_target_2 = critic_target_2.to(self.device)
@@ -444,117 +515,147 @@
             clone.critic_2_optimizer = critic_2_optimizer
 
         clone.fitness = copy.deepcopy(self.fitness)
         clone.steps = copy.deepcopy(self.steps)
         clone.scores = copy.deepcopy(self.scores)
 
         return clone
-    
+
     def wrap_models(self):
         if self.accelerator is not None:
-            self.actor, self.actor_target, self.critic_1, self.critic_target_1, \
-            self.critic_2, self.critic_target_2, self.actor_optimizer, \
-            self.critic_1_optimizer, self.critic_2_optimizer = self.accelerator.prepare(self.actor,
-                                                                                        self.actor_target,
-                                                                                        self.critic_1,
-                                                                                        self.critic_target_1,
-                                                                                        self.critic_2,
-                                                                                        self.critic_target_2,
-                                                                                        self.actor_optimizer_type,
-                                                                                        self.critic_1_optimizer_type,
-                                                                                        self.critic_2_optimizer_type)
-    
+            (
+                self.actor,
+                self.actor_target,
+                self.critic_1,
+                self.critic_target_1,
+                self.critic_2,
+                self.critic_target_2,
+                self.actor_optimizer,
+                self.critic_1_optimizer,
+                self.critic_2_optimizer,
+            ) = self.accelerator.prepare(
+                self.actor,
+                self.actor_target,
+                self.critic_1,
+                self.critic_target_1,
+                self.critic_2,
+                self.critic_target_2,
+                self.actor_optimizer_type,
+                self.critic_1_optimizer_type,
+                self.critic_2_optimizer_type,
+            )
+
     def unwrap_models(self):
         if self.accelerator is not None:
             self.actor = self.accelerator.unwrap_model(self.actor)
             self.actor_target = self.accelerator.unwrap_model(self.actor_target)
             self.critic_1 = self.accelerator.unwrap_model(self.critic_1)
             self.critic_target_1 = self.accelerator.unwrap_model(self.critic_target_1)
             self.critic_2 = self.accelerator.unwrap_model(self.critic_2)
             self.critic_target_2 = self.accelerator.unwrap_model(self.critic_target_2)
             self.actor_optimizer = self.accelerator.unwrap_model(self.actor_optimizer)
-            self.critic_1_optimizer = self.accelerator.unwrap_model(self.critic_1_optimizer)
-            self.critic_2_optimizer = self.accelerator.unwrap_model(self.critic_2_optimizer)
+            self.critic_1_optimizer = self.accelerator.unwrap_model(
+                self.critic_1_optimizer
+            )
+            self.critic_2_optimizer = self.accelerator.unwrap_model(
+                self.critic_2_optimizer
+            )
 
     def saveCheckpoint(self, path):
         """Saves a checkpoint of agent properties and network weights to path.
 
         :param path: Location to save checkpoint at
         :type path: string
         """
-        torch.save({
-            'actor_init_dict': self.actor.init_dict,
-            'actor_state_dict': self.actor.state_dict(),
-            'actor_target_init_dict': self.actor_target.init_dict,
-            'actor_target_state_dict': self.actor_target.state_dict(),
-            'critic_1_init_dict': self.critic_1.init_dict,
-            'critic_1_state_dict': self.critic_1.state_dict(),
-            'critic_target_1_init_dict': self.critic_target_1.init_dict,
-            'critic_target_1_state_dict': self.critic_target_1.state_dict(),
-            'critic_2_init_dict': self.critic_2.init_dict,
-            'critic_2_state_dict': self.critic_2.state_dict(),
-            'critic_target_2_init_dict': self.critic_target_2.init_dict,
-            'critic_target_2_state_dict': self.critic_target_2.state_dict(),
-            'actor_optimizer_state_dict': self.actor_optimizer.state_dict(),
-            'critic_1_optimizer_state_dict': self.critic_1_optimizer.state_dict(),
-            'critic_2_optimizer_state_dict': self.critic_2_optimizer.state_dict(),
-            'net_config': self.net_config,
-            'batch_size': self.batch_size,
-            'lr': self.lr,
-            'learn_step': self.learn_step,
-            'gamma': self.gamma,
-            'tau': self.tau,
-            'mutation': self.mut,
-            'max_action':self.max_action,
-            'expl_noise':self.expl_noise,
-            'index': self.index,
-            'scores': self.scores,
-            'fitness': self.fitness,
-            'steps': self.steps,
-        }, path, pickle_module=dill)
+        torch.save(
+            {
+                "actor_init_dict": self.actor.init_dict,
+                "actor_state_dict": self.actor.state_dict(),
+                "actor_target_init_dict": self.actor_target.init_dict,
+                "actor_target_state_dict": self.actor_target.state_dict(),
+                "critic_1_init_dict": self.critic_1.init_dict,
+                "critic_1_state_dict": self.critic_1.state_dict(),
+                "critic_target_1_init_dict": self.critic_target_1.init_dict,
+                "critic_target_1_state_dict": self.critic_target_1.state_dict(),
+                "critic_2_init_dict": self.critic_2.init_dict,
+                "critic_2_state_dict": self.critic_2.state_dict(),
+                "critic_target_2_init_dict": self.critic_target_2.init_dict,
+                "critic_target_2_state_dict": self.critic_target_2.state_dict(),
+                "actor_optimizer_state_dict": self.actor_optimizer.state_dict(),
+                "critic_1_optimizer_state_dict": self.critic_1_optimizer.state_dict(),
+                "critic_2_optimizer_state_dict": self.critic_2_optimizer.state_dict(),
+                "net_config": self.net_config,
+                "batch_size": self.batch_size,
+                "lr": self.lr,
+                "learn_step": self.learn_step,
+                "gamma": self.gamma,
+                "tau": self.tau,
+                "mutation": self.mut,
+                "max_action": self.max_action,
+                "expl_noise": self.expl_noise,
+                "index": self.index,
+                "scores": self.scores,
+                "fitness": self.fitness,
+                "steps": self.steps,
+            },
+            path,
+            pickle_module=dill,
+        )
 
     def loadCheckpoint(self, path):
         """Loads saved agent properties and network weights from checkpoint.
 
         :param path: Location to load checkpoint from
         :type path: string
         """
         checkpoint = torch.load(path, pickle_module=dill)
-        self.net_config = checkpoint['net_config']
-        if self.net_config['arch'] == 'mlp':
-            self.actor = EvolvableMLP(**checkpoint['actor_init_dict'])
-            self.actor_target = EvolvableMLP(**checkpoint['actor_target_init_dict'])
-            self.critic_1 = EvolvableMLP(**checkpoint['critic_1_init_dict'])
-            self.critic_target_1 = EvolvableMLP(**checkpoint['critic_target_1_init_dict'])
-            self.critic_2 = EvolvableMLP(**checkpoint['critic_2_init_dict'])
-            self.critic_target_2 = EvolvableMLP(**checkpoint['critic_target_2_init_dict'])
-        elif self.net_config['arch'] == 'cnn':
-            self.actor = EvolvableCNN(**checkpoint['actor_init_dict'])
-            self.actor_target = EvolvableCNN(**checkpoint['actor_target_init_dict'])
-            self.critic_1 = EvolvableCNN(**checkpoint['critic_1_init_dict'])
-            self.critic_target_1 = EvolvableCNN(**checkpoint['critic_target_1_init_dict'])
-            self.critic_2 = EvolvableCNN(**checkpoint['critic_2_init_dict'])
-            self.critic_target_2 = EvolvableCNN(**checkpoint['critic_target_2_init_dict'])
-        self.lr = checkpoint['lr']
+        self.net_config = checkpoint["net_config"]
+        if self.net_config["arch"] == "mlp":
+            self.actor = EvolvableMLP(**checkpoint["actor_init_dict"])
+            self.actor_target = EvolvableMLP(**checkpoint["actor_target_init_dict"])
+            self.critic_1 = EvolvableMLP(**checkpoint["critic_1_init_dict"])
+            self.critic_target_1 = EvolvableMLP(
+                **checkpoint["critic_target_1_init_dict"]
+            )
+            self.critic_2 = EvolvableMLP(**checkpoint["critic_2_init_dict"])
+            self.critic_target_2 = EvolvableMLP(
+                **checkpoint["critic_target_2_init_dict"]
+            )
+        elif self.net_config["arch"] == "cnn":
+            self.actor = EvolvableCNN(**checkpoint["actor_init_dict"])
+            self.actor_target = EvolvableCNN(**checkpoint["actor_target_init_dict"])
+            self.critic_1 = EvolvableCNN(**checkpoint["critic_1_init_dict"])
+            self.critic_target_1 = EvolvableCNN(
+                **checkpoint["critic_target_1_init_dict"]
+            )
+            self.critic_2 = EvolvableCNN(**checkpoint["critic_2_init_dict"])
+            self.critic_target_2 = EvolvableCNN(
+                **checkpoint["critic_target_2_init_dict"]
+            )
+        self.lr = checkpoint["lr"]
         self.actor_optimizer = optim.Adam(self.actor.parameters(), lr=self.lr)
         self.critic_1_optimizer = optim.Adam(self.critic_1.parameters(), lr=self.lr)
         self.critic_2_optimizer = optim.Adam(self.critic_2.parameters(), lr=self.lr)
-        self.actor.load_state_dict(checkpoint['actor_state_dict'])
-        self.actor_target.load_state_dict(checkpoint['actor_target_state_dict'])
-        self.critic_1.load_state_dict(checkpoint['critic_1_state_dict'])
-        self.critic_target_1.load_state_dict(checkpoint['critic_target_1_state_dict'])
-        self.critic_2.load_state_dict(checkpoint['critic_2_state_dict'])
-        self.critic_target_2.load_state_dict(checkpoint['critic_target_2_state_dict'])
-        self.actor_optimizer.load_state_dict(checkpoint['actor_optimizer_state_dict'])
-        self.critic_1_optimizer.load_state_dict(checkpoint['critic_1_optimizer_state_dict'])
-        self.critic_2_optimizer.load_state_dict(checkpoint['critic_2_optimizer_state_dict'])
-        self.batch_size = checkpoint['batch_size']
-        self.learn_step = checkpoint['learn_step']
-        self.gamma = checkpoint['gamma']
-        self.tau = checkpoint['tau']
-        self.mut = checkpoint['mutation']
-        self.max_action = checkpoint['max_action']
-        self.expl_noise = checkpoint['expl_noise']
-        self.index = checkpoint['index']
-        self.scores = checkpoint['scores']
-        self.fitness = checkpoint['fitness']
-        self.steps = checkpoint['steps']
+        self.actor.load_state_dict(checkpoint["actor_state_dict"])
+        self.actor_target.load_state_dict(checkpoint["actor_target_state_dict"])
+        self.critic_1.load_state_dict(checkpoint["critic_1_state_dict"])
+        self.critic_target_1.load_state_dict(checkpoint["critic_target_1_state_dict"])
+        self.critic_2.load_state_dict(checkpoint["critic_2_state_dict"])
+        self.critic_target_2.load_state_dict(checkpoint["critic_target_2_state_dict"])
+        self.actor_optimizer.load_state_dict(checkpoint["actor_optimizer_state_dict"])
+        self.critic_1_optimizer.load_state_dict(
+            checkpoint["critic_1_optimizer_state_dict"]
+        )
+        self.critic_2_optimizer.load_state_dict(
+            checkpoint["critic_2_optimizer_state_dict"]
+        )
+        self.batch_size = checkpoint["batch_size"]
+        self.learn_step = checkpoint["learn_step"]
+        self.gamma = checkpoint["gamma"]
+        self.tau = checkpoint["tau"]
+        self.mut = checkpoint["mutation"]
+        self.max_action = checkpoint["max_action"]
+        self.expl_noise = checkpoint["expl_noise"]
+        self.index = checkpoint["index"]
+        self.scores = checkpoint["scores"]
+        self.fitness = checkpoint["fitness"]
+        self.steps = checkpoint["steps"]
```

### Comparing `agilerl-0.1.8/agilerl/components/multi_agent_replay_buffer.py` & `agilerl-0.1.9/agilerl/components/multi_agent_replay_buffer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,122 @@
-import torch
-import numpy as np
-from collections import deque, namedtuple
 import random
+from collections import deque, namedtuple
+
+import numpy as np
+import torch
 
 
 class MultiAgentReplayBuffer:
-    '''The Multi-Agent Experience Replay Buffer class. Used to store multiple agents'
+    """The Multi-Agent Experience Replay Buffer class. Used to store multiple agents'
     experiences and allow off-policy learning.
 
     :param memory_size: Maximum length of the replay buffer
     :type memory_size: int
     :param field_names: Field names for experience named tuple, e.g. ['state', 'action', 'reward']
     :type field_names: List[str]
     :param agent_ids: Names of all agents that will act in the environment
     :type agent_ids: List[str]
     :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to None
     :type device: str, optional
 
-    '''
+    """
+
     def __init__(self, memory_size, field_names, agent_ids, device=None):
         self.memory = memory_size
         self.memory = deque(maxlen=memory_size)
-        self.experience = namedtuple('Experience', field_names=field_names)
+        self.experience = namedtuple("Experience", field_names=field_names)
         self.counter = 0
         self.device = device
         self.agent_ids = agent_ids
 
     def __len__(self):
         return len(self.memory)
-    
+
     def _add(self, state, action, reward, next_state, done):
         e = self.experience(state, action, reward, next_state, done)
         self.memory.append(e)
 
     def sample(self, batch_size):
         """Returns sample of experiences from memory.
 
         :param batch_size: Number of samples to return
         :type batch_size: int
         """
         experiences = random.sample(self.memory, k=batch_size)
 
         if self.device is not None:
-            states = {agent_id: torch.from_numpy(np.stack([e.state[agent_id] for e in experiences])).to(self.device) for agent_id in self.agent_ids}
-            actions = {agent_id: torch.from_numpy(np.stack([e.action[agent_id] for e in experiences])).to(self.device) for agent_id in self.agent_ids}
-            rewards = {agent_id: torch.from_numpy(np.vstack([e.reward[agent_id] for e in experiences])).float().to(self.device) for agent_id in self.agent_ids}
-            next_states = {agent_id: torch.from_numpy(np.stack([e.next_state[agent_id] for e in experiences])).float().to(self.device) for agent_id in self.agent_ids}
-            dones = {agent_id: torch.from_numpy(np.vstack([e.done[agent_id] for e in experiences]).astype(np.uint8)).float().to(self.device) for agent_id in self.agent_ids}
+            states = {
+                agent_id: torch.from_numpy(
+                    np.stack([e.state[agent_id] for e in experiences])
+                ).to(self.device)
+                for agent_id in self.agent_ids
+            }
+            actions = {
+                agent_id: torch.from_numpy(
+                    np.stack([e.action[agent_id] for e in experiences])
+                ).to(self.device)
+                for agent_id in self.agent_ids
+            }
+            rewards = {
+                agent_id: torch.from_numpy(
+                    np.vstack([e.reward[agent_id] for e in experiences])
+                )
+                .float()
+                .to(self.device)
+                for agent_id in self.agent_ids
+            }
+            next_states = {
+                agent_id: torch.from_numpy(
+                    np.stack([e.next_state[agent_id] for e in experiences])
+                )
+                .float()
+                .to(self.device)
+                for agent_id in self.agent_ids
+            }
+            dones = {
+                agent_id: torch.from_numpy(
+                    np.vstack([e.done[agent_id] for e in experiences]).astype(np.uint8)
+                )
+                .float()
+                .to(self.device)
+                for agent_id in self.agent_ids
+            }
         else:
-            states = {agent_id: torch.from_numpy(np.stack([e.state[agent_id] for e in experiences])) for agent_id in self.agent_ids}
-            actions = {agent_id: torch.from_numpy(np.stack([e.action[agent_id] for e in experiences])) for agent_id in self.agent_ids}
-            rewards = {agent_id: torch.from_numpy(np.vstack([e.reward[agent_id] for e in experiences])).float() for agent_id in self.agent_ids}
-            next_states = {agent_id: torch.from_numpy(np.stack([e.next_state[agent_id] for e in experiences])).float()for agent_id in self.agent_ids}
-            dones = {agent_id: torch.from_numpy(np.vstack([e.done[agent_id] for e in experiences]).astype(np.uint8)).float() for agent_id in self.agent_ids}
-        
-        return states, actions, rewards, next_states, dones
+            states = {
+                agent_id: torch.from_numpy(
+                    np.stack([e.state[agent_id] for e in experiences])
+                )
+                for agent_id in self.agent_ids
+            }
+            actions = {
+                agent_id: torch.from_numpy(
+                    np.stack([e.action[agent_id] for e in experiences])
+                )
+                for agent_id in self.agent_ids
+            }
+            rewards = {
+                agent_id: torch.from_numpy(
+                    np.vstack([e.reward[agent_id] for e in experiences])
+                ).float()
+                for agent_id in self.agent_ids
+            }
+            next_states = {
+                agent_id: torch.from_numpy(
+                    np.stack([e.next_state[agent_id] for e in experiences])
+                ).float()
+                for agent_id in self.agent_ids
+            }
+            dones = {
+                agent_id: torch.from_numpy(
+                    np.vstack([e.done[agent_id] for e in experiences]).astype(np.uint8)
+                ).float()
+                for agent_id in self.agent_ids
+            }
 
+        return states, actions, rewards, next_states, dones
 
     def save2memory(self, state, action, reward, next_state, done):
         """Saves experience to memory.
 
         :param state: Environment observation
         :type state: Dict[str, numpy.Array]
         :param action: Action in environment
@@ -69,12 +126,7 @@
         :param next_state: Environment observation of next state
         :type next_state: Dict[str, numpy.Array]
         :param done: True if environment episode finished, else False
         :type done: Dict[str, bool]
         """
         self._add(state, action, reward, next_state, done)
         self.counter += 1
-
-    
-        
-
-
```

### Comparing `agilerl-0.1.8/agilerl/components/replay_buffer.py` & `agilerl-0.1.9/agilerl/components/replay_buffer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,95 +1,106 @@
-import torch
-import numpy as np
-from collections import deque, namedtuple
-import random
-
-
-class ReplayBuffer():
-    """The Experience Replay Buffer class. Used to store experiences and allow 
-    off-policy learning.
-
-    :param n_actions: Action dimension
-    :type n_actions: int
-    :param memory_size: Maximum length of replay buffer
-    :type memory_size: int
-    :param field_names: Field names for experience named tuple, e.g. ['state', 'action', 'reward']
-    :type field_names: List[str]
-    :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to None
-    :type device: str, optional
-    """
-
-    def __init__(self, action_dim, memory_size, field_names, device=None):
-        self.n_actions = action_dim
-        self.memory = deque(maxlen=memory_size)
-        self.experience = namedtuple("Experience", field_names=field_names)
-        self.counter = 0    # update cycle counter
-        self.device = device
-
-    def __len__(self):
-        return len(self.memory)
-
-    def _add(self, state, action, reward, next_state, done):
-        e = self.experience(state, action, reward, next_state, done)
-        self.memory.append(e)
-
-    def sample(self, batch_size):
-        """Returns sample of experiences from memory.
-
-        :param batch_size: Number of samples to return
-        :type batch_size: int
-        """
-        experiences = random.sample(self.memory, k=batch_size)
-
-        states = torch.from_numpy(np.stack(
-            [e.state for e in experiences if e is not None], axis=0))
-        actions = torch.from_numpy(
-            np.vstack([e.action for e in experiences if e is not None]))
-        rewards = torch.from_numpy(np.vstack(
-            [e.reward for e in experiences if e is not None])).float()
-        next_states = torch.from_numpy(np.stack(
-            [e.next_state for e in experiences if e is not None], axis=0)).float()
-        dones = torch.from_numpy(np.vstack([e.done for e in experiences if e is not None]).astype(
-            np.uint8)).float()
-        
-        if self.device is not None:
-            states, actions, rewards, next_states, dones = states.to(self.device), \
-                actions.to(self.device), rewards.to(self.device), \
-                    next_states.to(self.device), dones.to(self.device)
-
-        return (states, actions, rewards, next_states, dones)
-
-    def save2memory(self, state, action, reward, next_state, done):
-        """Saves experience to memory.
-
-        :param state: Environment observation
-        :type state: float or List[float]
-        :param action: Action in environment
-        :type action: float or List[float]
-        :param reward: Reward from environment
-        :type reward: float
-        :param next_state: Environment observation of next state
-        :type next_state: float or List[float]
-        :param done: True if environment episode finished, else False
-        :type done: bool
-        """
-        self._add(state, action, reward, next_state, done)
-        self.counter += 1
-
-    def save2memoryVectEnvs(self, states, actions, rewards, next_states, dones):
-        """Saves multiple experiences to memory.
-
-        :param states: Multiple environment observations in a batch
-        :type states: List[float] or List[List[float]]
-        :param actions: Multiple actions in environment a batch
-        :type actions: List[float] or List[List[float]]
-        :param rewards: Multiple rewards from environment in a batch
-        :type rewards: List[float]
-        :param next_states: Multiple environment observations of next states in a batch
-        :type next_states: List[float] or List[List[float]]
-        :param dones: True if environment episodes finished, else False, in a batch
-        :type dones: List[bool]
-        """
-        for state, action, reward, next_state, done in zip(
-                states, actions, rewards, next_states, dones):
-            self._add(state, action, reward, next_state, done)
-            self.counter += 1
+import random
+from collections import deque, namedtuple
+
+import numpy as np
+import torch
+
+
+class ReplayBuffer:
+    """The Experience Replay Buffer class. Used to store experiences and allow
+    off-policy learning.
+
+    :param n_actions: Action dimension
+    :type n_actions: int
+    :param memory_size: Maximum length of replay buffer
+    :type memory_size: int
+    :param field_names: Field names for experience named tuple, e.g. ['state', 'action', 'reward']
+    :type field_names: List[str]
+    :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to None
+    :type device: str, optional
+    """
+
+    def __init__(self, action_dim, memory_size, field_names, device=None):
+        self.n_actions = action_dim
+        self.memory = deque(maxlen=memory_size)
+        self.experience = namedtuple("Experience", field_names=field_names)
+        self.counter = 0  # update cycle counter
+        self.device = device
+
+    def __len__(self):
+        return len(self.memory)
+
+    def _add(self, state, action, reward, next_state, done):
+        e = self.experience(state, action, reward, next_state, done)
+        self.memory.append(e)
+
+    def sample(self, batch_size):
+        """Returns sample of experiences from memory.
+
+        :param batch_size: Number of samples to return
+        :type batch_size: int
+        """
+        experiences = random.sample(self.memory, k=batch_size)
+
+        states = torch.from_numpy(
+            np.stack([e.state for e in experiences if e is not None], axis=0)
+        )
+        actions = torch.from_numpy(
+            np.vstack([e.action for e in experiences if e is not None])
+        )
+        rewards = torch.from_numpy(
+            np.vstack([e.reward for e in experiences if e is not None])
+        ).float()
+        next_states = torch.from_numpy(
+            np.stack([e.next_state for e in experiences if e is not None], axis=0)
+        ).float()
+        dones = torch.from_numpy(
+            np.vstack([e.done for e in experiences if e is not None]).astype(np.uint8)
+        ).float()
+
+        if self.device is not None:
+            states, actions, rewards, next_states, dones = (
+                states.to(self.device),
+                actions.to(self.device),
+                rewards.to(self.device),
+                next_states.to(self.device),
+                dones.to(self.device),
+            )
+
+        return (states, actions, rewards, next_states, dones)
+
+    def save2memory(self, state, action, reward, next_state, done):
+        """Saves experience to memory.
+
+        :param state: Environment observation
+        :type state: float or List[float]
+        :param action: Action in environment
+        :type action: float or List[float]
+        :param reward: Reward from environment
+        :type reward: float
+        :param next_state: Environment observation of next state
+        :type next_state: float or List[float]
+        :param done: True if environment episode finished, else False
+        :type done: bool
+        """
+        self._add(state, action, reward, next_state, done)
+        self.counter += 1
+
+    def save2memoryVectEnvs(self, states, actions, rewards, next_states, dones):
+        """Saves multiple experiences to memory.
+
+        :param states: Multiple environment observations in a batch
+        :type states: List[float] or List[List[float]]
+        :param actions: Multiple actions in environment a batch
+        :type actions: List[float] or List[List[float]]
+        :param rewards: Multiple rewards from environment in a batch
+        :type rewards: List[float]
+        :param next_states: Multiple environment observations of next states in a batch
+        :type next_states: List[float] or List[List[float]]
+        :param dones: True if environment episodes finished, else False, in a batch
+        :type dones: List[bool]
+        """
+        for state, action, reward, next_state, done in zip(
+            states, actions, rewards, next_states, dones
+        ):
+            self._add(state, action, reward, next_state, done)
+            self.counter += 1
```

### Comparing `agilerl-0.1.8/agilerl/components/replay_data.py` & `agilerl-0.1.9/agilerl/components/replay_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from torch.utils.data import IterableDataset
 
+
 class ReplayDataset(IterableDataset):
     """
-    Iterable Dataset containing the ReplayBuffer which will be updated with new 
+    Iterable Dataset containing the ReplayBuffer which will be updated with new
     experiences during training
 
     :param buffer: Experience replay buffer
     :type buffer: agilerl.components.replay_buffer.ReplayBuffer()
     :param batch_size: Number of experiences to sample at a time, defaults to 256
     :type batch_size: int, optional
     """
+
     def __init__(self, buffer, batch_size=256):
         self.buffer = buffer
         self.batch_size = batch_size
 
     def __iter__(self):
         yield self.buffer.sample(self.batch_size)
```

### Comparing `agilerl-0.1.8/agilerl/data/language_environment.py` & `agilerl-0.1.9/agilerl/data/language_environment.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
+
 from abc import ABC, abstractmethod
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any
+
 from agilerl.utils.cache import Cache
 
 
 class Language_Observation(ABC):
     @abstractmethod
-    def to_sequence(self) -> Tuple[List[str, Optional[float]], bool]:
+    def to_sequence(self) -> tuple[list[str, float | None], bool]:
         # returns a List of Tuples and a bool indicating terminal
         # each state Tuple should be: (str, None)
         # each action Tuple should be: (str, reward)
         pass
 
     @abstractmethod
     def __str__(self) -> str:
         pass
 
-    def metadata(self) -> Optional[Dict[str, Any]]:
+    def metadata(self) -> dict[str, Any] | None:
         return None
 
 
 class Language_Environment(ABC):
     @abstractmethod
-    def step(self, action: str) -> Tuple[Language_Observation, float, bool]:
+    def step(self, action: str) -> tuple[Language_Observation, float, bool]:
         pass
 
     @abstractmethod
     def reset(self) -> Language_Observation:
         pass
 
     @abstractmethod
@@ -46,16 +48,19 @@
     def train(self):
         pass
 
     def eval(self):
         pass
 
 
-def interact_environment(env: Language_Environment, policy: Policy,
-                         obs: Optional[Language_Observation] = None):
+def interact_environment(
+    env: Language_Environment,
+    policy: Policy,
+    obs: Language_Observation | None = None,
+):
     obs_sequence = []
     if obs is None:
         obs = env.reset()
     while not env.is_terminal():
         action = policy.act(obs)
         new_obs, r, t = env.step(action)
         obs_sequence.append((obs, action, r, t))
```

### Comparing `agilerl-0.1.8/agilerl/data/rl_data.py` & `agilerl-0.1.9/agilerl/data/rl_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional
+
 import torch
+
 from agilerl.data.language_environment import Language_Observation
 from agilerl.data.tokenizer import Tokenizer
 
 
 class TokenReward(ABC):
     @abstractmethod
     def get_token_reward(self, tokens: List[int]) -> List[float]:
@@ -17,26 +19,28 @@
         self.c = c
 
     def get_token_reward(self, tokens: List[int]) -> List[float]:
         return [self.c] * (len(tokens) - 1)
 
 
 class SepcifiedTokenReward(TokenReward):
-    def __init__(self, token_data: Dict[int, float],
-                 scale: float = 1.0, shift: float = 0.0):
+    def __init__(
+        self, token_data: Dict[int, float], scale: float = 1.0, shift: float = 0.0
+    ):
         self.token_data = token_data
         self.scale = scale
         self.shift = shift
 
     def get_token_reward(self, tokens: List[int]) -> List[float]:
-        return [(self.token_data[tok] *
-                 self.scale +
-                 self.shift) if tok in self.token_data else (0.0 *
-                                                             self.scale +
-                                                             self.shift) for tok in tokens[1:]]
+        return [
+            (self.token_data[tok] * self.scale + self.shift)
+            if tok in self.token_data
+            else (0.0 * self.scale + self.shift)
+            for tok in tokens[1:]
+        ]
 
 
 @dataclass
 class DataPoint:
     raw_str: str
     tokens: List[int]
     state_idxs: List[int]
@@ -57,28 +61,34 @@
         term = torch.tensor(self.terminals).to(device)
         u_s = torch.tensor(self.utterance_state_idxs).long().to(device)
         u_a = torch.tensor(self.utterance_action_idxs).long().to(device)
         u_r = torch.tensor(self.utterance_rewards).long().to(device)
         u_term = torch.tensor(self.utterance_terminals).long().to(device)
         if max_length is not None:
             tok = tok[:max_length]
-            s = s[:(s < max_length).sum()]
-            a = a[:max(min((a < (max_length - 1)).sum().item(), s.shape[0] - 1), 0)]
-            r = r[:a.shape[0]]
-            term = term[:s.shape[0]]
-            u_s = u_s[:(s < max_length).sum()]
-            u_a = u_a[:max(
-                min((u_a < (max_length - 1)).sum().item(), u_s.shape[0] - 1), 0)]
-            u_r = u_r[:u_a.shape[0]]
-            u_term = u_term[:u_s.shape[0]]
+            s = s[: (s < max_length).sum()]
+            a = a[: max(min((a < (max_length - 1)).sum().item(), s.shape[0] - 1), 0)]
+            r = r[: a.shape[0]]
+            term = term[: s.shape[0]]
+            u_s = u_s[: (s < max_length).sum()]
+            u_a = u_a[
+                : max(min((u_a < (max_length - 1)).sum().item(), u_s.shape[0] - 1), 0)
+            ]
+            u_r = u_r[: u_a.shape[0]]
+            u_term = u_term[: u_s.shape[0]]
         return tok, s, a, r, term, u_s, u_a, u_r, u_term
 
     @classmethod
-    def from_obs(cls, obs: Language_Observation, tokenizer: Tokenizer,
-                 token_reward: TokenReward, meta: Optional[Dict[str, Any]] = None):
+    def from_obs(
+        cls,
+        obs: Language_Observation,
+        tokenizer: Tokenizer,
+        token_reward: TokenReward,
+        meta: Optional[Dict[str, Any]] = None,
+    ):
         sequence, terminal = obs.to_sequence()
         obs_meta = obs.metadata()
         if meta is not None and obs_meta is not None:
             meta = {**obs_meta, **meta}
         elif obs_meta is not None:
             meta = obs_meta
         if len(sequence) == 0 or sequence[0][1] is not None:
@@ -112,69 +122,105 @@
                 action_idxs.extend(list(range(curr_idx, i)))
                 state_idxs.extend(list(range(curr_idx, i)))
                 reward.extend([token_rewards[x] for x in range(curr_idx, i)])
                 reward[-1] += action_rewards[curr_action_idx]
                 utterance_action_idxs.append(i)
                 utterance_state_idxs.append(curr_idx)
                 utterance_rewards.append(
-                    action_rewards[curr_action_idx] + sum([token_rewards[x] for x in range(curr_idx, i)]))
+                    action_rewards[curr_action_idx]
+                    + sum([token_rewards[x] for x in range(curr_idx, i)])
+                )
                 curr_idx = i
                 curr_action_idx += 1
         state_idxs.append(len(tokens) - 1)
         utterance_state_idxs.append(len(tokens) - 1)
         terminals = ([0] * (len(state_idxs) - 1)) + [int(terminal)]
-        utterance_terminals = (
-            [0] * (len(utterance_state_idxs) - 1)) + [int(terminal)]
-        return cls(raw_str, tokens, state_idxs, action_idxs, reward, terminals,
-                   utterance_state_idxs, utterance_action_idxs,
-                   utterance_rewards, utterance_terminals, meta=meta)
+        utterance_terminals = ([0] * (len(utterance_state_idxs) - 1)) + [int(terminal)]
+        return cls(
+            raw_str,
+            tokens,
+            state_idxs,
+            action_idxs,
+            reward,
+            terminals,
+            utterance_state_idxs,
+            utterance_action_idxs,
+            utterance_rewards,
+            utterance_terminals,
+            meta=meta,
+        )
 
     @staticmethod
-    def get_token_reward(obs: Language_Observation,
-                         tokenizer: Tokenizer, token_reward: TokenReward):
+    def get_token_reward(
+        obs: Language_Observation, tokenizer: Tokenizer, token_reward: TokenReward
+    ):
         return DataPoint.from_obs(obs, tokenizer, token_reward).rewards
 
 
 class RL_Dataset(ABC):
-    def __init__(self,
-                 tokenizer: Tokenizer,
-                 token_reward: TokenReward,
-                 max_len: Optional[int]) -> None:
+    def __init__(
+        self, tokenizer: Tokenizer, token_reward: TokenReward, max_len: Optional[int]
+    ) -> None:
         super().__init__()
         self.tokenizer = tokenizer
         self.token_reward = token_reward
         self.max_len = max_len
 
     def collate(self, items: List[DataPoint], device):
-        tokens, state_idxs, action_idxs, rewards, terminals, u_state_idxs, u_action_idxs, u_rewards, u_terminals = zip(
-            *map(lambda x: x.to_tensors(device, self.max_len), items))
+        (
+            tokens,
+            state_idxs,
+            action_idxs,
+            rewards,
+            terminals,
+            u_state_idxs,
+            u_action_idxs,
+            u_rewards,
+            u_terminals,
+        ) = zip(*map(lambda x: x.to_tensors(device, self.max_len), items))
         tokens = torch.nn.utils.rnn.pad_sequence(
-            tokens, batch_first=True, padding_value=self.tokenizer.pad_token_id)
+            tokens, batch_first=True, padding_value=self.tokenizer.pad_token_id
+        )
         attn_mask = (tokens != self.tokenizer.pad_token_id).float()
         state_idxs = torch.nn.utils.rnn.pad_sequence(
-            state_idxs, batch_first=True, padding_value=0)
+            state_idxs, batch_first=True, padding_value=0
+        )
         action_idxs = torch.nn.utils.rnn.pad_sequence(
-            action_idxs, batch_first=True, padding_value=0)
+            action_idxs, batch_first=True, padding_value=0
+        )
         terminals = torch.nn.utils.rnn.pad_sequence(
-            terminals, batch_first=True, padding_value=1)
+            terminals, batch_first=True, padding_value=1
+        )
         rewards = torch.nn.utils.rnn.pad_sequence(
-            rewards, batch_first=True, padding_value=0.0)
+            rewards, batch_first=True, padding_value=0.0
+        )
         u_state_idxs = torch.nn.utils.rnn.pad_sequence(
-            u_state_idxs, batch_first=True, padding_value=0)
+            u_state_idxs, batch_first=True, padding_value=0
+        )
         u_action_idxs = torch.nn.utils.rnn.pad_sequence(
-            u_action_idxs, batch_first=True, padding_value=0)
+            u_action_idxs, batch_first=True, padding_value=0
+        )
         u_terminals = torch.nn.utils.rnn.pad_sequence(
-            u_terminals, batch_first=True, padding_value=1)
+            u_terminals, batch_first=True, padding_value=1
+        )
         u_rewards = torch.nn.utils.rnn.pad_sequence(
-            u_rewards, batch_first=True, padding_value=0.0)
-        return {'tokens': tokens, 'attn_mask': attn_mask,
-                'state_idxs': state_idxs, 'action_idxs': action_idxs,
-                'rewards': rewards, 'terminals': terminals,
-                'u_state_idxs': u_state_idxs, 'u_action_idxs': u_action_idxs,
-                'u_rewards': u_rewards, 'u_terminals': u_terminals}
+            u_rewards, batch_first=True, padding_value=0.0
+        )
+        return {
+            "tokens": tokens,
+            "attn_mask": attn_mask,
+            "state_idxs": state_idxs,
+            "action_idxs": action_idxs,
+            "rewards": rewards,
+            "terminals": terminals,
+            "u_state_idxs": u_state_idxs,
+            "u_action_idxs": u_action_idxs,
+            "u_rewards": u_rewards,
+            "u_terminals": u_terminals,
+        }
 
 
 class List_RL_Dataset(RL_Dataset):
     @abstractmethod
     def get_item(self, idx: int) -> DataPoint:
         pass
```

### Comparing `agilerl-0.1.8/agilerl/data/torch_datasets.py` & `agilerl-0.1.9/agilerl/data/torch_datasets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-import torch
-from torch.utils.data import IterableDataset, Dataset
-from agilerl.data.rl_data import List_RL_Dataset, Iterable_RL_Dataset
 from typing import Union
 
+import torch
+from torch.utils.data import Dataset, IterableDataset
+
+from agilerl.data.rl_data import Iterable_RL_Dataset, List_RL_Dataset
+
 
 class GeneralIterDataset(IterableDataset):
-    def __init__(self, rl_dataset: Iterable_RL_Dataset,
-                 device: Union[torch.device, str]):
+    def __init__(
+        self, rl_dataset: Iterable_RL_Dataset, device: Union[torch.device, str]
+    ):
         self.rl_dataset = rl_dataset
         self.device = device
 
     def __iter__(self):
         return self
 
     def __next__(self):
@@ -20,16 +23,15 @@
         return self.rl_dataset.collate(items, self.device)
 
     def collate_simple(self, items):
         return items
 
 
 class GeneralDataset(Dataset):
-    def __init__(self, rl_dataset: List_RL_Dataset,
-                 device: Union[torch.device, str]):
+    def __init__(self, rl_dataset: List_RL_Dataset, device: Union[torch.device, str]):
         self.rl_dataset = rl_dataset
         self.device = device
 
     def __len__(self):
         return self.rl_dataset.size()
 
     def __getitem__(self, i):
```

### Comparing `agilerl-0.1.8/agilerl/hpo/tournament.py` & `agilerl-0.1.9/agilerl/hpo/tournament.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,59 @@
-import numpy as np
-import copy
-
-
-class TournamentSelection():
-    """The tournament selection class.
-
-    :param tournament_size: Tournament selection size
-    :type tournament_size: int
-    :param elitism: Elitism in tournament selection
-    :type elitism: bool
-    :param population_size: Number of agents in population
-    :type population_size: int
-    :param evo_step: Number of most recent fitness scores to use in evaluation
-    :type evo_step: int
-    """
-
-    def __init__(self, tournament_size, elitism, population_size, evo_step):
-        self.tournament_size = tournament_size
-        self.elitism = elitism
-        self.population_size = population_size
-        self.evo_step = evo_step
-
-    def _tournament(self, fitness_values):
-        selection = np.random.randint(
-            0, len(fitness_values), size=self.tournament_size)
-        selection_values = [fitness_values[i] for i in selection]
-        winner = selection[np.argmax(selection_values)]
-        return winner
-
-    def select(self, population):
-        """Returns best agent and new population of agents following tournament selection.
-
-        :param population: Population of agents
-        :type population: List[object]
-        """
-        last_fitness = [np.mean(indi.fitness[-self.evo_step:])
-                        for indi in population]
-        rank = np.argsort(last_fitness).argsort()
-
-        max_id = max([ind.index for ind in population])
-
-        model = population[np.argsort(rank)[-1]]
-        elite = copy.deepcopy(model)
-
-        new_population = []
-        if self.elitism:  # keep top agent in population
-            new_population.append(elite.clone(wrap=False))
-            selection_size = self.population_size - 1
-        else:
-            selection_size = self.population_size
-
-        # select parents of next gen using tournament selection
-        for idx in range(selection_size):
-            max_id += 1
-            actor_parent = population[self._tournament(rank)]
-            new_individual = actor_parent.clone(max_id, wrap=False)
-            new_population.append(new_individual)
-
-        return elite, new_population
+import copy
+
+import numpy as np
+
+
+class TournamentSelection:
+    """The tournament selection class.
+
+    :param tournament_size: Tournament selection size
+    :type tournament_size: int
+    :param elitism: Elitism in tournament selection
+    :type elitism: bool
+    :param population_size: Number of agents in population
+    :type population_size: int
+    :param evo_step: Number of most recent fitness scores to use in evaluation
+    :type evo_step: int
+    """
+
+    def __init__(self, tournament_size, elitism, population_size, evo_step):
+        self.tournament_size = tournament_size
+        self.elitism = elitism
+        self.population_size = population_size
+        self.evo_step = evo_step
+
+    def _tournament(self, fitness_values):
+        selection = np.random.randint(0, len(fitness_values), size=self.tournament_size)
+        selection_values = [fitness_values[i] for i in selection]
+        winner = selection[np.argmax(selection_values)]
+        return winner
+
+    def select(self, population):
+        """Returns best agent and new population of agents following tournament selection.
+
+        :param population: Population of agents
+        :type population: List[object]
+        """
+        last_fitness = [np.mean(indi.fitness[-self.evo_step :]) for indi in population]
+        rank = np.argsort(last_fitness).argsort()
+
+        max_id = max([ind.index for ind in population])
+
+        model = population[np.argsort(rank)[-1]]
+        elite = copy.deepcopy(model)
+
+        new_population = []
+        if self.elitism:  # keep top agent in population
+            new_population.append(elite.clone(wrap=False))
+            selection_size = self.population_size - 1
+        else:
+            selection_size = self.population_size
+
+        # select parents of next gen using tournament selection
+        for idx in range(selection_size):
+            max_id += 1
+            actor_parent = population[self._tournament(rank)]
+            new_individual = actor_parent.clone(max_id, wrap=False)
+            new_population.append(new_individual)
+
+        return elite, new_population
```

### Comparing `agilerl-0.1.8/agilerl/networks/custom_architecture.py` & `agilerl-0.1.9/agilerl/networks/custom_architecture.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import torch
-import torch.nn.functional as F
 import torch.nn as nn
+import torch.nn.functional as F
+
 
 class GumbelSoftmax(nn.Module):
-    """Applies gumbel softmax function element-wise
-    """
+    """Applies gumbel softmax function element-wise"""
+
     @staticmethod
     def gumbel_softmax(logits, tau=1.0, eps=1e-20):
         """Implementation of the gumbel softmax activation function
-        
+
         :param logits: Tensor containing unnormalized log probabilities for each class.
         :type logits: torch.Tensor
         :param tau: Tau, defaults to 1.0
         :type tau: float, optional
         :param eps: Epsilon, defaults to 1e-20
         :type eps: float, optional
         """
         epsilon = torch.rand_like(logits)
         logits += -torch.log(-torch.log(epsilon + eps) + eps)
         return F.softmax(logits / tau, dim=-1)
 
     def forward(self, input: torch.Tensor) -> torch.Tensor:
-        return self.gumbel_softmax(input)
+        return self.gumbel_softmax(input)
```

### Comparing `agilerl-0.1.8/agilerl/networks/evolvable_bert.py` & `agilerl-0.1.9/agilerl/networks/evolvable_bert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import copy
+import math
+import warnings
 from collections import OrderedDict
 from typing import List
 
 import numpy as np
 import torch
 import torch.nn as nn
-import math
-import warnings
 
 
 class EvolvableBERT(nn.Module):
     """The Evolvable BERT class.
 
     :param encoder_layers: Encoder layer(s) hidden size
     :type encoder_layers: List[int]
@@ -47,34 +47,35 @@
     :param stored_values: Stored network weights, defaults to None
     :type stored_values: numpy.array(), optional
     :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
     :type device: str, optional
     """
 
     def __init__(
-            self,
-            encoder_layers: List[int],
-            decoder_layers: List[int],
-            end2end: bool = True,
-            src_vocab_size: int = 10837,
-            tgt_vocab_size: int = 10837,
-            encoder_norm: bool = True,
-            decoder_norm: bool = True,
-            d_model: int = 512,
-            n_head: int = 8,
-            dropout: float = 0.1,
-            activation: str = 'relu',
-            layer_norm_eps: float = 1e-5,
-            batch_first: bool = False,
-            norm_first: bool = False,
-            max_encoder_layers: int = 12,
-            max_decoder_layers: int = 12,
-            stored_values=None,
-            device='cpu'):
-        super(EvolvableBERT, self).__init__()
+        self,
+        encoder_layers: List[int],
+        decoder_layers: List[int],
+        end2end: bool = True,
+        src_vocab_size: int = 10837,
+        tgt_vocab_size: int = 10837,
+        encoder_norm: bool = True,
+        decoder_norm: bool = True,
+        d_model: int = 512,
+        n_head: int = 8,
+        dropout: float = 0.1,
+        activation: str = "relu",
+        layer_norm_eps: float = 1e-5,
+        batch_first: bool = False,
+        norm_first: bool = False,
+        max_encoder_layers: int = 12,
+        max_decoder_layers: int = 12,
+        stored_values=None,
+        device="cpu",
+    ):
+        super().__init__()
 
         self.encoder_layers = encoder_layers
         self.decoder_layers = decoder_layers
         self.end2end = end2end
         self.src_vocab_size = src_vocab_size
         self.tgt_vocab_size = tgt_vocab_size
         self.encoder_norm = encoder_norm
@@ -91,107 +92,115 @@
 
         self.device = device
 
         if self.end2end:
             self.generator = nn.Linear(self.d_model, tgt_vocab_size)
             self.src_tok_emb = TokenEmbedding(src_vocab_size, self.d_model)
             self.tgt_tok_emb = TokenEmbedding(tgt_vocab_size, self.d_model)
-            self.positional_encoding = PositionalEncoder(
-                self.d_model, self.dropout)
+            self.positional_encoding = PositionalEncoder(self.d_model, self.dropout)
         else:
             self.wte = TokenEmbedding(src_vocab_size, self.d_model)
             if len(self.encoder_layers) > 0:
-                self.wpe = PositionalEncoding(
-                    self.d_model, self.encoder_layers[0])
+                self.wpe = PositionalEncoding(self.d_model, self.encoder_layers[0])
             else:
-                self.wpe = PositionalEncoding(
-                    self.d_model, self.decoder_layers[0])
+                self.wpe = PositionalEncoding(self.d_model, self.decoder_layers[0])
 
         self.encoder, self.decoder = self.create_nets()
         self.encoder_keys = list(self.encoder.keys())
         self.decoder_keys = list(self.decoder.keys())
 
         if stored_values is not None:
-            self.inject_parameters(
-                pvec=stored_values, without_layer_norm=False)
+            self.inject_parameters(pvec=stored_values, without_layer_norm=False)
 
     def get_activation(self, activation_names):
         """Returns activation function for corresponding activation name.
 
         :param activation_names: Activation function name
         :type activation_names: str
         """
         activation_functions = {
-            'tanh': nn.Tanh,
-            'linear': nn.Identity,
-            'relu': nn.ReLU,
-            'elu': nn.ELU,
-            'softsign': nn.Softsign,
-            'sigmoid': nn.Sigmoid,
-            'softplus': nn.Softplus,
-            'lrelu': nn.LeakyReLU,
-            'prelu': nn.PReLU,
-            'gelu': nn.GELU}
+            "tanh": nn.Tanh,
+            "linear": nn.Identity,
+            "relu": nn.ReLU,
+            "elu": nn.ELU,
+            "softsign": nn.Softsign,
+            "sigmoid": nn.Sigmoid,
+            "softplus": nn.Softplus,
+            "lrelu": nn.LeakyReLU,
+            "prelu": nn.PReLU,
+            "gelu": nn.GELU,
+        }
 
         return activation_functions[activation_names]()
 
     def create_nets(self):
-        """Creates and returns transformer neural network.
-        """
+        """Creates and returns transformer neural network."""
         encoder_dict = OrderedDict()
         decoder_dict = OrderedDict()
 
         # Create the encoder
         for n, dim_feedfwd in enumerate(self.encoder_layers):
-            encoder_dict[f"encoder_layer_{str(n)}"] = nn.modules.TransformerEncoderLayer(
+            encoder_dict[
+                f"encoder_layer_{str(n)}"
+            ] = nn.modules.TransformerEncoderLayer(
                 self.d_model,
                 self.n_head,
                 dim_feedfwd,
                 self.dropout,
                 self.activation,
                 self.layer_norm_eps,
                 self.batch_first,
                 self.norm_first,
-                device=self.device)
+                device=self.device,
+            )
         if self.encoder_norm:
             encoder_dict["encoder_norm_0"] = nn.modules.normalization.LayerNorm(
-                self.d_model, eps=self.layer_norm_eps, device=self.device)
+                self.d_model, eps=self.layer_norm_eps, device=self.device
+            )
 
         # Create the decoder
         for n, dim_feedfwd in enumerate(self.decoder_layers):
-            decoder_dict[f"decoder_layer_{str(n)}"] = nn.modules.TransformerDecoderLayer(
+            decoder_dict[
+                f"decoder_layer_{str(n)}"
+            ] = nn.modules.TransformerDecoderLayer(
                 self.d_model,
                 self.n_head,
                 dim_feedfwd,
                 self.dropout,
                 self.activation,
                 self.layer_norm_eps,
                 self.batch_first,
                 self.norm_first,
-                device=self.device)
+                device=self.device,
+            )
         if self.decoder_norm:
             decoder_dict["decoder_norm_0"] = nn.modules.normalization.LayerNorm(
-                self.d_model, eps=self.layer_norm_eps, device=self.device)
+                self.d_model, eps=self.layer_norm_eps, device=self.device
+            )
 
         self._reset_parameters()
 
         return nn.ModuleDict(encoder_dict), nn.ModuleDict(decoder_dict)
 
     def generate_square_subsequent_mask(self, sz):
-        """Returns a square mask for the sequence that prevents the model from looking into the future words when 
+        """Returns a square mask for the sequence that prevents the model from looking into the future words when
         making predictions.
         The masked positions are filled with float('-inf'). Unmasked positions are filled with float(0.0).
 
         :param sz: Size of mask to generate
         :type sz: int
         """
-        mask = (torch.triu(torch.ones((sz, sz), device=self.device))
-                == 1).transpose(0, 1)
-        mask = mask.float().masked_fill(mask == 0, float(
-            '-inf')).masked_fill(mask == 1, float(0.0))
+        mask = (torch.triu(torch.ones((sz, sz), device=self.device)) == 1).transpose(
+            0, 1
+        )
+        mask = (
+            mask.float()
+            .masked_fill(mask == 0, float("-inf"))
+            .masked_fill(mask == 1, float(0.0))
+        )
         return mask
 
     def create_mask(self, src, tgt, pad_idx):
         """Returns masks to hide source and target padding tokens.
 
         :param src: Source
         :type src: torch.Tensor
@@ -200,40 +209,45 @@
         :param pad_idx: Index of padding symbol <pad> in special symbols list
         :type pad_idx: int
         """
         src_seq_len = src.shape[0]
         tgt_seq_len = tgt.shape[0]
 
         tgt_mask = self.generate_square_subsequent_mask(tgt_seq_len)
-        src_mask = torch.zeros((src_seq_len, src_seq_len),
-                               device=self.device).type(torch.bool)
+        src_mask = torch.zeros((src_seq_len, src_seq_len), device=self.device).type(
+            torch.bool
+        )
 
         src_padding_mask = (src == pad_idx).transpose(0, 1)
         tgt_padding_mask = (tgt == pad_idx).transpose(0, 1)
-        return src_mask.to(self.device), tgt_mask.to(self.device), src_padding_mask.to(
-            self.device), tgt_padding_mask.to(self.device)
+        return (
+            src_mask.to(self.device),
+            tgt_mask.to(self.device),
+            src_padding_mask.to(self.device),
+            tgt_padding_mask.to(self.device),
+        )
 
     def _reset_parameters(self):
-        """Initiate parameters in the transformer model.
-        """
+        """Initiate parameters in the transformer model."""
         for p in self.parameters():
             if p.dim() > 1:
                 nn.init.xavier_uniform_(p)
 
     def forward(
-            self,
-            src,
-            tgt,
-            src_mask=None,
-            tgt_mask=None,
-            memory_mask=None,
-            src_key_padding_mask=None,
-            tgt_key_padding_mask=None,
-            memory_key_padding_mask=None,
-            is_causal=False):
+        self,
+        src,
+        tgt,
+        src_mask=None,
+        tgt_mask=None,
+        memory_mask=None,
+        src_key_padding_mask=None,
+        tgt_key_padding_mask=None,
+        memory_key_padding_mask=None,
+        is_causal=False,
+    ):
         """Returns output of neural network.
 
         :param src: Encoder input sequence
         :type src: torch.Tensor
         :param tgt: Decoder input sequence
         :type tgt: torch.Tensor
         :param src_mask: Additive mask for the src sequence, defaults to None
@@ -248,18 +262,25 @@
         :type tgt_key_padding_mask: torch.Tensor, optional
         :param memory_key_padding_mask: Tensor mask for memory keys per batch, defaults to None
         :type memory_key_padding_mask: torch.Tensor, optional
         :param is_causal: Applies a causal mask as mask and ignores attn_mask for computing scaled dot product attention, defaults to False
         :type is_causal: bool, optional
         """
         encoder_output, encoder_hidden_states = self.encode(
-            src, src_mask, src_key_padding_mask, is_causal)
+            src, src_mask, src_key_padding_mask, is_causal
+        )
         memory = encoder_output
         decoder_output, decoder_hidden_states = self.decode(
-            tgt, memory, tgt_mask, memory_mask, tgt_key_padding_mask, memory_key_padding_mask)
+            tgt,
+            memory,
+            tgt_mask,
+            memory_mask,
+            tgt_key_padding_mask,
+            memory_key_padding_mask,
+        )
 
         if self.end2end:
             decoder_output = self.generator(decoder_output)
 
         return decoder_output
 
     def encode(self, src, src_mask=None, src_key_padding_mask=None, is_causal=False):
@@ -279,64 +300,78 @@
 
         # Encoder forward pass preparation
         src_key_padding_mask = _canonical_mask(
             mask=src_key_padding_mask,
             mask_name="src_key_padding_mask",
             other_type=_none_or_dtype(src_mask),
             other_name="mask",
-            target_type=src.dtype
+            target_type=src.dtype,
         )
         encoder_output = src
         first_layer = self.encoder[self.encoder_keys[0]]
         str_first_layer = "self.net[0]"
         src_key_padding_mask_for_layers = src_key_padding_mask
-        encoder_output, convert_to_nested, src_key_padding_mask_for_layers = self.check_encoder_sparsity_fast_path(
-            src, encoder_output, first_layer, str_first_layer, 
-            src_mask, src_key_padding_mask, src_key_padding_mask_for_layers)
+        (
+            encoder_output,
+            convert_to_nested,
+            src_key_padding_mask_for_layers,
+        ) = self.check_encoder_sparsity_fast_path(
+            src,
+            encoder_output,
+            first_layer,
+            str_first_layer,
+            src_mask,
+            src_key_padding_mask,
+            src_key_padding_mask_for_layers,
+        )
 
         # Prevent type refinement
-        make_causal = (is_causal is True)
+        make_causal = is_causal is True
 
         if is_causal is None:
             if src_mask is not None:
                 sz = src_mask.size(0)
                 causal_comparison = torch.triu(
-                    torch.ones(
-                        sz,
-                        sz,
-                        device=src_mask.device) *
-                    float('-inf'),
-                    diagonal=1).to(
-                    src_mask.dtype)
+                    torch.ones(sz, sz, device=src_mask.device) * float("-inf"),
+                    diagonal=1,
+                ).to(src_mask.dtype)
                 if torch.equal(src_mask, causal_comparison):
                     make_causal = True
         is_causal = make_causal
 
         all_hidden_states = ()
 
         # Encoder forward pass
         for key in self.encoder_keys:
-            if 'norm' not in key:
+            if "norm" not in key:
                 all_hidden_states = all_hidden_states + (encoder_output,)
                 encoder_output = self.encoder[key](
                     encoder_output,
                     src_mask=src_mask,
                     is_causal=is_causal,
-                    src_key_padding_mask=src_key_padding_mask_for_layers)
+                    src_key_padding_mask=src_key_padding_mask_for_layers,
+                )
         all_hidden_states = all_hidden_states + (encoder_output,)
         if convert_to_nested:
-            encoder_output = encoder_output.to_padded_tensor(0.)
+            encoder_output = encoder_output.to_padded_tensor(0.0)
             all_hidden_states = all_hidden_states + (encoder_output,)
-        if ['encoder_norm_0'] in self.encoder_keys:
-            encoder_output = self.encoder['encoder_norm_0'](encoder_output)
+        if ["encoder_norm_0"] in self.encoder_keys:
+            encoder_output = self.encoder["encoder_norm_0"](encoder_output)
             all_hidden_states = all_hidden_states + (encoder_output,)
         return encoder_output, all_hidden_states
 
-    def decode(self, tgt, memory, tgt_mask=None, memory_mask=None,
-               tgt_key_padding_mask=None, memory_key_padding_mask=None):
+    def decode(
+        self,
+        tgt,
+        memory,
+        tgt_mask=None,
+        memory_mask=None,
+        tgt_key_padding_mask=None,
+        memory_key_padding_mask=None,
+    ):
         """Returns decoded transformer input.
 
         :param tgt: Decoder input sequence
         :type tgt: torch.Tensor
         :param memory: Encoder output sequence
         :type memory: torch.Tensory
         :param tgt_mask: Additive mask for the tgt sequence, defaults to None
@@ -352,38 +387,40 @@
             tgt = self.positional_encoding(self.src_tok_emb(tgt))
 
         all_hidden_states = ()
 
         # Decoder forward pass
         decoder_output = tgt
         for key in self.decoder_keys:
-            if 'norm' not in key:
+            if "norm" not in key:
                 all_hidden_states = all_hidden_states + (decoder_output,)
                 decoder_output = self.decoder[key](
                     decoder_output,
                     memory,
                     tgt_mask=tgt_mask,
                     memory_mask=memory_mask,
                     tgt_key_padding_mask=tgt_key_padding_mask,
-                    memory_key_padding_mask=memory_key_padding_mask)
+                    memory_key_padding_mask=memory_key_padding_mask,
+                )
         all_hidden_states = all_hidden_states + (decoder_output,)
-        if ['decoder_norm_0'] in self.decoder_keys:
-            decoder_output = self.decoder['decoder_norm_0'](decoder_output)
+        if ["decoder_norm_0"] in self.decoder_keys:
+            decoder_output = self.decoder["decoder_norm_0"](decoder_output)
             all_hidden_states = all_hidden_states + (decoder_output,)
         return decoder_output, all_hidden_states
 
     def check_encoder_sparsity_fast_path(
-            self,
-            src,
-            output,
-            first_layer,
-            str_first_layer,
-            mask,
-            src_key_padding_mask,
-            src_key_padding_mask_for_layers):
+        self,
+        src,
+        output,
+        first_layer,
+        str_first_layer,
+        mask,
+        src_key_padding_mask,
+        src_key_padding_mask_for_layers,
+    ):
         """Returns encoder output, conversion to nested and padding mask depending on if sparsity fast path possible.
         :param src: Encoder input sequence
         :type src: torch.Tensor
         :param output: Encoder output sequence
         :type output: torch.Tensor
         :param first_layer: First layer of encoder
         :type first_layer: torch.Module()
@@ -392,43 +429,58 @@
         :param mask: Mask for the src sequence
         :type mask: torch.Tensor
         :param src_key_padding_mask: Tensor mask for src keys per batch
         :type src_key_padding_mask: torch.Tensor
         :param src_key_padding_mask_for_layers: Tensor mask for src keys per batch for layers
         :type src_key_padding_mask_for_layers: torch.Tensor
         """
-        why_not_sparsity_fast_path = ''
+        why_not_sparsity_fast_path = ""
         convert_to_nested = False
         if not isinstance(first_layer, torch.nn.TransformerEncoderLayer):
-            why_not_sparsity_fast_path = f"{str_first_layer} was not TransformerEncoderLayer"
+            why_not_sparsity_fast_path = (
+                f"{str_first_layer} was not TransformerEncoderLayer"
+            )
         elif first_layer.norm_first:
             why_not_sparsity_fast_path = f"{str_first_layer}.norm_first was True"
         elif first_layer.training:
             why_not_sparsity_fast_path = f"{str_first_layer} was in training mode"
         elif not first_layer.self_attn.batch_first:
-            why_not_sparsity_fast_path = f" {str_first_layer}.self_attn.batch_first was not True"
+            why_not_sparsity_fast_path = (
+                f" {str_first_layer}.self_attn.batch_first was not True"
+            )
         elif not first_layer.self_attn._qkv_same_embed_dim:
-            why_not_sparsity_fast_path = f"{str_first_layer}.self_attn._qkv_same_embed_dim was not True"
+            why_not_sparsity_fast_path = (
+                f"{str_first_layer}.self_attn._qkv_same_embed_dim was not True"
+            )
         elif not first_layer.activation_relu_or_gelu:
-            why_not_sparsity_fast_path = f" {str_first_layer}.activation_relu_or_gelu was not True"
+            why_not_sparsity_fast_path = (
+                f" {str_first_layer}.activation_relu_or_gelu was not True"
+            )
         elif not (first_layer.norm1.eps == first_layer.norm2.eps):
             why_not_sparsity_fast_path = f"{str_first_layer}.norm1.eps was not equal to {str_first_layer}.norm2.eps"
         elif not src.dim() == 3:
-            why_not_sparsity_fast_path = f"input not batched; expected src.dim() of 3 but got {src.dim()}"
+            why_not_sparsity_fast_path = (
+                f"input not batched; expected src.dim() of 3 but got {src.dim()}"
+            )
         elif not self.enable_nested_tensor:
             why_not_sparsity_fast_path = "enable_nested_tensor was not True"
         elif src_key_padding_mask is None:
             why_not_sparsity_fast_path = "src_key_padding_mask was None"
-        elif (((not hasattr(self, "mask_check")) or self.mask_check)
-                and not torch._nested_tensor_from_mask_left_aligned(src, src_key_padding_mask.logical_not())):
+        elif (
+            (not hasattr(self, "mask_check")) or self.mask_check
+        ) and not torch._nested_tensor_from_mask_left_aligned(
+            src, src_key_padding_mask.logical_not()
+        ):
             why_not_sparsity_fast_path = "mask_check enabled, and src and src_key_padding_mask was not left aligned"
         elif output.is_nested:
             why_not_sparsity_fast_path = "NestedTensor input is not supported"
         elif mask is not None:
-            why_not_sparsity_fast_path = "src_key_padding_mask and mask were both supplied"
+            why_not_sparsity_fast_path = (
+                "src_key_padding_mask and mask were both supplied"
+            )
         elif first_layer.self_attn.num_heads % 2 == 1:
             why_not_sparsity_fast_path = "num_head is odd"
         elif torch.is_autocast_enabled():
             why_not_sparsity_fast_path = "autocast is enabled"
 
         if not why_not_sparsity_fast_path:
             tensor_args = (
@@ -443,104 +495,104 @@
                 first_layer.norm2.bias,
                 first_layer.linear1.weight,
                 first_layer.linear1.bias,
                 first_layer.linear2.weight,
                 first_layer.linear2.bias,
             )
 
-            if not (src.is_cuda or 'cpu' in str(src.device)):
+            if not (src.is_cuda or "cpu" in str(src.device)):
                 why_not_sparsity_fast_path = "src is neither CUDA nor CPU"
             elif torch.is_grad_enabled() and any(x.requires_grad for x in tensor_args):
-                why_not_sparsity_fast_path = (
-                    "grad is enabled and at least one of query or the i/o projection weights or biases requires_grad")
+                why_not_sparsity_fast_path = "grad is enabled and at least one of query or the i/o projection weights or biases requires_grad"
 
             if (not why_not_sparsity_fast_path) and (src_key_padding_mask is not None):
                 convert_to_nested = True
                 output = torch._nested_tensor_from_mask(
-                    output, src_key_padding_mask.logical_not(), mask_check=False)
+                    output, src_key_padding_mask.logical_not(), mask_check=False
+                )
                 src_key_padding_mask_for_layers = None
 
         return output, convert_to_nested, src_key_padding_mask_for_layers
 
     def get_model_dict(self):
-        """Returns dictionary with model information and weights.
-        """
+        """Returns dictionary with model information and weights."""
         model_dict = self.init_dict
         model_dict.update(
-            {'stored_values': self.extract_parameters(without_layer_norm=False)})
+            {"stored_values": self.extract_parameters(without_layer_norm=False)}
+        )
         return model_dict
 
     def count_parameters(self, without_layer_norm=False):
         """Returns number of parameters in neural network.
 
         :param without_layer_norm: Exclude normalization layers, defaults to False
         :type without_layer_norm: bool, optional
         """
         count = 0
         for name, param in self.named_parameters():
-            if not without_layer_norm or 'layer_norm' not in name:
+            if not without_layer_norm or "layer_norm" not in name:
                 count += param.data.cpu().numpy().flatten().shape[0]
         return count
 
     def extract_grad(self, without_layer_norm=False):
         """Returns current pytorch gradient in same order as genome's flattened parameter vector.
 
         :param without_layer_norm: Exclude normalization layers, defaults to False
         :type without_layer_norm: bool, optional
         """
         tot_size = self.count_parameters(without_layer_norm)
         pvec = np.zeros(tot_size, np.float32)
         count = 0
         for name, param in self.named_parameters():
-            if not without_layer_norm or 'layer_norm' not in name:
+            if not without_layer_norm or "layer_norm" not in name:
                 sz = param.grad.data.cpu().numpy().flatten().shape[0]
-                pvec[count:count + sz] = param.grad.data.cpu().numpy().flatten()
+                pvec[count : count + sz] = param.grad.data.cpu().numpy().flatten()
                 count += sz
         return pvec.copy()
 
     def extract_parameters(self, without_layer_norm=False):
         """Returns current flattened neural network weights.
 
         :param without_layer_norm: Exclude normalization layers, defaults to False
         :type without_layer_norm: bool, optional
         """
         tot_size = self.count_parameters(without_layer_norm)
         pvec = np.zeros(tot_size, np.float32)
         count = 0
         for name, param in self.named_parameters():
-            if not without_layer_norm or 'layer_norm' not in name:
+            if not without_layer_norm or "layer_norm" not in name:
                 sz = param.data.cpu().detach().numpy().flatten().shape[0]
-                pvec[count:count + sz] = param.data.cpu().detach().numpy().flatten()
+                pvec[count : count + sz] = param.data.cpu().detach().numpy().flatten()
                 count += sz
         return copy.deepcopy(pvec)
 
     def inject_parameters(self, pvec, without_layer_norm=False):
         """Injects a flat vector of neural network parameters into the model's current neural network weights.
 
         :param pvec: Network weights
         :type pvec: np.array()
         :param without_layer_norm: Exclude normalization layers, defaults to False
         :type without_layer_norm: bool, optional
         """
         count = 0
 
         for name, param in self.named_parameters():
-            if not without_layer_norm or 'layer_norm' not in name:
+            if not without_layer_norm or "layer_norm" not in name:
                 sz = param.data.cpu().numpy().flatten().shape[0]
-                raw = pvec[count:count + sz]
+                raw = pvec[count : count + sz]
                 reshaped = raw.reshape(param.data.cpu().numpy().shape)
-                param.data = torch.from_numpy(
-                    copy.deepcopy(reshaped)).type(torch.FloatTensor)
+                param.data = torch.from_numpy(copy.deepcopy(reshaped)).type(
+                    torch.FloatTensor
+                )
                 count += sz
         return pvec
 
     @property
     def init_dict(self):
-        """Returns model information in dictionary.
-        """
+        """Returns model information in dictionary."""
         init_dict = {
             "encoder_layers": self.encoder_layers,
             "decoder_layers": self.decoder_layers,
             "end2end": self.end2end,
             "src_vocab_size": self.src_vocab_size,
             "tgt_vocab_size": self.tgt_vocab_size,
             "encoder_norm": self.encoder_norm,
@@ -550,47 +602,44 @@
             "dropout": self.dropout,
             "activation": self.activation,
             "layer_norm_eps": self.layer_norm_eps,
             "batch_first": self.batch_first,
             "norm_first": self.norm_first,
             "max_encoder_layers": self.max_encoder_layers,
             "max_decoder_layers": self.max_decoder_layers,
-            "device": self.device}
+            "device": self.device,
+        }
         return init_dict
 
     def add_encoder_layer(self):
-        """Adds an encoder layer to transformer.
-        """
+        """Adds an encoder layer to transformer."""
         if len(self.encoder_layers) < self.max_encoder_layers:
             self.encoder_layers += [self.encoder_layers[-1]]
             self.recreate_nets()
         # else:
         #     self.add_node()
 
     def add_decoder_layer(self):
-        """Adds a decoder layer to transformer.
-        """
+        """Adds a decoder layer to transformer."""
         if len(self.decoder_layers) < self.max_decoder_layers:
             self.decoder_layers += [self.decoder_layers[-1]]
             self.recreate_nets()
         # else:
         #     self.add_node()
 
     def remove_encoder_layer(self):
-        """Removes an encoder layer from transformer.
-        """
+        """Removes an encoder layer from transformer."""
         if len(self.encoder_layers) > 1:
             self.encoder_layers = self.encoder_layers[:-1]
             self.recreate_shrunk_nets()
         # else:
         #     self.add_node()
 
     def remove_decoder_layer(self):
-        """Removes a decoder layer from transformer.
-        """
+        """Removes a decoder layer from transformer."""
         if len(self.decoder_layers) > 1:
             self.decoder_layers = self.decoder_layers[:-1]
             self.recreate_shrunk_nets()
         # else:
         #     self.add_node()
 
     def add_node(self, network=None, hidden_layer=None, numb_new_nodes=None):
@@ -600,94 +649,97 @@
         :type network: str, optional
         :param hidden_layer: Depth of hidden layer to add nodes to, defaults to None
         :type hidden_layer: int, optional
         :param numb_new_nodes: Number of nodes to add to hidden layer, defaults to None
         :type numb_new_nodes: int, optional
         """
         if network is None:
-            network = np.random.choice(['encoder', 'decoder'], 1)[0]
+            network = np.random.choice(["encoder", "decoder"], 1)[0]
         if numb_new_nodes is None:
             numb_new_nodes = np.random.choice([16, 32, 64], 1)[0]
-        if network == 'encoder':
+        if network == "encoder":
             if hidden_layer is None:
-                hidden_layer = np.random.randint(
-                    0, len(self.encoder_layers), 1)[0]
+                hidden_layer = np.random.randint(0, len(self.encoder_layers), 1)[0]
             else:
                 hidden_layer = min(hidden_layer, len(self.encoder_layers) - 1)
 
             self.encoder_layers[hidden_layer] += numb_new_nodes
         else:
             if hidden_layer is None:
-                hidden_layer = np.random.randint(
-                    0, len(self.decoder_layers), 1)[0]
+                hidden_layer = np.random.randint(0, len(self.decoder_layers), 1)[0]
             else:
                 hidden_layer = min(hidden_layer, len(self.decoder_layers) - 1)
 
             self.decoder_layers[hidden_layer] += numb_new_nodes
         self.recreate_nets()
-        return {"hidden_layer": hidden_layer,
-                "numb_new_nodes": numb_new_nodes, "network": network}
+        return {
+            "hidden_layer": hidden_layer,
+            "numb_new_nodes": numb_new_nodes,
+            "network": network,
+        }
 
     def remove_node(self, network=None, hidden_layer=None, numb_new_nodes=None):
         """Removes nodes from hidden layer of encoder/decoder.
 
         :param network: Network to remove node from, 'encoder' or 'decoder', defaults to None
         :type network: str, optional
         :param hidden_layer: Depth of hidden layer to remove nodes from, defaults to None
         :type hidden_layer: int, optional
         :param numb_new_nodes: Number of nodes to remove from hidden layer, defaults to None
         :type numb_new_nodes: int, optional
         """
         if network is None:
-            network = np.random.choice(['encoder', 'decoder'], 1)[0]
+            network = np.random.choice(["encoder", "decoder"], 1)[0]
         if numb_new_nodes is None:
             numb_new_nodes = np.random.choice([16, 32, 64], 1)[0]
-        if network == 'encoder':
+        if network == "encoder":
             if hidden_layer is None:
-                hidden_layer = np.random.randint(
-                    0, len(self.encoder_layers), 1)[0]
+                hidden_layer = np.random.randint(0, len(self.encoder_layers), 1)[0]
             else:
                 hidden_layer = min(hidden_layer, len(self.encoder_layers) - 1)
             if self.encoder_layers[hidden_layer] - numb_new_nodes > 64:  # HARD LIMIT
                 self.encoder_layers[hidden_layer] -= numb_new_nodes
         else:
             if hidden_layer is None:
-                hidden_layer = np.random.randint(
-                    0, len(self.decoder_layers), 1)[0]
+                hidden_layer = np.random.randint(0, len(self.decoder_layers), 1)[0]
             else:
                 hidden_layer = min(hidden_layer, len(self.decoder_layers) - 1)
             if self.decoder_layers[hidden_layer] - numb_new_nodes > 64:  # HARD LIMIT
                 self.decoder_layers[hidden_layer] -= numb_new_nodes
         self.recreate_shrunk_nets()
-        return {"hidden_layer": hidden_layer,
-                "numb_new_nodes": numb_new_nodes, "network": network}
+        return {
+            "hidden_layer": hidden_layer,
+            "numb_new_nodes": numb_new_nodes,
+            "network": network,
+        }
 
     def recreate_nets(self):
-        """Recreates neural networks.
-        """
+        """Recreates neural networks."""
         new_encoder, new_decoder = self.create_nets()
         new_encoder = self.preserve_parameters(
-            old_net=self.encoder, new_net=new_encoder)
+            old_net=self.encoder, new_net=new_encoder
+        )
         new_decoder = self.preserve_parameters(
-            old_net=self.decoder, new_net=new_decoder)
+            old_net=self.decoder, new_net=new_decoder
+        )
         self.encoder, self.decoder = new_encoder, new_decoder
 
     def recreate_shrunk_nets(self):
-        """Recreates shrunk neural networks.
-        """
+        """Recreates shrunk neural networks."""
         new_encoder, new_decoder = self.create_nets()
         new_encoder = self.shrink_preserve_parameters(
-            old_net=self.encoder, new_net=new_encoder)
+            old_net=self.encoder, new_net=new_encoder
+        )
         new_decoder = self.shrink_preserve_parameters(
-            old_net=self.decoder, new_net=new_decoder)
+            old_net=self.decoder, new_net=new_decoder
+        )
         self.encoder, self.decoder = new_encoder, new_decoder
 
     def clone(self):
-        """Returns clone of neural net with identical parameters.
-        """
+        """Returns clone of neural net with identical parameters."""
         clone = EvolvableBERT(**copy.deepcopy(self.init_dict))
         clone.load_state_dict(self.state_dict())
         return clone
 
     def preserve_parameters(self, old_net, new_net):
         """Returns new neural network with copied parameters from old network.
 
@@ -703,27 +755,25 @@
                 if old_net_dict[key].data.size() == param.data.size():
                     param.data = old_net_dict[key].data
                 else:
                     if "norm" not in key:
                         old_size = old_net_dict[key].data.size()
                         new_size = param.data.size()
                         if len(param.data.size()) == 1:
-                            param.data[:min(old_size[0], new_size[0])] = old_net_dict[key].data[
-                                :min(old_size[0], new_size[0])]
+                            param.data[: min(old_size[0], new_size[0])] = old_net_dict[
+                                key
+                            ].data[: min(old_size[0], new_size[0])]
                         else:
-                            param.data[:min(old_size[0], new_size[0]), :min(old_size[1], new_size[1])] = old_net_dict[
-                                key].data[
-                                :min(old_size[
-                                    0],
-                                    new_size[
-                                    0]),
-                                :min(old_size[
-                                    1],
-                                    new_size[
-                                    1])]
+                            param.data[
+                                : min(old_size[0], new_size[0]),
+                                : min(old_size[1], new_size[1]),
+                            ] = old_net_dict[key].data[
+                                : min(old_size[0], new_size[0]),
+                                : min(old_size[1], new_size[1]),
+                            ]
 
         return new_net
 
     def shrink_preserve_parameters(self, old_net, new_net):
         """Returns shrunk new neural network with copied parameters from old network.
 
         :param old_net: Old neural network
@@ -742,82 +792,84 @@
                         old_size = old_net_dict[key].data.size()
                         new_size = param.data.size()
                         min_0 = min(old_size[0], new_size[0])
                         if len(param.data.size()) == 1:
                             param.data[:min_0] = old_net_dict[key].data[:min_0]
                         else:
                             min_1 = min(old_size[1], new_size[1])
-                            param.data[:min_0,
-                                       :min_1] = old_net_dict[key].data[:min_0, :min_1]
+                            param.data[:min_0, :min_1] = old_net_dict[key].data[
+                                :min_0, :min_1
+                            ]
         return new_net
 
 
-def _canonical_mask(mask, mask_name, other_type, other_name,
-                    target_type, check_other=True):
+def _canonical_mask(
+    mask, mask_name, other_type, other_name, target_type, check_other=True
+):
     """Returns canconical mask. Adapted from torch.nn.functional"""
     if mask is not None:
         _mask_dtype = mask.dtype
         _mask_is_float = torch.is_floating_point(mask)
         if _mask_dtype != torch.bool and not _mask_is_float:
             raise AssertionError(
-                f"only bool and floating types of {mask_name} are supported")
+                f"only bool and floating types of {mask_name} are supported"
+            )
         if check_other and other_type is not None:
             if _mask_dtype != other_type:
                 warnings.warn(
                     f"Support for mismatched {mask_name} and {other_name} "
                     "is deprecated. Use same type for both instead."
                 )
         if not _mask_is_float:
-            mask = (
-                torch.zeros_like(mask, dtype=target_type)
-                .masked_fill_(mask, float("-inf"))
+            mask = torch.zeros_like(mask, dtype=target_type).masked_fill_(
+                mask, float("-inf")
             )
     return mask
 
 
 class PositionalEncoder(nn.Module):
-    """The Positional Encoder class. 
+    """The Positional Encoder class.
     Adds positional encoding to the token embedding to introduce a notion of word order.
 
     :param emb_size: Number of expected features
     :type emb_size: int
     :param dropout: Dropout value, defaults to 0.1
     :type dropout: float, optional
     :param maxlen: Maximum length of sequence, defaults to 5000
     :type maxlen: int, optional
     """
 
     def __init__(self, emb_size: int, dropout: float, maxlen: int = 5000):
-        super(PositionalEncoder, self).__init__()
+        super().__init__()
 
-        den = torch.exp(- torch.arange(0, emb_size, 2)
-                        * math.log(10000) / emb_size)
+        den = torch.exp(-torch.arange(0, emb_size, 2) * math.log(10000) / emb_size)
         pos = torch.arange(0, maxlen).reshape(maxlen, 1)
         pos_embedding = torch.zeros((maxlen, emb_size))
         pos_embedding[:, 0::2] = torch.sin(pos * den)
         pos_embedding[:, 1::2] = torch.cos(pos * den)
         pos_embedding = pos_embedding.unsqueeze(-2)
 
         self.dropout = nn.Dropout(dropout)
-        self.register_buffer('pos_embedding', pos_embedding)
+        self.register_buffer("pos_embedding", pos_embedding)
 
     def forward(self, x: torch.Tensor):
         """Forward pass through positional encoder.
         :param x: Input to positional encoder, shape [seq_len, batch_size, embedding_dim]
         :type x: torch.Tensor
         """
-        return self.dropout(x + self.pos_embedding[:x.size(0), :])
+        return self.dropout(x + self.pos_embedding[: x.size(0), :])
 
 
 class PositionalEncoding(nn.Module):
-    """The positional embedding class. 
-    Converts tensor of input indices into corresponding tensor of position embeddings."""
+    """The positional embedding class.
+    Converts tensor of input indices into corresponding tensor of position embeddings.
+    """
 
     def __init__(self, max_positions: int, emb_size):
-        super(PositionalEncoding, self).__init__()
+        super().__init__()
         self.embedding = nn.Embedding(max_positions, emb_size)
         self.emb_size = emb_size
 
     def forward(self, tokens: torch.Tensor):
         """Forward pass through position embedding module.
         :param tokens: Tokens to embed
         :type tokens: torch.Tensor
@@ -825,15 +877,15 @@
         return self.embedding(tokens)
 
 
 class TokenEmbedding(nn.Module):
     """The token embedding class. Converts tensor of input indices into corresponding tensor of token embeddings."""
 
     def __init__(self, vocab_size: int, emb_size):
-        super(TokenEmbedding, self).__init__()
+        super().__init__()
         self.embedding = nn.Embedding(vocab_size, emb_size)
         self.emb_size = emb_size
 
     def forward(self, tokens: torch.Tensor):
         """Forward pass through token embedding module.
         :param tokens: Tokens to embed
         :type tokens: torch.Tensor
@@ -847,9 +899,8 @@
     :param input: Input to return dtype of
     :type input: Any
     """
     if input is None:
         return None
     elif isinstance(input, torch.Tensor):
         return input.dtype
-    raise RuntimeError(
-        "input to _none_or_dtype() must be None or torch.Tensor")
+    raise RuntimeError("input to _none_or_dtype() must be None or torch.Tensor")
```

### Comparing `agilerl-0.1.8/agilerl/networks/evolvable_cnn.py` & `agilerl-0.1.9/agilerl/networks/evolvable_cnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 import copy
 import math
 from collections import OrderedDict
 from typing import List
-from agilerl.networks.custom_architecture import GumbelSoftmax
 
 import numpy as np
 import torch
 import torch.autograd as autograd
 import torch.nn as nn
 import torch.nn.functional as F
 
+from agilerl.networks.custom_architecture import GumbelSoftmax
+
 
 class NoisyLinear(nn.Module):
     """The Noisy Linear Neural Network class.
 
     :param in_features: Input features size
     :type in_features: int
     :param out_features: Output features size
     :type out_features: int
     :param std_init: Standard deviation, defaults to 0.4
     :type std_init: float, optional
     """
 
     def __init__(self, in_features, out_features, std_init=0.4):
-        super(NoisyLinear, self).__init__()
+        super().__init__()
 
         self.in_features = in_features
         self.out_features = out_features
         self.std_init = std_init
 
-        self.weight_mu = nn.Parameter(
-            torch.FloatTensor(out_features, in_features))
-        self.weight_sigma = nn.Parameter(
-            torch.FloatTensor(out_features, in_features))
+        self.weight_mu = nn.Parameter(torch.FloatTensor(out_features, in_features))
+        self.weight_sigma = nn.Parameter(torch.FloatTensor(out_features, in_features))
         self.register_buffer(
-            'weight_epsilon', torch.FloatTensor(out_features, in_features))
+            "weight_epsilon", torch.FloatTensor(out_features, in_features)
+        )
 
         self.bias_mu = nn.Parameter(torch.FloatTensor(out_features))
         self.bias_sigma = nn.Parameter(torch.FloatTensor(out_features))
-        self.register_buffer('bias_epsilon', torch.FloatTensor(out_features))
+        self.register_buffer("bias_epsilon", torch.FloatTensor(out_features))
 
         self.reset_parameters()
         self.reset_noise()
 
     def forward(self, x):
         """Returns output of neural network.
 
@@ -58,29 +58,27 @@
         else:
             weight = self.weight_mu
             bias = self.bias_mu
 
         return F.linear(x, weight, bias)
 
     def reset_parameters(self):
-        """Resets neural network parameters.
-        """
+        """Resets neural network parameters."""
         mu_range = 1 / math.sqrt(self.weight_mu.size(1))
 
         self.weight_mu.data.uniform_(-mu_range, mu_range)
         self.weight_sigma.data.fill_(
-            self.std_init / math.sqrt(self.weight_sigma.size(1)))
+            self.std_init / math.sqrt(self.weight_sigma.size(1))
+        )
 
         self.bias_mu.data.uniform_(-mu_range, mu_range)
-        self.bias_sigma.data.fill_(
-            self.std_init / math.sqrt(self.bias_sigma.size(0)))
+        self.bias_sigma.data.fill_(self.std_init / math.sqrt(self.bias_sigma.size(0)))
 
     def reset_noise(self):
-        """Resets neural network noise.
-        """
+        """Resets neural network noise."""
         epsilon_in = self._scale_noise(self.in_features)
         epsilon_out = self._scale_noise(self.out_features)
 
         self.weight_epsilon.copy_(epsilon_out.ger(epsilon_in))
         self.bias_epsilon.copy_(epsilon_out)
 
     def _scale_noise(self, size):
@@ -132,39 +130,39 @@
     :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
     :type device: str, optional
     :param accelerator: Accelerator for distributed computing, defaults to None
     :type accelerator: Hugging Face accelerate.Accelerator(), optional
     """
 
     def __init__(
-            self,
-            input_shape: List[int],
-            channel_size: List[int],
-            kernal_size: List[int],
-            stride_size: List[int],
-            hidden_size: List[int],
-            num_actions: int,
-            num_atoms=51,
-            mlp_activation='relu',
-            cnn_activation='relu',
-            n_agents=None,
-            multi=False,
-            layer_norm=False,
-            stored_values=None,
-            rainbow=False,
-            critic=False,
-            normalize=True,
-            device='cpu',
-            accelerator=None):
-
-        super(EvolvableCNN, self).__init__()
+        self,
+        input_shape: List[int],
+        channel_size: List[int],
+        kernel_size: List[int],
+        stride_size: List[int],
+        hidden_size: List[int],
+        num_actions: int,
+        num_atoms=51,
+        mlp_activation="relu",
+        cnn_activation="relu",
+        n_agents=None,
+        multi=False,
+        layer_norm=False,
+        stored_values=None,
+        rainbow=False,
+        critic=False,
+        normalize=True,
+        device="cpu",
+        accelerator=None,
+    ):
+        super().__init__()
 
         self.input_shape = input_shape
         self.channel_size = channel_size
-        self.kernal_size = kernal_size
+        self.kernel_size = kernel_size
         self.stride_size = stride_size
         self.hidden_size = hidden_size
         self.num_actions = num_actions
         self.num_atoms = num_atoms
         self.mlp_activation = mlp_activation
         self.cnn_activation = cnn_activation
         self.layer_norm = layer_norm
@@ -174,178 +172,206 @@
         self.device = device
         self.accelerator = accelerator
         self.multi = multi
         self.n_agents = n_agents
 
         self.net = self.create_nets()
         self.feature_net, self.value_net, self.advantage_net = self.create_nets()
-        
+
         if stored_values is not None:
             self.inject_parameters(pvec=stored_values, without_layer_norm=False)
 
-
     def get_activation(self, activation_names):
         """Returns activation function for corresponding activation name.
 
         :param activation_names: Activation function name
         :type activation_names: str
         """
         activation_functions = {
-            'tanh': nn.Tanh,
-            'gelu': nn.GELU,
-            'relu': nn.ReLU,
-            'elu': nn.ELU,
-            'softsign': nn.Softsign,
-            'sigmoid': nn.Sigmoid,
-            'gumbel_softmax' : GumbelSoftmax,
-            'softplus': nn.Softplus,
-            'lrelu': nn.LeakyReLU,
-            'prelu': nn.PReLU}
-        return activation_functions[activation_names]()
+            "tanh": nn.Tanh,
+            "gelu": nn.GELU,
+            "relu": nn.ReLU,
+            "elu": nn.ELU,
+            "softsign": nn.Softsign,
+            "sigmoid": nn.Sigmoid,
+            "softmax": nn.Softmax,
+            "gumbel_softmax": GumbelSoftmax,
+            "softplus": nn.Softplus,
+            "lrelu": nn.LeakyReLU,
+            "prelu": nn.PReLU,
+        }
+        return activation_functions[activation_names](dim=1) if activation_names == 'softmax' \
+            else activation_functions[activation_names]()
 
     def create_mlp(self, input_size, output_size, hidden_size, name):
-        """Creates and returns multi-layer perceptron.
-        """
+        """Creates and returns multi-layer perceptron."""
         net_dict = OrderedDict()
-        net_dict[f"{name}_linear_layer_0"] = NoisyLinear(
-            input_size, hidden_size[0])
+        net_dict[f"{name}_linear_layer_0"] = NoisyLinear(input_size, hidden_size[0])
         if self.layer_norm:
             net_dict[f"{name}_layer_norm_0"] = nn.LayerNorm(hidden_size[0])
-        net_dict[f"{name}_activation_0"] = self.get_activation(
-            self.mlp_activation)
+        net_dict[f"{name}_activation_0"] = self.get_activation(self.mlp_activation)
 
         if len(hidden_size) > 1:
             for l_no in range(1, len(hidden_size)):
                 net_dict[f"{name}_linear_layer_{str(l_no)}"] = NoisyLinear(
-                    hidden_size[l_no - 1], hidden_size[l_no])
+                    hidden_size[l_no - 1], hidden_size[l_no]
+                )
                 if self.layer_norm:
                     net_dict[f"{name}_layer_norm_{str(l_no)}"] = nn.LayerNorm(
-                        hidden_size[l_no])
+                        hidden_size[l_no]
+                    )
                 net_dict[f"{name}_activation_{str(l_no)}"] = self.get_activation(
-                    self.mlp_activation)
+                    self.mlp_activation
+                )
         net_dict[f"{name}_linear_layer_output"] = NoisyLinear(
-            hidden_size[-1], output_size)
+            hidden_size[-1], output_size
+        )
         return nn.Sequential(net_dict)
 
-    def create_cnn(self, input_size, channel_size, kernal_size, stride_size, name):
-        """Creates and returns convolutional neural network.
-        """
+    def create_cnn(self, input_size, channel_size, kernel_size, stride_size, name):
+        """Creates and returns convolutional neural network."""
         if self.multi:
             net_dict = OrderedDict()
             net_dict[f"{name}_conv_layer_0"] = nn.Conv3d(
                 in_channels=input_size,
                 out_channels=channel_size[0],
-                kernel_size=kernal_size[0],
-                stride=stride_size[0]            ## Maybe include the ability to have 3 dim kernel and stride
+                kernel_size=kernel_size[0],
+                stride=stride_size[
+                    0
+                ],  ## Maybe include the ability to have 3 dim kernel and stride
             )
             if self.layer_norm:
                 net_dict[f"{name}_layer_norm_0"] = nn.BatchNorm3d(channel_size[0])
             net_dict[f"{name}_activation_0"] = self.get_activation(self.cnn_activation)
 
             if len(channel_size) > 1:
                 for l_no in range(1, len(channel_size)):
-                    net_dict[f"{name}_conv_layer_{str(l_no)}"] = nn.Conv3d(in_channels=channel_size[l_no - 1],
-                                                                           out_channels=channel_size[l_no],
-                                                                           kernel_size=kernal_size[l_no],
-                                                                           stride=stride_size[l_no])
+                    net_dict[f"{name}_conv_layer_{str(l_no)}"] = nn.Conv3d(
+                        in_channels=channel_size[l_no - 1],
+                        out_channels=channel_size[l_no],
+                        kernel_size=kernel_size[l_no],
+                        stride=stride_size[l_no],
+                    )
                     if self.layer_norm:
                         net_dict[f"{name}_layer_norm_{str(l_no)}"] = nn.BatchNorm3d(
-                            channel_size[l_no])
+                            channel_size[l_no]
+                        )
                     net_dict[f"{name}_activation_{str(l_no)}"] = self.get_activation(
                         self.cnn_activation
                     )
         else:
             net_dict = OrderedDict()
             net_dict[f"{name}_conv_layer_0"] = nn.Conv2d(
                 in_channels=input_size,
                 out_channels=channel_size[0],
-                kernel_size=kernal_size[0],
-                stride=stride_size[0])
+                kernel_size=kernel_size[0],
+                stride=stride_size[0],
+            )
             if self.layer_norm:
                 net_dict[f"{name}_layer_norm_0"] = nn.BatchNorm2d(channel_size[0])
-            net_dict[f"{name}_activation_0"] = self.get_activation(
-                self.cnn_activation)
+            net_dict[f"{name}_activation_0"] = self.get_activation(self.cnn_activation)
 
             if len(channel_size) > 1:
                 for l_no in range(1, len(channel_size)):
-                    net_dict[f"{name}_conv_layer_{str(l_no)}"] = nn.Conv2d(in_channels=channel_size[l_no - 1],
-                                                                            out_channels=channel_size[l_no],
-                                                                            kernel_size=kernal_size[l_no],
-                                                                            stride=stride_size[l_no])
+                    net_dict[f"{name}_conv_layer_{str(l_no)}"] = nn.Conv2d(
+                        in_channels=channel_size[l_no - 1],
+                        out_channels=channel_size[l_no],
+                        kernel_size=kernel_size[l_no],
+                        stride=stride_size[l_no],
+                    )
                     if self.layer_norm:
                         net_dict[f"{name}_layer_norm_{str(l_no)}"] = nn.BatchNorm2d(
-                            channel_size[l_no])
+                            channel_size[l_no]
+                        )
                     net_dict[f"{name}_activation_{str(l_no)}"] = self.get_activation(
-                        self.cnn_activation)
+                        self.cnn_activation
+                    )
 
         return nn.Sequential(net_dict)
 
     def create_nets(self):
-        """Creates and returns neural networks.
-        """
-        
+        """Creates and returns neural networks."""
+
         feature_net = self.create_cnn(
             self.input_shape[0],
             self.channel_size,
-            self.kernal_size,
+            self.kernel_size,
             self.stride_size,
-            name="feature")
+            name="feature",
+        )
 
         if self.multi:
-            input_size = feature_net(autograd.Variable(
-                    torch.zeros(1, *self.input_shape).unsqueeze(2))).view(1, -1).size(1)
+            input_size = (
+                feature_net(
+                    autograd.Variable(torch.zeros(1, *self.input_shape).unsqueeze(2))
+                )
+                .view(1, -1)
+                .size(1)
+            )
         else:
-            input_size = feature_net(autograd.Variable(
-                torch.zeros(1, *self.input_shape))).view(1, -1).size(1)
+            input_size = (
+                feature_net(autograd.Variable(torch.zeros(1, *self.input_shape)))
+                .view(1, -1)
+                .size(1)
+            )
 
         if self.critic:
             input_size += self.num_actions
 
         if self.rainbow:
             value_net = self.create_mlp(
                 input_size,
                 output_size=self.num_atoms,
                 hidden_size=self.hidden_size,
-                name="value")
+                name="value",
+            )
             advantage_net = self.create_mlp(
                 input_size,
-                output_size=self.num_atoms *
-                self.num_actions,
+                output_size=self.num_atoms * self.num_actions,
                 hidden_size=self.hidden_size,
-                name="advantage")
+                name="advantage",
+            )
             if self.accelerator is not None:
-                feature_net, value_net, advantage_net \
-                    = self.accelerator.prepare(feature_net, value_net, advantage_net)
+                feature_net, value_net, advantage_net = self.accelerator.prepare(
+                    feature_net, value_net, advantage_net
+                )
             else:
-                self.feature_net, self.value_net, self.advantage_net \
-                    = feature_net.to(self.device), value_net.to(self.device), \
-                        advantage_net.to(self.device)
+                self.feature_net, self.value_net, self.advantage_net = (
+                    feature_net.to(self.device),
+                    value_net.to(self.device),
+                    advantage_net.to(self.device),
+                )
         else:
             if self.critic:
                 value_net = self.create_mlp(
                     input_size,
                     output_size=1,
                     hidden_size=self.hidden_size,
-                    name="value")
+                    name="value",
+                )
             else:
                 value_net = self.create_mlp(
                     input_size,
                     output_size=self.num_actions,
                     hidden_size=self.hidden_size,
-                    name="value")
+                    name="value",
+                )
             advantage_net = None
             if self.accelerator is None:
-                self.feature_net, self.value_net, = feature_net.to(self.device), \
-                    value_net.to(self.device)
-                
+                (
+                    self.feature_net,
+                    self.value_net,
+                ) = feature_net.to(
+                    self.device
+                ), value_net.to(self.device)
+
         return feature_net, value_net, advantage_net
 
     def reset_noise(self):
-        """Resets noise of value and advantage networks.
-        """
+        """Resets noise of value and advantage networks."""
         for layer in self.value_net:
             if isinstance(layer, NoisyLinear):
                 layer.reset_noise()
         if self.rainbow:
             for layer in self.advantage_net:
                 if isinstance(layer, NoisyLinear):
                     layer.reset_noise()
@@ -358,158 +384,157 @@
         :param xc: Actions to be evaluated by critic, defaults to None
         :type xc: torch.Tensor() or np.array, optional
         """
         if not isinstance(x, torch.Tensor):
             x = torch.FloatTensor(x)
 
         batch_size = x.size(0)
-        
+
         if self.normalize:
-            x = x / 255.
+            x = x / 255.0
 
         x = self.feature_net(x)
         x = x.reshape(batch_size, -1)
 
         if self.critic:
             x = torch.cat([x, xc], dim=1)
 
-
         value = self.value_net(x)
 
         if self.rainbow:
             advantage = self.advantage_net(x)
 
             value = value.view(batch_size, 1, self.num_atoms)
-            advantage = advantage.view(
-                batch_size, self.num_actions, self.num_atoms)
+            advantage = advantage.view(batch_size, self.num_actions, self.num_atoms)
 
             x = value + advantage - advantage.mean(1, keepdim=True)
-            x = F.softmax(x.view(-1, self.num_atoms), dim=-
-                          1).view(-1, self.num_actions, self.num_atoms)
+            x = F.softmax(x.view(-1, self.num_atoms), dim=-1).view(
+                -1, self.num_actions, self.num_atoms
+            )
 
         else:
             x = F.softmax(value, dim=-1)
-        
+
         return x
 
     def get_model_dict(self):
-        """Returns dictionary with model information and weights.
-        """
+        """Returns dictionary with model information and weights."""
         model_dict = self.init_dict
         model_dict.update(
-            {'stored_values': self.extract_parameters(without_layer_norm=False)})
+            {"stored_values": self.extract_parameters(without_layer_norm=False)}
+        )
         return model_dict
 
     def count_parameters(self, without_layer_norm=False):
         """Returns number of parameters in neural network.
 
         :param without_layer_norm: Exclude normalization layers, defaults to False
         :type without_layer_norm: bool, optional
         """
         count = 0
         for name, param in self.named_parameters():
-            if not without_layer_norm or 'layer_norm' not in name:
+            if not without_layer_norm or "layer_norm" not in name:
                 count += param.data.cpu().numpy().flatten().shape[0]
         return count
 
     def extract_grad(self, without_layer_norm=False):
-        """Returns current pytorch gradient in same order as genome's flattened 
+        """Returns current pytorch gradient in same order as genome's flattened
         parameter vector.
 
         :param without_layer_norm: Exclude normalization layers, defaults to False
         :type without_layer_norm: bool, optional
         """
         tot_size = self.count_parameters(without_layer_norm)
         pvec = np.zeros(tot_size, np.float32)
         count = 0
         for name, param in self.named_parameters():
-            if not without_layer_norm or 'layer_norm' not in name:
+            if not without_layer_norm or "layer_norm" not in name:
                 sz = param.grad.data.cpu().numpy().flatten().shape[0]
-                pvec[count:count + sz] = param.grad.data.cpu().numpy().flatten()
+                pvec[count : count + sz] = param.grad.data.cpu().numpy().flatten()
                 count += sz
         return pvec.copy()
 
     def extract_parameters(self, without_layer_norm=False):
         """Returns current flattened neural network weights.
 
         :param without_layer_norm: Exclude normalization layers, defaults to False
         :type without_layer_norm: bool, optional
         """
         tot_size = self.count_parameters(without_layer_norm)
         pvec = np.zeros(tot_size, np.float32)
         count = 0
         for name, param in self.named_parameters():
-            if not without_layer_norm or 'layer_norm' not in name:
+            if not without_layer_norm or "layer_norm" not in name:
                 sz = param.data.cpu().detach().numpy().flatten().shape[0]
-                pvec[count:count + sz] = param.data.cpu().detach().numpy().flatten()
+                pvec[count : count + sz] = param.data.cpu().detach().numpy().flatten()
                 count += sz
         return copy.deepcopy(pvec)
 
     def inject_parameters(self, pvec, without_layer_norm=False):
-        """Injects a flat vector of neural network parameters into the model's current 
+        """Injects a flat vector of neural network parameters into the model's current
         neural network weights.
 
         :param pvec: Network weights
         :type pvec: np.array()
         :param without_layer_norm: Exclude normalization layers, defaults to False
         :type without_layer_norm: bool, optional
         """
         count = 0
 
         for name, param in self.named_parameters():
-            if not without_layer_norm or 'layer_norm' not in name:
+            if not without_layer_norm or "layer_norm" not in name:
                 sz = param.data.cpu().numpy().flatten().shape[0]
-                raw = pvec[count:count + sz]
+                raw = pvec[count : count + sz]
                 reshaped = raw.reshape(param.data.cpu().numpy().shape)
-                param.data = torch.from_numpy(
-                    copy.deepcopy(reshaped)).type(torch.FloatTensor)
+                param.data = torch.from_numpy(copy.deepcopy(reshaped)).type(
+                    torch.FloatTensor
+                )
                 count += sz
         return pvec
 
     @property
     def short_dict(self):
-        """Returns shortened version of model information in dictionary.
-        """
+        """Returns shortened version of model information in dictionary."""
         short_dict = {
             "channel_size": self.channel_size,
-            "kernal_size": self.kernal_size,
+            "kernel_size": self.kernel_size,
             "stride_size": self.stride_size,
             "hidden_size": self.hidden_size,
             "num_atoms": self.num_atoms,
             "mlp_activation": self.mlp_activation,
             "cnn_activation": self.cnn_activation,
-            "layer_norm": self.layer_norm}
+            "layer_norm": self.layer_norm,
+        }
         return short_dict
 
     @property
     def init_dict(self):
-        """Returns model information in dictionary.
-        """
+        """Returns model information in dictionary."""
         initdict = {
             "input_shape": self.input_shape,
             "channel_size": self.channel_size,
-            "kernal_size": self.kernal_size,
+            "kernel_size": self.kernel_size,
             "stride_size": self.stride_size,
             "hidden_size": self.hidden_size,
             "num_actions": self.num_actions,
             "n_agents": self.n_agents,
             "num_atoms": self.num_atoms,
             "normalize": self.normalize,
             "mlp_activation": self.mlp_activation,
             "cnn_activation": self.cnn_activation,
-            "multi":self.multi,
+            "multi": self.multi,
             "layer_norm": self.layer_norm,
             "critic": self.critic,
             "device": self.device,
-            "accelerator": self.accelerator}
+            "accelerator": self.accelerator,
+        }
         return initdict
 
     def add_mlp_layer(self):
-        """Adds a hidden layer to Multi-layer Perceptron.
-        """
+        """Adds a hidden layer to Multi-layer Perceptron."""
         if len(self.hidden_size) < 3:  # HARD LIMIT
             self.hidden_size += [self.hidden_size[-1]]
 
             self.recreate_nets()
         else:
             self.add_mlp_node()
 
@@ -525,67 +550,87 @@
             hidden_layer = np.random.randint(0, len(self.hidden_size), 1)[0]
         else:
             hidden_layer = min(hidden_layer, len(self.hidden_size) - 1)
         if numb_new_nodes is None:
             numb_new_nodes = np.random.choice([32, 64, 128], 1)[0]
 
         if self.hidden_size[hidden_layer] + numb_new_nodes <= 1024:  # HARD LIMIT
-
             self.hidden_size[hidden_layer] += numb_new_nodes
 
             self.recreate_nets()
         return {"hidden_layer": hidden_layer, "numb_new_nodes": numb_new_nodes}
 
     def add_cnn_layer(self):
-        """Adds a hidden layer to Convolutional Neural Network.
-        """
+        """Adds a hidden layer to Convolutional Neural Network."""
         if self.multi:
             if len(self.channel_size) < 6:  # HARD LIMIT
                 self.channel_size += [self.channel_size[-1]]
-                self.kernal_size += [(1, 3, 3)]
-                stride_size_list = [[4], [4, 2], [4, 2, 1], [
-                        2, 2, 2, 1], [2, 1, 2, 1, 2], [2, 1, 2, 1, 2, 1]]
+                self.kernel_size += [(1, 3, 3)]
+                stride_size_list = [
+                    [4],
+                    [4, 2],
+                    [4, 2, 1],
+                    [2, 2, 2, 1],
+                    [2, 1, 2, 1, 2],
+                    [2, 1, 2, 1, 2, 1],
+                ]
                 self.stride_size = stride_size_list[len(self.channel_size) - 1]
 
                 self.recreate_nets()
             else:
                 self.add_cnn_channel()
 
         else:
             if len(self.channel_size) < 6:  # HARD LIMIT
                 self.channel_size += [self.channel_size[-1]]
-                self.kernal_size += [3]
+                self.kernel_size += [3]
 
-                stride_size_list = [[4], [4, 2], [4, 2, 1], [
-                    2, 2, 2, 1], [2, 1, 2, 1, 2], [2, 1, 2, 1, 2, 1]]
+                stride_size_list = [
+                    [4],
+                    [4, 2],
+                    [4, 2, 1],
+                    [2, 2, 2, 1],
+                    [2, 1, 2, 1, 2],
+                    [2, 1, 2, 1, 2, 1],
+                ]
                 self.stride_size = stride_size_list[len(self.channel_size) - 1]
 
                 self.recreate_nets()
             else:
                 self.add_cnn_channel()
 
-    def change_cnn_kernal(self):
-        """Randomly alters convolution kernal of random CNN layer.
-        """
+    def change_cnn_kernel(self):
+        """Randomly alters convolution kernel of random CNN layer."""
 
         if self.multi:
             if len(self.channel_size) > 1:
-                hidden_layer = np.random.randint(1, min(4, len(self.channel_size)), 1)[0]
-                kernal_size_value = np.random.choice([3, 4, 5, 7])
+                hidden_layer = np.random.randint(1, min(4, len(self.channel_size)), 1)[
+                    0
+                ]
+                kernel_size_value = np.random.choice([3, 4, 5, 7])
                 if self.critic:
-                    self.kernal_size[hidden_layer] = tuple(min(kernal_size_value, self.n_agents - 1) if idx == 0 else kernal_size_value for idx in range(3))
+                    self.kernel_size[hidden_layer] = tuple(
+                        min(kernel_size_value, self.n_agents - 1)
+                        if idx == 0
+                        else kernel_size_value
+                        for idx in range(3)
+                    )
                 else:
-                    self.kernal_size[hidden_layer] = tuple(1 if idx == 0 else kernal_size_value for idx in range(3))
+                    self.kernel_size[hidden_layer] = tuple(
+                        1 if idx == 0 else kernel_size_value for idx in range(3)
+                    )
                 self.recreate_nets()
             else:
                 self.add_cnn_layer()
         else:
             if len(self.channel_size) > 1:
-                hidden_layer = np.random.randint(1, min(4, len(self.channel_size)), 1)[0]
-                self.kernal_size[hidden_layer] = np.random.choice([3, 4, 5, 7])
+                hidden_layer = np.random.randint(1, min(4, len(self.channel_size)), 1)[
+                    0
+                ]
+                self.kernel_size[hidden_layer] = np.random.choice([3, 4, 5, 7])
 
                 self.recreate_nets()
             else:
                 self.add_cnn_layer()
 
     def add_cnn_channel(self, hidden_layer=None, numb_new_channels=None):
         """Adds channel to hidden layer of Convolutional Neural Network.
@@ -599,37 +644,41 @@
             hidden_layer = np.random.randint(0, len(self.channel_size), 1)[0]
         else:
             hidden_layer = min(hidden_layer, len(self.channel_size) - 1)
         if numb_new_channels is None:
             numb_new_channels = np.random.choice([8, 16, 32], 1)[0]
 
         if self.channel_size[hidden_layer] + numb_new_channels <= 256:  # HARD LIMIT
-
             self.channel_size[hidden_layer] += numb_new_channels
 
             self.recreate_nets()
 
         return {"hidden_layer": hidden_layer, "numb_new_channels": numb_new_channels}
 
     def recreate_nets(self):
-        """Recreates neural networks.
-        """
+        """Recreates neural networks."""
         new_feature_net, new_value_net, new_advantage_net = self.create_nets()
         new_feature_net = self.preserve_parameters(
-            old_net=self.feature_net, new_net=new_feature_net)
+            old_net=self.feature_net, new_net=new_feature_net
+        )
         new_value_net = self.preserve_parameters(
-            old_net=self.value_net, new_net=new_value_net)
+            old_net=self.value_net, new_net=new_value_net
+        )
         if self.rainbow:
             new_advantage_net = self.preserve_parameters(
-                old_net=self.advantage_net, new_net=new_advantage_net)
-        self.feature_net, self.value_net, self.advantage_net = new_feature_net, new_value_net, new_advantage_net
+                old_net=self.advantage_net, new_net=new_advantage_net
+            )
+        self.feature_net, self.value_net, self.advantage_net = (
+            new_feature_net,
+            new_value_net,
+            new_advantage_net,
+        )
 
     def clone(self):
-        """Returns clone of neural net with identical parameters.
-        """
+        """Returns clone of neural net with identical parameters."""
         clone = EvolvableCNN(**copy.deepcopy(self.init_dict))
         clone.load_state_dict(self.state_dict())
         clone.rainbow = self.rainbow
         clone.critic = self.critic
         return clone
 
     def preserve_parameters(self, old_net, new_net):
@@ -647,44 +696,37 @@
                 if old_net_dict[key].data.size() == param.data.size():
                     param.data = old_net_dict[key].data
                 else:
                     if "norm" not in key:
                         old_size = old_net_dict[key].data.size()
                         new_size = param.data.size()
                         if len(param.data.size()) == 1:
-                            param.data[:min(old_size[0], new_size[0])] = old_net_dict[key].data[
-                                :min(old_size[0], new_size[0])]
+                            param.data[: min(old_size[0], new_size[0])] = old_net_dict[
+                                key
+                            ].data[: min(old_size[0], new_size[0])]
                         elif len(param.data.size()) == 2:
-                            param.data[:min(old_size[0], new_size[0]), :min(old_size[1], new_size[1])] = old_net_dict[
-                                key].data[
-                                :min(old_size[
-                                    0],
-                                    new_size[
-                                    0]),
-                                :min(old_size[
-                                    1],
-                                    new_size[
-                                    1])]
+                            param.data[
+                                : min(old_size[0], new_size[0]),
+                                : min(old_size[1], new_size[1]),
+                            ] = old_net_dict[key].data[
+                                : min(old_size[0], new_size[0]),
+                                : min(old_size[1], new_size[1]),
+                            ]
                         else:
-                            param.data[:min(old_size[0],
-                                            new_size[0]),
-                                       :min(old_size[1],
-                                            new_size[1]),
-                                       :min(old_size[2],
-                                            new_size[2]),
-                                       :min(old_size[3],
-                                            new_size[3])] = old_net_dict[key].data[:min(old_size[0],
-                                                                                        new_size[0]),
-                                                                                   :min(old_size[1],
-                                                                                        new_size[1]),
-                                                                                   :min(old_size[2],
-                                                                                        new_size[2]),
-                                                                                   :min(old_size[3],
-                                                                                        new_size[3]),
-                                                                                   ]
+                            param.data[
+                                : min(old_size[0], new_size[0]),
+                                : min(old_size[1], new_size[1]),
+                                : min(old_size[2], new_size[2]),
+                                : min(old_size[3], new_size[3]),
+                            ] = old_net_dict[key].data[
+                                : min(old_size[0], new_size[0]),
+                                : min(old_size[1], new_size[1]),
+                                : min(old_size[2], new_size[2]),
+                                : min(old_size[3], new_size[3]),
+                            ]
 
         return new_net
 
     def shrink_preserve_parameters(self, old_net, new_net):
         """Returns shrunk new neural network with copied parameters from old network.
 
         :param old_net: Old neural network
@@ -703,10 +745,11 @@
                         old_size = old_net_dict[key].data.size()
                         new_size = param.data.size()
                         min_0 = min(old_size[0], new_size[0])
                         if len(param.data.size()) == 1:
                             param.data[:min_0] = old_net_dict[key].data[:min_0]
                         else:
                             min_1 = min(old_size[1], new_size[1])
-                            param.data[:min_0,
-                                       :min_1] = old_net_dict[key].data[:min_0, :min_1]
+                            param.data[:min_0, :min_1] = old_net_dict[key].data[
+                                :min_0, :min_1
+                            ]
         return new_net
```

### Comparing `agilerl-0.1.8/agilerl/networks/evolvable_gpt.py` & `agilerl-0.1.9/agilerl/networks/evolvable_gpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import copy
-from collections import OrderedDict
 import inspect
+import math
+import warnings
+from collections import OrderedDict
+
 import numpy as np
 import torch
 import torch.nn as nn
 from torch.nn import functional as F
-import math
-import warnings
+
 from agilerl.networks.evolvable_mlp import EvolvableMLP
 
 
 class EvolvableGPT(nn.Module):
     """The Evolvable GPT class.
 
     :param n_layer: Number of transformer block layers, defaults to 12
@@ -42,31 +44,32 @@
     :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
     :type device: str, optional
     :param accelerator: Accelerator for distributed computing, defaults to None
     :type accelerator: Hugging Face accelerate.Accelerator(), optional
     """
 
     def __init__(
-            self,
-            n_layer: int = 12,
-            vocab_size: int = 50257,
-            n_embd: int = 768,
-            n_head: int = 12,
-            dim_feedfwd: int = 3072,
-            block_size: int = 1024,
-            dropout: float = 0.0,
-            activation: str = 'gelu',
-            layer_norm_eps: float = 1e-5,
-            min_layers: int = 8,
-            max_layers: int = 16,
-            bias: bool = True,
-            stored_values = None,
-            device='cpu',
-            accelerator=None):
-        super(EvolvableGPT, self).__init__()
+        self,
+        n_layer: int = 12,
+        vocab_size: int = 50257,
+        n_embd: int = 768,
+        n_head: int = 12,
+        dim_feedfwd: int = 3072,
+        block_size: int = 1024,
+        dropout: float = 0.0,
+        activation: str = "gelu",
+        layer_norm_eps: float = 1e-5,
+        min_layers: int = 8,
+        max_layers: int = 16,
+        bias: bool = True,
+        stored_values=None,
+        device="cpu",
+        accelerator=None,
+    ):
+        super().__init__()
 
         self.n_layer = n_layer
         self.vocab_size = vocab_size
         self.n_embd = n_embd
         self.n_head = n_head
         self.dim_feedfwd = dim_feedfwd
         self.block_size = block_size
@@ -83,25 +86,25 @@
         self.transformer_keys = list(self.transformer.keys())
 
         self.lm_head = nn.Linear(self.n_embd, self.vocab_size, bias=False)
 
         self.transformer.wte.weight = self.lm_head.weight
 
         if stored_values is not None:
-            self.inject_parameters(
-                pvec=stored_values, without_layer_norm=False)
+            self.inject_parameters(pvec=stored_values, without_layer_norm=False)
 
         else:
             # init all weights
             self.apply(self._init_weights)
             # apply special scaled init to the residual projections, per GPT-2 paper
             for pn, p in self.named_parameters():
-                if pn.endswith('c_proj.weight'):
+                if pn.endswith("c_proj.weight"):
                     torch.nn.init.normal_(
-                        p, mean=0.0, std=0.02 / math.sqrt(2 * self.n_layer))
+                        p, mean=0.0, std=0.02 / math.sqrt(2 * self.n_layer)
+                    )
 
         # report number of parameters
         # print("number of parameters: %.2fM" % (self.get_num_params() / 1e6,))
 
     def get_num_params(self, non_embedding=True):
         """Return the number of parameters in the model.
         For non-embedding count (default), the position embeddings get subtracted.
@@ -124,76 +127,96 @@
     def get_activation(self, activation_names):
         """Returns activation function for corresponding activation name.
 
         :param activation_names: Activation function name
         :type activation_names: str
         """
         activation_functions = {
-            'tanh': nn.Tanh,
-            'linear': nn.Identity,
-            'relu': nn.ReLU,
-            'elu': nn.ELU,
-            'softsign': nn.Softsign,
-            'sigmoid': nn.Sigmoid,
-            'softplus': nn.Softplus,
-            'lrelu': nn.LeakyReLU,
-            'prelu': nn.PReLU,
-            'gelu': nn.GELU}
+            "tanh": nn.Tanh,
+            "linear": nn.Identity,
+            "relu": nn.ReLU,
+            "elu": nn.ELU,
+            "softsign": nn.Softsign,
+            "sigmoid": nn.Sigmoid,
+            "softplus": nn.Softplus,
+            "lrelu": nn.LeakyReLU,
+            "prelu": nn.PReLU,
+            "gelu": nn.GELU,
+        }
 
         return activation_functions[activation_names]()
 
     def create_net(self):
-        """Creates and returns transformer neural network.
-        """
+        """Creates and returns transformer neural network."""
         net_dict = OrderedDict()
-        net_dict['wte'] = nn.Embedding(self.vocab_size, self.n_embd)
-        net_dict['wpe'] = nn.Embedding(self.block_size, self.n_embd)
-        net_dict['drop'] = nn.Dropout(self.dropout)
-        net_dict['h'] = nn.ModuleList([Block(self.n_embd,
-                                             self.n_head,
-                                             self.bias,
-                                             self.dropout,
-                                             self.block_size,
-                                             self.dim_feedfwd,
-                                             self.activation,
-                                             self.layer_norm_eps) for _ in range(self.n_layer)])
-        net_dict['ln_f'] = LayerNorm(self.n_embd, bias=self.bias)
+        net_dict["wte"] = nn.Embedding(self.vocab_size, self.n_embd)
+        net_dict["wpe"] = nn.Embedding(self.block_size, self.n_embd)
+        net_dict["drop"] = nn.Dropout(self.dropout)
+        net_dict["h"] = nn.ModuleList(
+            [
+                Block(
+                    self.n_embd,
+                    self.n_head,
+                    self.bias,
+                    self.dropout,
+                    self.block_size,
+                    self.dim_feedfwd,
+                    self.activation,
+                    self.layer_norm_eps,
+                )
+                for _ in range(self.n_layer)
+            ]
+        )
+        net_dict["ln_f"] = LayerNorm(self.n_embd, bias=self.bias)
         return nn.ModuleDict(net_dict)
 
-    def forward(self, idx=None, tok_emb=None, targets=None, attn_mask=None, past_key_values=None, pos=None, 
-                is_causal=True):
+    def forward(
+        self,
+        idx=None,
+        tok_emb=None,
+        targets=None,
+        attn_mask=None,
+        past_key_values=None,
+        pos=None,
+        is_causal=True,
+    ):
         """Forward pass through evolvable GPT model.
-        
+
         :param idxs: Input ids
         :type idxs: torch.Tensor
         :param targets: Target ids
         :type targets: torch.Tensor
         """
         if idx is not None:
             device = idx.device
             t = idx.size(1)
         else:
             device = tok_emb.device
             t = tok_emb.size(-2)
-        
-        assert t <= self.block_size, f"Cannot forward sequence of length {t}, block size is only {self.block_size}"
+
+        assert (
+            t <= self.block_size
+        ), f"Cannot forward sequence of length {t}, block size is only {self.block_size}"
 
         presents = ()
         all_hidden_states = ()
         if past_key_values is None:
             past_length = 0
             past_key_values = tuple([None] * self.n_layer)
         else:
             past_length = past_key_values[0][0].size(-2)
 
         if pos is not None:
             pos = pos.view(-1, t)
         else:
-            pos = torch.arange(past_length, t+past_length, dtype=torch.long,
-                            device=device).unsqueeze(0)  # shape (1, t)
+            pos = torch.arange(
+                past_length, t + past_length, dtype=torch.long, device=device
+            ).unsqueeze(
+                0
+            )  # shape (1, t)
 
         # forward the GPT model itself
         # token embeddings of shape (b, t, n_embd)
         if tok_emb is None:
             tok_emb = self.transformer.wte(idx)
         # position embeddings of shape (1, t, n_embd)
         pos_emb = self.transformer.wpe(pos)
@@ -211,94 +234,103 @@
         all_hidden_states = all_hidden_states + (x,)
 
         logits = self.lm_head(x)
         if targets is not None:
             # if we are given some desired targets also calculate the loss
             # logits = self.lm_head(x)
             loss = F.cross_entropy(
-                logits.view(-1, logits.size(-1)), 
-                targets.view(-1).type(torch.LongTensor).to(self.device), 
-                ignore_index=-1)
+                logits.view(-1, logits.size(-1)),
+                targets.view(-1).type(torch.LongTensor).to(self.device),
+                ignore_index=-1,
+            )
         else:
-            # inference-time mini-optimization: only forward the lm_head on the very last 
+            # inference-time mini-optimization: only forward the lm_head on the very last
             # position
             # note: using list [-1] to preserve the time dim
             # logits = self.lm_head(x[:, [-1], :])
             loss = None
 
         return logits, all_hidden_states, presents, loss
 
     def crop_block_size(self, block_size):
         # model surgery to decrease the block size if necessary
         # e.g. we may load the GPT2 pretrained model checkpoint (block size 1024)
         # but want to use a smaller block size for some smaller, simpler model
         assert block_size <= self.block_size
         self.block_size = block_size
         self.transformer.wpe.weight = nn.Parameter(
-            self.transformer.wpe.weight[:block_size])
+            self.transformer.wpe.weight[:block_size]
+        )
         for block in self.transformer.h:
-            if hasattr(block.attn, 'bias'):
-                block.attn.bias = block.attn.bias[:,
-                                                  :, :block_size, :block_size]
+            if hasattr(block.attn, "bias"):
+                block.attn.bias = block.attn.bias[:, :, :block_size, :block_size]
 
     @classmethod
     def from_pretrained(cls, model_type, override_args=None, custom_sd=None):
-        assert model_type in {'gpt2', 'gpt2-medium', 'gpt2-large', 'gpt2-xl'}
+        assert model_type in {"gpt2", "gpt2-medium", "gpt2-large", "gpt2-xl"}
         override_args = override_args or {}  # default to empty dict
         from transformers import GPT2Config, GPT2LMHeadModel
+
         print("loading weights from pretrained gpt: %s" % model_type)
         config_args = {
-            'gpt2':         dict(n_layer=12, n_head=12, n_embd=768),  # 124M params
-            'gpt2-medium':  dict(n_layer=24, n_head=16, n_embd=1024), # 350M params
-            'gpt2-large':   dict(n_layer=36, n_head=20, n_embd=1280), # 774M params
-            'gpt2-xl':      dict(n_layer=48, n_head=25, n_embd=1600), # 1558M params
+            "gpt2": dict(n_layer=12, n_head=12, n_embd=768),  # 124M params
+            "gpt2-medium": dict(n_layer=24, n_head=16, n_embd=1024),  # 350M params
+            "gpt2-large": dict(n_layer=36, n_head=20, n_embd=1280),  # 774M params
+            "gpt2-xl": dict(n_layer=48, n_head=25, n_embd=1600),  # 1558M params
         }[model_type]
-        config_args['vocab_size'] = 50257 # always 50257 for GPT model checkpoints
-        config_args['block_size'] = 1024 # always 1024 for GPT model checkpoints
-        config_args['bias'] = True # always True for GPT model checkpoints
+        config_args["vocab_size"] = 50257  # always 50257 for GPT model checkpoints
+        config_args["block_size"] = 1024  # always 1024 for GPT model checkpoints
+        config_args["bias"] = True  # always True for GPT model checkpoints
         # we can override the dropout rate, if desired
-        if 'dropout' in override_args:
+        if "dropout" in override_args:
             print(f"overriding dropout rate to {override_args['dropout']}")
-            config_args['dropout'] = override_args['dropout']
+            config_args["dropout"] = override_args["dropout"]
 
         if custom_sd is not None:
-            if 'vocab_size' in override_args:
+            if "vocab_size" in override_args:
                 print(f"overriding vocab_size to {override_args['vocab_size']}")
-                config_args['vocab_size'] = override_args['vocab_size']
+                config_args["vocab_size"] = override_args["vocab_size"]
             model = EvolvableGPT(**config_args)
             sd_hf = torch.load(custom_sd)
             config = GPT2Config(**config_args)
             model_hf = GPT2LMHeadModel(config)
-            sd_hf = {k.split("model.")[-1]: v for k,v in sd_hf.items()}
+            sd_hf = {k.split("model.")[-1]: v for k, v in sd_hf.items()}
             model_hf.load_state_dict(sd_hf)
-        else:         
+        else:
             # create a from-scratch initialized Evolvable GPT model
             model = EvolvableGPT(**config_args)
             # init a huggingface/transformers model
-            model_hf = GPT2LMHeadModel.from_pretrained(model_type)       
-            sd_hf = model_hf.state_dict()      
+            model_hf = GPT2LMHeadModel.from_pretrained(model_type)
+            sd_hf = model_hf.state_dict()
 
         sd = model.state_dict()
         sd_keys = sd.keys()
         # discard this mask / buffer, not a param
-        sd_keys = [k for k in sd_keys if not k.endswith('.attn.bias')]  
+        sd_keys = [k for k in sd_keys if not k.endswith(".attn.bias")]
 
         # copy while ensuring all of the parameters are aligned and match in names
         # and shapes
         sd_keys_hf = sd_hf.keys()
-        sd_keys_hf = [k for k in sd_keys_hf if not k.endswith(
-            '.attn.masked_bias')]  # ignore these, just a buffer
-        sd_keys_hf = [k for k in sd_keys_hf if not k.endswith(
-            '.attn.bias')]  # same, just the mask (buffer)
-        transposed = ['attn.c_attn.weight', 'attn.c_proj.weight',
-                      'mlp.c_fc.weight', 'mlp.c_proj.weight']
+        sd_keys_hf = [
+            k for k in sd_keys_hf if not k.endswith(".attn.masked_bias")
+        ]  # ignore these, just a buffer
+        sd_keys_hf = [
+            k for k in sd_keys_hf if not k.endswith(".attn.bias")
+        ]  # same, just the mask (buffer)
+        transposed = [
+            "attn.c_attn.weight",
+            "attn.c_proj.weight",
+            "mlp.c_fc.weight",
+            "mlp.c_proj.weight",
+        ]
         # basically the openai checkpoints use a "Conv1D" module, but we only want to use a vanilla Linear
         # this means that we have to transpose these weights when we import them
         assert len(sd_keys_hf) == len(
-            sd_keys), f"mismatched keys: {len(sd_keys_hf)} != {len(sd_keys)}"
+            sd_keys
+        ), f"mismatched keys: {len(sd_keys_hf)} != {len(sd_keys)}"
         for khf, k in zip(sd_keys_hf, sd_keys):
             if any(khf.endswith(w) for w in transposed):
                 # special treatment for the Conv1D weights we need to transpose
                 assert sd_hf[khf].shape[::-1] == sd[k].shape
                 with torch.no_grad():
                     sd[k].copy_(sd_hf[khf].t())
             else:
@@ -316,75 +348,90 @@
         We are then returning the PyTorch optimizer object.
         """
 
         # separate out all parameters to those that will and won't experience
         # regularizing weight decay
         decay = set()
         no_decay = set()
-        whitelist_weight_modules = (torch.nn.Linear, )
-        blacklist_weight_modules = (
-            torch.nn.LayerNorm, LayerNorm, torch.nn.Embedding)
+        whitelist_weight_modules = (torch.nn.Linear,)
+        blacklist_weight_modules = (torch.nn.LayerNorm, LayerNorm, torch.nn.Embedding)
         for mn, m in self.named_modules():
             for pn, p in m.named_parameters():
-                fpn = '%s.%s' % (mn, pn) if mn else pn  # full param name
+                fpn = f"{mn}.{pn}" if mn else pn  # full param name
                 # random note: because named_modules and named_parameters are recursive
                 # we will see the same tensors p many many times. but doing it this way
                 # allows us to know which parent module any tensor p belongs to...
-                if pn.endswith('bias'):
+                if pn.endswith("bias"):
                     # all biases will not be decayed
                     no_decay.add(fpn)
-                elif pn.endswith('weight') and isinstance(m, whitelist_weight_modules):
+                elif pn.endswith("weight") and isinstance(m, whitelist_weight_modules):
                     # weights of whitelist modules will be weight decayed
                     decay.add(fpn)
-                elif pn.endswith('weight') and isinstance(m, blacklist_weight_modules):
+                elif pn.endswith("weight") and isinstance(m, blacklist_weight_modules):
                     # weights of blacklist modules will NOT be weight decayed
                     no_decay.add(fpn)
 
         # subtle: 'transformer.wte.weight' and 'lm_head.weight' are tied, so they
         # will appear in the no_decay and decay sets respectively after the above.
         # In addition, because named_parameters() doesn't return duplicates, it
-        # will only return the first occurence, key'd by 'transformer.wte.weight', below.
+        # will only return the first occurrence, key'd by 'transformer.wte.weight', below.
         # so let's manually remove 'lm_head.weight' from decay set. This will include
         # this tensor into optimization via transformer.wte.weight only, and not
         # decayed.
-        decay.remove('lm_head.weight')
+        decay.remove("lm_head.weight")
 
         # validate that we considered every parameter
         param_dict = {pn: p for pn, p in self.named_parameters()}
         inter_params = decay & no_decay
         union_params = decay | no_decay
-        assert len(
-            inter_params) == 0, "parameters %s made it into both decay/no_decay sets!" % (str(inter_params), )
-        assert len(
-            param_dict.keys() - union_params) == 0, "parameters %s were not separated into either decay/no_decay set!" \
-            % (str(param_dict.keys() - union_params), )
+        assert (
+            len(inter_params) == 0
+        ), "parameters {} made it into both decay/no_decay sets!".format(
+            str(inter_params)
+        )
+        assert (
+            len(param_dict.keys() - union_params) == 0
+        ), "parameters {} were not separated into either decay/no_decay set!".format(
+            str(param_dict.keys() - union_params),
+        )
 
         # create the pytorch optimizer object
         optim_groups = [
-            {"params": [param_dict[pn] for pn in sorted(
-                list(decay))], "weight_decay": weight_decay},
-            {"params": [param_dict[pn]
-                        for pn in sorted(list(no_decay))], "weight_decay": 0.0},
+            {
+                "params": [param_dict[pn] for pn in sorted(list(decay))],
+                "weight_decay": weight_decay,
+            },
+            {
+                "params": [param_dict[pn] for pn in sorted(list(no_decay))],
+                "weight_decay": 0.0,
+            },
         ]
         # new PyTorch nightly has a new 'fused' option for AdamW that is much faster
-        use_fused = (device_type == 'cuda') and (
-            'fused' in inspect.signature(torch.optim.AdamW).parameters)
+        use_fused = (device_type == "cuda") and (
+            "fused" in inspect.signature(torch.optim.AdamW).parameters
+        )
         print(f"using fused AdamW: {use_fused}")
         extra_args = dict(fused=True) if use_fused else dict()
         optimizer = torch.optim.AdamW(
-            optim_groups, lr=learning_rate, betas=betas, **extra_args)
+            optim_groups, lr=learning_rate, betas=betas, **extra_args
+        )
 
         return optimizer
 
     def estimate_mfu(self, fwdbwd_per_iter, dt):
-        """ estimate model flops utilization (MFU) in units of A100 bfloat16 peak FLOPS """
+        """estimate model flops utilization (MFU) in units of A100 bfloat16 peak FLOPS"""
         # first estimate the number of flops we do per iteration.
         # see PaLM paper Appendix B as ref: https://arxiv.org/abs/2204.02311
         N = self.get_num_params()
-        L, H, Q, T = self.n_layer, self.n_head, self.n_embd // self.n_head, self.block_size
+        L, H, Q, T = (
+            self.n_layer,
+            self.n_head,
+            self.n_embd // self.n_head,
+            self.block_size,
+        )
         flops_per_token = 6 * N + 12 * L * H * Q * T
         flops_per_fwdbwd = flops_per_token * T
         flops_per_iter = flops_per_fwdbwd * fwdbwd_per_iter
         # express our flops throughput as ratio of A100 bfloat16 peak flops
         flops_achieved = flops_per_iter * (1.0 / dt)  # per second
         flops_promised = 312e12  # A100 GPU bfloat16 peak flops is 312 TFLOPS
         mfu = flops_achieved / flops_promised
@@ -395,137 +442,137 @@
         """
         Take a conditioning sequence of indices idx (LongTensor of shape (b,t)) and complete
         the sequence max_new_tokens times, feeding the predictions back into the model each time.
         Most likely you'll want to make sure to be in model.eval() mode of operation for this.
         """
         for _ in range(max_new_tokens):
             # if the sequence context is growing too long we must crop it at block_size
-            idx_cond = idx if idx.size(
-                1) <= self.block_size else idx[:, -self.block_size:]
+            idx_cond = (
+                idx if idx.size(1) <= self.block_size else idx[:, -self.block_size :]
+            )
             # forward the model to get the logits for the index in the sequence
             logits, _ = self(idx_cond)
             # pluck the logits at the final step and scale by desired temperature
             logits = logits[:, -1, :] / temperature
             # optionally crop the logits to only the top k options
             if top_k is not None:
                 v, _ = torch.topk(logits, min(top_k, logits.size(-1)))
-                logits[logits < v[:, [-1]]] = -float('Inf')
+                logits[logits < v[:, [-1]]] = -float("Inf")
             # apply softmax to convert logits to (normalized) probabilities
             probs = F.softmax(logits, dim=-1)
             # sample from the distribution
             idx_next = torch.multinomial(probs, num_samples=1)
             # append sampled index to the running sequence and continue
             idx = torch.cat((idx, idx_next), dim=1)
 
         return idx
 
     def get_model_dict(self):
-        """Returns dictionary with model information and weights.
-        """
+        """Returns dictionary with model information and weights."""
         model_dict = self.init_dict
         model_dict.update(
-            {'stored_values': self.extract_parameters(without_layer_norm=False)})
+            {"stored_values": self.extract_parameters(without_layer_norm=False)}
+        )
         return model_dict
 
     def count_parameters(self, without_layer_norm=False):
         """Returns number of parameters in neural network.
 
         :param without_layer_norm: Exclude normalization layers, defaults to False
         :type without_layer_norm: bool, optional
         """
         count = 0
         for name, param in self.named_parameters():
-            if not without_layer_norm or 'layer_norm' not in name:
+            if not without_layer_norm or "layer_norm" not in name:
                 count += param.data.cpu().numpy().flatten().shape[0]
         return count
 
     def extract_grad(self, without_layer_norm=False):
         """Returns current pytorch gradient in same order as genome's flattened parameter vector.
 
         :param without_layer_norm: Exclude normalization layers, defaults to False
         :type without_layer_norm: bool, optional
         """
         tot_size = self.count_parameters(without_layer_norm)
         pvec = np.zeros(tot_size, np.float32)
         count = 0
         for name, param in self.named_parameters():
-            if not without_layer_norm or 'layer_norm' not in name:
+            if not without_layer_norm or "layer_norm" not in name:
                 sz = param.grad.data.cpu().numpy().flatten().shape[0]
-                pvec[count:count + sz] = param.grad.data.cpu().numpy().flatten()
+                pvec[count : count + sz] = param.grad.data.cpu().numpy().flatten()
                 count += sz
         return pvec.copy()
 
     def extract_parameters(self, without_layer_norm=False):
         """Returns current flattened neural network weights.
 
         :param without_layer_norm: Exclude normalization layers, defaults to False
         :type without_layer_norm: bool, optional
         """
         tot_size = self.count_parameters(without_layer_norm)
         pvec = np.zeros(tot_size, np.float32)
         count = 0
         for name, param in self.named_parameters():
-            if not without_layer_norm or 'layer_norm' not in name:
+            if not without_layer_norm or "layer_norm" not in name:
                 sz = param.data.cpu().detach().numpy().flatten().shape[0]
-                pvec[count:count + sz] = param.data.cpu().detach().numpy().flatten()
+                pvec[count : count + sz] = param.data.cpu().detach().numpy().flatten()
                 count += sz
         return copy.deepcopy(pvec)
 
     def inject_parameters(self, pvec, without_layer_norm=False):
         """Injects a flat vector of neural network parameters into the model's current neural network weights.
 
         :param pvec: Network weights
         :type pvec: np.array()
         :param without_layer_norm: Exclude normalization layers, defaults to False
         :type without_layer_norm: bool, optional
         """
         count = 0
 
         for name, param in self.named_parameters():
-            if not without_layer_norm or 'layer_norm' not in name:
+            if not without_layer_norm or "layer_norm" not in name:
                 sz = param.data.cpu().numpy().flatten().shape[0]
-                raw = pvec[count:count + sz]
+                raw = pvec[count : count + sz]
                 reshaped = raw.reshape(param.data.cpu().numpy().shape)
-                param.data = torch.from_numpy(
-                    copy.deepcopy(reshaped)).type(torch.FloatTensor)
+                param.data = torch.from_numpy(copy.deepcopy(reshaped)).type(
+                    torch.FloatTensor
+                )
                 count += sz
         return pvec
 
     @property
     def init_dict(self):
-        """Returns model information in dictionary.
-        """
+        """Returns model information in dictionary."""
         init_dict = {
             "n_layer": self.n_layer,
             "vocab_size": self.vocab_size,
             "n_embd": self.n_embd,
             "n_head": self.n_head,
             "dim_feedfwd": self.dim_feedfwd,
             "block_size": self.block_size,
             "dropout": self.dropout,
             "activation": self.activation,
             "layer_norm_eps": self.layer_norm_eps,
             "min_layers": self.min_layers,
             "max_layers": self.max_layers,
             "bias": self.bias,
-            "device": self.device}
+            "device": self.device,
+        }
         return init_dict
 
     def add_layer(self):
-        """Adds a block layer to transformer.
-        """
+        """Adds a block layer to transformer."""
         if self.n_layer < self.max_layers:
             self.n_layer += 1
             self.recreate_nets()
         # else:
         #     self.add_nodes()
 
     def remove_layer(self):
-        """Removes a block layer from transformer.
-        """
+        """Removes a block layer from transformer."""
         if self.n_layer > self.min_layers:
             self.n_layer -= 1
             self.recreate_shrunk_nets()
         # else:
         #     self.add_nodes()
 
     def add_node(self, numb_new_nodes=None):
@@ -549,30 +596,29 @@
         if numb_new_nodes is None:
             numb_new_nodes = np.random.choice([32, 64, 128], 1)[0]
         self.dim_feedfwd -= numb_new_nodes
         self.recreate_shrunk_nets()
         return {"numb_new_nodes": numb_new_nodes}
 
     def recreate_nets(self):
-        """Recreates neural network.
-        """
+        """Recreates neural network."""
         new_transformer = self.create_net()
         self.transformer = self.preserve_parameters(
-            old_net=self.transformer, new_net=new_transformer)
+            old_net=self.transformer, new_net=new_transformer
+        )
 
     def recreate_shrunk_nets(self):
-        """Recreates shrunk neural network.
-        """
+        """Recreates shrunk neural network."""
         new_transformer = self.create_net()
         self.transformer = self.shrink_preserve_parameters(
-            old_net=self.transformer, new_net=new_transformer)
+            old_net=self.transformer, new_net=new_transformer
+        )
 
     def clone(self):
-        """Returns clone of neural net with identical parameters.
-        """
+        """Returns clone of neural net with identical parameters."""
         clone = EvolvableGPT(**copy.deepcopy(self.init_dict))
         clone.load_state_dict(self.state_dict())
         return clone
 
     def preserve_parameters(self, old_net, new_net):
         """Returns new neural network with copied parameters from old network.
 
@@ -588,27 +634,25 @@
                 if old_net_dict[key].data.size() == param.data.size():
                     param.data = old_net_dict[key].data
                 else:
                     if "norm" not in key:
                         old_size = old_net_dict[key].data.size()
                         new_size = param.data.size()
                         if len(param.data.size()) == 1:
-                            param.data[:min(old_size[0], new_size[0])] = old_net_dict[key].data[
-                                :min(old_size[0], new_size[0])]
+                            param.data[: min(old_size[0], new_size[0])] = old_net_dict[
+                                key
+                            ].data[: min(old_size[0], new_size[0])]
                         else:
-                            param.data[:min(old_size[0], new_size[0]), :min(old_size[1], new_size[1])] = old_net_dict[
-                                key].data[
-                                :min(old_size[
-                                    0],
-                                    new_size[
-                                    0]),
-                                :min(old_size[
-                                    1],
-                                    new_size[
-                                    1])]
+                            param.data[
+                                : min(old_size[0], new_size[0]),
+                                : min(old_size[1], new_size[1]),
+                            ] = old_net_dict[key].data[
+                                : min(old_size[0], new_size[0]),
+                                : min(old_size[1], new_size[1]),
+                            ]
 
         return new_net
 
     def shrink_preserve_parameters(self, old_net, new_net):
         """Returns shrunk new neural network with copied parameters from old network.
 
         :param old_net: Old neural network
@@ -627,54 +671,57 @@
                         old_size = old_net_dict[key].data.size()
                         new_size = param.data.size()
                         min_0 = min(old_size[0], new_size[0])
                         if len(param.data.size()) == 1:
                             param.data[:min_0] = old_net_dict[key].data[:min_0]
                         else:
                             min_1 = min(old_size[1], new_size[1])
-                            param.data[:min_0,
-                                       :min_1] = old_net_dict[key].data[:min_0, :min_1]
+                            param.data[:min_0, :min_1] = old_net_dict[key].data[
+                                :min_0, :min_1
+                            ]
         return new_net
 
 
-def _canonical_mask(mask, mask_name, other_type, other_name,
-                    target_type, check_other=True):
+def _canonical_mask(
+    mask, mask_name, other_type, other_name, target_type, check_other=True
+):
     """Returns canconical mask. Adapted from torch.nn.functional"""
     if mask is not None:
         _mask_dtype = mask.dtype
         _mask_is_float = torch.is_floating_point(mask)
         if _mask_dtype != torch.bool and not _mask_is_float:
             raise AssertionError(
-                f"only bool and floating types of {mask_name} are supported")
+                f"only bool and floating types of {mask_name} are supported"
+            )
         if check_other and other_type is not None:
             if _mask_dtype != other_type:
                 warnings.warn(
                     f"Support for mismatched {mask_name} and {other_name} "
                     "is deprecated. Use same type for both instead."
                 )
         if not _mask_is_float:
-            mask = (
-                torch.zeros_like(mask, dtype=target_type)
-                .masked_fill_(mask, float("-inf"))
+            mask = torch.zeros_like(mask, dtype=target_type).masked_fill_(
+                mask, float("-inf")
             )
     return mask
 
 
 class LayerNorm(nn.Module):
-    """ LayerNorm but with an optional bias. PyTorch doesn't support simply bias=False """
+    """LayerNorm but with an optional bias. PyTorch doesn't support simply bias=False"""
 
     def __init__(self, ndim, bias, layer_norm_eps=1e-5):
         super().__init__()
         self.weight = nn.Parameter(torch.ones(ndim))
         self.bias = nn.Parameter(torch.zeros(ndim)) if bias else None
         self.layer_norm_eps = layer_norm_eps
 
     def forward(self, input):
-        return F.layer_norm(input, self.weight.shape, self.weight,
-                            self.bias, self.layer_norm_eps)
+        return F.layer_norm(
+            input, self.weight.shape, self.weight, self.bias, self.layer_norm_eps
+        )
 
 
 class CausalSelfAttention(nn.Module):
     def __init__(self, n_embd, n_head, bias, dropout, block_size):
         super().__init__()
         assert n_embd % n_head == 0
         # key, query, value projections for all heads, but in a batch
@@ -685,92 +732,121 @@
         self.attn_dropout = nn.Dropout(dropout)
         self.resid_dropout = nn.Dropout(dropout)
         self.n_head = n_head
         self.n_embd = n_embd
         self.dropout = dropout
         self.bias = bias
         # flash attention make GPU go brrrrr but support is only in PyTorch >= 2.0
-        self.flash = hasattr(torch.nn.functional,
-                             'scaled_dot_product_attention')
+        self.flash = hasattr(torch.nn.functional, "scaled_dot_product_attention")
         if not self.flash:
             print(
-                "WARNING: using slow attention. Flash Attention requires PyTorch >= 2.0")
+                "WARNING: using slow attention. Flash Attention requires PyTorch >= 2.0"
+            )
             # causal mask to ensure that attention is only applied to the left in the
             # input sequence
-            self.register_buffer("bias", torch.tril(torch.ones(block_size, block_size))
-                                 .view(1, 1, block_size, block_size))
+            self.register_buffer(
+                "bias",
+                torch.tril(torch.ones(block_size, block_size)).view(
+                    1, 1, block_size, block_size
+                ),
+            )
 
     def forward(self, x, attn_mask=None, layer_past=None, is_causal=True):
-        B, T, C = x.size()  # batch size, sequence length, embedding dimensionality (n_embd)
+        (
+            B,
+            T,
+            C,
+        ) = x.size()  # batch size, sequence length, embedding dimensionality (n_embd)
 
         # calculate query, key, values for all heads in batch and move head
         # forward to be the batch dim
         q, k, v = self.c_attn(x).split(self.n_embd, dim=2)
-        k = k.view(B, T, self.n_head, C //
-                   self.n_head).transpose(1, 2)  # (B, nh, T, hs)
-        q = q.view(B, T, self.n_head, C //
-                   self.n_head).transpose(1, 2)  # (B, nh, T, hs)
-        v = v.view(B, T, self.n_head, C //
-                   self.n_head).transpose(1, 2)  # (B, nh, T, hs)
+        k = k.view(B, T, self.n_head, C // self.n_head).transpose(
+            1, 2
+        )  # (B, nh, T, hs)
+        q = q.view(B, T, self.n_head, C // self.n_head).transpose(
+            1, 2
+        )  # (B, nh, T, hs)
+        v = v.view(B, T, self.n_head, C // self.n_head).transpose(
+            1, 2
+        )  # (B, nh, T, hs)
 
         if layer_past is not None:
             past_key, past_value = layer_past
             k = torch.cat((past_key, k), dim=-2)
             v = torch.cat((past_value, v), dim=-2)
-            
+
         present = (k, v)
 
         # causal self-attention; Self-attend: (B, nh, T, hs) x (B, nh, hs, T) ->
         # (B, nh, T, T)
         if self.flash:
             # efficient attention using Flash Attention CUDA kernels
             y = torch.nn.functional.scaled_dot_product_attention(
                 q,
                 k,
                 v,
                 attn_mask=attn_mask,
                 dropout_p=self.dropout if self.training else 0,
-                is_causal=is_causal)
+                is_causal=is_causal,
+            )
         else:
             # manual implementation of attention
             att = (q @ k.transpose(-2, -1)) * (1.0 / math.sqrt(k.size(-1)))
-            att = att.masked_fill(self.bias[:, :, :T, :T] == 0, float('-inf'))
+            att = att.masked_fill(self.bias[:, :, :T, :T] == 0, float("-inf"))
             att = F.softmax(att, dim=-1)
             att = self.attn_dropout(att)
             y = att @ v  # (B, nh, T, T) x (B, nh, T, hs) -> (B, nh, T, hs)
         # re-assemble all head outputs side by side
         y = y.transpose(1, 2).contiguous().view(B, T, C)
 
         # output projection
         y = self.resid_dropout(self.c_proj(y))
 
         return y, present
 
 
 class Block(nn.Module):
-    def __init__(self, n_embd, n_head, bias, dropout, block_size,
-                 hidden_size, activation='gelu', layer_norm_eps=1e-5):
+    def __init__(
+        self,
+        n_embd,
+        n_head,
+        bias,
+        dropout,
+        block_size,
+        hidden_size,
+        activation="gelu",
+        layer_norm_eps=1e-5,
+    ):
         super().__init__()
         self.ln_1 = LayerNorm(n_embd, bias=bias, layer_norm_eps=layer_norm_eps)
-        self.attn = CausalSelfAttention(
-            n_embd, n_head, bias, dropout, block_size)
+        self.attn = CausalSelfAttention(n_embd, n_head, bias, dropout, block_size)
         self.ln_2 = LayerNorm(n_embd, bias=bias, layer_norm_eps=layer_norm_eps)
         self.mlp = MLP(n_embd, dropout, hidden_size, activation)
 
     def forward(self, x, attn_mask=None, layer_past=None, is_causal=True):
-        attn_output, present = self.attn(self.ln_1(x), attn_mask=attn_mask, layer_past=layer_past, is_causal=is_causal)
+        attn_output, present = self.attn(
+            self.ln_1(x),
+            attn_mask=attn_mask,
+            layer_past=layer_past,
+            is_causal=is_causal,
+        )
         x = x + attn_output
         x = x + self.mlp(self.ln_2(x))
         return x, present
 
 
 class MLP(EvolvableMLP):
-    def __init__(self, n_embd, dropout, hidden_size, activation='gelu'):
-        super().__init__(num_inputs=n_embd, num_outputs=n_embd,
-                         hidden_size=[hidden_size], activation=activation)
+    def __init__(self, n_embd, dropout, hidden_size, activation="gelu"):
+        super().__init__(
+            num_inputs=n_embd,
+            num_outputs=n_embd,
+            hidden_size=[hidden_size],
+            activation=activation,
+        )
         self.dropout = nn.Dropout(dropout)
 
     def forward(self, x):
         """Returns output of neural network.
 
         :param x: Neural network input
         :type x: torch.Tensor() or np.array
@@ -785,44 +861,55 @@
     def get_activation(self, activation_names):
         """Returns activation function for corresponding activation name.
 
         :param activation_names: Activation function name
         :type activation_names: str
         """
         activation_functions = {
-            'tanh': nn.Tanh,
-            'linear': nn.Identity,
-            'relu': nn.ReLU,
-            'elu': nn.ELU,
-            'softsign': nn.Softsign,
-            'sigmoid': nn.Sigmoid,
-            'softplus': nn.Softplus,
-            'lrelu': nn.LeakyReLU,
-            'prelu': nn.PReLU,
-            'gelu': new_gelu}
+            "tanh": nn.Tanh,
+            "linear": nn.Identity,
+            "relu": nn.ReLU,
+            "elu": nn.ELU,
+            "softsign": nn.Softsign,
+            "sigmoid": nn.Sigmoid,
+            "softplus": nn.Softplus,
+            "lrelu": nn.LeakyReLU,
+            "prelu": nn.PReLU,
+            "gelu": new_gelu,
+        }
 
         return activation_functions[activation_names]()
 
 
 class new_gelu(nn.Module):
     """
     Implementation of the GELU activation function currently in Google BERT repo (identical to OpenAI GPT).
     Reference: Gaussian Error Linear Units (GELU) paper: https://arxiv.org/abs/1606.08415
     """
+
     def forward(self, x):
-        return 0.5 * x * (1.0 + torch.tanh(math.sqrt(2.0 / math.pi)
-                      * (x + 0.044715 * torch.pow(x, 3.0))))
+        return (
+            0.5
+            * x
+            * (
+                1.0
+                + torch.tanh(
+                    math.sqrt(2.0 / math.pi) * (x + 0.044715 * torch.pow(x, 3.0))
+                )
+            )
+        )
 
 
 class PositionalEncoding(nn.Module):
-    """The positional embedding class. 
-    Converts tensor of input indices into corresponding tensor of position embeddings."""
+    """The positional embedding class.
+    Converts tensor of input indices into corresponding tensor of position embeddings.
+    """
 
     def __init__(self, max_positions: int, emb_size):
-        super(PositionalEncoding, self).__init__()
+        super().__init__()
         self.embedding = nn.Embedding(max_positions, emb_size)
         self.emb_size = emb_size
 
     def forward(self, tokens: torch.Tensor):
         """Forward pass through position embedding module.
         :param tokens: Tokens to embed
         :type tokens: torch.Tensor
@@ -830,15 +917,15 @@
         return self.embedding(tokens)
 
 
 class TokenEmbedding(nn.Module):
     """The token embedding class. Converts tensor of input indices into corresponding tensor of token embeddings."""
 
     def __init__(self, vocab_size: int, emb_size):
-        super(TokenEmbedding, self).__init__()
+        super().__init__()
         self.embedding = nn.Embedding(vocab_size, emb_size)
         self.emb_size = emb_size
 
     def forward(self, tokens: torch.Tensor):
         """Forward pass through token embedding module.
         :param tokens: Tokens to embed
         :type tokens: torch.Tensor
@@ -852,9 +939,8 @@
     :param input: Input to return dtype of
     :type input: Any
     """
     if input is None:
         return None
     elif isinstance(input, torch.Tensor):
         return input.dtype
-    raise RuntimeError(
-        "input to _none_or_dtype() must be None or torch.Tensor")
+    raise RuntimeError("input to _none_or_dtype() must be None or torch.Tensor")
```

### Comparing `agilerl-0.1.8/agilerl/networks/evolvable_mlp.py` & `agilerl-0.1.9/agilerl/networks/evolvable_mlp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,383 +1,385 @@
-import copy
-from collections import OrderedDict
-from typing import List
-
-import numpy as np
-import torch
-import torch.nn as nn
-
-
-class EvolvableMLP(nn.Module):
-    """The Evolvable Multi-layer Perceptron class.
-
-    :param num_inputs: Input layer dimension
-    :type num_inputs: int
-    :param num_outputs: Output layer dimension
-    :type num_outputs: int
-    :param hidden_size: Hidden layer(s) size
-    :type hidden_size: List[int]
-    :param activation: Activation layer, defaults to 'relu'
-    :type activation: str, optional
-    :param output_activation: Output activation layer, defaults to None
-    :type output_activation: str, optional
-    :param layer_norm: Normalization between layers, defaults to False
-    :type layer_norm: bool, optional
-    :param output_vanish: Vanish output by multiplying by 0.1, defaults to True
-    :type output_vanish: bool, optional
-    :param stored_values: Stored network weights, defaults to None
-    :type stored_values: numpy.array(), optional
-    :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
-    :type device: str, optional
-    :param accelerator: Accelerator for distributed computing, defaults to None
-    :type accelerator: Hugging Face accelerate.Accelerator(), optional
-    """
-
-    def __init__(
-            self,
-            num_inputs: int,
-            num_outputs: int,
-            hidden_size: List[int],
-            activation='relu',
-            output_activation=None,
-            layer_norm=False,
-            output_vanish=True,
-            stored_values=None,
-            device='cpu',
-            accelerator=None):
-        super(EvolvableMLP, self).__init__()
-
-        self.num_inputs = num_inputs
-        self.num_outputs = num_outputs
-        self.activation = activation
-        self.output_activation = output_activation
-        self.layer_norm = layer_norm
-        self.output_vanish = output_vanish
-        self.hidden_size = hidden_size
-        self.device = device
-        self.accelerator = accelerator
-
-        self.net = self.create_net()
-
-        if stored_values is not None:
-            self.inject_parameters(
-                pvec=stored_values, without_layer_norm=False)
-
-    def get_activation(self, activation_names):
-        """Returns activation function for corresponding activation name.
-
-        :param activation_names: Activation function name
-        :type activation_names: str
-        """
-        activation_functions = {
-            'tanh': nn.Tanh,
-            'linear': nn.Identity,
-            'relu': nn.ReLU,
-            'elu': nn.ELU,
-            'softsign': nn.Softsign,
-            'sigmoid': nn.Sigmoid,
-            'softplus': nn.Softplus,
-            'softmax': nn.Softmax,
-            'lrelu': nn.LeakyReLU,
-            'prelu': nn.PReLU,
-            'gelu': nn.GELU}
-
-        return activation_functions[activation_names](dim=1) if activation_names == 'softmax' else activation_functions[activation_names]()
-
-    def create_net(self):
-        """Creates and returns neural network.
-        """
-        net_dict = OrderedDict()
-
-        net_dict["linear_layer_0"] = nn.Linear(
-            self.num_inputs, self.hidden_size[0])
-        if self.layer_norm:
-            net_dict["layer_norm_0"] = nn.LayerNorm(self.hidden_size[0])
-        net_dict["activation_0"] = self.get_activation(self.activation)
-
-        if len(self.hidden_size) > 1:
-            for l_no in range(1, len(self.hidden_size)):
-                net_dict[f"linear_layer_{str(l_no)}"] = nn.Linear(
-                    self.hidden_size[l_no - 1], self.hidden_size[l_no])
-                if self.layer_norm:
-                    net_dict[f"layer_norm_{str(l_no)}"] = nn.LayerNorm(
-                        self.hidden_size[l_no])
-                net_dict[f"activation_{str(l_no)}"] = self.get_activation(
-                    self.activation)
-
-        output_layer = nn.Linear(self.hidden_size[-1], self.num_outputs)
-
-        if self.output_vanish:
-            output_layer.weight.data.mul_(0.1)
-            output_layer.bias.data.mul_(0.1)
-
-        net_dict["linear_layer_output"] = output_layer
-        if self.output_activation is not None:
-            net_dict["activation_output"] = self.get_activation(
-                self.output_activation)
-            
-        net = nn.Sequential(net_dict)
-            
-        if self.accelerator is None:
-            net = net.to(self.device)
-
-        return net
-
-    def forward(self, x):
-        """Returns output of neural network.
-
-        :param x: Neural network input
-        :type x: torch.Tensor() or np.array
-        """
-        if not isinstance(x, torch.Tensor):
-            x = torch.FloatTensor(np.array(x))
-            if self.accelerator is None:
-                x = x.to(self.device)
-        x = self.net(x)
-        return x
-
-    def get_model_dict(self):
-        """Returns dictionary with model information and weights.
-        """
-        model_dict = self.init_dict
-        model_dict.update(
-            {'stored_values': self.extract_parameters(without_layer_norm=False)})
-        return model_dict
-
-    def count_parameters(self, without_layer_norm=False):
-        """Returns number of parameters in neural network.
-
-        :param without_layer_norm: Exclude normalization layers, defaults to False
-        :type without_layer_norm: bool, optional
-        """
-        count = 0
-        for name, param in self.named_parameters():
-            if not without_layer_norm or 'layer_norm' not in name:
-                count += param.data.cpu().numpy().flatten().shape[0]
-        return count
-
-    def extract_grad(self, without_layer_norm=False):
-        """Returns current pytorch gradient in same order as genome's flattened 
-        parameter vector.
-
-        :param without_layer_norm: Exclude normalization layers, defaults to False
-        :type without_layer_norm: bool, optional
-        """
-        tot_size = self.count_parameters(without_layer_norm)
-        pvec = np.zeros(tot_size, np.float32)
-        count = 0
-        for name, param in self.named_parameters():
-            if not without_layer_norm or 'layer_norm' not in name:
-                sz = param.grad.data.cpu().numpy().flatten().shape[0]
-                pvec[count:count + sz] = param.grad.data.cpu().numpy().flatten()
-                count += sz
-        return pvec.copy()
-
-    def extract_parameters(self, without_layer_norm=False):
-        """Returns current flattened neural network weights.
-
-        :param without_layer_norm: Exclude normalization layers, defaults to False
-        :type without_layer_norm: bool, optional
-        """
-        tot_size = self.count_parameters(without_layer_norm)
-        pvec = np.zeros(tot_size, np.float32)
-        count = 0
-        for name, param in self.named_parameters():
-            if not without_layer_norm or 'layer_norm' not in name:
-                sz = param.data.cpu().detach().numpy().flatten().shape[0]
-                pvec[count:count + sz] = param.data.cpu().detach().numpy().flatten()
-                count += sz
-        return copy.deepcopy(pvec)
-
-    def inject_parameters(self, pvec, without_layer_norm=False):
-        """Injects a flat vector of neural network parameters into the model's current 
-        neural network weights.
-
-        :param pvec: Network weights
-        :type pvec: np.array()
-        :param without_layer_norm: Exclude normalization layers, defaults to False
-        :type without_layer_norm: bool, optional
-        """
-        count = 0
-
-        for name, param in self.named_parameters():
-            if not without_layer_norm or 'layer_norm' not in name:
-                sz = param.data.cpu().numpy().flatten().shape[0]
-                raw = pvec[count:count + sz]
-                reshaped = raw.reshape(param.data.cpu().numpy().shape)
-                param.data = torch.from_numpy(
-                    copy.deepcopy(reshaped)).type(torch.FloatTensor)
-                count += sz
-        return pvec
-
-    @property
-    def init_dict(self):
-        """Returns model information in dictionary.
-        """
-        init_dict = {
-            "num_inputs": self.num_inputs,
-            "num_outputs": self.num_outputs,
-            "hidden_size": self.hidden_size,
-            "activation": self.activation,
-            "output_activation": self.output_activation,
-            "layer_norm": self.layer_norm,
-            "device": self.device,
-            "accelerator":self.accelerator}
-        return init_dict
-
-    @property
-    def short_dict(self):
-        """Returns shortened version of model information in dictionary.
-        """
-        short_dict = {
-            "hidden_size": self.hidden_size,
-            "activation": self.activation,
-            "output_activation": self.output_activation,
-            "layer_norm": self.layer_norm}
-        return short_dict
-
-    def add_layer(self):
-        """Adds a hidden layer to neural network.
-        """
-        # add layer to hyper params
-        if len(self.hidden_size) < 3:  # HARD LIMIT
-            self.hidden_size += [self.hidden_size[-1]]
-
-            # copy old params to new net
-            new_net = self.create_net()
-            new_net = self.preserve_parameters(
-                old_net=self.net, new_net=new_net)
-            self.net = new_net
-        else:
-            self.add_node()
-
-    def remove_layer(self):
-        """Removes a hidden layer from neural network.
-        """
-        if len(self.hidden_size) > 1:  # HARD LIMIT
-            self.hidden_size = self.hidden_size[:1]
-            new_net = self.create_net()
-            new_net = self.shrink_preserve_parameters(
-                old_net=self.net, new_net=new_net)
-            self.net = new_net
-        else:
-            self.add_node()
-
-    def add_node(self, hidden_layer=None, numb_new_nodes=None):
-        """Adds nodes to hidden layer of neural network.
-
-        :param hidden_layer: Depth of hidden layer to add nodes to, defaults to None
-        :type hidden_layer: int, optional
-        :param numb_new_nodes: Number of nodes to add to hidden layer, defaults to None
-        :type numb_new_nodes: int, optional
-        """
-        if hidden_layer is None:
-            hidden_layer = np.random.randint(0, len(self.hidden_size), 1)[0]
-        else:
-            hidden_layer = min(hidden_layer, len(self.hidden_size) - 1)
-        if numb_new_nodes is None:
-            numb_new_nodes = np.random.choice([16, 32, 64], 1)[0]
-
-        if self.hidden_size[hidden_layer] + numb_new_nodes <= 500:  # HARD LIMIT
-            self.hidden_size[hidden_layer] += numb_new_nodes
-            new_net = self.create_net()
-            new_net = self.preserve_parameters(
-                old_net=self.net, new_net=new_net)
-
-            self.net = new_net
-
-        return {"hidden_layer": hidden_layer, "numb_new_nodes": numb_new_nodes}
-
-    def remove_node(self, hidden_layer=None, numb_new_nodes=None):
-        """Removes nodes from hidden layer of neural network.
-
-        :param hidden_layer: Depth of hidden layer to remove nodes from, defaults to None
-        :type hidden_layer: int, optional
-        :param numb_new_nodes: Number of nodes to remove from hidden layer, defaults to None
-        :type numb_new_nodes: int, optional
-        """
-        if hidden_layer is None:
-            hidden_layer = np.random.randint(0, len(self.hidden_size), 1)[0]
-        else:
-            hidden_layer = min(hidden_layer, len(self.hidden_size) - 1)
-        if numb_new_nodes is None:
-            numb_new_nodes = np.random.choice([16, 32, 64], 1)[0]
-
-        if self.hidden_size[hidden_layer] - numb_new_nodes > 64:  # HARD LIMIT
-            self.hidden_size[hidden_layer] = self.hidden_size[hidden_layer] - \
-                numb_new_nodes
-            new_net = self.create_net()
-            new_net = self.shrink_preserve_parameters(
-                old_net=self.net, new_net=new_net)
-
-            self.net = new_net
-
-        return {"hidden_layer": hidden_layer, "numb_new_nodes": numb_new_nodes}
-
-    def clone(self):
-        """Returns clone of neural net with identical parameters.
-        """
-        clone = EvolvableMLP(**copy.deepcopy(self.init_dict))
-        clone.load_state_dict(self.state_dict())
-        return clone
-
-    def preserve_parameters(self, old_net, new_net):
-        """Returns new neural network with copied parameters from old network.
-
-        :param old_net: Old neural network
-        :type old_net: nn.Module()
-        :param new_net: New neural network
-        :type new_net: nn.Module()
-        """
-        old_net_dict = dict(old_net.named_parameters())
-
-        for key, param in new_net.named_parameters():
-            if key in old_net_dict.keys():
-                if old_net_dict[key].data.size() == param.data.size():
-                    param.data = old_net_dict[key].data
-                else:
-                    if "norm" not in key:
-                        old_size = old_net_dict[key].data.size()
-                        new_size = param.data.size()
-                        if len(param.data.size()) == 1:
-                            param.data[:min(old_size[0], new_size[0])] = old_net_dict[key].data[
-                                :min(old_size[0], new_size[0])]
-                        else:
-                            param.data[:min(old_size[0], new_size[0]), :min(old_size[1], new_size[1])] = old_net_dict[
-                                key].data[
-                                :min(old_size[
-                                    0],
-                                    new_size[
-                                    0]),
-                                :min(old_size[
-                                    1],
-                                    new_size[
-                                    1])]
-
-        return new_net
-
-    def shrink_preserve_parameters(self, old_net, new_net):
-        """Returns shrunk new neural network with copied parameters from old network.
-
-        :param old_net: Old neural network
-        :type old_net: nn.Module()
-        :param new_net: New neural network
-        :type new_net: nn.Module()
-        """
-        old_net_dict = dict(old_net.named_parameters())
-
-        for key, param in new_net.named_parameters():
-            if key in old_net_dict.keys():
-                if old_net_dict[key].data.size() == param.data.size():
-                    param.data = old_net_dict[key].data
-                else:
-                    if "norm" not in key:
-                        old_size = old_net_dict[key].data.size()
-                        new_size = param.data.size()
-                        min_0 = min(old_size[0], new_size[0])
-                        if len(param.data.size()) == 1:
-                            param.data[:min_0] = old_net_dict[key].data[:min_0]
-                        else:
-                            min_1 = min(old_size[1], new_size[1])
-                            param.data[:min_0,
-                                       :min_1] = old_net_dict[key].data[:min_0, :min_1]
-        return new_net
+import copy
+from collections import OrderedDict
+from typing import List
+
+import numpy as np
+import torch
+import torch.nn as nn
+
+from agilerl.networks.custom_architecture import GumbelSoftmax
+
+
+class EvolvableMLP(nn.Module):
+    """The Evolvable Multi-layer Perceptron class.
+
+    :param num_inputs: Input layer dimension
+    :type num_inputs: int
+    :param num_outputs: Output layer dimension
+    :type num_outputs: int
+    :param hidden_size: Hidden layer(s) size
+    :type hidden_size: List[int]
+    :param activation: Activation layer, defaults to 'relu'
+    :type activation: str, optional
+    :param output_activation: Output activation layer, defaults to None
+    :type output_activation: str, optional
+    :param layer_norm: Normalization between layers, defaults to False
+    :type layer_norm: bool, optional
+    :param output_vanish: Vanish output by multiplying by 0.1, defaults to True
+    :type output_vanish: bool, optional
+    :param stored_values: Stored network weights, defaults to None
+    :type stored_values: numpy.array(), optional
+    :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
+    :type device: str, optional
+    :param accelerator: Accelerator for distributed computing, defaults to None
+    :type accelerator: Hugging Face accelerate.Accelerator(), optional
+    """
+
+    def __init__(
+        self,
+        num_inputs: int,
+        num_outputs: int,
+        hidden_size: List[int],
+        activation="relu",
+        output_activation=None,
+        layer_norm=False,
+        output_vanish=True,
+        stored_values=None,
+        device="cpu",
+        accelerator=None,
+    ):
+        super().__init__()
+
+        self.num_inputs = num_inputs
+        self.num_outputs = num_outputs
+        self.activation = activation
+        self.output_activation = output_activation
+        self.layer_norm = layer_norm
+        self.output_vanish = output_vanish
+        self.hidden_size = hidden_size
+        self.device = device
+        self.accelerator = accelerator
+
+        self.net = self.create_net()
+
+        if stored_values is not None:
+            self.inject_parameters(pvec=stored_values, without_layer_norm=False)
+
+    def get_activation(self, activation_names):
+        """Returns activation function for corresponding activation name.
+
+        :param activation_names: Activation function name
+        :type activation_names: str
+        """
+        activation_functions = {
+            "tanh": nn.Tanh,
+            "linear": nn.Identity,
+            "relu": nn.ReLU,
+            "elu": nn.ELU,
+            "softsign": nn.Softsign,
+            "sigmoid": nn.Sigmoid,
+            "gumbel_softmax": GumbelSoftmax,
+            "softplus": nn.Softplus,
+            "softmax": nn.Softmax,
+            "lrelu": nn.LeakyReLU,
+            "prelu": nn.PReLU,
+            "gelu": nn.GELU,
+        }
+
+        return (
+            activation_functions[activation_names](dim=1)
+            if activation_names == "softmax"
+            else activation_functions[activation_names]()
+        )
+
+    def create_net(self):
+        """Creates and returns neural network."""
+        net_dict = OrderedDict()
+
+        net_dict["linear_layer_0"] = nn.Linear(self.num_inputs, self.hidden_size[0])
+        if self.layer_norm:
+            net_dict["layer_norm_0"] = nn.LayerNorm(self.hidden_size[0])
+        net_dict["activation_0"] = self.get_activation(self.activation)
+
+        if len(self.hidden_size) > 1:
+            for l_no in range(1, len(self.hidden_size)):
+                net_dict[f"linear_layer_{str(l_no)}"] = nn.Linear(
+                    self.hidden_size[l_no - 1], self.hidden_size[l_no]
+                )
+                if self.layer_norm:
+                    net_dict[f"layer_norm_{str(l_no)}"] = nn.LayerNorm(
+                        self.hidden_size[l_no]
+                    )
+                net_dict[f"activation_{str(l_no)}"] = self.get_activation(
+                    self.activation
+                )
+
+        output_layer = nn.Linear(self.hidden_size[-1], self.num_outputs)
+
+        if self.output_vanish:
+            output_layer.weight.data.mul_(0.1)
+            output_layer.bias.data.mul_(0.1)
+
+        net_dict["linear_layer_output"] = output_layer
+        if self.output_activation is not None:
+            net_dict["activation_output"] = self.get_activation(self.output_activation)
+
+        net = nn.Sequential(net_dict)
+
+        if self.accelerator is None:
+            net = net.to(self.device)
+
+        return net
+
+    def forward(self, x):
+        """Returns output of neural network.
+
+        :param x: Neural network input
+        :type x: torch.Tensor() or np.array
+        """
+        if not isinstance(x, torch.Tensor):
+            x = torch.FloatTensor(np.array(x))
+            if self.accelerator is None:
+                x = x.to(self.device)
+        x = self.net(x)
+        return x
+
+    def get_model_dict(self):
+        """Returns dictionary with model information and weights."""
+        model_dict = self.init_dict
+        model_dict.update(
+            {"stored_values": self.extract_parameters(without_layer_norm=False)}
+        )
+        return model_dict
+
+    def count_parameters(self, without_layer_norm=False):
+        """Returns number of parameters in neural network.
+
+        :param without_layer_norm: Exclude normalization layers, defaults to False
+        :type without_layer_norm: bool, optional
+        """
+        count = 0
+        for name, param in self.named_parameters():
+            if not without_layer_norm or "layer_norm" not in name:
+                count += param.data.cpu().numpy().flatten().shape[0]
+        return count
+
+    def extract_grad(self, without_layer_norm=False):
+        """Returns current pytorch gradient in same order as genome's flattened
+        parameter vector.
+
+        :param without_layer_norm: Exclude normalization layers, defaults to False
+        :type without_layer_norm: bool, optional
+        """
+        tot_size = self.count_parameters(without_layer_norm)
+        pvec = np.zeros(tot_size, np.float32)
+        count = 0
+        for name, param in self.named_parameters():
+            if not without_layer_norm or "layer_norm" not in name:
+                sz = param.grad.data.cpu().numpy().flatten().shape[0]
+                pvec[count : count + sz] = param.grad.data.cpu().numpy().flatten()
+                count += sz
+        return pvec.copy()
+
+    def extract_parameters(self, without_layer_norm=False):
+        """Returns current flattened neural network weights.
+
+        :param without_layer_norm: Exclude normalization layers, defaults to False
+        :type without_layer_norm: bool, optional
+        """
+        tot_size = self.count_parameters(without_layer_norm)
+        pvec = np.zeros(tot_size, np.float32)
+        count = 0
+        for name, param in self.named_parameters():
+            if not without_layer_norm or "layer_norm" not in name:
+                sz = param.data.cpu().detach().numpy().flatten().shape[0]
+                pvec[count : count + sz] = param.data.cpu().detach().numpy().flatten()
+                count += sz
+        return copy.deepcopy(pvec)
+
+    def inject_parameters(self, pvec, without_layer_norm=False):
+        """Injects a flat vector of neural network parameters into the model's current
+        neural network weights.
+
+        :param pvec: Network weights
+        :type pvec: np.array()
+        :param without_layer_norm: Exclude normalization layers, defaults to False
+        :type without_layer_norm: bool, optional
+        """
+        count = 0
+
+        for name, param in self.named_parameters():
+            if not without_layer_norm or "layer_norm" not in name:
+                sz = param.data.cpu().numpy().flatten().shape[0]
+                raw = pvec[count : count + sz]
+                reshaped = raw.reshape(param.data.cpu().numpy().shape)
+                param.data = torch.from_numpy(copy.deepcopy(reshaped)).type(
+                    torch.FloatTensor
+                )
+                count += sz
+        return pvec
+
+    @property
+    def init_dict(self):
+        """Returns model information in dictionary."""
+        init_dict = {
+            "num_inputs": self.num_inputs,
+            "num_outputs": self.num_outputs,
+            "hidden_size": self.hidden_size,
+            "activation": self.activation,
+            "output_activation": self.output_activation,
+            "layer_norm": self.layer_norm,
+            "device": self.device,
+            "accelerator": self.accelerator,
+        }
+        return init_dict
+
+    @property
+    def short_dict(self):
+        """Returns shortened version of model information in dictionary."""
+        short_dict = {
+            "hidden_size": self.hidden_size,
+            "activation": self.activation,
+            "output_activation": self.output_activation,
+            "layer_norm": self.layer_norm,
+        }
+        return short_dict
+
+    def add_layer(self):
+        """Adds a hidden layer to neural network."""
+        # add layer to hyper params
+        if len(self.hidden_size) < 3:  # HARD LIMIT
+            self.hidden_size += [self.hidden_size[-1]]
+
+            # copy old params to new net
+            new_net = self.create_net()
+            new_net = self.preserve_parameters(old_net=self.net, new_net=new_net)
+            self.net = new_net
+        else:
+            self.add_node()
+
+    def remove_layer(self):
+        """Removes a hidden layer from neural network."""
+        if len(self.hidden_size) > 1:  # HARD LIMIT
+            self.hidden_size = self.hidden_size[:1]
+            new_net = self.create_net()
+            new_net = self.shrink_preserve_parameters(old_net=self.net, new_net=new_net)
+            self.net = new_net
+        else:
+            self.add_node()
+
+    def add_node(self, hidden_layer=None, numb_new_nodes=None):
+        """Adds nodes to hidden layer of neural network.
+
+        :param hidden_layer: Depth of hidden layer to add nodes to, defaults to None
+        :type hidden_layer: int, optional
+        :param numb_new_nodes: Number of nodes to add to hidden layer, defaults to None
+        :type numb_new_nodes: int, optional
+        """
+        if hidden_layer is None:
+            hidden_layer = np.random.randint(0, len(self.hidden_size), 1)[0]
+        else:
+            hidden_layer = min(hidden_layer, len(self.hidden_size) - 1)
+        if numb_new_nodes is None:
+            numb_new_nodes = np.random.choice([16, 32, 64], 1)[0]
+
+        if self.hidden_size[hidden_layer] + numb_new_nodes <= 500:  # HARD LIMIT
+            self.hidden_size[hidden_layer] += numb_new_nodes
+            new_net = self.create_net()
+            new_net = self.preserve_parameters(old_net=self.net, new_net=new_net)
+
+            self.net = new_net
+
+        return {"hidden_layer": hidden_layer, "numb_new_nodes": numb_new_nodes}
+
+    def remove_node(self, hidden_layer=None, numb_new_nodes=None):
+        """Removes nodes from hidden layer of neural network.
+
+        :param hidden_layer: Depth of hidden layer to remove nodes from, defaults to None
+        :type hidden_layer: int, optional
+        :param numb_new_nodes: Number of nodes to remove from hidden layer, defaults to None
+        :type numb_new_nodes: int, optional
+        """
+        if hidden_layer is None:
+            hidden_layer = np.random.randint(0, len(self.hidden_size), 1)[0]
+        else:
+            hidden_layer = min(hidden_layer, len(self.hidden_size) - 1)
+        if numb_new_nodes is None:
+            numb_new_nodes = np.random.choice([16, 32, 64], 1)[0]
+
+        if self.hidden_size[hidden_layer] - numb_new_nodes > 64:  # HARD LIMIT
+            self.hidden_size[hidden_layer] = (
+                self.hidden_size[hidden_layer] - numb_new_nodes
+            )
+            new_net = self.create_net()
+            new_net = self.shrink_preserve_parameters(old_net=self.net, new_net=new_net)
+
+            self.net = new_net
+
+        return {"hidden_layer": hidden_layer, "numb_new_nodes": numb_new_nodes}
+
+    def clone(self):
+        """Returns clone of neural net with identical parameters."""
+        clone = EvolvableMLP(**copy.deepcopy(self.init_dict))
+        clone.load_state_dict(self.state_dict())
+        return clone
+
+    def preserve_parameters(self, old_net, new_net):
+        """Returns new neural network with copied parameters from old network.
+
+        :param old_net: Old neural network
+        :type old_net: nn.Module()
+        :param new_net: New neural network
+        :type new_net: nn.Module()
+        """
+        old_net_dict = dict(old_net.named_parameters())
+
+        for key, param in new_net.named_parameters():
+            if key in old_net_dict.keys():
+                if old_net_dict[key].data.size() == param.data.size():
+                    param.data = old_net_dict[key].data
+                else:
+                    if "norm" not in key:
+                        old_size = old_net_dict[key].data.size()
+                        new_size = param.data.size()
+                        if len(param.data.size()) == 1:
+                            param.data[: min(old_size[0], new_size[0])] = old_net_dict[
+                                key
+                            ].data[: min(old_size[0], new_size[0])]
+                        else:
+                            param.data[
+                                : min(old_size[0], new_size[0]),
+                                : min(old_size[1], new_size[1]),
+                            ] = old_net_dict[key].data[
+                                : min(old_size[0], new_size[0]),
+                                : min(old_size[1], new_size[1]),
+                            ]
+
+        return new_net
+
+    def shrink_preserve_parameters(self, old_net, new_net):
+        """Returns shrunk new neural network with copied parameters from old network.
+
+        :param old_net: Old neural network
+        :type old_net: nn.Module()
+        :param new_net: New neural network
+        :type new_net: nn.Module()
+        """
+        old_net_dict = dict(old_net.named_parameters())
+
+        for key, param in new_net.named_parameters():
+            if key in old_net_dict.keys():
+                if old_net_dict[key].data.size() == param.data.size():
+                    param.data = old_net_dict[key].data
+                else:
+                    if "norm" not in key:
+                        old_size = old_net_dict[key].data.size()
+                        new_size = param.data.size()
+                        min_0 = min(old_size[0], new_size[0])
+                        if len(param.data.size()) == 1:
+                            param.data[:min_0] = old_net_dict[key].data[:min_0]
+                        else:
+                            min_1 = min(old_size[1], new_size[1])
+                            param.data[:min_0, :min_1] = old_net_dict[key].data[
+                                :min_0, :min_1
+                            ]
+        return new_net
```

### Comparing `agilerl-0.1.8/agilerl/training/train.py` & `agilerl-0.1.9/agilerl/training/train.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,297 +1,351 @@
-import numpy as np
-import os
-from tqdm import trange
-import wandb
-from datetime import datetime
-from torch.utils.data import DataLoader
-from agilerl.components.replay_data import ReplayDataset
-from agilerl.components.sampler import Sampler
-
-
-def train(env, env_name, algo, pop, memory, INIT_HP, MUT_P, swap_channels=False, n_episodes=2000, 
-          max_steps=500, evo_epochs=5, evo_loop=1, eps_start=1.0, eps_end=0.1, 
-          eps_decay=0.995, target=200., tournament=None, mutation=None, checkpoint=None, 
-          checkpoint_path=None, wb=False, accelerator=None):
-    """The general online RL training function. Returns trained population of agents 
-    and their fitnesses.
-
-    :param env: The environment to train in. Can be vectorized.
-    :type env: Gym-style environment
-    :param env_name: Environment name
-    :type env_name: str
-    :param algo: RL algorithm name
-    :type algo: str
-    :param pop: Population of agents
-    :type pop: List[object]
-    :param memory: Experience Replay Buffer
-    :type memory: object
-    :param swap_channels: Swap image channels dimension from last to first [H, W, C] -> [C, H, W], defaults to False
-    :type swap_channels: bool, optional
-    :param n_episodes: Maximum number of training episodes, defaults to 2000
-    :type n_episodes: int, optional
-    :param max_steps: Maximum number of steps in environment per episode, defaults to 500
-    :type max_steps: int, optional
-    :param evo_epochs: Evolution frequency (episodes), defaults to 5
-    :type evo_epochs: int, optional
-    :param evo_loop: Number of evaluation episodes, defaults to 1
-    :type evo_loop: int, optional
-    :param eps_start: Maximum exploration - initial epsilon value, defaults to 1.0
-    :type eps_start: float, optional
-    :param eps_end: Minimum exploration - final epsilon value, defaults to 0.1
-    :type eps_end: float, optional
-    :param eps_decay: Epsilon decay per episode, defaults to 0.995
-    :type eps_decay: float, optional
-    :param target: Target score for early stopping, defaults to 200.
-    :type target: float, optional
-    :param tournament: Tournament selection object, defaults to None
-    :type tournament: object, optional
-    :param mutation: Mutation object, defaults to None
-    :type mutation: object, optional
-    :param checkpoint: Checkpoint frequency (episodes), defaults to None
-    :type checkpoint: int, optional
-    :param checkpoint_path: Location to save checkpoint, defaults to None
-    :type checkpoint_path: str, optional
-    :param wb: Weights & Biases tracking, defaults to False
-    :type wb: bool, optional
-    :param accelerator: Accelerator for distributed computing, defaults to None
-    :type accelerator: Hugging Face accelerate.Accelerator(), optional
-    """
-    if wb:
-        if accelerator is not None:
-            accelerator.wait_for_everyone()
-            if accelerator.is_main_process:
-                wandb.init(
-                    # set the wandb project where this run will be logged
-                    project="AgileRL",
-                    name="{}-EvoHPO-{}-{}".format(env_name, algo,
-                                                datetime.now().strftime("%m%d%Y%H%M%S")),
-                    # track hyperparameters and run metadata
-                    config={
-                        "algo": "Evo HPO {}".format(algo),
-                        "env": env_name,
-                        "batch_size" : INIT_HP['BATCH_SIZE'],
-                        "lr" : INIT_HP['LR'],
-                        "gamma": INIT_HP['GAMMA'],
-                        "memory_size" : INIT_HP['MEMORY_SIZE'],
-                        "learn_step" : INIT_HP['LEARN_STEP'],
-                        "tau" : INIT_HP['TAU'],
-                        "pop_size" : INIT_HP['TOURN_SIZE'],
-                        "no_mut" : MUT_P['NO_MUT'],
-                        "arch_mut" :  MUT_P['ARCH_MUT'],
-                        "params_mut" : MUT_P['PARAMS_MUT'],
-                        "act_mut" : MUT_P['ACT_MUT'],
-                        "rl_hp_mut" : MUT_P['RL_HP_MUT']}
-                )
-            accelerator.wait_for_everyone()
-        else:
-            wandb.init(
-                    # set the wandb project where this run will be logged
-                    project="AgileRL",
-                    name="{}-EvoHPO-{}-{}".format(env_name, algo,
-                                                datetime.now().strftime("%m%d%Y%H%M%S")),
-                    # track hyperparameters and run metadata
-                    config={
-                        "algo": "Evo HPO {}".format(algo),
-                        "env": env_name,
-                        "batch_size" : INIT_HP['BATCH_SIZE'],
-                        "lr" : INIT_HP['LR'],
-                        "gamma": INIT_HP['GAMMA'],
-                        "memory_size" : INIT_HP['MEMORY_SIZE'],
-                        "learn_step" : INIT_HP['LEARN_STEP'],
-                        "tau" : INIT_HP['TAU'],
-                        "pop_size" : INIT_HP['TOURN_SIZE'],
-                        "no_mut" : MUT_P['NO_MUT'],
-                        "arch_mut" :  MUT_P['ARCH_MUT'],
-                        "params_mut" : MUT_P['PARAMS_MUT'],
-                        "act_mut" : MUT_P['ACT_MUT'],
-                        "rl_hp_mut" : MUT_P['RL_HP_MUT']}
-                )
-
-    if accelerator is not None:
-        accel_temp_models_path = 'models/{}'.format(env_name)
-        if accelerator.is_main_process:
-            if not os.path.exists(accel_temp_models_path):
-                os.makedirs(accel_temp_models_path)
-
-    save_path = checkpoint_path.split('.pt')[0] if checkpoint_path is not None else "{}-EvoHPO-{}-{}".format(
-        env_name, algo, datetime.now().strftime("%m%d%Y%H%M%S"))
-    
-    if accelerator is not None:
-        # Create dataloader from replay buffer
-        replay_dataset = ReplayDataset(memory, pop[0].batch_size)
-        replay_dataloader = DataLoader(replay_dataset, batch_size=None)
-        replay_dataloader = accelerator.prepare(replay_dataloader)
-        sampler = Sampler(distributed=True, 
-                          dataset=replay_dataset, 
-                          dataloader=replay_dataloader)
-    else:
-        sampler = Sampler(distributed=False, memory=memory)
-
-    epsilon = eps_start
-
-    if accelerator is not None:
-        print(f'\nDistributed training on {accelerator.device}...')
-    else:
-        print('\nTraining...')
-
-    bar_format = '{l_bar}{bar:10}| {n:4}/{total_fmt} [{elapsed:>7}<{remaining:>7}, {rate_fmt}{postfix}]'
-    if accelerator is not None:
-        pbar = trange(n_episodes, unit="ep", bar_format=bar_format, ascii=True, 
-                      disable=not accelerator.is_local_main_process)
-    else:
-        pbar = trange(n_episodes, unit="ep", bar_format=bar_format, ascii=True)
-
-    pop_fitnesses = []
-    total_steps = 0
-
-    # Pre-training mutation
-    if mutation is not None:
-        pop = mutation.mutation(pop, pre_training_mut=True)
-
-    # RL training loop
-    for idx_epi in pbar:
-        if accelerator is not None:
-            accelerator.wait_for_everyone()   
-        for agent in pop:   # Loop through population            
-            state = env.reset()[0]  # Reset environment at start of episode
-            score = 0
-            for idx_step in range(max_steps):
-                if swap_channels:
-                    state = np.moveaxis(state, [3], [1])
-                # Get next action from agent
-                action = agent.getAction(state, epsilon)
-                next_state, reward, done, _, _ = env.step(action)   # Act in environment
-
-                # Save experience to replay buffer
-                if swap_channels:
-                    memory.save2memoryVectEnvs(
-                        state, action, reward, np.moveaxis(next_state, [3], [1]), done)
-                else:
-                    memory.save2memoryVectEnvs(
-                        state, action, reward, next_state, done)
-
-                # Learn according to learning frequency
-                if memory.counter % agent.learn_step == 0 and len(
-                        memory) >= agent.batch_size:
-                    # Sample replay buffer
-                    experiences = sampler.sample(agent.batch_size)
-                    # Learn according to agent's RL algorithm
-                    agent.learn(experiences)
-
-                state = next_state
-                score += reward
-
-            agent.scores.append(score)
-
-            agent.steps[-1] += max_steps
-            total_steps += max_steps
-
-        # Update epsilon for exploration
-        epsilon = max(eps_end, epsilon * eps_decay)
-
-        # Now evolve if necessary
-        if (idx_epi + 1) % evo_epochs == 0:
-            
-            # Evaluate population
-            fitnesses = [
-                agent.test(
-                    env,
-                    swap_channels=swap_channels,
-                    max_steps=max_steps,
-                    loop=evo_loop) for agent in pop]
-            pop_fitnesses.append(fitnesses)
-
-            mean_scores = np.mean([agent.scores[-20:] for agent in pop], axis=1)
-
-            if wb:
-                if accelerator is not None:
-                    accelerator.wait_for_everyone()
-                    if accelerator.is_main_process:
-                        wandb.log({"global_step": total_steps*accelerator.state.num_processes,
-                                "eval/mean_score": np.mean(mean_scores),
-                                "eval/mean_reward": np.mean(fitnesses),
-                                "eval/best_fitness": np.max(fitnesses)})
-                    accelerator.wait_for_everyone()
-                else:
-                    wandb.log({"global_step": total_steps,
-                                "eval/mean_score": np.mean(mean_scores),
-                                "eval/mean_reward": np.mean(fitnesses),
-                                "eval/best_fitness": np.max(fitnesses)})
-
-            # Update step counter
-            for agent in pop:
-                agent.steps.append(agent.steps[-1])
-
-            fitness = ["%.2f"%fitness for fitness in fitnesses]
-            avg_fitness = ["%.2f"%np.mean(agent.fitness[-100:]) for agent in pop]
-            avg_score = ["%.2f"%np.mean(agent.scores[-100:]) for agent in pop]
-            agents = [agent.index for agent in pop]
-            num_steps = [agent.steps[-1] for agent in pop]
-            muts = [agent.mut for agent in pop]
-            perf_info = f'Fitness: {fitness}, 100 fitness avgs: {avg_fitness}, 100 score avgs: {avg_score}'
-            pop_info = f'Agents: {agents}, Steps: {num_steps}, Mutations: {muts}' 
-            pbar_string = perf_info + ', ' + pop_info
-            pbar.set_postfix_str(pbar_string)
-            pbar.update(0)
-
-            # Early stop if consistently reaches target
-            if np.all(np.greater([np.mean(agent.fitness[-100:])
-                      for agent in pop], target)) and idx_epi >= 100:
-                if wb:
-                    wandb.finish()
-                return pop, pop_fitnesses
-
-            # Tournament selection and population mutation
-            if tournament and mutation is not None:
-                if accelerator is not None:
-                    accelerator.wait_for_everyone()
-                    for model in pop:
-                        model.unwrap_models()
-                    accelerator.wait_for_everyone()
-                    if accelerator.is_main_process:
-                        elite, pop = tournament.select(pop)
-                        pop = mutation.mutation(pop)
-                        for pop_i, model in enumerate(pop):
-                            model.saveCheckpoint(f'{accel_temp_models_path}/{algo}_{pop_i}.pt')
-                    accelerator.wait_for_everyone()
-                    if not accelerator.is_main_process:
-                        for pop_i, model in enumerate(pop):
-                            model.loadCheckpoint(f'{accel_temp_models_path}/{algo}_{pop_i}.pt')
-                    accelerator.wait_for_everyone()
-                    for model in pop:
-                        model.wrap_models()
-                else:
-                    elite, pop = tournament.select(pop)
-                    pop = mutation.mutation(pop)
-                    
-        # Save model checkpoint
-        if checkpoint is not None:
-            if (idx_epi + 1) % checkpoint == 0:
-                if accelerator is not None:
-                    accelerator.wait_for_everyone()
-                    for model in pop:
-                        model.unwrap_models()
-                    accelerator.wait_for_everyone()
-                    if accelerator.is_main_process:
-                        for i, agent in enumerate(pop):
-                            agent.saveCheckpoint(f'{save_path}_{i}_{idx_epi+1}.pt')
-                        print('Saved checkpoint.')
-                    accelerator.wait_for_everyone()
-                    for model in pop:
-                        model.wrap_models()
-                    accelerator.wait_for_everyone()
-                else:
-                    for i, agent in enumerate(pop):
-                        agent.saveCheckpoint(f'{save_path}_{i}_{idx_epi+1}.pt')
-                    print('Saved checkpoint.')
-
-    if wb:
-        if accelerator is not None:
-            accelerator.wait_for_everyone()
-            if accelerator.is_main_process:
-                wandb.finish()
-            accelerator.wait_for_everyone()
-        else:
-            wandb.finish()
-
-    return pop, pop_fitnesses
+import os
+from datetime import datetime
+
+import numpy as np
+from torch.utils.data import DataLoader
+from tqdm import trange
+
+import wandb
+from agilerl.components.replay_data import ReplayDataset
+from agilerl.components.sampler import Sampler
+
+
+def train(
+    env,
+    env_name,
+    algo,
+    pop,
+    memory,
+    INIT_HP,
+    MUT_P,
+    swap_channels=False,
+    n_episodes=2000,
+    max_steps=500,
+    evo_epochs=5,
+    evo_loop=1,
+    eps_start=1.0,
+    eps_end=0.1,
+    eps_decay=0.995,
+    target=200.0,
+    tournament=None,
+    mutation=None,
+    checkpoint=None,
+    checkpoint_path=None,
+    wb=False,
+    accelerator=None,
+):
+    """The general online RL training function. Returns trained population of agents
+    and their fitnesses.
+
+    :param env: The environment to train in. Can be vectorized.
+    :type env: Gym-style environment
+    :param env_name: Environment name
+    :type env_name: str
+    :param algo: RL algorithm name
+    :type algo: str
+    :param pop: Population of agents
+    :type pop: List[object]
+    :param memory: Experience Replay Buffer
+    :type memory: object
+    :param swap_channels: Swap image channels dimension from last to first [H, W, C] -> [C, H, W], defaults to False
+    :type swap_channels: bool, optional
+    :param n_episodes: Maximum number of training episodes, defaults to 2000
+    :type n_episodes: int, optional
+    :param max_steps: Maximum number of steps in environment per episode, defaults to 500
+    :type max_steps: int, optional
+    :param evo_epochs: Evolution frequency (episodes), defaults to 5
+    :type evo_epochs: int, optional
+    :param evo_loop: Number of evaluation episodes, defaults to 1
+    :type evo_loop: int, optional
+    :param eps_start: Maximum exploration - initial epsilon value, defaults to 1.0
+    :type eps_start: float, optional
+    :param eps_end: Minimum exploration - final epsilon value, defaults to 0.1
+    :type eps_end: float, optional
+    :param eps_decay: Epsilon decay per episode, defaults to 0.995
+    :type eps_decay: float, optional
+    :param target: Target score for early stopping, defaults to 200.
+    :type target: float, optional
+    :param tournament: Tournament selection object, defaults to None
+    :type tournament: object, optional
+    :param mutation: Mutation object, defaults to None
+    :type mutation: object, optional
+    :param checkpoint: Checkpoint frequency (episodes), defaults to None
+    :type checkpoint: int, optional
+    :param checkpoint_path: Location to save checkpoint, defaults to None
+    :type checkpoint_path: str, optional
+    :param wb: Weights & Biases tracking, defaults to False
+    :type wb: bool, optional
+    :param accelerator: Accelerator for distributed computing, defaults to None
+    :type accelerator: Hugging Face accelerate.Accelerator(), optional
+    """
+    if wb:
+        if accelerator is not None:
+            accelerator.wait_for_everyone()
+            if accelerator.is_main_process:
+                wandb.init(
+                    # set the wandb project where this run will be logged
+                    project="AgileRL",
+                    name="{}-EvoHPO-{}-{}".format(
+                        env_name, algo, datetime.now().strftime("%m%d%Y%H%M%S")
+                    ),
+                    # track hyperparameters and run metadata
+                    config={
+                        "algo": f"Evo HPO {algo}",
+                        "env": env_name,
+                        "batch_size": INIT_HP["BATCH_SIZE"],
+                        "lr": INIT_HP["LR"],
+                        "gamma": INIT_HP["GAMMA"],
+                        "memory_size": INIT_HP["MEMORY_SIZE"],
+                        "learn_step": INIT_HP["LEARN_STEP"],
+                        "tau": INIT_HP["TAU"],
+                        "pop_size": INIT_HP["TOURN_SIZE"],
+                        "no_mut": MUT_P["NO_MUT"],
+                        "arch_mut": MUT_P["ARCH_MUT"],
+                        "params_mut": MUT_P["PARAMS_MUT"],
+                        "act_mut": MUT_P["ACT_MUT"],
+                        "rl_hp_mut": MUT_P["RL_HP_MUT"],
+                    },
+                )
+            accelerator.wait_for_everyone()
+        else:
+            wandb.init(
+                # set the wandb project where this run will be logged
+                project="AgileRL",
+                name="{}-EvoHPO-{}-{}".format(
+                    env_name, algo, datetime.now().strftime("%m%d%Y%H%M%S")
+                ),
+                # track hyperparameters and run metadata
+                config={
+                    "algo": f"Evo HPO {algo}",
+                    "env": env_name,
+                    "batch_size": INIT_HP["BATCH_SIZE"],
+                    "lr": INIT_HP["LR"],
+                    "gamma": INIT_HP["GAMMA"],
+                    "memory_size": INIT_HP["MEMORY_SIZE"],
+                    "learn_step": INIT_HP["LEARN_STEP"],
+                    "tau": INIT_HP["TAU"],
+                    "pop_size": INIT_HP["TOURN_SIZE"],
+                    "no_mut": MUT_P["NO_MUT"],
+                    "arch_mut": MUT_P["ARCH_MUT"],
+                    "params_mut": MUT_P["PARAMS_MUT"],
+                    "act_mut": MUT_P["ACT_MUT"],
+                    "rl_hp_mut": MUT_P["RL_HP_MUT"],
+                },
+            )
+
+    if accelerator is not None:
+        accel_temp_models_path = f"models/{env_name}"
+        if accelerator.is_main_process:
+            if not os.path.exists(accel_temp_models_path):
+                os.makedirs(accel_temp_models_path)
+
+    save_path = (
+        checkpoint_path.split(".pt")[0]
+        if checkpoint_path is not None
+        else "{}-EvoHPO-{}-{}".format(
+            env_name, algo, datetime.now().strftime("%m%d%Y%H%M%S")
+        )
+    )
+
+    if accelerator is not None:
+        # Create dataloader from replay buffer
+        replay_dataset = ReplayDataset(memory, pop[0].batch_size)
+        replay_dataloader = DataLoader(replay_dataset, batch_size=None)
+        replay_dataloader = accelerator.prepare(replay_dataloader)
+        sampler = Sampler(
+            distributed=True, dataset=replay_dataset, dataloader=replay_dataloader
+        )
+    else:
+        sampler = Sampler(distributed=False, memory=memory)
+
+    epsilon = eps_start
+
+    if accelerator is not None:
+        print(f"\nDistributed training on {accelerator.device}...")
+    else:
+        print("\nTraining...")
+
+    bar_format = "{l_bar}{bar:10}| {n:4}/{total_fmt} [{elapsed:>7}<{remaining:>7}, {rate_fmt}{postfix}]"
+    if accelerator is not None:
+        pbar = trange(
+            n_episodes,
+            unit="ep",
+            bar_format=bar_format,
+            ascii=True,
+            disable=not accelerator.is_local_main_process,
+        )
+    else:
+        pbar = trange(n_episodes, unit="ep", bar_format=bar_format, ascii=True)
+
+    pop_fitnesses = []
+    total_steps = 0
+
+    # Pre-training mutation
+    if mutation is not None:
+        pop = mutation.mutation(pop, pre_training_mut=True)
+
+    # RL training loop
+    for idx_epi in pbar:
+        if accelerator is not None:
+            accelerator.wait_for_everyone()
+        for agent in pop:  # Loop through population
+            state = env.reset()[0]  # Reset environment at start of episode
+            score = 0
+            for idx_step in range(max_steps):
+                if swap_channels:
+                    state = np.moveaxis(state, [3], [1])
+                # Get next action from agent
+                action = agent.getAction(state, epsilon)
+                next_state, reward, done, _, _ = env.step(action)  # Act in environment
+
+                # Save experience to replay buffer
+                if swap_channels:
+                    memory.save2memoryVectEnvs(
+                        state, action, reward, np.moveaxis(next_state, [3], [1]), done
+                    )
+                else:
+                    memory.save2memoryVectEnvs(state, action, reward, next_state, done)
+
+                # Learn according to learning frequency
+                if (
+                    memory.counter % agent.learn_step == 0
+                    and len(memory) >= agent.batch_size
+                ):
+                    # Sample replay buffer
+                    experiences = sampler.sample(agent.batch_size)
+                    # Learn according to agent's RL algorithm
+                    agent.learn(experiences)
+
+                state = next_state
+                score += reward
+
+            agent.scores.append(score)
+
+            agent.steps[-1] += max_steps
+            total_steps += max_steps
+
+        # Update epsilon for exploration
+        epsilon = max(eps_end, epsilon * eps_decay)
+
+        # Now evolve if necessary
+        if (idx_epi + 1) % evo_epochs == 0:
+            # Evaluate population
+            fitnesses = [
+                agent.test(
+                    env, swap_channels=swap_channels, max_steps=max_steps, loop=evo_loop
+                )
+                for agent in pop
+            ]
+            pop_fitnesses.append(fitnesses)
+
+            mean_scores = np.mean([agent.scores[-20:] for agent in pop], axis=1)
+
+            if wb:
+                if accelerator is not None:
+                    accelerator.wait_for_everyone()
+                    if accelerator.is_main_process:
+                        wandb.log(
+                            {
+                                "global_step": total_steps
+                                * accelerator.state.num_processes,
+                                "eval/mean_score": np.mean(mean_scores),
+                                "eval/mean_reward": np.mean(fitnesses),
+                                "eval/best_fitness": np.max(fitnesses),
+                            }
+                        )
+                    accelerator.wait_for_everyone()
+                else:
+                    wandb.log(
+                        {
+                            "global_step": total_steps,
+                            "eval/mean_score": np.mean(mean_scores),
+                            "eval/mean_reward": np.mean(fitnesses),
+                            "eval/best_fitness": np.max(fitnesses),
+                        }
+                    )
+
+            # Update step counter
+            for agent in pop:
+                agent.steps.append(agent.steps[-1])
+
+            fitness = ["%.2f" % fitness for fitness in fitnesses]
+            avg_fitness = ["%.2f" % np.mean(agent.fitness[-100:]) for agent in pop]
+            avg_score = ["%.2f" % np.mean(agent.scores[-100:]) for agent in pop]
+            agents = [agent.index for agent in pop]
+            num_steps = [agent.steps[-1] for agent in pop]
+            muts = [agent.mut for agent in pop]
+            perf_info = f"Fitness: {fitness}, 100 fitness avgs: {avg_fitness}, 100 score avgs: {avg_score}"
+            pop_info = f"Agents: {agents}, Steps: {num_steps}, Mutations: {muts}"
+            pbar_string = perf_info + ", " + pop_info
+            pbar.set_postfix_str(pbar_string)
+            pbar.update(0)
+
+            # Early stop if consistently reaches target
+            if (
+                np.all(
+                    np.greater([np.mean(agent.fitness[-100:]) for agent in pop], target)
+                )
+                and idx_epi >= 100
+            ):
+                if wb:
+                    wandb.finish()
+                return pop, pop_fitnesses
+
+            # Tournament selection and population mutation
+            if tournament and mutation is not None:
+                if accelerator is not None:
+                    accelerator.wait_for_everyone()
+                    for model in pop:
+                        model.unwrap_models()
+                    accelerator.wait_for_everyone()
+                    if accelerator.is_main_process:
+                        elite, pop = tournament.select(pop)
+                        pop = mutation.mutation(pop)
+                        for pop_i, model in enumerate(pop):
+                            model.saveCheckpoint(
+                                f"{accel_temp_models_path}/{algo}_{pop_i}.pt"
+                            )
+                    accelerator.wait_for_everyone()
+                    if not accelerator.is_main_process:
+                        for pop_i, model in enumerate(pop):
+                            model.loadCheckpoint(
+                                f"{accel_temp_models_path}/{algo}_{pop_i}.pt"
+                            )
+                    accelerator.wait_for_everyone()
+                    for model in pop:
+                        model.wrap_models()
+                else:
+                    elite, pop = tournament.select(pop)
+                    pop = mutation.mutation(pop)
+
+        # Save model checkpoint
+        if checkpoint is not None:
+            if (idx_epi + 1) % checkpoint == 0:
+                if accelerator is not None:
+                    accelerator.wait_for_everyone()
+                    for model in pop:
+                        model.unwrap_models()
+                    accelerator.wait_for_everyone()
+                    if accelerator.is_main_process:
+                        for i, agent in enumerate(pop):
+                            agent.saveCheckpoint(f"{save_path}_{i}_{idx_epi+1}.pt")
+                        print("Saved checkpoint.")
+                    accelerator.wait_for_everyone()
+                    for model in pop:
+                        model.wrap_models()
+                    accelerator.wait_for_everyone()
+                else:
+                    for i, agent in enumerate(pop):
+                        agent.saveCheckpoint(f"{save_path}_{i}_{idx_epi+1}.pt")
+                    print("Saved checkpoint.")
+
+    if wb:
+        if accelerator is not None:
+            accelerator.wait_for_everyone()
+            if accelerator.is_main_process:
+                wandb.finish()
+            accelerator.wait_for_everyone()
+        else:
+            wandb.finish()
+
+    return pop, pop_fitnesses
```

### Comparing `agilerl-0.1.8/agilerl/training/train_bc_lm.py` & `agilerl-0.1.9/agilerl/training/train_ilql.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,157 +1,224 @@
-
-from accelerate import Accelerator
-from collections import deque
-from functools import partial
 import json
 import os
-from tqdm.auto import tqdm
-import wandb
+from collections import deque
+from functools import partial
+
 import torch
+from accelerate import Accelerator
 from torch.utils.data import DataLoader
 from torch.utils.data.dataset import IterableDataset
+from tqdm import tqdm
+
+import wandb
 from agilerl.data.rl_data import Iterable_RL_Dataset
 from agilerl.data.torch_datasets import GeneralDataset, GeneralIterDataset
+from agilerl.utils.ilql_utils import add_system_configs, convert_path
 from agilerl.utils.load_objects import load_item
 from agilerl.utils.log_utils import DistributeCombineLogs, label_logs
-from agilerl.utils.ilql_utils import add_system_configs, convert_path
 from agilerl.utils.torch_utils import to
 
+
 def train(cfg):
-    print('using config:', cfg)
-    train_cfg = cfg['train']
-    train_cfg['save_checkpoint_dir'] = convert_path(train_cfg['save_checkpoint_dir'])
-    train_cfg['optim_state_path'] = convert_path(train_cfg['optim_state_path'])
-    wandb_cfg = cfg['wandb']
+    """The ILQL training function."""
+    print("using config:", cfg)
+    train_cfg = cfg["train"]
+    train_cfg["save_checkpoint_dir"] = convert_path(train_cfg["save_checkpoint_dir"])
+    train_cfg["optim_state_path"] = convert_path(train_cfg["optim_state_path"])
+    wandb_cfg = cfg["wandb"]
     accelerator = Accelerator()
     system_cfg = add_system_configs(cfg, accelerator)
-    print('using device:', system_cfg['device'])
-    print('num processes:', system_cfg['num_processes'])
-    print('using fp16:', system_cfg['use_fp16'])
-    if not os.path.exists(train_cfg['save_checkpoint_dir']):
-        os.makedirs(train_cfg['save_checkpoint_dir'])
-    with open(os.path.join(train_cfg['save_checkpoint_dir'], 'config.json'), 'w') as f:
+    print("using device:", system_cfg["device"])
+    print("num processes:", system_cfg["num_processes"])
+    print("using fp16:", system_cfg["use_fp16"])
+    if not os.path.exists(train_cfg["save_checkpoint_dir"]):
+        os.makedirs(train_cfg["save_checkpoint_dir"])
+    with open(os.path.join(train_cfg["save_checkpoint_dir"], "config.json"), "w") as f:
         json.dump(cfg, f)
 
-    if wandb_cfg['use_wandb']:
+    if wandb_cfg["use_wandb"]:
         accelerator.wait_for_everyone()
         if accelerator.is_main_process:
-            wandb.init(project=wandb_cfg['wandb_project'], config=cfg)
+            wandb.init(project=wandb_cfg["wandb_project"], config=cfg)
         accelerator.wait_for_everyone()
-    
-    raw_dataset_train = load_item(cfg['train_dataset'], system_cfg['device'])
-    raw_dataset_eval = load_item(cfg['eval_dataset'], system_cfg['device'])
+
+    raw_dataset_train = load_item(cfg["train_dataset"], system_cfg["device"])
+    raw_dataset_eval = load_item(cfg["eval_dataset"], system_cfg["device"])
     if isinstance(raw_dataset_train, Iterable_RL_Dataset):
-        dataset_train = GeneralIterDataset(raw_dataset_train, 'cpu')
+        dataset_train = GeneralIterDataset(raw_dataset_train, "cpu")
     else:
-        dataset_train = GeneralDataset(raw_dataset_train, 'cpu')
+        dataset_train = GeneralDataset(raw_dataset_train, "cpu")
     if isinstance(raw_dataset_eval, Iterable_RL_Dataset):
-        dataset_eval = GeneralIterDataset(raw_dataset_eval, 'cpu')
+        dataset_eval = GeneralIterDataset(raw_dataset_eval, "cpu")
     else:
-        dataset_eval = GeneralDataset(raw_dataset_eval, 'cpu')
-    train_data_loader_kwargs = {'num_workers': train_cfg['dataloader_workers'], 
-                                'batch_size': train_cfg['bsize'], 
-                                'collate_fn': dataset_train.collate}
-    eval_data_loader_kwargs = {'num_workers': train_cfg['dataloader_workers'], 
-                               'batch_size': train_cfg['eval_bsize'], 
-                               'collate_fn': dataset_eval.collate}
+        dataset_eval = GeneralDataset(raw_dataset_eval, "cpu")
+    train_data_loader_kwargs = {
+        "num_workers": train_cfg["dataloader_workers"],
+        "batch_size": cfg["model"]["batch_size"],
+        "collate_fn": dataset_train.collate,
+    }
+    eval_data_loader_kwargs = {
+        "num_workers": train_cfg["dataloader_workers"],
+        "batch_size": train_cfg["eval_bsize"],
+        "collate_fn": dataset_eval.collate,
+    }
     if not isinstance(dataset_train, IterableDataset):
-        train_data_loader_kwargs['shuffle'] = True
+        train_data_loader_kwargs["shuffle"] = True
     if not isinstance(dataset_eval, IterableDataset):
-        eval_data_loader_kwargs['shuffle'] = True
+        eval_data_loader_kwargs["shuffle"] = True
     data_loader = DataLoader(dataset_train, **train_data_loader_kwargs)
     eval_data_loader = DataLoader(dataset_eval, **eval_data_loader_kwargs)
 
     evaluator = None
-    if cfg['evaluator'] is not None:
-        evaluator = load_item(cfg['evaluator'], system_cfg['device'])
+    if cfg["evaluator"] is not None:
+        evaluator = load_item(cfg["evaluator"], system_cfg["device"])
 
-    model = load_item(cfg['model'], system_cfg['device'])
+    model = load_item(cfg["model"], system_cfg["device"])
     model.train()
 
-    if hasattr(model, 'param_groups'):
-        params = [{'params': frozenset().union(*list(map(
-            lambda x: x.parameters(), p))), **f(train_cfg)} for p, f in model.param_groups]
-    else:
-        params = model.parameters()
-    optim = torch.optim.AdamW(params, lr=train_cfg['lr'], weight_decay=train_cfg['weight_decay'])
-    if train_cfg['optim_state_path'] is not None and os.path.exists(train_cfg['optim_state_path']):
+    if hasattr(model, "param_groups"):
+        params = [
+            {
+                "params": frozenset().union(*list(map(lambda x: x.parameters(), p))),
+                **f(train_cfg),
+            }
+            for p, f in model.param_groups
+        ]
+        model.optimizer = torch.optim.AdamW(
+            params, lr=model.lr, weight_decay=model.weight_decay
+        )
+    optim = model.optimizer
+
+    if train_cfg["optim_state_path"] is not None and os.path.exists(
+        train_cfg["optim_state_path"]
+    ):
         print(f'loading optimizer state from: {train_cfg["optim_state_path"]}')
-        optim.load_state_dict(torch.load(train_cfg['optim_state_path'], map_location=system_cfg['device']))
-        print('loaded.')
-    if isinstance(dataset_train, IterableDataset) and isinstance(dataset_eval, IterableDataset):
+        optim.load_state_dict(
+            torch.load(train_cfg["optim_state_path"], map_location=system_cfg["device"])
+        )
+        print("loaded.")
+    if isinstance(dataset_train, IterableDataset) and isinstance(
+        dataset_eval, IterableDataset
+    ):
         model, optim = accelerator.prepare(model, optim)
     elif isinstance(dataset_train, IterableDataset):
-        model, optim, eval_data_loader = accelerator.prepare(model, optim, eval_data_loader)
+        model, optim, eval_data_loader = accelerator.prepare(
+            model, optim, eval_data_loader
+        )
     elif isinstance(dataset_eval, IterableDataset):
         model, optim, data_loader = accelerator.prepare(model, optim, data_loader)
     else:
-        model, optim, data_loader, eval_data_loader = accelerator.prepare(model, optim, data_loader, eval_data_loader)
+        model, optim, data_loader, eval_data_loader = accelerator.prepare(
+            model, optim, data_loader, eval_data_loader
+        )
 
-    train_logs = DistributeCombineLogs(accelerator, use_wandb=wandb_cfg['use_wandb'])
-    eval_logs = DistributeCombineLogs(accelerator, use_wandb=wandb_cfg['use_wandb'])
+    train_logs = DistributeCombineLogs(accelerator, use_wandb=wandb_cfg["use_wandb"])
+    eval_logs = DistributeCombineLogs(accelerator, use_wandb=wandb_cfg["use_wandb"])
     step = 0
-    best_loss = float('inf')
+    best_loss = float("inf")
     saved_checkpoints = deque([])
-    for epoch in tqdm(range(train_cfg['epochs']), disable=not accelerator.is_local_main_process):
+
+    # bar_format = '{l_bar}{bar:10}| {n:4}/{total_fmt} [{elapsed:>7}<{remaining:>7}, {rate_fmt}{postfix}]'
+    # pbar = trange(n_episodes, unit="ep", bar_format=bar_format, ascii=True)
+
+    # RL training loop
+    for epoch in range(train_cfg["epochs"]):
         for items in tqdm(data_loader, disable=not accelerator.is_local_main_process):
-            items = to(items, system_cfg['device'])
-            loss, logs, postproc_fs = accelerator.unwrap_model(model).get_loss(items, **train_cfg['loss'])
-            accelerator.backward(loss / train_cfg['grad_accum_steps'])
+            items = to(items, system_cfg["device"])
+            loss, logs, postproc_fs = accelerator.unwrap_model(model).get_loss(
+                items, **train_cfg["loss"]
+            )
+            accelerator.backward(loss / train_cfg["grad_accum_steps"])
             train_logs.accum_logs(logs)
-            if (step + 1) % train_cfg['grad_accum_steps'] == 0:
+            if (step + 1) % train_cfg["grad_accum_steps"] == 0:
                 optim.step()
                 optim.zero_grad()
-            if (step + 1) % train_cfg['log_every'] == 0:
-                train_logs.log(*postproc_fs, 
-                               partial(label_logs, label='train'), 
-                               iteration=step, epoch=epoch)
-            if (step + 1) % train_cfg['grad_accum_steps'] == 0:
+                if (
+                    train_cfg["loss"]["q_loss_weight"] != 0.0
+                    or train_cfg["loss"]["v_loss_weight"] != 0.0
+                ):
+                    accelerator.unwrap_model(model).softUpdate()
+            if (train_cfg["hard_update_every"] is not None) and (
+                (step + 1) % train_cfg["hard_update_every"] == 0
+            ):
+                accelerator.unwrap_model(model).hardUpdate()
+            if (step + 1) % train_cfg["log_every"] == 0:
+                train_logs.log(
+                    *postproc_fs,
+                    partial(label_logs, label="train"),
+                    iteration=step,
+                    epoch=epoch,
+                )
+            if (step + 1) % train_cfg["grad_accum_steps"] == 0:
                 train_logs.reset_logs()
-            if (step + 1) % train_cfg['eval_every'] == 0:
+            if (step + 1) % train_cfg["eval_every"] == 0:
                 model.eval()
                 eval_logs.reset_logs()
                 with torch.no_grad():
                     for i, eval_items in enumerate(eval_data_loader):
-                        eval_items = to(eval_items, system_cfg['device'])
-                        if i >= train_cfg['eval_batches']:
+                        eval_items = to(eval_items, system_cfg["device"])
+                        if i >= train_cfg["eval_batches"]:
                             break
-                        _, logs, postproc_fs = accelerator.unwrap_model(model).get_loss(eval_items, **train_cfg['loss'])
+                        _, logs, postproc_fs = accelerator.unwrap_model(model).get_loss(
+                            eval_items, **train_cfg["loss"]
+                        )
                         if evaluator is not None:
-                            evaluator_logs = evaluator.evaluate(accelerator.unwrap_model(model), eval_items)
+                            evaluator_logs = evaluator.evaluate(
+                                accelerator.unwrap_model(model), eval_items
+                            )
                             if evaluator_logs is not None:
-                                logs['evaluation'] = evaluator_logs
+                                logs["evaluation"] = evaluator_logs
                         eval_logs.accum_logs(logs)
-                eval_label = 'eval'
-                eval_total_logs = eval_logs.log(*postproc_fs, 
-                                                partial(label_logs, label=eval_label), 
-                                                iteration=step, epoch=epoch)
+                eval_label = "eval"
+                eval_total_logs = eval_logs.log(
+                    *postproc_fs,
+                    partial(label_logs, label=eval_label),
+                    iteration=step,
+                    epoch=epoch,
+                )
                 accelerator.wait_for_everyone()
                 if accelerator.is_main_process:
-                    if eval_total_logs[eval_label]['loss'] < best_loss:
-                        print('new best eval loss! Saving ...')
-                        if not os.path.exists(train_cfg['save_checkpoint_dir']):
-                            os.makedirs(train_cfg['save_checkpoint_dir'])
-                        torch.save(accelerator.unwrap_model(model).state_dict(),
-                                    os.path.join(train_cfg['save_checkpoint_dir'], 'model.pkl'))
-                        torch.save(optim.state_dict(), os.path.join(train_cfg['save_checkpoint_dir'], 'optim.pkl'))
-                        print('saved.')
-                        best_loss = eval_total_logs[eval_label]['loss']
+                    if eval_total_logs[eval_label]["loss"] < best_loss:
+                        print("new best eval loss! Saving ...")
+                        if not os.path.exists(train_cfg["save_checkpoint_dir"]):
+                            os.makedirs(train_cfg["save_checkpoint_dir"])
+                        torch.save(
+                            accelerator.unwrap_model(model).state_dict(),
+                            os.path.join(train_cfg["save_checkpoint_dir"], "model.pkl"),
+                        )
+                        torch.save(
+                            optim.state_dict(),
+                            os.path.join(train_cfg["save_checkpoint_dir"], "optim.pkl"),
+                        )
+                        print("saved.")
+                        best_loss = eval_total_logs[eval_label]["loss"]
                 accelerator.wait_for_everyone()
                 model.train()
-            if train_cfg['save_every'] is not None and (step + 1) % train_cfg['save_every'] == 0:
+            if (
+                train_cfg["save_every"] is not None
+                and (step + 1) % train_cfg["save_every"] == 0
+            ):
                 accelerator.wait_for_everyone()
                 if accelerator.is_main_process:
-                    print('saving checkpoint...')
-                    if not os.path.exists(train_cfg['save_checkpoint_dir']):
-                        os.makedirs(train_cfg['save_checkpoint_dir'])
-                    if (train_cfg['max_checkpoints'] is not None) and (len(
-                        saved_checkpoints) >= train_cfg['max_checkpoints']):
-                        os.system('rm -rf %s' % (saved_checkpoints.popleft()))
-                    torch.save(accelerator.unwrap_model(model).state_dict(),
-                                os.path.join(train_cfg['save_checkpoint_dir'], 'model_%d.pkl' % (step)))
-                    saved_checkpoints.append(os.path.join(train_cfg['save_checkpoint_dir'], 'model_%d.pkl' % (step)))
-                    print('saved.')
+                    print("saving checkpoint...")
+                    if not os.path.exists(train_cfg["save_checkpoint_dir"]):
+                        os.makedirs(train_cfg["save_checkpoint_dir"])
+                    if (train_cfg["max_checkpoints"] is not None) and (
+                        len(saved_checkpoints) >= train_cfg["max_checkpoints"]
+                    ):
+                        os.system("rm -rf %s" % (saved_checkpoints.popleft()))
+                    torch.save(
+                        accelerator.unwrap_model(model).state_dict(),
+                        os.path.join(
+                            train_cfg["save_checkpoint_dir"], "model_%d.pkl" % (step)
+                        ),
+                    )
+                    saved_checkpoints.append(
+                        os.path.join(
+                            train_cfg["save_checkpoint_dir"], "model_%d.pkl" % (step)
+                        )
+                    )
+                    print("saved.")
                 accelerator.wait_for_everyone()
             step += 1
-            if train_cfg['max_steps'] is not None and step >= train_cfg['max_steps']:
+            if train_cfg["max_steps"] is not None and step >= train_cfg["max_steps"]:
                 return
```

### Comparing `agilerl-0.1.8/agilerl/training/train_ilql.py` & `agilerl-0.1.9/agilerl/training/train_bc_lm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,169 +1,211 @@
-from accelerate import Accelerator
-from collections import deque
-from functools import partial
 import json
 import os
-from tqdm import tqdm
-import wandb
+from collections import deque
+from functools import partial
+
 import torch
-from torch.utils.data.dataset import IterableDataset
+from accelerate import Accelerator
 from torch.utils.data import DataLoader
+from torch.utils.data.dataset import IterableDataset
+from tqdm.auto import tqdm
+
+import wandb
+from agilerl.data.rl_data import Iterable_RL_Dataset
+from agilerl.data.torch_datasets import GeneralDataset, GeneralIterDataset
+from agilerl.utils.ilql_utils import add_system_configs, convert_path
 from agilerl.utils.load_objects import load_item
-from agilerl.utils.ilql_utils import convert_path, add_system_configs
 from agilerl.utils.log_utils import DistributeCombineLogs, label_logs
 from agilerl.utils.torch_utils import to
-from agilerl.data.rl_data import Iterable_RL_Dataset
-from agilerl.data.torch_datasets import GeneralDataset, GeneralIterDataset
+
 
 def train(cfg):
-    """The ILQL training function. 
-    """
-    print('using config:', cfg)
-    train_cfg = cfg['train']
-    train_cfg['save_checkpoint_dir'] = convert_path(train_cfg['save_checkpoint_dir'])
-    train_cfg['optim_state_path'] = convert_path(train_cfg['optim_state_path'])
-    wandb_cfg = cfg['wandb']
+    print("using config:", cfg)
+    train_cfg = cfg["train"]
+    train_cfg["save_checkpoint_dir"] = convert_path(train_cfg["save_checkpoint_dir"])
+    train_cfg["optim_state_path"] = convert_path(train_cfg["optim_state_path"])
+    wandb_cfg = cfg["wandb"]
     accelerator = Accelerator()
     system_cfg = add_system_configs(cfg, accelerator)
-    print('using device:', system_cfg['device'])
-    print('num processes:', system_cfg['num_processes'])
-    print('using fp16:', system_cfg['use_fp16'])
-    if not os.path.exists(train_cfg['save_checkpoint_dir']):
-        os.makedirs(train_cfg['save_checkpoint_dir'])
-    with open(os.path.join(train_cfg['save_checkpoint_dir'], 'config.json'), 'w') as f:
+    print("using device:", system_cfg["device"])
+    print("num processes:", system_cfg["num_processes"])
+    print("using fp16:", system_cfg["use_fp16"])
+    if not os.path.exists(train_cfg["save_checkpoint_dir"]):
+        os.makedirs(train_cfg["save_checkpoint_dir"])
+    with open(os.path.join(train_cfg["save_checkpoint_dir"], "config.json"), "w") as f:
         json.dump(cfg, f)
 
-    if wandb_cfg['use_wandb']:
+    if wandb_cfg["use_wandb"]:
         accelerator.wait_for_everyone()
         if accelerator.is_main_process:
-            wandb.init(project=wandb_cfg['wandb_project'], config=cfg)
+            wandb.init(project=wandb_cfg["wandb_project"], config=cfg)
         accelerator.wait_for_everyone()
 
-    raw_dataset_train = load_item(cfg['train_dataset'], system_cfg['device'])
-    raw_dataset_eval = load_item(cfg['eval_dataset'], system_cfg['device'])
+    raw_dataset_train = load_item(cfg["train_dataset"], system_cfg["device"])
+    raw_dataset_eval = load_item(cfg["eval_dataset"], system_cfg["device"])
     if isinstance(raw_dataset_train, Iterable_RL_Dataset):
-        dataset_train = GeneralIterDataset(raw_dataset_train, 'cpu')
+        dataset_train = GeneralIterDataset(raw_dataset_train, "cpu")
     else:
-        dataset_train = GeneralDataset(raw_dataset_train, 'cpu')
+        dataset_train = GeneralDataset(raw_dataset_train, "cpu")
     if isinstance(raw_dataset_eval, Iterable_RL_Dataset):
-        dataset_eval = GeneralIterDataset(raw_dataset_eval, 'cpu')
+        dataset_eval = GeneralIterDataset(raw_dataset_eval, "cpu")
     else:
-        dataset_eval = GeneralDataset(raw_dataset_eval, 'cpu')
-    train_data_loader_kwargs = {'num_workers': train_cfg['dataloader_workers'], 
-                                'batch_size': cfg['model']['batch_size'], 
-                                'collate_fn': dataset_train.collate}
-    eval_data_loader_kwargs = {'num_workers': train_cfg['dataloader_workers'], 
-                               'batch_size': train_cfg['eval_bsize'], 
-                               'collate_fn': dataset_eval.collate}
+        dataset_eval = GeneralDataset(raw_dataset_eval, "cpu")
+    train_data_loader_kwargs = {
+        "num_workers": train_cfg["dataloader_workers"],
+        "batch_size": train_cfg["bsize"],
+        "collate_fn": dataset_train.collate,
+    }
+    eval_data_loader_kwargs = {
+        "num_workers": train_cfg["dataloader_workers"],
+        "batch_size": train_cfg["eval_bsize"],
+        "collate_fn": dataset_eval.collate,
+    }
     if not isinstance(dataset_train, IterableDataset):
-        train_data_loader_kwargs['shuffle'] = True
+        train_data_loader_kwargs["shuffle"] = True
     if not isinstance(dataset_eval, IterableDataset):
-        eval_data_loader_kwargs['shuffle'] = True
+        eval_data_loader_kwargs["shuffle"] = True
     data_loader = DataLoader(dataset_train, **train_data_loader_kwargs)
     eval_data_loader = DataLoader(dataset_eval, **eval_data_loader_kwargs)
 
     evaluator = None
-    if cfg['evaluator'] is not None:
-        evaluator = load_item(cfg['evaluator'], system_cfg['device'])
+    if cfg["evaluator"] is not None:
+        evaluator = load_item(cfg["evaluator"], system_cfg["device"])
 
-    model = load_item(cfg['model'], system_cfg['device'])
+    model = load_item(cfg["model"], system_cfg["device"])
     model.train()
 
-    if hasattr(model, 'param_groups'):
-        params = [{'params': frozenset().union(*list(
-            map(lambda x: x.parameters(), p))), **f(train_cfg)} for p, f in model.param_groups]
-        model.optimizer = torch.optim.AdamW(
-            params, lr=model.lr, weight_decay=model.weight_decay)
-    optim = model.optimizer
-
-    if train_cfg['optim_state_path'] is not None and os.path.exists(train_cfg['optim_state_path']):
+    if hasattr(model, "param_groups"):
+        params = [
+            {
+                "params": frozenset().union(*list(map(lambda x: x.parameters(), p))),
+                **f(train_cfg),
+            }
+            for p, f in model.param_groups
+        ]
+    else:
+        params = model.parameters()
+    optim = torch.optim.AdamW(
+        params, lr=train_cfg["lr"], weight_decay=train_cfg["weight_decay"]
+    )
+    if train_cfg["optim_state_path"] is not None and os.path.exists(
+        train_cfg["optim_state_path"]
+    ):
         print(f'loading optimizer state from: {train_cfg["optim_state_path"]}')
-        optim.load_state_dict(torch.load(train_cfg['optim_state_path'], map_location=system_cfg['device']))
-        print('loaded.')
-    if isinstance(dataset_train, IterableDataset) and isinstance(dataset_eval, IterableDataset):
+        optim.load_state_dict(
+            torch.load(train_cfg["optim_state_path"], map_location=system_cfg["device"])
+        )
+        print("loaded.")
+    if isinstance(dataset_train, IterableDataset) and isinstance(
+        dataset_eval, IterableDataset
+    ):
         model, optim = accelerator.prepare(model, optim)
     elif isinstance(dataset_train, IterableDataset):
-        model, optim, eval_data_loader = accelerator.prepare(model, optim, eval_data_loader)
+        model, optim, eval_data_loader = accelerator.prepare(
+            model, optim, eval_data_loader
+        )
     elif isinstance(dataset_eval, IterableDataset):
         model, optim, data_loader = accelerator.prepare(model, optim, data_loader)
     else:
-        model, optim, data_loader, eval_data_loader = accelerator.prepare(model, optim, data_loader, eval_data_loader)
+        model, optim, data_loader, eval_data_loader = accelerator.prepare(
+            model, optim, data_loader, eval_data_loader
+        )
 
-    train_logs = DistributeCombineLogs(accelerator, use_wandb=wandb_cfg['use_wandb'])
-    eval_logs = DistributeCombineLogs(accelerator, use_wandb=wandb_cfg['use_wandb'])
+    train_logs = DistributeCombineLogs(accelerator, use_wandb=wandb_cfg["use_wandb"])
+    eval_logs = DistributeCombineLogs(accelerator, use_wandb=wandb_cfg["use_wandb"])
     step = 0
-    best_loss = float('inf')
+    best_loss = float("inf")
     saved_checkpoints = deque([])
-
-    # bar_format = '{l_bar}{bar:10}| {n:4}/{total_fmt} [{elapsed:>7}<{remaining:>7}, {rate_fmt}{postfix}]'
-    # pbar = trange(n_episodes, unit="ep", bar_format=bar_format, ascii=True)
-
-
-    # RL training loop
-    for epoch in range(train_cfg['epochs']):
+    for epoch in tqdm(
+        range(train_cfg["epochs"]), disable=not accelerator.is_local_main_process
+    ):
         for items in tqdm(data_loader, disable=not accelerator.is_local_main_process):
-            items = to(items, system_cfg['device'])
-            loss, logs, postproc_fs = accelerator.unwrap_model(model).get_loss(items, **train_cfg['loss'])
-            accelerator.backward(loss / train_cfg['grad_accum_steps'])
+            items = to(items, system_cfg["device"])
+            loss, logs, postproc_fs = accelerator.unwrap_model(model).get_loss(
+                items, **train_cfg["loss"]
+            )
+            accelerator.backward(loss / train_cfg["grad_accum_steps"])
             train_logs.accum_logs(logs)
-            if (step + 1) % train_cfg['grad_accum_steps'] == 0:
+            if (step + 1) % train_cfg["grad_accum_steps"] == 0:
                 optim.step()
                 optim.zero_grad()
-                if train_cfg['loss']['q_loss_weight'] != 0.0 or train_cfg['loss']['v_loss_weight'] != 0.0:
-                    accelerator.unwrap_model(model).softUpdate()
-            if (train_cfg['hard_update_every'] is not None) and ((step + 1) % train_cfg['hard_update_every'] == 0):
-                accelerator.unwrap_model(model).hardUpdate()
-            if (step + 1) % train_cfg['log_every'] == 0:
-                train_logs.log(*postproc_fs, 
-                               partial(label_logs, label='train'), 
-                               iteration=step, epoch=epoch)
-            if (step + 1) % train_cfg['grad_accum_steps'] == 0:
+            if (step + 1) % train_cfg["log_every"] == 0:
+                train_logs.log(
+                    *postproc_fs,
+                    partial(label_logs, label="train"),
+                    iteration=step,
+                    epoch=epoch,
+                )
+            if (step + 1) % train_cfg["grad_accum_steps"] == 0:
                 train_logs.reset_logs()
-            if (step + 1) % train_cfg['eval_every'] == 0:
+            if (step + 1) % train_cfg["eval_every"] == 0:
                 model.eval()
                 eval_logs.reset_logs()
                 with torch.no_grad():
                     for i, eval_items in enumerate(eval_data_loader):
-                        eval_items = to(eval_items, system_cfg['device'])
-                        if i >= train_cfg['eval_batches']:
+                        eval_items = to(eval_items, system_cfg["device"])
+                        if i >= train_cfg["eval_batches"]:
                             break
-                        _, logs, postproc_fs = accelerator.unwrap_model(model).get_loss(eval_items, **train_cfg['loss'])
+                        _, logs, postproc_fs = accelerator.unwrap_model(model).get_loss(
+                            eval_items, **train_cfg["loss"]
+                        )
                         if evaluator is not None:
-                            evaluator_logs = evaluator.evaluate(accelerator.unwrap_model(model), eval_items)
+                            evaluator_logs = evaluator.evaluate(
+                                accelerator.unwrap_model(model), eval_items
+                            )
                             if evaluator_logs is not None:
-                                logs['evaluation'] = evaluator_logs
+                                logs["evaluation"] = evaluator_logs
                         eval_logs.accum_logs(logs)
-                eval_label = 'eval'
-                eval_total_logs = eval_logs.log(*postproc_fs, 
-                                                partial(label_logs, label=eval_label), 
-                                                iteration=step, epoch=epoch)
+                eval_label = "eval"
+                eval_total_logs = eval_logs.log(
+                    *postproc_fs,
+                    partial(label_logs, label=eval_label),
+                    iteration=step,
+                    epoch=epoch,
+                )
                 accelerator.wait_for_everyone()
                 if accelerator.is_main_process:
-                    if eval_total_logs[eval_label]['loss'] < best_loss:
-                        print('new best eval loss! Saving ...')
-                        if not os.path.exists(train_cfg['save_checkpoint_dir']):
-                            os.makedirs(train_cfg['save_checkpoint_dir'])
-                        torch.save(accelerator.unwrap_model(model).state_dict(),
-                                    os.path.join(train_cfg['save_checkpoint_dir'], 'model.pkl'))
-                        torch.save(optim.state_dict(), os.path.join(train_cfg['save_checkpoint_dir'], 'optim.pkl'))
-                        print('saved.')
-                        best_loss = eval_total_logs[eval_label]['loss']
+                    if eval_total_logs[eval_label]["loss"] < best_loss:
+                        print("new best eval loss! Saving ...")
+                        if not os.path.exists(train_cfg["save_checkpoint_dir"]):
+                            os.makedirs(train_cfg["save_checkpoint_dir"])
+                        torch.save(
+                            accelerator.unwrap_model(model).state_dict(),
+                            os.path.join(train_cfg["save_checkpoint_dir"], "model.pkl"),
+                        )
+                        torch.save(
+                            optim.state_dict(),
+                            os.path.join(train_cfg["save_checkpoint_dir"], "optim.pkl"),
+                        )
+                        print("saved.")
+                        best_loss = eval_total_logs[eval_label]["loss"]
                 accelerator.wait_for_everyone()
                 model.train()
-            if train_cfg['save_every'] is not None and (step + 1) % train_cfg['save_every'] == 0:
+            if (
+                train_cfg["save_every"] is not None
+                and (step + 1) % train_cfg["save_every"] == 0
+            ):
                 accelerator.wait_for_everyone()
                 if accelerator.is_main_process:
-                    print('saving checkpoint...')
-                    if not os.path.exists(train_cfg['save_checkpoint_dir']):
-                        os.makedirs(train_cfg['save_checkpoint_dir'])
-                    if (train_cfg['max_checkpoints'] is not None) and (len(
-                        saved_checkpoints) >= train_cfg['max_checkpoints']):
-                        os.system('rm -rf %s' % (saved_checkpoints.popleft()))
-                    torch.save(accelerator.unwrap_model(model).state_dict(),
-                                os.path.join(train_cfg['save_checkpoint_dir'], 'model_%d.pkl' % (step)))
-                    saved_checkpoints.append(os.path.join(train_cfg['save_checkpoint_dir'], 'model_%d.pkl' % (step)))
-                    print('saved.')
+                    print("saving checkpoint...")
+                    if not os.path.exists(train_cfg["save_checkpoint_dir"]):
+                        os.makedirs(train_cfg["save_checkpoint_dir"])
+                    if (train_cfg["max_checkpoints"] is not None) and (
+                        len(saved_checkpoints) >= train_cfg["max_checkpoints"]
+                    ):
+                        os.system("rm -rf %s" % (saved_checkpoints.popleft()))
+                    torch.save(
+                        accelerator.unwrap_model(model).state_dict(),
+                        os.path.join(
+                            train_cfg["save_checkpoint_dir"], "model_%d.pkl" % (step)
+                        ),
+                    )
+                    saved_checkpoints.append(
+                        os.path.join(
+                            train_cfg["save_checkpoint_dir"], "model_%d.pkl" % (step)
+                        )
+                    )
+                    print("saved.")
                 accelerator.wait_for_everyone()
             step += 1
-            if train_cfg['max_steps'] is not None and step >= train_cfg['max_steps']:
-                return
+            if train_cfg["max_steps"] is not None and step >= train_cfg["max_steps"]:
+                return
```

### Comparing `agilerl-0.1.8/agilerl/training/train_multi_agent.py` & `agilerl-0.1.9/agilerl/training/train_multi_agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,63 @@
-import numpy as np
 import os
-from tqdm import trange
-import wandb
 from datetime import datetime
+
+import numpy as np
 from torch.utils.data import DataLoader
+from tqdm import trange
+
+import wandb
 from agilerl.components.replay_data import ReplayDataset
 from agilerl.components.sampler import Sampler
 
 
-def train_multi_agent(env, env_name, algo, pop, memory, INIT_HP, MUT_P, net_config, swap_channels=False, n_episodes=2000, 
-          max_steps=25, evo_epochs=5, evo_loop=5, eps_start=1.0, eps_end=0.1, 
-          eps_decay=0.995, target=200., tournament=None, mutation=None, checkpoint=None, 
-          checkpoint_path=None, wb=False, accelerator=None):
-    """The general online multi-agent RL training function. Returns trained population of agents 
+def train_multi_agent(
+    env,
+    env_name,
+    algo,
+    pop,
+    memory,
+    INIT_HP,
+    MUT_P,
+    net_config,
+    swap_channels=False,
+    n_episodes=2000,
+    max_steps=25,
+    evo_epochs=5,
+    evo_loop=5,
+    eps_start=1.0,
+    eps_end=0.1,
+    eps_decay=0.995,
+    target=200.0,
+    tournament=None,
+    mutation=None,
+    checkpoint=None,
+    checkpoint_path=None,
+    wb=False,
+    accelerator=None,
+):
+    """The general online multi-agent RL training function. Returns trained population of agents
     and their fitnesses.
 
     :param env: The environment to train in. Can be vectorized.
     :type env: Gym-style environment
     :param env_name: Environment name
     :type env_name: str
     :param algo: RL algorithm name
     :type algo: str
     :param pop: Population of agents
     :type pop: List[object]
     :param memory: Experience Replay Buffer
     :type memory: object
-    :param swap_channels: Swap image channels dimension from last to first 
+    :param swap_channels: Swap image channels dimension from last to first
     [H, W, C] -> [C, H, W], defaults to False
     :type swap_channels: bool, optional
     :param n_episodes: Maximum number of training episodes, defaults to 2000
     :type n_episodes: int, optional
-    :param max_steps: Maximum number of steps in environment per episode, defaults to 
+    :param max_steps: Maximum number of steps in environment per episode, defaults to
     500
     :type max_steps: int, optional
     :param evo_epochs: Evolution frequency (episodes), defaults to 5
     :type evo_epochs: int, optional
     :param evo_loop: Number of evaluation episodes, defaults to 1
     :type evo_loop: int, optional
     :param eps_start: Maximum exploration - initial epsilon value, defaults to 1.0
@@ -61,212 +84,255 @@
     if wb:
         if accelerator is not None:
             accelerator.wait_for_everyone()
             if accelerator.is_main_process:
                 wandb.init(
                     # set the wandb project where this run will be logged
                     project="EvoMADDPGTesting",
-                    name="{}-MultiAgentEvoHPO-{}-{}".format(env_name, algo,
-                                                datetime.now().strftime("%m%d%Y%H%M%S")),
+                    name="{}-MultiAgentEvoHPO-{}-{}".format(
+                        env_name, algo, datetime.now().strftime("%m%d%Y%H%M%S")
+                    ),
                     # track hyperparameters and run metadata
                     config={
-                        "algo": "Evo HPO {}".format(algo),
+                        "algo": f"Evo HPO {algo}",
                         "env": env_name,
                         "net_config": net_config,
-                        "batch_size" : INIT_HP['BATCH_SIZE'],
-                        "lr" : INIT_HP['LR'],
-                        "gamma": INIT_HP['GAMMA'],
-                        "memory_size" : INIT_HP['MEMORY_SIZE'],
-                        "learn_step" : INIT_HP['LEARN_STEP'],
-                        "tau" : INIT_HP['TAU'],
-                        "pop_size" : INIT_HP['TOURN_SIZE'],
-                        "no_mut" : MUT_P['NO_MUT'],
-                        "arch_mut" :  MUT_P['ARCH_MUT'],
-                        "params_mut" : MUT_P['PARAMS_MUT'],
-                        "act_mut" : MUT_P['ACT_MUT'],
-                        "rl_hp_mut" : MUT_P['RL_HP_MUT']}
+                        "batch_size": INIT_HP["BATCH_SIZE"],
+                        "lr": INIT_HP["LR"],
+                        "gamma": INIT_HP["GAMMA"],
+                        "memory_size": INIT_HP["MEMORY_SIZE"],
+                        "learn_step": INIT_HP["LEARN_STEP"],
+                        "tau": INIT_HP["TAU"],
+                        "pop_size": INIT_HP["TOURN_SIZE"],
+                        "no_mut": MUT_P["NO_MUT"],
+                        "arch_mut": MUT_P["ARCH_MUT"],
+                        "params_mut": MUT_P["PARAMS_MUT"],
+                        "act_mut": MUT_P["ACT_MUT"],
+                        "rl_hp_mut": MUT_P["RL_HP_MUT"],
+                    },
                 )
             accelerator.wait_for_everyone()
         else:
             wandb.init(
-                    # set the wandb project where this run will be logged
-                    entity = "agilerl",
-                    project="MADDPG Benchmarking",
-                    name="{}-{}-{}-RandomActions".format(env_name, algo,
-                                                datetime.now().strftime("%m%d%Y%H%M%S")),
-                    # track hyperparameters and run metadata
-                    config={
-                        "algo": "Evo HPO {}".format(algo),
-                        "env": env_name,
-                        "net_config": net_config,
-                        "batch_size" : INIT_HP['BATCH_SIZE'],
-                        "lr" : INIT_HP['LR'],
-                        "gamma": INIT_HP['GAMMA'],
-                        "memory_size" : INIT_HP['MEMORY_SIZE'],
-                        "learn_step" : INIT_HP['LEARN_STEP'],
-                        "tau" : INIT_HP['TAU'],
-                        "pop_size" : INIT_HP['TOURN_SIZE'],
-                        "no_mut" : MUT_P['NO_MUT'],
-                        "arch_mut" :  MUT_P['ARCH_MUT'],
-                        "params_mut" : MUT_P['PARAMS_MUT'],
-                        "act_mut" : MUT_P['ACT_MUT'],
-                        "rl_hp_mut" : MUT_P['RL_HP_MUT']}
-                )
-            
+                # set the wandb project where this run will be logged
+                entity="agilerl",
+                project="MADDPG Benchmarking",
+                name="{}-{}-{}-RandomActions".format(
+                    env_name, algo, datetime.now().strftime("%m%d%Y%H%M%S")
+                ),
+                # track hyperparameters and run metadata
+                config={
+                    "algo": f"Evo HPO {algo}",
+                    "env": env_name,
+                    "net_config": net_config,
+                    "batch_size": INIT_HP["BATCH_SIZE"],
+                    "lr": INIT_HP["LR"],
+                    "gamma": INIT_HP["GAMMA"],
+                    "memory_size": INIT_HP["MEMORY_SIZE"],
+                    "learn_step": INIT_HP["LEARN_STEP"],
+                    "tau": INIT_HP["TAU"],
+                    "pop_size": INIT_HP["TOURN_SIZE"],
+                    "no_mut": MUT_P["NO_MUT"],
+                    "arch_mut": MUT_P["ARCH_MUT"],
+                    "params_mut": MUT_P["PARAMS_MUT"],
+                    "act_mut": MUT_P["ACT_MUT"],
+                    "rl_hp_mut": MUT_P["RL_HP_MUT"],
+                },
+            )
+
     if accelerator is not None:
-        accel_temp_models_path = 'models/{}'.format(env_name)
+        accel_temp_models_path = f"models/{env_name}"
         if accelerator.is_main_process:
             if not os.path.exists(accel_temp_models_path):
                 os.makedirs(accel_temp_models_path)
 
-    save_path = checkpoint_path.split('.pt')[0] if checkpoint_path is not None else "{}-EvoHPO-{}-{}".format(
-        env_name, algo, datetime.now().strftime("%m%d%Y%H%M%S"))
-    
+    save_path = (
+        checkpoint_path.split(".pt")[0]
+        if checkpoint_path is not None
+        else "{}-EvoHPO-{}-{}".format(
+            env_name, algo, datetime.now().strftime("%m%d%Y%H%M%S")
+        )
+    )
+
     if accelerator is not None:
         # Create dataloader from replay buffer
         replay_dataset = ReplayDataset(memory, pop[0].batch_size)
         replay_dataloader = DataLoader(replay_dataset, batch_size=None)
         replay_dataloader = accelerator.prepare(replay_dataloader)
-        sampler = Sampler(distributed=True, 
-                          dataset=replay_dataset, 
-                          dataloader=replay_dataloader)
+        sampler = Sampler(
+            distributed=True, dataset=replay_dataset, dataloader=replay_dataloader
+        )
     else:
         sampler = Sampler(distributed=False, memory=memory)
 
     epsilon = eps_start
 
     if accelerator is not None:
-        print(f'\nDistributed training on {accelerator.device}...')
+        print(f"\nDistributed training on {accelerator.device}...")
     else:
-        print('\nTraining...')
+        print("\nTraining...")
 
-    bar_format = '{l_bar}{bar:10}| {n:4}/{total_fmt} [{elapsed:>7}<{remaining:>7}, {rate_fmt}{postfix}]'
+    bar_format = "{l_bar}{bar:10}| {n:4}/{total_fmt} [{elapsed:>7}<{remaining:>7}, {rate_fmt}{postfix}]"
     if accelerator is not None:
-        pbar = trange(n_episodes, unit="ep", bar_format=bar_format, ascii=True, 
-                      disable=not accelerator.is_local_main_process)
+        pbar = trange(
+            n_episodes,
+            unit="ep",
+            bar_format=bar_format,
+            ascii=True,
+            disable=not accelerator.is_local_main_process,
+        )
     else:
         pbar = trange(n_episodes, unit="ep", bar_format=bar_format, ascii=True)
 
     pop_fitnesses = []
     total_steps = 0
 
     # Pre-training mutation
     if accelerator is None:
         if mutation is not None:
             pop = mutation.mutation(pop, pre_training_mut=True)
 
-
     # RL training loop
     for idx_epi in pbar:
         if accelerator is not None:
-            accelerator.wait_for_everyone()   
-        for agent in pop:   # Loop through population 
+            accelerator.wait_for_everyone()
+        for agent in pop:  # Loop through population
             state = env.reset()[0]  # Reset environment at start of episode
             agent_reward = {agent_id: 0 for agent_id in env.agents}
             if swap_channels:
-                state = {agent_id: np.moveaxis(np.expand_dims(s, 0), [3], [1]) for agent_id, s in state.items()}
+                state = {
+                    agent_id: np.moveaxis(np.expand_dims(s, 0), [3], [1])
+                    for agent_id, s in state.items()
+                }
 
             for _ in range(max_steps):
                 total_steps += 1
                 # Get next action from agent
                 action = agent.getAction(state, epsilon)
-                next_state, reward, done, truncation, _ = env.step(action)   # Act in environment
-                
+                next_state, reward, done, truncation, _ = env.step(
+                    action
+                )  # Act in environment
+
                 # Save experience to replay buffer
                 if swap_channels:
                     state = {agent_id: np.squeeze(s) for agent_id, s in state.items()}
-                    next_state = {agent_id: np.moveaxis(ns, [2], [0]) for agent_id, ns in next_state.items()}
+                    next_state = {
+                        agent_id: np.moveaxis(ns, [2], [0])
+                        for agent_id, ns in next_state.items()
+                    }
 
                 if any(truncation.values()) or any(done.values()):
                     break
-                
+
                 memory.save2memory(state, action, reward, next_state, done)
-                
+
                 for agent_id, r in reward.items():
-                    agent_reward[agent_id] += r 
+                    agent_reward[agent_id] += r
 
-                #Learn according to learning frequency
-                if (memory.counter % agent.learn_step == 0) and (len(
-                        memory) >= agent.batch_size):
+                # Learn according to learning frequency
+                if (memory.counter % agent.learn_step == 0) and (
+                    len(memory) >= agent.batch_size
+                ):
                     # Sample replay buffer
                     experiences = sampler.sample(agent.batch_size)
                     # Learn according to agent's RL algorithm
                     agent.learn(experiences)
-                
-                # Update the state 
+
+                # Update the state
                 if swap_channels:
-                    next_state = {agent_id: np.expand_dims(ns,0) for agent_id, ns in next_state.items()}
+                    next_state = {
+                        agent_id: np.expand_dims(ns, 0)
+                        for agent_id, ns in next_state.items()
+                    }
                 state = next_state
-            
+
             score = sum(agent_reward.values())
             agent.scores.append(score)
 
             agent.steps[-1] += total_steps
 
         # Update epsilon for exploration
         epsilon = max(eps_end, epsilon * eps_decay)
 
         # Now evolve if necessary
         if (idx_epi + 1) % evo_epochs == 0:
-            
             # Evaluate population
             fitnesses = [
                 agent.test(
-                    env,
-                    swap_channels=swap_channels,
-                    max_steps=max_steps,
-                    loop=evo_loop) for agent in pop]
+                    env, swap_channels=swap_channels, max_steps=max_steps, loop=evo_loop
+                )
+                for agent in pop
+            ]
             pop_fitnesses.append(fitnesses)
 
             mean_scores = np.mean([agent.scores[-20:] for agent in pop], axis=1)
 
             if wb:
                 if accelerator is not None:
                     accelerator.wait_for_everyone()
                     if accelerator.is_main_process:
-                        wandb.log({"global_step": total_steps*accelerator.state.num_processes,
+                        wandb.log(
+                            {
+                                "global_step": total_steps
+                                * accelerator.state.num_processes,
                                 "eval/mean_score": np.mean(mean_scores),
-                                "eval/best_score": np.max([agent.scores[-1] for agent in pop]),
+                                "eval/best_score": np.max(
+                                    [agent.scores[-1] for agent in pop]
+                                ),
                                 "eval/mean_fitness": np.mean(fitnesses),
-                                "eval/best_fitness": np.max(fitnesses)})
+                                "eval/best_fitness": np.max(fitnesses),
+                            }
+                        )
                     accelerator.wait_for_everyone()
                 else:
-                    wandb.log({"global_step": total_steps,
-                                "eval/mean_score": np.mean(mean_scores),
-                                "eval/best_score": np.max([agent.scores[-1] for agent in pop]),
-                                "eval/mean_fitness": np.mean(fitnesses),
-                                "eval/best_fitness": np.max(fitnesses)})
-                    
+                    wandb.log(
+                        {
+                            "global_step": total_steps,
+                            "eval/mean_score": np.mean(mean_scores),
+                            "eval/best_score": np.max(
+                                [agent.scores[-1] for agent in pop]
+                            ),
+                            "eval/mean_fitness": np.mean(fitnesses),
+                            "eval/best_fitness": np.max(fitnesses),
+                        }
+                    )
+
                 for idx, agent in enumerate(pop):
-                    wandb.log({
-                        f"learn_step_agent_{idx}": agent.learn_step,
-                        f"learning_rate_agent_{idx}" : agent.lr,
-                        f"batch_size_agent_{idx}" : agent.batch_size,
-                        f"indi_fitness_agent_{idx}": agent.fitness[-1]
-                    })
+                    wandb.log(
+                        {
+                            f"learn_step_agent_{idx}": agent.learn_step,
+                            f"learning_rate_agent_{idx}": agent.lr,
+                            f"batch_size_agent_{idx}": agent.batch_size,
+                            f"indi_fitness_agent_{idx}": agent.fitness[-1],
+                        }
+                    )
 
             # Update step counter
             for agent in pop:
                 agent.steps.append(agent.steps[-1])
 
-            fitness = ["%.2f"%fitness for fitness in fitnesses]
-            avg_fitness = ["%.2f"%np.mean(agent.fitness[-100:]) for agent in pop]
-            avg_score = ["%.2f"%np.mean(agent.scores[-100:]) for agent in pop]
+            fitness = ["%.2f" % fitness for fitness in fitnesses]
+            avg_fitness = ["%.2f" % np.mean(agent.fitness[-100:]) for agent in pop]
+            avg_score = ["%.2f" % np.mean(agent.scores[-100:]) for agent in pop]
             agents = [agent.index for agent in pop]
             num_steps = [agent.steps[-1] for agent in pop]
             muts = [agent.mut for agent in pop]
-            perf_info = f'Fitness: {fitness}, 100 fitness avgs: {avg_fitness}, 100 score avgs: {avg_score}'
-            pop_info = f'Agents: {agents}, Steps: {num_steps}, Mutations: {muts}' 
-            pbar_string = perf_info + ', ' + pop_info
+            perf_info = f"Fitness: {fitness}, 100 fitness avgs: {avg_fitness}, 100 score avgs: {avg_score}"
+            pop_info = f"Agents: {agents}, Steps: {num_steps}, Mutations: {muts}"
+            pbar_string = perf_info + ", " + pop_info
             pbar.set_postfix_str(pbar_string)
             pbar.update(0)
 
             # Early stop if consistently reaches target
-            if np.all(np.greater([np.mean(agent.fitness[-100:])
-                      for agent in pop], target)) and idx_epi >= 100:
+            if (
+                np.all(
+                    np.greater([np.mean(agent.fitness[-100:]) for agent in pop], target)
+                )
+                and idx_epi >= 100
+            ):
                 if wb:
                     wandb.finish()
                 return pop, pop_fitnesses
 
             # Tournament selection and population mutation
             if tournament and mutation is not None:
                 if accelerator is not None:
@@ -274,38 +340,42 @@
                     for model in pop:
                         model.unwrap_models()
                     accelerator.wait_for_everyone()
                     if accelerator.is_main_process:
                         elite, pop = tournament.select(pop)
                         pop = mutation.mutation(pop)
                         for pop_i, model in enumerate(pop):
-                            model.saveCheckpoint(f'{accel_temp_models_path}/{algo}_{pop_i}.pt')
+                            model.saveCheckpoint(
+                                f"{accel_temp_models_path}/{algo}_{pop_i}.pt"
+                            )
                     accelerator.wait_for_everyone()
                     if not accelerator.is_main_process:
                         for pop_i, model in enumerate(pop):
-                            model.loadCheckpoint(f'{accel_temp_models_path}/{algo}_{pop_i}.pt')
+                            model.loadCheckpoint(
+                                f"{accel_temp_models_path}/{algo}_{pop_i}.pt"
+                            )
                     accelerator.wait_for_everyone()
                     for model in pop:
                         model.wrap_models()
                 else:
                     elite, pop = tournament.select(pop)
-                    pop = mutation.mutation(pop) 
+                    pop = mutation.mutation(pop)
 
         # Save model checkpoint
         if checkpoint is not None:
             if (idx_epi + 1) % checkpoint == 0:
                 if accelerator is not None:
                     accelerator.wait_for_everyone()
                     if not accelerator.is_main_process:
                         for i, agent in enumerate(pop):
-                            agent.saveCheckpoint(f'{save_path}_{i}_{idx_epi+1}.pt')
+                            agent.saveCheckpoint(f"{save_path}_{i}_{idx_epi+1}.pt")
                     accelerator.wait_for_everyone()
                 else:
                     for i, agent in enumerate(pop):
-                        agent.saveCheckpoint(f'{save_path}_{i}_{idx_epi+1}.pt')
+                        agent.saveCheckpoint(f"{save_path}_{i}_{idx_epi+1}.pt")
 
     if wb:
         if accelerator is not None:
             accelerator.wait_for_everyone()
             if accelerator.is_main_process:
                 wandb.finish()
             accelerator.wait_for_everyone()
```

### Comparing `agilerl-0.1.8/agilerl/training/train_offline.py` & `agilerl-0.1.9/agilerl/training/train_offline.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,44 @@
-import numpy as np
 import os
-from tqdm import trange
-import wandb
 from datetime import datetime
-from agilerl.utils.minari_utils import MinariToAgileBuffer
+
+import numpy as np
 from torch.utils.data import DataLoader
+from tqdm import trange
+
+import wandb
 from agilerl.components.replay_data import ReplayDataset
 from agilerl.components.sampler import Sampler
+from agilerl.utils.minari_utils import MinariToAgileBuffer
 
 
-def train(env, env_name, dataset, algo, pop, memory, INIT_HP, MUT_P, swap_channels=False, 
-          n_episodes=2000, max_steps=500, evo_epochs=5, evo_loop=1, target=200., 
-          tournament=None, mutation=None, checkpoint=None, checkpoint_path=None, 
-          wb=False, accelerator=None, minari_dataset_id=None, remote=False):
+def train(
+    env,
+    env_name,
+    dataset,
+    algo,
+    pop,
+    memory,
+    INIT_HP,
+    MUT_P,
+    swap_channels=False,
+    n_episodes=2000,
+    max_steps=500,
+    evo_epochs=5,
+    evo_loop=1,
+    target=200.0,
+    tournament=None,
+    mutation=None,
+    checkpoint=None,
+    checkpoint_path=None,
+    wb=False,
+    accelerator=None,
+    minari_dataset_id=None,
+    remote=False,
+):
     """The general offline RL training function. Returns trained population of agents and their fitnesses.
 
     :param env: The environment to train in
     :type env: Gym-style environment
     :param env_name: Environment name
     :type env_name: str
     :param dataset: Offline RL dataset
@@ -55,196 +77,224 @@
     if wb:
         if accelerator is not None:
             accelerator.wait_for_everyone()
             if accelerator.is_main_process:
                 wandb.init(
                     # set the wandb project where this run will be logged
                     project="AgileRL",
-                    name="{}-EvoHPO-{}-{}".format(env_name, algo,
-                                                datetime.now().strftime("%m%d%Y%H%M%S")),
+                    name="{}-EvoHPO-{}-{}".format(
+                        env_name, algo, datetime.now().strftime("%m%d%Y%H%M%S")
+                    ),
                     # track hyperparameters and run metadata
                     config={
-                        "algo": "Evo HPO {}".format(algo),
+                        "algo": f"Evo HPO {algo}",
                         "env": env_name,
-                        "batch_size" : INIT_HP['BATCH_SIZE'],
-                        "lr" : INIT_HP['LR'],
-                        "gamma": INIT_HP['GAMMA'],
-                        "memory_size" : INIT_HP['MEMORY_SIZE'],
-                        "learn_step" : INIT_HP['LEARN_STEP'],
-                        "tau" : INIT_HP['TAU'],
-                        "pop_size" : INIT_HP['TOURN_SIZE'],
-                        "no_mut" : MUT_P['NO_MUT'],
-                        "arch_mut" :  MUT_P['ARCH_MUT'],
-                        "params_mut" : MUT_P['PARAMS_MUT'],
-                        "act_mut" : MUT_P['ACT_MUT'],
-                        "rl_hp_mut" : MUT_P['RL_HP_MUT']}
+                        "batch_size": INIT_HP["BATCH_SIZE"],
+                        "lr": INIT_HP["LR"],
+                        "gamma": INIT_HP["GAMMA"],
+                        "memory_size": INIT_HP["MEMORY_SIZE"],
+                        "learn_step": INIT_HP["LEARN_STEP"],
+                        "tau": INIT_HP["TAU"],
+                        "pop_size": INIT_HP["TOURN_SIZE"],
+                        "no_mut": MUT_P["NO_MUT"],
+                        "arch_mut": MUT_P["ARCH_MUT"],
+                        "params_mut": MUT_P["PARAMS_MUT"],
+                        "act_mut": MUT_P["ACT_MUT"],
+                        "rl_hp_mut": MUT_P["RL_HP_MUT"],
+                    },
                 )
             accelerator.wait_for_everyone()
         else:
             wandb.init(
-                    # set the wandb project where this run will be logged
-                    project="AgileRL",
-                    name="{}-EvoHPO-{}-{}".format(env_name, algo,
-                                                datetime.now().strftime("%m%d%Y%H%M%S")),
-                    # track hyperparameters and run metadata
-                    config={
-                        "algo": "Evo HPO {}".format(algo),
-                        "env": env_name,
-                        "batch_size" : INIT_HP['BATCH_SIZE'],
-                        "lr" : INIT_HP['LR'],
-                        "gamma": INIT_HP['GAMMA'],
-                        "memory_size" : INIT_HP['MEMORY_SIZE'],
-                        "learn_step" : INIT_HP['LEARN_STEP'],
-                        "tau" : INIT_HP['TAU'],
-                        "pop_size" : INIT_HP['TOURN_SIZE'],
-                        "no_mut" : MUT_P['NO_MUT'],
-                        "arch_mut" :  MUT_P['ARCH_MUT'],
-                        "params_mut" : MUT_P['PARAMS_MUT'],
-                        "act_mut" : MUT_P['ACT_MUT'],
-                        "rl_hp_mut" : MUT_P['RL_HP_MUT']}
-                )
+                # set the wandb project where this run will be logged
+                project="AgileRL",
+                name="{}-EvoHPO-{}-{}".format(
+                    env_name, algo, datetime.now().strftime("%m%d%Y%H%M%S")
+                ),
+                # track hyperparameters and run metadata
+                config={
+                    "algo": f"Evo HPO {algo}",
+                    "env": env_name,
+                    "batch_size": INIT_HP["BATCH_SIZE"],
+                    "lr": INIT_HP["LR"],
+                    "gamma": INIT_HP["GAMMA"],
+                    "memory_size": INIT_HP["MEMORY_SIZE"],
+                    "learn_step": INIT_HP["LEARN_STEP"],
+                    "tau": INIT_HP["TAU"],
+                    "pop_size": INIT_HP["TOURN_SIZE"],
+                    "no_mut": MUT_P["NO_MUT"],
+                    "arch_mut": MUT_P["ARCH_MUT"],
+                    "params_mut": MUT_P["PARAMS_MUT"],
+                    "act_mut": MUT_P["ACT_MUT"],
+                    "rl_hp_mut": MUT_P["RL_HP_MUT"],
+                },
+            )
 
     if accelerator is not None:
-        accel_temp_models_path = 'models/{}'.format(env_name)
+        accel_temp_models_path = f"models/{env_name}"
         if accelerator.is_main_process:
             if not os.path.exists(accel_temp_models_path):
                 os.makedirs(accel_temp_models_path)
 
-    save_path = checkpoint_path.split('.pt')[0] if checkpoint_path is not None else "{}-EvoHPO-{}-{}".format(
-        env_name, algo, datetime.now().strftime("%m%d%Y%H%M%S"))
-    
+    save_path = (
+        checkpoint_path.split(".pt")[0]
+        if checkpoint_path is not None
+        else "{}-EvoHPO-{}-{}".format(
+            env_name, algo, datetime.now().strftime("%m%d%Y%H%M%S")
+        )
+    )
+
     if accelerator is not None:
         if accelerator.is_main_process:
-            print('Filling replay buffer with dataset...')
+            print("Filling replay buffer with dataset...")
         accelerator.wait_for_everyone()
     else:
-        print('Filling replay buffer with dataset...')
-        
+        print("Filling replay buffer with dataset...")
+
     if minari_dataset_id:
         print(f"Loading Minari Dataset with dataset_id {minari_dataset_id} in Buffer")
-        
-        memory = MinariToAgileBuffer(minari_dataset_id, memory, accelerator,remote)
-        
+
+        memory = MinariToAgileBuffer(minari_dataset_id, memory, accelerator, remote)
+
         print(f"Minari Dataset with dataset_id {minari_dataset_id} loaded in Buffer")
-    
+
     else:
-        print('Loading buffer...')
-        dataset_length = dataset['rewards'].shape[0]
+        print("Loading buffer...")
+        dataset_length = dataset["rewards"].shape[0]
         # for i in range(dataset_length):
         #     state = dataset['observations'][i]
         #     next_state = dataset['next_observations'][i]
         #     if swap_channels:
         #         state = np.moveaxis(state, [3], [1])
         #         next_state = np.moveaxis(next_state, [3], [1])
         #     action = dataset['actions'][i]
         #     reward = dataset['rewards'][i]
         #     done = bool(dataset['terminals'][i])
         #     memory.save2memory(state, action, next_state, reward, done)
-        for i in range(dataset_length-1):
-            state = dataset['observations'][i]
-            next_state = dataset['observations'][i+1]
+        for i in range(dataset_length - 1):
+            state = dataset["observations"][i]
+            next_state = dataset["observations"][i + 1]
             if swap_channels:
                 state = np.moveaxis(state, [3], [1])
                 next_state = np.moveaxis(next_state, [3], [1])
-            action = dataset['actions'][i]
-            reward = dataset['rewards'][i]
-            done = bool(dataset['terminals'][i])
+            action = dataset["actions"][i]
+            reward = dataset["rewards"][i]
+            done = bool(dataset["terminals"][i])
             memory.save2memory(state, action, reward, next_state, done)
         if accelerator is not None:
-          if accelerator.is_main_process:
-              print('Loaded buffer.')
-          accelerator.wait_for_everyone()
+            if accelerator.is_main_process:
+                print("Loaded buffer.")
+            accelerator.wait_for_everyone()
         else:
-          print('Loaded buffer.')
-    
+            print("Loaded buffer.")
 
     if accelerator is not None:
         # Create dataloader from replay buffer
         replay_dataset = ReplayDataset(memory, pop[0].batch_size)
         replay_dataloader = DataLoader(replay_dataset, batch_size=None)
         replay_dataloader = accelerator.prepare(replay_dataloader)
-        sampler = Sampler(distributed=True, 
-                          dataset=replay_dataset, 
-                          dataloader=replay_dataloader)
+        sampler = Sampler(
+            distributed=True, dataset=replay_dataset, dataloader=replay_dataloader
+        )
     else:
         sampler = Sampler(distributed=False, memory=memory)
-    
+
     if accelerator is not None:
-        print(f'\nDistributed training on {accelerator.device}...')
+        print(f"\nDistributed training on {accelerator.device}...")
     else:
-        print('\nTraining...')
+        print("\nTraining...")
 
-    bar_format = '{l_bar}{bar:10}| {n:4}/{total_fmt} [{elapsed:>7}<{remaining:>7}, {rate_fmt}{postfix}]'
+    bar_format = "{l_bar}{bar:10}| {n:4}/{total_fmt} [{elapsed:>7}<{remaining:>7}, {rate_fmt}{postfix}]"
     if accelerator is not None:
-        pbar = trange(n_episodes, unit="ep", bar_format=bar_format, ascii=True, 
-                      disable=not accelerator.is_local_main_process)
+        pbar = trange(
+            n_episodes,
+            unit="ep",
+            bar_format=bar_format,
+            ascii=True,
+            disable=not accelerator.is_local_main_process,
+        )
     else:
         pbar = trange(n_episodes, unit="ep", bar_format=bar_format, ascii=True)
 
     pop_fitnesses = []
     total_steps = 0
 
     # Pre-training mutation
     if mutation is not None:
         pop = mutation.mutation(pop, pre_training_mut=True)
 
     # RL training loop
     for idx_epi in pbar:
         if accelerator is not None:
-            accelerator.wait_for_everyone() 
-        for agent in pop:   # Loop through population
+            accelerator.wait_for_everyone()
+        for agent in pop:  # Loop through population
             for idx_step in range(max_steps):
-                experiences = sampler.sample(agent.batch_size)   # Sample replay buffer
+                experiences = sampler.sample(agent.batch_size)  # Sample replay buffer
                 # Learn according to agent's RL algorithm
                 agent.learn(experiences)
 
             agent.steps[-1] += max_steps
             total_steps += max_steps
 
         # Now evolve if necessary
         if (idx_epi + 1) % evo_epochs == 0:
             # Evaluate population
-            fitnesses = [agent.test(env,
-                                    swap_channels=swap_channels,
-                                    max_steps=max_steps,
-                                    loop=evo_loop) for agent in pop]
+            fitnesses = [
+                agent.test(
+                    env, swap_channels=swap_channels, max_steps=max_steps, loop=evo_loop
+                )
+                for agent in pop
+            ]
             pop_fitnesses.append(fitnesses)
 
             if wb:
                 if accelerator is not None:
                     accelerator.wait_for_everyone()
                     if accelerator.is_main_process:
-                        wandb.log({"global_step": total_steps*accelerator.state.num_processes,
+                        wandb.log(
+                            {
+                                "global_step": total_steps
+                                * accelerator.state.num_processes,
                                 "eval/mean_reward": np.mean(fitnesses),
-                                "eval/best_fitness": np.max(fitnesses)})
+                                "eval/best_fitness": np.max(fitnesses),
+                            }
+                        )
                     accelerator.wait_for_everyone()
                 else:
-                    wandb.log({"global_step": total_steps,
-                                "eval/mean_reward": np.mean(fitnesses),
-                                "eval/best_fitness": np.max(fitnesses)})
+                    wandb.log(
+                        {
+                            "global_step": total_steps,
+                            "eval/mean_reward": np.mean(fitnesses),
+                            "eval/best_fitness": np.max(fitnesses),
+                        }
+                    )
 
             # Update step counter
             for agent in pop:
                 agent.steps.append(agent.steps[-1])
 
-            fitness = ["%.2f"%fitness for fitness in fitnesses]
-            avg_fitness = ["%.2f"%np.mean(agent.fitness[-100:]) for agent in pop]
-            avg_score = ["%.2f"%np.mean(agent.scores[-100:]) for agent in pop]
+            fitness = ["%.2f" % fitness for fitness in fitnesses]
+            avg_fitness = ["%.2f" % np.mean(agent.fitness[-100:]) for agent in pop]
+            avg_score = ["%.2f" % np.mean(agent.scores[-100:]) for agent in pop]
             agents = [agent.index for agent in pop]
             num_steps = [agent.steps[-1] for agent in pop]
             muts = [agent.mut for agent in pop]
-            perf_info = f'Fitness: {fitness}, 100 fitness avgs: {avg_fitness}, 100 score avgs: {avg_score}'
-            pop_info = f'Agents: {agents}, Steps: {num_steps}, Mutations: {muts}'
-            pbar_string = perf_info + ', ' + pop_info
+            perf_info = f"Fitness: {fitness}, 100 fitness avgs: {avg_fitness}, 100 score avgs: {avg_score}"
+            pop_info = f"Agents: {agents}, Steps: {num_steps}, Mutations: {muts}"
+            pbar_string = perf_info + ", " + pop_info
             pbar.set_postfix_str(pbar_string)
             pbar.update(0)
 
             # Early stop if consistently reaches target
-            if np.all(np.greater([np.mean(agent.fitness[-100:])
-                      for agent in pop], target)) and idx_epi >= 100:
+            if (
+                np.all(
+                    np.greater([np.mean(agent.fitness[-100:]) for agent in pop], target)
+                )
+                and idx_epi >= 100
+            ):
                 if wb:
                     wandb.finish()
                 return pop, pop_fitnesses
 
             # Tournament selection and population mutation
             if tournament and mutation is not None:
                 if accelerator is not None:
@@ -252,19 +302,23 @@
                     for model in pop:
                         model.unwrap_models()
                     accelerator.wait_for_everyone()
                     if accelerator.is_main_process:
                         elite, pop = tournament.select(pop)
                         pop = mutation.mutation(pop)
                         for pop_i, model in enumerate(pop):
-                            model.saveCheckpoint(f'{accel_temp_models_path}/{algo}_{pop_i}.pt')
+                            model.saveCheckpoint(
+                                f"{accel_temp_models_path}/{algo}_{pop_i}.pt"
+                            )
                     accelerator.wait_for_everyone()
                     if not accelerator.is_main_process:
                         for pop_i, model in enumerate(pop):
-                            model.loadCheckpoint(f'{accel_temp_models_path}/{algo}_{pop_i}.pt')
+                            model.loadCheckpoint(
+                                f"{accel_temp_models_path}/{algo}_{pop_i}.pt"
+                            )
                     accelerator.wait_for_everyone()
                     for model in pop:
                         model.wrap_models()
                 else:
                     elite, pop = tournament.select(pop)
                     pop = mutation.mutation(pop)
 
@@ -273,28 +327,28 @@
                 if accelerator is not None:
                     accelerator.wait_for_everyone()
                     for model in pop:
                         model.unwrap_models()
                     accelerator.wait_for_everyone()
                     if accelerator.is_main_process:
                         for i, agent in enumerate(pop):
-                            agent.saveCheckpoint(f'{save_path}_{i}_{idx_epi+1}.pt')
-                        print('Saved checkpoint.')
+                            agent.saveCheckpoint(f"{save_path}_{i}_{idx_epi+1}.pt")
+                        print("Saved checkpoint.")
                     accelerator.wait_for_everyone()
                     for model in pop:
                         model.wrap_models()
                     accelerator.wait_for_everyone()
                 else:
                     for i, agent in enumerate(pop):
-                        agent.saveCheckpoint(f'{save_path}_{i}_{idx_epi+1}.pt')
-                    print('Saved checkpoint.')
+                        agent.saveCheckpoint(f"{save_path}_{i}_{idx_epi+1}.pt")
+                    print("Saved checkpoint.")
 
     if wb:
         if accelerator is not None:
             accelerator.wait_for_everyone()
             if accelerator.is_main_process:
                 wandb.finish()
             accelerator.wait_for_everyone()
         else:
             wandb.finish()
-            
+
     return pop, pop_fitnesses
```

### Comparing `agilerl-0.1.8/agilerl/utils/cache.py` & `agilerl-0.1.9/agilerl/utils/cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 from __future__ import annotations
-from typing import Any, Dict, Optional
+
 import os
 import pickle as pkl
+from typing import Any
+
 
 class Cache:
-    def __init__(self, cache_init: Optional[Dict]=None) -> None:
+    def __init__(self, cache_init: dict | None = None) -> None:
         assert cache_init is None or isinstance(cache_init, dict)
         if cache_init is None:
             cache_init = {}
         self.cache = cache_init
         self.cache_hit_rate = 1.0
 
     def dump(self, file_name: str):
         if not os.path.exists(os.path.dirname(file_name)):
             os.makedirs(os.path.dirname(file_name))
-        with open(file_name, 'wb') as f:
+        with open(file_name, "wb") as f:
             pkl.dump(self.cache, f)
-    
+
     def load(self, file_name: str):
-        with open(file_name, 'rb') as f:
+        with open(file_name, "rb") as f:
             self.cache.update(pkl.load(f))
-    
-    def __getitem__(self, key: str) -> Dict:
+
+    def __getitem__(self, key: str) -> dict:
         self.cache_hit_rate = (self.cache_hit_rate * 0.99) + 0.01
         return self.cache[key]
-    
+
     def __setitem__(self, key: str, newvalue: Any):
         self.cache_hit_rate = self.cache_hit_rate * 0.99
         self.cache[key] = newvalue
-    
+
     def __contains__(self, key: str) -> bool:
         return key in self.cache
-    
+
     def __len__(self) -> int:
         return len(self.cache)
-    
+
     def items(self):
         return list(self.cache.items())
-    
+
     def keys(self):
         return list(self.cache.keys())
-    
+
     def values(self):
         return list(self.cache.values())
-    
-    def update(self, new_stuff: Dict):
+
+    def update(self, new_stuff: dict):
         self.cache.update(new_stuff)
-    
+
     def get_hit_rate(self):
         return self.cache_hit_rate
-    
+
     def get_cache(self):
         return self.cache
```

### Comparing `agilerl-0.1.8/agilerl/utils/ilql_utils.py` & `agilerl-0.1.9/agilerl/utils/ilql_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,84 +1,110 @@
 import os
-import sys
 import pickle as pkl
-from typing import Dict, Any, List
+import sys
 from collections import defaultdict
+from typing import Any, Dict, List
+
 import torch
 
+
 def convert_path(path):
     if path is None:
         return None
-    return os.path.join(os.path.dirname(os.path.realpath(__file__)), '../../', path)
+    return os.path.join(os.path.dirname(os.path.realpath(__file__)), "../../", path)
+
 
 def add_system_configs(cfg, accelerator):
-    cfg['system'] = {}
-    cfg['system']['device'] = str(accelerator.device)
-    cfg['system']['num_processes'] = accelerator.num_processes
-    cfg['system']['use_fp16'] = accelerator.use_fp16
-    return cfg['system']
+    cfg["system"] = {}
+    cfg["system"]["device"] = str(accelerator.device)
+    cfg["system"]["num_processes"] = accelerator.num_processes
+    cfg["system"]["use_fp16"] = accelerator.use_fp16
+    return cfg["system"]
+
 
 def to_bin(n, pad_to_size=None):
     bins = to_bin(n // 2) + [n % 2] if n > 1 else [n]
     if pad_to_size is None:
         return bins
-    return ([0]*(pad_to_size-len(bins)))+bins
+    return ([0] * (pad_to_size - len(bins))) + bins
+
 
 def strip_from_end(str_item, strip_key):
     return strip_from_beginning(str_item[::-1], strip_key[::-1])[::-1]
 
+
 def strip_from_beginning(str_item, strip_key):
-    if str_item[:len(strip_key)] == strip_key:
-        return str_item[len(strip_key):]
+    if str_item[: len(strip_key)] == strip_key:
+        return str_item[len(strip_key) :]
     return str_item
 
+
 def migrate_pkl(pkl_path):
     from wordle import wordle_game
-    sys.modules['wordle.wordle_mdp'] = wordle_game
-    with open(pkl_path, 'rb') as f:
+
+    sys.modules["wordle.wordle_mdp"] = wordle_game
+    with open(pkl_path, "rb") as f:
         d = pkl.load(f)
-    del sys.modules['wordle.wordle_mdp']
-    with open(pkl_path, 'wb') as f:
+    del sys.modules["wordle.wordle_mdp"]
+    with open(pkl_path, "wb") as f:
         pkl.dump(d, f)
 
+
 def convert_old_ad_model(model_path, dataset, multiple_transformers=False):
-    w = torch.load(model_path, map_location='cpu')
-    embs = w['model.transformer.wte.weight']
+    w = torch.load(model_path, map_location="cpu")
+    embs = w["model.transformer.wte.weight"]
     if embs.shape[0] < dataset.tokenizer.num_tokens():
-        w['model.transformer.wte.weight'] = torch.cat((embs, torch.zeros(dataset.tokenizer.num_tokens()-embs.shape[0], 
-                                                                         embs.shape[1])), dim=0)
-    head = w['model.lm_head.weight']
+        w["model.transformer.wte.weight"] = torch.cat(
+            (
+                embs,
+                torch.zeros(
+                    dataset.tokenizer.num_tokens() - embs.shape[0], embs.shape[1]
+                ),
+            ),
+            dim=0,
+        )
+    head = w["model.lm_head.weight"]
     if head.shape[0] < dataset.tokenizer.num_tokens():
-        w['model.lm_head.weight'] = torch.cat((head, torch.zeros(dataset.tokenizer.num_tokens()-head.shape[0], 
-                                                                 head.shape[1])), dim=0)
+        w["model.lm_head.weight"] = torch.cat(
+            (
+                head,
+                torch.zeros(
+                    dataset.tokenizer.num_tokens() - head.shape[0], head.shape[1]
+                ),
+            ),
+            dim=0,
+        )
     if multiple_transformers:
         for k, v in list(w.items()):
-            if k.startswith('model.'):
-                w['lm_policy.'+k[len('model.'):]] = v.clone()
-                w['lm_target.'+k[len('model.'):]] = v.clone()
+            if k.startswith("model."):
+                w["lm_policy." + k[len("model.") :]] = v.clone()
+                w["lm_target." + k[len("model.") :]] = v.clone()
     torch.save(w, model_path)
 
+
 def stack_dicts(dicts: List[Dict[str, Any]]):
     stacked = defaultdict(list)
     for item in dicts:
         for k, v in item.items():
             stacked[k].append(v)
     # rough quick check for dicts have the same set of keys, could be more rigorous
     assert len(set(map(len, stacked.values()))) == 1
     return stacked
 
+
 def unstack_dicts(stacked_dict: Dict[str, List[Any]]):
     dict_len = set(map(lambda x: len(list(x)), stacked_dict.values()))
     assert len(dict_len) == 1
     dicts = [{} for _ in range(dict_len.pop())]
     for k, v in stacked_dict.items():
         for i, item in enumerate(v):
             dicts[i][k] = item
     return dicts
 
+
 class PrecisionRecallAcc:
     def __init__(self, classes) -> None:
         self.precisions = {class_: [0, 0] for class_ in classes}
         self.recalls = {class_: [0, 0] for class_ in classes}
         self.correct = 0
         self.total = 0
 
@@ -88,16 +114,16 @@
             self.precisions[prediction_type][0] += correct
             self.precisions[prediction_type][1] += 1
         if actual_type in self.recalls:
             self.recalls[actual_type][0] += correct
             self.recalls[actual_type][1] += 1
         self.correct += correct
         self.total += 1
-    
+
     def return_summary(self):
         logs = {}
-        logs['accuracy'] = (self.correct / self.total, self.total)
+        logs["accuracy"] = (self.correct / self.total, self.total)
         for k, (a, b) in self.precisions.items():
-            logs[str(k)+'_precision'] = (a / b if b != 0 else -1, b)
+            logs[str(k) + "_precision"] = (a / b if b != 0 else -1, b)
         for k, (a, b) in self.recalls.items():
-            logs[str(k)+'_recall'] = (a / b if b != 0 else -1, b)
-        return logs
+            logs[str(k) + "_recall"] = (a / b if b != 0 else -1, b)
+        return logs
```

### Comparing `agilerl-0.1.8/agilerl/utils/load_objects.py` & `agilerl-0.1.9/agilerl/utils/load_objects.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,227 +1,313 @@
 import json
+
 import torch
+
 from agilerl.algorithms.bc_lm import BC_LM, BC_Evaluator, BC_Policy
-from agilerl.algorithms.ilql import ILQL, ILQL_Policy, ILQL_Evaluator, TopAdvantageNGrams
+from agilerl.algorithms.ilql import (
+    ILQL,
+    ILQL_Evaluator,
+    ILQL_Policy,
+    TopAdvantageNGrams,
+)
+from agilerl.data.rl_data import ConstantTokenReward, SepcifiedTokenReward
 from agilerl.networks.evolvable_gpt import EvolvableGPT
 from agilerl.utils.ilql_utils import convert_path
-from agilerl.data.rl_data import ConstantTokenReward, SepcifiedTokenReward
-from agilerl.wordle.policy import MixturePolicy, MonteCarloPolicy, OptimalPolicy, RandomMixturePolicy, RepeatPolicy, \
-    StartWordPolicy, UserPolicy, WrongPolicy
-from agilerl.wordle.wordle_dataset import WordleHumanDataset, WordleIterableDataset, WordleListDataset
+from agilerl.wordle.policy import (
+    MixturePolicy,
+    MonteCarloPolicy,
+    OptimalPolicy,
+    RandomMixturePolicy,
+    RepeatPolicy,
+    StartWordPolicy,
+    UserPolicy,
+    WrongPolicy,
+)
+from agilerl.wordle.wordle_dataset import (
+    WordleHumanDataset,
+    WordleIterableDataset,
+    WordleListDataset,
+)
 from agilerl.wordle.wordle_env import WordleEnvironment
+from agilerl.wordle.wordle_evaluators import (
+    Action_Ranking_Evaluator,
+    Action_Ranking_Evaluator_Adversarial,
+)
 from agilerl.wordle.wordle_game import Vocabulary
-from agilerl.wordle.wordle_evaluators import Action_Ranking_Evaluator, Action_Ranking_Evaluator_Adversarial
 
 registry = {}
 cache = {}
 
+
 def register(name):
     def add_f(f):
         registry[name] = f
         return f
+
     return add_f
 
+
 def load_item(config, *args, verbose=True):
     config = config.copy()
-    name = config.pop('name')
+    name = config.pop("name")
     if name not in registry:
         raise NotImplementedError
-    if 'cache_id' in config:
-        if (name, config['cache_id']) in cache:
+    if "cache_id" in config:
+        if (name, config["cache_id"]) in cache:
             if verbose:
                 print(f'loading from cache ({name}, {config["cache_id"]})')
-            return cache[(name, config['cache_id'])]
+            return cache[(name, config["cache_id"])]
     if verbose:
-        print(f'loading {name}: {config}')
+        print(f"loading {name}: {config}")
     item = registry[name](config, *args, verbose=verbose)
-    if 'cache_id' in config:
+    if "cache_id" in config:
         print(f'saving to cache ({name}, {config["cache_id"]})')
-        cache[(name, config['cache_id'])] = item
+        cache[(name, config["cache_id"])] = item
     return item
 
+
 def load_model(config, model, device, verbose=True):
     model = model.to(device)
-    if config['checkpoint_path'] is not None:
+    if config["checkpoint_path"] is not None:
+        if verbose:
+            print(
+                "loading %s state dict from: %s"
+                % (config["name"], convert_path(config["checkpoint_path"]))
+            )
+        chkpt_state_dict = torch.load(
+            convert_path(config["checkpoint_path"]), map_location="cpu"
+        )
+        model.load_state_dict(chkpt_state_dict, strict=config["strict_load"])
         if verbose:
-            print('loading %s state dict from: %s' % (config['name'], convert_path(config["checkpoint_path"])))
-        chkpt_state_dict = torch.load(convert_path(config['checkpoint_path']), map_location='cpu')
-        model.load_state_dict(chkpt_state_dict, strict=config['strict_load'])
-        if verbose: 
-            print('loaded.')
-    elif config['gpt_pretrained']:
-        if verbose:
-            print('loading %s state dict from: %s' % (config['name'], convert_path(config["gpt_checkpoint_path"])))
-        pretrained_state_dict = convert_path(config['gpt_checkpoint_path'])
-        model.model = EvolvableGPT.from_pretrained(model_type=config['gpt_model_type'],
-                                                   override_args=model.net_config,
-                                                   custom_sd=pretrained_state_dict)
+            print("loaded.")
+    elif config["gpt_pretrained"]:
+        if verbose:
+            print(
+                "loading %s state dict from: %s"
+                % (config["name"], convert_path(config["gpt_checkpoint_path"]))
+            )
+        pretrained_state_dict = convert_path(config["gpt_checkpoint_path"])
+        model.model = EvolvableGPT.from_pretrained(
+            model_type=config["gpt_model_type"],
+            override_args=model.net_config,
+            custom_sd=pretrained_state_dict,
+        )
         model.copy_model_to_actor_target()
     return model
 
-@register('constant_token_reward')
+
+@register("constant_token_reward")
 def load_constant_token_reward(config, device, verbose=True):
-    return ConstantTokenReward(config['c'])
+    return ConstantTokenReward(config["c"])
+
 
-@register('specified_token_reward')
+@register("specified_token_reward")
 def load_specified_token_reward(config, device, verbose=True):
-    with open(convert_path(config['token_file']), 'r') as f:
+    with open(convert_path(config["token_file"])) as f:
         token_data = {int(k): v for k, v in json.load(f).items()}
-    return SepcifiedTokenReward(token_data, config['scale'], config['shift'])
+    return SepcifiedTokenReward(token_data, config["scale"], config["shift"])
 
-@register('gpt2')
+
+@register("gpt2")
 def load_gpt2(config, verbose=True):
-    if config['from_pretrained']:
-        return EvolvableGPT.from_pretrained(config['gpt2_type'])
+    if config["from_pretrained"]:
+        return EvolvableGPT.from_pretrained(config["gpt2_type"])
     return EvolvableGPT()
 
-@register('bc_lm')
+
+@register("bc_lm")
 def load_bc_lm(config, device, verbose=True):
-    dataset = load_item(config['dataset'], device, verbose=verbose)
-    config.pop('dataset')
-    load_config = config.pop('load')
+    dataset = load_item(config["dataset"], device, verbose=verbose)
+    config.pop("dataset")
+    load_config = config.pop("load")
     model = BC_LM(**config, dataset=dataset, device=device)
     return load_model(load_config, model, device, verbose=verbose)
 
-@register('bc_policy')
+
+@register("bc_policy")
 def load_bc_policy(config, device, verbose=True):
-    bc_lm = load_item(config['bc_lm'], device, verbose=verbose)
-    return BC_Policy(bc_lm, config['kind'], **config['generation_kwargs'])
+    bc_lm = load_item(config["bc_lm"], device, verbose=verbose)
+    return BC_Policy(bc_lm, config["kind"], **config["generation_kwargs"])
+
 
-@register('bc_evaluator')
+@register("bc_evaluator")
 def load_bc_evaluator(config, device, verbose=True):
-    env = load_item(config['env'], device, verbose=verbose)
-    return BC_Evaluator(env, config['env'], config['kind'], **config['generation_kwargs'])
+    env = load_item(config["env"], device, verbose=verbose)
+    return BC_Evaluator(
+        env, config["env"], config["kind"], **config["generation_kwargs"]
+    )
 
-@register('per_token_iql')
+
+@register("per_token_iql")
 def load_per_token_iql(config, device, verbose=True):
-    dataset = load_item(config['dataset'], device, verbose=verbose)
-    config.pop('dataset')
-    load_config = config.pop('load')
+    dataset = load_item(config["dataset"], device, verbose=verbose)
+    config.pop("dataset")
+    load_config = config.pop("load")
     model = ILQL(**config, dataset=dataset, device=device)
     return load_model(load_config, model, device, verbose=verbose)
 
-@register('iql_policy')
+
+@register("iql_policy")
 def load_iql_policy(config, device, verbose=True):
-    iql_model = load_item(config['iql_model'], device, verbose=verbose)
-    return ILQL_Policy(iql_model, config['kind'], **config['generation_kwargs'])
+    iql_model = load_item(config["iql_model"], device, verbose=verbose)
+    return ILQL_Policy(iql_model, config["kind"], **config["generation_kwargs"])
 
-@register('iql_evaluator')
+
+@register("iql_evaluator")
 def load_iql_evaluator(config, device, verbose=True):
-    env = load_item(config['env'], device, verbose=verbose)
-    return ILQL_Evaluator(env, config['verbose'], config['kind'], **config['generation_kwargs'])
+    env = load_item(config["env"], device, verbose=verbose)
+    return ILQL_Evaluator(
+        env, config["verbose"], config["kind"], **config["generation_kwargs"]
+    )
+
 
-@register('top_advantage_n_grams')
+@register("top_advantage_n_grams")
 def load_top_advantage_n_grams(config, device, verbose=True):
-    data = load_item(config['data'], device, verbose=verbose)
-    return TopAdvantageNGrams(data, config['print_every'], config['print_k'], config['n_gram'])
+    data = load_item(config["data"], device, verbose=verbose)
+    return TopAdvantageNGrams(
+        data, config["print_every"], config["print_k"], config["n_gram"]
+    )
+
 
-@register('vocab')
+@register("vocab")
 def load_vocab(config, verbose=True):
-    vocab = Vocabulary.from_file(convert_path(config['vocab_path']), config['fill_cache'])
-    if config['cache_path'] is not None:
+    vocab = Vocabulary.from_file(
+        convert_path(config["vocab_path"]), config["fill_cache"]
+    )
+    if config["cache_path"] is not None:
         if verbose:
-            print('loading vocab cache from: %s' % convert_path(config['cache_path']))
-        vocab.cache.load(convert_path(config['cache_path']))
+            print("loading vocab cache from: %s" % convert_path(config["cache_path"]))
+        vocab.cache.load(convert_path(config["cache_path"]))
         if verbose:
-            print('loaded.')
+            print("loaded.")
     return vocab
 
-@register('wordle_env')
+
+@register("wordle_env")
 def load_wordle_environment(config, device, verbose=True):
-    vocab = load_item(config['vocab'], verbose=verbose)
+    vocab = load_item(config["vocab"], verbose=verbose)
     return WordleEnvironment(vocab)
 
-@register('user_policy')
+
+@register("user_policy")
 def load_user_policy(config, device, verbose=True):
     vocab, hint_policy = None, None
-    if config['hint_policy'] is not None:
-        hint_policy = load_item(config['hint_policy'], device, verbose=verbose)
-    if config['vocab'] is not None:
-        vocab = load_item(config['vocab'], verbose=verbose)
+    if config["hint_policy"] is not None:
+        hint_policy = load_item(config["hint_policy"], device, verbose=verbose)
+    if config["vocab"] is not None:
+        vocab = load_item(config["vocab"], verbose=verbose)
     return UserPolicy(hint_policy=hint_policy, vocab=vocab)
 
-@register('start_word_policy')
+
+@register("start_word_policy")
 def load_start_word_policy(config, device, verbose=True):
-    return StartWordPolicy(config['start_words'])
+    return StartWordPolicy(config["start_words"])
+
 
-@register('optimal_policy')
+@register("optimal_policy")
 def load_optimal_policy(config, device, verbose=True):
     start_word_policy = None
-    if config['start_word_policy'] is not None:
-        start_word_policy = load_item(config['start_word_policy'], device, verbose=verbose)
-    policy = OptimalPolicy(start_word_policy=start_word_policy, progress_bar=config['progress_bar'])
-    if config['cache_path'] is not None:
+    if config["start_word_policy"] is not None:
+        start_word_policy = load_item(
+            config["start_word_policy"], device, verbose=verbose
+        )
+    policy = OptimalPolicy(
+        start_word_policy=start_word_policy, progress_bar=config["progress_bar"]
+    )
+    if config["cache_path"] is not None:
         if verbose:
-            print('loading optimal policy cache from: %s' % convert_path(config['cache_path']))
-        policy.cache.load(convert_path(config['cache_path']))
+            print(
+                "loading optimal policy cache from: %s"
+                % convert_path(config["cache_path"])
+            )
+        policy.cache.load(convert_path(config["cache_path"]))
         if verbose:
-            print('loaded.')
+            print("loaded.")
     return policy
 
-@register('wrong_policy')
+
+@register("wrong_policy")
 def load_wrong_policy(config, device, verbose=True):
-    vocab = load_item(config['vocab'], verbose=verbose)
+    vocab = load_item(config["vocab"], verbose=verbose)
     return WrongPolicy(vocab=vocab)
 
-@register('repeat_policy')
+
+@register("repeat_policy")
 def load_repeat_policy(config, device, verbose=True):
     start_word_policy = None
-    if config['start_word_policy'] is not None:
-        start_word_policy = load_item(config['start_word_policy'], device, verbose=verbose)
-    return RepeatPolicy(start_word_policy=start_word_policy, first_n=config['first_n'])
+    if config["start_word_policy"] is not None:
+        start_word_policy = load_item(
+            config["start_word_policy"], device, verbose=verbose
+        )
+    return RepeatPolicy(start_word_policy=start_word_policy, first_n=config["first_n"])
 
-@register('mixture_policy')
+
+@register("mixture_policy")
 def load_mixture_policy(config, device, verbose=True):
-    policy1 = load_item(config['policy1'], device, verbose=verbose)
-    policy2 = load_item(config['policy2'], device, verbose=verbose)
-    return MixturePolicy(config['prob1'], policy1, policy2)
+    policy1 = load_item(config["policy1"], device, verbose=verbose)
+    policy2 = load_item(config["policy2"], device, verbose=verbose)
+    return MixturePolicy(config["prob1"], policy1, policy2)
+
 
-@register('random_mixture_policy')
+@register("random_mixture_policy")
 def load_random_mixture_policy(config, device, verbose=True):
     vocab = None
-    if config['vocab'] is not None:
-        vocab = load_item(config['vocab'], verbose=verbose)
-    return RandomMixturePolicy(prob_smart=config['prob_smart'], vocab=vocab)
+    if config["vocab"] is not None:
+        vocab = load_item(config["vocab"], verbose=verbose)
+    return RandomMixturePolicy(prob_smart=config["prob_smart"], vocab=vocab)
+
 
-@register('monte_carlo_policy')
+@register("monte_carlo_policy")
 def load_monte_carlo_policy(config, device, verbose=True):
-    sample_policy = load_item(config['sample_policy'], device, verbose=verbose)
-    return MonteCarloPolicy(n_samples=config['n_samples'], sample_policy=sample_policy)
+    sample_policy = load_item(config["sample_policy"], device, verbose=verbose)
+    return MonteCarloPolicy(n_samples=config["n_samples"], sample_policy=sample_policy)
 
-@register('wordle_iterable_dataset')
+
+@register("wordle_iterable_dataset")
 def load_wordle_iterable_dataset(config, device, verbose=True):
-    policy = load_item(config['policy'], device, verbose=verbose)
-    vocab = load_item(config['vocab'], verbose=verbose)
-    token_reward = load_item(config['token_reward'], device, verbose=verbose)
-    return WordleIterableDataset(policy, vocab, max_len=config['max_len'], token_reward=token_reward)
+    policy = load_item(config["policy"], device, verbose=verbose)
+    vocab = load_item(config["vocab"], verbose=verbose)
+    token_reward = load_item(config["token_reward"], device, verbose=verbose)
+    return WordleIterableDataset(
+        policy, vocab, max_len=config["max_len"], token_reward=token_reward
+    )
+
 
-@register('wordle_dataset')
+@register("wordle_dataset")
 def load_wordle_dataset(config, device, verbose=True):
-    if config['vocab'] is not None:
-        vocab = load_item(config['vocab'], verbose=verbose)
+    if config["vocab"] is not None:
+        vocab = load_item(config["vocab"], verbose=verbose)
     else:
         vocab = None
-    token_reward = load_item(config['token_reward'], device, verbose=verbose)
-    return WordleListDataset.from_file(convert_path(config['file_path']), config['max_len'], vocab, token_reward)
+    token_reward = load_item(config["token_reward"], device, verbose=verbose)
+    return WordleListDataset.from_file(
+        convert_path(config["file_path"]), config["max_len"], vocab, token_reward
+    )
 
-@register('wordle_human_dataset')
+
+@register("wordle_human_dataset")
 def load_human_dataset(config, device, verbose=True):
-    token_reward = load_item(config['token_reward'], device, verbose=verbose)
+    token_reward = load_item(config["token_reward"], device, verbose=verbose)
     game_indexes = None
-    if config['index_file'] is not None:
-        with open(convert_path(config['index_file']), 'r') as f:
+    if config["index_file"] is not None:
+        with open(convert_path(config["index_file"])) as f:
             game_indexes = json.load(f)
-    return WordleHumanDataset.from_file(convert_path(config['file_path']), config['use_true_word'], 
-                                        config['max_len'], token_reward, 
-                                        game_indexes, config['top_p'])
+    return WordleHumanDataset.from_file(
+        convert_path(config["file_path"]),
+        config["use_true_word"],
+        config["max_len"],
+        token_reward,
+        game_indexes,
+        config["top_p"],
+    )
+
 
-@register('action_ranking_evaluator')
+@register("action_ranking_evaluator")
 def load_action_ranking_evaluator(config, device, verbose=True):
-    branching_data = load_item(config['branching_data'], device, verbose=verbose)
+    branching_data = load_item(config["branching_data"], device, verbose=verbose)
     return Action_Ranking_Evaluator(branching_data)
 
-@register('action_ranking_evaluator_adversarial')
+
+@register("action_ranking_evaluator_adversarial")
 def load_action_ranking_evaluator_adversarial(config, device, verbose=True):
-    adversarial_data = load_item(config['adversarial_data'], device, verbose=verbose)
+    adversarial_data = load_item(config["adversarial_data"], device, verbose=verbose)
     return Action_Ranking_Evaluator_Adversarial(adversarial_data)
-
```

### Comparing `agilerl-0.1.8/agilerl/utils/log_utils.py` & `agilerl-0.1.9/agilerl/utils/log_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,65 +1,71 @@
+import json
+
 import torch
-import wandb
 from flatten_dict import flatten, unflatten
-import json
+
+import wandb
+
 
 class DistributeCombineLogs:
-    count_tag = '__count__'
+    count_tag = "__count__"
 
     def __init__(self, accelerator, use_wandb=False):
         self.totals = {}
         self.accelerator = accelerator
         self.use_wandb = use_wandb
 
     def convert_key(self, k):
-        return (self.count_tag,)+k
-    
+        return (self.count_tag,) + k
+
     def key_is_count(self, k):
         return k[0] == self.count_tag
-    
+
     def log(self, *postproc_funcs, **additional_items):
         self.accelerator.wait_for_everyone()
         total_logs = self.gather_logs(*postproc_funcs, **additional_items)
         if self.accelerator.is_main_process:
             if self.use_wandb:
                 wandb.log(total_logs)
             print(total_logs)
         self.accelerator.wait_for_everyone()
         return total_logs
-    
+
     def accum_logs(self, logs):
         logs = flatten(logs)
         for k, (item, n) in logs.items():
             new_item = torch.tensor([item]).float().to(self.accelerator.device)
             count_item = torch.tensor([n]).float().to(self.accelerator.device)
             if k in self.totals:
-                self.totals[k] += new_item*count_item
+                self.totals[k] += new_item * count_item
                 self.totals[self.convert_key(k)] += count_item
             else:
-                self.totals[k] = new_item*count_item
+                self.totals[k] = new_item * count_item
                 self.totals[self.convert_key(k)] = count_item
 
     def gather_logs(self, *postproc_funcs, **additional_items):
         str_totals = {json.dumps(list(k)): v for k, v in self.totals.items()}
         combined_totals = self.accelerator.gather(str_totals)
-        combined_totals = {tuple(json.loads(k)): v.sum().item() for k, v in combined_totals.items()}
+        combined_totals = {
+            tuple(json.loads(k)): v.sum().item() for k, v in combined_totals.items()
+        }
         final_logs = {}
         for k, v in combined_totals.items():
             if not self.key_is_count(k):
                 if combined_totals[self.convert_key(k)] == 0:
-                    final_logs[k] = v * float('inf')
+                    final_logs[k] = v * float("inf")
                 else:
                     final_logs[k] = v / combined_totals[self.convert_key(k)]
         final_logs = unflatten(final_logs)
         for f in postproc_funcs:
             result = f(final_logs)
             if result is not None:
                 final_logs = result
         final_logs = {**final_logs, **additional_items}
         return final_logs
 
     def reset_logs(self):
         self.totals = {}
 
+
 def label_logs(logs, label):
-    return {label: logs}
+    return {label: logs}
```

### Comparing `agilerl-0.1.8/agilerl/utils/minari_utils.py` & `agilerl-0.1.9/agilerl/utils/minari_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,88 +1,90 @@
 import os
+
+import h5py
 import minari
+from minari.storage.datasets_root_dir import get_dataset_path
 from minari.storage.hosting import download_dataset
 from minari.storage.local import load_dataset
-from minari.storage.datasets_root_dir import get_dataset_path
-import h5py
+
 
 def load_minari_dataset(dataset_id, accelerator=None, remote=False):
-    
-    if remote:    
+    if remote:
         if dataset_id not in list(minari.list_remote_datasets().keys()):
-            raise KeyError("Enter a valid remote Minari Dataset ID. check https://minari.farama.org/ for more details.")
-        
+            raise KeyError(
+                "Enter a valid remote Minari Dataset ID. check https://minari.farama.org/ for more details."
+            )
+
     file_path = get_dataset_path(dataset_id)
 
     if not os.path.exists(file_path):
         if remote:
             if accelerator is not None:
                 accelerator.wait_for_everyone()
                 if accelerator.is_main_process:
                     print("download dataset: ", dataset_id)
                     download_dataset(dataset_id)
                 accelerator.wait_for_everyone()
             else:
                 print("download dataset: ", dataset_id)
                 download_dataset(dataset_id)
         else:
-            raise FileNotFoundError(f"No local Dataset found for dataset id {dataset_id}. check https://minari.farama.org/ for more details on remote dataset. For loading a remote dataset assign remote=True")
-    
+            raise FileNotFoundError(
+                f"No local Dataset found for dataset id {dataset_id}. check https://minari.farama.org/ for more details on remote dataset. For loading a remote dataset assign remote=True"
+            )
+
     minari_dataset = load_dataset(dataset_id)
-    
+
     return minari_dataset
 
+
 def MinariToAgileBuffer(dataset_id, memory, accelerator=None, remote=False):
-    
     minari_dataset = load_minari_dataset(dataset_id, accelerator, remote)
-    
+
     for episode in minari_dataset.iterate_episodes():
-        
         for num_steps in range(0, len(episode.rewards)):
-            
             observation = episode.observations[num_steps]
-            next_observation = episode.observations[num_steps+1]
+            next_observation = episode.observations[num_steps + 1]
             action = episode.actions[num_steps]
             reward = episode.rewards[num_steps]
             terminal = episode.terminations[num_steps]
             memory.save2memory(observation, action, reward, next_observation, terminal)
-    
+
     return memory
 
+
 def MinariToAgileDataset(dataset_id, remote=False):
-    
     observations = []
     next_observations = []
     actions = []
     rewards = []
     terminals = []
 
     minari_dataset = load_minari_dataset(dataset_id, remote)
-    
+
     for episode in minari_dataset.iterate_episodes():
-        
         observations.extend(episode.observations[:-1])
         next_observations.extend(episode.observations[1:])
         actions.extend(episode.actions[:])
         rewards.extend(episode.rewards[:])
         terminals.extend(episode.terminations[:])
 
     agile_dataset_id = dataset_id.split("-")
-    agile_dataset_id[0] = agile_dataset_id[0] + '_agile'
+    agile_dataset_id[0] = agile_dataset_id[0] + "_agile"
     agile_dataset_id = "-".join(agile_dataset_id)
-    
+
     agile_file_path = get_dataset_path(agile_dataset_id)
-    
+
     agile_dataset_path = os.path.join(agile_file_path, "data")
     os.makedirs(agile_dataset_path, exist_ok=True)
     data_path = os.path.join(agile_dataset_path, "main_data.hdf5")
 
     # with h5py.File(os.path.join(agile_file_path, "data", "main_data.hdf5"), "w") as f:
-    f = h5py.File(data_path, 'w')
-    
-    f.create_dataset('observations', data=observations)
-    f.create_dataset('next_observations', data=next_observations)
-    f.create_dataset('actions', data=actions)
-    f.create_dataset('rewards', data=rewards)
-    f.create_dataset('terminals', data=terminals)
-    
-    return f
+    f = h5py.File(data_path, "w")
+
+    f.create_dataset("observations", data=observations)
+    f.create_dataset("next_observations", data=next_observations)
+    f.create_dataset("actions", data=actions)
+    f.create_dataset("rewards", data=rewards)
+    f.create_dataset("terminals", data=terminals)
+
+    return f
```

### Comparing `agilerl-0.1.8/agilerl/utils/sampling_utils.py` & `agilerl-0.1.9/agilerl/utils/sampling_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,84 @@
+import numpy as np
 import torch
 import torch.nn.functional as F
-import numpy as np
+
 
 def select_batch_idxs(x, idxs):
-    return torch.gather(x, dim=0, 
-                        index=idxs.repeat(*x.shape[1:], 1).permute(len(x.shape) - 1, *list(range(len(x.shape) - 1))))
+    return torch.gather(
+        x,
+        dim=0,
+        index=idxs.repeat(*x.shape[1:], 1).permute(
+            len(x.shape) - 1, *list(range(len(x.shape) - 1))
+        ),
+    )
+
 
 def map_all_kvs(f, kvs):
     return tuple([tuple(map(f, items)) for items in kvs])
 
+
 def map_decoder_kvs(f, kvs):
     return tuple([(tuple(map(f, items[:2])) + tuple(items[2:])) for items in kvs])
 
+
 def pad_sequence(seq, to_len, val, device, dim):
-    return torch.cat((seq, torch.full(
-        (*seq.shape[:dim], to_len - seq.shape[dim], *seq.shape[dim + 1:]), val).to(device)), dim=dim)
+    return torch.cat(
+        (
+            seq,
+            torch.full(
+                (*seq.shape[:dim], to_len - seq.shape[dim], *seq.shape[dim + 1 :]), val
+            ).to(device),
+        ),
+        dim=dim,
+    )
+
 
 def update_kvs(kvs, updated_kvs, lens_chosen, idx):
     for i, layer in enumerate(kvs):
         for x, item in enumerate(layer):
             item[lens_chosen, :, idx, :] = updated_kvs[i][x][:, :, idx, :]
     return kvs
 
+
 def update_decoder_kvs(kvs, updated_kvs, lens_chosen, idx):
     for i, layer in enumerate(kvs):
         for x, item in enumerate(layer[:2]):
             item[lens_chosen, :, idx, :] = updated_kvs[i][x][:, :, idx, :]
     return kvs
 
+
 def get_relevent_kvs(kvs, lens_chosen, idx):
     kvs = map_all_kvs(lambda x: select_batch_idxs(x, lens_chosen), kvs)
-    kvs = map_all_kvs(lambda x: x[:,:,:idx,:], kvs)
+    kvs = map_all_kvs(lambda x: x[:, :, :idx, :], kvs)
     return kvs
 
+
 def top_k_logits(logits, k):
     # logits = (batch, time, dim)
-    _, bottom_k_idx = torch.topk(-logits, logits.shape[2]-k, dim=2)
-    return torch.scatter(logits, dim=2, index=bottom_k_idx, value=float('-inf'))
+    _, bottom_k_idx = torch.topk(-logits, logits.shape[2] - k, dim=2)
+    return torch.scatter(logits, dim=2, index=bottom_k_idx, value=float("-inf"))
+
 
 def top_p_logits(logits, p):
     # logits = (batch, time, dim)
     sorted_logits, _ = torch.sort(logits, dim=2, descending=True)
-    num_to_take = torch.sum(torch.cumsum(F.softmax(sorted_logits, dim=2), dim=2) <= p, dim=2).unsqueeze(2)
-    mask = logits < torch.gather(sorted_logits, dim=2, index=torch.clamp(num_to_take, max=logits.shape[2]-1))
-    return logits.masked_fill(mask, float('-inf'))
+    num_to_take = torch.sum(
+        torch.cumsum(F.softmax(sorted_logits, dim=2), dim=2) <= p, dim=2
+    ).unsqueeze(2)
+    mask = logits < torch.gather(
+        sorted_logits, dim=2, index=torch.clamp(num_to_take, max=logits.shape[2] - 1)
+    )
+    return logits.masked_fill(mask, float("-inf"))
+
 
 def process_logits(logits, temp=1.0, top_k=None, top_p=None):
     logits /= temp
     if top_k is not None:
         logits = top_k_logits(logits, top_k)
     if top_p is not None:
         logits = top_p_logits(logits, top_p)
     return logits
 
+
 def always_terminate(s: np.ndarray):
     return True
-
```

### Comparing `agilerl-0.1.8/agilerl/utils/serve_queue.py` & `agilerl-0.1.9/agilerl/utils/serve_queue.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,121 @@
-from typing import Generator
-import redis
-import time
-import pickle as pkl
 import multiprocessing as mp
+import pickle as pkl
+import time
 from functools import partial
+from typing import Generator
+
+import redis
+
 
 class Config:
-    redis_host = 'localhost'
+    redis_host = "localhost"
     redis_port = 6379
     redis_db = 0
     client_refresh_delay = 0.01
-    self_indicator = '__self__'
-    init_message = '__init_message__'
+    self_indicator = "__self__"
+    init_message = "__init_message__"
+
 
 def serve_class(ModelCls):
     cache_cls = pkl.dumps(ModelCls)
+
     class WrappedModel:
         def __init__(self, *args, **kwargs):
-            self.r = redis.Redis(host=Config.redis_host, port=Config.redis_port, db=Config.redis_db)
-            self.Q = initalize_server(self, super().__getattribute__(
-                'r'), cache_cls, args, kwargs)
-        
+            self.r = redis.Redis(
+                host=Config.redis_host, port=Config.redis_port, db=Config.redis_db
+            )
+            self.Q = initalize_server(
+                self, super().__getattribute__("r"), cache_cls, args, kwargs
+            )
+
         def __getattribute__(self, name):
-            return partial(build_method(name, super().__getattribute__(
-                'r'), super().__getattribute__('Q')), self)
-    
+            return partial(
+                build_method(
+                    name, super().__getattribute__("r"), super().__getattribute__("Q")
+                ),
+                self,
+            )
+
         def __call__(self, *args, **kwargs):
-            return build_method('__call__',  super().__getattribute__(
-                'r'), super().__getattribute__('Q'))(self, *args, **kwargs)
-        
+            return build_method(
+                "__call__", super().__getattribute__("r"), super().__getattribute__("Q")
+            )(self, *args, **kwargs)
+
         def __getitem__(self, key):
-            return build_method('__getitem__',  super().__getattribute__(
-                'r'), super().__getattribute__('Q'))(self, key)
-        
+            return build_method(
+                "__getitem__",
+                super().__getattribute__("r"),
+                super().__getattribute__("Q"),
+            )(self, key)
+
         def __setitem__(self, key, value):
-            return build_method('__setitem__',  super().__getattribute__(
-                'r'), super().__getattribute__('Q'))(self, key, value)
-        
+            return build_method(
+                "__setitem__",
+                super().__getattribute__("r"),
+                super().__getattribute__("Q"),
+            )(self, key, value)
+
         def __contains__(self, key):
-            return build_method('__contains__',  super().__getattribute__(
-                'r'), super().__getattribute__('Q'))(self, key)
-        
+            return build_method(
+                "__contains__",
+                super().__getattribute__("r"),
+                super().__getattribute__("Q"),
+            )(self, key)
+
         def __len__(self):
-            return build_method('__len__',  super().__getattribute__(
-                'r'), super().__getattribute__('Q'))(self)
+            return build_method(
+                "__len__", super().__getattribute__("r"), super().__getattribute__("Q")
+            )(self)
+
     return WrappedModel
 
+
 def build_method(method, r, Q):
     def call_method(self, *args, **kwargs):
-        request_id = int(r.incr('request_id_counter'))
-        Q.put((request_id, method, args, kwargs,))
-        while not r.exists(f'result_{request_id}'):
+        request_id = int(r.incr("request_id_counter"))
+        Q.put(
+            (
+                request_id,
+                method,
+                args,
+                kwargs,
+            )
+        )
+        while not r.exists(f"result_{request_id}"):
             time.sleep(Config.client_refresh_delay)
-        result = pkl.loads(r.get(f'result_{request_id}'))
-        r.delete(f'result_{request_id}')
+        result = pkl.loads(r.get(f"result_{request_id}"))
+        r.delete(f"result_{request_id}")
         if result == Config.self_indicator:
             return self
         return result
+
     return call_method
 
+
 def server_process(Q, ModelCls_pkl, args, kwargs):
     r = redis.Redis(host=Config.redis_host, port=Config.redis_port, db=Config.redis_db)
     model = pkl.loads(ModelCls_pkl)(*args, **kwargs)
     while True:
         try:
             request_id, method, args, kwargs = Q.get()
             if method == Config.init_message:
-                r.set(f'result_{request_id}', pkl.dumps(method))
+                r.set(f"result_{request_id}", pkl.dumps(method))
                 continue
             result = getattr(model, method)(*args, **kwargs)
             if isinstance(result, Generator):
                 result = tuple(result)
             if result == model:
                 result = Config.self_indicator
-            r.set(f'result_{request_id}', pkl.dumps(result))
+            r.set(f"result_{request_id}", pkl.dumps(result))
         except EOFError:
             return
         except Exception:
             raise Exception
 
+
 def initalize_server(self, r, ModelCls_pkl, args, kwargs):
     Q = mp.Manager().Queue()
     p = mp.Process(target=server_process, args=(Q, ModelCls_pkl, args, kwargs))
     p.start()
     build_method(Config.init_message, r, Q)(self)
     return Q
```

### Comparing `agilerl-0.1.8/agilerl/utils/torch_utils.py` & `agilerl-0.1.9/agilerl/utils/torch_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,54 @@
-from typing import Any, List, Callable, Union
+import math
+from typing import Any, Callable, List, Union
+
+import numpy as np
 import torch
 import torch.nn as nn
-import numpy as np
-import math
 
-def map_pytree(f: Callable[[Union[np.ndarray, torch.Tensor]], Any], 
-               item: Any):
+
+def map_pytree(f: Callable[[Union[np.ndarray, torch.Tensor]], Any], item: Any):
     if isinstance(item, dict):
         return {k: map_pytree(f, v) for k, v in item.items()}
     elif isinstance(item, list) or isinstance(item, set) or isinstance(item, tuple):
         return [map_pytree(f, v) for v in item]
     elif isinstance(item, np.ndarray) or isinstance(item, torch.Tensor):
         return f(item)
     else:
         return item
 
+
 def to(item: Any, device: torch.device):
     return map_pytree(lambda x: torch.tensor(x).to(device), item)
 
+
 def to_decorator(f, device):
     def new_f(*args, **kwargs):
         return to(f(*args, **kwargs), device)
+
     return new_f
 
+
 def parameter_norm(model: nn.Module):
     norm = 0.0
     for param in model.parameters():
         norm += (param.norm() ** 2).item()
     return math.sqrt(norm)
 
-def get_transformer_logs(attentions: List[torch.Tensor], model: nn.Module, attn_mask: torch.Tensor):
+
+def get_transformer_logs(
+    attentions: List[torch.Tensor], model: nn.Module, attn_mask: torch.Tensor
+):
     logs = {}
     n = attn_mask.sum()
-    model_attention_entropy = -sum(map(
-        lambda x: ((x * torch.log(x+1e-7)).sum(
-        dim=-1) * attn_mask.unsqueeze(1)).sum().item(), attentions)) / (len(attentions) * n)
+    model_attention_entropy = -sum(
+        map(
+            lambda x: ((x * torch.log(x + 1e-7)).sum(dim=-1) * attn_mask.unsqueeze(1))
+            .sum()
+            .item(),
+            attentions,
+        )
+    ) / (len(attentions) * n)
     model_parameter_norm = parameter_norm(model)
-    logs['attention_entropy'] = (model_attention_entropy, n * len(attentions))
-    logs['parameter_norm'] = (model_parameter_norm, 1)
+    logs["attention_entropy"] = (model_attention_entropy, n * len(attentions))
+    logs["parameter_norm"] = (model_parameter_norm, 1)
     return logs
```

### Comparing `agilerl-0.1.8/agilerl/utils/utils.py` & `agilerl-0.1.9/agilerl/utils/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 import gymnasium as gym
-import numpy as np
 import matplotlib.pyplot as plt
+import numpy as np
+
 from agilerl.algorithms.cqn import CQN
-from agilerl.algorithms.dqn import DQN
 from agilerl.algorithms.ddpg import DDPG
-from agilerl.algorithms.td3 import TD3
+from agilerl.algorithms.dqn import DQN
 from agilerl.algorithms.maddpg import MADDPG
 from agilerl.algorithms.matd3 import MATD3
+from agilerl.algorithms.td3 import TD3
 
 
 def makeVectEnvs(env_name, num_envs=1):
     """Returns async-vectorized gym environments.
 
     :param env_name: Gym environment name
     :type env_name: str
     :param num_envs: Number of vectorized environments, defaults to 1
     :type num_envs: int, optional
     """
     return gym.vector.AsyncVectorEnv(
-        [lambda: gym.make(env_name) for i in range(num_envs)])
+        [lambda: gym.make(env_name) for i in range(num_envs)]
+    )
 
 
-def initialPopulation(algo, state_dim, action_dim, one_hot,
-                      net_config, INIT_HP, population_size=1, device='cpu', 
-                      accelerator=None):
+def initialPopulation(
+    algo,
+    state_dim,
+    action_dim,
+    one_hot,
+    net_config,
+    INIT_HP,
+    population_size=1,
+    device="cpu",
+    accelerator=None,
+):
     """Returns population of identical agents.
 
     :param algo: RL algorithm
     :type algo: str
     :param state_dim: State observation dimension
     :type state_dim: int
     :param action_dim: Action dimension
@@ -41,152 +51,154 @@
     :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
     :type device: str, optional
     :param accelerator: Accelerator for distributed computing, defaults to None
     :type accelerator: Hugging Face accelerate.Accelerator(), optional
     """
     population = []
 
-    if algo == 'DQN':
+    if algo == "DQN":
         for idx in range(population_size):
             agent = DQN(
                 state_dim=state_dim,
                 action_dim=action_dim,
                 one_hot=one_hot,
                 index=idx,
                 net_config=net_config,
-                batch_size=INIT_HP['BATCH_SIZE'],
-                lr=INIT_HP['LR'],
-                learn_step=INIT_HP['LEARN_STEP'],
-                gamma=INIT_HP['GAMMA'],
-                tau=INIT_HP['TAU'],
-                double=INIT_HP['DOUBLE'],
+                batch_size=INIT_HP["BATCH_SIZE"],
+                lr=INIT_HP["LR"],
+                learn_step=INIT_HP["LEARN_STEP"],
+                gamma=INIT_HP["GAMMA"],
+                tau=INIT_HP["TAU"],
+                double=INIT_HP["DOUBLE"],
                 device=device,
-                accelerator=accelerator
+                accelerator=accelerator,
             )
             population.append(agent)
 
-    elif algo == 'DDPG':
+    elif algo == "DDPG":
         for idx in range(population_size):
             agent = DDPG(
                 state_dim=state_dim,
                 action_dim=action_dim,
                 one_hot=one_hot,
                 index=idx,
                 net_config=net_config,
-                batch_size=INIT_HP['BATCH_SIZE'],
-                lr=INIT_HP['LR'],
-                learn_step=INIT_HP['LEARN_STEP'],
-                gamma=INIT_HP['GAMMA'],
-                tau=INIT_HP['TAU'],
-                policy_freq=INIT_HP['POLICY_FREQ'],
+                batch_size=INIT_HP["BATCH_SIZE"],
+                lr=INIT_HP["LR"],
+                learn_step=INIT_HP["LEARN_STEP"],
+                gamma=INIT_HP["GAMMA"],
+                tau=INIT_HP["TAU"],
+                policy_freq=INIT_HP["POLICY_FREQ"],
                 device=device,
-                accelerator=accelerator
+                accelerator=accelerator,
             )
             population.append(agent)
 
-    elif algo == 'CQN':
+    elif algo == "CQN":
         for idx in range(population_size):
             agent = CQN(
                 state_dim=state_dim,
                 action_dim=action_dim,
                 one_hot=one_hot,
                 index=idx,
                 net_config=net_config,
-                batch_size=INIT_HP['BATCH_SIZE'],
-                lr=INIT_HP['LR'],
-                learn_step=INIT_HP['LEARN_STEP'],
-                gamma=INIT_HP['GAMMA'],
-                tau=INIT_HP['TAU'],
-                double=INIT_HP['DOUBLE'],
+                batch_size=INIT_HP["BATCH_SIZE"],
+                lr=INIT_HP["LR"],
+                learn_step=INIT_HP["LEARN_STEP"],
+                gamma=INIT_HP["GAMMA"],
+                tau=INIT_HP["TAU"],
+                double=INIT_HP["DOUBLE"],
                 device=device,
-                accelerator=accelerator
+                accelerator=accelerator,
             )
             population.append(agent)
 
-    elif algo == 'TD3':
+    elif algo == "TD3":
         for idx in range(population_size):
             agent = TD3(
                 state_dim=state_dim,
                 action_dim=action_dim,
                 one_hot=one_hot,
-                max_action=INIT_HP['MAX_ACTION'],
+                max_action=INIT_HP["MAX_ACTION"],
                 index=idx,
                 net_config=net_config,
-                batch_size=INIT_HP['BATCH_SIZE'],
-                lr=INIT_HP['LR'],
-                learn_step=INIT_HP['LEARN_STEP'],
-                gamma=INIT_HP['GAMMA'],
-                tau=INIT_HP['TAU'],
-                policy_freq=INIT_HP['POLICY_FREQ'],
+                batch_size=INIT_HP["BATCH_SIZE"],
+                lr=INIT_HP["LR"],
+                learn_step=INIT_HP["LEARN_STEP"],
+                gamma=INIT_HP["GAMMA"],
+                tau=INIT_HP["TAU"],
+                policy_freq=INIT_HP["POLICY_FREQ"],
                 device=device,
-                accelerator=accelerator
+                accelerator=accelerator,
             )
             population.append(agent)
 
-    elif algo == 'MADDPG':
+    elif algo == "MADDPG":
         for idx in range(population_size):
             agent = MADDPG(
                 state_dims=state_dim,
                 action_dims=action_dim,
                 one_hot=one_hot,
-                n_agents=INIT_HP['N_AGENTS'],
-                agent_ids=INIT_HP['AGENT_IDS'],
+                n_agents=INIT_HP["N_AGENTS"],
+                agent_ids=INIT_HP["AGENT_IDS"],
                 index=idx,
-                max_action = INIT_HP['MAX_ACTION'],
-                min_action = INIT_HP['MIN_ACTION'],
+                max_action=INIT_HP["MAX_ACTION"],
+                min_action=INIT_HP["MIN_ACTION"],
                 net_config=net_config,
-                batch_size=INIT_HP['BATCH_SIZE'],
-                lr=INIT_HP['LR'],
-                learn_step=INIT_HP['LEARN_STEP'],
-                gamma=INIT_HP['GAMMA'],
-                tau=INIT_HP['TAU'],
-                discrete_actions=INIT_HP['DISCRETE_ACTIONS'],
+                batch_size=INIT_HP["BATCH_SIZE"],
+                lr=INIT_HP["LR"],
+                learn_step=INIT_HP["LEARN_STEP"],
+                gamma=INIT_HP["GAMMA"],
+                tau=INIT_HP["TAU"],
+                discrete_actions=INIT_HP["DISCRETE_ACTIONS"],
                 device=device,
                 accelerator=accelerator,
             )
             population.append(agent)
 
-    elif algo == 'MATD3':
+    elif algo == "MATD3":
         for idx in range(population_size):
             agent = MATD3(
                 state_dims=state_dim,
                 action_dims=action_dim,
                 one_hot=one_hot,
-                n_agents=INIT_HP['N_AGENTS'],
-                agent_ids=INIT_HP['AGENT_IDS'],
+                n_agents=INIT_HP["N_AGENTS"],
+                agent_ids=INIT_HP["AGENT_IDS"],
                 index=idx,
-                max_action = INIT_HP['MAX_ACTION'],
-                min_action = INIT_HP['MIN_ACTION'],
+                max_action=INIT_HP["MAX_ACTION"],
+                min_action=INIT_HP["MIN_ACTION"],
                 net_config=net_config,
-                batch_size=INIT_HP['BATCH_SIZE'],
-                lr=INIT_HP['LR'],
-                policy_freq=INIT_HP['POLICY_FREQ'],
-                learn_step=INIT_HP['LEARN_STEP'],
-                gamma=INIT_HP['GAMMA'],
-                tau=INIT_HP['TAU'],
-                discrete_actions=INIT_HP['DISCRETE_ACTIONS'],
+                batch_size=INIT_HP["BATCH_SIZE"],
+                lr=INIT_HP["LR"],
+                policy_freq=INIT_HP["POLICY_FREQ"],
+                learn_step=INIT_HP["LEARN_STEP"],
+                gamma=INIT_HP["GAMMA"],
+                tau=INIT_HP["TAU"],
+                discrete_actions=INIT_HP["DISCRETE_ACTIONS"],
                 device=device,
                 accelerator=accelerator,
             )
             population.append(agent)
 
-
     return population
 
 
 def printHyperparams(pop):
     """Prints current hyperparameters of agents in a population and their fitnesses.
 
     :param pop: Population of agents
     :type pop: List[object]
     """
-    
+
     for agent in pop:
-        print('Agent ID: {}    Mean 100 fitness: {:.2f}    lr: {}    Batch Size: {}'.format(
-            agent.index, np.mean(agent.fitness[-100:]), agent.lr, agent.batch_size))
+        print(
+            "Agent ID: {}    Mean 100 fitness: {:.2f}    lr: {}    Batch Size: {}".format(
+                agent.index, np.mean(agent.fitness[-100:]), agent.lr, agent.batch_size
+            )
+        )
 
 
 def plotPopulationScore(pop):
     """Plots the fitness scores of agents in a population.
 
     :param pop: Population of agents
     :type pop: List[object]
```

### Comparing `agilerl-0.1.8/agilerl/wordle/policy.py` & `agilerl-0.1.9/agilerl/wordle/policy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,106 +1,151 @@
-from collections import defaultdict
-from typing import Union
+import math
 import random
-from typing import List, Optional
+from collections import defaultdict
+from typing import List, Optional, Union
+
+from tqdm.auto import tqdm
+
+from agilerl.data.language_environment import Policy
 from agilerl.utils.cache import Cache
 from agilerl.wordle.wordle_env import WordleObservation
 from agilerl.wordle.wordle_game import Vocabulary
-import math
-from tqdm.auto import tqdm
-from agilerl.data.language_environment import Policy
+
 
 class UserPolicy(Policy):
-    def __init__(self, hint_policy: Optional[Policy], vocab: Optional[Union[str, Vocabulary]]):
+    def __init__(
+        self, hint_policy: Optional[Policy], vocab: Optional[Union[str, Vocabulary]]
+    ):
         super().__init__()
         self.vocab = vocab
         if isinstance(self.vocab, str):
             self.vocab = Vocabulary.from_file(self.vocab)
         self.hint_policy = hint_policy
 
     def act(self, obs: WordleObservation) -> str:
         print(obs.game)
         while True:
             if self.hint_policy is not None:
-                want_a_hint = input('hint? ')
-                if want_a_hint.lower() == 'y' or want_a_hint.lower() == 'yes':
+                want_a_hint = input("hint? ")
+                if want_a_hint.lower() == "y" or want_a_hint.lower() == "yes":
                     result = self.hint_policy.act(obs)
                     print()
                     return result
             result = input("Enter a word: ")
             if len(result) != 5:
                 print("Please enter a 5 letter word.")
             elif (self.vocab is not None) and (result not in self.vocab.all_vocab):
-                print('Not a word. Try again.')
+                print("Not a word. Try again.")
             else:
                 break
         print()
         return result
 
+
 class StartWordPolicy(Policy):
-    def __init__(self, start_words: Optional[List[str]]=None):
+    def __init__(self, start_words: Optional[List[str]] = None):
         super().__init__()
         self.start_words = start_words
         if self.start_words is None:
             # "tales" is the optimal word under 10k_words.txt
             # "raise" is the optimal word under wordle_official.txt
-            self.start_words = ['opera', 'tears', 'soare', 'roate', 'raise', 'arose', 
-                                'earls', 'laser', 'reals', 'aloes', 'reais', 'slate', 
-                                'sauce', 'slice', 'shale', 'saute', 'share', 'sooty', 
-                                'shine', 'suite', 'crane', 'adieu', 'audio', 'stare', 
-                                'roast', 'ratio', 'arise', 'tales']
-    
-    def act(self, obs: WordleObservation) -> str:
-        filtered_start_words = list(filter(lambda x: x in obs.game.vocab.filtered_vocab, self.start_words))
+            self.start_words = [
+                "opera",
+                "tears",
+                "soare",
+                "roate",
+                "raise",
+                "arose",
+                "earls",
+                "laser",
+                "reals",
+                "aloes",
+                "reais",
+                "slate",
+                "sauce",
+                "slice",
+                "shale",
+                "saute",
+                "share",
+                "sooty",
+                "shine",
+                "suite",
+                "crane",
+                "adieu",
+                "audio",
+                "stare",
+                "roast",
+                "ratio",
+                "arise",
+                "tales",
+            ]
+
+    def act(self, obs: WordleObservation) -> str:
+        filtered_start_words = list(
+            filter(lambda x: x in obs.game.vocab.filtered_vocab, self.start_words)
+        )
         if len(filtered_start_words) == 0:
             filtered_start_words = obs.game.vocab.filtered_vocab
         return random.choice(filtered_start_words)
 
+
 class OptimalPolicy(Policy):
-    def __init__(self, start_word_policy: Optional[Policy]=None, progress_bar: bool=False):
+    def __init__(
+        self, start_word_policy: Optional[Policy] = None, progress_bar: bool = False
+    ):
         super().__init__()
         self.start_word_policy = start_word_policy
         self.progress_bar = progress_bar
         self.cache = Cache()
 
     def act(self, obs: WordleObservation) -> str:
         if obs.game.state in self.cache:
             return random.choice(self.cache[obs.game.state])
         if len(obs.game.action_history) == 0 and self.start_word_policy is not None:
             return self.start_word_policy.act(obs)
         best_words = []
-        best_info = float('-inf')
-        for word in tqdm(obs.game.vocab.filtered_vocab) if self.progress_bar else obs.game.vocab.filtered_vocab:
+        best_info = float("-inf")
+        for word in (
+            tqdm(obs.game.vocab.filtered_vocab)
+            if self.progress_bar
+            else obs.game.vocab.filtered_vocab
+        ):
             total_entropy = 0.0
             total = 0
             for next_state, state_count in obs.game.all_next(word):
-                total_entropy += math.log(next_state.vocab.filtered_vocab_size()) * state_count
+                total_entropy += (
+                    math.log(next_state.vocab.filtered_vocab_size()) * state_count
+                )
                 total += state_count
-            info_gain = math.log(obs.game.vocab.filtered_vocab_size()) - (total_entropy / total)
+            info_gain = math.log(obs.game.vocab.filtered_vocab_size()) - (
+                total_entropy / total
+            )
             if info_gain > best_info:
                 best_words, best_info = [word], info_gain
             elif info_gain == best_info:
                 best_words.append(word)
         self.cache[obs.game.state] = best_words
         return random.choice(best_words)
 
+
 class RepeatPolicy(Policy):
     def __init__(self, start_word_policy: Optional[Policy], first_n: Optional[int]):
         super().__init__()
         self.first_n = first_n
         self.start_word_policy = start_word_policy
-    
+
     def act(self, obs: WordleObservation) -> str:
         if len(obs.game.action_history) == 0:
             if self.start_word_policy is not None:
                 return self.start_word_policy.act(obs)
             return obs.game.vocab.get_random_word_all()
         if self.first_n is None:
             return random.choice(obs.game.action_history)
-        return random.choice(obs.game.action_history[:self.first_n])
+        return random.choice(obs.game.action_history[: self.first_n])
+
 
 class RandomMixturePolicy(Policy):
     def __init__(self, prob_smart: float, vocab: Optional[Union[str, Vocabulary]]):
         super().__init__()
         self.vocab = vocab
         if isinstance(self.vocab, str):
             self.vocab = Vocabulary.from_file(self.vocab)
@@ -113,50 +158,55 @@
             v = self.vocab
         if random.random() < self.prob_smart:
             if self.vocab is not None:
                 v = v.update_vocab(obs.game.state)
             return v.get_random_word_filtered()
         return v.get_random_word_all()
 
+
 class WrongPolicy(Policy):
     def __init__(self, vocab: Union[str, Vocabulary]):
         super().__init__()
         self.vocab = vocab
         if isinstance(self.vocab, str):
             self.vocab = Vocabulary.from_file(self.vocab)
         self.choices = set(self.vocab.all_vocab)
 
     def act(self, obs: WordleObservation) -> str:
         bad_options = self.choices.difference(obs.game.vocab.filtered_vocab)
         if len(bad_options) == 0:
             return self.vocab.get_random_word_all()
         return random.sample(bad_options, 1)[0]
 
+
 class MixturePolicy(Policy):
     def __init__(self, prob1: float, policy1: Policy, policy2: Policy):
         super().__init__()
         self.prob1 = prob1
         self.policy1 = policy1
         self.policy2 = policy2
-    
+
     def act(self, obs: WordleObservation) -> str:
         if random.random() < self.prob1:
             return self.policy1.act(obs)
         return self.policy2.act(obs)
 
+
 class MonteCarloPolicy(Policy):
     def __init__(self, n_samples: int, sample_policy: Policy):
         super().__init__()
         self.n_samples = n_samples
         self.sample_policy = sample_policy
-    
+
     def act(self, obs: WordleObservation) -> str:
         action_scores = defaultdict(list)
         for _ in range(self.n_samples):
             curr_obs = obs
             total_reward = 0
             while not curr_obs.game.is_terminal():
                 word_choice = self.sample_policy.act(curr_obs)
                 curr_obs, r, _ = curr_obs.game.next(word_choice)
                 total_reward += r
-            action_scores[curr_obs.action_history[len(obs.game.action_history)]].append(total_reward)
+            action_scores[curr_obs.action_history[len(obs.game.action_history)]].append(
+                total_reward
+            )
         return max(action_scores.items(), key=lambda x: sum(x[1]) / len(x[1]))[0]
```

### Comparing `agilerl-0.1.8/agilerl/wordle/wordle_dataset.py` & `agilerl-0.1.9/agilerl/wordle/wordle_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,128 +1,184 @@
-from agilerl.data.language_environment import interact_environment
+import json
+import pickle as pkl
+import random
+from typing import Any, Dict, List, Optional, Tuple
+
+import numpy as np
+from tqdm.auto import tqdm
+
+from agilerl.data.language_environment import Policy, interact_environment
+from agilerl.data.rl_data import (
+    ConstantTokenReward,
+    DataPoint,
+    Iterable_RL_Dataset,
+    List_RL_Dataset,
+    TokenReward,
+)
 from agilerl.utils.ilql_utils import convert_path
-from typing import List, Optional, Dict, Any, Tuple
-from agilerl.data.rl_data import ConstantTokenReward, List_RL_Dataset, Iterable_RL_Dataset, DataPoint, TokenReward
-from agilerl.data.language_environment import Policy
 from agilerl.wordle.wordle_env import WordleEnvironment, WordleObservation
 from agilerl.wordle.wordle_game import Vocabulary, WordleGame, WordleState
 from agilerl.wordle.wordle_tokenizer import WordleTokenizer
-import pickle as pkl
-import json
-from tqdm.auto import tqdm
-import random
-import numpy as np
+
 
 class WordleListDataset(List_RL_Dataset):
-    def __init__(self, 
-                 items: List[Tuple[WordleObservation, Optional[Dict[str, Any]]]], 
-                 max_len: Optional[int], 
-                 token_reward: TokenReward) -> None:
+    def __init__(
+        self,
+        items: List[Tuple[WordleObservation, Optional[Dict[str, Any]]]],
+        max_len: Optional[int],
+        token_reward: TokenReward,
+    ) -> None:
         tokenizer = WordleTokenizer()
         super().__init__(tokenizer, token_reward, max_len)
         self.items = items
-    
+
     def get_item(self, idx: int):
-        return DataPoint.from_obs(self.items[idx][0], self.tokenizer, self.token_reward, self.items[idx][1])
-    
+        return DataPoint.from_obs(
+            self.items[idx][0], self.tokenizer, self.token_reward, self.items[idx][1]
+        )
+
     def size(self):
         return len(self.items)
-    
+
     @classmethod
-    def from_file(cls, file_path: str, max_len: Optional[int], vocab: Optional[Vocabulary], token_reward: TokenReward):
-        with open(file_path, 'rb') as f:
+    def from_file(
+        cls,
+        file_path: str,
+        max_len: Optional[int],
+        vocab: Optional[Vocabulary],
+        token_reward: TokenReward,
+    ):
+        with open(file_path, "rb") as f:
             d = pkl.load(f)
         if vocab is None:
-            vocab = Vocabulary.from_file(convert_path(d['vocab_path']))
-            if d['vocab_cache_path'] is not None:
-                vocab.cache.load(convert_path(d['vocab_cache_path']))
-        wordle_items = [WordleObservation(WordleGame(item['state'], vocab.update_vocab(
-            item['state']), item['actions'])) for item in tqdm(d['state_actions'])]
-        meta = [{**item['meta'], 'self': wordle_items[i]} if 'meta' in item else {
-            'self': wordle_items[i]} for i, item in enumerate(d['state_actions'])]
+            vocab = Vocabulary.from_file(convert_path(d["vocab_path"]))
+            if d["vocab_cache_path"] is not None:
+                vocab.cache.load(convert_path(d["vocab_cache_path"]))
+        wordle_items = [
+            WordleObservation(
+                WordleGame(
+                    item["state"], vocab.update_vocab(item["state"]), item["actions"]
+                )
+            )
+            for item in tqdm(d["state_actions"])
+        ]
+        meta = [
+            {**item["meta"], "self": wordle_items[i]}
+            if "meta" in item
+            else {"self": wordle_items[i]}
+            for i, item in enumerate(d["state_actions"])
+        ]
         return WordleListDataset(list(zip(wordle_items, meta)), max_len, token_reward)
-    
+
+
 class WordleIterableDataset(Iterable_RL_Dataset):
-    def __init__(self, 
-                 policy: Policy, 
-                 vocab: Vocabulary, 
-                 max_len: Optional[int], 
-                 token_reward: TokenReward) -> None:
+    def __init__(
+        self,
+        policy: Policy,
+        vocab: Vocabulary,
+        max_len: Optional[int],
+        token_reward: TokenReward,
+    ) -> None:
         tokenizer = WordleTokenizer()
         super().__init__(tokenizer, token_reward, max_len)
         self.policy = policy
         self.env = WordleEnvironment(vocab)
 
     def sample_item(self):
-        return DataPoint.from_obs(interact_environment(self.env, self.policy, None)[0], self.tokenizer, 
-                                  self.token_reward, None)
+        return DataPoint.from_obs(
+            interact_environment(self.env, self.policy, None)[0],
+            self.tokenizer,
+            self.token_reward,
+            None,
+        )
+
 
 class WordleHumanDataset(Iterable_RL_Dataset):
-    def __init__(self, 
-                 games: List[Tuple[str, List[str]]], 
-                 transitions: Dict[str, Dict[str, List[str]]], 
-                 use_true_word: bool, 
-                 max_len: Optional[int], 
-                 token_reward: TokenReward, 
-                 game_indexes: Optional[List[int]], 
-                 top_p: Optional[float], 
-                ) -> None:
+    def __init__(
+        self,
+        games: List[Tuple[str, List[str]]],
+        transitions: Dict[str, Dict[str, List[str]]],
+        use_true_word: bool,
+        max_len: Optional[int],
+        token_reward: TokenReward,
+        game_indexes: Optional[List[int]],
+        top_p: Optional[float],
+    ) -> None:
         tokenizer = WordleTokenizer()
         super().__init__(tokenizer, token_reward, max_len)
         self.games = games
         if game_indexes is not None:
             self.games = [self.games[idx] for idx in game_indexes]
-        if top_p is  not None:
+        if top_p is not None:
             lens = [len(game) for _, game in self.games]
-            self.games = [self.games[idx] for idx in np.argsort(lens)[:int(len(lens)*top_p)]]
+            self.games = [
+                self.games[idx] for idx in np.argsort(lens)[: int(len(lens) * top_p)]
+            ]
         self.transitions = transitions
         self.use_true_word = use_true_word
 
     def sample_item(self):
         true_word, game = random.choice(self.games)
         if self.use_true_word:
             while True:
                 actions = []
                 for transition in game:
-                    if transition not in self.transitions[true_word] or len(
-                        self.transitions[true_word][transition]) == 0:
+                    if (
+                        transition not in self.transitions[true_word]
+                        or len(self.transitions[true_word][transition]) == 0
+                    ):
                         break
-                    actions.append(random.choice(self.transitions[true_word][transition]))
+                    actions.append(
+                        random.choice(self.transitions[true_word][transition])
+                    )
                 if len(actions) == len(game):
                     break
                 else:
                     true_word, game = random.choice(self.games)
         else:
             word_choices = list(self.transitions.keys())
             while True:
                 true_word = random.choice(word_choices)
                 actions = []
                 for transition in game:
-                    if transition not in self.transitions[true_word] or len(
-                        self.transitions[true_word][transition]) == 0:
+                    if (
+                        transition not in self.transitions[true_word]
+                        or len(self.transitions[true_word][transition]) == 0
+                    ):
                         break
-                    actions.append(random.choice(self.transitions[true_word][transition]))
+                    actions.append(
+                        random.choice(self.transitions[true_word][transition])
+                    )
                 if len(actions) == len(game):
                     break
                 else:
                     true_word, game = random.choice(self.games)
         state = WordleState.initial_state()
         for action in actions:
             state = state.transition_state(action, true_word)
         vocab = Vocabulary([true_word], state, cache=None, fill_cache=False)
         obs = WordleObservation(WordleGame(state, vocab, actions))
-        return DataPoint.from_obs(obs, self.tokenizer, self.token_reward, {'obs': obs})
-    
+        return DataPoint.from_obs(obs, self.tokenizer, self.token_reward, {"obs": obs})
+
     @classmethod
-    def from_file(cls, file_path: str, 
-                  use_true_word: bool=False, 
-                  max_len: Optional[int]=None, 
-                  token_reward: Optional[TokenReward]=None, 
-                  game_indexes: Optional[List[int]]=None, 
-                  top_p: Optional[float]=None):
+    def from_file(
+        cls,
+        file_path: str,
+        use_true_word: bool = False,
+        max_len: Optional[int] = None,
+        token_reward: Optional[TokenReward] = None,
+        game_indexes: Optional[List[int]] = None,
+        top_p: Optional[float] = None,
+    ):
         if token_reward is None:
             token_reward = ConstantTokenReward(0.0)
-        with open(file_path, 'r') as f:
+        with open(file_path) as f:
             d = json.load(f)
-        return WordleHumanDataset(d['games'], d['transitions'], use_true_word, max_len, token_reward, 
-                                  game_indexes, top_p)
-
+        return WordleHumanDataset(
+            d["games"],
+            d["transitions"],
+            use_true_word,
+            max_len,
+            token_reward,
+            game_indexes,
+            top_p,
+        )
```

### Comparing `agilerl-0.1.8/agilerl/wordle/wordle_env.py` & `agilerl-0.1.9/agilerl/wordle/wordle_env.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from typing import List, Optional, Tuple
+
 from agilerl.data.language_environment import Language_Environment, Language_Observation
 from agilerl.wordle.wordle_game import Vocabulary, WordleGame
 
+
 class WordleObservation(Language_Observation):
     def __init__(self, game: WordleGame):
         self.game = game
 
     def to_sequence(self) -> Tuple[List[Tuple[str, Optional[float]]], bool]:
         return self.game.transition_sequence()
-    
+
     def __str__(self) -> str:
         return str(self.game)
 
+
 class WordleEnvironment(Language_Environment):
     def __init__(self, vocab: Vocabulary):
         self.vocab = vocab
         self.state = self.reset()
 
     def step(self, action: str) -> Tuple[WordleObservation, float, bool]:
         wordle_game, r, t = self.state.game.next(action)
```

### Comparing `agilerl-0.1.8/agilerl/wordle/wordle_evaluators.py` & `agilerl-0.1.9/agilerl/wordle/wordle_evaluators.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,145 +1,314 @@
+import random
+from collections import defaultdict
 from typing import Any, Dict, Optional
+
+from agilerl.algorithms.ilql import ILQL
 from agilerl.data.rl_data import DataPoint
 from agilerl.wordle.wordle_dataset import WordleListDataset
 from agilerl.wordle.wordle_env import WordleObservation
 from agilerl.wordle.wordle_game import N_CHARS, WordleGame
-from collections import defaultdict
-from agilerl.algorithms.ilql import ILQL
-import random
 
-class Action_Ranking_Evaluator():
+
+class Action_Ranking_Evaluator:
     def __init__(self, branching_data: WordleListDataset) -> None:
         self.branching_data = branching_data
         self.expert_actions = defaultdict(list)
         self.non_expert_actions = defaultdict(list)
         for i in range(self.branching_data.size()):
             item = self.branching_data.get_item(i)
-            assert item.meta is not None and 'kind' in item.meta
-            if item.meta['kind'] == 'expert':
-                for prefix in item.meta['prefixes']:
-                    self.expert_actions[self.hashable_state(prefix)].append(item.meta['self_actions'][len(prefix[1])])
-            elif item.meta['kind'] == 'branch_suboptimal':
-                start = item.meta['start']
-                self.non_expert_actions[self.hashable_state(start)].append(item.meta['self_actions'][len(start[1])])
+            assert item.meta is not None and "kind" in item.meta
+            if item.meta["kind"] == "expert":
+                for prefix in item.meta["prefixes"]:
+                    self.expert_actions[self.hashable_state(prefix)].append(
+                        item.meta["self_actions"][len(prefix[1])]
+                    )
+            elif item.meta["kind"] == "branch_suboptimal":
+                start = item.meta["start"]
+                self.non_expert_actions[self.hashable_state(start)].append(
+                    item.meta["self_actions"][len(start[1])]
+                )
             else:
                 raise NotImplementedError
-        self.states = list(set(self.expert_actions.keys()).intersection(set(self.non_expert_actions.keys())))
-        self.vocab = self.branching_data.get_item(0).meta['self'].game.vocab
+        self.states = list(
+            set(self.expert_actions.keys()).intersection(
+                set(self.non_expert_actions.keys())
+            )
+        )
+        self.vocab = self.branching_data.get_item(0).meta["self"].game.vocab
 
     def hashable_state(self, state):
-        return (state[0], tuple(state[1]),)
-    
+        return (
+            state[0],
+            tuple(state[1]),
+        )
+
     def evaluate(self, model: ILQL, items) -> Optional[Dict[str, Any]]:
         assert not model.double_q
-        tokens = model.prepare_inputs(items)['tokens']
-        total_correct = [0 for _ in range(N_CHARS+1)]
-        total_correct_target = [0 for _ in range(N_CHARS+1)]
+        tokens = model.prepare_inputs(items)["tokens"]
+        total_correct = [0 for _ in range(N_CHARS + 1)]
+        total_correct_target = [0 for _ in range(N_CHARS + 1)]
         total = 0
         for _ in range(tokens.shape[0]):
             s, a = random.choice(self.states)
             obs = WordleObservation(WordleGame(s, self.vocab.update_vocab(s), list(a)))
-            expert_state, _, _ = obs.game.next(random.choice(self.expert_actions[self.hashable_state((s, a,))]))
-            non_expert_state, _, _ = obs.game.next(random.choice(self.non_expert_actions[self.hashable_state((s, a,))]))
-            expert_datapoint = DataPoint.from_obs(WordleObservation(expert_state), self.branching_data.token_reward, 
-                                                  self.branching_data.tokenizer)
-            non_expert_datapoint = DataPoint.from_obs(WordleObservation(non_expert_state), 
-                                                      self.branching_data.token_reward, self.branching_data.tokenizer)
+            expert_state, _, _ = obs.game.next(
+                random.choice(
+                    self.expert_actions[
+                        self.hashable_state(
+                            (
+                                s,
+                                a,
+                            )
+                        )
+                    ]
+                )
+            )
+            non_expert_state, _, _ = obs.game.next(
+                random.choice(
+                    self.non_expert_actions[
+                        self.hashable_state(
+                            (
+                                s,
+                                a,
+                            )
+                        )
+                    ]
+                )
+            )
+            expert_datapoint = DataPoint.from_obs(
+                WordleObservation(expert_state),
+                self.branching_data.token_reward,
+                self.branching_data.tokenizer,
+            )
+            non_expert_datapoint = DataPoint.from_obs(
+                WordleObservation(non_expert_state),
+                self.branching_data.token_reward,
+                self.branching_data.tokenizer,
+            )
             iql_outputs = model.get_qvs([expert_datapoint, non_expert_datapoint])
-            qs, target_qs, terminals = iql_outputs['qs'], iql_outputs['target_qs'], iql_outputs['terminals']
-            for i in range(N_CHARS+1):
-                total_correct[i] += int(qs[0, 
-                                           (1 - terminals[0, :-1]).sum()-1-i] > qs[1, 
-                                                                                   (1 - terminals[1, :-1]).sum()-1-i])
+            qs, target_qs, terminals = (
+                iql_outputs["qs"],
+                iql_outputs["target_qs"],
+                iql_outputs["terminals"],
+            )
+            for i in range(N_CHARS + 1):
+                total_correct[i] += int(
+                    qs[0, (1 - terminals[0, :-1]).sum() - 1 - i]
+                    > qs[1, (1 - terminals[1, :-1]).sum() - 1 - i]
+                )
                 total_correct_target[i] += int(
-                    target_qs[0, (1 - terminals[0, :-1]).sum()-1-i] > target_qs[1, (1 - terminals[1, :-1]).sum()-1-i])
+                    target_qs[0, (1 - terminals[0, :-1]).sum() - 1 - i]
+                    > target_qs[1, (1 - terminals[1, :-1]).sum() - 1 - i]
+                )
             total += 1
-        return {**{('q_rank_acc_-%d' % (i+1)): (total_correct[i] / total, total) for i in range(N_CHARS+1)}, **{
-            ('q_target_rank_acc_-%d' % (i+1)): (total_correct_target[i] / total, total) for i in range(N_CHARS+1)}}
+        return {
+            **{
+                ("q_rank_acc_-%d" % (i + 1)): (total_correct[i] / total, total)
+                for i in range(N_CHARS + 1)
+            },
+            **{
+                ("q_target_rank_acc_-%d" % (i + 1)): (
+                    total_correct_target[i] / total,
+                    total,
+                )
+                for i in range(N_CHARS + 1)
+            },
+        }
 
-class Action_Ranking_Evaluator_Adversarial():
+
+class Action_Ranking_Evaluator_Adversarial:
     def __init__(self, adversarial_data: WordleListDataset) -> None:
         self.adversarial_data = adversarial_data
         self.expert_actions = defaultdict(list)
         self.adversarial_actions = defaultdict(list)
         self.suboptimal_actions = defaultdict(list)
         for i in range(self.adversarial_data.size()):
             item = self.adversarial_data.get_item(i)
-            assert item.meta is not None and 'kind' in item.meta
-            if item.meta['kind'] == 'expert':
-                self.expert_actions[self.hashable_state(item.meta['s_0'])].append(item.meta['a_0'])
-                if 's_2' in item.meta:
-                    self.expert_actions[self.hashable_state(item.meta['s_2'])].append(item.meta['a_2'])
-            elif item.meta['kind'] == 'adversarial':
-                self.adversarial_actions[self.hashable_state(item.meta['s_2'])].append(item.meta['a_2'])
-            elif item.meta['kind'] == 'suboptimal':
-                self.suboptimal_actions[self.hashable_state(item.meta['s_0'])].append(item.meta['a_0'])
+            assert item.meta is not None and "kind" in item.meta
+            if item.meta["kind"] == "expert":
+                self.expert_actions[self.hashable_state(item.meta["s_0"])].append(
+                    item.meta["a_0"]
+                )
+                if "s_2" in item.meta:
+                    self.expert_actions[self.hashable_state(item.meta["s_2"])].append(
+                        item.meta["a_2"]
+                    )
+            elif item.meta["kind"] == "adversarial":
+                self.adversarial_actions[self.hashable_state(item.meta["s_2"])].append(
+                    item.meta["a_2"]
+                )
+            elif item.meta["kind"] == "suboptimal":
+                self.suboptimal_actions[self.hashable_state(item.meta["s_0"])].append(
+                    item.meta["a_0"]
+                )
             else:
                 raise NotImplementedError
-        self.initial_states = list(set(self.expert_actions.keys()).intersection(set(self.suboptimal_actions.keys())))
-        self.branch_states = list(set(self.expert_actions.keys()).intersection(set(self.adversarial_actions.keys())))
-        self.vocab = self.adversarial_data.get_item(0).meta['self'].game.vocab
+        self.initial_states = list(
+            set(self.expert_actions.keys()).intersection(
+                set(self.suboptimal_actions.keys())
+            )
+        )
+        self.branch_states = list(
+            set(self.expert_actions.keys()).intersection(
+                set(self.adversarial_actions.keys())
+            )
+        )
+        self.vocab = self.adversarial_data.get_item(0).meta["self"].game.vocab
 
     def hashable_state(self, state):
-        return (state[0], tuple(state[1]),)
-    
+        return (
+            state[0],
+            tuple(state[1]),
+        )
+
     def evaluate(self, model: ILQL, items) -> Optional[Dict[str, Any]]:
         # evaluate Q-values for suboptimal verses expert at the first action
         # evaluate Q-values for expert versus adversarial at the third action
         assert not model.double_q
-        tokens = model.prepare_inputs(items)['tokens']
-        initial_total_correct = [0 for _ in range(N_CHARS+1)]
-        initial_total_correct_target = [0 for _ in range(N_CHARS+1)]
-        branch_total_correct = [0 for _ in range(N_CHARS+1)]
-        branch_total_correct_target = [0 for _ in range(N_CHARS+1)]
+        tokens = model.prepare_inputs(items)["tokens"]
+        initial_total_correct = [0 for _ in range(N_CHARS + 1)]
+        initial_total_correct_target = [0 for _ in range(N_CHARS + 1)]
+        branch_total_correct = [0 for _ in range(N_CHARS + 1)]
+        branch_total_correct_target = [0 for _ in range(N_CHARS + 1)]
         total = 0
         for _ in range(tokens.shape[0]):
             initial_s, initial_a = random.choice(self.initial_states)
-            initial_obs = WordleObservation(WordleGame(initial_s, self.vocab.update_vocab(initial_s), list(initial_a)))
-            initial_expert_a = random.choice(self.expert_actions[self.hashable_state((initial_s, initial_a,))])
-            initial_suboptimal_a = random.choice(self.suboptimal_actions[self.hashable_state((initial_s, initial_a,))])
+            initial_obs = WordleObservation(
+                WordleGame(
+                    initial_s, self.vocab.update_vocab(initial_s), list(initial_a)
+                )
+            )
+            initial_expert_a = random.choice(
+                self.expert_actions[
+                    self.hashable_state(
+                        (
+                            initial_s,
+                            initial_a,
+                        )
+                    )
+                ]
+            )
+            initial_suboptimal_a = random.choice(
+                self.suboptimal_actions[
+                    self.hashable_state(
+                        (
+                            initial_s,
+                            initial_a,
+                        )
+                    )
+                ]
+            )
             initial_expert_state, _, _ = initial_obs.game.next(initial_expert_a)
             initial_suboptimal_state, _, _ = initial_obs.game.next(initial_suboptimal_a)
-            initial_expert_datapoint = DataPoint.from_obs(WordleObservation(initial_expert_state), 
-                                                          self.adversarial_data.tokenizer, 
-                                                          self.adversarial_data.token_reward)
-            initial_suboptimal_datapoint = DataPoint.from_obs(WordleObservation(initial_suboptimal_state), 
-                                                              self.adversarial_data.tokenizer, 
-                                                              self.adversarial_data.token_reward)
-            iql_outputs = model.get_qvs([initial_expert_datapoint, initial_suboptimal_datapoint])
-            qs, target_qs, terminals = iql_outputs['qs'], iql_outputs['target_qs'], iql_outputs['terminals']
-            for i in range(N_CHARS+1):
-                initial_total_correct[i] += int(qs[0, (1 - terminals[0, :-1]).sum()-1-i] > qs[1, (
-                    1 - terminals[1, :-1]).sum()-1-i])
+            initial_expert_datapoint = DataPoint.from_obs(
+                WordleObservation(initial_expert_state),
+                self.adversarial_data.tokenizer,
+                self.adversarial_data.token_reward,
+            )
+            initial_suboptimal_datapoint = DataPoint.from_obs(
+                WordleObservation(initial_suboptimal_state),
+                self.adversarial_data.tokenizer,
+                self.adversarial_data.token_reward,
+            )
+            iql_outputs = model.get_qvs(
+                [initial_expert_datapoint, initial_suboptimal_datapoint]
+            )
+            qs, target_qs, terminals = (
+                iql_outputs["qs"],
+                iql_outputs["target_qs"],
+                iql_outputs["terminals"],
+            )
+            for i in range(N_CHARS + 1):
+                initial_total_correct[i] += int(
+                    qs[0, (1 - terminals[0, :-1]).sum() - 1 - i]
+                    > qs[1, (1 - terminals[1, :-1]).sum() - 1 - i]
+                )
                 initial_total_correct_target[i] += int(
-                    target_qs[0, (1 - terminals[0, :-1]).sum()-1-i] > target_qs[1, (1 - terminals[1, :-1]).sum()-1-i])
-            
+                    target_qs[0, (1 - terminals[0, :-1]).sum() - 1 - i]
+                    > target_qs[1, (1 - terminals[1, :-1]).sum() - 1 - i]
+                )
+
             branch_s, branch_a = random.choice(self.branch_states)
-            branch_obs = WordleObservation(WordleGame(branch_s, self.vocab.update_vocab(branch_s), list(branch_a)))
-            branch_expert_a = random.choice(self.expert_actions[self.hashable_state((branch_s, branch_a,))])
-            branch_adversarial_a = random.choice(self.adversarial_actions[self.hashable_state((branch_s, branch_a,))])
+            branch_obs = WordleObservation(
+                WordleGame(branch_s, self.vocab.update_vocab(branch_s), list(branch_a))
+            )
+            branch_expert_a = random.choice(
+                self.expert_actions[
+                    self.hashable_state(
+                        (
+                            branch_s,
+                            branch_a,
+                        )
+                    )
+                ]
+            )
+            branch_adversarial_a = random.choice(
+                self.adversarial_actions[
+                    self.hashable_state(
+                        (
+                            branch_s,
+                            branch_a,
+                        )
+                    )
+                ]
+            )
             branch_expert_state, _, _ = branch_obs.game.next(branch_expert_a)
             branch_adversarial_state, _, _ = branch_obs.game.next(branch_adversarial_a)
-            branch_expert_datapoint = DataPoint.from_obs(WordleObservation(branch_expert_state), 
-                                                         self.adversarial_data.tokenizer, 
-                                                         self.adversarial_data.token_reward)
-            branch_adversarial_datapoint = DataPoint.from_obs(WordleObservation(branch_adversarial_state), 
-                                                              self.adversarial_data.tokenizer, 
-                                                              self.adversarial_data.token_reward)
-            iql_outputs = model.get_qvs([branch_expert_datapoint, branch_adversarial_datapoint])
-            qs, target_qs, terminals = iql_outputs['qs'], iql_outputs['target_qs'], iql_outputs['terminals']
-            for i in range(N_CHARS+1):
+            branch_expert_datapoint = DataPoint.from_obs(
+                WordleObservation(branch_expert_state),
+                self.adversarial_data.tokenizer,
+                self.adversarial_data.token_reward,
+            )
+            branch_adversarial_datapoint = DataPoint.from_obs(
+                WordleObservation(branch_adversarial_state),
+                self.adversarial_data.tokenizer,
+                self.adversarial_data.token_reward,
+            )
+            iql_outputs = model.get_qvs(
+                [branch_expert_datapoint, branch_adversarial_datapoint]
+            )
+            qs, target_qs, terminals = (
+                iql_outputs["qs"],
+                iql_outputs["target_qs"],
+                iql_outputs["terminals"],
+            )
+            for i in range(N_CHARS + 1):
                 branch_total_correct[i] += int(
-                    qs[0, (1 - terminals[0, :-1]).sum()-1-i] > qs[1, (1 - terminals[1, :-1]).sum()-1-i])
+                    qs[0, (1 - terminals[0, :-1]).sum() - 1 - i]
+                    > qs[1, (1 - terminals[1, :-1]).sum() - 1 - i]
+                )
                 branch_total_correct_target[i] += int(
-                    target_qs[0, (1 - terminals[0, :-1]).sum()-1-i] > target_qs[1, (1 - terminals[1, :-1]).sum()-1-i])
+                    target_qs[0, (1 - terminals[0, :-1]).sum() - 1 - i]
+                    > target_qs[1, (1 - terminals[1, :-1]).sum() - 1 - i]
+                )
             total += 1
         return {
-                **{('initial_q_rank_acc_-%d' % (i+1)): (
-                    initial_total_correct[i] / total, total) for i in range(N_CHARS+1)}, 
-                **{('initial_q_target_rank_acc_-%d' % (i+1)): (
-                    initial_total_correct_target[i] / total, total) for i in range(N_CHARS+1)}, 
-                **{('branch_q_rank_acc_-%d' % (i+1)): (
-                    branch_total_correct[i] / total, total) for i in range(N_CHARS+1)}, 
-                **{('branch_q_target_rank_acc_-%d' % (i+1)): (
-                    branch_total_correct_target[i] / total, total) for i in range(N_CHARS+1)}, 
-               }
+            **{
+                ("initial_q_rank_acc_-%d" % (i + 1)): (
+                    initial_total_correct[i] / total,
+                    total,
+                )
+                for i in range(N_CHARS + 1)
+            },
+            **{
+                ("initial_q_target_rank_acc_-%d" % (i + 1)): (
+                    initial_total_correct_target[i] / total,
+                    total,
+                )
+                for i in range(N_CHARS + 1)
+            },
+            **{
+                ("branch_q_rank_acc_-%d" % (i + 1)): (
+                    branch_total_correct[i] / total,
+                    total,
+                )
+                for i in range(N_CHARS + 1)
+            },
+            **{
+                ("branch_q_target_rank_acc_-%d" % (i + 1)): (
+                    branch_total_correct_target[i] / total,
+                    total,
+                )
+                for i in range(N_CHARS + 1)
+            },
+        }
```

### Comparing `agilerl-0.1.8/agilerl/wordle/wordle_game.py` & `agilerl-0.1.9/agilerl/wordle/wordle_game.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,263 +1,359 @@
 from __future__ import annotations
+
+import random
 from collections import defaultdict
 from copy import deepcopy
-import random
-from enum import Enum
-from typing import List, Optional
 from dataclasses import dataclass
+from enum import Enum
+
 from termcolor import colored
+
 from agilerl.utils.cache import Cache
 
-IDX2CHAR = list('abcdefghijklmnopqrstuvwxyz')
+IDX2CHAR = list("abcdefghijklmnopqrstuvwxyz")
 CHAR2IDX = {c: i for i, c in enumerate(IDX2CHAR)}
 ALPHA_SIZE = len(IDX2CHAR)
 N_CHARS = 5
 N_TRIES = 6
 
+
 class CharKnowledge(Enum):
     NOT_HERE = 0
     POSSIBLE = 1
     HERE = 2
 
+
 @dataclass
 class CharState:
-    position_knowledge: List[CharKnowledge]
+    position_knowledge: list[CharKnowledge]
 
     def __post_init__(self):
         assert len(self.position_knowledge) == N_CHARS
-    
+
     def __eq__(self, other: CharState):
         return self.position_knowledge == other.position_knowledge
 
     def __hash__(self) -> int:
         return hash(tuple(self.position_knowledge))
-    
+
     @classmethod
     def unknown(cls):
         return cls([CharKnowledge.POSSIBLE for _ in range(N_CHARS)])
-    
+
     @classmethod
     def not_used(cls):
         return cls([CharKnowledge.NOT_HERE for _ in range(N_CHARS)])
-    
+
     def correct_pos(self, pos):
         new_mask = deepcopy(self.position_knowledge)
         new_mask[pos] = CharKnowledge.HERE
         return CharState(new_mask)
-    
+
     def wrong_pos(self, pos):
         new_mask = deepcopy(self.position_knowledge)
         new_mask[pos] = CharKnowledge.NOT_HERE
         return CharState(new_mask)
-    
+
     def word_satisfies(self, c, word):
         if all([k == CharKnowledge.POSSIBLE for k in self.position_knowledge]):
             return True
         if all([k == CharKnowledge.NOT_HERE for k in self.position_knowledge]):
             return c not in word
         for i in range(N_CHARS):
             if self.position_knowledge[i] == CharKnowledge.HERE:
                 if c != word[i]:
                     return False
             if self.position_knowledge[i] == CharKnowledge.NOT_HERE:
                 if c == word[i]:
                     return False
         return c in word
 
+
 class WordleState:
-    def __init__(self, state: List[CharState]):
+    def __init__(self, state: list[CharState]):
         assert len(state) == ALPHA_SIZE
         self.state = state
-    
+
     @classmethod
     def initial_state(cls):
         return cls([CharState.unknown() for i in range(ALPHA_SIZE)])
-    
+
     def word_in_state(self, word: str) -> bool:
         for i in range(len(self.state)):
             if not self.state[i].word_satisfies(IDX2CHAR[i], word):
                 return False
         return True
-    
+
     def transition_state(self, selected_word: str, target_word: str):
         # assert self.word_in_state(target_word)
         new_state = deepcopy(self.state)
         for i, c in enumerate(selected_word):
             if c == target_word[i]:
                 new_state[CHAR2IDX[c]] = new_state[CHAR2IDX[c]].correct_pos(i)
             elif c in target_word:
                 new_state[CHAR2IDX[c]] = new_state[CHAR2IDX[c]].wrong_pos(i)
             else:
                 new_state[CHAR2IDX[c]] = new_state[CHAR2IDX[c]].not_used()
         return WordleState(new_state)
 
     def __eq__(self, other: WordleState) -> bool:
         return self.state == other.state
-    
+
     def __hash__(self) -> int:
         return hash(tuple(self.state))
-    
+
     def __str__(self):
         str_items = defaultdict(list)
         for i in range(len(self.state)):
-            if all([item == CharKnowledge.POSSIBLE for item in self.state[i].position_knowledge]):
+            if all(
+                [
+                    item == CharKnowledge.POSSIBLE
+                    for item in self.state[i].position_knowledge
+                ]
+            ):
                 continue
-            if all([item == CharKnowledge.NOT_HERE for item in self.state[i].position_knowledge]):
-                str_items['none'].append(IDX2CHAR[i])
+            if all(
+                [
+                    item == CharKnowledge.NOT_HERE
+                    for item in self.state[i].position_knowledge
+                ]
+            ):
+                str_items["none"].append(IDX2CHAR[i])
                 continue
             char_values = []
-            k = 'wrong_pos'
+            k = "wrong_pos"
             for x in range(N_CHARS):
                 if self.state[i].position_knowledge[x] == CharKnowledge.HERE:
-                    k = 'known'
-                    char_values.append(colored(str(x), 'green'))
+                    k = "known"
+                    char_values.append(colored(str(x), "green"))
                 elif self.state[i].position_knowledge[x] == CharKnowledge.NOT_HERE:
-                    char_values.append(colored(str(x), 'yellow'))
+                    char_values.append(colored(str(x), "yellow"))
             str_items[k].append(f'{IDX2CHAR[i]}: {",".join(char_values)}')
-        return '\n'.join(['\n'.join(str_items[k]) for k in ['known', 'wrong_pos', 'none'] if len(str_items[k]) > 0])
+        return "\n".join(
+            [
+                "\n".join(str_items[k])
+                for k in ["known", "wrong_pos", "none"]
+                if len(str_items[k]) > 0
+            ]
+        )
+
 
 class Vocabulary:
-    def __init__(self, all_vocab: List[str], 
-                 wordle_state: Optional[WordleState], 
-                 cache: Optional[Cache]=None, 
-                 fill_cache: bool=True):
+    def __init__(
+        self,
+        all_vocab: list[str],
+        wordle_state: WordleState | None,
+        cache: Cache | None = None,
+        fill_cache: bool = True,
+    ):
         # assert all([len(w) == N_CHARS for w in filtered_vocab])
         self.fill_cache = fill_cache
         self.cache = cache
         if self.cache is None:
             self.cache = Cache()
         self.all_vocab = all_vocab
         if wordle_state is not None:
             if wordle_state in self.cache:
                 self.filtered_vocab = self.cache[wordle_state]
             else:
-                self.filtered_vocab = list(filter(lambda x: wordle_state.word_in_state(x), self.all_vocab))
+                self.filtered_vocab = list(
+                    filter(lambda x: wordle_state.word_in_state(x), self.all_vocab)
+                )
                 if self.fill_cache:
                     self.cache[wordle_state] = self.filtered_vocab
         else:
             self.filtered_vocab = list(self.all_vocab)
-    
+
     @classmethod
-    def from_file(cls, vocab_file: str, fill_cache: bool=True):
+    def from_file(cls, vocab_file: str, fill_cache: bool = True):
         vocab = []
-        for item in open(vocab_file, 'r'):
+        for item in open(vocab_file):
             item = item.strip()
             if len(item) == N_CHARS:
                 vocab.append(item)
         return cls(vocab, None, None, fill_cache)
-    
+
     def filtered_vocab_size(self):
         return len(self.filtered_vocab)
-    
+
     def all_vocab_size(self):
         return len(self.all_vocab)
-    
+
     def get_random_word_filtered(self):
         return random.choice(self.filtered_vocab)
-    
+
     def get_random_word_all(self):
         return random.choice(self.all_vocab)
-    
+
     def update_vocab(self, wordle_state: WordleState):
-        return Vocabulary(self.all_vocab, wordle_state, cache=self.cache, fill_cache=self.fill_cache)
+        return Vocabulary(
+            self.all_vocab, wordle_state, cache=self.cache, fill_cache=self.fill_cache
+        )
 
     def __str__(self) -> str:
-        return '\n'.join(self.filtered_vocab)
+        return "\n".join(self.filtered_vocab)
+
 
 class WordleGame:
-    def __init__(self, 
-                 state: WordleState, 
-                 vocab: Vocabulary, 
-                 action_history: List[str]):
+    def __init__(
+        self, state: WordleState, vocab: Vocabulary, action_history: list[str]
+    ):
         self.state = state
         self.vocab = vocab
         self.action_history = action_history
-    
+
     @classmethod
     def initialize(cls, vocab: Vocabulary):
         init_wordle = WordleState.initial_state()
         return cls(init_wordle, vocab.update_vocab(init_wordle), action_history=[])
-    
+
     def next(self, action: str):
         if len(action) != N_CHARS or (not all([c in CHAR2IDX for c in action])):
-            new_mdp = WordleGame(self.state, self.vocab, action_history=self.action_history+[action])
+            new_mdp = WordleGame(
+                self.state, self.vocab, action_history=self.action_history + [action]
+            )
             return new_mdp, new_mdp.reward(), new_mdp.is_terminal()
         if self.is_terminal():
             return None
         word = self.vocab.get_random_word_filtered()
         new_state = self.state.transition_state(action, word)
-        new_mdp = WordleGame(new_state, self.vocab.update_vocab(new_state), 
-        action_history=self.action_history+[action])
+        new_mdp = WordleGame(
+            new_state,
+            self.vocab.update_vocab(new_state),
+            action_history=self.action_history + [action],
+        )
         return new_mdp, new_mdp.reward(), new_mdp.is_terminal()
-    
+
     def all_next(self, action: str):
         if len(action) != N_CHARS or (not all([c in CHAR2IDX for c in action])):
-            return [(WordleGame(self.state, self.vocab, action_history=self.action_history+[action]), 1,)]
+            return [
+                (
+                    WordleGame(
+                        self.state,
+                        self.vocab,
+                        action_history=self.action_history + [action],
+                    ),
+                    1,
+                )
+            ]
         if self.is_terminal():
             return []
         new_states = defaultdict(list)
         for word in self.vocab.filtered_vocab:
             new_states[self.state.transition_state(action, word)].append(word)
-        return [(WordleGame(new_state, self.vocab.update_vocab(new_state), 
-                            action_history=self.action_history+[words[0]]), 
-                            len(words)) for new_state, words in new_states.items()]
-    
+        return [
+            (
+                WordleGame(
+                    new_state,
+                    self.vocab.update_vocab(new_state),
+                    action_history=self.action_history + [words[0]],
+                ),
+                len(words),
+            )
+            for new_state, words in new_states.items()
+        ]
+
     def __str__(self):
         all_action_strs = []
         for action in self.action_history:
             if len(action) != N_CHARS or (not all([c in CHAR2IDX for c in action])):
                 all_action_strs.append(action)
                 continue
-            action_str = ''
+            action_str = ""
             for i, c in enumerate(action):
-                if self.state.state[CHAR2IDX[c]].position_knowledge[i] == CharKnowledge.HERE:
-                    action_str += colored(c, 'green')
-                elif all([k == CharKnowledge.NOT_HERE for k in self.state.state[CHAR2IDX[c]].position_knowledge]):
+                if (
+                    self.state.state[CHAR2IDX[c]].position_knowledge[i]
+                    == CharKnowledge.HERE
+                ):
+                    action_str += colored(c, "green")
+                elif all(
+                    [
+                        k == CharKnowledge.NOT_HERE
+                        for k in self.state.state[CHAR2IDX[c]].position_knowledge
+                    ]
+                ):
                     action_str += c
-                elif self.state.state[CHAR2IDX[c]].position_knowledge[i] == CharKnowledge.NOT_HERE:
-                    action_str += colored(c, 'yellow')
+                elif (
+                    self.state.state[CHAR2IDX[c]].position_knowledge[i]
+                    == CharKnowledge.NOT_HERE
+                ):
+                    action_str += colored(c, "yellow")
             all_action_strs.append(action_str)
-        return '\n'.join(all_action_strs)
-    
+        return "\n".join(all_action_strs)
+
     def __repr__(self) -> str:
         all_action_strs = []
         for action in self.action_history:
             if len(action) != N_CHARS or (not all([c in CHAR2IDX for c in action])):
-                all_action_strs.append(action + '</a>')
+                all_action_strs.append(action + "</a>")
                 continue
-            action_str = action + '</a>'
+            action_str = action + "</a>"
             for i, c in enumerate(action):
-                if self.state.state[CHAR2IDX[c]].position_knowledge[i] == CharKnowledge.HERE:
-                    action_str += '<g>'
-                elif all([k == CharKnowledge.NOT_HERE for k in self.state.state[CHAR2IDX[c]].position_knowledge]):
-                    action_str += '<b>'
-                elif self.state.state[CHAR2IDX[c]].position_knowledge[i] == CharKnowledge.NOT_HERE:
-                    action_str += '<y>'
+                if (
+                    self.state.state[CHAR2IDX[c]].position_knowledge[i]
+                    == CharKnowledge.HERE
+                ):
+                    action_str += "<g>"
+                elif all(
+                    [
+                        k == CharKnowledge.NOT_HERE
+                        for k in self.state.state[CHAR2IDX[c]].position_knowledge
+                    ]
+                ):
+                    action_str += "<b>"
+                elif (
+                    self.state.state[CHAR2IDX[c]].position_knowledge[i]
+                    == CharKnowledge.NOT_HERE
+                ):
+                    action_str += "<y>"
             all_action_strs.append(action_str)
-        return '<s>' + '</s>'.join(all_action_strs) + ('</s>' if len(all_action_strs) > 0 else '')
-    
+        return (
+            "<s>"
+            + "</s>".join(all_action_strs)
+            + ("</s>" if len(all_action_strs) > 0 else "")
+        )
+
     def transition_sequence(self):
         transition_strs = []
         for x, action in enumerate(self.action_history):
             if len(action) != N_CHARS or (not all([c in CHAR2IDX for c in action])):
                 transition_strs.append((action, -1.0))
                 continue
-            transition_strs.append((action, -1.0 if x < (len(self.action_history) -1) else self.reward()))
-            state_str = ''
+            transition_strs.append(
+                (action, -1.0 if x < (len(self.action_history) - 1) else self.reward())
+            )
+            state_str = ""
             for i, c in enumerate(action):
-                if self.state.state[CHAR2IDX[c]].position_knowledge[i] == CharKnowledge.HERE:
-                    state_str += '<g>'
-                elif all([k == CharKnowledge.NOT_HERE for k in self.state.state[CHAR2IDX[c]].position_knowledge]):
-                    state_str += '<b>'
-                elif self.state.state[CHAR2IDX[c]].position_knowledge[i] == CharKnowledge.NOT_HERE:
-                    state_str += '<y>'
+                if (
+                    self.state.state[CHAR2IDX[c]].position_knowledge[i]
+                    == CharKnowledge.HERE
+                ):
+                    state_str += "<g>"
+                elif all(
+                    [
+                        k == CharKnowledge.NOT_HERE
+                        for k in self.state.state[CHAR2IDX[c]].position_knowledge
+                    ]
+                ):
+                    state_str += "<b>"
+                elif (
+                    self.state.state[CHAR2IDX[c]].position_knowledge[i]
+                    == CharKnowledge.NOT_HERE
+                ):
+                    state_str += "<y>"
             transition_strs.append((state_str, None))
         return transition_strs, self.is_terminal()
 
     def reward(self):
         if len(self.action_history) > 0 and len(self.action_history[-1]) != N_CHARS:
             return -1.0
-        return int(self.vocab.filtered_vocab_size() == 1 and self.vocab.filtered_vocab[0] in self.action_history) - 1
-    
+        return (
+            int(
+                self.vocab.filtered_vocab_size() == 1
+                and self.vocab.filtered_vocab[0] in self.action_history
+            )
+            - 1
+        )
+
     def is_terminal(self):
         return len(self.action_history) == N_TRIES or self.reward() == 0
```

### Comparing `agilerl-0.1.8/agilerl/wordle/wordle_tokenizer.py` & `agilerl-0.1.9/agilerl/wordle/wordle_tokenizer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,79 @@
 import re
+
 from agilerl.data.tokenizer import Tokenizer
 
+
 class WordleTokenizer(Tokenizer):
     def __init__(self):
-        self.special_vocab = ['<g>', '<b>', '<y>', '<|pad|>', '</a>', '</s>', '<s>', 
-                              '<a>', '</eod>']
-        self.vocab = list('abcdefghijklmnopqrstuvwxyz') + self.special_vocab
+        self.special_vocab = [
+            "<g>",
+            "<b>",
+            "<y>",
+            "<|pad|>",
+            "</a>",
+            "</s>",
+            "<s>",
+            "<a>",
+            "</eod>",
+        ]
+        self.vocab = list("abcdefghijklmnopqrstuvwxyz") + self.special_vocab
         self.t2i = {w: i for i, w in enumerate(self.vocab)}
-        super().__init__(self.token_to_id('<|pad|>'), 
-                         self.token_to_id('</s>'), 
-                         self.token_to_id('</a>'), 
-                         self.token_to_id('<s>'), 
-                         self.token_to_id('<a>'), 
-                         self.token_to_id('</eod>'))
-    
+        super().__init__(
+            self.token_to_id("<|pad|>"),
+            self.token_to_id("</s>"),
+            self.token_to_id("</a>"),
+            self.token_to_id("<s>"),
+            self.token_to_id("<a>"),
+            self.token_to_id("</eod>"),
+        )
+
     def encode(self, str_, **kwargs):
         if isinstance(str_, str):
             special_idxs = []
             for special_char in self.special_vocab:
-                special_idxs += list(map(lambda x: (x.start(), x.end(), 
-                                                    self.token_to_id(special_char)), 
-                                                    re.finditer(re.escape(special_char), 
-                                                                str_)))
+                special_idxs += list(
+                    map(
+                        lambda x: (x.start(), x.end(), self.token_to_id(special_char)),
+                        re.finditer(re.escape(special_char), str_),
+                    )
+                )
             special_idxs.sort(key=lambda x: x[0])
             tokens = []
             curr = 0
             for s, e, tok in special_idxs:
                 tokens.extend([self.token_to_id(c) for c in str_[curr:s]])
                 tokens.append(tok)
                 curr = e
             tokens.extend([self.token_to_id(c) for c in str_[curr:]])
             return tokens, [int(t != self.pad_token_id) for t in tokens]
         elif isinstance(str_, list):
             tokens, pads = zip(*[self.encode(item) for item in str_])
             max_len = max(map(len, tokens))
-            return [list(item)+([self.pad_token_id]*(max_len-len(
-                item))) for item in tokens], [list(item)+([0]*(max_len-len(
-                item))) for item in pads]
+            return [
+                list(item) + ([self.pad_token_id] * (max_len - len(item)))
+                for item in tokens
+            ], [list(item) + ([0] * (max_len - len(item))) for item in pads]
         else:
-            raise ValueError('str_ must be a string or a list of strings')
-    
+            raise ValueError("str_ must be a string or a list of strings")
+
     def decode(self, tokens, **kwargs):
         if len(tokens) == 0:
-            return ''
+            return ""
         if not isinstance(tokens[0], list):
-            return ''.join([self.id_to_token(item) for item in tokens])
+            return "".join([self.id_to_token(item) for item in tokens])
         elif isinstance(tokens[0], list):
             return [self.decode(item) for item in tokens]
         else:
-            raise ValueError('tokens must be a list of ints or a list of lists of ints')
-    
+            raise ValueError("tokens must be a list of ints or a list of lists of ints")
+
     def num_tokens(self):
         return len(self.vocab)
-    
+
     def id_to_token(self, id_):
         return self.vocab[id_]
-    
+
     def token_to_id(self, token):
         return self.t2i[token]
-    
+
     def get_vocab(self):
         return self.vocab
```

### Comparing `agilerl-0.1.8/pyproject.toml` & `agilerl-0.1.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agilerl"
-version = "0.1.8"
+version = "0.1.9"
 description = "AgileRL is a deep reinforcement learning library focused on improving RL development through RLOps."
 authors = ["Nick Ustaran-Anderegg <dev@agilerl.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -17,14 +17,15 @@
 hydra-core = "^1.3.2"
 importlib = "^1.0.4"
 matplotlib = "^3.4.3"
 minari = "^0.4.1"
 numpy = "^1.24.2"
 omegaconf = "^2.3.0"
 pettingzoo = "^1.23.1"
+pre-commit = "^3.4.0"
 redis = "^4.4.4"
 SuperSuit = "^3.9.0"
 termcolor = "^1.1.0"
 torch = "^2.0.1"
 tqdm = "^4.65.0"
 transformers = "^4.30.0"
 wandb = "^0.13.10"
```

### Comparing `agilerl-0.1.8/PKG-INFO` & `agilerl-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agilerl
-Version: 0.1.8
+Version: 0.1.9
 Summary: AgileRL is a deep reinforcement learning library focused on improving RL development through RLOps.
 License: Apache 2.0
 Author: Nick Ustaran-Anderegg
 Author-email: dev@agilerl.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -22,14 +22,15 @@
 Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
 Requires-Dist: importlib (>=1.0.4,<2.0.0)
 Requires-Dist: matplotlib (>=3.4.3,<4.0.0)
 Requires-Dist: minari (>=0.4.1,<0.5.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: pettingzoo (>=1.23.1,<2.0.0)
+Requires-Dist: pre-commit (>=3.4.0,<4.0.0)
 Requires-Dist: redis (>=4.4.4,<5.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: transformers (>=4.30.0,<5.0.0)
 Requires-Dist: wandb (>=0.13.10,<0.14.0)
 Description-Content-Type: text/markdown
@@ -49,15 +50,15 @@
 
 **_NEW: AgileRL now supports distributed training with HuggingFace Accelerate!<br>
 Train even faster by taking full advantage of your entire compute stack._**
 
 </div>
 
 This is a Deep Reinforcement Learning library focused on improving development by introducing RLOps - MLOps for reinforcement learning.
-  
+
 This library is initially focused on reducing the time taken for training models and hyperparameter optimization (HPO) by pioneering evolutionary HPO techniques for reinforcement learning.<br>
 Evolutionary HPO has been shown to drastically reduce overall training times by automatically converging on optimal hyperparameters, without requiring numerous training runs.<br>
 We are constantly adding more algorithms, with a view to add hierarchical and multi-agent algorithms soon.
 
 <p align="center">
   <img src=https://user-images.githubusercontent.com/47857277/236407686-21363eb3-ffcf-419f-b019-0be4ddf1ed4a.gif height="250">
 </p>
@@ -69,37 +70,44 @@
   * [Algorithms implemented](#algorithms-implemented-more-coming-soon)
   * [Train an agent on a Gym environment (Online)](#train-an-agent-on-a-gym-environment-online)
     + [Custom Online Training Loop](#custom-online-training-loop)
   * [Train an agent on data (Offline)](#train-an-agent-on-data-offline)
     + [Custom Offline Training Loop](#custom-offline-training-loop)
   * [Train an agent on a language environment (RLHF)](#train-an-agent-on-a-language-environment-rlhf)
   * [Distributed training](#distributed-training)
+  * [Multi-agent training](#multi-agent-training)
 
 ## Benchmarks
 
 Reinforcement learning algorithms and libraries are usually benchmarked once the optimal hyperparameters for training are known, but it often takes hundreds or thousands of experiments to discover these. This is unrealistic and does not reflect the true, total time taken for training. What if we could remove the need to conduct all these prior experiments?
 
 In the charts below, a single AgileRL run, which automatically tunes hyperparameters, is benchmarked against Optuna's multiple training runs traditionally required for hyperparameter optimization, demonstrating the real time savings possible. Global steps is the sum of every step taken by any agent in the environment, including across an entire population.
 
 <p align="center">
   <img src=https://user-images.githubusercontent.com/47857277/227481592-27a9688f-7c0a-4655-ab32-90d659a71c69.png height="500">
 </p>
 <p align="center">AgileRL offers an order of magnitude speed up in hyperparameter optimization vs popular reinforcement learning training frameworks combined with Optuna. Remove the need for multiple training runs and save yourself hours.</p>
 
+AgileRL also supports multi-agent reinforcement learning using the Petting Zoo-style (parallel API). The charts below highlight the performance of our MADDPG and MATD3 algorithms with evolutionary hyper-parameter optimisation (HPO), benchmarked against epymarl's MADDPG algorithm with grid-search HPO for the simple speaker listener and simple spread environments.
+
+<p align="center">
+  <img src=https://github-production-user-asset-6210df.s3.amazonaws.com/118982716/264712154-4965ea5f-b777-423c-989b-e4db86eda3bd.png>
+</p>
+
 ## Get Started
-Install as a package with pip: 
+Install as a package with pip:
 ```bash
 pip install agilerl
 ```
 Or install in development mode: (Recommended due to nascent nature of this library)
 ```bash
 git clone https://github.com/AgileRL/AgileRL.git && cd AgileRL
 pip install -r requirements.txt
 ```
-If using ILQL on Wordle, download and unzip data.zip <a href="https://drive.google.com/drive/folders/13LFspsFQ-7XIlFjnsZttKf4nfVDlnmW2?usp=sharing">here</a>. 
+If using ILQL on Wordle, download and unzip data.zip <a href="https://drive.google.com/drive/folders/13LFspsFQ-7XIlFjnsZttKf4nfVDlnmW2?usp=sharing">here</a>.
 
 Demo:
 ```bash
 python demo_online.py
 ```
 or to demo distributed training:
 ```bash
@@ -108,14 +116,16 @@
 
 ## Algorithms implemented (more coming soon!)
   * DQN
   * DDPG
   * CQL
   * ILQL
   * TD3
+  * MADDPG
+  * MATD3
 
 ## Train an agent on a Gym environment (Online)
 Before starting training, there are some meta-hyperparameters and settings that must be set. These are defined in <code>INIT_HP</code>, for general parameters, and <code>MUTATION_PARAMS</code>, which define the evolutionary probabilities, and <code>NET_CONFIG</code>, which defines the network architecture. For example:
 ```python
 INIT_HP = {
     'ENV_NAME': 'LunarLander-v2',   # Gym environment name
     'ALGO': 'DQN',                  # Algorithm
@@ -333,36 +343,36 @@
         state = env.reset()[0]  # Reset environment at start of episode
         score = 0
         for idx_step in range(max_steps):
             if INIT_HP['CHANNELS_LAST']:
                 state = np.moveaxis(state, [3], [1])
             action = agent.getAction(state, epsilon)    # Get next action from agent
             next_state, reward, done, _, _ = env.step(action)   # Act in environment
-            
+
             # Save experience to replay buffer
             if INIT_HP['CHANNELS_LAST']:
                 memory.save2memoryVectEnvs(
                     state, action, reward, np.moveaxis(next_state, [3], [1]), done)
             else:
                 memory.save2memoryVectEnvs(
                     state, action, reward, next_state, done)
 
             # Learn according to learning frequency
             if memory.counter % agent.learn_step == 0 and len(memory) >= agent.batch_size:
                 experiences = memory.sample(agent.batch_size) # Sample replay buffer
                 agent.learn(experiences)    # Learn according to agent's RL algorithm
-            
+
             state = next_state
             score += reward
 
     epsilon = max(eps_end, epsilon*eps_decay) # Update epsilon for exploration
 
     # Now evolve population if necessary
     if (idx_epi+1) % evo_epochs == 0:
-        
+
         # Evaluate population
         fitnesses = [agent.test(env, swap_channels=INIT_HP['CHANNELS_LAST'], max_steps=max_steps, loop=evo_loop) for agent in pop]
 
         print(f'Episode {idx_epi+1}/{max_episodes}')
         print(f'Fitnesses: {["%.2f"%fitness for fitness in fitnesses]}')
         print(f'100 fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:]) for agent in pop]}')
 
@@ -612,15 +622,15 @@
         for idx_step in range(max_steps):
             experiences = memory.sample(agent.batch_size)   # Sample replay buffer
             # Learn according to agent's RL algorithm
             agent.learn(experiences)
 
     # Now evolve population if necessary
     if (idx_epi+1) % evo_epochs == 0:
-        
+
         # Evaluate population
         fitnesses = [agent.test(env, swap_channels=False, max_steps=max_steps, loop=evo_loop) for agent in pop]
 
         print(f'Episode {idx_epi+1}/{max_episodes}')
         print(f'Fitnesses: {["%.2f"%fitness for fitness in fitnesses]}')
         print(f'100 fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:]) for agent in pop]}')
 
@@ -628,38 +638,38 @@
         elite, pop = tournament.select(pop)
         pop = mutations.mutation(pop)
 
 env.close()
 ```
 
 ## Train an agent on a language environment (RLHF)
-We implement RLHF on Wordle, and use <a href="https://arxiv.org/pdf/2206.11871.pdf">ILQL</a> to finetune our model. To create your own language environment, 
+We implement RLHF on Wordle, and use <a href="https://arxiv.org/pdf/2206.11871.pdf">ILQL</a> to finetune our model. To create your own language environment,
 see https://github.com/Sea-Snell/Implicit-Language-Q-Learning.
-The <code>EvolvableGPT</code> class allows us to combine LLMs and transformer architectures with evolvable HPO, which can massively reduce the time taken to finetune 
-these expensive models. Due to the vast number of parameters and settings involved in training a Large Language Model (LLM) on human feedback, these are defined in 
-<code>configs</code>. 
+The <code>EvolvableGPT</code> class allows us to combine LLMs and transformer architectures with evolvable HPO, which can massively reduce the time taken to finetune
+these expensive models. Due to the vast number of parameters and settings involved in training a Large Language Model (LLM) on human feedback, these are defined in
+<code>configs</code>.
 
-In order to finetune a model with RLHF, we need a trained model as a starting point. We can use behavioural cloning (BC, supervised learning) to build this first version of 
+In order to finetune a model with RLHF, we need a trained model as a starting point. We can use behavioural cloning (BC, supervised learning) to build this first version of
 the model. To train your own model from scratch:
 ```bash
 python run_bc_lm.py
 ```
 If you want to use pretrained model weights, these can be defined in <code>configs/wordle/train_bc.yaml</code> in <code>model: load:</code>.
 
 Similarly, to then run ILQL and perform RLHF on the BC model:
 ```bash
 python run_ilql.py
 ```
 
 ## Distributed training
-AgileRL can also be used for distributed training if you have multiple devices you want to take advantage of. We use the HuggingFace 
-<a href="https://github.com/huggingface/accelerate">Accelerate</a> library to implement this in an open manner, without hiding behind too many layers of abstraction. 
+AgileRL can also be used for distributed training if you have multiple devices you want to take advantage of. We use the HuggingFace
+<a href="https://github.com/huggingface/accelerate">Accelerate</a> library to implement this in an open manner, without hiding behind too many layers of abstraction.
 This should make implementations simple, but also highly customisable, by continuing to expose the PyTorch training loop beneath it all.
 
-To launch distributed training scripts in bash, use <code>accelerate launch</code>. To customise the distributed training properties, specify the key <code>--config_file</code>. An example 
+To launch distributed training scripts in bash, use <code>accelerate launch</code>. To customise the distributed training properties, specify the key <code>--config_file</code>. An example
 config file has been provided at <code>configs/accelerate/accelerate.yaml</code>.
 
 Putting this all together, launching a distributed training script can be done as follows:
 ```bash
 accelerate_launch --config_file configs/accelerate/accelerate.yaml demo_online_distributed.py
 ```
 
@@ -731,16 +741,16 @@
     field_names = ["state", "action", "reward", "next_state", "done"]
     memory = ReplayBuffer(action_dim=action_dim,    # Number of agent actions
                         memory_size=10000,        # Max replay buffer size
                         field_names=field_names)  # Field names to store in memory
     replay_dataset = ReplayDataset(memory, INIT_HP['BATCH_SIZE'])
     replay_dataloader = DataLoader(replay_dataset, batch_size=None)
     replay_dataloader = accelerator.prepare(replay_dataloader)
-    sampler = Sampler(distributed=True, 
-                    dataset=replay_dataset, 
+    sampler = Sampler(distributed=True,
+                    dataset=replay_dataset,
                     dataloader=replay_dataloader)
 
     tournament = TournamentSelection(tournament_size=2,  # Tournament selection size
                                     elitism=True,      # Elitism in tournament selection
                                     population_size=INIT_HP['POPULATION_SIZE'],  # Population size
                                     evo_step=1)        # Evaluate using last N fitness scores
 
@@ -839,9 +849,163 @@
             accelerator.wait_for_everyone()
             for model in pop:
                 model.wrap_models()
 
     env.close()
 ```
 
+## Multi-agent training
+
+As in previous examples, before starting training, meta-hyperparameters ```INIT_HP```, ```MUTATION_PARAMS```, and ```NET_CONFIG``` must first be defined.
+
+```python
+NET_CONFIG = {
+        'arch': 'mlp',          # Network architecture
+        'h_size': [32, 32],     # Actor hidden size
+    }
+
+    INIT_HP = {
+        'ALGO': 'MADDPG',               # Algorithm
+        'BATCH_SIZE': 512,              # Batch size
+        'LR': 0.01,                     # Learning rate
+        'EPISODES': 10_000,             # Max no. episodes
+        'GAMMA': 0.95,                  # Discount factor
+        'MEMORY_SIZE': 1_000_000,       # Max memory buffer size
+        'LEARN_STEP': 5,                # Learning frequency
+        'TAU': 0.01,                    # For soft update of target parameters
+        # Swap image channels dimension from last to first [H, W, C] -> [C, H, W]
+        'CHANNELS_LAST': False,
+        "WANDB": False                  # Start run with Weights&Biases
+    }
+
+    MUTATION_PARAMS = {
+        "NO_MUT": 0.4,                              # No mutation
+        "ARCH_MUT": 0.2,                            # Architecture mutation
+        "NEW_LAYER": 0.2,                           # New layer mutation
+        "PARAMS_MUT": 0.2,                           # Network parameters mutation
+        "ACT_MUT": 0,                               # Activation layer mutation
+        "RL_HP_MUT": 0.2,                           # Learning HP mutation
+        # Learning HPs to choose from
+        "RL_HP_SELECTION": ["lr", "batch_size", "learn_step"],
+        "MUT_SD": 0.1,                              # Mutation strength
+        "RAND_SEED": 42,                            # Random seed
+        "MIN_LR": 0.0001,                           # Define max and min limits for mutating RL hyperparams
+        "MAX_LR": 0.01,
+        "MIN_LEARN_STEP": 1,
+        "MAX_LEARN_STEP": 200,
+        "MIN_BATCH_SIZE": 8,
+        "MAX_BATCH_SIZE": 1024
+    }
+```
+Use ```utils.utils.initialPopulation``` to create a list of agents - our population that will evolve and mutate to the optimal hyperparameters.
+```python
+    from agilerl.utils.utils import initialPopulation
+    from pettingzoo.mpe import simple_speaker_listener_v4
+    import torch
+
+    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+    env = simple_speaker_listener_v4.parallel_env(continuous_actions=True)
+    env.reset()
+
+    # Configure the multi-agent algo input arguments
+    try:
+        state_dim = [env.observation_space(agent).n for agent in env.agents]
+        one_hot = True
+    except Exception:
+        state_dim = [env.observation_space(agent).shape for agent in env.agents]
+        one_hot = False
+    try:
+        action_dim = [env.action_space(agent).n for agent in env.agents]
+        INIT_HP['DISCRETE_ACTIONS'] = True
+        INIT_HP['MAX_ACTION'] = None
+        INIT_HP['MIN_ACTION'] = None
+    except Exception:
+        action_dim = [env.action_space(agent).shape[0] for agent in env.agents]
+        INIT_HP['DISCRETE_ACTIONS'] = False
+        INIT_HP['MAX_ACTION'] = [env.action_space(agent).high for agent in env.agents]
+        INIT_HP['MIN_ACTION'] = [env.action_space(agent).low for agent in env.agents]
+
+    if INIT_HP['CHANNELS_LAST']:
+        state_dim = [(state_dim[2], state_dim[0], state_dim[1]) for state_dim in state_dim]
+
+    INIT_HP['N_AGENTS'] = env.num_agents
+    INIT_HP['AGENT_IDS'] = [agent_id for agent_id in env.agents]
+
+    agent_pop = initialPopulation(algo=INIT_HP['ALGO'],
+                                  state_dim=state_dim,
+                                  action_dim=action_dim,
+                                  one_hot=one_hot,
+                                  net_config=NET_CONFIG,
+                                  INIT_HP=INIT_HP,
+                                  population_size=6,
+                                  device=device)
+
+```
+
+Next, create the tournament, mutations and experience replay buffer objects that allow agents to share memory and efficiently perform evolutionary HPO.
+
+```python
+    from agilerl.components.multi_agent_replay_buffer import MultiAgentReplayBuffer
+    from agilerl.hpo.tournament import TournamentSelection
+    from agilerl.hpo.mutation import Mutations
+
+    field_names = ["state", "action", "reward", "next_state", "done"]
+
+    memory = MultiAgentReplayBuffer(memory_size=1_000_000,        # Max replay buffer size
+                                    field_names=field_names,  # Field names to store in memory
+                                    agent_ids=INIT_HP['AGENT_IDS'],
+                                    device=torch.device("cuda"))
+
+    tournament = TournamentSelection(tournament_size=2, # Tournament selection size
+                                     elitism=True,      # Elitism in tournament selection
+                                     population_size=6, # Population size
+                                     evo_step=1)        # Evaluate using last N fitness scores
+
+    mutations = Mutations(algo=INIT_HP['ALGO'],
+                          no_mutation=MUTATION_PARAMS['NO_MUT'],
+                          architecture=MUTATION_PARAMS['ARCH_MUT'],
+                          new_layer_prob=MUTATION_PARAMS['NEW_LAYER'],
+                          parameters=MUTATION_PARAMS['PARAMS_MUT'],
+                          activation=MUTATION_PARAMS['ACT_MUT'],
+                          rl_hp=MUTATION_PARAMS['RL_HP_MUT'],
+                          rl_hp_selection=MUTATION_PARAMS['RL_HP_SELECTION'],
+                          mutation_sd=MUTATION_PARAMS['MUT_SD'],
+                          min_lr=MUTATION_PARAMS['MIN_LR'],
+                          max_lr=MUTATION_PARAMS['MAX_LR'],
+                          min_learn_step=MUTATION_PARAMS['MIN_LEARN_STEP'],
+                          max_learn_step=MUTATION_PARAMS['MAX_LEARN_STEP'],
+                          min_batch_size=MUTATION_PARAMS['MIN_BATCH_SIZE'],
+                          max_batch_size=MUTATION_PARAMS['MAX_BATCH_SIZE'],
+                          agent_ids=INIT_HP['AGENT_IDS'],
+                          arch=NET_CONFIG['arch'],
+                          rand_seed=MUTATION_PARAMS['RAND_SEED'],
+                          device=device)
+
+```
+The easiest training loop implementation is to use our ```training.train_multi_agent.train_multi_agent()``` function. It requires the agent have functions ```getAction()``` and ```learn()```.
+
+```python
+
+    from agilerl.training.train_multi_agent import train_multi_agent
+    import torch
+
+    trained_pop, pop_fitnesses = train_multi_agent(env=env,                              # Pettingzoo-style environment
+                                                env_name='simple_speaker_listener_v4',   # Environment name
+                                                algo=INIT_HP['ALGO'],                    # Algorithm
+                                                pop=agent_pop,                           # Population of agents
+                                                memory=memory,                           # Replay buffer
+                                                INIT_HP=INIT_HP,                         # IINIT_HP dictionary
+                                                MUT_P=MUTATION_PARAMS,                   # MUTATION_PARAMS dictionary
+                                                net_config=NET_CONFIG,                   # Network configuration
+                                                swap_channels=INIT_HP['CHANNELS_LAST'],  # Swap image channel from last to first
+                                                n_episodes=INIT_HP['EPISODES'],          # Max number of training episodes
+                                                evo_epochs=20,                           # Evolution frequency
+                                                evo_loop=1,                              # Number of evaluation episodes per agent
+                                                max_steps=900,                           # Max steps to take in the environment
+                                                target=200.,                             # Target score for early stopping
+                                                tournament=tournament,                   # Tournament selection object
+                                                mutation=mutations,                      # Mutations object
+                                                wb=INIT_HP["WANDB"])                     # Weights and Biases tracking
+
+```
 View <a href="https://agilerl.readthedocs.io/en/latest/">documentation</a>.
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: agilerl Version: 0.1.8 Summary: AgileRL is a deep
+Metadata-Version: 2.1 Name: agilerl Version: 0.1.9 Summary: AgileRL is a deep
 reinforcement learning library focused on improving RL development through
 RLOps. License: Apache 2.0 Author: Nick Ustaran-Anderegg Author-email:
 dev@agilerl.com Requires-Python: >=3.8,<4.0 Classifier: License :: Other/
 Proprietary License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: SuperSuit
 (>=3.9.0,<4.0.0) Requires-Dist: accelerate (>=0.18.0,<0.19.0) Requires-Dist:
 dill (>=0.3.7,<0.4.0) Requires-Dist: fastrand (>=1.3.0,<2.0.0) Requires-Dist:
 flatten_dict (>=0.4.2,<0.5.0) Requires-Dist: gymnasium (>=0.28.1,<0.29.0)
 Requires-Dist: h5py (>=3.8.0,<4.0.0) Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
 Requires-Dist: importlib (>=1.0.4,<2.0.0) Requires-Dist: matplotlib
 (>=3.4.3,<4.0.0) Requires-Dist: minari (>=0.4.1,<0.5.0) Requires-Dist: numpy
 (>=1.24.2,<2.0.0) Requires-Dist: omegaconf (>=2.3.0,<3.0.0) Requires-Dist:
-pettingzoo (>=1.23.1,<2.0.0) Requires-Dist: redis (>=4.4.4,<5.0.0) Requires-
-Dist: termcolor (>=1.1.0,<2.0.0) Requires-Dist: torch (>=2.0.1,<3.0.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0) Requires-Dist: transformers
-(>=4.30.0,<5.0.0) Requires-Dist: wandb (>=0.13.10,<0.14.0) Description-Content-
-Type: text/markdown # AgileRL
+pettingzoo (>=1.23.1,<2.0.0) Requires-Dist: pre-commit (>=3.4.0,<4.0.0)
+Requires-Dist: redis (>=4.4.4,<5.0.0) Requires-Dist: termcolor (>=1.1.0,<2.0.0)
+Requires-Dist: torch (>=2.0.1,<3.0.0) Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: transformers (>=4.30.0,<5.0.0) Requires-Dist: wandb
+(>=0.13.10,<0.14.0) Description-Content-Type: text/markdown # AgileRL
  [https://user-images.githubusercontent.com/47857277/222710068-e09a4e3c-368c-
                           458a-9e01-b68674806887.png]
                       RReeiinnffoorrcceemmeenntt lleeaarrnniinngg ssttrreeaammlliinneedd..
  Easier and faster reinforcement learning with RLOps. Visit our _w_e_b_s_i_t_e. View
                                 _d_o_c_u_m_e_n_t_a_t_i_o_n.
                     Join the _D_i_s_c_o_r_d_ _S_e_r_v_e_r to collaborate.
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://
@@ -52,61 +52,68 @@
 ## Table of Contents * [Benchmarks](#benchmarks) * [Get Started](#get-started)
 * [Algorithms implemented](#algorithms-implemented-more-coming-soon) * [Train
 an agent on a Gym environment (Online)](#train-an-agent-on-a-gym-environment-
 online) + [Custom Online Training Loop](#custom-online-training-loop) * [Train
 an agent on data (Offline)](#train-an-agent-on-data-offline) + [Custom Offline
 Training Loop](#custom-offline-training-loop) * [Train an agent on a language
 environment (RLHF)](#train-an-agent-on-a-language-environment-rlhf) *
-[Distributed training](#distributed-training) ## Benchmarks Reinforcement
-learning algorithms and libraries are usually benchmarked once the optimal
-hyperparameters for training are known, but it often takes hundreds or
-thousands of experiments to discover these. This is unrealistic and does not
-reflect the true, total time taken for training. What if we could remove the
-need to conduct all these prior experiments? In the charts below, a single
-AgileRL run, which automatically tunes hyperparameters, is benchmarked against
-Optuna's multiple training runs traditionally required for hyperparameter
-optimization, demonstrating the real time savings possible. Global steps is the
-sum of every step taken by any agent in the environment, including across an
-entire population.
+[Distributed training](#distributed-training) * [Multi-agent training](#multi-
+agent-training) ## Benchmarks Reinforcement learning algorithms and libraries
+are usually benchmarked once the optimal hyperparameters for training are
+known, but it often takes hundreds or thousands of experiments to discover
+these. This is unrealistic and does not reflect the true, total time taken for
+training. What if we could remove the need to conduct all these prior
+experiments? In the charts below, a single AgileRL run, which automatically
+tunes hyperparameters, is benchmarked against Optuna's multiple training runs
+traditionally required for hyperparameter optimization, demonstrating the real
+time savings possible. Global steps is the sum of every step taken by any agent
+in the environment, including across an entire population.
  [https://user-images.githubusercontent.com/47857277/227481592-27a9688f-7c0a-
                           4655-ab32-90d659a71c69.png]
 AgileRL offers an order of magnitude speed up in hyperparameter optimization vs
 popular reinforcement learning training frameworks combined with Optuna. Remove
          the need for multiple training runs and save yourself hours.
+AgileRL also supports multi-agent reinforcement learning using the Petting Zoo-
+style (parallel API). The charts below highlight the performance of our MADDPG
+and MATD3 algorithms with evolutionary hyper-parameter optimisation (HPO),
+benchmarked against epymarl's MADDPG algorithm with grid-search HPO for the
+simple speaker listener and simple spread environments.
+   [https://github-production-user-asset-6210df.s3.amazonaws.com/118982716/
+              264712154-4965ea5f-b777-423c-989b-e4db86eda3bd.png]
 ## Get Started Install as a package with pip: ```bash pip install agilerl ```
 Or install in development mode: (Recommended due to nascent nature of this
 library) ```bash git clone https://github.com/AgileRL/AgileRL.git && cd AgileRL
 pip install -r requirements.txt ``` If using ILQL on Wordle, download and unzip
 data.zip _h_e_r_e. Demo: ```bash python demo_online.py ``` or to demo distributed
 training: ```bash accelerate launch --config_file configs/accelerate/
 accelerate.yaml demo_online_distributed.py ``` ## Algorithms implemented (more
-coming soon!) * DQN * DDPG * CQL * ILQL * TD3 ## Train an agent on a Gym
-environment (Online) Before starting training, there are some meta-
-hyperparameters and settings that must be set. These are defined in INIT_HP,
-for general parameters, and MUTATION_PARAMS, which define the evolutionary
-probabilities, and NET_CONFIG, which defines the network architecture. For
-example: ```python INIT_HP = { 'ENV_NAME': 'LunarLander-v2', # Gym environment
-name 'ALGO': 'DQN', # Algorithm 'DOUBLE': True, # Use double Q-learning
-'CHANNELS_LAST': False, # Swap image channels dimension from last to first [H,
-W, C] -> [C, H, W] 'BATCH_SIZE': 256, # Batch size 'LR': 1e-3, # Learning rate
-'EPISODES': 2000, # Max no. episodes 'TARGET_SCORE': 200., # Early training
-stop at avg score of last 100 episodes 'GAMMA': 0.99, # Discount factor
-'MEMORY_SIZE': 10000, # Max memory buffer size 'LEARN_STEP': 1, # Learning
-frequency 'TAU': 1e-3, # For soft update of target parameters 'TOURN_SIZE': 2,
-# Tournament size 'ELITISM': True, # Elitism in tournament selection
-'POP_SIZE': 6, # Population size 'EVO_EPOCHS': 20, # Evolution frequency
-'POLICY_FREQ': 2, # Policy network update frequency 'WANDB': True # Log with
-Weights and Biases } ``` ```python MUTATION_PARAMS = { # Relative probabilities
-'NO_MUT': 0.4, # No mutation 'ARCH_MUT': 0.2, # Architecture mutation
-'NEW_LAYER': 0.2, # New layer mutation 'PARAMS_MUT': 0.2, # Network parameters
-mutation 'ACT_MUT': 0, # Activation layer mutation 'RL_HP_MUT': 0.2, # Learning
-HP mutation 'RL_HP_SELECTION': ['lr', 'batch_size'], # Learning HPs to choose
-from 'MUT_SD': 0.1, # Mutation strength 'RAND_SEED': 1, # Random seed } ```
-```python NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size': [32,
-32], # Actor hidden size } ``` First, use utils.utils.initialPopulation to
+coming soon!) * DQN * DDPG * CQL * ILQL * TD3 * MADDPG * MATD3 ## Train an
+agent on a Gym environment (Online) Before starting training, there are some
+meta-hyperparameters and settings that must be set. These are defined in
+INIT_HP, for general parameters, and MUTATION_PARAMS, which define the
+evolutionary probabilities, and NET_CONFIG, which defines the network
+architecture. For example: ```python INIT_HP = { 'ENV_NAME': 'LunarLander-v2',
+# Gym environment name 'ALGO': 'DQN', # Algorithm 'DOUBLE': True, # Use double
+Q-learning 'CHANNELS_LAST': False, # Swap image channels dimension from last to
+first [H, W, C] -> [C, H, W] 'BATCH_SIZE': 256, # Batch size 'LR': 1e-3, #
+Learning rate 'EPISODES': 2000, # Max no. episodes 'TARGET_SCORE': 200., #
+Early training stop at avg score of last 100 episodes 'GAMMA': 0.99, # Discount
+factor 'MEMORY_SIZE': 10000, # Max memory buffer size 'LEARN_STEP': 1, #
+Learning frequency 'TAU': 1e-3, # For soft update of target parameters
+'TOURN_SIZE': 2, # Tournament size 'ELITISM': True, # Elitism in tournament
+selection 'POP_SIZE': 6, # Population size 'EVO_EPOCHS': 20, # Evolution
+frequency 'POLICY_FREQ': 2, # Policy network update frequency 'WANDB': True #
+Log with Weights and Biases } ``` ```python MUTATION_PARAMS = { # Relative
+probabilities 'NO_MUT': 0.4, # No mutation 'ARCH_MUT': 0.2, # Architecture
+mutation 'NEW_LAYER': 0.2, # New layer mutation 'PARAMS_MUT': 0.2, # Network
+parameters mutation 'ACT_MUT': 0, # Activation layer mutation 'RL_HP_MUT': 0.2,
+# Learning HP mutation 'RL_HP_SELECTION': ['lr', 'batch_size'], # Learning HPs
+to choose from 'MUT_SD': 0.1, # Mutation strength 'RAND_SEED': 1, # Random seed
+} ``` ```python NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size':
+[32, 32], # Actor hidden size } ``` First, use utils.utils.initialPopulation to
 create a list of agents - our population that will evolve and mutate to the
 optimal hyperparameters. ```python from agilerl.utils.utils import
 makeVectEnvs, initialPopulation import torch device = torch.device("cuda" if
 torch.cuda.is_available() else "cpu") env = makeVectEnvs(env_name=INIT_HP
 ['ENV_NAME'], num_envs=16) try: state_dim = env.single_observation_space.n #
 Discrete observation space one_hot = True # Requires one-hot encoding except
 Exception: state_dim = env.single_observation_space.shape # Continuous
@@ -456,8 +463,86 @@
 pop: model.unwrap_models() accelerator.wait_for_everyone() if
 accelerator.is_main_process: elite, pop = tournament.select(pop) pop =
 mutations.mutation(pop) for pop_i, model in enumerate(pop):
 model.saveCheckpoint(f'{accel_temp_models_path}/DQN_{pop_i}.pt')
 accelerator.wait_for_everyone() if not accelerator.is_main_process: for pop_i,
 model in enumerate(pop): model.loadCheckpoint(f'{accel_temp_models_path}/DQN_
 {pop_i}.pt') accelerator.wait_for_everyone() for model in pop:
-model.wrap_models() env.close() ``` View _d_o_c_u_m_e_n_t_a_t_i_o_n.
+model.wrap_models() env.close() ``` ## Multi-agent training As in previous
+examples, before starting training, meta-hyperparameters ```INIT_HP```,
+```MUTATION_PARAMS```, and ```NET_CONFIG``` must first be defined. ```python
+NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size': [32, 32], #
+Actor hidden size } INIT_HP = { 'ALGO': 'MADDPG', # Algorithm 'BATCH_SIZE':
+512, # Batch size 'LR': 0.01, # Learning rate 'EPISODES': 10_000, # Max no.
+episodes 'GAMMA': 0.95, # Discount factor 'MEMORY_SIZE': 1_000_000, # Max
+memory buffer size 'LEARN_STEP': 5, # Learning frequency 'TAU': 0.01, # For
+soft update of target parameters # Swap image channels dimension from last to
+first [H, W, C] -> [C, H, W] 'CHANNELS_LAST': False, "WANDB": False # Start run
+with Weights&Biases } MUTATION_PARAMS = { "NO_MUT": 0.4, # No mutation
+"ARCH_MUT": 0.2, # Architecture mutation "NEW_LAYER": 0.2, # New layer mutation
+"PARAMS_MUT": 0.2, # Network parameters mutation "ACT_MUT": 0, # Activation
+layer mutation "RL_HP_MUT": 0.2, # Learning HP mutation # Learning HPs to
+choose from "RL_HP_SELECTION": ["lr", "batch_size", "learn_step"], "MUT_SD":
+0.1, # Mutation strength "RAND_SEED": 42, # Random seed "MIN_LR": 0.0001, #
+Define max and min limits for mutating RL hyperparams "MAX_LR": 0.01,
+"MIN_LEARN_STEP": 1, "MAX_LEARN_STEP": 200, "MIN_BATCH_SIZE": 8,
+"MAX_BATCH_SIZE": 1024 } ``` Use ```utils.utils.initialPopulation``` to create
+a list of agents - our population that will evolve and mutate to the optimal
+hyperparameters. ```python from agilerl.utils.utils import initialPopulation
+from pettingzoo.mpe import simple_speaker_listener_v4 import torch device =
+torch.device("cuda" if torch.cuda.is_available() else "cpu") env =
+simple_speaker_listener_v4.parallel_env(continuous_actions=True) env.reset() #
+Configure the multi-agent algo input arguments try: state_dim =
+[env.observation_space(agent).n for agent in env.agents] one_hot = True except
+Exception: state_dim = [env.observation_space(agent).shape for agent in
+env.agents] one_hot = False try: action_dim = [env.action_space(agent).n for
+agent in env.agents] INIT_HP['DISCRETE_ACTIONS'] = True INIT_HP['MAX_ACTION'] =
+None INIT_HP['MIN_ACTION'] = None except Exception: action_dim =
+[env.action_space(agent).shape[0] for agent in env.agents] INIT_HP
+['DISCRETE_ACTIONS'] = False INIT_HP['MAX_ACTION'] = [env.action_space
+(agent).high for agent in env.agents] INIT_HP['MIN_ACTION'] = [env.action_space
+(agent).low for agent in env.agents] if INIT_HP['CHANNELS_LAST']: state_dim = [
+(state_dim[2], state_dim[0], state_dim[1]) for state_dim in state_dim] INIT_HP
+['N_AGENTS'] = env.num_agents INIT_HP['AGENT_IDS'] = [agent_id for agent_id in
+env.agents] agent_pop = initialPopulation(algo=INIT_HP['ALGO'],
+state_dim=state_dim, action_dim=action_dim, one_hot=one_hot,
+net_config=NET_CONFIG, INIT_HP=INIT_HP, population_size=6, device=device) ```
+Next, create the tournament, mutations and experience replay buffer objects
+that allow agents to share memory and efficiently perform evolutionary HPO.
+```python from agilerl.components.multi_agent_replay_buffer import
+MultiAgentReplayBuffer from agilerl.hpo.tournament import TournamentSelection
+from agilerl.hpo.mutation import Mutations field_names = ["state", "action",
+"reward", "next_state", "done"] memory = MultiAgentReplayBuffer
+(memory_size=1_000_000, # Max replay buffer size field_names=field_names, #
+Field names to store in memory agent_ids=INIT_HP['AGENT_IDS'],
+device=torch.device("cuda")) tournament = TournamentSelection
+(tournament_size=2, # Tournament selection size elitism=True, # Elitism in
+tournament selection population_size=6, # Population size evo_step=1) #
+Evaluate using last N fitness scores mutations = Mutations(algo=INIT_HP
+['ALGO'], no_mutation=MUTATION_PARAMS['NO_MUT'], architecture=MUTATION_PARAMS
+['ARCH_MUT'], new_layer_prob=MUTATION_PARAMS['NEW_LAYER'],
+parameters=MUTATION_PARAMS['PARAMS_MUT'], activation=MUTATION_PARAMS
+['ACT_MUT'], rl_hp=MUTATION_PARAMS['RL_HP_MUT'],
+rl_hp_selection=MUTATION_PARAMS['RL_HP_SELECTION'], mutation_sd=MUTATION_PARAMS
+['MUT_SD'], min_lr=MUTATION_PARAMS['MIN_LR'], max_lr=MUTATION_PARAMS['MAX_LR'],
+min_learn_step=MUTATION_PARAMS['MIN_LEARN_STEP'],
+max_learn_step=MUTATION_PARAMS['MAX_LEARN_STEP'],
+min_batch_size=MUTATION_PARAMS['MIN_BATCH_SIZE'],
+max_batch_size=MUTATION_PARAMS['MAX_BATCH_SIZE'], agent_ids=INIT_HP
+['AGENT_IDS'], arch=NET_CONFIG['arch'], rand_seed=MUTATION_PARAMS['RAND_SEED'],
+device=device) ``` The easiest training loop implementation is to use our
+```training.train_multi_agent.train_multi_agent()``` function. It requires the
+agent have functions ```getAction()``` and ```learn()```. ```python from
+agilerl.training.train_multi_agent import train_multi_agent import torch
+trained_pop, pop_fitnesses = train_multi_agent(env=env, # Pettingzoo-style
+environment env_name='simple_speaker_listener_v4', # Environment name
+algo=INIT_HP['ALGO'], # Algorithm pop=agent_pop, # Population of agents
+memory=memory, # Replay buffer INIT_HP=INIT_HP, # IINIT_HP dictionary
+MUT_P=MUTATION_PARAMS, # MUTATION_PARAMS dictionary net_config=NET_CONFIG, #
+Network configuration swap_channels=INIT_HP['CHANNELS_LAST'], # Swap image
+channel from last to first n_episodes=INIT_HP['EPISODES'], # Max number of
+training episodes evo_epochs=20, # Evolution frequency evo_loop=1, # Number of
+evaluation episodes per agent max_steps=900, # Max steps to take in the
+environment target=200., # Target score for early stopping
+tournament=tournament, # Tournament selection object mutation=mutations, #
+Mutations object wb=INIT_HP["WANDB"]) # Weights and Biases tracking ``` View
+_d_o_c_u_m_e_n_t_a_t_i_o_n.
```

