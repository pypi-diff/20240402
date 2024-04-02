# Comparing `tmp/netket-3.9.1.tar.gz` & `tmp/netket-3.9.2.tar.gz`

## Comparing `netket-3.9.1.tar` & `netket-3.9.2.tar`

### file list

```diff
@@ -1,263 +1,263 @@
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 netket-3.9.1/netket/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 netket-3.9.1/netket/_version.py
--rw-r--r--   0        0        0    25304 2020-02-02 00:00:00.000000 netket-3.9.1/netket/errors.py
--rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 netket-3.9.1/netket/exact.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 netket-3.9.1/netket/callbacks/__init__.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 netket-3.9.1/netket/callbacks/convergence_stopping.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 netket-3.9.1/netket/callbacks/earlystopping.py
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 netket-3.9.1/netket/callbacks/invalidlossstopping.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 netket-3.9.1/netket/callbacks/timeout.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 netket-3.9.1/netket/driver/__init__.py
--rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 netket-3.9.1/netket/driver/abstract_variational_driver.py
--rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 netket-3.9.1/netket/driver/steady_state.py
--rw-r--r--   0        0        0     5691 2020-02-02 00:00:00.000000 netket-3.9.1/netket/driver/vmc.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 netket-3.9.1/netket/driver/vmc_common.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/driver/__init__.py
--rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/driver/tdvp.py
--rw-r--r--   0        0        0    17314 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/driver/tdvp_common.py
--rw-r--r--   0        0        0    11601 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/driver/tdvp_schmitt.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/dynamics/__init__.py
--rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/dynamics/_rk_solver.py
--rw-r--r--   0        0        0    13184 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/dynamics/_rk_solver_structures.py
--rw-r--r--   0        0        0    10730 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/dynamics/_rk_tableau.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/hilbert/__init__.py
--rw-r--r--   0        0        0     6814 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/hilbert/spin_orbital_fermions.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/hilbert/random/__init__.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/hilbert/random/spin_orbital_fermions.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/logging/__init__.py
--rw-r--r--   0        0        0     7361 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/logging/hdf5_log.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/operator/__init__.py
--rw-r--r--   0        0        0    25157 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/operator/_fermion_operator_2nd.py
--rw-r--r--   0        0        0    13155 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/operator/_fermion_operator_2nd_utils.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/operator/fermion.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/qsr/__init__.py
--rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/qsr/dataset.py
--rw-r--r--   0        0        0    19562 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/qsr/driver.py
--rw-r--r--   0        0        0     8058 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/qsr/logic_helpers.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/sampler/__init__.py
--rw-r--r--   0        0        0     8540 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/sampler/metropolis_pmap.py
--rw-r--r--   0        0        0    21309 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/sampler/metropolis_pt.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/vqs/__init__.py
--rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 netket-3.9.1/netket/experimental/vqs/io.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 netket-3.9.1/netket/graph/__init__.py
--rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 netket-3.9.1/netket/graph/_lattice_edge_logic.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 netket-3.9.1/netket/graph/abstract_graph.py
--rw-r--r--   0        0        0    19802 2020-02-02 00:00:00.000000 netket-3.9.1/netket/graph/common_lattices.py
--rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 netket-3.9.1/netket/graph/graph.py
--rw-r--r--   0        0        0    28347 2020-02-02 00:00:00.000000 netket-3.9.1/netket/graph/lattice.py
--rw-r--r--   0        0        0    12996 2020-02-02 00:00:00.000000 netket-3.9.1/netket/graph/space_group.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/__init__.py
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/abstract_hilbert.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/continuous_hilbert.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/custom_hilbert.py
--rw-r--r--   0        0        0     8590 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/discrete_hilbert.py
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/doubled_hilbert.py
--rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/fock.py
--rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/homogeneous.py
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/particle.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/qubit.py
--rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/spin.py
--rw-r--r--   0        0        0     6931 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/tensor_hilbert.py
--rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/tensor_hilbert_discrete.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/index/__init__.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/index/base.py
--rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/index/constrained.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/index/unconstrained.py
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/random/__init__.py
--rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/random/base.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/random/custom.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/random/doubled.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/random/fock.py
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/random/particle.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/random/qubit.py
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/random/spin.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 netket-3.9.1/netket/hilbert/random/tensor_hilbert.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 netket-3.9.1/netket/jax/__init__.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 netket-3.9.1/netket/jax/_chunk_utils.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 netket-3.9.1/netket/jax/_expect.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 netket-3.9.1/netket/jax/_grad.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 netket-3.9.1/netket/jax/_math.py
--rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 netket-3.9.1/netket/jax/_scanmap.py
--rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 netket-3.9.1/netket/jax/_vjp.py
--rw-r--r--   0        0        0     8560 2020-02-02 00:00:00.000000 netket-3.9.1/netket/jax/_vjp_chunked.py
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 netket-3.9.1/netket/jax/_vmap_chunked.py
--rw-r--r--   0        0        0    10586 2020-02-02 00:00:00.000000 netket-3.9.1/netket/jax/utils.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 netket-3.9.1/netket/jax/_jacobian/__init__.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 netket-3.9.1/netket/jax/_jacobian/default_mode.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 netket-3.9.1/netket/jax/_jacobian/jacobian_dense.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 netket-3.9.1/netket/jax/_jacobian/jacobian_pytree.py
--rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 netket-3.9.1/netket/jax/_jacobian/logic.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 netket-3.9.1/netket/logging/__init__.py
--rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 netket-3.9.1/netket/logging/json_log.py
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 netket-3.9.1/netket/logging/runtime_log.py
--rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 netket-3.9.1/netket/logging/state_log.py
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 netket-3.9.1/netket/logging/tensorboard.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 netket-3.9.1/netket/models/README.md
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 netket-3.9.1/netket/models/__init__.py
--rw-r--r--   0        0        0    13327 2020-02-02 00:00:00.000000 netket-3.9.1/netket/models/autoreg.py
--rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 netket-3.9.1/netket/models/deepset.py
--rw-r--r--   0        0        0    33559 2020-02-02 00:00:00.000000 netket-3.9.1/netket/models/equivariant.py
--rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 netket-3.9.1/netket/models/fast_autoreg.py
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 netket-3.9.1/netket/models/full_space.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 netket-3.9.1/netket/models/gaussian.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 netket-3.9.1/netket/models/jastrow.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 netket-3.9.1/netket/models/mlp.py
--rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 netket-3.9.1/netket/models/mps.py
--rw-r--r--   0        0        0     7760 2020-02-02 00:00:00.000000 netket-3.9.1/netket/models/ndm.py
--rw-r--r--   0        0        0     9722 2020-02-02 00:00:00.000000 netket-3.9.1/netket/models/rbm.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 netket-3.9.1/netket/models/utils.py
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 netket-3.9.1/netket/nn/__init__.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 netket-3.9.1/netket/nn/activation.py
--rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 netket-3.9.1/netket/nn/deprecation.py
--rw-r--r--   0        0        0    16212 2020-02-02 00:00:00.000000 netket-3.9.1/netket/nn/fast_masked_linear.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 netket-3.9.1/netket/nn/initializers.py
--rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 netket-3.9.1/netket/nn/masked_linear.py
--rw-r--r--   0        0        0    35416 2020-02-02 00:00:00.000000 netket-3.9.1/netket/nn/symmetric_linear.py
--rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 netket-3.9.1/netket/nn/utils.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 netket-3.9.1/netket/nn/blocks/__init__.py
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 netket-3.9.1/netket/nn/blocks/deepset.py
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 netket-3.9.1/netket/nn/blocks/mlp.py
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 netket-3.9.1/netket/nn/blocks/symmetry_sum.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/__init__.py
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_abstract_operator.py
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_abstract_super_operator.py
--rw-r--r--   0        0        0    11408 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_bose_hubbard.py
--rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_continuous_operator.py
--rw-r--r--   0        0        0    10630 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_discrete_operator.py
--rw-r--r--   0        0        0     8590 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_discrete_operator_jax.py
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_graph_operator.py
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_hamiltonian.py
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_heisenberg.py
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_kinetic.py
--rw-r--r--   0        0        0     6435 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_lazy.py
--rw-r--r--   0        0        0    16259 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_local_liouvillian.py
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_potential.py
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_sumoperators.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/boson.py
--rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/spin.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_ising/__init__.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_ising/base.py
--rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_ising/jax.py
--rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_ising/numba.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_local_operator/__init__.py
--rw-r--r--   0        0        0    25787 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_local_operator/base.py
--rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_local_operator/compile_helpers.py
--rw-r--r--   0        0        0     6711 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_local_operator/convert.py
--rw-r--r--   0        0        0     9879 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_local_operator/helpers.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_pauli_strings/__init__.py
--rw-r--r--   0        0        0    17099 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_pauli_strings/base.py
--rw-r--r--   0        0        0    14345 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_pauli_strings/jax.py
--rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 netket-3.9.1/netket/operator/_pauli_strings/numba.py
--rw-r--r--   0        0        0     6619 2020-02-02 00:00:00.000000 netket-3.9.1/netket/optimizer/__init__.py
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 netket-3.9.1/netket/optimizer/linear_operator.py
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 netket-3.9.1/netket/optimizer/preconditioner.py
--rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 netket-3.9.1/netket/optimizer/sr.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 netket-3.9.1/netket/optimizer/qgt/__init__.py
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 netket-3.9.1/netket/optimizer/qgt/common.py
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 netket-3.9.1/netket/optimizer/qgt/default.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 netket-3.9.1/netket/optimizer/qgt/qgt_jacobian_common.py
--rw-r--r--   0        0        0    10502 2020-02-02 00:00:00.000000 netket-3.9.1/netket/optimizer/qgt/qgt_jacobian_dense.py
--rw-r--r--   0        0        0    11075 2020-02-02 00:00:00.000000 netket-3.9.1/netket/optimizer/qgt/qgt_jacobian_pytree.py
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 netket-3.9.1/netket/optimizer/qgt/qgt_jacobian_pytree_logic.py
--rw-r--r--   0        0        0     9185 2020-02-02 00:00:00.000000 netket-3.9.1/netket/optimizer/qgt/qgt_onthefly.py
--rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 netket-3.9.1/netket/optimizer/qgt/qgt_onthefly_logic.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 netket-3.9.1/netket/optimizer/solver/__init__.py
--rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 netket-3.9.1/netket/optimizer/solver/solvers.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 netket-3.9.1/netket/sampler/__init__.py
--rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 netket-3.9.1/netket/sampler/autoreg.py
--rw-r--r--   0        0        0    18149 2020-02-02 00:00:00.000000 netket-3.9.1/netket/sampler/base.py
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 netket-3.9.1/netket/sampler/exact.py
--rw-r--r--   0        0        0    27062 2020-02-02 00:00:00.000000 netket-3.9.1/netket/sampler/metropolis.py
--rw-r--r--   0        0        0     9397 2020-02-02 00:00:00.000000 netket-3.9.1/netket/sampler/metropolis_numpy.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 netket-3.9.1/netket/sampler/rules/__init__.py
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 netket-3.9.1/netket/sampler/rules/base.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 netket-3.9.1/netket/sampler/rules/continuous_gaussian.py
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 netket-3.9.1/netket/sampler/rules/custom_numpy.py
--rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 netket-3.9.1/netket/sampler/rules/exchange.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 netket-3.9.1/netket/sampler/rules/fixed.py
--rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 netket-3.9.1/netket/sampler/rules/hamiltonian.py
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 netket-3.9.1/netket/sampler/rules/hamiltonian_numpy.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 netket-3.9.1/netket/sampler/rules/langevin.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 netket-3.9.1/netket/sampler/rules/local.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 netket-3.9.1/netket/sampler/rules/local_numpy.py
--rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 netket-3.9.1/netket/sampler/rules/multiple.py
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 netket-3.9.1/netket/sampler/rules/tensor.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 netket-3.9.1/netket/stats/__init__.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 netket-3.9.1/netket/stats/_autocorr.py
--rw-r--r--   0        0        0     9643 2020-02-02 00:00:00.000000 netket-3.9.1/netket/stats/mc_stats.py
--rw-r--r--   0        0        0     6922 2020-02-02 00:00:00.000000 netket-3.9.1/netket/stats/mc_stats_old.py
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 netket-3.9.1/netket/stats/mpi_stats.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netket-3.9.1/netket/tools/__init__.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 netket-3.9.1/netket/tools/_common.py
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 netket-3.9.1/netket/tools/_cpu_info.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 netket-3.9.1/netket/tools/_mpi_info.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 netket-3.9.1/netket/tools/check_mpi.py
--rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 netket-3.9.1/netket/tools/info.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/__init__.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/_dependencies_check.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/array.py
--rw-r--r--   0        0        0     6614 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/config_flags.py
--rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/deprecation.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/dispatch.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/float.py
--rw-r--r--   0        0        0    12748 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/history.py
--rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/holomorphic.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/jax.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/moduletools.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/numbers.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/optional_deps.py
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/partial.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/seed.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/static_number.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/summation.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/types.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/version_check.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/group/__init__.py
--rw-r--r--   0        0        0    15118 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/group/_group.py
--rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/group/_permutation_group.py
--rw-r--r--   0        0        0    21830 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/group/_point_group.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/group/_semigroup.py
--rw-r--r--   0        0        0    10404 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/group/axial.py
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/group/cubic.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/group/icosa.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/group/planar.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/model_frameworks/__init__.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/model_frameworks/base.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/model_frameworks/flax.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/model_frameworks/haiku.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/model_frameworks/jax.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/mpi/__init__.py
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/mpi/mpi.py
--rw-r--r--   0        0        0     7319 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/mpi/primitives.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/struct/__init__.py
--rw-r--r--   0        0        0    16933 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/struct/dataclass.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 netket-3.9.1/netket/utils/struct/utils.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/__init__.py
--rw-r--r--   0        0        0    15652 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/base.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/deprecated.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/experimental.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/full_summ/__init__.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/full_summ/expect.py
--rw-r--r--   0        0        0    12303 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/full_summ/state.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/mc/__init__.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/mc/common.py
--rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/mc/kernels.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/mc/mc_mixed_state/__init__.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/mc/mc_mixed_state/expect.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/mc/mc_mixed_state/expect_chunked.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/mc/mc_mixed_state/expect_grad_chunked.py
--rw-r--r--   0        0        0    10393 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/mc/mc_mixed_state/state.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/mc/mc_state/__init__.py
--rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/mc/mc_state/expect.py
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/mc/mc_state/expect_chunked.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/mc/mc_state/expect_forces.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/mc/mc_state/expect_forces_chunked.py
--rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/mc/mc_state/expect_grad.py
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/mc/mc_state/expect_grad_chunked.py
--rw-r--r--   0        0        0    28586 2020-02-02 00:00:00.000000 netket-3.9.1/netket/vqs/mc/mc_state/state.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 netket-3.9.1/.gitignore
--rw-r--r--   0        0        0    10173 2020-02-02 00:00:00.000000 netket-3.9.1/LICENSE
--rw-r--r--   0        0        0     5877 2020-02-02 00:00:00.000000 netket-3.9.1/README.md
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 netket-3.9.1/pyproject.toml
--rw-r--r--   0        0        0     8646 2020-02-02 00:00:00.000000 netket-3.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 netket-3.9.2/netket/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 netket-3.9.2/netket/_version.py
+-rw-r--r--   0        0        0    25304 2020-02-02 00:00:00.000000 netket-3.9.2/netket/errors.py
+-rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 netket-3.9.2/netket/exact.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 netket-3.9.2/netket/callbacks/__init__.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 netket-3.9.2/netket/callbacks/convergence_stopping.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 netket-3.9.2/netket/callbacks/earlystopping.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 netket-3.9.2/netket/callbacks/invalidlossstopping.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 netket-3.9.2/netket/callbacks/timeout.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 netket-3.9.2/netket/driver/__init__.py
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 netket-3.9.2/netket/driver/abstract_variational_driver.py
+-rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 netket-3.9.2/netket/driver/steady_state.py
+-rw-r--r--   0        0        0     5691 2020-02-02 00:00:00.000000 netket-3.9.2/netket/driver/vmc.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 netket-3.9.2/netket/driver/vmc_common.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/driver/__init__.py
+-rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/driver/tdvp.py
+-rw-r--r--   0        0        0    17346 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/driver/tdvp_common.py
+-rw-r--r--   0        0        0    11599 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/driver/tdvp_schmitt.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/dynamics/__init__.py
+-rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/dynamics/_rk_solver.py
+-rw-r--r--   0        0        0    13184 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/dynamics/_rk_solver_structures.py
+-rw-r--r--   0        0        0    10730 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/dynamics/_rk_tableau.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/hilbert/__init__.py
+-rw-r--r--   0        0        0     6814 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/hilbert/spin_orbital_fermions.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/hilbert/random/__init__.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/hilbert/random/spin_orbital_fermions.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/logging/__init__.py
+-rw-r--r--   0        0        0     7361 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/logging/hdf5_log.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/operator/__init__.py
+-rw-r--r--   0        0        0    25157 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/operator/_fermion_operator_2nd.py
+-rw-r--r--   0        0        0    13155 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/operator/_fermion_operator_2nd_utils.py
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/operator/fermion.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/qsr/__init__.py
+-rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/qsr/dataset.py
+-rw-r--r--   0        0        0    19562 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/qsr/driver.py
+-rw-r--r--   0        0        0     8058 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/qsr/logic_helpers.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/sampler/__init__.py
+-rw-r--r--   0        0        0     8540 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/sampler/metropolis_pmap.py
+-rw-r--r--   0        0        0    21309 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/sampler/metropolis_pt.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/vqs/__init__.py
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 netket-3.9.2/netket/experimental/vqs/io.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 netket-3.9.2/netket/graph/__init__.py
+-rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 netket-3.9.2/netket/graph/_lattice_edge_logic.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 netket-3.9.2/netket/graph/abstract_graph.py
+-rw-r--r--   0        0        0    19802 2020-02-02 00:00:00.000000 netket-3.9.2/netket/graph/common_lattices.py
+-rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 netket-3.9.2/netket/graph/graph.py
+-rw-r--r--   0        0        0    28347 2020-02-02 00:00:00.000000 netket-3.9.2/netket/graph/lattice.py
+-rw-r--r--   0        0        0    12996 2020-02-02 00:00:00.000000 netket-3.9.2/netket/graph/space_group.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/__init__.py
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/abstract_hilbert.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/continuous_hilbert.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/custom_hilbert.py
+-rw-r--r--   0        0        0     8590 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/discrete_hilbert.py
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/doubled_hilbert.py
+-rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/fock.py
+-rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/homogeneous.py
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/particle.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/qubit.py
+-rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/spin.py
+-rw-r--r--   0        0        0     6931 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/tensor_hilbert.py
+-rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/tensor_hilbert_discrete.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/index/__init__.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/index/base.py
+-rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/index/constrained.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/index/unconstrained.py
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/random/__init__.py
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/random/base.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/random/custom.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/random/doubled.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/random/fock.py
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/random/particle.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/random/qubit.py
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/random/spin.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 netket-3.9.2/netket/hilbert/random/tensor_hilbert.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 netket-3.9.2/netket/jax/__init__.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 netket-3.9.2/netket/jax/_chunk_utils.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 netket-3.9.2/netket/jax/_expect.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 netket-3.9.2/netket/jax/_grad.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 netket-3.9.2/netket/jax/_math.py
+-rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 netket-3.9.2/netket/jax/_scanmap.py
+-rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 netket-3.9.2/netket/jax/_vjp.py
+-rw-r--r--   0        0        0     8560 2020-02-02 00:00:00.000000 netket-3.9.2/netket/jax/_vjp_chunked.py
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 netket-3.9.2/netket/jax/_vmap_chunked.py
+-rw-r--r--   0        0        0    10586 2020-02-02 00:00:00.000000 netket-3.9.2/netket/jax/utils.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 netket-3.9.2/netket/jax/_jacobian/__init__.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 netket-3.9.2/netket/jax/_jacobian/default_mode.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 netket-3.9.2/netket/jax/_jacobian/jacobian_dense.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 netket-3.9.2/netket/jax/_jacobian/jacobian_pytree.py
+-rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 netket-3.9.2/netket/jax/_jacobian/logic.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 netket-3.9.2/netket/logging/__init__.py
+-rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 netket-3.9.2/netket/logging/json_log.py
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 netket-3.9.2/netket/logging/runtime_log.py
+-rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 netket-3.9.2/netket/logging/state_log.py
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 netket-3.9.2/netket/logging/tensorboard.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 netket-3.9.2/netket/models/README.md
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 netket-3.9.2/netket/models/__init__.py
+-rw-r--r--   0        0        0    13327 2020-02-02 00:00:00.000000 netket-3.9.2/netket/models/autoreg.py
+-rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 netket-3.9.2/netket/models/deepset.py
+-rw-r--r--   0        0        0    33559 2020-02-02 00:00:00.000000 netket-3.9.2/netket/models/equivariant.py
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 netket-3.9.2/netket/models/fast_autoreg.py
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 netket-3.9.2/netket/models/full_space.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 netket-3.9.2/netket/models/gaussian.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 netket-3.9.2/netket/models/jastrow.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 netket-3.9.2/netket/models/mlp.py
+-rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 netket-3.9.2/netket/models/mps.py
+-rw-r--r--   0        0        0     7760 2020-02-02 00:00:00.000000 netket-3.9.2/netket/models/ndm.py
+-rw-r--r--   0        0        0     9722 2020-02-02 00:00:00.000000 netket-3.9.2/netket/models/rbm.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 netket-3.9.2/netket/models/utils.py
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 netket-3.9.2/netket/nn/__init__.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 netket-3.9.2/netket/nn/activation.py
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 netket-3.9.2/netket/nn/deprecation.py
+-rw-r--r--   0        0        0    16212 2020-02-02 00:00:00.000000 netket-3.9.2/netket/nn/fast_masked_linear.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 netket-3.9.2/netket/nn/initializers.py
+-rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 netket-3.9.2/netket/nn/masked_linear.py
+-rw-r--r--   0        0        0    35416 2020-02-02 00:00:00.000000 netket-3.9.2/netket/nn/symmetric_linear.py
+-rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 netket-3.9.2/netket/nn/utils.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 netket-3.9.2/netket/nn/blocks/__init__.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 netket-3.9.2/netket/nn/blocks/deepset.py
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 netket-3.9.2/netket/nn/blocks/mlp.py
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 netket-3.9.2/netket/nn/blocks/symmetry_sum.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/__init__.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_abstract_operator.py
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_abstract_super_operator.py
+-rw-r--r--   0        0        0    11408 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_bose_hubbard.py
+-rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_continuous_operator.py
+-rw-r--r--   0        0        0    10630 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_discrete_operator.py
+-rw-r--r--   0        0        0     8590 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_discrete_operator_jax.py
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_graph_operator.py
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_hamiltonian.py
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_heisenberg.py
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_kinetic.py
+-rw-r--r--   0        0        0     6435 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_lazy.py
+-rw-r--r--   0        0        0    16259 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_local_liouvillian.py
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_potential.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_sumoperators.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/boson.py
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/spin.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_ising/__init__.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_ising/base.py
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_ising/jax.py
+-rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_ising/numba.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_local_operator/__init__.py
+-rw-r--r--   0        0        0    25846 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_local_operator/base.py
+-rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_local_operator/compile_helpers.py
+-rw-r--r--   0        0        0     6711 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_local_operator/convert.py
+-rw-r--r--   0        0        0     9879 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_local_operator/helpers.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_pauli_strings/__init__.py
+-rw-r--r--   0        0        0    17099 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_pauli_strings/base.py
+-rw-r--r--   0        0        0    14345 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_pauli_strings/jax.py
+-rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 netket-3.9.2/netket/operator/_pauli_strings/numba.py
+-rw-r--r--   0        0        0     6619 2020-02-02 00:00:00.000000 netket-3.9.2/netket/optimizer/__init__.py
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 netket-3.9.2/netket/optimizer/linear_operator.py
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 netket-3.9.2/netket/optimizer/preconditioner.py
+-rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 netket-3.9.2/netket/optimizer/sr.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 netket-3.9.2/netket/optimizer/qgt/__init__.py
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 netket-3.9.2/netket/optimizer/qgt/common.py
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 netket-3.9.2/netket/optimizer/qgt/default.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 netket-3.9.2/netket/optimizer/qgt/qgt_jacobian_common.py
+-rw-r--r--   0        0        0    10502 2020-02-02 00:00:00.000000 netket-3.9.2/netket/optimizer/qgt/qgt_jacobian_dense.py
+-rw-r--r--   0        0        0    11075 2020-02-02 00:00:00.000000 netket-3.9.2/netket/optimizer/qgt/qgt_jacobian_pytree.py
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 netket-3.9.2/netket/optimizer/qgt/qgt_jacobian_pytree_logic.py
+-rw-r--r--   0        0        0     9185 2020-02-02 00:00:00.000000 netket-3.9.2/netket/optimizer/qgt/qgt_onthefly.py
+-rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 netket-3.9.2/netket/optimizer/qgt/qgt_onthefly_logic.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 netket-3.9.2/netket/optimizer/solver/__init__.py
+-rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 netket-3.9.2/netket/optimizer/solver/solvers.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 netket-3.9.2/netket/sampler/__init__.py
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 netket-3.9.2/netket/sampler/autoreg.py
+-rw-r--r--   0        0        0    18149 2020-02-02 00:00:00.000000 netket-3.9.2/netket/sampler/base.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 netket-3.9.2/netket/sampler/exact.py
+-rw-r--r--   0        0        0    27062 2020-02-02 00:00:00.000000 netket-3.9.2/netket/sampler/metropolis.py
+-rw-r--r--   0        0        0     9397 2020-02-02 00:00:00.000000 netket-3.9.2/netket/sampler/metropolis_numpy.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 netket-3.9.2/netket/sampler/rules/__init__.py
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 netket-3.9.2/netket/sampler/rules/base.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 netket-3.9.2/netket/sampler/rules/continuous_gaussian.py
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 netket-3.9.2/netket/sampler/rules/custom_numpy.py
+-rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 netket-3.9.2/netket/sampler/rules/exchange.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 netket-3.9.2/netket/sampler/rules/fixed.py
+-rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 netket-3.9.2/netket/sampler/rules/hamiltonian.py
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 netket-3.9.2/netket/sampler/rules/hamiltonian_numpy.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 netket-3.9.2/netket/sampler/rules/langevin.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 netket-3.9.2/netket/sampler/rules/local.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 netket-3.9.2/netket/sampler/rules/local_numpy.py
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 netket-3.9.2/netket/sampler/rules/multiple.py
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 netket-3.9.2/netket/sampler/rules/tensor.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 netket-3.9.2/netket/stats/__init__.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 netket-3.9.2/netket/stats/_autocorr.py
+-rw-r--r--   0        0        0     9643 2020-02-02 00:00:00.000000 netket-3.9.2/netket/stats/mc_stats.py
+-rw-r--r--   0        0        0     6922 2020-02-02 00:00:00.000000 netket-3.9.2/netket/stats/mc_stats_old.py
+-rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 netket-3.9.2/netket/stats/mpi_stats.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netket-3.9.2/netket/tools/__init__.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 netket-3.9.2/netket/tools/_common.py
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 netket-3.9.2/netket/tools/_cpu_info.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 netket-3.9.2/netket/tools/_mpi_info.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 netket-3.9.2/netket/tools/check_mpi.py
+-rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 netket-3.9.2/netket/tools/info.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/__init__.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/_dependencies_check.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/array.py
+-rw-r--r--   0        0        0     6614 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/config_flags.py
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/deprecation.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/dispatch.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/float.py
+-rw-r--r--   0        0        0    12748 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/history.py
+-rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/holomorphic.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/jax.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/moduletools.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/numbers.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/optional_deps.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/partial.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/seed.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/static_number.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/summation.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/types.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/version_check.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/group/__init__.py
+-rw-r--r--   0        0        0    15118 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/group/_group.py
+-rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/group/_permutation_group.py
+-rw-r--r--   0        0        0    21830 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/group/_point_group.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/group/_semigroup.py
+-rw-r--r--   0        0        0    10404 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/group/axial.py
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/group/cubic.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/group/icosa.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/group/planar.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/model_frameworks/base.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/model_frameworks/flax.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/model_frameworks/haiku.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/model_frameworks/jax.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/mpi/__init__.py
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/mpi/mpi.py
+-rw-r--r--   0        0        0     7319 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/mpi/primitives.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/struct/__init__.py
+-rw-r--r--   0        0        0    16933 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/struct/dataclass.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 netket-3.9.2/netket/utils/struct/utils.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/__init__.py
+-rw-r--r--   0        0        0    15652 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/base.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/deprecated.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/experimental.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/full_summ/__init__.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/full_summ/expect.py
+-rw-r--r--   0        0        0    12303 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/full_summ/state.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/mc/__init__.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/mc/common.py
+-rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/mc/kernels.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/mc/mc_mixed_state/__init__.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/mc/mc_mixed_state/expect.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/mc/mc_mixed_state/expect_chunked.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/mc/mc_mixed_state/expect_grad_chunked.py
+-rw-r--r--   0        0        0    10393 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/mc/mc_mixed_state/state.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/mc/mc_state/__init__.py
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/mc/mc_state/expect.py
+-rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/mc/mc_state/expect_chunked.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/mc/mc_state/expect_forces.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/mc/mc_state/expect_forces_chunked.py
+-rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/mc/mc_state/expect_grad.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/mc/mc_state/expect_grad_chunked.py
+-rw-r--r--   0        0        0    28586 2020-02-02 00:00:00.000000 netket-3.9.2/netket/vqs/mc/mc_state/state.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 netket-3.9.2/.gitignore
+-rw-r--r--   0        0        0    10173 2020-02-02 00:00:00.000000 netket-3.9.2/LICENSE
+-rw-r--r--   0        0        0     5877 2020-02-02 00:00:00.000000 netket-3.9.2/README.md
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 netket-3.9.2/pyproject.toml
+-rw-r--r--   0        0        0     8646 2020-02-02 00:00:00.000000 netket-3.9.2/PKG-INFO
```

### Comparing `netket-3.9.1/netket/__init__.py` & `netket-3.9.2/netket/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/errors.py` & `netket-3.9.2/netket/errors.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/exact.py` & `netket-3.9.2/netket/exact.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/callbacks/__init__.py` & `netket-3.9.2/netket/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/callbacks/convergence_stopping.py` & `netket-3.9.2/netket/callbacks/convergence_stopping.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/callbacks/earlystopping.py` & `netket-3.9.2/netket/callbacks/earlystopping.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/callbacks/invalidlossstopping.py` & `netket-3.9.2/netket/callbacks/invalidlossstopping.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/callbacks/timeout.py` & `netket-3.9.2/netket/callbacks/timeout.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/driver/__init__.py` & `netket-3.9.2/netket/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/driver/abstract_variational_driver.py` & `netket-3.9.2/netket/driver/abstract_variational_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,15 +241,19 @@
         else:
             loggers = tuple()
             show_progress = False
 
         callbacks = _to_iterable(callback)
         callback_stop = False
 
-        with tqdm(total=n_iter, disable=not show_progress) as pbar:
+        with tqdm(
+            total=n_iter,
+            disable=not show_progress,
+            dynamic_ncols=True,
+        ) as pbar:
             old_step = self.step_count
             first_step = True
 
             for step in self.iter(n_iter, step_size):
 
                 log_data = self.estimate(obs)
                 self._log_additional_data(log_data, step)
```

### Comparing `netket-3.9.1/netket/driver/steady_state.py` & `netket-3.9.2/netket/driver/steady_state.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/driver/vmc.py` & `netket-3.9.2/netket/driver/vmc.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/driver/vmc_common.py` & `netket-3.9.2/netket/driver/vmc_common.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/__init__.py` & `netket-3.9.2/netket/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/driver/__init__.py` & `netket-3.9.2/netket/experimental/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/driver/tdvp.py` & `netket-3.9.2/netket/experimental/driver/tdvp.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/driver/tdvp_common.py` & `netket-3.9.2/netket/experimental/driver/tdvp_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,14 +324,15 @@
         callback_stop = False
 
         t_end = np.asarray(self.t + T)
         with tqdm(
             total=t_end,
             disable=not show_progress,
             unit_scale=True,
+            dynamic_ncols=True,
         ) as pbar:
             first_step = True
 
             # We need a closure to pass to self._iter in order to update the progress bar even if
             # there are no tstops
             def update_progress_bar():
                 # Reset the timing of tqdm after the first step to ignore compilation time
```

### Comparing `netket-3.9.1/netket/experimental/driver/tdvp_schmitt.py` & `netket-3.9.2/netket/experimental/driver/tdvp_schmitt.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
 # found at github.com/markusschmitt/vmc_jax and licensed according to
 # MIT License, Copyright (c) 2021 Markus Schmitt
 
 
 @partial(jax.jit, static_argnames=("n_samples"))
 def _impl(parameters, n_samples, E_loc, S, rhs_coeff, rcond, rcond_smooth, snr_atol):
     E = stats.statistics(E_loc)
-    ΔE_loc = E_loc.T.reshape(-1, 1) - E.mean
+    ΔE_loc = E_loc.reshape(-1, 1) - E.mean
 
     stack_jacobian = S.mode == "complex"
 
     O = S.O / jnp.sqrt(n_samples)  # already divided by jnp.sqrt(n_s)
     if stack_jacobian:
         O = O.reshape(-1, 2, S.O.shape[-1])
         O = O[:, 0, :] + 1j * O[:, 1, :]
```

### Comparing `netket-3.9.1/netket/experimental/dynamics/__init__.py` & `netket-3.9.2/netket/experimental/dynamics/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/dynamics/_rk_solver.py` & `netket-3.9.2/netket/experimental/dynamics/_rk_solver.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/dynamics/_rk_solver_structures.py` & `netket-3.9.2/netket/experimental/dynamics/_rk_solver_structures.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/dynamics/_rk_tableau.py` & `netket-3.9.2/netket/experimental/dynamics/_rk_tableau.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/hilbert/__init__.py` & `netket-3.9.2/netket/experimental/hilbert/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/hilbert/spin_orbital_fermions.py` & `netket-3.9.2/netket/experimental/hilbert/spin_orbital_fermions.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/hilbert/random/__init__.py` & `netket-3.9.2/netket/experimental/hilbert/random/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/hilbert/random/spin_orbital_fermions.py` & `netket-3.9.2/netket/experimental/hilbert/random/spin_orbital_fermions.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/logging/__init__.py` & `netket-3.9.2/netket/experimental/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/logging/hdf5_log.py` & `netket-3.9.2/netket/experimental/logging/hdf5_log.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/operator/__init__.py` & `netket-3.9.2/netket/experimental/operator/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/operator/_fermion_operator_2nd.py` & `netket-3.9.2/netket/experimental/operator/_fermion_operator_2nd.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/operator/_fermion_operator_2nd_utils.py` & `netket-3.9.2/netket/experimental/operator/_fermion_operator_2nd_utils.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/operator/fermion.py` & `netket-3.9.2/netket/experimental/operator/fermion.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/qsr/__init__.py` & `netket-3.9.2/netket/experimental/qsr/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/qsr/dataset.py` & `netket-3.9.2/netket/experimental/qsr/dataset.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/qsr/driver.py` & `netket-3.9.2/netket/experimental/qsr/driver.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/qsr/logic_helpers.py` & `netket-3.9.2/netket/experimental/qsr/logic_helpers.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/sampler/__init__.py` & `netket-3.9.2/netket/experimental/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/sampler/metropolis_pmap.py` & `netket-3.9.2/netket/experimental/sampler/metropolis_pmap.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/sampler/metropolis_pt.py` & `netket-3.9.2/netket/experimental/sampler/metropolis_pt.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/vqs/__init__.py` & `netket-3.9.2/netket/experimental/vqs/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/experimental/vqs/io.py` & `netket-3.9.2/netket/experimental/vqs/io.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/graph/__init__.py` & `netket-3.9.2/netket/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/graph/_lattice_edge_logic.py` & `netket-3.9.2/netket/graph/_lattice_edge_logic.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/graph/abstract_graph.py` & `netket-3.9.2/netket/graph/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/graph/common_lattices.py` & `netket-3.9.2/netket/graph/common_lattices.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/graph/graph.py` & `netket-3.9.2/netket/graph/graph.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/graph/lattice.py` & `netket-3.9.2/netket/graph/lattice.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/graph/space_group.py` & `netket-3.9.2/netket/graph/space_group.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/__init__.py` & `netket-3.9.2/netket/hilbert/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/abstract_hilbert.py` & `netket-3.9.2/netket/hilbert/abstract_hilbert.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/continuous_hilbert.py` & `netket-3.9.2/netket/hilbert/continuous_hilbert.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/custom_hilbert.py` & `netket-3.9.2/netket/hilbert/custom_hilbert.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/discrete_hilbert.py` & `netket-3.9.2/netket/hilbert/discrete_hilbert.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/doubled_hilbert.py` & `netket-3.9.2/netket/hilbert/doubled_hilbert.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/fock.py` & `netket-3.9.2/netket/hilbert/fock.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/homogeneous.py` & `netket-3.9.2/netket/hilbert/homogeneous.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/particle.py` & `netket-3.9.2/netket/hilbert/particle.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/qubit.py` & `netket-3.9.2/netket/hilbert/qubit.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/spin.py` & `netket-3.9.2/netket/hilbert/spin.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/tensor_hilbert.py` & `netket-3.9.2/netket/hilbert/tensor_hilbert.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/tensor_hilbert_discrete.py` & `netket-3.9.2/netket/hilbert/tensor_hilbert_discrete.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/index/__init__.py` & `netket-3.9.2/netket/hilbert/index/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/index/base.py` & `netket-3.9.2/netket/hilbert/index/base.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/index/constrained.py` & `netket-3.9.2/netket/hilbert/index/constrained.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/index/unconstrained.py` & `netket-3.9.2/netket/hilbert/index/unconstrained.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/random/__init__.py` & `netket-3.9.2/netket/hilbert/random/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/random/base.py` & `netket-3.9.2/netket/hilbert/random/base.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/random/custom.py` & `netket-3.9.2/netket/hilbert/random/custom.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/random/doubled.py` & `netket-3.9.2/netket/hilbert/random/doubled.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/random/fock.py` & `netket-3.9.2/netket/hilbert/random/fock.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/random/particle.py` & `netket-3.9.2/netket/hilbert/random/particle.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/random/qubit.py` & `netket-3.9.2/netket/hilbert/random/qubit.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/random/spin.py` & `netket-3.9.2/netket/hilbert/random/spin.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/hilbert/random/tensor_hilbert.py` & `netket-3.9.2/netket/hilbert/random/tensor_hilbert.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/jax/__init__.py` & `netket-3.9.2/netket/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/jax/_chunk_utils.py` & `netket-3.9.2/netket/jax/_chunk_utils.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/jax/_expect.py` & `netket-3.9.2/netket/jax/_expect.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/jax/_grad.py` & `netket-3.9.2/netket/jax/_grad.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/jax/_math.py` & `netket-3.9.2/netket/jax/_math.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/jax/_scanmap.py` & `netket-3.9.2/netket/jax/_scanmap.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/jax/_vjp.py` & `netket-3.9.2/netket/jax/_vjp.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/jax/_vjp_chunked.py` & `netket-3.9.2/netket/jax/_vjp_chunked.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/jax/_vmap_chunked.py` & `netket-3.9.2/netket/jax/_vmap_chunked.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/jax/utils.py` & `netket-3.9.2/netket/jax/utils.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/jax/_jacobian/default_mode.py` & `netket-3.9.2/netket/jax/_jacobian/default_mode.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/jax/_jacobian/jacobian_dense.py` & `netket-3.9.2/netket/jax/_jacobian/jacobian_dense.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/jax/_jacobian/jacobian_pytree.py` & `netket-3.9.2/netket/jax/_jacobian/jacobian_pytree.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/jax/_jacobian/logic.py` & `netket-3.9.2/netket/jax/_jacobian/logic.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/logging/__init__.py` & `netket-3.9.2/netket/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/logging/json_log.py` & `netket-3.9.2/netket/logging/json_log.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/logging/runtime_log.py` & `netket-3.9.2/netket/logging/runtime_log.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/logging/state_log.py` & `netket-3.9.2/netket/logging/state_log.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/logging/tensorboard.py` & `netket-3.9.2/netket/logging/tensorboard.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/models/__init__.py` & `netket-3.9.2/netket/models/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/models/autoreg.py` & `netket-3.9.2/netket/models/autoreg.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/models/deepset.py` & `netket-3.9.2/netket/models/deepset.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/models/equivariant.py` & `netket-3.9.2/netket/models/equivariant.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/models/fast_autoreg.py` & `netket-3.9.2/netket/models/fast_autoreg.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/models/full_space.py` & `netket-3.9.2/netket/models/full_space.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/models/gaussian.py` & `netket-3.9.2/netket/models/gaussian.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/models/jastrow.py` & `netket-3.9.2/netket/models/jastrow.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/models/mlp.py` & `netket-3.9.2/netket/models/mlp.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/models/mps.py` & `netket-3.9.2/netket/models/mps.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/models/ndm.py` & `netket-3.9.2/netket/models/ndm.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/models/rbm.py` & `netket-3.9.2/netket/models/rbm.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/models/utils.py` & `netket-3.9.2/netket/models/utils.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/nn/__init__.py` & `netket-3.9.2/netket/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/nn/activation.py` & `netket-3.9.2/netket/nn/activation.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/nn/deprecation.py` & `netket-3.9.2/netket/nn/deprecation.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/nn/fast_masked_linear.py` & `netket-3.9.2/netket/nn/fast_masked_linear.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/nn/initializers.py` & `netket-3.9.2/netket/nn/initializers.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/nn/masked_linear.py` & `netket-3.9.2/netket/nn/masked_linear.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/nn/symmetric_linear.py` & `netket-3.9.2/netket/nn/symmetric_linear.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/nn/utils.py` & `netket-3.9.2/netket/nn/utils.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/nn/blocks/__init__.py` & `netket-3.9.2/netket/nn/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/nn/blocks/deepset.py` & `netket-3.9.2/netket/nn/blocks/deepset.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/nn/blocks/mlp.py` & `netket-3.9.2/netket/nn/blocks/mlp.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/nn/blocks/symmetry_sum.py` & `netket-3.9.2/netket/nn/blocks/symmetry_sum.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/__init__.py` & `netket-3.9.2/netket/operator/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_abstract_operator.py` & `netket-3.9.2/netket/operator/_abstract_operator.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_abstract_super_operator.py` & `netket-3.9.2/netket/operator/_abstract_super_operator.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_bose_hubbard.py` & `netket-3.9.2/netket/operator/_bose_hubbard.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_continuous_operator.py` & `netket-3.9.2/netket/operator/_continuous_operator.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_discrete_operator.py` & `netket-3.9.2/netket/operator/_discrete_operator.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_discrete_operator_jax.py` & `netket-3.9.2/netket/operator/_discrete_operator_jax.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_graph_operator.py` & `netket-3.9.2/netket/operator/_graph_operator.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_hamiltonian.py` & `netket-3.9.2/netket/operator/_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_heisenberg.py` & `netket-3.9.2/netket/operator/_heisenberg.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_kinetic.py` & `netket-3.9.2/netket/operator/_kinetic.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_lazy.py` & `netket-3.9.2/netket/operator/_lazy.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_local_liouvillian.py` & `netket-3.9.2/netket/operator/_local_liouvillian.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_potential.py` & `netket-3.9.2/netket/operator/_potential.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_sumoperators.py` & `netket-3.9.2/netket/operator/_sumoperators.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/boson.py` & `netket-3.9.2/netket/operator/boson.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/spin.py` & `netket-3.9.2/netket/operator/spin.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_ising/__init__.py` & `netket-3.9.2/netket/operator/_ising/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_ising/base.py` & `netket-3.9.2/netket/operator/_ising/base.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_ising/jax.py` & `netket-3.9.2/netket/operator/_ising/jax.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_ising/numba.py` & `netket-3.9.2/netket/operator/_ising/numba.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_local_operator/__init__.py` & `netket-3.9.2/netket/operator/_local_operator/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_local_operator/base.py` & `netket-3.9.2/netket/operator/_local_operator/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from typing import Tuple, Union, List, Optional
 
 import numbers
 
 from textwrap import dedent
 
 import numpy as np
+import jax.numpy as jnp
 import numba
 from scipy.sparse import issparse
 
 from netket.hilbert import AbstractHilbert
 from netket.utils.types import DType, Array
 from netket.utils.numbers import dtype as _dtype, is_scalar
 from netket.errors import concrete_or_error, NumbaOperatorGetConnDuringTracingError
@@ -257,15 +258,15 @@
     def __isub__(self, other):
         return self.__iadd__(-other)
 
     def __neg__(self):
         return -1 * self
 
     def __add__(self, other: Union["LocalOperator", numbers.Number]):
-        op = self.copy(dtype=np.promote_types(self.dtype, _dtype(other)))
+        op = self.copy(dtype=jnp.promote_types(self.dtype, _dtype(other)))
         op = op.__iadd__(other)
         return op
 
     def __iadd__(self, other):
         if isinstance(other, LocalOperator):
             if self.hilbert != other.hilbert:
                 return NotImplemented
@@ -305,31 +306,33 @@
         return self.__mul__(1.0 / other)
 
     def __rmul__(self, other):
         return self.__mul__(other)
 
     def __mul__(self, other):
         if isinstance(other, DiscreteOperator):
-            op = self.copy(dtype=np.promote_types(self.dtype, _dtype(other)))
+            op = self.copy(dtype=jnp.promote_types(self.dtype, _dtype(other)))
             return op.__imatmul__(other)
         elif is_scalar(other):
-            op = self.copy(dtype=np.promote_types(self.dtype, _dtype(other)))
+            op = self.copy(dtype=jnp.promote_types(self.dtype, _dtype(other)))
             return op.__imul__(other)
         return NotImplemented
 
     def __imul__(self, other):
         if isinstance(other, DiscreteOperator):
             return self.__imatmul__(other)
         elif is_scalar(other):
             if not np.can_cast(_dtype(other), self.dtype, casting="same_kind"):
                 raise ValueError(
                     f"Cannot add inplace operator of type {type(other)} and "
                     f"dtype {_dtype(other)} to operator with dtype {self.dtype}"
                 )
-            other = np.asarray(other, dtype=np.promote_types(self.dtype, _dtype(other)))
+            other = np.asarray(
+                other, dtype=jnp.promote_types(self.dtype, _dtype(other))
+            )
 
             self._constant *= other
             if np.abs(other) <= self.mel_cutoff:
                 self._operators_dict = {}
             else:
                 for key in self._operators_dict:
                     self._operators_dict[key] = other * self._operators_dict[key]
@@ -349,15 +352,15 @@
             )
 
         return self._op_imatmul_(other)
 
     def _op__matmul__(self, other: "LocalOperator") -> "LocalOperator":
         if not isinstance(other, LocalOperator):
             return NotImplemented
-        op = self.copy(dtype=np.promote_types(self.dtype, _dtype(other)))
+        op = self.copy(dtype=jnp.promote_types(self.dtype, _dtype(other)))
         return op._op_imatmul_(other)
 
     def _op_imatmul_(self, other: "LocalOperator") -> "LocalOperator":
         if not isinstance(other, LocalOperator):
             return NotImplemented
 
         # (α + ∑ᵢAᵢ)(β + ∑ᵢBᵢ) =
```

### Comparing `netket-3.9.1/netket/operator/_local_operator/compile_helpers.py` & `netket-3.9.2/netket/operator/_local_operator/compile_helpers.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_local_operator/convert.py` & `netket-3.9.2/netket/operator/_local_operator/convert.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_local_operator/helpers.py` & `netket-3.9.2/netket/operator/_local_operator/helpers.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_pauli_strings/__init__.py` & `netket-3.9.2/netket/operator/_pauli_strings/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_pauli_strings/base.py` & `netket-3.9.2/netket/operator/_pauli_strings/base.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_pauli_strings/jax.py` & `netket-3.9.2/netket/operator/_pauli_strings/jax.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/operator/_pauli_strings/numba.py` & `netket-3.9.2/netket/operator/_pauli_strings/numba.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/optimizer/__init__.py` & `netket-3.9.2/netket/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/optimizer/linear_operator.py` & `netket-3.9.2/netket/optimizer/linear_operator.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/optimizer/preconditioner.py` & `netket-3.9.2/netket/optimizer/preconditioner.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/optimizer/sr.py` & `netket-3.9.2/netket/optimizer/sr.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/optimizer/qgt/__init__.py` & `netket-3.9.2/netket/optimizer/qgt/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/optimizer/qgt/common.py` & `netket-3.9.2/netket/optimizer/qgt/common.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/optimizer/qgt/default.py` & `netket-3.9.2/netket/optimizer/qgt/default.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/optimizer/qgt/qgt_jacobian_common.py` & `netket-3.9.2/netket/optimizer/qgt/qgt_jacobian_common.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/optimizer/qgt/qgt_jacobian_dense.py` & `netket-3.9.2/netket/optimizer/qgt/qgt_jacobian_dense.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/optimizer/qgt/qgt_jacobian_pytree.py` & `netket-3.9.2/netket/optimizer/qgt/qgt_jacobian_pytree.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/optimizer/qgt/qgt_jacobian_pytree_logic.py` & `netket-3.9.2/netket/optimizer/qgt/qgt_jacobian_pytree_logic.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/optimizer/qgt/qgt_onthefly.py` & `netket-3.9.2/netket/optimizer/qgt/qgt_onthefly.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/optimizer/qgt/qgt_onthefly_logic.py` & `netket-3.9.2/netket/optimizer/qgt/qgt_onthefly_logic.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/optimizer/solver/solvers.py` & `netket-3.9.2/netket/optimizer/solver/solvers.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/sampler/__init__.py` & `netket-3.9.2/netket/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/sampler/autoreg.py` & `netket-3.9.2/netket/sampler/autoreg.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/sampler/base.py` & `netket-3.9.2/netket/sampler/base.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/sampler/exact.py` & `netket-3.9.2/netket/sampler/exact.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/sampler/metropolis.py` & `netket-3.9.2/netket/sampler/metropolis.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/sampler/metropolis_numpy.py` & `netket-3.9.2/netket/sampler/metropolis_numpy.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/sampler/rules/__init__.py` & `netket-3.9.2/netket/sampler/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/sampler/rules/base.py` & `netket-3.9.2/netket/sampler/rules/base.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/sampler/rules/continuous_gaussian.py` & `netket-3.9.2/netket/sampler/rules/continuous_gaussian.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/sampler/rules/custom_numpy.py` & `netket-3.9.2/netket/sampler/rules/custom_numpy.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/sampler/rules/exchange.py` & `netket-3.9.2/netket/sampler/rules/exchange.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/sampler/rules/fixed.py` & `netket-3.9.2/netket/sampler/rules/fixed.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/sampler/rules/hamiltonian.py` & `netket-3.9.2/netket/sampler/rules/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/sampler/rules/hamiltonian_numpy.py` & `netket-3.9.2/netket/sampler/rules/hamiltonian_numpy.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/sampler/rules/langevin.py` & `netket-3.9.2/netket/sampler/rules/langevin.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/sampler/rules/local.py` & `netket-3.9.2/netket/sampler/rules/local.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/sampler/rules/local_numpy.py` & `netket-3.9.2/netket/sampler/rules/local_numpy.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/sampler/rules/multiple.py` & `netket-3.9.2/netket/sampler/rules/multiple.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/sampler/rules/tensor.py` & `netket-3.9.2/netket/sampler/rules/tensor.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/stats/__init__.py` & `netket-3.9.2/netket/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/stats/_autocorr.py` & `netket-3.9.2/netket/stats/_autocorr.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/stats/mc_stats.py` & `netket-3.9.2/netket/stats/mc_stats.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/stats/mc_stats_old.py` & `netket-3.9.2/netket/stats/mc_stats_old.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/stats/mpi_stats.py` & `netket-3.9.2/netket/stats/mpi_stats.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/tools/_common.py` & `netket-3.9.2/netket/tools/_common.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/tools/_cpu_info.py` & `netket-3.9.2/netket/tools/_cpu_info.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/tools/_mpi_info.py` & `netket-3.9.2/netket/tools/_mpi_info.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/tools/check_mpi.py` & `netket-3.9.2/netket/tools/check_mpi.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/tools/info.py` & `netket-3.9.2/netket/tools/info.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/__init__.py` & `netket-3.9.2/netket/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/_dependencies_check.py` & `netket-3.9.2/netket/utils/_dependencies_check.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/array.py` & `netket-3.9.2/netket/utils/array.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/config_flags.py` & `netket-3.9.2/netket/utils/config_flags.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/deprecation.py` & `netket-3.9.2/netket/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/dispatch.py` & `netket-3.9.2/netket/utils/dispatch.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/float.py` & `netket-3.9.2/netket/utils/float.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/history.py` & `netket-3.9.2/netket/utils/history.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/holomorphic.py` & `netket-3.9.2/netket/utils/holomorphic.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/jax.py` & `netket-3.9.2/netket/utils/jax.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/moduletools.py` & `netket-3.9.2/netket/utils/moduletools.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/numbers.py` & `netket-3.9.2/netket/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/optional_deps.py` & `netket-3.9.2/netket/utils/optional_deps.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/partial.py` & `netket-3.9.2/netket/utils/partial.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/seed.py` & `netket-3.9.2/netket/utils/seed.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/static_number.py` & `netket-3.9.2/netket/utils/static_number.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/summation.py` & `netket-3.9.2/netket/utils/summation.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/types.py` & `netket-3.9.2/netket/utils/types.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/version_check.py` & `netket-3.9.2/netket/utils/version_check.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/group/__init__.py` & `netket-3.9.2/netket/utils/group/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/group/_group.py` & `netket-3.9.2/netket/utils/group/_group.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/group/_permutation_group.py` & `netket-3.9.2/netket/utils/group/_permutation_group.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/group/_point_group.py` & `netket-3.9.2/netket/utils/group/_point_group.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/group/_semigroup.py` & `netket-3.9.2/netket/utils/group/_semigroup.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/group/axial.py` & `netket-3.9.2/netket/utils/group/axial.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/group/cubic.py` & `netket-3.9.2/netket/utils/group/cubic.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/group/icosa.py` & `netket-3.9.2/netket/utils/group/icosa.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/group/planar.py` & `netket-3.9.2/netket/utils/group/planar.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/model_frameworks/__init__.py` & `netket-3.9.2/netket/utils/model_frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/model_frameworks/base.py` & `netket-3.9.2/netket/utils/model_frameworks/base.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/model_frameworks/flax.py` & `netket-3.9.2/netket/utils/model_frameworks/flax.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/model_frameworks/haiku.py` & `netket-3.9.2/netket/utils/model_frameworks/haiku.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/model_frameworks/jax.py` & `netket-3.9.2/netket/utils/model_frameworks/jax.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/mpi/__init__.py` & `netket-3.9.2/netket/utils/mpi/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/mpi/mpi.py` & `netket-3.9.2/netket/utils/mpi/mpi.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/mpi/primitives.py` & `netket-3.9.2/netket/utils/mpi/primitives.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/struct/__init__.py` & `netket-3.9.2/netket/utils/struct/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/struct/dataclass.py` & `netket-3.9.2/netket/utils/struct/dataclass.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/utils/struct/utils.py` & `netket-3.9.2/netket/utils/struct/utils.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/__init__.py` & `netket-3.9.2/netket/vqs/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/base.py` & `netket-3.9.2/netket/vqs/base.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/experimental.py` & `netket-3.9.2/netket/vqs/experimental.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/full_summ/__init__.py` & `netket-3.9.2/netket/vqs/full_summ/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/full_summ/expect.py` & `netket-3.9.2/netket/vqs/full_summ/expect.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/full_summ/state.py` & `netket-3.9.2/netket/vqs/full_summ/state.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/mc/__init__.py` & `netket-3.9.2/netket/vqs/mc/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/mc/common.py` & `netket-3.9.2/netket/vqs/mc/common.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/mc/kernels.py` & `netket-3.9.2/netket/vqs/mc/kernels.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/mc/mc_mixed_state/__init__.py` & `netket-3.9.2/netket/vqs/mc/mc_mixed_state/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/mc/mc_mixed_state/expect.py` & `netket-3.9.2/netket/vqs/mc/mc_mixed_state/expect.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/mc/mc_mixed_state/expect_chunked.py` & `netket-3.9.2/netket/vqs/mc/mc_mixed_state/expect_chunked.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/mc/mc_mixed_state/expect_grad_chunked.py` & `netket-3.9.2/netket/vqs/mc/mc_mixed_state/expect_grad_chunked.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/mc/mc_mixed_state/state.py` & `netket-3.9.2/netket/vqs/mc/mc_mixed_state/state.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/mc/mc_state/__init__.py` & `netket-3.9.2/netket/vqs/mc/mc_state/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/mc/mc_state/expect.py` & `netket-3.9.2/netket/vqs/mc/mc_state/expect.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/mc/mc_state/expect_chunked.py` & `netket-3.9.2/netket/vqs/mc/mc_state/expect_chunked.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/mc/mc_state/expect_forces.py` & `netket-3.9.2/netket/vqs/mc/mc_state/expect_forces.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/mc/mc_state/expect_forces_chunked.py` & `netket-3.9.2/netket/vqs/mc/mc_state/expect_forces_chunked.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/mc/mc_state/expect_grad.py` & `netket-3.9.2/netket/vqs/mc/mc_state/expect_grad.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/mc/mc_state/expect_grad_chunked.py` & `netket-3.9.2/netket/vqs/mc/mc_state/expect_grad_chunked.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/netket/vqs/mc/mc_state/state.py` & `netket-3.9.2/netket/vqs/mc/mc_state/state.py`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/.gitignore` & `netket-3.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/LICENSE` & `netket-3.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/README.md` & `netket-3.9.2/README.md`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/pyproject.toml` & `netket-3.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `netket-3.9.1/PKG-INFO` & `netket-3.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NetKet
-Version: 3.9.1
+Version: 3.9.2
 Summary: Netket : Machine Learning toolbox for many-body quantum systems.
 Project-URL: homepage, https://www.netket.org
 Project-URL: documentation, https://netket.readthedocs.io/en/latest/#
 Project-URL: repository, https://github.com/netket/netket
 Project-URL: changelog, https://netket.readthedocs.io/en/latest/docs/changelog.html
 Author: Giuseppe Carleo, Filippo Vicentini, The NetKet authors
 License: Apache 2.0
```

