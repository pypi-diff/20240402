# Comparing `tmp/angr-9.2.96.tar.gz` & `tmp/angr-9.2.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angr-9.2.96.tar", last modified: Tue Mar 26 17:02:33 2024, max compression
+gzip compressed data, was "angr-9.2.97.tar", last modified: Tue Apr  2 17:02:57 2024, max compression
```

## Comparing `angr-9.2.96.tar` & `angr-9.2.97.tar`

### file list

```diff
@@ -1,1399 +1,1399 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.285511 angr-9.2.96/
--rw-r--r--   0 vsts      (1001) docker     (127)     1327 2024-03-26 17:00:59.000000 angr-9.2.96/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      107 2024-03-26 17:00:59.000000 angr-9.2.96/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     4769 2024-03-26 17:02:33.285511 angr-9.2.96/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2603 2024-03-26 17:00:59.000000 angr-9.2.96/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.773516 angr-9.2.96/angr/
--rw-r--r--   0 vsts      (1001) docker     (127)     3992 2024-03-26 17:01:07.000000 angr-9.2.96/angr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1887 2024-03-26 17:00:59.000000 angr-9.2.96/angr/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.789516 angr-9.2.96/angr/analyses/
--rw-r--r--   0 vsts      (1001) docker     (127)     1773 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12277 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27287 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/backward_slice.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26267 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/binary_optimizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    51815 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/bindiff.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2448 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/boyscout.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2835 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/callee_cleanup_finder.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40039 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/calling_convention.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6361 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cdg.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.793516 angr-9.2.96/angr/analyses/cfg/
--rw-r--r--   0 vsts      (1001) docker     (127)      321 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15450 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg/cfb.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3146 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg/cfg.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3112 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg/cfg_arch_options.py
--rw-r--r--   0 vsts      (1001) docker     (127)   122546 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg/cfg_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)   152842 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg/cfg_emulated.py
--rw-r--r--   0 vsts      (1001) docker     (127)   218220 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg/cfg_fast.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26047 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg/cfg_fast_soot.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5989 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg/cfg_job_base.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.797515 angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/
--rw-r--r--   0 vsts      (1001) docker     (127)      361 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2083 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/amd64_elf_got.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1777 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/amd64_pe_iat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5231 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/arm_elf_fast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5273 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/const_resolver.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1441 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/default_resolvers.py
--rw-r--r--   0 vsts      (1001) docker     (127)   101955 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/jumptable.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19350 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/mips_elf_fast.py
--rw-r--r--   0 vsts      (1001) docker     (127)      880 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/propagator_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3019 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/resolver.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2971 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/x86_elf_pic_plt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1621 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/x86_pe_iat.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.797515 angr-9.2.96/angr/analyses/cfg_slice_to_sink/
--rw-r--r--   0 vsts      (1001) docker     (127)      120 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg_slice_to_sink/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3982 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg_slice_to_sink/cfg_slice_to_sink.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3560 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg_slice_to_sink/graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/cfg_slice_to_sink/transitions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2969 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/class_identifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3641 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/code_tagging.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17719 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/complete_calling_conventions.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16456 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/congruency_check.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.797515 angr-9.2.96/angr/analyses/data_dep/
--rw-r--r--   0 vsts      (1001) docker     (127)      180 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/data_dep/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25296 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/data_dep/data_dependency_analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4650 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/data_dep/dep_nodes.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1527 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/data_dep/sim_act_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3386 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/datagraph_meta.py
--rw-r--r--   0 vsts      (1001) docker     (127)    63426 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/ddg.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.809515 angr-9.2.96/angr/analyses/decompiler/
--rw-r--r--   0 vsts      (1001) docker     (127)      540 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    60888 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/ail_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1595 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/ailgraph_walker.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10576 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/block_io_finder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6531 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/block_similarity.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17199 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/block_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1205 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/call_counter.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15083 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/callsite_maker.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.809515 angr-9.2.96/angr/analyses/decompiler/ccall_rewriters/
--rw-r--r--   0 vsts      (1001) docker     (127)      102 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/ccall_rewriters/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21551 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/ccall_rewriters/amd64_ccalls.py
--rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/ccall_rewriters/rewriter_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)    87477 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/clinic.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49449 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/condition_processor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/decompilation_cache.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8240 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/decompilation_options.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22137 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/decompiler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7368 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/empty_node_remover.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2867 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/expression_counters.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3545 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/expression_narrower.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2485 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/goto_manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16502 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/graph_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1181 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/jump_target_collector.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/jumptable_entry_condition_rewriter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.817515 angr-9.2.96/angr/analyses/decompiler/optimization_passes/
--rw-r--r--   0 vsts      (1001) docker     (127)     3811 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5289 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/base_ptr_save_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15319 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/code_motion.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10593 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/const_derefs.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4033 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/cross_jump_reverter.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17442 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/div_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10388 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/engine_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4701 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/expr_op_swapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3946 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/flip_boolean_cmp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7756 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/ite_expr_converter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6762 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/ite_region_converter.py
--rw-r--r--   0 vsts      (1001) docker     (127)    34328 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/lowered_switch_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3124 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/mod_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10420 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/multi_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14331 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/optimization_pass.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7398 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/register_save_area_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6470 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/ret_addr_save_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7828 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/ret_deduplicator.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18394 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/return_duplicator_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1803 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/return_duplicator_high.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4973 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/return_duplicator_low.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12559 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/stack_canary_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4523 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/switch_default_case_duplicator.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12304 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/win_stack_canary_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/optimization_passes/x86_gcc_getpc_simplifier.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.829515 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/
--rw-r--r--   0 vsts      (1001) docker     (127)     3208 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1727 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/a_div_const_add_a_mul_n_div_const.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1365 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/a_mul_const_div_shr_const.py
--rw-r--r--   0 vsts      (1001) docker     (127)      988 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/a_shl_const_sub_a.py
--rw-r--r--   0 vsts      (1001) docker     (127)      953 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2050 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div_const_mul_const.py
--rw-r--r--   0 vsts      (1001) docker     (127)      619 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/a_sub_a_sub_n.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9333 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/arm_cmpf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3538 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/base.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1056 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_add_n.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_and_mask.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1298 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/bitwise_or_to_logical_or.py
--rw-r--r--   0 vsts      (1001) docker     (127)      991 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/bool_expr_xor_1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6238 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/bswap.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1020 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/coalesce_same_cascading_ifs.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3691 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/const_mull_a_shift.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1583 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/constant_derefs.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2578 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/conv_a_sub0_shr_and.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2070 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/conv_shl_shr.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10131 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/eager_eval.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2015 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/extended_byte_and_mask.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2601 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/inlined_strcpy.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4676 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/inlined_strcpy_consolidation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2084 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/invert_negated_logical_conjuction_disjunction.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1136 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/one_sub_bool.py
--rw-r--r--   0 vsts      (1001) docker     (127)      591 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/remove_cascading_conversions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1560 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/remove_empty_if_body.py
--rw-r--r--   0 vsts      (1001) docker     (127)      739 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/remove_noop_conversions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1635 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/remove_redundant_bitmasks.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6583 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/remove_redundant_conversions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1189 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/remove_redundant_ite_branch.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1869 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/remove_redundant_ite_comparisons.py
--rw-r--r--   0 vsts      (1001) docker     (127)      503 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/remove_redundant_nots.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1394 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/remove_redundant_reinterprets.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1665 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/remove_redundant_shifts.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1578 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/remove_redundant_shifts_around_comparators.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3327 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/rewrite_bit_extractions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1809 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/rewrite_mips_gp_loads.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2814 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/rol_ror.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5282 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/sar_to_signed_div.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1477 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/simplify_pc_relative_loads.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1837 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/single_bit_cond_to_boolexpr.py
--rw-r--r--   0 vsts      (1001) docker     (127)      940 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/single_bit_xor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4833 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/tidy_stack_addr.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5385 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/redundant_label_remover.py
--rw-r--r--   0 vsts      (1001) docker     (127)    45489 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/region_identifier.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.833515 angr-9.2.96/angr/analyses/decompiler/region_simplifiers/
--rw-r--r--   0 vsts      (1001) docker     (127)       48 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/region_simplifiers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3721 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/region_simplifiers/cascading_cond_transformer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2490 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/region_simplifiers/cascading_ifs.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24008 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/region_simplifiers/expr_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6032 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/region_simplifiers/goto.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5034 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/region_simplifiers/if_.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3681 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/region_simplifiers/ifelse.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5861 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/region_simplifiers/loop.py
--rw-r--r--   0 vsts      (1001) docker     (127)      565 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/region_simplifiers/node_address_finder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8209 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/region_simplifiers/region_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24545 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/region_simplifiers/switch_cluster_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3327 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/region_simplifiers/switch_expr_simplifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)      717 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/region_walker.py
--rw-r--r--   0 vsts      (1001) docker     (127)      529 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/seq_to_blocks.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8428 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/sequence_walker.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.837515 angr-9.2.96/angr/analyses/decompiler/structured_codegen/
--rw-r--r--   0 vsts      (1001) docker     (127)      290 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/structured_codegen/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3845 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/structured_codegen/base.py
--rw-r--r--   0 vsts      (1001) docker     (127)   135109 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/structured_codegen/c.py
--rw-r--r--   0 vsts      (1001) docker     (127)      535 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/structured_codegen/dummy.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6773 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/structured_codegen/dwarf_import.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.837515 angr-9.2.96/angr/analyses/decompiler/structuring/
--rw-r--r--   0 vsts      (1001) docker     (127)      371 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/structuring/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    48400 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/structuring/dream.py
--rw-r--r--   0 vsts      (1001) docker     (127)   119472 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/structuring/phoenix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7078 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/structuring/recursive_structurer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41330 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/structuring/structurer_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11964 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/structuring/structurer_nodes.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27930 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/decompiler/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    45941 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/disassembly.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2989 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/disassembly_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1245 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/dominance_frontier.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9882 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/find_objects_static.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7847 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/flirt.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.841515 angr-9.2.96/angr/analyses/forward_analysis/
--rw-r--r--   0 vsts      (1001) docker     (127)      144 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/forward_analysis/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19264 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/forward_analysis/forward_analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1579 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/forward_analysis/job_info.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.841515 angr-9.2.96/angr/analyses/forward_analysis/visitors/
--rw-r--r--   0 vsts      (1001) docker     (127)      174 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/forward_analysis/visitors/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      713 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/forward_analysis/visitors/call_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2739 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/forward_analysis/visitors/function_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8067 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/forward_analysis/visitors/graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)      711 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/forward_analysis/visitors/loop.py
--rw-r--r--   0 vsts      (1001) docker     (127)      768 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/forward_analysis/visitors/single_node_graph.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.845515 angr-9.2.96/angr/analyses/identifier/
--rw-r--r--   0 vsts      (1001) docker     (127)       33 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4757 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/custom_callable.py
--rw-r--r--   0 vsts      (1001) docker     (127)      157 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/errors.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1749 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/func.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.849515 angr-9.2.96/angr/analyses/identifier/functions/
--rw-r--r--   0 vsts      (1001) docker     (127)     1059 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2110 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/atoi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3294 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/based_atoi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4353 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/fdprintf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1941 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/free.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8665 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/int2str.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3845 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/malloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1953 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/memcmp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3166 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/memcpy.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1188 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/memset.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4307 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/printf.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11564 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/recv_until.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2356 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/skip_calloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3186 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/skip_realloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2886 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/skip_recv_n.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4179 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/snprintf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4119 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/sprintf.py
--rw-r--r--   0 vsts      (1001) docker     (127)      806 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/strcasecmp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3459 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/strcmp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1187 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/strcpy.py
--rw-r--r--   0 vsts      (1001) docker     (127)      753 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/strlen.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3297 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/strncmp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2008 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/strncpy.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2426 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/functions/strtol.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33287 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/identify.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13739 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/identifier/runner.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8531 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/init_finder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9412 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/loop_analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7122 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/loopfinder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.853515 angr-9.2.96/angr/analyses/propagator/
--rw-r--r--   0 vsts      (1001) docker     (127)       43 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/propagator/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    68580 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/propagator/engine_ail.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1735 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/propagator/engine_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12491 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/propagator/engine_vex.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6890 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/propagator/outdated_definition_walker.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16071 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/propagator/propagator.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/propagator/tmpvar_finder.py
--rw-r--r--   0 vsts      (1001) docker     (127)      359 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/propagator/top_checker_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/propagator/values.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1433 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/propagator/vex_vars.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16323 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/proximity_graph.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.857515 angr-9.2.96/angr/analyses/reaching_definitions/
--rw-r--r--   0 vsts      (1001) docker     (127)     1989 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/reaching_definitions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2217 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/reaching_definitions/call_trace.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14886 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/reaching_definitions/dep_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)    45997 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/reaching_definitions/engine_ail.py
--rw-r--r--   0 vsts      (1001) docker     (127)    42934 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/reaching_definitions/engine_vex.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/reaching_definitions/external_codeloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26839 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/reaching_definitions/function_handler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2634 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/reaching_definitions/heap_allocator.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11224 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/reaching_definitions/rd_initializer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23537 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/reaching_definitions/rd_state.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23438 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/reaching_definitions/reaching_definitions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1995 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/reaching_definitions/subject.py
--rw-r--r--   0 vsts      (1001) docker     (127)   100412 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/reassembler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8941 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/soot_class_hierarchy.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29868 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/stack_pointer_tracker.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1711 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/static_hooker.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.865515 angr-9.2.96/angr/analyses/typehoon/
--rw-r--r--   0 vsts      (1001) docker     (127)       31 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/typehoon/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3519 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/typehoon/dfa.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2805 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/typehoon/lifter.py
--rw-r--r--   0 vsts      (1001) docker     (127)    48619 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/typehoon/simple_solver.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8610 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/typehoon/translator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7030 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/typehoon/typeconsts.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9353 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/typehoon/typehoon.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15783 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/typehoon/typevars.py
--rw-r--r--   0 vsts      (1001) docker     (127)      158 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/typehoon/variance.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.869515 angr-9.2.96/angr/analyses/variable_recovery/
--rw-r--r--   0 vsts      (1001) docker     (127)      105 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/variable_recovery/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1403 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/variable_recovery/annotations.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25704 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/variable_recovery/engine_ail.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41633 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/variable_recovery/engine_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19046 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/variable_recovery/engine_vex.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4701 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/variable_recovery/irsb_scanner.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21802 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/variable_recovery/variable_recovery.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14821 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/variable_recovery/variable_recovery_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24125 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/variable_recovery/variable_recovery_fast.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25224 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/veritesting.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75256 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/vfg.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16173 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/vsa_ddg.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3874 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/vtable.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9714 2024-03-26 17:00:59.000000 angr-9.2.96/angr/analyses/xrefs.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.869515 angr-9.2.96/angr/angrdb/
--rw-r--r--   0 vsts      (1001) docker     (127)      231 2024-03-26 17:00:59.000000 angr-9.2.96/angr/angrdb/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6459 2024-03-26 17:00:59.000000 angr-9.2.96/angr/angrdb/db.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4750 2024-03-26 17:00:59.000000 angr-9.2.96/angr/angrdb/models.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.873515 angr-9.2.96/angr/angrdb/serializers/
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-03-26 17:00:59.000000 angr-9.2.96/angr/angrdb/serializers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1297 2024-03-26 17:00:59.000000 angr-9.2.96/angr/angrdb/serializers/cfg_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1531 2024-03-26 17:00:59.000000 angr-9.2.96/angr/angrdb/serializers/comments.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1696 2024-03-26 17:00:59.000000 angr-9.2.96/angr/angrdb/serializers/funcs.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3688 2024-03-26 17:00:59.000000 angr-9.2.96/angr/angrdb/serializers/kb.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1425 2024-03-26 17:00:59.000000 angr-9.2.96/angr/angrdb/serializers/labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2494 2024-03-26 17:00:59.000000 angr-9.2.96/angr/angrdb/serializers/loader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4190 2024-03-26 17:00:59.000000 angr-9.2.96/angr/angrdb/serializers/structured_code.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2383 2024-03-26 17:00:59.000000 angr-9.2.96/angr/angrdb/serializers/variables.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1180 2024-03-26 17:00:59.000000 angr-9.2.96/angr/angrdb/serializers/xrefs.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10818 2024-03-26 17:00:59.000000 angr-9.2.96/angr/annocfg.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15519 2024-03-26 17:00:59.000000 angr-9.2.96/angr/blade.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14468 2024-03-26 17:00:59.000000 angr-9.2.96/angr/block.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6034 2024-03-26 17:00:59.000000 angr-9.2.96/angr/callable.py
--rw-r--r--   0 vsts      (1001) docker     (127)    91291 2024-03-26 17:00:59.000000 angr-9.2.96/angr/calling_conventions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5476 2024-03-26 17:00:59.000000 angr-9.2.96/angr/code_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3784 2024-03-26 17:00:59.000000 angr-9.2.96/angr/codenode.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.881515 angr-9.2.96/angr/concretization_strategies/
--rw-r--r--   0 vsts      (1001) docker     (127)     3727 2024-03-26 17:00:59.000000 angr-9.2.96/angr/concretization_strategies/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      438 2024-03-26 17:00:59.000000 angr-9.2.96/angr/concretization_strategies/any.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1341 2024-03-26 17:00:59.000000 angr-9.2.96/angr/concretization_strategies/any_named.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2218 2024-03-26 17:00:59.000000 angr-9.2.96/angr/concretization_strategies/controlled_data.py
--rw-r--r--   0 vsts      (1001) docker     (127)      617 2024-03-26 17:00:59.000000 angr-9.2.96/angr/concretization_strategies/eval.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-03-26 17:00:59.000000 angr-9.2.96/angr/concretization_strategies/logging.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1035 2024-03-26 17:00:59.000000 angr-9.2.96/angr/concretization_strategies/max.py
--rw-r--r--   0 vsts      (1001) docker     (127)      536 2024-03-26 17:00:59.000000 angr-9.2.96/angr/concretization_strategies/nonzero.py
--rw-r--r--   0 vsts      (1001) docker     (127)      784 2024-03-26 17:00:59.000000 angr-9.2.96/angr/concretization_strategies/nonzero_range.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1435 2024-03-26 17:00:59.000000 angr-9.2.96/angr/concretization_strategies/norepeats.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1564 2024-03-26 17:00:59.000000 angr-9.2.96/angr/concretization_strategies/norepeats_range.py
--rw-r--r--   0 vsts      (1001) docker     (127)      555 2024-03-26 17:00:59.000000 angr-9.2.96/angr/concretization_strategies/range.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-03-26 17:00:59.000000 angr-9.2.96/angr/concretization_strategies/signed_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-03-26 17:00:59.000000 angr-9.2.96/angr/concretization_strategies/single.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-03-26 17:00:59.000000 angr-9.2.96/angr/concretization_strategies/solutions.py
--rw-r--r--   0 vsts      (1001) docker     (127)      529 2024-03-26 17:00:59.000000 angr-9.2.96/angr/concretization_strategies/unlimited_range.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.881515 angr-9.2.96/angr/distributed/
--rw-r--r--   0 vsts      (1001) docker     (127)      140 2024-03-26 17:00:59.000000 angr-9.2.96/angr/distributed/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6682 2024-03-26 17:00:59.000000 angr-9.2.96/angr/distributed/server.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6075 2024-03-26 17:00:59.000000 angr-9.2.96/angr/distributed/worker.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.885515 angr-9.2.96/angr/engines/
--rw-r--r--   0 vsts      (1001) docker     (127)     1066 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7468 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/concrete.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8109 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/engine.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/failure.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2546 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/hook.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.889515 angr-9.2.96/angr/engines/light/
--rw-r--r--   0 vsts      (1001) docker     (127)      186 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/light/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23132 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/light/data.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40791 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/light/engine.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.889515 angr-9.2.96/angr/engines/pcode/
--rw-r--r--   0 vsts      (1001) docker     (127)       83 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/pcode/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28720 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/pcode/behavior.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2994 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/pcode/cc.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16718 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/pcode/emulate.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10551 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/pcode/engine.py
--rw-r--r--   0 vsts      (1001) docker     (127)    52362 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/pcode/lifter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/procedure.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.893514 angr-9.2.96/angr/engines/soot/
--rw-r--r--   0 vsts      (1001) docker     (127)       30 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17238 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/engine.py
--rw-r--r--   0 vsts      (1001) docker     (127)      221 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.901514 angr-9.2.96/angr/engines/soot/expressions/
--rw-r--r--   0 vsts      (1001) docker     (127)     1706 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/expressions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      857 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/expressions/arrayref.py
--rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/expressions/base.py
--rw-r--r--   0 vsts      (1001) docker     (127)      781 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/expressions/binop.py
--rw-r--r--   0 vsts      (1001) docker     (127)      753 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/expressions/cast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1260 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/expressions/condition.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1387 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/expressions/constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)      313 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/expressions/instanceOf.py
--rw-r--r--   0 vsts      (1001) docker     (127)      234 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/expressions/instancefieldref.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4525 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/expressions/invoke.py
--rw-r--r--   0 vsts      (1001) docker     (127)      189 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/expressions/length.py
--rw-r--r--   0 vsts      (1001) docker     (127)      215 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/expressions/local.py
--rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/expressions/new.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1970 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/expressions/newArray.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3400 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/expressions/newMultiArray.py
--rw-r--r--   0 vsts      (1001) docker     (127)      224 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/expressions/paramref.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1192 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/expressions/phi.py
--rw-r--r--   0 vsts      (1001) docker     (127)      232 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/expressions/staticfieldref.py
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/expressions/thisref.py
--rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/expressions/unsupported.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1940 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/field_dispatcher.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1780 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/method_dispatcher.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.905514 angr-9.2.96/angr/engines/soot/statements/
--rw-r--r--   0 vsts      (1001) docker     (127)      893 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/statements/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1271 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/statements/assign.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2094 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/statements/base.py
--rw-r--r--   0 vsts      (1001) docker     (127)      325 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/statements/goto.py
--rw-r--r--   0 vsts      (1001) docker     (127)      421 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/statements/identity.py
--rw-r--r--   0 vsts      (1001) docker     (127)      560 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/statements/if_.py
--rw-r--r--   0 vsts      (1001) docker     (127)      284 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/statements/invoke.py
--rw-r--r--   0 vsts      (1001) docker     (127)      466 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/statements/return_.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1301 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/statements/switch.py
--rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/statements/throw.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.905514 angr-9.2.96/angr/engines/soot/values/
--rw-r--r--   0 vsts      (1001) docker     (127)      792 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/values/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4427 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/values/arrayref.py
--rw-r--r--   0 vsts      (1001) docker     (127)      121 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/values/base.py
--rw-r--r--   0 vsts      (1001) docker     (127)      403 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/values/constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1593 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/values/instancefieldref.py
--rw-r--r--   0 vsts      (1001) docker     (127)      385 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/values/local.py
--rw-r--r--   0 vsts      (1001) docker     (127)      413 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/values/paramref.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1240 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/values/staticfieldref.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1107 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/values/strref.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5739 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/soot/values/thisref.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23679 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/successors.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2177 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/syscall.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24447 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/unicorn.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.909515 angr-9.2.96/angr/engines/vex/
--rw-r--r--   0 vsts      (1001) docker     (127)       95 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/vex/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.909515 angr-9.2.96/angr/engines/vex/claripy/
--rw-r--r--   0 vsts      (1001) docker     (127)       40 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/vex/claripy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    82570 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/vex/claripy/ccall.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5123 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/vex/claripy/datalayer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    46171 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/vex/claripy/irop.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.909515 angr-9.2.96/angr/engines/vex/heavy/
--rw-r--r--   0 vsts      (1001) docker     (127)      201 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/vex/heavy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8871 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/vex/heavy/actions.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14702 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/vex/heavy/concretizers.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18699 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/vex/heavy/dirty.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15822 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/vex/heavy/heavy.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2317 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/vex/heavy/inspect.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3737 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/vex/heavy/resilience.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1180 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/vex/heavy/super_fastpath.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17132 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/vex/lifter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.913514 angr-9.2.96/angr/engines/vex/light/
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/vex/light/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21729 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/vex/light/light.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2002 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/vex/light/resilience.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2023 2024-03-26 17:00:59.000000 angr-9.2.96/angr/engines/vex/light/slicing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8299 2024-03-26 17:00:59.000000 angr-9.2.96/angr/errors.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.921514 angr-9.2.96/angr/exploration_techniques/
--rw-r--r--   0 vsts      (1001) docker     (127)     6980 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2588 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/bucketizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2262 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1167 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/dfs.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17917 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/director.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3531 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/driller_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6163 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/explorer.py
--rw-r--r--   0 vsts      (1001) docker     (127)      550 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/lengthlimiter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2583 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/local_loop_seer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11640 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/loop_seer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3091 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/manual_mergepoint.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1271 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/memory_watcher.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3520 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/oppologist.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5126 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/slicecutor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9382 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/spiller.py
--rw-r--r--   0 vsts      (1001) docker     (127)      818 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/spiller_db.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2059 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/stochastic.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6969 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/suggestions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3122 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/symbion.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1586 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/tech_builder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2976 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/threading.py
--rw-r--r--   0 vsts      (1001) docker     (127)      923 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/timeout.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50249 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/tracer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4413 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/unique.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1350 2024-03-26 17:00:59.000000 angr-9.2.96/angr/exploration_techniques/veritesting.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17411 2024-03-26 17:00:59.000000 angr-9.2.96/angr/factory.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.921514 angr-9.2.96/angr/flirt/
--rw-r--r--   0 vsts      (1001) docker     (127)     4428 2024-03-26 17:00:59.000000 angr-9.2.96/angr/flirt/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10109 2024-03-26 17:00:59.000000 angr-9.2.96/angr/flirt/build_sig.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-26 17:00:59.000000 angr-9.2.96/angr/graph_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18129 2024-03-26 17:00:59.000000 angr-9.2.96/angr/keyed_region.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.925514 angr-9.2.96/angr/knowledge_base/
--rw-r--r--   0 vsts      (1001) docker     (127)       42 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_base/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4623 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_base/knowledge_base.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.929514 angr-9.2.96/angr/knowledge_plugins/
--rw-r--r--   0 vsts      (1001) docker     (127)      697 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1597 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/callsite_prototypes.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.933514 angr-9.2.96/angr/knowledge_plugins/cfg/
--rw-r--r--   0 vsts      (1001) docker     (127)      382 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/cfg/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2302 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/cfg/cfg_manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41756 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/cfg/cfg_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17229 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/cfg/cfg_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2145 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/cfg/indirect_jump.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5040 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/cfg/memory_data.py
--rw-r--r--   0 vsts      (1001) docker     (127)      304 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/comments.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1027 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/custom_strings.py
--rw-r--r--   0 vsts      (1001) docker     (127)      839 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/data.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8189 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/debug_variables.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.937514 angr-9.2.96/angr/knowledge_plugins/functions/
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/functions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    66932 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/functions/function.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18990 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/functions/function_manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11916 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/functions/function_parser.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4971 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/functions/soot_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1024 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/indirect_jumps.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.945514 angr-9.2.96/angr/knowledge_plugins/key_definitions/
--rw-r--r--   0 vsts      (1001) docker     (127)      397 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/key_definitions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9753 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/key_definitions/atoms.py
--rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/key_definitions/constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8661 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/key_definitions/definition.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3461 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/key_definitions/environment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      922 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/key_definitions/heap_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3251 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/key_definitions/key_definition_manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39440 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/key_definitions/live_definitions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7140 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/key_definitions/liveness.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7312 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/key_definitions/rd_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1682 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/key_definitions/tag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1236 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/key_definitions/undefined.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1510 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/key_definitions/unknown_size.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6620 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/key_definitions/uses.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3137 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4373 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/patches.py
--rw-r--r--   0 vsts      (1001) docker     (127)      733 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/plugin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.949514 angr-9.2.96/angr/knowledge_plugins/propagations/
--rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/propagations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7706 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/propagations/prop_value.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2122 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/propagations/propagation_manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2786 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/propagations/propagation_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)    38297 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/propagations/states.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.949514 angr-9.2.96/angr/knowledge_plugins/structured_code/
--rw-r--r--   0 vsts      (1001) docker     (127)       43 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/structured_code/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2071 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/structured_code/manager.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.949514 angr-9.2.96/angr/knowledge_plugins/sync/
--rw-r--r--   0 vsts      (1001) docker     (127)       44 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/sync/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9276 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/sync/sync_controller.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1897 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.949514 angr-9.2.96/angr/knowledge_plugins/variables/
--rw-r--r--   0 vsts      (1001) docker     (127)       60 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/variables/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3751 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/variables/variable_access.py
--rw-r--r--   0 vsts      (1001) docker     (127)    44720 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/variables/variable_manager.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.953514 angr-9.2.96/angr/knowledge_plugins/xrefs/
--rw-r--r--   0 vsts      (1001) docker     (127)       94 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/xrefs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4963 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/xrefs/xref.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4009 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/xrefs/xref_manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)      271 2024-03-26 17:00:59.000000 angr-9.2.96/angr/knowledge_plugins/xrefs/xref_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.957514 angr-9.2.96/angr/misc/
--rw-r--r--   0 vsts      (1001) docker     (127)      237 2024-03-26 17:00:59.000000 angr-9.2.96/angr/misc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      807 2024-03-26 17:00:59.000000 angr-9.2.96/angr/misc/ansi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3426 2024-03-26 17:00:59.000000 angr-9.2.96/angr/misc/autoimport.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4241 2024-03-26 17:00:59.000000 angr-9.2.96/angr/misc/bug_report.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4486 2024-03-26 17:00:59.000000 angr-9.2.96/angr/misc/hookset.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1943 2024-03-26 17:00:59.000000 angr-9.2.96/angr/misc/import_hooks.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4225 2024-03-26 17:00:59.000000 angr-9.2.96/angr/misc/loggers.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1276 2024-03-26 17:00:59.000000 angr-9.2.96/angr/misc/picklable_lock.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9370 2024-03-26 17:00:59.000000 angr-9.2.96/angr/misc/plugins.py
--rw-r--r--   0 vsts      (1001) docker     (127)      509 2024-03-26 17:00:59.000000 angr-9.2.96/angr/misc/range.py
--rw-r--r--   0 vsts      (1001) docker     (127)      593 2024-03-26 17:00:59.000000 angr-9.2.96/angr/misc/testing.py
--rw-r--r--   0 vsts      (1001) docker     (127)      701 2024-03-26 17:00:59.000000 angr-9.2.96/angr/misc/ux.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1453 2024-03-26 17:00:59.000000 angr-9.2.96/angr/misc/weakpatch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.961514 angr-9.2.96/angr/procedures/
--rw-r--r--   0 vsts      (1001) docker     (127)      119 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.961514 angr-9.2.96/angr/procedures/advapi32/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/advapi32/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:32.965514 angr-9.2.96/angr/procedures/cgc/
--rw-r--r--   0 vsts      (1001) docker     (127)       76 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/cgc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      224 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/cgc/_terminate.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3371 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/cgc/allocate.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1984 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/cgc/deallocate.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2802 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/cgc/fdwait.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2334 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/cgc/random.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3758 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/cgc/receive.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2368 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/cgc/transmit.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.145512 angr-9.2.96/angr/procedures/definitions/
--rw-r--r--   0 vsts      (1001) docker     (127)    32023 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/cgc.py
--rw-r--r--   0 vsts      (1001) docker     (127)   394191 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/glibc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/gnulib.py
--rw-r--r--   0 vsts      (1001) docker     (127)      700 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/libstdcpp.py
--rw-r--r--   0 vsts      (1001) docker     (127)   238887 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/linux_kernel.py
--rw-r--r--   0 vsts      (1001) docker     (127)      219 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/linux_loader.py
--rw-r--r--   0 vsts      (1001) docker     (127)      601 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/msvcr.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1795 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/parse_syscalls_from_local_system.py
--rw-r--r--   0 vsts      (1001) docker     (127)   110573 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/parse_win32json.py
--rw-r--r--   0 vsts      (1001) docker     (127)  9998064 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/types_win32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1458 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/wdk_api-ms-win-dx-d3dkmt-l1-1-4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1000 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/wdk_api-ms-win-dx-d3dkmt-l1-1-6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22852 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/wdk_clfs.py
--rw-r--r--   0 vsts      (1001) docker     (127)   111981 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/wdk_fltmgr.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1730 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/wdk_fwpkclnt.py
--rw-r--r--   0 vsts      (1001) docker     (127)    68446 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/wdk_fwpuclnt.py
--rw-r--r--   0 vsts      (1001) docker     (127)    37307 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/wdk_gdi32.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11415 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/wdk_hal.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12527 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/wdk_ksecdd.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33948 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/wdk_ndis.py
--rw-r--r--   0 vsts      (1001) docker     (127)   593050 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/wdk_ntoskrnl.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9862 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/wdk_offreg.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1980 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/wdk_pshed.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3478 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/wdk_secur32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1942 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/wdk_vhfum.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1553 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_aclui.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7877 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_activeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)   310929 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_advapi32.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22314 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_advpack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3430 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_amsi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3769 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3051 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-3.py
--rw-r--r--   0 vsts      (1001) docker     (127)      922 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-6.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-apiquery-l2-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1060 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-backgroundtask-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1134 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1167 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1488 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-enclave-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1037 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-errorhandling-l1-1-3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2317 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1217 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4874 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-file-fromapp-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1125 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-handle-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5164 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-ioring-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2219 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-marshal-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2528 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1492 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-5.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3867 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-6.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2362 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-7.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2378 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-8.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8406 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-path-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1547 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1562 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1429 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1850 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1281 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-slapi-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1682 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-state-helpers-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1540 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-synch-l1-2-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)      995 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1184 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1467 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-4.py
--rw-r--r--   0 vsts      (1001) docker     (127)      951 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-6.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1537 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-util-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3268 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3777 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3228 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-winrt-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1162 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-winrt-registration-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)      901 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-winrt-robuffer-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1694 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-winrt-roparameterizediid-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10986 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1550 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1653 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-wow64-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6949 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6680 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-dx-d3dkmt-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1043 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-gaming-deviceinformation-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1347 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-gaming-expandedresources-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3983 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1753 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5014 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2233 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4359 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1207 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-mm-misc-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3912 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-net-isolation-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1434 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-security-base-l1-2-2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1041 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1100 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1289 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1344 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1833 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-5.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1687 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2545 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-1.py
--rw-r--r--   0 vsts      (1001) docker     (127)      994 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1817 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-shcore-stream-winrt-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3586 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-wsl-api-l1-1-0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1117 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_apphelp.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17589 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_authz.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2884 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_avicap32.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18938 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_avifil32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5529 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_avrt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1328 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_bcp47mrm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24333 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_bcrypt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1325 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_bcryptprimitives.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17641 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_bluetoothapis.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10950 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_bthprops.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3094 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_bthprops_cpl.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16642 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_cabinet.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6820 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_certadm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4345 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_certpoleng.py
--rw-r--r--   0 vsts      (1001) docker     (127)   101560 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_cfgmgr32.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26407 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_chakra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14271 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_cldapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24138 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_clfsw32.py
--rw-r--r--   0 vsts      (1001) docker     (127)   111741 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_clusapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43365 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_comctl32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4894 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_comdlg32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2651 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_compstui.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19474 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_computecore.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16032 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_computenetwork.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4405 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_computestorage.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2241 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_comsvcs.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1201 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_coremessaging.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11823 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_credui.py
--rw-r--r--   0 vsts      (1001) docker     (127)   105559 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_crypt32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3864 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_cryptnet.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4935 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_cryptui.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9065 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_cryptxml.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1769 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_cscapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5253 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_d2d1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11546 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_d3d10.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_d3d10_1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3575 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_d3d11.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4078 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_d3d12.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3002 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_d3d9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13432 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_d3dcompiler_47.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4827 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_d3dcsx.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7266 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_davclnt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2063 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dbgeng.py
--rw-r--r--   0 vsts      (1001) docker     (127)   109042 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dbghelp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1028 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dbgmodel.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7151 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dciman32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4837 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dcomp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4233 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_ddraw.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1134 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_deviceaccess.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1145 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dflayout.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5570 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dhcpcsvc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2967 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dhcpcsvc6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    81410 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dhcpsapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13697 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_diagnosticdataquery.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1243 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dinput8.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1621 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_directml.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1261 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dmprocessxmlfiltered.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22815 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dnsapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5579 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_drt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3373 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_drtprov.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1445 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_drttransport.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5367 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dsound.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11582 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dsparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2935 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dsprop.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6189 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dssec.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1855 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dsuiext.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9715 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dwmapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1120 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dwrite.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1484 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dxcompiler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1061 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dxcore.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2185 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dxgi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14554 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_dxva2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10117 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_eappcfg.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9178 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_eappprxy.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1311 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_efswrt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2446 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_elscore.py
--rw-r--r--   0 vsts      (1001) docker     (127)   105927 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_esent.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3146 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_evr.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1687 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_faultrep.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2401 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_fhsvcctl.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2011 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_firewallapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12020 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_fltlib.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4105 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_fontsub.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1227 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_forceinline.py
--rw-r--r--   0 vsts      (1001) docker     (127)    93548 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_fwpuclnt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1129 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_fxsutility.py
--rw-r--r--   0 vsts      (1001) docker     (127)   148174 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_gdi32.py
--rw-r--r--   0 vsts      (1001) docker     (127)   247483 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_gdiplus.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16771 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_glu32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2162 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_gpedit.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1678 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_hhctrl_ocx.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21797 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_hid.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12512 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_hlink.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1027 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_hrtfapo.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19733 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_httpapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12533 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_icm32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1161 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_icmui.py
--rw-r--r--   0 vsts      (1001) docker     (127)   373759 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_icu.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10129 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_ieframe.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11559 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_imagehlp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3884 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_imgutil.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28246 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_imm32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8100 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_infocardapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8943 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_inkobjcore.py
--rw-r--r--   0 vsts      (1001) docker     (127)    65729 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_iphlpapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28599 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_iscsidsc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1293 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_isolatedwindowsenvironmentutils.py
--rw-r--r--   0 vsts      (1001) docker     (127)   505053 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_kernel32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3158 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_kernelbase.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2060 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_keycredmgr.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3689 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_ksproxy_ax.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4328 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_ksuser.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14607 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_ktmw32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1582 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_licenseprotection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4334 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_loadperf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6878 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_magnification.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25169 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mapi32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1411 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mdmlocalmanagement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4765 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mdmregistration.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17507 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1358 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mfcore.py
--rw-r--r--   0 vsts      (1001) docker     (127)    45685 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mfplat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1326 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mfplay.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2429 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mfreadwrite.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4363 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mfsensorgroup.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1451 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mfsrcsnk.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4531 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mgmtapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1232 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1326 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mmdevapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19241 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mpr.py
--rw-r--r--   0 vsts      (1001) docker     (127)    47666 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mprapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13037 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mqrt.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11736 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mrmsupport.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19430 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_msacm32.py
--rw-r--r--   0 vsts      (1001) docker     (127)   183424 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_msajapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    34895 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mscms.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11975 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mscoree.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1327 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_msctfmonitor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7687 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_msdelta.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4589 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_msdmo.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39076 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_msdrm.py
--rw-r--r--   0 vsts      (1001) docker     (127)   103106 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_msi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2796 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_msimg32.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11181 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mspatcha.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6011 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mspatchc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2844 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_msports.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7471 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_msrating.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7594 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mssign32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mstask.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16749 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_msvfw32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9190 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mswsock.py
--rw-r--r--   0 vsts      (1001) docker     (127)      973 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_mtxdm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19693 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_ncrypt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6200 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_ndfapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86057 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_netapi32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3436 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_netsh.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1151 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_netshell.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6101 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_newdev.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11168 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_ninput.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_normaliz.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27742 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_ntdll.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1087 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_ntdllk.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35639 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_ntdsapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4407 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_ntlanman.py
--rw-r--r--   0 vsts      (1001) docker     (127)    94760 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_odbc32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8509 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_odbcbcp.py
--rw-r--r--   0 vsts      (1001) docker     (127)   103812 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_ole32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7007 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_oleacc.py
--rw-r--r--   0 vsts      (1001) docker     (127)   123410 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_oleaut32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6811 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_oledlg.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2609 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_ondemandconnroutehelper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75467 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_opengl32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1461 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_opmxbox.py
--rw-r--r--   0 vsts      (1001) docker     (127)    32523 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_p2p.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12455 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_p2pgraph.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39415 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_pdh.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14293 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_peerdist.py
--rw-r--r--   0 vsts      (1001) docker     (127)    32180 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_powrprof.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_prntvpt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7998 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_projectedfslib.py
--rw-r--r--   0 vsts      (1001) docker     (127)    69946 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_propsys.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10760 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_psapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1362 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_quartz.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2051 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_query.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5253 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_qwave.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30989 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_rasapi32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2820 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_rasdlg.py
--rw-r--r--   0 vsts      (1001) docker     (127)    54566 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_resutils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1012 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_rometadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22447 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_rpcns4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1683 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_rpcproxy.py
--rw-r--r--   0 vsts      (1001) docker     (127)   148359 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_rpcrt4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4988 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_rstrtmgr.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36043 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_rtm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15136 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_rtutils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9078 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_rtworkq.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_sas.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1646 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_scarddlg.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3588 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_schannel.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1712 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_sechost.py
--rw-r--r--   0 vsts      (1001) docker     (127)    37550 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_secur32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1495 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_sensapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13284 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_sensorsutilsv2.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157765 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_setupapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2546 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_sfc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1932 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_shdocvw.py
--rw-r--r--   0 vsts      (1001) docker     (127)    81141 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_shell32.py
--rw-r--r--   0 vsts      (1001) docker     (127)   108109 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_shlwapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14350 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_slc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2850 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_slcext.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1143 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_slwga.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6443 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_snmpapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9685 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_spoolss.py
--rw-r--r--   0 vsts      (1001) docker     (127)      954 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_srclient.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3752 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_srpapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3032 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_sspicli.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1150 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_sti.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9597 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_t2embed.py
--rw-r--r--   0 vsts      (1001) docker     (127)    94966 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_tapi32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4951 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_tbs.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11389 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_tdh.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4744 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_tokenbinding.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8278 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_traffic.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4327 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_txfw32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1627 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_ualapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    31556 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_uiautomationcore.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27741 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_urlmon.py
--rw-r--r--   0 vsts      (1001) docker     (127)   252469 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_user32.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15838 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_userenv.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23757 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_usp10.py
--rw-r--r--   0 vsts      (1001) docker     (127)    31235 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_uxtheme.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1567 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_verifier.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7235 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3659 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_vertdll.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13507 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_virtdisk.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6032 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_vmdevicehost.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17637 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_vmsavedstatedumpprovider.py
--rw-r--r--   0 vsts      (1001) docker     (127)      987 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_vssapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2698 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wcmapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3339 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wdsbp.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13944 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wdsclientapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2846 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wdsmc.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13248 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wdspxe.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4149 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wdstptc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4708 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_webauthn.py
--rw-r--r--   0 vsts      (1001) docker     (127)   106080 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_webservices.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7433 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_websocket.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6419 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wecapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7708 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16155 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wevtapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21479 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_winbio.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1003 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_windows_ai_machinelearning.py
--rw-r--r--   0 vsts      (1001) docker     (127)      929 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_windows_data_pdf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3260 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_windows_media_mediacontrol.py
--rw-r--r--   0 vsts      (1001) docker     (127)      965 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_windows_networking.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1722 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_windows_ui_xaml.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4488 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_windowscodecs.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22678 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_winfax.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22808 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_winhttp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2752 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_winhvemulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40942 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_winhvplatform.py
--rw-r--r--   0 vsts      (1001) docker     (127)   116017 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wininet.py
--rw-r--r--   0 vsts      (1001) docker     (127)      969 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_winml.py
--rw-r--r--   0 vsts      (1001) docker     (127)    55061 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_winmm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29221 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_winscard.py
--rw-r--r--   0 vsts      (1001) docker     (127)   114656 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_winspool.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70042 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_winspool_drv.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22342 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wintrust.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14539 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_winusb.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30095 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wlanapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1412 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wlanui.py
--rw-r--r--   0 vsts      (1001) docker     (127)    97431 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wldap32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4202 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wldp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3239 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wmvcore.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1385 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wnvapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5271 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wofutil.py
--rw-r--r--   0 vsts      (1001) docker     (127)    65609 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_ws2_32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2275 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wscapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1471 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wsclient.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11200 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wsdapi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16329 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wsmsvc.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17715 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wsnmp32.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25864 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_wtsapi32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1876 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_xaudio2_8.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2916 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_xinput1_4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4574 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_xinputuap.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3101 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_xmllite.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3094 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_xolehlp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2387 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/definitions/win32_xpsprint.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.149512 angr-9.2.96/angr/procedures/glibc/
--rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/glibc/__ctype_b_loc.py
--rw-r--r--   0 vsts      (1001) docker     (127)      791 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/glibc/__ctype_tolower_loc.py
--rw-r--r--   0 vsts      (1001) docker     (127)      791 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/glibc/__ctype_toupper_loc.py
--rw-r--r--   0 vsts      (1001) docker     (127)      157 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/glibc/__errno_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      110 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/glibc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1520 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/glibc/__libc_init.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11094 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/glibc/__libc_start_main.py
--rw-r--r--   0 vsts      (1001) docker     (127)      660 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/glibc/dynamic_loading.py
--rw-r--r--   0 vsts      (1001) docker     (127)      146 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/glibc/scanf.py
--rw-r--r--   0 vsts      (1001) docker     (127)       75 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/glibc/sscanf.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.149512 angr-9.2.96/angr/procedures/gnulib/
--rw-r--r--   0 vsts      (1001) docker     (127)      115 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/gnulib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      181 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/gnulib/xalloc_die.py
--rw-r--r--   0 vsts      (1001) docker     (127)      239 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/gnulib/xstrtol_fatal.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.149512 angr-9.2.96/angr/procedures/java/
--rw-r--r--   0 vsts      (1001) docker     (127)     1224 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3381 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java/unconstrained.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.149512 angr-9.2.96/angr/procedures/java_io/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_io/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      335 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_io/read.py
--rw-r--r--   0 vsts      (1001) docker     (127)      613 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_io/write.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.153512 angr-9.2.96/angr/procedures/java_jni/
--rw-r--r--   0 vsts      (1001) docker     (127)    21472 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_jni/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10385 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_jni/array_operations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1056 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_jni/class_and_interface_operations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4789 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_jni/field_access.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_jni/global_and_local_refs.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9597 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_jni/method_calls.py
--rw-r--r--   0 vsts      (1001) docker     (127)      932 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_jni/not_implemented.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2725 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_jni/object_operations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2602 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_jni/string_operations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      229 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_jni/version_information.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.161512 angr-9.2.96/angr/procedures/java_lang/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_lang/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      983 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_lang/character.py
--rw-r--r--   0 vsts      (1001) docker     (127)      734 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_lang/double.py
--rw-r--r--   0 vsts      (1001) docker     (127)      255 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_lang/exit.py
--rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_lang/getsimplename.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1497 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_lang/integer.py
--rw-r--r--   0 vsts      (1001) docker     (127)      241 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_lang/load_library.py
--rw-r--r--   0 vsts      (1001) docker     (127)      346 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_lang/math.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3174 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_lang/string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1579 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_lang/stringbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)      413 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_lang/system.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.165512 angr-9.2.96/angr/procedures/java_util/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1229 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_util/collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1605 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_util/iterator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3727 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_util/list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4870 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_util/map.py
--rw-r--r--   0 vsts      (1001) docker     (127)      373 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_util/random.py
--rw-r--r--   0 vsts      (1001) docker     (127)      797 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/java_util/scanner_nextline.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.193512 angr-9.2.96/angr/procedures/libc/
--rw-r--r--   0 vsts      (1001) docker     (127)       95 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      105 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/abort.py
--rw-r--r--   0 vsts      (1001) docker     (127)      285 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/access.py
--rw-r--r--   0 vsts      (1001) docker     (127)      365 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/atoi.py
--rw-r--r--   0 vsts      (1001) docker     (127)      296 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/atol.py
--rw-r--r--   0 vsts      (1001) docker     (127)      185 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/calloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)      183 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/closelog.py
--rw-r--r--   0 vsts      (1001) docker     (127)      430 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/err.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2276 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/error.py
--rw-r--r--   0 vsts      (1001) docker     (127)      198 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/exit.py
--rw-r--r--   0 vsts      (1001) docker     (127)      590 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/fclose.py
--rw-r--r--   0 vsts      (1001) docker     (127)      572 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/feof.py
--rw-r--r--   0 vsts      (1001) docker     (127)      223 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/fflush.py
--rw-r--r--   0 vsts      (1001) docker     (127)      615 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/fgetc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2805 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/fgets.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2598 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/fopen.py
--rw-r--r--   0 vsts      (1001) docker     (127)      730 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/fprintf.py
--rw-r--r--   0 vsts      (1001) docker     (127)      537 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/fputc.py
--rw-r--r--   0 vsts      (1001) docker     (127)      662 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/fputs.py
--rw-r--r--   0 vsts      (1001) docker     (127)      614 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/fread.py
--rw-r--r--   0 vsts      (1001) docker     (127)      159 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/free.py
--rw-r--r--   0 vsts      (1001) docker     (127)      649 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/fscanf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/fseek.py
--rw-r--r--   0 vsts      (1001) docker     (127)      515 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/ftell.py
--rw-r--r--   0 vsts      (1001) docker     (127)      508 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/fwrite.py
--rw-r--r--   0 vsts      (1001) docker     (127)      315 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/getchar.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4047 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/getdelim.py
--rw-r--r--   0 vsts      (1001) docker     (127)      126 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/getegid.py
--rw-r--r--   0 vsts      (1001) docker     (127)      126 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/geteuid.py
--rw-r--r--   0 vsts      (1001) docker     (127)      125 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/getgid.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2636 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/gets.py
--rw-r--r--   0 vsts      (1001) docker     (127)      125 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/getuid.py
--rw-r--r--   0 vsts      (1001) docker     (127)      221 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/malloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3226 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/memcmp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1460 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/memcpy.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2395 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/memset.py
--rw-r--r--   0 vsts      (1001) docker     (127)      206 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/openlog.py
--rw-r--r--   0 vsts      (1001) docker     (127)      333 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/perror.py
--rw-r--r--   0 vsts      (1001) docker     (127)      846 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/printf.py
--rw-r--r--   0 vsts      (1001) docker     (127)      275 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/putchar.py
--rw-r--r--   0 vsts      (1001) docker     (127)      449 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/puts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      196 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/rand.py
--rw-r--r--   0 vsts      (1001) docker     (127)      167 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/realloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)      237 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/rewind.py
--rw-r--r--   0 vsts      (1001) docker     (127)      513 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/scanf.py
--rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/setbuf.py
--rw-r--r--   0 vsts      (1001) docker     (127)      110 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/setvbuf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1175 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/snprintf.py
--rw-r--r--   0 vsts      (1001) docker     (127)      675 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/sprintf.py
--rw-r--r--   0 vsts      (1001) docker     (127)       90 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/srand.py
--rw-r--r--   0 vsts      (1001) docker     (127)      353 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/sscanf.py
--rw-r--r--   0 vsts      (1001) docker     (127)      485 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/stpcpy.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/strcat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1771 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/strchr.py
--rw-r--r--   0 vsts      (1001) docker     (127)      818 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/strcmp.py
--rw-r--r--   0 vsts      (1001) docker     (127)      412 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/strcpy.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3540 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/strlen.py
--rw-r--r--   0 vsts      (1001) docker     (127)      501 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/strncat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7653 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/strncmp.py
--rw-r--r--   0 vsts      (1001) docker     (127)      600 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/strncpy.py
--rw-r--r--   0 vsts      (1001) docker     (127)      384 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/strnlen.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3676 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/strstr.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11852 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/strtol.py
--rw-r--r--   0 vsts      (1001) docker     (127)      273 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/strtoul.py
--rw-r--r--   0 vsts      (1001) docker     (127)      340 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/system.py
--rw-r--r--   0 vsts      (1001) docker     (127)      264 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/time.py
--rw-r--r--   0 vsts      (1001) docker     (127)      512 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/tmpnam.py
--rw-r--r--   0 vsts      (1001) docker     (127)      206 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/tolower.py
--rw-r--r--   0 vsts      (1001) docker     (127)      207 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/toupper.py
--rw-r--r--   0 vsts      (1001) docker     (127)      625 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/ungetc.py
--rw-r--r--   0 vsts      (1001) docker     (127)      415 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/vsnprintf.py
--rw-r--r--   0 vsts      (1001) docker     (127)      538 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libc/wchar.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.193512 angr-9.2.96/angr/procedures/libstdcpp/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libstdcpp/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      181 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libstdcpp/_unwind_resume.py
--rw-r--r--   0 vsts      (1001) docker     (127)      321 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libstdcpp/std____throw_bad_alloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)      320 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libstdcpp/std____throw_bad_cast.py
--rw-r--r--   0 vsts      (1001) docker     (127)      379 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libstdcpp/std____throw_length_error.py
--rw-r--r--   0 vsts      (1001) docker     (127)      378 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libstdcpp/std____throw_logic_error.py
--rw-r--r--   0 vsts      (1001) docker     (127)      268 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/libstdcpp/std__terminate.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.209512 angr-9.2.96/angr/procedures/linux_kernel/
--rw-r--r--   0 vsts      (1001) docker     (127)      111 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      569 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/access.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1045 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/arch_prctl.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1558 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/arm_user_helpers.py
--rw-r--r--   0 vsts      (1001) docker     (127)      329 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/brk.py
--rw-r--r--   0 vsts      (1001) docker     (127)      719 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/cwd.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5177 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/fstat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6392 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/fstat64.py
--rw-r--r--   0 vsts      (1001) docker     (127)      524 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/futex.py
--rw-r--r--   0 vsts      (1001) docker     (127)      375 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/getegid.py
--rw-r--r--   0 vsts      (1001) docker     (127)      375 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/geteuid.py
--rw-r--r--   0 vsts      (1001) docker     (127)      373 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/getgid.py
--rw-r--r--   0 vsts      (1001) docker     (127)      229 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/getpid.py
--rw-r--r--   0 vsts      (1001) docker     (127)      779 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/getrlimit.py
--rw-r--r--   0 vsts      (1001) docker     (127)      141 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/gettid.py
--rw-r--r--   0 vsts      (1001) docker     (127)      373 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/getuid.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1450 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/iovec.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1190 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/lseek.py
--rw-r--r--   0 vsts      (1001) docker     (127)      484 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/mmap.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1396 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/mprotect.py
--rw-r--r--   0 vsts      (1001) docker     (127)      186 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/munmap.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1076 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/openat.py
--rw-r--r--   0 vsts      (1001) docker     (127)      205 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/set_tid_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)      618 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/sigaction.py
--rw-r--r--   0 vsts      (1001) docker     (127)      748 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/sigprocmask.py
--rw-r--r--   0 vsts      (1001) docker     (127)      666 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/stat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2205 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/sysinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      236 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/tgkill.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1000 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/time.py
--rw-r--r--   0 vsts      (1001) docker     (127)      764 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/uid.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1127 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/uname.py
--rw-r--r--   0 vsts      (1001) docker     (127)      708 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/unlink.py
--rw-r--r--   0 vsts      (1001) docker     (127)      492 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_kernel/vsyscall.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.213512 angr-9.2.96/angr/procedures/linux_loader/
--rw-r--r--   0 vsts      (1001) docker     (127)      115 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_loader/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      129 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_loader/_dl_initial_error_catch_tsd.py
--rw-r--r--   0 vsts      (1001) docker     (127)      337 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_loader/_dl_rtld_lock.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1876 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_loader/sim_loader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1548 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/linux_loader/tls.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.213512 angr-9.2.96/angr/procedures/msvcr/
--rw-r--r--   0 vsts      (1001) docker     (127)      691 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/msvcr/__getmainargs.py
--rw-r--r--   0 vsts      (1001) docker     (127)      116 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/msvcr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1363 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/msvcr/_initterm.py
--rw-r--r--   0 vsts      (1001) docker     (127)      752 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/msvcr/fmode.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.213512 angr-9.2.96/angr/procedures/ntdll/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/ntdll/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2693 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/ntdll/exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.237511 angr-9.2.96/angr/procedures/posix/
--rw-r--r--   0 vsts      (1001) docker     (127)       66 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1246 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/accept.py
--rw-r--r--   0 vsts      (1001) docker     (127)      316 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/bind.py
--rw-r--r--   0 vsts      (1001) docker     (127)      174 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/bzero.py
--rw-r--r--   0 vsts      (1001) docker     (127)      739 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/chroot.py
--rw-r--r--   0 vsts      (1001) docker     (127)      200 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/close.py
--rw-r--r--   0 vsts      (1001) docker     (127)       64 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/closedir.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1917 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/dup.py
--rw-r--r--   0 vsts      (1001) docker     (127)      314 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/fcntl.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2850 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/fdopen.py
--rw-r--r--   0 vsts      (1001) docker     (127)      414 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/fileno.py
--rw-r--r--   0 vsts      (1001) docker     (127)      292 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/fork.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1383 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/getenv.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1573 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/gethostbyname.py
--rw-r--r--   0 vsts      (1001) docker     (127)      484 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/getpass.py
--rw-r--r--   0 vsts      (1001) docker     (127)      187 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/getsockopt.py
--rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/htonl.py
--rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/htons.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1950 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/inet_ntoa.py
--rw-r--r--   0 vsts      (1001) docker     (127)      315 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/listen.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5042 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/mmap.py
--rw-r--r--   0 vsts      (1001) docker     (127)      537 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/open.py
--rw-r--r--   0 vsts      (1001) docker     (127)      291 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/opendir.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2247 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/poll.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1355 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/pread64.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2402 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/pthread.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1362 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/pwrite64.py
--rw-r--r--   0 vsts      (1001) docker     (127)      252 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/read.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2161 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/readdir.py
--rw-r--r--   0 vsts      (1001) docker     (127)      275 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/recv.py
--rw-r--r--   0 vsts      (1001) docker     (127)      298 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/recvfrom.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1979 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/select.py
--rw-r--r--   0 vsts      (1001) docker     (127)      711 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/send.py
--rw-r--r--   0 vsts      (1001) docker     (127)      167 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/setsockopt.py
--rw-r--r--   0 vsts      (1001) docker     (127)      784 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/sigaction.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1654 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/sim_time.py
--rw-r--r--   0 vsts      (1001) docker     (127)      145 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/sleep.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/socket.py
--rw-r--r--   0 vsts      (1001) docker     (127)      678 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/strcasecmp.py
--rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/strdup.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2791 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/strtok_r.py
--rw-r--r--   0 vsts      (1001) docker     (127)      430 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/syslog.py
--rw-r--r--   0 vsts      (1001) docker     (127)      260 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/tz.py
--rw-r--r--   0 vsts      (1001) docker     (127)      282 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/unlink.py
--rw-r--r--   0 vsts      (1001) docker     (127)      140 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/usleep.py
--rw-r--r--   0 vsts      (1001) docker     (127)      254 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/posix/write.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1865 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/procedure_dict.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.241511 angr-9.2.96/angr/procedures/stubs/
--rw-r--r--   0 vsts      (1001) docker     (127)      219 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/stubs/CallReturn.py
--rw-r--r--   0 vsts      (1001) docker     (127)      413 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/stubs/NoReturnUnconstrained.py
--rw-r--r--   0 vsts      (1001) docker     (127)       76 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/stubs/Nop.py
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/stubs/PathTerminator.py
--rw-r--r--   0 vsts      (1001) docker     (127)      439 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/stubs/Redirect.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/stubs/ReturnChar.py
--rw-r--r--   0 vsts      (1001) docker     (127)      774 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/stubs/ReturnUnconstrained.py
--rw-r--r--   0 vsts      (1001) docker     (127)      153 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/stubs/UnresolvableCallTarget.py
--rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/stubs/UnresolvableJumpTarget.py
--rw-r--r--   0 vsts      (1001) docker     (127)      561 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/stubs/UserHook.py
--rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/stubs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      342 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/stubs/b64_decode.py
--rw-r--r--   0 vsts      (1001) docker     (127)      343 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/stubs/caller.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/stubs/crazy_scanf.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28192 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/stubs/format_parser.py
--rw-r--r--   0 vsts      (1001) docker     (127)      902 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/stubs/syscall_stub.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.241511 angr-9.2.96/angr/procedures/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/testing/manyargs.py
--rw-r--r--   0 vsts      (1001) docker     (127)      171 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/testing/retreg.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.245511 angr-9.2.96/angr/procedures/tracer/
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/tracer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      232 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/tracer/random.py
--rw-r--r--   0 vsts      (1001) docker     (127)      573 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/tracer/receive.py
--rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/tracer/transmit.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.245511 angr-9.2.96/angr/procedures/uclibc/
--rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/uclibc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      293 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/uclibc/__uClibc_main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.249511 angr-9.2.96/angr/procedures/win32/
--rw-r--r--   0 vsts      (1001) docker     (127)       97 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/EncodePointer.py
--rw-r--r--   0 vsts      (1001) docker     (127)      134 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/ExitProcess.py
--rw-r--r--   0 vsts      (1001) docker     (127)      228 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/GetCommandLine.py
--rw-r--r--   0 vsts      (1001) docker     (127)      105 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/GetCurrentProcessId.py
--rw-r--r--   0 vsts      (1001) docker     (127)      104 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/GetCurrentThreadId.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/GetLastInputInfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      940 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/GetModuleHandle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1124 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/GetProcessAffinityMask.py
--rw-r--r--   0 vsts      (1001) docker     (127)      557 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/InterlockedExchange.py
--rw-r--r--   0 vsts      (1001) docker     (127)      201 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/IsProcessorFeaturePresent.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3985 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/VirtualAlloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2274 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/VirtualProtect.py
--rw-r--r--   0 vsts      (1001) docker     (127)       86 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      277 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/critical_section.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3424 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/dynamic_loading.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1455 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/file_handles.py
--rw-r--r--   0 vsts      (1001) docker     (127)      318 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/gethostbyname.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1541 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/heap.py
--rw-r--r--   0 vsts      (1001) docker     (127)      757 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/is_bad_ptr.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2130 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/local_storage.py
--rw-r--r--   0 vsts      (1001) docker     (127)      177 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/mutex.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5332 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/sim_time.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1238 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32/system_paths.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.249511 angr-9.2.96/angr/procedures/win32_kernel/
--rw-r--r--   0 vsts      (1001) docker     (127)      423 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32_kernel/ExAllocatePool.py
--rw-r--r--   0 vsts      (1001) docker     (127)      225 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32_kernel/ExFreePoolWithTag.py
--rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win32_kernel/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.249511 angr-9.2.96/angr/procedures/win_user32/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win_user32/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win_user32/chars.py
--rw-r--r--   0 vsts      (1001) docker     (127)      377 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win_user32/keyboard.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1717 2024-03-26 17:00:59.000000 angr-9.2.96/angr/procedures/win_user32/messagebox.py
--rw-r--r--   0 vsts      (1001) docker     (127)    37186 2024-03-26 17:00:59.000000 angr-9.2.96/angr/project.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.249511 angr-9.2.96/angr/protos/
--rw-r--r--   0 vsts      (1001) docker     (127)      378 2024-03-26 17:00:59.000000 angr-9.2.96/angr/protos/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2389 2024-03-26 17:00:59.000000 angr-9.2.96/angr/protos/cfg_pb2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2146 2024-03-26 17:00:59.000000 angr-9.2.96/angr/protos/function_pb2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8527 2024-03-26 17:00:59.000000 angr-9.2.96/angr/protos/primitives_pb2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8112 2024-03-26 17:00:59.000000 angr-9.2.96/angr/protos/variables_pb2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1247 2024-03-26 17:00:59.000000 angr-9.2.96/angr/protos/xrefs_pb2.py
--rw-r--r--   0 vsts      (1001) docker     (127)        8 2024-03-26 17:00:59.000000 angr-9.2.96/angr/py.typed
--rw-r--r--   0 vsts      (1001) docker     (127)     1502 2024-03-26 17:00:59.000000 angr-9.2.96/angr/serializable.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1102 2024-03-26 17:00:59.000000 angr-9.2.96/angr/service.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39300 2024-03-26 17:00:59.000000 angr-9.2.96/angr/sim_manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18057 2024-03-26 17:00:59.000000 angr-9.2.96/angr/sim_options.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26081 2024-03-26 17:00:59.000000 angr-9.2.96/angr/sim_procedure.py
--rw-r--r--   0 vsts      (1001) docker     (127)    37826 2024-03-26 17:00:59.000000 angr-9.2.96/angr/sim_state.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12530 2024-03-26 17:00:59.000000 angr-9.2.96/angr/sim_state_options.py
--rw-r--r--   0 vsts      (1001) docker     (127)   121935 2024-03-26 17:00:59.000000 angr-9.2.96/angr/sim_type.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17228 2024-03-26 17:00:59.000000 angr-9.2.96/angr/sim_variable.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.253511 angr-9.2.96/angr/simos/
--rw-r--r--   0 vsts      (1001) docker     (127)      755 2024-03-26 17:00:59.000000 angr-9.2.96/angr/simos/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5568 2024-03-26 17:00:59.000000 angr-9.2.96/angr/simos/cgc.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21461 2024-03-26 17:00:59.000000 angr-9.2.96/angr/simos/javavm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23327 2024-03-26 17:00:59.000000 angr-9.2.96/angr/simos/linux.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18188 2024-03-26 17:00:59.000000 angr-9.2.96/angr/simos/simos.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5679 2024-03-26 17:00:59.000000 angr-9.2.96/angr/simos/snimmuc_nxp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7351 2024-03-26 17:00:59.000000 angr-9.2.96/angr/simos/userland.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26047 2024-03-26 17:00:59.000000 angr-9.2.96/angr/simos/windows.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10640 2024-03-26 17:00:59.000000 angr-9.2.96/angr/slicer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8467 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_hierarchy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.265511 angr-9.2.96/angr/state_plugins/
--rw-r--r--   0 vsts      (1001) docker     (127)      735 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12092 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/callstack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4247 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/cgc.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13310 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/concrete.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6844 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/debug_variables.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15902 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/filesystem.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5125 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/gdb.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1507 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/globals.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.265511 angr-9.2.96/angr/state_plugins/heap/
--rw-r--r--   0 vsts      (1001) docker     (127)      136 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/heap/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6229 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/heap/heap_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5412 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/heap/heap_brk.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7886 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/heap/heap_freelist.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1858 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/heap/heap_libc.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28967 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/heap/heap_ptmalloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)      793 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/heap/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19104 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/history.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11317 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/inspect.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/javavm_classloader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3403 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/jni_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23586 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/libc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6747 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/light_registers.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2364 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/log.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4209 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/loop_data.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6187 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/plugin.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27145 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/posix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8053 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/preconstrainer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6178 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/scratch.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9763 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/sim_action.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4268 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/sim_action_object.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2061 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/sim_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)    45221 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/solver.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11039 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/symbolizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30091 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/trace_additions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2643 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/uc_manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)    78095 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/unicorn_engine.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12361 2024-03-26 17:00:59.000000 angr-9.2.96/angr/state_plugins/view.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.265511 angr-9.2.96/angr/storage/
--rw-r--r--   0 vsts      (1001) docker     (127)      182 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    48379 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/file.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.269511 angr-9.2.96/angr/storage/memory_mixins/
--rw-r--r--   0 vsts      (1001) docker     (127)    11892 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1944 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/__init__.pyi
--rw-r--r--   0 vsts      (1001) docker     (127)     3402 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/actions_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16569 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/address_concretization_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2901 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/bvv_conversion_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5496 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/clouseau_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)      929 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/conditional_store_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10302 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/convenient_mappings_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6034 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/default_filler_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)      317 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/dirty_addrs_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3668 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/hex_dumper_mixin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.269511 angr-9.2.96/angr/storage/memory_mixins/javavm_memory/
--rw-r--r--   0 vsts      (1001) docker     (127)       51 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/javavm_memory/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15456 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/javavm_memory/javavm_memory_mixin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.273511 angr-9.2.96/angr/storage/memory_mixins/keyvalue_memory/
--rw-r--r--   0 vsts      (1001) docker     (127)       55 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/keyvalue_memory/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      906 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/keyvalue_memory/keyvalue_memory_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)      858 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/label_merger_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2561 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/multi_value_merger_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3412 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/name_resolution_mixin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.273511 angr-9.2.96/angr/storage/memory_mixins/paged_memory/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/paged_memory/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10282 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/paged_memory/page_backer_mixins.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28529 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/paged_memory/paged_memory_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2192 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/paged_memory/paged_memory_multivalue_mixin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.273511 angr-9.2.96/angr/storage/memory_mixins/paged_memory/pages/
--rw-r--r--   0 vsts      (1001) docker     (127)     1469 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/paged_memory/pages/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12776 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/paged_memory/pages/cooperation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3039 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/paged_memory/pages/history_tracking_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2050 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/paged_memory/pages/ispo_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14108 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/paged_memory/pages/list_page.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11302 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/paged_memory/pages/multi_values.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15981 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/paged_memory/pages/mv_list_page.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/paged_memory/pages/permissions_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1701 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/paged_memory/pages/refcount_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19139 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/paged_memory/pages/ultra_page.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1541 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/paged_memory/privileged_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3283 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/paged_memory/stack_allocation_mixin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.277511 angr-9.2.96/angr/storage/memory_mixins/regioned_memory/
--rw-r--r--   0 vsts      (1001) docker     (127)      351 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/regioned_memory/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1098 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/regioned_memory/abstract_address_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1313 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/regioned_memory/abstract_merger_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)      128 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/regioned_memory/region_category_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9196 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/regioned_memory/region_data.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4355 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/regioned_memory/region_meta_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4891 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/regioned_memory/regioned_address_concretization_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18638 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/regioned_memory/regioned_memory_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2240 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/regioned_memory/static_find_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2492 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/simple_interface_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)      502 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/simplification_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5659 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/size_resolution_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4884 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/slotted_memory.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5655 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/smart_find_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)      411 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/symbolic_merger_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)      659 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/top_merger_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2590 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/underconstrained_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1027 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_mixins/unwrapper_mixin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6253 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/memory_object.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1940 2024-03-26 17:00:59.000000 angr-9.2.96/angr/storage/pcap.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3239 2024-03-26 17:00:59.000000 angr-9.2.96/angr/tablespecs.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.281511 angr-9.2.96/angr/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)      980 2024-03-26 17:00:59.000000 angr-9.2.96/angr/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      995 2024-03-26 17:00:59.000000 angr-9.2.96/angr/utils/algo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      209 2024-03-26 17:00:59.000000 angr-9.2.96/angr/utils/constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2079 2024-03-26 17:00:59.000000 angr-9.2.96/angr/utils/cowdict.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3107 2024-03-26 17:00:59.000000 angr-9.2.96/angr/utils/dynamic_dictlist.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2091 2024-03-26 17:00:59.000000 angr-9.2.96/angr/utils/enums_conv.py
--rw-r--r--   0 vsts      (1001) docker     (127)      363 2024-03-26 17:00:59.000000 angr-9.2.96/angr/utils/env.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4217 2024-03-26 17:00:59.000000 angr-9.2.96/angr/utils/formatting.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5006 2024-03-26 17:00:59.000000 angr-9.2.96/angr/utils/funcid.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28417 2024-03-26 17:00:59.000000 angr-9.2.96/angr/utils/graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)      308 2024-03-26 17:00:59.000000 angr-9.2.96/angr/utils/lazy_import.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7202 2024-03-26 17:00:59.000000 angr-9.2.96/angr/utils/library.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1944 2024-03-26 17:00:59.000000 angr-9.2.96/angr/utils/loader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1822 2024-03-26 17:00:59.000000 angr-9.2.96/angr/utils/mp.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20431 2024-03-26 17:00:59.000000 angr-9.2.96/angr/utils/segment_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1334 2024-03-26 17:00:59.000000 angr-9.2.96/angr/utils/timing.py
--rw-r--r--   0 vsts      (1001) docker     (127)      417 2024-03-26 17:00:59.000000 angr-9.2.96/angr/utils/typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9701 2024-03-26 17:00:59.000000 angr-9.2.96/angr/vaults.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.281511 angr-9.2.96/angr.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     4769 2024-03-26 17:02:32.000000 angr-9.2.96/angr.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)    56598 2024-03-26 17:02:32.000000 angr-9.2.96/angr.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-26 17:02:32.000000 angr-9.2.96/angr.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       44 2024-03-26 17:02:32.000000 angr-9.2.96/angr.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      567 2024-03-26 17:02:32.000000 angr-9.2.96/angr.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-03-26 17:02:32.000000 angr-9.2.96/angr.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.281511 angr-9.2.96/native/
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-03-26 17:00:59.000000 angr-9.2.96/native/Makefile
--rw-r--r--   0 vsts      (1001) docker     (127)      320 2024-03-26 17:00:59.000000 angr-9.2.96/native/Makefile-win
--rw-r--r--   0 vsts      (1001) docker     (127)     1431 2024-03-26 17:00:59.000000 angr-9.2.96/native/angr_native.def
--rw-r--r--   0 vsts      (1001) docker     (127)     3940 2024-03-26 17:00:59.000000 angr-9.2.96/native/log.c
--rw-r--r--   0 vsts      (1001) docker     (127)     2754 2024-03-26 17:00:59.000000 angr-9.2.96/native/log.h
--rw-r--r--   0 vsts      (1001) docker     (127)   119496 2024-03-26 17:00:59.000000 angr-9.2.96/native/sim_unicorn.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    28878 2024-03-26 17:00:59.000000 angr-9.2.96/native/sim_unicorn.hpp
--rw-r--r--   0 vsts      (1001) docker     (127)      855 2024-03-26 17:01:07.000000 angr-9.2.96/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     1634 2024-03-26 17:02:33.285511 angr-9.2.96/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     3580 2024-03-26 17:00:59.000000 angr-9.2.96/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:02:33.281511 angr-9.2.96/tests/
--rwxr-xr-x   0 vsts      (1001) docker     (127)     3392 2024-03-26 17:00:59.000000 angr-9.2.96/tests/test_calling_conventions.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)    14468 2024-03-26 17:00:59.000000 angr-9.2.96/tests/test_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.082492 angr-9.2.97/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1327 2024-04-02 17:01:36.000000 angr-9.2.97/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      107 2024-04-02 17:01:36.000000 angr-9.2.97/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     4769 2024-04-02 17:02:57.082492 angr-9.2.97/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2603 2024-04-02 17:01:36.000000 angr-9.2.97/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.678491 angr-9.2.97/angr/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3992 2024-04-02 17:01:44.000000 angr-9.2.97/angr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1887 2024-04-02 17:01:36.000000 angr-9.2.97/angr/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.686491 angr-9.2.97/angr/analyses/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1773 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12277 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27287 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/backward_slice.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26267 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/binary_optimizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    51815 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/bindiff.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2448 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/boyscout.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2835 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/callee_cleanup_finder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40039 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/calling_convention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6361 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cdg.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.686491 angr-9.2.97/angr/analyses/cfg/
+-rw-r--r--   0 vsts      (1001) docker     (127)      321 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15450 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/cfb.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3146 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/cfg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3112 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/cfg_arch_options.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   122546 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/cfg_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   152842 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/cfg_emulated.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   218220 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/cfg_fast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26047 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/cfg_fast_soot.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5989 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/cfg_job_base.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.690491 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      361 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2083 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/amd64_elf_got.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1777 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/amd64_pe_iat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5231 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/arm_elf_fast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5273 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/const_resolver.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1441 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/default_resolvers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   101955 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/jumptable.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19350 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/mips_elf_fast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      880 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/propagator_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3019 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/resolver.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2971 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/x86_elf_pic_plt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1621 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/x86_pe_iat.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.690491 angr-9.2.97/angr/analyses/cfg_slice_to_sink/
+-rw-r--r--   0 vsts      (1001) docker     (127)      120 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg_slice_to_sink/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3982 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg_slice_to_sink/cfg_slice_to_sink.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3560 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg_slice_to_sink/graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/cfg_slice_to_sink/transitions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2969 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/class_identifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3641 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/code_tagging.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18492 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/complete_calling_conventions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16456 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/congruency_check.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.690491 angr-9.2.97/angr/analyses/data_dep/
+-rw-r--r--   0 vsts      (1001) docker     (127)      180 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/data_dep/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25296 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/data_dep/data_dependency_analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4650 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/data_dep/dep_nodes.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1527 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/data_dep/sim_act_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3386 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/datagraph_meta.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    63426 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/ddg.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.698491 angr-9.2.97/angr/analyses/decompiler/
+-rw-r--r--   0 vsts      (1001) docker     (127)      540 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61504 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/ail_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1595 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/ailgraph_walker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10576 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/block_io_finder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6531 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/block_similarity.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17199 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/block_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1205 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/call_counter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15083 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/callsite_maker.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.698491 angr-9.2.97/angr/analyses/decompiler/ccall_rewriters/
+-rw-r--r--   0 vsts      (1001) docker     (127)      102 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/ccall_rewriters/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21551 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/ccall_rewriters/amd64_ccalls.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/ccall_rewriters/rewriter_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    87477 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/clinic.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49596 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/condition_processor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/decompilation_cache.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8240 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/decompilation_options.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22137 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/decompiler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7368 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/empty_node_remover.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2867 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/expression_counters.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3545 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/expression_narrower.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2485 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/goto_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16502 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/graph_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1181 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/jump_target_collector.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/jumptable_entry_condition_rewriter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.702491 angr-9.2.97/angr/analyses/decompiler/optimization_passes/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3811 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5289 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/base_ptr_save_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15319 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/code_motion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10593 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/const_derefs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4033 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/cross_jump_reverter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17442 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/div_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10388 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/engine_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4701 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/expr_op_swapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3946 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/flip_boolean_cmp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7756 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/ite_expr_converter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6762 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/ite_region_converter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34328 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/lowered_switch_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3124 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/mod_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10420 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/multi_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14331 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/optimization_pass.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7398 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/register_save_area_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6470 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/ret_addr_save_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7828 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/ret_deduplicator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18394 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/return_duplicator_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1803 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/return_duplicator_high.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4973 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/return_duplicator_low.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12559 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/stack_canary_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4523 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/switch_default_case_duplicator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12304 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/win_stack_canary_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/optimization_passes/x86_gcc_getpc_simplifier.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.714491 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3208 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1727 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_div_const_add_a_mul_n_div_const.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1365 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_mul_const_div_shr_const.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      988 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_shl_const_sub_a.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      953 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2050 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div_const_mul_const.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      619 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_sub_a_sub_n.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9333 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/arm_cmpf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3538 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1056 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_add_n.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_and_mask.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1298 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/bitwise_or_to_logical_or.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      991 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/bool_expr_xor_1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6238 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/bswap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1020 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/coalesce_same_cascading_ifs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3691 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/const_mull_a_shift.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1583 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/constant_derefs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2578 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/conv_a_sub0_shr_and.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2070 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/conv_shl_shr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10131 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/eager_eval.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2015 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/extended_byte_and_mask.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2601 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/inlined_strcpy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4676 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/inlined_strcpy_consolidation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2084 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/invert_negated_logical_conjuction_disjunction.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1136 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/one_sub_bool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      591 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_cascading_conversions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1560 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_empty_if_body.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      739 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_noop_conversions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1635 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_bitmasks.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6583 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_conversions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1189 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_ite_branch.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1869 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_ite_comparisons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      503 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_nots.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1394 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_reinterprets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1665 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_shifts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1578 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_shifts_around_comparators.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3327 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/rewrite_bit_extractions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1809 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/rewrite_mips_gp_loads.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2814 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/rol_ror.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5282 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/sar_to_signed_div.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1477 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/simplify_pc_relative_loads.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1837 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/single_bit_cond_to_boolexpr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      940 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/single_bit_xor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4833 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/tidy_stack_addr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5385 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/redundant_label_remover.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    45489 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_identifier.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.714491 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/
+-rw-r--r--   0 vsts      (1001) docker     (127)       48 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3721 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/cascading_cond_transformer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2490 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/cascading_ifs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24008 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/expr_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6032 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/goto.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5034 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/if_.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3681 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/ifelse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5861 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/loop.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      565 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/node_address_finder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8209 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/region_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24545 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/switch_cluster_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3327 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_simplifiers/switch_expr_simplifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      717 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/region_walker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      529 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/seq_to_blocks.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8428 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/sequence_walker.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.714491 angr-9.2.97/angr/analyses/decompiler/structured_codegen/
+-rw-r--r--   0 vsts      (1001) docker     (127)      290 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structured_codegen/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3845 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structured_codegen/base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   135109 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structured_codegen/c.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      535 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structured_codegen/dummy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6773 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structured_codegen/dwarf_import.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.718491 angr-9.2.97/angr/analyses/decompiler/structuring/
+-rw-r--r--   0 vsts      (1001) docker     (127)      371 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structuring/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    48400 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structuring/dream.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   119472 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structuring/phoenix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7078 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structuring/recursive_structurer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41330 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structuring/structurer_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11964 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/structuring/structurer_nodes.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27930 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/decompiler/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    45941 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/disassembly.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2989 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/disassembly_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1245 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/dominance_frontier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10158 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/find_objects_static.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7847 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/flirt.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.718491 angr-9.2.97/angr/analyses/forward_analysis/
+-rw-r--r--   0 vsts      (1001) docker     (127)      144 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/forward_analysis/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19939 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/forward_analysis/forward_analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1579 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/forward_analysis/job_info.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.718491 angr-9.2.97/angr/analyses/forward_analysis/visitors/
+-rw-r--r--   0 vsts      (1001) docker     (127)      174 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/forward_analysis/visitors/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      713 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/forward_analysis/visitors/call_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2739 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/forward_analysis/visitors/function_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8067 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/forward_analysis/visitors/graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      711 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/forward_analysis/visitors/loop.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      768 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/forward_analysis/visitors/single_node_graph.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.722491 angr-9.2.97/angr/analyses/identifier/
+-rw-r--r--   0 vsts      (1001) docker     (127)       33 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4757 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/custom_callable.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      157 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/errors.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1749 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/func.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.726491 angr-9.2.97/angr/analyses/identifier/functions/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1059 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2110 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/atoi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3294 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/based_atoi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4353 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/fdprintf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1941 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/free.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8665 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/int2str.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3845 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/malloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1953 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/memcmp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3166 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/memcpy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1188 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/memset.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4307 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/printf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11564 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/recv_until.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2356 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/skip_calloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3186 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/skip_realloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2886 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/skip_recv_n.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4179 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/snprintf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4119 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/sprintf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      806 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/strcasecmp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3459 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/strcmp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1187 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/strcpy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      753 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/strlen.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3297 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/strncmp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2008 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/strncpy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2426 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/functions/strtol.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33287 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/identify.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13739 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/identifier/runner.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8531 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/init_finder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9412 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/loop_analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7122 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/loopfinder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.726491 angr-9.2.97/angr/analyses/propagator/
+-rw-r--r--   0 vsts      (1001) docker     (127)       43 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/propagator/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    68660 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/propagator/engine_ail.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1735 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/propagator/engine_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12491 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/propagator/engine_vex.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6890 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/propagator/outdated_definition_walker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16134 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/propagator/propagator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/propagator/tmpvar_finder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      359 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/propagator/top_checker_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/propagator/values.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1433 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/propagator/vex_vars.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16323 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/proximity_graph.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.730491 angr-9.2.97/angr/analyses/reaching_definitions/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1989 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2217 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/call_trace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14886 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/dep_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    45997 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/engine_ail.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    42934 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/engine_vex.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/external_codeloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26839 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/function_handler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2634 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/heap_allocator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11224 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/rd_initializer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23986 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/rd_state.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23988 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/reaching_definitions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1995 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reaching_definitions/subject.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   100412 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/reassembler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8941 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/soot_class_hierarchy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29868 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/stack_pointer_tracker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1711 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/static_hooker.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.730491 angr-9.2.97/angr/analyses/typehoon/
+-rw-r--r--   0 vsts      (1001) docker     (127)       31 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/typehoon/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3519 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/typehoon/dfa.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2805 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/typehoon/lifter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    48619 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/typehoon/simple_solver.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8610 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/typehoon/translator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7030 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/typehoon/typeconsts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9353 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/typehoon/typehoon.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15783 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/typehoon/typevars.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      158 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/typehoon/variance.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.734491 angr-9.2.97/angr/analyses/variable_recovery/
+-rw-r--r--   0 vsts      (1001) docker     (127)      105 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/variable_recovery/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1403 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/variable_recovery/annotations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25716 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/variable_recovery/engine_ail.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41633 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/variable_recovery/engine_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19046 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/variable_recovery/engine_vex.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4701 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/variable_recovery/irsb_scanner.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21802 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/variable_recovery/variable_recovery.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14960 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/variable_recovery/variable_recovery_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24125 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/variable_recovery/variable_recovery_fast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25224 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/veritesting.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75256 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/vfg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16173 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/vsa_ddg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3874 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/vtable.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9714 2024-04-02 17:01:36.000000 angr-9.2.97/angr/analyses/xrefs.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.734491 angr-9.2.97/angr/angrdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)      231 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6459 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/db.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4750 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/models.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.738491 angr-9.2.97/angr/angrdb/serializers/
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/serializers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1297 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/serializers/cfg_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1531 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/serializers/comments.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1696 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/serializers/funcs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3688 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/serializers/kb.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1425 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/serializers/labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2494 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/serializers/loader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4190 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/serializers/structured_code.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2383 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/serializers/variables.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1180 2024-04-02 17:01:36.000000 angr-9.2.97/angr/angrdb/serializers/xrefs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10818 2024-04-02 17:01:36.000000 angr-9.2.97/angr/annocfg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15519 2024-04-02 17:01:36.000000 angr-9.2.97/angr/blade.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14468 2024-04-02 17:01:36.000000 angr-9.2.97/angr/block.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6034 2024-04-02 17:01:36.000000 angr-9.2.97/angr/callable.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    91291 2024-04-02 17:01:36.000000 angr-9.2.97/angr/calling_conventions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5476 2024-04-02 17:01:36.000000 angr-9.2.97/angr/code_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3784 2024-04-02 17:01:36.000000 angr-9.2.97/angr/codenode.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.742491 angr-9.2.97/angr/concretization_strategies/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3727 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      438 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/any.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1341 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/any_named.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2218 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/controlled_data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      617 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/eval.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/logging.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1035 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/max.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      536 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/nonzero.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      784 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/nonzero_range.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1435 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/norepeats.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1564 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/norepeats_range.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      555 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/range.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/signed_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/single.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/solutions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      529 2024-04-02 17:01:36.000000 angr-9.2.97/angr/concretization_strategies/unlimited_range.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.742491 angr-9.2.97/angr/distributed/
+-rw-r--r--   0 vsts      (1001) docker     (127)      140 2024-04-02 17:01:36.000000 angr-9.2.97/angr/distributed/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6682 2024-04-02 17:01:36.000000 angr-9.2.97/angr/distributed/server.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6075 2024-04-02 17:01:36.000000 angr-9.2.97/angr/distributed/worker.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.742491 angr-9.2.97/angr/engines/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1066 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7468 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/concrete.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8109 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/engine.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/failure.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2546 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/hook.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.746491 angr-9.2.97/angr/engines/light/
+-rw-r--r--   0 vsts      (1001) docker     (127)      186 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/light/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23132 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/light/data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40918 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/light/engine.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.746491 angr-9.2.97/angr/engines/pcode/
+-rw-r--r--   0 vsts      (1001) docker     (127)       83 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/pcode/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28720 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/pcode/behavior.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2994 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/pcode/cc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16718 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/pcode/emulate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10551 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/pcode/engine.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    52362 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/pcode/lifter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/procedure.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.746491 angr-9.2.97/angr/engines/soot/
+-rw-r--r--   0 vsts      (1001) docker     (127)       30 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17238 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/engine.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      221 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.754491 angr-9.2.97/angr/engines/soot/expressions/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1706 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      857 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/arrayref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      781 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/binop.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      753 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/cast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1260 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/condition.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1387 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      313 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/instanceOf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      234 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/instancefieldref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4525 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/invoke.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      189 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/length.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      215 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/local.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/new.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1970 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/newArray.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3400 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/newMultiArray.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      224 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/paramref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1192 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/phi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      232 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/staticfieldref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/thisref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/expressions/unsupported.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1940 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/field_dispatcher.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1780 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/method_dispatcher.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.762491 angr-9.2.97/angr/engines/soot/statements/
+-rw-r--r--   0 vsts      (1001) docker     (127)      893 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/statements/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1271 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/statements/assign.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2094 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/statements/base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      325 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/statements/goto.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      421 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/statements/identity.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      560 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/statements/if_.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      284 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/statements/invoke.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      466 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/statements/return_.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1301 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/statements/switch.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/statements/throw.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.766491 angr-9.2.97/angr/engines/soot/values/
+-rw-r--r--   0 vsts      (1001) docker     (127)      792 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/values/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4427 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/values/arrayref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      121 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/values/base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      403 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/values/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1593 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/values/instancefieldref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      385 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/values/local.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      413 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/values/paramref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1240 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/values/staticfieldref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1107 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/values/strref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5739 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/soot/values/thisref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23679 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/successors.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2177 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/syscall.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24447 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/unicorn.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.766491 angr-9.2.97/angr/engines/vex/
+-rw-r--r--   0 vsts      (1001) docker     (127)       95 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.766491 angr-9.2.97/angr/engines/vex/claripy/
+-rw-r--r--   0 vsts      (1001) docker     (127)       40 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/claripy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    82570 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/claripy/ccall.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5123 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/claripy/datalayer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    46171 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/claripy/irop.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.770491 angr-9.2.97/angr/engines/vex/heavy/
+-rw-r--r--   0 vsts      (1001) docker     (127)      201 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/heavy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8871 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/heavy/actions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14702 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/heavy/concretizers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18699 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/heavy/dirty.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15822 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/heavy/heavy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2317 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/heavy/inspect.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3737 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/heavy/resilience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1180 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/heavy/super_fastpath.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17132 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/lifter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.770491 angr-9.2.97/angr/engines/vex/light/
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/light/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21729 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/light/light.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2002 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/light/resilience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2023 2024-04-02 17:01:36.000000 angr-9.2.97/angr/engines/vex/light/slicing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8299 2024-04-02 17:01:36.000000 angr-9.2.97/angr/errors.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.774491 angr-9.2.97/angr/exploration_techniques/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6980 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2588 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/bucketizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2262 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1167 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/dfs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17917 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/director.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3531 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/driller_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6163 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/explorer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      550 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/lengthlimiter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2583 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/local_loop_seer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11640 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/loop_seer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3091 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/manual_mergepoint.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1271 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/memory_watcher.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3520 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/oppologist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5126 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/slicecutor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9382 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/spiller.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      818 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/spiller_db.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2059 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/stochastic.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6969 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/suggestions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3122 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/symbion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1586 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/tech_builder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2976 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/threading.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      923 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/timeout.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50249 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/tracer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4413 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/unique.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1350 2024-04-02 17:01:36.000000 angr-9.2.97/angr/exploration_techniques/veritesting.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17411 2024-04-02 17:01:36.000000 angr-9.2.97/angr/factory.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.774491 angr-9.2.97/angr/flirt/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4428 2024-04-02 17:01:36.000000 angr-9.2.97/angr/flirt/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10109 2024-04-02 17:01:36.000000 angr-9.2.97/angr/flirt/build_sig.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:36.000000 angr-9.2.97/angr/graph_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18129 2024-04-02 17:01:36.000000 angr-9.2.97/angr/keyed_region.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.778491 angr-9.2.97/angr/knowledge_base/
+-rw-r--r--   0 vsts      (1001) docker     (127)       42 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_base/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4623 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_base/knowledge_base.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.778491 angr-9.2.97/angr/knowledge_plugins/
+-rw-r--r--   0 vsts      (1001) docker     (127)      697 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1597 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/callsite_prototypes.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.778491 angr-9.2.97/angr/knowledge_plugins/cfg/
+-rw-r--r--   0 vsts      (1001) docker     (127)      382 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/cfg/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2302 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/cfg/cfg_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41756 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/cfg/cfg_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17229 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/cfg/cfg_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2145 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/cfg/indirect_jump.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5040 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/cfg/memory_data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      304 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/comments.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1027 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/custom_strings.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      839 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8189 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/debug_variables.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.782491 angr-9.2.97/angr/knowledge_plugins/functions/
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/functions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    66932 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/functions/function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18990 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/functions/function_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11916 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/functions/function_parser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4971 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/functions/soot_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1024 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/indirect_jumps.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.786491 angr-9.2.97/angr/knowledge_plugins/key_definitions/
+-rw-r--r--   0 vsts      (1001) docker     (127)      397 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9753 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/atoms.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8661 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/definition.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3907 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/environment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      922 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/heap_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3251 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/key_definition_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40482 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/live_definitions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7140 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/liveness.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7312 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/rd_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1682 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/tag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1236 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/undefined.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1510 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/unknown_size.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7468 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/key_definitions/uses.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3137 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4373 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/patches.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      733 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/plugin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.786491 angr-9.2.97/angr/knowledge_plugins/propagations/
+-rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/propagations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7706 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/propagations/prop_value.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2122 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/propagations/propagation_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2786 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/propagations/propagation_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39023 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/propagations/states.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.786491 angr-9.2.97/angr/knowledge_plugins/structured_code/
+-rw-r--r--   0 vsts      (1001) docker     (127)       43 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/structured_code/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2071 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/structured_code/manager.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.786491 angr-9.2.97/angr/knowledge_plugins/sync/
+-rw-r--r--   0 vsts      (1001) docker     (127)       44 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/sync/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9276 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/sync/sync_controller.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2038 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.786491 angr-9.2.97/angr/knowledge_plugins/variables/
+-rw-r--r--   0 vsts      (1001) docker     (127)       60 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/variables/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3751 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/variables/variable_access.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    45603 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/variables/variable_manager.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.794491 angr-9.2.97/angr/knowledge_plugins/xrefs/
+-rw-r--r--   0 vsts      (1001) docker     (127)       94 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/xrefs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4963 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/xrefs/xref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4009 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/xrefs/xref_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      271 2024-04-02 17:01:36.000000 angr-9.2.97/angr/knowledge_plugins/xrefs/xref_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.798491 angr-9.2.97/angr/misc/
+-rw-r--r--   0 vsts      (1001) docker     (127)      237 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      807 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/ansi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3426 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/autoimport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4241 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/bug_report.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4486 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/hookset.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1943 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/import_hooks.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4225 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/loggers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1276 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/picklable_lock.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9370 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/plugins.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      509 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/range.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      593 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/testing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      701 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/ux.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1453 2024-04-02 17:01:36.000000 angr-9.2.97/angr/misc/weakpatch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.798491 angr-9.2.97/angr/procedures/
+-rw-r--r--   0 vsts      (1001) docker     (127)      119 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.798491 angr-9.2.97/angr/procedures/advapi32/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/advapi32/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.798491 angr-9.2.97/angr/procedures/cgc/
+-rw-r--r--   0 vsts      (1001) docker     (127)       76 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/cgc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      224 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/cgc/_terminate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3371 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/cgc/allocate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1984 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/cgc/deallocate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2802 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/cgc/fdwait.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2334 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/cgc/random.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3758 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/cgc/receive.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2368 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/cgc/transmit.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.946492 angr-9.2.97/angr/procedures/definitions/
+-rw-r--r--   0 vsts      (1001) docker     (127)    32023 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/cgc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   394191 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/glibc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/gnulib.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      700 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/libstdcpp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   238887 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/linux_kernel.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      219 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/linux_loader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      601 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/msvcr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1795 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/parse_syscalls_from_local_system.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   110573 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/parse_win32json.py
+-rw-r--r--   0 vsts      (1001) docker     (127)  9998064 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/types_win32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1458 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_api-ms-win-dx-d3dkmt-l1-1-4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1000 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_api-ms-win-dx-d3dkmt-l1-1-6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22852 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_clfs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   111981 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_fltmgr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1730 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_fwpkclnt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    68446 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_fwpuclnt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    37307 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_gdi32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11415 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_hal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12527 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_ksecdd.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33948 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_ndis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   593050 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_ntoskrnl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9862 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_offreg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1980 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_pshed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3478 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_secur32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1942 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/wdk_vhfum.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1553 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_aclui.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7877 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_activeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   310929 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_advapi32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22314 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_advpack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3430 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_amsi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3769 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3051 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      922 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-apiquery-l2-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1060 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-backgroundtask-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1134 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1167 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1488 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-enclave-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1037 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-errorhandling-l1-1-3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2317 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1217 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4874 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-file-fromapp-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1125 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-handle-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5164 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-ioring-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2219 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-marshal-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2528 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1492 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3867 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2362 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2378 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8406 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-path-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1547 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1562 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1429 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1850 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1281 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-slapi-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1682 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-state-helpers-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1540 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-synch-l1-2-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      995 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1184 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1467 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      951 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1537 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-util-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3268 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3777 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3228 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1162 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-registration-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      901 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-robuffer-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1694 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-roparameterizediid-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10986 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1550 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1653 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-wow64-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6949 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6680 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-dx-d3dkmt-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1043 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-deviceinformation-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1347 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-expandedresources-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3983 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1753 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5014 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2233 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4359 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1207 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-mm-misc-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3912 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-net-isolation-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1434 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-security-base-l1-2-2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1041 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1100 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1289 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1344 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1833 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1687 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2545 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      994 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1817 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-shcore-stream-winrt-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3586 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-wsl-api-l1-1-0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1117 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_apphelp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17589 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_authz.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2884 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_avicap32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18938 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_avifil32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5529 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_avrt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1328 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_bcp47mrm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24333 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_bcrypt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1325 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_bcryptprimitives.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17641 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_bluetoothapis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10950 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_bthprops.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3094 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_bthprops_cpl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16642 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_cabinet.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6820 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_certadm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4345 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_certpoleng.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   101560 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_cfgmgr32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26407 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_chakra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14271 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_cldapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24138 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_clfsw32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   111741 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_clusapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43365 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_comctl32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4894 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_comdlg32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2651 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_compstui.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19474 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_computecore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16032 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_computenetwork.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4405 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_computestorage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2241 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_comsvcs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1201 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_coremessaging.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11823 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_credui.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   105559 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_crypt32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3864 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_cryptnet.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4935 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_cryptui.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9065 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_cryptxml.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1769 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_cscapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5253 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_d2d1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11546 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_d3d10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_d3d10_1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3575 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_d3d11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4078 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_d3d12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3002 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_d3d9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13432 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_d3dcompiler_47.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4827 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_d3dcsx.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7266 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_davclnt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2063 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dbgeng.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   109042 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dbghelp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1028 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dbgmodel.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7151 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dciman32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4837 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dcomp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4233 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ddraw.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1134 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_deviceaccess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1145 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dflayout.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5570 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dhcpcsvc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2967 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dhcpcsvc6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    81410 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dhcpsapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13697 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_diagnosticdataquery.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1243 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dinput8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1621 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_directml.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1261 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dmprocessxmlfiltered.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22815 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dnsapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5579 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_drt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3373 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_drtprov.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1445 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_drttransport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5367 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dsound.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11582 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dsparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2935 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dsprop.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6189 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dssec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1855 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dsuiext.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9715 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dwmapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1120 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dwrite.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1484 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dxcompiler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1061 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dxcore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2185 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dxgi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14554 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_dxva2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10117 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_eappcfg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9178 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_eappprxy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1311 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_efswrt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2446 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_elscore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   105927 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_esent.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3146 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_evr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1687 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_faultrep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2401 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_fhsvcctl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2011 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_firewallapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12020 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_fltlib.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4105 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_fontsub.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1227 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_forceinline.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    93548 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_fwpuclnt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1129 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_fxsutility.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   148174 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_gdi32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   247483 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_gdiplus.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16771 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_glu32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2162 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_gpedit.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1678 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_hhctrl_ocx.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21797 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_hid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12512 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_hlink.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1027 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_hrtfapo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19733 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_httpapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12533 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_icm32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1161 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_icmui.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   373759 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_icu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10129 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ieframe.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11559 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_imagehlp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3884 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_imgutil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28246 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_imm32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8100 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_infocardapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8943 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_inkobjcore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    65729 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_iphlpapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28599 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_iscsidsc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1293 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_isolatedwindowsenvironmentutils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   505053 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_kernel32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3158 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_kernelbase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2060 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_keycredmgr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3689 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ksproxy_ax.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4328 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ksuser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14607 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ktmw32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1582 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_licenseprotection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4334 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_loadperf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6878 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_magnification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25169 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mapi32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1411 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mdmlocalmanagement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4765 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mdmregistration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17507 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1358 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mfcore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    45685 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mfplat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1326 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mfplay.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2429 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mfreadwrite.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4363 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mfsensorgroup.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1451 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mfsrcsnk.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4531 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mgmtapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1232 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1326 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mmdevapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19241 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mpr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    47666 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mprapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13037 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mqrt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11736 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mrmsupport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19430 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msacm32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   183424 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msajapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34895 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mscms.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11975 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mscoree.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1327 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msctfmonitor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7687 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msdelta.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4589 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msdmo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39076 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msdrm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   103106 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2796 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msimg32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11181 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mspatcha.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6011 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mspatchc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2844 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msports.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7471 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msrating.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7594 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mssign32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mstask.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16749 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_msvfw32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9190 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mswsock.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      973 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_mtxdm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19693 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ncrypt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6200 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ndfapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86057 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_netapi32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3436 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_netsh.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1151 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_netshell.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6101 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_newdev.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11168 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ninput.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_normaliz.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27742 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ntdll.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1087 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ntdllk.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    35639 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ntdsapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4407 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ntlanman.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    94760 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_odbc32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8509 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_odbcbcp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   103812 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ole32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7007 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_oleacc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   123410 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_oleaut32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6811 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_oledlg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2609 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ondemandconnroutehelper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75467 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_opengl32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1461 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_opmxbox.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    32523 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_p2p.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12455 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_p2pgraph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39415 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_pdh.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14293 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_peerdist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    32180 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_powrprof.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_prntvpt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7998 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_projectedfslib.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    69946 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_propsys.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10760 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_psapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1362 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_quartz.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2051 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_query.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5253 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_qwave.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30989 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_rasapi32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2820 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_rasdlg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    54566 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_resutils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1012 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_rometadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22447 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_rpcns4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1683 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_rpcproxy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   148359 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_rpcrt4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4988 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_rstrtmgr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36043 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_rtm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15136 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_rtutils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9078 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_rtworkq.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_sas.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1646 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_scarddlg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3588 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_schannel.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1712 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_sechost.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    37550 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_secur32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1495 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_sensapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13284 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_sensorsutilsv2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157765 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_setupapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2546 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_sfc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1932 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_shdocvw.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    81141 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_shell32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   108109 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_shlwapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14350 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_slc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2850 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_slcext.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1143 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_slwga.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6443 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_snmpapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9685 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_spoolss.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      954 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_srclient.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3752 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_srpapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3032 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_sspicli.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1150 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_sti.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9597 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_t2embed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    94966 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_tapi32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4951 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_tbs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11389 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_tdh.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4744 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_tokenbinding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8278 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_traffic.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4327 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_txfw32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1627 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ualapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    31556 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_uiautomationcore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27741 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_urlmon.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   252469 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_user32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15838 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_userenv.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23757 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_usp10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    31235 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_uxtheme.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1567 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_verifier.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7235 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3659 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_vertdll.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13507 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_virtdisk.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6032 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_vmdevicehost.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17637 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_vmsavedstatedumpprovider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      987 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_vssapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2698 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wcmapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3339 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wdsbp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13944 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wdsclientapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2846 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wdsmc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13248 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wdspxe.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4149 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wdstptc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4708 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_webauthn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   106080 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_webservices.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7433 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_websocket.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6419 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wecapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7708 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16155 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wevtapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21479 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winbio.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1003 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_windows_ai_machinelearning.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      929 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_windows_data_pdf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3260 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_windows_media_mediacontrol.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      965 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_windows_networking.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1722 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_windows_ui_xaml.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4488 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_windowscodecs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22678 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winfax.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22808 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winhttp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2752 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winhvemulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40942 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winhvplatform.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   116017 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wininet.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      969 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winml.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    55061 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winmm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29221 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winscard.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   114656 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winspool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70042 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winspool_drv.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22342 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wintrust.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14539 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_winusb.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30095 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wlanapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1412 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wlanui.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    97431 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wldap32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4202 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wldp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3239 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wmvcore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1385 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wnvapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5271 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wofutil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    65609 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_ws2_32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2275 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wscapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1471 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wsclient.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11200 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wsdapi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16329 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wsmsvc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17715 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wsnmp32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25864 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_wtsapi32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1876 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_xaudio2_8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2916 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_xinput1_4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4574 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_xinputuap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3101 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_xmllite.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3094 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_xolehlp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2387 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/definitions/win32_xpsprint.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.946492 angr-9.2.97/angr/procedures/glibc/
+-rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/glibc/__ctype_b_loc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      791 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/glibc/__ctype_tolower_loc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      791 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/glibc/__ctype_toupper_loc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      157 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/glibc/__errno_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      110 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/glibc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1520 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/glibc/__libc_init.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11094 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/glibc/__libc_start_main.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      660 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/glibc/dynamic_loading.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      146 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/glibc/scanf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       75 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/glibc/sscanf.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.950492 angr-9.2.97/angr/procedures/gnulib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      115 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/gnulib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      181 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/gnulib/xalloc_die.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      239 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/gnulib/xstrtol_fatal.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.950492 angr-9.2.97/angr/procedures/java/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1224 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3381 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java/unconstrained.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.950492 angr-9.2.97/angr/procedures/java_io/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_io/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      335 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_io/read.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      613 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_io/write.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.954492 angr-9.2.97/angr/procedures/java_jni/
+-rw-r--r--   0 vsts      (1001) docker     (127)    21472 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_jni/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10385 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_jni/array_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1056 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_jni/class_and_interface_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4789 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_jni/field_access.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_jni/global_and_local_refs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9597 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_jni/method_calls.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      932 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_jni/not_implemented.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2725 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_jni/object_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2602 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_jni/string_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      229 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_jni/version_information.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.958492 angr-9.2.97/angr/procedures/java_lang/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      983 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/character.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      734 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/double.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      255 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/exit.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/getsimplename.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1497 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/integer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      241 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/load_library.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      346 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/math.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3174 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1579 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/stringbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      413 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_lang/system.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.958492 angr-9.2.97/angr/procedures/java_util/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1229 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_util/collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1605 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_util/iterator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3727 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_util/list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4870 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_util/map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      373 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_util/random.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      797 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/java_util/scanner_nextline.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.994492 angr-9.2.97/angr/procedures/libc/
+-rw-r--r--   0 vsts      (1001) docker     (127)       95 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      105 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/abort.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      285 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/access.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      365 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/atoi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      296 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/atol.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      185 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/calloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      183 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/closelog.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      430 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/err.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2276 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/error.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      198 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/exit.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      590 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fclose.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      572 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/feof.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      223 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fflush.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      615 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fgetc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2805 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fgets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2598 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fopen.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      730 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fprintf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      537 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fputc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      662 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fputs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      614 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fread.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      159 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/free.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      649 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fscanf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fseek.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      515 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/ftell.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      508 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/fwrite.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      315 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/getchar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4047 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/getdelim.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      126 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/getegid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      126 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/geteuid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      125 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/getgid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2636 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/gets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      125 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/getuid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      221 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/malloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3226 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/memcmp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1460 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/memcpy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2395 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/memset.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      206 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/openlog.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      333 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/perror.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      846 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/printf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      275 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/putchar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      449 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/puts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      196 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/rand.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      167 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/realloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      237 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/rewind.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      513 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/scanf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/setbuf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      110 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/setvbuf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1175 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/snprintf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      675 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/sprintf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       90 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/srand.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      353 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/sscanf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      485 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/stpcpy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strcat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1771 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strchr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      818 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strcmp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      412 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strcpy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3540 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strlen.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      501 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strncat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7653 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strncmp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      600 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strncpy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      384 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strnlen.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3676 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strstr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11852 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strtol.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      273 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/strtoul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      340 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/system.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      264 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/time.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      512 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/tmpnam.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      206 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/tolower.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      207 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/toupper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      625 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/ungetc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      415 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/vsnprintf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      538 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libc/wchar.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:56.994492 angr-9.2.97/angr/procedures/libstdcpp/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libstdcpp/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      181 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libstdcpp/_unwind_resume.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      321 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libstdcpp/std____throw_bad_alloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      320 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libstdcpp/std____throw_bad_cast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      379 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libstdcpp/std____throw_length_error.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      378 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libstdcpp/std____throw_logic_error.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      268 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/libstdcpp/std__terminate.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.006492 angr-9.2.97/angr/procedures/linux_kernel/
+-rw-r--r--   0 vsts      (1001) docker     (127)      111 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      569 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/access.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1045 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/arch_prctl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1558 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/arm_user_helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      329 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/brk.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      719 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/cwd.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5177 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/fstat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6392 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/fstat64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      524 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/futex.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      375 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/getegid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      375 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/geteuid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      373 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/getgid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      229 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/getpid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      779 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/getrlimit.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      141 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/gettid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      373 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/getuid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1450 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/iovec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1190 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/lseek.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      484 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/mmap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1396 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/mprotect.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      186 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/munmap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1076 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/openat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      205 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/set_tid_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      618 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/sigaction.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      748 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/sigprocmask.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      666 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/stat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2205 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/sysinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      236 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/tgkill.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1000 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/time.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      764 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/uid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1127 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/uname.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      708 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/unlink.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      492 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_kernel/vsyscall.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.006492 angr-9.2.97/angr/procedures/linux_loader/
+-rw-r--r--   0 vsts      (1001) docker     (127)      115 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_loader/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      129 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_loader/_dl_initial_error_catch_tsd.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      337 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_loader/_dl_rtld_lock.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1876 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_loader/sim_loader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1548 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/linux_loader/tls.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.006492 angr-9.2.97/angr/procedures/msvcr/
+-rw-r--r--   0 vsts      (1001) docker     (127)      691 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/msvcr/__getmainargs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      116 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/msvcr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1363 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/msvcr/_initterm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      752 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/msvcr/fmode.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.010492 angr-9.2.97/angr/procedures/ntdll/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/ntdll/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2693 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/ntdll/exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.022492 angr-9.2.97/angr/procedures/posix/
+-rw-r--r--   0 vsts      (1001) docker     (127)       66 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1246 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/accept.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      316 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/bind.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      174 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/bzero.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      739 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/chroot.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      200 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/close.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       64 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/closedir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1917 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/dup.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      314 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/fcntl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2850 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/fdopen.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      414 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/fileno.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      292 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/fork.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1383 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/getenv.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1573 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/gethostbyname.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      484 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/getpass.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      187 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/getsockopt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/htonl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/htons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1950 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/inet_ntoa.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      315 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/listen.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5042 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/mmap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      537 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/open.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      291 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/opendir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2247 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/poll.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1355 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/pread64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2402 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/pthread.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1362 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/pwrite64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      252 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/read.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2161 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/readdir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      275 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/recv.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      298 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/recvfrom.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1979 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/select.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      711 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/send.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      167 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/setsockopt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      784 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/sigaction.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1654 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/sim_time.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      145 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/sleep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/socket.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      678 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/strcasecmp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/strdup.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2791 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/strtok_r.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      430 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/syslog.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      260 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/tz.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      282 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/unlink.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      140 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/usleep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      254 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/posix/write.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1865 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/procedure_dict.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.026492 angr-9.2.97/angr/procedures/stubs/
+-rw-r--r--   0 vsts      (1001) docker     (127)      219 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/CallReturn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      413 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/NoReturnUnconstrained.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       76 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/Nop.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/PathTerminator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      439 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/Redirect.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/ReturnChar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      774 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/ReturnUnconstrained.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      153 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/UnresolvableCallTarget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/UnresolvableJumpTarget.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      561 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/UserHook.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       67 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      342 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/b64_decode.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      343 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/caller.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/crazy_scanf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28192 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/format_parser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      902 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/stubs/syscall_stub.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.026492 angr-9.2.97/angr/procedures/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/testing/manyargs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      171 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/testing/retreg.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.030492 angr-9.2.97/angr/procedures/tracer/
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/tracer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      232 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/tracer/random.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      573 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/tracer/receive.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/tracer/transmit.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.030492 angr-9.2.97/angr/procedures/uclibc/
+-rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/uclibc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      293 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/uclibc/__uClibc_main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.038492 angr-9.2.97/angr/procedures/win32/
+-rw-r--r--   0 vsts      (1001) docker     (127)       97 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/EncodePointer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      134 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/ExitProcess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      228 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/GetCommandLine.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      105 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/GetCurrentProcessId.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      104 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/GetCurrentThreadId.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/GetLastInputInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      940 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/GetModuleHandle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1124 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/GetProcessAffinityMask.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      557 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/InterlockedExchange.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      201 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/IsProcessorFeaturePresent.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3985 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/VirtualAlloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2274 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/VirtualProtect.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       86 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      277 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/critical_section.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3424 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/dynamic_loading.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1455 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/file_handles.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      318 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/gethostbyname.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1541 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/heap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      757 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/is_bad_ptr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2130 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/local_storage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      177 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/mutex.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5332 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/sim_time.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1238 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32/system_paths.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.038492 angr-9.2.97/angr/procedures/win32_kernel/
+-rw-r--r--   0 vsts      (1001) docker     (127)      423 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32_kernel/ExAllocatePool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      225 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32_kernel/ExFreePoolWithTag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win32_kernel/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.038492 angr-9.2.97/angr/procedures/win_user32/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win_user32/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win_user32/chars.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      377 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win_user32/keyboard.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1717 2024-04-02 17:01:36.000000 angr-9.2.97/angr/procedures/win_user32/messagebox.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    37186 2024-04-02 17:01:36.000000 angr-9.2.97/angr/project.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.042492 angr-9.2.97/angr/protos/
+-rw-r--r--   0 vsts      (1001) docker     (127)      378 2024-04-02 17:01:36.000000 angr-9.2.97/angr/protos/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2389 2024-04-02 17:01:36.000000 angr-9.2.97/angr/protos/cfg_pb2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2146 2024-04-02 17:01:36.000000 angr-9.2.97/angr/protos/function_pb2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8527 2024-04-02 17:01:36.000000 angr-9.2.97/angr/protos/primitives_pb2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8112 2024-04-02 17:01:36.000000 angr-9.2.97/angr/protos/variables_pb2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1247 2024-04-02 17:01:36.000000 angr-9.2.97/angr/protos/xrefs_pb2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        8 2024-04-02 17:01:36.000000 angr-9.2.97/angr/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (127)     1502 2024-04-02 17:01:36.000000 angr-9.2.97/angr/serializable.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1102 2024-04-02 17:01:36.000000 angr-9.2.97/angr/service.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39300 2024-04-02 17:01:36.000000 angr-9.2.97/angr/sim_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18057 2024-04-02 17:01:36.000000 angr-9.2.97/angr/sim_options.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26081 2024-04-02 17:01:36.000000 angr-9.2.97/angr/sim_procedure.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    37826 2024-04-02 17:01:36.000000 angr-9.2.97/angr/sim_state.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12530 2024-04-02 17:01:36.000000 angr-9.2.97/angr/sim_state_options.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   121935 2024-04-02 17:01:36.000000 angr-9.2.97/angr/sim_type.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17228 2024-04-02 17:01:36.000000 angr-9.2.97/angr/sim_variable.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.046492 angr-9.2.97/angr/simos/
+-rw-r--r--   0 vsts      (1001) docker     (127)      755 2024-04-02 17:01:36.000000 angr-9.2.97/angr/simos/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5568 2024-04-02 17:01:36.000000 angr-9.2.97/angr/simos/cgc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21461 2024-04-02 17:01:36.000000 angr-9.2.97/angr/simos/javavm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23327 2024-04-02 17:01:36.000000 angr-9.2.97/angr/simos/linux.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18275 2024-04-02 17:01:36.000000 angr-9.2.97/angr/simos/simos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5679 2024-04-02 17:01:36.000000 angr-9.2.97/angr/simos/snimmuc_nxp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7351 2024-04-02 17:01:36.000000 angr-9.2.97/angr/simos/userland.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26047 2024-04-02 17:01:36.000000 angr-9.2.97/angr/simos/windows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10640 2024-04-02 17:01:36.000000 angr-9.2.97/angr/slicer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8467 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_hierarchy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.054492 angr-9.2.97/angr/state_plugins/
+-rw-r--r--   0 vsts      (1001) docker     (127)      735 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12092 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/callstack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4247 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/cgc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13310 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/concrete.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6844 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/debug_variables.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15902 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/filesystem.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5125 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/gdb.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1507 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/globals.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.054492 angr-9.2.97/angr/state_plugins/heap/
+-rw-r--r--   0 vsts      (1001) docker     (127)      136 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/heap/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6229 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/heap/heap_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5412 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/heap/heap_brk.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7886 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/heap/heap_freelist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1858 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/heap/heap_libc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28967 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/heap/heap_ptmalloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      793 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/heap/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19104 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/history.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11317 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/inspect.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/javavm_classloader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3403 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/jni_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23586 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/libc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6747 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/light_registers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2364 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4209 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/loop_data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6187 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27145 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/posix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8053 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/preconstrainer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6178 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/scratch.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9763 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/sim_action.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4268 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/sim_action_object.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2061 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/sim_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    45221 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/solver.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11039 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/symbolizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30091 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/trace_additions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2643 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/uc_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    78095 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/unicorn_engine.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12361 2024-04-02 17:01:36.000000 angr-9.2.97/angr/state_plugins/view.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.058493 angr-9.2.97/angr/storage/
+-rw-r--r--   0 vsts      (1001) docker     (127)      182 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    48379 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/file.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.066492 angr-9.2.97/angr/storage/memory_mixins/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11944 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1944 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/__init__.pyi
+-rw-r--r--   0 vsts      (1001) docker     (127)     3402 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/actions_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16569 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/address_concretization_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2901 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/bvv_conversion_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5496 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/clouseau_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      929 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/conditional_store_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10302 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/convenient_mappings_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6034 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/default_filler_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      317 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/dirty_addrs_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3668 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/hex_dumper_mixin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.066492 angr-9.2.97/angr/storage/memory_mixins/javavm_memory/
+-rw-r--r--   0 vsts      (1001) docker     (127)       51 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/javavm_memory/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15456 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/javavm_memory/javavm_memory_mixin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.066492 angr-9.2.97/angr/storage/memory_mixins/keyvalue_memory/
+-rw-r--r--   0 vsts      (1001) docker     (127)       55 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/keyvalue_memory/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      906 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/keyvalue_memory/keyvalue_memory_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      858 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/label_merger_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3036 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/multi_value_merger_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3412 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/name_resolution_mixin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.070492 angr-9.2.97/angr/storage/memory_mixins/paged_memory/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10282 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/page_backer_mixins.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29219 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/paged_memory_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2192 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/paged_memory_multivalue_mixin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.070492 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1469 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12776 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/cooperation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3039 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/history_tracking_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2050 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/ispo_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14108 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/list_page.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11302 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/multi_values.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17647 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/mv_list_page.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/permissions_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1701 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/refcount_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19139 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/ultra_page.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1541 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/privileged_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3283 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/paged_memory/stack_allocation_mixin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.074493 angr-9.2.97/angr/storage/memory_mixins/regioned_memory/
+-rw-r--r--   0 vsts      (1001) docker     (127)      351 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/regioned_memory/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1098 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/regioned_memory/abstract_address_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1313 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/regioned_memory/abstract_merger_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      128 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/regioned_memory/region_category_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9196 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/regioned_memory/region_data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4355 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/regioned_memory/region_meta_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4891 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/regioned_memory/regioned_address_concretization_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18638 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/regioned_memory/regioned_memory_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2240 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/regioned_memory/static_find_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2492 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/simple_interface_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      502 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/simplification_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5659 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/size_resolution_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4884 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/slotted_memory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5655 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/smart_find_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      411 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/symbolic_merger_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      659 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/top_merger_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2590 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/underconstrained_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1027 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_mixins/unwrapper_mixin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6253 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/memory_object.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1940 2024-04-02 17:01:36.000000 angr-9.2.97/angr/storage/pcap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3239 2024-04-02 17:01:36.000000 angr-9.2.97/angr/tablespecs.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.078492 angr-9.2.97/angr/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)      980 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      995 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/algo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      209 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2160 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/cowdict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3107 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/dynamic_dictlist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2091 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/enums_conv.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      363 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/env.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4217 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/formatting.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5240 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/funcid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28417 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      308 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/lazy_import.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7202 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/library.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1944 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/loader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1825 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/mp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20431 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/segment_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1334 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/timing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      417 2024-04-02 17:01:36.000000 angr-9.2.97/angr/utils/typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9701 2024-04-02 17:01:36.000000 angr-9.2.97/angr/vaults.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.078492 angr-9.2.97/angr.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4769 2024-04-02 17:02:56.000000 angr-9.2.97/angr.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    56598 2024-04-02 17:02:56.000000 angr-9.2.97/angr.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-02 17:02:56.000000 angr-9.2.97/angr.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       44 2024-04-02 17:02:56.000000 angr-9.2.97/angr.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      567 2024-04-02 17:02:56.000000 angr-9.2.97/angr.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-04-02 17:02:56.000000 angr-9.2.97/angr.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.078492 angr-9.2.97/native/
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-02 17:01:36.000000 angr-9.2.97/native/Makefile
+-rw-r--r--   0 vsts      (1001) docker     (127)      320 2024-04-02 17:01:36.000000 angr-9.2.97/native/Makefile-win
+-rw-r--r--   0 vsts      (1001) docker     (127)     1431 2024-04-02 17:01:36.000000 angr-9.2.97/native/angr_native.def
+-rw-r--r--   0 vsts      (1001) docker     (127)     3940 2024-04-02 17:01:36.000000 angr-9.2.97/native/log.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     2754 2024-04-02 17:01:36.000000 angr-9.2.97/native/log.h
+-rw-r--r--   0 vsts      (1001) docker     (127)   119496 2024-04-02 17:01:36.000000 angr-9.2.97/native/sim_unicorn.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    28878 2024-04-02 17:01:36.000000 angr-9.2.97/native/sim_unicorn.hpp
+-rw-r--r--   0 vsts      (1001) docker     (127)      855 2024-04-02 17:01:44.000000 angr-9.2.97/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1634 2024-04-02 17:02:57.082492 angr-9.2.97/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     3580 2024-04-02 17:01:36.000000 angr-9.2.97/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:57.078492 angr-9.2.97/tests/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     3392 2024-04-02 17:01:36.000000 angr-9.2.97/tests/test_calling_conventions.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)    14468 2024-04-02 17:01:36.000000 angr-9.2.97/tests/test_types.py
```

### Comparing `angr-9.2.96/LICENSE` & `angr-9.2.97/LICENSE`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/PKG-INFO` & `angr-9.2.97/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angr
-Version: 9.2.96
+Version: 9.2.97
 Summary: A multi-architecture binary analysis toolkit, with the ability to perform dynamic symbolic execution and various static analyses on binaries
 Home-page: https://github.com/angr/angr
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -13,31 +13,31 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: CppHeaderParser
 Requires-Dist: GitPython
-Requires-Dist: ailment==9.2.96
-Requires-Dist: archinfo==9.2.96
+Requires-Dist: ailment==9.2.97
+Requires-Dist: archinfo==9.2.97
 Requires-Dist: cachetools
 Requires-Dist: capstone==5.0.0.post1
 Requires-Dist: cffi>=1.14.0
-Requires-Dist: claripy==9.2.96
-Requires-Dist: cle==9.2.96
+Requires-Dist: claripy==9.2.97
+Requires-Dist: cle==9.2.97
 Requires-Dist: dpkt
 Requires-Dist: itanium-demangler
 Requires-Dist: mulpyplexer
 Requires-Dist: nampa
 Requires-Dist: networkx!=2.8.1,>=2.0
 Requires-Dist: protobuf>=3.19.0
 Requires-Dist: psutil
 Requires-Dist: pycparser>=2.18
 Requires-Dist: pyformlang
-Requires-Dist: pyvex==9.2.96
+Requires-Dist: pyvex==9.2.97
 Requires-Dist: rich>=13.1.0
 Requires-Dist: rpyc
 Requires-Dist: sortedcontainers
 Requires-Dist: sympy
 Requires-Dist: unicorn==2.0.1.post1
 Requires-Dist: unique-log-filter
 Requires-Dist: colorama; platform_system == "Windows"
```

### Comparing `angr-9.2.96/README.md` & `angr-9.2.97/README.md`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/__init__.py` & `angr-9.2.97/angr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=wildcard-import
 # pylint: disable=wrong-import-position
 
-__version__ = "9.2.96"
+__version__ = "9.2.97"
 
 if bytes is str:
     raise Exception(
         """
 
 =-=-=-=-=-=-=-=-=-=-=-=-=  WELCOME TO THE FUTURE!  =-=-=-=-=-=-=-=-=-=-=-=-=-=
```

### Comparing `angr-9.2.96/angr/__main__.py` & `angr-9.2.97/angr/__main__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/__init__.py` & `angr-9.2.97/angr/analyses/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/analysis.py` & `angr-9.2.97/angr/analyses/analysis.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/backward_slice.py` & `angr-9.2.97/angr/analyses/backward_slice.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/binary_optimizer.py` & `angr-9.2.97/angr/analyses/binary_optimizer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/bindiff.py` & `angr-9.2.97/angr/analyses/bindiff.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/boyscout.py` & `angr-9.2.97/angr/analyses/boyscout.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/callee_cleanup_finder.py` & `angr-9.2.97/angr/analyses/callee_cleanup_finder.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/calling_convention.py` & `angr-9.2.97/angr/analyses/calling_convention.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cdg.py` & `angr-9.2.97/angr/analyses/cdg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg/cfb.py` & `angr-9.2.97/angr/analyses/cfg/cfb.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg/cfg.py` & `angr-9.2.97/angr/analyses/cfg/cfg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg/cfg_arch_options.py` & `angr-9.2.97/angr/analyses/cfg/cfg_arch_options.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg/cfg_base.py` & `angr-9.2.97/angr/analyses/cfg/cfg_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg/cfg_emulated.py` & `angr-9.2.97/angr/analyses/cfg/cfg_emulated.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg/cfg_fast.py` & `angr-9.2.97/angr/analyses/cfg/cfg_fast.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg/cfg_fast_soot.py` & `angr-9.2.97/angr/analyses/cfg/cfg_fast_soot.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg/cfg_job_base.py` & `angr-9.2.97/angr/analyses/cfg/cfg_job_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/amd64_elf_got.py` & `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/amd64_elf_got.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/amd64_pe_iat.py` & `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/amd64_pe_iat.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/arm_elf_fast.py` & `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/arm_elf_fast.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/const_resolver.py` & `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/const_resolver.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/default_resolvers.py` & `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/default_resolvers.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/jumptable.py` & `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/jumptable.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/mips_elf_fast.py` & `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/mips_elf_fast.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/propagator_utils.py` & `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/propagator_utils.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/resolver.py` & `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/resolver.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/x86_elf_pic_plt.py` & `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/x86_elf_pic_plt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg/indirect_jump_resolvers/x86_pe_iat.py` & `angr-9.2.97/angr/analyses/cfg/indirect_jump_resolvers/x86_pe_iat.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg_slice_to_sink/cfg_slice_to_sink.py` & `angr-9.2.97/angr/analyses/cfg_slice_to_sink/cfg_slice_to_sink.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg_slice_to_sink/graph.py` & `angr-9.2.97/angr/analyses/cfg_slice_to_sink/graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/cfg_slice_to_sink/transitions.py` & `angr-9.2.97/angr/analyses/cfg_slice_to_sink/transitions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/class_identifier.py` & `angr-9.2.97/angr/analyses/class_identifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/code_tagging.py` & `angr-9.2.97/angr/analyses/code_tagging.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/complete_calling_conventions.py` & `angr-9.2.97/angr/analyses/complete_calling_conventions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+# pylint:disable=import-outside-toplevel
 from typing import Tuple, Optional, Callable, Iterable, Dict, Set, TYPE_CHECKING
 import queue
 import threading
 import time
 import logging
 from collections import defaultdict
 
 import networkx
 
 import claripy
 
 from angr.utils.graph import GraphUtils
+from angr.simos import SimWindows
 from ..utils.mp import mp_context, Initializer
 from ..knowledge_plugins.cfg import CFGModel
 from . import Analysis, register_analysis, VariableRecoveryFast, CallingConventionAnalysis
 
 if TYPE_CHECKING:
     from angr.calling_conventions import SimCC
     from angr.sim_type import SimTypeFunction
@@ -84,19 +86,21 @@
         self._func_graphs = {} if not func_graphs else func_graphs
         self.prototype_libnames: Set[str] = set()
 
         self._func_addrs = []  # a list that holds addresses of all functions to be analyzed
         self._results = []
         if workers > 0:
             self._remaining_funcs = _mp_context.Value("i", 0)
-            self._func_queue = _mp_context.Queue()
             self._results = _mp_context.Queue()
+            self._results_lock = _mp_context.Lock()
+            self._func_queue = _mp_context.Queue()
             self._func_queue_lock = _mp_context.Lock()
         else:
             self._remaining_funcs = None  # not needed
+            self._results_lock = None  # not needed
             self._func_queue = None  # not needed
             self._func_queue_lock = threading.Lock()
 
         self._analyze()
         if self._auto_start:
             self.work()
 
@@ -201,41 +205,51 @@
                 depends_on[func_addr] = set()
                 for callee in self.kb.functions.callgraph.successors(func_addr):
                     if callee not in traversed_func_addrs and callee in func_addrs_set:
                         depends_on[func_addr].add(callee)
                         dependents[callee].add(func_addr)
 
             # enqueue all leaf functions
-            for func_addr in list(
-                k for k in depends_on if not depends_on[k]
-            ):  # pylint:disable=consider-using-dict-items
+            for func_addr in [k for k in depends_on if not depends_on[k]]:  # pylint:disable=consider-using-dict-items
                 self._func_queue.put((func_addr, None))
                 del depends_on[func_addr]
 
             self._update_progress(0, text="Spawning workers...")
             cc_callback = self._cc_callback
             self._cc_callback = None
 
+            if self.project.simos is not None and isinstance(self.project.simos, SimWindows):
+                # delayed import
+                from angr.procedures.definitions import load_win32api_definitions
+
+                Initializer.get().register(load_win32api_definitions)
+
             # spawn workers to perform the analysis
             with self._func_queue_lock:
                 procs = [
-                    _mp_context.Process(target=self._worker_routine, args=(Initializer.get(),), daemon=True)
-                    for _ in range(self._workers)
+                    _mp_context.Process(target=self._worker_routine, args=(worker_id, Initializer.get()), daemon=True)
+                    for worker_id in range(self._workers)
                 ]
                 for proc_idx, proc in enumerate(procs):
                     self._update_progress(0, text=f"Spawning worker {proc_idx}...")
                     proc.start()
 
             self._cc_callback = cc_callback
 
             # update progress
             self._update_progress(0)
             idx = 0
             while idx < total_funcs:
-                func_addr, cc, proto, proto_libname, varman = self._results.get(True)
+                try:
+                    with self._results_lock:
+                        func_addr, cc, proto, proto_libname, varman = self._results.get(True, timeout=0.01)
+                except queue.Empty:
+                    time.sleep(0.1)
+                    continue
+
                 func = self.kb.functions.get_by_addr(func_addr)
                 if cc is not None or proto is not None:
                     func.calling_convention = cc
                     self._set_function_prototype(func, proto, proto_libname)
                     if proto_libname is not None:
                         self.prototype_libnames.add(proto_libname)
 
@@ -256,21 +270,22 @@
 
                 # enqueue functions whose callees have been analyzed
                 if func_addr in dependents:
                     for dependent in dependents[func_addr]:
                         depends_on[dependent].discard(func_addr)
                         if not depends_on[dependent]:
                             callee_prototypes = self._get_callees_cc_prototypes(dependent)
-                            self._func_queue.put((dependent, callee_prototypes))
+                            with self._func_queue_lock:
+                                self._func_queue.put((dependent, callee_prototypes))
                             del depends_on[dependent]
 
             for proc in procs:
                 proc.join()
 
-    def _worker_routine(self, initializer: Initializer):
+    def _worker_routine(self, worker_id: int, initializer: Initializer):
         initializer.initialize()
         idx = 0
         while self._remaining_funcs.value > 0:
             try:
                 with self._func_queue_lock:
                     func_addr, callee_info = self._func_queue.get(True, timeout=0.01)
                     self._remaining_funcs.value -= 1
@@ -289,17 +304,18 @@
             if self._low_priority:
                 if idx % 3 == 0:
                     time.sleep(0.1)
 
             try:
                 cc, proto, proto_libname, varman = self._analyze_core(func_addr)
             except Exception:  # pylint:disable=broad-except
-                _l.error("Exception occurred during _analyze_core().", exc_info=True)
+                _l.error("Worker %d: Exception occurred during _analyze_core().", worker_id, exc_info=True)
                 cc, proto, proto_libname, varman = None, None, None, None
-            self._results.put((func_addr, cc, proto, proto_libname, varman))
+            with self._results_lock:
+                self._results.put((func_addr, cc, proto, proto_libname, varman))
 
     def _analyze_core(
         self, func_addr: int
     ) -> Tuple[Optional["SimCC"], Optional["SimTypeFunction"], Optional["str"], Optional["VariableManagerInternal"]]:
         func = self.kb.functions.get_by_addr(func_addr)
         if func.ran_cca:
             return (
```

### Comparing `angr-9.2.96/angr/analyses/congruency_check.py` & `angr-9.2.97/angr/analyses/congruency_check.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/data_dep/data_dependency_analysis.py` & `angr-9.2.97/angr/analyses/data_dep/data_dependency_analysis.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/data_dep/dep_nodes.py` & `angr-9.2.97/angr/analyses/data_dep/dep_nodes.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/data_dep/sim_act_location.py` & `angr-9.2.97/angr/analyses/data_dep/sim_act_location.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/datagraph_meta.py` & `angr-9.2.97/angr/analyses/datagraph_meta.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/ddg.py` & `angr-9.2.97/angr/analyses/ddg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/__init__.py` & `angr-9.2.97/angr/analyses/decompiler/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/ail_simplifier.py` & `angr-9.2.97/angr/analyses/decompiler/ail_simplifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint:disable=too-many-boolean-expressions
 from typing import Set, Dict, List, Tuple, Any, Optional, TYPE_CHECKING
 from collections import defaultdict
 import logging
 
 from ailment import AILBlockWalker
 from ailment.block import Block
 from ailment.statement import Statement, Assignment, Store, Call, ConditionalJump, DirtyStatement
@@ -179,14 +180,15 @@
         rd = self.project.analyses.ReachingDefinitions(
             subject=self.func,
             func_graph=self.func_graph,
             # init_context=(),    <-- in case of fire break glass
             observe_all=False,
             use_callee_saved_regs_at_return=self._use_callee_saved_regs_at_return,
             track_tmps=True,
+            element_limit=1,
         ).model
         self._reaching_definitions = rd
         return rd
 
     def _compute_propagation(self, immediate_stmt_removal: bool = False):
         # Propagate expressions or return the existing result
         if self._propagator is not None:
@@ -500,15 +502,17 @@
         if not walker.operations:
             if expr is None:
                 return None, None
             return expr.size, ("expr", (expr,))
 
         first_op = walker.operations[0]
         if isinstance(first_op, Convert):
-            return first_op.to_bits // self.project.arch.byte_width, ("convert", (first_op,))
+            if first_op.to_bits >= self.project.arch.byte_width:
+                # we need at least one byte!
+                return first_op.to_bits // self.project.arch.byte_width, ("convert", (first_op,))
         if isinstance(first_op, BinaryOp):
             second_op = None
             if len(walker.operations) >= 2:
                 second_op = walker.operations[1]
             if (
                 first_op.op == "And"
                 and isinstance(first_op.operands[1], Const)
@@ -522,14 +526,15 @@
                 if mask == 0xFFFF_FFFF:
                     return 4, ("mask", (first_op, second_op)) if second_op is not None else ("mask", (first_op,))
             if (
                 (first_op.operands[0] is expr or first_op.operands[1] is expr)
                 and first_op.op not in {"Shr", "Sar"}
                 and isinstance(second_op, Convert)
                 and second_op.from_bits == expr.bits
+                and second_op.to_bits >= self.project.arch.byte_width  # we need at least one byte!
             ):
                 return min(expr.bits, second_op.to_bits) // self.project.arch.byte_width, (
                     "binop-convert",
                     (expr, first_op, second_op),
                 )
 
         if expr is None:
@@ -717,21 +722,21 @@
                             if any(
                                 (def_ != arg_copy_def and def_.atom == arg_copy_def.atom)
                                 for def_ in rd.all_definitions
                                 if isinstance(def_.atom, atoms.MemoryLocation)
                             ):
                                 continue
 
-                            # Make sure the register is never updated across this function
-                            if any(
-                                (def_ != the_def and def_.atom == the_def.atom)
-                                for def_ in rd.all_definitions
-                                if isinstance(def_.atom, atoms.Register) and rd.all_uses.get_uses(def_)
-                            ):
-                                continue
+                        # Make sure the register is never updated across this function
+                        if any(
+                            (def_ != the_def and def_.atom == the_def.atom)
+                            for def_ in rd.all_definitions
+                            if isinstance(def_.atom, atoms.Register) and rd.all_uses.get_uses(def_)
+                        ):
+                            continue
 
                         # find all its uses
                         all_arg_copy_var_uses: Set[Tuple[CodeLocation, Any]] = set(
                             rd.all_uses.get_uses_with_expr(arg_copy_def)
                         )
                         all_uses_with_def = set()
 
@@ -1210,14 +1215,21 @@
                     if stackarg_offsets is not None and isinstance(def_.atom.addr, atoms.SpOffset):
                         if (def_.atom.addr.offset & mask) not in stackarg_offsets:
                             continue
                     else:
                         continue
 
             uses = rd.all_uses.get_uses(def_)
+            if (
+                isinstance(def_.atom, atoms.Register)
+                and def_.atom.reg_offset in self.project.arch.artificial_registers_offsets
+            ):
+                if len(uses) == 1 and next(iter(uses)) == def_.codeloc:
+                    # cc_ndep = amd64g_calculate_condition(..., cc_ndep)
+                    uses = set()
 
             if not uses:
                 if not isinstance(def_.codeloc, ExternalCodeLocation):
                     stmts_to_remove_per_block[(def_.codeloc.block_addr, def_.codeloc.block_idx)].add(
                         def_.codeloc.stmt_idx
                     )
```

### Comparing `angr-9.2.96/angr/analyses/decompiler/ailgraph_walker.py` & `angr-9.2.97/angr/analyses/decompiler/ailgraph_walker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/block_io_finder.py` & `angr-9.2.97/angr/analyses/decompiler/block_io_finder.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/block_similarity.py` & `angr-9.2.97/angr/analyses/decompiler/block_similarity.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/block_simplifier.py` & `angr-9.2.97/angr/analyses/decompiler/block_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/call_counter.py` & `angr-9.2.97/angr/analyses/decompiler/call_counter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/callsite_maker.py` & `angr-9.2.97/angr/analyses/decompiler/callsite_maker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/ccall_rewriters/amd64_ccalls.py` & `angr-9.2.97/angr/analyses/decompiler/ccall_rewriters/amd64_ccalls.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/clinic.py` & `angr-9.2.97/angr/analyses/decompiler/clinic.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/condition_processor.py` & `angr-9.2.97/angr/analyses/decompiler/condition_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -762,14 +762,16 @@
             self._condition_mapping[var.args[0]] = condition
             return var
         elif isinstance(condition, ailment.Expr.Const):
             if condition.value is True or condition.value is False:
                 var = claripy.BoolV(condition.value)
             else:
                 var = claripy.BVV(condition.value, condition.bits)
+            if isinstance(var, claripy.Bits) and var.size() == 1:
+                var = claripy.true if var.concrete_value == 1 else claripy.false
             return var
         elif isinstance(condition, ailment.Expr.Tmp):
             l.warning("Left-over ailment.Tmp variable %s.", condition)
             if condition.bits == 1:
                 var = claripy.BoolS("ailtmp_%d" % condition.tmp_idx, explicit_name=True)
             else:
                 var = claripy.BVS("ailtmp_%d" % condition.tmp_idx, condition.bits, explicit_name=True)
```

### Comparing `angr-9.2.96/angr/analyses/decompiler/decompilation_cache.py` & `angr-9.2.97/angr/analyses/decompiler/decompilation_cache.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/decompilation_options.py` & `angr-9.2.97/angr/analyses/decompiler/decompilation_options.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/decompiler.py` & `angr-9.2.97/angr/analyses/decompiler/decompiler.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/empty_node_remover.py` & `angr-9.2.97/angr/analyses/decompiler/empty_node_remover.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/expression_counters.py` & `angr-9.2.97/angr/analyses/decompiler/expression_counters.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/expression_narrower.py` & `angr-9.2.97/angr/analyses/decompiler/expression_narrower.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/goto_manager.py` & `angr-9.2.97/angr/analyses/decompiler/goto_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/graph_region.py` & `angr-9.2.97/angr/analyses/decompiler/graph_region.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/jump_target_collector.py` & `angr-9.2.97/angr/analyses/decompiler/jump_target_collector.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/jumptable_entry_condition_rewriter.py` & `angr-9.2.97/angr/analyses/decompiler/jumptable_entry_condition_rewriter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/__init__.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/base_ptr_save_simplifier.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/base_ptr_save_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/code_motion.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/code_motion.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/const_derefs.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/const_derefs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/cross_jump_reverter.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/cross_jump_reverter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/div_simplifier.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/div_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/engine_base.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/engine_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/expr_op_swapper.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/expr_op_swapper.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/flip_boolean_cmp.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/flip_boolean_cmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/ite_expr_converter.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/ite_expr_converter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/ite_region_converter.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/ite_region_converter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/lowered_switch_simplifier.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/lowered_switch_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/mod_simplifier.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/mod_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/multi_simplifier.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/multi_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/optimization_pass.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/optimization_pass.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/register_save_area_simplifier.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/register_save_area_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/ret_addr_save_simplifier.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/ret_addr_save_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/ret_deduplicator.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/ret_deduplicator.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/return_duplicator_base.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/return_duplicator_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/return_duplicator_high.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/return_duplicator_high.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/return_duplicator_low.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/return_duplicator_low.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/stack_canary_simplifier.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/stack_canary_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/switch_default_case_duplicator.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/switch_default_case_duplicator.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/win_stack_canary_simplifier.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/win_stack_canary_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/optimization_passes/x86_gcc_getpc_simplifier.py` & `angr-9.2.97/angr/analyses/decompiler/optimization_passes/x86_gcc_getpc_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/__init__.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/a_div_const_add_a_mul_n_div_const.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_div_const_add_a_mul_n_div_const.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/a_mul_const_div_shr_const.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_mul_const_div_shr_const.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/a_shl_const_sub_a.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_shl_const_sub_a.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div_const_mul_const.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_sub_a_div_const_mul_const.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/a_sub_a_sub_n.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/a_sub_a_sub_n.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/arm_cmpf.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/arm_cmpf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/base.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_add_n.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_add_n.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_and_mask.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/basepointeroffset_and_mask.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/bitwise_or_to_logical_or.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/bitwise_or_to_logical_or.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/bool_expr_xor_1.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/bool_expr_xor_1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/bswap.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/bswap.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/coalesce_same_cascading_ifs.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/coalesce_same_cascading_ifs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/const_mull_a_shift.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/const_mull_a_shift.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/constant_derefs.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/constant_derefs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/conv_a_sub0_shr_and.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/conv_a_sub0_shr_and.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/conv_shl_shr.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/conv_shl_shr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/eager_eval.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/eager_eval.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/extended_byte_and_mask.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/extended_byte_and_mask.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/inlined_strcpy.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/inlined_strcpy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/inlined_strcpy_consolidation.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/inlined_strcpy_consolidation.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/invert_negated_logical_conjuction_disjunction.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/invert_negated_logical_conjuction_disjunction.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/one_sub_bool.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/one_sub_bool.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/remove_cascading_conversions.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_cascading_conversions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/remove_empty_if_body.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_empty_if_body.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/remove_noop_conversions.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_noop_conversions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/remove_redundant_bitmasks.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_bitmasks.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/remove_redundant_conversions.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_conversions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/remove_redundant_ite_branch.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_ite_branch.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/remove_redundant_ite_comparisons.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_ite_comparisons.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/remove_redundant_reinterprets.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_reinterprets.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/remove_redundant_shifts.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_shifts.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/remove_redundant_shifts_around_comparators.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/remove_redundant_shifts_around_comparators.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/rewrite_bit_extractions.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/rewrite_bit_extractions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/rewrite_mips_gp_loads.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/rewrite_mips_gp_loads.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/rol_ror.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/rol_ror.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/sar_to_signed_div.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/sar_to_signed_div.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/simplify_pc_relative_loads.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/simplify_pc_relative_loads.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/single_bit_cond_to_boolexpr.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/single_bit_cond_to_boolexpr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/single_bit_xor.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/single_bit_xor.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/peephole_optimizations/tidy_stack_addr.py` & `angr-9.2.97/angr/analyses/decompiler/peephole_optimizations/tidy_stack_addr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/redundant_label_remover.py` & `angr-9.2.97/angr/analyses/decompiler/redundant_label_remover.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/region_identifier.py` & `angr-9.2.97/angr/analyses/decompiler/region_identifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/region_simplifiers/cascading_cond_transformer.py` & `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/cascading_cond_transformer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/region_simplifiers/cascading_ifs.py` & `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/cascading_ifs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/region_simplifiers/expr_folding.py` & `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/expr_folding.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/region_simplifiers/goto.py` & `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/goto.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/region_simplifiers/if_.py` & `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/if_.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/region_simplifiers/ifelse.py` & `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/ifelse.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/region_simplifiers/loop.py` & `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/loop.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/region_simplifiers/node_address_finder.py` & `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/node_address_finder.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/region_simplifiers/region_simplifier.py` & `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/region_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/region_simplifiers/switch_cluster_simplifier.py` & `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/switch_cluster_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/region_simplifiers/switch_expr_simplifier.py` & `angr-9.2.97/angr/analyses/decompiler/region_simplifiers/switch_expr_simplifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/region_walker.py` & `angr-9.2.97/angr/analyses/decompiler/region_walker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/seq_to_blocks.py` & `angr-9.2.97/angr/analyses/decompiler/seq_to_blocks.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/sequence_walker.py` & `angr-9.2.97/angr/analyses/decompiler/sequence_walker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/structured_codegen/base.py` & `angr-9.2.97/angr/analyses/decompiler/structured_codegen/base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/structured_codegen/c.py` & `angr-9.2.97/angr/analyses/decompiler/structured_codegen/c.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/structured_codegen/dummy.py` & `angr-9.2.97/angr/analyses/decompiler/structured_codegen/dummy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/structured_codegen/dwarf_import.py` & `angr-9.2.97/angr/analyses/decompiler/structured_codegen/dwarf_import.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/structuring/dream.py` & `angr-9.2.97/angr/analyses/decompiler/structuring/dream.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/structuring/phoenix.py` & `angr-9.2.97/angr/analyses/decompiler/structuring/phoenix.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/structuring/recursive_structurer.py` & `angr-9.2.97/angr/analyses/decompiler/structuring/recursive_structurer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/structuring/structurer_base.py` & `angr-9.2.97/angr/analyses/decompiler/structuring/structurer_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/structuring/structurer_nodes.py` & `angr-9.2.97/angr/analyses/decompiler/structuring/structurer_nodes.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/decompiler/utils.py` & `angr-9.2.97/angr/analyses/decompiler/utils.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/disassembly.py` & `angr-9.2.97/angr/analyses/disassembly.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/disassembly_utils.py` & `angr-9.2.97/angr/analyses/disassembly_utils.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/dominance_frontier.py` & `angr-9.2.97/angr/analyses/dominance_frontier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/find_objects_static.py` & `angr-9.2.97/angr/analyses/find_objects_static.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,15 @@
      address outside the mapped binary to the newly created space(possible object).
 
      It also tracks if the function called right after new() is passed the same 'this' pointer and is a constructor,
      if so we mark it as an instance of the class the constructor belongs to.(only for non stripped binaries)
     """
 
     def __init__(self, max_addr=None, new_func_addr=None, project=None):
+        super().__init__()
         self.max_addr = max_addr
 
         # this is a map between an object addr outside the mapped binary and PossibleObject instance
         self.possible_objects_dict = {}
 
         # address of the new() function
         self.new_func_addr = new_func_addr
@@ -100,24 +101,28 @@
             offset_to_values = {}
 
             for offset in range(0, size, word_size):
                 offset_to_values[offset] = {claripy.BVV(0, word_size * state.arch.byte_width)}
             data.depends(memory_location, value=MultiValues(offset_to_values=offset_to_values))
             self.max_addr += size
 
-        elif "ctor" in self.project.kb.functions[function_address].demangled_name:
-            # check if rdi has a possible this pointer/ object address, if so then we can assign this object this class
-            # also if the func is a constructor(not stripped binaries)
-            for addr, possible_object in self.possible_objects_dict.items():
-                v1 = state.registers.load(72, state.arch.bits // state.arch.byte_width).one_value()
-                obj_addr = v1.concrete_value if v1 is not None and v1.concrete else None
-                if obj_addr is not None and addr == obj_addr:
-                    col_ind = self.project.kb.functions[function_address].demangled_name.rfind("::")
-                    class_name = self.project.kb.functions[function_address].demangled_name[:col_ind]
-                    possible_object.class_name = class_name
+        else:
+            if self.project.kb.functions.contains_addr(function_address):
+                func = self.project.kb.functions.get_by_addr(function_address)
+                if func is not None and "ctor" in func.demangled_name:
+                    # check if rdi has a possible this pointer/ object address, if so then we can assign this object
+                    # this class
+                    # also if the func is a constructor(not stripped binaries)
+                    for addr, possible_object in self.possible_objects_dict.items():
+                        v1 = state.registers.load(72, state.arch.bits // state.arch.byte_width).one_value()
+                        obj_addr = v1.concrete_value if v1 is not None and v1.concrete else None
+                        if obj_addr is not None and addr == obj_addr:
+                            col_ind = self.project.kb.functions[function_address].demangled_name.rfind("::")
+                            class_name = self.project.kb.functions[function_address].demangled_name[:col_ind]
+                            possible_object.class_name = class_name
 
 
 class StaticObjectFinder(Analysis):
     """
     This analysis tries to find objects on the heap based on calls to new(), and subsequent calls to constructors with
      the 'this' pointer
     """
```

### Comparing `angr-9.2.96/angr/analyses/flirt.py` & `angr-9.2.97/angr/analyses/flirt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/forward_analysis/forward_analysis.py` & `angr-9.2.97/angr/analyses/forward_analysis/forward_analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -205,14 +205,28 @@
         :param states: Abstract states to merge.
         :return:       A merged abstract state, and a boolean variable indicating if a local fixed-point has reached (
                        i.e., union(state0, state1) == state0), in which case, its successors will not be revisited.
         """
 
         raise NotImplementedError("_merge_states() is not implemented.")
 
+    def _compare_states(self, node: NodeType, old_state: AnalysisState, new_state: AnalysisState) -> bool:
+        """
+        Determine if the analysis has reached fixed point at `node`.
+
+        You can override this method to implement a faster _compare_states() method.
+
+        :param node:        The node that has been analyzed.
+        :param old_state:   The original output state out of node.
+        :param new_state:   The new output state out of node.
+        :return:            True if the analysis has reached fixed at node. False otherwise.
+        """
+        _, has_no_changes = self._merge_states(node, old_state, new_state)
+        return has_no_changes
+
     def _widen_states(self, *states: AnalysisState) -> AnalysisState:
         raise NotImplementedError("_widen_states() is not implemented.")
 
     # Special interfaces for non-graph-traversal mode
 
     def _merge_jobs(self, *jobs: JobType):
         raise NotImplementedError("_merge_jobs() is not implemented.")
@@ -284,15 +298,15 @@
                 # the change of states are determined during state merging (_add_input_state()) instead of during
                 # simulated execution (_run_on_node()).
 
                 if self._node_key(n) not in self._output_state:
                     reached_fixedpoint = False
                 else:
                     # is the output state the same as the old one?
-                    _, reached_fixedpoint = self._merge_states(n, self._output_state[self._node_key(n)], output_state)
+                    reached_fixedpoint = self._compare_states(n, self._output_state[self._node_key(n)], output_state)
                 self._output_state[self._node_key(n)] = output_state
 
                 if not reached_fixedpoint:
                     successors_to_visit = self._add_input_state(n, output_state)
                     # revisit all successors in the `successors_to_visit` list
                     for succ in successors_to_visit:
                         self._graph_visitor.revisit_node(succ)
```

### Comparing `angr-9.2.96/angr/analyses/forward_analysis/job_info.py` & `angr-9.2.97/angr/analyses/forward_analysis/job_info.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/forward_analysis/visitors/call_graph.py` & `angr-9.2.97/angr/analyses/forward_analysis/visitors/call_graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/forward_analysis/visitors/function_graph.py` & `angr-9.2.97/angr/analyses/forward_analysis/visitors/function_graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/forward_analysis/visitors/graph.py` & `angr-9.2.97/angr/analyses/forward_analysis/visitors/graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/forward_analysis/visitors/loop.py` & `angr-9.2.97/angr/analyses/forward_analysis/visitors/loop.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/forward_analysis/visitors/single_node_graph.py` & `angr-9.2.97/angr/analyses/forward_analysis/visitors/single_node_graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/custom_callable.py` & `angr-9.2.97/angr/analyses/identifier/custom_callable.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/func.py` & `angr-9.2.97/angr/analyses/identifier/func.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/__init__.py` & `angr-9.2.97/angr/analyses/identifier/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/atoi.py` & `angr-9.2.97/angr/analyses/identifier/functions/atoi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/based_atoi.py` & `angr-9.2.97/angr/analyses/identifier/functions/based_atoi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/fdprintf.py` & `angr-9.2.97/angr/analyses/identifier/functions/fdprintf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/free.py` & `angr-9.2.97/angr/analyses/identifier/functions/free.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/int2str.py` & `angr-9.2.97/angr/analyses/identifier/functions/int2str.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/malloc.py` & `angr-9.2.97/angr/analyses/identifier/functions/malloc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/memcmp.py` & `angr-9.2.97/angr/analyses/identifier/functions/memcmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/memcpy.py` & `angr-9.2.97/angr/analyses/identifier/functions/memcpy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/memset.py` & `angr-9.2.97/angr/analyses/identifier/functions/memset.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/printf.py` & `angr-9.2.97/angr/analyses/identifier/functions/printf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/recv_until.py` & `angr-9.2.97/angr/analyses/identifier/functions/recv_until.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/skip_calloc.py` & `angr-9.2.97/angr/analyses/identifier/functions/skip_calloc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/skip_realloc.py` & `angr-9.2.97/angr/analyses/identifier/functions/skip_realloc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/skip_recv_n.py` & `angr-9.2.97/angr/analyses/identifier/functions/skip_recv_n.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/snprintf.py` & `angr-9.2.97/angr/analyses/identifier/functions/snprintf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/sprintf.py` & `angr-9.2.97/angr/analyses/identifier/functions/sprintf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/strcasecmp.py` & `angr-9.2.97/angr/analyses/identifier/functions/strcasecmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/strcmp.py` & `angr-9.2.97/angr/analyses/identifier/functions/strcmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/strcpy.py` & `angr-9.2.97/angr/analyses/identifier/functions/strcpy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/strlen.py` & `angr-9.2.97/angr/analyses/identifier/functions/strlen.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/strncmp.py` & `angr-9.2.97/angr/analyses/identifier/functions/strncmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/strncpy.py` & `angr-9.2.97/angr/analyses/identifier/functions/strncpy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/functions/strtol.py` & `angr-9.2.97/angr/analyses/identifier/functions/strtol.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/identify.py` & `angr-9.2.97/angr/analyses/identifier/identify.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/identifier/runner.py` & `angr-9.2.97/angr/analyses/identifier/runner.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/init_finder.py` & `angr-9.2.97/angr/analyses/init_finder.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/loop_analysis.py` & `angr-9.2.97/angr/analyses/loop_analysis.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/loopfinder.py` & `angr-9.2.97/angr/analyses/loopfinder.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/propagator/engine_ail.py` & `angr-9.2.97/angr/analyses/propagator/engine_ail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1217,14 +1217,16 @@
                     o0_expr if o0_expr is not None else expr.operands[0],
                     o1_expr if o1_expr is not None else expr.operands[1],
                 ],
                 expr.signed,
                 bits=expr.bits,
                 floating_point=expr.floating_point,
                 rounding_mode=expr.rounding_mode,
+                from_bits=expr.from_bits,
+                to_bits=expr.to_bits,
                 **expr.tags,
             )
         return PropValue.from_value_and_details(value, expr.size, new_expr, self._codeloc())
 
     def _ail_handle_Mod(self, expr):
         o0_value = self._expr(expr.operands[0])
         o1_value = self._expr(expr.operands[1])
```

### Comparing `angr-9.2.96/angr/analyses/propagator/engine_base.py` & `angr-9.2.97/angr/analyses/propagator/engine_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/propagator/engine_vex.py` & `angr-9.2.97/angr/analyses/propagator/engine_vex.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/propagator/outdated_definition_walker.py` & `angr-9.2.97/angr/analyses/propagator/outdated_definition_walker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/propagator/propagator.py` & `angr-9.2.97/angr/analyses/propagator/propagator.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     def __init__(
         self,
         func=None,
         block=None,
         func_graph=None,
         base_state=None,
-        max_iterations=3,
+        max_iterations=30,
         load_callback=None,
         stack_pointer_tracker=None,
         only_consts=False,
         completed_funcs=None,
         do_binops=True,
         store_tops=True,
         vex_cross_insn_opt=False,
@@ -75,15 +75,18 @@
         elif block is not None:
             # traversing a block (but func might be specified at the same time to provide extra information, e.g., the
             # value for register t9 for MIPS32/64 binaries)
             self.flavor = "block"
         else:
             raise ValueError("Unsupported analysis target.")
 
-        start = time.perf_counter_ns() / 1000000
+        if profiling:
+            start = time.perf_counter_ns() / 1000000
+        else:
+            start = 0
 
         self._base_state = base_state
         self._function = func
         self._func_addr = func_addr if func_addr is not None else (None if func is None else func.addr)
         self._block = block
         self._block_addr = block.addr if block is not None else None
         self._max_iterations = max_iterations
@@ -316,15 +319,15 @@
             PropagatorState.merge_replacements(self.model.replacements, state._replacements)
 
         self.model.equivalence |= state._equivalence
 
         # TODO: Clear registers according to calling conventions
 
         if self.model.node_iterations[block_key] < self._max_iterations:
-            return True, state
+            return None, state
         else:
             return False, state
 
     def _process_input_state_for_successor(
         self, node, successor, input_state: Union[PropagatorAILState, PropagatorVEXState]
     ):
         if self._only_consts:
```

### Comparing `angr-9.2.96/angr/analyses/propagator/values.py` & `angr-9.2.97/angr/analyses/propagator/values.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/propagator/vex_vars.py` & `angr-9.2.97/angr/analyses/propagator/vex_vars.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/proximity_graph.py` & `angr-9.2.97/angr/analyses/proximity_graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/reaching_definitions/__init__.py` & `angr-9.2.97/angr/analyses/reaching_definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/reaching_definitions/call_trace.py` & `angr-9.2.97/angr/analyses/reaching_definitions/call_trace.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/reaching_definitions/dep_graph.py` & `angr-9.2.97/angr/analyses/reaching_definitions/dep_graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/reaching_definitions/engine_ail.py` & `angr-9.2.97/angr/analyses/reaching_definitions/engine_ail.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/reaching_definitions/engine_vex.py` & `angr-9.2.97/angr/analyses/reaching_definitions/engine_vex.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/reaching_definitions/function_handler.py` & `angr-9.2.97/angr/analyses/reaching_definitions/function_handler.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/reaching_definitions/heap_allocator.py` & `angr-9.2.97/angr/analyses/reaching_definitions/heap_allocator.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/reaching_definitions/rd_initializer.py` & `angr-9.2.97/angr/analyses/reaching_definitions/rd_initializer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/reaching_definitions/rd_state.py` & `angr-9.2.97/angr/analyses/reaching_definitions/rd_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
         "all_definitions",
         "_canonical_size",
         "heap_allocator",
         "_environment",
         "_track_consts",
         "_sp_adjusted",
         "exit_observed",
+        "_element_limit",
     )
 
     def __init__(
         self,
         codeloc: CodeLocation,
         arch: archinfo.Arch,
         subject: Subject,
@@ -86,24 +87,26 @@
         live_definitions: Optional[LiveDefinitions] = None,
         canonical_size: int = 8,
         heap_allocator: HeapAllocator = None,
         environment: Environment = None,
         sp_adjusted: bool = False,
         all_definitions: Optional[Set[Definition]] = None,
         initializer: Optional["RDAStateInitializer"] = None,
+        element_limit: int = 5,
     ):
         # handy short-hands
         self.codeloc = codeloc
         self.arch: archinfo.Arch = arch
         self._subject = subject
         self._track_tmps = track_tmps
         self._track_consts = track_consts
         self.analysis = analysis
         self._canonical_size: int = canonical_size
         self._sp_adjusted: bool = sp_adjusted
+        self._element_limit: int = element_limit
 
         self.all_definitions: Set[Definition] = set() if all_definitions is None else all_definitions
 
         self.heap_allocator = heap_allocator or HeapAllocator(canonical_size)
         self._environment: Environment = environment or Environment()
 
         self.codeloc_uses: Set[Definition] = set()
@@ -118,15 +121,18 @@
         # This must stay at the end of the __init__ method, because the _set_initialization_values method will call
         # the state initializer which might need to access some of the above attributes, e.g. the heap_allocator
         # to do its job
 
         if live_definitions is None:
             # the first time this state is created. initialize it
             self.live_definitions = LiveDefinitions(
-                self.arch, track_tmps=self._track_tmps, canonical_size=canonical_size
+                self.arch,
+                track_tmps=self._track_tmps,
+                canonical_size=canonical_size,
+                element_limit=element_limit,
             )
             if self.analysis is not None:
                 self.live_definitions.project = self.analysis.project
             self._set_initialization_values(
                 subject, rtoc_value, initializer=initializer, project=self.live_definitions.project
             )
         else:
@@ -306,27 +312,34 @@
             analysis=self.analysis,
             live_definitions=self.live_definitions.copy(discard_tmpdefs=discard_tmpdefs),
             canonical_size=self._canonical_size,
             heap_allocator=self.heap_allocator,
             environment=self._environment,
             sp_adjusted=self._sp_adjusted,
             all_definitions=self.all_definitions.copy(),
+            element_limit=self._element_limit,
         )
 
         return rd
 
     def merge(self, *others) -> Tuple["ReachingDefinitionsState", bool]:
         state = self.copy()
         others: Iterable["ReachingDefinitionsState"]
 
         state.live_definitions, merged_0 = state.live_definitions.merge(*[other.live_definitions for other in others])
         state._environment, merged_1 = state.environment.merge(*[other.environment for other in others])
 
         return state, merged_0 or merged_1
 
+    def compare(self, other: "ReachingDefinitionsState") -> bool:
+        r0 = self.live_definitions.compare(other.live_definitions)
+        r1 = self.environment.compare(other.environment)
+
+        return r0 and r1
+
     def move_codelocs(self, new_codeloc: CodeLocation) -> None:
         if self.codeloc != new_codeloc:
             self.codeloc = new_codeloc
             self.codeloc_uses = set()
 
     def kill_definitions(self, atom: Atom) -> None:
         """
```

### Comparing `angr-9.2.96/angr/analyses/reaching_definitions/reaching_definitions.py` & `angr-9.2.97/angr/analyses/reaching_definitions/reaching_definitions.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     * Some more documentation and examples would be nice.
     """
 
     def __init__(
         self,
         subject: Union[Subject, ailment.Block, Block, Function, str] = None,
         func_graph=None,
-        max_iterations=3,
+        max_iterations=30,
         track_tmps=False,
         track_consts=True,
         observation_points: "Iterable[ObservationPoint]" = None,
         init_state: ReachingDefinitionsState = None,
         init_context=None,
         state_initializer: Optional["RDAStateInitializer"] = None,
         cc=None,
@@ -70,14 +70,15 @@
         observe_callback=None,
         canonical_size=8,
         stack_pointer_tracker=None,
         use_callee_saved_regs_at_return=True,
         interfunction_level: int = 0,
         track_liveness: bool = True,
         func_addr: Optional[int] = None,
+        element_limit: int = 5,
     ):
         """
         :param subject:                         The subject of the analysis: a function, or a single basic block
         :param func_graph:                      Alternative graph for function.graph.
         :param max_iterations:                  The maximum number of iterations before the analysis is terminated.
         :param track_tmps:                      Whether or not temporary variables should be taken into consideration
                                                 during the analysis.
@@ -127,14 +128,15 @@
         self._track_consts = track_consts
         self._max_iterations = max_iterations
         self._observation_points = observation_points
         self._init_state = init_state
         self._canonical_size = canonical_size
         self._use_callee_saved_regs_at_return = use_callee_saved_regs_at_return
         self._func_addr = func_addr
+        self._element_limit = element_limit
 
         if dep_graph is None or dep_graph is False:
             self._dep_graph = None
         elif dep_graph is True:
             self._dep_graph = DepGraph()
         else:
             self._dep_graph = dep_graph
@@ -465,21 +467,36 @@
                 self.project.arch,
                 self.subject,
                 track_tmps=self._track_tmps,
                 track_consts=self._track_consts,
                 analysis=self,
                 canonical_size=self._canonical_size,
                 initializer=self._state_initializer,
+                element_limit=self._element_limit,
             )
 
     # pylint: disable=no-self-use,arguments-differ
     def _merge_states(self, _node, *states: ReachingDefinitionsState):
+        assert len(states) >= 2
         merged_state, merge_occurred = states[0].merge(*states[1:])
         return merged_state, not merge_occurred
 
+    def _compare_states(self, node, old_state: ReachingDefinitionsState, new_state: ReachingDefinitionsState) -> bool:
+        """
+        Return True if new_state >= old_state in the lattice.
+
+        :param node:
+        :param old_state:
+        :param new_state:
+        :return:
+        """
+
+        reached_fixedpoint = new_state.compare(old_state)
+        return reached_fixedpoint
+
     def _run_on_node(self, node, state: ReachingDefinitionsState):
         """
 
         :param node:    The current node.
         :param state:   The analysis state.
         :return:        A tuple: (reached fix-point, successor state)
         """
@@ -546,15 +563,15 @@
                 for loc in locs:
                     self.all_uses.add_use(tmp_def, loc)
 
         # drop definitions and uses because we will not need them anymore
         state.downsize()
 
         if self._node_iterations[block_key] < self._max_iterations:
-            return True, state
+            return None, state
         else:
             return False, state
 
     def _intra_analysis(self):
         pass
 
     def _post_analysis(self):
```

### Comparing `angr-9.2.96/angr/analyses/reaching_definitions/subject.py` & `angr-9.2.97/angr/analyses/reaching_definitions/subject.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/reassembler.py` & `angr-9.2.97/angr/analyses/reassembler.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/soot_class_hierarchy.py` & `angr-9.2.97/angr/analyses/soot_class_hierarchy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/stack_pointer_tracker.py` & `angr-9.2.97/angr/analyses/stack_pointer_tracker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/static_hooker.py` & `angr-9.2.97/angr/analyses/static_hooker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/typehoon/dfa.py` & `angr-9.2.97/angr/analyses/typehoon/dfa.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/typehoon/lifter.py` & `angr-9.2.97/angr/analyses/typehoon/lifter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/typehoon/simple_solver.py` & `angr-9.2.97/angr/analyses/typehoon/simple_solver.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/typehoon/translator.py` & `angr-9.2.97/angr/analyses/typehoon/translator.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/typehoon/typeconsts.py` & `angr-9.2.97/angr/analyses/typehoon/typeconsts.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/typehoon/typehoon.py` & `angr-9.2.97/angr/analyses/typehoon/typehoon.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/typehoon/typevars.py` & `angr-9.2.97/angr/analyses/typehoon/typevars.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/variable_recovery/annotations.py` & `angr-9.2.97/angr/analyses/variable_recovery/annotations.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/variable_recovery/engine_ail.py` & `angr-9.2.97/angr/analyses/variable_recovery/engine_ail.py`

 * *Files 0% similar despite different names*

```diff
@@ -465,28 +465,28 @@
         )
 
     def _ail_handle_DivMod(self, expr: ailment.Expr.BinaryOp):
         arg0, arg1 = expr.operands
 
         r0 = self._expr(arg0)
         r1 = self._expr(arg1)
-        from_size = r1.bits
-        to_size = r0.bits
+        from_size = expr.from_bits
+        to_size = expr.to_bits
 
         if expr.signed:
-            quotient = r0.data.SDiv(claripy.SignExt(to_size - from_size, r1.data))
-            remainder = r0.data.SMod(claripy.SignExt(to_size - from_size, r1.data))
+            quotient = r0.data.SDiv(claripy.SignExt(from_size - to_size, r1.data))
+            remainder = r0.data.SMod(claripy.SignExt(from_size - to_size, r1.data))
             quotient_size = to_size
             remainder_size = to_size
             r = claripy.Concat(
                 claripy.Extract(remainder_size - 1, 0, remainder), claripy.Extract(quotient_size - 1, 0, quotient)
             )
         else:
-            quotient = r0.data // claripy.ZeroExt(to_size - from_size, r1.data)
-            remainder = r0.data % claripy.ZeroExt(to_size - from_size, r1.data)
+            quotient = r0.data // claripy.ZeroExt(from_size - to_size, r1.data)
+            remainder = r0.data % claripy.ZeroExt(from_size - to_size, r1.data)
             quotient_size = to_size
             remainder_size = to_size
             r = claripy.Concat(
                 claripy.Extract(remainder_size - 1, 0, remainder), claripy.Extract(quotient_size - 1, 0, quotient)
             )
 
         return RichR(
```

### Comparing `angr-9.2.96/angr/analyses/variable_recovery/engine_base.py` & `angr-9.2.97/angr/analyses/variable_recovery/engine_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/variable_recovery/engine_vex.py` & `angr-9.2.97/angr/analyses/variable_recovery/engine_vex.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/variable_recovery/irsb_scanner.py` & `angr-9.2.97/angr/analyses/variable_recovery/irsb_scanner.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/variable_recovery/variable_recovery.py` & `angr-9.2.97/angr/analyses/variable_recovery/variable_recovery.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/variable_recovery/variable_recovery_base.py` & `angr-9.2.97/angr/analyses/variable_recovery/variable_recovery_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,55 +171,58 @@
         if stack_region is not None:
             self.stack_region: MultiValuedMemory = stack_region
             self.stack_region._phi_maker = self._make_phi_variable
         else:
             self.stack_region: MultiValuedMemory = MultiValuedMemory(
                 memory_id="mem",
                 top_func=self.top,
+                is_top_func=self.is_top,
                 phi_maker=self._make_phi_variable,
                 skip_missing_values_during_merging=True,
                 page_kwargs={"mo_cmp": self._mo_cmp},
             )
         self.stack_region.set_state(self)
 
         if register_region is not None:
             self.register_region: MultiValuedMemory = register_region
             self.register_region._phi_maker = self._make_phi_variable
         else:
             self.register_region: MultiValuedMemory = MultiValuedMemory(
                 memory_id="reg",
                 top_func=self.top,
+                is_top_func=self.is_top,
                 phi_maker=self._make_phi_variable,
                 skip_missing_values_during_merging=True,
                 page_kwargs={"mo_cmp": self._mo_cmp},
             )
         self.register_region.set_state(self)
 
         if global_region is not None:
             self.global_region: MultiValuedMemory = global_region
             self.global_region._phi_maker = self._make_phi_variable
         else:
             self.global_region: MultiValuedMemory = MultiValuedMemory(
                 memory_id="mem",
                 top_func=self.top,
+                is_top_func=self.is_top,
                 phi_maker=self._make_phi_variable,
                 skip_missing_values_during_merging=True,
                 page_kwargs={"mo_cmp": self._mo_cmp},
             )
         self.global_region.set_state(self)
 
         # Used during merging
         self.successor_block_addr: Optional[int] = None
         self.phi_variables: Dict[SimVariable, SimVariable] = {}
 
         self.typevars = TypeVariables() if typevars is None else typevars
         self.type_constraints = defaultdict(set) if type_constraints is None else type_constraints
         self.func_typevar = func_typevar
         self.delayed_type_constraints = (
-            DefaultChainMapCOW(set, collapse_threshold=25)
+            DefaultChainMapCOW(default_factory=set, collapse_threshold=25)
             if delayed_type_constraints is None
             else delayed_type_constraints
         )
         self.stack_offset_typevars: Dict[int, TypeVariable] = (
             {} if stack_offset_typevars is None else stack_offset_typevars
         )
```

### Comparing `angr-9.2.96/angr/analyses/variable_recovery/variable_recovery_fast.py` & `angr-9.2.97/angr/analyses/variable_recovery/variable_recovery_fast.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/veritesting.py` & `angr-9.2.97/angr/analyses/veritesting.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/vfg.py` & `angr-9.2.97/angr/analyses/vfg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/vsa_ddg.py` & `angr-9.2.97/angr/analyses/vsa_ddg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/vtable.py` & `angr-9.2.97/angr/analyses/vtable.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/analyses/xrefs.py` & `angr-9.2.97/angr/analyses/xrefs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/angrdb/db.py` & `angr-9.2.97/angr/angrdb/db.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/angrdb/models.py` & `angr-9.2.97/angr/angrdb/models.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/angrdb/serializers/cfg_model.py` & `angr-9.2.97/angr/angrdb/serializers/cfg_model.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/angrdb/serializers/comments.py` & `angr-9.2.97/angr/angrdb/serializers/comments.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/angrdb/serializers/funcs.py` & `angr-9.2.97/angr/angrdb/serializers/funcs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/angrdb/serializers/kb.py` & `angr-9.2.97/angr/angrdb/serializers/kb.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/angrdb/serializers/labels.py` & `angr-9.2.97/angr/angrdb/serializers/labels.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/angrdb/serializers/loader.py` & `angr-9.2.97/angr/angrdb/serializers/loader.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/angrdb/serializers/structured_code.py` & `angr-9.2.97/angr/angrdb/serializers/structured_code.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/angrdb/serializers/variables.py` & `angr-9.2.97/angr/angrdb/serializers/variables.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/angrdb/serializers/xrefs.py` & `angr-9.2.97/angr/angrdb/serializers/xrefs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/annocfg.py` & `angr-9.2.97/angr/annocfg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/blade.py` & `angr-9.2.97/angr/blade.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/block.py` & `angr-9.2.97/angr/block.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/callable.py` & `angr-9.2.97/angr/callable.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/calling_conventions.py` & `angr-9.2.97/angr/calling_conventions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/code_location.py` & `angr-9.2.97/angr/code_location.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/codenode.py` & `angr-9.2.97/angr/codenode.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/concretization_strategies/__init__.py` & `angr-9.2.97/angr/concretization_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/concretization_strategies/any_named.py` & `angr-9.2.97/angr/concretization_strategies/any_named.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/concretization_strategies/controlled_data.py` & `angr-9.2.97/angr/concretization_strategies/controlled_data.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/concretization_strategies/eval.py` & `angr-9.2.97/angr/concretization_strategies/eval.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/concretization_strategies/logging.py` & `angr-9.2.97/angr/concretization_strategies/logging.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/concretization_strategies/max.py` & `angr-9.2.97/angr/concretization_strategies/max.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/concretization_strategies/nonzero.py` & `angr-9.2.97/angr/concretization_strategies/nonzero.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/concretization_strategies/nonzero_range.py` & `angr-9.2.97/angr/concretization_strategies/nonzero_range.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/concretization_strategies/norepeats.py` & `angr-9.2.97/angr/concretization_strategies/norepeats.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/concretization_strategies/norepeats_range.py` & `angr-9.2.97/angr/concretization_strategies/norepeats_range.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/concretization_strategies/range.py` & `angr-9.2.97/angr/concretization_strategies/range.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/concretization_strategies/signed_add.py` & `angr-9.2.97/angr/concretization_strategies/signed_add.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/concretization_strategies/solutions.py` & `angr-9.2.97/angr/concretization_strategies/solutions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/concretization_strategies/unlimited_range.py` & `angr-9.2.97/angr/concretization_strategies/unlimited_range.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/distributed/server.py` & `angr-9.2.97/angr/distributed/server.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/distributed/worker.py` & `angr-9.2.97/angr/distributed/worker.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/__init__.py` & `angr-9.2.97/angr/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/concrete.py` & `angr-9.2.97/angr/engines/concrete.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/engine.py` & `angr-9.2.97/angr/engines/engine.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/failure.py` & `angr-9.2.97/angr/engines/failure.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/hook.py` & `angr-9.2.97/angr/engines/hook.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/light/data.py` & `angr-9.2.97/angr/engines/light/data.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/light/engine.py` & `angr-9.2.97/angr/engines/light/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1074,15 +1074,22 @@
 
         if expr_0 is None:
             expr_0 = arg0
         if expr_1 is None:
             expr_1 = arg1
 
         return ailment.Expr.BinaryOp(
-            expr.idx, "DivMod", [expr_0, expr_1], expr.signed, bits=expr_0.bits * 2, **expr.tags
+            expr.idx,
+            "DivMod",
+            [expr_0, expr_1],
+            expr.signed,
+            bits=expr.bits,
+            from_bits=expr.from_bits,
+            to_bits=expr.to_bits,
+            **expr.tags,
         )
 
     def _ail_handle_Mod(self, expr):
         arg0, arg1 = expr.operands
 
         expr_0 = self._expr(arg0)
         expr_1 = self._expr(arg1)
```

### Comparing `angr-9.2.96/angr/engines/pcode/behavior.py` & `angr-9.2.97/angr/engines/pcode/behavior.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/pcode/cc.py` & `angr-9.2.97/angr/engines/pcode/cc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/pcode/emulate.py` & `angr-9.2.97/angr/engines/pcode/emulate.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/pcode/engine.py` & `angr-9.2.97/angr/engines/pcode/engine.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/pcode/lifter.py` & `angr-9.2.97/angr/engines/pcode/lifter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/procedure.py` & `angr-9.2.97/angr/engines/procedure.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/engine.py` & `angr-9.2.97/angr/engines/soot/engine.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/expressions/__init__.py` & `angr-9.2.97/angr/engines/soot/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/expressions/arrayref.py` & `angr-9.2.97/angr/engines/soot/expressions/arrayref.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/expressions/binop.py` & `angr-9.2.97/angr/engines/soot/expressions/binop.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/expressions/cast.py` & `angr-9.2.97/angr/engines/soot/expressions/cast.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/expressions/condition.py` & `angr-9.2.97/angr/engines/soot/expressions/condition.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/expressions/constants.py` & `angr-9.2.97/angr/engines/soot/expressions/constants.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/expressions/invoke.py` & `angr-9.2.97/angr/engines/soot/expressions/invoke.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/expressions/new.py` & `angr-9.2.97/angr/engines/soot/expressions/new.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/expressions/newArray.py` & `angr-9.2.97/angr/engines/soot/expressions/newArray.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/expressions/newMultiArray.py` & `angr-9.2.97/angr/engines/soot/expressions/newMultiArray.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/expressions/phi.py` & `angr-9.2.97/angr/engines/soot/expressions/phi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/field_dispatcher.py` & `angr-9.2.97/angr/engines/soot/field_dispatcher.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/method_dispatcher.py` & `angr-9.2.97/angr/engines/soot/method_dispatcher.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/statements/__init__.py` & `angr-9.2.97/angr/engines/soot/statements/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/statements/assign.py` & `angr-9.2.97/angr/engines/soot/statements/assign.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/statements/base.py` & `angr-9.2.97/angr/engines/soot/statements/base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/statements/if_.py` & `angr-9.2.97/angr/engines/soot/statements/if_.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/statements/switch.py` & `angr-9.2.97/angr/engines/soot/statements/switch.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/values/__init__.py` & `angr-9.2.97/angr/engines/soot/values/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/values/arrayref.py` & `angr-9.2.97/angr/engines/soot/values/arrayref.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/values/instancefieldref.py` & `angr-9.2.97/angr/engines/soot/values/instancefieldref.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/values/staticfieldref.py` & `angr-9.2.97/angr/engines/soot/values/staticfieldref.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/values/strref.py` & `angr-9.2.97/angr/engines/soot/values/strref.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/soot/values/thisref.py` & `angr-9.2.97/angr/engines/soot/values/thisref.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/successors.py` & `angr-9.2.97/angr/engines/successors.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/syscall.py` & `angr-9.2.97/angr/engines/syscall.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/unicorn.py` & `angr-9.2.97/angr/engines/unicorn.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/vex/claripy/ccall.py` & `angr-9.2.97/angr/engines/vex/claripy/ccall.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/vex/claripy/datalayer.py` & `angr-9.2.97/angr/engines/vex/claripy/datalayer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/vex/claripy/irop.py` & `angr-9.2.97/angr/engines/vex/claripy/irop.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/vex/heavy/actions.py` & `angr-9.2.97/angr/engines/vex/heavy/actions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/vex/heavy/concretizers.py` & `angr-9.2.97/angr/engines/vex/heavy/concretizers.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/vex/heavy/dirty.py` & `angr-9.2.97/angr/engines/vex/heavy/dirty.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/vex/heavy/heavy.py` & `angr-9.2.97/angr/engines/vex/heavy/heavy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/vex/heavy/inspect.py` & `angr-9.2.97/angr/engines/vex/heavy/inspect.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/vex/heavy/resilience.py` & `angr-9.2.97/angr/engines/vex/heavy/resilience.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/vex/heavy/super_fastpath.py` & `angr-9.2.97/angr/engines/vex/heavy/super_fastpath.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/vex/lifter.py` & `angr-9.2.97/angr/engines/vex/lifter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/vex/light/light.py` & `angr-9.2.97/angr/engines/vex/light/light.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/vex/light/resilience.py` & `angr-9.2.97/angr/engines/vex/light/resilience.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/engines/vex/light/slicing.py` & `angr-9.2.97/angr/engines/vex/light/slicing.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/errors.py` & `angr-9.2.97/angr/errors.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/__init__.py` & `angr-9.2.97/angr/exploration_techniques/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/bucketizer.py` & `angr-9.2.97/angr/exploration_techniques/bucketizer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/common.py` & `angr-9.2.97/angr/exploration_techniques/common.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/dfs.py` & `angr-9.2.97/angr/exploration_techniques/dfs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/director.py` & `angr-9.2.97/angr/exploration_techniques/director.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/driller_core.py` & `angr-9.2.97/angr/exploration_techniques/driller_core.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/explorer.py` & `angr-9.2.97/angr/exploration_techniques/explorer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/lengthlimiter.py` & `angr-9.2.97/angr/exploration_techniques/lengthlimiter.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/local_loop_seer.py` & `angr-9.2.97/angr/exploration_techniques/local_loop_seer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/loop_seer.py` & `angr-9.2.97/angr/exploration_techniques/loop_seer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/manual_mergepoint.py` & `angr-9.2.97/angr/exploration_techniques/manual_mergepoint.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/memory_watcher.py` & `angr-9.2.97/angr/exploration_techniques/memory_watcher.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/oppologist.py` & `angr-9.2.97/angr/exploration_techniques/oppologist.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/slicecutor.py` & `angr-9.2.97/angr/exploration_techniques/slicecutor.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/spiller.py` & `angr-9.2.97/angr/exploration_techniques/spiller.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/spiller_db.py` & `angr-9.2.97/angr/exploration_techniques/spiller_db.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/stochastic.py` & `angr-9.2.97/angr/exploration_techniques/stochastic.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/suggestions.py` & `angr-9.2.97/angr/exploration_techniques/suggestions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/symbion.py` & `angr-9.2.97/angr/exploration_techniques/symbion.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/tech_builder.py` & `angr-9.2.97/angr/exploration_techniques/tech_builder.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/threading.py` & `angr-9.2.97/angr/exploration_techniques/threading.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/timeout.py` & `angr-9.2.97/angr/exploration_techniques/timeout.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/tracer.py` & `angr-9.2.97/angr/exploration_techniques/tracer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/unique.py` & `angr-9.2.97/angr/exploration_techniques/unique.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/exploration_techniques/veritesting.py` & `angr-9.2.97/angr/exploration_techniques/veritesting.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/factory.py` & `angr-9.2.97/angr/factory.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/flirt/__init__.py` & `angr-9.2.97/angr/flirt/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/flirt/build_sig.py` & `angr-9.2.97/angr/flirt/build_sig.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/keyed_region.py` & `angr-9.2.97/angr/keyed_region.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_base/knowledge_base.py` & `angr-9.2.97/angr/knowledge_base/knowledge_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/__init__.py` & `angr-9.2.97/angr/knowledge_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/callsite_prototypes.py` & `angr-9.2.97/angr/knowledge_plugins/callsite_prototypes.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/cfg/cfg_manager.py` & `angr-9.2.97/angr/knowledge_plugins/cfg/cfg_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/cfg/cfg_model.py` & `angr-9.2.97/angr/knowledge_plugins/cfg/cfg_model.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/cfg/cfg_node.py` & `angr-9.2.97/angr/knowledge_plugins/cfg/cfg_node.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/cfg/indirect_jump.py` & `angr-9.2.97/angr/knowledge_plugins/cfg/indirect_jump.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/cfg/memory_data.py` & `angr-9.2.97/angr/knowledge_plugins/cfg/memory_data.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/custom_strings.py` & `angr-9.2.97/angr/knowledge_plugins/custom_strings.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/data.py` & `angr-9.2.97/angr/knowledge_plugins/data.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/debug_variables.py` & `angr-9.2.97/angr/knowledge_plugins/debug_variables.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/functions/function.py` & `angr-9.2.97/angr/knowledge_plugins/functions/function.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/functions/function_manager.py` & `angr-9.2.97/angr/knowledge_plugins/functions/function_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/functions/function_parser.py` & `angr-9.2.97/angr/knowledge_plugins/functions/function_parser.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/functions/soot_function.py` & `angr-9.2.97/angr/knowledge_plugins/functions/soot_function.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/indirect_jumps.py` & `angr-9.2.97/angr/knowledge_plugins/indirect_jumps.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/key_definitions/atoms.py` & `angr-9.2.97/angr/knowledge_plugins/key_definitions/atoms.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/key_definitions/definition.py` & `angr-9.2.97/angr/knowledge_plugins/key_definitions/definition.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/key_definitions/environment.py` & `angr-9.2.97/angr/knowledge_plugins/key_definitions/environment.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     Represent the environment in which a program runs.
     It's a mapping of variable names, to `claripy.ast.Base` that should contain possible addresses, or <UNDEFINED>, at
     which their respective values are stored.
 
     **Note**: The <Environment> object does not store the values associated with variables themselves.
     """
 
+    __slots__ = ("_environment",)
+
     def __init__(self, environment: Dict[Union[str, Undefined], Set[claripy.ast.Base]] = None):
         self._environment: Dict[Union[str, Undefined], Set[claripy.ast.Base]] = environment or {}
 
     def get(self, names: Set[str]) -> Tuple[Set[claripy.ast.Base], bool]:
         """
         :param names: Potential values for the name of the environment variable to get the pointers of.
         :return:
@@ -77,7 +79,16 @@
                     return v
                 return v | w
 
             new_env = dict(map(lambda k: (k, _dataset_from_key(k, new_env, other._environment)), keys))
 
         merge_occurred = new_env != self._environment
         return Environment(environment=new_env), merge_occurred
+
+    def compare(self, other: "Environment") -> bool:
+        for k in set(self._environment.keys()).union(set(other._environment.keys())):
+            if k not in self._environment:
+                return False
+            if k in self._environment and k in other._environment:
+                if not self._environment[k].issuperset(other._environment[k]):
+                    return False
+        return True
```

### Comparing `angr-9.2.96/angr/knowledge_plugins/key_definitions/heap_address.py` & `angr-9.2.97/angr/knowledge_plugins/key_definitions/heap_address.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/key_definitions/key_definition_manager.py` & `angr-9.2.97/angr/knowledge_plugins/key_definitions/key_definition_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/key_definitions/live_definitions.py` & `angr-9.2.97/angr/knowledge_plugins/key_definitions/live_definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,38 +45,35 @@
 
 
 class DefinitionAnnotation(Annotation):
     """
     An annotation that attaches a `Definition` to an AST.
     """
 
-    __slots__ = ("definition",)
+    __slots__ = ("definition", "_hash")
 
     def __init__(self, definition):
         super().__init__()
         self.definition = definition
+        self._hash = hash((DefinitionAnnotation, self.definition))
 
     @property
     def relocatable(self):
         return True
 
     @property
     def eliminatable(self):
         return False
 
     def __hash__(self):
-        return hash((self.definition, self.relocatable, self.eliminatable))
+        return self._hash
 
     def __eq__(self, other: "object"):
-        if isinstance(other, DefinitionAnnotation):
-            return (
-                self.definition == other.definition
-                and self.relocatable == other.relocatable
-                and self.eliminatable == other.eliminatable
-            )
+        if type(other) is DefinitionAnnotation:
+            return self.definition == other.definition
         else:
             return False
 
     def __repr__(self):
         return f"<{self.__class__.__name__}({repr(self.definition)})"
 
 
@@ -125,57 +122,66 @@
         others=None,
         register_uses=None,
         stack_uses=None,
         heap_uses=None,
         memory_uses=None,
         tmp_uses=None,
         other_uses=None,
+        element_limit=5,
     ):
         self.project: Optional["Project"] = None
         self.arch = arch
         self.track_tmps = track_tmps
         self._canonical_size: int = canonical_size  # TODO: Drop canonical_size
 
         self.registers: MultiValuedMemory = (
             MultiValuedMemory(
                 memory_id="reg",
                 top_func=self.top,
+                is_top_func=self.is_top,
                 skip_missing_values_during_merging=False,
                 page_kwargs={"mo_cmp": self._mo_cmp},
                 endness=self.arch.register_endness,
+                element_limit=element_limit,
             )
             if registers is None
             else registers
         )
         self.stack: MultiValuedMemory = (
             MultiValuedMemory(
                 memory_id="mem",
                 top_func=self.top,
+                is_top_func=self.is_top,
                 skip_missing_values_during_merging=False,
                 page_kwargs={"mo_cmp": self._mo_cmp},
+                element_limit=element_limit,
             )
             if stack is None
             else stack
         )
         self.memory: MultiValuedMemory = (
             MultiValuedMemory(
                 memory_id="mem",
                 top_func=self.top,
+                is_top_func=self.is_top,
                 skip_missing_values_during_merging=False,
                 page_kwargs={"mo_cmp": self._mo_cmp},
+                element_limit=element_limit,
             )
             if memory is None
             else memory
         )
         self.heap: MultiValuedMemory = (
             MultiValuedMemory(
                 memory_id="mem",
                 top_func=self.top,
+                is_top_func=self.is_top,
                 skip_missing_values_during_merging=False,
                 page_kwargs={"mo_cmp": self._mo_cmp},
+                element_limit=element_limit,
             )
             if heap is None
             else heap
         )
         self.tmps: Dict[int, Set[Definition]] = {} if tmps is None else tmps
         self.others: Dict[Atom, MultiValues] = others if others is not None else {}
 
@@ -460,14 +466,41 @@
             merge_occurred |= state.stack_uses.merge(other.stack_uses)
             merge_occurred |= state.heap_uses.merge(other.heap_uses)
             merge_occurred |= state.memory_uses.merge(other.memory_uses)
             merge_occurred |= state.other_uses.merge(other.other_uses)
 
         return state, merge_occurred
 
+    def compare(self, other: "LiveDefinitions") -> bool:
+        r0 = self.registers.compare(other.registers)
+        if r0 is False:
+            return False
+        r1 = self.heap.compare(other.heap)
+        if r1 is False:
+            return False
+        r2 = self.memory.compare(other.memory)
+        if r2 is False:
+            return False
+        r3 = self.stack.compare(other.stack)
+        if r3 is False:
+            return False
+
+        r4 = True
+        for k in other.others:
+            if k in self.others:
+                thing = self.others[k].merge(other.others[k])
+                if thing != self.others[k]:
+                    r4 = False
+                    break
+            else:
+                r4 = False
+                break
+
+        return r0 and r1 and r2 and r3 and r4
+
     def kill_definitions(self, atom: Atom) -> None:
         """
         Overwrite existing definitions w.r.t 'atom' with a dummy definition instance. A dummy definition will not be
         removed during simplification.
 
         :param atom:
         :return: None
```

### Comparing `angr-9.2.96/angr/knowledge_plugins/key_definitions/liveness.py` & `angr-9.2.97/angr/knowledge_plugins/key_definitions/liveness.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/key_definitions/rd_model.py` & `angr-9.2.97/angr/knowledge_plugins/key_definitions/rd_model.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/key_definitions/tag.py` & `angr-9.2.97/angr/knowledge_plugins/key_definitions/tag.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/key_definitions/undefined.py` & `angr-9.2.97/angr/knowledge_plugins/key_definitions/undefined.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/key_definitions/unknown_size.py` & `angr-9.2.97/angr/knowledge_plugins/key_definitions/unknown_size.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/key_definitions/uses.py` & `angr-9.2.97/angr/knowledge_plugins/key_definitions/uses.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,29 +17,35 @@
 
     def __init__(
         self,
         uses_by_definition: Optional[DefaultChainMapCOW] = None,
         uses_by_location: Optional[DefaultChainMapCOW] = None,
     ):
         self._uses_by_definition: DefaultChainMapCOW["Definition", Set[Tuple[CodeLocation, Optional[Any]]]] = (
-            DefaultChainMapCOW(set, collapse_threshold=25) if uses_by_definition is None else uses_by_definition
+            DefaultChainMapCOW(default_factory=set, collapse_threshold=25)
+            if uses_by_definition is None
+            else uses_by_definition
         )
         self._uses_by_location: DefaultChainMapCOW[CodeLocation, Set[Tuple["Definition", Optional[Any]]]] = (
-            DefaultChainMapCOW(set, collapse_threshold=25) if uses_by_location is None else uses_by_location
+            DefaultChainMapCOW(default_factory=set, collapse_threshold=25)
+            if uses_by_location is None
+            else uses_by_location
         )
 
     def add_use(self, definition: "Definition", codeloc: CodeLocation, expr: Optional[Any] = None):
         """
         Add a use for a given definition.
 
         :param definition:  The definition that is used.
         :param codeloc:     The code location where the use occurs.
         :param expr:        The expression that uses the specified definition at this location.
         """
+        self._uses_by_definition = self._uses_by_definition.clean()
         self._uses_by_definition[definition].add((codeloc, expr))
+        self._uses_by_location = self._uses_by_location.clean()
         self._uses_by_location[codeloc].add((definition, expr))
 
     def get_uses(self, definition: "Definition") -> Set[CodeLocation]:
         """
         Retrieve the uses of a given definition.
 
         :param definition: The definition for which we get the uses.
@@ -61,37 +67,41 @@
         :param definition:  The definition of which to remove the uses.
         :param codeloc:     The code location where the use is.
         :param expr:        The expression that uses the definition at the given location.
         :return:            None
         """
         if definition in self._uses_by_definition:
             if codeloc in self._uses_by_definition[definition]:
+                self._uses_by_definition = self._uses_by_definition.clean()
                 if expr is None:
                     for codeloc_, expr_ in list(self._uses_by_definition[definition]):
                         if codeloc_ == codeloc:
                             self._uses_by_definition[definition].remove((codeloc_, expr_))
                 else:
                     self._uses_by_definition[definition].remove((codeloc, expr))
 
         if codeloc in self._uses_by_location:
+            self._uses_by_location = self._uses_by_location.clean()
             for item in list(self._uses_by_location[codeloc]):
                 if item[0] == definition:
                     self._uses_by_location[codeloc].remove(item)
 
     def remove_uses(self, definition: "Definition"):
         """
         Remove all uses of a given definition.
 
         :param definition:  The definition of which to remove the uses.
         :return:            None
         """
         if definition in self._uses_by_definition:
+            self._uses_by_definition = self._uses_by_definition.clean()
             codeloc_and_ids = self._uses_by_definition[definition]
             del self._uses_by_definition[definition]
 
+            self._uses_by_location = self._uses_by_location.clean()
             for codeloc, _ in codeloc_and_ids:
                 for item in list(self._uses_by_location[codeloc]):
                     if item[0] == definition:
                         self._uses_by_location[codeloc].remove(item)
 
     def get_uses_by_location(
         self, codeloc: CodeLocation, exprs: bool = False
@@ -145,22 +155,26 @@
         :param other: The other <Uses> from which the data will be added to the current instance.
         :return: True if any merge occurred, False otherwise
         """
         merge_occurred = False
 
         for k, v in other._uses_by_definition.items():
             if k not in self._uses_by_definition:
+                self._uses_by_definition = self._uses_by_definition.clean()
                 self._uses_by_definition[k] = v
                 merge_occurred = True
             elif not v.issubset(self._uses_by_definition[k]):
                 merge_occurred = True
-                self._uses_by_definition[k] |= v
+                self._uses_by_definition = self._uses_by_definition.clean()
+                self._uses_by_definition[k] = self._uses_by_definition[k] | v
 
         for k, v in other._uses_by_location.items():
             if k not in self._uses_by_location:
+                self._uses_by_location = self._uses_by_location.clean()
                 self._uses_by_location[k] = v
                 merge_occurred = True
             elif not v.issubset(self._uses_by_location[k]):
                 merge_occurred = True
-                self._uses_by_location[k] |= v
+                self._uses_by_location = self._uses_by_location.clean()
+                self._uses_by_location[k] = self._uses_by_location[k] | v
 
         return merge_occurred
```

### Comparing `angr-9.2.96/angr/knowledge_plugins/labels.py` & `angr-9.2.97/angr/knowledge_plugins/labels.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/patches.py` & `angr-9.2.97/angr/knowledge_plugins/patches.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/plugin.py` & `angr-9.2.97/angr/knowledge_plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/propagations/prop_value.py` & `angr-9.2.97/angr/knowledge_plugins/propagations/prop_value.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/propagations/propagation_manager.py` & `angr-9.2.97/angr/knowledge_plugins/propagations/propagation_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/propagations/propagation_model.py` & `angr-9.2.97/angr/knowledge_plugins/propagations/propagation_model.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/propagations/states.py` & `angr-9.2.97/angr/knowledge_plugins/propagations/states.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,17 +217,18 @@
             else:
                 for var, repl in vars_.items():
                     if var not in replacements_0[loc]:
                         replacements_0[loc][var] = repl
                         merge_occurred = True
                     else:
                         if PropagatorState.is_top(repl) or PropagatorState.is_top(replacements_0[loc][var]):
-                            t = PropagatorState.top(_get_repl_size(repl))
-                            replacements_0[loc][var] = t
-                            merge_occurred = True
+                            if not PropagatorState.is_top(replacements_0[loc][var]):
+                                t = PropagatorState.top(_get_repl_size(repl))
+                                replacements_0[loc][var] = t
+                                merge_occurred = True
                         elif (
                             isinstance(replacements_0[loc][var], claripy.ast.Base) or isinstance(repl, claripy.ast.Base)
                         ) and replacements_0[loc][var] is not repl:
                             replacements_0[loc][var] = repl
                             merge_occurred = True
                         elif (
                             not isinstance(replacements_0[loc][var], claripy.ast.Base)
@@ -312,14 +313,20 @@
     def eliminatable(self) -> bool:
         return True
 
     @property
     def relocatable(self) -> bool:
         return True
 
+    def __hash__(self):
+        return hash((RegisterAnnotation, self.offset, self.size))
+
+    def __eq__(self, other):
+        return type(other) is RegisterAnnotation and self.offset == other.offset and self.size == other.size
+
 
 class RegisterComparisonAnnotation(claripy.Annotation):
     """
     Annotate TOP values that are the result of register values comparing against constant values.
     """
 
     def __init__(self, offset, size, cmp_op, value):
@@ -332,14 +339,26 @@
     def eliminatable(self) -> bool:
         return True
 
     @property
     def relocatable(self) -> bool:
         return True
 
+    def __hash__(self):
+        return hash((RegisterComparisonAnnotation, self.offset, self.size, self.cmp_op, self.value))
+
+    def __eq__(self, other):
+        return (
+            type(other) is RegisterAnnotation
+            and self.offset == other.offset
+            and self.size == other.size
+            and self.cmp_op == other.cmp_op
+            and self.value == other.value
+        )
+
 
 class PropagatorVEXState(PropagatorState):
     """
     Describes the state used in the VEX engine of Propagator.
     """
 
     __slots__ = (
```

### Comparing `angr-9.2.96/angr/knowledge_plugins/structured_code/manager.py` & `angr-9.2.97/angr/knowledge_plugins/structured_code/manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/sync/sync_controller.py` & `angr-9.2.97/angr/knowledge_plugins/sync/sync_controller.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/types.py` & `angr-9.2.97/angr/knowledge_plugins/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,14 +52,20 @@
 
         super().__setitem__(item, value.with_arch(self._kb._project.arch))
 
     def __iter__(self):
         yield from super().__iter__()
         yield from iter(ALL_TYPES)
 
+    def __getstate__(self):
+        return self.data  # do not pickle self.kb
+
+    def __setstate__(self, state):
+        self.data = state
+
     def iter_own(self):
         """
         Iterate over all the names which are stored in this object - i.e. ``values()`` without ``ALL_TYPES``
         """
         for key in super().__iter__():
             yield self[key]
```

### Comparing `angr-9.2.96/angr/knowledge_plugins/variables/variable_access.py` & `angr-9.2.97/angr/knowledge_plugins/variables/variable_access.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/variables/variable_manager.py` & `angr-9.2.97/angr/knowledge_plugins/variables/variable_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,40 @@
     # Serialization
     #
 
     def __setstate__(self, state):
         self.__dict__.update(state)
 
     def __getstate__(self):
-        d = dict(self.__dict__)
+        attributes = [
+            "func_addr",
+            "_variables",
+            "_global_region",
+            "_stack_region",
+            "_register_region",
+            "_live_variables",
+            "_variable_accesses",
+            "_insn_to_variable",
+            "_stmt_to_variable",
+            "_variable_to_stmt",
+            "_atom_to_variable",
+            "_ident_to_variable",
+            "_variable_counters",
+            "_unified_variables",
+            "_variables_to_unified_variables",
+            "_phi_variables",
+            "_variables_to_phivars",
+            "_phi_variables_by_block",
+            "types",
+            "variable_to_types",
+            "variables_with_manual_types",
+            "_variables_without_writes",
+            "ret_val_size",
+        ]
+        d = {k: getattr(self, k) for k in attributes}
         d["manager"] = None
         d["types"].kb = None
         return d
 
     def set_manager(self, manager: "VariableManager"):
         self.manager = manager
         self.types.kb = manager._kb
@@ -755,18 +780,19 @@
 
         input_variables = []
 
         for variable in self._variables_without_writes:
             if variable in self._phi_variables:
                 # a phi variable is definitely not an input variable
                 continue
-            accesses = self._variable_accesses[variable]
-            if has_read_access(accesses):
-                if not exclude_specials or not variable.category:
-                    input_variables.append(variable)
+            if variable in self._variable_accesses:
+                accesses = self._variable_accesses[variable]
+                if has_read_access(accesses):
+                    if not exclude_specials or not variable.category:
+                        input_variables.append(variable)
 
         return input_variables
 
     def assign_variable_names(self, labels=None, types=None):
         """
         Assign default names to all SSA variables.
```

### Comparing `angr-9.2.96/angr/knowledge_plugins/xrefs/xref.py` & `angr-9.2.97/angr/knowledge_plugins/xrefs/xref.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/knowledge_plugins/xrefs/xref_manager.py` & `angr-9.2.97/angr/knowledge_plugins/xrefs/xref_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/misc/ansi.py` & `angr-9.2.97/angr/misc/ansi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/misc/autoimport.py` & `angr-9.2.97/angr/misc/autoimport.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/misc/bug_report.py` & `angr-9.2.97/angr/misc/bug_report.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/misc/hookset.py` & `angr-9.2.97/angr/misc/hookset.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/misc/import_hooks.py` & `angr-9.2.97/angr/misc/import_hooks.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/misc/loggers.py` & `angr-9.2.97/angr/misc/loggers.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/misc/picklable_lock.py` & `angr-9.2.97/angr/misc/picklable_lock.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/misc/plugins.py` & `angr-9.2.97/angr/misc/plugins.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/misc/testing.py` & `angr-9.2.97/angr/misc/testing.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/misc/ux.py` & `angr-9.2.97/angr/misc/ux.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/misc/weakpatch.py` & `angr-9.2.97/angr/misc/weakpatch.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/cgc/allocate.py` & `angr-9.2.97/angr/procedures/cgc/allocate.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/cgc/deallocate.py` & `angr-9.2.97/angr/procedures/cgc/deallocate.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/cgc/fdwait.py` & `angr-9.2.97/angr/procedures/cgc/fdwait.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/cgc/random.py` & `angr-9.2.97/angr/procedures/cgc/random.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/cgc/receive.py` & `angr-9.2.97/angr/procedures/cgc/receive.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/cgc/transmit.py` & `angr-9.2.97/angr/procedures/cgc/transmit.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/__init__.py` & `angr-9.2.97/angr/procedures/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/glibc.py` & `angr-9.2.97/angr/procedures/definitions/glibc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/gnulib.py` & `angr-9.2.97/angr/procedures/definitions/gnulib.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/libstdcpp.py` & `angr-9.2.97/angr/procedures/definitions/libstdcpp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/linux_kernel.py` & `angr-9.2.97/angr/procedures/definitions/linux_kernel.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/msvcr.py` & `angr-9.2.97/angr/procedures/definitions/msvcr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/parse_syscalls_from_local_system.py` & `angr-9.2.97/angr/procedures/definitions/parse_syscalls_from_local_system.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/parse_win32json.py` & `angr-9.2.97/angr/procedures/definitions/parse_win32json.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/types_win32.py` & `angr-9.2.97/angr/procedures/definitions/types_win32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/wdk_api-ms-win-dx-d3dkmt-l1-1-4.py` & `angr-9.2.97/angr/procedures/definitions/wdk_api-ms-win-dx-d3dkmt-l1-1-4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/wdk_api-ms-win-dx-d3dkmt-l1-1-6.py` & `angr-9.2.97/angr/procedures/definitions/wdk_api-ms-win-dx-d3dkmt-l1-1-6.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/wdk_clfs.py` & `angr-9.2.97/angr/procedures/definitions/wdk_clfs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/wdk_fltmgr.py` & `angr-9.2.97/angr/procedures/definitions/wdk_fltmgr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/wdk_fwpkclnt.py` & `angr-9.2.97/angr/procedures/definitions/wdk_fwpkclnt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/wdk_fwpuclnt.py` & `angr-9.2.97/angr/procedures/definitions/wdk_fwpuclnt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/wdk_gdi32.py` & `angr-9.2.97/angr/procedures/definitions/wdk_gdi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/wdk_hal.py` & `angr-9.2.97/angr/procedures/definitions/wdk_hal.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/wdk_ksecdd.py` & `angr-9.2.97/angr/procedures/definitions/wdk_ksecdd.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/wdk_ndis.py` & `angr-9.2.97/angr/procedures/definitions/wdk_ndis.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/wdk_ntoskrnl.py` & `angr-9.2.97/angr/procedures/definitions/wdk_ntoskrnl.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/wdk_offreg.py` & `angr-9.2.97/angr/procedures/definitions/wdk_offreg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/wdk_pshed.py` & `angr-9.2.97/angr/procedures/definitions/wdk_pshed.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/wdk_secur32.py` & `angr-9.2.97/angr/procedures/definitions/wdk_secur32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/wdk_vhfum.py` & `angr-9.2.97/angr/procedures/definitions/wdk_vhfum.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_aclui.py` & `angr-9.2.97/angr/procedures/definitions/win32_aclui.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_activeds.py` & `angr-9.2.97/angr/procedures/definitions/win32_activeds.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_advapi32.py` & `angr-9.2.97/angr/procedures/definitions/win32_advapi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_advpack.py` & `angr-9.2.97/angr/procedures/definitions/win32_advpack.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_amsi.py` & `angr-9.2.97/angr/procedures/definitions/win32_amsi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-1.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-3.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-3.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-6.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-appmodel-runtime-l1-1-6.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-apiquery-l2-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-apiquery-l2-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-backgroundtask-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-backgroundtask-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-1.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-2.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-comm-l1-1-2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-enclave-l1-1-1.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-enclave-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-errorhandling-l1-1-3.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-errorhandling-l1-1-3.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-1.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-featurestaging-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-file-fromapp-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-file-fromapp-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-handle-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-handle-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-ioring-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-ioring-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-marshal-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-marshal-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-3.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-3.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-4.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-5.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-5.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-6.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-6.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-7.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-7.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-8.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-memory-l1-1-8.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-path-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-path-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-1.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-psm-appnotify-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-1.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-2.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-realtime-l1-1-2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-slapi-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-slapi-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-state-helpers-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-state-helpers-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-synch-l1-2-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-synch-l1-2-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-3.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-3.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-4.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-6.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-sysinfo-l1-2-6.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-util-l1-1-1.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-util-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-1.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-error-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-winrt-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-winrt-registration-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-registration-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-winrt-robuffer-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-robuffer-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-winrt-roparameterizediid-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-roparameterizediid-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-1.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-winrt-string-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-core-wow64-l1-1-1.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-core-wow64-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-1.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-devices-query-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-dx-d3dkmt-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-dx-d3dkmt-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-gaming-deviceinformation-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-deviceinformation-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-gaming-expandedresources-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-expandedresources-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-1.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-2.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-3.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-3.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-4.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-gaming-tcui-l1-1-4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-mm-misc-l1-1-1.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-mm-misc-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-net-isolation-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-net-isolation-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-security-base-l1-2-2.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-security-base-l1-2-2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-1.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-security-isolatedcontainer-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-3.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-3.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-4.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-5.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-service-core-l1-1-5.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-1.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-2.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-shcore-scaling-l1-1-2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-shcore-stream-winrt-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-shcore-stream-winrt-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_api-ms-win-wsl-api-l1-1-0.py` & `angr-9.2.97/angr/procedures/definitions/win32_api-ms-win-wsl-api-l1-1-0.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_apphelp.py` & `angr-9.2.97/angr/procedures/definitions/win32_apphelp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_authz.py` & `angr-9.2.97/angr/procedures/definitions/win32_authz.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_avicap32.py` & `angr-9.2.97/angr/procedures/definitions/win32_avicap32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_avifil32.py` & `angr-9.2.97/angr/procedures/definitions/win32_avifil32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_avrt.py` & `angr-9.2.97/angr/procedures/definitions/win32_avrt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_bcp47mrm.py` & `angr-9.2.97/angr/procedures/definitions/win32_bcp47mrm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_bcrypt.py` & `angr-9.2.97/angr/procedures/definitions/win32_bcrypt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_bcryptprimitives.py` & `angr-9.2.97/angr/procedures/definitions/win32_bcryptprimitives.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_bluetoothapis.py` & `angr-9.2.97/angr/procedures/definitions/win32_bluetoothapis.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_bthprops.py` & `angr-9.2.97/angr/procedures/definitions/win32_bthprops.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_bthprops_cpl.py` & `angr-9.2.97/angr/procedures/definitions/win32_bthprops_cpl.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_cabinet.py` & `angr-9.2.97/angr/procedures/definitions/win32_cabinet.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_certadm.py` & `angr-9.2.97/angr/procedures/definitions/win32_certadm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_certpoleng.py` & `angr-9.2.97/angr/procedures/definitions/win32_certpoleng.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_cfgmgr32.py` & `angr-9.2.97/angr/procedures/definitions/win32_cfgmgr32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_chakra.py` & `angr-9.2.97/angr/procedures/definitions/win32_chakra.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_cldapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_cldapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_clfsw32.py` & `angr-9.2.97/angr/procedures/definitions/win32_clfsw32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_clusapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_clusapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_comctl32.py` & `angr-9.2.97/angr/procedures/definitions/win32_comctl32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_comdlg32.py` & `angr-9.2.97/angr/procedures/definitions/win32_comdlg32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_compstui.py` & `angr-9.2.97/angr/procedures/definitions/win32_compstui.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_computecore.py` & `angr-9.2.97/angr/procedures/definitions/win32_computecore.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_computenetwork.py` & `angr-9.2.97/angr/procedures/definitions/win32_computenetwork.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_computestorage.py` & `angr-9.2.97/angr/procedures/definitions/win32_computestorage.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_comsvcs.py` & `angr-9.2.97/angr/procedures/definitions/win32_comsvcs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_coremessaging.py` & `angr-9.2.97/angr/procedures/definitions/win32_coremessaging.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_credui.py` & `angr-9.2.97/angr/procedures/definitions/win32_credui.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_crypt32.py` & `angr-9.2.97/angr/procedures/definitions/win32_crypt32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_cryptnet.py` & `angr-9.2.97/angr/procedures/definitions/win32_cryptnet.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_cryptui.py` & `angr-9.2.97/angr/procedures/definitions/win32_cryptui.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_cryptxml.py` & `angr-9.2.97/angr/procedures/definitions/win32_cryptxml.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_cscapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_cscapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_d2d1.py` & `angr-9.2.97/angr/procedures/definitions/win32_d2d1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_d3d10.py` & `angr-9.2.97/angr/procedures/definitions/win32_d3d10.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_d3d10_1.py` & `angr-9.2.97/angr/procedures/definitions/win32_d3d10_1.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_d3d11.py` & `angr-9.2.97/angr/procedures/definitions/win32_d3d11.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_d3d12.py` & `angr-9.2.97/angr/procedures/definitions/win32_d3d12.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_d3d9.py` & `angr-9.2.97/angr/procedures/definitions/win32_d3d9.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_d3dcompiler_47.py` & `angr-9.2.97/angr/procedures/definitions/win32_d3dcompiler_47.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_d3dcsx.py` & `angr-9.2.97/angr/procedures/definitions/win32_d3dcsx.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_davclnt.py` & `angr-9.2.97/angr/procedures/definitions/win32_davclnt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dbgeng.py` & `angr-9.2.97/angr/procedures/definitions/win32_dbgeng.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dbghelp.py` & `angr-9.2.97/angr/procedures/definitions/win32_dbghelp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dbgmodel.py` & `angr-9.2.97/angr/procedures/definitions/win32_dbgmodel.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dciman32.py` & `angr-9.2.97/angr/procedures/definitions/win32_dciman32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dcomp.py` & `angr-9.2.97/angr/procedures/definitions/win32_dcomp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_ddraw.py` & `angr-9.2.97/angr/procedures/definitions/win32_ddraw.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_deviceaccess.py` & `angr-9.2.97/angr/procedures/definitions/win32_deviceaccess.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dflayout.py` & `angr-9.2.97/angr/procedures/definitions/win32_dflayout.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dhcpcsvc.py` & `angr-9.2.97/angr/procedures/definitions/win32_dhcpcsvc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dhcpcsvc6.py` & `angr-9.2.97/angr/procedures/definitions/win32_dhcpcsvc6.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dhcpsapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_dhcpsapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_diagnosticdataquery.py` & `angr-9.2.97/angr/procedures/definitions/win32_diagnosticdataquery.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dinput8.py` & `angr-9.2.97/angr/procedures/definitions/win32_dinput8.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_directml.py` & `angr-9.2.97/angr/procedures/definitions/win32_directml.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dmprocessxmlfiltered.py` & `angr-9.2.97/angr/procedures/definitions/win32_dmprocessxmlfiltered.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dnsapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_dnsapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_drt.py` & `angr-9.2.97/angr/procedures/definitions/win32_drt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_drtprov.py` & `angr-9.2.97/angr/procedures/definitions/win32_drtprov.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_drttransport.py` & `angr-9.2.97/angr/procedures/definitions/win32_drttransport.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dsound.py` & `angr-9.2.97/angr/procedures/definitions/win32_dsound.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dsparse.py` & `angr-9.2.97/angr/procedures/definitions/win32_dsparse.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dsprop.py` & `angr-9.2.97/angr/procedures/definitions/win32_dsprop.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dssec.py` & `angr-9.2.97/angr/procedures/definitions/win32_dssec.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dsuiext.py` & `angr-9.2.97/angr/procedures/definitions/win32_dsuiext.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dwmapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_dwmapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dwrite.py` & `angr-9.2.97/angr/procedures/definitions/win32_dwrite.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dxcompiler.py` & `angr-9.2.97/angr/procedures/definitions/win32_dxcompiler.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dxcore.py` & `angr-9.2.97/angr/procedures/definitions/win32_dxcore.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dxgi.py` & `angr-9.2.97/angr/procedures/definitions/win32_dxgi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_dxva2.py` & `angr-9.2.97/angr/procedures/definitions/win32_dxva2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_eappcfg.py` & `angr-9.2.97/angr/procedures/definitions/win32_eappcfg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_eappprxy.py` & `angr-9.2.97/angr/procedures/definitions/win32_eappprxy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_efswrt.py` & `angr-9.2.97/angr/procedures/definitions/win32_efswrt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_elscore.py` & `angr-9.2.97/angr/procedures/definitions/win32_elscore.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_esent.py` & `angr-9.2.97/angr/procedures/definitions/win32_esent.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_evr.py` & `angr-9.2.97/angr/procedures/definitions/win32_evr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_faultrep.py` & `angr-9.2.97/angr/procedures/definitions/win32_faultrep.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_fhsvcctl.py` & `angr-9.2.97/angr/procedures/definitions/win32_fhsvcctl.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_firewallapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_firewallapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_fltlib.py` & `angr-9.2.97/angr/procedures/definitions/win32_fltlib.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_fontsub.py` & `angr-9.2.97/angr/procedures/definitions/win32_fontsub.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_forceinline.py` & `angr-9.2.97/angr/procedures/definitions/win32_forceinline.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_fwpuclnt.py` & `angr-9.2.97/angr/procedures/definitions/win32_fwpuclnt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_fxsutility.py` & `angr-9.2.97/angr/procedures/definitions/win32_fxsutility.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_gdi32.py` & `angr-9.2.97/angr/procedures/definitions/win32_gdi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_gdiplus.py` & `angr-9.2.97/angr/procedures/definitions/win32_gdiplus.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_glu32.py` & `angr-9.2.97/angr/procedures/definitions/win32_glu32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_gpedit.py` & `angr-9.2.97/angr/procedures/definitions/win32_gpedit.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_hhctrl_ocx.py` & `angr-9.2.97/angr/procedures/definitions/win32_hhctrl_ocx.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_hid.py` & `angr-9.2.97/angr/procedures/definitions/win32_hid.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_hlink.py` & `angr-9.2.97/angr/procedures/definitions/win32_hlink.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_hrtfapo.py` & `angr-9.2.97/angr/procedures/definitions/win32_hrtfapo.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_httpapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_httpapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_icm32.py` & `angr-9.2.97/angr/procedures/definitions/win32_icm32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_icmui.py` & `angr-9.2.97/angr/procedures/definitions/win32_icmui.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_icu.py` & `angr-9.2.97/angr/procedures/definitions/win32_icu.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_ieframe.py` & `angr-9.2.97/angr/procedures/definitions/win32_ieframe.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_imagehlp.py` & `angr-9.2.97/angr/procedures/definitions/win32_imagehlp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_imgutil.py` & `angr-9.2.97/angr/procedures/definitions/win32_imgutil.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_imm32.py` & `angr-9.2.97/angr/procedures/definitions/win32_imm32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_infocardapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_infocardapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_inkobjcore.py` & `angr-9.2.97/angr/procedures/definitions/win32_inkobjcore.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_iphlpapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_iphlpapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_iscsidsc.py` & `angr-9.2.97/angr/procedures/definitions/win32_iscsidsc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_isolatedwindowsenvironmentutils.py` & `angr-9.2.97/angr/procedures/definitions/win32_isolatedwindowsenvironmentutils.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_kernel32.py` & `angr-9.2.97/angr/procedures/definitions/win32_kernel32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_kernelbase.py` & `angr-9.2.97/angr/procedures/definitions/win32_kernelbase.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_keycredmgr.py` & `angr-9.2.97/angr/procedures/definitions/win32_keycredmgr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_ksproxy_ax.py` & `angr-9.2.97/angr/procedures/definitions/win32_ksproxy_ax.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_ksuser.py` & `angr-9.2.97/angr/procedures/definitions/win32_ksuser.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_ktmw32.py` & `angr-9.2.97/angr/procedures/definitions/win32_ktmw32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_licenseprotection.py` & `angr-9.2.97/angr/procedures/definitions/win32_licenseprotection.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_loadperf.py` & `angr-9.2.97/angr/procedures/definitions/win32_loadperf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_magnification.py` & `angr-9.2.97/angr/procedures/definitions/win32_magnification.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mapi32.py` & `angr-9.2.97/angr/procedures/definitions/win32_mapi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mdmlocalmanagement.py` & `angr-9.2.97/angr/procedures/definitions/win32_mdmlocalmanagement.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mdmregistration.py` & `angr-9.2.97/angr/procedures/definitions/win32_mdmregistration.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mf.py` & `angr-9.2.97/angr/procedures/definitions/win32_mf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mfcore.py` & `angr-9.2.97/angr/procedures/definitions/win32_mfcore.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mfplat.py` & `angr-9.2.97/angr/procedures/definitions/win32_mfplat.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mfplay.py` & `angr-9.2.97/angr/procedures/definitions/win32_mfplay.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mfreadwrite.py` & `angr-9.2.97/angr/procedures/definitions/win32_mfreadwrite.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mfsensorgroup.py` & `angr-9.2.97/angr/procedures/definitions/win32_mfsensorgroup.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mfsrcsnk.py` & `angr-9.2.97/angr/procedures/definitions/win32_mfsrcsnk.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mgmtapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_mgmtapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mi.py` & `angr-9.2.97/angr/procedures/definitions/win32_mi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mmdevapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_mmdevapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mpr.py` & `angr-9.2.97/angr/procedures/definitions/win32_mpr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mprapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_mprapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mqrt.py` & `angr-9.2.97/angr/procedures/definitions/win32_mqrt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mrmsupport.py` & `angr-9.2.97/angr/procedures/definitions/win32_mrmsupport.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_msacm32.py` & `angr-9.2.97/angr/procedures/definitions/win32_msacm32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_msajapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_msajapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mscms.py` & `angr-9.2.97/angr/procedures/definitions/win32_mscms.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mscoree.py` & `angr-9.2.97/angr/procedures/definitions/win32_mscoree.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_msctfmonitor.py` & `angr-9.2.97/angr/procedures/definitions/win32_msctfmonitor.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_msdelta.py` & `angr-9.2.97/angr/procedures/definitions/win32_msdelta.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_msdmo.py` & `angr-9.2.97/angr/procedures/definitions/win32_msdmo.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_msdrm.py` & `angr-9.2.97/angr/procedures/definitions/win32_msdrm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_msi.py` & `angr-9.2.97/angr/procedures/definitions/win32_msi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_msimg32.py` & `angr-9.2.97/angr/procedures/definitions/win32_msimg32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mspatcha.py` & `angr-9.2.97/angr/procedures/definitions/win32_mspatcha.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mspatchc.py` & `angr-9.2.97/angr/procedures/definitions/win32_mspatchc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_msports.py` & `angr-9.2.97/angr/procedures/definitions/win32_msports.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_msrating.py` & `angr-9.2.97/angr/procedures/definitions/win32_msrating.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mssign32.py` & `angr-9.2.97/angr/procedures/definitions/win32_mssign32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mstask.py` & `angr-9.2.97/angr/procedures/definitions/win32_mstask.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_msvfw32.py` & `angr-9.2.97/angr/procedures/definitions/win32_msvfw32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mswsock.py` & `angr-9.2.97/angr/procedures/definitions/win32_mswsock.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_mtxdm.py` & `angr-9.2.97/angr/procedures/definitions/win32_mtxdm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_ncrypt.py` & `angr-9.2.97/angr/procedures/definitions/win32_ncrypt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_ndfapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_ndfapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_netapi32.py` & `angr-9.2.97/angr/procedures/definitions/win32_netapi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_netsh.py` & `angr-9.2.97/angr/procedures/definitions/win32_netsh.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_netshell.py` & `angr-9.2.97/angr/procedures/definitions/win32_netshell.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_newdev.py` & `angr-9.2.97/angr/procedures/definitions/win32_newdev.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_ninput.py` & `angr-9.2.97/angr/procedures/definitions/win32_ninput.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_normaliz.py` & `angr-9.2.97/angr/procedures/definitions/win32_normaliz.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_ntdll.py` & `angr-9.2.97/angr/procedures/definitions/win32_ntdll.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_ntdllk.py` & `angr-9.2.97/angr/procedures/definitions/win32_ntdllk.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_ntdsapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_ntdsapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_ntlanman.py` & `angr-9.2.97/angr/procedures/definitions/win32_ntlanman.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_odbc32.py` & `angr-9.2.97/angr/procedures/definitions/win32_odbc32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_odbcbcp.py` & `angr-9.2.97/angr/procedures/definitions/win32_odbcbcp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_ole32.py` & `angr-9.2.97/angr/procedures/definitions/win32_ole32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_oleacc.py` & `angr-9.2.97/angr/procedures/definitions/win32_oleacc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_oleaut32.py` & `angr-9.2.97/angr/procedures/definitions/win32_oleaut32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_oledlg.py` & `angr-9.2.97/angr/procedures/definitions/win32_oledlg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_ondemandconnroutehelper.py` & `angr-9.2.97/angr/procedures/definitions/win32_ondemandconnroutehelper.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_opengl32.py` & `angr-9.2.97/angr/procedures/definitions/win32_opengl32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_opmxbox.py` & `angr-9.2.97/angr/procedures/definitions/win32_opmxbox.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_p2p.py` & `angr-9.2.97/angr/procedures/definitions/win32_p2p.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_p2pgraph.py` & `angr-9.2.97/angr/procedures/definitions/win32_p2pgraph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_pdh.py` & `angr-9.2.97/angr/procedures/definitions/win32_pdh.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_peerdist.py` & `angr-9.2.97/angr/procedures/definitions/win32_peerdist.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_powrprof.py` & `angr-9.2.97/angr/procedures/definitions/win32_powrprof.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_prntvpt.py` & `angr-9.2.97/angr/procedures/definitions/win32_prntvpt.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_projectedfslib.py` & `angr-9.2.97/angr/procedures/definitions/win32_projectedfslib.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_propsys.py` & `angr-9.2.97/angr/procedures/definitions/win32_propsys.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_psapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_psapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_quartz.py` & `angr-9.2.97/angr/procedures/definitions/win32_quartz.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_query.py` & `angr-9.2.97/angr/procedures/definitions/win32_query.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_qwave.py` & `angr-9.2.97/angr/procedures/definitions/win32_qwave.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_rasapi32.py` & `angr-9.2.97/angr/procedures/definitions/win32_rasapi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_rasdlg.py` & `angr-9.2.97/angr/procedures/definitions/win32_rasdlg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_resutils.py` & `angr-9.2.97/angr/procedures/definitions/win32_resutils.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_rometadata.py` & `angr-9.2.97/angr/procedures/definitions/win32_rometadata.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_rpcns4.py` & `angr-9.2.97/angr/procedures/definitions/win32_rpcns4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_rpcproxy.py` & `angr-9.2.97/angr/procedures/definitions/win32_rpcproxy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_rpcrt4.py` & `angr-9.2.97/angr/procedures/definitions/win32_rpcrt4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_rstrtmgr.py` & `angr-9.2.97/angr/procedures/definitions/win32_rstrtmgr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_rtm.py` & `angr-9.2.97/angr/procedures/definitions/win32_rtm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_rtutils.py` & `angr-9.2.97/angr/procedures/definitions/win32_rtutils.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_rtworkq.py` & `angr-9.2.97/angr/procedures/definitions/win32_rtworkq.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_sas.py` & `angr-9.2.97/angr/procedures/definitions/win32_sas.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_scarddlg.py` & `angr-9.2.97/angr/procedures/definitions/win32_scarddlg.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_schannel.py` & `angr-9.2.97/angr/procedures/definitions/win32_schannel.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_sechost.py` & `angr-9.2.97/angr/procedures/definitions/win32_sechost.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_secur32.py` & `angr-9.2.97/angr/procedures/definitions/win32_secur32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_sensapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_sensapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_sensorsutilsv2.py` & `angr-9.2.97/angr/procedures/definitions/win32_sensorsutilsv2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_setupapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_setupapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_sfc.py` & `angr-9.2.97/angr/procedures/definitions/win32_sfc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_shdocvw.py` & `angr-9.2.97/angr/procedures/definitions/win32_shdocvw.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_shell32.py` & `angr-9.2.97/angr/procedures/definitions/win32_shell32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_shlwapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_shlwapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_slc.py` & `angr-9.2.97/angr/procedures/definitions/win32_slc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_slcext.py` & `angr-9.2.97/angr/procedures/definitions/win32_slcext.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_slwga.py` & `angr-9.2.97/angr/procedures/definitions/win32_slwga.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_snmpapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_snmpapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_spoolss.py` & `angr-9.2.97/angr/procedures/definitions/win32_spoolss.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_srclient.py` & `angr-9.2.97/angr/procedures/definitions/win32_srclient.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_srpapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_srpapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_sspicli.py` & `angr-9.2.97/angr/procedures/definitions/win32_sspicli.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_sti.py` & `angr-9.2.97/angr/procedures/definitions/win32_sti.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_t2embed.py` & `angr-9.2.97/angr/procedures/definitions/win32_t2embed.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_tapi32.py` & `angr-9.2.97/angr/procedures/definitions/win32_tapi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_tbs.py` & `angr-9.2.97/angr/procedures/definitions/win32_tbs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_tdh.py` & `angr-9.2.97/angr/procedures/definitions/win32_tdh.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_tokenbinding.py` & `angr-9.2.97/angr/procedures/definitions/win32_tokenbinding.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_traffic.py` & `angr-9.2.97/angr/procedures/definitions/win32_traffic.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_txfw32.py` & `angr-9.2.97/angr/procedures/definitions/win32_txfw32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_ualapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_ualapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_uiautomationcore.py` & `angr-9.2.97/angr/procedures/definitions/win32_uiautomationcore.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_urlmon.py` & `angr-9.2.97/angr/procedures/definitions/win32_urlmon.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_user32.py` & `angr-9.2.97/angr/procedures/definitions/win32_user32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_userenv.py` & `angr-9.2.97/angr/procedures/definitions/win32_userenv.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_usp10.py` & `angr-9.2.97/angr/procedures/definitions/win32_usp10.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_uxtheme.py` & `angr-9.2.97/angr/procedures/definitions/win32_uxtheme.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_verifier.py` & `angr-9.2.97/angr/procedures/definitions/win32_verifier.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_version.py` & `angr-9.2.97/angr/procedures/definitions/win32_version.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_vertdll.py` & `angr-9.2.97/angr/procedures/definitions/win32_vertdll.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_virtdisk.py` & `angr-9.2.97/angr/procedures/definitions/win32_virtdisk.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_vmdevicehost.py` & `angr-9.2.97/angr/procedures/definitions/win32_vmdevicehost.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_vmsavedstatedumpprovider.py` & `angr-9.2.97/angr/procedures/definitions/win32_vmsavedstatedumpprovider.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_vssapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_vssapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wcmapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_wcmapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wdsbp.py` & `angr-9.2.97/angr/procedures/definitions/win32_wdsbp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wdsclientapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_wdsclientapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wdsmc.py` & `angr-9.2.97/angr/procedures/definitions/win32_wdsmc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wdspxe.py` & `angr-9.2.97/angr/procedures/definitions/win32_wdspxe.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wdstptc.py` & `angr-9.2.97/angr/procedures/definitions/win32_wdstptc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_webauthn.py` & `angr-9.2.97/angr/procedures/definitions/win32_webauthn.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_webservices.py` & `angr-9.2.97/angr/procedures/definitions/win32_webservices.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_websocket.py` & `angr-9.2.97/angr/procedures/definitions/win32_websocket.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wecapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_wecapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wer.py` & `angr-9.2.97/angr/procedures/definitions/win32_wer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wevtapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_wevtapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_winbio.py` & `angr-9.2.97/angr/procedures/definitions/win32_winbio.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_windows_ai_machinelearning.py` & `angr-9.2.97/angr/procedures/definitions/win32_windows_ai_machinelearning.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_windows_data_pdf.py` & `angr-9.2.97/angr/procedures/definitions/win32_windows_data_pdf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_windows_media_mediacontrol.py` & `angr-9.2.97/angr/procedures/definitions/win32_windows_media_mediacontrol.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_windows_networking.py` & `angr-9.2.97/angr/procedures/definitions/win32_windows_networking.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_windows_ui_xaml.py` & `angr-9.2.97/angr/procedures/definitions/win32_windows_ui_xaml.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_windowscodecs.py` & `angr-9.2.97/angr/procedures/definitions/win32_windowscodecs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_winfax.py` & `angr-9.2.97/angr/procedures/definitions/win32_winfax.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_winhttp.py` & `angr-9.2.97/angr/procedures/definitions/win32_winhttp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_winhvemulation.py` & `angr-9.2.97/angr/procedures/definitions/win32_winhvemulation.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_winhvplatform.py` & `angr-9.2.97/angr/procedures/definitions/win32_winhvplatform.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wininet.py` & `angr-9.2.97/angr/procedures/definitions/win32_wininet.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_winml.py` & `angr-9.2.97/angr/procedures/definitions/win32_winml.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_winmm.py` & `angr-9.2.97/angr/procedures/definitions/win32_winmm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_winscard.py` & `angr-9.2.97/angr/procedures/definitions/win32_winscard.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_winspool.py` & `angr-9.2.97/angr/procedures/definitions/win32_winspool.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_winspool_drv.py` & `angr-9.2.97/angr/procedures/definitions/win32_winspool_drv.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wintrust.py` & `angr-9.2.97/angr/procedures/definitions/win32_wintrust.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_winusb.py` & `angr-9.2.97/angr/procedures/definitions/win32_winusb.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wlanapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_wlanapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wlanui.py` & `angr-9.2.97/angr/procedures/definitions/win32_wlanui.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wldap32.py` & `angr-9.2.97/angr/procedures/definitions/win32_wldap32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wldp.py` & `angr-9.2.97/angr/procedures/definitions/win32_wldp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wmvcore.py` & `angr-9.2.97/angr/procedures/definitions/win32_wmvcore.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wnvapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_wnvapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wofutil.py` & `angr-9.2.97/angr/procedures/definitions/win32_wofutil.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_ws2_32.py` & `angr-9.2.97/angr/procedures/definitions/win32_ws2_32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wscapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_wscapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wsclient.py` & `angr-9.2.97/angr/procedures/definitions/win32_wsclient.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wsdapi.py` & `angr-9.2.97/angr/procedures/definitions/win32_wsdapi.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wsmsvc.py` & `angr-9.2.97/angr/procedures/definitions/win32_wsmsvc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wsnmp32.py` & `angr-9.2.97/angr/procedures/definitions/win32_wsnmp32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_wtsapi32.py` & `angr-9.2.97/angr/procedures/definitions/win32_wtsapi32.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_xaudio2_8.py` & `angr-9.2.97/angr/procedures/definitions/win32_xaudio2_8.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_xinput1_4.py` & `angr-9.2.97/angr/procedures/definitions/win32_xinput1_4.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_xinputuap.py` & `angr-9.2.97/angr/procedures/definitions/win32_xinputuap.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_xmllite.py` & `angr-9.2.97/angr/procedures/definitions/win32_xmllite.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_xolehlp.py` & `angr-9.2.97/angr/procedures/definitions/win32_xolehlp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/definitions/win32_xpsprint.py` & `angr-9.2.97/angr/procedures/definitions/win32_xpsprint.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/glibc/__ctype_b_loc.py` & `angr-9.2.97/angr/procedures/glibc/__ctype_b_loc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/glibc/__ctype_tolower_loc.py` & `angr-9.2.97/angr/procedures/glibc/__ctype_tolower_loc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/glibc/__ctype_toupper_loc.py` & `angr-9.2.97/angr/procedures/glibc/__ctype_toupper_loc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/glibc/__libc_init.py` & `angr-9.2.97/angr/procedures/glibc/__libc_init.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/glibc/__libc_start_main.py` & `angr-9.2.97/angr/procedures/glibc/__libc_start_main.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/glibc/dynamic_loading.py` & `angr-9.2.97/angr/procedures/glibc/dynamic_loading.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java/__init__.py` & `angr-9.2.97/angr/procedures/java/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java/unconstrained.py` & `angr-9.2.97/angr/procedures/java/unconstrained.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java_io/write.py` & `angr-9.2.97/angr/procedures/java_io/write.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java_jni/__init__.py` & `angr-9.2.97/angr/procedures/java_jni/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java_jni/array_operations.py` & `angr-9.2.97/angr/procedures/java_jni/array_operations.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java_jni/class_and_interface_operations.py` & `angr-9.2.97/angr/procedures/java_jni/class_and_interface_operations.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java_jni/field_access.py` & `angr-9.2.97/angr/procedures/java_jni/field_access.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java_jni/global_and_local_refs.py` & `angr-9.2.97/angr/procedures/java_jni/global_and_local_refs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java_jni/method_calls.py` & `angr-9.2.97/angr/procedures/java_jni/method_calls.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java_jni/not_implemented.py` & `angr-9.2.97/angr/procedures/java_jni/not_implemented.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java_jni/object_operations.py` & `angr-9.2.97/angr/procedures/java_jni/object_operations.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java_jni/string_operations.py` & `angr-9.2.97/angr/procedures/java_jni/string_operations.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java_lang/character.py` & `angr-9.2.97/angr/procedures/java_lang/character.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java_lang/double.py` & `angr-9.2.97/angr/procedures/java_lang/double.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java_lang/integer.py` & `angr-9.2.97/angr/procedures/java_lang/integer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java_lang/string.py` & `angr-9.2.97/angr/procedures/java_lang/string.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java_lang/stringbuilder.py` & `angr-9.2.97/angr/procedures/java_lang/stringbuilder.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java_util/collection.py` & `angr-9.2.97/angr/procedures/java_util/collection.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java_util/iterator.py` & `angr-9.2.97/angr/procedures/java_util/iterator.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java_util/list.py` & `angr-9.2.97/angr/procedures/java_util/list.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java_util/map.py` & `angr-9.2.97/angr/procedures/java_util/map.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/java_util/scanner_nextline.py` & `angr-9.2.97/angr/procedures/java_util/scanner_nextline.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/error.py` & `angr-9.2.97/angr/procedures/libc/error.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/fclose.py` & `angr-9.2.97/angr/procedures/libc/fclose.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/feof.py` & `angr-9.2.97/angr/procedures/libc/feof.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/fgetc.py` & `angr-9.2.97/angr/procedures/libc/fgetc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/fgets.py` & `angr-9.2.97/angr/procedures/libc/fgets.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/fopen.py` & `angr-9.2.97/angr/procedures/libc/fopen.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/fprintf.py` & `angr-9.2.97/angr/procedures/libc/fprintf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/fputc.py` & `angr-9.2.97/angr/procedures/libc/fputc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/fputs.py` & `angr-9.2.97/angr/procedures/libc/fputs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/fread.py` & `angr-9.2.97/angr/procedures/libc/fread.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/fscanf.py` & `angr-9.2.97/angr/procedures/libc/fscanf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/fseek.py` & `angr-9.2.97/angr/procedures/libc/fseek.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/ftell.py` & `angr-9.2.97/angr/procedures/libc/ftell.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/getdelim.py` & `angr-9.2.97/angr/procedures/libc/getdelim.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/gets.py` & `angr-9.2.97/angr/procedures/libc/gets.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/memcmp.py` & `angr-9.2.97/angr/procedures/libc/memcmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/memcpy.py` & `angr-9.2.97/angr/procedures/libc/memcpy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/memset.py` & `angr-9.2.97/angr/procedures/libc/memset.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/printf.py` & `angr-9.2.97/angr/procedures/libc/printf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/scanf.py` & `angr-9.2.97/angr/procedures/libc/scanf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/snprintf.py` & `angr-9.2.97/angr/procedures/libc/snprintf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/sprintf.py` & `angr-9.2.97/angr/procedures/libc/sprintf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/strchr.py` & `angr-9.2.97/angr/procedures/libc/strchr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/strcmp.py` & `angr-9.2.97/angr/procedures/libc/strcmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/strlen.py` & `angr-9.2.97/angr/procedures/libc/strlen.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/strncmp.py` & `angr-9.2.97/angr/procedures/libc/strncmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/strncpy.py` & `angr-9.2.97/angr/procedures/libc/strncpy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/strstr.py` & `angr-9.2.97/angr/procedures/libc/strstr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/strtol.py` & `angr-9.2.97/angr/procedures/libc/strtol.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/tmpnam.py` & `angr-9.2.97/angr/procedures/libc/tmpnam.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/ungetc.py` & `angr-9.2.97/angr/procedures/libc/ungetc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/libc/wchar.py` & `angr-9.2.97/angr/procedures/libc/wchar.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_kernel/access.py` & `angr-9.2.97/angr/procedures/linux_kernel/access.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_kernel/arch_prctl.py` & `angr-9.2.97/angr/procedures/linux_kernel/arch_prctl.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_kernel/arm_user_helpers.py` & `angr-9.2.97/angr/procedures/linux_kernel/arm_user_helpers.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_kernel/cwd.py` & `angr-9.2.97/angr/procedures/linux_kernel/cwd.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_kernel/fstat.py` & `angr-9.2.97/angr/procedures/linux_kernel/fstat.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_kernel/fstat64.py` & `angr-9.2.97/angr/procedures/linux_kernel/fstat64.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_kernel/futex.py` & `angr-9.2.97/angr/procedures/linux_kernel/futex.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_kernel/getrlimit.py` & `angr-9.2.97/angr/procedures/linux_kernel/getrlimit.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_kernel/iovec.py` & `angr-9.2.97/angr/procedures/linux_kernel/iovec.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_kernel/lseek.py` & `angr-9.2.97/angr/procedures/linux_kernel/lseek.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_kernel/mprotect.py` & `angr-9.2.97/angr/procedures/linux_kernel/mprotect.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_kernel/openat.py` & `angr-9.2.97/angr/procedures/linux_kernel/openat.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_kernel/sigaction.py` & `angr-9.2.97/angr/procedures/linux_kernel/sigaction.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_kernel/sigprocmask.py` & `angr-9.2.97/angr/procedures/linux_kernel/sigprocmask.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_kernel/stat.py` & `angr-9.2.97/angr/procedures/linux_kernel/stat.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_kernel/sysinfo.py` & `angr-9.2.97/angr/procedures/linux_kernel/sysinfo.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_kernel/time.py` & `angr-9.2.97/angr/procedures/linux_kernel/time.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_kernel/uid.py` & `angr-9.2.97/angr/procedures/linux_kernel/uid.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_kernel/uname.py` & `angr-9.2.97/angr/procedures/linux_kernel/uname.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_kernel/unlink.py` & `angr-9.2.97/angr/procedures/linux_kernel/unlink.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_loader/sim_loader.py` & `angr-9.2.97/angr/procedures/linux_loader/sim_loader.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/linux_loader/tls.py` & `angr-9.2.97/angr/procedures/linux_loader/tls.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/msvcr/__getmainargs.py` & `angr-9.2.97/angr/procedures/msvcr/__getmainargs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/msvcr/_initterm.py` & `angr-9.2.97/angr/procedures/msvcr/_initterm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/msvcr/fmode.py` & `angr-9.2.97/angr/procedures/msvcr/fmode.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/ntdll/exceptions.py` & `angr-9.2.97/angr/procedures/ntdll/exceptions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/posix/accept.py` & `angr-9.2.97/angr/procedures/posix/accept.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/posix/chroot.py` & `angr-9.2.97/angr/procedures/posix/chroot.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/posix/dup.py` & `angr-9.2.97/angr/procedures/posix/dup.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/posix/fdopen.py` & `angr-9.2.97/angr/procedures/posix/fdopen.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/posix/getenv.py` & `angr-9.2.97/angr/procedures/posix/getenv.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/posix/gethostbyname.py` & `angr-9.2.97/angr/procedures/posix/gethostbyname.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/posix/inet_ntoa.py` & `angr-9.2.97/angr/procedures/posix/inet_ntoa.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/posix/mmap.py` & `angr-9.2.97/angr/procedures/posix/mmap.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/posix/open.py` & `angr-9.2.97/angr/procedures/posix/open.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/posix/poll.py` & `angr-9.2.97/angr/procedures/posix/poll.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/posix/pread64.py` & `angr-9.2.97/angr/procedures/posix/pread64.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/posix/pthread.py` & `angr-9.2.97/angr/procedures/posix/pthread.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/posix/pwrite64.py` & `angr-9.2.97/angr/procedures/posix/pwrite64.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/posix/readdir.py` & `angr-9.2.97/angr/procedures/posix/readdir.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/posix/select.py` & `angr-9.2.97/angr/procedures/posix/select.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/posix/send.py` & `angr-9.2.97/angr/procedures/posix/send.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/posix/sigaction.py` & `angr-9.2.97/angr/procedures/posix/sigaction.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/posix/sim_time.py` & `angr-9.2.97/angr/procedures/posix/sim_time.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/posix/socket.py` & `angr-9.2.97/angr/procedures/posix/socket.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/posix/strcasecmp.py` & `angr-9.2.97/angr/procedures/posix/strcasecmp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/posix/strtok_r.py` & `angr-9.2.97/angr/procedures/posix/strtok_r.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/procedure_dict.py` & `angr-9.2.97/angr/procedures/procedure_dict.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/stubs/ReturnUnconstrained.py` & `angr-9.2.97/angr/procedures/stubs/ReturnUnconstrained.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/stubs/UserHook.py` & `angr-9.2.97/angr/procedures/stubs/UserHook.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/stubs/crazy_scanf.py` & `angr-9.2.97/angr/procedures/stubs/crazy_scanf.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/stubs/format_parser.py` & `angr-9.2.97/angr/procedures/stubs/format_parser.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/stubs/syscall_stub.py` & `angr-9.2.97/angr/procedures/stubs/syscall_stub.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/tracer/receive.py` & `angr-9.2.97/angr/procedures/tracer/receive.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/tracer/transmit.py` & `angr-9.2.97/angr/procedures/tracer/transmit.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/win32/GetLastInputInfo.py` & `angr-9.2.97/angr/procedures/win32/GetLastInputInfo.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/win32/GetModuleHandle.py` & `angr-9.2.97/angr/procedures/win32/GetModuleHandle.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/win32/GetProcessAffinityMask.py` & `angr-9.2.97/angr/procedures/win32/GetProcessAffinityMask.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/win32/InterlockedExchange.py` & `angr-9.2.97/angr/procedures/win32/InterlockedExchange.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/win32/VirtualAlloc.py` & `angr-9.2.97/angr/procedures/win32/VirtualAlloc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/win32/VirtualProtect.py` & `angr-9.2.97/angr/procedures/win32/VirtualProtect.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/win32/dynamic_loading.py` & `angr-9.2.97/angr/procedures/win32/dynamic_loading.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/win32/file_handles.py` & `angr-9.2.97/angr/procedures/win32/file_handles.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/win32/heap.py` & `angr-9.2.97/angr/procedures/win32/heap.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/win32/is_bad_ptr.py` & `angr-9.2.97/angr/procedures/win32/is_bad_ptr.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/win32/local_storage.py` & `angr-9.2.97/angr/procedures/win32/local_storage.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/win32/sim_time.py` & `angr-9.2.97/angr/procedures/win32/sim_time.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/win32/system_paths.py` & `angr-9.2.97/angr/procedures/win32/system_paths.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/procedures/win_user32/messagebox.py` & `angr-9.2.97/angr/procedures/win_user32/messagebox.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/project.py` & `angr-9.2.97/angr/project.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/protos/cfg_pb2.py` & `angr-9.2.97/angr/protos/cfg_pb2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/protos/function_pb2.py` & `angr-9.2.97/angr/protos/function_pb2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/protos/primitives_pb2.py` & `angr-9.2.97/angr/protos/primitives_pb2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/protos/variables_pb2.py` & `angr-9.2.97/angr/protos/variables_pb2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/protos/xrefs_pb2.py` & `angr-9.2.97/angr/protos/xrefs_pb2.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/serializable.py` & `angr-9.2.97/angr/serializable.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/service.py` & `angr-9.2.97/angr/service.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/sim_manager.py` & `angr-9.2.97/angr/sim_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/sim_options.py` & `angr-9.2.97/angr/sim_options.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/sim_procedure.py` & `angr-9.2.97/angr/sim_procedure.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/sim_state.py` & `angr-9.2.97/angr/sim_state.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/sim_state_options.py` & `angr-9.2.97/angr/sim_state_options.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/sim_type.py` & `angr-9.2.97/angr/sim_type.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/sim_variable.py` & `angr-9.2.97/angr/sim_variable.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/simos/__init__.py` & `angr-9.2.97/angr/simos/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/simos/cgc.py` & `angr-9.2.97/angr/simos/cgc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/simos/javavm.py` & `angr-9.2.97/angr/simos/javavm.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/simos/linux.py` & `angr-9.2.97/angr/simos/linux.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/simos/simos.py` & `angr-9.2.97/angr/simos/simos.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,14 +273,16 @@
         else:
             state = state.copy()
             state.regs.ip = addr
         cc.setup_callsite(state, ret_addr, args, prototype, stack_base, alloc_base, grow_like_stack)
 
         if state.arch.name == "PPC64" and toc is not None:
             state.regs.r2 = toc
+        elif state.arch.name in ("MIPS32", "MIPS64"):
+            state.regs.t9 = addr
 
         return state
 
     def prepare_call_state(self, calling_state, initial_state=None, preserve_registers=(), preserve_memory=()):
         """
         This function prepares a state that is executing a call instruction.
         If given an initial_state, it copies over all of the critical registers to it from the
```

### Comparing `angr-9.2.96/angr/simos/snimmuc_nxp.py` & `angr-9.2.97/angr/simos/snimmuc_nxp.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/simos/userland.py` & `angr-9.2.97/angr/simos/userland.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/simos/windows.py` & `angr-9.2.97/angr/simos/windows.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/slicer.py` & `angr-9.2.97/angr/slicer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_hierarchy.py` & `angr-9.2.97/angr/state_hierarchy.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/__init__.py` & `angr-9.2.97/angr/state_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/callstack.py` & `angr-9.2.97/angr/state_plugins/callstack.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/cgc.py` & `angr-9.2.97/angr/state_plugins/cgc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/concrete.py` & `angr-9.2.97/angr/state_plugins/concrete.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/debug_variables.py` & `angr-9.2.97/angr/state_plugins/debug_variables.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/filesystem.py` & `angr-9.2.97/angr/state_plugins/filesystem.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/gdb.py` & `angr-9.2.97/angr/state_plugins/gdb.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/globals.py` & `angr-9.2.97/angr/state_plugins/globals.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/heap/heap_base.py` & `angr-9.2.97/angr/state_plugins/heap/heap_base.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/heap/heap_brk.py` & `angr-9.2.97/angr/state_plugins/heap/heap_brk.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/heap/heap_freelist.py` & `angr-9.2.97/angr/state_plugins/heap/heap_freelist.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/heap/heap_libc.py` & `angr-9.2.97/angr/state_plugins/heap/heap_libc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/heap/heap_ptmalloc.py` & `angr-9.2.97/angr/state_plugins/heap/heap_ptmalloc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/heap/utils.py` & `angr-9.2.97/angr/state_plugins/heap/utils.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/history.py` & `angr-9.2.97/angr/state_plugins/history.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/inspect.py` & `angr-9.2.97/angr/state_plugins/inspect.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/javavm_classloader.py` & `angr-9.2.97/angr/state_plugins/javavm_classloader.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/jni_references.py` & `angr-9.2.97/angr/state_plugins/jni_references.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/libc.py` & `angr-9.2.97/angr/state_plugins/libc.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/light_registers.py` & `angr-9.2.97/angr/state_plugins/light_registers.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/log.py` & `angr-9.2.97/angr/state_plugins/log.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/loop_data.py` & `angr-9.2.97/angr/state_plugins/loop_data.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/plugin.py` & `angr-9.2.97/angr/state_plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/posix.py` & `angr-9.2.97/angr/state_plugins/posix.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/preconstrainer.py` & `angr-9.2.97/angr/state_plugins/preconstrainer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/scratch.py` & `angr-9.2.97/angr/state_plugins/scratch.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/sim_action.py` & `angr-9.2.97/angr/state_plugins/sim_action.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/sim_action_object.py` & `angr-9.2.97/angr/state_plugins/sim_action_object.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/sim_event.py` & `angr-9.2.97/angr/state_plugins/sim_event.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/solver.py` & `angr-9.2.97/angr/state_plugins/solver.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/symbolizer.py` & `angr-9.2.97/angr/state_plugins/symbolizer.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/trace_additions.py` & `angr-9.2.97/angr/state_plugins/trace_additions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/uc_manager.py` & `angr-9.2.97/angr/state_plugins/uc_manager.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/unicorn_engine.py` & `angr-9.2.97/angr/state_plugins/unicorn_engine.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/state_plugins/view.py` & `angr-9.2.97/angr/state_plugins/view.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/file.py` & `angr-9.2.97/angr/storage/file.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/__init__.py` & `angr-9.2.97/angr/storage/memory_mixins/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,17 @@
 
     def store(self, addr, data, **kwargs):
         pass
 
     def merge(self, others, merge_conditions, common_ancestor=None) -> bool:
         pass
 
+    def compare(self, other) -> bool:
+        pass
+
     def widen(self, others):
         pass
 
     def permissions(self, addr, permissions=None, **kwargs):
         pass
 
     def map_region(self, addr, length, permissions, init_zero=False, **kwargs):
```

### Comparing `angr-9.2.96/angr/storage/memory_mixins/__init__.pyi` & `angr-9.2.97/angr/storage/memory_mixins/__init__.pyi`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/actions_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/actions_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/address_concretization_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/address_concretization_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/bvv_conversion_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/bvv_conversion_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/clouseau_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/clouseau_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/conditional_store_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/conditional_store_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/convenient_mappings_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/convenient_mappings_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/default_filler_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/default_filler_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/hex_dumper_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/hex_dumper_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/javavm_memory/javavm_memory_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/javavm_memory/javavm_memory_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/keyvalue_memory/keyvalue_memory_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/keyvalue_memory/keyvalue_memory_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/label_merger_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/label_merger_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/multi_value_merger_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/multi_value_merger_mixin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,67 @@
+# pylint:disable=missing-class-docstring
 from typing import Iterable, Tuple, Any, Callable, Optional
 
 from . import MemoryMixin
 
 
 class MultiValueMergerMixin(MemoryMixin):
-    def __init__(self, *args, element_limit=5, annotation_limit=256, top_func=None, phi_maker=None, **kwargs):
+    def __init__(
+        self, *args, element_limit=5, annotation_limit=256, top_func=None, is_top_func=None, phi_maker=None, **kwargs
+    ):
         self._element_limit = element_limit
         self._annotation_limit = annotation_limit
         self._top_func: Callable = top_func
+        self._is_top_func: Callable = is_top_func
         self._phi_maker: Optional[Callable] = phi_maker
 
         super().__init__(*args, **kwargs)
 
     def _merge_values(self, values: Iterable[Tuple[Any, Any]], merged_size: int, **kwargs):
         values_set = {v for v, _ in values}
         if self._phi_maker is not None:
             phi_var = self._phi_maker(values_set)
             if phi_var is not None:
                 return {phi_var}
 
         # try to merge it in the traditional way
-        if len(values_set) > self._element_limit:
-            # strip annotations from each value and see how many raw values there are in total
-            # We have to use cache_key to determine uniqueness here, because if __hash__ collides,
-            # python implicitly calls __eq__ to determine if the two objects are actually the same
-            # and that just results in a new AST for a BV. Python then tries to convert that AST to a bool
-            # which fails with the safeguard in claripy.ast.bool.Bool.__bool__.
-            stripped_values_set = {v._apply_to_annotations(lambda alist: None).cache_key for v in values_set}
-            if len(stripped_values_set) > 1:
+        has_top = any(self._is_top_func(v) for v in values_set)
+        if has_top or len(values_set) > self._element_limit:
+            if has_top:
                 ret_val = self._top_func(merged_size * self.state.arch.byte_width)
             else:
-                # Get the AST back from the cache_key
-                ret_val = next(iter(stripped_values_set)).ast
+                # strip annotations from each value and see how many raw values there are in total
+                # We have to use cache_key to determine uniqueness here, because if __hash__ collides,
+                # python implicitly calls __eq__ to determine if the two objects are actually the same
+                # and that just results in a new AST for a BV. Python then tries to convert that AST to a bool
+                # which fails with the safeguard in claripy.ast.bool.Bool.__bool__.
+                stripped_values_set = {v._apply_to_annotations(lambda alist: None).cache_key for v in values_set}
+                if len(stripped_values_set) > 1:
+                    ret_val = self._top_func(merged_size * self.state.arch.byte_width)
+                else:
+                    # Get the AST back from the cache_key
+                    ret_val = next(iter(stripped_values_set)).ast
+
             # migrate annotations
             annotations = []
             annotations_set = set()
             for v in values_set:
                 for anno in v.annotations:
                     if anno not in annotations_set:
                         annotations.append(anno)
                         annotations_set.add(anno)
             if annotations:
+                annotations = sorted(annotations, key=str)
                 ret_val = ret_val.annotate(*annotations[: self._annotation_limit])
             merged_val = {ret_val}
         else:
             merged_val = values_set
         return merged_val
 
     def copy(self, memo=None):
         copied = super().copy(memo)
         copied._element_limit = self._element_limit
         copied._annotation_limit = self._annotation_limit
         copied._top_func = self._top_func
+        copied._is_top_func = self._is_top_func
         copied._phi_maker = self._phi_maker
         return copied
```

### Comparing `angr-9.2.96/angr/storage/memory_mixins/name_resolution_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/name_resolution_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/paged_memory/page_backer_mixins.py` & `angr-9.2.97/angr/storage/memory_mixins/paged_memory/page_backer_mixins.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/paged_memory/paged_memory_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/paged_memory/paged_memory_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,14 +290,32 @@
                 other_pages, merge_conditions, page_addr=page_addr, memory=self, changed_offsets=changed_offsets
             )
             for off in merged_offsets:
                 merged_bytes.add(page_addr + off)
 
         return bool(merged_bytes)
 
+    def compare(self, other: "PagedMemoryMixin") -> bool:
+        changed_pages_and_offsets: Dict[int, Optional[Set[int]]] = dict(self.changed_pages(other))
+
+        for page_no in sorted(changed_pages_and_offsets):
+            page = self._get_page(page_no, False)
+            page_addr = page_no * self.page_size
+            if page_no in other._pages:
+                r = page.compare(
+                    other._pages[page_no],
+                    page_addr=page_addr,
+                    memory=self,
+                    changed_offsets=changed_pages_and_offsets[page_no],
+                )
+                if r is False:
+                    return False
+
+        return True
+
     def permissions(self, addr, permissions=None, **kwargs):
         if type(addr) is not int:
             raise TypeError("addr must be an int in paged memory")
         pageno, _ = self._divide_addr(addr)
         try:
             page = self._get_page(pageno, permissions is not None, allow_default=False, **kwargs)
         except SimMemoryError as e:
@@ -639,18 +657,18 @@
 class LabeledPagesMixin(PagedMemoryMixin):
     def load_with_labels(
         self, addr: int, size: int = None, endness=None, **kwargs
     ) -> Tuple[claripy.ast.Base, Tuple[Tuple[int, int, int, Any]]]:
         if endness is None:
             endness = self.endness
 
-        if type(size) is not int:
+        if not isinstance(size, int):
             raise TypeError("Need size to be resolved to an int by this point")
 
-        if type(addr) is not int:
+        if not isinstance(addr, int):
             raise TypeError("Need addr to be resolved to an int by this point")
 
         pageno, pageoff = self._divide_addr(addr)
         vals = []
 
         # fasttrack basic case
         if pageoff + size <= self.page_size:
```

### Comparing `angr-9.2.96/angr/storage/memory_mixins/paged_memory/paged_memory_multivalue_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/paged_memory/paged_memory_multivalue_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/paged_memory/pages/__init__.py` & `angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/paged_memory/pages/cooperation.py` & `angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/cooperation.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/paged_memory/pages/history_tracking_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/history_tracking_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/paged_memory/pages/ispo_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/ispo_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/paged_memory/pages/list_page.py` & `angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/list_page.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/paged_memory/pages/multi_values.py` & `angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/multi_values.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/paged_memory/pages/mv_list_page.py` & `angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/mv_list_page.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# pylint:disable=abstract-method,arguments-differ
+# pylint:disable=abstract-method,arguments-differ,assignment-from-no-return
 import logging
-from typing import Optional, List, Set, Tuple, Union, Callable
+from typing import Optional, List, Set, Tuple, Union, Callable, Any, FrozenSet
 
 from angr.utils.dynamic_dictlist import DynamicDictList
 from .....storage.memory_object import SimMemoryObject, SimLabeledMemoryObject
 from . import PageBase
 from .cooperation import MemoryObjectSetMixin
 
 
@@ -162,121 +162,158 @@
         merged_offsets = set()
         for b in sorted(changed_offsets):
             if merged_to is not None and not b >= merged_to:
                 l.info("merged_to = %d ... already merged byte 0x%x", merged_to, b)
                 continue
             l.debug("... on byte 0x%x", b)
 
-            memory_objects = []
+            memory_object_sets: Set[Tuple[FrozenSet[SimMemoryObject], Any]] = set()
             unconstrained_in = []
 
-            # first get a list of all memory objects at that location, and
-            # all memories that don't have those bytes
+            # first get a list of all memory objects at that location, and all memories that don't have those bytes
+            self_has_memory_object_set = False
             for sm, fv in zip(all_pages, merge_conditions):
                 if sm._contains(b, page_addr):
                     l.info("... present in %s", fv)
+                    memory_objects = set()
                     for mo in sm.content_gen(b):
                         if mo.includes(page_addr + b):
-                            memory_objects.append((mo, fv))
+                            memory_objects.add(mo)
+                    memory_object_sets.add((frozenset(memory_objects), fv))
+                    if sm is self:
+                        self_has_memory_object_set = True
                 else:
                     l.info("... not present in %s", fv)
                     unconstrained_in.append((sm, fv))
 
-            if not memory_objects:
+            if not memory_object_sets:
+                continue
+            if self_has_memory_object_set and len(memory_object_sets) == 1:
                 continue
 
-            mos = {mo for mo, _ in memory_objects}
-            mo_bases = {mo.base for mo, _ in memory_objects}
-            mo_lengths = {mo.length for mo, _ in memory_objects}
-            endnesses = {mo.endness for mo in mos}
+            mo_sets = {mo_set for mo_set, _ in memory_object_sets}
+            mo_bases = set()
+            mo_lengths = set()
+            endnesses = set()
+            for mo_set in mo_sets:
+                for mo in mo_set:
+                    mo_bases.add(mo.base)
+                    mo_lengths.add(mo.length)
+                    endnesses.add(mo.endness)
 
-            if not unconstrained_in and not (mos - merged_objects):  # pylint:disable=superfluous-parens
+            if not unconstrained_in and not (mo_sets - merged_objects):  # pylint:disable=superfluous-parens
                 continue
 
             # first, optimize the case where we are dealing with the same-sized memory objects
             if len(mo_bases) == 1 and len(mo_lengths) == 1 and not unconstrained_in and len(endnesses) == 1:
+                if len(memory_object_sets) == 1:
+                    # nothing to merge!
+                    continue
+
                 the_endness = next(iter(endnesses))
-                to_merge = [(mo.object, fv) for mo, fv in memory_objects]
+                to_merge = []
+                for mo_set, fv in memory_object_sets:
+                    for mo in mo_set:
+                        to_merge.append((mo.object, fv))
 
                 # Update `merged_to`
                 mo_base = list(mo_bases)[0]
-                mo_length = memory_objects[0][0].length
+                mo_length = next(iter(mo_lengths))
                 size = min(mo_length - (page_addr + b - mo_base), len(self.content) - b)
                 merged_to = b + size
 
                 merged_val = self._merge_values(to_merge, mo_length, memory=memory)
                 if merged_val is None:
                     # merge_values() determines that we should not attempt to merge this value
                     continue
 
                 # do the replacement
                 # TODO: Implement in-place replacement instead of calling store()
                 # new_object = self._replace_memory_object(our_mo, merged_val, page_addr, memory.page_size)
 
-                first_value = True
-                for v in merged_val:
-                    self.store(
-                        b,
-                        {SimMemoryObject(v, mo_base, endness=the_endness)},
-                        size=size,
-                        cooperate=True,
-                        weak=not first_value,
-                    )
-                    first_value = False
+                new_mos = {SimMemoryObject(v, mo_base, endness=the_endness) for v in merged_val}
+                self.store(b, new_mos, size=size, cooperate=True, weak=False)
 
                 merged_offsets.add(b)
 
             else:
-                # get the size that we can merge easily. This is the minimum of
-                # the size of all memory objects and unallocated spaces.
-                min_size = min(
-                    [mo.length - (b + page_addr - mo.base) for mo, _ in memory_objects] + [len(self.content) - b]
-                )
+                # get the size that we can merge easily. This is the minimum of the size of all memory objects and
+                # unallocated spaces.
+                min_size = len(self.content) - b
+                for mo_set in mo_sets:
+                    for mo in mo_set:
+                        min_size = min(min_size, mo.length - (b + page_addr - mo.base))
                 for um, _ in unconstrained_in:
                     for i in range(0, min_size):
                         if um._contains(b + i, page_addr):
                             min_size = i
                             break
                 merged_to = b + min_size
                 l.info("... determined minimum size of %d", min_size)
 
                 # Now, we have the minimum size. We'll extract/create expressions of that
                 # size and merge them
-                extracted = (
-                    [(mo.bytes_at(page_addr + b, min_size), fv) for mo, fv in memory_objects] if min_size != 0 else []
-                )
+                extracted = []
+                if min_size != 0:
+                    for mo_set, fv in memory_object_sets:
+                        for mo in mo_set:
+                            extracted.append((mo.bytes_at(page_addr + b, min_size), fv))
                 if not memory.skip_missing_values_during_merging:
                     created = [
                         (self._default_value(None, min_size, name=f"merge_uc_{uc.id}_{b:x}", memory=memory), fv)
                         for uc, fv in unconstrained_in
                     ]
                     to_merge = extracted + created
                 else:
                     to_merge = extracted
 
                 merged_val = self._merge_values(to_merge, min_size, memory=memory)
                 if merged_val is None:
                     continue
 
-                first_value = True
-                for v in merged_val:
-                    self.store(
-                        b,
-                        {SimMemoryObject(v, page_addr + b, endness="Iend_BE")},
-                        size=min_size,
-                        endness="Iend_BE",
-                        cooperate=True,
-                        weak=not first_value,
-                    )  # do not convert endianness again
-                    first_value = False
+                new_mos = {SimMemoryObject(v, page_addr + b, endness="Iend_BE") for v in merged_val}
+                self.store(b, new_mos, size=min_size, cooperate=True, weak=False)
                 merged_offsets.add(b)
 
         self.stored_offset |= merged_offsets
         return merged_offsets
 
+    def compare(
+        self, other: "MVListPage", page_addr: int = None, memory=None, changed_offsets=None
+    ) -> bool:  # pylint: disable=unused-argument
+        compared_to = None
+        for b in sorted(changed_offsets):
+            if compared_to is not None and not b >= compared_to:
+                continue
+
+            unconstrained_in = []
+            self_has_memory_object_set = False
+            memory_object_sets: Set[FrozenSet[SimMemoryObject]] = set()
+            for sm in [self, other]:
+                if sm._contains(b, page_addr):
+                    memory_objects = set()
+                    for mo in sm.content_gen(b):
+                        if mo.includes(page_addr + b):
+                            memory_objects.add(mo)
+                    memory_object_sets.add(frozenset(memory_objects))
+                    if sm is self:
+                        self_has_memory_object_set = True
+                else:
+                    unconstrained_in.append(sm)
+
+            if not memory_object_sets:
+                continue
+            if self_has_memory_object_set and len(memory_object_sets) == 1:
+                continue
+
+            # TODO: compare_values even more?
+            return False
+
+        return True
+
     def changed_bytes(self, other: "MVListPage", page_addr: int = None):
         candidates: Set[int] = super().changed_bytes(other)
         if candidates is not None:
             # using the result from the history tracking mixin as an approximation
             return candidates
 
         # slower path
```

### Comparing `angr-9.2.96/angr/storage/memory_mixins/paged_memory/pages/permissions_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/permissions_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/paged_memory/pages/refcount_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/refcount_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/paged_memory/pages/ultra_page.py` & `angr-9.2.97/angr/storage/memory_mixins/paged_memory/pages/ultra_page.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/paged_memory/privileged_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/paged_memory/privileged_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/paged_memory/stack_allocation_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/paged_memory/stack_allocation_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/regioned_memory/abstract_address_descriptor.py` & `angr-9.2.97/angr/storage/memory_mixins/regioned_memory/abstract_address_descriptor.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/regioned_memory/abstract_merger_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/regioned_memory/abstract_merger_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/regioned_memory/region_data.py` & `angr-9.2.97/angr/storage/memory_mixins/regioned_memory/region_data.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/regioned_memory/region_meta_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/regioned_memory/region_meta_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/regioned_memory/regioned_address_concretization_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/regioned_memory/regioned_address_concretization_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/regioned_memory/regioned_memory_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/regioned_memory/regioned_memory_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/regioned_memory/static_find_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/regioned_memory/static_find_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/simple_interface_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/simple_interface_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/size_resolution_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/size_resolution_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/slotted_memory.py` & `angr-9.2.97/angr/storage/memory_mixins/slotted_memory.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/smart_find_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/smart_find_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/top_merger_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/top_merger_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/underconstrained_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/underconstrained_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_mixins/unwrapper_mixin.py` & `angr-9.2.97/angr/storage/memory_mixins/unwrapper_mixin.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/memory_object.py` & `angr-9.2.97/angr/storage/memory_object.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/storage/pcap.py` & `angr-9.2.97/angr/storage/pcap.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/tablespecs.py` & `angr-9.2.97/angr/tablespecs.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/utils/__init__.py` & `angr-9.2.97/angr/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/utils/algo.py` & `angr-9.2.97/angr/utils/algo.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/utils/cowdict.py` & `angr-9.2.97/angr/utils/cowdict.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 class DefaultChainMapCOW(ChainMapCOW):
     """
     Implements a copy-on-write version of ChainMap with default values that supports auto-collapsing.
     """
 
-    def __init__(self, default_factory, *args, collapse_threshold=None):
+    def __init__(self, *args, default_factory=None, collapse_threshold=None):
         super().__init__(*args, collapse_threshold=collapse_threshold)
         self.default_factory = default_factory
 
     def __getitem__(self, key):
         try:
             return super().__getitem__(key)
         except KeyError:
@@ -49,14 +49,16 @@
     def clean(self):
         if self.dirty:
             # collapse?
             if self.collapse_threshold is not None and len(self.maps) >= self.collapse_threshold:
                 collapsed = {}
                 for m in reversed(self.maps):
                     collapsed.update(m)
-                return DefaultChainMapCOW(collapsed, collapse_threshold=self.collapse_threshold)
+                return DefaultChainMapCOW(
+                    collapsed, default_factory=self.default_factory, collapse_threshold=self.collapse_threshold
+                )
             r = self.new_child()
             r.default_factory = self.default_factory
             r.collapse_threshold = self.collapse_threshold
             return r
         else:
             return self
```

### Comparing `angr-9.2.96/angr/utils/dynamic_dictlist.py` & `angr-9.2.97/angr/utils/dynamic_dictlist.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/utils/enums_conv.py` & `angr-9.2.97/angr/utils/enums_conv.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/utils/formatting.py` & `angr-9.2.97/angr/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/utils/funcid.py` & `angr-9.2.97/angr/utils/funcid.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 def is_function_security_check_cookie(func, project, security_cookie_addr: int) -> bool:
     # disassemble the first instruction
     if func.is_plt or func.is_syscall or func.is_simprocedure:
         return False
     block = project.factory.block(func.addr)
     if block.instructions != 2:
         return False
+    if not block.capstone.insns or len(block.capstone.insns) != 2:
+        return False
     ins0 = block.capstone.insns[0]
     if (
         ins0.mnemonic == "cmp"
         and len(ins0.operands) == 2
         and ins0.operands[0].type == capstone.x86.X86_OP_REG
         and ins0.operands[0].reg == capstone.x86.X86_REG_RCX
         and ins0.operands[1].type == capstone.x86.X86_OP_MEM
@@ -53,14 +55,16 @@
     else:
         return False
     for node_addr, node_size in preds:
         # lift the block and check the last instruction
         block = project.factory.block(node_addr, size=node_size)
         if not block.instructions:
             continue
+        if not block.capstone.insns:
+            continue
         last_insn = block.capstone.insns[-1]
         if (
             last_insn.mnemonic == "mov"
             and len(last_insn.operands) == 2
             and last_insn.operands[0].type == capstone.x86.X86_OP_MEM
             and last_insn.operands[0].mem.base == capstone.x86.X86_REG_RIP
             and last_insn.operands[0].mem.index == 0
@@ -74,14 +78,16 @@
 def is_function_security_init_cookie_win8(func: "Function", project, security_cookie_addr: int) -> bool:
     # disassemble the first instruction
     if func.is_plt or func.is_syscall or func.is_simprocedure:
         return False
     block = project.factory.block(func.addr)
     if block.instructions != 3:
         return False
+    if not block.capstone.insns or len(block.capstone.insns) != 3:
+        return False
     ins0 = block.capstone.insns[0]
     if (
         ins0.mnemonic == "mov"
         and len(ins0.operands) == 2
         and ins0.operands[0].type == capstone.x86.X86_OP_REG
         and ins0.operands[0].reg == capstone.x86.X86_REG_RAX
         and ins0.operands[1].type == capstone.x86.X86_OP_MEM
```

### Comparing `angr-9.2.96/angr/utils/graph.py` & `angr-9.2.97/angr/utils/graph.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/utils/library.py` & `angr-9.2.97/angr/utils/library.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/utils/loader.py` & `angr-9.2.97/angr/utils/loader.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/utils/mp.py` & `angr-9.2.97/angr/utils/mp.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         A shortcut for adding Closures as initializers
         """
         self.initializers.append(Closure(f, args, kwargs))
 
     def initialize(self) -> None:
         """
         Initialize a multiprocessing.Process
-        Set the current global initalizer to the same state as this initalizer, then calls each initalizer
+        Set the current global initializer to the same state as this initializer, then calls each initializer
         """
         self._single = self
         for i in self.initializers:
             i.f(*i.args, **i.kwargs)
 
 
 def mp_context():
```

### Comparing `angr-9.2.96/angr/utils/segment_list.py` & `angr-9.2.97/angr/utils/segment_list.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/utils/timing.py` & `angr-9.2.97/angr/utils/timing.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr/vaults.py` & `angr-9.2.97/angr/vaults.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr.egg-info/PKG-INFO` & `angr-9.2.97/angr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angr
-Version: 9.2.96
+Version: 9.2.97
 Summary: A multi-architecture binary analysis toolkit, with the ability to perform dynamic symbolic execution and various static analyses on binaries
 Home-page: https://github.com/angr/angr
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -13,31 +13,31 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: CppHeaderParser
 Requires-Dist: GitPython
-Requires-Dist: ailment==9.2.96
-Requires-Dist: archinfo==9.2.96
+Requires-Dist: ailment==9.2.97
+Requires-Dist: archinfo==9.2.97
 Requires-Dist: cachetools
 Requires-Dist: capstone==5.0.0.post1
 Requires-Dist: cffi>=1.14.0
-Requires-Dist: claripy==9.2.96
-Requires-Dist: cle==9.2.96
+Requires-Dist: claripy==9.2.97
+Requires-Dist: cle==9.2.97
 Requires-Dist: dpkt
 Requires-Dist: itanium-demangler
 Requires-Dist: mulpyplexer
 Requires-Dist: nampa
 Requires-Dist: networkx!=2.8.1,>=2.0
 Requires-Dist: protobuf>=3.19.0
 Requires-Dist: psutil
 Requires-Dist: pycparser>=2.18
 Requires-Dist: pyformlang
-Requires-Dist: pyvex==9.2.96
+Requires-Dist: pyvex==9.2.97
 Requires-Dist: rich>=13.1.0
 Requires-Dist: rpyc
 Requires-Dist: sortedcontainers
 Requires-Dist: sympy
 Requires-Dist: unicorn==2.0.1.post1
 Requires-Dist: unique-log-filter
 Requires-Dist: colorama; platform_system == "Windows"
```

### Comparing `angr-9.2.96/angr.egg-info/SOURCES.txt` & `angr-9.2.97/angr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/angr.egg-info/requires.txt` & `angr-9.2.97/angr.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 CppHeaderParser
 GitPython
-ailment==9.2.96
-archinfo==9.2.96
+ailment==9.2.97
+archinfo==9.2.97
 cachetools
 capstone==5.0.0.post1
 cffi>=1.14.0
-claripy==9.2.96
-cle==9.2.96
+claripy==9.2.97
+cle==9.2.97
 dpkt
 itanium-demangler
 mulpyplexer
 nampa
 networkx!=2.8.1,>=2.0
 protobuf>=3.19.0
 psutil
 pycparser>=2.18
 pyformlang
-pyvex==9.2.96
+pyvex==9.2.97
 rich>=13.1.0
 rpyc
 sortedcontainers
 sympy
 unicorn==2.0.1.post1
 unique-log-filter
```

### Comparing `angr-9.2.96/native/Makefile` & `angr-9.2.97/native/Makefile`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/native/angr_native.def` & `angr-9.2.97/native/angr_native.def`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/native/log.c` & `angr-9.2.97/native/log.c`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/native/log.h` & `angr-9.2.97/native/log.h`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/native/sim_unicorn.cpp` & `angr-9.2.97/native/sim_unicorn.cpp`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/native/sim_unicorn.hpp` & `angr-9.2.97/native/sim_unicorn.hpp`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/pyproject.toml` & `angr-9.2.97/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=59", "wheel", "pyvex==9.2.96", "unicorn==2.0.1.post1"]
+requires = ["setuptools>=59", "wheel", "pyvex==9.2.97", "unicorn==2.0.1.post1"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
 target-version = ['py38']
 force-exclude = '''
 /(
```

### Comparing `angr-9.2.96/setup.cfg` & `angr-9.2.97/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -18,31 +18,31 @@
 	Programming Language :: Python :: 3.12
 
 [options]
 packages = find:
 install_requires = 
 	CppHeaderParser
 	GitPython
-	ailment==9.2.96
-	archinfo==9.2.96
+	ailment==9.2.97
+	archinfo==9.2.97
 	cachetools
 	capstone==5.0.0.post1
 	cffi>=1.14.0
-	claripy==9.2.96
-	cle==9.2.96
+	claripy==9.2.97
+	cle==9.2.97
 	dpkt
 	itanium-demangler
 	mulpyplexer
 	nampa
 	networkx!=2.8.1,>=2.0
 	protobuf>=3.19.0
 	psutil
 	pycparser>=2.18
 	pyformlang
-	pyvex==9.2.96
+	pyvex==9.2.97
 	rich>=13.1.0
 	rpyc
 	sortedcontainers
 	sympy
 	unicorn==2.0.1.post1
 	unique-log-filter
 	colorama;platform_system=='Windows'
```

### Comparing `angr-9.2.96/setup.py` & `angr-9.2.97/setup.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/tests/test_calling_conventions.py` & `angr-9.2.97/tests/test_calling_conventions.py`

 * *Files identical despite different names*

### Comparing `angr-9.2.96/tests/test_types.py` & `angr-9.2.97/tests/test_types.py`

 * *Files identical despite different names*

