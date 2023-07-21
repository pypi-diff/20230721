# Comparing `tmp/unified_planning-1.0.0.29.dev1.tar.gz` & `tmp/unified_planning-1.0.0.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unified_planning-1.0.0.29.dev1.tar", last modified: Fri Jul 21 08:18:22 2023, max compression
+gzip compressed data, was "unified_planning-1.0.0.6.dev1.tar", last modified: Mon Jul 17 07:51:10 2023, max compression
```

## Comparing `unified_planning-1.0.0.29.dev1.tar` & `unified_planning-1.0.0.6.dev1.tar`

### file list

```diff
@@ -1,380 +1,376 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.737512 unified_planning-1.0.0.29.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-21 08:18:22.737512 unified_planning-1.0.0.29.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 08:18:22.737512 unified_planning-1.0.0.29.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.693512 unified_planning-1.0.0.29.dev1/unified_planning/
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.693512 unified_planning-1.0.0.29.dev1/unified_planning/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/cmd/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/cmd/up.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.697512 unified_planning-1.0.0.29.dev1/unified_planning/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.697512 unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/bounded_types_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/compilers_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    19001 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    19106 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/ma_conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/ma_disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    17381 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/negative_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    14003 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/quantifiers_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/state_invariants_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/tarski_grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    29926 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    20771 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/credits.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    48595 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/meta_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.701512 unified_planning-1.0.0.29.dev1/unified_planning/engines/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/mixins/anytime_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/mixins/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/mixins/oneshot_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/mixins/plan_repairer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/mixins/plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/mixins/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/mixins/replanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/mixins/sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/oversubscription_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    11047 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/pddl_anytime_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    18248 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/pddl_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10455 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/replanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12778 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    35416 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/engines/sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.701512 unified_planning-1.0.0.29.dev1/unified_planning/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/grpc/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.701512 unified_planning-1.0.0.29.dev1/unified_planning/grpc/generated/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/grpc/generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20618 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/grpc/generated/unified_planning_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    38742 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/grpc/proto_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    38783 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/grpc/proto_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.701512 unified_planning-1.0.0.29.dev1/unified_planning/interop/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/interop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/interop/from_tarski.py
--rw-r--r--   0 runner    (1001) docker     (123)    18068 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/interop/to_tarski.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.705512 unified_planning-1.0.0.29.dev1/unified_planning/io/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16387 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/io/anml_grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)    46716 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/io/anml_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    19259 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/io/anml_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    39290 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/io/ma_pddl_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    77329 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/io/pddl_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    40589 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/io/pddl_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.705512 unified_planning-1.0.0.29.dev1/unified_planning/model/
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/abstract_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    29564 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/contingent_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/delta_stn.py
--rw-r--r--   0 runner    (1001) docker     (123)    18666 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    28717 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/fluent.py
--rw-r--r--   0 runner    (1001) docker     (123)    17991 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/fnode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.705512 unified_planning-1.0.0.29.dev1/unified_planning/model/htn/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/htn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/htn/hierarchical_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/htn/method.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/htn/ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/htn/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8843 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/htn/task_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    13510 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.709512 unified_planning-1.0.0.29.dev1/unified_planning/model/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/mixins/actions_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/mixins/agents_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/mixins/fluents_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/mixins/initial_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/mixins/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/mixins/objects_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/mixins/time_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/mixins/timed_conds_effs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/mixins/user_types_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.709512 unified_planning-1.0.0.29.dev1/unified_planning/model/multi_agent/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/multi_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/multi_agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/multi_agent/ma_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19329 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/multi_agent/ma_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    43542 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/problem_kind.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.709512 unified_planning-1.0.0.29.dev1/unified_planning/model/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/scheduling/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/scheduling/chronicle.py
--rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/scheduling/scheduling_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.709512 unified_planning-1.0.0.29.dev1/unified_planning/model/tamp/
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/tamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/tamp/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/tamp/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/tamp/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/tamp/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/type_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.713512 unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/any.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/dnf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/fluents_substituter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/free_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/identitydag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/linear_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/names_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/operators_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/quantifier_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    17364 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/state_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/substituter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/type_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    24752 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/usertype_fluents_walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.713512 unified_planning-1.0.0.29.dev1/unified_planning/plans/
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/plans/contingent_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/plans/hierarchical_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/plans/partial_order_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/plans/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/plans/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/plans/sequential_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    20055 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/plans/stn_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/plans/time_triggered_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.713512 unified_planning-1.0.0.29.dev1/unified_planning/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/plot/causal_graph_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    31499 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/plot/plan_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/plot/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    30679 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.721512 unified_planning-1.0.0.29.dev1/unified_planning/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.721512 unified_planning-1.0.0.29.dev1/unified_planning/test/anml/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/anml/basic.anml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/anml/basic_conditional.anml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/anml/connected_locations.anml
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/anml/constants.anml
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/anml/constants_no_variable_duration.anml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/anml/durative_goals.anml
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/anml/forall.anml
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/anml/hydrone.anml
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/anml/match.anml
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/anml/match_int_id.anml
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/anml/match_test_parser.anml
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/anml/safe_road.anml
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/anml/simple_mais.anml
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/anml/tils.anml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.689512 unified_planning-1.0.0.29.dev1/unified_planning/test/contingent_pddl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.725512 unified_planning-1.0.0.29.dev1/unified_planning/test/contingent_pddl/colorballs/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.725512 unified_planning-1.0.0.29.dev1/unified_planning/test/contingent_pddl/logistic_conf/
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.725512 unified_planning-1.0.0.29.dev1/unified_planning/test/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/examples/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/examples/minimals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13633 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/examples/multi_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    40351 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/examples/realistic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.725512 unified_planning-1.0.0.29.dev1/unified_planning/test/examples/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/examples/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/examples/scheduling/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/examples/scheduling/jobshop.py
--rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/examples/tamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    37280 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/examples/testing_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.693512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.725512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/
--rw-r--r--   0 runner    (1001) docker     (123)    34291 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.725512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/
--rw-r--r--   0 runner    (1001) docker     (123)    33635 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.725512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-PCP/
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-PCP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.725512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Rover/
--rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.725512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Satellite/
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.725512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Transport/
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.725512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/
--rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.729512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.729512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.729512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Childsnack/
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.729512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Depots/
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.729512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/
--rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.729512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Entertainment/
--rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.729512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Factories-simple/
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.729512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Hiking/
--rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.729512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/
--rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.729512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)   189505 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.729512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.729512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/
--rw-r--r--   0 runner    (1001) docker     (123)    33123 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.729512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/
--rw-r--r--   0 runner    (1001) docker     (123)    36329 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.733512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.733512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Robot/
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Robot/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.733512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.733512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.733512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Snake/
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.733512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Towers/
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Towers/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.733512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Transport/
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.733512 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Woodworking/
--rw-r--r--   0 runner    (1001) docker     (123)    34612 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.733512 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.733512 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/citycar/
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/citycar/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/citycar/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.733512 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/counters/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/counters/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/counters/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/counters/problem2.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.733512 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/depot/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/depot/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/depot/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/enhsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.733512 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/htn-transport/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/htn-transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/htn-transport/problem.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.733512 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/matchcellar/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/matchcellar/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/matchcellar/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.737512 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/miconic/
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/miconic/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/miconic/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.737512 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/robot_fastener/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/robot_fastener/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.737512 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/safe_road/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/safe_road/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/safe_road/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.737512 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/sailing/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/sailing/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/sailing/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.737512 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/tpp_metric/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/tpp_metric/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/tpp_metric/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.737512 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/visit_precedence/
--rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/visit_precedence/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    31213 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_anml_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    15583 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_anml_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_anytime.py
--rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_bounded_types_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_compilers_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_compilers_quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_contingent_pddl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_credits.py
--rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_dnf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_expression_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    17057 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_htn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_infix_notation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_ma_conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_ma_disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_multi_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_negative_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_partial_order_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    35383 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_pddl_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    14880 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_pddl_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15206 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    25295 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    18899 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_protobuf_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_pyperplan.py
--rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_quantifier_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_replanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_scheduling.py
--rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25431 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_simulated_effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_state_invariants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_stn_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_substituter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_tamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_tarski_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_tarski_grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)    13076 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_trajectory_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_trajectory_constraints_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_usertype_fluents_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/test/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-21 08:18:18.000000 unified_planning-1.0.0.29.dev1/unified_planning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:18:22.693512 unified_planning-1.0.0.29.dev1/unified_planning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-21 08:18:22.000000 unified_planning-1.0.0.29.dev1/unified_planning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-07-21 08:18:22.000000 unified_planning-1.0.0.29.dev1/unified_planning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 08:18:22.000000 unified_planning-1.0.0.29.dev1/unified_planning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-21 08:18:22.000000 unified_planning-1.0.0.29.dev1/unified_planning.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-21 08:18:22.000000 unified_planning-1.0.0.29.dev1/unified_planning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 08:18:22.000000 unified_planning-1.0.0.29.dev1/unified_planning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.065088 unified_planning-1.0.0.6.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-17 07:51:10.065088 unified_planning-1.0.0.6.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 07:51:10.065088 unified_planning-1.0.0.6.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.025088 unified_planning-1.0.0.6.dev1/unified_planning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.025088 unified_planning-1.0.0.6.dev1/unified_planning/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/cmd/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/cmd/up.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.029088 unified_planning-1.0.0.6.dev1/unified_planning/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.029088 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/bounded_types_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/compilers_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19001 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19106 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/ma_conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/ma_disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17381 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/negative_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14003 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/quantifiers_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/state_invariants_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/tarski_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29926 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20771 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/credits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48595 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/meta_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.029088 unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/anytime_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/oneshot_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/plan_repairer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/replanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/oversubscription_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/pddl_anytime_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18248 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/pddl_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10455 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/replanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12778 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35416 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/engines/sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.033088 unified_planning-1.0.0.6.dev1/unified_planning/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/grpc/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.033088 unified_planning-1.0.0.6.dev1/unified_planning/grpc/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/grpc/generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20618 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/grpc/generated/unified_planning_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38742 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/grpc/proto_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38783 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/grpc/proto_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.033088 unified_planning-1.0.0.6.dev1/unified_planning/interop/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/interop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/interop/from_tarski.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18068 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/interop/to_tarski.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.033088 unified_planning-1.0.0.6.dev1/unified_planning/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14734 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/io/anml_grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41471 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/io/anml_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/io/anml_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39290 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/io/ma_pddl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77329 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/io/pddl_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40589 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/io/pddl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.037088 unified_planning-1.0.0.6.dev1/unified_planning/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/abstract_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29564 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/contingent_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/delta_stn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18666 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28717 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/fluent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17991 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/fnode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.037088 unified_planning-1.0.0.6.dev1/unified_planning/model/htn/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/htn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/htn/hierarchical_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/htn/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/htn/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/htn/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8843 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/htn/task_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13510 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.037088 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/actions_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/agents_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/fluents_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/initial_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/objects_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/time_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/timed_conds_effs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/user_types_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.037088 unified_planning-1.0.0.6.dev1/unified_planning/model/multi_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/multi_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/multi_agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/multi_agent/ma_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19329 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/multi_agent/ma_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43540 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/problem_kind.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.037088 unified_planning-1.0.0.6.dev1/unified_planning/model/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/scheduling/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/scheduling/chronicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/scheduling/scheduling_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.041088 unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/type_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.041088 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/dnf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/fluents_substituter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/free_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/identitydag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/linear_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/names_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/operators_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/quantifier_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17069 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/state_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/substituter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13657 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24752 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/usertype_fluents_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.041088 unified_planning-1.0.0.6.dev1/unified_planning/plans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plans/contingent_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plans/hierarchical_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plans/partial_order_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plans/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plans/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plans/sequential_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20055 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plans/stn_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plans/time_triggered_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.045088 unified_planning-1.0.0.6.dev1/unified_planning/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plot/causal_graph_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31499 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plot/plan_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/plot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30679 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.049088 unified_planning-1.0.0.6.dev1/unified_planning/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/basic.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/basic_conditional.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/connected_locations.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/constants.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/constants_no_variable_duration.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/durative_goals.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/forall.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/hydrone.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/match.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/match_int_id.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/match_test_parser.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/simple_mais.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/anml/tils.anml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.021088 unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/colorballs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/logistic_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/minimals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13633 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/multi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40351 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/realistic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/scheduling/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/scheduling/jobshop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/tamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37280 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/examples/testing_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.021088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    34291 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    33635 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-PCP/
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-PCP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Rover/
+-rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Satellite/
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.053088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/
+-rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Childsnack/
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Depots/
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/
+-rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Entertainment/
+-rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Factories-simple/
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Hiking/
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/
+-rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)   189505 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    33123 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    36329 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.057088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Robot/
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Robot/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Snake/
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Towers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Towers/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Woodworking/
+-rw-r--r--   0 runner    (1001) docker     (123)    34612 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/citycar/
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/citycar/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/citycar/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/counters/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/counters/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/counters/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/counters/problem2.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/depot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/depot/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/depot/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/enhsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/htn-transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/htn-transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/htn-transport/problem.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/matchcellar/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/matchcellar/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/matchcellar/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/miconic/
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/miconic/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/miconic/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/robot_fastener/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/robot_fastener/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.061088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/safe_road/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/safe_road/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/safe_road/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.065088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/sailing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/sailing/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/sailing/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.065088 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/visit_precedence/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/visit_precedence/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    27054 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_anml_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_anml_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_anytime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_bounded_types_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_compilers_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_compilers_quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_contingent_pddl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_credits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_dnf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_expression_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17057 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_htn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_infix_notation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_ma_conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_ma_disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_multi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_negative_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_partial_order_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34650 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_pddl_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14880 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_pddl_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15206 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25295 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18899 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_protobuf_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_pyperplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_quantifier_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_replanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25431 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_simulated_effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_state_invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_stn_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_substituter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_tamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_tarski_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_tarski_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13076 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_trajectory_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_trajectory_constraints_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_usertype_fluents_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/test/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-17 07:51:06.000000 unified_planning-1.0.0.6.dev1/unified_planning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:51:10.025088 unified_planning-1.0.0.6.dev1/unified_planning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-17 07:51:09.000000 unified_planning-1.0.0.6.dev1/unified_planning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14727 2023-07-17 07:51:10.000000 unified_planning-1.0.0.6.dev1/unified_planning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 07:51:09.000000 unified_planning-1.0.0.6.dev1/unified_planning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-17 07:51:09.000000 unified_planning-1.0.0.6.dev1/unified_planning.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-17 07:51:09.000000 unified_planning-1.0.0.6.dev1/unified_planning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 07:51:09.000000 unified_planning-1.0.0.6.dev1/unified_planning.egg-info/top_level.txt
```

### Comparing `unified_planning-1.0.0.29.dev1/LICENSE` & `unified_planning-1.0.0.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/PKG-INFO` & `unified_planning-1.0.0.6.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unified_planning
-Version: 1.0.0.29.dev1
+Version: 1.0.0.6.dev1
 Summary: Unified Planning Framework
 Home-page: https://www.aiplan4eu-project.eu
 Author: AIPlan4EU Project
 Author-email: aiplan4eu@fbk.eu
 License: APACHE
 Description: Unified Planning: A library that makes it easy to formulate planning problems and to invoke automated planners.
 Keywords: planning logic STRIPS RDDL
```

### Comparing `unified_planning-1.0.0.29.dev1/README.md` & `unified_planning-1.0.0.6.dev1/README.md`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/setup.py` & `unified_planning-1.0.0.6.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,25 +21,25 @@
     install_requires=["pyparsing", "networkx"],
     extras_require={
         "dev": ["tarski[arithmetic]", "pytest", "pytest-cov", "mypy"],
         "grpc": ["grpcio", "grpcio-tools", "grpc-stubs"],
         "tarski": ["tarski[arithmetic]"],
         "pyperplan": ["up-pyperplan==1.0.0"],
         "tamer": ["up-tamer==1.0.0"],
-        "enhsp": ["up-enhsp==0.0.17"],
+        "enhsp": ["up-enhsp==0.0.16"],
         "fast-downward": ["up-fast-downward==0.2.3"],
         "lpg": ["up-lpg==0.0.7"],
         "fmap": ["up-fmap==0.0.7"],
         "aries": ["up-aries>=0.0.8"],
         "symk": ["up-symk>=0.0.3"],
         "engines": [
             "tarski[arithmetic]",
             "up-pyperplan==1.0.0",
             "up-tamer==1.0.0",
-            "up-enhsp==0.0.17",
+            "up-enhsp==0.0.16",
             "up-fast-downward==0.2.3",
             "up-lpg==0.0.7",
             "up-fmap==0.0.7",
             "up-aries>=0.0.8",
             "up-symk>=0.0.3",
         ],
         "plot": ["plotly", "matplotlib", "kaleido", "pygraphviz", "pandas"],
```

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/cmd/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/cmd/arg_parser.py` & `unified_planning-1.0.0.6.dev1/unified_planning/cmd/arg_parser.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/cmd/up.py` & `unified_planning-1.0.0.6.dev1/unified_planning/cmd/up.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/bounded_types_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/bounded_types_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/compilers_pipeline.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/compilers_pipeline.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/conditional_effects_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/conditional_effects_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/grounder.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/ma_conditional_effects_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/ma_conditional_effects_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/ma_disjunctive_conditions_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/ma_disjunctive_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/negative_conditions_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/negative_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/quantifiers_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/quantifiers_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/state_invariants_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/state_invariants_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/tarski_grounder.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/tarski_grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/compilers/utils.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/compilers/utils.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/credits.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/credits.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/engine.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/engine.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/factory.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/factory.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/meta_engine.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/meta_engine.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/mixins/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/mixins/anytime_planner.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/anytime_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/mixins/compiler.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,19 +29,14 @@
     DISJUNCTIVE_CONDITIONS_REMOVING = auto()
     NEGATIVE_CONDITIONS_REMOVING = auto()
     QUANTIFIERS_REMOVING = auto()
     TRAJECTORY_CONSTRAINTS_REMOVING = auto()
     USERTYPE_FLUENTS_REMOVING = auto()
     BOUNDED_TYPES_REMOVING = auto()
     STATE_INVARIANTS_REMOVING = auto()
-    MA_SINGLE_AGENT_PROJECTION = auto()
-    MA_CENTRALIZATION = auto()
-    MA_SL_ROBUSTNESS_VERIFICATION = auto()
-    MA_SL_SOCIAL_LAW = auto()
-    SA_MA_CONVERSION = auto()
 
 
 class CompilerMixin(ABC):
     """Generic class for a compiler defining it's interface."""
 
     def __init__(self, default: Optional[CompilationKind] = None):
         self._default = default
```

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/mixins/oneshot_planner.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/oneshot_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/mixins/plan_repairer.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/plan_repairer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/mixins/plan_validator.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/plan_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/mixins/portfolio.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/portfolio.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/mixins/replanner.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/replanner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/mixins/sequential_simulator.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/mixins/sequential_simulator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/oversubscription_planner.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/oversubscription_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/parallel.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/parallel.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/pddl_anytime_planner.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/pddl_anytime_planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
             plan is generated and added to the Queue.
         - writer.last_plan_found: The last complete plan found and parsed.
         """
         assert isinstance(self._writer, PDDLWriter)
         for l in planner_output.splitlines():
             if self._starting_plan_str() in l:
                 writer.storing = True
-            elif writer.storing and self._ending_plan_str() in l:
+            elif self._ending_plan_str() in l:
                 plan_str = "\n".join(writer.current_plan)
                 plan = self._plan_from_str(
                     writer.problem, plan_str, self._writer.get_item_named
                 )
                 res = PlanGenerationResult(
                     PlanGenerationResultStatus.INTERMEDIATE,
                     plan=plan,
```

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/pddl_planner.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/pddl_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/plan_validator.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/plan_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/replanner.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/replanner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/results.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/results.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/engines/sequential_simulator.py` & `unified_planning-1.0.0.6.dev1/unified_planning/engines/sequential_simulator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/environment.py` & `unified_planning-1.0.0.6.dev1/unified_planning/environment.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/exceptions.py` & `unified_planning-1.0.0.6.dev1/unified_planning/exceptions.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/grpc/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/grpc/converter.py` & `unified_planning-1.0.0.6.dev1/unified_planning/grpc/converter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/grpc/generated/unified_planning_pb2.py` & `unified_planning-1.0.0.6.dev1/unified_planning/grpc/generated/unified_planning_pb2.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py` & `unified_planning-1.0.0.6.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/grpc/proto_reader.py` & `unified_planning-1.0.0.6.dev1/unified_planning/grpc/proto_reader.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/grpc/proto_writer.py` & `unified_planning-1.0.0.6.dev1/unified_planning/grpc/proto_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/interop/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/interop/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/interop/from_tarski.py` & `unified_planning-1.0.0.6.dev1/unified_planning/interop/from_tarski.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/interop/to_tarski.py` & `unified_planning-1.0.0.6.dev1/unified_planning/interop/to_tarski.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/io/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/io/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/io/anml_grammar.py` & `unified_planning-1.0.0.6.dev1/unified_planning/io/anml_grammar.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 
 
 # ANMl keywords definition as tokens
 TK_COMMA = ","
 TK_SEMI = ";"
 TK_COLON = ":"
 TK_ASSIGN = ":="
-TKS_INCREASE = (":+=", ":increase")
-TKS_DECREASE = (":-=", ":decrease")
+TK_INCREASE = ":+="
+TK_DECREASE = ":-="
 TK_IN_ASSIGN = ":in"
 TK_ANNOTATION = "::"
 TK_L_BRACE = "{"
 TK_R_BRACE = "}"
 TK_L_BRACKET = "["
 TK_R_BRACKET = "]"
 TK_L_PARENTHESIS = "("
@@ -96,28 +96,26 @@
 TK_XOR = "xor"
 TK_IMPLIES = "implies"
 TK_NOT = "not"
 TK_TRUE = "true"
 TK_FALSE = "false"
 TK_COMMENT = "//"
 TK_WHEN = "when"
-TK_INFINITY = "infinity"
 
 
 class ANMLGrammar:
     """
     This class defines the grammar used from the :class:`~unified_planning.io.ANMLReader`
     to parse a :class:`~unified_planning.model.Problem` from an ANML file.
     """
 
     def __init__(self):
 
         # Data structures to populate while parsing
         self.types: List[ParseResults] = []
-        self.constant_fluents: List[ParseResults] = []
         self.fluents: List[ParseResults] = []
         self.actions: List[ParseResults] = []
         self.objects: List[ParseResults] = []
         self.timed_assignments_or_goals: List[ParseResults] = []
         self.timed_assignment_or_goal: List[ParseResults] = []
 
         # Base Expression elements
@@ -168,17 +166,16 @@
             ],
         )
         boolean_expression <<= infix_notation(
             quantified_expression | relations_expression | boolean_const,
             [
                 (TK_NOT, 1, OpAssoc.RIGHT),
                 (one_of([TK_AND, TK_OR, TK_XOR]), 2, OpAssoc.LEFT, group_binary),
-                (TK_IMPLIES, 2, OpAssoc.RIGHT, group_binary),
                 (
-                    one_of([TK_ASSIGN, *TKS_INCREASE, *TKS_DECREASE]),
+                    one_of([TK_ASSIGN, TK_INCREASE, TK_DECREASE]),
                     2,
                     OpAssoc.LEFT,
                     group_binary,
                 ),
             ],
         )
         conditional_expression = Forward()
@@ -235,36 +232,19 @@
         identifier_list = identifier - ZeroOrMore(Suppress(TK_COMMA) - identifier)
         primitive_type = (
             set_results_name(Literal(TK_BOOLEAN), "name")
             | (
                 set_results_name(Literal(TK_INTEGER), "name")
                 - Optional(
                     Group(
-                        (
-                            (
-                                Suppress(TK_L_BRACKET)
-                                - set_results_name(integer, "left_bound")
-                            )
-                            | (
-                                Suppress(TK_L_PARENTHESIS)
-                                - Suppress("-")
-                                - set_results_name(Literal(TK_INFINITY), "left_bound")
-                            )
-                        )
+                        Suppress(TK_L_BRACKET)
+                        - set_results_name(integer, "left_bound")
                         - Suppress(TK_COMMA)
-                        - (
-                            (
-                                set_results_name(integer, "right_bound")
-                                - Suppress(TK_R_BRACKET)
-                            )
-                            | (
-                                set_results_name(Literal(TK_INFINITY), "right_bound")
-                                - Suppress(TK_R_PARENTHESIS)
-                            )
-                        )
+                        - set_results_name(integer, "right_bound")
+                        - Suppress(TK_R_BRACKET)
                     )
                 )
             )
             | (
                 set_results_name(TK_FLOAT, "name")
                 - Optional(
                     Group(
@@ -284,35 +264,16 @@
             - set_results_name(Group(identifier_list), "names")
         )
         set_parse_action(instance_decl, self.objects.append)
 
         parameter_list = Optional(Group(Group(type_ref) - identifier)) - ZeroOrMore(
             Suppress(TK_COMMA) - Group(Group(type_ref) - identifier)
         )
-        constant_decl = (
-            Suppress(TK_CONSTANT)
-            - set_results_name(type_ref, "type")
-            - set_results_name(identifier, "name")
-            - set_results_name(
-                Group(
-                    Optional(
-                        Suppress(TK_L_PARENTHESIS)
-                        - parameter_list
-                        - Suppress(TK_R_PARENTHESIS)
-                    )
-                ),
-                "parameters",
-            )
-            - set_results_name(
-                Optional(Suppress(TK_ASSIGN) - Group(expression)), "init"
-            )
-        )
-        set_parse_action(constant_decl, self.constant_fluents.append)
         fluent_decl = (
-            Suppress(TK_FLUENT)
+            Suppress(one_of([TK_FLUENT, TK_CONSTANT]))
             - set_results_name(type_ref, "type")
             - set_results_name(identifier, "name")
             - set_results_name(
                 Group(
                     Optional(
                         Suppress(TK_L_PARENTHESIS)
                         - parameter_list
@@ -343,27 +304,26 @@
                 (
                     Group(temporal_expression)
                     + Optional(Suppress(TK_COMMA) + Group(temporal_expression))
                 )
             )
             + one_of([TK_R_BRACKET, TK_R_PARENTHESIS])
         )
-        quantified_expression_def = Group(
+        quantified_expression <<= Group(
             one_of([TK_FORALL, TK_EXISTS])
             - Suppress(TK_L_PARENTHESIS)
             - set_results_name(Group(parameter_list), "quantifier_variables")
             - Suppress(TK_R_PARENTHESIS)
             - Suppress(TK_L_BRACE)
             - set_results_name(
-                Group(OneOrMore(expression - Suppress(TK_SEMI))),
+                Group(OneOrMore(boolean_expression - Suppress(TK_SEMI))),
                 "quantifier_body",
             )
             - Suppress(TK_R_BRACE)
         )
-        quantified_expression <<= infix_notation(quantified_expression_def, [])
 
         # Standalone expressions are defined to handle differently expressions
         # defined inside an action from the expressions defined outside an action
         standalone_timed_expression = timed_expression.copy()
         set_parse_action(
             standalone_timed_expression, self.timed_assignment_or_goal.append
         )
@@ -380,15 +340,14 @@
             standalone_timed_expression
             | standalone_expression_block
             | TK_L_BRACE - goal_body - TK_R_BRACE
         )
         anml_stmt = (
             instance_decl
             | type_decl
-            | constant_decl
             | fluent_decl
             | action_decl
             | standalone_expression_block
             | goal_decl
             | standalone_timed_expression
         )
```

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/io/anml_reader.py` & `unified_planning-1.0.0.6.dev1/unified_planning/io/anml_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 from collections import OrderedDict
 import unified_planning as up
 import networkx as nx
 from unified_planning.io.anml_grammar import (
     TK_ALL,
     TK_AND,
     TK_ASSIGN,
-    TKS_DECREASE,
+    TK_DECREASE,
     TK_DIV,
     TK_DURATION,
     TK_END,
     TK_EQUALS,
     TK_FALSE,
     TK_FORALL,
     TK_EXISTS,
     TK_GE,
     TK_GT,
     TK_IMPLIES,
-    TKS_INCREASE,
+    TK_INCREASE,
     TK_L_BRACKET,
     TK_L_PARENTHESIS,
     TK_LE,
     TK_LT,
     TK_MINUS,
     TK_NOT,
     TK_NOT_EQUALS,
@@ -48,15 +48,14 @@
     TK_TIMES,
     TK_TRUE,
     TK_WHEN,
     TK_XOR,
     ANMLGrammar,
     TK_BOOLEAN,
     TK_INTEGER,
-    TK_INFINITY,
     TK_FLOAT,
 )
 from unified_planning.environment import Environment, get_environment
 from unified_planning.exceptions import ANMLSyntaxError, UPUnsupportedProblemTypeError
 from unified_planning.model import (
     DurationInterval,
     Effect,
@@ -92,17 +91,14 @@
         * ``duration == expression;``
         * ``duration := expression;``
         * ``duration CT expression and duration CT expression``, where ``CT`` are Compare Tokens, so ``>``, ``>=``, ``<`` and ``<=``.
 
         All the other ways to define the duration of an Action are not supported.
     #. Statements containing both conditions and effects are **not** supported ( ``(at(l_from) == true) := false);`` or ``(at(l_from) == true) and (at(l_from) := false);`` ).
     #. Quantifier body does not support intervals, they can only be defined outside.
-    #. Forall over the assignments are not nested.
-    #. Only one effect can be specified in a forall over assignments.
-    #. No conditions can be specified ina  forall over assignments, 2 different foralls must be specified.
     #. Conditional effects are not supported inside an expression block.
     """
 
     def __init__(self, env: Optional[Environment] = None):
         self._env = get_environment(env)
         self._em = self._env.expression_manager
         self._tm = self._env.type_manager
@@ -144,26 +140,14 @@
         self._problem = up.model.Problem(
             problem_name,
             self._env,
             initial_defaults={self._tm.BoolType(): self._em.FALSE()},
         )
         types_map: Dict[str, "up.model.Type"] = self._create_types_map(grammar.types)
 
-        self._constant_fluents: Set["up.model.Fluent"] = set()
-
-        for fluent_res in grammar.constant_fluents:
-            (up_fluent, initial_default) = self._parse_fluent(fluent_res, types_map)
-            if initial_default is not None:
-                self._problem.add_fluent(
-                    up_fluent, default_initial_value=initial_default
-                )
-            else:
-                self._problem.add_fluent(up_fluent)
-            self._constant_fluents.add(up_fluent)
-
         for fluent_res in grammar.fluents:
             (up_fluent, initial_default) = self._parse_fluent(fluent_res, types_map)
             if initial_default is not None:
                 self._problem.add_fluent(
                     up_fluent, default_initial_value=initial_default
                 )
             else:
@@ -207,21 +191,14 @@
                     interval_and_expressions_res[0],
                     expression,
                     params,
                     types_map,
                     global_start,
                     global_end,
                 )
-        # check that every fluent defined as a constant is a static fluent
-        static_fluents = self._problem.get_static_fluents()
-        for constant_fluent in self._constant_fluents:
-            if constant_fluent not in static_fluents:
-                raise ANMLSyntaxError(
-                    f"The constant {constant_fluent} is modified in the problem."
-                )
         return self._problem
 
     def parse_problem(
         self,
         problem_filename: Union[str, Sequence[str]],
         problem_name: Optional[str] = None,
     ) -> "up.model.Problem":
@@ -315,41 +292,34 @@
         interval: ParseResults,
         expression: ParseResults,
         parameters: Dict[str, "Parameter"],
         types_map: Dict[str, "Type"],
         global_start: "Timing",
         global_end: "Timing",
     ):
-        relevant_words = {TK_DURATION, TK_ASSIGN, *TKS_INCREASE, *TKS_DECREASE, TK_WHEN}
+        relevant_words = {TK_DURATION, TK_ASSIGN, TK_INCREASE, TK_DECREASE, TK_WHEN}
         found_words = find_strings(expression, relevant_words)
         f_duration = TK_DURATION in found_words
         f_when = TK_WHEN in found_words
         f_assign = TK_ASSIGN in found_words
-        f_increase = any(tk_increase in found_words for tk_increase in TKS_INCREASE)
-        f_decrease = any(tk_decrease in found_words for tk_decrease in TKS_DECREASE)
+        f_increase = TK_INCREASE in found_words
+        f_decrease = TK_DECREASE in found_words
         if f_duration:
             raise ANMLSyntaxError("duration keyword can't be used outside of an action")
         if f_when or f_assign or f_increase or f_decrease:  # effect
             interval_and_exp = ParseResults([interval, expression])
             up_timing, up_effect = self._parse_assignment(
-                interval_and_exp,
-                parameters,
-                types_map,
-                is_global=True,
+                interval_and_exp, parameters, types_map, is_global=True
             )
             if (
                 up_timing == global_start
                 and not up_effect.is_conditional()
                 and up_effect.is_assignment()
             ):
-                if up_effect.is_forall():
-                    for e in up_effect.expand_effect(self._problem):
-                        self._problem.set_initial_value(e.fluent, e.value)
-                else:
-                    self._problem.set_initial_value(up_effect.fluent, up_effect.value)
+                self._problem.set_initial_value(up_effect.fluent, up_effect.value)
             else:
                 self._problem._add_effect_instance(up_timing, up_effect)
         else:  # condition
             up_interval = self._parse_interval(
                 interval, parameters, types_map, is_global=True
             )
             goal = self._parse_expression(expression, parameters, types_map)
@@ -366,42 +336,33 @@
         if name == TK_BOOLEAN:
             return self._tm.BoolType()
         elif name in (TK_INTEGER, TK_FLOAT):
             lower_bound, upper_bound = None, None
             if len(type_res) == 2:
                 _p: Dict[str, "up.model.Parameter"] = {}
                 interval = type_res[1]
-                lb_exp = interval[0]
-                if lb_exp != TK_INFINITY:
-                    lower_bound_exp = self._parse_expression(
-                        lb_exp, parameters=_p, types_map=types_map
-                    )
-                    if (
-                        lower_bound_exp.is_int_constant()
-                        or lower_bound_exp.is_real_constant()
-                    ):
-                        lower_bound = lower_bound_exp.constant_value()
-                    else:
-                        raise ANMLSyntaxError(
-                            f"bounds of type {type_res} must be integer or real constants"
-                        )
-                ub_exp = interval[1]
-                if ub_exp != TK_INFINITY:
-                    upper_bound_exp = self._parse_expression(
-                        ub_exp, parameters=_p, types_map=types_map
+                lower_bound_exp = self._parse_expression(
+                    interval[0], parameters=_p, types_map=types_map
+                )
+                upper_bound_exp = self._parse_expression(
+                    interval[1], parameters=_p, types_map=types_map
+                )
+                if (
+                    lower_bound_exp.is_int_constant()
+                    or lower_bound_exp.is_real_constant()
+                ) and (
+                    upper_bound_exp.is_int_constant()
+                    or upper_bound_exp.is_real_constant()
+                ):
+                    lower_bound = lower_bound_exp.constant_value()
+                    upper_bound = upper_bound_exp.constant_value()
+                else:
+                    raise ANMLSyntaxError(
+                        f"bounds of type {type_res} must be integer of real constants"
                     )
-                    if (
-                        upper_bound_exp.is_int_constant()
-                        or upper_bound_exp.is_real_constant()
-                    ):
-                        upper_bound = upper_bound_exp.constant_value()
-                    else:
-                        raise ANMLSyntaxError(
-                            f"bounds of type {type_res} must be integer or real constants"
-                        )
             else:
                 assert len(type_res) == 1, "Parse error"
             if name == TK_INTEGER:
                 if isinstance(lower_bound, Fraction) or isinstance(
                     upper_bound, Fraction
                 ):
                     raise ANMLSyntaxError(
@@ -469,27 +430,21 @@
         self,
         action: "up.model.DurativeAction",
         action_body_res: ParseResults,
         action_parameters: Dict[str, "up.model.Parameter"],
         types_map: Dict[str, "Type"],
     ) -> None:
         for interval_and_exp in action_body_res:
-            relevant_words = {
-                TK_DURATION,
-                TK_ASSIGN,
-                *TKS_INCREASE,
-                *TKS_DECREASE,
-                TK_WHEN,
-            }
+            relevant_words = {TK_DURATION, TK_ASSIGN, TK_INCREASE, TK_DECREASE, TK_WHEN}
             found_words = find_strings(interval_and_exp, relevant_words)
             f_duration = TK_DURATION in found_words
             f_when = TK_WHEN in found_words
             f_assign = TK_ASSIGN in found_words
-            f_increase = any(tk_increase in found_words for tk_increase in TKS_INCREASE)
-            f_decrease = any(tk_decrease in found_words for tk_decrease in TKS_DECREASE)
+            f_increase = TK_INCREASE in found_words
+            f_decrease = TK_DECREASE in found_words
 
             if f_duration:  # handle duration
                 if f_when:
                     raise ANMLSyntaxError(
                         "expressions containing the duration can't be conditional"
                     )
                 if f_increase:
@@ -608,20 +563,17 @@
 
     def _parse_interval(
         self,
         interval_res: ParseResults,
         parameters: Dict[str, "Parameter"],
         types_map: Dict[str, "Type"],
         is_global: bool = False,
-        is_constant: bool = False,
     ) -> Union["Timing", "TimeInterval"]:
         if len(interval_res) == 0:
             if is_global:
-                if is_constant:
-                    return GlobalStartTiming()
                 raise UPUnsupportedProblemTypeError(
                     "ANML constant initialization is currently not supported."
                 )
             else:
                 return StartTiming()
 
         contains_TK_ALL = TK_ALL in find_strings(interval_res, set((TK_ALL,)))
@@ -735,149 +687,83 @@
             return Timing(delay, timing.timepoint)
         else:
             raise UPUnsupportedProblemTypeError(
                 f"Timing parsed: {parsed_timing_exp}. UP currently only supports",
                 f" {TK_START} + constant, {TK_END} - constant or just a constant",
             )
 
-    def _check_conditional_intervals(
-        self,
-        interval_res: ParseResults,
-        condition_interval: ParseResults,
-        effect_interval: ParseResults,
-    ) -> ParseResults:
-        # interval_res is the interval defined outside the conditional block
-        # condition_interval is the interval defined before the condition
-        # effect_interval is the interval defined before the effect
-        res = None
-        if interval_res:
-            res = interval_res
-        if condition_interval and res is not None:
-            if str(condition_interval) != str(res):
-                raise UPUnsupportedProblemTypeError(
-                    "In conditional effect parsing the "
-                    + "condition time interval and the time interval outside the block are different, "
-                    + "this is not supported by the UP."
-                )
-        elif condition_interval:
-            res = condition_interval
-        if effect_interval and res is not None:
-            if str(effect_interval) != str(res):
-                raise UPUnsupportedProblemTypeError(
-                    "In conditional effect parsing the "
-                    + "condition time interval and the time interval outside the block are different, "
-                    + "this is not supported by the UP."
-                )
-        elif effect_interval:
-            res = effect_interval
-        if res is None:
-            return interval_res
-        return res
-
     def _parse_assignment(
         self,
         interval_and_effect: ParseResults,
         parameters: Dict[str, "up.model.Parameter"],
         types_map: Dict[str, "Type"],
         is_global: bool = False,
     ) -> Tuple["Timing", "Effect"]:
         interval_res = interval_and_effect[0]
         effect_res = interval_and_effect[1]
         if effect_res[0] == TK_WHEN:  # Conditional effect
             condition_interval = effect_res[1][0]
             condition_exp_res = effect_res[1][1]
             effect_interval = effect_res[2][0]
             effect_exp = effect_res[2][1][0]
+            if str(condition_interval) != str(effect_interval):
+                raise UPUnsupportedProblemTypeError(
+                    "In conditional effect parsing the "
+                    + "condition time interval and the effect time interval are different, "
+                    + "this is not supported by the UP."
+                )
+            if len(interval_res) > 0:
+                raise ANMLSyntaxError(
+                    "A conditional effect can not have an interval specified before the when keyword."
+                )
             condition = self._parse_expression(condition_exp_res, parameters, types_map)
-            interval_res = self._check_conditional_intervals(
-                interval_res, condition_interval, effect_interval
-            )
+            interval_res = condition_interval
         else:
             condition = self._em.TRUE()
             effect_exp = effect_res[0]
-        variables: Dict[str, "up.model.Variable"] = {}
-        if effect_exp[0] == TK_FORALL:  # Forall assignment
-            variables = dict(
-                (
-                    (n, Variable(n, t))
-                    for n, t in self._parse_parameters_def(
-                        effect_exp["quantifier_variables"], types_map
-                    ).items()
-                )
-            )
-            effect_exp = effect_exp[2]
-            if effect_exp[0] == TK_WHEN:  # Conditional effect
-                assert len(effect_exp) == 3, "Multiple expressions in forall assignment"
-                condition_interval = effect_exp[1][0]
-                condition_exp_res = effect_exp[1][1]
-                effect_interval = effect_exp[2][0]
-                effect_exp = effect_exp[2][1][0]
-                interval_res = self._check_conditional_intervals(
-                    interval_res, condition_interval, effect_interval
-                )
-                condition = self._em.And(
-                    self._parse_expression(
-                        condition_exp_res, parameters, types_map, variables=variables
-                    ),
-                    condition,
-                )
-            else:
-                effect_exp = effect_exp[0]
+        up_interval = self._parse_interval(
+            interval_res, parameters, types_map, is_global
+        )
         fluent_ref = effect_exp[0]
         assignment_operator = effect_exp[1]
         assigned_expression = effect_exp[2]
-        up_fluent = self._parse_expression(
-            fluent_ref, parameters, types_map, variables=variables
-        )
+        up_fluent = self._parse_expression(fluent_ref, parameters, types_map)
         if not up_fluent.is_fluent_exp():
             raise ANMLSyntaxError("left side of the assignment is not a valid fluent")
-        is_constant = up_fluent.fluent() in self._constant_fluents
-        up_interval = self._parse_interval(
-            interval_res, parameters, types_map, is_global, is_constant
-        )
-        up_value = self._parse_expression(
-            assigned_expression, parameters, types_map, variables=variables
-        )
+        up_value = self._parse_expression(assigned_expression, parameters, types_map)
         if assignment_operator == TK_ASSIGN:
             kind = EffectKind.ASSIGN
-        elif assignment_operator in TKS_INCREASE:
+        elif assignment_operator == TK_INCREASE:
             kind = EffectKind.INCREASE
-        elif assignment_operator in TKS_DECREASE:
+        elif assignment_operator == TK_DECREASE:
             kind = EffectKind.DECREASE
         else:
             raise NotImplementedError(
                 f"Currently the unified planning does not support the assignment operator {assignment_operator}"
             )
         if not isinstance(up_interval, Timing):
             raise UPUnsupportedProblemTypeError(
                 "An effect with a durative interval is not supported"
             )
-        return (
-            up_interval,
-            Effect(
-                up_fluent, up_value, condition, kind=kind, forall=variables.values()
-            ),
-        )
+        return (up_interval, Effect(up_fluent, up_value, condition, kind=kind))
 
     def _parse_expression(
         self,
         expression: Union[ParseResults, List, str],
         parameters: Dict[str, "up.model.Parameter"],
         types_map: Dict[str, "Type"],
         is_global: Optional[bool] = None,
-        variables: Optional[Dict[str, "up.model.Variable"]] = None,
     ) -> "up.model.FNode":
         # A string here means it is a number or a boolean token. To avoid code duplication, just
         # wrap it in a temporary list and let the stack management handle it.
         if isinstance(expression, str):
             expression = [expression]
-        vars = {} if variables is None else variables
-        stack: List[
-            Tuple[Union[ParseResults, List, str], bool, Dict[str, "Variable"]]
-        ] = [(expression, False, vars)]
+        stack: List[Tuple[Union[ParseResults, List], bool, Dict[str, "Variable"]]] = [
+            (expression, False, {})
+        ]
         solved: List[FNode] = []
         while len(stack) > 0:
             exp, already_expanded, vars = stack.pop()
             if already_expanded:
                 assert isinstance(exp, ParseResults) or isinstance(exp, List)
                 if len(exp) <= 1:
                     assert len(exp) == 1, "algorithm error"
@@ -931,16 +817,18 @@
                         )
                 elif len(exp) == 3:  # binary operator or parameters list
                     first_token = exp[0]
                     if isinstance(first_token, str) and first_token in (
                         TK_FORALL,
                         TK_EXISTS,
                     ):
-                        assert isinstance(exp, ParseResults) or isinstance(exp, list)
-                        quantified_expressions = [solved.pop() for _ in exp[2]]
+                        assert isinstance(exp, ParseResults)
+                        quantified_expressions = [
+                            solved.pop() for _ in exp["quantifier_body"]
+                        ]
                         solved.append(
                             self._operators[first_token](
                                 self._em.And(quantified_expressions), *vars.values()
                             )
                         )
                     else:
                         operator = exp[1]
@@ -982,50 +870,40 @@
             else:  # not solved
                 if isinstance(exp, ParseResults) or isinstance(exp, List):
                     first_token = exp[0]
                     if isinstance(first_token, str) and first_token in (
                         TK_FORALL,
                         TK_EXISTS,
                     ):  # quantifier
-                        assert isinstance(exp, ParseResults) or isinstance(
-                            exp, list
-                        ), f"{exp} <- {expression}, {type(exp)}"
-                        name_type = self._parse_parameters_def(exp[1], types_map)
+                        assert isinstance(exp, ParseResults)
+                        name_type = self._parse_parameters_def(
+                            exp["quantifier_variables"], types_map
+                        )
                         new_vars = {n: Variable(n, t) for n, t in name_type.items()}
                         stack.append((exp, True, new_vars))
                         all_vars = vars.copy()
                         all_vars.update(new_vars)
-                        for e in exp[2]:
+                        for e in exp["quantifier_body"]:
                             stack.append((e, False, all_vars))
                     else:
                         stack.append((exp, True, vars))
                         for e in exp:
                             if not isinstance(e, str):  # nested structure
                                 if len(e) > 0:
                                     stack.append((e, False, vars))
-                            else:
-                                assert isinstance(e, str)
-                                if (
-                                    e.isnumeric()
-                                    or is_float(e)
-                                    or e == TK_TRUE
-                                    or e == TK_FALSE
-                                ):
-                                    stack.append((e, False, vars))
+                            elif e.isnumeric():  # int
+                                solved.append(self._em.Int(int(e)))
+                            elif is_float(e):  # float
+                                solved.append(self._em.Real(Fraction(float(e))))
+                            elif e == TK_TRUE:  # true
+                                solved.append(self._em.TRUE())
+                            elif e == TK_FALSE:  # false
+                                solved.append(self._em.FALSE())
                 elif isinstance(exp, str):
-                    if exp.isnumeric():  # int
-                        solved.append(self._em.Int(int(exp)))
-                    elif is_float(exp):  # float
-                        solved.append(self._em.Real(Fraction(float(exp))))
-                    elif exp == TK_TRUE:  # true
-                        solved.append(self._em.TRUE())
-                    elif exp == TK_FALSE:  # false
-                        solved.append(self._em.FALSE())
-                    else:
-                        raise ANMLSyntaxError(f"Unable to solve {exp}")
+                    assert False, "problem, should not have strings here"
                 else:
                     raise NotImplementedError
         assert len(stack) == 0
         assert len(solved) == 1, f"{expression}"
         res = solved.pop()
         return res.simplify()
```

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/io/anml_writer.py` & `unified_planning-1.0.0.6.dev1/unified_planning/io/anml_writer.py`

 * *Files 7% similar despite different names*

```diff
@@ -120,37 +120,29 @@
 
     def convert(self, expression):
         """Converts the given expression to a ANML string."""
         return self.walk(
             self.simplifier.simplify(expression)
         )  # NOTE maybe the converter could remove the first and last char, if they are '(' and ')'
 
-    def convert_forall_variables(self, vars):
-        """Converts the given variables to a ANML string."""
-        vars_string_gen = (
-            f"{_get_anml_name(v.type, self._names_mapping)} {_get_anml_name(v, self._names_mapping)}"
-            for v in vars
-        )
-        return f"{', '.join(vars_string_gen)}"
-
     def walk_exists(self, expression, args):
         assert len(args) == 1
         vars_string_gen = (
             f"{_get_anml_name(v.type, self._names_mapping)} {_get_anml_name(v, self._names_mapping)}"
             for v in expression.variables()
         )
-        return f'(exists({", ".join(vars_string_gen)}) {{ {args[0]}; }})'
+        return f'(exists({", ".join(vars_string_gen)}) {{ {args[0]} }})'
 
     def walk_forall(self, expression, args):
         assert len(args) == 1
         vars_string_gen = (
             f"{_get_anml_name(v.type, self._names_mapping)} {_get_anml_name(v, self._names_mapping)}"
             for v in expression.variables()
         )
-        return f'(forall({", ".join(vars_string_gen)}) {{ {args[0]}; }})'
+        return f'(forall({", ".join(vars_string_gen)}) {{ {args[0]} }})'
 
     def walk_variable_exp(self, expression, args):
         assert len(args) == 0
         return _get_anml_name(expression.variable(), self._names_mapping)
 
     def walk_and(self, expression, args):
         assert len(args) > 1
@@ -166,15 +158,15 @@
 
     def walk_implies(self, expression, args):
         assert len(args) == 2
         return f"({args[0]} implies {args[1]})"
 
     def walk_iff(self, expression, args):
         assert len(args) == 2
-        return f"({args[0]} == {args[1]})"
+        return f"({args[0]} iff {args[1]})"
 
     def walk_fluent_exp(self, expression, args):
         if len(args) == 0:
             return self._names_mapping[expression.fluent()]
         else:
             return f'{self._names_mapping[expression.fluent()]}({", ".join(args)})'
 
@@ -402,40 +394,31 @@
         timing: Optional["up.model.Timing"] = None,
         spaces_from_left: int = 0,
     ) -> str:
         results: List[str] = []
         anml_timing = (
             self._convert_anml_timing(timing) if timing is not None else "start"
         )
-        results.append(f"[ {anml_timing} ] ")
-        if effect.is_forall():
-            vars = converter.convert_forall_variables(effect.forall)
-            spaces_from_left += 3
-            results.append(f'forall ({vars}){{\n{spaces_from_left*" "}')
         if effect.is_conditional():
-            spaces_from_left += 3
             results.append(
-                f'when {converter.convert(effect.condition)}\n{spaces_from_left*" "}{{'
+                f'when [ {anml_timing} ] {converter.convert(effect.condition)}\n{spaces_from_left*" "}{{'
             )
+        results.append(f"[ {anml_timing} ] ")
         results.append(converter.convert(effect.fluent))
         if effect.is_assignment():
             results.append(" := ")
         elif effect.is_increase():
             results.append(f" :increase ")
         elif effect.is_decrease():
             results.append(f" :decrease ")
         else:
             raise NotImplementedError
         results.append(f"{converter.convert(effect.value)};\n")
         if effect.is_conditional():
-            results.append(f'{spaces_from_left*" "}}};\n')
-            spaces_from_left -= 3
-        if effect.is_forall():
-            spaces_from_left -= 3
-            results.append(f'{spaces_from_left*" "}}};\n')
+            results.append(f'{spaces_from_left*" "}}}\n')
         return "".join(results)
 
     def _convert_anml_timing(self, timing: "up.model.Timing") -> str:
         time = "start" if timing.is_from_start() else "end"
         if timing.delay > 0:
             return f"{time} + {str(timing.delay)}"
         elif timing.delay == 0:
```

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/io/ma_pddl_writer.py` & `unified_planning-1.0.0.6.dev1/unified_planning/io/ma_pddl_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/io/pddl_reader.py` & `unified_planning-1.0.0.6.dev1/unified_planning/io/pddl_reader.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/io/pddl_writer.py` & `unified_planning-1.0.0.6.dev1/unified_planning/io/pddl_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/io/utils.py` & `unified_planning-1.0.0.6.dev1/unified_planning/io/utils.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/abstract_problem.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/abstract_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/action.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/action.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/contingent_problem.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/contingent_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/delta_stn.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/delta_stn.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/effect.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/effect.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/expression.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/expression.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/fluent.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/fluent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/fnode.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/fnode.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/htn/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/htn/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/htn/hierarchical_problem.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/htn/hierarchical_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/htn/method.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/htn/method.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/htn/ordering.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/htn/ordering.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/htn/task.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/htn/task.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/htn/task_network.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/htn/task_network.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/metrics.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/metrics.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/mixins/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/mixins/actions_set.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/actions_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/mixins/agents_set.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/agents_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/mixins/fluents_set.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/fluents_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/mixins/initial_state.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/initial_state.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/mixins/metrics.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/metrics.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/mixins/objects_set.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/objects_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/mixins/time_model.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/time_model.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/mixins/timed_conds_effs.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/timed_conds_effs.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/mixins/user_types_set.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/mixins/user_types_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/multi_agent/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/multi_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/multi_agent/agent.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/multi_agent/agent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/multi_agent/ma_environment.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/multi_agent/ma_environment.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/multi_agent/ma_problem.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/multi_agent/ma_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/object.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/object.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/operators.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/operators.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/parameter.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/parameter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/problem.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/problem.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,16 +387,16 @@
         :param goal: The expression that must be evaluated to `True` in the given `interval`.
         """
         assert (
             isinstance(goal, bool) or goal.environment == self._env
         ), "timed_goal does not have the same environment of the problem"
         if isinstance(interval, up.model.Timing):
             interval = up.model.TimePointInterval(interval)
-        if (interval.lower.is_from_end() and interval.lower.delay != 0) or (
-            interval.upper.is_from_end() and interval.upper.delay != 0
+        if (interval.lower.is_from_end() and interval.lower.delay > 0) or (
+            interval.upper.is_from_end() and interval.upper.delay > 0
         ):
             raise UPProblemDefinitionError(
                 "Problem timing can not be `end - k` with k > 0."
             )
         (goal_exp,) = self._env.expression_manager.auto_promote(goal)
         assert self._env.type_checker.get_type(goal_exp).is_bool_type()
         goals = self._timed_goals.setdefault(interval, [])
```

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/problem_kind.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/problem_kind.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/scheduling/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/scheduling/activity.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/scheduling/activity.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/scheduling/chronicle.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/scheduling/chronicle.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/scheduling/scheduling_problem.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/scheduling/scheduling_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/state.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/state.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/tamp/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/tamp/action.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/action.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/tamp/objects.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/objects.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/tamp/path.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/path.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/tamp/types.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/tamp/types.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/timing.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/timing.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/type_manager.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/type_manager.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/types.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/types.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/variable.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/variable.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/any.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/any.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/dag.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/dag.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/dnf.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/dnf.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/fluents_substituter.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/fluents_substituter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/free_vars.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/free_vars.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/generic.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/generic.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/identitydag.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/identitydag.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/linear_checker.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/linear_checker.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/names_extractor.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/names_extractor.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/operators_extractor.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/operators_extractor.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/quantifier_simplifier.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/quantifier_simplifier.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/simplifier.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/simplifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from fractions import Fraction
 from collections import OrderedDict
-from typing import Dict, List, Optional, Set, Union, cast
+from typing import Dict, List, Optional, Set, Union
 import unified_planning as up
 import unified_planning.environment
 import unified_planning.model.walkers as walkers
 from unified_planning.model.fnode import FNode
-from unified_planning.model.types import _UserType
 import unified_planning.model.operators as op
 
 
 class Simplifier(walkers.dag.DagWalker):
     """Performs basic simplifications of the input expression.
 
     Important NOTE:
@@ -281,19 +280,16 @@
 
         if sl.is_constant() and sr.is_constant():
             l = sl.constant_value()
             r = sr.constant_value()
             return self.manager.Bool(l == r)
         elif sl == sr:
             return self.manager.TRUE()
-        elif sl.type.is_user_type() and sr.type.is_user_type():
-            slt, srt = cast(_UserType, sl.type), cast(_UserType, sr.type)
-            if not slt.is_compatible(srt) and not srt.is_compatible(slt):
-                return self.manager.FALSE()
-        return self.manager.Equals(sl, sr)
+        else:
+            return self.manager.Equals(sl, sr)
 
     def walk_le(self, expression: FNode, args: List[FNode]) -> FNode:
         assert len(args) == 2
 
         sl = args[0]
         sr = args[1]
```

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/state_evaluator.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/state_evaluator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/substituter.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/substituter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/type_checker.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/type_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #
 
 
 from fractions import Fraction
 import unified_planning.model.types
 import unified_planning.environment
 import unified_planning.model.walkers as walkers
-from unified_planning.model.types import BOOL, TIME, _UserType
+from unified_planning.model.types import BOOL, TIME, _IntType, _RealType
 from unified_planning.model.fnode import FNode
 from unified_planning.model.operators import OperatorKind
 from unified_planning.exceptions import UPTypeError
 from typing import List, Optional, cast
 import math
 
 
@@ -355,21 +355,15 @@
                 return None
             elif (
                 t.is_user_type()
                 and t != x
                 and not t.is_compatible(x)
                 and not x.is_compatible(t)
             ):
-                # check if t and x have at least one common ancestor
-                t = cast(_UserType, t)
-                if x.is_user_type():
-                    x = cast(_UserType, x)
-                    x_ancestors = set(x.ancestors)
-                    if all(t_ancestor not in x_ancestors for t_ancestor in t.ancestors):
-                        return None
+                return None
             elif (t.is_int_type() or t.is_real_type()) and not (
                 x.is_int_type() or x.is_real_type()
             ):
                 return None
         return BOOL
 
     @walkers.handles(OperatorKind.DOT)
```

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/model/walkers/usertype_fluents_walker.py` & `unified_planning-1.0.0.6.dev1/unified_planning/model/walkers/usertype_fluents_walker.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/plans/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plans/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/plans/contingent_plan.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plans/contingent_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/plans/hierarchical_plan.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plans/hierarchical_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/plans/partial_order_plan.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plans/partial_order_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/plans/plan.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plans/plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/plans/schedule.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plans/schedule.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/plans/sequential_plan.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plans/sequential_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/plans/stn_plan.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plans/stn_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/plans/time_triggered_plan.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plans/time_triggered_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/plot/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/plot/causal_graph_plot.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plot/causal_graph_plot.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/plot/plan_plot.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plot/plan_plot.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/plot/utils.py` & `unified_planning-1.0.0.6.dev1/unified_planning/plot/utils.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/shortcuts.py` & `unified_planning-1.0.0.6.dev1/unified_planning/shortcuts.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/anml/connected_locations.anml` & `unified_planning-1.0.0.6.dev1/unified_planning/test/anml/connected_locations.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/anml/constants.anml` & `unified_planning-1.0.0.6.dev1/unified_planning/test/anml/constants.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/anml/constants_no_variable_duration.anml` & `unified_planning-1.0.0.6.dev1/unified_planning/test/anml/constants_no_variable_duration.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/anml/forall.anml` & `unified_planning-1.0.0.6.dev1/unified_planning/test/anml/forall.anml`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,17 @@
    forall(Location l2) {
       not precedes(l2, l) or visited(l2);
    };
 };
 
 instance Location l1, l2, l3;
 
-[start] forall(Location lx) {visited(lx) := false;};
+[start] visited(l1) := false;
+[start] visited(l2) := false;
+[start] visited(l3) := false;
 
 [start] precedes(l1, l2) := true;
 [start] precedes(l1, l3) := true;
 [start] precedes(l2, l3) := true;
 
 [start] precedes(l1, l1) := false;
```

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml` & `unified_planning-1.0.0.6.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/anml/hydrone.anml` & `unified_planning-1.0.0.6.dev1/unified_planning/test/anml/hydrone.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/anml/match.anml` & `unified_planning-1.0.0.6.dev1/unified_planning/test/anml/match.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/anml/match_int_id.anml` & `unified_planning-1.0.0.6.dev1/unified_planning/test/anml/match_int_id.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/anml/match_test_parser.anml` & `unified_planning-1.0.0.6.dev1/unified_planning/test/anml/match_test_parser.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/anml/simple_mais.anml` & `unified_planning-1.0.0.6.dev1/unified_planning/test/anml/simple_mais.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/examples/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/examples/hierarchical.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/examples/hierarchical.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/examples/minimals.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/examples/minimals.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/examples/multi_agent.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/examples/multi_agent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/examples/realistic.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/examples/realistic.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/examples/scheduling/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/examples/scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/examples/scheduling/examples.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/examples/scheduling/examples.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/examples/scheduling/jobshop.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/examples/scheduling/jobshop.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/examples/tamp.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/examples/tamp.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/examples/testing_variants.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/examples/testing_variants.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/__init__.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/citycar/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/citycar/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/citycar/problem.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/citycar/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/counters/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/counters/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/counters/problem2.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/counters/problem2.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/depot/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/depot/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/depot/problem.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/depot/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/enhsp.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/enhsp.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/htn-transport/domain.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/htn-transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/htn-transport/problem.hddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/htn-transport/problem.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/matchcellar/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/matchcellar/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/miconic/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/miconic/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/safe_road/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/safe_road/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/sailing/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/sailing/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl` & `unified_planning-1.0.0.6.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_anml_reader.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_anml_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,32 +9,29 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-import tempfile
 from typing import cast
 from unified_planning.shortcuts import *
 from unified_planning.model import DurativeAction
 from unified_planning.test import TestCase
-from unified_planning.io import ANMLReader, ANMLWriter
-from unified_planning.test.examples import get_example_problems
+from unified_planning.io import ANMLReader
 import os
 
 
 FILE_PATH = os.path.dirname(os.path.abspath(__file__))
 ANML_FILES_PATH = os.path.join(FILE_PATH, "anml")
 
 
 class TestANMLReader(TestCase):
     def setUp(self):
         TestCase.setUp(self)
-        self.problems = get_example_problems()
         self.start_timing = StartTiming()
         self.start_interval = TimePointInterval(self.start_timing)
         self.end_timing = EndTiming()
         self.global_start_timing = GlobalStartTiming()
         self.global_end_timing = GlobalEndTiming()
         self.all_interval = ClosedTimeInterval(self.start_timing, self.end_timing)
 
@@ -648,91 +645,7 @@
                 self.assertTrue(False)
 
         with open(problem_filename, "r", encoding="utf-8") as file:
             problem_str = file.read()
 
         problem_2 = reader.parse_problem_string(problem_str, problem_filename)
         self.assertEqual(problem, problem_2)
-
-    def test_safe_road_reader(self):
-        reader = ANMLReader()
-        problem_filename = os.path.join(ANML_FILES_PATH, "safe_road.anml")
-        problem = reader.parse_problem(problem_filename)
-
-        self.assertIsNotNone(problem)
-        self.assertEqual(len(problem.fluents), 2)
-        self.assertEqual(len(problem.actions), 2)
-        self.assertEqual(len(list(problem.objects(problem.user_type("location")))), 3)
-        self.assertEqual(len(problem.goals), 2)
-        self.assertEqual(len(problem.timed_goals), 0)
-        self.assertEqual(len(problem.timed_effects), 0)
-
-        check = cast(DurativeAction, problem.action("check"))
-        for interval, cond_list in check.conditions.items():
-            self.assertEqual(interval, self.start_interval)
-            self.assertEqual(len(cond_list), 1)
-        for timing, effect_list in check.effects.items():
-            self.assertEqual(timing, self.start_timing)
-            self.assertEqual(len(effect_list), 1)
-
-        nd = cast(DurativeAction, problem.action("natural_disaster"))
-        self.assertEqual(len(nd.conditions), 0)
-        for timing, effect_list in nd.effects.items():
-            if timing == self.start_timing:
-                self.assertEqual(len(effect_list), 1)
-                self.assertFalse(effect_list[0].is_forall())
-            elif timing == self.end_timing:
-                self.assertEqual(len(effect_list), 1)
-                self.assertTrue(effect_list[0].is_forall())
-            else:
-                self.assertTrue(False)
-
-        with open(problem_filename, "r", encoding="utf-8") as file:
-            problem_str = file.read()
-
-        problem_2 = reader.parse_problem_string(problem_str, problem_filename)
-        self.assertEqual(problem, problem_2)
-
-    def test_anml_io(self):
-        for example in self.problems.values():
-            problem = example.problem
-            problems_to_skip = []
-            if problem.name in problems_to_skip:
-                continue
-            kind = problem.kind
-            if not kind.has_action_based():
-                continue
-            with tempfile.TemporaryDirectory() as tempdir:
-                problem_filename = os.path.join(tempdir, "problem.anml")
-
-                w = ANMLWriter(problem)
-                w.write_problem(problem_filename)
-                reader = ANMLReader()
-                parsed_problem = reader.parse_problem(problem_filename)
-            self.assertEqual(len(problem.user_types), len(parsed_problem.user_types))
-            self.assertEqual(len(problem.actions), len(parsed_problem.actions))
-            for act, parsed_act in zip(problem.actions, parsed_problem.actions):
-                if isinstance(act, InstantaneousAction):
-                    conditions = (
-                        {TimePointInterval(StartTiming()): act.preconditions}
-                        if act.preconditions
-                        else {}
-                    )
-                    effects = {StartTiming(): act.effects} if act.effects else {}
-                else:
-                    assert isinstance(act, DurativeAction)
-                    conditions = act.conditions
-                    effects = act.effects
-                assert isinstance(parsed_act, DurativeAction)
-                if conditions != parsed_act.conditions:
-                    for i, cl in conditions.items():
-                        parsed_cl = parsed_act.conditions[i]
-                        self.assertEqual(len(cl), len(parsed_cl))
-                if effects != parsed_act.effects:
-                    for t, el in effects.items():
-                        parsed_el = parsed_act.effects[t]
-                        self.assertEqual(len(el), len(parsed_el))
-                        for eff, parsed_eff in zip(el, parsed_el):
-                            self.assertTrue(
-                                eff.is_conditional() == parsed_eff.is_conditional()
-                            )
-                            self.assertTrue(eff.is_forall() == parsed_eff.is_forall())
```

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_anml_writer.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_anml_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from unified_planning.shortcuts import *
 from unified_planning.test import TestCase, main, skipIfEngineNotAvailable
 from unified_planning.test.examples import get_example_problems
-from unified_planning.io import ANMLWriter, PDDLReader
+from unified_planning.io import ANMLWriter
 import tempfile
 import os
 
 
 class TestANMLWriter(TestCase):
     def setUp(self):
         TestCase.setUp(self)
@@ -103,16 +103,16 @@
         expected_result = """type Location;
 fluent boolean is_at(Location position);
 constant boolean is_connected(Location location_1, Location location_2);
 action move(Location l_from, Location l_to) {
    duration >= 6 and duration <= 6;
    [ start, start ] is_at(l_from);
    [ start, start ] (not is_at(l_to));
-   [ start, start ] (exists(Location mid_loc) { ((not ((mid_loc == l_from) or (mid_loc == l_to))) and (is_connected(l_from, mid_loc) or is_connected(mid_loc, l_from)) and (is_connected(l_to, mid_loc) or is_connected(mid_loc, l_to))); });
-   [ start, end ] (exists(Location mid_loc) { ((not ((mid_loc == l_from) or (mid_loc == l_to))) and (is_connected(l_from, mid_loc) or is_connected(mid_loc, l_from)) and (is_connected(l_to, mid_loc) or is_connected(mid_loc, l_to))); });
+   [ start, start ] (exists(Location mid_loc) { ((not ((mid_loc == l_from) or (mid_loc == l_to))) and (is_connected(l_from, mid_loc) or is_connected(mid_loc, l_from)) and (is_connected(l_to, mid_loc) or is_connected(mid_loc, l_to))) });
+   [ start, end ] (exists(Location mid_loc) { ((not ((mid_loc == l_from) or (mid_loc == l_to))) and (is_connected(l_from, mid_loc) or is_connected(mid_loc, l_from)) and (is_connected(l_to, mid_loc) or is_connected(mid_loc, l_to))) });
    [ start + 1 ] is_at(l_from) := false;
    [ end - 5 ] is_at(l_to) := true;
 };
 instance Location l1, l2, l3, l4, l5;
 [ start ] is_at(l1) := true;
 is_connected(l1, l2) := true;
 is_connected(l2, l3) := true;
@@ -246,59 +246,23 @@
         problem.add_object(obj)
         problem.set_initial_value(fl, False)
         aw = ANMLWriter(problem)
         anml_problem = aw.get_problem()
         expected_result = """type when_;
 fluent boolean f_4ction;
 action variable_(when_ fluent_) {
-   [ start ] when (fluent_ == predicate_)
-      {f_4ction := true;
-      };
+   when [ start ] (fluent_ == predicate_)
+   {[ start ] f_4ction := true;
+   }
 };
 instance when_ predicate_;
 [ start ] f_4ction := false;
 """
         self.assertEqual(anml_problem, expected_result)
 
-    def test_forall_effects(self):
-        FILE_PATH = os.path.dirname(os.path.abspath(__file__))
-        PDDL_DOMAINS_PATH = os.path.join(FILE_PATH, "pddl")
-        reader = PDDLReader()
-        domain_filename = os.path.join(PDDL_DOMAINS_PATH, "safe_road", "domain.pddl")
-        problem_filename = os.path.join(PDDL_DOMAINS_PATH, "safe_road", "problem.pddl")
-        problem = reader.parse_problem(domain_filename, problem_filename)
-        aw = ANMLWriter(problem)
-        anml_problem = aw.get_problem()
-
-        expected_result = """type location;
-fluent boolean safe(location l1_0, location l2_0);
-action check(location l1_0, location l2_0) {
-   [ start ] (not safe(l1_0, l2_0));
-   [ start ] safe(l1_0, l2_0) := true;
-};
-action natural_disaster() {
-   [ start ] forall (location l1_1, location l2_1){
-      when safe(l1_1, l2_1)
-         {safe(l1_1, l2_1) := false;
-         };
-   };
-};
-instance location l1, l2, l3;
-[ start ] safe(l1, l1) := true;
-[ start ] safe(l2, l2) := true;
-[ start ] safe(l3, l3) := true;
-[ start ] safe(l2, l1) := false;
-[ start ] safe(l3, l1) := false;
-[ start ] safe(l1, l2) := false;
-[ start ] safe(l3, l2) := false;
-[ start ] safe(l1, l3) := false;
-[ start ] safe(l2, l3) := false;
-"""
-        self.assertEqual(anml_problem, expected_result)
-
     @skipIfEngineNotAvailable("tamer")
     def test_with_pytamer(self):
         import pytamer
 
         with tempfile.TemporaryDirectory() as tempdir:
             temp_file_name = os.path.join(tempdir, "test_file.anml")
             with OneshotPlanner(name="tamer") as tamer:
```

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_anytime.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_anytime.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_bounded_types_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_bounded_types_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_compilers_pipeline.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_compilers_pipeline.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_compilers_quality_metrics.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_compilers_quality_metrics.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_conditional_effects_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_conditional_effects_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_contingent_pddl.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_contingent_pddl.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_credits.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_credits.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_disjunctive_conditions_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_disjunctive_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_dnf.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_dnf.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_expression_analysis.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_expression_analysis.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_factory.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_factory.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_grounder.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_htn.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_htn.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_infix_notation.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_infix_notation.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_ma_conditional_effects_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_ma_conditional_effects_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_ma_disjunctive_conditions_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_ma_disjunctive_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_model.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_model.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_multi_agent.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_multi_agent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_negative_conditions_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_negative_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_partial_order_plan.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_partial_order_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_pddl_io.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_pddl_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -816,32 +816,14 @@
             problem.add_fluent(y, default_initial_value=False)
             problem.add_fluent(z, default_initial_value=False)
             problem.add_goal(goal)
             writer = PDDLWriter(problem)
             pddl_problem = writer.get_problem()
             self.assertIn(expected_goal, pddl_problem)
 
-    def test_grounding_tpp_metric(self):
-        reader = PDDLReader()
-
-        domain_filename = os.path.join(PDDL_DOMAINS_PATH, "tpp_metric", "domain.pddl")
-        problem_filename = os.path.join(PDDL_DOMAINS_PATH, "tpp_metric", "problem.pddl")
-        problem = reader.parse_problem(domain_filename, problem_filename)
-
-        self.assertIsNotNone(problem)
-
-        with Compiler(
-            name="up_grounder", compilation_kind=CompilationKind.GROUNDING
-        ) as grounder:
-            grounded_problem = grounder.compile(
-                problem, compilation_kind=CompilationKind.GROUNDING
-            ).problem
-        self.assertEqual(40, len(grounded_problem.actions))
-        self.assertEqual(3, len(problem.actions))
-
 
 def _have_same_user_types_considering_renamings(
     original_problem: unified_planning.model.Problem,
     tested_problem: unified_planning.model.Problem,
     get_item_named,
 ) -> bool:
     for tested_type in tested_problem.user_types:
```

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_pddl_planner.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_pddl_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_plan_validator.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_plan_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_planner.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_problem.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_protobuf_io.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_protobuf_io.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_pyperplan.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_pyperplan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_quantifier_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_quantifier_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_replanner.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_replanner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_scheduling.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_sequential_simulator.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_sequential_simulator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_simplifier.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_simplifier.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_simulated_effects.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_simulated_effects.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_state_invariants.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_state_invariants.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_stn_plan.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_stn_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_substituter.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_substituter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_tamp.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_tamp.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_tarski_converter.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_tarski_converter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_tarski_grounder.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_tarski_grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_temporal.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_temporal.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_trajectory_constraint.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_trajectory_constraint.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_trajectory_constraints_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_trajectory_constraints_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_usertype_fluents_remover.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_usertype_fluents_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/test/test_validator.py` & `unified_planning-1.0.0.6.dev1/unified_planning/test/test_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning/utils.py` & `unified_planning-1.0.0.6.dev1/unified_planning/utils.py`

 * *Files identical despite different names*

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning.egg-info/PKG-INFO` & `unified_planning-1.0.0.6.dev1/unified_planning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unified-planning
-Version: 1.0.0.29.dev1
+Version: 1.0.0.6.dev1
 Summary: Unified Planning Framework
 Home-page: https://www.aiplan4eu-project.eu
 Author: AIPlan4EU Project
 Author-email: aiplan4eu@fbk.eu
 License: APACHE
 Description: Unified Planning: A library that makes it easy to formulate planning problems and to invoke automated planners.
 Keywords: planning logic STRIPS RDDL
```

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning.egg-info/SOURCES.txt` & `unified_planning-1.0.0.6.dev1/unified_planning.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -206,15 +206,14 @@
 unified_planning/test/anml/durative_goals.anml
 unified_planning/test/anml/forall.anml
 unified_planning/test/anml/hierarchical_blocks_world.anml
 unified_planning/test/anml/hydrone.anml
 unified_planning/test/anml/match.anml
 unified_planning/test/anml/match_int_id.anml
 unified_planning/test/anml/match_test_parser.anml
-unified_planning/test/anml/safe_road.anml
 unified_planning/test/anml/simple_mais.anml
 unified_planning/test/anml/tils.anml
 unified_planning/test/contingent_pddl/colorballs/domain.pddl
 unified_planning/test/contingent_pddl/colorballs/problem.pddl
 unified_planning/test/contingent_pddl/logistic_conf/domain.pddl
 unified_planning/test/contingent_pddl/logistic_conf/problem.pddl
 unified_planning/test/examples/__init__.py
@@ -300,11 +299,9 @@
 unified_planning/test/pddl/miconic/problem.pddl
 unified_planning/test/pddl/robot_fastener/domain.pddl
 unified_planning/test/pddl/robot_fastener/problem.pddl
 unified_planning/test/pddl/safe_road/domain.pddl
 unified_planning/test/pddl/safe_road/problem.pddl
 unified_planning/test/pddl/sailing/domain.pddl
 unified_planning/test/pddl/sailing/problem.pddl
-unified_planning/test/pddl/tpp_metric/domain.pddl
-unified_planning/test/pddl/tpp_metric/problem.pddl
 unified_planning/test/pddl/visit_precedence/domain.pddl
 unified_planning/test/pddl/visit_precedence/problem.pddl
```

### Comparing `unified_planning-1.0.0.29.dev1/unified_planning.egg-info/requires.txt` & `unified_planning-1.0.0.6.dev1/unified_planning.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 pytest-cov
 mypy
 
 [engines]
 tarski[arithmetic]
 up-pyperplan==1.0.0
 up-tamer==1.0.0
-up-enhsp==0.0.17
+up-enhsp==0.0.16
 up-fast-downward==0.2.3
 up-lpg==0.0.7
 up-fmap==0.0.7
 up-aries>=0.0.8
 up-symk>=0.0.3
 
 [enhsp]
-up-enhsp==0.0.17
+up-enhsp==0.0.16
 
 [fast-downward]
 up-fast-downward==0.2.3
 
 [fmap]
 up-fmap==0.0.7
```

