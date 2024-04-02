# Comparing `tmp/kubemarine-0.28.0.tar.gz` & `tmp/kubemarine-0.28.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubemarine-0.28.0.tar", last modified: Mon Mar 11 11:18:49 2024, max compression
+gzip compressed data, was "kubemarine-0.28.1.tar", last modified: Mon Apr  1 09:25:06 2024, max compression
```

## Comparing `kubemarine-0.28.0.tar` & `kubemarine-0.28.1.tar`

### file list

```diff
@@ -1,273 +1,272 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.840584 kubemarine-0.28.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-03-11 11:18:27.000000 kubemarine-0.28.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      183 2024-03-11 11:18:27.000000 kubemarine-0.28.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13978 2024-03-11 11:18:49.840584 kubemarine-0.28.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9311 2024-03-11 11:18:27.000000 kubemarine-0.28.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.772584 kubemarine-0.28.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)     1076 2024-03-11 11:18:27.000000 kubemarine-0.28.0/bin/kubemarine
--rw-r--r--   0 root         (0) root         (0)      657 2024-03-11 11:18:27.000000 kubemarine-0.28.0/bin/kubemarine.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.776584 kubemarine-0.28.0/kubemarine/
--rw-r--r--   0 root         (0) root         (0)      603 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     8303 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/__main__.py
--rw-r--r--   0 root         (0) root         (0)    29086 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/admission.py
--rw-r--r--   0 root         (0) root         (0)     5625 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/apparmor.py
--rw-r--r--   0 root         (0) root         (0)     5517 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/apt.py
--rw-r--r--   0 root         (0) root         (0)     6228 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/audit.py
--rw-r--r--   0 root         (0) root         (0)     2203 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/controlplane.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.784584 kubemarine-0.28.0/kubemarine/core/
--rw-r--r--   0 root         (0) root         (0)      604 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2044 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/core/action.py
--rw-r--r--   0 root         (0) root         (0)     2151 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/core/annotations.py
--rwxr-xr-x   0 root         (0) root         (0)    28019 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/core/cluster.py
--rw-r--r--   0 root         (0) root         (0)     4224 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/core/connections.py
--rwxr-xr-x   0 root         (0) root         (0)    28358 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/core/defaults.py
--rw-r--r--   0 root         (0) root         (0)     1125 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/core/environment.py
--rw-r--r--   0 root         (0) root         (0)     7482 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/core/errors.py
--rw-r--r--   0 root         (0) root         (0)    28797 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/core/executor.py
--rwxr-xr-x   0 root         (0) root         (0)    21799 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/core/flow.py
--rwxr-xr-x   0 root         (0) root         (0)    38631 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/core/group.py
--rw-r--r--   0 root         (0) root         (0)    15334 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/core/log.py
--rw-r--r--   0 root         (0) root         (0)     1060 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/core/os.py
--rw-r--r--   0 root         (0) root         (0)     2640 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/core/patch.py
--rw-r--r--   0 root         (0) root         (0)    24538 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/core/resources.py
--rw-r--r--   0 root         (0) root         (0)    15524 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/core/schema.py
--rw-r--r--   0 root         (0) root         (0)     2412 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/core/static.py
--rw-r--r--   0 root         (0) root         (0)     2183 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/core/summary.py
--rwxr-xr-x   0 root         (0) root         (0)    26348 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/core/utils.py
--rw-r--r--   0 root         (0) root         (0)     1993 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/core/yaml_merger.py
--rw-r--r--   0 root         (0) root         (0)     7230 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/coredns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.784584 kubemarine-0.28.0/kubemarine/cri/
--rw-r--r--   0 root         (0) root         (0)     3373 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/cri/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    16741 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/cri/containerd.py
--rwxr-xr-x   0 root         (0) root         (0)     3892 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/cri/docker.py
--rw-r--r--   0 root         (0) root         (0)    27236 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/demo.py
--rw-r--r--   0 root         (0) root         (0)     4648 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/etcd.py
--rw-r--r--   0 root         (0) root         (0)    10637 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/haproxy.py
--rw-r--r--   0 root         (0) root         (0)     2734 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/jinja.py
--rw-r--r--   0 root         (0) root         (0)     2347 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/k8s_certs.py
--rw-r--r--   0 root         (0) root         (0)    12492 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/keepalived.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.788584 kubemarine-0.28.0/kubemarine/kubernetes/
--rw-r--r--   0 root         (0) root         (0)    54805 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46264 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/kubernetes/components.py
--rw-r--r--   0 root         (0) root         (0)     2219 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/kubernetes/daemonset.py
--rw-r--r--   0 root         (0) root         (0)     1783 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/kubernetes/deployment.py
--rw-r--r--   0 root         (0) root         (0)     3993 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/kubernetes/object.py
--rw-r--r--   0 root         (0) root         (0)     2162 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/kubernetes/replicaset.py
--rw-r--r--   0 root         (0) root         (0)     4342 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/kubernetes/secrets.py
--rw-r--r--   0 root         (0) root         (0)     2007 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/kubernetes/statefulset.py
--rw-r--r--   0 root         (0) root         (0)     5945 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/kubernetes_accounts.py
--rw-r--r--   0 root         (0) root         (0)     4007 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/modprobe.py
--rw-r--r--   0 root         (0) root         (0)    30768 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/packages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.788584 kubemarine-0.28.0/kubemarine/patches/
--rw-r--r--   0 root         (0) root         (0)     1379 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/patches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2222 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/patches/disable_token_automount.py
--rw-r--r--   0 root         (0) root         (0)     1036 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/patches/software_upgrade.yaml
--rw-r--r--   0 root         (0) root         (0)     1586 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/patches/strong_ciphers_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.792584 kubemarine-0.28.0/kubemarine/plugins/
--rwxr-xr-x   0 root         (0) root         (0)    44549 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7859 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/builtin.py
--rwxr-xr-x   0 root         (0) root         (0)    29024 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/calico.py
--rw-r--r--   0 root         (0) root         (0)     7889 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/kubernetes_dashboard.py
--rw-r--r--   0 root         (0) root         (0)     7928 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/local_path_provisioner.py
--rw-r--r--   0 root         (0) root         (0)    27745 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/manifest.py
--rw-r--r--   0 root         (0) root         (0)    19679 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/nginx_ingress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.800584 kubemarine-0.28.0/kubemarine/plugins/yaml/
--rw-r--r--   0 root         (0) root         (0)     5796 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/calico-apiserver-v3.24.2-original.yaml
--rw-r--r--   0 root         (0) root         (0)     5874 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/calico-apiserver-v3.25.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)     5886 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/calico-apiserver-v3.26.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)     5886 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/calico-apiserver-v3.26.4-original.yaml
--rw-r--r--   0 root         (0) root         (0)     5886 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/calico-apiserver-v3.27.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)   222019 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml
--rw-r--r--   0 root         (0) root         (0)   239857 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml
--rw-r--r--   0 root         (0) root         (0)   243952 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)   250597 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/calico-v3.26.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)   250781 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/calico-v3.26.4-original.yaml
--rw-r--r--   0 root         (0) root         (0)   258410 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/calico-v3.27.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)     7621 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)     7621 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml
--rw-r--r--   0 root         (0) root         (0)     3752 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.25-original.yaml
--rw-r--r--   0 root         (0) root         (0)     3752 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.26-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15311 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15775 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15704 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15642 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15662 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.4-original.yaml
--rw-r--r--   0 root         (0) root         (0)    16337 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.4-original.yaml
--rw-r--r--   0 root         (0) root         (0)    16107 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.5-original.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.804584 kubemarine-0.28.0/kubemarine/procedures/
--rw-r--r--   0 root         (0) root         (0)      890 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/procedures/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4643 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/procedures/add_node.py
--rwxr-xr-x   0 root         (0) root         (0)    32509 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/procedures/backup.py
--rwxr-xr-x   0 root         (0) root         (0)     3553 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/procedures/cert_renew.py
--rwxr-xr-x   0 root         (0) root         (0)    71092 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/procedures/check_iaas.py
--rwxr-xr-x   0 root         (0) root         (0)    90567 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/procedures/check_paas.py
--rw-r--r--   0 root         (0) root         (0)     2548 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/procedures/config.py
--rwxr-xr-x   0 root         (0) root         (0)     4891 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/procedures/do.py
--rwxr-xr-x   0 root         (0) root         (0)    23256 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/procedures/install.py
--rwxr-xr-x   0 root         (0) root         (0)     1643 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/procedures/manage_psp.py
--rwxr-xr-x   0 root         (0) root         (0)     1532 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/procedures/manage_pss.py
--rwxr-xr-x   0 root         (0) root         (0)     8120 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/procedures/migrate_cri.py
--rw-r--r--   0 root         (0) root         (0)    21620 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/procedures/migrate_kubemarine.py
--rwxr-xr-x   0 root         (0) root         (0)     2435 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/procedures/reboot.py
--rw-r--r--   0 root         (0) root         (0)     2607 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/procedures/reconfigure.py
--rwxr-xr-x   0 root         (0) root         (0)     3928 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/procedures/remove_node.py
--rwxr-xr-x   0 root         (0) root         (0)    14156 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/procedures/restore.py
--rwxr-xr-x   0 root         (0) root         (0)    13035 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/procedures/upgrade.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.804584 kubemarine-0.28.0/kubemarine/resources/
--rw-r--r--   0 root         (0) root         (0)      604 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.804584 kubemarine-0.28.0/kubemarine/resources/configurations/
--rw-r--r--   0 root         (0) root         (0)      604 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/configurations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.804584 kubemarine-0.28.0/kubemarine/resources/configurations/compatibility/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.808584 kubemarine-0.28.0/kubemarine/resources/configurations/compatibility/internal/
--rw-r--r--   0 root         (0) root         (0)     4716 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml
--rw-r--r--   0 root         (0) root         (0)     5889 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml
--rw-r--r--   0 root         (0) root         (0)     5025 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml
--rw-r--r--   0 root         (0) root         (0)     7663 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
--rw-r--r--   0 root         (0) root         (0)     3944 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
--rw-r--r--   0 root         (0) root         (0)    31923 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/configurations/defaults.yaml
--rw-r--r--   0 root         (0) root         (0)    11291 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/configurations/globals.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.808584 kubemarine-0.28.0/kubemarine/resources/drop_ins/
--rw-r--r--   0 root         (0) root         (0)      604 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/drop_ins/__init__.py
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/drop_ins/haproxy.conf
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/drop_ins/keepalived.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.768584 kubemarine-0.28.0/kubemarine/resources/etalons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.808584 kubemarine-0.28.0/kubemarine/resources/etalons/patches/
--rw-r--r--   0 root         (0) root         (0)     1126 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/etalons/patches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1036 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/etalons/patches/software_upgrade.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.808584 kubemarine-0.28.0/kubemarine/resources/psp/
--rw-r--r--   0 root         (0) root         (0)      604 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/psp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1457 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/psp/anyuid.yaml
--rw-r--r--   0 root         (0) root         (0)     1923 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/psp/default.yaml
--rw-r--r--   0 root         (0) root         (0)     1618 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/psp/host-network.yaml
--rw-r--r--   0 root         (0) root         (0)     1204 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/psp/privileged.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.808584 kubemarine-0.28.0/kubemarine/resources/reports/
--rw-r--r--   0 root         (0) root         (0)      604 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/reports/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1773 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/reports/check_report.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.812584 kubemarine-0.28.0/kubemarine/resources/schemas/
--rw-r--r--   0 root         (0) root         (0)      478 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/add_node.json
--rw-r--r--   0 root         (0) root         (0)     2643 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/backup.json
--rw-r--r--   0 root         (0) root         (0)     1635 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/cert_renew.json
--rw-r--r--   0 root         (0) root         (0)      415 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/check_paas.json
--rw-r--r--   0 root         (0) root         (0)     3142 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/cluster.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.816584 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.816584 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/common/
--rw-r--r--   0 root         (0) root         (0)     1429 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/common/node_ref.json
--rw-r--r--   0 root         (0) root         (0)     1722 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/common/utils.json
--rw-r--r--   0 root         (0) root         (0)      708 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/gateway_node.json
--rw-r--r--   0 root         (0) root         (0)     4072 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/globals.json
--rw-r--r--   0 root         (0) root         (0)     1501 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/node.json
--rw-r--r--   0 root         (0) root         (0)     2363 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/node_defaults.json
--rw-r--r--   0 root         (0) root         (0)      575 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugin_defaults.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.820584 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/
--rw-r--r--   0 root         (0) root         (0)     7227 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/calico.json
--rw-r--r--   0 root         (0) root         (0)     2009 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.820584 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/installation/
--rw-r--r--   0 root         (0) root         (0)     1278 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json
--rw-r--r--   0 root         (0) root         (0)      689 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json
--rw-r--r--   0 root         (0) root         (0)     3120 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json
--rw-r--r--   0 root         (0) root         (0)     1220 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json
--rw-r--r--   0 root         (0) root         (0)      606 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json
--rw-r--r--   0 root         (0) root         (0)     2265 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json
--rw-r--r--   0 root         (0) root         (0)     2498 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json
--rw-r--r--   0 root         (0) root         (0)     1780 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/installation.json
--rw-r--r--   0 root         (0) root         (0)     3129 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json
--rw-r--r--   0 root         (0) root         (0)     1743 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json
--rw-r--r--   0 root         (0) root         (0)     3472 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json
--rw-r--r--   0 root         (0) root         (0)      605 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins.json
--rw-r--r--   0 root         (0) root         (0)      749 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/procedures.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.820584 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/rbac/
--rw-r--r--   0 root         (0) root         (0)      661 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/rbac/account.json
--rw-r--r--   0 root         (0) root         (0)     3266 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json
--rw-r--r--   0 root         (0) root         (0)     3759 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/rbac/psp.json
--rw-r--r--   0 root         (0) root         (0)     2453 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/rbac/pss.json
--rw-r--r--   0 root         (0) root         (0)      709 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/rbac.json
--rw-r--r--   0 root         (0) root         (0)     1951 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/registry.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.824584 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/
--rw-r--r--   0 root         (0) root         (0)     1948 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/audit.json
--rw-r--r--   0 root         (0) root         (0)     9668 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/coredns.json
--rw-r--r--   0 root         (0) root         (0)     3115 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/cri.json
--rw-r--r--   0 root         (0) root         (0)      644 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json
--rw-r--r--   0 root         (0) root         (0)     1963 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/kernel_security.json
--rw-r--r--   0 root         (0) root         (0)     5430 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/kubeadm.json
--rw-r--r--   0 root         (0) root         (0)      998 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/kubeadm_kube-proxy.json
--rw-r--r--   0 root         (0) root         (0)      938 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json
--rw-r--r--   0 root         (0) root         (0)     2764 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json
--rw-r--r--   0 root         (0) root         (0)     5264 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json
--rw-r--r--   0 root         (0) root         (0)     1001 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/modprobe.json
--rw-r--r--   0 root         (0) root         (0)     2302 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/ntp.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.824584 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/packages/
--rw-r--r--   0 root         (0) root         (0)     4268 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/packages/associations.json
--rw-r--r--   0 root         (0) root         (0)     5144 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/packages.json
--rw-r--r--   0 root         (0) root         (0)      479 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/resolv.conf.json
--rw-r--r--   0 root         (0) root         (0)     1243 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/sysctl.json
--rw-r--r--   0 root         (0) root         (0)     3302 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/thirdparties.json
--rw-r--r--   0 root         (0) root         (0)     1965 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services.json
--rw-r--r--   0 root         (0) root         (0)     3130 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/definitions/vrrp_ip.json
--rw-r--r--   0 root         (0) root         (0)      757 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/manage_psp.json
--rw-r--r--   0 root         (0) root         (0)     1657 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/manage_pss.json
--rw-r--r--   0 root         (0) root         (0)     1749 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/migrate_cri.json
--rw-r--r--   0 root         (0) root         (0)     2885 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/migrate_kubemarine.json
--rw-r--r--   0 root         (0) root         (0)      798 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/reboot.json
--rw-r--r--   0 root         (0) root         (0)     2326 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/reconfigure.json
--rw-r--r--   0 root         (0) root         (0)      872 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/remove_node.json
--rw-r--r--   0 root         (0) root         (0)     3365 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/restore.json
--rw-r--r--   0 root         (0) root         (0)     3504 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/schemas/upgrade.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.832584 kubemarine-0.28.0/kubemarine/resources/scripts/
--rw-r--r--   0 root         (0) root         (0)      604 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/scripts/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      288 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/scripts/check_haproxy.sh
--rw-r--r--   0 root         (0) root         (0)     1814 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/scripts/check_url_availability.py
--rwxr-xr-x   0 root         (0) root         (0)     3646 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/scripts/etcdctl.sh
--rwxr-xr-x   0 root         (0) root         (0)  2664796 2024-03-11 11:18:44.000000 kubemarine-0.28.0/kubemarine/resources/scripts/ipip_check.gz
--rw-r--r--   0 root         (0) root         (0)     1483 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/scripts/simple_port_client.py
--rw-r--r--   0 root         (0) root         (0)     2022 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/scripts/simple_port_listener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.768584 kubemarine-0.28.0/kubemarine/resources/scripts/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.832584 kubemarine-0.28.0/kubemarine/resources/scripts/source/ipip_check/
--rw-r--r--   0 root         (0) root         (0)       71 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/scripts/source/ipip_check/go.mod
--rw-r--r--   0 root         (0) root         (0)     1446 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/scripts/source/ipip_check/go.sum
--rw-r--r--   0 root         (0) root         (0)     5732 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/resources/scripts/source/ipip_check/ipip_check.go
--rw-r--r--   0 root         (0) root         (0)     8542 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/selinux.py
--rw-r--r--   0 root         (0) root         (0)     4073 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/sysctl.py
--rw-r--r--   0 root         (0) root         (0)    26273 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.832584 kubemarine-0.28.0/kubemarine/templates/
--rw-r--r--   0 root         (0) root         (0)      604 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)      667 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/admission.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     2431 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/haproxy.cfg.j2
--rw-r--r--   0 root         (0) root         (0)      996 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/keepalived.conf.j2
--rw-r--r--   0 root         (0) root         (0)     1126 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/kubelet.service.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.832584 kubemarine-0.28.0/kubemarine/templates/patches/
--rw-r--r--   0 root         (0) root         (0)      151 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/patches/control-plane-pod.json.j2
--rw-r--r--   0 root         (0) root         (0)       76 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/patches/kubelet.yaml.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.836584 kubemarine-0.28.0/kubemarine/templates/plugins/
--rw-r--r--   0 root         (0) root         (0)      604 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      879 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/plugins/calico-ippool.yaml.j2
--rw-r--r--   0 root         (0) root         (0)      286 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/plugins/calico-kube-controllers-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      245 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/plugins/calico-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      436 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/plugins/calico-rr.sh.j2
--rw-r--r--   0 root         (0) root         (0)      960 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/plugins/calico-rr.yaml.j2
--rw-r--r--   0 root         (0) root         (0)      262 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/plugins/calico-typha-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      136 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/plugins/calicoctl.cfg.j2
--rw-r--r--   0 root         (0) root         (0)      107 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/plugins/dashboard-ingress.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     8826 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     8905 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     2749 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/plugins/iperf3.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     5401 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     9973 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2
--rw-r--r--   0 root         (0) root         (0)    17847 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2
--rw-r--r--   0 root         (0) root         (0)    11852 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/testsuite.py
--rw-r--r--   0 root         (0) root         (0)    19546 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/thirdparties.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/version
--rw-r--r--   0 root         (0) root         (0)     5696 2024-03-11 11:18:27.000000 kubemarine-0.28.0/kubemarine/yum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:18:49.836584 kubemarine-0.28.0/kubemarine.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13978 2024-03-11 11:18:49.000000 kubemarine-0.28.0/kubemarine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10714 2024-03-11 11:18:49.000000 kubemarine-0.28.0/kubemarine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-11 11:18:49.000000 kubemarine-0.28.0/kubemarine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2024-03-11 11:18:49.000000 kubemarine-0.28.0/kubemarine.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      492 2024-03-11 11:18:49.000000 kubemarine-0.28.0/kubemarine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-03-11 11:18:49.000000 kubemarine-0.28.0/kubemarine.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3535 2024-03-11 11:18:27.000000 kubemarine-0.28.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-11 11:18:49.840584 kubemarine-0.28.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1628 2024-03-11 11:18:27.000000 kubemarine-0.28.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.132035 kubemarine-0.28.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-01 09:24:41.000000 kubemarine-0.28.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      183 2024-04-01 09:24:41.000000 kubemarine-0.28.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    13978 2024-04-01 09:25:06.132035 kubemarine-0.28.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9311 2024-04-01 09:24:41.000000 kubemarine-0.28.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.064035 kubemarine-0.28.1/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     1076 2024-04-01 09:24:41.000000 kubemarine-0.28.1/bin/kubemarine
+-rw-r--r--   0 root         (0) root         (0)      657 2024-04-01 09:24:41.000000 kubemarine-0.28.1/bin/kubemarine.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.072035 kubemarine-0.28.1/kubemarine/
+-rw-r--r--   0 root         (0) root         (0)      603 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7924 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    29086 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/admission.py
+-rw-r--r--   0 root         (0) root         (0)     5625 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/apparmor.py
+-rw-r--r--   0 root         (0) root         (0)     5517 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/apt.py
+-rw-r--r--   0 root         (0) root         (0)     6228 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/audit.py
+-rw-r--r--   0 root         (0) root         (0)     2203 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/controlplane.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.076035 kubemarine-0.28.1/kubemarine/core/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2044 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/action.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/annotations.py
+-rwxr-xr-x   0 root         (0) root         (0)    28019 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     4224 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/connections.py
+-rwxr-xr-x   0 root         (0) root         (0)    28358 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/defaults.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/environment.py
+-rw-r--r--   0 root         (0) root         (0)     7299 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    30247 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/executor.py
+-rwxr-xr-x   0 root         (0) root         (0)    21799 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/flow.py
+-rwxr-xr-x   0 root         (0) root         (0)    38504 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/group.py
+-rw-r--r--   0 root         (0) root         (0)    15334 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/log.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/os.py
+-rw-r--r--   0 root         (0) root         (0)     2640 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/patch.py
+-rw-r--r--   0 root         (0) root         (0)    24538 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/resources.py
+-rw-r--r--   0 root         (0) root         (0)    15524 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/schema.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/static.py
+-rw-r--r--   0 root         (0) root         (0)     2183 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/summary.py
+-rwxr-xr-x   0 root         (0) root         (0)    26348 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1993 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/core/yaml_merger.py
+-rw-r--r--   0 root         (0) root         (0)     7230 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/coredns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.080035 kubemarine-0.28.1/kubemarine/cri/
+-rw-r--r--   0 root         (0) root         (0)     3373 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/cri/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    16741 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/cri/containerd.py
+-rwxr-xr-x   0 root         (0) root         (0)     3892 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/cri/docker.py
+-rw-r--r--   0 root         (0) root         (0)    27236 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/demo.py
+-rw-r--r--   0 root         (0) root         (0)     4648 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/etcd.py
+-rw-r--r--   0 root         (0) root         (0)    10637 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/haproxy.py
+-rw-r--r--   0 root         (0) root         (0)     2734 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/jinja.py
+-rw-r--r--   0 root         (0) root         (0)     2347 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/k8s_certs.py
+-rw-r--r--   0 root         (0) root         (0)    12492 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/keepalived.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.080035 kubemarine-0.28.1/kubemarine/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)    55178 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47459 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/kubernetes/components.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/kubernetes/daemonset.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/kubernetes/deployment.py
+-rw-r--r--   0 root         (0) root         (0)     3993 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/kubernetes/object.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/kubernetes/replicaset.py
+-rw-r--r--   0 root         (0) root         (0)     4342 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/kubernetes/secrets.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/kubernetes/statefulset.py
+-rw-r--r--   0 root         (0) root         (0)     5945 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/kubernetes_accounts.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/modprobe.py
+-rw-r--r--   0 root         (0) root         (0)    30768 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/packages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.080035 kubemarine-0.28.1/kubemarine/patches/
+-rw-r--r--   0 root         (0) root         (0)     1224 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/patches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/patches/patch_kubelet_configmap.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/patches/software_upgrade.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.084035 kubemarine-0.28.1/kubemarine/plugins/
+-rwxr-xr-x   0 root         (0) root         (0)    44549 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7859 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/builtin.py
+-rwxr-xr-x   0 root         (0) root         (0)    29024 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/calico.py
+-rw-r--r--   0 root         (0) root         (0)     7889 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/kubernetes_dashboard.py
+-rw-r--r--   0 root         (0) root         (0)     7928 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/local_path_provisioner.py
+-rw-r--r--   0 root         (0) root         (0)    27745 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/manifest.py
+-rw-r--r--   0 root         (0) root         (0)    19679 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/nginx_ingress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.092035 kubemarine-0.28.1/kubemarine/plugins/yaml/
+-rw-r--r--   0 root         (0) root         (0)     5796 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-apiserver-v3.24.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     5874 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-apiserver-v3.25.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     5886 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-apiserver-v3.26.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     5886 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-apiserver-v3.26.4-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     5886 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-apiserver-v3.27.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   222019 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   239857 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   243952 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   250597 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.26.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   250781 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.26.4-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   258410 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.27.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     7621 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     7621 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     3752 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.25-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     3752 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.26-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15311 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15775 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15704 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15642 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15662 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.4-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    16337 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.4-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    16107 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.5-original.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.096035 kubemarine-0.28.1/kubemarine/procedures/
+-rw-r--r--   0 root         (0) root         (0)     3369 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4643 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/add_node.py
+-rwxr-xr-x   0 root         (0) root         (0)    32509 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/backup.py
+-rwxr-xr-x   0 root         (0) root         (0)     3553 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/cert_renew.py
+-rwxr-xr-x   0 root         (0) root         (0)    73784 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/check_iaas.py
+-rwxr-xr-x   0 root         (0) root         (0)    90567 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/check_paas.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/config.py
+-rwxr-xr-x   0 root         (0) root         (0)     4891 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/do.py
+-rwxr-xr-x   0 root         (0) root         (0)    23256 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/install.py
+-rwxr-xr-x   0 root         (0) root         (0)     1643 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/manage_psp.py
+-rwxr-xr-x   0 root         (0) root         (0)     1532 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/manage_pss.py
+-rwxr-xr-x   0 root         (0) root         (0)     8120 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/migrate_cri.py
+-rw-r--r--   0 root         (0) root         (0)    21620 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/migrate_kubemarine.py
+-rwxr-xr-x   0 root         (0) root         (0)     2435 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/reboot.py
+-rw-r--r--   0 root         (0) root         (0)     2607 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/reconfigure.py
+-rwxr-xr-x   0 root         (0) root         (0)     3928 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/remove_node.py
+-rwxr-xr-x   0 root         (0) root         (0)    14156 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/restore.py
+-rwxr-xr-x   0 root         (0) root         (0)    13035 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/procedures/upgrade.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.096035 kubemarine-0.28.1/kubemarine/resources/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.100035 kubemarine-0.28.1/kubemarine/resources/configurations/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/configurations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.100035 kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.100035 kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/internal/
+-rw-r--r--   0 root         (0) root         (0)     4716 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml
+-rw-r--r--   0 root         (0) root         (0)     5889 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/internal/packages.yaml
+-rw-r--r--   0 root         (0) root         (0)     5025 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/internal/plugins.yaml
+-rw-r--r--   0 root         (0) root         (0)     7663 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
+-rw-r--r--   0 root         (0) root         (0)     3944 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
+-rw-r--r--   0 root         (0) root         (0)    31923 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/configurations/defaults.yaml
+-rw-r--r--   0 root         (0) root         (0)    11291 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/configurations/globals.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.100035 kubemarine-0.28.1/kubemarine/resources/drop_ins/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/drop_ins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/drop_ins/haproxy.conf
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/drop_ins/keepalived.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.060035 kubemarine-0.28.1/kubemarine/resources/etalons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.100035 kubemarine-0.28.1/kubemarine/resources/etalons/patches/
+-rw-r--r--   0 root         (0) root         (0)     1126 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/etalons/patches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/etalons/patches/software_upgrade.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.104035 kubemarine-0.28.1/kubemarine/resources/psp/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/psp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/psp/anyuid.yaml
+-rw-r--r--   0 root         (0) root         (0)     1923 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/psp/default.yaml
+-rw-r--r--   0 root         (0) root         (0)     1618 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/psp/host-network.yaml
+-rw-r--r--   0 root         (0) root         (0)     1204 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/psp/privileged.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.104035 kubemarine-0.28.1/kubemarine/resources/reports/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/reports/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/reports/check_report.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.108035 kubemarine-0.28.1/kubemarine/resources/schemas/
+-rw-r--r--   0 root         (0) root         (0)      478 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/add_node.json
+-rw-r--r--   0 root         (0) root         (0)     2643 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/backup.json
+-rw-r--r--   0 root         (0) root         (0)     1635 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/cert_renew.json
+-rw-r--r--   0 root         (0) root         (0)      415 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/check_paas.json
+-rw-r--r--   0 root         (0) root         (0)     3142 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/cluster.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.108035 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.112035 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/common/
+-rw-r--r--   0 root         (0) root         (0)     1429 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/common/node_ref.json
+-rw-r--r--   0 root         (0) root         (0)     1722 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/common/utils.json
+-rw-r--r--   0 root         (0) root         (0)      708 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/gateway_node.json
+-rw-r--r--   0 root         (0) root         (0)     4072 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/globals.json
+-rw-r--r--   0 root         (0) root         (0)     1501 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/node.json
+-rw-r--r--   0 root         (0) root         (0)     2363 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/node_defaults.json
+-rw-r--r--   0 root         (0) root         (0)      575 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugin_defaults.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.112035 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/
+-rw-r--r--   0 root         (0) root         (0)     7227 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/calico.json
+-rw-r--r--   0 root         (0) root         (0)     2009 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.112035 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json
+-rw-r--r--   0 root         (0) root         (0)      689 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/config.json
+-rw-r--r--   0 root         (0) root         (0)     3120 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/expect.json
+-rw-r--r--   0 root         (0) root         (0)     1220 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/helm.json
+-rw-r--r--   0 root         (0) root         (0)      606 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/python.json
+-rw-r--r--   0 root         (0) root         (0)     2265 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/shell.json
+-rw-r--r--   0 root         (0) root         (0)     2498 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/template.json
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation.json
+-rw-r--r--   0 root         (0) root         (0)     3129 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json
+-rw-r--r--   0 root         (0) root         (0)     1743 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json
+-rw-r--r--   0 root         (0) root         (0)     3472 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json
+-rw-r--r--   0 root         (0) root         (0)      605 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins.json
+-rw-r--r--   0 root         (0) root         (0)      749 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/procedures.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.116035 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac/
+-rw-r--r--   0 root         (0) root         (0)      661 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac/account.json
+-rw-r--r--   0 root         (0) root         (0)     3266 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac/account_defaults.json
+-rw-r--r--   0 root         (0) root         (0)     3759 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac/psp.json
+-rw-r--r--   0 root         (0) root         (0)     2453 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac/pss.json
+-rw-r--r--   0 root         (0) root         (0)      709 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac.json
+-rw-r--r--   0 root         (0) root         (0)     1951 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/registry.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.120035 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/
+-rw-r--r--   0 root         (0) root         (0)     1948 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/audit.json
+-rw-r--r--   0 root         (0) root         (0)     9668 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/coredns.json
+-rw-r--r--   0 root         (0) root         (0)     3115 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/cri.json
+-rw-r--r--   0 root         (0) root         (0)      644 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/etc_hosts.json
+-rw-r--r--   0 root         (0) root         (0)     1963 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/kernel_security.json
+-rw-r--r--   0 root         (0) root         (0)     5430 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/kubeadm.json
+-rw-r--r--   0 root         (0) root         (0)      998 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/kubeadm_kube-proxy.json
+-rw-r--r--   0 root         (0) root         (0)      938 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json
+-rw-r--r--   0 root         (0) root         (0)     2764 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json
+-rw-r--r--   0 root         (0) root         (0)     5264 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/loadbalancer.json
+-rw-r--r--   0 root         (0) root         (0)     1001 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/modprobe.json
+-rw-r--r--   0 root         (0) root         (0)     2302 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/ntp.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.120035 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/packages/
+-rw-r--r--   0 root         (0) root         (0)     4268 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/packages/associations.json
+-rw-r--r--   0 root         (0) root         (0)     5144 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/packages.json
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/resolv.conf.json
+-rw-r--r--   0 root         (0) root         (0)     1243 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/sysctl.json
+-rw-r--r--   0 root         (0) root         (0)     3302 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/thirdparties.json
+-rw-r--r--   0 root         (0) root         (0)     1965 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services.json
+-rw-r--r--   0 root         (0) root         (0)     3130 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/definitions/vrrp_ip.json
+-rw-r--r--   0 root         (0) root         (0)      757 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/manage_psp.json
+-rw-r--r--   0 root         (0) root         (0)     1657 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/manage_pss.json
+-rw-r--r--   0 root         (0) root         (0)     1749 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/migrate_cri.json
+-rw-r--r--   0 root         (0) root         (0)     2885 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/migrate_kubemarine.json
+-rw-r--r--   0 root         (0) root         (0)      798 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/reboot.json
+-rw-r--r--   0 root         (0) root         (0)     2326 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/reconfigure.json
+-rw-r--r--   0 root         (0) root         (0)      872 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/remove_node.json
+-rw-r--r--   0 root         (0) root         (0)     3365 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/restore.json
+-rw-r--r--   0 root         (0) root         (0)     3504 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/schemas/upgrade.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.124035 kubemarine-0.28.1/kubemarine/resources/scripts/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/scripts/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      288 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/scripts/check_haproxy.sh
+-rw-r--r--   0 root         (0) root         (0)     1814 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/scripts/check_url_availability.py
+-rwxr-xr-x   0 root         (0) root         (0)     3646 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/scripts/etcdctl.sh
+-rwxr-xr-x   0 root         (0) root         (0)  2664796 2024-04-01 09:25:00.000000 kubemarine-0.28.1/kubemarine/resources/scripts/ipip_check.gz
+-rw-r--r--   0 root         (0) root         (0)     1483 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/scripts/simple_port_client.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/scripts/simple_port_listener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.060035 kubemarine-0.28.1/kubemarine/resources/scripts/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.124035 kubemarine-0.28.1/kubemarine/resources/scripts/source/ipip_check/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/scripts/source/ipip_check/go.mod
+-rw-r--r--   0 root         (0) root         (0)     1446 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/scripts/source/ipip_check/go.sum
+-rw-r--r--   0 root         (0) root         (0)     5732 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/resources/scripts/source/ipip_check/ipip_check.go
+-rw-r--r--   0 root         (0) root         (0)     8542 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/selinux.py
+-rw-r--r--   0 root         (0) root         (0)     4073 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/sysctl.py
+-rw-r--r--   0 root         (0) root         (0)    26273 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.128035 kubemarine-0.28.1/kubemarine/templates/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      667 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/admission.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     2431 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/haproxy.cfg.j2
+-rw-r--r--   0 root         (0) root         (0)      996 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/keepalived.conf.j2
+-rw-r--r--   0 root         (0) root         (0)     1126 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/kubelet.service.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.128035 kubemarine-0.28.1/kubemarine/templates/patches/
+-rw-r--r--   0 root         (0) root         (0)      151 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/patches/control-plane-pod.json.j2
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/patches/kubelet.yaml.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.132035 kubemarine-0.28.1/kubemarine/templates/plugins/
+-rw-r--r--   0 root         (0) root         (0)      604 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      879 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/calico-ippool.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)      286 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/calico-kube-controllers-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/calico-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      436 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/calico-rr.sh.j2
+-rw-r--r--   0 root         (0) root         (0)      960 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/calico-rr.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)      262 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/calico-typha-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      136 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/calicoctl.cfg.j2
+-rw-r--r--   0 root         (0) root         (0)      107 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/dashboard-ingress.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     8826 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     8905 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     2749 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/iperf3.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     5401 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/local-path-provisioner.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     9973 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)    17847 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)    11852 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/testsuite.py
+-rw-r--r--   0 root         (0) root         (0)    19546 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/thirdparties.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/version
+-rw-r--r--   0 root         (0) root         (0)     5696 2024-04-01 09:24:41.000000 kubemarine-0.28.1/kubemarine/yum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 09:25:06.132035 kubemarine-0.28.1/kubemarine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13978 2024-04-01 09:25:06.000000 kubemarine-0.28.1/kubemarine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10671 2024-04-01 09:25:06.000000 kubemarine-0.28.1/kubemarine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 09:25:06.000000 kubemarine-0.28.1/kubemarine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2024-04-01 09:25:06.000000 kubemarine-0.28.1/kubemarine.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      492 2024-04-01 09:25:06.000000 kubemarine-0.28.1/kubemarine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-01 09:25:06.000000 kubemarine-0.28.1/kubemarine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3535 2024-04-01 09:24:41.000000 kubemarine-0.28.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-01 09:25:06.132035 kubemarine-0.28.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1628 2024-04-01 09:24:41.000000 kubemarine-0.28.1/setup.py
```

### Comparing `kubemarine-0.28.0/LICENSE` & `kubemarine-0.28.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/PKG-INFO` & `kubemarine-0.28.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubemarine
-Version: 0.28.0
+Version: 0.28.1
 Summary: Management tool for Kubernetes cluster deployment and maintenance
 Home-page: https://github.com/Netcracker/KubeMarine
 Author-email: Kubemarine Group <kubemarinegroup@netcracker.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Netcracker/KubeMarine
 Project-URL: Documentation, https://github.com/Netcracker/KubeMarine#documentation
 Project-URL: Issues, https://github.com/Netcracker/KubeMarine/issues/
@@ -61,38 +61,38 @@
 
 # Kubemarine
 
 Kubemarine is an open source, lightweight and powerful management tool built for end-to-end Kubernetes cluster deployment and maintenance. It is applicable for many purposes like simple and quick onboarding Kubernetes on local and production environments in different HA schemes depending on your aims, budget, and capabilities. Together with simplicity, Kubemarine can be a very flexible and customizable tool covering specific configurability cases on both deployment and maintenance stages. This library provides powerful CLI commands, as well as can be customized using a Python extension API.
 
 ## Highlights
 - Easy to use
-- Many procedures supported following the [generic maintenance approach](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#basics):
-  - [install](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#)
-  - [add_node](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#add-node-procedure)
-  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#remove-node-procedure)
-  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#upgrade-procedure)
-  - [backup](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#backup-procedure)
-  - [restore](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#restore-procedure)
-  - [reconfigure](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#reconfigure-procedure)
-  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Kubecheck.md#iaas-procedure)
-  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Kubecheck.md#paas-procedure)
-  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#kubemarine-migration-procedure)
-  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#manage-psp-procedure)
-  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#manage-pss-procedure)
-  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#certificate-renew-procedure)
-  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#cri-migration-procedure)
-- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#configuration) for all operations, highly customizable
+- Many procedures supported following the [generic maintenance approach](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#basics):
+  - [install](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#)
+  - [add_node](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#add-node-procedure)
+  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#remove-node-procedure)
+  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#upgrade-procedure)
+  - [backup](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#backup-procedure)
+  - [restore](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#restore-procedure)
+  - [reconfigure](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#reconfigure-procedure)
+  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Kubecheck.md#iaas-procedure)
+  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Kubecheck.md#paas-procedure)
+  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#kubemarine-migration-procedure)
+  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#manage-psp-procedure)
+  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#manage-pss-procedure)
+  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#certificate-renew-procedure)
+  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#cri-migration-procedure)
+- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#configuration) for all operations, highly customizable
 - Default values of all parameters in configurations with a minimum of required parameters
-- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
-- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
-- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#custom-plugins-installation-procedures) support
-- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#installation-without-internet-resources) with private registries
-- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#dump-files)
+- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
+- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
+- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#custom-plugins-installation-procedures) support
+- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#installation-without-internet-resources) with private registries
+- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#dump-files)
 - Build supported as a package, container, and binary
-- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/PackageExtension.md)
+- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/PackageExtension.md)
 - Support different deployment schemes (all-in-one, mini-HA, HA, and so on)
 
 ## Kubemarine Binary Installation
 Proceed the following steps to install Kubemarine  on your environment:
 1. Download the binary file for your system from the latest [release](https://github.com/Netcracker/KubeMarine/releases)
 2. Move binary kubemarine to a separate folder 
 3. Now you can proceed to run Kubemarine! Try the following:
@@ -110,15 +110,15 @@
    ```bash
    python3 -m pip install --upgrade pip
    ```
    Windows:
    ```bash
    python -m pip install --upgrade pip
    ```
-1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#prerequisites-for-deployment-node).
+1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#prerequisites-for-deployment-node).
 1. Create and activate a [virtual environment](https://realpython.com/python-virtual-environments-a-primer/) if necessary.
 1. Install Kubemarine package.
 
    Linux / MacOS:
    ```bash
    python3 -m pip install kubemarine
    ```
@@ -129,15 +129,15 @@
 1. Now you can proceed to run Kubemarine! Try the following:
    ```bash
    kubemarine help
    ```
 
 
 ## Kubemarine Installation from Sources
-Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/README.md#kubemarine-package-installation).
+Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/README.md#kubemarine-package-installation).
 The exception is instead of installing the package from [PyPI](https://pypi.org/project/kubemarine/), do the following:
 1. [Download the latest release](https://github.com/netcracker/kubemarine/releases) or clone the repository:
    ```bash
    git clone https://github.com/netcracker/kubemarine.git
    ```
 1. Unpack the project from the archive if required:
    ```bash
@@ -158,24 +158,24 @@
    python -m pip install -e .
    ```
 1. Now you can proceed to run Kubemarine. Try the following:
     ```bash
     kubemarine help
     ```
 
-**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/Dockerfile) is also available.
+**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/Dockerfile) is also available.
 
 
 **Note:** Kubemarine debugging available via `kubemarine/__main__.py`.
 
 
 ## Running Cluster Installation
 To install a Kubernetes cluster using Kubemarine:
-1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
-1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
+1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#prerequisites-for-cluster-nodes).
+1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
    ```yaml
    node_defaults:
      keyfile: "/home/username/.ssh/id_rsa"
      password: '{{ env.PASS }}'     #Either keyfile or password can be used.
      username: "centos"
 
    vrrp_ips:
@@ -204,42 +204,42 @@
    kubemarine install
    ```
 1. Check the health of the newly installed cluster:
    ```bash
    kubemarine check_paas
    ```
 
-For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/README.md#documentation).
+For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/README.md#documentation).
 
 ## Kubemarine Docker Installation
 To start, download the Kubmarine image ```docker pull ghcr.io/netcracker/kubemarine:main```
 
 Run Kubemarine from the container, for example:
    ```
    docker run -it --mount type=bind,source=/root/cluster.yaml,target=/opt/kubemarine/cluster.yaml --mount type=bind,source=/root/rsa_key,target=/opt/kubemarine/rsa_key kubemarine install -c /opt/kubemarine/cluster.yaml
    ```
    *Note*: Do not forget to pass the inventory file and connection key inside the container.
    For more execution details, refer to ["Installation of Kubernetes using CLI" guide on Github](https://github.com/Netcracker/kubemarine/blob/main/documentation/Installation.md#installation-of-kubernetes-using-cli).
 
 ## Documentation
 The following documents and tutorials are available:
-- [Installation](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md)
-- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md)
-- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Troubleshooting.md)
-- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Kubecheck.md)
-- [Logging](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Logging.md)
+- [Installation](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md)
+- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md)
+- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Troubleshooting.md)
+- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Kubecheck.md)
+- [Logging](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Logging.md)
 
 Also, check out the following inventory examples:
-- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/examples/cluster.yaml)
-- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/examples/procedure.yaml)
+- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/examples/cluster.yaml)
+- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/examples/procedure.yaml)
 
 ## Issues, Questions
 If you have any problems while working with Kubemarine, feel free to open a [new issue](https://github.com/netcracker/kubemarine/issues) or even
 [PR](https://github.com/netcracker/kubemarine/pulls) with related changes.
-Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
+Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
 
-In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/SECURITY.md)
+In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/SECURITY.md)
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/netcracker/kubemarine/releases).
 
 ## License
-[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/LICENSE)
+[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/LICENSE)
```

### Comparing `kubemarine-0.28.0/README.md` & `kubemarine-0.28.1/README.md`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/bin/kubemarine` & `kubemarine-0.28.1/bin/kubemarine`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/bin/kubemarine.cmd` & `kubemarine-0.28.1/bin/kubemarine.cmd`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/__init__.py` & `kubemarine-0.28.1/kubemarine/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/__main__.py` & `kubemarine-0.28.1/kubemarine/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -196,39 +196,32 @@
 
         for attr in dir(module):
             if isinstance(getattr(module, attr), types.ModuleType):
                 imports.append(attr)
 
         print("%s has %s imports" % (procedure, len(imports)))
 
-        if "main" not in dir(module):
-            raise Exception("No main method in %s" % procedure)
-        if procedure not in ["do", "migrate_kubemarine", "config"]:
-            if "tasks" not in dir(module):
-                raise Exception("Tasks tree is not presented in %s" % procedure)
-            if not isinstance(module.tasks, OrderedDict):
-                raise Exception("Tasks are not ordered in %s" % procedure)
-            if not module.tasks:
-                raise Exception("Tasks are empty in %s" % procedure)
+        if isinstance(module, proc.TasksProcedure) and not module.tasks:
+            raise Exception("Tasks are empty in %s" % procedure)
 
         print("%s OK" % procedure)
 
         del module
         proc.deimport_procedure(procedure)
 
     print("\nTrying fake cluster...")
 
     from kubemarine import demo
 
     demo.new_cluster(demo.generate_inventory(**demo.FULLHA))
 
     print('\nValidating patch duplicates ...')
 
-    module = proc.import_procedure('migrate_kubemarine')
-    patches = module.load_patches()
+    from kubemarine.procedures import migrate_kubemarine
+    patches = migrate_kubemarine.load_patches()
     patch_ids = [patch.identifier for patch in patches]
     unique = set()
     for p_id in patch_ids:
         if p_id in unique:
             raise Exception(f'Patches identifier {p_id!r} is duplicated')
         unique.add(p_id)
```

### Comparing `kubemarine-0.28.0/kubemarine/admission.py` & `kubemarine-0.28.1/kubemarine/admission.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/apparmor.py` & `kubemarine-0.28.1/kubemarine/apparmor.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/apt.py` & `kubemarine-0.28.1/kubemarine/apt.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/audit.py` & `kubemarine-0.28.1/kubemarine/audit.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/controlplane.py` & `kubemarine-0.28.1/kubemarine/controlplane.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/core/__init__.py` & `kubemarine-0.28.1/kubemarine/core/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/core/action.py` & `kubemarine-0.28.1/kubemarine/core/action.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/core/annotations.py` & `kubemarine-0.28.1/kubemarine/core/annotations.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/core/cluster.py` & `kubemarine-0.28.1/kubemarine/core/cluster.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/core/connections.py` & `kubemarine-0.28.1/kubemarine/core/connections.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/core/defaults.py` & `kubemarine-0.28.1/kubemarine/core/defaults.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/core/environment.py` & `kubemarine-0.28.1/kubemarine/core/environment.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/core/errors.py` & `kubemarine-0.28.1/kubemarine/core/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import io
 import sys
 import traceback
 from abc import ABC, abstractmethod
 
-from concurrent.futures import TimeoutError
 from textwrap import dedent
 from typing import Type, List
 
 from kubemarine.core import log as klog
 
 
 def get_kme_dictionary() -> dict:
@@ -29,18 +28,14 @@
         "KME0000": {
             "name": "Test exception"
         },
         "KME0002": {
             "instance": GroupException,
             "name": "Remote group exception\n{reason}"
         },
-        "KME0003": {
-            "instance": TimeoutError,
-            "name": "Action took too long to complete and timed out"
-        },
         "KME0004": {
             "name": "There are no workers defined in the cluster scheme"
         },
         "KME0005": {
             "name": "{hostnames} are not sudoers"
         },
         "KME0006": {
```

### Comparing `kubemarine-0.28.0/kubemarine/core/executor.py` & `kubemarine-0.28.1/kubemarine/core/executor.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
 import invoke
 
 from kubemarine.core import log, static
 from kubemarine.core.connections import ConnectionPool
 from kubemarine.core.environment import Environment
 
+EXIT_CODE_PATTERN = re.compile(r'^\n(\d+)\n')
+
 
 class RunnersResult:
     def __init__(self, commands: List[str], exit_codes: List[int], stdout: str = "", stderr: str = "",
                  hide: bool = False) -> None:
         self.commands = commands
         self.stdout = stdout
         self.stderr = stderr
@@ -192,24 +194,21 @@
 _PayloadItem = Tuple[_Action, Optional[Callback], Token]
 
 _T = TypeVar('_T', bound='RawExecutor')
 
 
 class RawExecutor:
 
-    def __init__(self, cluster: Environment, connection_pool: ConnectionPool = None, timeout: int = None) -> None:
+    def __init__(self, cluster: Environment, connection_pool: ConnectionPool = None) -> None:
         self.logger = cluster.log
         if connection_pool is not None:
             self.connection_pool = connection_pool
         else:
             self.connection_pool = cluster.connection_pool
         self.inventory = cluster.inventory
-        self.timeout = timeout
-        if timeout is None:
-            self.timeout = static.GLOBALS['nodes']['command_execution']['timeout']
         self._connections_queue: Dict[str, List[_PayloadItem]] = {}
         self._last_token = -1
         self._last_results: Dict[str, TokenizedResult] = {}
         self._command_separator = ''.join(random.choice('=-_') for _ in range(32))
         self._supported_args = {'hide', 'warn', 'timeout', 'env', 'out_stream', 'err_stream'}
         self._closed = False
 
@@ -255,17 +254,14 @@
         for host, raw_result in raw_results.items():
             payloads = batch[host]
             conn_results: TokenizedResult = collections.OrderedDict()
             reparsed_results[host] = conn_results
 
             runner_exception = None
             if isinstance(raw_result, invoke.UnexpectedExit) or isinstance(raw_result, invoke.CommandTimedOut):
-                # If UnexpectedExit, all separators are printed till the last failed command.
-                # CommandTimedOut may currently arise only for the single command in the batch,
-                # so it definitely have no separators in the output, and it is thus safe to parse it.
                 runner_exception = raw_result
                 raw_result = raw_result.result
 
             if not isinstance(raw_result, fabric.runners.Result):
                 token = payloads[0][2]
                 conn_results[token] = raw_result
                 continue
@@ -276,46 +272,81 @@
                 reparsed_result: GenericResult = result
                 _, callback, token = payloads[i]
                 if i == len(results) - 1 and runner_exception is not None:
                     if isinstance(runner_exception, invoke.UnexpectedExit):
                         # Commands were successful until the last command in the batch.
                         reparsed_result = UnexpectedExit(result)
                     if isinstance(runner_exception, invoke.CommandTimedOut):
-                        # There can be only one (and the last) command with 'timeout' in the batch.
+                        # Commands were successful until the last reparsed command.
+
+                        # Take common timeout as timeout for the last command.
+                        # This is not honest enough, as previous commands also consumed some time.
+                        # This is acceptable for an exceptional case when we did not expect long-running command,
+                        # as this is applicable only for commands without explicit timeout
+                        # (i.e. having timeout=globals.nodes.command_execution.timeout).
                         reparsed_result = CommandTimedOut(result, runner_exception.timeout)
 
                 conn_results[token] = reparsed_result
                 if callback is not None and isinstance(reparsed_result, RunnersResult):
                     callback.accept(host, token, reparsed_result)
 
         return reparsed_results
 
     def _reparse_fabric_result(self, payloads: List[_PayloadItem],
                                result: fabric.runners.Result) -> List[RunnersResult]:
         # unpack last action in list of payloads
         _, _, kwargs = payloads[-1][0]
+        hide = kwargs.get('hide', False)
 
-        stderrs = result.stderr.split(self._command_separator + '\n')
-        raw_stdouts = result.stdout.split(self._command_separator + '\n')
-        stdouts = []
-        exit_codes = []
-        i = 0
-        while i < len(raw_stdouts):
-            stdouts.append(raw_stdouts[i])
-            if i + 1 < len(raw_stdouts):
-                exit_codes.append(int(raw_stdouts[i + 1].strip()))
-            i += 2
-        exit_codes.append(result.exited)
+        # Raw stdout may not fully contain the separator,
+        # if the channel was closed due to a timeout while reading the separator from the remote output.
+        # In this case the part of the separator becomes a part of the reparsed command output.
+        # This is acceptable as the situation is considered extremely rare,
+        # and because the only we can do with not finished command is to print its partial output.
+        raw_stderrs = result.stderr.split(self._command_separator)
+        raw_stdouts = result.stdout.split(self._command_separator)
 
         results = []
-        for i, code in enumerate(exit_codes):
-            action, _, _ = payloads[i]
+        result_i = 0
+        stdout = stderr = ''
+        code = result.exited
+
+        out_i = 0
+        err_i = 0
+        has_next = True
+        while has_next:
+            has_next = out_i < len(raw_stdouts) and err_i < len(raw_stderrs)
+            if has_next:
+                stdout = raw_stdouts[out_i]
+                stderr = raw_stderrs[err_i]
+                if result_i > 0:
+                    # cut LF from the previous "echo <separator>" command
+                    stdout = stdout[1:]
+                    stderr = stderr[1:]
+
+                has_next = out_i + 1 < len(raw_stdouts)
+                if has_next:
+                    matcher = EXIT_CODE_PATTERN.match(raw_stdouts[out_i + 1])
+                    if matcher is not None:
+                        code = int(matcher.group(1))
+                    else:
+                        has_next = False
+
+                has_next = has_next and err_i + 1 < len(raw_stderrs)
+
+            action, _, _ = payloads[result_i]
             command: str = action[1][0]
-            results.append(RunnersResult(
-                    [command], [code], stdouts[i], stderrs[i], hide=kwargs.get('hide', False)))
+            results.append(RunnersResult([command], [code], stdout, stderr, hide=hide))
+
+            stdout = stderr = ''
+            code = result.exited
+            result_i += 1
+
+            err_i += 1
+            out_i += 2
 
         return results
 
     def _get_separator(self, warn: bool) -> str:
         if warn:
             separator_symbol = ";"
         else:
@@ -455,17 +486,16 @@
                     'Executing put %s on host %s with options: %s' % (('<text>', remote_file), host, kwargs))
             else:
                 self.logger.verbose('Executing put %s on host %s with options: %s' % (args, host, kwargs))
 
             args = (local_stream, remote_file)
 
         if do_type in ('run', 'sudo'):
-            # Do not add 'timeout=self.timeout'.
-            # Though it is possible in case of only one command in the batch, it is unsafe in case of few commands.
-            # If few commands failed with timeout, we currently do not have safe algorithm to reparse the results.
+            if kwargs.get('timeout', None) is None:
+                kwargs = {**kwargs, 'timeout': static.GLOBALS['nodes']['command_execution']['timeout']}
 
             commands: List[str] = [action[1][0] for action, _, _ in payloads]
             self.logger.verbose('Executing %s %s on host %s with options: %s' % (do_type, commands, host, kwargs))
 
             precommand = ''
             if do_type == 'sudo':
                 precommand = 'sudo '
@@ -502,15 +532,19 @@
 
         for host, payloads in batch.items():
             cxn = self.connection_pool.get_connection(host)
             do_type, args, kwargs = self._prepare_merged_action(host, payloads)
             safe_exec(futures, host, lambda: tpe.submit(getattr(cxn, do_type), *args, **kwargs))
 
         for host, future in futures.items():
-            safe_exec(results, host, lambda: future.result(timeout=self.timeout))
+            # We try to shut down ThreadPoolExecutor gracefully with joining of all the threads.
+            # This makes usage of future timeout useless, as the operation is not stopped.
+            # Instead, we always pass timeout for run/sudo and so have CommandTimedOut.
+            # For put/get fabric & paramiko do not offer timeout, so transfer cannot be stopped currently.
+            safe_exec(results, host, lambda: future.result(timeout=None))
 
         self._flush_logger_writers(batch)
 
         return self._reparse_results(results, batch)
 
     def _get_remained_batch(self, batch: Dict[str, List[_PayloadItem]],
                             batch_results: Dict[str, TokenizedResult]) -> Dict[str, List[_PayloadItem]]:
```

### Comparing `kubemarine-0.28.0/kubemarine/core/flow.py` & `kubemarine-0.28.1/kubemarine/core/flow.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/core/group.py` & `kubemarine-0.28.1/kubemarine/core/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -643,19 +643,19 @@
 class NodeGroup(AbstractGroup[RunnersGroupResult]):
     def _make_group(self: NodeGroup, ips: Iterable[Union[str, NodeGroup]]) -> NodeGroup:
         return NodeGroup(ips, self.cluster)
 
     def _make_defer(self, executor: RemoteExecutor) -> DeferredGroup:
         return DeferredGroup(self.nodes, self.cluster, executor)
 
-    def new_defer(self, timeout: int = None) -> DeferredGroup:
-        return self.new_executor(timeout).group
+    def new_defer(self) -> DeferredGroup:
+        return self.new_executor().group
 
-    def new_executor(self, timeout: int = None) -> RemoteExecutor:
-        return RemoteExecutor(self, timeout=timeout)
+    def new_executor(self) -> RemoteExecutor:
+        return RemoteExecutor(self)
 
     def get(self, remote_file: str, local_file: str) -> None:
         self._do_exec("get", remote_file, local_file)
 
     def _put(self, local_stream: Union[io.BytesIO, str], remote_file: str) -> None:
         self._do_exec("put", local_stream, remote_file)
 
@@ -675,15 +675,15 @@
 
         results = self._do_exec(do_type, command, **kwargs)
         return self._unsafe_make_runners_result(results)
 
     def _do_exec(self, do_type: str, *args: object, **kwargs: Any) -> HostToResult:
         callback: Callback = kwargs.pop('callback', None)
 
-        executor = RawExecutor(self.cluster, timeout=kwargs.get('timeout'))
+        executor = RawExecutor(self.cluster)
         executor.queue(self.get_hosts(), (do_type, args, kwargs), callback=callback)
         executor.flush()
 
         results = {host: next(iter(results.values()))
                    for host, results in executor.get_last_results().items()}
 
         if any(isinstance(result, Exception) for result in results.values()):
@@ -821,16 +821,16 @@
 
     def _check_same_bound_executor(self, group: DeferredGroup) -> None:
         if self._executor is not group._executor:
             raise ValueError("Trying to apply set operation on deferred groups bound to different executors")
 
 
 class RemoteExecutor(RawExecutor):
-    def __init__(self, group: NodeGroup, connection_pool: ConnectionPool = None, timeout: int = None) -> None:
-        super().__init__(group.cluster, connection_pool, timeout)
+    def __init__(self, group: NodeGroup, connection_pool: ConnectionPool = None) -> None:
+        super().__init__(group.cluster, connection_pool)
         self.group: DeferredGroup = group._make_defer(self)
         self.cluster = group.cluster
 
     def flush(self) -> None:
         """
         Flushes the connections' queue.
         Throws GroupException in case of any failure.
```

### Comparing `kubemarine-0.28.0/kubemarine/core/log.py` & `kubemarine-0.28.1/kubemarine/core/log.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/core/os.py` & `kubemarine-0.28.1/kubemarine/core/os.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/core/patch.py` & `kubemarine-0.28.1/kubemarine/core/patch.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/core/resources.py` & `kubemarine-0.28.1/kubemarine/core/resources.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/core/schema.py` & `kubemarine-0.28.1/kubemarine/core/schema.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/core/static.py` & `kubemarine-0.28.1/kubemarine/core/static.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/core/summary.py` & `kubemarine-0.28.1/kubemarine/core/summary.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/core/utils.py` & `kubemarine-0.28.1/kubemarine/core/utils.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/core/yaml_merger.py` & `kubemarine-0.28.1/kubemarine/core/yaml_merger.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/coredns.py` & `kubemarine-0.28.1/kubemarine/coredns.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/cri/__init__.py` & `kubemarine-0.28.1/kubemarine/cri/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/cri/containerd.py` & `kubemarine-0.28.1/kubemarine/cri/containerd.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/cri/docker.py` & `kubemarine-0.28.1/kubemarine/cri/docker.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/demo.py` & `kubemarine-0.28.1/kubemarine/demo.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/etcd.py` & `kubemarine-0.28.1/kubemarine/etcd.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/haproxy.py` & `kubemarine-0.28.1/kubemarine/haproxy.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/jinja.py` & `kubemarine-0.28.1/kubemarine/jinja.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/k8s_certs.py` & `kubemarine-0.28.1/kubemarine/k8s_certs.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/keepalived.py` & `kubemarine-0.28.1/kubemarine/keepalived.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/kubernetes/__init__.py` & `kubemarine-0.28.1/kubemarine/kubernetes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -487,15 +487,18 @@
         hide=False)
 
     copy_admin_config(log, first_control_plane)
 
     kubeconfig_filepath = fetch_admin_config(cluster)
     summary.schedule_report(cluster.context, summary.SummaryItem.KUBECONFIG, kubeconfig_filepath)
 
-    # Invoke method from admission module for applying default PSS or privileged PSP if they are enabled
+    # Remove default resolvConf from kubelet-config ConfigMap for debian OS family
+    first_control_plane.call(components.patch_kubelet_configmap)
+
+    # Invoke method from admission module for applying the privileged PSP if it is enabled
     first_control_plane.call(admission.apply_admission)
 
     # Preparing join_dict to init other nodes
     control_plane_lines = list(result.values())[0].stdout. \
                        split("You can now join any number of the control-plane")[1].splitlines()[2:5]
     worker_lines = list(result.values())[0].stdout. \
                        split("Then you can join any number of worker")[1].splitlines()[2:4]
@@ -693,14 +696,18 @@
     first_control_plane.sudo(
         f"sudo kubeadm upgrade apply {version} {flags} && "
         f"sudo kubectl uncordon {node_name} && "
         f"sudo systemctl restart kubelet", hide=False)
 
     copy_admin_config(cluster.log, first_control_plane)
 
+    # In some versions, kubeadm reverts resolvConf to the default during `upgrade apply`
+    # Remove default resolvConf from kubelet-config ConfigMap for debian OS family
+    first_control_plane.call(components.patch_kubelet_configmap)
+
     expect_kubernetes_version(cluster, version, apply_filter=node_name)
     components.wait_for_pods(first_control_plane)
     exclude_node_from_upgrade_list(first_control_plane, node_name)
 
 
 def upgrade_other_control_planes(upgrade_group: NodeGroup, cluster: KubernetesCluster, **drain_kwargs: Any) -> None:
     version = cluster.inventory["services"]["kubeadm"]["kubernetesVersion"]
```

### Comparing `kubemarine-0.28.0/kubemarine/kubernetes/components.py` & `kubemarine-0.28.1/kubemarine/kubernetes/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -496,14 +496,34 @@
     defer = node.new_defer()
     for component in COMPONENTS_SUPPORT_PATCHES:
         _create_kubeadm_patches_for_component_on_node(cluster, defer, component)
 
     defer.flush()
 
 
+def patch_kubelet_configmap(control_plane: AbstractGroup[RunResult]) -> None:
+    """
+    Apply W/A until https://github.com/kubernetes/kubeadm/issues/3034 is resolved
+    for all the supported Kubernetes versions.
+
+    :param control_plane: control plane to operate on
+    """
+    # Make sure to check kubeadm_kubelet in the inventory.
+    cluster: KubernetesCluster = control_plane.cluster
+    kubeadm_config = KubeadmConfig(cluster)
+    if 'resolvConf' in kubeadm_config.maps['kubelet-config']:
+        return
+
+    configmap_name = _get_configmap_name(cluster, 'kubelet-config')
+    control_plane.sudo(
+        f'kubectl get cm -n kube-system {configmap_name} -o yaml '
+        '| grep -v "resolvConf:" '
+        '| sudo kubectl apply -f -')
+
+
 def _upload_config(cluster: KubernetesCluster, control_plane: AbstractGroup[RunResult],
                    kubeadm_config: KubeadmConfig, remote_path: str,
                    *, patches_dir: str = '/etc/kubernetes/patches') -> None:
     name = remote_path.rstrip('.yaml').split('/')[-1]
 
     init_config = get_init_config(cluster, control_plane, init=True)
     init_config['patches']['directory'] = patches_dir
@@ -554,14 +574,16 @@
     return configmap_name
 
 
 def _configmap_init_phase_uploader(configmap: str, upload_config: str) -> Callable[[DeferredGroup], None]:
     def upload(control_plane: DeferredGroup) -> None:
         init_phase = CONFIGMAPS_CONSTANTS[configmap]['init_phase']
         control_plane.run(f'sudo kubeadm init phase {init_phase} --config {upload_config}')
+        if configmap == 'kubelet-config':
+            patch_kubelet_configmap(control_plane)
 
     return upload
 
 
 def _kube_proxy_configmap_uploader(cluster: KubernetesCluster, kubeadm_config: KubeadmConfig) \
         -> Callable[[DeferredGroup], None]:
 
@@ -933,16 +955,19 @@
 
         split_logs = re.compile(r'^\[.*].*$\n', flags=re.M)
         cfg = next(filter(lambda ln: 'kind: KubeletConfiguration' in ln, split_logs.split(output)))
         cfg = dedent(cfg)
 
         key = CONFIGMAPS_CONSTANTS[configmap]['key']
         generated_config = yaml.safe_load(cfg)['data'][key]
+        if 'resolvConf' not in kubeadm_config.maps[configmap]:
+            generated_config = _filter_kubelet_configmap_resolv_conf(generated_config)
 
         kubeadm_config.load(configmap, control_plane)
+        # Use loaded_maps that preserve original formatting
         stored_config = kubeadm_config.loaded_maps[configmap].obj["data"][key]
 
         if yaml.safe_load(generated_config) == yaml.safe_load(stored_config):
             return None
 
         return utils.get_unified_diff(stored_config, generated_config,
                                       fromfile=f'{configmap} ConfigMap',
@@ -974,15 +999,19 @@
         logger.verbose(diff)
         return True
 
     return False
 
 
 def _filter_etcd_initial_cluster_args(content: str) -> str:
-    return '\n'.join(filter(lambda ln: '--initial-cluster' not in ln, content.splitlines()))
+    return '\n'.join(ln for ln in content.splitlines() if '--initial-cluster' not in ln)
+
+
+def _filter_kubelet_configmap_resolv_conf(content: str) -> str:
+    return '\n'.join(ln for ln in content.splitlines() if 'resolvConf:' not in ln)
 
 
 def _restart_containers(cluster: KubernetesCluster, node: NodeGroup, components: Sequence[str]) -> None:
     if not components:
         return
 
     logger = cluster.log
```

### Comparing `kubemarine-0.28.0/kubemarine/kubernetes/daemonset.py` & `kubemarine-0.28.1/kubemarine/kubernetes/daemonset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/kubernetes/deployment.py` & `kubemarine-0.28.1/kubemarine/kubernetes/deployment.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/kubernetes/object.py` & `kubemarine-0.28.1/kubemarine/kubernetes/object.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/kubernetes/replicaset.py` & `kubemarine-0.28.1/kubemarine/kubernetes/replicaset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/kubernetes/secrets.py` & `kubemarine-0.28.1/kubemarine/kubernetes/secrets.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/kubernetes/statefulset.py` & `kubemarine-0.28.1/kubemarine/kubernetes/statefulset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/kubernetes_accounts.py` & `kubemarine-0.28.1/kubemarine/kubernetes_accounts.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/modprobe.py` & `kubemarine-0.28.1/kubemarine/modprobe.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/packages.py` & `kubemarine-0.28.1/kubemarine/packages.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/patches/__init__.py` & `kubemarine-0.28.1/kubemarine/patches/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,18 +18,16 @@
 
 The whole directory is automatically cleared and reset after new version of Kubemarine is released.
 """
 
 from typing import List
 
 from kubemarine.core.patch import Patch
-from kubemarine.patches.disable_token_automount import DisableTokenAutomount
-from kubemarine.patches.strong_ciphers_patch import UpdateApiServerCipherSuites
+from kubemarine.patches.patch_kubelet_configmap import KubeletResolvConf
 
 patches: List[Patch] = [
-    DisableTokenAutomount(), 
-    UpdateApiServerCipherSuites(),# Add the new patch to the list
+    KubeletResolvConf(),
 ]
 """
 List of patches that is sorted according to the Patch.priority() before execution.
 Patches that have the same priority, are executed in the declared order.
 """
```

### Comparing `kubemarine-0.28.0/kubemarine/patches/software_upgrade.yaml` & `kubemarine-0.28.1/kubemarine/patches/software_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/__init__.py` & `kubemarine-0.28.1/kubemarine/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/builtin.py` & `kubemarine-0.28.1/kubemarine/plugins/builtin.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/calico.py` & `kubemarine-0.28.1/kubemarine/plugins/calico.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/kubernetes_dashboard.py` & `kubemarine-0.28.1/kubemarine/plugins/kubernetes_dashboard.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/local_path_provisioner.py` & `kubemarine-0.28.1/kubemarine/plugins/local_path_provisioner.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/manifest.py` & `kubemarine-0.28.1/kubemarine/plugins/manifest.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/nginx_ingress.py` & `kubemarine-0.28.1/kubemarine/plugins/nginx_ingress.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/calico-apiserver-v3.24.2-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-apiserver-v3.24.2-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/calico-apiserver-v3.25.1-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-apiserver-v3.25.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/calico-apiserver-v3.26.1-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-apiserver-v3.26.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/calico-apiserver-v3.26.4-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-apiserver-v3.26.4-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/calico-apiserver-v3.27.0-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-apiserver-v3.27.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/calico-v3.26.1-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.26.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/calico-v3.26.4-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.26.4-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/calico-v3.27.0-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/calico-v3.27.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.25-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.25-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.26-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.26-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.1-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.4-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.8.4-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.4-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.4-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.5-original.yaml` & `kubemarine-0.28.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.9.5-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/procedures/add_node.py` & `kubemarine-0.28.1/kubemarine/procedures/add_node.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/procedures/backup.py` & `kubemarine-0.28.1/kubemarine/procedures/backup.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/procedures/cert_renew.py` & `kubemarine-0.28.1/kubemarine/procedures/cert_renew.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/procedures/check_iaas.py` & `kubemarine-0.28.1/kubemarine/procedures/check_iaas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1368,14 +1368,61 @@
         cluster.log.debug("Delete binaries")
         with group_to_rollback.new_executor() as exe:
             for node_exe in exe.group.get_ordered_members_list():
                 node_exe.sudo(f"pkill -9 -P $(cat {ipip_check}.pid | xargs | tr ' ' ','); " \
                               f"sudo rm -f {ipip_check} {ipip_check}.pid", warn=True)
 
 
+def fs_mount_options(cluster: KubernetesCluster) -> None:
+    with TestCase(cluster, '018', 'System', 'Filesystem mount options') as tc:
+
+        failed_nodes: Set[str] = set()
+        cri_root = ""
+        # Only Kubernetes nodes should be checked
+        group = cluster.make_group_from_roles(['control-plane', 'worker']).get_sudo_nodes()
+        # Get CRI root
+        if cluster.inventory['services']['cri']['containerRuntime'] == "containerd":
+            # Containerd root
+            if cluster.inventory['services']['cri']['containerdConfig'].get('root', ""):
+                cri_root = cluster.inventory['services']['cri']['containerdConfig']['root']
+            else:
+                cri_root = "/var/lib/containerd"
+        # Get rid of that part after KubeMarine stop supporting Kubernetes version lower v1.24
+        if cluster.inventory['services']['cri']['containerRuntime'] == "docker":
+            # Docker root
+            if cluster.inventory['services']['cri']['dockerConfig'].get('data-root', ""):
+                cri_root = cluster.inventory['services']['cri']['dockerConfig']['data-root']
+            else:
+                cri_root = "/var/lib/docker"
+        if not cri_root:
+                raise TestWarn("Check cannot be completed, unknown CRI")
+        cluster.log.debug("Mount options check")
+        # Check the mount options for filesystem where containerd root is located.
+        # If containerd root doesn't exist the script check the parent directory and so forth.
+        # At the end of the script 'findmnt' return the filesytem mount point, device,
+        # and mount options for nearest parent directory of CRI root.
+        # 'findmnt' perform the recursive search of mount point for filesystem
+        # from the given path to the root, that's exactly what we need.
+        cmd = f"CRI_PATH={cri_root}; while [ ! -d \"${{CRI_PATH}}\" ]; do CRI_PATH=$(dirname \"${{CRI_PATH}}\"); " \
+              f"done; findmnt -T \"${{CRI_PATH}}\" | grep 'nosuid'"
+        results = group.run(f"{cmd}", warn=True)
+
+        # Check output and create result message
+        for host, item in results.items():
+            node_name = cluster.get_node_name(host)
+            if len(item.stdout) > 0:
+                failed_nodes.add(f"{node_name}")
+
+        if failed_nodes:
+            raise TestFailure(f"The 'nosuid' mount option affects container functionality. "
+                              f"Please change mount options for filesystem where CRI "
+                              f"root is located on the following nodes. CRI root path is '{cri_root}'",
+                              hint='\n'.join(failed_nodes))
+
+
 def make_reports(context: dict, testsuite: TestSuite) -> None:
     if not context['execution_arguments'].get('disable_csv_report', False):
         testsuite.save_csv(context['execution_arguments']['csv_report'], context['execution_arguments']['csv_report_delimiter'])
     if not context['execution_arguments'].get('disable_html_report', False):
         testsuite.save_html(context['execution_arguments']['html_report'], context['initial_procedure'].upper())
 
 
@@ -1408,18 +1455,19 @@
             'control-planes': lambda cluster: hardware_cpu(cluster, 'control-plane'),
             'workers': lambda cluster: hardware_cpu(cluster, 'worker')
         },
         'ram': {
             'balancers': lambda cluster: hardware_ram(cluster, 'balancer'),
             'control-planes': lambda cluster: hardware_ram(cluster, 'control-plane'),
             'workers': lambda cluster: hardware_ram(cluster, 'worker')
-        }
+        },
     },
     'system': {
-        'distributive': system_distributive
+        'distributive': system_distributive,
+        'fs_mount_options': fs_mount_options
     },
     'software': {
         'kernel': {
             'version': check_kernel_version
         },
         'thirdparties': {
             'availability': check_access_to_thirdparties
```

### Comparing `kubemarine-0.28.0/kubemarine/procedures/check_paas.py` & `kubemarine-0.28.1/kubemarine/procedures/check_paas.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/procedures/config.py` & `kubemarine-0.28.1/kubemarine/procedures/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,27 +54,31 @@
     format_ = arguments['output']
     if format_ == 'yaml':
         print(yaml.safe_dump(cfg, sort_keys=False), end='')
     elif format_ == 'json':
         print(json.dumps(cfg, indent=4))
 
 
-def main(cli_arguments: List[str] = None) -> None:
+def create_context(cli_arguments: List[str] = None) -> dict:
     if cli_arguments is None:
         cli_arguments = sys.argv[1:]
 
     parser = argparse.ArgumentParser(formatter_class=argparse.RawTextHelpFormatter,
                                      prog='config',
                                      description=HELP_DESCRIPTION)
 
     parser.add_argument('-o', '--output',
                         choices=['yaml', 'json'], default='yaml',
                         help='output format')
 
     arguments = vars(parser.parse_args(cli_arguments))
+    return {'config_arguments': arguments}
+
 
+def main(cli_arguments: List[str] = None) -> None:
+    arguments = create_context(cli_arguments)['config_arguments']
     cfg = make_config()
     print_config(cfg, arguments)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `kubemarine-0.28.0/kubemarine/procedures/do.py` & `kubemarine-0.28.1/kubemarine/procedures/do.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/procedures/install.py` & `kubemarine-0.28.1/kubemarine/procedures/install.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/procedures/manage_psp.py` & `kubemarine-0.28.1/kubemarine/procedures/manage_psp.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/procedures/manage_pss.py` & `kubemarine-0.28.1/kubemarine/procedures/manage_pss.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/procedures/migrate_cri.py` & `kubemarine-0.28.1/kubemarine/procedures/migrate_cri.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/procedures/migrate_kubemarine.py` & `kubemarine-0.28.1/kubemarine/procedures/migrate_kubemarine.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/procedures/reboot.py` & `kubemarine-0.28.1/kubemarine/procedures/reboot.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/procedures/reconfigure.py` & `kubemarine-0.28.1/kubemarine/procedures/reconfigure.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/procedures/remove_node.py` & `kubemarine-0.28.1/kubemarine/procedures/remove_node.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/procedures/restore.py` & `kubemarine-0.28.1/kubemarine/procedures/restore.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/procedures/upgrade.py` & `kubemarine-0.28.1/kubemarine/procedures/upgrade.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/__init__.py` & `kubemarine-0.28.1/kubemarine/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/configurations/__init__.py` & `kubemarine-0.28.1/kubemarine/resources/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml` & `kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml` & `kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/internal/packages.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml` & `kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/internal/plugins.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml` & `kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml` & `kubemarine-0.28.1/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/configurations/defaults.yaml` & `kubemarine-0.28.1/kubemarine/resources/configurations/defaults.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/configurations/globals.yaml` & `kubemarine-0.28.1/kubemarine/resources/configurations/globals.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/drop_ins/__init__.py` & `kubemarine-0.28.1/kubemarine/resources/drop_ins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/etalons/patches/__init__.py` & `kubemarine-0.28.1/kubemarine/resources/etalons/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/etalons/patches/software_upgrade.yaml` & `kubemarine-0.28.1/kubemarine/resources/etalons/patches/software_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/psp/__init__.py` & `kubemarine-0.28.1/kubemarine/resources/psp/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/psp/anyuid.yaml` & `kubemarine-0.28.1/kubemarine/resources/psp/anyuid.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/psp/default.yaml` & `kubemarine-0.28.1/kubemarine/resources/psp/default.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/psp/host-network.yaml` & `kubemarine-0.28.1/kubemarine/resources/psp/host-network.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/psp/privileged.yaml` & `kubemarine-0.28.1/kubemarine/resources/psp/privileged.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/reports/__init__.py` & `kubemarine-0.28.1/kubemarine/resources/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/reports/check_report.css` & `kubemarine-0.28.1/kubemarine/resources/reports/check_report.css`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/backup.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/backup.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/cert_renew.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/cert_renew.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/cluster.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/cluster.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/common/node_ref.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/common/node_ref.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/common/utils.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/common/utils.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/gateway_node.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/gateway_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/globals.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/globals.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/node.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/node_defaults.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/node_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugin_defaults.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugin_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/calico.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/calico.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/config.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/expect.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/helm.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/python.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/shell.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation/template.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/installation.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/installation.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/plugins.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/plugins.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/procedures.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/procedures.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/rbac/account.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac/account.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac/account_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/rbac/psp.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac/psp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/rbac/pss.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac/pss.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/rbac.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/rbac.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/registry.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/registry.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/audit.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/audit.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/coredns.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/coredns.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/cri.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/cri.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/etc_hosts.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/kernel_security.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/kernel_security.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/kubeadm.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/kubeadm.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/kubeadm_kube-proxy.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/kubeadm_kube-proxy.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/loadbalancer.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/modprobe.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/modprobe.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/ntp.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/ntp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/packages/associations.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/packages/associations.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/packages.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/packages.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/sysctl.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/sysctl.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services/thirdparties.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services/thirdparties.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/services.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/services.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/definitions/vrrp_ip.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/definitions/vrrp_ip.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/manage_psp.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/manage_psp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/manage_pss.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/manage_pss.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/migrate_cri.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/migrate_cri.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/migrate_kubemarine.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/migrate_kubemarine.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/reboot.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/reboot.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/reconfigure.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/reconfigure.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/remove_node.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/remove_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/restore.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/restore.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/schemas/upgrade.json` & `kubemarine-0.28.1/kubemarine/resources/schemas/upgrade.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/scripts/__init__.py` & `kubemarine-0.28.1/kubemarine/resources/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/scripts/check_url_availability.py` & `kubemarine-0.28.1/kubemarine/resources/scripts/check_url_availability.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/scripts/etcdctl.sh` & `kubemarine-0.28.1/kubemarine/resources/scripts/etcdctl.sh`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/scripts/ipip_check.gz` & `kubemarine-0.28.1/kubemarine/resources/scripts/ipip_check.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipip_check", last modified: Mon Mar 11 11:18:44 2024, from Unix
+gzip compressed data, was "ipip_check", last modified: Mon Apr  1 09:25:00 2024, from Unix
```

### Comparing `kubemarine-0.28.0/kubemarine/resources/scripts/simple_port_client.py` & `kubemarine-0.28.1/kubemarine/resources/scripts/simple_port_client.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/scripts/simple_port_listener.py` & `kubemarine-0.28.1/kubemarine/resources/scripts/simple_port_listener.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/scripts/source/ipip_check/go.sum` & `kubemarine-0.28.1/kubemarine/resources/scripts/source/ipip_check/go.sum`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/resources/scripts/source/ipip_check/ipip_check.go` & `kubemarine-0.28.1/kubemarine/resources/scripts/source/ipip_check/ipip_check.go`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/selinux.py` & `kubemarine-0.28.1/kubemarine/selinux.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/sysctl.py` & `kubemarine-0.28.1/kubemarine/sysctl.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/system.py` & `kubemarine-0.28.1/kubemarine/system.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/templates/__init__.py` & `kubemarine-0.28.1/kubemarine/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/templates/admission.yaml.j2` & `kubemarine-0.28.1/kubemarine/templates/admission.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/templates/haproxy.cfg.j2` & `kubemarine-0.28.1/kubemarine/templates/haproxy.cfg.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/templates/keepalived.conf.j2` & `kubemarine-0.28.1/kubemarine/templates/keepalived.conf.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/templates/kubelet.service.j2` & `kubemarine-0.28.1/kubemarine/templates/kubelet.service.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/templates/plugins/__init__.py` & `kubemarine-0.28.1/kubemarine/templates/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/templates/plugins/calico-ippool.yaml.j2` & `kubemarine-0.28.1/kubemarine/templates/plugins/calico-ippool.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/templates/plugins/calico-rr.yaml.j2` & `kubemarine-0.28.1/kubemarine/templates/plugins/calico-rr.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2` & `kubemarine-0.28.1/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2` & `kubemarine-0.28.1/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/templates/plugins/iperf3.yaml.j2` & `kubemarine-0.28.1/kubemarine/templates/plugins/iperf3.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2` & `kubemarine-0.28.1/kubemarine/templates/plugins/local-path-provisioner.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2` & `kubemarine-0.28.1/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2` & `kubemarine-0.28.1/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/testsuite.py` & `kubemarine-0.28.1/kubemarine/testsuite.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/thirdparties.py` & `kubemarine-0.28.1/kubemarine/thirdparties.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine/yum.py` & `kubemarine-0.28.1/kubemarine/yum.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.28.0/kubemarine.egg-info/PKG-INFO` & `kubemarine-0.28.1/kubemarine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubemarine
-Version: 0.28.0
+Version: 0.28.1
 Summary: Management tool for Kubernetes cluster deployment and maintenance
 Home-page: https://github.com/Netcracker/KubeMarine
 Author-email: Kubemarine Group <kubemarinegroup@netcracker.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Netcracker/KubeMarine
 Project-URL: Documentation, https://github.com/Netcracker/KubeMarine#documentation
 Project-URL: Issues, https://github.com/Netcracker/KubeMarine/issues/
@@ -61,38 +61,38 @@
 
 # Kubemarine
 
 Kubemarine is an open source, lightweight and powerful management tool built for end-to-end Kubernetes cluster deployment and maintenance. It is applicable for many purposes like simple and quick onboarding Kubernetes on local and production environments in different HA schemes depending on your aims, budget, and capabilities. Together with simplicity, Kubemarine can be a very flexible and customizable tool covering specific configurability cases on both deployment and maintenance stages. This library provides powerful CLI commands, as well as can be customized using a Python extension API.
 
 ## Highlights
 - Easy to use
-- Many procedures supported following the [generic maintenance approach](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#basics):
-  - [install](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#)
-  - [add_node](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#add-node-procedure)
-  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#remove-node-procedure)
-  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#upgrade-procedure)
-  - [backup](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#backup-procedure)
-  - [restore](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#restore-procedure)
-  - [reconfigure](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#reconfigure-procedure)
-  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Kubecheck.md#iaas-procedure)
-  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Kubecheck.md#paas-procedure)
-  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#kubemarine-migration-procedure)
-  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#manage-psp-procedure)
-  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#manage-pss-procedure)
-  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#certificate-renew-procedure)
-  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md#cri-migration-procedure)
-- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#configuration) for all operations, highly customizable
+- Many procedures supported following the [generic maintenance approach](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#basics):
+  - [install](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#)
+  - [add_node](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#add-node-procedure)
+  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#remove-node-procedure)
+  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#upgrade-procedure)
+  - [backup](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#backup-procedure)
+  - [restore](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#restore-procedure)
+  - [reconfigure](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#reconfigure-procedure)
+  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Kubecheck.md#iaas-procedure)
+  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Kubecheck.md#paas-procedure)
+  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#kubemarine-migration-procedure)
+  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#manage-psp-procedure)
+  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#manage-pss-procedure)
+  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#certificate-renew-procedure)
+  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md#cri-migration-procedure)
+- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#configuration) for all operations, highly customizable
 - Default values of all parameters in configurations with a minimum of required parameters
-- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
-- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
-- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#custom-plugins-installation-procedures) support
-- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#installation-without-internet-resources) with private registries
-- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#dump-files)
+- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
+- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
+- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#custom-plugins-installation-procedures) support
+- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#installation-without-internet-resources) with private registries
+- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#dump-files)
 - Build supported as a package, container, and binary
-- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/PackageExtension.md)
+- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/PackageExtension.md)
 - Support different deployment schemes (all-in-one, mini-HA, HA, and so on)
 
 ## Kubemarine Binary Installation
 Proceed the following steps to install Kubemarine  on your environment:
 1. Download the binary file for your system from the latest [release](https://github.com/Netcracker/KubeMarine/releases)
 2. Move binary kubemarine to a separate folder 
 3. Now you can proceed to run Kubemarine! Try the following:
@@ -110,15 +110,15 @@
    ```bash
    python3 -m pip install --upgrade pip
    ```
    Windows:
    ```bash
    python -m pip install --upgrade pip
    ```
-1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#prerequisites-for-deployment-node).
+1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#prerequisites-for-deployment-node).
 1. Create and activate a [virtual environment](https://realpython.com/python-virtual-environments-a-primer/) if necessary.
 1. Install Kubemarine package.
 
    Linux / MacOS:
    ```bash
    python3 -m pip install kubemarine
    ```
@@ -129,15 +129,15 @@
 1. Now you can proceed to run Kubemarine! Try the following:
    ```bash
    kubemarine help
    ```
 
 
 ## Kubemarine Installation from Sources
-Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/README.md#kubemarine-package-installation).
+Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/README.md#kubemarine-package-installation).
 The exception is instead of installing the package from [PyPI](https://pypi.org/project/kubemarine/), do the following:
 1. [Download the latest release](https://github.com/netcracker/kubemarine/releases) or clone the repository:
    ```bash
    git clone https://github.com/netcracker/kubemarine.git
    ```
 1. Unpack the project from the archive if required:
    ```bash
@@ -158,24 +158,24 @@
    python -m pip install -e .
    ```
 1. Now you can proceed to run Kubemarine. Try the following:
     ```bash
     kubemarine help
     ```
 
-**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/Dockerfile) is also available.
+**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/Dockerfile) is also available.
 
 
 **Note:** Kubemarine debugging available via `kubemarine/__main__.py`.
 
 
 ## Running Cluster Installation
 To install a Kubernetes cluster using Kubemarine:
-1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
-1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
+1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#prerequisites-for-cluster-nodes).
+1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
    ```yaml
    node_defaults:
      keyfile: "/home/username/.ssh/id_rsa"
      password: '{{ env.PASS }}'     #Either keyfile or password can be used.
      username: "centos"
 
    vrrp_ips:
@@ -204,42 +204,42 @@
    kubemarine install
    ```
 1. Check the health of the newly installed cluster:
    ```bash
    kubemarine check_paas
    ```
 
-For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/README.md#documentation).
+For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/README.md#documentation).
 
 ## Kubemarine Docker Installation
 To start, download the Kubmarine image ```docker pull ghcr.io/netcracker/kubemarine:main```
 
 Run Kubemarine from the container, for example:
    ```
    docker run -it --mount type=bind,source=/root/cluster.yaml,target=/opt/kubemarine/cluster.yaml --mount type=bind,source=/root/rsa_key,target=/opt/kubemarine/rsa_key kubemarine install -c /opt/kubemarine/cluster.yaml
    ```
    *Note*: Do not forget to pass the inventory file and connection key inside the container.
    For more execution details, refer to ["Installation of Kubernetes using CLI" guide on Github](https://github.com/Netcracker/kubemarine/blob/main/documentation/Installation.md#installation-of-kubernetes-using-cli).
 
 ## Documentation
 The following documents and tutorials are available:
-- [Installation](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Installation.md)
-- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Maintenance.md)
-- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Troubleshooting.md)
-- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Kubecheck.md)
-- [Logging](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/documentation/Logging.md)
+- [Installation](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Installation.md)
+- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Maintenance.md)
+- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Troubleshooting.md)
+- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Kubecheck.md)
+- [Logging](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/documentation/Logging.md)
 
 Also, check out the following inventory examples:
-- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/examples/cluster.yaml)
-- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/examples/procedure.yaml)
+- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/examples/cluster.yaml)
+- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/examples/procedure.yaml)
 
 ## Issues, Questions
 If you have any problems while working with Kubemarine, feel free to open a [new issue](https://github.com/netcracker/kubemarine/issues) or even
 [PR](https://github.com/netcracker/kubemarine/pulls) with related changes.
-Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
+Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
 
-In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/SECURITY.md)
+In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/SECURITY.md)
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/netcracker/kubemarine/releases).
 
 ## License
-[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/v0.28.0/LICENSE)
+[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/v0.28.1/LICENSE)
```

### Comparing `kubemarine-0.28.0/kubemarine.egg-info/SOURCES.txt` & `kubemarine-0.28.1/kubemarine.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -64,17 +64,16 @@
 kubemarine/kubernetes/daemonset.py
 kubemarine/kubernetes/deployment.py
 kubemarine/kubernetes/object.py
 kubemarine/kubernetes/replicaset.py
 kubemarine/kubernetes/secrets.py
 kubemarine/kubernetes/statefulset.py
 kubemarine/patches/__init__.py
-kubemarine/patches/disable_token_automount.py
+kubemarine/patches/patch_kubelet_configmap.py
 kubemarine/patches/software_upgrade.yaml
-kubemarine/patches/strong_ciphers_patch.py
 kubemarine/plugins/__init__.py
 kubemarine/plugins/builtin.py
 kubemarine/plugins/calico.py
 kubemarine/plugins/kubernetes_dashboard.py
 kubemarine/plugins/local_path_provisioner.py
 kubemarine/plugins/manifest.py
 kubemarine/plugins/nginx_ingress.py
```

### Comparing `kubemarine-0.28.0/pyproject.toml` & `kubemarine-0.28.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 Documentation = "https://github.com/Netcracker/KubeMarine#documentation"
 Issues = "https://github.com/Netcracker/KubeMarine/issues/"
 
 # To change version with automatic push and triggering of the release workflow use
 # 1. pip install bumpver
 # 2. bumpver update --set-version <new version>
 [tool.bumpver]
-current_version = "v0.28.0"
+current_version = "v0.28.1"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version to {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `kubemarine-0.28.0/setup.py` & `kubemarine-0.28.1/setup.py`

 * *Files identical despite different names*

