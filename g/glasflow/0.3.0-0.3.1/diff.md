# Comparing `tmp/glasflow-0.3.0.tar.gz` & `tmp/glasflow-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glasflow-0.3.0.tar", last modified: Fri Aug 18 11:08:25 2023, max compression
+gzip compressed data, was "glasflow-0.3.1.tar", last modified: Tue Apr  2 10:11:46 2024, max compression
```

## Comparing `glasflow-0.3.0.tar` & `glasflow-0.3.1.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.640915 glasflow-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.612914 glasflow-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.620915 glasflow-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-08-18 11:08:15.000000 glasflow-0.3.0/.github/workflows/integration-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-08-18 11:08:15.000000 glasflow-0.3.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-08-18 11:08:15.000000 glasflow-0.3.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-08-18 11:08:15.000000 glasflow-0.3.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-18 11:08:15.000000 glasflow-0.3.0/.github/workflows/tests_nflows_fork.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-18 11:08:15.000000 glasflow-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-18 11:08:15.000000 glasflow-0.3.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-18 11:08:15.000000 glasflow-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-08-18 11:08:15.000000 glasflow-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-08-18 11:08:15.000000 glasflow-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-18 11:08:15.000000 glasflow-0.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-08-18 11:08:25.640915 glasflow-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-18 11:08:15.000000 glasflow-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.620915 glasflow-0.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-08-18 11:08:15.000000 glasflow-0.3.0/examples/conditional_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-08-18 11:08:15.000000 glasflow-0.3.0/examples/moons_nvp_example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.624915 glasflow-0.3.0/glasflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-08-18 11:08:25.000000 glasflow-0.3.0/glasflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-08-18 11:08:25.000000 glasflow-0.3.0/glasflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-18 11:08:25.000000 glasflow-0.3.0/glasflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-18 11:08:25.000000 glasflow-0.3.0/glasflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-18 11:08:25.000000 glasflow-0.3.0/glasflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-18 11:08:15.000000 glasflow-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-08-18 11:08:25.640915 glasflow-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-18 11:08:15.000000 glasflow-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.616914 glasflow-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.624915 glasflow-0.3.0/src/glasflow/
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-08-18 11:08:15.000000 glasflow-0.3.0/src/glasflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.624915 glasflow-0.3.0/src/glasflow/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-18 11:08:15.000000 glasflow-0.3.0/src/glasflow/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-08-18 11:08:15.000000 glasflow-0.3.0/src/glasflow/distributions/resampled.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-08-18 11:08:15.000000 glasflow-0.3.0/src/glasflow/distributions/uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.624915 glasflow-0.3.0/src/glasflow/flows/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-18 11:08:15.000000 glasflow-0.3.0/src/glasflow/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-08-18 11:08:15.000000 glasflow-0.3.0/src/glasflow/flows/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-08-18 11:08:15.000000 glasflow-0.3.0/src/glasflow/flows/coupling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-08-18 11:08:15.000000 glasflow-0.3.0/src/glasflow/flows/nsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-08-18 11:08:15.000000 glasflow-0.3.0/src/glasflow/flows/realnvp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.624915 glasflow-0.3.0/src/glasflow/nets/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-18 11:08:15.000000 glasflow-0.3.0/src/glasflow/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-08-18 11:08:15.000000 glasflow-0.3.0/src/glasflow/nets/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.624915 glasflow-0.3.0/src/glasflow/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-18 11:08:15.000000 glasflow-0.3.0/src/glasflow/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-08-18 11:08:15.000000 glasflow-0.3.0/src/glasflow/transforms/coupling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-18 11:08:15.000000 glasflow-0.3.0/src/glasflow/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-18 11:08:15.000000 glasflow-0.3.0/src/glasflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.616914 glasflow-0.3.0/submodules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.616914 glasflow-0.3.0/submodules/nflows/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.628915 glasflow-0.3.0/submodules/nflows/nflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.628915 glasflow-0.3.0/submodules/nflows/nflows/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/distributions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/distributions/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/distributions/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/distributions/normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/distributions/uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.628915 glasflow-0.3.0/submodules/nflows/nflows/flows/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/flows/autoregressive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/flows/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/flows/realnvp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.628915 glasflow-0.3.0/submodules/nflows/nflows/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.628915 glasflow-0.3.0/submodules/nflows/nflows/nn/nde/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/nn/nde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14282 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/nn/nde/made.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.628915 glasflow-0.3.0/submodules/nflows/nflows/nn/nets/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/nn/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/nn/nets/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/nn/nets/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.632915 glasflow-0.3.0/submodules/nflows/nflows/transforms/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.632915 glasflow-0.3.0/submodules/nflows/nflows/transforms/UMNN/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/UMNN/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/UMNN/autoregressive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/UMNN/coupling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/UMNN/monotonicnormalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16261 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/autoregressive.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/coupling.py
--rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/lu.py
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/made.py
--rw-r--r--   0 runner    (1001) docker     (123)    16106 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/nonlinearities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/orthogonal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/permutations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/reshape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.636915 glasflow-0.3.0/submodules/nflows/nflows/transforms/splines/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/splines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/splines/cubic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/splines/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/splines/quadratic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/splines/rational_quadratic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/transforms/svd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.636915 glasflow-0.3.0/submodules/nflows/nflows/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/utils/torchutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/utils/typechecks.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-18 11:08:16.000000 glasflow-0.3.0/submodules/nflows/nflows/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.636915 glasflow-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-18 11:08:15.000000 glasflow-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.636915 glasflow-0.3.0/tests/test_distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-08-18 11:08:15.000000 glasflow-0.3.0/tests/test_distributions/test_resampled.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-08-18 11:08:15.000000 glasflow-0.3.0/tests/test_distributions/test_uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.636915 glasflow-0.3.0/tests/test_flows/
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-08-18 11:08:15.000000 glasflow-0.3.0/tests/test_flows/test_coupling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-08-18 11:08:15.000000 glasflow-0.3.0/tests/test_flows/test_nsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-08-18 11:08:15.000000 glasflow-0.3.0/tests/test_flows/test_realnvp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-18 11:08:15.000000 glasflow-0.3.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-18 11:08:15.000000 glasflow-0.3.0/tests/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.636915 glasflow-0.3.0/tests/test_nets/
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-08-18 11:08:15.000000 glasflow-0.3.0/tests/test_nets/test_mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 11:08:25.640915 glasflow-0.3.0/tests/test_transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-18 11:08:15.000000 glasflow-0.3.0/tests/test_transforms/test_coupling_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-18 11:08:15.000000 glasflow-0.3.0/tests/test_transforms/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-18 11:08:15.000000 glasflow-0.3.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.296942 glasflow-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.276942 glasflow-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.280942 glasflow-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-02 10:11:41.000000 glasflow-0.3.1/.github/workflows/integration-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-02 10:11:41.000000 glasflow-0.3.1/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-02 10:11:41.000000 glasflow-0.3.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-02 10:11:41.000000 glasflow-0.3.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-02 10:11:41.000000 glasflow-0.3.1/.github/workflows/tests_nflows_fork.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-02 10:11:41.000000 glasflow-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-02 10:11:41.000000 glasflow-0.3.1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-02 10:11:41.000000 glasflow-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-02 10:11:41.000000 glasflow-0.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-02 10:11:41.000000 glasflow-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-02 10:11:41.000000 glasflow-0.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-02 10:11:46.296942 glasflow-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-02 10:11:41.000000 glasflow-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.280942 glasflow-0.3.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-04-02 10:11:41.000000 glasflow-0.3.1/examples/conditional_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-04-02 10:11:41.000000 glasflow-0.3.1/examples/moons_nvp_example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.292942 glasflow-0.3.1/glasflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-02 10:11:46.000000 glasflow-0.3.1/glasflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-02 10:11:46.000000 glasflow-0.3.1/glasflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:11:46.000000 glasflow-0.3.1/glasflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-02 10:11:46.000000 glasflow-0.3.1/glasflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 10:11:46.000000 glasflow-0.3.1/glasflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-02 10:11:41.000000 glasflow-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-02 10:11:46.296942 glasflow-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-02 10:11:41.000000 glasflow-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.276942 glasflow-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.280942 glasflow-0.3.1/src/glasflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-02 10:11:41.000000 glasflow-0.3.1/src/glasflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.280942 glasflow-0.3.1/src/glasflow/distributions/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-02 10:11:41.000000 glasflow-0.3.1/src/glasflow/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-02 10:11:41.000000 glasflow-0.3.1/src/glasflow/distributions/resampled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-02 10:11:41.000000 glasflow-0.3.1/src/glasflow/distributions/uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.280942 glasflow-0.3.1/src/glasflow/flows/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 10:11:41.000000 glasflow-0.3.1/src/glasflow/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-02 10:11:41.000000 glasflow-0.3.1/src/glasflow/flows/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-04-02 10:11:41.000000 glasflow-0.3.1/src/glasflow/flows/coupling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-02 10:11:41.000000 glasflow-0.3.1/src/glasflow/flows/nsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-02 10:11:41.000000 glasflow-0.3.1/src/glasflow/flows/realnvp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.284942 glasflow-0.3.1/src/glasflow/nets/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-02 10:11:41.000000 glasflow-0.3.1/src/glasflow/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-02 10:11:41.000000 glasflow-0.3.1/src/glasflow/nets/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.284942 glasflow-0.3.1/src/glasflow/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-02 10:11:41.000000 glasflow-0.3.1/src/glasflow/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-02 10:11:41.000000 glasflow-0.3.1/src/glasflow/transforms/coupling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-02 10:11:41.000000 glasflow-0.3.1/src/glasflow/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-02 10:11:41.000000 glasflow-0.3.1/src/glasflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.276942 glasflow-0.3.1/submodules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.276942 glasflow-0.3.1/submodules/nflows/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.284942 glasflow-0.3.1/submodules/nflows/nflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.284942 glasflow-0.3.1/submodules/nflows/nflows/distributions/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/distributions/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/distributions/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/distributions/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/distributions/normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/distributions/uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.284942 glasflow-0.3.1/submodules/nflows/nflows/flows/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/flows/autoregressive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/flows/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/flows/realnvp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.284942 glasflow-0.3.1/submodules/nflows/nflows/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.284942 glasflow-0.3.1/submodules/nflows/nflows/nn/nde/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/nn/nde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14282 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/nn/nde/made.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.284942 glasflow-0.3.1/submodules/nflows/nflows/nn/nets/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/nn/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/nn/nets/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/nn/nets/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.288942 glasflow-0.3.1/submodules/nflows/nflows/transforms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.288942 glasflow-0.3.1/submodules/nflows/nflows/transforms/UMNN/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/UMNN/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/UMNN/autoregressive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/UMNN/coupling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/UMNN/monotonicnormalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16261 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/autoregressive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18613 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/coupling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/lu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/made.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16106 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/nonlinearities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/orthogonal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/permutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/qr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/reshape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.288942 glasflow-0.3.1/submodules/nflows/nflows/transforms/splines/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/splines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/splines/cubic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/splines/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/splines/quadratic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/splines/rational_quadratic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/transforms/svd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.292942 glasflow-0.3.1/submodules/nflows/nflows/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/utils/torchutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/utils/typechecks.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 10:11:42.000000 glasflow-0.3.1/submodules/nflows/nflows/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.292942 glasflow-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-02 10:11:41.000000 glasflow-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.292942 glasflow-0.3.1/tests/test_distributions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-02 10:11:41.000000 glasflow-0.3.1/tests/test_distributions/test_resampled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-04-02 10:11:41.000000 glasflow-0.3.1/tests/test_distributions/test_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.292942 glasflow-0.3.1/tests/test_flows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-02 10:11:41.000000 glasflow-0.3.1/tests/test_flows/test_coupling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-02 10:11:41.000000 glasflow-0.3.1/tests/test_flows/test_nsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-02 10:11:41.000000 glasflow-0.3.1/tests/test_flows/test_realnvp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-02 10:11:41.000000 glasflow-0.3.1/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-02 10:11:41.000000 glasflow-0.3.1/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.292942 glasflow-0.3.1/tests/test_nets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-02 10:11:41.000000 glasflow-0.3.1/tests/test_nets/test_mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:11:46.292942 glasflow-0.3.1/tests/test_transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-02 10:11:41.000000 glasflow-0.3.1/tests/test_transforms/test_coupling_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-02 10:11:41.000000 glasflow-0.3.1/tests/test_transforms/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-02 10:11:41.000000 glasflow-0.3.1/tests/test_utils.py
```

### Comparing `glasflow-0.3.0/.github/workflows/integration-tests.yml` & `glasflow-0.3.1/.github/workflows/integration-tests.yml`

 * *Files 7% similar despite different names*

```diff
@@ -23,19 +23,19 @@
         os: [macOS, Ubuntu, Windows]
         python-version: ["3.7", "3.8", "3.9", "3.10"]
         use-nflows: [True, False]
     runs-on: ${{ matrix.os }}-latest
 
     steps:
     - name: Checkout repository and submodules
-      uses: actions/checkout@v2
+      uses: actions/checkout@v4
       with:
         submodules: recursive
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[dev]
     - name: Optionally install nflows
```

### Comparing `glasflow-0.3.0/.github/workflows/lint.yml` & `glasflow-0.3.1/.github/workflows/lint.yml`

 * *Files 10% similar despite different names*

```diff
@@ -11,26 +11,27 @@
   cancel-in-progress: true
 
 jobs:
   black:
     name: Black
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v4
       - uses: psf/black@stable
         with:
           jupyter: true
           options: "--check --diff"
+          version: "24.2"
   flake8:
     name: Flake8
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install flake8
     - name: Lint with flake8
```

### Comparing `glasflow-0.3.0/.github/workflows/publish-to-pypi.yml` & `glasflow-0.3.1/.github/workflows/publish-to-pypi.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 jobs:
   build-n-publish:
     name: Build and publish Python 🐍 distributions 📦 to PyPI
     runs-on: ubuntu-latest
     steps:
     - name: Checkout repository and submodules
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
       with:
         submodules: recursive
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.x"
     - name: Install pypa/build
       run: >-
         python -m
         pip install
         build
```

### Comparing `glasflow-0.3.0/.github/workflows/tests.yml` & `glasflow-0.3.1/.github/workflows/tests.yml`

 * *Files 7% similar despite different names*

```diff
@@ -23,19 +23,19 @@
         os: [macOS, Ubuntu, Windows]
         python-version: ["3.7", "3.8", "3.9", "3.10"]
         use-nflows: [True, False]
     runs-on: ${{ matrix.os }}-latest
 
     steps:
     - name: Checkout repository and submodules
-      uses: actions/checkout@v2
+      uses: actions/checkout@v4
       with:
         submodules: recursive
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[dev]
     - name: Optionally install nflows
```

### Comparing `glasflow-0.3.0/.github/workflows/tests_nflows_fork.yml` & `glasflow-0.3.1/.github/workflows/tests_nflows_fork.yml`

 * *Files 12% similar despite different names*

```diff
@@ -18,19 +18,19 @@
     strategy:
       fail-fast: false
       matrix:
         os: [macOS, Ubuntu, Windows]
     runs-on: ${{ matrix.os }}-latest
     steps:
     - name: Checkout repository and submodules
-      uses: actions/checkout@v2
+      uses: actions/checkout@v4
       with:
         submodules: recursive
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v5
       with:
         python-version: '3.10'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[nflows-test]
     - name: Test with pytest
```

### Comparing `glasflow-0.3.0/.gitignore` & `glasflow-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/CHANGELOG.md` & `glasflow-0.3.1/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.3.1]
+
+### Fixed
+
+- Addressed a deprecation warning in the `nflows` submodule when using LU decomposition (https://github.com/uofgravity/nflows/pull/10, https://github.com/uofgravity/glasflow/pull/57)
+
 ## [0.3.0]
 
 ### Added
 
 - Keyword arguments passed to `glasflow.transform.coupling.AffineCouplingTransform` are now propogated to the parent class. ([#51](https://github.com/uofgravity/glasflow/pull/51))
 - Add support `scale_activation` to `glasflow.transform.coupling.AffineCouplingTransform` and set the default to `nflows_general`. ([#52](https://github.com/uofgravity/glasflow/pull/52), [#54](https://github.com/uofgravity/glasflow/pull/54))
 
@@ -60,13 +66,14 @@
 ### Added
 
 - Add `RealNVP`
 - Add `CouplingNSF` (Coupling Neural Spline Flow)
 - Add `nflows` submodule that replaces `nflows` dependency
 - Add option for user-defined masks in coupling-based flows
 
-[Unreleased]: https://github.com/uofgravity/glasflow/compare/v0.3.0...HEAD
+[Unreleased]: https://github.com/uofgravity/glasflow/compare/v0.3.1...HEAD
+[0.3.1]: https://github.com/uofgravity/glasflow/compare/v0.3.0...v0.3.1
 [0.3.0]: https://github.com/uofgravity/glasflow/compare/v0.2.0...v0.3.0
 [0.2.0]: https://github.com/uofgravity/glasflow/compare/v0.1.2...v0.2.0
 [0.1.2]: https://github.com/uofgravity/glasflow/compare/v0.1.1...v0.1.2
 [0.1.1]: https://github.com/uofgravity/glasflow/compare/v0.1.0...v0.1.1
 [0.1.0]: https://github.com/uofgravity/glasflow/releases/tag/v0.1.0
```

### Comparing `glasflow-0.3.0/CONTRIBUTING.md` & `glasflow-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/LICENSE.md` & `glasflow-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/PKG-INFO` & `glasflow-0.3.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: glasflow
-Version: 0.3.0
-Summary: Normalising flows using nflows
-Home-page: https://github.com/uofgravity/glasflow
-Author: IGR
-Author-email: m.williams.4@research.gla.ac.uk
-License: MIT
-Keywords: normalising flows,machine learning
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: nflows
-Provides-Extra: nflows-test
-Provides-Extra: dev
-Provides-Extra: examples
-License-File: LICENSE.md
-
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7108558.svg)](https://doi.org/10.5281/zenodo.7108558)
 [![PyPI](https://img.shields.io/pypi/v/glasflow)](https://pypi.org/project/glasflow/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/glasflow.svg)](https://anaconda.org/conda-forge/glasflow)
 
 # Glasflow
 
 glasflow is a Python library containing a collection of [Normalizing flows](https://arxiv.org/abs/1912.02762) using [PyTorch](https://pytorch.org). It builds upon [nflows](https://github.com/bayesiains/nflows).
```

### Comparing `glasflow-0.3.0/examples/conditional_example.ipynb` & `glasflow-0.3.1/examples/conditional_example.ipynb`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/examples/moons_nvp_example.ipynb` & `glasflow-0.3.1/examples/moons_nvp_example.ipynb`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/glasflow.egg-info/SOURCES.txt` & `glasflow-0.3.1/glasflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/setup.cfg` & `glasflow-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/src/glasflow/__init__.py` & `glasflow-0.3.1/src/glasflow/__init__.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/src/glasflow/distributions/resampled.py` & `glasflow-0.3.1/src/glasflow/distributions/resampled.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Distributions that include Learned Accept/Reject Sampling (LARS)."""
+
 from typing import Callable, Union
 
 from glasflow.nflows.distributions import Distribution
 from glasflow.nflows.utils import torchutils
 from glasflow.utils import get_torch_size
 import numpy as np
 import torch
```

### Comparing `glasflow-0.3.0/src/glasflow/distributions/uniform.py` & `glasflow-0.3.1/src/glasflow/distributions/uniform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Multidimensional uniform distribution.
 """
+
 from typing import Union
 
 from glasflow.nflows.distributions import Distribution
 import torch
 
 
 class MultivariateUniform(Distribution):
```

### Comparing `glasflow-0.3.0/src/glasflow/flows/base.py` & `glasflow-0.3.1/src/glasflow/flows/base.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/src/glasflow/flows/coupling.py` & `glasflow-0.3.1/src/glasflow/flows/coupling.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/src/glasflow/flows/nsf.py` & `glasflow-0.3.1/src/glasflow/flows/nsf.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/src/glasflow/flows/realnvp.py` & `glasflow-0.3.1/src/glasflow/flows/realnvp.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/src/glasflow/nets/mlp.py` & `glasflow-0.3.1/src/glasflow/nets/mlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Multi-layer perceptrons"""
+
 from typing import Callable, List, Optional, Union
 import numpy as np
 
 import torch
 from torch import nn
 import torch.nn.functional as F
```

### Comparing `glasflow-0.3.0/src/glasflow/transforms/coupling.py` & `glasflow-0.3.1/src/glasflow/transforms/coupling.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/src/glasflow/transforms/utils.py` & `glasflow-0.3.1/src/glasflow/transforms/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for the transforms submodule"""
+
 from typing import Callable, Union
 import torch
 import torch.nn.functional as F
 
 
 SCALE_ACTIVATIONS = dict(
     nflows=lambda x: torch.sigmoid(x + 2) + 1e-3,
```

### Comparing `glasflow-0.3.0/src/glasflow/utils.py` & `glasflow-0.3.1/src/glasflow/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """General utilities"""
+
 from collections.abc import Iterable
 from typing import Union
 
 import torch
 
 
 def get_torch_size(shape: Union[int, Iterable]) -> torch.Size:
```

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/distributions/base.py` & `glasflow-0.3.1/submodules/nflows/nflows/distributions/base.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/distributions/discrete.py` & `glasflow-0.3.1/submodules/nflows/nflows/distributions/discrete.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/distributions/mixture.py` & `glasflow-0.3.1/submodules/nflows/nflows/distributions/mixture.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/distributions/normal.py` & `glasflow-0.3.1/submodules/nflows/nflows/distributions/normal.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/distributions/uniform.py` & `glasflow-0.3.1/submodules/nflows/nflows/distributions/uniform.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/flows/autoregressive.py` & `glasflow-0.3.1/submodules/nflows/nflows/flows/autoregressive.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/flows/base.py` & `glasflow-0.3.1/submodules/nflows/nflows/flows/base.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/flows/realnvp.py` & `glasflow-0.3.1/submodules/nflows/nflows/flows/realnvp.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/nn/nde/made.py` & `glasflow-0.3.1/submodules/nflows/nflows/nn/nde/made.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/nn/nets/mlp.py` & `glasflow-0.3.1/submodules/nflows/nflows/nn/nets/mlp.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/nn/nets/resnet.py` & `glasflow-0.3.1/submodules/nflows/nflows/nn/nets/resnet.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/UMNN/autoregressive.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/UMNN/autoregressive.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/UMNN/coupling.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/UMNN/coupling.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/UMNN/monotonicnormalizer.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/UMNN/monotonicnormalizer.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/__init__.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/autoregressive.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/autoregressive.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/base.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/base.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/conv.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/conv.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/coupling.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/coupling.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/linear.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/linear.py`

 * *Files 6% similar despite different names*

```diff
@@ -175,16 +175,16 @@
             logabsdet = O(D^3)
         where:
             D = num of features
             N = num of inputs
         """
         batch_size = inputs.shape[0]
         outputs = inputs - self.bias
-        lu, lu_pivots = torch.lu(self._weight)
-        outputs = torch.lu_solve(outputs.t(), lu, lu_pivots).t()
+        lu, lu_pivots = torch.linalg.lu_factor(self._weight)
+        outputs = torch.linalg.lu_solve(lu, lu_pivots, outputs.t()).t()
         # The linear-system solver returns the LU decomposition of the weights, which we
         # can use to obtain the log absolute determinant directly.
         logabsdet = -torch.sum(torch.log(torch.abs(torch.diag(lu))))
         logabsdet = logabsdet * outputs.new_ones(batch_size)
         return outputs, logabsdet
 
     def weight(self):
@@ -208,16 +208,16 @@
             inverse = O(D^3)
             logabsdet = O(D)
         where:
             D = num of features
         """
         # If both weight inverse and logabsdet are needed, it's cheaper to compute both together.
         identity = torch.eye(self.features, self.features)
-        lu, lu_pivots = torch.lu(self._weight)
-        weight_inv = torch.lu_solve(identity, lu, lu_pivots)
+        lu, lu_pivots = torch.linalg.lu_factor(self._weight)
+        weight_inv = torch.linalg.lu_solve(lu, lu_pivots, identity)
         logabsdet = torch.sum(torch.log(torch.abs(torch.diag(lu))))
         return weight_inv, logabsdet
 
     def logabsdet(self):
         """Cost:
             logabsdet = O(D^3)
         where:
```

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/lu.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/lu.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/made.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/made.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/nonlinearities.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/nonlinearities.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/normalization.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/normalization.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/orthogonal.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/orthogonal.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/permutations.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/permutations.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/qr.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/qr.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/reshape.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/reshape.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/splines/cubic.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/splines/cubic.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/splines/linear.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/splines/linear.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/splines/quadratic.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/splines/quadratic.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/splines/rational_quadratic.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/splines/rational_quadratic.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/standard.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/standard.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/transforms/svd.py` & `glasflow-0.3.1/submodules/nflows/nflows/transforms/svd.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/submodules/nflows/nflows/utils/torchutils.py` & `glasflow-0.3.1/submodules/nflows/nflows/utils/torchutils.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/tests/test_distributions/test_resampled.py` & `glasflow-0.3.1/tests/test_distributions/test_resampled.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for the resampled distributions"""
+
 from glasflow.distributions.resampled import ResampledGaussian
 from glasflow.nflows.distributions import StandardNormal
 from glasflow.nets.mlp import MLP
 import pytest
 import torch
```

### Comparing `glasflow-0.3.0/tests/test_distributions/test_uniform.py` & `glasflow-0.3.1/tests/test_distributions/test_uniform.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/tests/test_flows/test_coupling.py` & `glasflow-0.3.1/tests/test_flows/test_coupling.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/tests/test_flows/test_nsf.py` & `glasflow-0.3.1/tests/test_flows/test_nsf.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/tests/test_flows/test_realnvp.py` & `glasflow-0.3.1/tests/test_flows/test_realnvp.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/tests/test_import.py` & `glasflow-0.3.1/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/tests/test_nets/test_mlp.py` & `glasflow-0.3.1/tests/test_nets/test_mlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for the MLP submodule"""
+
 from unittest.mock import create_autospec
 from glasflow.nets.mlp import MLP
 import pytest
 import torch
 
 
 @pytest.fixture
```

### Comparing `glasflow-0.3.0/tests/test_transforms/test_coupling_transforms.py` & `glasflow-0.3.1/tests/test_transforms/test_coupling_transforms.py`

 * *Files identical despite different names*

### Comparing `glasflow-0.3.0/tests/test_transforms/test_utils.py` & `glasflow-0.3.1/tests/test_transforms/test_utils.py`

 * *Files identical despite different names*

