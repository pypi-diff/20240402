# Comparing `tmp/hpc-beeflow-0.1.7.tar.gz` & `tmp/hpc_beeflow-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpc-beeflow-0.1.7.tar", max compression
+gzip compressed data, was "hpc_beeflow-0.1.8.tar", max compression
```

## Comparing `hpc-beeflow-0.1.7.tar` & `hpc_beeflow-0.1.8.tar`

### file list

```diff
@@ -1,303 +1,302 @@
--rw-r--r--   0        0        0     1477 2024-03-28 22:16:36.348299 hpc-beeflow-0.1.7/LICENSE
--rw-r--r--   0        0        0     5235 2024-03-29 16:50:01.342051 hpc-beeflow-0.1.7/README.rst
--rw-r--r--   0        0        0      122 2024-03-28 22:16:36.349367 hpc-beeflow-0.1.7/beeflow/client/README.md
--rw-r--r--   0        0        0    22324 2024-03-29 16:50:01.343590 hpc-beeflow-0.1.7/beeflow/client/bee_client.py
--rw-r--r--   0        0        0    23683 2024-03-29 16:50:01.344218 hpc-beeflow-0.1.7/beeflow/client/core.py
--rw-r--r--   0        0        0     8036 2024-03-28 22:16:36.350389 hpc-beeflow-0.1.7/beeflow/cloud_launcher.py
--rw-r--r--   0        0        0      234 2024-03-28 22:16:36.350628 hpc-beeflow-0.1.7/beeflow/common/README.md
--rw-r--r--   0        0        0      459 2024-03-28 22:16:36.350800 hpc-beeflow-0.1.7/beeflow/common/api.py
--rw-r--r--   0        0        0    11473 2024-03-28 22:16:36.351063 hpc-beeflow-0.1.7/beeflow/common/build/README.md
--rw-r--r--   0        0        0     5116 2024-03-29 16:50:01.344806 hpc-beeflow-0.1.7/beeflow/common/build/build_driver.py
--rw-r--r--   0        0        0    19130 2024-03-29 16:50:01.345249 hpc-beeflow-0.1.7/beeflow/common/build/container_drivers.py
--rw-r--r--   0        0        0      733 2024-03-29 16:50:01.345495 hpc-beeflow-0.1.7/beeflow/common/build/utils.py
--rw-r--r--   0        0        0     3534 2024-03-29 16:50:01.346124 hpc-beeflow-0.1.7/beeflow/common/build_interfaces.py
--rw-r--r--   0        0        0      163 2024-03-28 22:16:36.352417 hpc-beeflow-0.1.7/beeflow/common/celery.py
--rw-r--r--   0        0        0      285 2024-03-28 22:16:36.352577 hpc-beeflow-0.1.7/beeflow/common/cli.py
--rw-r--r--   0        0        0     3023 2024-03-28 22:16:36.352758 hpc-beeflow-0.1.7/beeflow/common/cli_connection.py
--rw-r--r--   0        0        0     2542 2024-03-28 22:16:36.353108 hpc-beeflow-0.1.7/beeflow/common/cloud/README.md
--rw-r--r--   0        0        0      830 2024-03-28 22:16:36.353287 hpc-beeflow-0.1.7/beeflow/common/cloud/__init__.py
--rw-r--r--   0        0        0     1166 2024-03-28 22:16:36.353541 hpc-beeflow-0.1.7/beeflow/common/cloud/chameleoncloud.py
--rw-r--r--   0        0        0      175 2024-03-28 22:16:36.353879 hpc-beeflow-0.1.7/beeflow/common/cloud/cloud.py
--rw-r--r--   0        0        0       42 2024-03-28 22:16:36.354153 hpc-beeflow-0.1.7/beeflow/common/cloud/constants.py
--rw-r--r--   0        0        0     1599 2024-03-28 22:16:36.354427 hpc-beeflow-0.1.7/beeflow/common/cloud/google.py
--rw-r--r--   0        0        0     1093 2024-03-28 22:16:36.354593 hpc-beeflow-0.1.7/beeflow/common/cloud/openstack.py
--rw-r--r--   0        0        0      784 2024-03-28 22:16:36.354764 hpc-beeflow-0.1.7/beeflow/common/cloud/provider.py
--rw-r--r--   0        0        0    22522 2024-03-29 16:50:01.346853 hpc-beeflow-0.1.7/beeflow/common/config_driver.py
--rw-r--r--   0        0        0     5891 2024-03-28 22:16:36.355303 hpc-beeflow-0.1.7/beeflow/common/config_validator.py
--rw-r--r--   0        0        0     2420 2024-03-28 22:16:36.355477 hpc-beeflow-0.1.7/beeflow/common/connection.py
--rw-r--r--   0        0        0      947 2024-03-28 22:16:36.355625 hpc-beeflow-0.1.7/beeflow/common/container_path.py
--rw-r--r--   0        0        0     7084 2024-03-29 16:50:01.347322 hpc-beeflow-0.1.7/beeflow/common/crt/charliecloud_driver.py
--rw-r--r--   0        0        0     1487 2024-03-28 22:16:36.356338 hpc-beeflow-0.1.7/beeflow/common/crt/crt_driver.py
--rw-r--r--   0        0        0     1760 2024-03-29 16:50:01.347773 hpc-beeflow-0.1.7/beeflow/common/crt/singularity_driver.py
--rw-r--r--   0        0        0     1551 2024-03-28 22:16:36.356875 hpc-beeflow-0.1.7/beeflow/common/crt_interface.py
--rw-r--r--   0        0        0     2486 2024-03-28 22:16:36.357355 hpc-beeflow-0.1.7/beeflow/common/db/bdb.py
--rw-r--r--   0        0        0     1675 2024-03-28 22:16:36.357568 hpc-beeflow-0.1.7/beeflow/common/db/sched_db.py
--rw-r--r--   0        0        0     5075 2024-03-28 22:16:36.357757 hpc-beeflow-0.1.7/beeflow/common/db/tm_db.py
--rw-r--r--   0        0        0     8816 2024-03-28 22:16:36.358119 hpc-beeflow-0.1.7/beeflow/common/db/wfm_db.py
--rw-r--r--   0        0        0     2133 2024-03-28 22:16:36.358379 hpc-beeflow-0.1.7/beeflow/common/expr.py
--rw-r--r--   0        0        0     5924 2024-03-28 22:16:36.358925 hpc-beeflow-0.1.7/beeflow/common/gdb/DESIGN.md
--rw-r--r--   0        0        0     8320 2024-03-29 16:50:01.348375 hpc-beeflow-0.1.7/beeflow/common/gdb/gdb_driver.py
--rw-r--r--   0        0        0    23439 2024-03-29 16:50:01.348932 hpc-beeflow-0.1.7/beeflow/common/gdb/neo4j_cypher.py
--rw-r--r--   0        0        0    22892 2024-03-29 16:50:01.349407 hpc-beeflow-0.1.7/beeflow/common/gdb/neo4j_driver.py
--rw-r--r--   0        0        0     9736 2024-03-28 22:16:36.359945 hpc-beeflow-0.1.7/beeflow/common/gdb_interface.py
--rw-r--r--   0        0        0     4222 2024-03-29 16:50:01.349743 hpc-beeflow-0.1.7/beeflow/common/integration/generated_workflows.py
--rw-r--r--   0        0        0     8370 2024-03-29 16:50:01.349960 hpc-beeflow-0.1.7/beeflow/common/integration/utils.py
--rw-r--r--   0        0        0    11162 2024-03-29 16:50:01.350145 hpc-beeflow-0.1.7/beeflow/common/integration_test.py
--rw-r--r--   0        0        0      642 2024-03-28 22:16:36.360815 hpc-beeflow-0.1.7/beeflow/common/log.py
--rw-r--r--   0        0        0       16 2024-03-28 22:16:36.361052 hpc-beeflow-0.1.7/beeflow/common/parser/.gitignore
--rw-r--r--   0        0        0     2614 2024-03-28 22:16:36.361301 hpc-beeflow-0.1.7/beeflow/common/parser/README.md
--rw-r--r--   0        0        0      102 2024-03-28 22:16:36.361545 hpc-beeflow-0.1.7/beeflow/common/parser/__init__.py
--rw-r--r--   0        0        0    15464 2024-03-29 16:50:01.350621 hpc-beeflow-0.1.7/beeflow/common/parser/parser.py
--rw-r--r--   0        0        0     2162 2024-03-28 22:16:36.362002 hpc-beeflow-0.1.7/beeflow/common/paths.py
--rw-r--r--   0        0        0      450 2024-03-28 22:16:36.362142 hpc-beeflow-0.1.7/beeflow/common/states.py
--rw-r--r--   0        0        0      493 2024-03-28 22:16:36.362369 hpc-beeflow-0.1.7/beeflow/common/tab_completion.py
--rw-r--r--   0        0        0     1643 2024-03-28 22:16:36.362570 hpc-beeflow-0.1.7/beeflow/common/validation.py
--rw-r--r--   0        0        0    12396 2024-03-29 16:50:01.351045 hpc-beeflow-0.1.7/beeflow/common/wf_data.py
--rw-r--r--   0        0        0    11679 2024-03-29 16:50:01.351480 hpc-beeflow-0.1.7/beeflow/common/wf_interface.py
--rw-r--r--   0        0        0     1522 2024-03-28 22:16:36.363159 hpc-beeflow-0.1.7/beeflow/common/wf_profiler.py
--rw-r--r--   0        0        0      493 2024-03-28 22:16:36.363554 hpc-beeflow-0.1.7/beeflow/common/worker/README.md
--rw-r--r--   0        0        0      597 2024-03-28 22:16:36.363810 hpc-beeflow-0.1.7/beeflow/common/worker/__init__.py
--rw-r--r--   0        0        0     5048 2024-03-28 22:16:36.364014 hpc-beeflow-0.1.7/beeflow/common/worker/flux_worker.py
--rw-r--r--   0        0        0     2570 2024-03-28 22:16:36.364334 hpc-beeflow-0.1.7/beeflow/common/worker/lsf_worker.py
--rw-r--r--   0        0        0     1731 2024-03-28 22:16:36.364550 hpc-beeflow-0.1.7/beeflow/common/worker/simple_worker.py
--rw-r--r--   0        0        0    10635 2024-03-29 16:50:01.352492 hpc-beeflow-0.1.7/beeflow/common/worker/slurm_worker.py
--rw-r--r--   0        0        0     2899 2024-03-28 22:16:36.364935 hpc-beeflow-0.1.7/beeflow/common/worker/worker.py
--rw-r--r--   0        0        0     1794 2024-03-28 22:16:36.365103 hpc-beeflow-0.1.7/beeflow/common/worker_interface.py
--rw-r--r--   0        0        0     4301 2024-03-28 22:16:36.365494 hpc-beeflow-0.1.7/beeflow/data/cloud_templates/dora.jinja
--rw-r--r--   0        0        0      866 2024-03-28 22:16:36.365754 hpc-beeflow-0.1.7/beeflow/data/cloud_templates/dora.yaml
--rw-r--r--   0        0        0      414 2024-03-28 22:16:36.366199 hpc-beeflow-0.1.7/beeflow/data/cwl/README.md
--rw-r--r--   0        0        0     1281 2024-03-28 22:16:36.366556 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/README.md
--rw-r--r--   0        0        0      315 2024-03-28 22:16:36.366812 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/README.md
--rw-r--r--   0        0        0      418 2024-03-28 22:16:36.366971 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/blast.yml
--rw-r--r--   0        0        0      423 2024-03-28 22:16:36.367127 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/blast_output.cwl
--rw-r--r--   0        0        0      300 2024-03-28 22:16:36.367264 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/blast_output_err.cwl
--rw-r--r--   0        0        0      410 2024-03-28 22:16:36.367399 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/blast_split.cwl
--rw-r--r--   0        0        0     2009 2024-03-28 22:16:36.367628 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/blast_wf.cwl
--rw-r--r--   0        0        0      559 2024-03-28 22:16:36.367934 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/blast_worker001.cwl
--rw-r--r--   0        0        0      559 2024-03-28 22:16:36.368162 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/blast_worker002.cwl
--rwxr-xr-x   0        0        0   930997 2024-03-28 22:16:36.372172 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/input/small.fasta
--rw-r--r--   0        0        0       77 2024-03-28 22:16:36.372485 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/cat-grep-fail/README.md
--rw-r--r--   0        0        0      258 2024-03-28 22:16:36.372649 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/cat-grep-fail/cat.cwl
--rw-r--r--   0        0        0      272 2024-03-28 22:16:36.372795 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/cat-grep-fail/grep0.cwl
--rw-r--r--   0        0        0      272 2024-03-28 22:16:36.372926 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/cat-grep-fail/grep1.cwl
--rw-r--r--   0        0        0       76 2024-03-28 22:16:36.373063 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/cat-grep-fail/input.yml
--rw-r--r--   0        0        0     3215 2024-03-28 22:16:36.373230 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/cat-grep-fail/lorem.txt
--rw-r--r--   0        0        0      422 2024-03-28 22:16:36.373386 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/cat-grep-fail/tar.cwl
--rw-r--r--   0        0        0      710 2024-03-28 22:16:36.373578 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/cat-grep-fail/workflow.cwl
--rw-r--r--   0        0        0      350 2024-03-28 22:16:36.374050 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ci/README.md
--rw-r--r--   0        0        0     1968 2024-03-28 22:16:36.374314 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ci/clamr.cwl
--rw-r--r--   0        0        0      302 2024-03-28 22:16:36.374472 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_job.json
--rw-r--r--   0        0        0      429 2024-03-28 22:16:36.374724 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_job.yml
--rw-r--r--   0        0        0     2228 2024-03-28 22:16:36.375020 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_wf.cwl
--rw-r--r--   0        0        0      765 2024-03-28 22:16:36.375279 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ci/ffmpeg.cwl
--rw-r--r--   0        0        0      411 2024-03-29 16:50:01.383257 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/Dockerfile.clamr-ffmpeg
--rw-r--r--   0        0        0      347 2024-03-29 16:50:01.353020 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/README.md
--rw-r--r--   0        0        0     1446 2024-03-29 16:50:01.353180 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/clamr.cwl
--rw-r--r--   0        0        0      302 2024-03-29 16:50:01.353324 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/clamr_job.json
--rw-r--r--   0        0        0      405 2024-03-29 16:50:01.353481 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/clamr_job.yml
--rw-r--r--   0        0        0     2019 2024-03-29 16:50:01.353624 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/clamr_wf.cwl
--rw-r--r--   0        0        0      815 2024-03-29 16:50:01.353790 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/ffmpeg.cwl
--rw-r--r--   0        0        0       17 2024-03-29 16:50:01.353940 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/post_run.sh
--rw-r--r--   0        0        0       18 2024-03-29 16:50:01.354112 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/pre_run.sh
--rw-r--r--   0        0        0      350 2024-03-28 22:16:36.384975 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf/README.md
--rw-r--r--   0        0        0     1977 2024-03-28 22:16:36.385149 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf/clamr.cwl
--rw-r--r--   0        0        0      302 2024-03-28 22:16:36.385371 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_job.json
--rw-r--r--   0        0        0      455 2024-03-28 22:16:36.385604 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_job.yml
--rw-r--r--   0        0        0     2145 2024-03-28 22:16:36.385833 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_wf.cwl
--rw-r--r--   0        0        0      815 2024-03-28 22:16:36.386026 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf/ffmpeg.cwl
--rw-r--r--   0        0        0      383 2024-03-28 22:16:36.377486 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/README.md
--rw-r--r--   0        0        0     1962 2024-03-28 22:16:36.377745 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr.cwl
--rw-r--r--   0        0        0      302 2024-03-28 22:16:36.377970 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_job.json
--rw-r--r--   0        0        0      411 2024-03-28 22:16:36.378197 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_job.yml
--rw-r--r--   0        0        0     2006 2024-03-28 22:16:36.378352 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_wf.cwl
--rw-r--r--   0        0        0      753 2024-03-28 22:16:36.378502 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/ffmpeg.cwl
--rw-r--r--   0        0        0      837 2024-03-28 22:16:36.378731 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/README.md
--rw-r--r--   0        0        0      304 2024-03-28 22:16:36.379016 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/lsf-charliecloud/README.md
--rw-r--r--   0        0        0     1234 2024-03-28 22:16:36.379190 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/lsf-charliecloud/cf-summit.cwl
--rw-r--r--   0        0        0      145 2024-03-28 22:16:36.379452 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/Dockerfile.clamr-lanl-x86_64
--rw-r--r--   0        0        0     3325 2024-03-28 22:16:36.379703 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/README.md
--rw-r--r--   0        0        0     1127 2024-03-28 22:16:36.379932 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-darwin.cwl
--rw-r--r--   0        0        0     1135 2024-03-28 22:16:36.380143 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-no-owrite.cwl
--rw-r--r--   0        0        0     1137 2024-03-28 22:16:36.380291 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf.cwl
--rw-r--r--   0        0        0     1176 2024-03-28 22:16:36.380433 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/copyContainer_containerName.cwl
--rw-r--r--   0        0        0     1137 2024-03-28 22:16:36.380602 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerFile_containerName.cwl
--rw-r--r--   0        0        0     1133 2024-03-28 22:16:36.380784 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerPull.cwl
--rw-r--r--   0        0        0      182 2024-03-28 22:16:36.381023 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-singularity/README.md
--rw-r--r--   0        0        0     1122 2024-03-28 22:16:36.381197 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-singularity/cf-singularity.cwl
--rw-r--r--   0        0        0      303 2024-03-28 22:16:36.381502 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/README.md
--rw-r--r--   0        0        0     1975 2024-03-28 22:16:36.381759 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr.cwl
--rw-r--r--   0        0        0      302 2024-03-28 22:16:36.381982 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_job.json
--rw-r--r--   0        0        0      418 2024-03-28 22:16:36.382180 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_job.yml
--rw-r--r--   0        0        0     2057 2024-03-28 22:16:36.382381 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_wf.cwl
--rw-r--r--   0        0        0      768 2024-03-28 22:16:36.382528 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/ffmpeg.cwl
--rw-r--r--   0        0        0      339 2024-03-28 22:16:36.382785 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-summit/README.md
--rw-r--r--   0        0        0     1962 2024-03-28 22:16:36.382941 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr.cwl
--rw-r--r--   0        0        0      302 2024-03-28 22:16:36.383083 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_job.json
--rw-r--r--   0        0        0      418 2024-03-28 22:16:36.383256 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_job.yml
--rw-r--r--   0        0        0     2103 2024-03-28 22:16:36.383480 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_wf.cwl
--rw-r--r--   0        0        0      765 2024-03-28 22:16:36.383728 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-summit/ffmpeg.cwl
--rw-r--r--   0        0        0      350 2024-03-28 22:16:36.384066 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/README.md
--rw-r--r--   0        0        0     1981 2024-03-28 22:16:36.384227 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr.cwl
--rw-r--r--   0        0        0      302 2024-03-28 22:16:36.384363 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_job.json
--rw-r--r--   0        0        0      430 2024-03-28 22:16:36.384497 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_job.yml
--rw-r--r--   0        0        0     1939 2024-03-28 22:16:36.384630 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_wf.cwl
--rw-r--r--   0        0        0      765 2024-03-28 22:16:36.384760 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/ffmpeg.cwl
--rw-r--r--   0        0        0      527 2024-03-28 22:16:36.386265 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/comd-mpi/comd.cwl
--rw-r--r--   0        0        0      110 2024-03-28 22:16:36.386428 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/comd-mpi/comd_job.yml
--rw-r--r--   0        0        0      555 2024-03-28 22:16:36.386570 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/comd-mpi/comd_wf.cwl
--rw-r--r--   0        0        0      831 2024-03-28 22:16:36.387677 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/lulesh-mpi/lulesh.cwl
--rw-r--r--   0        0        0       24 2024-03-28 22:16:36.387837 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/lulesh-mpi/lulesh.yml
--rw-r--r--   0        0        0      264 2024-03-28 22:16:36.386879 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/lulesh-mpi-multi-file/lulesh.cwl
--rw-r--r--   0        0        0       24 2024-03-28 22:16:36.387091 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/lulesh-mpi-multi-file/lulesh_job.yml
--rw-r--r--   0        0        0      469 2024-03-28 22:16:36.387331 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/lulesh-mpi-multi-file/lulesh_wf.cwl
--rw-r--r--   0        0        0     1282 2024-03-28 22:16:36.388066 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/nwchem-mpi/README.md
--rw-r--r--   0        0        0      590 2024-03-28 22:16:36.388225 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem.cwl
--rw-r--r--   0        0        0      161 2024-03-28 22:16:36.388407 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem.yml
--rw-r--r--   0        0        0      199 2024-03-28 22:16:36.388620 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem_bin.cwl
--rw-r--r--   0        0        0      344 2024-03-28 22:16:36.392197 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant/graph.cwl
--rw-r--r--   0        0        0       43 2024-03-28 22:16:36.392532 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant/pennant.yml
--rw-r--r--   0        0        0      192 2024-03-28 22:16:36.392781 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant/pennant_1_node.cwl
--rw-r--r--   0        0        0      192 2024-03-28 22:16:36.393036 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant/pennant_2_node.cwl
--rw-r--r--   0        0        0      192 2024-03-28 22:16:36.393273 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant/pennant_4_node.cwl
--rw-r--r--   0        0        0     1217 2024-03-28 22:16:36.393572 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant/pennant_wf.cwl
--rw-r--r--   0        0        0     3881 2024-03-28 22:16:36.388879 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/Dockerfile.pennant-flux-x86_64
--rw-r--r--   0        0        0      789 2024-03-28 22:16:36.389106 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/Dockerfile.pennant-graph-x86_64
--rw-r--r--   0        0        0      407 2024-03-28 22:16:36.389420 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/graph.cwl
--rw-r--r--   0        0        0     1294 2024-03-28 22:16:36.389670 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/graph_pennant.py
--rw-r--r--   0        0        0      110 2024-03-28 22:16:36.389905 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/graph_pennant.sh
--rw-r--r--   0        0        0       43 2024-03-28 22:16:36.390208 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/pennant.yml
--rw-r--r--   0        0        0      192 2024-03-28 22:16:36.390730 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/pennant_1_node.cwl
--rw-r--r--   0        0        0      192 2024-03-28 22:16:36.390984 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/pennant_2_node.cwl
--rw-r--r--   0        0        0      192 2024-03-28 22:16:36.391226 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/pennant_4_node.cwl
--rw-r--r--   0        0        0      192 2024-03-28 22:16:36.391471 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/pennant_8_node.cwl
--rw-r--r--   0        0        0     1741 2024-03-28 22:16:36.391720 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/pennant_wf.cwl
--rw-r--r--   0        0        0       71 2024-03-28 22:16:36.393816 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pytest.ini
--rw-r--r--   0        0        0      317 2024-03-28 22:16:36.394254 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/simple-workflows/README.md
--rw-r--r--   0        0        0      986 2024-03-28 22:16:36.394516 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/simple-workflows/cancel.cwl
--rw-r--r--   0        0        0      217 2024-03-28 22:16:36.394918 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/README.md
--rw-r--r--   0        0        0     1083 2024-03-28 22:16:36.395183 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc-nc.cwl
--rw-r--r--   0        0        0     1325 2024-03-28 22:16:36.395445 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc.cwl
--rw-r--r--   0        0        0     3776 2024-03-28 22:16:36.395702 hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/lorem.txt
--rw-r--r--   0        0        0      426 2024-03-28 22:16:36.396138 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/README.md
--rwxr-xr-x   0        0        0      398 2024-03-28 22:16:36.396514 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/builder/dockerFile.cwl
--rwxr-xr-x   0        0        0      317 2024-03-28 22:16:36.396740 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/builder/dockerPull.cwl
--rw-r--r--   0        0        0     1202 2024-03-28 22:16:36.397093 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/grep-wordcount/gc.cwl
--rw-r--r--   0        0        0     3776 2024-03-28 22:16:36.397288 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/grep-wordcount/lorem.txt
--rwxr-xr-x   0        0        0      169 2024-03-28 22:16:36.397530 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/helloworld.cwl
--rw-r--r--   0        0        0       19 2024-03-28 22:16:36.397778 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/helloworld_input.yaml
--rw-r--r--   0        0        0    59407 2024-03-28 22:16:36.398764 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/DAG_example-1.png
--rw-r--r--   0        0        0      833 2024-03-28 22:16:36.399006 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/README.md
--rw-r--r--   0        0        0      254 2024-03-28 22:16:36.399215 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/add.cwl
--rw-r--r--   0        0        0      351 2024-03-28 22:16:36.399447 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/add_multiply_example_workflow.cwl
--rw-r--r--   0        0        0      245 2024-03-28 22:16:36.399597 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/add_step1.py
--rw-r--r--   0        0        0      386 2024-03-28 22:16:36.399737 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/isolated test.cwl
--rw-r--r--   0        0        0       21 2024-03-28 22:16:36.399903 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/job.yaml
--rw-r--r--   0        0        0      304 2024-03-28 22:16:36.400111 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/multiply.cwl
--rw-r--r--   0        0        0      267 2024-03-28 22:16:36.400335 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/multiply_step2.py
--rw-r--r--   0        0        0      407 2024-03-28 22:16:36.400569 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/workflow_generater_python.py
--rw-r--r--   0        0        0     3496 2024-03-28 22:16:36.400990 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/README.md
--rw-r--r--   0        0        0      901 2024-03-28 22:16:36.401373 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/decision_tree.py
--rw-r--r--   0        0        0      443 2024-03-28 22:16:36.401536 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/decision_tree_output.txt
--rw-r--r--   0        0        0      234 2024-03-28 22:16:36.401680 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/decision_tree_tool.cwl
--rw-r--r--   0        0        0      178 2024-03-28 22:16:36.401859 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/expectedValue.txt
--rw-r--r--   0        0        0      157 2024-03-28 22:16:36.402053 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/hiring1.txt
--rw-r--r--   0        0        0      467 2024-03-28 22:16:36.402274 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/linear_regress_output.txt
--rw-r--r--   0        0        0     1203 2024-03-28 22:16:36.402518 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/linear_regression.py
--rw-r--r--   0        0        0      692 2024-03-28 22:16:36.402779 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/machinelearning_pipeline.cwl
--rw-r--r--   0        0        0    12405 2024-03-28 22:16:36.403118 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/out.PNG
--rw-r--r--   0        0        0     1517 2024-03-28 22:16:36.403293 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/predict_code.py
--rw-r--r--   0        0        0      336 2024-03-28 22:16:36.403435 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/predict_tool.cwl
--rw-r--r--   0        0        0     1054 2024-03-28 22:16:36.403665 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/read_dataset.py
--rw-r--r--   0        0        0      235 2024-03-28 22:16:36.403835 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/read_dataset_tool.cwl
--rw-r--r--   0        0        0      239 2024-03-28 22:16:36.404013 hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/regress_tool.cwl
--rw-r--r--   0        0        0       80 2024-03-28 22:16:36.404371 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.builder_demo
--rw-r--r--   0        0        0      411 2024-03-28 22:16:36.404802 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.clamr-ffmpeg
--rw-r--r--   0        0        0      145 2024-03-28 22:16:36.405084 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.clamr-lanl-x86_64
--rw-r--r--   0        0        0      724 2024-03-28 22:16:36.405299 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.clamr-ppc64le
--rw-r--r--   0        0        0     3698 2024-03-28 22:16:36.405538 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.comd-flux-x86_64
--rw-r--r--   0        0        0     2303 2024-03-28 22:16:36.405728 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.comd-x86_64
--rw-r--r--   0        0        0      270 2024-03-28 22:16:36.405908 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.deb9ompi-x86_64
--rw-r--r--   0        0        0     2592 2024-03-28 22:16:36.406063 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.lulesh-x86_64
--rw-r--r--   0        0        0     1605 2024-03-28 22:16:36.406255 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.neo4j-ppc64le
--rw-r--r--   0        0        0     2489 2024-03-28 22:16:36.406541 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.nwchem-x86_64
--rw-r--r--   0        0        0     3881 2024-03-28 22:16:36.406803 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.pennant-flux-x86_64
--rw-r--r--   0        0        0     3446 2024-03-28 22:16:36.407037 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.vaspompi-x86_64
--rw-r--r--   0        0        0      614 2024-03-28 22:16:36.407192 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/README.md
--rw-r--r--   0        0        0      331 2024-03-28 22:16:36.407464 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.comd-x86_64-wpmix
--rw-r--r--   0        0        0      573 2024-03-28 22:16:36.407617 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.debian
--rw-r--r--   0        0        0     3941 2024-03-28 22:16:36.407776 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.openmpi-3.1.5
--rw-r--r--   0        0        0      509 2024-03-28 22:16:36.407913 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/comd-pmix-support/README.md
--rw-r--r--   0        0        0      813 2024-03-28 22:16:36.408098 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/comd-pmix-support/dont-init-ucx-on-intel-cray.patch
--rw-r--r--   0        0        0      789 2024-03-28 22:16:36.408377 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/pennant-graph/Dockerfile.pennant-graph-x86_64
--rw-r--r--   0        0        0     1294 2024-03-28 22:16:36.408604 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/pennant-graph/graph_pennant.py
--rw-r--r--   0        0        0      110 2024-03-28 22:16:36.408820 hpc-beeflow-0.1.7/beeflow/data/dockerfiles/pennant-graph/graph_pennant.sh
--rw-r--r--   0        0        0      640 2024-03-28 22:16:36.409201 hpc-beeflow-0.1.7/beeflow/enhanced_client/README.rst
--rw-r--r--   0        0        0        0 2024-03-28 22:16:36.409471 hpc-beeflow-0.1.7/beeflow/enhanced_client/data/.gitkeep
--rw-r--r--   0        0        0      386 2024-03-28 22:16:36.409640 hpc-beeflow-0.1.7/beeflow/enhanced_client/forge.config.js
--rw-r--r--   0        0        0     1682 2024-03-28 22:16:36.409813 hpc-beeflow-0.1.7/beeflow/enhanced_client/main.js
--rw-r--r--   0        0        0   231716 2024-03-29 16:50:01.355750 hpc-beeflow-0.1.7/beeflow/enhanced_client/package-lock.json
--rw-r--r--   0        0        0     1078 2024-03-28 22:16:36.411301 hpc-beeflow-0.1.7/beeflow/enhanced_client/package.json
--rw-r--r--   0        0        0     1219 2024-03-28 22:16:36.411639 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/app.js
--rw-r--r--   0        0        0     5151 2024-03-28 22:16:36.411951 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/client.js
--rw-r--r--   0        0        0      872 2024-03-28 22:16:36.412170 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/config.js
--rw-r--r--   0        0        0     2013 2024-03-28 22:16:36.412332 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/control.js
--rw-r--r--   0        0        0     3610 2024-03-28 22:16:36.412502 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/database.js
--rw-r--r--   0        0        0    12140 2024-03-28 22:16:36.412701 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/display.js
--rw-r--r--   0        0        0      455 2024-03-28 22:16:36.412897 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/gdb.js
--rw-r--r--   0        0        0    33601 2024-03-28 22:16:36.413313 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/img/logo.png
--rw-r--r--   0        0        0     2751 2024-03-28 22:16:36.413585 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/main.html
--rw-r--r--   0        0        0   206620 2024-03-28 22:16:36.414373 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/styles/bulma.min.css
--rw-r--r--   0        0        0      374 2024-03-28 22:16:36.414563 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/styles/main.css
--rw-r--r--   0        0        0      498 2024-03-28 22:16:36.414733 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/tunnel.js
--rw-r--r--   0        0        0      428 2024-03-28 22:16:36.414973 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/viz.html
--rw-r--r--   0        0        0     1071 2024-03-28 22:16:36.415256 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/viz.js
--rw-r--r--   0        0        0     7603 2024-03-28 22:16:36.415531 hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/workflows.js
--rw-r--r--   0        0        0     1708 2024-03-28 22:16:36.415837 hpc-beeflow-0.1.7/beeflow/scheduler/README.md
--rw-r--r--   0        0        0    10098 2024-03-28 22:16:36.416106 hpc-beeflow-0.1.7/beeflow/scheduler/algorithms.py
--rw-r--r--   0        0        0     9347 2024-03-28 22:16:36.416370 hpc-beeflow-0.1.7/beeflow/scheduler/resource_allocation.py
--rw-r--r--   0        0        0     3738 2024-03-28 22:16:36.416539 hpc-beeflow-0.1.7/beeflow/scheduler/scheduler.py
--rw-r--r--   0        0        0     2890 2024-03-28 22:16:36.416765 hpc-beeflow-0.1.7/beeflow/scheduler/scheduler.yaml
--rw-r--r--   0        0        0      708 2024-03-28 22:16:36.417035 hpc-beeflow-0.1.7/beeflow/scheduler/serializable.py
--rw-r--r--   0        0        0     2296 2024-03-28 22:16:36.417255 hpc-beeflow-0.1.7/beeflow/scheduler/task.py
--rw-r--r--   0        0        0     5500 2024-03-29 16:50:01.356040 hpc-beeflow-0.1.7/beeflow/task_manager/background.py
--rw-r--r--   0        0        0     1239 2024-03-29 16:50:01.356206 hpc-beeflow-0.1.7/beeflow/task_manager/task_actions.py
--rw-r--r--   0        0        0     1538 2024-03-29 16:50:01.356349 hpc-beeflow-0.1.7/beeflow/task_manager/task_manager.py
--rw-r--r--   0        0        0      856 2024-03-29 16:50:01.356488 hpc-beeflow-0.1.7/beeflow/task_manager/task_submit.py
--rw-r--r--   0        0        0     3602 2024-03-29 16:50:01.356645 hpc-beeflow-0.1.7/beeflow/task_manager/utils.py
--rw-r--r--   0        0        0    34925 2024-03-28 22:16:36.418588 hpc-beeflow-0.1.7/beeflow/tests/42.tgz
--rw-r--r--   0        0        0      236 2024-03-28 22:16:36.418758 hpc-beeflow-0.1.7/beeflow/tests/README.md
--rw-r--r--   0        0        0     1139 2024-03-28 22:16:36.418913 hpc-beeflow-0.1.7/beeflow/tests/cf.cwl
--rw-r--r--   0        0        0     1093 2024-03-28 22:16:36.419527 hpc-beeflow-0.1.7/beeflow/tests/clamr-wf/clamr.cwl
--rw-r--r--   0        0        0      302 2024-03-28 22:16:36.419765 hpc-beeflow-0.1.7/beeflow/tests/clamr-wf/clamr_job.json
--rw-r--r--   0        0        0      424 2024-03-28 22:16:36.419927 hpc-beeflow-0.1.7/beeflow/tests/clamr-wf/clamr_job.yml
--rw-r--r--   0        0        0     1320 2024-03-28 22:16:36.420116 hpc-beeflow-0.1.7/beeflow/tests/clamr-wf/clamr_wf.cwl
--rw-r--r--   0        0        0      680 2024-03-28 22:16:36.420363 hpc-beeflow-0.1.7/beeflow/tests/clamr-wf/ffmpeg.cwl
--rw-r--r--   0        0        0      273 2024-03-28 22:16:36.420655 hpc-beeflow-0.1.7/beeflow/tests/clamr-wf/mv_script.cwl
--rwxr-xr-x   0        0        0      324 2024-03-28 22:16:36.420825 hpc-beeflow-0.1.7/beeflow/tests/clamr-wf/mv_script.sh
--rw-r--r--   0        0        0     2401 2024-03-28 22:16:36.419154 hpc-beeflow-0.1.7/beeflow/tests/clamr-wf.tgz
--rw-r--r--   0        0        0      774 2024-03-28 22:16:36.420989 hpc-beeflow-0.1.7/beeflow/tests/gdb.py
--rw-r--r--   0        0        0    12378 2024-03-28 22:16:36.421252 hpc-beeflow-0.1.7/beeflow/tests/mocks.py
--rw-r--r--   0        0        0      267 2024-03-28 22:16:36.421532 hpc-beeflow-0.1.7/beeflow/tests/test_cloud.py
--rw-r--r--   0        0        0     6006 2024-03-28 22:16:36.421841 hpc-beeflow-0.1.7/beeflow/tests/test_config_validator.py
--rw-r--r--   0        0        0      807 2024-03-28 22:16:36.422052 hpc-beeflow-0.1.7/beeflow/tests/test_container_path.py
--rw-r--r--   0        0        0      946 2024-03-28 22:16:36.422217 hpc-beeflow-0.1.7/beeflow/tests/test_db_sched.py
--rw-r--r--   0        0        0     4410 2024-03-28 22:16:36.422409 hpc-beeflow-0.1.7/beeflow/tests/test_db_tm.py
--rw-r--r--   0        0        0    16813 2024-03-29 16:50:01.357222 hpc-beeflow-0.1.7/beeflow/tests/test_parser.py
--rw-r--r--   0        0        0    15134 2024-03-28 22:16:36.422830 hpc-beeflow-0.1.7/beeflow/tests/test_scheduler.py
--rw-r--r--   0        0        0     2630 2024-03-28 22:16:36.423055 hpc-beeflow-0.1.7/beeflow/tests/test_scheduler_resource_allocation.py
--rw-r--r--   0        0        0     6557 2024-03-28 22:16:36.423487 hpc-beeflow-0.1.7/beeflow/tests/test_scheduler_rest.py
--rw-r--r--   0        0        0     4908 2024-03-28 22:16:36.423804 hpc-beeflow-0.1.7/beeflow/tests/test_slurm_worker.py
--rw-r--r--   0        0        0     3796 2024-03-29 16:50:01.358063 hpc-beeflow-0.1.7/beeflow/tests/test_tm.py
--rw-r--r--   0        0        0    33819 2024-03-28 22:16:36.424442 hpc-beeflow-0.1.7/beeflow/tests/test_wf_interface.py
--rw-r--r--   0        0        0    11213 2024-03-29 16:50:01.358653 hpc-beeflow-0.1.7/beeflow/tests/test_wf_manager.py
--rwxr-xr-x   0        0        0     7823 2024-03-28 22:16:36.425016 hpc-beeflow-0.1.7/beeflow/wf_manager/common/dep_manager.py
--rw-r--r--   0        0        0    10373 2024-03-28 22:16:36.425189 hpc-beeflow-0.1.7/beeflow/wf_manager/common/wf_db.py
--rw-r--r--   0        0        0     4722 2024-03-29 16:50:01.359171 hpc-beeflow-0.1.7/beeflow/wf_manager/resources/wf_actions.py
--rw-r--r--   0        0        0     8674 2024-03-28 22:16:36.425643 hpc-beeflow-0.1.7/beeflow/wf_manager/resources/wf_list.py
--rw-r--r--   0        0        0      560 2024-03-28 22:16:36.425839 hpc-beeflow-0.1.7/beeflow/wf_manager/resources/wf_metadata.py
--rw-r--r--   0        0        0     6266 2024-03-29 16:50:01.359605 hpc-beeflow-0.1.7/beeflow/wf_manager/resources/wf_update.py
--rw-r--r--   0        0        0     8816 2024-03-28 22:16:36.426616 hpc-beeflow-0.1.7/beeflow/wf_manager/resources/wf_utils.py
--rw-r--r--   0        0        0     1793 2024-03-28 22:16:36.426816 hpc-beeflow-0.1.7/beeflow/wf_manager/wf_manager.py
--rw-r--r--   0        0        0     2715 2024-03-29 16:50:01.369059 hpc-beeflow-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     9244 2024-04-01 17:14:02.170565 hpc-beeflow-0.1.7/setup.py
--rw-r--r--   0        0        0     7288 2024-04-01 17:14:02.171060 hpc-beeflow-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1477 2024-03-26 22:59:00.103073 hpc_beeflow-0.1.8/LICENSE
+-rw-r--r--   0        0        0     5235 2024-03-26 22:59:00.103218 hpc_beeflow-0.1.8/README.rst
+-rw-r--r--   0        0        0      122 2024-03-26 22:59:00.103538 hpc_beeflow-0.1.8/beeflow/client/README.md
+-rw-r--r--   0        0        0    22324 2024-04-02 20:31:14.877496 hpc_beeflow-0.1.8/beeflow/client/bee_client.py
+-rw-r--r--   0        0        0    23686 2024-04-02 20:32:24.402241 hpc_beeflow-0.1.8/beeflow/client/core.py
+-rw-r--r--   0        0        0     8036 2024-03-26 22:59:00.104350 hpc_beeflow-0.1.8/beeflow/cloud_launcher.py
+-rw-r--r--   0        0        0      234 2024-03-26 22:59:00.104492 hpc_beeflow-0.1.8/beeflow/common/README.md
+-rw-r--r--   0        0        0      459 2024-03-26 22:59:00.104600 hpc_beeflow-0.1.8/beeflow/common/api.py
+-rw-r--r--   0        0        0    11473 2024-03-26 22:59:00.104764 hpc_beeflow-0.1.8/beeflow/common/build/README.md
+-rw-r--r--   0        0        0     5116 2024-04-02 20:31:14.878573 hpc_beeflow-0.1.8/beeflow/common/build/build_driver.py
+-rw-r--r--   0        0        0    19130 2024-04-02 20:31:14.879080 hpc_beeflow-0.1.8/beeflow/common/build/container_drivers.py
+-rw-r--r--   0        0        0      733 2024-04-02 20:31:14.879219 hpc_beeflow-0.1.8/beeflow/common/build/utils.py
+-rw-r--r--   0        0        0     3534 2024-04-02 20:31:14.879725 hpc_beeflow-0.1.8/beeflow/common/build_interfaces.py
+-rw-r--r--   0        0        0      163 2024-03-26 22:59:00.105823 hpc_beeflow-0.1.8/beeflow/common/celery.py
+-rw-r--r--   0        0        0      285 2024-03-26 22:59:00.105912 hpc_beeflow-0.1.8/beeflow/common/cli.py
+-rw-r--r--   0        0        0     3023 2024-03-26 22:59:00.106056 hpc_beeflow-0.1.8/beeflow/common/cli_connection.py
+-rw-r--r--   0        0        0     2542 2024-03-26 22:59:00.106219 hpc_beeflow-0.1.8/beeflow/common/cloud/README.md
+-rw-r--r--   0        0        0      830 2024-03-26 22:59:00.106339 hpc_beeflow-0.1.8/beeflow/common/cloud/__init__.py
+-rw-r--r--   0        0        0     1166 2024-03-26 22:59:00.106448 hpc_beeflow-0.1.8/beeflow/common/cloud/chameleoncloud.py
+-rw-r--r--   0        0        0      175 2024-03-26 22:59:00.106563 hpc_beeflow-0.1.8/beeflow/common/cloud/cloud.py
+-rw-r--r--   0        0        0       42 2024-03-26 22:59:00.106675 hpc_beeflow-0.1.8/beeflow/common/cloud/constants.py
+-rw-r--r--   0        0        0     1599 2024-03-26 22:59:00.106807 hpc_beeflow-0.1.8/beeflow/common/cloud/google.py
+-rw-r--r--   0        0        0     1093 2024-03-26 22:59:00.106908 hpc_beeflow-0.1.8/beeflow/common/cloud/openstack.py
+-rw-r--r--   0        0        0      784 2024-03-26 22:59:00.107032 hpc_beeflow-0.1.8/beeflow/common/cloud/provider.py
+-rw-r--r--   0        0        0    22522 2024-03-26 23:05:07.487824 hpc_beeflow-0.1.8/beeflow/common/config_driver.py
+-rw-r--r--   0        0        0     5891 2024-03-26 22:59:00.107375 hpc_beeflow-0.1.8/beeflow/common/config_validator.py
+-rw-r--r--   0        0        0     2420 2024-03-26 22:59:00.107486 hpc_beeflow-0.1.8/beeflow/common/connection.py
+-rw-r--r--   0        0        0      947 2024-03-26 22:59:00.107588 hpc_beeflow-0.1.8/beeflow/common/container_path.py
+-rw-r--r--   0        0        0     7084 2024-04-02 20:31:14.880127 hpc_beeflow-0.1.8/beeflow/common/crt/charliecloud_driver.py
+-rw-r--r--   0        0        0     1487 2024-03-26 22:59:00.107940 hpc_beeflow-0.1.8/beeflow/common/crt/crt_driver.py
+-rw-r--r--   0        0        0     1760 2024-04-02 20:31:14.880685 hpc_beeflow-0.1.8/beeflow/common/crt/singularity_driver.py
+-rw-r--r--   0        0        0     1551 2024-03-26 22:59:00.108180 hpc_beeflow-0.1.8/beeflow/common/crt_interface.py
+-rw-r--r--   0        0        0     2486 2024-03-26 22:59:00.108391 hpc_beeflow-0.1.8/beeflow/common/db/bdb.py
+-rw-r--r--   0        0        0     1675 2024-03-26 22:59:00.108500 hpc_beeflow-0.1.8/beeflow/common/db/sched_db.py
+-rw-r--r--   0        0        0     5075 2024-03-26 22:59:00.108596 hpc_beeflow-0.1.8/beeflow/common/db/tm_db.py
+-rw-r--r--   0        0        0     8816 2024-03-26 22:59:00.108723 hpc_beeflow-0.1.8/beeflow/common/db/wfm_db.py
+-rw-r--r--   0        0        0     2133 2024-03-26 22:59:00.108836 hpc_beeflow-0.1.8/beeflow/common/expr.py
+-rw-r--r--   0        0        0     5924 2024-03-26 22:59:00.109122 hpc_beeflow-0.1.8/beeflow/common/gdb/DESIGN.md
+-rw-r--r--   0        0        0     8320 2024-03-26 23:05:07.488240 hpc_beeflow-0.1.8/beeflow/common/gdb/gdb_driver.py
+-rw-r--r--   0        0        0    23439 2024-03-26 23:05:07.488689 hpc_beeflow-0.1.8/beeflow/common/gdb/neo4j_cypher.py
+-rw-r--r--   0        0        0    22892 2024-03-26 23:05:07.489036 hpc_beeflow-0.1.8/beeflow/common/gdb/neo4j_driver.py
+-rw-r--r--   0        0        0     9736 2024-03-26 22:59:00.109844 hpc_beeflow-0.1.8/beeflow/common/gdb_interface.py
+-rw-r--r--   0        0        0     4222 2024-03-26 22:59:00.110016 hpc_beeflow-0.1.8/beeflow/common/integration/generated_workflows.py
+-rw-r--r--   0        0        0     8370 2024-04-02 20:31:14.881145 hpc_beeflow-0.1.8/beeflow/common/integration/utils.py
+-rw-r--r--   0        0        0    11162 2024-04-02 20:31:14.881543 hpc_beeflow-0.1.8/beeflow/common/integration_test.py
+-rw-r--r--   0        0        0      642 2024-03-26 22:59:00.110697 hpc_beeflow-0.1.8/beeflow/common/log.py
+-rw-r--r--   0        0        0       16 2024-03-26 22:59:00.110868 hpc_beeflow-0.1.8/beeflow/common/parser/.gitignore
+-rw-r--r--   0        0        0     2614 2024-03-26 22:59:00.110998 hpc_beeflow-0.1.8/beeflow/common/parser/README.md
+-rw-r--r--   0        0        0      102 2024-03-26 22:59:00.111098 hpc_beeflow-0.1.8/beeflow/common/parser/__init__.py
+-rw-r--r--   0        0        0    15464 2024-03-26 23:05:21.150788 hpc_beeflow-0.1.8/beeflow/common/parser/parser.py
+-rw-r--r--   0        0        0     2162 2024-03-26 22:59:00.111367 hpc_beeflow-0.1.8/beeflow/common/paths.py
+-rw-r--r--   0        0        0      450 2024-03-26 22:59:00.111455 hpc_beeflow-0.1.8/beeflow/common/states.py
+-rw-r--r--   0        0        0      493 2024-03-26 22:59:00.111562 hpc_beeflow-0.1.8/beeflow/common/tab_completion.py
+-rw-r--r--   0        0        0     1643 2024-03-26 22:59:00.111671 hpc_beeflow-0.1.8/beeflow/common/validation.py
+-rw-r--r--   0        0        0    12396 2024-03-26 22:59:00.111814 hpc_beeflow-0.1.8/beeflow/common/wf_data.py
+-rw-r--r--   0        0        0    11679 2024-03-26 23:05:07.489776 hpc_beeflow-0.1.8/beeflow/common/wf_interface.py
+-rw-r--r--   0        0        0     1522 2024-03-26 22:59:00.112074 hpc_beeflow-0.1.8/beeflow/common/wf_profiler.py
+-rw-r--r--   0        0        0      493 2024-03-26 22:59:00.112356 hpc_beeflow-0.1.8/beeflow/common/worker/README.md
+-rw-r--r--   0        0        0      597 2024-03-26 22:59:00.112489 hpc_beeflow-0.1.8/beeflow/common/worker/__init__.py
+-rw-r--r--   0        0        0     5048 2024-03-26 22:59:00.112639 hpc_beeflow-0.1.8/beeflow/common/worker/flux_worker.py
+-rw-r--r--   0        0        0     2570 2024-03-26 22:59:00.112797 hpc_beeflow-0.1.8/beeflow/common/worker/lsf_worker.py
+-rw-r--r--   0        0        0     1731 2024-03-26 22:59:00.112918 hpc_beeflow-0.1.8/beeflow/common/worker/simple_worker.py
+-rw-r--r--   0        0        0    10635 2024-03-26 23:05:21.151213 hpc_beeflow-0.1.8/beeflow/common/worker/slurm_worker.py
+-rw-r--r--   0        0        0     2899 2024-03-26 22:59:00.113143 hpc_beeflow-0.1.8/beeflow/common/worker/worker.py
+-rw-r--r--   0        0        0     1794 2024-03-26 22:59:00.113236 hpc_beeflow-0.1.8/beeflow/common/worker_interface.py
+-rw-r--r--   0        0        0     4301 2024-03-26 22:59:00.113442 hpc_beeflow-0.1.8/beeflow/data/cloud_templates/dora.jinja
+-rw-r--r--   0        0        0      866 2024-03-26 22:59:00.113546 hpc_beeflow-0.1.8/beeflow/data/cloud_templates/dora.yaml
+-rw-r--r--   0        0        0      414 2024-03-26 22:59:00.113909 hpc_beeflow-0.1.8/beeflow/data/cwl/README.md
+-rw-r--r--   0        0        0     1281 2024-03-26 22:59:00.114177 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/README.md
+-rw-r--r--   0        0        0      315 2024-03-26 22:59:00.114358 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/blast/README.md
+-rw-r--r--   0        0        0      418 2024-03-26 22:59:00.114478 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/blast/blast.yml
+-rw-r--r--   0        0        0      423 2024-03-26 22:59:00.114608 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/blast/blast_output.cwl
+-rw-r--r--   0        0        0      300 2024-03-26 22:59:00.114721 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/blast/blast_output_err.cwl
+-rw-r--r--   0        0        0      410 2024-03-26 22:59:00.114836 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/blast/blast_split.cwl
+-rw-r--r--   0        0        0     2009 2024-03-26 22:59:00.114959 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/blast/blast_wf.cwl
+-rw-r--r--   0        0        0      559 2024-03-26 22:59:00.115070 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/blast/blast_worker001.cwl
+-rw-r--r--   0        0        0      559 2024-03-26 22:59:00.115158 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/blast/blast_worker002.cwl
+-rwxr-xr-x   0        0        0   930997 2024-03-26 22:59:00.118031 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/blast/input/small.fasta
+-rw-r--r--   0        0        0       77 2024-03-26 22:59:00.118202 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/cat-grep-fail/README.md
+-rw-r--r--   0        0        0      258 2024-03-26 22:59:00.118316 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/cat-grep-fail/cat.cwl
+-rw-r--r--   0        0        0      272 2024-03-26 22:59:00.118407 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/cat-grep-fail/grep0.cwl
+-rw-r--r--   0        0        0      272 2024-03-26 22:59:00.118483 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/cat-grep-fail/grep1.cwl
+-rw-r--r--   0        0        0       76 2024-03-26 22:59:00.118555 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/cat-grep-fail/input.yml
+-rw-r--r--   0        0        0     3215 2024-03-26 22:59:00.118635 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/cat-grep-fail/lorem.txt
+-rw-r--r--   0        0        0      422 2024-03-26 22:59:00.118726 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/cat-grep-fail/tar.cwl
+-rw-r--r--   0        0        0      710 2024-03-26 22:59:00.118976 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/cat-grep-fail/workflow.cwl
+-rw-r--r--   0        0        0      350 2024-03-26 22:59:00.119140 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-ci/README.md
+-rw-r--r--   0        0        0     1968 2024-03-26 22:59:00.119243 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-ci/clamr.cwl
+-rw-r--r--   0        0        0      302 2024-03-26 22:59:00.119338 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_job.json
+-rw-r--r--   0        0        0      429 2024-03-26 22:59:00.119436 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_job.yml
+-rw-r--r--   0        0        0     2228 2024-03-26 22:59:00.119529 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_wf.cwl
+-rw-r--r--   0        0        0      765 2024-03-26 22:59:00.119649 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-ci/ffmpeg.cwl
+-rw-r--r--   0        0        0      411 2024-03-26 23:05:21.151411 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/Dockerfile.clamr-ffmpeg
+-rw-r--r--   0        0        0      347 2024-03-26 23:05:21.151505 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/README.md
+-rw-r--r--   0        0        0     1446 2024-03-26 23:05:21.151599 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/clamr.cwl
+-rw-r--r--   0        0        0      302 2024-03-26 23:05:21.151685 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/clamr_job.json
+-rw-r--r--   0        0        0      405 2024-03-26 23:05:21.151768 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/clamr_job.yml
+-rw-r--r--   0        0        0     2019 2024-03-26 23:05:21.151864 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/clamr_wf.cwl
+-rw-r--r--   0        0        0      815 2024-03-26 23:05:21.151944 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/ffmpeg.cwl
+-rw-r--r--   0        0        0       17 2024-03-26 23:05:21.152299 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/post_run.sh
+-rw-r--r--   0        0        0       18 2024-03-26 23:05:21.152403 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/pre_run.sh
+-rw-r--r--   0        0        0      350 2024-03-26 22:59:00.124034 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf/README.md
+-rw-r--r--   0        0        0     1977 2024-03-26 22:59:00.124182 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf/clamr.cwl
+-rw-r--r--   0        0        0      302 2024-03-26 22:59:00.124289 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_job.json
+-rw-r--r--   0        0        0      455 2024-03-26 22:59:00.124404 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_job.yml
+-rw-r--r--   0        0        0     2145 2024-03-26 22:59:00.124506 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_wf.cwl
+-rw-r--r--   0        0        0      815 2024-03-26 22:59:00.124601 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf/ffmpeg.cwl
+-rw-r--r--   0        0        0      383 2024-03-26 22:59:00.119802 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/README.md
+-rw-r--r--   0        0        0     1962 2024-03-26 22:59:00.119909 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr.cwl
+-rw-r--r--   0        0        0      302 2024-03-26 22:59:00.119981 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_job.json
+-rw-r--r--   0        0        0      411 2024-03-26 22:59:00.120059 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_job.yml
+-rw-r--r--   0        0        0     2006 2024-03-26 22:59:00.120141 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_wf.cwl
+-rw-r--r--   0        0        0      753 2024-03-26 22:59:00.120230 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/ffmpeg.cwl
+-rw-r--r--   0        0        0      837 2024-03-26 22:59:00.120377 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/README.md
+-rw-r--r--   0        0        0      304 2024-03-26 22:59:00.120539 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/lsf-charliecloud/README.md
+-rw-r--r--   0        0        0     1234 2024-03-26 22:59:00.120658 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/lsf-charliecloud/cf-summit.cwl
+-rw-r--r--   0        0        0      145 2024-03-26 22:59:00.120800 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/Dockerfile.clamr-lanl-x86_64
+-rw-r--r--   0        0        0     3325 2024-03-26 22:59:00.120886 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/README.md
+-rw-r--r--   0        0        0     1127 2024-03-26 22:59:00.120956 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-darwin.cwl
+-rw-r--r--   0        0        0     1135 2024-03-26 22:59:00.121056 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-no-owrite.cwl
+-rw-r--r--   0        0        0     1137 2024-03-26 22:59:00.121159 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf.cwl
+-rw-r--r--   0        0        0     1176 2024-03-26 22:59:00.121304 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/copyContainer_containerName.cwl
+-rw-r--r--   0        0        0     1137 2024-03-26 22:59:00.121413 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerFile_containerName.cwl
+-rw-r--r--   0        0        0     1133 2024-03-26 22:59:00.121508 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerPull.cwl
+-rw-r--r--   0        0        0      182 2024-03-26 22:59:00.121668 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-singularity/README.md
+-rw-r--r--   0        0        0     1122 2024-03-26 22:59:00.121762 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-singularity/cf-singularity.cwl
+-rw-r--r--   0        0        0      303 2024-03-26 22:59:00.121923 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/README.md
+-rw-r--r--   0        0        0     1975 2024-03-26 22:59:00.122037 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr.cwl
+-rw-r--r--   0        0        0      302 2024-03-26 22:59:00.122131 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_job.json
+-rw-r--r--   0        0        0      418 2024-03-26 22:59:00.122217 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_job.yml
+-rw-r--r--   0        0        0     2057 2024-03-26 22:59:00.122296 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_wf.cwl
+-rw-r--r--   0        0        0      768 2024-03-26 22:59:00.122385 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/ffmpeg.cwl
+-rw-r--r--   0        0        0      339 2024-03-26 22:59:00.122555 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-summit/README.md
+-rw-r--r--   0        0        0     1962 2024-03-26 22:59:00.122665 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr.cwl
+-rw-r--r--   0        0        0      302 2024-03-26 22:59:00.122756 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_job.json
+-rw-r--r--   0        0        0      418 2024-03-26 22:59:00.122843 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_job.yml
+-rw-r--r--   0        0        0     2103 2024-03-26 22:59:00.122930 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_wf.cwl
+-rw-r--r--   0        0        0      765 2024-03-26 22:59:00.123016 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-summit/ffmpeg.cwl
+-rw-r--r--   0        0        0      350 2024-03-26 22:59:00.123172 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/README.md
+-rw-r--r--   0        0        0     1981 2024-03-26 22:59:00.123287 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr.cwl
+-rw-r--r--   0        0        0      302 2024-03-26 22:59:00.123378 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_job.json
+-rw-r--r--   0        0        0      430 2024-03-26 22:59:00.123463 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_job.yml
+-rw-r--r--   0        0        0     1939 2024-03-26 22:59:00.123552 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_wf.cwl
+-rw-r--r--   0        0        0      765 2024-03-26 22:59:00.123649 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/ffmpeg.cwl
+-rw-r--r--   0        0        0      527 2024-03-26 22:59:00.124762 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/comd-mpi/comd.cwl
+-rw-r--r--   0        0        0      110 2024-03-26 22:59:00.124849 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/comd-mpi/comd_job.yml
+-rw-r--r--   0        0        0      555 2024-03-26 22:59:00.125040 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/comd-mpi/comd_wf.cwl
+-rw-r--r--   0        0        0      831 2024-03-26 22:59:00.125515 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/lulesh-mpi/lulesh.cwl
+-rw-r--r--   0        0        0       24 2024-03-26 22:59:00.125616 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/lulesh-mpi/lulesh.yml
+-rw-r--r--   0        0        0      264 2024-03-26 22:59:00.125193 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/lulesh-mpi-multi-file/lulesh.cwl
+-rw-r--r--   0        0        0       24 2024-03-26 22:59:00.125291 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/lulesh-mpi-multi-file/lulesh_job.yml
+-rw-r--r--   0        0        0      469 2024-03-26 22:59:00.125374 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/lulesh-mpi-multi-file/lulesh_wf.cwl
+-rw-r--r--   0        0        0     1282 2024-03-26 22:59:00.125832 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/nwchem-mpi/README.md
+-rw-r--r--   0        0        0      590 2024-03-26 22:59:00.125990 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem.cwl
+-rw-r--r--   0        0        0      161 2024-03-26 22:59:00.126085 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem.yml
+-rw-r--r--   0        0        0      199 2024-03-26 22:59:00.126197 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem_bin.cwl
+-rw-r--r--   0        0        0      344 2024-03-26 22:59:00.127396 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant/graph.cwl
+-rw-r--r--   0        0        0       43 2024-03-26 22:59:00.127480 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant/pennant.yml
+-rw-r--r--   0        0        0      192 2024-03-26 22:59:00.127555 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant/pennant_1_node.cwl
+-rw-r--r--   0        0        0      192 2024-03-26 22:59:00.127622 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant/pennant_2_node.cwl
+-rw-r--r--   0        0        0      192 2024-03-26 22:59:00.127685 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant/pennant_4_node.cwl
+-rw-r--r--   0        0        0     1217 2024-03-26 22:59:00.127769 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant/pennant_wf.cwl
+-rw-r--r--   0        0        0     3881 2024-03-26 22:59:00.126378 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant-build/Dockerfile.pennant-flux-x86_64
+-rw-r--r--   0        0        0      789 2024-03-26 22:59:00.126494 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant-build/Dockerfile.pennant-graph-x86_64
+-rw-r--r--   0        0        0      407 2024-03-26 22:59:00.126593 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant-build/graph.cwl
+-rw-r--r--   0        0        0     1294 2024-03-26 22:59:00.126693 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant-build/graph_pennant.py
+-rw-r--r--   0        0        0      110 2024-03-26 22:59:00.126793 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant-build/graph_pennant.sh
+-rw-r--r--   0        0        0       43 2024-03-26 22:59:00.126890 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant-build/pennant.yml
+-rw-r--r--   0        0        0      192 2024-03-26 22:59:00.126979 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant-build/pennant_1_node.cwl
+-rw-r--r--   0        0        0      192 2024-03-26 22:59:00.127064 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant-build/pennant_2_node.cwl
+-rw-r--r--   0        0        0      192 2024-03-26 22:59:00.127131 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant-build/pennant_4_node.cwl
+-rw-r--r--   0        0        0      192 2024-03-26 22:59:00.127197 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant-build/pennant_8_node.cwl
+-rw-r--r--   0        0        0     1741 2024-03-26 22:59:00.127275 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant-build/pennant_wf.cwl
+-rw-r--r--   0        0        0       71 2024-03-26 22:59:00.127847 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pytest.ini
+-rw-r--r--   0        0        0      317 2024-03-26 22:59:00.128000 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/simple-workflows/README.md
+-rw-r--r--   0        0        0      986 2024-03-26 22:59:00.128101 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/simple-workflows/cancel.cwl
+-rw-r--r--   0        0        0      217 2024-03-26 22:59:00.128254 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/README.md
+-rw-r--r--   0        0        0     1083 2024-03-26 22:59:00.128349 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc-nc.cwl
+-rw-r--r--   0        0        0     1325 2024-03-26 22:59:00.128433 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc.cwl
+-rw-r--r--   0        0        0     3776 2024-03-26 22:59:00.128534 hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/lorem.txt
+-rw-r--r--   0        0        0      426 2024-03-26 22:59:00.128766 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/README.md
+-rwxr-xr-x   0        0        0      398 2024-03-26 22:59:00.128904 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/builder/dockerFile.cwl
+-rwxr-xr-x   0        0        0      317 2024-03-26 22:59:00.128980 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/builder/dockerPull.cwl
+-rw-r--r--   0        0        0     1202 2024-03-26 22:59:00.129095 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/grep-wordcount/gc.cwl
+-rw-r--r--   0        0        0     3776 2024-03-26 22:59:00.129198 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/grep-wordcount/lorem.txt
+-rwxr-xr-x   0        0        0      169 2024-03-26 22:59:00.129311 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/helloworld.cwl
+-rw-r--r--   0        0        0       19 2024-03-26 22:59:00.129408 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/helloworld_input.yaml
+-rw-r--r--   0        0        0    59407 2024-03-26 22:59:00.129909 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/DAG_example-1.png
+-rw-r--r--   0        0        0      833 2024-03-26 22:59:00.130038 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/README.md
+-rw-r--r--   0        0        0      254 2024-03-26 22:59:00.130135 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/add.cwl
+-rw-r--r--   0        0        0      351 2024-03-26 22:59:00.130211 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/add_multiply_example_workflow.cwl
+-rw-r--r--   0        0        0      245 2024-03-26 22:59:00.130288 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/add_step1.py
+-rw-r--r--   0        0        0      386 2024-03-26 22:59:00.130371 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/isolated test.cwl
+-rw-r--r--   0        0        0       21 2024-03-26 22:59:00.130453 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/job.yaml
+-rw-r--r--   0        0        0      304 2024-03-26 22:59:00.130535 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/multiply.cwl
+-rw-r--r--   0        0        0      267 2024-03-26 22:59:00.130611 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/multiply_step2.py
+-rw-r--r--   0        0        0      407 2024-03-26 22:59:00.130700 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/workflow_generater_python.py
+-rw-r--r--   0        0        0     3496 2024-03-26 22:59:00.143884 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/README.md
+-rw-r--r--   0        0        0      901 2024-03-26 22:59:00.144014 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/decision_tree.py
+-rw-r--r--   0        0        0      443 2024-03-26 22:59:00.144107 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/decision_tree_output.txt
+-rw-r--r--   0        0        0      234 2024-03-26 22:59:00.144198 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/decision_tree_tool.cwl
+-rw-r--r--   0        0        0      178 2024-03-26 22:59:00.144279 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/expectedValue.txt
+-rw-r--r--   0        0        0      157 2024-03-26 22:59:00.144363 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/hiring1.txt
+-rw-r--r--   0        0        0      467 2024-03-26 22:59:00.144442 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/linear_regress_output.txt
+-rw-r--r--   0        0        0     1203 2024-03-26 22:59:00.144530 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/linear_regression.py
+-rw-r--r--   0        0        0      692 2024-03-26 22:59:00.144618 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/machinelearning_pipeline.cwl
+-rw-r--r--   0        0        0    12405 2024-03-26 22:59:00.144766 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/out.PNG
+-rw-r--r--   0        0        0     1517 2024-03-26 22:59:00.144903 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/predict_code.py
+-rw-r--r--   0        0        0      336 2024-03-26 22:59:00.145003 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/predict_tool.cwl
+-rw-r--r--   0        0        0     1054 2024-03-26 22:59:00.145102 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/read_dataset.py
+-rw-r--r--   0        0        0      235 2024-03-26 22:59:00.145207 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/read_dataset_tool.cwl
+-rw-r--r--   0        0        0      239 2024-03-26 22:59:00.145310 hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/regress_tool.cwl
+-rw-r--r--   0        0        0       80 2024-03-26 22:59:00.145461 hpc_beeflow-0.1.8/beeflow/data/dockerfiles/Dockerfile.builder_demo
+-rw-r--r--   0        0        0      411 2024-03-26 22:59:00.145599 hpc_beeflow-0.1.8/beeflow/data/dockerfiles/Dockerfile.clamr-ffmpeg
+-rw-r--r--   0        0        0      145 2024-03-26 22:59:00.145695 hpc_beeflow-0.1.8/beeflow/data/dockerfiles/Dockerfile.clamr-lanl-x86_64
+-rw-r--r--   0        0        0      724 2024-03-26 22:59:00.145798 hpc_beeflow-0.1.8/beeflow/data/dockerfiles/Dockerfile.clamr-ppc64le
+-rw-r--r--   0        0        0     3698 2024-03-26 22:59:00.145922 hpc_beeflow-0.1.8/beeflow/data/dockerfiles/Dockerfile.comd-flux-x86_64
+-rw-r--r--   0        0        0     2303 2024-03-26 22:59:00.146047 hpc_beeflow-0.1.8/beeflow/data/dockerfiles/Dockerfile.comd-x86_64
+-rw-r--r--   0        0        0      270 2024-03-26 22:59:00.146162 hpc_beeflow-0.1.8/beeflow/data/dockerfiles/Dockerfile.deb9ompi-x86_64
+-rw-r--r--   0        0        0     2592 2024-03-26 22:59:00.146267 hpc_beeflow-0.1.8/beeflow/data/dockerfiles/Dockerfile.lulesh-x86_64
+-rw-r--r--   0        0        0     1605 2024-03-26 22:59:00.146377 hpc_beeflow-0.1.8/beeflow/data/dockerfiles/Dockerfile.neo4j-ppc64le
+-rw-r--r--   0        0        0     2489 2024-03-26 22:59:00.146489 hpc_beeflow-0.1.8/beeflow/data/dockerfiles/Dockerfile.nwchem-x86_64
+-rw-r--r--   0        0        0     3881 2024-03-26 22:59:00.146605 hpc_beeflow-0.1.8/beeflow/data/dockerfiles/Dockerfile.pennant-flux-x86_64
+-rw-r--r--   0        0        0     3446 2024-03-26 22:59:00.146740 hpc_beeflow-0.1.8/beeflow/data/dockerfiles/Dockerfile.vaspompi-x86_64
+-rw-r--r--   0        0        0      614 2024-03-26 22:59:00.146876 hpc_beeflow-0.1.8/beeflow/data/dockerfiles/README.md
+-rw-r--r--   0        0        0      331 2024-03-26 22:59:00.147063 hpc_beeflow-0.1.8/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.comd-x86_64-wpmix
+-rw-r--r--   0        0        0      573 2024-03-26 22:59:00.147190 hpc_beeflow-0.1.8/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.debian
+-rw-r--r--   0        0        0     3941 2024-03-26 22:59:00.147315 hpc_beeflow-0.1.8/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.openmpi-3.1.5
+-rw-r--r--   0        0        0      509 2024-03-26 22:59:00.147420 hpc_beeflow-0.1.8/beeflow/data/dockerfiles/comd-pmix-support/README.md
+-rw-r--r--   0        0        0      813 2024-03-26 22:59:00.147595 hpc_beeflow-0.1.8/beeflow/data/dockerfiles/comd-pmix-support/dont-init-ucx-on-intel-cray.patch
+-rw-r--r--   0        0        0      789 2024-03-26 22:59:00.147796 hpc_beeflow-0.1.8/beeflow/data/dockerfiles/pennant-graph/Dockerfile.pennant-graph-x86_64
+-rw-r--r--   0        0        0     1294 2024-03-26 22:59:00.147912 hpc_beeflow-0.1.8/beeflow/data/dockerfiles/pennant-graph/graph_pennant.py
+-rw-r--r--   0        0        0      110 2024-03-26 22:59:00.148036 hpc_beeflow-0.1.8/beeflow/data/dockerfiles/pennant-graph/graph_pennant.sh
+-rw-r--r--   0        0        0      640 2024-03-26 22:59:00.148190 hpc_beeflow-0.1.8/beeflow/enhanced_client/README.rst
+-rw-r--r--   0        0        0        0 2024-03-26 22:59:00.148338 hpc_beeflow-0.1.8/beeflow/enhanced_client/data/.gitkeep
+-rw-r--r--   0        0        0      386 2024-03-26 22:59:00.148456 hpc_beeflow-0.1.8/beeflow/enhanced_client/forge.config.js
+-rw-r--r--   0        0        0     1682 2024-03-26 22:59:00.148551 hpc_beeflow-0.1.8/beeflow/enhanced_client/main.js
+-rw-r--r--   0        0        0   231716 2024-04-02 20:32:24.403546 hpc_beeflow-0.1.8/beeflow/enhanced_client/package-lock.json
+-rw-r--r--   0        0        0     1078 2024-03-26 22:59:00.149467 hpc_beeflow-0.1.8/beeflow/enhanced_client/package.json
+-rw-r--r--   0        0        0     1219 2024-03-26 22:59:00.149633 hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/app.js
+-rw-r--r--   0        0        0     5151 2024-03-26 22:59:00.149784 hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/client.js
+-rw-r--r--   0        0        0      872 2024-03-26 22:59:00.149886 hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/config.js
+-rw-r--r--   0        0        0     2013 2024-03-26 22:59:00.149982 hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/control.js
+-rw-r--r--   0        0        0     3610 2024-03-26 22:59:00.150594 hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/database.js
+-rw-r--r--   0        0        0    12140 2024-03-26 22:59:00.150769 hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/display.js
+-rw-r--r--   0        0        0      455 2024-03-26 22:59:00.150879 hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/gdb.js
+-rw-r--r--   0        0        0    33601 2024-03-26 22:59:00.151204 hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/img/logo.png
+-rw-r--r--   0        0        0     2751 2024-03-26 22:59:00.151356 hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/main.html
+-rw-r--r--   0        0        0   206620 2024-03-26 22:59:00.152028 hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/styles/bulma.min.css
+-rw-r--r--   0        0        0      374 2024-03-26 22:59:00.152169 hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/styles/main.css
+-rw-r--r--   0        0        0      498 2024-03-26 22:59:00.152280 hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/tunnel.js
+-rw-r--r--   0        0        0      428 2024-03-26 22:59:00.152390 hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/viz.html
+-rw-r--r--   0        0        0     1071 2024-03-26 22:59:00.152524 hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/viz.js
+-rw-r--r--   0        0        0     7603 2024-03-26 22:59:00.152667 hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/workflows.js
+-rw-r--r--   0        0        0     1708 2024-03-26 22:59:00.152826 hpc_beeflow-0.1.8/beeflow/scheduler/README.md
+-rw-r--r--   0        0        0    10098 2024-03-26 22:59:00.152999 hpc_beeflow-0.1.8/beeflow/scheduler/algorithms.py
+-rw-r--r--   0        0        0     9347 2024-03-26 22:59:00.153122 hpc_beeflow-0.1.8/beeflow/scheduler/resource_allocation.py
+-rw-r--r--   0        0        0     3738 2024-03-26 22:59:00.153246 hpc_beeflow-0.1.8/beeflow/scheduler/scheduler.py
+-rw-r--r--   0        0        0     2890 2024-03-26 22:59:00.153401 hpc_beeflow-0.1.8/beeflow/scheduler/scheduler.yaml
+-rw-r--r--   0        0        0      708 2024-03-26 22:59:00.153526 hpc_beeflow-0.1.8/beeflow/scheduler/serializable.py
+-rw-r--r--   0        0        0     2296 2024-03-26 22:59:00.153644 hpc_beeflow-0.1.8/beeflow/scheduler/task.py
+-rw-r--r--   0        0        0     5500 2024-04-02 20:31:14.883205 hpc_beeflow-0.1.8/beeflow/task_manager/background.py
+-rw-r--r--   0        0        0     1239 2024-03-26 22:59:00.153977 hpc_beeflow-0.1.8/beeflow/task_manager/task_actions.py
+-rw-r--r--   0        0        0     1538 2024-03-26 22:59:00.154073 hpc_beeflow-0.1.8/beeflow/task_manager/task_manager.py
+-rw-r--r--   0        0        0      856 2024-03-26 22:59:00.154176 hpc_beeflow-0.1.8/beeflow/task_manager/task_submit.py
+-rw-r--r--   0        0        0     3602 2024-03-26 22:59:00.154292 hpc_beeflow-0.1.8/beeflow/task_manager/utils.py
+-rw-r--r--   0        0        0    34925 2024-03-26 22:59:00.154613 hpc_beeflow-0.1.8/beeflow/tests/42.tgz
+-rw-r--r--   0        0        0      236 2024-03-26 22:59:00.154727 hpc_beeflow-0.1.8/beeflow/tests/README.md
+-rw-r--r--   0        0        0     1139 2024-03-26 22:59:00.154837 hpc_beeflow-0.1.8/beeflow/tests/cf.cwl
+-rw-r--r--   0        0        0     1093 2024-03-26 22:59:00.155105 hpc_beeflow-0.1.8/beeflow/tests/clamr-wf/clamr.cwl
+-rw-r--r--   0        0        0      302 2024-03-26 22:59:00.155214 hpc_beeflow-0.1.8/beeflow/tests/clamr-wf/clamr_job.json
+-rw-r--r--   0        0        0      424 2024-03-26 22:59:00.155326 hpc_beeflow-0.1.8/beeflow/tests/clamr-wf/clamr_job.yml
+-rw-r--r--   0        0        0     1320 2024-03-26 22:59:00.155432 hpc_beeflow-0.1.8/beeflow/tests/clamr-wf/clamr_wf.cwl
+-rw-r--r--   0        0        0      680 2024-03-26 22:59:00.155532 hpc_beeflow-0.1.8/beeflow/tests/clamr-wf/ffmpeg.cwl
+-rw-r--r--   0        0        0      273 2024-03-26 22:59:00.155655 hpc_beeflow-0.1.8/beeflow/tests/clamr-wf/mv_script.cwl
+-rwxr-xr-x   0        0        0      324 2024-03-26 22:59:00.155767 hpc_beeflow-0.1.8/beeflow/tests/clamr-wf/mv_script.sh
+-rw-r--r--   0        0        0     2401 2024-03-26 22:59:00.154950 hpc_beeflow-0.1.8/beeflow/tests/clamr-wf.tgz
+-rw-r--r--   0        0        0      774 2024-03-26 22:59:00.155864 hpc_beeflow-0.1.8/beeflow/tests/gdb.py
+-rw-r--r--   0        0        0    12378 2024-03-26 22:59:00.155977 hpc_beeflow-0.1.8/beeflow/tests/mocks.py
+-rw-r--r--   0        0        0      267 2024-03-26 22:59:00.156078 hpc_beeflow-0.1.8/beeflow/tests/test_cloud.py
+-rw-r--r--   0        0        0     6006 2024-03-26 22:59:00.156230 hpc_beeflow-0.1.8/beeflow/tests/test_config_validator.py
+-rw-r--r--   0        0        0      807 2024-03-26 22:59:00.156323 hpc_beeflow-0.1.8/beeflow/tests/test_container_path.py
+-rw-r--r--   0        0        0      946 2024-03-26 22:59:00.156420 hpc_beeflow-0.1.8/beeflow/tests/test_db_sched.py
+-rw-r--r--   0        0        0     4410 2024-03-26 22:59:00.156541 hpc_beeflow-0.1.8/beeflow/tests/test_db_tm.py
+-rw-r--r--   0        0        0    16813 2024-03-26 23:05:21.152824 hpc_beeflow-0.1.8/beeflow/tests/test_parser.py
+-rw-r--r--   0        0        0    15134 2024-03-26 22:59:00.156968 hpc_beeflow-0.1.8/beeflow/tests/test_scheduler.py
+-rw-r--r--   0        0        0     2630 2024-03-26 22:59:00.157106 hpc_beeflow-0.1.8/beeflow/tests/test_scheduler_resource_allocation.py
+-rw-r--r--   0        0        0     6557 2024-03-26 22:59:00.157241 hpc_beeflow-0.1.8/beeflow/tests/test_scheduler_rest.py
+-rw-r--r--   0        0        0     4908 2024-03-26 22:59:00.157404 hpc_beeflow-0.1.8/beeflow/tests/test_slurm_worker.py
+-rw-r--r--   0        0        0     3796 2024-03-26 22:59:00.157535 hpc_beeflow-0.1.8/beeflow/tests/test_tm.py
+-rw-r--r--   0        0        0    33819 2024-03-26 22:59:00.157735 hpc_beeflow-0.1.8/beeflow/tests/test_wf_interface.py
+-rw-r--r--   0        0        0    11213 2024-04-02 20:31:14.883764 hpc_beeflow-0.1.8/beeflow/tests/test_wf_manager.py
+-rwxr-xr-x   0        0        0     7823 2024-03-26 22:59:00.158109 hpc_beeflow-0.1.8/beeflow/wf_manager/common/dep_manager.py
+-rw-r--r--   0        0        0    10373 2024-03-26 22:59:00.158227 hpc_beeflow-0.1.8/beeflow/wf_manager/common/wf_db.py
+-rw-r--r--   0        0        0     4722 2024-04-02 20:31:14.884248 hpc_beeflow-0.1.8/beeflow/wf_manager/resources/wf_actions.py
+-rw-r--r--   0        0        0     8674 2024-03-26 22:59:00.158538 hpc_beeflow-0.1.8/beeflow/wf_manager/resources/wf_list.py
+-rw-r--r--   0        0        0      560 2024-03-26 22:59:00.158619 hpc_beeflow-0.1.8/beeflow/wf_manager/resources/wf_metadata.py
+-rw-r--r--   0        0        0     6266 2024-04-02 20:31:14.884876 hpc_beeflow-0.1.8/beeflow/wf_manager/resources/wf_update.py
+-rw-r--r--   0        0        0     8816 2024-03-26 22:59:00.158856 hpc_beeflow-0.1.8/beeflow/wf_manager/resources/wf_utils.py
+-rw-r--r--   0        0        0     1793 2024-03-26 22:59:00.158967 hpc_beeflow-0.1.8/beeflow/wf_manager/wf_manager.py
+-rw-r--r--   0        0        0     2713 2024-04-02 20:32:24.404164 hpc_beeflow-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     7390 1970-01-01 00:00:00.000000 hpc_beeflow-0.1.8/PKG-INFO
```

### Comparing `hpc-beeflow-0.1.7/LICENSE` & `hpc_beeflow-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/README.rst` & `hpc_beeflow-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/client/bee_client.py` & `hpc_beeflow-0.1.8/beeflow/client/bee_client.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/client/core.py` & `hpc_beeflow-0.1.8/beeflow/client/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,14 @@
 from beeflow.common import paths
 from beeflow.wf_manager.resources import wf_utils
 
 from beeflow.common.db import wfm_db
 from beeflow.common.db.bdb import connect_db
 from beeflow.wf_manager.common import dep_manager
 
-db_path = wf_utils.get_db_path()
-
 
 class ComponentManager:
     """Component manager class."""
 
     def __init__(self):
         """Construct the component manager."""
         self.components = {}
@@ -463,14 +461,15 @@
     beeflow_log = paths.log_fname('beeflow')
     if query == "no":
         print(f'Beeflow has stopped. Check the log at "{beeflow_log}".')
 
 
 def kill_active_workflows(active_states, workflow_list):
     """Kill workflows with active states."""
+    db_path = wf_utils.get_db_path()
     db = connect_db(wfm_db, db_path)
     success = True
     for name, wf_id, state in workflow_list:
         if state in active_states:
             pid = db.workflows.get_gdb_pid(wf_id)
             if pid > 0:
                 dep_manager.kill_gdb(pid)
```

### Comparing `hpc-beeflow-0.1.7/beeflow/cloud_launcher.py` & `hpc_beeflow-0.1.8/beeflow/cloud_launcher.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/build/README.md` & `hpc_beeflow-0.1.8/beeflow/common/build/README.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/build/build_driver.py` & `hpc_beeflow-0.1.8/beeflow/common/build/build_driver.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/build/container_drivers.py` & `hpc_beeflow-0.1.8/beeflow/common/build/container_drivers.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/build/utils.py` & `hpc_beeflow-0.1.8/beeflow/common/build/utils.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/build_interfaces.py` & `hpc_beeflow-0.1.8/beeflow/common/build_interfaces.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/cli_connection.py` & `hpc_beeflow-0.1.8/beeflow/common/cli_connection.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/cloud/README.md` & `hpc_beeflow-0.1.8/beeflow/common/cloud/README.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/cloud/__init__.py` & `hpc_beeflow-0.1.8/beeflow/common/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/cloud/chameleoncloud.py` & `hpc_beeflow-0.1.8/beeflow/common/cloud/chameleoncloud.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/cloud/google.py` & `hpc_beeflow-0.1.8/beeflow/common/cloud/google.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/cloud/openstack.py` & `hpc_beeflow-0.1.8/beeflow/common/cloud/openstack.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/cloud/provider.py` & `hpc_beeflow-0.1.8/beeflow/common/cloud/provider.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/config_driver.py` & `hpc_beeflow-0.1.8/beeflow/common/config_driver.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/config_validator.py` & `hpc_beeflow-0.1.8/beeflow/common/config_validator.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/connection.py` & `hpc_beeflow-0.1.8/beeflow/common/connection.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/container_path.py` & `hpc_beeflow-0.1.8/beeflow/common/container_path.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/crt/charliecloud_driver.py` & `hpc_beeflow-0.1.8/beeflow/common/crt/charliecloud_driver.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/crt/crt_driver.py` & `hpc_beeflow-0.1.8/beeflow/common/crt/crt_driver.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/crt/singularity_driver.py` & `hpc_beeflow-0.1.8/beeflow/common/crt/singularity_driver.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/crt_interface.py` & `hpc_beeflow-0.1.8/beeflow/common/crt_interface.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/db/bdb.py` & `hpc_beeflow-0.1.8/beeflow/common/db/bdb.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/db/sched_db.py` & `hpc_beeflow-0.1.8/beeflow/common/db/sched_db.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/db/tm_db.py` & `hpc_beeflow-0.1.8/beeflow/common/db/tm_db.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/db/wfm_db.py` & `hpc_beeflow-0.1.8/beeflow/common/db/wfm_db.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/expr.py` & `hpc_beeflow-0.1.8/beeflow/common/expr.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/gdb/DESIGN.md` & `hpc_beeflow-0.1.8/beeflow/common/gdb/DESIGN.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/gdb/gdb_driver.py` & `hpc_beeflow-0.1.8/beeflow/common/gdb/gdb_driver.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/gdb/neo4j_cypher.py` & `hpc_beeflow-0.1.8/beeflow/common/gdb/neo4j_cypher.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/gdb/neo4j_driver.py` & `hpc_beeflow-0.1.8/beeflow/common/gdb/neo4j_driver.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/gdb_interface.py` & `hpc_beeflow-0.1.8/beeflow/common/gdb_interface.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/integration/generated_workflows.py` & `hpc_beeflow-0.1.8/beeflow/common/integration/generated_workflows.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/integration/utils.py` & `hpc_beeflow-0.1.8/beeflow/common/integration/utils.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/integration_test.py` & `hpc_beeflow-0.1.8/beeflow/common/integration_test.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/log.py` & `hpc_beeflow-0.1.8/beeflow/common/log.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/parser/README.md` & `hpc_beeflow-0.1.8/beeflow/common/parser/README.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/parser/parser.py` & `hpc_beeflow-0.1.8/beeflow/common/parser/parser.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/paths.py` & `hpc_beeflow-0.1.8/beeflow/common/paths.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/validation.py` & `hpc_beeflow-0.1.8/beeflow/common/validation.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/wf_data.py` & `hpc_beeflow-0.1.8/beeflow/common/wf_data.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/wf_interface.py` & `hpc_beeflow-0.1.8/beeflow/common/wf_interface.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/wf_profiler.py` & `hpc_beeflow-0.1.8/beeflow/common/wf_profiler.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/worker/__init__.py` & `hpc_beeflow-0.1.8/beeflow/common/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/worker/flux_worker.py` & `hpc_beeflow-0.1.8/beeflow/common/worker/flux_worker.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/worker/lsf_worker.py` & `hpc_beeflow-0.1.8/beeflow/common/worker/lsf_worker.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/worker/simple_worker.py` & `hpc_beeflow-0.1.8/beeflow/common/worker/simple_worker.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/worker/slurm_worker.py` & `hpc_beeflow-0.1.8/beeflow/common/worker/slurm_worker.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/worker/worker.py` & `hpc_beeflow-0.1.8/beeflow/common/worker/worker.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/common/worker_interface.py` & `hpc_beeflow-0.1.8/beeflow/common/worker_interface.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cloud_templates/dora.jinja` & `hpc_beeflow-0.1.8/beeflow/data/cloud_templates/dora.jinja`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cloud_templates/dora.yaml` & `hpc_beeflow-0.1.8/beeflow/data/cloud_templates/dora.yaml`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/README.md` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/README.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/blast_wf.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/blast/blast_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/blast_worker001.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/blast/blast_worker001.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/blast_worker002.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/blast/blast_worker002.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/blast/input/small.fasta` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/blast/input/small.fasta`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/cat-grep-fail/lorem.txt` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/cat-grep-fail/lorem.txt`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/cat-grep-fail/workflow.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/cat-grep-fail/workflow.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ci/clamr.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-ci/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_wf.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-ci/clamr_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ci/ffmpeg.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-ci/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/clamr.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/clamr_wf.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/clamr_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/ffmpeg.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-ffmpeg-build_script/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf/clamr.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_wf.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf/clamr_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf/ffmpeg.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_wf.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/clamr_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/ffmpeg.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-chicoma/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/README.md` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/README.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/lsf-charliecloud/cf-summit.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/lsf-charliecloud/cf-summit.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/README.md` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/README.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-darwin.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-darwin.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-no-owrite.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf-no-owrite.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/cf.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/copyContainer_containerName.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/copyContainer_containerName.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerFile_containerName.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerFile_containerName.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerPull.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-charliecloud/dockerPull.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-singularity/cf-singularity.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-noyaml/slurm-singularity/cf-singularity.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_wf.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/clamr_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/ffmpeg.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-singularity/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_wf.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-summit/clamr_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-summit/ffmpeg.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-summit/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_wf.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/clamr_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/ffmpeg.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/clamr-wf-use-container/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/comd-mpi/comd.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/comd-mpi/comd.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/comd-mpi/comd_wf.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/comd-mpi/comd_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/lulesh-mpi/lulesh.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/lulesh-mpi/lulesh.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/nwchem-mpi/README.md` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/nwchem-mpi/README.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/nwchem-mpi/nwchem.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant/pennant_wf.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant/pennant_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/Dockerfile.pennant-flux-x86_64` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant-build/Dockerfile.pennant-flux-x86_64`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/Dockerfile.pennant-graph-x86_64` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant-build/Dockerfile.pennant-graph-x86_64`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/graph_pennant.py` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant-build/graph_pennant.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/pennant-build/pennant_wf.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/pennant-build/pennant_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/simple-workflows/cancel.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/simple-workflows/cancel.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc-nc.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc-nc.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/gc.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/lorem.txt` & `hpc_beeflow-0.1.8/beeflow/data/cwl/bee_workflows/simple-workflows/grep-wordcount/lorem.txt`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/grep-wordcount/gc.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/grep-wordcount/gc.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/grep-wordcount/lorem.txt` & `hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/grep-wordcount/lorem.txt`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/DAG_example-1.png` & `hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/DAG_example-1.png`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/README.md` & `hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/example-1/README.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/README.md` & `hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/README.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/decision_tree.py` & `hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/decision_tree.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/linear_regression.py` & `hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/linear_regression.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/machinelearning_pipeline.cwl` & `hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/machinelearning_pipeline.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/out.PNG` & `hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/out.PNG`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/predict_code.py` & `hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/predict_code.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/read_dataset.py` & `hpc_beeflow-0.1.8/beeflow/data/cwl/cwl_validation/ml-workflow/machine_learning/read_dataset.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.clamr-ppc64le` & `hpc_beeflow-0.1.8/beeflow/data/dockerfiles/Dockerfile.clamr-ppc64le`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.comd-flux-x86_64` & `hpc_beeflow-0.1.8/beeflow/data/dockerfiles/Dockerfile.comd-flux-x86_64`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.comd-x86_64` & `hpc_beeflow-0.1.8/beeflow/data/dockerfiles/Dockerfile.comd-x86_64`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.lulesh-x86_64` & `hpc_beeflow-0.1.8/beeflow/data/dockerfiles/Dockerfile.lulesh-x86_64`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.neo4j-ppc64le` & `hpc_beeflow-0.1.8/beeflow/data/dockerfiles/Dockerfile.neo4j-ppc64le`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.nwchem-x86_64` & `hpc_beeflow-0.1.8/beeflow/data/dockerfiles/Dockerfile.nwchem-x86_64`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.pennant-flux-x86_64` & `hpc_beeflow-0.1.8/beeflow/data/dockerfiles/Dockerfile.pennant-flux-x86_64`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/Dockerfile.vaspompi-x86_64` & `hpc_beeflow-0.1.8/beeflow/data/dockerfiles/Dockerfile.vaspompi-x86_64`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/README.md` & `hpc_beeflow-0.1.8/beeflow/data/dockerfiles/README.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.debian` & `hpc_beeflow-0.1.8/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.debian`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.openmpi-3.1.5` & `hpc_beeflow-0.1.8/beeflow/data/dockerfiles/comd-pmix-support/Dockerfile.openmpi-3.1.5`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/comd-pmix-support/dont-init-ucx-on-intel-cray.patch` & `hpc_beeflow-0.1.8/beeflow/data/dockerfiles/comd-pmix-support/dont-init-ucx-on-intel-cray.patch`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/pennant-graph/Dockerfile.pennant-graph-x86_64` & `hpc_beeflow-0.1.8/beeflow/data/dockerfiles/pennant-graph/Dockerfile.pennant-graph-x86_64`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/data/dockerfiles/pennant-graph/graph_pennant.py` & `hpc_beeflow-0.1.8/beeflow/data/dockerfiles/pennant-graph/graph_pennant.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/enhanced_client/README.rst` & `hpc_beeflow-0.1.8/beeflow/enhanced_client/README.rst`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/enhanced_client/main.js` & `hpc_beeflow-0.1.8/beeflow/enhanced_client/main.js`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/enhanced_client/package-lock.json` & `hpc_beeflow-0.1.8/beeflow/enhanced_client/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999412593984962%*

 * *Differences: {"'packages'": "{'node_modules/follow-redirects': {'version': '1.15.6', 'resolved': "*

 * *               "'https://registry.npmjs.org/follow-redirects/-/follow-redirects-1.15.6.tgz', "*

 * *               "'integrity': "*

 * *               "'sha512-wWN62YITEaOpSK584EZXJafH1AGpO8RVgElfkuXbTOrPX4fIfOyEpW/CsiNd8JdYrAoOvafRTOEnvsO++qCqFA=='}, "*

 * *               "'node_modules/ip': {'version': '2.0.1', 'resolved': "*

 * *               "'https://registry.npmjs.org/ip/-/ip-2.0.1.tgz', 'integrity': "*

 * *               "'sha512-lJUL9imLT […]*

```diff
@@ -3190,22 +3190,22 @@
             },
             "funding": [
                 {
                     "type": "individual",
                     "url": "https://github.com/sponsors/RubenVerborgh"
                 }
             ],
-            "integrity": "sha512-vSFWUON1B+yAw1VN4xMfxgn5fTUiaOzAJCKBwIIgT/+7CuGy9+r+5gITvP62j3RmaD5Ph65UaERdOSRGUzZtgw==",
+            "integrity": "sha512-wWN62YITEaOpSK584EZXJafH1AGpO8RVgElfkuXbTOrPX4fIfOyEpW/CsiNd8JdYrAoOvafRTOEnvsO++qCqFA==",
             "peerDependenciesMeta": {
                 "debug": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/follow-redirects/-/follow-redirects-1.15.5.tgz",
-            "version": "1.15.5"
+            "resolved": "https://registry.npmjs.org/follow-redirects/-/follow-redirects-1.15.6.tgz",
+            "version": "1.15.6"
         },
         "node_modules/form-data": {
             "dependencies": {
                 "asynckit": "^0.4.0",
                 "combined-stream": "^1.0.8",
                 "mime-types": "^2.1.12"
             },
@@ -3765,17 +3765,17 @@
             },
             "integrity": "sha512-6xwYfHbajpoF0xLW+iwLkhwgvLoZDfjYfoFNu8ftMoXINzwuymNLd9u/KmwtdT2GbR+/Cz66otEGEVVUHX9QLQ==",
             "resolved": "https://registry.npmjs.org/interpret/-/interpret-3.1.1.tgz",
             "version": "3.1.1"
         },
         "node_modules/ip": {
             "dev": true,
-            "integrity": "sha512-WKa+XuLG1A1R0UWhl2+1XQSi+fZWMsYKffMZTTYsiZaUD8k2yDAj5atimTUD2TZkyCkNEeYE5NhFZmupOGtjYQ==",
-            "resolved": "https://registry.npmjs.org/ip/-/ip-2.0.0.tgz",
-            "version": "2.0.0"
+            "integrity": "sha512-lJUL9imLTNi1ZfXT+DU6rBBdbiKGBuay9B6xGSPVjUeQwaH1RIGqef8RZkUtHioLmSNpPR5M4HVKJGm1j8FWVQ==",
+            "resolved": "https://registry.npmjs.org/ip/-/ip-2.0.1.tgz",
+            "version": "2.0.1"
         },
         "node_modules/is-arrayish": {
             "dev": true,
             "integrity": "sha512-zz06S8t0ozoDXMG+ube26zeCTNXcKIPJZJi8hBrF4idCLms4CG9QtK7qBl1boi5ODzFpjswb5JPmHCbMpjaYzg==",
             "resolved": "https://registry.npmjs.org/is-arrayish/-/is-arrayish-0.2.1.tgz",
             "version": "0.2.1"
         },
```

### Comparing `hpc-beeflow-0.1.7/beeflow/enhanced_client/package.json` & `hpc_beeflow-0.1.8/beeflow/enhanced_client/package.json`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/app.js` & `hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/app.js`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/client.js` & `hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/client.js`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/config.js` & `hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/config.js`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/control.js` & `hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/control.js`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/database.js` & `hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/database.js`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/display.js` & `hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/display.js`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/img/logo.png` & `hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/img/logo.png`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/main.html` & `hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/main.html`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/styles/bulma.min.css` & `hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/styles/bulma.min.css`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/viz.js` & `hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/viz.js`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/enhanced_client/renderer/workflows.js` & `hpc_beeflow-0.1.8/beeflow/enhanced_client/renderer/workflows.js`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/scheduler/README.md` & `hpc_beeflow-0.1.8/beeflow/scheduler/README.md`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/scheduler/algorithms.py` & `hpc_beeflow-0.1.8/beeflow/scheduler/algorithms.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/scheduler/resource_allocation.py` & `hpc_beeflow-0.1.8/beeflow/scheduler/resource_allocation.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/scheduler/scheduler.py` & `hpc_beeflow-0.1.8/beeflow/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/scheduler/scheduler.yaml` & `hpc_beeflow-0.1.8/beeflow/scheduler/scheduler.yaml`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/scheduler/serializable.py` & `hpc_beeflow-0.1.8/beeflow/scheduler/serializable.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/scheduler/task.py` & `hpc_beeflow-0.1.8/beeflow/scheduler/task.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/task_manager/background.py` & `hpc_beeflow-0.1.8/beeflow/task_manager/background.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/task_manager/task_actions.py` & `hpc_beeflow-0.1.8/beeflow/task_manager/task_actions.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/task_manager/task_manager.py` & `hpc_beeflow-0.1.8/beeflow/task_manager/task_manager.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/task_manager/task_submit.py` & `hpc_beeflow-0.1.8/beeflow/task_manager/task_submit.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/task_manager/utils.py` & `hpc_beeflow-0.1.8/beeflow/task_manager/utils.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/tests/42.tgz` & `hpc_beeflow-0.1.8/beeflow/tests/42.tgz`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/tests/cf.cwl` & `hpc_beeflow-0.1.8/beeflow/tests/cf.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/tests/clamr-wf/clamr.cwl` & `hpc_beeflow-0.1.8/beeflow/tests/clamr-wf/clamr.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/tests/clamr-wf/clamr_wf.cwl` & `hpc_beeflow-0.1.8/beeflow/tests/clamr-wf/clamr_wf.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/tests/clamr-wf/ffmpeg.cwl` & `hpc_beeflow-0.1.8/beeflow/tests/clamr-wf/ffmpeg.cwl`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/tests/clamr-wf.tgz` & `hpc_beeflow-0.1.8/beeflow/tests/clamr-wf.tgz`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/tests/gdb.py` & `hpc_beeflow-0.1.8/beeflow/tests/gdb.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/tests/mocks.py` & `hpc_beeflow-0.1.8/beeflow/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/tests/test_config_validator.py` & `hpc_beeflow-0.1.8/beeflow/tests/test_config_validator.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/tests/test_container_path.py` & `hpc_beeflow-0.1.8/beeflow/tests/test_container_path.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/tests/test_db_sched.py` & `hpc_beeflow-0.1.8/beeflow/tests/test_db_sched.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/tests/test_db_tm.py` & `hpc_beeflow-0.1.8/beeflow/tests/test_db_tm.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/tests/test_parser.py` & `hpc_beeflow-0.1.8/beeflow/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/tests/test_scheduler.py` & `hpc_beeflow-0.1.8/beeflow/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/tests/test_scheduler_resource_allocation.py` & `hpc_beeflow-0.1.8/beeflow/tests/test_scheduler_resource_allocation.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/tests/test_scheduler_rest.py` & `hpc_beeflow-0.1.8/beeflow/tests/test_scheduler_rest.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/tests/test_slurm_worker.py` & `hpc_beeflow-0.1.8/beeflow/tests/test_slurm_worker.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/tests/test_tm.py` & `hpc_beeflow-0.1.8/beeflow/tests/test_tm.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/tests/test_wf_interface.py` & `hpc_beeflow-0.1.8/beeflow/tests/test_wf_interface.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/tests/test_wf_manager.py` & `hpc_beeflow-0.1.8/beeflow/tests/test_wf_manager.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/wf_manager/common/dep_manager.py` & `hpc_beeflow-0.1.8/beeflow/wf_manager/common/dep_manager.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/wf_manager/common/wf_db.py` & `hpc_beeflow-0.1.8/beeflow/wf_manager/common/wf_db.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/wf_manager/resources/wf_actions.py` & `hpc_beeflow-0.1.8/beeflow/wf_manager/resources/wf_actions.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/wf_manager/resources/wf_list.py` & `hpc_beeflow-0.1.8/beeflow/wf_manager/resources/wf_list.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/wf_manager/resources/wf_metadata.py` & `hpc_beeflow-0.1.8/beeflow/wf_manager/resources/wf_metadata.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/wf_manager/resources/wf_update.py` & `hpc_beeflow-0.1.8/beeflow/wf_manager/resources/wf_update.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/wf_manager/resources/wf_utils.py` & `hpc_beeflow-0.1.8/beeflow/wf_manager/resources/wf_utils.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/beeflow/wf_manager/wf_manager.py` & `hpc_beeflow-0.1.8/beeflow/wf_manager/wf_manager.py`

 * *Files identical despite different names*

### Comparing `hpc-beeflow-0.1.7/pyproject.toml` & `hpc_beeflow-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hpc-beeflow"
-version = "0.1.7"
+version = "0.1.8"
 description = "A software package for containerizing HPC applications and managing job workflows"
 
 
 authors = [
     "BEE-LANL Dev Team <bee-dev@lanl.gov>"
 ]
 
@@ -86,14 +86,14 @@
 pydocstyle = "6.1.1"
 pyflakes = "3.0.1"
 pylama = "8.4.1"
 pylint = "2.15.9"
 pytest = "7.2.0"
 pytest-mock = "3.3.1"
 # This is commented out until we can figure out why it's causing `poetry update` to loop forever
-sphinx = "^2.1"
+sphinx = "^6"
 sphinx-rtd-theme = "^1.0"
 cwltool = "^3.0.20200324120055"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `hpc-beeflow-0.1.7/PKG-INFO` & `hpc_beeflow-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpc-beeflow
-Version: 0.1.7
+Version: 0.1.8
 Summary: A software package for containerizing HPC applications and managing job workflows
 Home-page: https://github.com/lanl/BEE
 Keywords: bee,hpc,workflow,cluster,computing
 Author: BEE-LANL Dev Team
 Author-email: bee-dev@lanl.gov
 Requires-Python: >=3.8.3,<=3.12.2
 Classifier: Environment :: Console
@@ -12,37 +12,39 @@
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Clustering
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: System :: Monitoring
-Provides-Extra: cloud_extras
+Provides-Extra: cloud-extras
 Requires-Dist: APScheduler (>=3.6.3,<4.0.0)
 Requires-Dist: Flask (>=2.0,<3.0)
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: celery[redis,sqlalchemy] (>=5.3.4,<6.0.0)
 Requires-Dist: cffi (>=1.15.1,<2.0.0)
 Requires-Dist: cwl-utils (>=0.16,<0.17)
 Requires-Dist: flask_restful (==0.3.9)
-Requires-Dist: google-api-python-client (>=2.66.0,<3.0.0); extra == "cloud_extras"
+Requires-Dist: google-api-python-client (>=2.66.0,<3.0.0) ; extra == "cloud-extras"
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: jsonpickle (>=2.2.0,<3.0.0)
 Requires-Dist: neo4j (>=1.7.4,<2.0.0)
 Requires-Dist: python-daemon (>=2.3.1,<3.0.0)
-Requires-Dist: python-heatclient (>=3.1.0,<4.0.0); extra == "cloud_extras"
-Requires-Dist: python-openstackclient (>=6.0.0,<7.0.0); extra == "cloud_extras"
+Requires-Dist: python-heatclient (>=3.1.0,<4.0.0) ; extra == "cloud-extras"
+Requires-Dist: python-openstackclient (>=6.0.0,<7.0.0) ; extra == "cloud-extras"
 Requires-Dist: requests (<2.29.0)
 Requires-Dist: requests-unixsocket (>=0.3.0,<0.4.0)
 Requires-Dist: typer (>=0.5.0,<0.6.0)
 Project-URL: Repository, https://github.com/lanl/BEE
 Description-Content-Type: text/x-rst
 
 BEE: Build and Execution Environment
```

