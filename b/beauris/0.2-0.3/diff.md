# Comparing `tmp/beauris-0.2.tar.gz` & `tmp/beauris-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beauris-0.2.tar", last modified: Fri Nov 10 16:39:48 2023, max compression
+gzip compressed data, was "beauris-0.3.tar", last modified: Tue Apr  2 15:58:47 2024, max compression
```

## Comparing `beauris-0.2.tar` & `beauris-0.3.tar`

### file list

```diff
@@ -1,126 +1,142 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 16:39:48.337765 beauris-0.2/
--rw-rw-rw-   0 root         (0) root         (0)     1119 2023-11-10 16:39:32.000000 beauris-0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      817 2023-11-10 16:39:48.337765 beauris-0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1202 2023-11-10 16:39:32.000000 beauris-0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 16:39:48.321764 beauris-0.2/beauris/
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-11-10 16:39:32.000000 beauris-0.2/beauris/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4575 2023-11-10 16:39:32.000000 beauris-0.2/beauris/annotation.py
--rw-rw-rw-   0 root         (0) root         (0)     7385 2023-11-10 16:39:32.000000 beauris-0.2/beauris/assembly.py
--rw-rw-rw-   0 root         (0) root         (0)     1166 2023-11-10 16:39:32.000000 beauris-0.2/beauris/beauris.py
--rw-rw-rw-   0 root         (0) root         (0)     4638 2023-11-10 16:39:32.000000 beauris-0.2/beauris/blastbank.py
--rw-rw-rw-   0 root         (0) root         (0)     3958 2023-11-10 16:39:32.000000 beauris-0.2/beauris/config.py
--rw-rw-rw-   0 root         (0) root         (0)     8903 2023-11-10 16:39:32.000000 beauris-0.2/beauris/data_locker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 16:39:48.323764 beauris-0.2/beauris/es_parsers/
--rw-rw-rw-   0 root         (0) root         (0)      216 2023-11-10 16:39:32.000000 beauris-0.2/beauris/es_parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1985 2023-11-10 16:39:32.000000 beauris-0.2/beauris/es_parsers/diamond_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2269 2023-11-10 16:39:32.000000 beauris-0.2/beauris/es_parsers/eggnog_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2228 2023-11-10 16:39:32.000000 beauris-0.2/beauris/es_parsers/gff_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2023-11-10 16:39:32.000000 beauris-0.2/beauris/es_parsers/interpro_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2744 2023-11-10 16:39:32.000000 beauris-0.2/beauris/expression_data.py
--rw-rw-rw-   0 root         (0) root         (0)    19592 2023-11-10 16:39:32.000000 beauris-0.2/beauris/job_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     9721 2023-11-10 16:39:32.000000 beauris-0.2/beauris/managed_entity.py
--rw-rw-rw-   0 root         (0) root         (0)    10876 2023-11-10 16:39:32.000000 beauris-0.2/beauris/managed_file.py
--rw-rw-rw-   0 root         (0) root         (0)     9513 2023-11-10 16:39:32.000000 beauris-0.2/beauris/organism.py
--rw-rw-rw-   0 root         (0) root         (0)     2453 2023-11-10 16:39:32.000000 beauris-0.2/beauris/proteome.py
--rw-rw-rw-   0 root         (0) root         (0)    10884 2023-11-10 16:39:32.000000 beauris-0.2/beauris/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 16:39:48.324764 beauris-0.2/beauris/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-11-10 16:39:32.000000 beauris-0.2/beauris/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6472 2023-11-10 16:39:32.000000 beauris-0.2/beauris/tasks/annotation.py
--rw-rw-rw-   0 root         (0) root         (0)     2075 2023-11-10 16:39:32.000000 beauris-0.2/beauris/tasks/assembly.py
--rw-rw-rw-   0 root         (0) root         (0)     4403 2023-11-10 16:39:32.000000 beauris-0.2/beauris/tasks/organism.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-11-10 16:39:32.000000 beauris-0.2/beauris/tasks/proteome.py
--rw-rw-rw-   0 root         (0) root         (0)     1086 2023-11-10 16:39:32.000000 beauris-0.2/beauris/tasks/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1015 2023-11-10 16:39:32.000000 beauris-0.2/beauris/tasks/track.py
--rw-rw-rw-   0 root         (0) root         (0)      850 2023-11-10 16:39:32.000000 beauris-0.2/beauris/tasks/transcriptome.py
--rw-rw-rw-   0 root         (0) root         (0)     3545 2023-11-10 16:39:32.000000 beauris-0.2/beauris/track.py
--rw-rw-rw-   0 root         (0) root         (0)     2499 2023-11-10 16:39:32.000000 beauris-0.2/beauris/transcriptome.py
--rw-rw-rw-   0 root         (0) root         (0)     2178 2023-11-10 16:39:32.000000 beauris-0.2/beauris/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 16:39:48.324764 beauris-0.2/beauris/validation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-10 16:39:32.000000 beauris-0.2/beauris/validation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 16:39:48.325765 beauris-0.2/beauris/validation/ogs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-10 16:39:32.000000 beauris-0.2/beauris/validation/ogs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-11-10 16:39:32.000000 beauris-0.2/beauris/validation/ogs/fasta_check.py
--rw-rw-rw-   0 root         (0) root         (0)    22629 2023-11-10 16:39:32.000000 beauris-0.2/beauris/validation/ogs/ogs_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 16:39:48.326764 beauris-0.2/beauris/validation/template/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-10 16:39:32.000000 beauris-0.2/beauris/validation/template/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1495 2023-11-10 16:39:32.000000 beauris-0.2/beauris/validation/template/ext.py
--rw-rw-rw-   0 root         (0) root         (0)     7736 2023-11-10 16:39:32.000000 beauris-0.2/beauris/validation/template/schema.yaml
--rw-rw-rw-   0 root         (0) root         (0)    21399 2023-11-10 16:39:32.000000 beauris-0.2/beauris/web_interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 16:39:48.326764 beauris-0.2/beauris/workflows/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 16:39:48.315764 beauris-0.2/beauris/workflows/ansible/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 16:39:48.315764 beauris-0.2/beauris/workflows/ansible/ansible_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 16:39:48.327764 beauris-0.2/beauris/workflows/ansible/ansible_data/project/
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/ansible/ansible_data/project/playbook_deploy.yml
--rw-rw-rw-   0 root         (0) root         (0)      276 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/ansible/ansible_data/project/playbook_shutdown.yml
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/ansible/ansible_data/project/playbook_update.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 16:39:48.327764 beauris-0.2/beauris/workflows/ansible/docker_files/
--rwxrwxrwx   0 root         (0) root         (0)    12385 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/ansible/docker_files/postgres-blast-entrypoint.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 16:39:48.328765 beauris-0.2/beauris/workflows/ansible/templates/
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/ansible/templates/default.conf.j2
--rw-rw-rw-   0 root         (0) root         (0)     8191 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/ansible/templates/docker-compose.yml.j2
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/ansible/templates/genoboo.json.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 16:39:48.328765 beauris-0.2/beauris/workflows/ansible/templates/web/
--rw-rw-rw-   0 root         (0) root         (0)     1663 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/ansible/templates/web/index.html.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 16:39:48.331765 beauris-0.2/beauris/workflows/drmaa/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/drmaa/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2018 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/drmaa/add_fa_description.py
--rw-rw-rw-   0 root         (0) root         (0)     1222 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/drmaa/add_gff_description.py
--rw-rw-rw-   0 root         (0) root         (0)     1680 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/drmaa/bam_to_wig.py
--rwxrwxrwx   0 root         (0) root         (0)      283 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/drmaa/bam_to_wig.sh
--rw-rw-rw-   0 root         (0) root         (0)     1588 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/drmaa/blastdb.py
--rwxrwxrwx   0 root         (0) root         (0)       83 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/drmaa/blastdb.sh
--rw-rw-rw-   0 root         (0) root         (0)     1585 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/drmaa/fatotwobit.py
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/drmaa/fatotwobit.sh
--rw-rw-rw-   0 root         (0) root         (0)     1265 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/drmaa/func_annot_bipaa.py
--rwxrwxrwx   0 root         (0) root         (0)      287 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/drmaa/func_annot_bipaa.sh
--rw-rw-rw-   0 root         (0) root         (0)     1873 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/drmaa/func_annot_orson.py
--rwxrwxrwx   0 root         (0) root         (0)     1216 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/drmaa/func_annot_orson.sh
--rw-rw-rw-   0 root         (0) root         (0)     2185 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/drmaa/gffread.py
--rwxrwxrwx   0 root         (0) root         (0)      384 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/drmaa/gffread.sh
--rw-rw-rw-   0 root         (0) root         (0)     3225 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/drmaa/gffread_fa_rename.py
--rw-rw-rw-   0 root         (0) root         (0)     1612 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/drmaa/index_bai.py
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/drmaa/index_bai.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 16:39:48.332764 beauris-0.2/beauris/workflows/galaxy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/galaxy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7918 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/galaxy/genoboo.py
--rw-rw-rw-   0 root         (0) root         (0)    12824 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/galaxy/jbrowse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 16:39:48.336765 beauris-0.2/beauris/workflows/local/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4283 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/apollo_deploy.py
--rw-rw-rw-   0 root         (0) root         (0)     2594 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/apollo_perms.py
--rw-rw-rw-   0 root         (0) root         (0)     1365 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/assembly_check.py
--rw-rw-rw-   0 root         (0) root         (0)     1784 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/build_elasticsearch.py
--rw-rw-rw-   0 root         (0) root         (0)     2117 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/check_yml.py
--rw-rw-rw-   0 root         (0) root         (0)      737 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/deploy_blast.py
--rw-rw-rw-   0 root         (0) root         (0)      908 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/deploy_download.py
--rw-rw-rw-   0 root         (0) root         (0)      991 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/deploy_elasticsearch.py
--rw-rw-rw-   0 root         (0) root         (0)      967 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/deploy_genoboo.py
--rw-rw-rw-   0 root         (0) root         (0)     1057 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/deploy_jbrowse.py
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/deploy_perms.py
--rw-rw-rw-   0 root         (0) root         (0)     3333 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/interface_setup.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/lock.py
--rw-rw-rw-   0 root         (0) root         (0)     4836 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/ogs_check.py
--rw-rw-rw-   0 root         (0) root         (0)     2984 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/prepare_workdir.py
--rw-rw-rw-   0 root         (0) root         (0)     2197 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/run_apollo.py
--rw-rw-rw-   0 root         (0) root         (0)     2653 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/run_apollo_perms.py
--rw-rw-rw-   0 root         (0) root         (0)     3864 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/run_build_elasticsearch.py
--rw-rw-rw-   0 root         (0) root         (0)     1614 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/track_check.py
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/track_check_bam.py
--rw-rw-rw-   0 root         (0) root         (0)      937 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/local/track_check_gff.py
--rw-rw-rw-   0 root         (0) root         (0)      473 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/minimal.bam
--rw-rw-rw-   0 root         (0) root         (0)      880 2023-11-10 16:39:32.000000 beauris-0.2/beauris/workflows/minimal.wg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 16:39:48.322764 beauris-0.2/beauris.egg-info/
--rw-r--r--   0 root         (0) root         (0)      817 2023-11-10 16:39:48.000000 beauris-0.2/beauris.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3687 2023-11-10 16:39:48.000000 beauris-0.2/beauris.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-10 16:39:48.000000 beauris-0.2/beauris.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-11-10 16:39:48.000000 beauris-0.2/beauris.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-11-10 16:39:48.000000 beauris-0.2/beauris.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-10 16:39:48.337765 beauris-0.2/scripts/
--rwxrwxrwx   0 root         (0) root         (0)      549 2023-11-10 16:39:32.000000 beauris-0.2/scripts/beauris_check_env
--rwxrwxrwx   0 root         (0) root         (0)      662 2023-11-10 16:39:32.000000 beauris-0.2/scripts/beauris_commit_lockfiles
--rwxrwxrwx   0 root         (0) root         (0)      303 2023-11-10 16:39:32.000000 beauris-0.2/scripts/beauris_diff_lockfiles
--rwxrwxrwx   0 root         (0) root         (0)      410 2023-11-10 16:39:32.000000 beauris-0.2/scripts/beauris_fetch_locked_artifacts
--rwxrwxrwx   0 root         (0) root         (0)      727 2023-11-10 16:39:32.000000 beauris-0.2/scripts/beauris_run_on_touched_orgs
--rw-rw-rw-   0 root         (0) root         (0)      132 2023-11-10 16:39:48.338765 beauris-0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1236 2023-11-10 16:39:32.000000 beauris-0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:58:47.069631 beauris-0.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2024-04-02 15:58:36.000000 beauris-0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      817 2024-04-02 15:58:47.069631 beauris-0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2024-04-02 15:58:36.000000 beauris-0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:58:47.047632 beauris-0.3/beauris/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-04-02 15:58:36.000000 beauris-0.3/beauris/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6055 2024-04-02 15:58:36.000000 beauris-0.3/beauris/annotation.py
+-rw-rw-rw-   0 root         (0) root         (0)     9677 2024-04-02 15:58:36.000000 beauris-0.3/beauris/assembly.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2024-04-02 15:58:36.000000 beauris-0.3/beauris/beauris.py
+-rw-rw-rw-   0 root         (0) root         (0)     5870 2024-04-02 15:58:36.000000 beauris-0.3/beauris/blastbank.py
+-rw-rw-rw-   0 root         (0) root         (0)     4503 2024-04-02 15:58:36.000000 beauris-0.3/beauris/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     9267 2024-04-02 15:58:36.000000 beauris-0.3/beauris/data_locker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:58:47.050632 beauris-0.3/beauris/deployers/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2024-04-02 15:58:36.000000 beauris-0.3/beauris/deployers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6611 2024-04-02 15:58:36.000000 beauris-0.3/beauris/deployers/authelia.py
+-rw-rw-rw-   0 root         (0) root         (0)     8353 2024-04-02 15:58:36.000000 beauris-0.3/beauris/deployers/basedeployer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2701 2024-04-02 15:58:36.000000 beauris-0.3/beauris/deployers/blast.py
+-rw-rw-rw-   0 root         (0) root         (0)     1445 2024-04-02 15:58:36.000000 beauris-0.3/beauris/deployers/deployers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1144 2024-04-02 15:58:36.000000 beauris-0.3/beauris/deployers/dockercompose.py
+-rw-rw-rw-   0 root         (0) root         (0)     2816 2024-04-02 15:58:36.000000 beauris-0.3/beauris/deployers/download.py
+-rw-rw-rw-   0 root         (0) root         (0)     3161 2024-04-02 15:58:36.000000 beauris-0.3/beauris/deployers/elasticsearch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4608 2024-04-02 15:58:36.000000 beauris-0.3/beauris/deployers/genoboo.py
+-rw-rw-rw-   0 root         (0) root         (0)     3045 2024-04-02 15:58:36.000000 beauris-0.3/beauris/deployers/genomehomepage.py
+-rw-rw-rw-   0 root         (0) root         (0)     6305 2024-04-02 15:58:36.000000 beauris-0.3/beauris/deployers/jbrowse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:58:47.051632 beauris-0.3/beauris/es_parsers/
+-rw-rw-rw-   0 root         (0) root         (0)      216 2024-04-02 15:58:36.000000 beauris-0.3/beauris/es_parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1985 2024-04-02 15:58:36.000000 beauris-0.3/beauris/es_parsers/diamond_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2269 2024-04-02 15:58:36.000000 beauris-0.3/beauris/es_parsers/eggnog_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2228 2024-04-02 15:58:36.000000 beauris-0.3/beauris/es_parsers/gff_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2024-04-02 15:58:36.000000 beauris-0.3/beauris/es_parsers/interpro_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2994 2024-04-02 15:58:36.000000 beauris-0.3/beauris/expression_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2702 2024-04-02 15:58:36.000000 beauris-0.3/beauris/extra_file.py
+-rw-rw-rw-   0 root         (0) root         (0)    20774 2024-04-02 15:58:36.000000 beauris-0.3/beauris/job_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)    13085 2024-04-02 15:58:36.000000 beauris-0.3/beauris/managed_entity.py
+-rw-rw-rw-   0 root         (0) root         (0)    11232 2024-04-02 15:58:36.000000 beauris-0.3/beauris/managed_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2024-04-02 15:58:36.000000 beauris-0.3/beauris/mr_bot.py
+-rw-rw-rw-   0 root         (0) root         (0)    12710 2024-04-02 15:58:36.000000 beauris-0.3/beauris/organism.py
+-rw-rw-rw-   0 root         (0) root         (0)     2566 2024-04-02 15:58:36.000000 beauris-0.3/beauris/proteome.py
+-rw-rw-rw-   0 root         (0) root         (0)    12571 2024-04-02 15:58:36.000000 beauris-0.3/beauris/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:58:47.053632 beauris-0.3/beauris/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-02 15:58:36.000000 beauris-0.3/beauris/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6522 2024-04-02 15:58:36.000000 beauris-0.3/beauris/tasks/annotation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2804 2024-04-02 15:58:36.000000 beauris-0.3/beauris/tasks/assembly.py
+-rw-rw-rw-   0 root         (0) root         (0)     4625 2024-04-02 15:58:36.000000 beauris-0.3/beauris/tasks/organism.py
+-rw-rw-rw-   0 root         (0) root         (0)      817 2024-04-02 15:58:36.000000 beauris-0.3/beauris/tasks/proteome.py
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2024-04-02 15:58:36.000000 beauris-0.3/beauris/tasks/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2024-04-02 15:58:36.000000 beauris-0.3/beauris/tasks/track.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2024-04-02 15:58:36.000000 beauris-0.3/beauris/tasks/transcriptome.py
+-rw-rw-rw-   0 root         (0) root         (0)     3647 2024-04-02 15:58:36.000000 beauris-0.3/beauris/track.py
+-rw-rw-rw-   0 root         (0) root         (0)     2612 2024-04-02 15:58:36.000000 beauris-0.3/beauris/transcriptome.py
+-rw-rw-rw-   0 root         (0) root         (0)     2178 2024-04-02 15:58:36.000000 beauris-0.3/beauris/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:58:47.053632 beauris-0.3/beauris/validation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 15:58:36.000000 beauris-0.3/beauris/validation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:58:47.054632 beauris-0.3/beauris/validation/ogs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 15:58:36.000000 beauris-0.3/beauris/validation/ogs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-04-02 15:58:36.000000 beauris-0.3/beauris/validation/ogs/fasta_check.py
+-rw-rw-rw-   0 root         (0) root         (0)    25071 2024-04-02 15:58:36.000000 beauris-0.3/beauris/validation/ogs/ogs_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:58:47.054632 beauris-0.3/beauris/validation/template/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 15:58:36.000000 beauris-0.3/beauris/validation/template/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2942 2024-04-02 15:58:36.000000 beauris-0.3/beauris/validation/template/ext.py
+-rw-rw-rw-   0 root         (0) root         (0)    11550 2024-04-02 15:58:36.000000 beauris-0.3/beauris/validation/template/schema.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:58:47.055631 beauris-0.3/beauris/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:58:47.041632 beauris-0.3/beauris/workflows/ansible/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:58:47.041632 beauris-0.3/beauris/workflows/ansible/ansible_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:58:47.056631 beauris-0.3/beauris/workflows/ansible/ansible_data/project/
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/ansible/ansible_data/project/playbook_deploy.yml
+-rw-rw-rw-   0 root         (0) root         (0)      276 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/ansible/ansible_data/project/playbook_shutdown.yml
+-rw-rw-rw-   0 root         (0) root         (0)      188 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/ansible/ansible_data/project/playbook_update.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:58:47.056631 beauris-0.3/beauris/workflows/ansible/docker_files/
+-rwxrwxrwx   0 root         (0) root         (0)    12385 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/ansible/docker_files/postgres-blast-entrypoint.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:58:47.057632 beauris-0.3/beauris/workflows/ansible/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/ansible/templates/default.conf.j2
+-rw-rw-rw-   0 root         (0) root         (0)    17405 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/ansible/templates/docker-compose.yml.j2
+-rw-rw-rw-   0 root         (0) root         (0)      914 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/ansible/templates/genoboo.json.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:58:47.057632 beauris-0.3/beauris/workflows/ansible/templates/web/
+-rw-rw-rw-   0 root         (0) root         (0)     1663 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/ansible/templates/web/index.html.j2
+-rw-rw-rw-   0 root         (0) root         (0)     5857 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/ansible/templates/web/search.html.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:58:47.061632 beauris-0.3/beauris/workflows/drmaa/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/drmaa/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2018 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/drmaa/add_fa_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     1222 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/drmaa/add_gff_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     1680 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/drmaa/bam_to_wig.py
+-rwxrwxrwx   0 root         (0) root         (0)      283 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/drmaa/bam_to_wig.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1588 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/drmaa/blastdb.py
+-rwxrwxrwx   0 root         (0) root         (0)       83 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/drmaa/blastdb.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/drmaa/fatotwobit.py
+-rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/drmaa/fatotwobit.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1265 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/drmaa/func_annot_bipaa.py
+-rwxrwxrwx   0 root         (0) root         (0)      287 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/drmaa/func_annot_bipaa.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/drmaa/func_annot_orson.py
+-rwxrwxrwx   0 root         (0) root         (0)     1245 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/drmaa/func_annot_orson.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2185 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/drmaa/gffread.py
+-rwxrwxrwx   0 root         (0) root         (0)      384 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/drmaa/gffread.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3239 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/drmaa/gffread_fa_rename.py
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/drmaa/index_bai.py
+-rwxrwxrwx   0 root         (0) root         (0)       34 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/drmaa/index_bai.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:58:47.061632 beauris-0.3/beauris/workflows/galaxy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/galaxy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9295 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/galaxy/genoboo.py
+-rw-rw-rw-   0 root         (0) root         (0)    14216 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/galaxy/jbrowse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:58:47.067631 beauris-0.3/beauris/workflows/local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6065 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/apollo_deploy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3277 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/apollo_perms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1365 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/assembly_check.py
+-rw-rw-rw-   0 root         (0) root         (0)     1715 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/build_elasticsearch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4304 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/check_yml.py
+-rw-rw-rw-   0 root         (0) root         (0)     3010 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/deploy_all.py
+-rw-rw-rw-   0 root         (0) root         (0)      690 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/deploy_authelia.py
+-rw-rw-rw-   0 root         (0) root         (0)      674 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/deploy_blast.py
+-rw-rw-rw-   0 root         (0) root         (0)      849 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/deploy_download.py
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/deploy_elasticsearch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/deploy_genoboo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1569 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/deploy_jbrowse.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/lock.py
+-rw-rw-rw-   0 root         (0) root         (0)     4933 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/ogs_check.py
+-rw-rw-rw-   0 root         (0) root         (0)     2984 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/prepare_workdir.py
+-rw-rw-rw-   0 root         (0) root         (0)     2197 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/run_apollo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2653 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/run_apollo_perms.py
+-rw-rw-rw-   0 root         (0) root         (0)     4121 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/run_build_elasticsearch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1614 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/track_check.py
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/track_check_bam.py
+-rw-rw-rw-   0 root         (0) root         (0)      937 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/track_check_gff.py
+-rw-rw-rw-   0 root         (0) root         (0)      481 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/local/track_check_vcf.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/minimal.bam
+-rw-rw-rw-   0 root         (0) root         (0)      880 2024-04-02 15:58:36.000000 beauris-0.3/beauris/workflows/minimal.wg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:58:47.068632 beauris-0.3/beauris.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      817 2024-04-02 15:58:47.000000 beauris-0.3/beauris.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4174 2024-04-02 15:58:47.000000 beauris-0.3/beauris.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 15:58:47.000000 beauris-0.3/beauris.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2024-04-02 15:58:47.000000 beauris-0.3/beauris.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-02 15:58:47.000000 beauris-0.3/beauris.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:58:47.068632 beauris-0.3/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)      549 2024-04-02 15:58:36.000000 beauris-0.3/scripts/beauris_check_env
+-rwxrwxrwx   0 root         (0) root         (0)     2903 2024-04-02 15:58:36.000000 beauris-0.3/scripts/beauris_clean_workdir
+-rwxrwxrwx   0 root         (0) root         (0)      662 2024-04-02 15:58:36.000000 beauris-0.3/scripts/beauris_commit_lockfiles
+-rwxrwxrwx   0 root         (0) root         (0)      303 2024-04-02 15:58:36.000000 beauris-0.3/scripts/beauris_diff_lockfiles
+-rwxrwxrwx   0 root         (0) root         (0)      410 2024-04-02 15:58:36.000000 beauris-0.3/scripts/beauris_fetch_locked_artifacts
+-rwxrwxrwx   0 root         (0) root         (0)      729 2024-04-02 15:58:36.000000 beauris-0.3/scripts/beauris_run_on_touched_orgs
+-rw-rw-rw-   0 root         (0) root         (0)      132 2024-04-02 15:58:47.069631 beauris-0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-02 15:58:36.000000 beauris-0.3/setup.py
```

### Comparing `beauris-0.2/LICENSE` & `beauris-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `beauris-0.2/PKG-INFO` & `beauris-0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beauris
-Version: 0.2
+Version: 0.3
 Summary: BEAURIS: an automated system for the creation of genome portals
 Home-page: https://gitlab.com/beaur1s/beauris
 Author: BEAURIS team
 Author-email: gogepp@inrae.fr
 License: MIT
 Platform: Posix
 Classifier: Development Status :: 4 - Beta
```

### Comparing `beauris-0.2/README.md` & `beauris-0.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # BEAURIS
 
  [![pipeline status](https://gitlab.com/beaur1s/beauris/badges/main/pipeline.svg)](https://gitlab.com/beaur1s/beauris/-/commits/main) [![PyPI version](https://badge.fury.io/py/beauris.svg)](https://badge.fury.io/py/beauris) [![Documentation Status](https://readthedocs.org/projects/beauris/badge/?version=latest)](https://beauris.readthedocs.io/en/latest/?badge=latest)
 
 BEAURIS: an automated system for the creation of genome portals
 
-Originally written for genomes hosted by GOGEPP on https://bipaa.genouest.org and https://bbip.genouest.org, as well as ABiMS and SEBIMER.
+Originally written for genomes hosted by [GenOuest](https://www.genouest.org)/GOGEPP on [BIPAA](https://bipaa.genouest.org) and [BBIP](https://bbip.genouest.org), as well as [ABiMS](http://abims.sb-roscoff.fr/) and [SEBIMER](https://bioinfo.ifremer.fr/).
+
+Have a look at the [BEAURIS presentation during JOBIM 2023](https://doi.org/10.5281/zenodo.8279917)
 
 ## Documentation
 
 This repository contains the common code needed to deploy any BEAURIS genome portal. To use it, you will need to create another GitLab repository, following the [provided example](https://gitlab.com/beaur1s/sample).
 
-Check out the [BEAURIS documentation](https://beauris.readthedocs.io/)!
+Check out the [BEAURIS documentation](https://beauris.readthedocs.io/).
 
 ## Authors
 
 BEAURIS was developped initially by:
 
-- GOGEPP/GenOuest (Rennes, France): used on [BIPAA](https://bipaa.genouest.org) and [BBIP](https://bbip.genouest.org)
-- ABiMS (Roscoff, France)
-- SEBIMER (Brest, France)
+- [GenOuest](https://www.genouest.org)/GOGEPP (Rennes, France): used on [BIPAA](https://bipaa.genouest.org) and [BBIP](https://bbip.genouest.org)
+- [ABiMS](http://abims.sb-roscoff.fr/) (Roscoff, France)
+- [SEBIMER](https://bioinfo.ifremer.fr/) (Brest, France)
 
 See [up-to-date contributors list](https://gitlab.com/beaur1s/beauris/-/graphs/main).
```

### Comparing `beauris-0.2/beauris/annotation.py` & `beauris-0.3/beauris/annotation.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,65 +10,80 @@
 log = logging.getLogger()
 
 
 class Annotation(ManagedEntity):
 
     def __init__(self, config, yml_data, assembly):
 
-        ManagedEntity.__init__(self, config, default_services=assembly.deploy_services, yml_data=yml_data)
-
         self.assembly = assembly
 
+        ManagedEntity.__init__(self, config, default_services=assembly.deploy_services, yml_data=yml_data)
+
         self.version = self.yml_data['version']
 
         self.entity_name = 'annotation'
 
+        self.xrefs = {}
+        if 'xrefs' in self.yml_data:
+            self.xrefs = self.yml_data['xrefs']
+
         self.input_files = {
             'gff': InputFile.from_yml(self.yml_data["file"], name='gff', version=self.version)
         }
 
         self.expressions = self._load_expressions()
 
         self.tasks = self.config.get_tasks(self)
 
         self.load_tasks_derived_files()
 
         self.blastbanks = [
-            BlastBank(self, 'blastdb_cds', self.derived_files['cds_fa'], self.derived_files['blastdb_cds_nhr'], "annotation_cds", 'nucl'),
-            BlastBank(self, 'blastdb_transcripts', self.derived_files['transcripts_fa'], self.derived_files['blastdb_transcripts_nhr'], "annotation_transcripts", 'nucl'),
-            BlastBank(self, 'blastdb_proteins', self.derived_files['proteins_fa'], self.derived_files['blastdb_proteins_phr'], "annotation_proteins", 'prot')
+            BlastBank(self, 'blastdb_cds', self.derived_files['cds_fa'], self.derived_files['blastdb_cds_nhr'], "annotation_cds", 'nucl', "blastdb_cds"),
+            BlastBank(self, 'blastdb_transcripts', self.derived_files['transcripts_fa'], self.derived_files['blastdb_transcripts_nhr'], "annotation_transcripts", 'nucl', "blastdb_transcripts"),
+            BlastBank(self, 'blastdb_proteins', self.derived_files['proteins_fa'], self.derived_files['blastdb_proteins_phr'], "annotation_proteins", 'prot', "blastdb_proteins")
         ]
 
-    def get_blast_link(self, bank, server):
-
-        # TODO add a link to GNB when ready
+    def get_blast_link(self, bank, server, restricted=False):
 
         link = '{id}'
 
         if bank.input_fasta.name in ('cds_fa', 'transcripts_fa'):
-            # Annotation tracks are indexed, it should be possible to link to features directly
-            if 'jbrowse' in self.get_deploy_services(server):
-                link = '<a href="' + self.config.get_service_url('jbrowse', server, self.assembly.organism) + '?data=data%2F' + self.assembly.slug(short=True) + '&loc={id}">{id}</a>'
+            if 'genoboo' in self.get_deploy_services(server):
+                link = '<a href="' + self.config.get_service_url('genoboo', server, self.assembly.organism, restricted) + 'gene/{id}?annotation=' + self.version + '">{id}</a>'
+
+                # Annotation tracks are indexed, it should be possible to link to features directly
+                if 'jbrowse' in self.get_deploy_services(server):
+                    link += ' <a href="' + self.config.get_service_url('jbrowse', server, self.assembly.organism, restricted) + '?data=data%2F' + self.assembly.slug(short=True) + '&loc={id}">JBrowse</a>'
+            else:
+                if 'jbrowse' in self.get_deploy_services(server):
+                    link = '<a href="' + self.config.get_service_url('jbrowse', server, self.assembly.organism, restricted) + '?data=data%2F' + self.assembly.slug(short=True) + '&loc={id}">{id}</a>'
 
             if 'apollo' in self.get_deploy_services(server) and 'apollo' in self.config.raw and server in self.config.raw['apollo']:
 
                 common_name = self.assembly.organism.pretty_name()
                 common_name += " {}".format(self.assembly.version)
                 common_name = common_name.replace(' ', '%20')
 
-                link += ' <a href="{}annotator/loadLink?organism='.format(self.config.get_service_url('apollo', server)) + common_name + '&loc={id}">Apollo</a>'
+                link += ' <a href="{}annotator/loadLink?organism='.format(self.config.get_service_url('apollo', server, restricted=restricted)) + common_name + '&loc={id}">Apollo</a>'
+
+        elif bank.input_fasta.name in ('proteins_fa'):
+
+            if 'genoboo' in self.get_deploy_services(server):
+                link = '<a href="' + self.config.get_service_url('genoboo', server, self.assembly.organism, restricted) + 'gene/{id}?annotation=' + self.version + '">{id}</a>'
+
+            # TODO linking to jbrowse/apollo would require to substitue -PA suffixes, or index it in jbrowse
 
         return link
 
     def slug(self, short=False):
 
         if short:
-            return "{}_annot{}".format(self.assembly.slug(short), self.version)
+            return "{}_annot{}".format(self.assembly.slug(short), self.sanitize(self.version))
         else:
-            return "{}/annotation_{}".format(self.assembly.slug(short), self.version)
+            return "{}/annotation_{}".format(self.assembly.slug(short), self.sanitize(self.version))
 
     def pretty_name(self, with_parent=True):
 
         if with_parent:
             return "{} annotation {}".format(self.assembly.pretty_name(), self.version)
         else:
             return "Annotation {}".format(self.version)
@@ -77,17 +92,21 @@
 
         return self.expressions
 
     def get_organism(self):
 
         return self.assembly.organism
 
+    def get_parent(self):
+
+        return self.assembly
+
     def get_work_dir(self):
 
-        return os.path.join(self.assembly.get_work_dir(), "annotation_{}".format(self.version))
+        return os.path.join(self.assembly.get_work_dir(), "annotation_{}".format(self.sanitize(self.version)))
 
     def get_locked_yml(self):
 
         locked_yml = self.yml_data
 
         locked_yml['file'] = self.input_files['gff'].to_yml()
 
@@ -130,7 +149,17 @@
 
     def _load_expressions(self):
         expressions = []
         for exp in self.yml_data.get("expression_data", []):
             expressions.append(ExpressionData(self.config, exp, self))
 
         return expressions
+
+    def purge_restricted_data(self):
+
+        kept_exp = []
+        for exp in self.expressions:
+            if exp.restricted_to is None:
+                exp.purge_restricted_data()
+                kept_exp.append(exp)
+
+        self.expressions = kept_exp
```

### Comparing `beauris-0.2/beauris/assembly.py` & `beauris-0.3/beauris/assembly.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,75 +1,87 @@
 import logging
 import os
 
 from .annotation import Annotation
 from .blastbank import BlastBank
+from .extra_file import ExtraFile
 from .managed_entity import ManagedEntity
 from .managed_file import InputFile
 from .track import Track
 
 
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger()
 
 
 class Assembly(ManagedEntity):
 
     def __init__(self, config, yml_data, organism):
 
-        ManagedEntity.__init__(self, config, default_services=organism.deploy_services, yml_data=yml_data)
-
         self.organism = organism
 
+        ManagedEntity.__init__(self, config, default_services=organism.deploy_services, yml_data=yml_data)
+
         self.version = self.yml_data['version']
 
+        self.xrefs = {}
+        if 'xrefs' in self.yml_data:
+            self.xrefs = self.yml_data['xrefs']
+
         self.entity_name = 'assembly'
 
         # TODO this should be configurable somehow
         self.wig_category_suffix = " Coverage"
 
+        self.restricted_to_apollo = self.yml_data.get('restricted_to_apollo', None)
+
         self.input_files = {
             'fasta': InputFile.from_yml(self.yml_data["file"], name='fasta', version=self.version)
         }
 
         self.annotations = self._load_annotations()
         self.tracks = self._load_tracks()
+        self.extra_files = self._load_extra_files()
 
         self.tasks = self.config.get_tasks(self)
 
         self.load_tasks_derived_files()
 
         self.blastbanks = [
-            BlastBank(self, 'blastdb_assembly', self.input_files['fasta'], self.derived_files['blastdb_nhr'], "assembly", 'nucl')
+            BlastBank(self, 'blastdb_assembly', self.input_files['fasta'], self.derived_files['blastdb_nhr'], "assembly", 'nucl', "blastdb")
         ]
 
-    def get_blast_link(self, bank, server):
+    def get_blast_link(self, bank, server, restricted=False):
 
         link = '{id}'
         if 'jbrowse' in self.get_deploy_services(server):
-            link = '<a href="' + self.config.get_service_url('jbrowse', server, self.organism) + '?data=data%2F' + self.slug(short=True) + '&loc={id}{jbrowse_track}">{id}</a>'
+            link = '<a href="' + self.config.get_service_url('jbrowse', server, self.organism, restricted) + '?data=data%2F' + self.slug(short=True) + '&loc={id}{jbrowse_track}">{id}</a>'
 
         if 'apollo' in self.get_deploy_services(server) and 'apollo' in self.config.raw and server in self.config.raw['apollo']:
 
             common_name = self.organism.pretty_name()
             common_name += " {}".format(self.version)
             common_name = common_name.replace(' ', '%20')
 
-            link += ' <a href="{}annotator/loadLink?organism='.format(self.config.get_service_url('apollo', server)) + common_name + '&loc={id}{apollo_track}">Apollo</a>'
+            link += ' <a href="{}annotator/loadLink?organism='.format(self.config.get_service_url('apollo', server, restricted=restricted)) + common_name + '&loc={id}{apollo_track}">Apollo</a>'
 
         return link
 
     def get_children(self):
 
-        return self.annotations + self.tracks
+        return self.annotations + self.tracks + self.extra_files
 
     def get_organism(self):
 
         return self.organism
 
+    def get_parent(self):
+
+        return self.organism
+
     def get_annotation(self, version):
 
         for annot in self.annotations:
             if annot.version == version:
                 return annot
 
         return None
@@ -81,17 +93,17 @@
                 return tr
 
         return None
 
     def slug(self, short=False):
 
         if short:
-            return "{}_ass{}".format(self.organism.slug(short), self.version)
+            return "{}_ass{}".format(self.organism.slug(short), self.sanitize(self.version))
         else:
-            return "{}/assembly_{}".format(self.organism.slug(short), self.version)
+            return "{}/assembly_{}".format(self.organism.slug(short), self.sanitize(self.version))
 
     def pretty_name(self, with_parent=True):
 
         if with_parent:
             return "{} assembly {}".format(self.organism.pretty_name(), self.version)
         else:
             return "Assembly {}".format(self.version)
@@ -106,17 +118,24 @@
     def _load_tracks(self):
         tracks = []
         for track in self.yml_data.get("tracks", []):
             tracks.append(Track(self.config, track, self))
 
         return tracks
 
+    def _load_extra_files(self):
+        extra_files = []
+        for xtra in self.yml_data.get("extra_files", []):
+            extra_files.append(ExtraFile(self.config, xtra, self))
+
+        return extra_files
+
     def get_work_dir(self):
 
-        return os.path.join(self.organism.get_work_dir(), "assembly_{}".format(self.version))
+        return os.path.join(self.organism.get_work_dir(), "assembly_{}".format(self.sanitize(self.version)))
 
     def get_locked_yml(self):
 
         locked_yml = self.yml_data
 
         locked_yml['file'] = self.input_files['fasta'].to_yml()
 
@@ -134,14 +153,20 @@
 
         if self.tracks:
             locked_yml['tracks'] = []
 
             for track in self.tracks:
                 locked_yml['tracks'].append(track.get_locked_yml())
 
+        if self.extra_files:
+            locked_yml['extra_files'] = []
+
+            for xtra in self.extra_files:
+                locked_yml['extra_files'].append(xtra.get_locked_yml())
+
         return locked_yml
 
     def get_metadata(self, inherit=True):
 
         metadata = {'assembly_version': self.version}
 
         if inherit:
@@ -164,38 +189,79 @@
                 annot.load_locked_data(matching, future)
 
         for track in self.tracks:
             matching = track.find_matching_yml_in_list(locked_yml.get("tracks", []))
             if matching:
                 track.load_locked_data(matching, future)
 
+        for xtra in self.extra_files:
+            matching = xtra.find_matching_yml_in_list(locked_yml.get("extra_files", []))
+            if matching:
+                xtra.load_locked_data(matching, future)
+
     def get_track_paths(self, prefer=None):
 
         tracks_paths = {}
 
         if prefer == 'locked':
             tracks_paths['gff'] = {(t.category, t.name): t.input_files['track_file'].get_locked_path() for t in self.tracks if t.type == "gff"}
             tracks_paths['bam'] = {(t.category, t.name): t.input_files['track_file'].get_locked_path() for t in self.tracks if t.type in ("rnaseq", "dnaseq")}
             tracks_paths['bai'] = {(t.category, t.name): t.derived_files['bai'].get_locked_path() for t in self.tracks if 'bai' in t.derived_files}
             tracks_paths['wig'] = {(t.category + self.wig_category_suffix, t.name): t.derived_files['wig'].get_locked_path() for t in self.tracks if 'wig' in t.derived_files}
+            tracks_paths['vcf'] = {(t.category, t.name): t.input_files['track_file'].get_locked_path() for t in self.tracks if t.type == "vcf"}
         else:
             force_work_dir = prefer == 'workdir'
 
             tracks_paths['gff'] = {(t.category, t.name): t.get_input_path('track_file') for t in self.tracks if t.type == "gff"}
             tracks_paths['bam'] = {(t.category, t.name): t.get_input_path('track_file') for t in self.tracks if t.type in ("rnaseq", "dnaseq")}
             tracks_paths['bai'] = {(t.category, t.name): t.derived_files['bai'].get_usable_path(force_work_dir=force_work_dir or t.derived_files['bai'].task.needs_to_run()) for t in self.tracks if 'bai' in t.derived_files}
             tracks_paths['wig'] = {(t.category + self.wig_category_suffix, t.name): t.derived_files['wig'].get_usable_path(force_work_dir=force_work_dir or t.derived_files['wig'].task.needs_to_run()) for t in self.tracks if 'wig' in t.derived_files}
-
+            tracks_paths['vcf'] = {(t.category, t.name): t.get_input_path('track_file') for t in self.tracks if t.type == "vcf"}
         return tracks_paths
 
     def jbrowse_track_swapping(self, json_tracks, tracks_real_path):
 
         to_swap = {}
 
         for jt in json_tracks:
             if 'storeClass' in jt and jt['storeClass'] == "JBrowse/Store/SeqFeature/BAM" and 'urlTemplate' in jt and (jt['category'], jt['key']) in tracks_real_path['bam']:
                 to_swap[jt['urlTemplate']] = tracks_real_path['bam'][(jt['category'], jt['key'])]
                 to_swap[jt['urlTemplate'] + ".bai"] = tracks_real_path['bai'][(jt['category'], jt['key'])]
             elif 'storeClass' in jt and jt['storeClass'] == "JBrowse/Store/SeqFeature/BigWig" and 'urlTemplate' in jt and (jt['category'], jt['key']) in tracks_real_path['wig']:
                 to_swap[jt['urlTemplate']] = tracks_real_path['wig'][(jt['category'], jt['key'])]
 
         return to_swap
+
+    def purge_restricted_data(self):
+
+        kept_ann = []
+        for ann in self.annotations:
+            if ann.restricted_to is None:
+                ann.purge_restricted_data()
+                kept_ann.append(ann)
+
+        self.annotations = kept_ann
+
+        kept_tra = []
+        for tra in self.tracks:
+            if tra.restricted_to is None:
+                tra.purge_restricted_data()
+                kept_tra.append(tra)
+
+        self.tracks = kept_tra
+
+        kept_xtra = []
+        for xtra in self.extra_files:
+            if xtra.restricted_to is None:
+                xtra.purge_restricted_data()
+                kept_tra.append(xtra)
+
+        self.extra_files = kept_xtra
+
+    def get_restricted_to_map(self, locked=False):
+
+        rtos = ManagedEntity.get_restricted_to_map(self, locked)
+
+        if self.restricted_to_apollo:
+            rtos[self.slug() + "__apollo__"] = self.restricted_to_apollo
+
+        return rtos
```

### Comparing `beauris-0.2/beauris/beauris.py` & `beauris-0.3/beauris/beauris.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
 
 from .config import Config
 from .data_locker import DataLockers
+from .deployers import Deployers
 from .job_runner import Runners
 from .organism import Organism
+from .util import Util
 
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger()
 
 
 class Beauris():
 
@@ -15,25 +17,37 @@
 
         self.config = Config(root_work_dir, config_file)
 
         self.runners = Runners(self.config.job_specs)
 
         self.data_lockers = DataLockers()
 
+        self.deployers = Deployers(self.config)
+
+        labels = Util.mr_labels
+
+        if 'logging-debug' in labels:
+            # Override root logger
+            logging.basicConfig(level=logging.DEBUG, force=True)
+
     def load_organism(self, yml_path, test_data=False, locked_dir=None, future_locked_dir=None):
 
         return Organism(self.config, yml_path, test_data=test_data, locked_dir=locked_dir, future_locked_dir=future_locked_dir, default_services=self.config.deploy_services)
 
-    def get_runner(self, method, entity, task_id, server=""):
+    def get_runner(self, method, entity, task_id, workdir="", server="", access_mode="public"):
 
-        return self.runners.get(method, entity, task_id, server)
+        return self.runners.get(method, entity, task_id, workdir, server, access_mode)
 
     def get_data_locker(self, override_conf={}):
 
         method = self.config.raw['data_locker']['method']
 
         locker_conf = self.config.raw['data_locker']['options']
 
         # This is used mainly for tests
         locker_conf.update(override_conf)
 
         return self.data_lockers.get(method, locker_conf)
+
+    def get_deployer(self, service, server, entity):
+
+        return self.deployers.get(service, server, entity)
```

### Comparing `beauris-0.2/beauris/blastbank.py` & `beauris-0.3/beauris/blastbank.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 #!/usr/bin/env python
 
 import collections
 import json
 import logging
 import os
+import tempfile
 
 
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger()
 
 
 class BlastBank:
 
-    def __init__(self, entity, task_id, input_fasta, dest, fasta_type, seq_type):
+    def __init__(self, entity, task_id, input_fasta, dest, fasta_type, seq_type, base_task_id="blastdb"):
 
         self.entity = entity
         self.task_id = task_id
         self.input_fasta = input_fasta  # An InputFile object
         self.dest = dest  # A DerivedFile object
         self.seq_type = seq_type
+        self.base_task_id = base_task_id
 
         self.title = entity.slug(short=True)
 
         self.pretty_name = entity.pretty_name()
 
         if fasta_type.startswith("annotation"):
 
@@ -36,55 +38,81 @@
             self.title += "_{}".format(annot_type)
             self.pretty_name += " {}".format(annot_type)
 
         # Just a stupid/hacky string used for sorting bank list
         self.sort_key = 'a_' if fasta_type == "genome" else 'b_'
         self.sort_key += self.pretty_name
 
-    def get_blast_link(self, server):
+    def get_blast_link(self, server, restricted=False):
 
-        return self.entity.get_blast_link(self, server)
+        return self.entity.get_blast_link(self, server, restricted)
 
     def get_input_fasta_path(self):
         # Resolve it as late as possible to make sure it takes into account locked path
 
         return self.input_fasta.get_usable_path(force_work_dir=self.input_fasta.needs_to_run())
 
     def get_dest_path(self):
         # Resolve it as late as possible to make sure it takes into account locked path
 
         return os.path.splitext(self.dest.get_usable_path(force_work_dir=self.dest.needs_to_run()))[0]
 
+    def get_link_path(self, files_path):
+
+        exts = ['phr', 'pin', 'pog', 'psd', 'psi', 'psq'] if self.seq_type == 'prot' else ['nhr', 'nin', 'nog', 'nsd', 'nsi', 'nsq']
+        os.makedirs(os.path.join(files_path, self.title), exist_ok=True)
+
+        for ext in exts:
+            task_id = "{}_{}".format(self.base_task_id, ext)
+            linked_file = self.entity.derived_files[task_id]
+            linked_file_path = linked_file.get_usable_path(force_work_dir=linked_file.needs_to_run())
+
+            dest_file = os.path.join(files_path, self.title, os.path.basename(linked_file_path))
+
+            if os.path.islink(dest_file):
+                if not os.readlink(dest_file) == linked_file:
+                    # Update link
+                    temp_link_name = tempfile.mktemp(dir=files_path)
+                    os.symlink(linked_file_path, temp_link_name)
+                    os.replace(temp_link_name, dest_file)
+            else:
+                os.symlink(linked_file_path, dest_file)
+
+        return os.path.splitext(dest_file)[0]
+
 
 class BankWriter:
 
-    def __init__(self, banks, base_path, server):
+    def __init__(self, banks, base_path, files_path, server, restricted=False):
 
         self.banks = banks
         self.base_path = base_path
+        self.files_path = files_path
         self.server = server
+        self.restricted = restricted
 
         self.nuc_list = collections.OrderedDict()
         self.prot_list = collections.OrderedDict()
         self.banks.sort(key=lambda x: x.sort_key)
         for b in self.banks:
             pretty_name = b.pretty_name
             tries = 1
             if b.seq_type == 'nucl':
                 while pretty_name in self.nuc_list.values() and tries < 50:
                     pretty_name = "{} ({})".format(b.pretty_name, tries)
-                self.nuc_list[b.get_dest_path()] = pretty_name
+                self.nuc_list[b.get_link_path(self.files_path)] = pretty_name
             else:
                 while pretty_name in self.prot_list.values() and tries < 50:
                     pretty_name = "{} ({})".format(b.pretty_name, tries)
-                self.prot_list[b.get_dest_path()] = pretty_name
+                self.prot_list[b.get_link_path(self.files_path)] = pretty_name
 
     def write_bank_yml(self):
         # Safety check
         os.makedirs(self.base_path, exist_ok=True)
+        os.makedirs(self.files_path, exist_ok=True)
 
         banks_file_path = os.path.join(self.base_path, 'banks.yml')
         log.info("Writing bank list in '%s'" % banks_file_path)
         nuc = "~"
         prot = "~"
 
         if self.nuc_list:
@@ -110,15 +138,15 @@
 
         with open(links_file_path, "w") as f:
 
             for bank in self.banks:
                 print("", file=f)
                 print("# %s" % (bank.pretty_name), file=f)
 
-                link = bank.get_blast_link(self.server)
+                link = bank.get_blast_link(self.server, self.restricted)
 
                 if link:
                     print("%s:" % (bank.title), file=f)
                     print("    db: '^%s$'" % (bank.title), file=f)
                     print("    '*': '%s'" % (link), file=f)
                 else:
                     print("# Skipped", file=f)
@@ -127,15 +155,7 @@
 def prettify(name, capital=True):
 
     # A bit of magic to make even prettier names
     name = name.replace(" annot ogs", " ogs")
     name = name.replace("ogs", "OGS")
 
     return name
-
-
-def sanitize(name):
-    name = name.lower()
-    name = name.replace(' ', '_')
-    name = name.replace('/', '_')
-
-    return name
```

### Comparing `beauris-0.2/beauris/config.py` & `beauris-0.3/beauris/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,18 @@
 
         self.job_specs = self.raw['job_specs'] if 'job_specs' in self.raw else {}
 
         self.deploy = {}
         if 'deploy' in self.raw and 'servers' in self.raw['deploy']:
             self.deploy = self.raw['deploy']['servers']
 
+        for dep in self.deploy:
+            if 'options' not in self.deploy[dep]:
+                self.deploy[dep]['options'] = {}
+
         self.deploy_services = {server: self.get_deploy_services(server) for server in self.get_deploy_servers()}
 
         self.tasks_by_entity = {}
         if 'tasks' in self.raw:
             for ent in self.raw['tasks']:
                 if not self.known_tasks.has(ent):
                     raise RuntimeError("Unknown entity type in tasks configuration: {}".format(ent))
@@ -99,26 +103,38 @@
                 new_task = tc(entity, tid, **params)
 
                 if entity.accept_task(new_task):
                     taskso[tid] = new_task
 
         return taskso
 
-    def get_service_url(self, service, server, organism=None):
+    def get_service_url(self, service, server, organism=None, restricted=False):
 
         url = ''
+        restricted_suffix = ""
+        if restricted:
+            restricted_suffix = "_restricted"
+
+        aliases = {
+            'genoboo': 'gnb'
+        }
+
+        if service in aliases:
+            # Sometimes we want the url to be shorter than the full service name
+            # FIXME make this configurable
+            service = aliases[service]
 
         if service == 'apollo':
             url = self.raw['apollo'][server]["external_url"]
         else:
             if organism is None:
                 raise RuntimeError("The 'organism' param is mandatory to get the url of service '{}'".format(service))
 
-            base_url = self.deploy[server]["base_url"].rstrip("/")
-            url_prefix = self.deploy[server]["url_prefix"].rstrip("/")
+            base_url = self.deploy[server]["base_url" + restricted_suffix].rstrip("/")
+            url_prefix = self.deploy[server]["url_prefix" + restricted_suffix].rstrip("/")
 
             url = '{}{}/{}/{}/'.format(base_url, url_prefix, organism.slug(), service)
 
         if not url.endswith('/'):
             url += '/'
 
         return url
```

### Comparing `beauris-0.2/beauris/data_locker.py` & `beauris-0.3/beauris/data_locker.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,14 +112,26 @@
 
         if 'annotation_version' in metadata:
             pattern += "{annotation_version}/"
 
         if 'track_id' in metadata:
             pattern += "{track_id}/"
 
+        if 'expression_data_id' in metadata:
+            pattern += "{expression_data_id}/"
+
+        if 'extra_file_id' in metadata:
+            pattern += "{extra_file_id}/"
+
+        if 'proteome_version' in metadata:
+            pattern += "{proteome_version}/"
+
+        if 'transcriptome_version' in metadata:
+            pattern += "{transcriptome_version}/"
+
         if 'tool_version' in metadata:  # TODO find something less hacky
             pattern += self.pattern_derived
         else:
             pattern += self.pattern_input
 
         pattern_replaced = pattern.format_map(metadata)
```

### Comparing `beauris-0.2/beauris/es_parsers/diamond_parser.py` & `beauris-0.3/beauris/es_parsers/diamond_parser.py`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/es_parsers/eggnog_parser.py` & `beauris-0.3/beauris/es_parsers/eggnog_parser.py`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/es_parsers/gff_parser.py` & `beauris-0.3/beauris/es_parsers/gff_parser.py`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/es_parsers/interpro_parser.py` & `beauris-0.3/beauris/es_parsers/interpro_parser.py`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/expression_data.py` & `beauris-0.3/beauris/expression_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,19 +10,22 @@
 log = logging.getLogger()
 
 
 class ExpressionData(ManagedEntity):
 
     def __init__(self, config, yml_data, annotation):
 
-        ManagedEntity.__init__(self, config, default_services=annotation.deploy_services, yml_data=yml_data)
-
         self.annotation = annotation
 
+        ManagedEntity.__init__(self, config, default_services=annotation.deploy_services, yml_data=yml_data)
+
         self.name = self.yml_data['name']
+        self.unit = self.yml_data['unit'] if 'unit' in self.yml_data else 'TPM'
+        self.replicates = self.yml_data['replicates'] if 'replicates' in self.yml_data else []
+
         self.safe_name = re.sub(r'[^a-zA-Z0-9-]', '_', self.name)
 
         self.version = "0"  # No version for this kind of data
 
         self.entity_name = 'expression_data'
 
         self.input_files = {
@@ -37,31 +40,35 @@
 
         return []
 
     def get_organism(self):
 
         return self.annotation.get_organism()
 
+    def get_parent(self):
+
+        return self.annotation
+
     def slug(self, short=False):
 
         if short:
-            return "{}_exp{}".format(self.annotation.slug(short), self.safe_name)
+            return "{}_exp{}".format(self.annotation.slug(short), self.sanitize(self.safe_name))
         else:
-            return "{}/expression_{}".format(self.annotation.slug(short), self.safe_name)
+            return "{}/expression_{}".format(self.annotation.slug(short), self.sanitize(self.safe_name))
 
     def pretty_name(self, with_parent=True):
 
         if with_parent:
             return "{} expression data {}".format(self.annotation.pretty_name(), self.name)
         else:
             return "Expression data {}".format(self.name)
 
     def get_work_dir(self):
 
-        return os.path.join(self.annotation.get_work_dir(), "expression_{}".format(self.safe_name))
+        return os.path.join(self.annotation.get_work_dir(), "expression_{}".format(self.sanitize(self.safe_name)))
 
     def get_locked_yml(self):
 
         locked_yml = self.yml_data
 
         locked_yml['table'] = self.input_files['table'].to_yml()
 
@@ -71,15 +78,15 @@
             for id, der in self.derived_files.items():
                 locked_yml['derived'].append(der.to_yml())
 
         return locked_yml
 
     def get_metadata(self, inherit=True):
 
-        metadata = {'expression_data_id': '{}_{}'.format(self.safe_name, self.version)}
+        metadata = {'expression_data_id': self.safe_name}
 
         if inherit:
             metadata.update(self.annotation.get_metadata())
 
         metadata.update(self.get_basic_metadata())
 
         return metadata
```

### Comparing `beauris-0.2/beauris/job_runner.py` & `beauris-0.3/beauris/job_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,32 +36,41 @@
             'drmaa': DrmaaRunner,
             'galaxy': GalaxyRunner,
             'nextflow': NextflowRunner,
         }
 
         self.job_specs = job_specs
 
-    def get(self, name, entity, task_id, server=""):
+    def get(self, name, entity, task_id, workdir="", server="", access_mode="public"):
 
         if name in self.runners:
-            return self.runners[name](self.job_specs, entity, task_id, server)
+            return self.runners[name](self.job_specs, entity, task_id, workdir, server, access_mode)
 
         raise RuntimeError('Could not find runner named "%s"' % name)
 
 
 class Runner():
 
-    def __init__(self, job_specs, entity, task_id, server=""):
+    def __init__(self, job_specs, entity, task_id, workdir="", server="", access_mode="public"):
 
         self.task = entity.tasks[task_id]
 
         self.job_specs = job_specs
 
         self.name = None
 
+        self.server = server
+
+        self.access_mode = access_mode
+
+        if workdir:
+            self.task.set_workdir(workdir)
+        self.task.set_server(self.server)
+        self.task.set_access_mode(self.access_mode)
+
     def get_job_specs(self, task_id):
 
         return self.job_specs[self.name][task_id] if self.name in self.job_specs and task_id in self.job_specs[self.name] else {}
 
     def run_or_resume_job(self, check_output=True, since='last_lock', **kwargs):
 
         if self.task.disable_run():
@@ -98,14 +107,16 @@
         """
 
         # We run a job, get rid of any trace left by a previous run
         self.task.clear_exit_code()
         self.task.clear_previous_logs()
         self.task.clear_jobid()
 
+        os.makedirs(self.task.get_work_dir(), exist_ok=True)
+
         # Save the current state of input data
         self.task.save_data_state()
 
         # We're really running something
         self.task.has_run = True
 
         # Subclasses are supposed to run their code here now
@@ -134,16 +145,16 @@
                     show_logs(last_out, last_err)
 
         return last_exit_code, last_out, last_err, has_already_run
 
 
 class LocalRunner(Runner):
 
-    def __init__(self, job_specs, entity, task_id, server=""):
-        Runner.__init__(self, job_specs, entity, task_id, server)
+    def __init__(self, job_specs, entity, task_id, workdir="", server="", access_mode="public"):
+        Runner.__init__(self, job_specs, entity, task_id, workdir, server, access_mode)
 
         self.name = 'local'
 
     def run_job(self, cmd=None, **kwargs):
 
         if cmd is None:
             raise RuntimeError("Cannot run job, param cmd is empty")
@@ -162,16 +173,16 @@
         self.task.save_logs(output, err)
 
         return retcode, output, err
 
 
 class AsyncRunner(Runner):
 
-    def __init__(self, job_specs, entity, task_id, server=""):
-        Runner.__init__(self, job_specs, entity, task_id, server)
+    def __init__(self, job_specs, entity, task_id, workdir="", server="", access_mode="public"):
+        Runner.__init__(self, job_specs, entity, task_id, workdir, server, access_mode)
 
     def check_previous_run(self, dest_rename={}, **kwargs):
 
         last_exit_code = self.task.get_previous_exit_code()
 
         last_out, last_err = self.task.get_previous_logs()
 
@@ -267,20 +278,20 @@
 
         # Only needed when results need to be downloaded
         pass
 
 
 class DrmaaRunner(AsyncRunner):
 
-    def __init__(self, job_specs, entity, task_id, server=""):
+    def __init__(self, job_specs, entity, task_id, server="", workdir="", access_mode="public"):
 
         if not drmaa_available:
             raise RuntimeError("Could not load drmaa python module, you can't use the DRMAA runner")
 
-        Runner.__init__(self, job_specs, entity, task_id, server)
+        Runner.__init__(self, job_specs, entity, task_id, workdir, server, access_mode)
 
         self.name = 'drmaa'
 
     def run_job(self, script_path=None, job_args=[], additional_script=[], **kwargs):
 
         if script_path is None:
             raise RuntimeError("Cannot run job, param script_path is empty")
@@ -426,17 +437,17 @@
                     stderr = fh_log.read()
 
         return stdout, stderr
 
 
 class GalaxyRunner(AsyncRunner):
 
-    def __init__(self, job_specs, entity, task_id, server=""):
+    def __init__(self, job_specs, entity, task_id, workdir="", server="", access_mode="public"):
 
-        Runner.__init__(self, job_specs, entity, task_id, server)
+        Runner.__init__(self, job_specs, entity, task_id, workdir, server, access_mode)
 
         self.name = 'galaxy'
 
         self.final_states = ['ok', 'error', 'failed', 'deleted']
 
         self.history_id = None
 
@@ -462,14 +473,16 @@
         log.info("Using params: {}".format(params))
 
         # Not storing history id, 1 history per execution (=runner instance lifetime)
         history_id = self.get_history(history_name)
 
         params = self.upload_files(history_name, uploads, params)
 
+        log.info("Using params after dataset upload: {}".format(params))
+
         tool_invocation = self.gi.tools.run_tool(history_id, tool_id, params)
 
         job_id = tool_invocation['jobs'][0]['id']
 
         log.info('Your job has been submitted with ID %s' % job_id)
         self.task.save_jobid(job_id)
 
@@ -512,35 +525,38 @@
         return tools[-1]['id']
 
     def upload_files(self, history_name, uploads, params):
 
         params_str = json.dumps(params)
 
         for id, infos in uploads.items():
-            upload_id = self.upload_file(history_name, infos['path'], file_name=infos['name'], file_type=infos['type'])
+            upload_id = self.upload_file(history_name, infos['path'], file_name=infos['name'], file_type=infos['type'], auto_decompress=infos.get('auto_decompress', False))
 
             params_str = params_str.replace("##UPLOADED_DATASET_ID__{}##".format(id), upload_id)
 
         return json.loads(params_str)
 
-    def upload_file(self, history_name, dataset, file_name=None, file_type=None):
+    def upload_file(self, history_name, dataset, file_name=None, file_type=None, auto_decompress=False):
 
         history_id = self.get_history(history_name)
 
         args = {
             'path': dataset,
             'history_id': history_id,
         }
 
         if file_name:
             args['file_name'] = file_name
 
         if file_type:
             args['file_type'] = file_type
 
+        if auto_decompress:
+            args['auto_decompress'] = auto_decompress
+
         dataset = self.gi.tools.upload_file(**args)
 
         return dataset['outputs'][0]['id']
 
     def wait_for_job(self, jobid, timeout=None):
 
         first_try = True
@@ -549,15 +565,15 @@
             # Default timeout
             timeout = 3600
 
         while first_try or retry:
             log.info('Waiting for job with ID %s' % jobid)
 
             try:
-                self.gi.jobs.wait_for_job(jobid, interval=30, check=False)
+                self.gi.jobs.wait_for_job(jobid, interval=30, check=False, maxwait=24000)
                 retry = False
             except TimeoutException:
                 if not retry:
                     raise
 
             first_try = False
 
@@ -609,23 +625,30 @@
 
     def delete_history(self, jobid):
 
         job_infos = self.gi.jobs.show_job(jobid)
 
         hid = job_infos['history_id']
 
+        hstate = self.gi.histories.show_history(hid)
+
+        if 'deleted' in hstate and hstate['deleted']:
+            log.debug(f'History {hid} is already deleted')
+            return
+
         self.gi.histories.delete_history(hid, purge=True)
 
 
 class NextflowRunner(AsyncRunner):
+    # Not used currently, and probably not useful (see Orson example, that uses drmaa)
 
-    def __init__(self, job_specs, entity, task_id, server=""):
+    def __init__(self, job_specs, entity, task_id, workdir="", server="", access_mode="public"):
 
-        Runner.__init__(self, job_specs, entity, task_id, server)
+        Runner.__init__(self, job_specs, entity, task_id, workdir, server, access_mode)
 
-        self.name = 'netxflow'
+        self.name = 'nextflow'
 
     def run_job(self, **kwargs):
 
         Runner.run_job(self)
 
         raise NotImplementedError()
```

### Comparing `beauris-0.2/beauris/managed_entity.py` & `beauris-0.3/beauris/managed_entity.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import logging
 import os
+import re
+from copy import deepcopy
 
 import yaml
 
 from .managed_file import DerivedFile
 
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger()
@@ -36,34 +38,48 @@
                 self.locked_yml_path = os.path.join(self.config.raw['data_locker']['options']['locked_yml_dir'], os.path.basename(self.yml_path))
 
             if future_locked_dir:
                 self.future_locked_yml_path = os.path.join(future_locked_dir, os.path.basename(self.yml_path))
             else:
                 self.future_locked_yml_path = os.path.join(self.config.raw['data_locker']['options']['locked_yml_dir_future'], os.path.basename(self.yml_path))
 
+        self.restricted_to_not_inherited = self.yml_data.get('restricted_to', None)
+        if self.get_parent():
+            self.restricted_to = self.yml_data.get('restricted_to', self.get_parent().restricted_to)
+        else:
+            self.restricted_to = self.yml_data.get('restricted_to', None)
+
+        self.locked_restricted_to = None
+
         # Dict of tasks that can be used to generate derived files
         self.tasks = {}
 
         # List of input reference files
         self.input_files = {}
 
         # List of output files generated by tasks (key=task name, value=list of file names relative to task work_dir)
         self.derived_files = {}
 
         # Dict of dict, key = task_id, value = dict of options to be passed to a task
         self.task_options = self.load_task_options(self.yml_data)
 
         # Dict of list of services (by server) that should be deployed for this entity
-        self.deploy_services = default_services
+        self.deploy_services = deepcopy(default_services)
 
         self.parse_services(self.yml_data)
 
         # A list of BlastBank objects
         self.blastbanks = []
 
+    def sanitize(self, name):
+
+        name = re.sub('[^0-9a-zA-Z_.-]+', '_', name)
+
+        return name
+
     def parse_services(self, yml_data):
 
         if 'services' in yml_data:
             for server in self.deploy_services:
                 if server in yml_data['services']:
                     # Force authelia if any services might requires it
                     require_authelia = 'authelia' in self.deploy_services[server]
@@ -103,14 +119,18 @@
 
     def get_derived_path(self, file_id):
 
         tmp_task = self.derived_files[file_id].task
 
         return self.derived_files[file_id].get_usable_path(force_work_dir=tmp_task.needs_to_run())
 
+    def get_parent(self):
+
+        return None
+
     def get_children(self):
 
         return []
 
     def get_organism(self):
 
         return None
@@ -121,14 +141,16 @@
 
         if 'derived' in locked_yml:
             by_name = {x['name']: x for x in locked_yml['derived']}
             for did, derived in self.derived_files.items():
                 if did in by_name:
                     derived.merge_with_locked(by_name[did], future)
 
+        self.locked_restricted_to = locked_yml.get("restricted_to", "")
+
         # Can't load input files here as their identifier is not the same in beauris and in the yml file
         # TODO maybe harmonize naming of input files between beauris and yml file?
 
     def save_locked_yml(self):
 
         dest = self.locked_yml_path
 
@@ -151,14 +173,15 @@
     def get_basic_metadata(self):
 
         meta = {}
         searched = [
             'description',
             'source',
             'date',
+            'restricted_to',
         ]
 
         for s in searched:
             if s in self.yml_data:
                 meta[s] = str(self.yml_data[s])
 
         return meta
@@ -242,34 +265,58 @@
         for child in self.get_children():
             files += child.get_files_to_publish()
 
         return files
 
     def get_deploy_services(self, server):
 
-        return self.deploy_services[server] if server in self.deploy_services else []
+        if server != "any":
+            return self.deploy_services[server] if server in self.deploy_services else []
+
+        servs = []
+        for aserver in self.deploy_services:
+            servs = list(set(servs + self.deploy_services[aserver]))
+
+        return servs
 
     def load_tasks_derived_files(self):
 
         self.derived_files = {}
 
         for t in self.tasks.values():
 
-            for out in t.get_derived_outputs(self):
+            for out in t.get_derived_outputs():
+
                 self.derived_files[out.name] = DerivedFile(
                     out.ftype,
                     os.path.join(self.get_work_dir(), t.name, out.path),
                     version=self.version,
                     task=t,
                     name=out.name,
                     tool_version=out.tool_version,
                     publish=out.publish,
                     depends_on=out.depends_on
                 )
 
+                if out.access_mode_from_children and self.has_mixed_data():
+                    # We only add the _restricted suffix when the entity has both public and restricted output
+                    # No suffix if all entity's data is public, or is restricted
+
+                    restr_name = "{}_restricted".format(out.name)
+                    self.derived_files[restr_name] = DerivedFile(
+                        out.ftype,
+                        os.path.join(self.get_work_dir(), t.name + "_restricted", out.path),
+                        version=self.version,
+                        task=t,
+                        name=restr_name,
+                        tool_version=out.tool_version,
+                        publish=out.publish,
+                        depends_on=out.depends_on
+                    )
+
     def accept_task(self, task):
         """
         Some entities can refuse to run selected tasks if not applicable
         """
 
         return True
 
@@ -279,10 +326,84 @@
 
         if recursive:
             for child in self.get_children():
                 banks += child.get_blast_banks()
 
         return banks
 
-    def get_blast_link(self, bank, server):
+    def get_blast_link(self, bank, server, restricted=False):
 
         return '{id}'
+
+    def copy_and_purge_restricted_data(self):
+
+        newent = deepcopy(self)
+
+        if newent.restricted_to is not None:
+            return None
+
+        newent.purge_restricted_data()
+
+        return newent
+
+    def purge_restricted_data(self):
+
+        # If there are no subentities, nothing to do.
+        return self
+
+    def is_restricted(self):
+
+        return self.restricted_to is not None
+
+    def has_public_data(self):
+
+        if self.restricted_to is None:
+            return True
+
+        for child in self.get_children():
+            if child.has_public_data():
+                return True
+
+        return False
+
+    def has_restricted_data(self):
+
+        if self.restricted_to is not None:
+            return True
+
+        for child in self.get_children():
+            if child.has_restricted_data():
+                return True
+
+        return False
+
+    def has_mixed_data(self):
+
+        return self.has_public_data() and self.has_restricted_data()
+
+    def get_restricted_tos(self):
+
+        rtos = set()
+
+        if self.restricted_to is not None:
+            rtos.add(self.restricted_to)
+
+        for child in self.get_children():
+            rtos.update(child.get_restricted_tos())
+
+        return sorted(list(rtos))
+
+    def get_restricted_to_map(self, locked=False):
+
+        rtos = {}
+
+        if locked:
+            if self.locked_restricted_to:
+                rtos[self.slug()] = self.locked_restricted_to
+        else:
+            if self.restricted_to_not_inherited:
+                rtos[self.slug()] = self.restricted_to_not_inherited
+
+        for ch in self.get_children():
+            rtos.update(ch.get_restricted_to_map(locked))
+
+        return rtos
```

### Comparing `beauris-0.2/beauris/managed_file.py` & `beauris-0.3/beauris/managed_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -237,16 +237,16 @@
 
         yml = {
             "type": self.type,
         }
 
         yml['locked_path'] = self.locked_path if self.locked_path else ""
 
-        if self.tool_version:
-            yml['tool_version'] = self.tool_version
+        if self.get_tool_version():
+            yml['tool_version'] = self.get_tool_version()
 
         yml['revision'] = self.get_revision()
 
         if self.name:
             yml['name'] = self.name
 
         if self.task:
@@ -259,15 +259,15 @@
 
         return yml
 
     def get_metadata(self):
 
         # Set some default metadata, overwrite with stored ones (if any)
         metadata = {
-            'tool_version': self.tool_version if self.tool_version else "",
+            'tool_version': self.get_tool_version(),
             'revision': self.get_revision(),
             'type': self.type,
             'filename': os.path.basename(self.locked_path) if self.locked_path else os.path.basename(self.path),
             'name': self.name if self.name else "",
             'task_id': self.task.name if self.task else ""
         }
         metadata.update(self.metadata)
@@ -303,14 +303,27 @@
             return 0
 
         if self.is_dirty():
             return self.locked_revision + 1
 
         return self.locked_revision
 
+    def get_tool_version(self):
+
+        if self.task is not None:
+            task_output = self.task.get_derived_output_by_name(self.name)
+
+            if task_output is not None and task_output.tool_version and self.is_dirty():
+                return task_output.tool_version
+
+        if self.tool_version:
+            return self.tool_version
+
+        return ""
+
     def has_changed_since_last_lock(self):
 
         if ManagedFile.has_changed_since_last_lock(self):
             return True
 
         if self.is_dirty():
             return True
```

### Comparing `beauris-0.2/beauris/proteome.py` & `beauris-0.3/beauris/proteome.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,59 +10,63 @@
 log = logging.getLogger()
 
 
 class Proteome(ManagedEntity):
 
     def __init__(self, config, yml_data, organism):
 
-        ManagedEntity.__init__(self, config, default_services=organism.deploy_services, yml_data=yml_data)
-
         self.organism = organism
 
+        ManagedEntity.__init__(self, config, default_services=organism.deploy_services, yml_data=yml_data)
+
         self.version = self.yml_data['version']
 
         self.entity_name = 'proteome'
 
         self.input_files = {
             'fasta': InputFile.from_yml(self.yml_data["file"], name='fasta', version=self.version)
         }
 
         self.tasks = self.config.get_tasks(self)
 
         self.load_tasks_derived_files()
 
         self.blastbanks = [
-            BlastBank(self, 'blastdb_proteome', self.input_files['fasta'], self.derived_files['blastdb_phr'], "proteome", 'prot')
+            BlastBank(self, 'blastdb_proteome', self.input_files['fasta'], self.derived_files['blastdb_phr'], "proteome", 'prot', "blastdb")
         ]
 
     def get_children(self):
 
         return []
 
     def get_organism(self):
 
         return self.organism
 
+    def get_parent(self):
+
+        return self.organism
+
     def slug(self, short=False):
 
         if short:
-            return "{}_prot{}".format(self.organism.slug(short), self.version)
+            return "{}_prot{}".format(self.organism.slug(short), self.sanitize(self.version))
         else:
-            return "{}/proteome_{}".format(self.organism.slug(short), self.version)
+            return "{}/proteome_{}".format(self.organism.slug(short), self.sanitize(self.version))
 
     def pretty_name(self, with_parent=True):
 
         if with_parent:
             return "{} proteome {}".format(self.organism.pretty_name(), self.version)
         else:
             return "Proteome {}".format(self.version)
 
     def get_work_dir(self):
 
-        return os.path.join(self.organism.get_work_dir(), "proteome_{}".format(self.version))
+        return os.path.join(self.organism.get_work_dir(), "proteome_{}".format(self.sanitize(self.version)))
 
     def get_locked_yml(self):
 
         locked_yml = self.yml_data
 
         locked_yml['file'] = self.input_files['fasta'].to_yml()
```

### Comparing `beauris-0.2/beauris/task.py` & `beauris-0.3/beauris/task.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,62 +5,100 @@
 from .util import Util, file_state
 
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger()
 
 
 class TaskOutput():
-    def __init__(self, name, ftype, path, tool_version=None, publish=True, depends_on=[]):
+    def __init__(self, name, ftype, path, tool_version=None, publish=True, access_mode_from_children=False, depends_on=[]):
 
         self.name = name
         self.ftype = ftype
         self.path = path  # The path of the output file relative to the task workdir
         self.publish = publish
+        self.access_mode_from_children = access_mode_from_children  # If some children have restricted access, this output must have too
         self.tool_version = tool_version  # TODO get this from config/job_specs or by parsing output files
         self.depends_on = depends_on
 
 
 class Task():
 
-    def __init__(self, entity, name, depends_on=[], check_perms=False, specs_id="", workdir="", always_run=False, server=""):
-
-        if workdir:
-            self.workdir = workdir
-        else:
-            self.workdir = name
-            if server:
-                self.workdir += "_{}".format(server)
+    def __init__(self, entity, name, depends_on=[], check_perms=False, specs_id="", workdir="", always_run=False, server="", access_mode="public"):
 
         self.specs_id = specs_id if specs_id else name
 
         self.name = name
         self.entity = entity
 
         self.server = server
+        self.access_mode = access_mode
+
+        self.forced_workdir = False
+        self.set_workdir(workdir)
 
-        # TODO changing access restriction will trigger all tasks, maybe we could limit to only triggering deploy tasks in this case ?
         self.check_perms = check_perms
 
         # Sometimes a task depends on some intput/derived files, but will not generate any derived file
         # In this case, you can define dependencies at the task level instead of doing it on a derived file
         self.depends_on = depends_on
 
         # True when the task has been run (not in a previous run, just now)
         self.has_run = False
 
         # True if a task should always run, whatever the state of dependencies
         self.always_run = always_run
 
-    def get_derived_outputs(self, entity):
+    def set_workdir(self, workdir=""):
+
+        if workdir:
+            self.workdir = workdir
+            self.forced_workdir = True
+        elif not self.forced_workdir:  # Do not overwrite a forced workdir value
+            self.workdir = self.name
+
+            if self.server:
+                self.workdir += "_{}".format(self.server)
+            if self.access_mode and self.access_mode != "public":
+                self.workdir += "_{}".format(self.access_mode)
+
+    def set_server(self, server):
+
+        self.server = server
+        self.set_workdir()
+
+    def set_access_mode(self, access_mode):
+
+        self.access_mode = access_mode
+        self.set_workdir()
+
+    def get_derived_outputs(self):
         """
         Returns a dict of derived files produced by current task
         """
 
         return []
 
+    def run_only_for_services(self):
+        """
+        Returns a list of tuples (service_name, entity), task will be run only if the services are enabled for the corresponding entity
+        entity can be a list, in this case, the task will run if any of the entities has the service
+        """
+
+        return []
+
+    def get_derived_output_by_name(self, name):
+
+        outs = self.get_derived_outputs()
+
+        for cand in outs:
+            if cand.name == name:
+                return cand
+
+        return None
+
     def slug(self, short=True):
 
         slug = "{}_{}".format(self.name, self.entity.slug(short=short))
 
         if self.server:
             slug += "_{}".format(self.server)
 
@@ -205,15 +243,15 @@
     def get_data_state(self):
 
         state = {}
 
         state['entity'] = self.entity.slug()
 
         if self.check_perms:
-            state['restricted_to'] = self.entity.get_organism().restricted_to
+            state['restricted_to'] = self.entity.get_restricted_to_map()
 
         dep_num = 0
 
         for id, exp_res in self.entity.derived_files.items():
 
             if exp_res.task.name != self.name or exp_res.task.server != self.server:
                 continue
@@ -239,30 +277,30 @@
         previous_state = self.load_previous_data_state()
 
         return current_state != previous_state
 
     def deps_have_changed_since_last_lock(self):
 
         if self.check_perms:
-            current_perms = self.entity.get_organism().restricted_to
-            locked_perms = self.entity.get_organism().locked_restricted_to
+            current_perms = self.entity.get_restricted_to_map()
+            locked_perms = self.entity.get_restricted_to_map(locked=True)
 
             if current_perms != locked_perms:
                 return True
 
         for id, exp_res in self.entity.derived_files.items():
 
             if exp_res.task.name != self.name or exp_res.task.server != self.server:
                 continue
 
             for res_dep in exp_res.depends_on:
                 if res_dep.has_changed_since_last_lock():
-                    log.debug("Dep {} has changed since last lock for {}".format(res_dep.name, exp_res.name))
+                    # log.debug("Dep {} has changed since last lock for {}".format(res_dep.name, exp_res.name))
                     return True
-                log.debug("No change since last lock in dep {} for {}".format(res_dep.name, exp_res.name))
+                # log.debug("No change since last lock in dep {} for {}".format(res_dep.name, exp_res.name))
 
         for res_dep in self.depends_on:
             if res_dep.has_changed_since_last_lock():
                 log.info("Task dep {} has changed since last lock".format(res_dep.name))
                 return True
             log.debug("No change since last lock in task dep {}".format(res_dep.name))
 
@@ -310,25 +348,45 @@
             if not exp.file_exists(locked=locked):
                 return False
 
         return True
 
     def needs_to_run(self, since='last_lock'):
 
+        required_by_service = self.check_required_by_services()
+
         changed = self.deps_have_changed(since=since)
 
         if self.disable_run():
             log.debug("Task {} is disabled by labels".format(self.name))
 
         elif self.force_run():
-            log.debug("Task {} is forced to run by labels".format(self.name))
+            log.debug("Task {} is forced to run".format(self.name))
 
         elif changed:
             log.debug("Task {} needs to run because of changed dependencies".format(self.name))
 
         elif not self.derived_files_exist(locked=True):
             log.debug("Task {} needs to run because of missing derived files".format(self.name))
 
-        # This could be cached in most cases, but it would made testing awkward
-        needs_to_run = not self.disable_run() and (self.force_run() or changed or not self.derived_files_exist(locked=True))
+        # This could be cached in most cases, but it would make testing awkward
+        needs_to_run = not self.disable_run() and required_by_service and (self.force_run() or changed or not self.derived_files_exist(locked=True))
 
         return needs_to_run
+
+    def check_required_by_services(self):
+
+        if len(self.run_only_for_services()) == 0:
+            return True
+
+        for rufs in self.run_only_for_services():
+            serv = rufs[0]
+            ents = rufs[1]
+
+            if not isinstance(ents, list):
+                ents = [ents]
+
+            for ent in ents:
+                if serv in ent.get_deploy_services("any"):
+                    return True
+
+        return False
```

### Comparing `beauris-0.2/beauris/tasks/annotation.py` & `beauris-0.3/beauris/tasks/annotation.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,43 +22,43 @@
             'blastdb_proteins': BlastProteinsTask,
             'blastdb_transcripts': BlastTranscriptsTask,
         }
 
 
 class OgsCheckTask(Task):
 
-    def get_derived_outputs(self, entity):
+    def get_derived_outputs(self):
 
-        deps = [entity.assembly.input_files['fasta'], entity.input_files['gff']]
+        deps = [self.entity.assembly.input_files['fasta'], self.entity.input_files['gff']]
 
         return [
             TaskOutput(name='fixed_gff', ftype='gff', path='fixed.gff', depends_on=deps),
         ]
 
 
 class GffReadTask(Task):
 
-    def get_derived_outputs(self, entity):
+    def get_derived_outputs(self):
 
-        deps = [entity.assembly.input_files['fasta'], entity.input_files['gff']]
+        deps = [self.entity.assembly.input_files['fasta'], self.entity.input_files['gff']]
 
         tool_version = '0.12.7'
 
         return [
-            TaskOutput(name='cds_fa', ftype='fasta', path="{}_cds.fa".format(entity.slug(True)), tool_version=tool_version, depends_on=deps),
-            TaskOutput(name='proteins_fa', ftype='fasta', path="{}_proteins.fa".format(entity.slug(True)), tool_version=tool_version, depends_on=deps),
-            TaskOutput(name='transcripts_fa', ftype='fasta', path="{}_transcripts.fa".format(entity.slug(True)), tool_version=tool_version, depends_on=deps),
+            TaskOutput(name='cds_fa', ftype='fasta', path="{}_cds.fa".format(self.entity.slug(True)), tool_version=tool_version, depends_on=deps),
+            TaskOutput(name='proteins_fa', ftype='fasta', path="{}_proteins.fa".format(self.entity.slug(True)), tool_version=tool_version, depends_on=deps),
+            TaskOutput(name='transcripts_fa', ftype='fasta', path="{}_transcripts.fa".format(self.entity.slug(True)), tool_version=tool_version, depends_on=deps),
         ]
 
 
 class FuncAnnotBipaaTask(Task):
 
-    def get_derived_outputs(self, entity):
+    def get_derived_outputs(self):
 
-        deps = [entity.derived_files['proteins_fa']]
+        deps = [self.entity.derived_files['proteins_fa']]
 
         return [
             TaskOutput(name='blast2go_annot', ftype='tsv', path="results/blast2go.annot", tool_version='2.5', depends_on=deps),
             TaskOutput(name='blast2go_gaf', ftype='tsv', path="results/blast2go.gaf", tool_version='2.5', depends_on=deps),
             TaskOutput(name='blast2go_pdf', ftype='pdf', path="results/blast2go_report.pdf", tool_version='2.5', depends_on=deps),
             TaskOutput(name='diamond', ftype='xml', path="results/diamond_all.xml", tool_version="2.0.13 on NR 2022-11-30", depends_on=deps),
             TaskOutput(name='eggnog', ftype='tsv', path="results/eggnog_annotations.tsv", tool_version="2.1.9", depends_on=deps),
@@ -70,18 +70,18 @@
 class FuncAnnotOrsonTask(Task):
 
     dmnd_ext = ['tab', 'xml']
     iprscan_ext = ['tsv', 'xml']
     emap_ext = ['annotations', 'hits', 'seed_orthologs']
     busco_ext = ['json', 'txt']
 
-    def get_derived_outputs(self, entity):
+    def get_derived_outputs(self):
 
-        options = entity.get_task_options(self.name)
-        deps = [entity.derived_files['proteins_fa']]
+        options = self.entity.get_task_options(self.name)
+        deps = [self.entity.derived_files['proteins_fa']]
         outputs = []
         for ext in self.dmnd_ext:
             outputs.append(TaskOutput(name='diamond_{}'.format(ext), ftype=ext,
                            path="results/03_final_results/merged_diamond.{}".format(ext),
                            tool_version="2.0.15 on Uniref90 2022-03", depends_on=deps))
         for ext in self.emap_ext:
             outputs.append(TaskOutput(name='eggnog_{}'.format(ext), ftype=ext,
@@ -101,40 +101,40 @@
         outputs.append(TaskOutput(name='beedeem', ftype='zml',
                                   path="results/03_final_results/merged_diamond_beedeem_annotation.zml",
                                   tool_version='4.7.6', depends_on=deps))
         if 'hectar' in options and options['hectar']:
             outputs.append(TaskOutput(name='hectar', ftype='csv',
                            path="results/03_final_results/result_hectar.csv",
                            tool_version="1.3", depends_on=deps))
-        outputs.append(TaskOutput(name='fasta', ftype='fa',
+        outputs.append(TaskOutput(name='described_fasta', ftype='fa',
                                   path="results/03_final_results/described_fasta.fa", depends_on=deps))
-        outputs.append(TaskOutput(name='gff', ftype='gff',
+        outputs.append(TaskOutput(name='described_gff', ftype='gff',
                                   path="results/03_final_results/described_gff.gff", depends_on=deps))
         return outputs
 
 
 class BlastTask(Task):
 
     blastdb_exts = ['nhr', 'nin', 'nog', 'nsd', 'nsi', 'nsq']
 
     fa_type = 'xxx'  # Adapt this in subclasses
 
     params = {
         'specs_id': 'blastdb'
     }
 
-    def get_derived_outputs(self, entity):
+    def get_derived_outputs(self):
 
         outputs = []
 
         tool_version = '2.6.0'
 
-        deps = [entity.derived_files['proteins_fa'], entity.derived_files['cds_fa'], entity.derived_files['transcripts_fa']]
+        deps = [self.entity.derived_files['proteins_fa'], self.entity.derived_files['cds_fa'], self.entity.derived_files['transcripts_fa']]
 
-        fasta_file = [file for file in entity.derived_files.values() if file.type == "fasta"]
+        fasta_file = [file for file in self.entity.derived_files.values() if file.type == "fasta"]
 
         for file in fasta_file:
             annot_type = file.name.split("_fa")[0]
             for ext in self.blastdb_exts:
                 if self.fa_type in file.name:
 
                     outputs.append(TaskOutput(name="blastdb_{}_{}".format(annot_type, ext), ftype=ext, path="annotation_{}.{}".format(annot_type, ext), tool_version=tool_version, publish=False, depends_on=deps))
```

### Comparing `beauris-0.2/beauris/tasks/assembly.py` & `beauris-0.3/beauris/tasks/assembly.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,34 +27,50 @@
 class FastaCheckTask(Task):
 
     pass
 
 
 class JBrowseTask(Task):
 
-    def get_derived_outputs(self, entity):
+    # If restricted_to changed on some track, need to regenerate
+    params = {
+        'check_perms': True
+    }
+
+    def run_only_for_services(self):
+
+        return [
+            ('jbrowse', self.entity),
+            ('apollo', self.entity),
+        ]
+
+    def get_derived_outputs(self):
 
-        deps = [entity.input_files['fasta']]
-        for ann in entity.annotations:
+        if not self.check_required_by_services():
+            log.info('Loading tasks plan: JBrowse is not derived for {}'.format(self.entity.slug()))
+            return []
+
+        deps = [self.entity.input_files['fasta']]
+        for ann in self.entity.annotations:
             deps.append(ann.input_files['gff'])
-        for track in entity.tracks:
+        for track in self.entity.tracks:
             deps.append(track.input_files['track_file'])
 
         tool_version = '1.16.11'
 
         return [
-            TaskOutput(name='jbrowse', ftype='jbrowse', path='jbrowse.tar.gz', tool_version=tool_version, publish=False, depends_on=deps),
+            TaskOutput(name='jbrowse', ftype='jbrowse', path='jbrowse.tar.gz', tool_version=tool_version, publish=False, access_mode_from_children=True, depends_on=deps),
         ]
 
 
 class FaToTwoBitTask(Task):
 
-    def get_derived_outputs(self, entity):
+    def get_derived_outputs(self):
 
-        deps = [entity.input_files['fasta']]
+        deps = [self.entity.input_files['fasta']]
 
         tool_version = '357'
 
         return [
             TaskOutput(name='2bit', ftype='2bit', path='genome.2bit', tool_version=tool_version, publish=False, depends_on=deps),
         ]
 
@@ -63,36 +79,43 @@
 
     params = {
         'specs_id': 'blastdb'
     }
 
     blastdb_exts = ['nhr', 'nin', 'nog', 'nsd', 'nsi', 'nsq']
 
-    def get_derived_outputs(self, entity):
+    def get_derived_outputs(self):
 
         outputs = []
 
         tool_version = '2.6.0'
 
-        deps = [entity.input_files['fasta']]
+        deps = [self.entity.input_files['fasta']]
 
         for ext in self.blastdb_exts:
             outputs.append(TaskOutput(name="blastdb_{}".format(ext), ftype=ext, path="assembly.{}".format(ext), tool_version=tool_version, publish=False, depends_on=deps))
 
         return outputs
 
 
 class ApolloTask(Task):
 
-    pass
+    # If restricted_to changed, jbrowse contextual menu may change => redeploy
+    params = {
+        'check_perms': True
+    }
 
 
 class ApolloPermsTask(Task):
 
     params = {
         'check_perms': True
     }
 
 
 class DeployJbrowseTask(Task):
 
-    pass
+    # If restricted_to changed, jbrowse contextual menu may change => redeploy
+    params = {
+        'check_perms': True,
+        'always_run': True
+    }
```

### Comparing `beauris-0.2/beauris/tasks/organism.py` & `beauris-0.3/beauris/tasks/organism.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,26 +10,27 @@
 
     entity_name = 'organism'
 
     @staticmethod
     def get_tasks():
 
         return {
-            'deploy_perms': DeployPermsTask,
+            'build_genoboo': BuildGenobooTask,
+            'build_elasticsearch': BuildElasticsearchTask,
+
+            'deploy_authelia': DeployAutheliaTask,
             'deploy_download': DeployDownloadTask,
             'deploy_blast': DeployBlastTask,
             'deploy_jbrowse': DeployJBrowseTask,
-            'build_genoboo': BuildGenobooTask,
             'deploy_genoboo': DeployGenobooTask,
-            'build_elasticsearch': BuildElasticsearchTask,
             'deploy_elasticsearch': DeployElasticsearchTask
         }
 
 
-class DeployPermsTask(Task):
+class DeployAutheliaTask(Task):
 
     params = {
         'always_run': True
     }
 
 
 class DeployDownloadTask(Task):
@@ -65,78 +66,94 @@
     params = {
         'always_run': True
     }
 
 
 class BuildGenobooTask(Task):
 
+    params = {
+        'check_perms': True
+    }
+
+    def run_only_for_services(self):
+
+        return [
+            ('genoboo', self.entity.assemblies)
+        ]
+
     def get_func_annot_files(self, annot):
         data = []
         # Need diamond (xml), interproscan (tsv), and eggnog (tsv)
         if 'func_annot_bipaa' in annot.tasks:
             data.append(annot.derived_files['interproscan'])
             data.append(annot.derived_files['diamond'])
             data.append(annot.derived_files['eggnog'])
         elif 'func_annot_orson' in annot.tasks:
             data.append(annot.derived_files['interproscan_tsv'])
             data.append(annot.derived_files['diamond_xml'])
             data.append(annot.derived_files['eggnog_annotations'])
         return data
 
-    def get_derived_outputs(self, entity):
+    def get_derived_outputs(self):
 
-        if not entity.assemblies or ('genoboo' not in entity.get_deploy_services("staging") and 'genoboo' not in entity.get_deploy_services("production")):
-            log.info('Genoboo is not derived for {}'.format(entity.slug()))
+        if not self.entity.assemblies or not self.check_required_by_services():
+            log.info('Loading tasks plan: Genoboo is not derived for {}'.format(self.entity.slug()))
             return []
 
         deps = []
-        if entity.assemblies:
-            for ass in entity.assemblies:
+        if self.entity.assemblies:
+            for ass in self.entity.assemblies:
                 deps.append(ass.input_files['fasta'])
                 for annot in ass.annotations:
                     deps.append(annot.input_files['gff'])
                     deps += self.get_func_annot_files(annot)
                     for exp in annot.expressions:
                         deps.append(exp.input_files['table'])
 
-        tool_version = '0.4.3'
+        tool_version = '0.4.13'
 
         return [
-            TaskOutput(name='build_genoboo', ftype='genoboo', path='genoboo.tar.bz2', tool_version=tool_version, publish=False, depends_on=deps),
+            TaskOutput(name='build_genoboo', ftype='genoboo', path='genoboo.tar.bz2', tool_version=tool_version, publish=False, access_mode_from_children=True, depends_on=deps),
         ]
 
 
 class BuildElasticsearchTask(Task):
 
     params = {
         'check_perms': True
     }
 
+    def run_only_for_services(self):
+
+        return [
+            ('elasticsearch', self.entity.assemblies)
+        ]
+
     def get_func_annot_files(self, annot):
         data = []
         # Need diamond (xml), interproscan (tsv), and eggnog (tsv)
         if 'func_annot_bipaa' in annot.tasks:
             data.append(annot.derived_files['interproscan'])
             data.append(annot.derived_files['diamond'])
             data.append(annot.derived_files['eggnog'])
         elif 'func_annot_orson' in annot.tasks:
             data.append(annot.derived_files['interproscan_tsv'])
             data.append(annot.derived_files['diamond_xml'])
             data.append(annot.derived_files['eggnog_annotations'])
         return data
 
-    def get_derived_outputs(self, entity):
+    def get_derived_outputs(self):
 
-        if not entity.assemblies or not any([ass.annotations for ass in entity.assemblies]) or ('elasticsearch' not in entity.get_deploy_services("staging") and 'elasticsearch' not in entity.get_deploy_services("production")):
-            log.info('Elasticsearch is not derived for {}'.format(entity.slug()))
+        if not self.entity.assemblies or not any([ass.annotations for ass in self.entity.assemblies]) or not self.check_required_by_services():
+            log.info('Loading tasks plan: Elasticsearch is not derived for {}'.format(self.entity.slug()))
             return []
 
         deps = []
-        if entity.assemblies:
-            for ass in entity.assemblies:
+        if self.entity.assemblies:
+            for ass in self.entity.assemblies:
                 deps.append(ass.input_files['fasta'])
                 for annot in ass.annotations:
                     deps.append(annot.input_files['gff'])
                     deps += self.get_func_annot_files(annot)
                     for exp in annot.expressions:
                         deps.append(exp.input_files['table'])
```

### Comparing `beauris-0.2/beauris/tasks/proteome.py` & `beauris-0.3/beauris/tasks/proteome.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 
     params = {
         'specs_id': 'blastdb'
     }
 
     blastdb_exts = ['phr', 'pin', 'pog', 'psd', 'psi', 'psq']
 
-    def get_derived_outputs(self, entity):
+    def get_derived_outputs(self):
 
         outputs = []
 
         tool_version = '2.6.0'
 
-        deps = [entity.input_files['fasta']]
+        deps = [self.entity.input_files['fasta']]
 
         for ext in self.blastdb_exts:
             outputs.append(TaskOutput(name="blastdb_{}".format(ext), ftype=ext, path="proteome.{}".format(ext), tool_version=tool_version, publish=False, depends_on=deps))
 
         return outputs
```

### Comparing `beauris-0.2/beauris/tasks/tasks.py` & `beauris-0.3/beauris/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/tasks/track.py` & `beauris-0.3/beauris/tasks/track.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,29 +23,29 @@
 class TrackCheckTask(Task):
 
     pass
 
 
 class IndexBaiTask(Task):
 
-    def get_derived_outputs(self, entity):
+    def get_derived_outputs(self):
 
-        deps = [entity.input_files['track_file']]
+        deps = [self.entity.input_files['track_file']]
 
         tool_version = '1.15'
 
         return [
             TaskOutput(name='bai', ftype='bai', path='index.bai', tool_version=tool_version, publish=False, depends_on=deps),
         ]
 
 
 class BamToWigTask(Task):
 
-    def get_derived_outputs(self, entity):
+    def get_derived_outputs(self):
 
-        deps = [entity.input_files['track_file']]
+        deps = [self.entity.input_files['track_file']]
 
         tool_version = '3.4.2'
 
         return [
             TaskOutput(name='wig', ftype='wig', path='index.wig', tool_version=tool_version, publish=False, depends_on=deps),
         ]
```

### Comparing `beauris-0.2/beauris/tasks/transcriptome.py` & `beauris-0.3/beauris/tasks/transcriptome.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 
     params = {
         'specs_id': 'blastdb'
     }
 
     blastdb_exts = ['nhr', 'nin', 'nog', 'nsd', 'nsi', 'nsq']
 
-    def get_derived_outputs(self, entity):
+    def get_derived_outputs(self):
 
         outputs = []
 
         tool_version = '2.6.0'
 
-        deps = [entity.input_files['fasta']]
+        deps = [self.entity.input_files['fasta']]
 
         for ext in self.blastdb_exts:
             outputs.append(TaskOutput(name="blastdb_{}".format(ext), ftype=ext, path="transcriptome.{}".format(ext), tool_version=tool_version, publish=False, depends_on=deps))
 
         return outputs
```

### Comparing `beauris-0.2/beauris/track.py` & `beauris-0.3/beauris/track.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 log = logging.getLogger()
 
 
 class Track(ManagedEntity):
 
     def __init__(self, config, yml_data, assembly):
 
-        ManagedEntity.__init__(self, config, default_services=assembly.deploy_services, yml_data=yml_data)
-
         self.assembly = assembly
 
+        ManagedEntity.__init__(self, config, default_services=assembly.deploy_services, yml_data=yml_data)
+
         self.name = yml_data['name']
         self.safe_name = re.sub(r'[^a-zA-Z0-9-]', '_', self.name)
         self.type = yml_data['type']
 
         self.version = "0"  # No version for this kind of data
 
         self.entity_name = 'track'
@@ -46,28 +46,28 @@
         self.tasks = self.config.get_tasks(self)
 
         self.load_tasks_derived_files()
 
     def slug(self, short=False):
 
         if short:
-            return "{}_track{}".format(self.assembly.slug(short), self.safe_name)
+            return "{}_track{}".format(self.assembly.slug(short), self.sanitize(self.safe_name))
         else:
-            return "{}/track_{}".format(self.assembly.slug(short), self.safe_name)
+            return "{}/track_{}".format(self.assembly.slug(short), self.sanitize(self.safe_name))
 
     def pretty_name(self, with_parent=True):
 
         if with_parent:
             return "{} track {}".format(self.assembly.pretty_name(), self.safe_name)
         else:
             return "Track {}".format(self.safe_name)
 
     def get_work_dir(self):
 
-        return os.path.join(self.assembly.get_work_dir(), "track_{}".format(self.safe_name))
+        return os.path.join(self.assembly.get_work_dir(), "track_{}".format(self.sanitize(self.safe_name)))
 
     def get_locked_yml(self):
 
         locked_yml = self.yml_data
 
         locked_yml['file'] = self.input_files['track_file'].to_yml()
 
@@ -120,7 +120,11 @@
     def accept_task(self, task):
         """
         Some entities can refuse to run selected tasks if not applicable
         """
 
         allowed_tasks = self.index_tasks() + ['track_check']
         return task.name in allowed_tasks
+
+    def get_parent(self):
+
+        return self.assembly
```

### Comparing `beauris-0.2/beauris/transcriptome.py` & `beauris-0.3/beauris/transcriptome.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,59 +10,63 @@
 log = logging.getLogger()
 
 
 class Transcriptome(ManagedEntity):
 
     def __init__(self, config, yml_data, organism):
 
-        ManagedEntity.__init__(self, config, default_services=organism.deploy_services, yml_data=yml_data)
-
         self.organism = organism
 
+        ManagedEntity.__init__(self, config, default_services=organism.deploy_services, yml_data=yml_data)
+
         self.version = self.yml_data['version']
 
         self.entity_name = 'transcriptome'
 
         self.input_files = {
             'fasta': InputFile.from_yml(self.yml_data["file"], name='fasta', version=self.version)
         }
 
         self.tasks = self.config.get_tasks(self)
 
         self.load_tasks_derived_files()
 
         self.blastbanks = [
-            BlastBank(self, 'blastdb_transcriptome', self.input_files['fasta'], self.derived_files['blastdb_nhr'], "transcriptome", 'nucl')
+            BlastBank(self, 'blastdb_transcriptome', self.input_files['fasta'], self.derived_files['blastdb_nhr'], "transcriptome", 'nucl', "blastdb")
         ]
 
     def get_children(self):
 
         return []
 
     def get_organism(self):
 
         return self.organism
 
+    def get_parent(self):
+
+        return self.organism
+
     def slug(self, short=False):
 
         if short:
-            return "{}_trans{}".format(self.organism.slug(short), self.version)
+            return "{}_trans{}".format(self.organism.slug(short), self.sanitize(self.version))
         else:
-            return "{}/transcriptome_{}".format(self.organism.slug(short), self.version)
+            return "{}/transcriptome_{}".format(self.organism.slug(short), self.sanitize(self.version))
 
     def pretty_name(self, with_parent=True):
 
         if with_parent:
             return "{} transcriptome {}".format(self.organism.pretty_name(), self.version)
         else:
             return "Transcriptome {}".format(self.version)
 
     def get_work_dir(self):
 
-        return os.path.join(self.organism.get_work_dir(), "transcriptome_{}".format(self.version))
+        return os.path.join(self.organism.get_work_dir(), "transcriptome_{}".format(self.sanitize(self.version)))
 
     def get_locked_yml(self):
 
         locked_yml = self.yml_data
 
         locked_yml['file'] = self.input_files['fasta'].to_yml()
```

### Comparing `beauris-0.2/beauris/util.py` & `beauris-0.3/beauris/util.py`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/validation/ogs/ogs_check.py` & `beauris-0.3/beauris/validation/ogs/ogs_check.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,24 +21,58 @@
         child.qualifiers[parentKeyName][0] = parentName
 
     return
 
 
 class OgsCheck():
 
-    def __init__(self, source=None, no_size=False, adopt_rna_suffix="-R", rna_prefix="", exons_are_cds=False):
+    def __init__(self, source=None, no_size=False, adopt_rna_suffix="-R", rna_prefix="", exons_are_cds=False, extend_parent=False):
         self.mRNA_ids = []
         self.exon_ids = []
         self.skipped_types = set()
         self.qlistName = ['Name', 'ID']
         self.source = source
         self.no_size = no_size
         self.adopt_rna_suffix = adopt_rna_suffix
         self.rna_prefix = rna_prefix
         self.exons_are_cds = exons_are_cds
+        self.extend_parent = extend_parent
+        # Error management for tests. Checking logger cache does not work (shared cache between tests)
+        self.has_error = False
+
+    def check_excluded(self, gchild, mrna, force_error=False):
+        if gchild.location.start < mrna.location.start or gchild.location.start > mrna.location.end or \
+           gchild.location.end < mrna.location.start or gchild.location.end > mrna.location.end:
+            if 'ID' in gchild.qualifiers:
+                temp_id = gchild.qualifiers['ID']
+            elif 'ID' in mrna.qualifiers:
+                temp_id = mrna.qualifiers['ID']
+            else:
+                temp_id = "{}-{}".format(gchild.location.start, gchild.location.end)
+            if (not self.extend_parent or force_error):
+                log.error("{} {} is misplaced".format(gchild.type, temp_id))
+                self.has_error = True
+            else:
+                log.warning("{} {} is misplaced. Will extend containing mRNA".format(gchild.type, temp_id))
+            return True
+        return False
+
+    def extend_mrna(self, gchild, mrna):
+        start = mrna.location.start
+        end = mrna.location.end
+
+        # Are all cases managed by this?
+        if gchild.location.start < mrna.location.start:
+            start = gchild.location.start
+            log.warning("Extending mRNA start to {}".format(start))
+        if gchild.location.end > mrna.location.end:
+            end = gchild.location.end
+            log.warning("Extending mRNA end to {}".format(end))
+
+        return start, end
 
     def guess_exons_from_cds_utr(self, mrna):
 
         exon_coords = []  # List of exons
 
         for gchild in mrna.sub_features:  # exons, cds, utr
 
@@ -80,26 +114,30 @@
 
         if mrna.type == 'transcript':
             mrna.type = "mRNA"
 
         if mrna.type != 'mRNA':
             log.error("Found an unexpected feature type (expected mRNA): type={} id={}".format(mrna.type, mrna.qualifiers['ID']))
             self.skipped_types.add(mrna.type)
+            self.has_error = True
             return None
 
         if 'ID' not in mrna.qualifiers or len(mrna.qualifiers['ID']) == 0:
             log.error("Found an mRNA without an ID attribute")
+            self.has_error = True
             return None
 
         if len(mrna.qualifiers['ID']) != 1:
             log.error("Found an mRNA with too many ID attributes ({})".format(mrna.qualifiers['ID']))
+            self.has_error = True
             return None
 
         if mrna.qualifiers['ID'][0] in self.mRNA_ids:
             log.error("Duplicate mRNA id: %s" % mrna.qualifiers['ID'][0])
+            self.has_error = True
             return None
 
         if 'Name' not in mrna.qualifiers:
             mrna.qualifiers['Name'] = mrna.qualifiers['ID']
 
         if is_complete:
             self.mRNA_ids.append(mrna.qualifiers['ID'][0])
@@ -122,14 +160,15 @@
             if gchild.type == "CDS":
                 if cds_min is None or gchild.location.start < cds_min:
                     cds_min = gchild.location.start
                 if cds_max is None or gchild.location.end > cds_max:
                     cds_max = gchild.location.end
 
         for gchild in mrna.sub_features:  # exons, cds, utr
+            skip = False
 
             if self.source:
                 gchild.qualifiers['source'][0] = self.source
 
             if gchild.type == "exon":
                 exon_coords[gchild.location.start] = gchild.location.end
             elif gchild.type == "CDS":
@@ -139,55 +178,60 @@
                 gchild.type = 'five_prime_UTR'
 
             elif gchild.type in ['three_prime_utr', "3'UTR"]:
                 gchild.type = 'three_prime_UTR'
 
             elif gchild.type == "UTR":
 
-                if gchild.location.start < mrna.location.start or gchild.location.start > mrna.location.end or \
-                   gchild.location.end < mrna.location.start or gchild.location.end > mrna.location.end:
-                    if 'ID' in gchild.qualifiers:
-                        temp_id = gchild.qualifiers['ID']
-                    elif 'ID' in mrna.qualifiers:
-                        temp_id = mrna.qualifiers['ID']
-                    else:
-                        temp_id = "{}-{}".format(gchild.location.start, gchild.location.end)
-                    log.error("UTR {} is misplaced".format(temp_id))
-
-                elif gchild.location.strand == 1:
+                if gchild.location.strand == 1:
                     if (gchild.location.start <= cds_min and  # noqa W504
                        gchild.location.end <= cds_min) or cds_min is None or cds_max is None:
                         gchild.type = 'five_prime_UTR'
 
                     elif gchild.location.start >= cds_max and gchild.location.end >= cds_max:
                         gchild.type = 'three_prime_UTR'
                 else:
                     if (gchild.location.start <= cds_min and  # noqa W504
                        gchild.location.end <= cds_min) or cds_min is None or cds_max is None:
                         gchild.type = 'three_prime_UTR'
 
                     elif gchild.location.start >= cds_max and gchild.location.end >= cds_max:
                         gchild.type = 'five_prime_UTR'
 
+            # UTR case is already managed above
+            if gchild.type in ['exon', 'CDS', 'five_prime_UTR', 'three_prime_UTR']:
+                if self.check_excluded(gchild, mrna):
+                    if self.extend_parent:
+                        new_start, new_end = self.extend_mrna(gchild, mrna)
+                        mrna.location = FeatureLocation(new_start, new_end, mrna.location.strand, mrna.location.ref, mrna.location.ref_db)
+                    else:
+                        skip = True
+            # We skip this entity, we cannot manage it
+            if skip:
+                continue
+
             if gchild.type in ['exon', 'CDS', 'five_prime_UTR', 'three_prime_UTR', 'non_canonical_five_prime_splice_site', 'non_canonical_three_prime_splice_site']:
                 kept_gchild.append(gchild)
             else:
                 self.skipped_types.add(gchild.type)
 
             if gchild.type == "exon":
                 if 'ID' not in gchild.qualifiers or len(gchild.qualifiers['ID']) == 0:
                     log.error("Found an exon without an ID attribute ({}-{})".format(gchild.location.start, gchild.location.end))
+                    self.has_error = True
                     return None
 
                 if len(gchild.qualifiers['ID']) != 1:
                     log.error("Found an exon with too many ID attributes ({})".format(gchild.qualifiers['ID']))
+                    self.has_error = True
                     return None
 
                 if gchild.qualifiers['ID'][0] in self.exon_ids:
                     log.error("Duplicate exon id: %s" % mrna.qualifiers['ID'][0])
+                    self.has_error = True
                     return None
 
                 self.exon_ids.append(gchild.qualifiers['ID'][0])
 
         mrna.sub_features = kept_gchild
 
         if cds_cumul > 0 and len(self.exon_ids) == 0:
@@ -272,14 +316,15 @@
         if orphan is not None:
 
             if parent_id in self.new_genes:
                 potential_parent = self.new_genes[parent_id]
 
                 if potential_parent.location.strand != orphan.location.strand:
                     log.error("Conflict between an orphan %s and its potential parent %s strand: %s != %s" % (orphan.type, parent_id, orphan.location.strand, potential_parent.location.strand))
+                    self.has_error = True
                     return None
 
                 potential_parent.sub_features.append(orphan)
 
                 if potential_parent.location.start > orphan.location.start:
                     potential_parent.location = FeatureLocation(orphan.location.start, potential_parent.location.end, strand=potential_parent.location.strand)
 
@@ -311,14 +356,15 @@
                 del self.inferred_parents[orphan.qualifiers['ID'][0]]
 
         if parent_id in self.all_mrnas:
             potential_parent = self.all_mrnas[parent_id]
 
             if potential_parent.location.strand != orphan.location.strand:
                 log.error("Conflict between an orphan %s and its potential parent %s strand: %s != %s" % (orphan.type, parent_id, orphan.location.strand, potential_parent.location.strand))
+                self.has_error = True
                 return None
 
             del orphan.qualifiers['Parent']  # previous parent is no longer parent
             potential_parent.sub_features.append(orphan)
 
             if potential_parent.location.start > orphan.location.start:
                 potential_parent.location = FeatureLocation(orphan.location.start, potential_parent.location.end, strand=potential_parent.location.strand)
@@ -378,14 +424,15 @@
                     fasta_content.add(line.split(" ")[0].strip().lstrip(">"))
 
         scaffs = []
         for scaff in GFF.parse(gff):
 
             if scaff.id not in fasta_content:
                 log.error("{} is not in related fasta file".format(scaff.id))
+                self.has_error = True
 
             scaff.annotations = {}
             scaff.seq = ""
 
             # Genes and mRNA list, reset on each new scaff
             self.new_genes = {}
             self.all_mrnas = {}
@@ -398,22 +445,25 @@
                 if topfeat.type not in ['gene', 'mRNA', 'CDS', 'exon']:
                     if topfeat.type != 'inferred_parent':
                         self.skipped_types.add(topfeat.type)
                     continue
 
                 if 'ID' not in topfeat.qualifiers or len(topfeat.qualifiers['ID']) == 0:
                     log.error("Found a top level %s feature without an ID attribute (%s-%s)" % (topfeat.type, topfeat.location.start, topfeat.location.end))
+                    self.has_error = True
                     continue
 
                 if len(topfeat.qualifiers['ID']) != 1:
                     log.error("Found a top level %s feature with too many ID attributes (%s)" % (topfeat.type, topfeat.qualifiers['ID']))
+                    self.has_error = True
                     continue
 
                 if topfeat.qualifiers['ID'][0] in self.new_genes.keys():
                     log.error("Duplicate top level %s feature id: %s" % (topfeat.qualifiers['ID'][0], topfeat.type))
+                    self.has_error = True
                     continue
 
                 if topfeat.type == 'gene':
                     # Simple case: a gene with sub features
                     new_mrnas = []
 
                     for mrna in topfeat.sub_features:
@@ -443,69 +493,76 @@
                     self.adopt_orphan_mrna(topfeat)
 
                 elif topfeat.type in ['exon', 'CDS']:
                     # Found an exon/cds without gene parent
                     self.adopt_orphan_exoncds(topfeat)
                 else:
                     log.error('Unexpected feature type %s. There is a bug.' % topfeat.type)
+                    self.has_error = True
 
             # Now handle the remaining inferred_parents
             for topfeat_name in self.inferred_parents:
                 topfeat = self.inferred_parents[topfeat_name]
 
                 if len(topfeat.sub_features) < 1:
                     log.error("Skipping an inferred_parent without children %s" % topfeat)
+                    self.has_error = True
                     continue
 
                 guessed_type = None
                 if topfeat.sub_features[0].type in ['exon', 'CDS', 'start_codon', 'stop_codon', 'UTR', "5'UTR", 'five_prime_UTR', 'five_prime_utr', "3'UTR", 'three_prime_UTR', 'three_prime_utr']:
                     guessed_type = 'mRNA'
                 elif topfeat.sub_features[0].type == 'mRNA':
                     guessed_type = 'gene'
                 else:
                     log.error("Skipping an inferred_parent: failed to guess type %s" % topfeat)
+                    self.has_error = True
                     continue
 
                 if guessed_type == 'mRNA':
                     num_seen = 0
                     for sub in topfeat.sub_features:
                         num_seen += 1
                         last_one = num_seen == len(topfeat.sub_features)
                         self.adopt_orphan_exoncds(sub, last_one=last_one)
 
                 elif guessed_type == 'gene':
                     for sub in topfeat.sub_features:
                         self.adopt_orphan_mrna(sub)
                 else:
                     log.error('Unexpected feature type %s. There is a bug.' % topfeat.type)
+                    self.has_error = True
 
             scaff.features = self.new_genes.values()
 
             if len(self.new_genes):
                 scaffs.append(scaff)
 
         if self.skipped_types:
             log.warning("Skipped unknown/misplaced feature types: %s" % (self.skipped_types))
 
         with open(out_gff, 'w') as f:
             GFF.write(scaffs, f)
 
+        return self.has_error
+
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     parser.add_argument('infile', type=str, help="Input GFF")
     parser.add_argument('genome', type=str, help="Genome sequence (fasta format)")
     parser.add_argument('dest', type=str, help="Output GFF")
     parser.add_argument('--source', help="Change the source to given value for all features")
     parser.add_argument('--no-size', action='store_true', help="Disable CDS and intron size checking")
     parser.add_argument('--adopt-rna-suffix', help="Suffix to be appended to orphan mRNA ids when adopted by newly created genes", default="-R")
     parser.add_argument('--exons-are-cds', action='store_true', help="Consider that exons represent CDS (when cds are absent and exons are present)")
     parser.add_argument("--rna-prefix", type=str, help="mRNA prefix to add to mRNAs and subfeatures", default="")
+    parser.add_argument('--extend-parent', action='store_true', help="Extend mRNA if subentities are outside of it")
     args = parser.parse_args()
 
     log.info("Checking %s (with genome %s), will write fixed GFF to %s" % (args.infile, args.genome, args.dest))
-    ogsc = OgsCheck(args.source, args.no_size, args.adopt_rna_suffix, args.rna_prefix, args.exons_are_cds)
+    ogsc = OgsCheck(args.source, args.no_size, args.adopt_rna_suffix, args.rna_prefix, args.exons_are_cds, args.extend_parent)
     ogsc.check(args.infile, args.genome, args.dest)
 
     # Raise an error if there were some logged
     if 40 in log._cache and log._cache[40]:
         sys.exit(1)
```

### Comparing `beauris-0.2/beauris/validation/template/ext.py` & `beauris-0.3/beauris/validation/template/ext.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,76 @@
 # -*- coding: utf-8 -*-
 
 import logging
 import os
 import re
 
+from pykwalify.errors import SchemaError
+
 import requests
 
 log = logging.getLogger(__name__)
 
 
 def is_file(value, rule_obj, path):
+    if not path.startswith("/"):
+        raise SchemaError("Path {} is not an absolute path".format(value))
     if os.path.isfile(value):
         return True
-    raise Exception("Path {} is not a file".format(value))
+    elif os.path.isdir(value):
+        raise SchemaError("Path {} is a directly".format(value))
+    else:
+        _validate_path_exists(value)
+    raise SchemaError("Path {} is not a file".format(value))
 
 
 def is_dir(value, rule_obj, path):
     if os.path.isdir(value):
         return True
-    raise Exception("Path {} is not a directory".format(value))
+
+    raise SchemaError("Path {} is not a directory".format(value))
 
 
 def is_valid_name(value, rule_obj, path):
     # Only accept alphanumericals & - & _
     if re.match(r'^[A-Za-z0-9_-]+$', value):
         return True
-    raise Exception("Name {} is not a valid internal name".format(value))
+    raise SchemaError("Name {} is not a valid internal name".format(value))
 
 
 def ext_onto_organism(value, rule_obj, path):
     log.debug("value: %s", value)
     log.debug("rule_obj: %s", rule_obj)
     log.debug("path: %s", path)
     # TODO: Better management when EBI is down
     return True
     # return _validate_ontological_term(value, "NCBITAXON")
 
 
+def _validate_path_exists(file_path, symlink=False):
+    current_path = "/"
+    for subpath in file_path.split("/"):
+        current_path = os.path.join(current_path, subpath)
+        if not os.path.exists(current_path):
+            if current_path == file_path:
+                if not os.path.islink(file_path):
+                    if symlink:
+                        raise SchemaError("Error with link {}. Linked file {} does not exists.".format(symlink, file_path))
+                    else:
+                        raise SchemaError("Path {} is not a file".format(file_path))
+                continue
+            if symlink:
+                raise SchemaError("Error with link {}. In linked file {}: directory {} does not exist, or permissions on containing folder are wrong.".format(symlink, file_path, current_path))
+            else:
+                raise SchemaError("File {} not found: directory {} does not exist, or permissions on containing folder are wrong.".format(file_path, current_path))
+    # Do the same for link target
+    if os.path.islink(file_path):
+        _validate_path_exists(os.readlink(file_path), symlink=file_path)
+
+
 def _validate_ontological_term(term, ontology, root_term_iri=""):
     base_path = "http://www.ebi.ac.uk/ols/api/search"
     body = {
         "q": term,
         "ontology": ontology.lower(),
         "type": "class",
         "exact": True,
```

### Comparing `beauris-0.2/beauris/validation/template/schema.yaml` & `beauris-0.3/beauris/validation/template/schema.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -31,15 +31,16 @@
         required: false
       "source_url":
         type: str
         required: false
   "common_name":
     type: scalar
     func: ext_onto_organism
-    required: true
+    required: false
+    desc: "A pretty name for the organism (default: guessed from genus, species, strain, sex attributes)"
   "computer_name":
     type: scalar
     func: is_valid_name
     required: false
     desc: "Optional, guessed from genus, species, strain and sex if absent"
   "restricted_to":
     type: str
@@ -94,23 +95,31 @@
                 required: false
               "revision":
                 type: number
                 required: false
               "type":
                 type: str
                 required: true
-                enum: ["fasta", "gff", "bam", "tsv", "jbrowse", "jbrowse2" , "txt"]
+                enum: ["fasta", "gff", "bam", "tsv", "jbrowse", "jbrowse2" , "txt", "wig", "tar.bz2", "tar.gz", "vcf"]
           "date":
             type: date
           "source":
             type: str
           "description":
             type: str
             required: false
             desc: "Optional, free text description"
+          "xrefs":
+            type: map
+            allowempty: True
+          "restricted_to":
+            type: str
+          "restricted_to_apollo":
+            desc: "To set different restriction level on apollo, compared to the rest of the services"
+            type: str
           "status":
             <<: *status
           "task_options":
             <<: *task_options
           "services":
             <<: *services
           "derived": &derived
@@ -151,47 +160,70 @@
                   "source":
                     type: str
                     required: false
                   "description":
                     type: str
                     required: false
                     desc: "Optional, free text description"
+                  "xrefs":
+                    type: map
+                    allowempty: True
+                  "restricted_to":
+                    type: str
                   "status":
                     <<: *status
                   "task_options":
                     <<: *task_options
                   "derived":
                     <<: *derived
                   "expression_data":
                     type: seq
                     sequence:
                       - type: map
                         mapping:
                           "name":
                             type: str
                             required: true
+                            desc: "Name must be unique"
                           "unit":
                             type: str
-                            required: true
+                            required: false
+                            desc: "Optional, default: TPM"
                           "table":
                             <<: *file
                           "date":
                             type: date
                             required: false
                           "source":
                             type: str
                             required: false
                           "description":
                             type: str
                             required: false
                             desc: "Optional, free text description"
+                          "restricted_to":
+                            type: str
                           "status":
                             <<: *status
                           "task_options":
                             <<: *task_options
+                          "replicates":
+                            type: seq
+                            sequence:
+                              - type: map
+                                mapping:
+                                  "name":
+                                    type: str
+                                    required: true
+                                  "cols":
+                                    required: true
+                                    type: seq
+                                    desc: "Number from 1, col 0 is the first column of the file, containing mRNA ids"
+                                    sequence:
+                                      - type: int
           "tracks":
             type: seq
             sequence:
               - type: map
                 mapping:
                   "name":
                     type: str
@@ -199,34 +231,81 @@
                     desc: "Name must be unique"
                   "sra_run_id":
                     type: str
                     required: false
                   "type":
                     type: str
                     required: true
-                    enum: ["rnaseq", "dnaseq", "gff"]
+                    enum: ["rnaseq", "dnaseq", "gff", "vcf"]
                   "category":
                     type: str
                     desc: "Name of a category where to place this track (e.g. for JBrowse). default=type attribute"
                   "date":
                     type: date
                     required: false
                   "source":
                     type: str
                     required: false
                   "description":
                     type: str
                     required: false
                     desc: "Optional, free text description"
+                  "restricted_to":
+                    type: str
+                  "file":
+                    type: map
+                    mapping:
+                      "path":
+                        type: str
+                        func: is_file
+                        required: true
+                      "locked_path":
+                        type: str
+                        func: is_file
+                        required: false
+                      "revision":
+                        type: number
+                        required: false
+                      "type":
+                        type: str
+                        required: true
+                        enum: ["gff", "bam", "vcf"]
+                  "status":
+                    <<: *status
+                  "task_options":
+                    <<: *task_options
+          "extra_files":
+            type: seq
+            sequence:
+              - type: map
+                mapping:
+                  "name":
+                    type: str
+                    required: true
+                    desc: "Name must be unique"
                   "file":
                     <<: *file
+                  "date":
+                    type: date
+                  "source":
+                    type: str
+                  "description":
+                    type: str
+                    required: false
+                    desc: "Optional, free text description"
+                  "restricted_to":
+                    type: str
                   "status":
                     <<: *status
                   "task_options":
                     <<: *task_options
+                  "services":
+                    <<: *services
+                  "derived":
+                    <<: *derived
   "proteomes":
     type: seq
     sequence:
       - type: map
         mapping:
           "version":
             type: str
@@ -237,14 +316,16 @@
             type: date
           "source":
             type: str
           "description":
             type: str
             required: false
             desc: "Optional, free text description"
+          "restricted_to":
+            type: str
           "status":
             <<: *status
           "task_options":
             <<: *task_options
           "services":
             <<: *services
           "derived":
@@ -263,14 +344,45 @@
             type: date
           "source":
             type: str
           "description":
             type: str
             required: false
             desc: "Optional, free text description"
+          "restricted_to":
+            type: str
+          "status":
+            <<: *status
+          "task_options":
+            <<: *task_options
+          "services":
+            <<: *services
+          "derived":
+            <<: *derived
+  "extra_files":
+    type: seq
+    sequence:
+      - type: map
+        mapping:
+          "name":
+            type: str
+            required: true
+            desc: "Name must be unique"
+          "file":
+            <<: *file
+          "date":
+            type: date
+          "source":
+            type: str
+          "description":
+            type: str
+            required: false
+            desc: "Optional, free text description"
+          "restricted_to":
+            type: str
           "status":
             <<: *status
           "task_options":
             <<: *task_options
           "services":
             <<: *services
           "derived":
```

### Comparing `beauris-0.2/beauris/workflows/ansible/ansible_data/project/playbook_deploy.yml` & `beauris-0.3/beauris/workflows/ansible/ansible_data/project/playbook_deploy.yml`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/workflows/ansible/docker_files/postgres-blast-entrypoint.sh` & `beauris-0.3/beauris/workflows/ansible/docker_files/postgres-blast-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/workflows/ansible/templates/web/index.html.j2` & `beauris-0.3/beauris/workflows/ansible/templates/web/index.html.j2`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,23 @@
     <title>{{ org.pretty_name() }}</title>
   </head>
     <body>
     <div id="page">
       <div style="text-align:center">
         Welcome to the page for <b>{{ org.pretty_name() }}<b/>!
       </div>
-      {% if deploy_blast or src_data_folder or deploy_jbrowse or use_apollo or deploy_genoboo %}
+      {% if deploy_blast or deploy_download or deploy_jbrowse or use_apollo or deploy_genoboo %}
       <ul id="primary-menu" class="nav-menu">
         {% if deploy_jbrowse %}
         <li id="menu-item-46" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-has-children menu-item-46"><a href="{{base_url}}{{ url_prefix }}/{{ sub_url }}/jbrowse">Jbrowse</a></li>
         {% endif %}
         {% if deploy_blast %}
         <li id="menu-item-46" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-has-children menu-item-46"><a href="{{base_url}}{{ url_prefix }}/{{ sub_url }}/blast">Blast</a></li>
         {% endif %}
-        {% if src_data_folder %}
+        {% if deploy_download %}
         <li id="menu-item-46" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-has-children menu-item-46"><a href="{{base_url}}{{ url_prefix }}/{{ sub_url }}/download/">Dowload</a></li>
         {% endif %}
         {% if use_apollo %}
         <li id="menu-item-46" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-has-children menu-item-46"><a href="{{ apollo_url }}">Apollo</a>
         {% endif %}
         {% if deploy_genoboo %}
         <li id="menu-item-46" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-has-children menu-item-46"><a href="{{base_url}}{{ url_prefix }}/{{ sub_url }}/gnb">Genoboo</a>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 Welcome to the page for {{{{ oorrgg..pprreettttyy__nnaammee(()) }}}}!!
-{% if deploy_blast or src_data_folder or deploy_jbrowse or use_apollo or
+{% if deploy_blast or deploy_download or deploy_jbrowse or use_apollo or
 deploy_genoboo %}
     * {% if deploy_jbrowse %}
     * _J_b_r_o_w_s_e
     * {% endif %} {% if deploy_blast %}
     * _B_l_a_s_t
-    * {% endif %} {% if src_data_folder %}
+    * {% endif %} {% if deploy_download %}
     * _D_o_w_l_o_a_d
     * {% endif %} {% if use_apollo %}
     * _A_p_o_l_l_o {% endif %} {% if deploy_genoboo %}
     * _G_e_n_o_b_o_o {% endif %}
 {% endif %}
```

### Comparing `beauris-0.2/beauris/workflows/drmaa/add_fa_description.py` & `beauris-0.3/beauris/workflows/drmaa/add_fa_description.py`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/workflows/drmaa/add_gff_description.py` & `beauris-0.3/beauris/workflows/drmaa/add_gff_description.py`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/workflows/drmaa/bam_to_wig.py` & `beauris-0.3/beauris/workflows/drmaa/bam_to_wig.py`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/workflows/drmaa/blastdb.py` & `beauris-0.3/beauris/workflows/drmaa/blastdb.py`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/workflows/drmaa/fatotwobit.py` & `beauris-0.3/beauris/workflows/drmaa/fatotwobit.py`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/workflows/drmaa/func_annot_bipaa.py` & `beauris-0.3/beauris/workflows/drmaa/func_annot_bipaa.py`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/workflows/drmaa/func_annot_orson.py` & `beauris-0.3/beauris/workflows/drmaa/func_annot_orson.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,14 +35,17 @@
 
             options = annot.get_task_options(task_id)
             cmd_options = []
 
             if 'hectar' in options and options['hectar']:
                 cmd_options.append("--hectar_enable true")
 
+            if 'hectar_type' in options:
+                cmd_options.append("--hectar_type {}".format(options['hectar_type']))
+
             if cmd_options:
                 job_args.append(" ".join(cmd_options))
 
             runner = bo.get_runner('drmaa', annot, task_id)
             add_script = []
             add_script.append(os.path.join(os.path.dirname(os.path.realpath(__file__)), 'add_fa_description.py'))
             add_script.append(os.path.join(os.path.dirname(os.path.realpath(__file__)), 'add_gff_description.py'))
```

### Comparing `beauris-0.2/beauris/workflows/drmaa/func_annot_orson.sh` & `beauris-0.3/beauris/workflows/drmaa/func_annot_orson.sh`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,16 @@
   --chunk_size 200 \
   -c $CLUSTER_CONFIG_PATH \
   --outdir ./results \
   -w $SCRATCH_WORK_DIR \
   --projectName func_annot_orson \
   -ansi-log false \
   -resume \
-  $3
+  ${3- } ${4- } \
+  ${5- } ${6- }
 
 SCRIPT_DIR="$( cd -- "$( dirname -- "${BASH_SOURCE[0]:-$0}"; )" &> /dev/null && pwd 2> /dev/null; )";
 python3 $SCRIPT_DIR/add_fa_description.py --infile $1 --outfile ./results/03_final_results/described_fasta.fa --annotfile ./results/03_final_results/result.emapper.annotations
 python3 $SCRIPT_DIR/add_gff_description.py --gffFile $2 --outFile ./results/03_final_results/described_gff.gff --eggFile ./results/03_final_results/result.emapper.annotations
 
 cd ./results/02_intermediate_data/00_busco/busco_results_auto
 ln -sf short_summary.specific.*.busco_results_auto.json short_summary.specific.busco_results_auto.json
```

### Comparing `beauris-0.2/beauris/workflows/drmaa/gffread.py` & `beauris-0.3/beauris/workflows/drmaa/gffread.py`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/workflows/drmaa/gffread_fa_rename.py` & `beauris-0.3/beauris/workflows/drmaa/gffread_fa_rename.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             if line.startswith(">"):
 
                 if ncbi:
                     cur_id = line[1:].split(' ')[0].strip()
 
                     if cur_id in id_map:
                         line = ">{}".format(id_map[cur_id])
-                else:
+                elif regex is not None and replace is not None:
                     line = re.sub(regex, replace, line)
 
             outfa.write("%s\n" % line.strip())
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
@@ -69,10 +69,10 @@
     transcripts_fa_in = "{}_transcripts_raw.fa".format(args.prefix)
     proteins_fa_in = "{}_proteins_raw.fa".format(args.prefix)
 
     cds_fa_out = "{}_cds.fa".format(args.prefix)
     transcripts_fa_out = "{}_transcripts.fa".format(args.prefix)
     proteins_fa_out = "{}_proteins.fa".format(args.prefix)
 
-    replace_ids_in_fa(cds_fa_in, cds_fa_out, ncbi=args.ncbi_ids, regex=args.regex, replace=args.replace, id_map=ncbi_map_transcripts)
-    replace_ids_in_fa(transcripts_fa_in, transcripts_fa_out, ncbi=args.ncbi_ids, regex=args.regex, replace=args.replace, id_map=ncbi_map_transcripts)
+    replace_ids_in_fa(cds_fa_in, cds_fa_out, ncbi=args.ncbi_ids, regex=None, replace=None, id_map=ncbi_map_transcripts)
+    replace_ids_in_fa(transcripts_fa_in, transcripts_fa_out, ncbi=args.ncbi_ids, regex=None, replace=None, id_map=ncbi_map_transcripts)
     replace_ids_in_fa(proteins_fa_in, proteins_fa_out, ncbi=args.ncbi_ids, regex=args.regex, replace=args.replace, id_map=ncbi_map_proteins)
```

### Comparing `beauris-0.2/beauris/workflows/drmaa/index_bai.py` & `beauris-0.3/beauris/workflows/drmaa/index_bai.py`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/workflows/galaxy/genoboo.py` & `beauris-0.3/beauris/workflows/galaxy/genoboo.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python
 import argparse
 import logging
-import os
 import sys
 
 from beauris import Beauris
 
 
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger()
@@ -13,46 +12,32 @@
 
 def get_func_annot_files(file_uploads, annot):
     has_annot = False
     blast_db = None
     # Need diamond (xml), interproscan (tsv), and eggnog (tsv)
     if 'func_annot_bipaa' in annot.tasks:
         has_annot = True
-        blast_db = annot.derived_files['diamond'].tool_version
+        blast_db = annot.derived_files['diamond'].get_tool_version()
         file_uploads['interpro_{}'.format(annot.version)] = {'type': 'tsv', 'path': annot.get_derived_path('interproscan'), 'name': 'interpro_{}'.format(annot.version)}
         file_uploads['diamond_{}'.format(annot.version)] = {'type': 'blastxml', 'path': annot.get_derived_path('diamond'), 'name': 'diamond_{}'.format(annot.version)}
         file_uploads['eggnog_{}'.format(annot.version)] = {'type': 'tsv', 'path': annot.get_derived_path('eggnog'), 'name': 'eggnog_{}'.format(annot.version)}
     elif 'func_annot_orson' in annot.tasks:
         has_annot = True
-        blast_db = annot.derived_files['diamond_xml'].tool_version
+        blast_db = annot.derived_files['diamond_xml'].get_tool_version()
         file_uploads['interpro_{}'.format(annot.version)] = {'type': 'tsv', 'path': annot.get_derived_path('interproscan_tsv'), 'name': 'interpro_{}'.format(annot.version)}
         file_uploads['diamond_{}'.format(annot.version)] = {'type': 'blastxml', 'path': annot.get_derived_path('diamond_xml'), 'name': 'diamond_{}'.format(annot.version)}
         file_uploads['eggnog_{}'.format(annot.version)] = {'type': 'tsv', 'path': annot.get_derived_path('eggnog_annotations'), 'name': 'eggnog_{}'.format(annot.version)}
     return file_uploads, has_annot, blast_db
 
 
-if __name__ == '__main__':
-    parser = argparse.ArgumentParser()
-    parser.add_argument('infile', type=str)
-    args = parser.parse_args()
-
-    bo = Beauris()
-    org = bo.load_organism(args.infile)
-
-    # We need to check for both staging and production
-    if 'genoboo' not in org.get_deploy_services("staging") and 'genoboo' not in org.get_deploy_services("production"):
-        log.info('Genoboo is not required for {}'.format(org.slug()))
-        sys.exit(0)
-
-    if not org.assemblies:
-        log.error('At least one assembly is required for Genoboo')
-        sys.exit(0)
+def run_genoboo_job(org, access_mode="public"):
 
     task_id = "build_genoboo"
-    runner = bo.get_runner('galaxy', org, task_id)
+    runner = bo.get_runner('galaxy', org, task_id, access_mode=access_mode)
+
     config_task = runner.get_job_specs(task_id)
 
     # Get config values
     # Not really a great solution, but envsubst + regex is not a good mix
     re_protein = config_task.get("re_protein", "$1-P$2").replace(r"\$", "$")
     re_protein_capture = config_task.get("re_protein_capture", "^(.*?)-R([A-Z]+)$")
     blast_algorithm = config_task.get("blast_algorithm", "blastp")
@@ -63,139 +48,181 @@
     tools_params = {
         "existing": None
     }
 
     num_ass = 0
     # Use a precise tool version if possible
     # tool = "Genoboo"
-    tool = "toolshed.g2.bx.psu.edu/repos/gga/genenotebook_genenotebook_build/genenotebook_build/0.4.5+galaxy0"
+    tool = "toolshed.g2.bx.psu.edu/repos/gga/genenotebook_genenotebook_build/genenotebook_build/0.4.13+galaxy0"
     file_uploads = {}
 
     # Should loop on assemblies later
     # For now, only take the last assembly
-    ass = org.assemblies[-1]
-
-    if not ass.annotations:
-        log.error('At least one annotation is required for Genoboo')
-        sys.exit(0)
-
-    num_annot = 0
-
-    file_uploads['ass_{}'.format(ass.slug(short=True))] = {'type': 'fasta', 'path': ass.get_input_path('fasta'), 'name': ass.slug(short=True)}
+    for ass in org.assemblies:
 
-    base_key_genome = "genomes_{}|".format(num_ass)
-    ass_dict = {
-        base_key_genome + "name": ass.pretty_name(),
-        base_key_genome + "public": True,
-        base_key_genome + "genome": {
-            "batch": False,
-            "values": [
-                {
-                    "id": "##UPLOADED_DATASET_ID__ass_{}##".format(ass.slug(short=True)),
-                    "src": "hda",
-                }
-            ]
-        }
-    }
-    tools_params.update(ass_dict)
-    num_ass += 1
-
-    # Should loop on annotations later
-    annot = ass.annotations[-1]
-
-    base_key_annot = "{}annots_{}|".format(base_key_genome, num_annot)
+        num_annot = 0
 
-    file_uploads['annot_{}'.format(annot.version)] = {'type': 'gff3', 'path': annot.get_derived_path('fixed_gff'), 'name': annot.version}
-    # Get func annotation files
-    # Need diamond (xml), interproscan (tsv), and eggnog (tsv)
-    file_uploads, has_func_annot, blast_db = get_func_annot_files(file_uploads, annot)
+        file_uploads['ass_{}'.format(ass.slug(short=True))] = {'type': 'fasta', 'path': ass.get_input_path('fasta'), 'name': ass.slug(short=True)}
 
-    annot_dict = {
-        base_key_annot + "prot_naming|method": "regex",
-        base_key_annot + "prot_naming|re_protein": re_protein,
-        base_key_annot + "prot_naming|re_protein_capture": re_protein_capture,
-        base_key_annot + "annotation": {
-            "batch": False,
-            "values": [
-                {
-                    "id": "##UPLOADED_DATASET_ID__annot_{}##".format(annot.version),
-                    "src": "hda",
-                }
-            ]
-        }
-    }
-    if has_func_annot:
-        annot_dict.update({
-            base_key_annot + "blast_cond|blast_choice": "diamond",
-            base_key_annot + "blast_cond|algorithm": blast_algorithm,
-            base_key_annot + "blast_cond|database": blast_db,
-            base_key_annot + "blast_cond|matrix": blast_matrix,
-            base_key_annot + "blast_cond|blast": {
-                "batch": False,
-                "values": [
-                    {
-                        "id": "##UPLOADED_DATASET_ID__diamond_{}##".format(annot.version),
-                        "src": "hda",
-                    }
-                ]
-            },
-            base_key_annot + "eggnog": {
+        base_key_genome = "genomes_{}|".format(num_ass)
+        ass_dict = {
+            base_key_genome + "name": ass.pretty_name(),
+            base_key_genome + "public": True,
+            base_key_genome + "genome": {
                 "batch": False,
                 "values": [
                     {
-                        "id": "##UPLOADED_DATASET_ID__eggnog_{}##".format(annot.version),
-                        "src": "hda",
-                    }
-                ]
-            },
-            base_key_annot + "interproscan": {
-                "batch": False,
-                "values": [
-                    {
-                        "id": "##UPLOADED_DATASET_ID__interpro_{}##".format(annot.version),
+                        "id": "##UPLOADED_DATASET_ID__ass_{}##".format(ass.slug(short=True)),
                         "src": "hda",
                     }
                 ]
             }
-        })
+        }
+        tools_params.update(ass_dict)
+        num_ass += 1
 
-    exp_n = 0
-    for exp in annot.expressions:
-        file_uploads['expression_{}'.format(exp.safe_name)] = {'type': 'tsv', 'path': exp.get_input_path('table'), 'name': 'expression_{}'.format(exp.safe_name)}
-
-        base_key_exp = base_key_annot + "expression_{}|".format(exp_n)
-        annot_dict.update({
-            base_key_exp + "sample_name": exp.name,  # TODO is this really a sample name?
-            base_key_exp + "replica_group": exp.name,  # TODO add this to schema
-            base_key_exp + "sample_description": exp.get_metadata().get('description', exp.name),
-            base_key_exp + "counts": {
-                "batch": False,
-                "values": [
-                    {
-                        "id": "##UPLOADED_DATASET_ID__expression_{}##".format(exp.safe_name),  # TODO check uniqueness of safe_name
-                        "src": "hda",
+        # Should loop on annotations later
+        for annot in ass.annotations:
+
+            base_key_annot = "{}annots_{}|".format(base_key_genome, num_annot)
+
+            file_uploads['annot_{}'.format(annot.version)] = {'type': 'gff3', 'path': annot.get_derived_path('fixed_gff'), 'name': annot.version}
+            # Get func annotation files
+            # Need diamond (xml), interproscan (tsv), and eggnog (tsv)
+            file_uploads, has_func_annot, blast_db = get_func_annot_files(file_uploads, annot)
+
+            annot_dict = {
+                base_key_annot + "prot_naming|method": "regex",
+                base_key_annot + "annot": annot.version,
+                base_key_annot + "prot_naming|re_protein": re_protein,
+                base_key_annot + "prot_naming|re_protein_capture": re_protein_capture,
+                base_key_annot + "annotation": {
+                    "batch": False,
+                    "values": [
+                        {
+                            "id": "##UPLOADED_DATASET_ID__annot_{}##".format(annot.version),
+                            "src": "hda",
+                        }
+                    ]
+                }
+            }
+            if has_func_annot:
+                annot_dict.update({
+                    base_key_annot + "blast_cond|blast_choice": "diamond",
+                    base_key_annot + "blast_cond|algorithm": blast_algorithm,
+                    base_key_annot + "blast_cond|database": blast_db,
+                    base_key_annot + "blast_cond|matrix": blast_matrix,
+                    base_key_annot + "blast_cond|diamond": {
+                        "batch": False,
+                        "values": [
+                            {
+                                "id": "##UPLOADED_DATASET_ID__diamond_{}##".format(annot.version),
+                                "src": "hda",
+                            }
+                        ]
+                    },
+                    base_key_annot + "eggnog": {
+                        "batch": False,
+                        "values": [
+                            {
+                                "id": "##UPLOADED_DATASET_ID__eggnog_{}##".format(annot.version),
+                                "src": "hda",
+                            }
+                        ]
+                    },
+                    base_key_annot + "interproscan": {
+                        "batch": False,
+                        "values": [
+                            {
+                                "id": "##UPLOADED_DATASET_ID__interpro_{}##".format(annot.version),
+                                "src": "hda",
+                            }
+                        ]
                     }
-                ]
-            },
-        })
-        exp_n += 1
+                })
+
+            exp_n = 0
+            for exp in annot.expressions:
+                file_uploads['expression_{}'.format(exp.safe_name)] = {'type': 'tsv', 'path': exp.get_input_path('table'), 'name': 'expression_{}'.format(exp.safe_name)}
+
+                base_key_exp = base_key_annot + "expression_{}|".format(exp_n)
+                annot_dict.update({
+                    base_key_exp + "public": True,
+                    base_key_exp + "counts": {
+                        "batch": False,
+                        "values": [
+                            {
+                                "id": "##UPLOADED_DATASET_ID__expression_{}##".format(exp.safe_name),  # TODO check uniqueness of safe_name
+                                "src": "hda",
+                            }
+                        ]
+                    },
+                })
+                replica_n = 0
+                for replica in exp.replicates:
+                    base_key_repl = base_key_exp + "expression_replicas_{}|".format(replica_n)
+                    annot_dict.update({
+                        base_key_repl + "replica_names": replica['name'],
+                        base_key_repl + "replicas": ",".join([str(x) for x in replica['cols']]),
+                    })
+                    replica_n += 1
+                exp_n += 1
 
-    tools_params.update(annot_dict)
-    num_annot += 1
+            tools_params.update(annot_dict)
+            num_annot += 1
 
     dest_rename = {
         'gnb_db': 'genoboo.tar.bz2'
     }
 
-    runner = bo.get_runner('galaxy', org, task_id)
     exit_code, out, err = runner.run_or_resume_job(tool=tool, params=tools_params, uploads=file_uploads, dest_rename=dest_rename, check_output=False)
 
     exit_code_all += exit_code
 
-    if (runner.task.has_run or not os.path.isfile(org.get_derived_path('build_genoboo'))) and exit_code_all == 0:
+    return exit_code_all
+
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser()
+    parser.add_argument('infile', type=str)
+    args = parser.parse_args()
+
+    bo = Beauris()
+    org = bo.load_organism(args.infile)
+
+    if not org.assemblies:
+        log.error('At least one assembly is required for Genoboo')
+        sys.exit(0)
+
+    if all([not ass.annotations for ass in org.assemblies]):
+        log.error('At least one annotation is required for Genoboo')
+        sys.exit(0)
+
+    task_id = "build_genoboo"
+    exit_code_all = 0
+
+    if not org.has_mixed_data():
+        exit_code = run_genoboo_job(org)
+        exit_code_all += exit_code
+    else:
+        purged_org = org.copy_and_purge_restricted_data()
+
+        if org:
+            exit_code = run_genoboo_job(purged_org)
+            exit_code_all += exit_code
+        else:
+            log.info("No data to deploy (nothing left after purging)")
+
+        exit_code = run_genoboo_job(org, "restricted")
+        exit_code_all += exit_code
+
+    # Check expected output: will take care of finding if restricted output is expected
+    task_id = "build_genoboo"
+    runner = bo.get_runner('galaxy', org, task_id)
+    if runner.task.has_run and exit_code_all == 0:
         exit_code_all += runner.task.check_expected_outputs()
 
     if exit_code_all != 0:
         log.error('Some {} job failed with exit code {} for {}, see log above.'.format(task_id, exit_code_all, org.slug()))
     else:
         log.info('All {} jobs succeeded for {}.'.format(task_id, org.slug()))
```

### Comparing `beauris-0.2/beauris/workflows/galaxy/jbrowse.py` & `beauris-0.3/beauris/workflows/galaxy/jbrowse.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,183 +114,240 @@
                 param_prefix + "scaling|scale_select": "auto_local",
                 param_prefix + "MultiBigWig": "false",
                 param_prefix + "track_visibility": "default_off",
                 param_prefix + "override_apollo_drag": "False",
                 param_prefix + "override_apollo_plugins": "False",
             })
 
+        elif track_type == "vcf":
+            track_params.update({
+                param_prefix + "data_format_select": "vcf",
+                param_prefix + "track_visibility": "default_off",
+                param_prefix + "override_apollo_drag": "False",
+                param_prefix + "override_apollo_plugins": "False",
+            })
+
         tool_params.update(track_params)
 
     return tool_params
 
 
-if __name__ == '__main__':
-    parser = argparse.ArgumentParser()
-    parser.add_argument('infile', type=str)
-    args = parser.parse_args()
-
-    bo = Beauris()
-    org = bo.load_organism(args.infile)
+def run_jbrowse_job(ass, access_mode="public"):
 
     task_id = "jbrowse"
+    runner = bo.get_runner('galaxy', ass, task_id, access_mode=access_mode)
 
     exit_code_all = 0
 
-    for ass in org.assemblies:
-
-        file_uploads = {}
-        file_uploads['ass_{}'.format(ass.slug(short=True))] = {'type': 'fasta', 'path': ass.get_input_path('fasta'), 'name': ass.slug(short=True)}
-
-        for annot in ass.annotations:
-            file_uploads['annot_{}'.format(annot.version)] = {'type': 'gff', 'path': annot.get_derived_path('fixed_gff'), 'name': annot.version}
+    file_uploads = {}
+    file_uploads['ass_{}'.format(ass.slug(short=True))] = {'type': 'fasta', 'path': ass.get_input_path('fasta'), 'name': ass.slug(short=True)}
 
-        for track in ass.tracks:
-            if track.input_files['track_file'].type == 'bam':
-                # TODO make this trick more documented/configurable
-                # Bam files are huge, and the galaxy tool doesn't read them much.
-                # So don't send them, send a fake tiny bam, and we'll replace it after job completion
-                fpath = os.path.join(os.path.dirname(os.path.realpath(__file__)), '../minimal.bam')
-            else:
-                fpath = track.get_input_path('track_file')
-            file_uploads['track_{}'.format(track.name)] = {'type': track.input_files['track_file'].type, 'path': fpath, 'name': track.name}
+    for annot in ass.annotations:
+        file_uploads['annot_{}'.format(annot.version)] = {'type': 'gff', 'path': annot.get_derived_path('fixed_gff'), 'name': annot.version}
 
-            if track.input_files['track_file'].type == 'bam':
-                # If it's a bam, it means we have a bigwig file too, upload a tiny fake one as we do for bams
-                wigpath = os.path.join(os.path.dirname(os.path.realpath(__file__)), '../minimal.wg')
-                file_uploads['track_wig_{}'.format(track.name)] = {'type': 'bigwig', 'path': wigpath, 'name': track.name}
-
-        # Use a precise tool version if possible
-        # tool = "JBrowse"
-        tool = "toolshed.g2.bx.psu.edu/repos/iuc/jbrowse/jbrowse/1.16.11+galaxy1"
-
-        tool_params = {
-            "action|action_select": "create",
-            "gencode": "1",
-            "jbgen|aboutDescription": "",
-            "jbgen|defaultLocation": "",
-            "jbgen|hideGenomeOptions": "false",
-            "jbgen|shareLink": "true",
-            "jbgen|show_menu": "true",
-            "jbgen|show_nav": "true",
-            "jbgen|show_overview": "true",
-            "jbgen|show_tracklist": "true",
-            "jbgen|trackPadding": 20,
-            "plugins|BlastView": "true",
-            "plugins|ComboTrackSelector": "false",
-            "plugins|GCContent": "false",
-            "reference_genome|genome": {
+    for track in ass.tracks:
+        auto_decompress = False
+        if track.input_files['track_file'].type == 'bam':
+            # TODO make this trick more documented/configurable
+            # Bam files are huge, and the galaxy tool doesn't read them much.
+            # So don't send them, send a fake tiny bam, and we'll replace it after job completion
+            fpath = os.path.join(os.path.dirname(os.path.realpath(__file__)), '../minimal.bam')
+        elif track.input_files['track_file'].type == 'vcf':
+            # Maybe we can set this up for all files. Galaxy should only extract when the file is actually an archive.
+            # Are there any files we DON'T want to extract?
+            auto_decompress = True
+            fpath = track.get_input_path('track_file')
+        else:
+            fpath = track.get_input_path('track_file')
+        file_uploads['track_{}'.format(track.name)] = {'type': track.input_files['track_file'].type, 'path': fpath, 'name': track.name, 'auto_decompress': auto_decompress}
+
+        if track.input_files['track_file'].type == 'bam':
+            # If it's a bam, it means we have a bigwig file too, upload a tiny fake one as we do for bams
+            wigpath = os.path.join(os.path.dirname(os.path.realpath(__file__)), '../minimal.wg')
+            file_uploads['track_wig_{}'.format(track.name)] = {'type': 'bigwig', 'path': wigpath, 'name': track.name, 'auto_decompress': False}
+
+    # Use a precise tool version if possible
+    # tool = "JBrowse"
+    tool = "toolshed.g2.bx.psu.edu/repos/iuc/jbrowse/jbrowse/1.16.11+galaxy1"
+
+    tool_params = {
+        "action|action_select": "create",
+        "gencode": "1",
+        "jbgen|aboutDescription": "",
+        "jbgen|defaultLocation": "",
+        "jbgen|hideGenomeOptions": "false",
+        "jbgen|shareLink": "true",
+        "jbgen|show_menu": "true",
+        "jbgen|show_nav": "true",
+        "jbgen|show_overview": "true",
+        "jbgen|show_tracklist": "true",
+        "jbgen|trackPadding": 20,
+        "plugins|BlastView": "true",
+        "plugins|ComboTrackSelector": "false",
+        "plugins|GCContent": "false",
+        "reference_genome|genome": {
+            "batch": False,
+            "values": [
+                {
+                    "id": "##UPLOADED_DATASET_ID__ass_{}##".format(ass.slug(short=True)),
+                    "src": "hda",
+                }
+            ]
+        },
+        "reference_genome|genome_type_select": "history",
+        "standalone": "minimal",
+        "track_groups_0|category": "Annotation",
+        "uglyTestingHack": ""
+    }
+
+    group_num = 0
+
+    annot_track_group = "track_groups_{}".format(group_num)
+    track_num = 0
+    for annot in ass.annotations:
+
+        param_prefix = "{}|data_tracks_{}|data_format|".format(annot_track_group, track_num)
+        track_params = {
+            param_prefix + "annotation": {
                 "batch": False,
                 "values": [
                     {
-                        "id": "##UPLOADED_DATASET_ID__ass_{}##".format(ass.slug(short=True)),
+                        "id": "##UPLOADED_DATASET_ID__annot_{}##".format(annot.version),
                         "src": "hda",
                     }
                 ]
             },
-            "reference_genome|genome_type_select": "history",
-            "standalone": "minimal",
-            "track_groups_0|category": "Annotation",
-            "uglyTestingHack": ""
+            param_prefix + "data_format_select": "gene_calls",
+            param_prefix + "index": "true",
+            param_prefix + "jbcolor_scale|color_score|color_score_select": "none",
+            param_prefix + "jbcolor_scale|color_score|color|color_select": "automatic",
+
+            param_prefix + "jbstyle|max_height": "600",
+            param_prefix + "jbstyle|style_classname": "transcript",
+            param_prefix + "jbstyle|style_description": "note,description",
+            param_prefix + "jbstyle|style_height": "10px",
+            param_prefix + "jbstyle|style_label": "product,name,id",
+            param_prefix + "match_part|match_part_select": "false",
+            param_prefix + "override_apollo_drag": "False",
+            param_prefix + "override_apollo_plugins": "False",
+            param_prefix + "track_config|html_options|topLevelFeatures": "",
+            param_prefix + "track_config|track_class": "NeatHTMLFeatures/View/Track/NeatFeatures",
+            param_prefix + "track_visibility": "default_off",
         }
 
-        group_num = 0
-
-        annot_track_group = "track_groups_{}".format(group_num)
-        track_num = 0
-        for annot in ass.annotations:
-            param_prefix = "{}|data_tracks_{}|data_format|".format(annot_track_group, track_num)
-            track_params = {
-                param_prefix + "annotation": {
-                    "batch": False,
-                    "values": [
-                        {
-                            "id": "##UPLOADED_DATASET_ID__annot_{}##".format(annot.version),
-                            "src": "hda",
-                        }
-                    ]
-                },
-                param_prefix + "data_format_select": "gene_calls",
-                param_prefix + "index": "true",
-                param_prefix + "jbcolor_scale|color_score|color_score_select": "none",
-                param_prefix + "jbcolor_scale|color_score|color|color_select": "automatic",
-
-                # param_prefix + "jbmenu|track_menu_0|menu_action": "iframeDialog",
-                # param_prefix + "jbmenu|track_menu_0|menu_icon": "dijitIconBookmark",
-                # param_prefix + "jbmenu|track_menu_0|menu_label": "View transcript report",
-                # param_prefix + "jbmenu|track_menu_0|menu_title": "Transcript {id}",
-                # param_prefix + "jbmenu|track_menu_0|menu_url": "https://bipaa.genouest.org/some/link/to/features",  # TODO make this a param
-
-                param_prefix + "jbstyle|max_height": "600",
-                param_prefix + "jbstyle|style_classname": "transcript",
-                param_prefix + "jbstyle|style_description": "note,description",
-                param_prefix + "jbstyle|style_height": "10px",
-                param_prefix + "jbstyle|style_label": "product,name,id",
-                param_prefix + "match_part|match_part_select": "false",
-                param_prefix + "override_apollo_drag": "False",
-                param_prefix + "override_apollo_plugins": "False",
-                param_prefix + "track_config|html_options|topLevelFeatures": "",
-                param_prefix + "track_config|track_class": "NeatHTMLFeatures/View/Track/NeatFeatures",
-                param_prefix + "track_visibility": "default_off",
+        menu_params = {}
+        if 'genoboo' in annot.get_deploy_services("production"):
+            gnb_url_prefix = "https://__BEAURIS_SERVICE_URL_PLACEHOLDER_genoboo__"
+            gnb_url = gnb_url_prefix + 'gene/{id}?annotation=' + annot.version
+
+            menu_params = {
+                param_prefix + "jbmenu|track_menu_0|menu_action": "iframeDialog",
+                param_prefix + "jbmenu|track_menu_0|menu_icon": "dijitIconBookmark",
+                param_prefix + "jbmenu|track_menu_0|menu_label": "View transcript report",
+                param_prefix + "jbmenu|track_menu_0|menu_title": "Transcript {id}",
+                param_prefix + "jbmenu|track_menu_0|menu_url": gnb_url,
             }
-            tool_params.update(track_params)
-            track_num += 1
 
-        tracks_by_cat = {}
-        for t in ass.tracks:
-            if t.category not in tracks_by_cat:
-                tracks_by_cat[t.category] = []
-            tracks_by_cat[t.category].append(t)
-
-        for cat in tracks_by_cat:
-            group_num += 1
-            params = add_tracks_in_category(cat, tracks_by_cat[cat], group_num)
-            tool_params.update(params)
-
-        # Add bigwig tracks for rnaseq/dnaseq
-        tracks_by_cat_wig = {}
-        for t in ass.tracks:
-            if t.type in ("rnaseq", "dnaseq"):
-                wig_cat = "{}{}".format(t.category, ass.wig_category_suffix)
-                if wig_cat not in tracks_by_cat_wig:
-                    tracks_by_cat_wig[wig_cat] = []
-
-                tracks_by_cat_wig[wig_cat].append(t)
-
-        for cat in tracks_by_cat_wig:
-            group_num += 1
-            params = add_tracks_in_category(cat, tracks_by_cat_wig[cat], group_num, upload_prefix='track_wig', track_type="wig")
-            tool_params.update(params)
+        track_params.update(menu_params)
+        tool_params.update(track_params)
+        track_num += 1
 
-        dest_rename = {
-            'output': 'jbrowse.zip'
-        }
+    tracks_by_cat = {}
+    for t in ass.tracks:
+        if t.category not in tracks_by_cat:
+            tracks_by_cat[t.category] = []
+        tracks_by_cat[t.category].append(t)
 
-        runner = bo.get_runner('galaxy', ass, task_id)
-        exit_code, out, err = runner.run_or_resume_job(tool=tool, params=tool_params, uploads=file_uploads, dest_rename=dest_rename, check_output=False)
+    for cat in tracks_by_cat:
+        group_num += 1
+        params = add_tracks_in_category(cat, tracks_by_cat[cat], group_num)
+        tool_params.update(params)
+
+    # Add bigwig tracks for rnaseq/dnaseq
+    tracks_by_cat_wig = {}
+    for t in ass.tracks:
+        if t.type in ("rnaseq", "dnaseq"):
+            wig_cat = "{}{}".format(t.category, ass.wig_category_suffix)
+            if wig_cat not in tracks_by_cat_wig:
+                tracks_by_cat_wig[wig_cat] = []
+
+            tracks_by_cat_wig[wig_cat].append(t)
+
+    for cat in tracks_by_cat_wig:
+        group_num += 1
+        params = add_tracks_in_category(cat, tracks_by_cat_wig[cat], group_num, upload_prefix='track_wig', track_type="wig")
+        tool_params.update(params)
 
-        exit_code_all += exit_code
+    dest_rename = {
+        'output': 'jbrowse.zip'
+    }
 
-        if (runner.task.has_run or not os.path.isfile(ass.get_derived_path('jbrowse'))) and exit_code_all == 0:
-            if os.path.isfile(ass.get_derived_path('jbrowse')):
-                os.remove(ass.get_derived_path('jbrowse'))
+    exit_code, out, err = runner.run_or_resume_job(tool=tool, params=tool_params, uploads=file_uploads, dest_rename=dest_rename, check_output=False)
 
-            log.info("Extracting data dir from downloaded archive + converting to tar.gz")
-            with ZipFile(os.path.join(ass.get_work_dir(), "jbrowse/jbrowse.zip")) as zipf:
+    exit_code_all += exit_code
 
-                # First find all fake files that we sent
-                with zipf.open('data/trackList.json') as trl:
-                    trl = json.load(trl)
+    if runner.task.has_run and exit_code_all == 0:
+        derived_id = 'jbrowse'
+        if access_mode != 'public':
+            derived_id += '_' + access_mode
 
-                    to_swap = ass.jbrowse_track_swapping(trl['tracks'], ass.get_track_paths())
+        if os.path.isfile(ass.get_derived_path(derived_id)):
+            os.remove(ass.get_derived_path(derived_id))
 
-                    # Using the usable path here, but for production this will be replace on-the-fly by locked path while deploying
-                    # (locked path may not be known here yet if using gopublish for example)
-                    replace_fake_files(ass.get_derived_path('2bit'), ass.get_derived_path('jbrowse'), to_swap, zipf)
+        log.info("Extracting data dir from downloaded archive + converting to tar.gz")
+        with ZipFile(os.path.join(runner.task.get_work_dir(), "jbrowse.zip")) as zipf:
+
+            # First find all fake files that we sent
+            with zipf.open('data/trackList.json') as trl:
+                trl = json.load(trl)
+
+                to_swap = ass.jbrowse_track_swapping(trl['tracks'], ass.get_track_paths())
+
+                # Using the usable path here, but for production this will be replace on-the-fly by locked path while deploying
+                # (locked path may not be known here yet if using gopublish for example)
+                replace_fake_files(ass.get_derived_path('2bit'), ass.get_derived_path(derived_id), to_swap, zipf)
+
+        # Output checking is delayed as we post process the result locally
+
+    return exit_code_all
+
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser()
+    parser.add_argument('infile', type=str)
+    args = parser.parse_args()
+
+    bo = Beauris()
+    org = bo.load_organism(args.infile)
+
+    task_id = "jbrowse"
+
+    exit_code_all = 0
+
+    for ass in org.assemblies:
+
+        if not ass.has_mixed_data():
+            exit_code = run_jbrowse_job(ass)
+            exit_code_all += exit_code
+        else:
+            purged_ass = ass.copy_and_purge_restricted_data()
+
+            if ass:
+                exit_code = run_jbrowse_job(purged_ass)
+                exit_code_all += exit_code
+            else:
+                log.info("No data to deploy (nothing left after purging)")
+
+            exit_code = run_jbrowse_job(ass, "restricted")
+            exit_code_all += exit_code
+
+        task_id = "jbrowse"
+        runner = bo.get_runner('galaxy', ass, task_id)
 
-            # Output checking is delayed as we post process the result locally
+        if runner.task.has_run and exit_code_all == 0:
 
             exit_code_all += runner.task.check_expected_outputs()
 
     if exit_code_all != 0:
         log.error('Some {} job failed with exit code {} for {}, see log above.'.format(task_id, exit_code_all, org.slug()))
     else:
         log.info('All {} jobs succeeded for {}.'.format(task_id, org.slug()))
```

### Comparing `beauris-0.2/beauris/workflows/local/apollo_deploy.py` & `beauris-0.3/beauris/workflows/local/apollo_deploy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python
 
 # Send an organism archive to a remote Apollo server
 
 import argparse
+import io
 import json
 import logging
 import os
 import sys
 import tarfile
 
 from beauris import Beauris
 
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger()
 
 
-def fix_track_paths(intarf, output, to_swap):
+def fix_track_paths(intarf, output, to_swap, entity, server):
 
     with tarfile.open(output, 'w:gz') as tarf:
         for member in intarf.getmembers():
             if member.name in to_swap:
                 log.info("Replacing archive file {} by symlink to {}".format(member.name, to_swap[member.name]))
                 # Creating a new TarInfo object to avoid strange bug when replacing a symlink by a new one
                 new_member = tarfile.TarInfo(name=member.name)
@@ -27,17 +28,43 @@
                 new_member.linkname = to_swap[member.name]
                 new_member.size = 0
                 new_member.mode = member.mode
                 new_member.mtime = member.mtime
                 tarf.addfile(
                     tarinfo=new_member
                 )
+            elif member.name == "trackList.json":
+                # Edit service urls on the fly
+                tl_content = intarf.extractfile(member).read().decode()
+
+                for service_name in entity.get_deploy_services(server):
+                    placeholder = f"https://__BEAURIS_SERVICE_URL_PLACEHOLDER_{service_name}__"
+
+                    url_needs_restricted = entity.organism.has_mixed_data() and entity.is_restricted()
+                    good_url = entity.config.get_service_url(service_name, server, entity.organism, restricted=url_needs_restricted)
+
+                    tl_content = tl_content.replace(placeholder, good_url)
+
+                tl_content = tl_content.encode('utf8')
+                member.size = len(tl_content)
+                tarf.addfile(member, io.BytesIO(tl_content))
             elif (member.isdir() or member.isfile()) and not member.issym():
                 extracted = intarf.extractfile(member)
                 tarf.addfile(member, extracted)
+            elif member.issym():
+                # symlink not in the to_swap dict => copy as is
+                new_member = tarfile.TarInfo(name=member.name)
+                new_member.type = tarfile.SYMTYPE
+                new_member.linkname = member.linkname
+                new_member.size = 0
+                new_member.mode = member.mode
+                new_member.mtime = member.mtime
+                tarf.addfile(
+                    tarinfo=new_member
+                )
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     parser.add_argument('server', type=str)
     parser.add_argument('infile', type=str)
     args = parser.parse_args()
@@ -67,32 +94,43 @@
 
         common_name = ass.organism.pretty_name()
         common_name += " {}".format(ass.version)
 
         runner = bo.get_runner('local', ass, task_id)
 
         # TODO Maybe task depends_on should be defined in beauris.tasks?
-        deps = [ass.derived_files['jbrowse']]
+
+        # Mixed data at assembly level? add only the restricted version (we'll do the same in apollo_perms)
+        # TODO make this configurable for other user cases?
+        jb_dataset = 'jbrowse'
+        if ass.has_mixed_data():
+            jb_dataset = 'jbrowse_restricted'
+
+        deps = [ass.derived_files[jb_dataset]]
         runner.task.depends_on = deps
 
-        jbrowse_arch_path = ass.get_derived_path('jbrowse')
-        if args.server == "production" and runner.task.needs_to_run() and not runner.task.disable_run():
+        jbrowse_arch_path = ass.get_derived_path(jb_dataset)
+        if runner.task.needs_to_run() and not runner.task.disable_run():
 
             # We need to edit the tar.gz archive because locked paths are only accessible after merging
-            log.info("Editing jbrowse tar.gz on the fly to use correct track file paths")
+            log.info("Editing jbrowse tar.gz on the fly to use correct track file paths and contextual menu urls")
 
-            with tarfile.open(ass.get_derived_path('jbrowse'), 'r:gz') as intarf:
+            with tarfile.open(ass.get_derived_path(jb_dataset), 'r:gz') as intarf:
 
                 # First find all bam files that we need to replace by proper symlinks
                 trackl = intarf.extractfile(intarf.getmember('trackList.json'))
                 trl = json.load(trackl)
-                to_swap = ass.jbrowse_track_swapping(trl['tracks'], ass.get_track_paths(prefer='locked'))
+
+                to_swap = {}  # In staging mode, no need to swap track paths (but still need to adapt menu urls)
+                if args.server == "production":
+                    to_swap = ass.jbrowse_track_swapping(trl['tracks'], ass.get_track_paths(prefer='locked'))
 
                 jbrowse_arch_path = "{}/jbrowse/jbrowse_fix_apollo_{}.tar.gz".format(ass.get_work_dir(), args.server)
-                fix_track_paths(intarf, jbrowse_arch_path, to_swap)
+
+                fix_track_paths(intarf, jbrowse_arch_path, to_swap, ass, args.server)
 
         log.info("Running create or update organism in Apollo for {}".format(jbrowse_arch_path))
 
         # Run in a subprocess to capture stdout/stderr + exit code
         cmd = ["python", "{}/run_apollo.py".format(script_dir), '--update']
         cmd += [jbrowse_arch_path, common_name, genus, species, bo.config.raw['apollo'][args.server]['url'], bo.config.raw['apollo'][args.server]['user'], bo.config.raw['apollo'][args.server]['password']]
```

### Comparing `beauris-0.2/beauris/workflows/local/assembly_check.py` & `beauris-0.3/beauris/workflows/local/assembly_check.py`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/workflows/local/build_elasticsearch.py` & `beauris-0.3/beauris/workflows/local/build_elasticsearch.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     exit_code = 0
     log.info("Running build elasticsearch for {}".format(org.pretty_name()))
 
     # Run in a subprocess to capture stdout/stderr + exit code
     cmd = ["python", "{}/run_build_elasticsearch.py".format(script_dir), args.infile]
     exit_code, out, err = runner.run_or_resume_job(cmd=cmd)
 
-    if (runner.task.has_run or not os.path.isfile(org.get_derived_path('build_elasticsearch'))) and exit_code == 0:
+    if runner.task.has_run and exit_code == 0:
         exit_code += runner.task.check_expected_outputs()
 
     if exit_code != 0:
         log.error('Some {} job failed with exit code {} for {}, see log above.'.format(task_id, exit_code, org.slug()))
     else:
         log.info('All {} jobs succeeded for {}.'.format(task_id, org.slug()))
```

### Comparing `beauris-0.2/beauris/workflows/local/deploy_blast.py` & `beauris-0.3/beauris/workflows/local/deploy_blast.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import argparse
 import logging
 import sys
 
 
 from beauris import Beauris
-from beauris.web_interface import WebInterface
 
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger()
 
 
 def main():
 
@@ -23,15 +22,15 @@
 
     if not bo.config.raw['deploy']['deploy_interface']:
         log.info("Skipping docker setup")
         sys.exit(0)
 
     org = bo.load_organism(args.infile)
 
-    web_interface = WebInterface(org, bo.config, args.server)
+    deployer = bo.get_deployer('blast', args.server, org)
 
     log.info("Setting up blast")
-    web_interface.write_blast_files()
+    deployer.write_data()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `beauris-0.2/beauris/workflows/local/deploy_download.py` & `beauris-0.3/beauris/workflows/local/deploy_authelia.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import argparse
 import logging
 import sys
 
 
 from beauris import Beauris
-from beauris.web_interface import WebInterface
 
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger()
 
 
 def main():
 
@@ -23,20 +22,15 @@
 
     if not bo.config.raw['deploy']['deploy_interface']:
         log.info("Skipping docker setup")
         sys.exit(0)
 
     org = bo.load_organism(args.infile)
 
-    web_interface = WebInterface(org, bo.config, args.server)
+    deployer = bo.get_deployer('authelia', args.server, org)
 
-    deploy_download = 'download' in org.get_deploy_services(args.server)
-
-    if deploy_download:
-        log.info("Setting up download symlinks")
-        web_interface.prepare_download()
-    else:
-        log.info("Skipping download setup")
+    log.info("Setting up access permissions")
+    deployer.write_data()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `beauris-0.2/beauris/workflows/local/deploy_perms.py` & `beauris-0.3/beauris/workflows/local/track_check_gff.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 #!/usr/bin/env python
 
+# Check that a bam file is ready for release
+
 import argparse
 import logging
 import sys
 
+from BCBio import GFF
+
+from Bio import SeqIO
 
-from beauris import Beauris
-from beauris.web_interface import WebInterface
 
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger()
 
 
-def main():
-
+if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    parser.add_argument('server', type=str)
-    parser.add_argument('infile', type=str)
+    parser.add_argument('gfffile', type=str)
+    parser.add_argument('genome', type=str)
     args = parser.parse_args()
 
-    bo = Beauris()
-
-    if not bo.config.raw['deploy']['deploy_interface']:
-        log.info("Skipping docker setup")
-        sys.exit(0)
+    log.info("Checking gff {} against genome {}".format(args.gfffile, args.genome))
 
-    org = bo.load_organism(args.infile)
+    fa_seqs = [r.id for r in SeqIO.parse(args.genome, "fasta")]
+    gff_seqs = [r.id for r in GFF.parse(args.gfffile)]
 
-    web_interface = WebInterface(org, bo.config, args.server)
-
-    log.info("Setting up access permissions")
-    web_interface.manage_permissions()
-
-
-if __name__ == '__main__':
-    main()
+    for gffs in gff_seqs:
+        if gffs not in fa_seqs:
+            log.error("Found unexpected scaffold '{}' in gff file".format(gffs))
+            sys.exit(1)
+
+    # We could do more checks but
+    #  1) we need to accept gff taht are not as standard as an OGS gff
+    #  2) GFF.parse will detect obvious problems
```

### Comparing `beauris-0.2/beauris/workflows/local/lock.py` & `beauris-0.3/beauris/workflows/local/lock.py`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/workflows/local/ogs_check.py` & `beauris-0.3/beauris/workflows/local/ogs_check.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,14 +99,16 @@
             if 'source' in options and options['source']:
                 cmd_options.append("--source")
                 cmd_options.append(options['source'])
             if 'no_size' in options:
                 cmd_options.append("--no-size")
             if 'exons_are_cds' in options:
                 cmd_options.append("--exons-are-cds")
+            if 'extend_parent' in options:
+                cmd_options.append("--extend-parent")
 
             # Run in a subprocess to capture stdout/stderr + exit code
             cmd = ["python",
                    "{}/ogs_check.py".format(script_dir)]
             cmd += cmd_options
             cmd += [annot.get_input_path('gff'),
                     ass.get_input_path('fasta'),
```

### Comparing `beauris-0.2/beauris/workflows/local/prepare_workdir.py` & `beauris-0.3/beauris/workflows/local/prepare_workdir.py`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/workflows/local/run_apollo.py` & `beauris-0.3/beauris/workflows/local/run_apollo.py`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/workflows/local/run_apollo_perms.py` & `beauris-0.3/beauris/workflows/local/run_apollo_perms.py`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/workflows/local/run_build_elasticsearch.py` & `beauris-0.3/beauris/workflows/local/run_build_elasticsearch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 import argparse
 import logging
 import sys
 import tarfile
+import time
 
 from beauris import Beauris
 from beauris.es_parsers import DiamondParser, EggnogParser, GffParser, InterproParser
 
 from elasticsearch import Elasticsearch
 from elasticsearch.helpers import bulk
 
@@ -41,15 +42,15 @@
     mapping = {
         "properties": {
             "gene_id": {"type": "text", "analyzer": "standard"},
             "organism": {"type": "text", "analyzer": "standard"},
             "organism_slug": {"enabled": False},
             "assembly": {"enabled": False},
             "assembly_slug": {"enabled": False},
-            "annotation": {"enabled": False},
+            "annotation": {"type": "text", "analyzer": "keyword"},
             "eggnog_og_terms": {"type": "text", "analyzer": "standard"},
             "go_ids": {"type": "text", "analyzer": "standard"},
             "go_terms": {"type": "text", "analyzer": "standard"},
             "interpro_ids": {"type": "text", "analyzer": "standard"},
             "interpro_terms": {"type": "text", "analyzer": "standard"},
             "diamond_ids": {"type": "text", "analyzer": "standard"},
             "diamond_terms": {"type": "text", "analyzer": "standard"},
@@ -74,22 +75,25 @@
     re_protein_capture = config_task.get("re_protein_capture", r"^(.*?)-R([A-Z]+)$")
     go_file = config_task.get("goterms_file")
     to_index = config_task.get("to_index", [])
 
     es_url = "http://localhost:9200"
     es = Elasticsearch(es_url)
 
+    # Try to delete the indice beforehand, just in case it's a multiple organisms job
+    es.indices.delete(index="genes", ignore_unavailable=True)
+
     es.indices.create(index="genes", mappings=mapping)
 
     # Check if org is public
-    is_public = not bool(org.restricted_to)
     slug = org.slug()
 
     for ass in org.assemblies:
         for annot in ass.annotations:
+            is_public = not bool(annot.restricted_to)
             data = GffParser(annot, re_protein=re_protein, re_protein_capture=re_protein_capture, is_public=is_public, slug=slug).parse()
             log.info("Number of genes indexed: " + str(len(data)))
             if 'interpro' in to_index:
                 log.info("Parsing interproscan")
                 data = InterproParser(annot, data).parse()
             if 'diamond' in to_index:
                 log.info("Parsing diamond")
@@ -99,9 +103,12 @@
                 data = EggnogParser(annot, data, go_file).parse()
 
             bulk(es, data_generator(data), refresh='wait_for')
 
     data_path = "/usr/share/elasticsearch/data/"
     archive_path = org.get_derived_path('build_elasticsearch')
 
+    # Wait a bit before creating the archive
+    time.sleep(20)
+
     with tarfile.open(archive_path, 'w:bz2') as outtarf:
         outtarf.add(data_path, arcname="data")
```

### Comparing `beauris-0.2/beauris/workflows/local/track_check.py` & `beauris-0.3/beauris/workflows/local/track_check.py`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/workflows/local/track_check_bam.py` & `beauris-0.3/beauris/workflows/local/track_check_bam.py`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris/workflows/minimal.wg` & `beauris-0.3/beauris/workflows/minimal.wg`

 * *Files identical despite different names*

### Comparing `beauris-0.2/beauris.egg-info/PKG-INFO` & `beauris-0.3/beauris.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beauris
-Version: 0.2
+Version: 0.3
 Summary: BEAURIS: an automated system for the creation of genome portals
 Home-page: https://gitlab.com/beaur1s/beauris
 Author: BEAURIS team
 Author-email: gogepp@inrae.fr
 License: MIT
 Platform: Posix
 Classifier: Development Status :: 4 - Beta
```

### Comparing `beauris-0.2/beauris.egg-info/SOURCES.txt` & `beauris-0.3/beauris.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,41 @@
 beauris/annotation.py
 beauris/assembly.py
 beauris/beauris.py
 beauris/blastbank.py
 beauris/config.py
 beauris/data_locker.py
 beauris/expression_data.py
+beauris/extra_file.py
 beauris/job_runner.py
 beauris/managed_entity.py
 beauris/managed_file.py
+beauris/mr_bot.py
 beauris/organism.py
 beauris/proteome.py
 beauris/task.py
 beauris/track.py
 beauris/transcriptome.py
 beauris/util.py
-beauris/web_interface.py
 beauris.egg-info/PKG-INFO
 beauris.egg-info/SOURCES.txt
 beauris.egg-info/dependency_links.txt
 beauris.egg-info/requires.txt
 beauris.egg-info/top_level.txt
+beauris/deployers/__init__.py
+beauris/deployers/authelia.py
+beauris/deployers/basedeployer.py
+beauris/deployers/blast.py
+beauris/deployers/deployers.py
+beauris/deployers/dockercompose.py
+beauris/deployers/download.py
+beauris/deployers/elasticsearch.py
+beauris/deployers/genoboo.py
+beauris/deployers/genomehomepage.py
+beauris/deployers/jbrowse.py
 beauris/es_parsers/__init__.py
 beauris/es_parsers/diamond_parser.py
 beauris/es_parsers/eggnog_parser.py
 beauris/es_parsers/gff_parser.py
 beauris/es_parsers/interpro_parser.py
 beauris/tasks/__init__.py
 beauris/tasks/annotation.py
@@ -52,14 +64,15 @@
 beauris/workflows/ansible/ansible_data/project/playbook_shutdown.yml
 beauris/workflows/ansible/ansible_data/project/playbook_update.yml
 beauris/workflows/ansible/docker_files/postgres-blast-entrypoint.sh
 beauris/workflows/ansible/templates/default.conf.j2
 beauris/workflows/ansible/templates/docker-compose.yml.j2
 beauris/workflows/ansible/templates/genoboo.json.j2
 beauris/workflows/ansible/templates/web/index.html.j2
+beauris/workflows/ansible/templates/web/search.html.j2
 beauris/workflows/drmaa/__init__.py
 beauris/workflows/drmaa/add_fa_description.py
 beauris/workflows/drmaa/add_gff_description.py
 beauris/workflows/drmaa/bam_to_wig.py
 beauris/workflows/drmaa/bam_to_wig.sh
 beauris/workflows/drmaa/blastdb.py
 beauris/workflows/drmaa/blastdb.sh
@@ -79,28 +92,30 @@
 beauris/workflows/galaxy/jbrowse.py
 beauris/workflows/local/__init__.py
 beauris/workflows/local/apollo_deploy.py
 beauris/workflows/local/apollo_perms.py
 beauris/workflows/local/assembly_check.py
 beauris/workflows/local/build_elasticsearch.py
 beauris/workflows/local/check_yml.py
+beauris/workflows/local/deploy_all.py
+beauris/workflows/local/deploy_authelia.py
 beauris/workflows/local/deploy_blast.py
 beauris/workflows/local/deploy_download.py
 beauris/workflows/local/deploy_elasticsearch.py
 beauris/workflows/local/deploy_genoboo.py
 beauris/workflows/local/deploy_jbrowse.py
-beauris/workflows/local/deploy_perms.py
-beauris/workflows/local/interface_setup.py
 beauris/workflows/local/lock.py
 beauris/workflows/local/ogs_check.py
 beauris/workflows/local/prepare_workdir.py
 beauris/workflows/local/run_apollo.py
 beauris/workflows/local/run_apollo_perms.py
 beauris/workflows/local/run_build_elasticsearch.py
 beauris/workflows/local/track_check.py
 beauris/workflows/local/track_check_bam.py
 beauris/workflows/local/track_check_gff.py
+beauris/workflows/local/track_check_vcf.py
 scripts/beauris_check_env
+scripts/beauris_clean_workdir
 scripts/beauris_commit_lockfiles
 scripts/beauris_diff_lockfiles
 scripts/beauris_fetch_locked_artifacts
 scripts/beauris_run_on_touched_orgs
```

### Comparing `beauris-0.2/scripts/beauris_check_env` & `beauris-0.3/scripts/beauris_check_env`

 * *Files identical despite different names*

### Comparing `beauris-0.2/scripts/beauris_commit_lockfiles` & `beauris-0.3/scripts/beauris_commit_lockfiles`

 * *Files identical despite different names*

### Comparing `beauris-0.2/scripts/beauris_run_on_touched_orgs` & `beauris-0.3/scripts/beauris_run_on_touched_orgs`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 set -eo pipefail
 
 if [ -z "$CI_MERGE_REQUEST_TARGET_BRANCH_NAME" ]
 then
     DIFF_RANGE="${CI_COMMIT_BEFORE_SHA}...${CI_COMMIT_SHA}"
 else
-    DIFF_RANGE="origin/${CI_MERGE_REQUEST_TARGET_BRANCH_NAME} origin/${CI_MERGE_REQUEST_SOURCE_BRANCH_NAME}"
+    DIFF_RANGE="origin/${CI_MERGE_REQUEST_TARGET_BRANCH_NAME}...origin/${CI_MERGE_REQUEST_SOURCE_BRANCH_NAME}"
 fi
 
 for org_yml in `git diff --diff-filter=ACMT --name-only ${DIFF_RANGE} | ( grep "^organisms/.*\.ya\?ml" )`; do
     cmd=`echo "$@" | sed "s|ORG_YML|$org_yml|"`
     echo "Running (as $RUN_USER): $cmd"
     su -c "$cmd" $RUN_USER
 done
```

### Comparing `beauris-0.2/setup.py` & `beauris-0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('requirements.txt') as f:
     requires = f.read().splitlines()
 
 setup(
     name="beauris",
-    version='0.2',
+    version='0.3',
     description="BEAURIS: an automated system for the creation of genome portals",
     author="BEAURIS team",
     author_email="gogepp@inrae.fr",
     url="https://gitlab.com/beaur1s/beauris",
     install_requires=requires,
     packages=find_packages(exclude=['*tests*']),
     license='MIT',
@@ -21,14 +21,15 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering",
         "Programming Language :: Python :: 3.9",
     ],
     scripts=[
         'scripts/beauris_check_env',
+        'scripts/beauris_clean_workdir',
         'scripts/beauris_commit_lockfiles',
         'scripts/beauris_diff_lockfiles',
         'scripts/beauris_run_on_touched_orgs',
         'scripts/beauris_fetch_locked_artifacts',
     ],
     include_package_data=True,
     package_data={
```

