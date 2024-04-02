# Comparing `tmp/jaxmarl-0.0.2.tar.gz` & `tmp/jaxmarl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxmarl-0.0.2.tar", last modified: Thu Nov 16 15:13:49 2023, max compression
+gzip compressed data, was "jaxmarl-0.0.3.tar", last modified: Tue Apr  2 14:10:58 2024, max compression
```

## Comparing `jaxmarl-0.0.2.tar` & `jaxmarl-0.0.3.tar`

### file list

```diff
@@ -1,116 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:49.782433 jaxmarl-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    10232 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9403 2023-11-16 15:13:49.782433 jaxmarl-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7865 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:49.766432 jaxmarl-0.0.2/baselines/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:49.770432 jaxmarl-0.0.2/baselines/IPPO/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/IPPO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13851 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/IPPO/ippo_ff_hanabi.py
--rw-r--r--   0 runner    (1001) docker     (127)    13182 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/IPPO/ippo_mabrax.py
--rw-r--r--   0 runner    (1001) docker     (127)    14304 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/IPPO/ippo_mlp_hanabi.py
--rw-r--r--   0 runner    (1001) docker     (127)    14249 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/IPPO/ippo_mpe.py
--rw-r--r--   0 runner    (1001) docker     (127)    12191 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/IPPO/ippo_mpe_facmac.py
--rw-r--r--   0 runner    (1001) docker     (127)    14122 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/IPPO/ippo_overcooked.py
--rw-r--r--   0 runner    (1001) docker     (127)    15101 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/IPPO/ippo_rnn_hanabi.py
--rw-r--r--   0 runner    (1001) docker     (127)    18367 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/IPPO/ippo_rnn_mpe.py
--rw-r--r--   0 runner    (1001) docker     (127)    17057 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/IPPO/ippo_rnn_smax.py
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/IPPO/ippo_switch_riddle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:49.770432 jaxmarl-0.0.2/baselines/QLearning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/QLearning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:49.770432 jaxmarl-0.0.2/baselines/QLearning/buffers/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/QLearning/buffers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/QLearning/buffers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/QLearning/buffers/circular_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/QLearning/buffers/clustered.py
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/QLearning/buffers/uniform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/QLearning/buffers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24950 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/QLearning/iql.py
--rw-r--r--   0 runner    (1001) docker     (127)    25826 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/QLearning/qmix.py
--rw-r--r--   0 runner    (1001) docker     (127)    27672 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/QLearning/qmix_pretrained.py
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/QLearning/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22972 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/baselines/QLearning/vdn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:49.770432 jaxmarl-0.0.2/jaxmarl/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:49.774432 jaxmarl-0.0.2/jaxmarl/environments/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:49.774432 jaxmarl-0.0.2/jaxmarl/environments/coin_game/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/coin_game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18857 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/coin_game/coin_game.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:49.774432 jaxmarl-0.0.2/jaxmarl/environments/hanabi/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/hanabi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24696 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/hanabi/hanabi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:49.774432 jaxmarl-0.0.2/jaxmarl/environments/mabrax/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/mabrax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8326 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/mabrax/mabrax_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/mabrax/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:49.774432 jaxmarl-0.0.2/jaxmarl/environments/mpe/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/mpe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/mpe/default_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/mpe/mpe_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19230 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/mpe/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/mpe/simple_adversary.py
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/mpe/simple_crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)    14108 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/mpe/simple_facmac.py
--rw-r--r--   0 runner    (1001) docker     (127)     6407 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/mpe/simple_push.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/mpe/simple_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/mpe/simple_speaker_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/mpe/simple_spread.py
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/mpe/simple_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    15841 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/mpe/simple_world_comm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/multi_agent_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:49.774432 jaxmarl-0.0.2/jaxmarl/environments/overcooked/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/overcooked/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/overcooked/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/overcooked/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/overcooked/layouts.py
--rw-r--r--   0 runner    (1001) docker     (127)    28695 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/overcooked/overcooked.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:49.778432 jaxmarl-0.0.2/jaxmarl/environments/smax/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/smax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6405 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/smax/distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6398 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/smax/heuristic_enemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/smax/heuristic_enemy_smax_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    34305 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/smax/smax_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     7153 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/smax/speed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/spaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:49.778432 jaxmarl-0.0.2/jaxmarl/environments/storm/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/storm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/storm/rendering.py
--rw-r--r--   0 runner    (1001) docker     (127)    44333 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/storm/storm_2p.py
--rw-r--r--   0 runner    (1001) docker     (127)    53422 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/storm/storm_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:49.778432 jaxmarl-0.0.2/jaxmarl/environments/switch_riddle/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/switch_riddle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6599 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/environments/switch_riddle/switch_riddle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:49.778432 jaxmarl-0.0.2/jaxmarl/gridworld/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/gridworld/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7523 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/gridworld/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/gridworld/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/gridworld/grid_viz.py
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/gridworld/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)    14329 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/gridworld/ma_maze.py
--rw-r--r--   0 runner    (1001) docker     (127)     9436 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/gridworld/maze.py
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/gridworld/tabular_q.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/registration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:49.778432 jaxmarl-0.0.2/jaxmarl/viz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/viz/grid_rendering.py
--rw-r--r--   0 runner    (1001) docker     (127)    11691 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/viz/overcooked_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/viz/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/viz/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:49.782433 jaxmarl-0.0.2/jaxmarl/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/wrappers/baselines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/jaxmarl/wrappers/gymnax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:49.770432 jaxmarl-0.0.2/jaxmarl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9403 2023-11-16 15:13:49.000000 jaxmarl-0.0.2/jaxmarl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2023-11-16 15:13:49.000000 jaxmarl-0.0.2/jaxmarl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 15:13:49.000000 jaxmarl-0.0.2/jaxmarl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 15:13:49.000000 jaxmarl-0.0.2/jaxmarl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      294 2023-11-16 15:13:49.000000 jaxmarl-0.0.2/jaxmarl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-16 15:13:49.000000 jaxmarl-0.0.2/jaxmarl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 15:13:49.782433 jaxmarl-0.0.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 15:13:49.782433 jaxmarl-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2023-11-16 15:13:35.000000 jaxmarl-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:58.600694 jaxmarl-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    24477 2024-04-02 14:10:58.600694 jaxmarl-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11116 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:58.588694 jaxmarl-0.0.3/jaxmarl/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:58.588694 jaxmarl-0.0.3/jaxmarl/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:58.588694 jaxmarl-0.0.3/jaxmarl/environments/coin_game/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/coin_game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18857 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/coin_game/coin_game.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:58.588694 jaxmarl-0.0.3/jaxmarl/environments/hanabi/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/hanabi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31503 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/hanabi/hanabi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17544 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/hanabi/hanabi_game.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/hanabi/manual_game.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:58.588694 jaxmarl-0.0.3/jaxmarl/environments/hanabi/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/hanabi/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/hanabi/pretrained/obl_r2d2_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/hanabi/pretrained/obl_r2d2_agent_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:58.588694 jaxmarl-0.0.3/jaxmarl/environments/mabrax/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/mabrax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8326 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/mabrax/mabrax_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/mabrax/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:58.592694 jaxmarl-0.0.3/jaxmarl/environments/mpe/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/mpe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/mpe/default_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/mpe/mpe_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19229 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/mpe/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/mpe/simple_adversary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/mpe/simple_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14108 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/mpe/simple_facmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/mpe/simple_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/mpe/simple_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/mpe/simple_speaker_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/mpe/simple_spread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/mpe/simple_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15841 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/mpe/simple_world_comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/multi_agent_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:58.592694 jaxmarl-0.0.3/jaxmarl/environments/overcooked/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/overcooked/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/overcooked/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/overcooked/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/overcooked/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28695 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/overcooked/overcooked.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:58.592694 jaxmarl-0.0.3/jaxmarl/environments/smax/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/smax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/smax/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/smax/heuristic_enemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/smax/heuristic_enemy_smax_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44558 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/smax/smax_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7153 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/smax/speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/spaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:58.596694 jaxmarl-0.0.3/jaxmarl/environments/storm/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/storm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/storm/rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44379 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/storm/storm_2p.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53520 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/storm/storm_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:58.596694 jaxmarl-0.0.3/jaxmarl/environments/switch_riddle/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/switch_riddle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/environments/switch_riddle/switch_riddle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:58.596694 jaxmarl-0.0.3/jaxmarl/gridworld/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/gridworld/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/gridworld/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/gridworld/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/gridworld/grid_viz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/gridworld/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14329 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/gridworld/ma_maze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/gridworld/maze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/gridworld/tabular_q.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/registration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:58.596694 jaxmarl-0.0.3/jaxmarl/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/tutorials/mpe_introduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/tutorials/overcooked_introduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/tutorials/smax_introduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/tutorials/storm_2p_introduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/tutorials/storm_introduction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:58.596694 jaxmarl-0.0.3/jaxmarl/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/viz/grid_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11691 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/viz/overcooked_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/viz/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/viz/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:58.600694 jaxmarl-0.0.3/jaxmarl/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13792 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/wrappers/baselines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/wrappers/gymnax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/jaxmarl/wrappers/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:58.600694 jaxmarl-0.0.3/jaxmarl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24477 2024-04-02 14:10:58.000000 jaxmarl-0.0.3/jaxmarl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-02 14:10:58.000000 jaxmarl-0.0.3/jaxmarl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:10:58.000000 jaxmarl-0.0.3/jaxmarl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-02 14:10:58.000000 jaxmarl-0.0.3/jaxmarl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 14:10:58.000000 jaxmarl-0.0.3/jaxmarl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:58.600694 jaxmarl-0.0.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-02 14:10:51.000000 jaxmarl-0.0.3/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 14:10:58.600694 jaxmarl-0.0.3/setup.cfg
```

### Comparing `jaxmarl-0.0.2/LICENSE` & `jaxmarl-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/PKG-INFO` & `jaxmarl-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,130 +1,111 @@
-Metadata-Version: 2.1
-Name: jaxmarl
-Version: 0.0.2
-Summary: Multi-Agent Reinforcement Learning with JAX
-Home-page: https://github.com/FLAIROx/JaxMARL
-Download-URL: https://github.com/FLAIROx/JaxMARL/archive/v0.0.2.tar.gz
-Author: Foerster Lab for AI Research
-Author-email: arutherford@robots.ox.ac.uk
-Keywords: MARL reinforcement-learning python jax
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: jax>=0.4.11
-Requires-Dist: flax>=0.7.2
-Requires-Dist: chex>=0.1.7
-Requires-Dist: dotmap>=1.3.30
-Requires-Dist: evosax>=0.1.4
-Requires-Dist: matplotlib>=3.3.4
-Requires-Dist: numpy>=1.22.4
-Requires-Dist: distrax>=0.1.3
-Requires-Dist: pillow>=9.5.0
-Requires-Dist: brax>=0.9
-Requires-Dist: gymnax>=0.0.6
-Requires-Dist: typing-extensions>=4.7.1
-Requires-Dist: wandb
-Requires-Dist: hydra-core>=1.3.2
-Requires-Dist: omegaconf>=2.3.0
-Requires-Dist: safetensors>=0.3.3
-Requires-Dist: optax>=0.1.4
-Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pettingzoo>=1.23.1; extra == "dev"
-Requires-Dist: tqdm>=4.65.0; extra == "dev"
-
 <h1 align="center">JaxMARL</h1>
 
 <p align="center">
        <a href="https://pypi.python.org/pypi/jaxmarl">
         <img src="https://img.shields.io/pypi/pyversions/jaxmarl.svg" /></a>
-       <a href= "https://badge.fury.io/py/jaxmarl">
+       <a href="https://badge.fury.io/py/jaxmarl">
         <img src="https://badge.fury.io/py/jaxmarl.svg" /></a>
        <a href= "https://github.com/FLAIROx/JaxMARL/blob/main/LICENSE">
         <img src="https://img.shields.io/badge/license-Apache2.0-blue.svg" /></a>
+       <a href= "https://colab.research.google.com/github/FLAIROx/JaxMARL/blob/main/jaxmarl/tutorials/JaxMARL_Walkthrough.ipynb">
+        <img src="https://colab.research.google.com/assets/colab-badge.svg" /></a>
+       <a href= "https://arxiv.org/abs/2311.10090">
+        <img src="https://img.shields.io/badge/arXiv-2311.10090-b31b1b.svg" /></a>
+       
 </p>
 
 [**Installation**](#install) | [**Quick Start**](#start) | [**Environments**](#environments) | [**Algorithms**](#algorithms) | [**Citation**](#cite)
 ---
 
 <div class="collage">
-    <div class="row" align="centre">
-        <img src="https://github.com/FLAIROx/JaxMARL/blob/main/docs/imgs/cramped_room.gif?raw=true" alt="Overcooked" width="20%">
-        <img src="https://github.com/FLAIROx/JaxMARL/blob/main/docs/imgs/qmix_MPE_simple_tag_v3.gif?raw=true" alt="MPE" width="20%">
-        <img src="https://github.com/FLAIROx/JaxMARL/blob/main/docs/imgs/storm.gif?raw=true" alt="STORM" width="20%">
-        <img src="https://github.com/FLAIROx/JaxMARL/blob/main/docs/imgs/smax.gif?raw=true" alt="SMAX" width="20%">
+    <div class="column" align="centre">
+        <div class="row" align="centre">
+            <img src="https://github.com/FLAIROx/JaxMARL/blob/main/docs/imgs/cramped_room.gif?raw=true" alt="Overcooked" width="20%">
+            <img src="https://github.com/FLAIROx/JaxMARL/blob/main/docs/imgs/mabrax.png?raw=true" alt="mabrax" width="20%">
+            <img src="https://github.com/FLAIROx/JaxMARL/blob/main/docs/imgs/storm.gif?raw=true" alt="STORM" width="20%">
+            <img src="https://github.com/FLAIROx/JaxMARL/blob/main/docs/imgs/hanabi.png?raw=true" alt="hanabi" width="20%">
+        </div>
+        <div class="row" align="centre">
+            <img src="https://github.com/FLAIROx/JaxMARL/blob/main/docs/imgs/coin_game.png?raw=true" alt="coin_game" width="20%">
+            <img src="https://github.com/FLAIROx/JaxMARL/blob/main/docs/imgs/qmix_MPE_simple_tag_v3.gif?raw=true" alt="MPE" width="20%">
+            <img src="https://github.com/FLAIROx/JaxMARL/blob/main/docs/imgs/switch_riddle.png?raw=true" alt="switch_riddle" width="20%">
+            <img src="https://github.com/FLAIROx/JaxMARL/blob/main/docs/imgs/smax.gif?raw=true" alt="SMAX" width="20%">
+        </div>
     </div>
 </div>
 
 ## Multi-Agent Reinforcement Learning in JAX
 
-JaxMARL combines ease-of-use with GPU enabled efficiency, and supports a wide range of commonly used MARL environments as well as popular baseline algorithms. Our aim is for one library that enables thorough evaluation of MARL methods across a wide range of tasks and against relevant baselines. We also introduce SMAX, a vectorised, simplifed version of the popular StarCraft Multi-Agent Challenge, which removes the need to run the StarCraft II game engine. 
+JaxMARL combines ease-of-use with GPU-enabled efficiency, and supports a wide range of commonly used MARL environments as well as popular baseline algorithms. Our aim is for one library that enables thorough evaluation of MARL methods across a wide range of tasks and against relevant baselines. We also introduce SMAX, a vectorised, simplified version of the popular StarCraft Multi-Agent Challenge, which removes the need to run the StarCraft II game engine. 
 
-For more details, take a look at our blog post or this notebook walks through the basic usage. LINKS TODO
+For more details, take a look at our [blog post](https://blog.foersterlab.com/jaxmarl/) or our [Colab notebook](https://colab.research.google.com/github/FLAIROx/JaxMARL/blob/main/jaxmarl/tutorials/JaxMARL_Walkthrough.ipynb), which walks through the basic usage.
 
 <h2 name="environments" id="environments">Environments 🌍 </h2>
 
 | Environment | Reference | README | Summary |
 | --- | --- | --- | --- |
 | 🔴 MPE | [Paper](https://arxiv.org/abs/1706.02275) | [Source](https://github.com/FLAIROx/JaxMARL/tree/main/jaxmarl/environments/mpe) | Communication orientated tasks in a multi-agent particle world
 | 🍲 Overcooked | [Paper](https://arxiv.org/abs/1910.05789) | [Source](https://github.com/FLAIROx/JaxMARL/tree/main/jaxmarl/environments/overcooked) | Fully-cooperative human-AI coordination tasks based on the homonyms video game | 
-| 🦾 Multi-Agent Brax | [Paper](https://arxiv.org/abs/2003.06709) | [Source](https://github.com/FLAIROx/JaxMARL/tree/main/jaxmarl/environments/mabrax) | Continuous multi-agent robotic control based on Brax, analagous to Multi-Agent MuJoCo |
+| 🦾 Multi-Agent Brax | [Paper](https://arxiv.org/abs/2003.06709) | [Source](https://github.com/FLAIROx/JaxMARL/tree/main/jaxmarl/environments/mabrax) | Continuous multi-agent robotic control based on Brax, analogous to Multi-Agent MuJoCo |
 | 🎆 Hanabi | [Paper](https://arxiv.org/abs/1902.00506) | [Source](https://github.com/FLAIROx/JaxMARL/tree/main/jaxmarl/environments/hanabi) | Fully-cooperative partially-observable multiplayer card game |
-| 👾 SMAX | Novel | [Source](https://github.com/FLAIROx/JaxMARL/tree/main/jaxmarl/environments/smax) | Simplifed cooperative StarCraft micro-management environment |
+| 👾 SMAX | Novel | [Source](https://github.com/FLAIROx/JaxMARL/tree/main/jaxmarl/environments/smax) | Simplified cooperative StarCraft micro-management environment |
 | 🧮 STORM: Spatial-Temporal Representations of Matrix Games | [Paper](https://openreview.net/forum?id=54F8woU8vhq) | [Source](https://github.com/FLAIROx/JaxMARL/tree/main/jaxmarl/environments/storm) | Matrix games represented as grid world scenarios
 | 🪙 Coin Game | [Paper](https://arxiv.org/abs/1802.09640) | [Source](https://github.com/FLAIROx/JaxMARL/tree/main/jaxmarl/environments/coin_game) | Two-player grid world environment which emulates social dilemmas
 | 💡 Switch Riddle | [Paper](https://proceedings.neurips.cc/paper_files/paper/2016/hash/c7635bfd99248a2cdef8249ef7bfbef4-Abstract.html) | [Source](https://github.com/FLAIROx/JaxMARL/tree/main/jaxmarl/environments/switch_riddle) | Simple cooperative communication game included for debugging
 
  
 <h2 name="algorithms" id="algorithms">Baseline Algorithms 🦉 </h2>
 
-We follow CleanRL's philosophy of providing single file implementations which can be found within the `baselines` directory.
+We follow CleanRL's philosophy of providing single file implementations which can be found within the `baselines` directory. We use Hydra to manage our config files, with specifics explained in each algorithm's README. Most files include `wandb` logging code, this is disabled by default but can be enabled within the file's config.
 
 | Algorithm | Reference | README | 
 | --- | --- | --- | 
 | IPPO | [Paper](https://arxiv.org/pdf/2011.09533.pdf) | [Source](https://github.com/FLAIROx/JaxMARL/tree/main/baselines/IPPO) | 
 | MAPPO | [Paper](https://arxiv.org/abs/2103.01955) | [Source](https://github.com/FLAIROx/JaxMARL/tree/main/baselines/MAPPO) | 
-| IQL | [Paper](https://arxiv.org/abs/1312.5602v1) | [Source](https://github.com/FLAIROx/JaxMARL/tree/main/baselines/QLearning) | DQN 
+| IQL | [Paper](https://arxiv.org/abs/1312.5602v1) | [Source](https://github.com/FLAIROx/JaxMARL/tree/main/baselines/QLearning) | 
 | VDN | [Paper](https://arxiv.org/abs/1706.05296)  | [Source](https://github.com/FLAIROx/JaxMARL/tree/main/baselines/QLearning) |
 | QMIX | [Paper](https://arxiv.org/abs/1803.11485) | [Source](https://github.com/FLAIROx/JaxMARL/tree/main/baselines/QLearning) |
+| TransfQMIX | [Peper](https://www.southampton.ac.uk/~eg/AAMAS2023/pdfs/p1679.pdf) | [Source](https://github.com/FLAIROx/JaxMARL/tree/main/baselines/QLearning) |
+| SHAQ | [Paper](https://arxiv.org/abs/2105.15013) | [Source](https://github.com/FLAIROx/JaxMARL/tree/main/baselines/QLearning) |
 
 <h2 name="install" id="install">Installation 🧗 </h2>
 
-Before installing, ensure you have the correct [JAX version](https://github.com/google/jax#installation) for your hardware accelerator. JaxMARL can then be installed directly from PyPi:
+**Environments** - Before installing, ensure you have the correct [JAX version](https://github.com/google/jax#installation) for your hardware accelerator. The JaxMARL environments can be installed directly from PyPi:
 
 ```
 pip install jaxmarl 
 ```
-We have tested JaxMARL on Python 3.8 and 3.9. To run our test scripts, some additional dependencies are required (for comparisons against existing implementations), these can be installed with:
-```
-pip install jaxmarl[dev]
-```
+
+**Algorithms** - If you would like to also run the algorithms, install the source code as follows:
+
+1. Clone the repository:
+    ```
+    git clone https://github.com/FLAIROx/JaxMARL.git && cd JaxMARL
+    ```
+2. The requirements for IPPO & MAPPO can be installed with:
+    ``` 
+    pip install -e .
+    export PYTHONPATH=./JaxMARL:$PYTHONPATH
+    ```
 
 <h2 name="start" id="start">Quick Start 🚀 </h2>
 
-We take inspiration from the [PettingZoo](https://github.com/Farama-Foundation/PettingZoo) and [Gymnax](https://github.com/RobertTLange/gymnax) interfaces. You can try out training an agent on XX in this Colab TODO. Further introduction scripts can be found [here](https://github.com/FLAIROx/JaxMARL/tree/main/jaxmarl/tutorials).
+We take inspiration from the [PettingZoo](https://github.com/Farama-Foundation/PettingZoo) and [Gymnax](https://github.com/RobertTLange/gymnax) interfaces. You can try out training an agent in our [Colab notebook](https://colab.research.google.com/github/FLAIROx/JaxMARL/blob/main/jaxmarl/tutorials/JaxMARL_Walkthrough.ipynb). Further introduction scripts can be found [here](https://github.com/FLAIROx/JaxMARL/tree/main/jaxmarl/tutorials).
 
 ### Basic JaxMARL API  Usage 🖥️
 
-Actions, observations, rewards and done values are passed as dictionaries keyed by agent name, allowing for differing action and observation spaces. The done dictionary contains an additional `"__all__"` key, specifying whether the episode has ended. We follow a parallel structure, with each agent passing an action at each timestep. For ascyhronous games, such as Hanabi, a dummy action is passed for agents not acting at a given timestep.
+Actions, observations, rewards and done values are passed as dictionaries keyed by agent name, allowing for differing action and observation spaces. The done dictionary contains an additional `"__all__"` key, specifying whether the episode has ended. We follow a parallel structure, with each agent passing an action at each timestep. For asynchronous games, such as Hanabi, a dummy action is passed for agents not acting at a given timestep.
 
 ```python 
 import jax
 from jaxmarl import make
 
 key = jax.random.PRNGKey(0)
-key, key_reset, key_act, key_step = jax.random.split(rng, 4)
+key, key_reset, key_act, key_step = jax.random.split(key, 4)
 
 # Initialise environment.
 env = make('MPE_simple_world_comm_v3')
 
 # Reset the environment.
 obs, state = env.reset(key_reset)
 
@@ -132,29 +113,46 @@
 key_act = jax.random.split(key_act, env.num_agents)
 actions = {agent: env.action_space(agent).sample(key_act[i]) for i, agent in enumerate(env.agents)}
 
 # Perform the step transition.
 obs, state, reward, done, infos = env.step(key_step, state, actions)
 ```
 
+### Dockerfile 🐋
+To help get experiments up and running we include a [Dockerfile](https://github.com/FLAIROx/JaxMARL/blob/main/Dockerfile) and its corresponding [Makefile](https://github.com/FLAIROx/JaxMARL/blob/main/Makefile). With Docker and the [Nvidia Container Toolkit](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/latest/index.html) installed, the container can be built with:
+```
+make build
+```
+The built container can then be run:
+```
+make run
+```
+
 ## Contributing 🔨
-Please contribute! Please take a look at our [contributing guide](https://github.com/FLAIROx/JaxMARL/blob/main/CONTRIBUTING.md) for how to add an environment/algorithm or submit a bug report.
+Please contribute! Please take a look at our [contributing guide](https://github.com/FLAIROx/JaxMARL/blob/main/CONTRIBUTING.md) for how to add an environment/algorithm or submit a bug report. Our roadmap also lives there.
 
 <h2 name="cite" id="cite">Citing JaxMARL 📜 </h2>
 If you use JaxMARL in your work, please cite us as follows:
 
 ```
-TODO
+@article{flair2023jaxmarl,
+      title={JaxMARL: Multi-Agent RL Environments in JAX},
+      author={Alexander Rutherford and Benjamin Ellis and Matteo Gallici and Jonathan Cook and Andrei Lupu and Gardar Ingvarsson and Timon Willi and Akbir Khan and Christian Schroeder de Witt and Alexandra Souly and Saptarashmi Bandyopadhyay and Mikayel Samvelyan and Minqi Jiang and Robert Tjarko Lange and Shimon Whiteson and Bruno Lacerda and Nick Hawes and Tim Rocktaschel and Chris Lu and Jakob Nicolaus Foerster},
+      journal={arXiv preprint arXiv:2311.10090},
+      year={2023}
+    }
 ```
 
 ## See Also 🙌
 There are a number of other libraries which inspired this work, we encourage you to take a look!
 
 JAX-native algorithms:
 - [Mava](https://github.com/instadeepai/Mava): JAX implementations of IPPO and MAPPO, two popular MARL algorithms.
 - [PureJaxRL](https://github.com/luchris429/purejaxrl): JAX implementation of PPO, and demonstration of end-to-end JAX-based RL training.
+- [Minimax](https://github.com/facebookresearch/minimax/): JAX implementations of autocurricula baselines for RL.
 
-JAX-native envrionments:
+JAX-native environments:
 - [Gymnax](https://github.com/RobertTLange/gymnax): Implementations of classic RL tasks including classic control, bsuite and MinAtar.
-- [Jumanji](https://github.com/instadeepai/jumanji): A diverse set of environments ranging from simple games to NP-hard combinatoral problems.
+- [Jumanji](https://github.com/instadeepai/jumanji): A diverse set of environments ranging from simple games to NP-hard combinatorial problems.
 - [Pgx](https://github.com/sotetsuk/pgx): JAX implementations of classic board games, such as Chess, Go and Shogi.
 - [Brax](https://github.com/google/brax): A fully differentiable physics engine written in JAX, features continuous control tasks.
+- [XLand-MiniGrid](https://github.com/corl-team/xland-minigrid): Meta-RL gridworld environments inspired by XLand and MiniGrid.
```

#### html2text {}

```diff
@@ -1,117 +1,129 @@
-Metadata-Version: 2.1 Name: jaxmarl Version: 0.0.2 Summary: Multi-Agent
-Reinforcement Learning with JAX Home-page: https://github.com/FLAIROx/JaxMARL
-Download-URL: https://github.com/FLAIROx/JaxMARL/archive/v0.0.2.tar.gz Author:
-Foerster Lab for AI Research Author-email: arutherford@robots.ox.ac.uk
-Keywords: MARL reinforcement-learning python jax Classifier: Intended Audience
-:: Science/Research Classifier: Intended Audience :: Developers Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: License :: OSI Approved
-:: Apache Software License Requires-Python: >=3.8 Description-Content-Type:
-text/markdown License-File: LICENSE Requires-Dist: jax>=0.4.11 Requires-Dist:
-flax>=0.7.2 Requires-Dist: chex>=0.1.7 Requires-Dist: dotmap>=1.3.30 Requires-
-Dist: evosax>=0.1.4 Requires-Dist: matplotlib>=3.3.4 Requires-Dist:
-numpy>=1.22.4 Requires-Dist: distrax>=0.1.3 Requires-Dist: pillow>=9.5.0
-Requires-Dist: brax>=0.9 Requires-Dist: gymnax>=0.0.6 Requires-Dist: typing-
-extensions>=4.7.1 Requires-Dist: wandb Requires-Dist: hydra-core>=1.3.2
-Requires-Dist: omegaconf>=2.3.0 Requires-Dist: safetensors>=0.3.3 Requires-
-Dist: optax>=0.1.4 Provides-Extra: dev Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pettingzoo>=1.23.1; extra == "dev" Requires-Dist: tqdm>=4.65.0;
-extra == "dev"
                              ************ JJaaxxMMAARRLL ************
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_j_a_x_m_a_r_l_._s_v_g_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/
-     _j_a_x_m_a_r_l_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_l_i_c_e_n_s_e_-_A_p_a_c_h_e_2_._0_-_b_l_u_e_._s_v_g_]
+_j_a_x_m_a_r_l_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_l_i_c_e_n_s_e_-_A_p_a_c_h_e_2_._0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
+_c_o_l_a_b_._r_e_s_e_a_r_c_h_._g_o_o_g_l_e_._c_o_m_/_a_s_s_e_t_s_/_c_o_l_a_b_-_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
+                         _a_r_X_i_v_-_2_3_1_1_._1_0_0_9_0_-_b_3_1_b_1_b_._s_v_g_]
 [**Installation**](#install) | [**Quick Start**](#start) | [**Environments**]
 (#environments) | [**Algorithms**](#algorithms) | [**Citation**](#cite) ---
-[Overcooked][MPE][STORM][SMAX]
+[Overcooked][mabrax][STORM][hanabi]
+[coin_game][MPE][switch_riddle][SMAX]
 ## Multi-Agent Reinforcement Learning in JAX JaxMARL combines ease-of-use with
-GPU enabled efficiency, and supports a wide range of commonly used MARL
+GPU-enabled efficiency, and supports a wide range of commonly used MARL
 environments as well as popular baseline algorithms. Our aim is for one library
 that enables thorough evaluation of MARL methods across a wide range of tasks
-and against relevant baselines. We also introduce SMAX, a vectorised, simplifed
-version of the popular StarCraft Multi-Agent Challenge, which removes the need
-to run the StarCraft II game engine. For more details, take a look at our blog
-post or this notebook walks through the basic usage. LINKS TODO
+and against relevant baselines. We also introduce SMAX, a vectorised,
+simplified version of the popular StarCraft Multi-Agent Challenge, which
+removes the need to run the StarCraft II game engine. For more details, take a
+look at our [blog post](https://blog.foersterlab.com/jaxmarl/) or our [Colab
+notebook](https://colab.research.google.com/github/FLAIROx/JaxMARL/blob/main/
+jaxmarl/tutorials/JaxMARL_Walkthrough.ipynb), which walks through the basic
+usage.
 ********** EEnnvviirroonnmmeennttss ?ð??? **********
 | Environment | Reference | README | Summary | | --- | --- | --- | --- | | ð´
 MPE | [Paper](https://arxiv.org/abs/1706.02275) | [Source](https://github.com/
 FLAIROx/JaxMARL/tree/main/jaxmarl/environments/mpe) | Communication orientated
 tasks in a multi-agent particle world | ð² Overcooked | [Paper](https://
 arxiv.org/abs/1910.05789) | [Source](https://github.com/FLAIROx/JaxMARL/tree/
 main/jaxmarl/environments/overcooked) | Fully-cooperative human-AI coordination
 tasks based on the homonyms video game | | ð¦¾ Multi-Agent Brax | [Paper]
 (https://arxiv.org/abs/2003.06709) | [Source](https://github.com/FLAIROx/
 JaxMARL/tree/main/jaxmarl/environments/mabrax) | Continuous multi-agent robotic
-control based on Brax, analagous to Multi-Agent MuJoCo | | ð Hanabi |
+control based on Brax, analogous to Multi-Agent MuJoCo | | ð Hanabi |
 [Paper](https://arxiv.org/abs/1902.00506) | [Source](https://github.com/
 FLAIROx/JaxMARL/tree/main/jaxmarl/environments/hanabi) | Fully-cooperative
 partially-observable multiplayer card game | | ð¾ SMAX | Novel | [Source]
 (https://github.com/FLAIROx/JaxMARL/tree/main/jaxmarl/environments/smax) |
-Simplifed cooperative StarCraft micro-management environment | | ð§® STORM:
+Simplified cooperative StarCraft micro-management environment | | ð§® STORM:
 Spatial-Temporal Representations of Matrix Games | [Paper](https://
 openreview.net/forum?id=54F8woU8vhq) | [Source](https://github.com/FLAIROx/
 JaxMARL/tree/main/jaxmarl/environments/storm) | Matrix games represented as
 grid world scenarios | ðª Coin Game | [Paper](https://arxiv.org/abs/
 1802.09640) | [Source](https://github.com/FLAIROx/JaxMARL/tree/main/jaxmarl/
 environments/coin_game) | Two-player grid world environment which emulates
 social dilemmas | ð¡ Switch Riddle | [Paper](https://proceedings.neurips.cc/
 paper_files/paper/2016/hash/c7635bfd99248a2cdef8249ef7bfbef4-Abstract.html) |
 [Source](https://github.com/FLAIROx/JaxMARL/tree/main/jaxmarl/environments/
 switch_riddle) | Simple cooperative communication game included for debugging
 ********** BBaasseelliinnee AAllggoorriitthhmmss ?ð??¦? **********
 We follow CleanRL's philosophy of providing single file implementations which
-can be found within the `baselines` directory. | Algorithm | Reference | README
-| | --- | --- | --- | | IPPO | [Paper](https://arxiv.org/pdf/2011.09533.pdf) |
-[Source](https://github.com/FLAIROx/JaxMARL/tree/main/baselines/IPPO) | | MAPPO
-| [Paper](https://arxiv.org/abs/2103.01955) | [Source](https://github.com/
-FLAIROx/JaxMARL/tree/main/baselines/MAPPO) | | IQL | [Paper](https://arxiv.org/
-abs/1312.5602v1) | [Source](https://github.com/FLAIROx/JaxMARL/tree/main/
-baselines/QLearning) | DQN | VDN | [Paper](https://arxiv.org/abs/1706.05296) |
+can be found within the `baselines` directory. We use Hydra to manage our
+config files, with specifics explained in each algorithm's README. Most files
+include `wandb` logging code, this is disabled by default but can be enabled
+within the file's config. | Algorithm | Reference | README | | --- | --- | --
+- | | IPPO | [Paper](https://arxiv.org/pdf/2011.09533.pdf) | [Source](https://
+github.com/FLAIROx/JaxMARL/tree/main/baselines/IPPO) | | MAPPO | [Paper](https:
+//arxiv.org/abs/2103.01955) | [Source](https://github.com/FLAIROx/JaxMARL/tree/
+main/baselines/MAPPO) | | IQL | [Paper](https://arxiv.org/abs/1312.5602v1) |
 [Source](https://github.com/FLAIROx/JaxMARL/tree/main/baselines/QLearning) | |
-QMIX | [Paper](https://arxiv.org/abs/1803.11485) | [Source](https://github.com/
-FLAIROx/JaxMARL/tree/main/baselines/QLearning) |
+VDN | [Paper](https://arxiv.org/abs/1706.05296) | [Source](https://github.com/
+FLAIROx/JaxMARL/tree/main/baselines/QLearning) | | QMIX | [Paper](https://
+arxiv.org/abs/1803.11485) | [Source](https://github.com/FLAIROx/JaxMARL/tree/
+main/baselines/QLearning) | | TransfQMIX | [Peper](https://
+www.southampton.ac.uk/~eg/AAMAS2023/pdfs/p1679.pdf) | [Source](https://
+github.com/FLAIROx/JaxMARL/tree/main/baselines/QLearning) | | SHAQ | [Paper]
+(https://arxiv.org/abs/2105.15013) | [Source](https://github.com/FLAIROx/
+JaxMARL/tree/main/baselines/QLearning) |
 ********** IInnssttaallllaattiioonn ?ð??§? **********
-Before installing, ensure you have the correct [JAX version](https://
-github.com/google/jax#installation) for your hardware accelerator. JaxMARL can
-then be installed directly from PyPi: ``` pip install jaxmarl ``` We have
-tested JaxMARL on Python 3.8 and 3.9. To run our test scripts, some additional
-dependencies are required (for comparisons against existing implementations),
-these can be installed with: ``` pip install jaxmarl[dev] ```
+**Environments** - Before installing, ensure you have the correct [JAX version]
+(https://github.com/google/jax#installation) for your hardware accelerator. The
+JaxMARL environments can be installed directly from PyPi: ``` pip install
+jaxmarl ``` **Algorithms** - If you would like to also run the algorithms,
+install the source code as follows: 1. Clone the repository: ``` git clone
+https://github.com/FLAIROx/JaxMARL.git && cd JaxMARL ``` 2. The requirements
+for IPPO & MAPPO can be installed with: ``` pip install -e . export
+PYTHONPATH=./JaxMARL:$PYTHONPATH ```
 ********** QQuuiicckk SSttaarrtt ?ð??? **********
 We take inspiration from the [PettingZoo](https://github.com/Farama-Foundation/
 PettingZoo) and [Gymnax](https://github.com/RobertTLange/gymnax) interfaces.
-You can try out training an agent on XX in this Colab TODO. Further
-introduction scripts can be found [here](https://github.com/FLAIROx/JaxMARL/
-tree/main/jaxmarl/tutorials). ### Basic JaxMARL API Usage ð¥ï¸ Actions,
-observations, rewards and done values are passed as dictionaries keyed by agent
-name, allowing for differing action and observation spaces. The done dictionary
-contains an additional `"__all__"` key, specifying whether the episode has
-ended. We follow a parallel structure, with each agent passing an action at
-each timestep. For ascyhronous games, such as Hanabi, a dummy action is passed
-for agents not acting at a given timestep. ```python import jax from jaxmarl
-import make key = jax.random.PRNGKey(0) key, key_reset, key_act, key_step =
-jax.random.split(rng, 4) # Initialise environment. env = make
-('MPE_simple_world_comm_v3') # Reset the environment. obs, state = env.reset
-(key_reset) # Sample random actions. key_act = jax.random.split(key_act,
-env.num_agents) actions = {agent: env.action_space(agent).sample(key_act[i])
-for i, agent in enumerate(env.agents)} # Perform the step transition. obs,
-state, reward, done, infos = env.step(key_step, state, actions) ``` ##
-Contributing ð¨ Please contribute! Please take a look at our [contributing
-guide](https://github.com/FLAIROx/JaxMARL/blob/main/CONTRIBUTING.md) for how to
-add an environment/algorithm or submit a bug report.
+You can try out training an agent in our [Colab notebook](https://
+colab.research.google.com/github/FLAIROx/JaxMARL/blob/main/jaxmarl/tutorials/
+JaxMARL_Walkthrough.ipynb). Further introduction scripts can be found [here]
+(https://github.com/FLAIROx/JaxMARL/tree/main/jaxmarl/tutorials). ### Basic
+JaxMARL API Usage ð¥ï¸ Actions, observations, rewards and done values are
+passed as dictionaries keyed by agent name, allowing for differing action and
+observation spaces. The done dictionary contains an additional `"__all__"` key,
+specifying whether the episode has ended. We follow a parallel structure, with
+each agent passing an action at each timestep. For asynchronous games, such as
+Hanabi, a dummy action is passed for agents not acting at a given timestep.
+```python import jax from jaxmarl import make key = jax.random.PRNGKey(0) key,
+key_reset, key_act, key_step = jax.random.split(key, 4) # Initialise
+environment. env = make('MPE_simple_world_comm_v3') # Reset the environment.
+obs, state = env.reset(key_reset) # Sample random actions. key_act =
+jax.random.split(key_act, env.num_agents) actions = {agent: env.action_space
+(agent).sample(key_act[i]) for i, agent in enumerate(env.agents)} # Perform the
+step transition. obs, state, reward, done, infos = env.step(key_step, state,
+actions) ``` ### Dockerfile ð To help get experiments up and running we
+include a [Dockerfile](https://github.com/FLAIROx/JaxMARL/blob/main/Dockerfile)
+and its corresponding [Makefile](https://github.com/FLAIROx/JaxMARL/blob/main/
+Makefile). With Docker and the [Nvidia Container Toolkit](https://
+docs.nvidia.com/datacenter/cloud-native/container-toolkit/latest/index.html)
+installed, the container can be built with: ``` make build ``` The built
+container can then be run: ``` make run ``` ## Contributing ð¨ Please
+contribute! Please take a look at our [contributing guide](https://github.com/
+FLAIROx/JaxMARL/blob/main/CONTRIBUTING.md) for how to add an environment/
+algorithm or submit a bug report. Our roadmap also lives there.
 ********** CCiittiinngg JJaaxxMMAARRLL ?ð??? **********
-If you use JaxMARL in your work, please cite us as follows: ``` TODO ``` ## See
-Also ð There are a number of other libraries which inspired this work, we
-encourage you to take a look! JAX-native algorithms: - [Mava](https://
-github.com/instadeepai/Mava): JAX implementations of IPPO and MAPPO, two
-popular MARL algorithms. - [PureJaxRL](https://github.com/luchris429/
-purejaxrl): JAX implementation of PPO, and demonstration of end-to-end JAX-
-based RL training. JAX-native envrionments: - [Gymnax](https://github.com/
-RobertTLange/gymnax): Implementations of classic RL tasks including classic
-control, bsuite and MinAtar. - [Jumanji](https://github.com/instadeepai/
-jumanji): A diverse set of environments ranging from simple games to NP-hard
-combinatoral problems. - [Pgx](https://github.com/sotetsuk/pgx): JAX
-implementations of classic board games, such as Chess, Go and Shogi. - [Brax]
-(https://github.com/google/brax): A fully differentiable physics engine written
-in JAX, features continuous control tasks.
+If you use JaxMARL in your work, please cite us as follows: ``` @article
+{flair2023jaxmarl, title={JaxMARL: Multi-Agent RL Environments in JAX}, author=
+{Alexander Rutherford and Benjamin Ellis and Matteo Gallici and Jonathan Cook
+and Andrei Lupu and Gardar Ingvarsson and Timon Willi and Akbir Khan and
+Christian Schroeder de Witt and Alexandra Souly and Saptarashmi Bandyopadhyay
+and Mikayel Samvelyan and Minqi Jiang and Robert Tjarko Lange and Shimon
+Whiteson and Bruno Lacerda and Nick Hawes and Tim Rocktaschel and Chris Lu and
+Jakob Nicolaus Foerster}, journal={arXiv preprint arXiv:2311.10090}, year=
+{2023} } ``` ## See Also ð There are a number of other libraries which
+inspired this work, we encourage you to take a look! JAX-native algorithms: -
+[Mava](https://github.com/instadeepai/Mava): JAX implementations of IPPO and
+MAPPO, two popular MARL algorithms. - [PureJaxRL](https://github.com/
+luchris429/purejaxrl): JAX implementation of PPO, and demonstration of end-to-
+end JAX-based RL training. - [Minimax](https://github.com/facebookresearch/
+minimax/): JAX implementations of autocurricula baselines for RL. JAX-native
+environments: - [Gymnax](https://github.com/RobertTLange/gymnax):
+Implementations of classic RL tasks including classic control, bsuite and
+MinAtar. - [Jumanji](https://github.com/instadeepai/jumanji): A diverse set of
+environments ranging from simple games to NP-hard combinatorial problems. -
+[Pgx](https://github.com/sotetsuk/pgx): JAX implementations of classic board
+games, such as Chess, Go and Shogi. - [Brax](https://github.com/google/brax): A
+fully differentiable physics engine written in JAX, features continuous control
+tasks. - [XLand-MiniGrid](https://github.com/corl-team/xland-minigrid): Meta-RL
+gridworld environments inspired by XLand and MiniGrid.
```

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/__init__.py` & `jaxmarl-0.0.3/jaxmarl/environments/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,11 +14,11 @@
     SimpleFacmacMPE6a,
     SimpleFacmacMPE9a
 )
 from .smax import SMAX, HeuristicEnemySMAX, LearnedPolicyEnemySMAX
 from .switch_riddle import SwitchRiddle
 from .overcooked import Overcooked, overcooked_layouts
 from .mabrax import Ant, Humanoid, Hopper, Walker2d, HalfCheetah
-from .hanabi import HanabiGame
+from .hanabi import Hanabi
 from .storm import InTheGrid, InTheGrid_2p
 from .coin_game import CoinGame
```

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/coin_game/coin_game.py` & `jaxmarl-0.0.3/jaxmarl/environments/coin_game/coin_game.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/hanabi/hanabi.py` & `jaxmarl-0.0.3/jaxmarl/environments/hanabi/hanabi_game.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+"""
+This class models the game dynamics of Hanabi (reset and step of the game).
+"""
+
 import numpy as np
 import jax
 import jax.numpy as jnp
 from jax import lax
 import chex
 from flax import struct
 from typing import Tuple, Dict
 from functools import partial
-from gymnax.environments.spaces import Discrete
 from jaxmarl.environments.multi_agent_env import MultiAgentEnv
 
 
 @struct.dataclass
 class State:
     deck: chex.Array
     discard_pile: chex.Array
@@ -20,539 +23,408 @@
     terminal: bool
     life_tokens: chex.Array
     card_knowledge: chex.Array
     colors_revealed: chex.Array
     ranks_revealed: chex.Array
     num_cards_dealt: int
     num_cards_discarded: int
-    last_moves: chex.Array
     cur_player_idx: chex.Array
     out_of_lives: bool
     last_round_count: int
     bombed: bool
     remaining_deck_size: chex.Array
+    turn: int
+    score: int
 
 
 class HanabiGame(MultiAgentEnv):
 
-    def __init__(self, num_agents=2, num_colors=5, num_ranks=5, hand_size=5, max_info_tokens=8, max_life_tokens=3,
-                 num_cards_of_rank=np.array([3, 2, 2, 2, 1]), agents=None, action_spaces=None, observation_spaces=None,
-                 obs_size=None, num_moves=None):
+    def __init__(
+        self,
+        num_agents=2,
+        num_colors=5,
+        num_ranks=5,
+        hand_size=5,
+        max_info_tokens=8,
+        max_life_tokens=3,
+        num_cards_of_rank=np.array([3, 2, 2, 2, 1]),
+        color_map=["R", "Y", "G", "W", "B"],
+    ):
         super().__init__(num_agents)
 
         self.num_agents = num_agents
         self.agent_range = jnp.arange(num_agents)
         self.num_colors = num_colors
         self.num_ranks = num_ranks
         self.hand_size = hand_size
         self.max_info_tokens = max_info_tokens
         self.max_life_tokens = max_life_tokens
         self.num_cards_of_rank = num_cards_of_rank
         self.deck_size = jnp.sum(num_cards_of_rank) * num_colors
+        self.color_map = color_map
 
-        if agents is None:
-            self.agents = [f"agent_{i}" for i in range(num_agents)]
-        else:
-            assert len(
-                agents) == num_agents, f"Number of agents {len(agents)} does not match number of agents {num_agents}"
-            self.agents = agents
-
-        if num_moves is None:
-            self.num_moves = np.sum(np.array([
-                # noop
-                1,
-                # discard, play
-                hand_size * 2,
-                # hint color, rank
-                (num_agents - 1) * (num_colors + num_ranks)
-            ])).squeeze()
-
-        if obs_size is None:
-            self.obs_size = (
-                    # card knowledge
-                    (hand_size * (num_colors * num_ranks)) +
-                    # color and rank hints
-                    (hand_size * (num_colors + num_ranks)) +
-                    # other hands
-                    ((num_agents - 1) * hand_size * num_colors * num_ranks) +
-                    # available actions
-                    # self.num_moves +
-                    # fireworks
-                    (num_colors * num_ranks) +
-                    # info tokens
-                    max_info_tokens +
-                    # life tokens
-                    max_life_tokens +
-                    # last moves
-                    (num_agents * self.num_moves) +
-                    # current player
-                    num_agents +
-                    # discard pile
-                    np.sum(num_cards_of_rank) * num_colors * num_colors * num_ranks +
-                    # remaining deck size
-                    np.sum(num_cards_of_rank) * num_colors
-            )
-
-        self.action_set = jnp.arange(self.num_moves)
-        if action_spaces is None:
-            self.action_spaces = {i: Discrete(self.num_moves) for i in self.agents}
-        if observation_spaces is None:
-            self.observation_spaces = {i: Discrete(self.obs_size) for i in self.agents}
-
-    def get_legal_moves(self, state: State) -> chex.Array:
-        """Get all agents' legal moves"""
-
-        @partial(jax.vmap, in_axes=[0, None])
-        def _legal_moves(aidx: int, state: State) -> chex.Array:
-            """
-            Legal moves encoding in order:
-            - discard for all cards in hand
-            - play for all cards in hand
-            - hint for all colors and ranks for all other players
-            """
-            move_idx = 1
-            legal_moves = jnp.zeros(self.num_moves)
-            hands = state.player_hands
-            fireworks = state.fireworks
-            info_tokens = state.info_tokens
-            # discard always legal
-            legal_moves = legal_moves.at[move_idx:move_idx+self.hand_size].set(1)
-            move_idx += self.hand_size
-            # play moves always legal
-            legal_moves = legal_moves.at[move_idx:move_idx+self.hand_size].set(1)
-            move_idx += self.hand_size
-            # hints depend on other player cards
-            other_hands = jnp.delete(hands, aidx, axis=0, assume_unique_indices=True)
-
-            def _get_hints_for_hand(carry, unused):
-                """Generates valid hints given hand"""
-                aidx, other_hands = carry
-                hand = other_hands[aidx]
-
-                # get occurrences of each card
-                card_counts = jnp.sum(hand, axis=0)
-                # get occurrences of each color
-                color_counts = jnp.sum(card_counts, axis=1)
-                # get occurrences of each rank
-                rank_counts = jnp.sum(card_counts, axis=0)
-                # check which colors/ranks in hand
-                colors_present = jnp.where(color_counts > 0, 1, 0)
-                ranks_present = jnp.where(rank_counts > 0, 1, 0)
-
-                valid_hints = jnp.concatenate([colors_present, ranks_present])
-                carry = (aidx + 1, other_hands)
-
-                return carry, valid_hints
-
-            _, valid_hints = lax.scan(_get_hints_for_hand, (0, other_hands), None, self.num_agents - 1)
-            # make other player positions relative to current player
-            valid_hints = jnp.roll(valid_hints, aidx, axis=0)
-            # include valid hints in legal moves
-            num_hints = (self.num_agents - 1) * (self.num_colors + self.num_ranks)
-            valid_hints = jnp.concatenate(valid_hints, axis=0)
-            info_tokens_available = (jnp.sum(info_tokens) != 0)
-            valid_hints *= info_tokens_available
-            legal_moves = legal_moves.at[move_idx:move_idx + num_hints].set(valid_hints)
-
-            # only enable noop if not current player
-            cur_player = jnp.nonzero(state.cur_player_idx, size=1)[0][0]
-            not_cur_player = (aidx != cur_player)
-            legal_moves -= legal_moves * not_cur_player
-            legal_moves = legal_moves.at[0].set(not_cur_player)
-
-            return legal_moves
-
-        legal_moves = _legal_moves(self.agent_range, state)
-
-        return {a: legal_moves[i] for i, a in enumerate(self.agents)}
-    
-    def reset(self, key: chex.PRNGKey) -> Tuple[Dict, State]:
-        """Reset the environment"""
-
-
-        def _gen_cards(aidx, unused):
-            """Generates one-hot card encodings given (color, rank) pairs"""
-            color, rank = shuffled_pairs[aidx]
-            card = jnp.zeros((self.num_colors, self.num_ranks))
-            card = card.at[color, rank].set(1)
-
-            return aidx + 1, card
-
-        # get all possible (colour, rank) pairs, including repetitions given num_cards_of_rank
-        colors = jnp.arange(self.num_colors)
-        ranks = jnp.arange(self.num_ranks)
-        ranks = jnp.repeat(ranks, self.num_cards_of_rank)
-        color_rank_pairs = jnp.dstack(jnp.meshgrid(colors, ranks)).reshape(-1, 2)
-        # randomly shuffle (colour, rank) pairs
-        key, _key = jax.random.split(key)
-        shuffled_pairs = jax.random.permutation(_key, color_rank_pairs, axis=0)
-        # generate one-hot encoded deck
-        _, deck = lax.scan(_gen_cards, 0, None, self.deck_size)
+    @partial(jax.jit, static_argnums=[0])
+    def get_first_state(self, key:chex.PRNGKey, deck:chex.Array) -> State:
+        """Get the initial state of the game"""
 
         def _deal_cards(aidx, unused):
             """Deals cards to players from top of deck"""
             # top of deck is first array element
             start = aidx * self.hand_size
-            hand = lax.dynamic_slice(deck, (start, 0, 0), (self.hand_size, self.num_colors, self.num_ranks))
+            hand = lax.dynamic_slice(
+                deck, (start, 0, 0), (self.hand_size, self.num_colors, self.num_ranks)
+            )
 
             return aidx + 1, hand
 
         _, hands = lax.scan(_deal_cards, 0, None, self.num_agents)
         num_cards_dealt = self.num_agents * self.hand_size
 
         # start off with all (color, rank) combinations being possible for all cards
-        card_knowledge = jnp.ones((self.num_agents, self.hand_size, (self.num_colors * self.num_ranks)))
+        card_knowledge = jnp.ones(
+            (self.num_agents, self.hand_size, (self.num_colors * self.num_ranks))
+        )
         colors_revealed = jnp.zeros((self.num_agents, self.hand_size, self.num_colors))
         ranks_revealed = jnp.zeros((self.num_agents, self.hand_size, self.num_ranks))
 
         # init discard pile
         discard_pile = jnp.zeros_like(deck)
         num_cards_discarded = 0
 
         # remove dealt cards from deck
-        deck = deck.at[:num_cards_dealt].set(jnp.zeros((self.num_colors, self.num_ranks)))
+        deck = deck.at[:num_cards_dealt].set(
+            jnp.zeros((self.num_colors, self.num_ranks))
+        )
         remaining_deck_size = jnp.zeros(self.deck_size).at[:-num_cards_dealt].set(1)
 
         # thermometer encoded
         life_tokens = jnp.ones(self.max_life_tokens)
         info_tokens = jnp.ones(self.max_info_tokens).astype(int)
         fireworks = jnp.zeros((self.num_colors, self.num_ranks))
 
         # other state variable inits
-        score = 0
         cur_player_idx = jnp.zeros(self.num_agents).at[0].set(1)
         terminal = False
         out_of_lives = False
         bombed = False
         last_round_count = 0
-        last_moves = jnp.zeros((self.num_agents, self.num_moves))
 
         state = State(
             deck=deck,
             discard_pile=discard_pile,
             fireworks=fireworks,
             player_hands=hands,
             info_tokens=info_tokens,
             terminal=terminal,
             life_tokens=life_tokens,
             card_knowledge=card_knowledge,
             colors_revealed=colors_revealed,
             ranks_revealed=ranks_revealed,
             num_cards_dealt=num_cards_dealt,
             num_cards_discarded=num_cards_discarded,
-            last_moves=last_moves,
             cur_player_idx=cur_player_idx,
             out_of_lives=out_of_lives,
             last_round_count=last_round_count,
             bombed=bombed,
-            remaining_deck_size=remaining_deck_size
+            remaining_deck_size=remaining_deck_size,
+            turn=0,
+            score=0,
         )
 
-        return self.get_obs(state), state
+        return state
 
     @partial(jax.jit, static_argnums=[0])
-    def get_obs(self, state: State) -> Dict:
-        """
-        Get all agents' observations
-        Card knowledge observation: includes per card information of past hints
-        as well as simple inferred knowledge
-        """
-        @partial(jax.vmap, in_axes=[0, None])
-        def _observation(aidx: int, state: State) -> chex.Array:
-            """Generate individual agent's observation"""
-            hands = state.player_hands
-            other_hands = jnp.delete(hands, aidx, axis=0, assume_unique_indices=True)
-            other_hands = jnp.roll(other_hands, aidx, axis=0)
-            other_hands = jnp.reshape(other_hands, (-1,))
-
-            knowledge = state.card_knowledge.at[aidx].get()
-            knowledge = jnp.reshape(knowledge, (-1,))
-
-            colors = state.colors_revealed.at[aidx].get()
-            colors = jnp.reshape(colors, (-1,))
-
-            ranks = state.ranks_revealed.at[aidx].get()
-            ranks = jnp.reshape(ranks, (-1,))
-
-            # legal_moves = state.legal_moves[aidx].get()
-
-            fireworks = jnp.reshape(state.fireworks, (-1,))
-
-            last_moves = jnp.roll(state.last_moves, aidx, axis=0)
-            last_moves = jnp.reshape(last_moves, (-1,))
+    def reset_game(self, key: chex.PRNGKey) -> State:
+        """Create a random deck and return the first state of the game"""
 
-            discard_pile = jnp.reshape(state.discard_pile, (-1,))
-
-            obs = jnp.concatenate([knowledge, colors, ranks, other_hands, # legal_moves,
-                                   last_moves, fireworks, state.info_tokens, state.life_tokens, state.cur_player_idx,
-                                   discard_pile, state.remaining_deck_size])
+        def _gen_cards(aidx, unused):
+            """Generates one-hot card encodings given (color, rank) pairs"""
+            color, rank = shuffled_pairs[aidx]
+            card = jnp.zeros((self.num_colors, self.num_ranks))
+            card = card.at[color, rank].set(1)
 
-            return obs
+            return aidx + 1, card
 
-        obs = _observation(self.agent_range, state)
+        # get all possible (colour, rank) pairs, including repetitions given num_cards_of_rank
+        colors = jnp.arange(self.num_colors)
+        ranks = jnp.arange(self.num_ranks)
+        ranks = jnp.repeat(ranks, self.num_cards_of_rank)
+        color_rank_pairs = jnp.dstack(jnp.meshgrid(colors, ranks)).reshape(-1, 2)
+        # randomly shuffle (colour, rank) pairs
+        key, _key = jax.random.split(key)
+        shuffled_pairs = jax.random.permutation(_key, color_rank_pairs, axis=0)
+        # generate one-hot encoded deck
+        _, deck = lax.scan(_gen_cards, 0, None, self.deck_size)
 
-        return {a: obs[i] for i, a in enumerate(self.agents)}
+        return self.get_first_state(key, deck)
 
     @partial(jax.jit, static_argnums=[0])
-    def step_env(self, key: chex.PRNGKey, state: State, actions: Dict,
-                 ) -> Tuple[chex.Array, State, Dict, Dict, Dict]:
-        """
-        Step the environment
-        Executes one turn
-        """
-        # get actions as array
-        actions = jnp.array([actions[i] for i in self.agents])
-        aidx = jnp.nonzero(state.cur_player_idx, size=1)[0][0]
-        action = actions.at[aidx].get()
-        # ignore noop for acting agent
-        action = action[0] - 1
-
-        # execute the current player's action and its consequences
-        state, reward = self.step_agent(key, state, aidx, action)
-
-        done = self.terminal(state)
-        dones = {agent: done for agent in self.agents}
-        dones["__all__"] = done
-
-        rewards = {agent: reward for agent in self.agents}
-        # rewards["__all__"] = reward
-
-        info = {}
+    def reset_game_from_deck(self, key: chex.PRNGKey, deck:chex.PRNGKey) -> State:
+        return self.get_first_state(key, deck)
 
-        return (
-            lax.stop_gradient(self.get_obs(state)),
-            lax.stop_gradient(state),
-            rewards,
-            dones,
-            info
-        )
-
-    def step_agent(self, key: chex.PRNGKey, state: State, aidx: int, action: int,
-                   ) -> Tuple[State, int]:
+    @partial(jax.jit, static_argnums=[0])
+    def step_game(
+        self,
+        state: State,
+        aidx: int,
+        action: int,
+    ) -> Tuple[State, int]:
         """
         Execute the current player's action and its consequences
         """
         # check move type
-        is_discard = (action < self.hand_size)
-        is_hint = ((2 * self.hand_size) <= action)
+        is_discard = action < self.hand_size
+        is_hint = (2 * self.hand_size) <= action
         # initialise reward for move
         reward = 0
 
         def _discard_play_fn(state, action):
             """Discard or play selected card according to action selection"""
             # get hand and card info
             hand_before = state.player_hands.at[aidx].get()
-            card_idx = ((is_discard * action) + (jnp.logical_not(is_discard) * (action - self.hand_size))
-                        ).astype(int)
+            card_idx = (
+                (is_discard * action)
+                + (jnp.logical_not(is_discard) * (action - self.hand_size))
+            ).astype(int)
             card = hand_before.at[card_idx].get()
 
-            # discard selected card if discard action
-            discard_card = jnp.zeros_like(card) + (is_discard * card)
-            discard_pile = state.discard_pile.at[state.num_cards_discarded].set(discard_card)
-            num_cards_discarded = state.num_cards_discarded + is_discard
-
             # gain an info token for discarding if discard action
             infos_remaining = jnp.sum(state.info_tokens)
-            infos_depleted = (infos_remaining < self.max_info_tokens)
+            infos_depleted = infos_remaining < self.max_info_tokens
             new_infos = (infos_remaining + (is_discard * infos_depleted)).astype(int)
             info_tokens = state.info_tokens.at[new_infos - 1].set(1)
 
             # play selected card if play action
             color, rank = jnp.nonzero(card, size=1)
             color_fireworks = state.fireworks.at[color].get()
-            is_valid_play = (rank == jnp.sum(color_fireworks))
-            make_play = jnp.logical_and(is_valid_play, jnp.logical_not(is_discard)).squeeze(0)
+            is_valid_play = rank == jnp.sum(color_fireworks)
+            make_play = jnp.logical_and(
+                is_valid_play, jnp.logical_not(is_discard)
+            ).squeeze(0)
+
+            # gain another info token if completed a color
+            is_final_card = jnp.logical_and(
+                is_valid_play, rank == self.num_ranks - 1
+            ).squeeze(0)
+            infos_remaining = jnp.sum(info_tokens)
+            infos_depleted = infos_remaining < self.max_info_tokens
+            new_infos = (infos_remaining + (is_final_card * infos_depleted)).astype(int)
+            info_tokens = info_tokens.at[new_infos - 1].set(1)
 
             # increment fireworks if valid play action
-            color_fireworks = color_fireworks.at[0, jnp.sum(color_fireworks).astype(int)].set(make_play)
+            color_fireworks = color_fireworks.at[
+                0, jnp.sum(color_fireworks).astype(int)
+            ].set(make_play)
             fireworks = state.fireworks.at[color].set(color_fireworks)
 
-            # discard if play action was invalid
-            failed_play = jnp.logical_and(jnp.logical_not(is_valid_play), jnp.logical_not(is_discard)).squeeze(0)
-            discard_card = jnp.zeros_like(card) + (failed_play * card)
-            discard_pile = state.discard_pile.at[state.num_cards_discarded].set(discard_card)
-            num_cards_discarded = state.num_cards_discarded + failed_play
+            # the card must be discarded if action is discard or the play action is not valid
+            discard_card = ((~is_valid_play) | (is_discard)).squeeze(0)
+            discarded_card = jnp.zeros_like(card) + (discard_card * card)
+            discard_pile = state.discard_pile.at[state.num_cards_discarded].set(
+                discarded_card
+            )
+            num_cards_discarded = state.num_cards_discarded + discard_card
 
             # remove life token if invalid play
-            life_lost = jnp.logical_and(jnp.logical_not(is_valid_play),
-                                        jnp.logical_not(is_discard)).squeeze(0)
+            life_lost = jnp.logical_and(
+                jnp.logical_not(is_valid_play), jnp.logical_not(is_discard)
+            ).squeeze(0)
             num_life_tokens = jnp.sum(state.life_tokens).astype(int)
-            life_tokens = state.life_tokens.at[num_life_tokens - 1].set(jnp.logical_not(life_lost))
+            life_tokens = state.life_tokens.at[num_life_tokens - 1].set(
+                jnp.logical_not(life_lost)
+            )
 
             # remove knowledge of selected card
             player_knowledge = state.card_knowledge.at[aidx].get()
-            player_knowledge = jnp.delete(player_knowledge, card_idx, axis=0, assume_unique_indices=True)
-            player_knowledge = jnp.append(player_knowledge, jnp.ones((1, self.num_colors * self.num_ranks)),
-                                          axis=0)
+            player_knowledge = jnp.delete(
+                player_knowledge, card_idx, axis=0, assume_unique_indices=True
+            )
+            player_knowledge = jnp.append(
+                player_knowledge,
+                jnp.ones((1, self.num_colors * self.num_ranks)),
+                axis=0,
+            )
             card_knowledge = state.card_knowledge.at[aidx].set(player_knowledge)
             # color hint knowledge removal
             player_colors_revealed = state.colors_revealed.at[aidx].get()
-            player_colors_revealed = jnp.delete(player_colors_revealed, card_idx, axis=0, assume_unique_indices=True)
-            player_colors_revealed = jnp.append(player_colors_revealed, jnp.ones((1, self.num_colors)), axis=0)
+            player_colors_revealed = jnp.delete(
+                player_colors_revealed, card_idx, axis=0, assume_unique_indices=True
+            )
+            player_colors_revealed = jnp.append(
+                player_colors_revealed, jnp.zeros((1, self.num_colors)), axis=0
+            )
             colors_revealed = state.colors_revealed.at[aidx].set(player_colors_revealed)
             # rank hint knowledge removal
             player_ranks_revealed = state.ranks_revealed.at[aidx].get()
-            player_ranks_revealed = jnp.delete(player_ranks_revealed, card_idx, axis=0, assume_unique_indices=True)
-            player_ranks_revealed = jnp.append(player_ranks_revealed, jnp.ones((1, self.num_ranks)), axis=0)
+            player_ranks_revealed = jnp.delete(
+                player_ranks_revealed, card_idx, axis=0, assume_unique_indices=True
+            )
+            player_ranks_revealed = jnp.append(
+                player_ranks_revealed, jnp.zeros((1, self.num_ranks)), axis=0
+            )
             ranks_revealed = state.ranks_revealed.at[aidx].set(player_ranks_revealed)
 
             # deal a new card
             # check if in last round
-            in_last_round = (state.last_round_count > 0)
+            in_last_round = state.last_round_count > 0
             # deal empty card from top of deck if in last round
             num_dealt = lax.select(in_last_round, 0, state.num_cards_dealt)
             new_card = state.deck.at[state.num_cards_dealt].get()
-            hand_without_old = jnp.delete(hand_before, card_idx, axis=0, assume_unique_indices=True)
+            hand_without_old = jnp.delete(
+                hand_before, card_idx, axis=0, assume_unique_indices=True
+            )
             new_hand = jnp.append(hand_without_old, new_card[jnp.newaxis, :, :], axis=0)
             hands = state.player_hands.at[aidx].set(new_hand)
             deck = state.deck.at[state.num_cards_dealt].set(jnp.zeros_like(card))
             # don't increment if in last round
-            num_cards_dealt = lax.select(in_last_round, state.num_cards_dealt, state.num_cards_dealt + 1)
+            num_cards_dealt = lax.select(
+                in_last_round, state.num_cards_dealt, state.num_cards_dealt + 1
+            )
             remaining_deck_size = state.remaining_deck_size.at[-num_cards_dealt].set(0)
 
             return state.replace(
                 deck=deck,
                 discard_pile=discard_pile,
                 player_hands=hands,
                 card_knowledge=card_knowledge,
                 colors_revealed=colors_revealed,
                 ranks_revealed=ranks_revealed,
                 fireworks=fireworks,
                 info_tokens=info_tokens,
                 life_tokens=life_tokens,
                 num_cards_dealt=num_cards_dealt,
                 num_cards_discarded=num_cards_discarded,
-                remaining_deck_size=remaining_deck_size
+                remaining_deck_size=remaining_deck_size,
             )
 
         def _hint_fn(state, action):
             # get effective hint action index
             action_idx = action - (2 * self.hand_size)
 
             # get player hint is being given to
             hints_per_player = self.num_colors + self.num_ranks
             hint_player_before = jnp.floor(action_idx / hints_per_player).astype(int)
-            hint_player = ((aidx + 1 + hint_player_before) % self.num_agents).astype(int)
+            hint_player = ((aidx + 1 + hint_player_before) % self.num_agents).astype(
+                int
+            )
             hint_idx = (action_idx % hints_per_player).astype(int)
 
             # define hint as possibilities to remove
             hint = jnp.zeros(hints_per_player)
             hint = hint.at[hint_idx].set(1)
-            is_color_hint = (hint_idx < self.num_colors)
+            is_color_hint = hint_idx < self.num_colors
             is_rank_hint = jnp.logical_not(is_color_hint)
-            hint_color = (hint.at[:self.num_colors].get() * is_color_hint).astype(int)
-            hint_rank = (hint.at[self.num_colors:].get() * is_rank_hint).astype(int)
+            hint_color = (hint.at[: self.num_colors].get() * is_color_hint).astype(int)
+            hint_rank = (hint.at[self.num_colors :].get() * is_rank_hint).astype(int)
 
             # get current card knowledge of relevant player
             cur_knowledge = state.card_knowledge.at[hint_player].get()
 
             # get relevant player's hand
             cards = state.player_hands.at[hint_player].get()
             card_colors = jnp.sum(cards, axis=2)
             card_ranks = jnp.sum(cards, axis=1)
 
             # check which cards have hinted color/rank
             color_hint_matches = jnp.matmul(card_colors, hint_color)
             rank_hint_matches = jnp.matmul(card_ranks, hint_rank)
 
             negative_color_hints = jnp.outer(1 - color_hint_matches, hint_color)
-            negative_color_hints = jnp.repeat(negative_color_hints, self.num_colors, axis=1).reshape(
-                cur_knowledge.shape
-            )
+            negative_color_hints = jnp.repeat(
+                negative_color_hints, self.num_colors, axis=1
+            ).reshape(cur_knowledge.shape)
             negative_rank_hints = jnp.outer(1 - rank_hint_matches, hint_rank)
-            negative_rank_hints = jnp.repeat(negative_rank_hints, self.num_ranks, axis=0).reshape(
-                cur_knowledge.shape
-            )
+            negative_rank_hints = jnp.repeat(
+                negative_rank_hints, self.num_ranks, axis=0
+            ).reshape(cur_knowledge.shape)
 
             color_mask = (color_hint_matches * jnp.ones_like(card_colors)).transpose()
             rank_mask = (rank_hint_matches * jnp.ones_like(card_ranks)).transpose()
 
             color_hints = color_mask * (1 - hint_color * jnp.ones_like(card_colors))
-            color_hints = jnp.repeat(color_hints, self.num_colors, axis=1).reshape(cur_knowledge.shape)
+            color_hints = jnp.repeat(color_hints, self.num_colors, axis=1).reshape(
+                cur_knowledge.shape
+            )
             rank_hints = rank_mask * (1 - hint_rank * jnp.ones_like(card_ranks))
-            rank_hints = jnp.repeat(rank_hints, self.num_ranks, axis=0).reshape(cur_knowledge.shape)
+            rank_hints = jnp.repeat(rank_hints, self.num_ranks, axis=0).reshape(
+                cur_knowledge.shape
+            )
 
             total_color_hint = color_hints + negative_color_hints
             total_rank_hint = rank_hints + negative_rank_hints
 
-            new_knowledge = (cur_knowledge - (is_color_hint * total_color_hint)).clip(min=0)
-            new_knowledge = (cur_knowledge - (is_rank_hint * total_rank_hint)).clip(min=0)
+            new_color_knowledge = (
+                cur_knowledge - (is_color_hint * total_color_hint)
+            ).clip(min=0)
+            new_rank_knowledge = (
+                cur_knowledge - (is_rank_hint * total_rank_hint)
+            ).clip(min=0)
+            new_knowledge = jnp.where(
+                is_color_hint, new_color_knowledge, new_rank_knowledge
+            )
             card_knowledge = state.card_knowledge.at[hint_player].set(new_knowledge)
 
             colors_revealed_player = jnp.outer(color_hint_matches, hint_color)
-            colors_revealed_player = (state.colors_revealed.at[hint_player].get() + colors_revealed_player
-                                      ).clip(max=1)
-            colors_revealed = state.colors_revealed.at[hint_player].set(colors_revealed_player)
+            colors_revealed_player = (
+                state.colors_revealed.at[hint_player].get() + colors_revealed_player
+            ).clip(max=1)
+            colors_revealed = state.colors_revealed.at[hint_player].set(
+                colors_revealed_player
+            )
             ranks_revealed_player = jnp.outer(rank_hint_matches, hint_rank)
-            ranks_revealed_player = (state.ranks_revealed.at[hint_player].get() + ranks_revealed_player
-                                      ).clip(max=1)
-            ranks_revealed = state.ranks_revealed.at[hint_player].set(ranks_revealed_player)
+            ranks_revealed_player = (
+                state.ranks_revealed.at[hint_player].get() + ranks_revealed_player
+            ).clip(max=1)
+            ranks_revealed = state.ranks_revealed.at[hint_player].set(
+                ranks_revealed_player
+            )
 
             # remove an info token
             num_info_tokens = jnp.sum(state.info_tokens).astype(int) - 1
             info_tokens = jnp.arange(self.max_info_tokens)
             info_tokens = (info_tokens < num_info_tokens).astype(int)
             return state.replace(
                 card_knowledge=card_knowledge,
                 info_tokens=info_tokens,
                 colors_revealed=colors_revealed,
-                ranks_revealed=ranks_revealed
+                ranks_revealed=ranks_revealed,
             )
 
         # update fireworks
         fireworks_before = jnp.sum(state.fireworks, axis=(0, 1))
         state = lax.cond(is_hint, _hint_fn, _discard_play_fn, state, action)
         fireworks_after = jnp.sum(state.fireworks, axis=(0, 1))
 
         # check if lives left
         num_lives = jnp.sum(state.life_tokens)
-        out_of_lives = (num_lives == 0)
+        out_of_lives = num_lives == 0
 
         # check if terminal
-        game_won = (fireworks_after == (self.num_colors * self.num_ranks))
-        deck_empty = (state.num_cards_dealt >= self.deck_size)
+        game_won = fireworks_after == (self.num_colors * self.num_ranks)
+        deck_empty = state.num_cards_dealt >= self.deck_size
         last_round_count = state.last_round_count + deck_empty
-        last_round_done = (last_round_count == self.num_agents)
-        terminal = jnp.logical_or(jnp.logical_or(state.out_of_lives, game_won), last_round_done)
-
-        # last moves
-        last_moves = state.last_moves.at[aidx, :].set(0)
-        last_moves = last_moves.at[aidx, action+1].set(1)
+        last_round_done = last_round_count == self.num_agents + 1
+        terminal = jnp.logical_or(
+            jnp.logical_or(state.out_of_lives, game_won), last_round_done
+        )
 
         # define reward as difference in fireworks
-        reward += (jnp.logical_not(out_of_lives) * (fireworks_after - fireworks_before))
+        reward += jnp.logical_not(out_of_lives) * (fireworks_after - fireworks_before)
         # bomb-0 scoring
-        reward -= (out_of_lives * fireworks_after * jnp.logical_not(state.bombed))
+        reward -= out_of_lives * fireworks_after * jnp.logical_not(state.bombed)
         bombed = jnp.logical_or(out_of_lives, state.bombed)
         aidx = (aidx + 1) % self.num_agents
 
         cur_player_idx = jnp.zeros(self.num_agents).at[aidx].set(1)
 
-        return state.replace(terminal=terminal,
-                             last_moves=last_moves,
-                             cur_player_idx=cur_player_idx,
-                             out_of_lives=out_of_lives,
-                             last_round_count=last_round_count,
-                             bombed=bombed
-                             ), reward
-
-    def terminal(self, state: State) -> bool:
-        """Check whether state is terminal."""
-        return state.terminal
-
-    @property
-    def name(self) -> str:
-        """Environment name."""
-        return "Hanabi"
-
-    @property
-    def num_actions(self) -> int:
-        """Number of actions possible in environment."""
-        return self.num_moves
-
-    def observation_space(self, agent: str):
-        """ Observation space for a given agent."""
-        return self.observation_spaces[agent]
-
-    def action_space(self, agent: str):
-        """ Action space for a given agent."""
-        return self.action_spaces[agent]
+        return (
+            state.replace(
+                terminal=terminal,
+                cur_player_idx=cur_player_idx,
+                out_of_lives=out_of_lives,
+                last_round_count=last_round_count,
+                bombed=bombed,
+                turn=state.turn + 1,
+                score=state.score + reward.astype(int),
+            ),
+            reward,
+        )
```

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/mabrax/mabrax_env.py` & `jaxmarl-0.0.3/jaxmarl/environments/mabrax/mabrax_env.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/mabrax/mappings.py` & `jaxmarl-0.0.3/jaxmarl/environments/mabrax/mappings.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/mpe/__init__.py` & `jaxmarl-0.0.3/jaxmarl/environments/mpe/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/mpe/mpe_visualizer.py` & `jaxmarl-0.0.3/jaxmarl/environments/mpe/mpe_visualizer.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/mpe/simple.py` & `jaxmarl-0.0.3/jaxmarl/environments/mpe/simple.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,16 +325,15 @@
 
         return self.action_decoder(self.agent_range, actions)
 
     @partial(jax.vmap, in_axes=[None, 0, 0])
     def _decode_continuous_action(
         self, a_idx: int, action: chex.Array
     ) -> Tuple[chex.Array, chex.Array]:
-        u = jnp.array([action[1] - action[2], action[3] - action[4]])
-
+        u = jnp.array([action[2] - action[1], action[4] - action[3]])
         u = u * self.accel[a_idx] * self.moveable[a_idx]
         c = action[5:]
         return u, c
 
     @partial(jax.vmap, in_axes=[None, 0, 0])
     def _decode_discrete_action(
         self, a_idx: int, action: chex.Array
```

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/mpe/simple_adversary.py` & `jaxmarl-0.0.3/jaxmarl/environments/mpe/simple_adversary.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/mpe/simple_crypto.py` & `jaxmarl-0.0.3/jaxmarl/environments/mpe/simple_crypto.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/mpe/simple_facmac.py` & `jaxmarl-0.0.3/jaxmarl/environments/mpe/simple_facmac.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/mpe/simple_push.py` & `jaxmarl-0.0.3/jaxmarl/environments/mpe/simple_push.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from functools import partial
 from jaxmarl.environments.mpe.simple import SimpleMPE, State
 from jaxmarl.environments.mpe.default_params import *
 from gymnax.environments.spaces import Box
 
 # Obstacle Colours
 COLOUR_1 = jnp.array([0.1, 0.9, 0.1])
-COLOUR_2 = jnp.array([0.1, 0.1, 0.9])  # BUG
+COLOUR_2 = jnp.array([0.1, 0.1, 0.9])  
 OBS_COLOUR = jnp.concatenate([COLOUR_1, COLOUR_2])
 
 
 class SimplePushMPE(SimpleMPE):
     def __init__(
         self,
         num_good_agents=1,
@@ -129,15 +129,15 @@
         def _good(aidx: int):
             goal_rel_pos = state.p_pos[state.goal + self.num_agents] - state.p_pos[aidx]
 
             agent_colour = jnp.full((3,), 0.25)
             agent_colour = agent_colour.at[state.goal + 1].set(0.75)
 
             return jnp.concatenate(
-                [  # TODO
+                [  
                     state.p_vel[aidx].flatten(),  # 2
                     goal_rel_pos.flatten(),  # 2
                     agent_colour,
                     landmark_pos[aidx].flatten(),  # 5, 2
                     OBS_COLOUR.flatten(),
                     other_pos[aidx].flatten(),  # 5, 2
                 ]
```

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/mpe/simple_reference.py` & `jaxmarl-0.0.3/jaxmarl/environments/mpe/simple_reference.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/mpe/simple_speaker_listener.py` & `jaxmarl-0.0.3/jaxmarl/environments/mpe/simple_speaker_listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     ) -> Tuple[chex.Array, chex.Array]:
         u = jnp.zeros((self.num_agents, self.dim_p))
         c = jnp.zeros((self.num_agents, self.dim_c))
         c = c.at[0].set(action[SPEAKER])
 
         u_act = action[LISTENER]
 
-        u_act = jnp.array([u_act[1] - u_act[2], u_act[3] - u_act[4]]) * self.accel[1]
+        u_act = jnp.array([u_act[2] - u_act[1], u_act[4] - u_act[3]]) * self.accel[1]
         u = u.at[1].set(u_act)
 
         return u, c
 
     def _decode_discrete_action(
         self,
         a_idx: int,
```

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/mpe/simple_spread.py` & `jaxmarl-0.0.3/jaxmarl/environments/mpe/simple_spread.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,18 @@
     ):
         dim_c = 2  # NOTE follows code rather than docs
 
         # Action and observation spaces
         agents = ["agent_{}".format(i) for i in range(num_agents)]
         landmarks = ["landmark {}".format(i) for i in range(num_landmarks)]
 
-        observation_spaces = {i: Box(-jnp.inf, jnp.inf, (18,)) for i in agents}
+        observation_spaces = {
+            i:Box(-jnp.inf, jnp.inf, (4+(num_agents-1)*4+(num_landmarks*2),)) 
+            for i in agents
+        }
 
         colour = [AGENT_COLOUR] * num_agents + [OBS_COLOUR] * num_landmarks
 
         # Env specific parameters
         self.local_ratio = local_ratio
         assert (
             self.local_ratio >= 0.0 and self.local_ratio <= 1.0
```

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/mpe/simple_tag.py` & `jaxmarl-0.0.3/jaxmarl/environments/mpe/simple_tag.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/mpe/simple_world_comm.py` & `jaxmarl-0.0.3/jaxmarl/environments/mpe/simple_world_comm.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         return u, c
 
     def _decode_continuous_action(
         self, a_idx: int, actions: chex.Array
     ) -> Tuple[chex.Array, chex.Array]:
         @partial(jax.vmap, in_axes=[0, 0])
         def _set_u(a_idx, action):
-            u = jnp.array([action[1] - action[2], action[3] - action[4]])
+            u = jnp.array([action[2] - action[1], action[4] - action[3]])
             return u * self.accel[a_idx] * self.moveable[a_idx]
 
         lact = actions[self.leader]
         aact = jnp.array([actions[a] for a in self.adversaries])
         gact = jnp.array([actions[a] for a in self.good_agents])
 
         u_acts = jnp.concatenate([lact[:5][None], aact, gact])
```

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/multi_agent_env.py` & `jaxmarl-0.0.3/jaxmarl/environments/multi_agent_env.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/overcooked/common.py` & `jaxmarl-0.0.3/jaxmarl/environments/overcooked/common.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/overcooked/interactive.py` & `jaxmarl-0.0.3/jaxmarl/environments/overcooked/interactive.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/overcooked/layouts.py` & `jaxmarl-0.0.3/jaxmarl/environments/overcooked/layouts.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/overcooked/overcooked.py` & `jaxmarl-0.0.3/jaxmarl/environments/overcooked/overcooked.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/smax/distributions.py` & `jaxmarl-0.0.3/jaxmarl/environments/smax/distributions.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/smax/heuristic_enemy.py` & `jaxmarl-0.0.3/jaxmarl/environments/smax/heuristic_enemy.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/smax/heuristic_enemy_smax_env.py` & `jaxmarl-0.0.3/jaxmarl/environments/smax/heuristic_enemy_smax_env.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import dataclasses
 from jaxmarl.environments.smax.smax_env import SMAX
+from jaxmarl.environments.smax.smax_env import State as SMAXState
 from jaxmarl.environments.smax.heuristic_enemy import (
     create_heuristic_policy,
     get_heuristic_policy_initial_state,
 )
 from jaxmarl.environments.multi_agent_env import MultiAgentEnv
 import chex
 from typing import Dict, Optional, Tuple
@@ -55,38 +57,82 @@
 
     def get_enemy_actions(self, key, enemy_policy_state, enemy_obs):
         raise NotImplementedError
 
     def get_enemy_policy_initial_state(self, key):
         raise NotImplementedError
 
-    @partial(jax.jit, static_argnums=(0,))
-    def step_env(self, key: chex.PRNGKey, state: State, actions: Dict[str, chex.Array]):
+    @partial(jax.jit, static_argnums=(0, 4))
+    def step_env(
+        self,
+        key: chex.PRNGKey,
+        state: State,
+        actions: Dict[str, chex.Array],
+        get_state_sequence=False,
+    ):
         jaxmarl_state = state.state
         obs = self._env.get_obs(jaxmarl_state)
-        enemy_obs = jnp.array([obs[agent] for agent in self.enemy_agents])
+        enemy_obs = self._env.get_obs_unit_list(jaxmarl_state)
+        enemy_obs = jnp.array([enemy_obs[agent] for agent in self.enemy_agents])
         key, action_key = jax.random.split(key)
         enemy_actions, enemy_policy_state = self.get_enemy_actions(
             action_key, state.enemy_policy_state, enemy_obs
         )
+        enemy_actions = jnp.array([enemy_actions[i] for i in self.enemy_agents])
+        actions = jnp.array([actions[i] for i in self.agents])
+        enemy_movement_actions, enemy_attack_actions = (
+            self._env._decode_discrete_actions(enemy_actions)
+        )
+        if self._env.action_type == "continuous":
+            cont_actions = jnp.zeros((len(self.all_agents), 4))
+            cont_actions = cont_actions.at[: self.num_allies].set(actions)
+            key, action_key = jax.random.split(key)
+            ally_movement_actions, ally_attack_actions = (
+                self._env._decode_continuous_actions(
+                    action_key, jaxmarl_state, cont_actions
+                )
+            )
+            ally_movement_actions = ally_movement_actions[: self.num_allies]
+            ally_attack_actions = ally_attack_actions[: self.num_allies]
+        else:
+            ally_movement_actions, ally_attack_actions = (
+                self._env._decode_discrete_actions(actions)
+            )
 
-        actions = {k: v.squeeze() for k, v in actions.items()}
-        actions = {**enemy_actions, **actions}
-        obs, jaxmarl_state, rewards, dones, infos = self._env.step_env(
-            key, jaxmarl_state, actions
+        movement_actions = jnp.concatenate(
+            [ally_movement_actions, enemy_movement_actions], axis=0
         )
-        new_obs = {agent: obs[agent] for agent in self.agents}
-        new_obs["world_state"] = obs["world_state"]
-        rewards = {agent: rewards[agent] for agent in self.agents}
-        all_done = dones["__all__"]
-        dones = {agent: dones[agent] for agent in self.agents}
-        dones["__all__"] = all_done
+        attack_actions = jnp.concatenate([ally_attack_actions, enemy_attack_actions], axis=0)
 
-        state = state.replace(enemy_policy_state=enemy_policy_state, state=jaxmarl_state)
-        return new_obs, state, rewards, dones, infos
+        if not get_state_sequence:
+            obs, jaxmarl_state, rewards, dones, infos = self._env.step_env_no_decode(
+                key,
+                jaxmarl_state,
+                (movement_actions, attack_actions),
+                get_state_sequence=get_state_sequence,
+            )
+            new_obs = {agent: obs[agent] for agent in self.agents}
+            new_obs["world_state"] = obs["world_state"]
+            rewards = {agent: rewards[agent] for agent in self.agents}
+            all_done = dones["__all__"]
+            dones = {agent: dones[agent] for agent in self.agents}
+            dones["__all__"] = all_done
+
+            state = state.replace(
+                enemy_policy_state=enemy_policy_state, state=jaxmarl_state
+            )
+            return new_obs, state, rewards, dones, infos
+        else:
+            states = self._env.step_env_no_decode(
+                key,
+                jaxmarl_state,
+                (movement_actions, attack_actions),
+                get_state_sequence=get_state_sequence,
+            )
+            return states
 
     @partial(jax.jit, static_argnums=(0,))
     def get_avail_actions(self, state: State):
         avail_actions = self._env.get_avail_actions(state.state)
         return {agent: avail_actions[agent] for agent in self.agents}
 
     def get_all_unit_obs(self, state: State):
@@ -106,36 +152,28 @@
         # TODO jit/scan this
         expanded_state_seq = []
 
         # TODO this actually can't take a key because recording this key is really hard
         # it's not exposed to the user so we can't ask them to store it. Not a problem
         # for now but will have to get creative in the future potentially.
         for key, state, actions in state_seq:
-            agents = self.all_agents
             # There is a split in the step function of MultiAgentEnv
             # We call split here so that the action key is the same.
             key, _ = jax.random.split(key)
-            key, key_action = jax.random.split(key)
-            obs = self.get_all_unit_obs(state)
-            obs = jnp.array([obs[agent] for agent in self.enemy_agents])
-            enemy_actions, _ = self.get_enemy_actions(
-                key_action, state.enemy_policy_state, obs
-            )
-            actions = {k: v.squeeze() for k, v in actions.items()}
-            actions = {**enemy_actions, **actions}
-            for _ in range(self.world_steps_per_env_step):
-                expanded_state_seq.append((key, state.state, actions))
-                world_actions = jnp.array([actions[i] for i in agents])
-                key, step_key = jax.random.split(key)
-                _state = state.state
-                _state = self._env._world_step(step_key, _state, world_actions)
-                _state = self._env._kill_agents_touching_walls(_state)
-                _state = self._env._update_dead_agents(_state)
-                _state = self._env._push_units_away(_state)
-                state = state.replace(state=_state)
+            states = self.step_env(key, state, actions, get_state_sequence=True)
+            states = list(map(SMAXState, *dataclasses.astuple(states)))
+            viz_actions = {
+                agent: states[-1].prev_attack_actions[i]
+                for i, agent in enumerate(self.all_agents)
+            }
+
+            expanded_state_seq.append((key, state.state, viz_actions))
+            expanded_state_seq.extend(
+                zip([key] * len(states), states, [viz_actions] * len(states))
+            )
             state = state.replace(
                 state=state.state.replace(terminal=self.is_terminal(state))
             )
         return expanded_state_seq
 
 
 class HeuristicEnemySMAX(EnemySMAX):
```

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/smax/smax_env.py` & `jaxmarl-0.0.3/jaxmarl/environments/smax/smax_env.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,41 @@
+import dataclasses
 import jax.numpy as jnp
 import jax
+from jax.experimental import sparse
 from jaxmarl.environments.multi_agent_env import MultiAgentEnv
 from jaxmarl.environments.spaces import Box, Discrete
 from jaxmarl.environments.smax.distributions import (
     SurroundAndReflectPositionDistribution,
     UniformUnitTypeDistribution,
 )
 import chex
 from typing import Tuple, Dict, Optional
 from flax.struct import dataclass
 from enum import IntEnum
 from functools import partial
 import io
+import math
 
 
 @dataclass
 class State:
     unit_positions: chex.Array
     unit_alive: chex.Array
     unit_teams: chex.Array
     unit_health: chex.Array
     unit_types: chex.Array
     unit_weapon_cooldowns: chex.Array
-    prev_actions: chex.Array
+    prev_movement_actions: chex.Array
+    prev_attack_actions: chex.Array
     time: int
     terminal: bool
 
 
 @dataclass
-class WorldDelta:
-    """Encapsulates the effect of an agent's action"""
-
-    pos: chex.Array
-    attacked_idx: int
-    cooldown_diff: float
-    health_diff: float
-
-
-@dataclass
 class Scenario:
     unit_types: chex.Array
     num_allies: int
     num_enemies: int
     smacv2_position_generation: bool
     smacv2_unit_type_generation: bool
 
@@ -143,14 +137,16 @@
         use_self_play_reward=False,
         see_enemy_actions=True,
         won_battle_bonus=1.0,
         walls_cause_death=True,
         max_steps=100,
         smacv2_position_generation=False,
         smacv2_unit_type_generation=False,
+        observation_type="unit_list",
+        action_type="discrete",
     ) -> None:
         self.num_allies = num_allies if scenario is None else scenario.num_allies
         self.num_enemies = num_enemies if scenario is None else scenario.num_enemies
         self.num_agents = self.num_allies + self.num_enemies
         self.walls_cause_death = walls_cause_death
         self.unit_type_names = unit_type_names
         self.unit_type_shorthands = unit_type_shorthands
@@ -194,46 +190,78 @@
         )
         self.agents = [f"ally_{i}" for i in range(self.num_allies)] + [
             f"enemy_{i}" for i in range(self.num_enemies)
         ]
         self.agent_ids = {agent: i for i, agent in enumerate(self.agents)}
         self.teams = jnp.zeros((self.num_agents,), dtype=jnp.uint8)
         self.teams = self.teams.at[self.num_allies :].set(1)
+        self.observation_type = observation_type
+        self.max_units_per_section = 2
+        self.num_sections = 32
+        self.action_type = action_type
+        self.continuous_action_dims = [
+            "shoot_last_enemy",
+            "do_shoot",
+            "coordinate_1",
+            "coordinate_2",
+        ]
         self.own_features = ["health", "position_x", "position_y", "weapon_cooldown"]
         self.own_features += [f"unit_type_bit_{i}" for i in range(self.unit_type_bits)]
         self.unit_features = [
             "health",
             "position_x",
             "position_y",
-            "last_action",
+            "last_movement_x",
+            "last_movement_y",
+            "last_targeted",
             "weapon_cooldown",
         ]
         self.unit_features += [
             f"unit_type_bits_{i}" for i in range(self.unit_type_bits)
         ]
-        self.obs_size = (
-            len(self.unit_features) * (self.num_allies - 1)
-            + len(self.unit_features) * self.num_enemies
-            + len(self.own_features)
-        )
+        self.obs_size = self._get_obs_size()
         self.state_size = (len(self.own_features) + 2) * self.num_agents
         self.observation_spaces = {
             i: Box(low=0.0, high=1.0, shape=(self.obs_size,)) for i in self.agents
         }
         self.num_ally_actions = self.num_enemies + self.num_movement_actions
         self.num_enemy_actions = self.num_allies + self.num_movement_actions
         self.action_spaces = {
-            agent: Discrete(
-                num_categories=self.num_ally_actions
-                if i < self.num_allies
-                else self.num_enemy_actions
-            )
+            agent: self._get_individual_action_space(i)
             for i, agent in enumerate(self.agents)
         }
 
+    def _get_individual_action_space(self, i):
+        if self.action_type == "discrete":
+            return Discrete(
+                num_categories=(
+                    self.num_ally_actions
+                    if i < self.num_allies
+                    else self.num_enemy_actions
+                )
+            )
+        elif self.action_type == "continuous":
+            return Box(low=0.0, high=1.0, shape=(len(self.continuous_action_dims),))
+        else:
+            raise ValueError("")
+
+    def _get_obs_size(self):
+        if self.observation_type == "unit_list":
+            return (
+                len(self.unit_features) * (self.num_allies - 1)
+                + len(self.unit_features) * self.num_enemies
+                + len(self.own_features)
+            )
+        elif self.observation_type == "conic":
+            return len(self.unit_features) * (
+                self.num_sections * self.max_units_per_section
+            ) + len(self.own_features)
+        else:
+            raise ValueError("Provided observation type is not valid")
+
     @partial(jax.jit, static_argnums=(0,))
     def reset(self, key: chex.PRNGKey) -> Tuple[Dict[str, chex.Array], State]:
         """Environment-specific reset."""
         key, team_0_key, team_1_key = jax.random.split(key, num=3)
         team_0_start = jnp.stack([jnp.array([8.0, 16.0])] * self.num_allies)
         team_0_start_noise = jax.random.uniform(
             team_0_key, shape=(self.num_allies, 2), minval=-2, maxval=2
@@ -267,73 +295,98 @@
         unit_health = self.unit_type_health[unit_types]
         state = State(
             unit_positions=unit_positions,
             unit_alive=jnp.ones((self.num_agents,), dtype=jnp.bool_),
             unit_teams=unit_teams,
             unit_health=unit_health,
             unit_types=unit_types,
-            prev_actions=jnp.zeros((self.num_agents,), dtype=jnp.int32),
+            prev_movement_actions=jnp.zeros((self.num_agents, 2)),
+            prev_attack_actions=jnp.zeros((self.num_agents,), dtype=jnp.int32),
             time=0,
             terminal=False,
             unit_weapon_cooldowns=unit_weapon_cooldowns,
         )
         state = self._push_units_away(state)
         obs = self.get_obs(state)
         world_state = self.get_world_state(state)
         obs["world_state"] = jax.lax.stop_gradient(world_state)
         return obs, state
 
-    @partial(jax.jit, static_argnums=(0,))
+    @partial(jax.jit, static_argnums=(0, 4))
     def step_env(
         self,
         key: chex.PRNGKey,
         state: State,
         actions: Dict[str, chex.Array],
+        get_state_sequence: bool = False,
     ) -> Tuple[Dict[str, chex.Array], State, Dict[str, float], Dict[str, bool], Dict]:
-        """Environment-specific step transition."""
         actions = jnp.array([actions[i] for i in self.agents])
+        key, action_key = jax.random.split(key)
+        actions = self._decode_actions(action_key, state, actions)
+        return self.step_env_no_decode(key, state, actions, get_state_sequence)
+
+    @partial(jax.jit, static_argnums=(0, 4))
+    def step_env_no_decode(
+        self,
+        key: chex.PRNGKey,
+        state: State,
+        actions: Dict[str, chex.Array],
+        get_state_sequence: bool = False,
+    ) -> Tuple[Dict[str, chex.Array], State, Dict[str, float], Dict[str, bool], Dict]:
+        """Environment-specific step transition."""
+
         health_before = jnp.copy(state.unit_health)
 
         def world_step_fn(carry, _):
             state, step_key = carry
             step_key, world_step_key = jax.random.split(step_key)
             state = partial(self._world_step, actions=actions)(
                 key=world_step_key, state=state
             )
             state = self._kill_agents_touching_walls(state)
             state = self._update_dead_agents(state)
             state = self._push_units_away(state)
-            return (state, step_key), None
+            state = state.replace(
+                prev_movement_actions=actions[0],
+                prev_attack_actions=actions[1],
+            )
+            return (state, step_key), state
 
-        (state, _), _ = jax.lax.scan(
+        (state, _), states = jax.lax.scan(
             world_step_fn,
             init=(state, key),
             xs=None,
             length=self.world_steps_per_env_step,
         )
         health_after = state.unit_health
         state = state.replace(
-            terminal=self.is_terminal(state), prev_actions=actions, time=state.time + 1
+            terminal=self.is_terminal(state),
+            prev_movement_actions=actions[0],
+            prev_attack_actions=actions[1],
+            time=state.time + 1,
         )
         obs = self.get_obs(state)
         dones = {
             agent: ~state.unit_alive[self.agent_ids[agent]] for agent in self.agents
         }
         rewards = self.compute_reward(state, health_before, health_after)
         dones["__all__"] = state.terminal
         world_state = self.get_world_state(state)
         infos = {}
         obs["world_state"] = jax.lax.stop_gradient(world_state)
-        return (
-            jax.lax.stop_gradient(obs),
-            jax.lax.stop_gradient(state),
-            rewards,
-            dones,
-            infos,
-        )
+        if not get_state_sequence:
+            return (
+                jax.lax.stop_gradient(obs),
+                jax.lax.stop_gradient(state),
+                rewards,
+                dones,
+                infos,
+            )
+        else:
+            return states
 
     @partial(jax.jit, static_argnums=(0,))
     def compute_reward(self, state, health_before, health_after):
         @partial(jax.jit, static_argnums=(0,))
         def compute_team_reward(team_idx):
             # compute how much the enemy team health has decreased
             other_team_idx = jnp.logical_not(team_idx).astype(jnp.uint32)
@@ -440,27 +493,28 @@
         unit_positions = (
             state.unit_positions
             + firmness * jnp.sum(delta_matrix * overlap_term[:, :, None], axis=1) / 2
         )
         return state.replace(unit_positions=unit_positions)
 
     @partial(jax.jit, static_argnums=(0,))
-    def _world_step(
-        self,
-        key: chex.PRNGKey,
-        state: State,
-        actions: Dict[str, chex.Array],
-    ) -> Tuple[Dict[str, chex.Array], State, Dict[str, float], Dict[str, bool], Dict]:
-        def update_position(idx, action):
-            # Compute the movements slightly strangely.
-            # The velocities below are for diagonal directions
-            # because these are easier to encode as actions than the four
-            # diagonal directions. Then rotate the velocity 45
-            # degrees anticlockwise to compute the movement.
-            pos = state.unit_positions[idx]
+    def _decode_actions(
+        self, key, state: State, actions: chex.Array
+    ) -> Tuple[chex.Array, chex.Array]:
+        if self.action_type == "discrete":
+            return self._decode_discrete_actions(actions)
+        elif self.action_type == "continuous":
+            return self._decode_continuous_actions(key, state, actions)
+        else:
+            raise ValueError("Invalid Action Type")
+
+    def _decode_discrete_actions(
+        self, actions: chex.Array
+    ) -> Tuple[chex.Array, chex.Array]:
+        def _decode_movement_action(action):
             vec = jax.lax.cond(
                 # action is an attack action OR stop (action 4)
                 action >= self.num_movement_actions - 1,
                 lambda: jnp.zeros((2,)),
                 lambda: jnp.array(
                     [
                         (-1) ** (action // 2) * (1.0 / jnp.sqrt(2)),
@@ -471,46 +525,154 @@
             rotation = jnp.array(
                 [
                     [1.0 / jnp.sqrt(2), -1.0 / jnp.sqrt(2)],
                     [1.0 / jnp.sqrt(2), 1.0 / jnp.sqrt(2)],
                 ]
             )
             vec = rotation @ vec
+            return vec
+
+        movement_actions = jax.vmap(_decode_movement_action)(actions)
+        attack_actions = jnp.where(
+            actions > self.num_movement_actions - 1, actions, jnp.zeros_like(actions)
+        )
+        return movement_actions, attack_actions
+
+    @partial(jax.jit, static_argnums=(0,))
+    def _decode_continuous_actions(
+        self, key, state: State, actions: chex.Array
+    ) -> Tuple[chex.Array, chex.Array]:
+        shoot_last_idx = self.continuous_action_dims.index("shoot_last_enemy")
+        action_idx = self.continuous_action_dims.index("do_shoot")
+        theta_idx = self.continuous_action_dims.index("coordinate_2")
+        r_idx = self.continuous_action_dims.index("coordinate_1")
+        shoot_last_enemy_logits = jnp.array(
+            [
+                jnp.log(actions[:, shoot_last_idx]),
+                jnp.log(1 - actions[:, shoot_last_idx]),
+            ]
+        )
+        logits = jnp.array(
+            [jnp.log(actions[:, action_idx]), jnp.log(1 - actions[:, action_idx])]
+        )
+        move_or_shoot_key, shoot_last_enemy_key = jax.random.split(key)
+        move_or_shoot = jax.random.categorical(move_or_shoot_key, logits, axis=0)
+        shoot_last_enemy = jax.random.categorical(
+            shoot_last_enemy_key, shoot_last_enemy_logits, axis=0
+        )
+        move_angles = jnp.stack([actions[:, theta_idx] * 2 * math.pi], axis=-1)
+        # for the units that didn't move, we want to get a 0 movement vector
+        # we do this by feeding [pi / 2, 0] into [jnp.cos, jnp.sin]
+        movement_actions = jnp.stack(
+            [
+                actions[:, r_idx] * jnp.cos(move_angles[:, 0]),
+                actions[:, r_idx] * jnp.sin(move_angles[:, 1]),
+            ],
+            axis=-1,
+        )
+        movement_actions = jnp.where(
+            move_or_shoot[:, None] == 0,
+            movement_actions,
+            jnp.zeros_like(movement_actions),
+        )
+        # attack actions
+        # convert positions from polar to x-y coordinates
+        positions = jnp.stack(
+            [
+                actions[:, r_idx] * jnp.cos(actions[:, theta_idx] * 2 * math.pi),
+                actions[:, r_idx] * jnp.sin(actions[:, theta_idx] * 2 * math.pi),
+            ],
+            axis=-1,
+        )
+        positions = state.unit_positions + positions
+
+        # get the closest enemy to each of these positions
+        def get_attack_action(idx, position):
+            team = idx < self.num_allies
+            team_mask = jnp.zeros((self.num_agents,))
+            team_mask = team_mask.at[: self.num_allies].set(idx < self.num_allies)
+            team_mask = team_mask.at[self.num_allies :].set(idx >= self.num_allies)
+            dist = jnp.linalg.norm(state.unit_positions - position, axis=-1)
+            # add artificially large distance to allies so they aren't the minimum
+            dist = dist + team_mask * 1e8
+            min_dist_idx = jnp.argmin(dist)
+            # only need to check whether we have chosen to shoot at an enemy here.
+            shootable = (move_or_shoot[idx] == 1) & jnp.logical_not(
+                team_mask[min_dist_idx]
+            )
+            attack_action = jnp.where(
+                team,
+                min_dist_idx - self.num_allies,
+                self.num_allies - 1 - min_dist_idx,
+            )
+            attack_action = attack_action + self.num_movement_actions
+            attack_action = jnp.where(
+                shoot_last_enemy[idx] == 1,
+                state.prev_attack_actions[idx],
+                attack_action,
+            )
+            attack_action = jnp.where(shootable, attack_action, 0)
+            return attack_action
+
+        attack_actions = jax.vmap(get_attack_action)(
+            jnp.arange(self.num_agents), positions
+        )
+        return movement_actions, attack_actions
+
+    @partial(jax.jit, static_argnums=(0,))
+    def _world_step(
+        self,
+        key: chex.PRNGKey,
+        state: State,
+        actions: Tuple[chex.Array, chex.Array],
+    ) -> Tuple[Dict[str, chex.Array], State, Dict[str, float], Dict[str, bool], Dict]:
+        def update_position(idx, vec):
+            # Compute the movements slightly strangely.
+            # The velocities below are for diagonal directions
+            # because these are easier to encode as actions than the four
+            # diagonal directions. Then rotate the velocity 45
+            # degrees anticlockwise to compute the movement.
+            pos = state.unit_positions[idx]
             new_pos = (
                 pos
                 + vec
                 * self.unit_type_velocities[state.unit_types[idx]]
                 * self.time_per_step
             )
             # avoid going out of bounds
             new_pos = jnp.maximum(
                 jnp.minimum(new_pos, jnp.array([self.map_width, self.map_height])),
                 jnp.zeros((2,)),
             )
-            return WorldDelta(new_pos, idx, -self.time_per_step, 0.0)
+            return new_pos
 
         def update_agent_health(idx, action, key):
             # for team 1, their attack actions are labelled in
             # reverse order because that is the order they are
             # observed in
             attacked_idx = jax.lax.cond(
                 idx < self.num_allies,
                 lambda: action + self.num_allies - self.num_movement_actions,
                 lambda: self.num_allies - 1 - (action - self.num_movement_actions),
             )
+            # deal with no-op attack actions (i.e. agents that are moving instead)
+            attacked_idx = jax.lax.select(
+                action < self.num_movement_actions, idx, attacked_idx
+            )
             attack_valid = (
                 (
                     jnp.linalg.norm(
                         state.unit_positions[idx] - state.unit_positions[attacked_idx]
                     )
                     < self.unit_type_attack_ranges[state.unit_types[idx]]
                 )
                 & state.unit_alive[idx]
                 & state.unit_alive[attacked_idx]
             )
+            attack_valid = attack_valid & (idx != attacked_idx)
             attack_valid = attack_valid & (state.unit_weapon_cooldowns[idx] <= 0.0)
             health_diff = jax.lax.select(
                 attack_valid,
                 -self.unit_type_attacks[state.unit_types[idx]],
                 0.0,
             )
             # design choice based on the pysc2 randomness details.
@@ -521,53 +683,62 @@
             )
             cooldown = (
                 self.unit_type_weapon_cooldowns[state.unit_types[idx]]
                 + cooldown_deviation
             )
             cooldown_diff = jax.lax.select(
                 attack_valid,
+                # subtract the current cooldown because we are
+                # going to add it back. This way we effectively
+                # set the new cooldown to `cooldown`
                 cooldown - state.unit_weapon_cooldowns[idx],
                 -self.time_per_step,
             )
-            return WorldDelta(
-                state.unit_positions[idx],
-                attacked_idx,
-                cooldown_diff,
-                health_diff,
-            )
+            return health_diff, attacked_idx, cooldown_diff
 
         def perform_agent_action(idx, action, key):
-            return jax.lax.cond(
-                actions[idx] > self.num_movement_actions - 1,
-                lambda: update_agent_health(idx, action, key),
-                lambda: update_position(idx, action),
+            movement_action, attack_action = action
+            new_pos = update_position(idx, movement_action)
+            health_diff, attacked_idxes, cooldown_diff = update_agent_health(
+                idx, attack_action, key
             )
 
-        keys = jax.random.split(key, num=self.num_agents)
-        deltas = jax.vmap(perform_agent_action)(
-            jnp.arange(self.num_agents), actions, keys
-        )
+            return new_pos, (health_diff, attacked_idxes), cooldown_diff
 
-        def update_health(carry: chex.Array, delta: WorldDelta):
-            unit_health, unit_weapon_cooldowns, idx = carry
-            unit_health = unit_health.at[delta.attacked_idx].set(
-                jnp.maximum(unit_health[delta.attacked_idx] + delta.health_diff, 0.0)
-            )
-            unit_weapon_cooldowns = unit_weapon_cooldowns.at[idx].set(
-                state.unit_weapon_cooldowns[idx] + delta.cooldown_diff
-            )
-            return (unit_health, unit_weapon_cooldowns, idx + 1), None
-
-        # TODO, just sum the deltas and take the max w/ 0
-        (unit_health, unit_weapon_cooldowns, _), _ = jax.lax.scan(
-            update_health, (state.unit_health, state.unit_weapon_cooldowns, 0), deltas
+        keys = jax.random.split(key, num=self.num_agents)
+        pos, (health_diff, attacked_idxes), cooldown_diff = jax.vmap(
+            perform_agent_action
+        )(jnp.arange(self.num_agents), actions, keys)
+        # Multiple enemies can attack the same unit.
+        # We have `(health_diff, attacked_idx)` pairs.
+        # `jax.lax.scatter_add` aggregates these exactly
+        # in the way we want -- duplicate idxes will have their
+        # health differences added together. However, it is a
+        # super thin wrapper around the XLA scatter operation,
+        # which has this bonkers syntax and requires this dnums
+        # parameter. The usage here was inferred from a test:
+        # https://github.com/google/jax/blob/main/tests/lax_test.py#L2296
+        dnums = jax.lax.ScatterDimensionNumbers(
+            update_window_dims=(),
+            inserted_window_dims=(0,),
+            scatter_dims_to_operand_dims=(0,),
+        )
+        unit_health = jnp.maximum(
+            jax.lax.scatter_add(
+                state.unit_health,
+                jnp.expand_dims(attacked_idxes, 1),
+                health_diff,
+                dnums,
+            ),
+            0.0,
         )
+        unit_weapon_cooldowns = state.unit_weapon_cooldowns + cooldown_diff
         state = state.replace(
             unit_health=unit_health,
-            unit_positions=deltas.pos,
+            unit_positions=pos,
             unit_weapon_cooldowns=unit_weapon_cooldowns,
         )
         return state
 
     def get_world_state(self, state: State) -> chex.Array:
         # get the features of every unit, as well as the teams that they belong to.
         def get_features(i):
@@ -584,85 +755,156 @@
 
         get_all_features = jax.vmap(get_features)
         unit_obs = get_all_features(jnp.arange(self.num_agents)).reshape(-1)
         unit_teams = state.unit_teams
         unit_types = state.unit_types
         return jnp.concatenate([unit_obs, unit_teams, unit_types], axis=-1)
 
+    @partial(jax.jit, static_argnums=(0,))
     def get_obs(self, state: State) -> Dict[str, chex.Array]:
+        if self.observation_type == "unit_list":
+            return self.get_obs_unit_list(state)
+        elif self.observation_type == "conic":
+            return self.get_obs_conic(state)
+
+    def get_obs_conic(self, state: State) -> Dict[str, chex.Array]:
+        def get_features(i: int):
+            relative_pos = (
+                state.unit_positions - state.unit_positions[i]
+            ) / self.unit_type_sight_ranges[state.unit_types[i]]
+            visible = jnp.linalg.norm(relative_pos, axis=-1) < 1
+
+            def get_segment(j: int):
+                #
+                angle = (
+                    jnp.arctan(relative_pos[:, 1] / (relative_pos[:, 0] + 1e-8))
+                    + (relative_pos[:, 0] < 0)
+                    * (2 * (relative_pos[:, 1] > 0) - 1)
+                    * math.pi
+                )
+                min_segment_angle = (2 * math.pi) * (j / self.num_sections) - math.pi
+                max_segment_angle = (2 * math.pi) * (
+                    (j + 1) / self.num_sections
+                ) - math.pi
+                self_mask = jnp.zeros((self.num_agents,)).at[i].set(1)
+                in_range_mask = (
+                    (angle > min_segment_angle)
+                    & (angle < max_segment_angle)
+                    & visible
+                    & jnp.logical_not(self_mask)
+                )
+                idxes = jnp.nonzero(
+                    in_range_mask * jnp.arange(self.num_agents),
+                    size=self.max_units_per_section,
+                    fill_value=-1,
+                )[0]
+                features = jax.vmap(self._observe_features, in_axes=(None, None, 0))(
+                    state, i, idxes
+                )
+                empty_features = jnp.zeros_like(features)
+                features = jnp.where(
+                    ((idxes == -1) | jnp.logical_not(state.unit_alive[i]))[:, None],
+                    empty_features,
+                    features,
+                )
+                # observe these indexes
+                return features
+
+            all_segment_features = jax.vmap(get_segment)(jnp.arange(self.num_sections))
+            own_features = self._get_own_features(state, i)
+            return jnp.concatenate(
+                [all_segment_features.reshape(-1), own_features], axis=-1
+            )
+
+        obs = jax.vmap(get_features)(jnp.arange(self.num_agents))
+        return {agent: obs[self.agent_ids[agent]] for agent in self.agents}
+
+    @partial(jax.jit, static_argnums=(0,))
+    def _observe_features(self, state: State, i: int, j_idx: int):
+        team_i_idx = (i >= self.num_allies).astype(jnp.int32)
+        team_j_idx = (j_idx >= self.num_allies).astype(jnp.int32)
+        empty_features = jnp.zeros(shape=(len(self.unit_features),))
+        features = empty_features.at[0].set(
+            state.unit_health[j_idx] / self.unit_type_health[state.unit_types[j_idx]]
+        )
+        features = features.at[1:3].set(
+            (state.unit_positions[j_idx] - state.unit_positions[i])
+            / self.unit_type_sight_ranges[state.unit_types[i]]
+        )
+        move_action_obs = jax.lax.select(
+            (team_i_idx == team_j_idx) | self.see_enemy_actions,
+            state.prev_movement_actions[j_idx],
+            jnp.zeros((2,)),
+        )
+        attack_action_obs = jax.lax.select(
+            (team_i_idx == team_j_idx) | self.see_enemy_actions,
+            state.prev_attack_actions[j_idx],
+            0,
+        )
+        features = features.at[3:5].set(move_action_obs)
+        features = features.at[5].set(attack_action_obs)
+        features = features.at[6].set(state.unit_weapon_cooldowns[j_idx])
+        features = features.at[7 + state.unit_types[j_idx]].set(1)
+        return features
+
+    @partial(jax.jit, static_argnums=(0,))
+    def _get_own_features(self, state: State, i: int):
+        empty_features = jnp.zeros(shape=(len(self.own_features),))
+        features = empty_features.at[0].set(
+            state.unit_health[i] / self.unit_type_health[state.unit_types[i]]
+        )
+        features = features.at[1:3].set(
+            state.unit_positions[i] / jnp.array([self.map_width, self.map_height])
+        )
+        features = features.at[3].set(state.unit_weapon_cooldowns[i])
+        features = features.at[4 + state.unit_types[i]].set(1)
+        return jax.lax.cond(
+            state.unit_alive[i], lambda: features, lambda: empty_features
+        )
+
+    def get_obs_unit_list(self, state: State) -> Dict[str, chex.Array]:
         """Applies observation function to state."""
-        actions = state.prev_actions
 
         def get_features(i, j):
             """Get features of unit j as seen from unit i"""
             # Can just keep them symmetrical for now.
             # j here means 'the jth unit that is not i'
             # The observation is such that allies are always first
             # so for units in the second team we count in reverse.
-            team_i_idx = (i >= self.num_allies).astype(jnp.int32)
             j = jax.lax.cond(
                 i < self.num_allies,
                 lambda: j,
                 lambda: self.num_agents - j - 1,
             )
             offset = jax.lax.cond(i < self.num_allies, lambda: 1, lambda: -1)
             j_idx = jax.lax.cond(
                 ((j < i) & (i < self.num_allies)) | ((j > i) & (i >= self.num_allies)),
                 lambda: j,
                 lambda: j + offset,
             )
-            team_j_idx = (j_idx >= self.num_allies).astype(jnp.int32)
             empty_features = jnp.zeros(shape=(len(self.unit_features),))
-            features = empty_features.at[0].set(
-                state.unit_health[j_idx]
-                / self.unit_type_health[state.unit_types[j_idx]]
-            )
-            features = features.at[1:3].set(
-                (state.unit_positions[j_idx] - state.unit_positions[i])
-                / self.unit_type_sight_ranges[state.unit_types[i]]
-            )
-            # TODO encode as one hot?
-            action_obs = jax.lax.select(
-                (team_i_idx == team_j_idx) | self.see_enemy_actions, actions[j_idx], 0
-            )
-            features = features.at[3].set(action_obs)
-            features = features.at[4].set(state.unit_weapon_cooldowns[j_idx])
-            features = features.at[5 + state.unit_types[j_idx]].set(1)
+            features = self._observe_features(state, i, j_idx)
             visible = (
                 jnp.linalg.norm(state.unit_positions[j_idx] - state.unit_positions[i])
                 < self.unit_type_sight_ranges[state.unit_types[i]]
             )
             return jax.lax.cond(
                 visible & state.unit_alive[i] & state.unit_alive[j_idx],
                 lambda: features,
                 lambda: empty_features,
             )
 
-        def get_self_features(i):
-            empty_features = jnp.zeros(shape=(len(self.own_features),))
-            features = empty_features.at[0].set(
-                state.unit_health[i] / self.unit_type_health[state.unit_types[i]]
-            )
-            features = features.at[1:3].set(
-                state.unit_positions[i] / jnp.array([self.map_width, self.map_height])
-            )
-            features = features.at[3].set(state.unit_weapon_cooldowns[i])
-            features = features.at[4 + state.unit_types[i]].set(1)
-            return jax.lax.cond(
-                state.unit_alive[i], lambda: features, lambda: empty_features
-            )
-
         get_all_features_for_unit = jax.vmap(get_features, in_axes=(None, 0))
         get_all_features = jax.vmap(get_all_features_for_unit, in_axes=(0, None))
         other_unit_obs = get_all_features(
             jnp.arange(self.num_agents), jnp.arange(self.num_agents - 1)
         )
         other_unit_obs = other_unit_obs.reshape((self.num_agents, -1))
-        get_all_self_features = jax.vmap(get_self_features)
-        own_unit_obs = get_all_self_features(jnp.arange(self.num_agents))
+        get_all_self_features = jax.vmap(self._get_own_features, in_axes=(None, 0))
+        own_unit_obs = get_all_self_features(state, jnp.arange(self.num_agents))
         obs = jnp.concatenate([other_unit_obs, own_unit_obs], axis=-1)
         return {agent: obs[self.agent_ids[agent]] for agent in self.agents}
 
     @partial(jax.jit, static_argnums=(0,))
     def get_avail_actions(self, state: State) -> Dict[str, chex.Array]:
         @partial(jax.jit, static_argnums=(1,))
         def get_individual_avail_actions(i, team):
@@ -697,32 +939,32 @@
         ally_avail_actions_masks = jax.vmap(
             get_individual_avail_actions, in_axes=(0, None)
         )(jnp.arange(self.num_allies), 0)
         enemy_avail_actions_masks = jax.vmap(
             get_individual_avail_actions, in_axes=(0, None)
         )(jnp.arange(self.num_allies, self.num_agents), 1)
         return {
-            agent: ally_avail_actions_masks[i]
-            if i < self.num_allies
-            else enemy_avail_actions_masks[i - self.num_allies]
+            agent: (
+                ally_avail_actions_masks[i]
+                if i < self.num_allies
+                else enemy_avail_actions_masks[i - self.num_allies]
+            )
             for i, agent in enumerate(self.agents)
         }
 
     def expand_state_seq(self, state_seq):
         expanded_state_seq = []
         for key, state, actions in state_seq:
-            agents = self.agents
-            for _ in range(self.world_steps_per_env_step):
-                expanded_state_seq.append((key, state, actions))
-                world_actions = jnp.array([actions[i] for i in agents])
-                key, step_key = jax.random.split(key)
-                state = self._world_step(step_key, state, world_actions)
-                state = self._kill_agents_touching_walls(state)
-                state = self._update_dead_agents(state)
-                state = self._push_units_away(state)
+            states = self.step_env(key, state, actions, get_state_sequence=True)
+            states = list(map(State, *dataclasses.astuple(states)))
+            viz_actions = {agent: states[0].prev_attack_actions[i] for i, agent in enumerate(self.agents)}
+            expanded_state_seq.extend(
+                zip([key] * len(states), states, [viz_actions] * len(states))
+            )
+
             state = state.replace(terminal=self.is_terminal(state))
         return expanded_state_seq
 
     def init_render(
         self,
         ax,
         state: Tuple[State, Dict],
```

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/smax/speed.py` & `jaxmarl-0.0.3/jaxmarl/environments/smax/speed.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/spaces.py` & `jaxmarl-0.0.3/jaxmarl/environments/spaces.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/storm/rendering.py` & `jaxmarl-0.0.3/jaxmarl/environments/storm/rendering.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/storm/storm_2p.py` & `jaxmarl-0.0.3/jaxmarl/environments/storm/storm_2p.py`

 * *Files 1% similar despite different names*

```diff
@@ -747,25 +747,27 @@
                 ),
             )
 
             # now calculate if done for inner or outer episode
             inner_t = state_nxt.inner_t
             outer_t = state_nxt.outer_t
             reset_inner = inner_t == num_inner_steps
-            done = {}
-            done["__all__"] = reset_inner = inner_t == num_inner_steps
 
             # if inner episode is done, return start state for next game
-            # state_re = _reset_state(key)
-            # state_re = state_re.replace(outer_t=outer_t + 1)
-            # state = jax.tree_map(
-            #     lambda x, y: jax.lax.select(reset_inner, x, y),
-            #     state_re,
-            #     state_nxt,
-            # )
+            state_re = _reset_state(key)
+            state_re = state_re.replace(outer_t=outer_t + 1)
+            state = jax.tree_map(
+                lambda x, y: jax.lax.select(reset_inner, x, y),
+                state_re,
+                state_nxt,
+            )
+            outer_t = state.outer_t
+            reset_outer = outer_t == num_outer_steps
+            done = {}
+            done["__all__"] = reset_outer
 
             obs = _get_obs(state)
             blue_reward = jnp.where(reset_inner, 0, blue_reward)
             red_reward = jnp.where(reset_inner, 0, red_reward)
             return (
                 obs,
                 state,
```

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/storm/storm_env.py` & `jaxmarl-0.0.3/jaxmarl/environments/storm/storm_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -882,26 +882,28 @@
                 coin_timer_coop=state.coin_timer_coop,
                 coin_timer_defect=state.coin_timer_defect,
             )
 
             # now calculate if done for inner or outer episode
             inner_t = state_nxt.inner_t
             outer_t = state_nxt.outer_t
-            done = {}
-            done["__all__"] = reset_inner = inner_t == num_inner_steps
-
+            reset_inner = inner_t == num_inner_steps
 
             # # # if inner episode is done, return start state for next game
-            # state_re = _reset_state(key)
-            # state_re = state_re.replace(outer_t=outer_t + 1)
-            # state = jax.tree_map(
-            #     lambda x, y: jax.lax.select(reset_inner, x, y),
-            #     state_re,
-            #     state_nxt,
-            # )
+            state_re = _reset_state(key)
+            state_re = state_re.replace(outer_t=outer_t + 1)
+            state = jax.tree_map(
+                lambda x, y: jax.lax.select(reset_inner, x, y),
+                state_re,
+                state_nxt,
+            )
+            outer_t = state.outer_t
+            reset_outer = outer_t == num_outer_steps
+            done = {}
+            done["__all__"] = reset_outer
 
             obs = _get_obs(state)
             rewards = jnp.where(reset_inner, 0, rewards)
 
             return (
                 obs,
                 state,
```

### Comparing `jaxmarl-0.0.2/jaxmarl/environments/switch_riddle/switch_riddle.py` & `jaxmarl-0.0.3/jaxmarl/environments/switch_riddle/switch_riddle.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/gridworld/common.py` & `jaxmarl-0.0.3/jaxmarl/gridworld/common.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/gridworld/env.py` & `jaxmarl-0.0.3/jaxmarl/gridworld/env.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/gridworld/grid_viz.py` & `jaxmarl-0.0.3/jaxmarl/gridworld/grid_viz.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/gridworld/interactive.py` & `jaxmarl-0.0.3/jaxmarl/gridworld/interactive.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/gridworld/ma_maze.py` & `jaxmarl-0.0.3/jaxmarl/gridworld/ma_maze.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/gridworld/maze.py` & `jaxmarl-0.0.3/jaxmarl/gridworld/maze.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/gridworld/tabular_q.py` & `jaxmarl-0.0.3/jaxmarl/gridworld/tabular_q.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/registration.py` & `jaxmarl-0.0.3/jaxmarl/registration.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Ant,
     Humanoid,
     Hopper,
     Walker2d,
     HalfCheetah,
     InTheGrid,
     InTheGrid_2p,
-    HanabiGame,
+    Hanabi,
     Overcooked,
     CoinGame,
 )
 
 
 
 def make(env_id: str, **env_kwargs):
@@ -72,15 +72,15 @@
         env = SMAX(**env_kwargs)
     elif env_id == "HeuristicEnemySMAX":
         env = HeuristicEnemySMAX(**env_kwargs)
     elif env_id == "LearnedPolicyEnemySMAX":
         env = LearnedPolicyEnemySMAX(**env_kwargs)
 
     # 4. MABrax
-    elif env_id == "ant_4x2":
+    if env_id == "ant_4x2":
         env = Ant(**env_kwargs)
     elif env_id == "halfcheetah_6x1":
         env = HalfCheetah(**env_kwargs)
     elif env_id == "hopper_3x1":
         env = Hopper(**env_kwargs)
     elif env_id == "humanoid_9|8":
         env = Humanoid(**env_kwargs)
@@ -92,15 +92,15 @@
         env = InTheGrid(**env_kwargs)
     # 5. InTheGrid
     elif env_id == "storm_2p":
         env = InTheGrid_2p(**env_kwargs)
     
     # 6. Hanabi
     elif env_id == "hanabi":
-        env = HanabiGame(**env_kwargs)
+        env = Hanabi(**env_kwargs)
 
     # 7. Overcooked
     elif env_id == "overcooked":
         env = Overcooked(**env_kwargs)
 
     # 8. Coin Game
     elif env_id == "coin_game":
```

### Comparing `jaxmarl-0.0.2/jaxmarl/viz/grid_rendering.py` & `jaxmarl-0.0.3/jaxmarl/viz/grid_rendering.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/viz/overcooked_visualizer.py` & `jaxmarl-0.0.3/jaxmarl/viz/overcooked_visualizer.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/viz/visualizer.py` & `jaxmarl-0.0.3/jaxmarl/viz/visualizer.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/viz/window.py` & `jaxmarl-0.0.3/jaxmarl/viz/window.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl/wrappers/gymnax.py` & `jaxmarl-0.0.3/jaxmarl/wrappers/gymnax.py`

 * *Files identical despite different names*

### Comparing `jaxmarl-0.0.2/jaxmarl.egg-info/SOURCES.txt` & `jaxmarl-0.0.3/jaxmarl.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,30 @@
 LICENSE
 MANIFEST.in
 README.md
-setup.py
-baselines/IPPO/__init__.py
-baselines/IPPO/ippo_ff_hanabi.py
-baselines/IPPO/ippo_mabrax.py
-baselines/IPPO/ippo_mlp_hanabi.py
-baselines/IPPO/ippo_mpe.py
-baselines/IPPO/ippo_mpe_facmac.py
-baselines/IPPO/ippo_overcooked.py
-baselines/IPPO/ippo_rnn_hanabi.py
-baselines/IPPO/ippo_rnn_mpe.py
-baselines/IPPO/ippo_rnn_smax.py
-baselines/IPPO/ippo_switch_riddle.py
-baselines/QLearning/__init__.py
-baselines/QLearning/iql.py
-baselines/QLearning/qmix.py
-baselines/QLearning/qmix_pretrained.py
-baselines/QLearning/utils.py
-baselines/QLearning/vdn.py
-baselines/QLearning/buffers/__init__.py
-baselines/QLearning/buffers/base.py
-baselines/QLearning/buffers/circular_buffer.py
-baselines/QLearning/buffers/clustered.py
-baselines/QLearning/buffers/uniform.py
-baselines/QLearning/buffers/utils.py
+pyproject.toml
 jaxmarl/__init__.py
-jaxmarl/_version.py
 jaxmarl/registration.py
 jaxmarl.egg-info/PKG-INFO
 jaxmarl.egg-info/SOURCES.txt
 jaxmarl.egg-info/dependency_links.txt
-jaxmarl.egg-info/not-zip-safe
 jaxmarl.egg-info/requires.txt
 jaxmarl.egg-info/top_level.txt
 jaxmarl/environments/__init__.py
 jaxmarl/environments/multi_agent_env.py
 jaxmarl/environments/spaces.py
 jaxmarl/environments/coin_game/__init__.py
 jaxmarl/environments/coin_game/coin_game.py
 jaxmarl/environments/hanabi/__init__.py
 jaxmarl/environments/hanabi/hanabi.py
+jaxmarl/environments/hanabi/hanabi_game.py
+jaxmarl/environments/hanabi/manual_game.py
+jaxmarl/environments/hanabi/pretrained/__init__.py
+jaxmarl/environments/hanabi/pretrained/obl_r2d2_agent.py
+jaxmarl/environments/hanabi/pretrained/obl_r2d2_agent_test.py
 jaxmarl/environments/mabrax/__init__.py
 jaxmarl/environments/mabrax/mabrax_env.py
 jaxmarl/environments/mabrax/mappings.py
 jaxmarl/environments/mpe/__init__.py
 jaxmarl/environments/mpe/default_params.py
 jaxmarl/environments/mpe/mpe_visualizer.py
 jaxmarl/environments/mpe/simple.py
@@ -78,17 +58,22 @@
 jaxmarl/gridworld/common.py
 jaxmarl/gridworld/env.py
 jaxmarl/gridworld/grid_viz.py
 jaxmarl/gridworld/interactive.py
 jaxmarl/gridworld/ma_maze.py
 jaxmarl/gridworld/maze.py
 jaxmarl/gridworld/tabular_q.py
+jaxmarl/tutorials/mpe_introduction.py
+jaxmarl/tutorials/overcooked_introduction.py
+jaxmarl/tutorials/smax_introduction.py
+jaxmarl/tutorials/storm_2p_introduction.py
+jaxmarl/tutorials/storm_introduction.py
 jaxmarl/viz/__init__.py
 jaxmarl/viz/grid_rendering.py
 jaxmarl/viz/overcooked_visualizer.py
 jaxmarl/viz/visualizer.py
 jaxmarl/viz/window.py
 jaxmarl/wrappers/__init__.py
 jaxmarl/wrappers/baselines.py
 jaxmarl/wrappers/gymnax.py
-requirements/requirements-dev.txt
+jaxmarl/wrappers/transformers.py
 requirements/requirements.txt
```

