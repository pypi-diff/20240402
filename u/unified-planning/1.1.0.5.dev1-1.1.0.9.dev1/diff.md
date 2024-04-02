# Comparing `tmp/unified_planning-1.1.0.5.dev1.tar.gz` & `tmp/unified_planning-1.1.0.9.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unified_planning-1.1.0.5.dev1.tar", last modified: Thu Mar 14 13:45:37 2024, max compression
+gzip compressed data, was "unified_planning-1.1.0.9.dev1.tar", last modified: Thu Mar 14 13:58:09 2024, max compression
```

## Comparing `unified_planning-1.1.0.5.dev1.tar` & `unified_planning-1.1.0.9.dev1.tar`

### file list

```diff
@@ -1,472 +1,472 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.758866 unified_planning-1.1.0.5.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-14 13:45:37.758866 unified_planning-1.1.0.5.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 13:45:37.758866 unified_planning-1.1.0.5.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.706866 unified_planning-1.1.0.5.dev1/unified_planning/
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.706866 unified_planning-1.1.0.5.dev1/unified_planning/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/cmd/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/cmd/up.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.710866 unified_planning-1.1.0.5.dev1/unified_planning/engines/
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.710866 unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/bounded_types_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/compilers_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)    19659 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)    20545 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/grounder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/ma_conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/ma_disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)    18039 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/negative_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)    14661 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/quantifiers_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     8645 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/state_invariants_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/tarski_grounder.py
--rw-r--r--   0 runner    (1001) docker     (127)    19971 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)    30421 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)    20883 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/credits.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    50392 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/meta_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.714866 unified_planning-1.1.0.5.dev1/unified_planning/engines/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/mixins/anytime_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/mixins/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/mixins/oneshot_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/mixins/plan_repairer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/mixins/plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/mixins/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/mixins/replanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9817 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/mixins/sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/oversubscription_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/pddl_anytime_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)    18533 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/pddl_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)    26835 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/replanner.py
--rw-r--r--   0 runner    (1001) docker     (127)    13174 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    36012 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/engines/sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.714866 unified_planning-1.1.0.5.dev1/unified_planning/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/grpc/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.714866 unified_planning-1.1.0.5.dev1/unified_planning/grpc/generated/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/grpc/generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21733 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/grpc/generated/unified_planning_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    39061 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/grpc/proto_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    39191 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/grpc/proto_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.714866 unified_planning-1.1.0.5.dev1/unified_planning/interop/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/interop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17397 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/interop/from_tarski.py
--rw-r--r--   0 runner    (1001) docker     (127)    18137 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/interop/to_tarski.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.714866 unified_planning-1.1.0.5.dev1/unified_planning/io/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16387 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/io/anml_grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)    46716 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/io/anml_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    19419 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/io/anml_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    43626 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/io/ma_pddl_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    78731 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/io/pddl_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    41392 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/io/pddl_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.718866 unified_planning-1.1.0.5.dev1/unified_planning/model/
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/abstract_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)    29564 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/contingent_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/delta_stn.py
--rw-r--r--   0 runner    (1001) docker     (127)    18666 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/effect.py
--rw-r--r--   0 runner    (1001) docker     (127)    28821 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/fluent.py
--rw-r--r--   0 runner    (1001) docker     (127)    17991 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/fnode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.718866 unified_planning-1.1.0.5.dev1/unified_planning/model/htn/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/htn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/htn/hierarchical_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/htn/method.py
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/htn/ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/htn/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/htn/task_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    13510 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.722866 unified_planning-1.1.0.5.dev1/unified_planning/model/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/mixins/actions_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/mixins/agents_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/mixins/fluents_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/mixins/initial_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/mixins/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/mixins/objects_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/mixins/time_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16467 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/mixins/timed_conds_effs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/mixins/user_types_set.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.722866 unified_planning-1.1.0.5.dev1/unified_planning/model/multi_agent/
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/multi_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12318 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/multi_agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/multi_agent/ma_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    19673 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/multi_agent/ma_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    56259 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/problem.py
--rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/problem_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/problem_kind_versioning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.722866 unified_planning-1.1.0.5.dev1/unified_planning/model/scheduling/
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/scheduling/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/scheduling/chronicle.py
--rw-r--r--   0 runner    (1001) docker     (127)    16483 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/scheduling/scheduling_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.722866 unified_planning-1.1.0.5.dev1/unified_planning/model/tamp/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/tamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/tamp/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/tamp/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/tamp/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/tamp/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/type_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.726866 unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/any.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/dnf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/fluents_substituter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/free_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/identitydag.py
--rw-r--r--   0 runner    (1001) docker     (127)     8838 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/linear_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/names_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/operators_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/quantifier_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    17364 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/simplifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/state_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/substituter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13983 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/type_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    24752 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/usertype_fluents_walker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.726866 unified_planning-1.1.0.5.dev1/unified_planning/plans/
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/plans/contingent_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8543 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/plans/hierarchical_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/plans/partial_order_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/plans/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/plans/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/plans/sequential_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    22033 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/plans/stn_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    20775 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/plans/time_triggered_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.726866 unified_planning-1.1.0.5.dev1/unified_planning/plot/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/plot/causal_graph_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    36257 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/plot/plan_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/plot/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    30976 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.734866 unified_planning-1.1.0.5.dev1/unified_planning/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.734866 unified_planning-1.1.0.5.dev1/unified_planning/test/anml/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/anml/basic.anml
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/anml/basic_conditional.anml
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/anml/connected_locations.anml
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/anml/constants.anml
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/anml/constants_no_variable_duration.anml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/anml/durative_goals.anml
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/anml/forall.anml
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/anml/hydrone.anml
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/anml/match.anml
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/anml/match_int_id.anml
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/anml/match_test_parser.anml
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/anml/safe_road.anml
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/anml/simple_mais.anml
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/anml/tils.anml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.698866 unified_planning-1.1.0.5.dev1/unified_planning/test/contingent_pddl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.734866 unified_planning-1.1.0.5.dev1/unified_planning/test/contingent_pddl/colorballs/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.734866 unified_planning-1.1.0.5.dev1/unified_planning/test/contingent_pddl/logistic_conf/
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.738866 unified_planning-1.1.0.5.dev1/unified_planning/test/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/examples/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (127)    18623 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/examples/minimals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13662 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/examples/multi_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    48848 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/examples/realistic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.738866 unified_planning-1.1.0.5.dev1/unified_planning/test/examples/scheduling/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/examples/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/examples/scheduling/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/examples/scheduling/jobshop.py
--rw-r--r--   0 runner    (1001) docker     (127)    14189 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/examples/tamp.py
--rw-r--r--   0 runner    (1001) docker     (127)    37854 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/examples/testing_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.702866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.738866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/
--rw-r--r--   0 runner    (1001) docker     (127)    34291 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.738866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/
--rw-r--r--   0 runner    (1001) docker     (127)    33635 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.738866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-PCP/
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-PCP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.738866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Rover/
--rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.738866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Satellite/
--rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.738866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Transport/
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.738866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/
--rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.738866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.738866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.738866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Childsnack/
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.742866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Depots/
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.742866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/
--rw-r--r--   0 runner    (1001) docker     (127)    10943 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.742866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Entertainment/
--rw-r--r--   0 runner    (1001) docker     (127)    18218 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.742866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Factories-simple/
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.742866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Hiking/
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.742866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/
--rw-r--r--   0 runner    (1001) docker     (127)    17213 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.742866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/
--rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)   189505 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.742866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)    11322 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.742866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/
--rw-r--r--   0 runner    (1001) docker     (127)    33123 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.742866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/
--rw-r--r--   0 runner    (1001) docker     (127)    36329 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)    12941 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.742866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.742866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Robot/
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Robot/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.742866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/
--rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.746866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.746866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Snake/
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.746866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Towers/
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Towers/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.746866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Transport/
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.746866 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Woodworking/
--rw-r--r--   0 runner    (1001) docker     (127)    34612 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.746866 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.746866 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/citycar/
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/citycar/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/citycar/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.746866 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/counters/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/counters/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/counters/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/counters/problem2.pddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.746866 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/depot/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/depot/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/depot/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/enhsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.746866 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/htn-transport/
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/htn-transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/htn-transport/problem.hddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.746866 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/matchcellar/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/matchcellar/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/matchcellar/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.746866 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/miconic/
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/miconic/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/miconic/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.746866 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/robot_fastener/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/robot_fastener/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.746866 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/safe_road/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/safe_road/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/safe_road/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.746866 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/sailing/
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/sailing/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/sailing/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.750866 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/tpp_metric/
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/tpp_metric/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/tpp_metric/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.750866 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/visit_precedence/
--rwxr-xr-x   0 runner    (1001) docker     (127)      555 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/visit_precedence/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (127)    31240 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_anml_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_anml_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_anytime.py
--rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_bounded_types_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_compilers_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_compilers_quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_contingent_pddl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)    13289 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_dnf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_expression_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    17139 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_grounder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_htn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_infix_notation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_ma_conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_ma_disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)    18052 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_multi_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_negative_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_partial_order_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    35427 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_pddl_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_pddl_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15243 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)    25272 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_problem_kind_versioning.py
--rw-r--r--   0 runner    (1001) docker     (127)    19040 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_protobuf_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_pyperplan.py
--rw-r--r--   0 runner    (1001) docker     (127)    12150 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_quantifier_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_replanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_scheduling.py
--rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    25494 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_simulated_effects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_state_invariants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_stn_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_substituter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_tamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_tarski_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_tarski_grounder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_temporal.py
--rw-r--r--   0 runner    (1001) docker     (127)    13103 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_trajectory_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_trajectory_constraints_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_ttp_to_stn.py
--rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_usertype_fluents_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/test/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/unified_planning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.706866 unified_planning-1.1.0.5.dev1/unified_planning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-14 13:45:37.000000 unified_planning-1.1.0.5.dev1/unified_planning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17775 2024-03-14 13:45:37.000000 unified_planning-1.1.0.5.dev1/unified_planning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 13:45:37.000000 unified_planning-1.1.0.5.dev1/unified_planning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-14 13:45:37.000000 unified_planning-1.1.0.5.dev1/unified_planning.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-14 13:45:37.000000 unified_planning-1.1.0.5.dev1/unified_planning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-14 13:45:37.000000 unified_planning-1.1.0.5.dev1/unified_planning.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.750866 unified_planning-1.1.0.5.dev1/up_test_cases/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.750866 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.750866 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/classical/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/classical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/classical/basic_problems.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.750866 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/classical/depots/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/classical/depots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/classical/metric_problems.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.750866 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/classical/tpp/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/classical/tpp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.750866 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/hierarchical/
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/hierarchical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.750866 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/multiagent/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/multiagent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8495 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/multiagent/depot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/multiagent/logistic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/multiagent/ma_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    13165 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/multiagent/procter_and_gamble.py
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/multiagent/taxi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.750866 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/block_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/complex_linear_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/complex_nonlinear_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/constant_additive_effects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.750866 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/depots/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/depots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/farmlands/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/farmlands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/fn_counters/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/fn_counters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/linear_effects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/nonlinear_effects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/plant_watering/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/plant_watering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/problem_basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/rovers/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/rovers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/sailing/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/sailing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/simple_linear_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/simple_nonlinear_conditions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/tamp/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/tamp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/tamp/construction/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/tamp/construction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/tamp/construction/test_01.py
--rw-r--r--   0 runner    (1001) docker     (127)     7877 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/tamp/construction/test_02.py
--rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/tamp/construction/test_03.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/tamp/office/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/tamp/office/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/tamp/office/test_01.py
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/tamp/office/test_02.py
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/tamp/office/test_03.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/temporal/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/temporal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/temporal/depot/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/builtin/temporal/depot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/performance/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/performance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/performance/classical/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/performance/classical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/performance/classical/depots/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/performance/classical/depots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/performance/classical/tpp/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/performance/classical/tpp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/performance/numeric/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/performance/numeric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/performance/numeric/block_grouping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/performance/numeric/depots/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/performance/numeric/depots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/performance/numeric/farmlands/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/performance/numeric/farmlands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/performance/numeric/fn_counters/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/performance/numeric/fn_counters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/performance/numeric/plant_watering/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/performance/numeric/plant_watering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/performance/numeric/rovers/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/performance/numeric/rovers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/performance/numeric/sailing/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/performance/numeric/sailing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/performance/temporal/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/performance/temporal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:45:37.754866 unified_planning-1.1.0.5.dev1/up_test_cases/performance/temporal/depot/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/performance/temporal/depot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30011 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-03-14 13:45:32.000000 unified_planning-1.1.0.5.dev1/up_test_cases/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.928569 unified_planning-1.1.0.9.dev1/unified_planning/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.932569 unified_planning-1.1.0.9.dev1/unified_planning/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/cmd/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/cmd/up.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.932569 unified_planning-1.1.0.9.dev1/unified_planning/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.936569 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/bounded_types_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/compilers_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19659 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20545 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/grounder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/ma_conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/ma_disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18039 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/negative_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14661 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/quantifiers_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8645 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/state_invariants_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/tarski_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19971 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30421 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20883 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50392 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/meta_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.936569 unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/anytime_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/oneshot_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/plan_repairer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/replanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9817 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/oversubscription_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/pddl_anytime_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18031 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/pddl_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26835 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/replanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13174 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36012 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/engines/sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.936569 unified_planning-1.1.0.9.dev1/unified_planning/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/grpc/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.936569 unified_planning-1.1.0.9.dev1/unified_planning/grpc/generated/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/grpc/generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21733 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/grpc/generated/unified_planning_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39061 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/grpc/proto_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39191 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/grpc/proto_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.940569 unified_planning-1.1.0.9.dev1/unified_planning/interop/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/interop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17397 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/interop/from_tarski.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18137 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/interop/to_tarski.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.940569 unified_planning-1.1.0.9.dev1/unified_planning/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16387 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/io/anml_grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46716 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/io/anml_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19419 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/io/anml_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41221 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/io/ma_pddl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78448 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/io/pddl_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45266 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/io/pddl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.944569 unified_planning-1.1.0.9.dev1/unified_planning/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/abstract_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29564 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/contingent_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/delta_stn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18666 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28821 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/fluent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17991 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/fnode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.944569 unified_planning-1.1.0.9.dev1/unified_planning/model/htn/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/htn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/htn/hierarchical_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/htn/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/htn/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/htn/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/htn/task_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13510 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.948569 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/actions_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/agents_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/fluents_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/initial_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/objects_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/time_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16467 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/timed_conds_effs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/user_types_set.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.948569 unified_planning-1.1.0.9.dev1/unified_planning/model/multi_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/multi_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12318 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/multi_agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/multi_agent/ma_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19673 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/multi_agent/ma_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56259 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/problem_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/problem_kind_versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.948569 unified_planning-1.1.0.9.dev1/unified_planning/model/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/scheduling/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/scheduling/chronicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16483 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/scheduling/scheduling_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.948569 unified_planning-1.1.0.9.dev1/unified_planning/model/tamp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/tamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/tamp/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/tamp/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/tamp/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/tamp/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/type_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.952569 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/any.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/dnf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/fluents_substituter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/free_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/identitydag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8838 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/linear_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/names_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/operators_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/quantifier_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17364 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/state_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/substituter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13983 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24752 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/usertype_fluents_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.952569 unified_planning-1.1.0.9.dev1/unified_planning/plans/
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plans/contingent_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8543 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plans/hierarchical_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plans/partial_order_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plans/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plans/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plans/sequential_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22033 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plans/stn_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20775 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plans/time_triggered_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.952569 unified_planning-1.1.0.9.dev1/unified_planning/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plot/causal_graph_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36257 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plot/plan_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/plot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30976 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.960569 unified_planning-1.1.0.9.dev1/unified_planning/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.964569 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/basic.anml
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/basic_conditional.anml
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/connected_locations.anml
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/constants.anml
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/constants_no_variable_duration.anml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/durative_goals.anml
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/forall.anml
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/hydrone.anml
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/match.anml
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/match_int_id.anml
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/match_test_parser.anml
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/safe_road.anml
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/simple_mais.anml
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/anml/tils.anml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.920569 unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.964569 unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/colorballs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.964569 unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/logistic_conf/
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.964569 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18623 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/minimals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13662 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/multi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48848 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/realistic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/scheduling/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/scheduling/jobshop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14189 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/tamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37854 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/examples/testing_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.924569 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/
+-rw-r--r--   0 runner    (1001) docker     (127)    34291 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/
+-rw-r--r--   0 runner    (1001) docker     (127)    33635 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-PCP/
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-PCP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Rover/
+-rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Satellite/
+-rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Transport/
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/
+-rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Childsnack/
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.968570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Depots/
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/
+-rw-r--r--   0 runner    (1001) docker     (127)    10943 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Entertainment/
+-rw-r--r--   0 runner    (1001) docker     (127)    18218 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Factories-simple/
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Hiking/
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/
+-rw-r--r--   0 runner    (1001) docker     (127)    17213 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/
+-rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)   189505 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)    11322 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/
+-rw-r--r--   0 runner    (1001) docker     (127)    33123 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/
+-rw-r--r--   0 runner    (1001) docker     (127)    36329 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)    12941 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.972570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Robot/
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Robot/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Snake/
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Towers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Towers/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Transport/
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Woodworking/
+-rw-r--r--   0 runner    (1001) docker     (127)    34612 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/citycar/
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/citycar/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/citycar/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/counters/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/counters/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/counters/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/counters/problem2.pddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/depot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/depot/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/depot/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/enhsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/htn-transport/
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/htn-transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/htn-transport/problem.hddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.976570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/matchcellar/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/matchcellar/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/matchcellar/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/miconic/
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/miconic/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/miconic/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/robot_fastener/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/robot_fastener/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/safe_road/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/safe_road/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/safe_road/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/sailing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/sailing/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/sailing/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/tpp_metric/
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/tpp_metric/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/tpp_metric/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/visit_precedence/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      555 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/visit_precedence/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (127)    31240 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_anml_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_anml_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_anytime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_bounded_types_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_compilers_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_compilers_quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_contingent_pddl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13289 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_dnf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_expression_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17139 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_htn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_infix_notation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_ma_conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_ma_disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18052 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_multi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_negative_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_partial_order_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35427 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_pddl_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_pddl_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15243 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25272 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_problem_kind_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19040 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_protobuf_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_pyperplan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12150 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_quantifier_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_replanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25494 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_simulated_effects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_state_invariants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_stn_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_substituter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_tamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_tarski_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_tarski_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13103 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_trajectory_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_trajectory_constraints_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_ttp_to_stn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_usertype_fluents_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/test/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/unified_planning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.928569 unified_planning-1.1.0.9.dev1/unified_planning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-14 13:58:09.000000 unified_planning-1.1.0.9.dev1/unified_planning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17775 2024-03-14 13:58:09.000000 unified_planning-1.1.0.9.dev1/unified_planning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 13:58:09.000000 unified_planning-1.1.0.9.dev1/unified_planning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-14 13:58:09.000000 unified_planning-1.1.0.9.dev1/unified_planning.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-14 13:58:09.000000 unified_planning-1.1.0.9.dev1/unified_planning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-14 13:58:09.000000 unified_planning-1.1.0.9.dev1/unified_planning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/up_test_cases/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/classical/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/classical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/classical/basic_problems.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/classical/depots/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/classical/depots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/classical/metric_problems.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/classical/tpp/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/classical/tpp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/hierarchical/
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/hierarchical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.980570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8495 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/depot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/logistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/ma_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13165 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/procter_and_gamble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/taxi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/block_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/complex_linear_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/complex_nonlinear_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/constant_additive_effects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/depots/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/depots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/farmlands/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/farmlands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/fn_counters/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/fn_counters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/linear_effects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/nonlinear_effects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/plant_watering/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/plant_watering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/problem_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/rovers/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/rovers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/sailing/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/sailing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/simple_linear_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/simple_nonlinear_conditions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/construction/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/construction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/construction/test_01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7877 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/construction/test_02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/construction/test_03.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/office/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/office/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/office/test_01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/office/test_02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/office/test_03.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.984570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/temporal/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/temporal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/temporal/depot/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/builtin/temporal/depot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/classical/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/classical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/classical/depots/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/classical/depots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/classical/tpp/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/classical/tpp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/block_grouping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/depots/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/depots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/farmlands/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/farmlands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/fn_counters/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/fn_counters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/plant_watering/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/plant_watering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/rovers/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/rovers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/sailing/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/sailing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/temporal/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/temporal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:58:09.988570 unified_planning-1.1.0.9.dev1/up_test_cases/performance/temporal/depot/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/performance/temporal/depot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30011 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-03-14 13:58:05.000000 unified_planning-1.1.0.9.dev1/up_test_cases/utils.py
```

### Comparing `unified_planning-1.1.0.5.dev1/LICENSE` & `unified_planning-1.1.0.9.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/PKG-INFO` & `unified_planning-1.1.0.9.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unified_planning
-Version: 1.1.0.5.dev1
+Version: 1.1.0.9.dev1
 Summary: Unified Planning Framework
 Home-page: https://www.aiplan4eu-project.eu
 Author: AIPlan4EU Project
 Author-email: aiplan4eu@fbk.eu
 License: APACHE
 Description: Unified Planning: A library that makes it easy to formulate planning problems and to invoke automated planners.
 Keywords: planning logic STRIPS RDDL
```

### Comparing `unified_planning-1.1.0.5.dev1/README.md` & `unified_planning-1.1.0.9.dev1/README.md`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/setup.py` & `unified_planning-1.1.0.9.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/cmd/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/cmd/arg_parser.py` & `unified_planning-1.1.0.9.dev1/unified_planning/cmd/arg_parser.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/cmd/up.py` & `unified_planning-1.1.0.9.dev1/unified_planning/cmd/up.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/bounded_types_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/bounded_types_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/compilers_pipeline.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/compilers_pipeline.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/conditional_effects_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/conditional_effects_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/grounder.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/ma_conditional_effects_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/ma_conditional_effects_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/ma_disjunctive_conditions_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/ma_disjunctive_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/negative_conditions_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/negative_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/quantifiers_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/quantifiers_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/state_invariants_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/state_invariants_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/tarski_grounder.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/tarski_grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/compilers/utils.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/compilers/utils.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/credits.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/credits.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/engine.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/engine.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/factory.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/factory.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/meta_engine.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/meta_engine.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/mixins/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/mixins/anytime_planner.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/anytime_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/mixins/compiler.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/compiler.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/mixins/oneshot_planner.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/oneshot_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/mixins/plan_repairer.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/plan_repairer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/mixins/plan_validator.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/plan_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/mixins/portfolio.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/portfolio.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/mixins/replanner.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/replanner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/mixins/sequential_simulator.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/mixins/sequential_simulator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/oversubscription_planner.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/oversubscription_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/parallel.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/parallel.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/pddl_anytime_planner.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/pddl_anytime_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/pddl_planner.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/pddl_planner.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,23 +106,15 @@
 
     def _plan_from_file(
         self,
         problem: "up.model.Problem",
         plan_filename: str,
         get_item_named: Callable[
             [str],
-            Union[
-                "up.model.Type",
-                "up.model.Action",
-                "up.model.Fluent",
-                "up.model.Object",
-                "up.model.Parameter",
-                "up.model.Variable",
-                "up.model.multi_agent.Agent",
-            ],
+            "up.io.pddl_writer.WithName",
         ],
     ) -> "up.plans.Plan":
         """
         Takes a problem, a filename and a map of renaming and returns the plan parsed from the file.
         :param problem: The up.model.problem.Problem instance for which the plan is generated.
         :param plan_filename: The path of the file in which the plan is written.
         :param get_item_named: A function that takes a name and returns the original up.model element instance
@@ -134,23 +126,15 @@
 
     def _plan_from_str(
         self,
         problem: "up.model.Problem",
         plan_str: str,
         get_item_named: Callable[
             [str],
-            Union[
-                "up.model.Type",
-                "up.model.Action",
-                "up.model.Fluent",
-                "up.model.Object",
-                "up.model.Parameter",
-                "up.model.Variable",
-                "up.model.multi_agent.Agent",
-            ],
+            "up.io.pddl_writer.WithName",
         ],
     ) -> "up.plans.Plan":
         """
         Takes a problem, a string and a map of renaming and returns the plan parsed from the string.
         :param problem: The up.model.problem.Problem instance for which the plan is generated.
         :param plan_str: The plan in string.
         :param get_item_named: A function that takes a name and returns the original up.model element instance linked to that renaming.
```

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/plan_validator.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/plan_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/replanner.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/replanner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/results.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/results.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/engines/sequential_simulator.py` & `unified_planning-1.1.0.9.dev1/unified_planning/engines/sequential_simulator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/environment.py` & `unified_planning-1.1.0.9.dev1/unified_planning/environment.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/exceptions.py` & `unified_planning-1.1.0.9.dev1/unified_planning/exceptions.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/grpc/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/grpc/converter.py` & `unified_planning-1.1.0.9.dev1/unified_planning/grpc/converter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/grpc/generated/unified_planning_pb2.py` & `unified_planning-1.1.0.9.dev1/unified_planning/grpc/generated/unified_planning_pb2.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py` & `unified_planning-1.1.0.9.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/grpc/proto_reader.py` & `unified_planning-1.1.0.9.dev1/unified_planning/grpc/proto_reader.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/grpc/proto_writer.py` & `unified_planning-1.1.0.9.dev1/unified_planning/grpc/proto_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/interop/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/interop/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/interop/from_tarski.py` & `unified_planning-1.1.0.9.dev1/unified_planning/interop/from_tarski.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/interop/to_tarski.py` & `unified_planning-1.1.0.9.dev1/unified_planning/interop/to_tarski.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/io/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/io/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/io/anml_grammar.py` & `unified_planning-1.1.0.9.dev1/unified_planning/io/anml_grammar.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/io/anml_reader.py` & `unified_planning-1.1.0.9.dev1/unified_planning/io/anml_reader.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/io/anml_writer.py` & `unified_planning-1.1.0.9.dev1/unified_planning/io/anml_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/io/ma_pddl_writer.py` & `unified_planning-1.1.0.9.dev1/unified_planning/io/ma_pddl_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,38 +40,28 @@
 )
 from unified_planning.model.types import _UserType
 from typing import Callable, Dict, List, Optional, Set, Union, cast
 from io import StringIO
 from unified_planning.io.pddl_writer import (
     ObjectsExtractor,
     ConverterToPDDLString,
-    PDDL_KEYWORDS,
-    INITIAL_LETTER,
+    MangleFunction,
+    WithName,
     _write_effect,
+    _get_pddl_name,
 )
 
 
 class ConverterToMAPDDLString(ConverterToPDDLString):
     """Expression converter to a MA-PDDL string."""
 
     def __init__(
         self,
         problem: MultiAgentProblem,
-        get_mangled_name: Callable[
-            [
-                Union[
-                    "up.model.Type",
-                    "up.model.Action",
-                    "up.model.Fluent",
-                    "up.model.Object",
-                    "up.model.multi_agent.Agent",
-                ]
-            ],
-            str,
-        ],
+        get_mangled_name: MangleFunction,
         agent: Optional["up.model.multi_agent.Agent"],
         unfactored: Optional[bool] = False,
     ):
         ConverterToPDDLString.__init__(self, problem.environment, get_mangled_name)
         self._problem = problem
         self._agent = agent
         self._unfactored = unfactored
@@ -130,37 +120,21 @@
         self.problem_kind = self.problem.kind
         self.explicit_false_initial_states = explicit_false_initial_states
         self.unfactored = unfactored
         self.needs_requirements = needs_requirements
         self.rewrite_bool_assignments = rewrite_bool_assignments
         # otn represents the old to new renamings
         self.otn_renamings: Dict[
-            Union[
-                "up.model.Type",
-                "up.model.Action",
-                "up.model.Fluent",
-                "up.model.Object",
-                "up.model.Parameter",
-                "up.model.Variable",
-                "up.model.multi_agent.Agent",
-            ],
+            WithName,
             str,
         ] = {}
         # nto represents the new to old renamings
         self.nto_renamings: Dict[
             str,
-            Union[
-                "up.model.Type",
-                "up.model.Action",
-                "up.model.Fluent",
-                "up.model.Object",
-                "up.model.Parameter",
-                "up.model.Variable",
-                "up.model.multi_agent.Agent",
-            ],
+            WithName,
         ] = {}
         # those 2 maps are "simmetrical", meaning that "(otn[k] == v) implies (nto[v] == k)"
         self.domain_objects: Optional[Dict[_UserType, Set[Object]]] = None
         self.domain_objects_agents: Dict[up.model.multi_agent.Agent, str]
         self.all_public_fluents: Set[Fluent] = set()
 
     def _write_domain(self):
@@ -823,23 +797,15 @@
                 functions.append(expression)
             else:
                 raise UPTypeError("MA-PDDL supports only boolean and numerical fluents")
         return predicates, functions
 
     def _get_mangled_name(
         self,
-        item: Union[
-            "up.model.Type",
-            "up.model.Action",
-            "up.model.Fluent",
-            "up.model.Object",
-            "up.model.Parameter",
-            "up.model.Variable",
-            "up.model.multi_agent.Agent",
-        ],
+        item: WithName,
     ) -> str:
         """This function returns a valid and unique MA-PDDL name."""
 
         # If we already encountered this item, return it
         if item in self.otn_renamings:
             return self.otn_renamings[item]
 
@@ -871,25 +837,15 @@
 
         else:
             new_name = tmp_name
         self.otn_renamings[item] = new_name
         self.nto_renamings[new_name] = item
         return new_name
 
-    def get_item_named(
-        self, name: str
-    ) -> Union[
-        "up.model.Type",
-        "up.model.Action",
-        "up.model.Fluent",
-        "up.model.Object",
-        "up.model.Parameter",
-        "up.model.Variable",
-        "up.model.multi_agent.Agent",
-    ]:
+    def get_item_named(self, name: str) -> WithName:
         """
         Since `MA-PDDL` has a stricter set of possible naming compared to the `unified_planning`, when writing
         a :class:`~unified_planning.model.Problem` it is possible that some things must be renamed. This is why the `MAPDDLWriter`
         offers this method, that takes a `MA-PDDL` name and returns the original `unified_planning` data structure that corresponds
         to the `MA-PDDL` entity with the given name.
 
         This method takes a name used in the `MA-PDDL` domain or `MA-PDDL` problem generated by this `MAPDDLWriter` and returns the original
@@ -974,47 +930,14 @@
                             _update_domain_objects(
                                 self.domain_objects, obe.get(e.condition)
                             )
                         _update_domain_objects(self.domain_objects, obe.get(e.fluent))
                         _update_domain_objects(self.domain_objects, obe.get(e.value))
 
 
-def _get_pddl_name(
-    item: Union[
-        "up.model.Type",
-        "up.model.Action",
-        "up.model.Fluent",
-        "up.model.Object",
-        "up.model.Parameter",
-        "up.model.Variable",
-        "up.model.Problem",
-        "up.model.multi_agent.MultiAgentProblem",
-        "up.model.multi_agent.Agent",
-    ]
-) -> str:
-    """This function returns a ma-pddl name for the chosen item"""
-    name = item.name  # type: ignore
-    assert name is not None
-    name = name.lower()
-    regex = re.compile(r"^[a-zA-Z]+.*")
-    if (
-        re.match(regex, name) is None
-    ):  # If the name does not start with an alphabetic char, we make it start with one.
-        name = f'{INITIAL_LETTER.get(type(item), "x")}_{name}'
-
-    name = re.sub("[^0-9a-zA-Z_]", "_", name)  # Substitute non-valid elements with "_"
-    while (
-        name in PDDL_KEYWORDS
-    ):  # If the name is in the keywords, apply an underscore at the end until it is not a keyword anymore.
-        name = f"{name}_"
-    if isinstance(item, up.model.Parameter) or isinstance(item, up.model.Variable):
-        name = f"?{name}"
-    return name
-
-
 def _update_domain_objects(
     dict_to_update: Dict[_UserType, Set[Object]], values: Dict[_UserType, Set[Object]]
 ) -> None:
     """Small utility method that updated a UserType -> Set[Object] dict with another dict of the same type."""
     for ut, os in values.items():
         os_to_update = dict_to_update.setdefault(ut, set())
         os_to_update |= os
```

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/io/pddl_reader.py` & `unified_planning-1.1.0.9.dev1/unified_planning/io/pddl_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1717,23 +1717,15 @@
     def parse_plan_string(
         self,
         problem: "up.model.Problem",
         plan_str: str,
         get_item_named: typing.Optional[
             Callable[
                 [str],
-                Union[
-                    "up.model.Type",
-                    "up.model.Action",
-                    "up.model.Fluent",
-                    "up.model.Object",
-                    "up.model.Parameter",
-                    "up.model.Variable",
-                    "up.model.multi_agent.Agent",
-                ],
+                "up.io.pddl_writer.WithName",
             ]
         ] = None,
     ) -> "up.plans.Plan":
         """
         Takes a problem, a string and optionally a map of renaming and returns the plan parsed from the string.
 
         The format of the file must be:
```

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/io/pddl_writer.py` & `unified_planning-1.1.0.9.dev1/unified_planning/io/pddl_writer.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     Timing,
 )
 from unified_planning.exceptions import (
     UPTypeError,
     UPProblemDefinitionError,
     UPException,
 )
+from unified_planning.model.htn import HierarchicalProblem
 from unified_planning.model.types import _UserType
 from unified_planning.plans import (
     SequentialPlan,
     TimeTriggeredPlan,
     Plan,
     ActionInstance,
 )
@@ -131,14 +132,27 @@
     DurativeAction: "a",
     Fluent: "f",
     Parameter: "p",
     Problem: "p",
     Object: "o",
 }
 
+WithName = Union[
+    "up.model.Type",
+    "up.model.Action",
+    "up.model.Fluent",
+    "up.model.Object",
+    "up.model.Parameter",
+    "up.model.Variable",
+    "up.model.multi_agent.Agent",
+    "up.model.htn.Method",
+    "up.model.htn.Task",
+]
+MangleFunction = Callable[[WithName], str]
+
 
 class ObjectsExtractor(walkers.DagWalker):
     """Returns the object instances appearing in the expression."""
 
     def __init__(self):
         walkers.dag.DagWalker.__init__(self)
 
@@ -173,26 +187,15 @@
     """Expression converter to a PDDL string."""
 
     DECIMAL_PRECISION = 10  # Number of decimal places to print real constants
 
     def __init__(
         self,
         environment: "up.environment.Environment",
-        get_mangled_name: Callable[
-            [
-                Union[
-                    "up.model.Type",
-                    "up.model.Action",
-                    "up.model.Fluent",
-                    "up.model.Object",
-                    "up.model.multi_agent.Agent",
-                ]
-            ],
-            str,
-        ],
+        get_mangled_name: MangleFunction,
     ):
         walkers.DagWalker.__init__(self)
         self.get_mangled_name = get_mangled_name
         self.simplifier = environment.simplifier
 
     def convert(self, expression):
         """Converts the given expression to a PDDL string."""
@@ -344,37 +347,21 @@
     ):
         self.problem = problem
         self.problem_kind = self.problem.kind
         self.needs_requirements = needs_requirements
         self.rewrite_bool_assignments = rewrite_bool_assignments
         # otn represents the old to new renamings
         self.otn_renamings: Dict[
-            Union[
-                "up.model.Type",
-                "up.model.Action",
-                "up.model.Fluent",
-                "up.model.Object",
-                "up.model.Parameter",
-                "up.model.Variable",
-                "up.model.multi_agent.Agent",
-            ],
+            WithName,
             str,
         ] = {}
         # nto represents the new to old renamings
         self.nto_renamings: Dict[
             str,
-            Union[
-                "up.model.Type",
-                "up.model.Action",
-                "up.model.Fluent",
-                "up.model.Object",
-                "up.model.Parameter",
-                "up.model.Variable",
-                "up.model.multi_agent.Agent",
-            ],
+            WithName,
         ] = {}
         # those 2 maps are "simmetrical", meaning that "(otn[k] == v) implies (nto[v] == k)"
         self.domain_objects: Optional[Dict[_UserType, Set[Object]]] = None
 
     def _write_domain(self, out: IO[str]):
         if self.problem_kind.has_intermediate_conditions_and_effects():
             raise UPProblemDefinitionError(
@@ -435,14 +422,18 @@
                     for e in le:
                         if not e.fluent.type.is_bool_type():
                             only_bool = False
                 if not only_bool:
                     out.write(" :timed-initial-effects")
                 else:
                     out.write(" :timed-initial-literals")
+            if self.problem_kind.has_hierarchical():
+                out.write(" :hierarchy")  # HTN / HDDL
+            if self.problem_kind.has_method_preconditions():
+                out.write(" :method-preconditions")
             out.write(")\n")
 
         if self.problem_kind.has_hierarchical_typing():
             user_types_hierarchy = self.problem.user_types_hierarchy
             out.write(f" (:types\n")
             stack: List["unified_planning.model.Type"] = (
                 user_types_hierarchy[None] if None in user_types_hierarchy else []
@@ -539,16 +530,59 @@
             elif metric.is_minimize_sequential_plan_length():
                 for a in self.problem.actions:
                     costs[a] = self.problem.environment.expression_manager.Int(1)
         elif len(metrics) > 1:
             raise up.exceptions.UPUnsupportedProblemTypeError(
                 "Only one metric is supported!"
             )
-
         em = self.problem.environment.expression_manager
+        if isinstance(self.problem, HierarchicalProblem):
+            for task in self.problem.tasks:
+                out.write(f" (:task {self._get_mangled_name(task)}")
+                out.write(f"\n  :parameters (")
+                for ap in task.parameters:
+                    if ap.type.is_user_type():
+                        out.write(
+                            f" {self._get_mangled_name(ap)} - {self._get_mangled_name(ap.type)}"
+                        )
+                    else:
+                        raise UPTypeError("PDDL supports only user type parameters")
+                out.write("))\n")
+
+            for m in self.problem.methods:
+                out.write(f" (:method {self._get_mangled_name(m)}")
+                out.write(f"\n  :parameters (")
+                for ap in m.parameters:
+                    if ap.type.is_user_type():
+                        out.write(
+                            f" {self._get_mangled_name(ap)} - {self._get_mangled_name(ap.type)}"
+                        )
+                    else:
+                        raise UPTypeError("PDDL supports only user type parameters")
+                out.write(")")
+
+                params_str = " ".join(
+                    converter.convert(em.ParameterExp(p))
+                    for p in m.achieved_task.parameters
+                )
+                out.write(
+                    f"\n  :task ({self._get_mangled_name(m.achieved_task.task)} {params_str})"
+                )
+                if len(m.preconditions) > 0:
+                    precond_str: List[str] = []
+                    for p in (c.simplify() for c in m.preconditions):
+                        if not p.is_true():
+                            if p.is_and():
+                                precond_str.extend(map(converter.convert, p.args))
+                            else:
+                                precond_str.append(converter.convert(p))
+                    out.write(f'\n  :precondition (and {" ".join(precond_str)})')
+                self._write_task_network(m, out, converter)
+                out.write(")\n")
+
         for a in self.problem.actions:
             if isinstance(a, up.model.InstantaneousAction):
                 if any(p.simplify().is_false() for p in a.preconditions):
                     continue
                 out.write(f" (:action {self._get_mangled_name(a)}")
                 out.write(f"\n  :parameters (")
                 for ap in a.parameters:
@@ -556,15 +590,15 @@
                         out.write(
                             f" {self._get_mangled_name(ap)} - {self._get_mangled_name(ap.type)}"
                         )
                     else:
                         raise UPTypeError("PDDL supports only user type parameters")
                 out.write(")")
                 if len(a.preconditions) > 0:
-                    precond_str: List[str] = []
+                    precond_str = []
                     for p in (c.simplify() for c in a.preconditions):
                         if not p.is_true():
                             if p.is_and():
                                 precond_str.extend(map(converter.convert, p.args))
                             else:
                                 precond_str.append(converter.convert(p))
                     out.write(f'\n  :precondition (and {" ".join(precond_str)})')
@@ -684,14 +718,18 @@
                     out.write(
                         f'\n   {" ".join([self._get_mangled_name(o) for o in objects])} - {self._get_mangled_name(t)}'
                     )
             out.write("\n )\n")
         converter = ConverterToPDDLString(
             self.problem.environment, self._get_mangled_name
         )
+        if isinstance(self.problem, up.model.htn.HierarchicalProblem):
+            out.write(" (:htn")
+            self._write_task_network(self.problem.task_network, out, converter)
+            out.write(")\n")
         out.write(" (:init")
         for f, v in self.problem.initial_values.items():
             if v.is_true():
                 out.write(f" {converter.convert(f)}")
             elif v.is_false():
                 pass
             else:
@@ -816,23 +854,15 @@
     def write_plan(self, plan: Plan, filename: str):
         """Dumps to file the `PDDL` plan."""
         with open(filename, "w") as f:
             self._write_plan(plan, f)
 
     def _get_mangled_name(
         self,
-        item: Union[
-            "up.model.Type",
-            "up.model.Action",
-            "up.model.Fluent",
-            "up.model.Object",
-            "up.model.Parameter",
-            "up.model.Variable",
-            "up.model.multi_agent.Agent",
-        ],
+        item: WithName,
     ) -> str:
         """This function returns a valid and unique PDDL name."""
 
         # If we already encountered this item, return it
         if item in self.otn_renamings:
             return self.otn_renamings[item]
 
@@ -860,25 +890,15 @@
             new_name not in self.nto_renamings
             and new_name not in self.otn_renamings.values()
         )
         self.otn_renamings[item] = new_name
         self.nto_renamings[new_name] = item
         return new_name
 
-    def get_item_named(
-        self, name: str
-    ) -> Union[
-        "up.model.Type",
-        "up.model.Action",
-        "up.model.Fluent",
-        "up.model.Object",
-        "up.model.Parameter",
-        "up.model.Variable",
-        "up.model.multi_agent.Agent",
-    ]:
+    def get_item_named(self, name: str) -> WithName:
         """
         Since `PDDL` has a stricter set of possible naming compared to the `unified_planning`, when writing
         a :class:`~unified_planning.model.Problem` it is possible that some things must be renamed. This is why the `PDDLWriter`
         offers this method, that takes a `PDDL` name and returns the original `unified_planning` data structure that corresponds
         to the `PDDL` entity with the given name.
 
         This method takes a name used in the `PDDL` domain or `PDDL` problem generated by this `PDDLWriter` and returns the original
@@ -941,28 +961,78 @@
                     for e in el:
                         if e.is_conditional():
                             _update_domain_objects(
                                 self.domain_objects, obe.get(e.condition)
                             )
                         _update_domain_objects(self.domain_objects, obe.get(e.fluent))
                         _update_domain_objects(self.domain_objects, obe.get(e.value))
+        if isinstance(self.problem, HierarchicalProblem):
+            for m in self.problem.methods:
+                for p in m.preconditions:
+                    _update_domain_objects(self.domain_objects, obe.get(p))
+                for subtask in m.subtasks:
+                    for targ in subtask.parameters:
+                        _update_domain_objects(self.domain_objects, obe.get(targ))
+                for c in m.non_temporal_constraints():
+                    _update_domain_objects(self.domain_objects, obe.get(c))
 
+    def _write_task_network(
+        self,
+        tn: up.model.htn.task_network.AbstractTaskNetwork,
+        out,
+        converter: ConverterToPDDLString,
+    ):
+        def format_subtask(t: up.model.htn.Subtask):
+            return f"({t.identifier} ({self._get_mangled_name(t.task)} {' '.join(map(converter.convert, t.parameters))}))"
 
-def _get_pddl_name(
-    item: Union[
-        "up.model.Type",
-        "up.model.Action",
-        "up.model.Fluent",
-        "up.model.Object",
-        "up.model.Parameter",
-        "up.model.Variable",
-        "up.model.Problem",
-        "up.model.multi_agent.Agent",
-    ]
-) -> str:
+        if isinstance(tn, up.model.htn.TaskNetwork) and len(tn.variables) > 0:
+            out.write(f"\n  :parameters (")
+            for ap in tn.variables:
+                if ap.type.is_user_type():
+                    out.write(
+                        f" {self._get_mangled_name(ap)} - {self._get_mangled_name(ap.type)}"
+                    )
+                else:
+                    raise UPTypeError("PDDL supports only user type parameters")
+            out.write(")")
+
+        to = tn.total_order()
+        po = tn.partial_order()
+        if len(tn.subtasks) == 0:
+            pass  # nothing to do
+        elif to is not None:  # subtasks form a total order
+            ordered_tasks = "\n    ".join(
+                format_subtask(tn.get_subtask(id)) for id in to
+            )
+            out.write(f"\n  :ordered-subtasks (and\n    {ordered_tasks})")
+        elif po is not None:  # subtasks for a partial order
+            tasks = "\n    ".join(format_subtask(t) for t in tn.subtasks)
+            out.write(f"\n  :subtasks (and\n    {tasks})")
+            orders = "\n    ".join(f"(< {id1} {id2})" for id1, id2 in po)
+            out.write(f"\n  :ordering (and\n    {orders})")
+        else:
+            raise UPProblemDefinitionError(
+                "HDDL does not support general temporal constraints. From:\n" + str(tn)
+            )
+
+        if len(tn.non_temporal_constraints()) > 0:
+            constraint_str: List[str] = []
+            for p in (c.simplify() for c in tn.non_temporal_constraints()):
+                if not p.is_true():
+                    if p.is_and():
+                        constraint_str.extend(map(converter.convert, p.args))
+                    else:
+                        constraint_str.append(converter.convert(p))
+            out.write(f'\n  :constraints (and {" ".join(constraint_str)})')
+            raise UPProblemDefinitionError(
+                "Task network constraints not supported by HDDL Writer yet"
+            )
+
+
+def _get_pddl_name(item: Union[WithName, "up.model.AbstractProblem"]) -> str:
     """This function returns a pddl name for the chosen item"""
     name = item.name  # type: ignore
     assert name is not None
     name = name.lower()
     regex = re.compile(r"^[a-zA-Z]+.*")
     if (
         re.match(regex, name) is None
@@ -990,28 +1060,15 @@
 
 def _write_effect(
     effect: Effect,
     timing: Optional[Timing],
     out: IO[str],
     converter: ConverterToPDDLString,
     rewrite_bool_assignments: bool,
-    get_mangled_name: Callable[
-        [
-            Union[
-                "up.model.Type",
-                "up.model.Action",
-                "up.model.Fluent",
-                "up.model.Object",
-                "up.model.Parameter",
-                "up.model.Variable",
-                "up.model.multi_agent.Agent",
-            ]
-        ],
-        str,
-    ],
+    get_mangled_name: MangleFunction,
 ):
     simplified_cond = effect.condition.simplify()
     # check for non-constant-bool-assignment
     non_const_bool_ass = (
         effect.value.type.is_bool_type()
         and not effect.value.is_true()
         and not effect.value.is_false()
```

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/io/utils.py` & `unified_planning-1.1.0.9.dev1/unified_planning/io/utils.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/abstract_problem.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/abstract_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/action.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/action.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/contingent_problem.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/contingent_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/delta_stn.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/delta_stn.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/effect.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/effect.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/expression.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/expression.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/fluent.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/fluent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/fnode.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/fnode.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/htn/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/htn/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/htn/hierarchical_problem.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/htn/hierarchical_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/htn/method.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/htn/method.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/htn/ordering.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/htn/ordering.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/htn/task.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/htn/task.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/htn/task_network.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/htn/task_network.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/metrics.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/metrics.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/mixins/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/mixins/actions_set.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/actions_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/mixins/agents_set.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/agents_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/mixins/fluents_set.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/fluents_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/mixins/initial_state.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/initial_state.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/mixins/metrics.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/metrics.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/mixins/objects_set.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/objects_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/mixins/time_model.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/time_model.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/mixins/timed_conds_effs.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/timed_conds_effs.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/mixins/user_types_set.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/mixins/user_types_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/multi_agent/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/multi_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/multi_agent/agent.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/multi_agent/agent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/multi_agent/ma_environment.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/multi_agent/ma_environment.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/multi_agent/ma_problem.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/multi_agent/ma_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/object.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/object.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/operators.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/operators.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/parameter.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/parameter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/problem.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/problem_kind.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/problem_kind.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/problem_kind_versioning.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/problem_kind_versioning.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/scheduling/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/scheduling/activity.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/scheduling/activity.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/scheduling/chronicle.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/scheduling/chronicle.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/scheduling/scheduling_problem.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/scheduling/scheduling_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/state.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/state.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/tamp/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/tamp/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/tamp/action.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/tamp/action.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/tamp/objects.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/tamp/objects.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/tamp/path.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/tamp/path.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/tamp/types.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/tamp/types.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/timing.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/timing.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/type_manager.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/type_manager.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/types.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/types.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/variable.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/variable.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/any.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/any.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/dag.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/dag.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/dnf.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/dnf.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/fluents_substituter.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/fluents_substituter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/free_vars.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/free_vars.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/generic.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/generic.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/identitydag.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/identitydag.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/linear_checker.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/linear_checker.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/names_extractor.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/names_extractor.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/operators_extractor.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/operators_extractor.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/quantifier_simplifier.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/quantifier_simplifier.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/simplifier.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/simplifier.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/state_evaluator.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/state_evaluator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/substituter.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/substituter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/type_checker.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/type_checker.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/model/walkers/usertype_fluents_walker.py` & `unified_planning-1.1.0.9.dev1/unified_planning/model/walkers/usertype_fluents_walker.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/plans/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plans/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/plans/contingent_plan.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plans/contingent_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/plans/hierarchical_plan.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plans/hierarchical_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/plans/partial_order_plan.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plans/partial_order_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/plans/plan.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plans/plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/plans/schedule.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plans/schedule.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/plans/sequential_plan.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plans/sequential_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/plans/stn_plan.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plans/stn_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/plans/time_triggered_plan.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plans/time_triggered_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/plot/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/plot/causal_graph_plot.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plot/causal_graph_plot.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/plot/plan_plot.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plot/plan_plot.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/plot/utils.py` & `unified_planning-1.1.0.9.dev1/unified_planning/plot/utils.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/shortcuts.py` & `unified_planning-1.1.0.9.dev1/unified_planning/shortcuts.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/anml/connected_locations.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/connected_locations.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/anml/constants.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/constants.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/anml/constants_no_variable_duration.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/constants_no_variable_duration.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/anml/forall.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/forall.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/anml/hydrone.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/hydrone.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/anml/match.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/match.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/anml/match_int_id.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/match_int_id.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/anml/match_test_parser.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/match_test_parser.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/anml/safe_road.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/safe_road.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/anml/simple_mais.anml` & `unified_planning-1.1.0.9.dev1/unified_planning/test/anml/simple_mais.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/examples/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/examples/hierarchical.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/examples/hierarchical.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/examples/minimals.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/examples/minimals.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/examples/multi_agent.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/examples/multi_agent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/examples/realistic.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/examples/realistic.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/examples/scheduling/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/examples/scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/examples/scheduling/examples.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/examples/scheduling/examples.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/examples/scheduling/jobshop.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/examples/scheduling/jobshop.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/examples/tamp.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/examples/tamp.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/examples/testing_variants.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/examples/testing_variants.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/__init__.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/citycar/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/citycar/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/citycar/problem.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/citycar/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/counters/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/counters/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/counters/problem2.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/counters/problem2.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/depot/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/depot/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/depot/problem.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/depot/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/enhsp.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/enhsp.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/htn-transport/domain.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/htn-transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/htn-transport/problem.hddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/htn-transport/problem.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/matchcellar/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/matchcellar/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/miconic/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/miconic/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/safe_road/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/safe_road/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/sailing/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/sailing/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/tpp_metric/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/tpp_metric/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/tpp_metric/problem.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/tpp_metric/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl` & `unified_planning-1.1.0.9.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_anml_reader.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_anml_reader.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_anml_writer.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_anml_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_anytime.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_anytime.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_bounded_types_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_bounded_types_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_compilers_pipeline.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_compilers_pipeline.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_compilers_quality_metrics.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_compilers_quality_metrics.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_conditional_effects_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_conditional_effects_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_contingent_pddl.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_contingent_pddl.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_credits.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_credits.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_disjunctive_conditions_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_disjunctive_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_dnf.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_dnf.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_expression_analysis.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_expression_analysis.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_factory.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_factory.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_grounder.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_htn.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_htn.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
+import tempfile
 
 import unified_planning as up
-from unified_planning.io import PDDLReader
+from unified_planning.io import PDDLReader, PDDLWriter
 from unified_planning.model.htn import TaskNetwork, Task
 from unified_planning.model.htn.ordering import PartialOrder, TotalOrder
 from unified_planning.shortcuts import *
 from unified_planning.test import unittest_TestCase, main, examples
 from unified_planning.test.examples import get_example_problems
 
 
@@ -151,7 +152,31 @@
                 TO_instances = [
                     "2020-po-Satellite"
                 ]  # these problems allow non-ordered goal tasks but have only one initial task in our test instance
                 assert (
                     "TASK_ORDER_PARTIAL" in problem.kind.features
                     or name in TO_instances
                 )
+
+    def test_hddl_writing(self):
+        """Tests that all HDDL benchmarks can be written to HDDL and reparsed."""
+        hddl_dir = os.path.join(FILE_PATH, "hddl")
+        subfolders = [f.path for f in os.scandir(hddl_dir) if f.is_dir()]
+        for id, domain in enumerate(subfolders[:]):
+            name = os.path.basename(domain)
+            print(f"=== [{id}] {name} ===")
+            domain_filename = os.path.join(domain, "domain.hddl")
+            problem_filename = os.path.join(domain, "instance.1.pb.hddl")
+            reader = PDDLReader()
+            problem = reader.parse_problem(domain_filename, problem_filename)
+
+            # print(problem)
+            w = PDDLWriter(problem)
+            with tempfile.TemporaryDirectory() as tempdir:
+                domain_filename = os.path.join(tempdir, "domain.pddl")
+                problem_filename = os.path.join(tempdir, "problem.pddl")
+                w.write_domain(domain_filename)
+                w.write_problem(problem_filename)
+
+                reader = PDDLReader()
+                parsed_problem = reader.parse_problem(domain_filename, problem_filename)
+                self.assertEqual(parsed_problem.kind, problem.kind)
```

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_infix_notation.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_infix_notation.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_ma_conditional_effects_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_ma_conditional_effects_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_ma_disjunctive_conditions_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_ma_disjunctive_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_model.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_model.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_multi_agent.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_multi_agent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_negative_conditions_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_negative_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_partial_order_plan.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_partial_order_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_pddl_io.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_pddl_io.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_pddl_planner.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_pddl_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_plan_validator.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_plan_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_planner.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_problem.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_problem_kind_versioning.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_problem_kind_versioning.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_protobuf_io.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_protobuf_io.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_pyperplan.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_pyperplan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_quantifier_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_quantifier_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_replanner.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_replanner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_scheduling.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_sequential_simulator.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_sequential_simulator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_simplifier.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_simplifier.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_simulated_effects.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_simulated_effects.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_state_invariants.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_state_invariants.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_stn_plan.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_stn_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_substituter.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_substituter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_tamp.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_tamp.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_tarski_converter.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_tarski_converter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_tarski_grounder.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_tarski_grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_temporal.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_temporal.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_trajectory_constraint.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_trajectory_constraint.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_trajectory_constraints_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_trajectory_constraints_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_ttp_to_stn.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_ttp_to_stn.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_usertype_fluents_remover.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_usertype_fluents_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/test/test_validator.py` & `unified_planning-1.1.0.9.dev1/unified_planning/test/test_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning/utils.py` & `unified_planning-1.1.0.9.dev1/unified_planning/utils.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning.egg-info/PKG-INFO` & `unified_planning-1.1.0.9.dev1/unified_planning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unified-planning
-Version: 1.1.0.5.dev1
+Version: 1.1.0.9.dev1
 Summary: Unified Planning Framework
 Home-page: https://www.aiplan4eu-project.eu
 Author: AIPlan4EU Project
 Author-email: aiplan4eu@fbk.eu
 License: APACHE
 Description: Unified Planning: A library that makes it easy to formulate planning problems and to invoke automated planners.
 Keywords: planning logic STRIPS RDDL
```

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning.egg-info/SOURCES.txt` & `unified_planning-1.1.0.9.dev1/unified_planning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/unified_planning.egg-info/requires.txt` & `unified_planning-1.1.0.9.dev1/unified_planning.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/classical/basic_problems.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/classical/basic_problems.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/classical/metric_problems.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/classical/metric_problems.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/hierarchical/__init__.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/hierarchical/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/multiagent/depot.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/depot.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/multiagent/logistic.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/logistic.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/multiagent/ma_basic.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/ma_basic.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/multiagent/procter_and_gamble.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/procter_and_gamble.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/multiagent/taxi.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/multiagent/taxi.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/block_grouping.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/block_grouping.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/complex_linear_conditions.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/complex_linear_conditions.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/complex_nonlinear_conditions.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/complex_nonlinear_conditions.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/constant_additive_effects.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/constant_additive_effects.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/linear_effects.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/linear_effects.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/nonlinear_effects.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/nonlinear_effects.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/problem_basic.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/problem_basic.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/sailing/__init__.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/sailing/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/simple_linear_conditions.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/simple_linear_conditions.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/numeric/simple_nonlinear_conditions.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/numeric/simple_nonlinear_conditions.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/tamp/construction/test_01.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/construction/test_01.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/tamp/construction/test_02.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/construction/test_02.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/tamp/construction/test_03.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/construction/test_03.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/tamp/office/test_01.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/office/test_01.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/tamp/office/test_02.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/office/test_02.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/builtin/tamp/office/test_03.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/builtin/tamp/office/test_03.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/performance/numeric/block_grouping.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/performance/numeric/block_grouping.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/report.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/report.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.1.0.5.dev1/up_test_cases/utils.py` & `unified_planning-1.1.0.9.dev1/up_test_cases/utils.py`

 * *Files identical despite different names*

