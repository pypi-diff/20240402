# Comparing `tmp/dask-kubernetes-2024.3.1.tar.gz` & `tmp/dask-kubernetes-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-kubernetes-2024.3.1.tar", last modified: Tue Mar  5 12:13:28 2024, max compression
+gzip compressed data, was "dask-kubernetes-2024.4.0.tar", last modified: Tue Apr  2 13:09:22 2024, max compression
```

## Comparing `dask-kubernetes-2024.3.1.tar` & `dask-kubernetes-2024.4.0.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.738922 dask-kubernetes-2024.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-03-05 12:13:28.738922 dask-kubernetes-2024.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.726922 dask-kubernetes-2024.3.1/dask_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-05 12:13:28.738922 dask-kubernetes-2024.3.1/dask_kubernetes/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.730922 dask-kubernetes-2024.3.1/dask_kubernetes/classic/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/classic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28855 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/classic/kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.730922 dask-kubernetes-2024.3.1/dask_kubernetes/classic/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/classic/tests/config-demo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/classic/tests/fake_gcp_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    28464 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/classic/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (127)    15181 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/classic/tests/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.730922 dask-kubernetes-2024.3.1/dask_kubernetes/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.730922 dask-kubernetes-2024.3.1/dask_kubernetes/common/
--rw-r--r--   0 runner    (1001) docker     (127)    16674 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/common/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/common/networking.py
--rw-r--r--   0 runner    (1001) docker     (127)    13351 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/common/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.730922 dask-kubernetes-2024.3.1/dask_kubernetes/common/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/common/tests/test_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/common/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.730922 dask-kubernetes-2024.3.1/dask_kubernetes/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.730922 dask-kubernetes-2024.3.1/dask_kubernetes/helm/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/helm/helmcluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.730922 dask-kubernetes-2024.3.1/dask_kubernetes/helm/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.730922 dask-kubernetes-2024.3.1/dask_kubernetes/helm/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/helm/tests/resources/values.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/helm/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/kubernetes.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.730922 dask-kubernetes-2024.3.1/dask_kubernetes/operator/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.730922 dask-kubernetes-2024.3.1/dask_kubernetes/operator/controller/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29651 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/controller/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.734922 dask-kubernetes-2024.3.1/dask_kubernetes/operator/controller/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/controller/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.734922 dask-kubernetes-2024.3.1/dask_kubernetes/operator/controller/plugins/noop/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/controller/plugins/noop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/controller/plugins/noop/noop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.734922 dask-kubernetes-2024.3.1/dask_kubernetes/operator/controller/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.734922 dask-kubernetes-2024.3.1/dask_kubernetes/operator/controller/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    28588 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/controller/tests/test_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.734922 dask-kubernetes-2024.3.1/dask_kubernetes/operator/customresources/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/customresources/daskautoscaler.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/customresources/daskautoscaler.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/customresources/daskcluster.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/customresources/daskcluster.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/customresources/daskjob.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/customresources/daskjob.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/customresources/daskworkergroup.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/customresources/daskworkergroup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/customresources/templates.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.726922 dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.734922 dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/chartpress.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.734922 dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.738922 dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   283847 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   471240 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   140704 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.738922 dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/rolebinding.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/serviceaccount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.738922 dask-kubernetes-2024.3.1/dask_kubernetes/operator/kubecluster/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/kubecluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/kubecluster/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    37802 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/kubecluster/kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.738922 dask-kubernetes-2024.3.1/dask_kubernetes/operator/kubecluster/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/kubecluster/tests/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/dask_kubernetes/operator/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 12:13:28.730922 dask-kubernetes-2024.3.1/dask_kubernetes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-03-05 12:13:28.000000 dask-kubernetes-2024.3.1/dask_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-03-05 12:13:28.000000 dask-kubernetes-2024.3.1/dask_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 12:13:28.000000 dask-kubernetes-2024.3.1/dask_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-05 12:13:28.000000 dask-kubernetes-2024.3.1/dask_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 12:13:28.000000 dask-kubernetes-2024.3.1/dask_kubernetes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-05 12:13:28.000000 dask-kubernetes-2024.3.1/dask_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-05 12:13:28.000000 dask-kubernetes-2024.3.1/dask_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-03-05 12:13:28.738922 dask-kubernetes-2024.3.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1033 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-03-05 12:13:16.000000 dask-kubernetes-2024.3.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.008818 dask-kubernetes-2024.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-02 13:09:22.012817 dask-kubernetes-2024.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:21.996817 dask-kubernetes-2024.4.0/dask_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-02 13:09:22.012817 dask-kubernetes-2024.4.0/dask_kubernetes/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.000818 dask-kubernetes-2024.4.0/dask_kubernetes/classic/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/classic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28855 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/classic/kubecluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.000818 dask-kubernetes-2024.4.0/dask_kubernetes/classic/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/classic/tests/config-demo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/classic/tests/fake_gcp_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28464 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/classic/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15181 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/classic/tests/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.000818 dask-kubernetes-2024.4.0/dask_kubernetes/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.000818 dask-kubernetes-2024.4.0/dask_kubernetes/common/
+-rw-r--r--   0 runner    (1001) docker     (127)    16674 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/common/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/common/networking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13351 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/common/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.000818 dask-kubernetes-2024.4.0/dask_kubernetes/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/common/tests/test_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/common/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.000818 dask-kubernetes-2024.4.0/dask_kubernetes/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.000818 dask-kubernetes-2024.4.0/dask_kubernetes/helm/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/helm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/helm/helmcluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.000818 dask-kubernetes-2024.4.0/dask_kubernetes/helm/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.000818 dask-kubernetes-2024.4.0/dask_kubernetes/helm/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/helm/tests/resources/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/helm/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/kubernetes.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.004818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.004818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29927 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.004818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.004818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/plugins/noop/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/plugins/noop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/plugins/noop/noop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.004818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.004818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    30973 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/test_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.004818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskautoscaler.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskautoscaler.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskcluster.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskcluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskjob.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskworkergroup.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskworkergroup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/templates.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:21.996817 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.004818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/chartpress.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.004818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.008818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   283847 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   471240 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   140704 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.008818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/rolebinding.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/serviceaccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.008818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/kubecluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/kubecluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/kubecluster/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37802 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/kubecluster/kubecluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.008818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/kubecluster/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/kubecluster/tests/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.000818 dask-kubernetes-2024.4.0/dask_kubernetes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-02 13:09:21.000000 dask-kubernetes-2024.4.0/dask_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-02 13:09:21.000000 dask-kubernetes-2024.4.0/dask_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:09:21.000000 dask-kubernetes-2024.4.0/dask_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 13:09:21.000000 dask-kubernetes-2024.4.0/dask_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:09:21.000000 dask-kubernetes-2024.4.0/dask_kubernetes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-02 13:09:21.000000 dask-kubernetes-2024.4.0/dask_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 13:09:21.000000 dask-kubernetes-2024.4.0/dask_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-02 13:09:22.012817 dask-kubernetes-2024.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1033 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/versioneer.py
```

### Comparing `dask-kubernetes-2024.3.1/LICENSE` & `dask-kubernetes-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/PKG-INFO` & `dask-kubernetes-2024.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-kubernetes
-Version: 2024.3.1
+Version: 2024.4.0
 Summary: Native Kubernetes integration for Dask
 Home-page: https://github.com/dask/dask-kubernetes
 Maintainer: Jacob Tomlinson
 License: BSD
 Keywords: dask,kubernetes,distributed
 Requires-Python: >=3.9
 License-File: LICENSE
```

### Comparing `dask-kubernetes-2024.3.1/README.rst` & `dask-kubernetes-2024.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/__init__.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/classic/kubecluster.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/classic/kubecluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/classic/tests/config-demo.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/classic/tests/config-demo.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/classic/tests/test_async.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/classic/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/classic/tests/test_sync.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/classic/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/cli/cli.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/cli/cli.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/common/auth.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/common/auth.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/common/networking.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/common/networking.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/common/objects.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/common/objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/common/tests/test_kind.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/common/tests/test_kind.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/common/tests/test_objects.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/common/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/common/utils.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/common/utils.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/conftest.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/conftest.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/experimental/__init__.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/helm/helmcluster.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/helm/helmcluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/helm/tests/test_helm.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/helm/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/kubernetes.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/kubernetes.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/_objects.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/_objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/controller/controller.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,29 +149,33 @@
     }
     deployment_spec = {
         "apiVersion": "apps/v1",
         "kind": "Deployment",
         "metadata": metadata,
         "spec": spec,
     }
-    env = [
-        {
-            "name": "DASK_WORKER_NAME",
-            "value": worker_name,
-        },
-        {
-            "name": "DASK_SCHEDULER_ADDRESS",
-            "value": f"tcp://{cluster_name}-scheduler.{namespace}.svc.cluster.local:8786",
-        },
-    ]
+    worker_env = {
+        "name": "DASK_WORKER_NAME",
+        "value": worker_name,
+    }
+    scheduler_env = {
+        "name": "DASK_SCHEDULER_ADDRESS",
+        "value": f"tcp://{cluster_name}-scheduler.{namespace}.svc.cluster.local:8786",
+    }
     for container in deployment_spec["spec"]["template"]["spec"]["containers"]:
-        if "env" in container:
-            container["env"].extend(env)
-        else:
-            container["env"] = env
+        if "env" not in container:
+            container["env"] = [worker_env, scheduler_env]
+            continue
+
+        container_env_names = [env_item["name"] for env_item in container["env"]]
+
+        if "DASK_WORKER_NAME" not in container_env_names:
+            container["env"].append(worker_env)
+        if "DASK_SCHEDULER_ADDRESS" not in container_env_names:
+            container["env"].append(scheduler_env)
     return deployment_spec
 
 
 def get_job_runner_pod_name(job_name):
     return f"{job_name}-runner"
```

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 apiVersion: kubernetes.dask.org/v1
 kind: DaskWorkerGroup
 metadata:
   name: simple-additional
 spec:
   cluster: simple
   worker:
-    replicas: 2
+    replicas: 1
     spec:
       containers:
         - name: worker
           image: "dask-kubernetes:dev"
           imagePullPolicy: "IfNotPresent"
           args:
             - dask-worker
@@ -19,7 +19,9 @@
           ports:
             - name: http-dashboard
               containerPort: 8788
               protocol: TCP
           env:
             - name: WORKER_ENV
               value: hello-world # We dont test the value, just the name
+            - name: DASK_WORKER_NAME
+              value: test-worker
```

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/controller/tests/test_controller.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/test_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from dask_kubernetes.operator.controller import (
     KUBERNETES_DATETIME_FORMAT,
     get_job_runner_pod_name,
 )
 
 DIR = pathlib.Path(__file__).parent.absolute()
 
-
 _EXPECTED_ANNOTATIONS = {"test-annotation": "annotation-value"}
 _EXPECTED_LABELS = {"test-label": "label-value"}
 DEFAULT_CLUSTER_NAME = "simple"
 
 
 @pytest.fixture()
 def gen_cluster_manifest(tmp_path):
@@ -43,15 +42,14 @@
 
 @pytest.fixture()
 def gen_cluster(k8s_cluster, ns, gen_cluster_manifest):
     """Yields an instantiated context manager for creating/deleting a simple cluster."""
 
     @asynccontextmanager
     async def cm(cluster_name=DEFAULT_CLUSTER_NAME):
-
         cluster_path = gen_cluster_manifest(cluster_name)
         # Create cluster resource
         k8s_cluster.kubectl("apply", "-n", ns, "-f", cluster_path)
         while cluster_name not in k8s_cluster.kubectl(
             "get", "daskclusters.kubernetes.dask.org", "-n", ns
         ):
             await asyncio.sleep(0.1)
@@ -91,14 +89,44 @@
                 "get", "daskjobs.kubernetes.dask.org", "-n", ns
             ):
                 await asyncio.sleep(0.1)
 
     yield cm
 
 
+@pytest.fixture()
+def gen_worker_group(k8s_cluster, ns):
+    """Yields an instantiated context manager for creating/deleting a worker group."""
+
+    @asynccontextmanager
+    async def cm(worker_group_file):
+        worker_group_path = os.path.join(DIR, "resources", worker_group_file)
+        with open(worker_group_path) as f:
+            worker_group_name = yaml.load(f, yaml.Loader)["metadata"]["name"]
+
+        # Create cluster resource
+        k8s_cluster.kubectl("apply", "-n", ns, "-f", worker_group_path)
+        while worker_group_name not in k8s_cluster.kubectl(
+            "get", "daskworkergroups.kubernetes.dask.org", "-n", ns
+        ):
+            await asyncio.sleep(0.1)
+
+        try:
+            yield worker_group_name, ns
+        finally:
+            # Test: remove the wait=True, because I think this is blocking the operator
+            k8s_cluster.kubectl("delete", "-n", ns, "-f", worker_group_path)
+            while worker_group_name in k8s_cluster.kubectl(
+                "get", "daskworkergroups.kubernetes.dask.org", "-n", ns
+            ):
+                await asyncio.sleep(0.1)
+
+    yield cm
+
+
 def test_customresources(k8s_cluster):
     assert "daskclusters.kubernetes.dask.org" in k8s_cluster.kubectl("get", "crd")
     assert "daskworkergroups.kubernetes.dask.org" in k8s_cluster.kubectl("get", "crd")
     assert "daskjobs.kubernetes.dask.org" in k8s_cluster.kubectl("get", "crd")
 
 
 def test_operator_runs(kopf_runner):
@@ -667,40 +695,67 @@
             assert isinstance(scheduler_deployment, Deployment)
 
             scheduler_service = await cluster.scheduler_service()
             assert isinstance(scheduler_service, Service)
 
 
 @pytest.mark.anyio
-async def test_object_dask_worker_group(k8s_cluster, kopf_runner, gen_cluster):
+async def test_object_dask_worker_group(
+    k8s_cluster, kopf_runner, gen_cluster, gen_worker_group
+):
     with kopf_runner:
-        async with gen_cluster() as (cluster_name, ns):
+        async with (
+            gen_cluster() as (cluster_name, ns),
+            gen_worker_group("simpleworkergroup.yaml") as (
+                additional_workergroup_name,
+                _,
+            ),
+        ):
             cluster = await DaskCluster.get(cluster_name, namespace=ns)
+            additional_workergroup = await DaskWorkerGroup.get(
+                additional_workergroup_name, namespace=ns
+            )
 
             worker_groups = []
             while not worker_groups:
                 worker_groups = await cluster.worker_groups()
                 await asyncio.sleep(0.1)
             assert len(worker_groups) == 1  # Just the default worker group
-            wg = worker_groups[0]
-            assert isinstance(wg, DaskWorkerGroup)
+            worker_groups = worker_groups + [additional_workergroup]
 
-            pods = []
-            while not pods:
-                pods = await wg.pods()
-                await asyncio.sleep(0.1)
-            assert all([isinstance(p, Pod) for p in pods])
+            for wg in worker_groups:
+                assert isinstance(wg, DaskWorkerGroup)
 
-            deployments = []
-            while not deployments:
-                deployments = await wg.deployments()
-                await asyncio.sleep(0.1)
-            assert all([isinstance(d, Deployment) for d in deployments])
+                deployments = []
+                while not deployments:
+                    deployments = await wg.deployments()
+                    await asyncio.sleep(0.1)
+                assert all([isinstance(d, Deployment) for d in deployments])
+
+                pods = []
+                while not pods:
+                    pods = await wg.pods()
+                    await asyncio.sleep(0.1)
+                assert all([isinstance(p, Pod) for p in pods])
+
+                assert (await wg.cluster()).name == cluster.name
 
-            assert (await wg.cluster()).name == cluster.name
+                for deployment in deployments:
+                    assert deployment.labels["dask.org/cluster-name"] == cluster.name
+                    for env in deployment.spec["template"]["spec"]["containers"][0][
+                        "env"
+                    ]:
+                        if env["name"] == "DASK_WORKER_NAME":
+                            if wg.name == additional_workergroup_name:
+                                assert env["value"] == "test-worker"
+                            else:
+                                assert env["value"] == deployment.name
+                        if env["name"] == "DASK_SCHEDULER_ADDRESS":
+                            scheduler_service = await cluster.scheduler_service()
+                            assert f"{scheduler_service.name}.{ns}" in env["value"]
 
 
 @pytest.mark.anyio
 @pytest.mark.skip(reason="Flaky in CI")
 async def test_object_dask_job(k8s_cluster, kopf_runner, gen_job):
     with kopf_runner:
         async with gen_job("simplejob.yaml") as (job_name, ns):
```

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/customresources/daskautoscaler.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskautoscaler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/customresources/daskcluster.patch.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskcluster.patch.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/customresources/daskcluster.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskcluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/customresources/daskjob.patch.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskjob.patch.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/customresources/daskjob.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/customresources/daskworkergroup.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/customresources/templates.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/templates.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/chartpress.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/chartpress.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/kubecluster/kubecluster.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/kubecluster/kubecluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/kubecluster/tests/test_discovery.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/kubecluster/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes/operator/networking.py` & `dask-kubernetes-2024.4.0/dask_kubernetes/operator/networking.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes.egg-info/PKG-INFO` & `dask-kubernetes-2024.4.0/dask_kubernetes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-kubernetes
-Version: 2024.3.1
+Version: 2024.4.0
 Summary: Native Kubernetes integration for Dask
 Home-page: https://github.com/dask/dask-kubernetes
 Maintainer: Jacob Tomlinson
 License: BSD
 Keywords: dask,kubernetes,distributed
 Requires-Python: >=3.9
 License-File: LICENSE
```

### Comparing `dask-kubernetes-2024.3.1/dask_kubernetes.egg-info/SOURCES.txt` & `dask-kubernetes-2024.4.0/dask_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/pyproject.toml` & `dask-kubernetes-2024.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/setup.cfg` & `dask-kubernetes-2024.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/setup.py` & `dask-kubernetes-2024.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.3.1/versioneer.py` & `dask-kubernetes-2024.4.0/versioneer.py`

 * *Files identical despite different names*

