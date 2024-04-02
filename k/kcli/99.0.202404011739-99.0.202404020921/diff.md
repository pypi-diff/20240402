# Comparing `tmp/kcli-99.0.202404011739.tar.gz` & `tmp/kcli-99.0.202404020921.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kcli-99.0.202404011739.tar", last modified: Mon Apr  1 17:39:25 2024, max compression
+gzip compressed data, was "kcli-99.0.202404020921.tar", last modified: Tue Apr  2 09:21:59 2024, max compression
```

## Comparing `kcli-99.0.202404011739.tar` & `kcli-99.0.202404020921.tar`

### file list

```diff
@@ -1,788 +1,788 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.951519 kcli-99.0.202404011739/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-01 17:39:25.951519 kcli-99.0.202404011739/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.859520 kcli-99.0.202404011739/extras/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/Dockerfile_curl
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/Dockerfile_kubectl
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/autoscale.yml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/aws_peering.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/aws_peering_cleaning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.859520 kcli-99.0.202404011739/extras/controller/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/controller/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/controller/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/controller/crd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/controller/deploy.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.863520 kcli-99.0.202404011739/extras/controller/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/controller/examples/cluster_simple.yml
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/controller/examples/plan_complex.yml
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/controller/examples/plan_simple.yml
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/controller/examples/plan_simple_with_file.yml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/controller/examples/vm_centos8stream.yml
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/controller/examples/vm_cirros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/controller/examples/vm_empty.yml
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/controller/examples/vm_fedora.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9970 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/controller/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/controller/stress_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/debian
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.863520 kcli-99.0.202404011739/extras/expose/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/expose/kcli.conf
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/expose/kcli.wsgi
--rwxr-xr-x   0 runner    (1001) docker     (127)      106 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/genrst.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/haproxy.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/haproxy_multiple_clusters.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/i_am_a_container
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/k8sdeploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/kfish.md
--rw-r--r--   0 runner    (1001) docker     (127)    38837 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/kfish.png
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/missing_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/openstack.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/openstack.sh.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/extras/zerotier.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.863520 kcli-99.0.202404011739/kcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-01 17:39:25.000000 kcli-99.0.202404011739/kcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27395 2024-04-01 17:39:25.000000 kcli-99.0.202404011739/kcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 17:39:25.000000 kcli-99.0.202404011739/kcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-01 17:39:25.000000 kcli-99.0.202404011739/kcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 17:36:27.000000 kcli-99.0.202404011739/kcli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-01 17:39:25.000000 kcli-99.0.202404011739/kcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 17:39:25.000000 kcli-99.0.202404011739/kcli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.867520 kcli-99.0.202404011739/kvirt/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.867520 kcli-99.0.202404011739/kvirt/ansibleutils/
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/ansibleutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    98843 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/baseconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)   171487 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/bottle.py
--rw-r--r--   0 runner    (1001) docker     (127)   277696 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.867520 kcli-99.0.202404011739/kvirt/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.867520 kcli-99.0.202404011739/kvirt/cluster/aks/
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/aks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/aks/fake.yml
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/aks/kcli_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.867520 kcli-99.0.202404011739/kvirt/cluster/eks/
--rw-r--r--   0 runner    (1001) docker     (127)    12290 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/eks/fake.yml
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/eks/kcli_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.867520 kcli-99.0.202404011739/kvirt/cluster/gke/
--rw-r--r--   0 runner    (1001) docker     (127)    12249 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/gke/fake.yml
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/gke/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/gke/kubeconfig.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.871520 kcli-99.0.202404011739/kvirt/cluster/hypershift/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/99-apps.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/99-forcedns
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/99-notifications.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/Corefile
--rw-r--r--   0 runner    (1001) docker     (127)    46322 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/assisted_infra.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/assisted_ingress.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/autoapprovercron.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/bmc.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/calico.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/cilium.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/cloud_lb_apps.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/disconnected.sh
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/extras.service
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/extras.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/hostedcluster.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/httpd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/ignition.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/kcli_plan.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/kcli_plan_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/keepalived.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/nmstateconfig.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/nodepool.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/nonlocalbind.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.871520 kcli-99.0.202404011739/kvirt/cluster/hypershift/staticpods/
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/staticpods/coredns.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/staticpods/keepalived.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/hypershift/staticpods/mdns.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.871520 kcli-99.0.202404011739/kvirt/cluster/k3s/
--rw-r--r--   0 runner    (1001) docker     (127)    13877 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/k3s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/k3s/bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/k3s/bootstrap.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/k3s/cloud_lb_api.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/k3s/ctlplanes.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/k3s/ctlplanes.yml
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/k3s/join.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/k3s/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/k3s/keepalived.conf
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/k3s/keepalived.sh
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/k3s/workers.sh
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/k3s/workers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.875520 kcli-99.0.202404011739/kvirt/cluster/kubeadm/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/10-flannel.link
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/90-flannel.rules
--rw-r--r--   0 runner    (1001) docker     (127)    14207 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.847520 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.875520 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/argocd/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/argocd/ingress.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/argocd/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/argocd/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/argocd/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.875520 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/autolabeller/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/autolabeller/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/autolabeller/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.875520 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/certmanager/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/certmanager/install.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.879520 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/dashboard/admin.yml
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/dashboard/ingress.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/dashboard/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/dashboard/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/dashboard/user.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.879520 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/falco/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/falco/falco_advertisements.yml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/falco/falco_ip.yml
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/falco/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/falco/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/falco/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.879520 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/ingress/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/ingress/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/ingress/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.879520 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/istio/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/istio/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/istio/istio-minimal-operator.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.879520 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/katacontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/katacontainer/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/katacontainer/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.879520 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/knative/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/knative/cr_eventing.yml
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/knative/cr_serving.yml
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/knative/install.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.879520 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/kubevirt/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/kubevirt/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/kubevirt/kcli_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.879520 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/metallb/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/metallb/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/metallb/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/metallb/metallb_advertisement.yml
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/metallb/metallb_cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/metallb/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.879520 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/olm/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/olm/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/olm/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.879520 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/policy_as_code/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/policy_as_code/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/policy_as_code/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/policy_as_code/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.883520 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/rancher/
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/rancher/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/rancher/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/rancher/rancher_advertisements.yml
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/rancher/rancher_ip.yml
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/rancher/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.883520 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/rook/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/rook/install.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.883520 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/submariner/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/submariner/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/submariner/kcli_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.883520 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/tekton/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/tekton/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/tekton/uninstall.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     3158 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/bootstrap.yml
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/cloud_lb_api.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/crictl.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/ctlplanes.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      343 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/deploy.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      598 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/join.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/keepalived.conf
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/keepalived.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/nfs.sh
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/nfs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/pre_el.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/pre_ubuntu.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/registry.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubeadm/workers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.883520 kcli-99.0.202404011739/kvirt/cluster/kubecommon/
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubecommon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.883520 kcli-99.0.202404011739/kvirt/cluster/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/kubernetes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.883520 kcli-99.0.202404011739/kvirt/cluster/microshift/
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/microshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/microshift/kcli_plan.yml
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/microshift/kcli_plan_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.883520 kcli-99.0.202404011739/kvirt/cluster/microshift/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/microshift/scripts/00_sslip.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/microshift/scripts/01_clients.sh
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/microshift/scripts/02_crio.sh
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/microshift/scripts/03_microshift.sh
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/microshift/scripts/04_kubeconfig.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/microshift/scripts/05_acm.sh
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/microshift/scripts/deploy.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.891520 kcli-99.0.202404011739/kvirt/cluster/openshift/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/01-workload-partitioning
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/10-node-ip-hint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/20-localhost-fix.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/99-apps.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/99-autologin.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/99-bootstrap-deletion-2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/99-bootstrap-deletion.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/99-chrony.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/99-forcedns
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/99-forcedns-ibm
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/99-kubevirt-fix.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/99-metal3-fake-machine.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/99-metal3-provisioning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/99-notifications.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/99-operatorhub.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/99-ovn.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/99-sno.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/Corefile
--rwxr-xr-x   0 runner    (1001) docker     (127)    96956 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.891520 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.895520 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/advanced-cluster-management/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/advanced-cluster-management/99-metal3-provisioning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sample.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2839 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sh
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/advanced-cluster-management/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/advanced-cluster-management/gen_registries.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/advanced-cluster-management/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/advanced-cluster-management/post.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.895520 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/argocd/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/argocd/configmap.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/argocd/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/argocd/kcli_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.895520 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/autolabeller/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/autolabeller/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/autolabeller/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/autolabeller/install.yml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/autolabeller/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/autolabeller/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.895520 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/cluster-logging/
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/cluster-logging/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/cluster-logging/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/cr.sh
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/install.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.895520 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/istio/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/istio/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/istio/istio-cni.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.895520 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/kubernetes-nmstate-operator/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/kubernetes-nmstate-operator/cr.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.895520 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/kcli_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.895520 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/local-storage-operator/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/local-storage-operator/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/local-storage-operator/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/local-storage-operator/post.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.895520 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/lvms-operator/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/lvms-operator/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/lvms-operator/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/lvms-operator/post.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.895520 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/metallb-operator/
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/metallb-operator/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/metallb-operator/kcli_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.899520 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/multicluster-engine/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/multicluster-engine/99-metal3-provisioning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sample.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2846 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sh
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/multicluster-engine/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/multicluster-engine/gen_registries.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/multicluster-engine/kcli_default.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)       55 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/multicluster-engine/post.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.899520 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/nfs/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2297 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/nfs/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/nfs/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/nfs/uninstall.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.899520 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/odf-operator/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/odf-operator/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/odf-operator/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/odf-operator/nad_cluster.yml
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/odf-operator/nad_public.yml
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/odf-operator/post.sh
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/odf-operator/pre.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.899520 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/serverless-operator/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/serverless-operator/cr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/serverless-operator/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/serverless-operator/post.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.899520 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/users/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/users/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/users/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/users/oauth.yml
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/users/oauth_hypershift.yml
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/apps/users/uninstall.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/autoapprovercron.yml
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/autorules.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/bootstrap.yml
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/calico.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/chrony.conf
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/cilium.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/cloud_bootstrap.yml
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/cloud_ctlplanes.yml
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/cloud_dns.yml
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/cloud_lb_api.yml
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/cloud_lb_apps.yml
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/cloud_workers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/cluster-ingress-02-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/cluster-scheduler-02-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/config.hcl.templ
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/ctlplanes.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.899520 kcli-99.0.202404011739/kvirt/cluster/openshift/customisation/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/customisation/00-kcli-namespace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/customisation/97-autoapprovercron-sa.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/customisation/98-autoapprovercron-binding.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/customisation/99-autoapprovercron-cronjob.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/customisation/99-ingress-controller.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/customisation/99-iptables.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/customisation/99-monitoring.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/customisation/99-registry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/dhcp.conf
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/dhcp.sh
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/dhcp.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.899520 kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.899520 kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      357 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected/bin/sync_image.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected/haproxy.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected/registry.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.903519 kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      201 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected/scripts/01_get_oc.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      243 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected/scripts/02_packages.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2412 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected/scripts/03_mirror.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2101 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected/scripts/03_registry.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      331 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected/scripts/04_extras.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2349 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected/scripts/05_olm.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      197 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected/scripts/06_web.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      841 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected/scripts/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected/scripts/mirror-config.yaml.sample
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/fake_kubeconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/fake_pull.json
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/haproxy.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/haproxy.cfg.kubevirt
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/httpd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/icsp.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/ignition.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/install-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/iso.sh
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/kcli-ipv6.conf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/kcli_default.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/keepalived.conf
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/nonlocalbind.conf
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/openshift-workload-pinning
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/patch_ipv6.json
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/relocate-ip-bootstrap.service
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/relocate-ip-bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/relocate-ip.sh
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/sno-finish.service
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/sno-finish.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/sno.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/sno_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.903519 kcli-99.0.202404011739/kvirt/cluster/openshift/staticpods/
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/staticpods/coredns.yml
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/staticpods/haproxy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/staticpods/keepalived.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/staticpods/mdns.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/openshift/workers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.903519 kcli-99.0.202404011739/kvirt/cluster/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/profiles/sample-kubeadm-default.yml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/profiles/sample-openshift-compact.yml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/profiles/sample-openshift-contrail.yml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/profiles/sample-openshift-ipv6.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/profiles/sample-openshift-sno-bm.yml
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/profiles/sample-openshift-sno.yml
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/cluster/sampleprovider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.907519 kcli-99.0.202404011739/kvirt/common/
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/common/Jenkinsfile.j2
--rw-r--r--   0 runner    (1001) docker     (127)   105808 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/common/autoscale.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/common/fake_kubeconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/common/ignition.j2
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/common/kubevirt_kcli_conf.j2
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/common/local_kcli_conf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/common/pipeline.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/common/pipeline_kube.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/common/playbook.j2
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/common/storage.sh.aws
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/common/storage.sh.gcp
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/common/storage.sh.ibmcloud
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/common/vm.ovf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/common/workflow.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/common/workflow_script.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)   190877 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.907519 kcli-99.0.202404011739/kvirt/container/
--rw-r--r--   0 runner    (1001) docker     (127)    14188 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/containerconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/defaults.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1475 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/ekstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    25462 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.907519 kcli-99.0.202404011739/kvirt/expose/
--rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.851520 kcli-99.0.202404011739/kvirt/expose/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.907519 kcli-99.0.202404011739/kvirt/expose/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/static/css/bootstrap-notify.css
--rw-r--r--   0 runner    (1001) docker     (127)   121125 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/static/css/dataTables.checkboxes.css
--rw-r--r--   0 runner    (1001) docker     (127)    13587 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/static/css/jquery.dataTables.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/static/css/kcli.css
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/static/css/wheel.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.907519 kcli-99.0.202404011739/kvirt/expose/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/static/images/sort_asc.png
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/static/images/sort_both.png
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/static/images/sort_desc.png
--rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/static/images/wheel.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.907519 kcli-99.0.202404011739/kvirt/expose/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/static/js/dataTables.checkboxes.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/static/js/exposeactions.js
--rw-r--r--   0 runner    (1001) docker     (127)    83059 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/static/js/jquery.dataTables.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    89795 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/static/js/list.js
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/swagger.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.911519 kcli-99.0.202404011739/kvirt/expose/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/templates/form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/templates/head.html
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/templates/infoplan.html
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/templates/planstable.html
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/expose/templates/result.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/gketoken.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4333 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/ignitionmerger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.911519 kcli-99.0.202404011739/kvirt/internalplans/
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/internalplans/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.911519 kcli-99.0.202404011739/kvirt/jinjafilters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/jinjafilters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/jinjafilters/jinjafilters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/keywords.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.911519 kcli-99.0.202404011739/kvirt/kfish/
--rw-r--r--   0 runner    (1001) docker     (127)    12858 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/kfish/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3395 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/klist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.911519 kcli-99.0.202404011739/kvirt/ksushy/
--rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/ksushy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      121 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/ksushy/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.911519 kcli-99.0.202404011739/kvirt/ksushy/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/ksushy/templates/bios.json
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/ksushy/templates/interface.json
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/ksushy/templates/interfaces.json
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/ksushy/templates/manager.json
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/ksushy/templates/managers.json
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/ksushy/templates/root.json
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/ksushy/templates/system.json
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/ksushy/templates/systems.json
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/ksushy/templates/virtualmedia_cd.json
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/ksushy/templates/virtualmedias.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.911519 kcli-99.0.202404011739/kvirt/miniconsole/
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/miniconsole/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.911519 kcli-99.0.202404011739/kvirt/nameutils/
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/nameutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.911519 kcli-99.0.202404011739/kvirt/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.911519 kcli-99.0.202404011739/kvirt/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (127)   106119 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/aws/assume_policy.json
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/aws/ctlplane_policy.json
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/aws/worker_policy.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.911519 kcli-99.0.202404011739/kvirt/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)    78530 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.911519 kcli-99.0.202404011739/kvirt/providers/fake/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/fake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.915519 kcli-99.0.202404011739/kvirt/providers/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)    99391 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/gcp/gcp-hack.service
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/gcp/gcp-hack.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.915519 kcli-99.0.202404011739/kvirt/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)    65793 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/ibm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.915519 kcli-99.0.202404011739/kvirt/providers/kubevirt/
--rw-r--r--   0 runner    (1001) docker     (127)    86428 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/kubevirt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.915519 kcli-99.0.202404011739/kvirt/providers/kvm/
--rw-r--r--   0 runner    (1001) docker     (127)   186412 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/kvm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/kvm/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.915519 kcli-99.0.202404011739/kvirt/providers/openstack/
--rw-r--r--   0 runner    (1001) docker     (127)    58301 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/openstack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.915519 kcli-99.0.202404011739/kvirt/providers/ovirt/
--rw-r--r--   0 runner    (1001) docker     (127)    63291 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/ovirt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.915519 kcli-99.0.202404011739/kvirt/providers/packet/
--rw-r--r--   0 runner    (1001) docker     (127)    31823 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/packet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.915519 kcli-99.0.202404011739/kvirt/providers/proxmox/
--rw-r--r--   0 runner    (1001) docker     (127)    35211 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/proxmox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/sampleprovider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.915519 kcli-99.0.202404011739/kvirt/providers/vsphere/
--rw-r--r--   0 runner    (1001) docker     (127)    73908 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/vsphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13503 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/vsphere/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/vsphere/tagging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.915519 kcli-99.0.202404011739/kvirt/providers/web/
--rw-r--r--   0 runner    (1001) docker     (127)    22043 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/providers/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.915519 kcli-99.0.202404011739/kvirt/version/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-01 17:39:25.000000 kcli-99.0.202404011739/kvirt/version/git
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.915519 kcli-99.0.202404011739/kvirt/web/
--rwxr-xr-x   0 runner    (1001) docker     (127)    46680 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.855520 kcli-99.0.202404011739/kvirt/web/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.919520 kcli-99.0.202404011739/kvirt/web/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/css/bootstrap-notify.css
--rw-r--r--   0 runner    (1001) docker     (127)    23409 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/css/bootstrap-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   121125 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/css/dataTables.checkboxes.css
--rw-r--r--   0 runner    (1001) docker     (127)    13587 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/css/jquery.dataTables.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/css/kcli.css
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/css/navbar.css
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/css/spice.css
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/css/wheel.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.919520 kcli-99.0.202404011739/kvirt/web/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.923519 kcli-99.0.202404011739/kvirt/web/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/images/Centos.png
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/images/Debian.png
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/images/Fedora.png
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/images/Redhat.png
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/images/Suse.png
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/images/Tux.png
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/images/Ubuntu.png
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/images/delete.png
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    23320 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/images/kcli-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    27185 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/images/kcli.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   113928 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/images/kcli.png
--rw-r--r--   0 runner    (1001) docker     (127)    48809 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/images/logo-header.svg
--rw-r--r--   0 runner    (1001) docker     (127)    48809 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/images/logo-main.svg
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/images/sort_asc.png
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/images/sort_both.png
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/images/sort_desc.png
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/images/start.png
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/images/stop.png
--rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/images/wheel.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.923519 kcli-99.0.202404011739/kvirt/web/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/bootstrap-notify.js
--rw-r--r--   0 runner    (1001) docker     (127)    37045 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/containeraction.js
--rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/dataTables.checkboxes.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/hostaction.js
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/imageaction.js
--rw-r--r--   0 runner    (1001) docker     (127)    83059 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/jquery.dataTables.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    87462 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/kcli.js
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/kubeaction.js
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/list.js
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/networkaction.js
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/planaction.js
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/poolaction.js
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/productaction.js
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/refresh.js
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/repoaction.js
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/snapshotaction.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.927519 kcli-99.0.202404011739/kvirt/web/static/js/spice/
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/atKeynames.js
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/bitmap.js
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/cursor.js
--rw-r--r--   0 runner    (1001) docker     (127)    49214 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/display.js
--rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/enums.js
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/filexfer.js
--rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/inputs.js
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/lz.js
--rw-r--r--   0 runner    (1001) docker     (127)    18370 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/main.js
--rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/playback.js
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/png.js
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/port.js
--rw-r--r--   0 runner    (1001) docker     (127)    44531 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/quic.js
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/resize.js
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/simulatecursor.js
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/spicearraybuffer.js
--rw-r--r--   0 runner    (1001) docker     (127)    18202 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/spiceconn.js
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/spicedataview.js
--rw-r--r--   0 runner    (1001) docker     (127)    33015 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/spicemsg.js
--rw-r--r--   0 runner    (1001) docker     (127)    12767 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/spicetype.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.927519 kcli-99.0.202404011739/kvirt/web/static/js/spice/thirdparty/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.931519 kcli-99.0.202404011739/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/.npmignore
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/rollup.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.931519 kcli-99.0.202404011739/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/babel-worker.js
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/browser-es-module-loader.js
--rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/thirdparty/jsbn.js
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/thirdparty/prng4.js
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/thirdparty/rng.js
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/thirdparty/rsa.js
--rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/thirdparty/sha1.js
--rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/ticket.js
--rw-r--r--   0 runner    (1001) docker     (127)    13628 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/utils.js
--rw-r--r--   0 runner    (1001) docker     (127)    21577 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/webm.js
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/spice/wire.js
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/vmaction.js
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/js/wheel.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.855520 kcli-99.0.202404011739/kvirt/web/static/vnc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.931519 kcli-99.0.202404011739/kvirt/web/static/vnc/app/
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/error-handler.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.935519 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/alt.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/clipboard.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/connect.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/ctrl.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/ctrlaltdel.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/disconnect.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/drag.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/error.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/esc.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/expander.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/fullscreen.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/handle.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/handle_bg.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.935519 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-120x120.png
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-144x144.png
--rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-152x152.png
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-24x24.png
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-48x48.png
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-60x60.png
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-64x64.png
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-72x72.png
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-76x76.png
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-96x96.png
--rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-icon-sm.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/info.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/keyboard.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/mouse_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/mouse_middle.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/mouse_none.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/mouse_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/power.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/settings.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/tab.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/toggleextrakeys.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/warning.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/windows.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.939519 kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/cs.json
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/de.json
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/el.json
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/es.json
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/ja.json
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/ko.json
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/nl.json
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/pl.json
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/ru.json
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/sv.json
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/tr.json
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/zh_CN.json
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/zh_TW.json
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/localization.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.939519 kcli-99.0.202404011739/kvirt/web/static/vnc/app/sounds/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/sounds/CREDITS
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/sounds/bell.mp3
--rw-r--r--   0 runner    (1001) docker     (127)     8495 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/sounds/bell.oga
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.939519 kcli-99.0.202404011739/kvirt/web/static/vnc/app/styles/
--rw-r--r--   0 runner    (1001) docker     (127)    38580 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/styles/Orbitron700.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    17472 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/styles/Orbitron700.woff
--rw-r--r--   0 runner    (1001) docker     (127)    18450 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/styles/base.css
--rw-r--r--   0 runner    (1001) docker     (127)    56845 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/ui.js
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/app/webutil.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.939519 kcli-99.0.202404011739/kvirt/web/static/vnc/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/base64.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.939519 kcli-99.0.202404011739/kvirt/web/static/vnc/core/decoders/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/decoders/copyrect.js
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/decoders/hextile.js
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/decoders/raw.js
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/decoders/rre.js
--rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/decoders/tight.js
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/decoders/tightpng.js
--rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/des.js
--rw-r--r--   0 runner    (1001) docker     (127)    20381 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/display.js
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/encodings.js
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/inflator.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.943519 kcli-99.0.202404011739/kvirt/web/static/vnc/core/input/
--rw-r--r--   0 runner    (1001) docker     (127)    11438 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/input/domkeytable.js
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/input/fixedkeys.js
--rw-r--r--   0 runner    (1001) docker     (127)    13090 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/input/keyboard.js
--rw-r--r--   0 runner    (1001) docker     (127)    34609 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/input/keysym.js
--rw-r--r--   0 runner    (1001) docker     (127)    25374 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/input/keysymdef.js
--rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/input/mouse.js
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/input/util.js
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/input/vkeys.js
--rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/input/xtscancodes.js
--rw-r--r--   0 runner    (1001) docker     (127)    74196 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/rfb.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.943519 kcli-99.0.202404011739/kvirt/web/static/vnc/core/util/
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/util/browser.js
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/util/cursor.js
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/util/events.js
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/util/eventtarget.js
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/util/logging.js
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/util/polyfill.js
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/util/strings.js
--rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/core/websock.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.943519 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.943519 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/browser-es-module-loader/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/browser-es-module-loader/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/browser-es-module-loader/rollup.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.943519 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/babel-worker.js
--rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/browser-es-module-loader.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.943519 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.855520 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.943519 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/utils/common.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.947519 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/adler32.js
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/constants.js
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/crc32.js
--rw-r--r--   0 runner    (1001) docker     (127)    60016 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/deflate.js
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/gzheader.js
--rw-r--r--   0 runner    (1001) docker     (127)    11690 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/inffast.js
--rw-r--r--   0 runner    (1001) docker     (127)    47128 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/inflate.js
--rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/inftrees.js
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/messages.js
--rw-r--r--   0 runner    (1001) docker     (127)    38767 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/trees.js
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/zstream.js
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/promise.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.951519 kcli-99.0.202404011739/kvirt/web/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/bootstrap.html
--rw-r--r--   0 runner    (1001) docker     (127)    14595 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/console.html
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/containercreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/containerprofiles.html
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/containerprofilestable.html
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/containers.html
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/containerstable.html
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/head.html
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/hosts.html
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/hoststable.html
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/imagecreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/images.html
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/imagestable.html
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/isos.html
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/isostable.html
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/kubecreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/kubeinfo.html
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/kubeprofiles.html
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/kubeprofilestable.html
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/kubes.html
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/kubestable.html
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/navbar.html
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/networkcreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/networks.html
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/networkstable.html
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/plancreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/plans.html
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/planstable.html
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/poolcreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/pools.html
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/poolstable.html
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/productcreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/products.html
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/productstable.html
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/repocreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/repos.html
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/repostable.html
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/vmcreate.html
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/vmprofiles.html
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/vmprofilestable.html
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/vms.html
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/kvirt/web/templates/vmstable.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.951519 kcli-99.0.202404011739/samples/
--rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/samples/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/samples/profiles.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 17:39:25.951519 kcli-99.0.202404011739/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-01 17:39:25.000000 kcli-99.0.202404011739/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:39:25.951519 kcli-99.0.202404011739/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-01 17:35:08.000000 kcli-99.0.202404011739/tests/test_kvirt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.376382 kcli-99.0.202404020921/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-02 09:21:59.376382 kcli-99.0.202404020921/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.284381 kcli-99.0.202404020921/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/Dockerfile_curl
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/Dockerfile_kubectl
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/autoscale.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/aws_peering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/aws_peering_cleaning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.284381 kcli-99.0.202404020921/extras/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/controller/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/controller/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/controller/crd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/controller/deploy.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.284381 kcli-99.0.202404020921/extras/controller/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/controller/examples/cluster_simple.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/controller/examples/plan_complex.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/controller/examples/plan_simple.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/controller/examples/plan_simple_with_file.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/controller/examples/vm_centos8stream.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/controller/examples/vm_cirros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/controller/examples/vm_empty.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/controller/examples/vm_fedora.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9970 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/controller/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/controller/stress_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/debian
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.284381 kcli-99.0.202404020921/extras/expose/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/expose/kcli.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/expose/kcli.wsgi
+-rwxr-xr-x   0 runner    (1001) docker     (127)      106 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/genrst.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/haproxy.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/haproxy_multiple_clusters.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/i_am_a_container
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/k8sdeploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/kfish.md
+-rw-r--r--   0 runner    (1001) docker     (127)    38837 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/kfish.png
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/missing_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/openstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/openstack.sh.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/extras/zerotier.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.284381 kcli-99.0.202404020921/kcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-02 09:21:58.000000 kcli-99.0.202404020921/kcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27395 2024-04-02 09:21:58.000000 kcli-99.0.202404020921/kcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 09:21:58.000000 kcli-99.0.202404020921/kcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-02 09:21:58.000000 kcli-99.0.202404020921/kcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 09:18:50.000000 kcli-99.0.202404020921/kcli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-02 09:21:58.000000 kcli-99.0.202404020921/kcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 09:21:58.000000 kcli-99.0.202404020921/kcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.288382 kcli-99.0.202404020921/kvirt/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.288382 kcli-99.0.202404020921/kvirt/ansibleutils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/ansibleutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98843 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/baseconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)   171487 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/bottle.py
+-rw-r--r--   0 runner    (1001) docker     (127)   277696 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.288382 kcli-99.0.202404020921/kvirt/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.288382 kcli-99.0.202404020921/kvirt/cluster/aks/
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/aks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/aks/fake.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/aks/kcli_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.288382 kcli-99.0.202404020921/kvirt/cluster/eks/
+-rw-r--r--   0 runner    (1001) docker     (127)    12290 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/eks/fake.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/eks/kcli_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.292382 kcli-99.0.202404020921/kvirt/cluster/gke/
+-rw-r--r--   0 runner    (1001) docker     (127)    12249 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/gke/fake.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/gke/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/gke/kubeconfig.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.292382 kcli-99.0.202404020921/kvirt/cluster/hypershift/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/99-apps.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/99-forcedns
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/99-notifications.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/Corefile
+-rw-r--r--   0 runner    (1001) docker     (127)    46322 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/assisted_infra.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/assisted_ingress.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/autoapprovercron.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/bmc.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/calico.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/cilium.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/cloud_lb_apps.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/disconnected.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/extras.service
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/extras.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/hostedcluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/httpd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/ignition.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/kcli_plan.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/kcli_plan_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/keepalived.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/nmstateconfig.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/nodepool.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/nonlocalbind.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.292382 kcli-99.0.202404020921/kvirt/cluster/hypershift/staticpods/
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/staticpods/coredns.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/staticpods/keepalived.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/hypershift/staticpods/mdns.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.296382 kcli-99.0.202404020921/kvirt/cluster/k3s/
+-rw-r--r--   0 runner    (1001) docker     (127)    13877 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/k3s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/k3s/bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/k3s/bootstrap.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/k3s/cloud_lb_api.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/k3s/ctlplanes.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/k3s/ctlplanes.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/k3s/join.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/k3s/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/k3s/keepalived.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/k3s/keepalived.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/k3s/workers.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/k3s/workers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.296382 kcli-99.0.202404020921/kvirt/cluster/kubeadm/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/10-flannel.link
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/90-flannel.rules
+-rw-r--r--   0 runner    (1001) docker     (127)    14207 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.272382 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.300382 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/argocd/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/argocd/ingress.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/argocd/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/argocd/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/argocd/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.300382 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/autolabeller/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/autolabeller/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/autolabeller/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.300382 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/certmanager/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/certmanager/install.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.300382 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/dashboard/admin.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/dashboard/ingress.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/dashboard/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/dashboard/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/dashboard/user.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.300382 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/falco/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/falco/falco_advertisements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/falco/falco_ip.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/falco/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/falco/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/falco/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.300382 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/ingress/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/ingress/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/ingress/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.300382 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/istio/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/istio/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/istio/istio-minimal-operator.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.300382 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/katacontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/katacontainer/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/katacontainer/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.300382 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/knative/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/knative/cr_eventing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/knative/cr_serving.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/knative/install.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.300382 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/kubevirt/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/kubevirt/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/kubevirt/kcli_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.304382 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/metallb/
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/metallb/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/metallb/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/metallb/metallb_advertisement.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/metallb/metallb_cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/metallb/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.304382 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/olm/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/olm/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/olm/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.304382 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/policy_as_code/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/policy_as_code/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/policy_as_code/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/policy_as_code/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.304382 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/rancher/
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/rancher/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/rancher/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/rancher/rancher_advertisements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/rancher/rancher_ip.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/rancher/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.304382 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/rook/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/rook/install.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.304382 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/submariner/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/submariner/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/submariner/kcli_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.304382 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/tekton/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/tekton/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/tekton/uninstall.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3158 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/bootstrap.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/cloud_lb_api.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/crictl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/ctlplanes.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      343 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/deploy.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      598 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/join.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/keepalived.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/keepalived.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/nfs.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/nfs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/pre_el.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/pre_ubuntu.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/registry.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubeadm/workers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.304382 kcli-99.0.202404020921/kvirt/cluster/kubecommon/
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubecommon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.304382 kcli-99.0.202404020921/kvirt/cluster/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/kubernetes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.304382 kcli-99.0.202404020921/kvirt/cluster/microshift/
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/microshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/microshift/kcli_plan.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/microshift/kcli_plan_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.304382 kcli-99.0.202404020921/kvirt/cluster/microshift/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/microshift/scripts/00_sslip.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/microshift/scripts/01_clients.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/microshift/scripts/02_crio.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/microshift/scripts/03_microshift.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/microshift/scripts/04_kubeconfig.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/microshift/scripts/05_acm.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/microshift/scripts/deploy.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.316382 kcli-99.0.202404020921/kvirt/cluster/openshift/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/01-workload-partitioning
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/10-node-ip-hint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/20-localhost-fix.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/99-apps.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/99-autologin.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/99-bootstrap-deletion-2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/99-bootstrap-deletion.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/99-chrony.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/99-forcedns
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/99-forcedns-ibm
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/99-kubevirt-fix.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/99-metal3-fake-machine.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/99-metal3-provisioning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/99-notifications.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/99-operatorhub.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/99-ovn.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/99-sno.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/Corefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)    96962 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.316382 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.316382 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/advanced-cluster-management/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/advanced-cluster-management/99-metal3-provisioning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sample.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2839 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/advanced-cluster-management/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/advanced-cluster-management/gen_registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/advanced-cluster-management/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/advanced-cluster-management/post.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.316382 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/argocd/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/argocd/configmap.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/argocd/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/argocd/kcli_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.316382 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/autolabeller/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/autolabeller/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/autolabeller/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/autolabeller/install.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/autolabeller/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/autolabeller/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.316382 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/cluster-logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/cluster-logging/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/cluster-logging/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/cr.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/install.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.316382 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/istio/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/istio/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/istio/istio-cni.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.316382 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/kubernetes-nmstate-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/kubernetes-nmstate-operator/cr.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.320382 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/kcli_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.320382 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/local-storage-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/local-storage-operator/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/local-storage-operator/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/local-storage-operator/post.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.320382 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/lvms-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/lvms-operator/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/lvms-operator/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/lvms-operator/post.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.320382 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/metallb-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/metallb-operator/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/metallb-operator/kcli_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.320382 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/multicluster-engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/multicluster-engine/99-metal3-provisioning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sample.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2846 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/multicluster-engine/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/multicluster-engine/gen_registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/multicluster-engine/kcli_default.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       55 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/multicluster-engine/post.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.320382 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/nfs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2297 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/nfs/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/nfs/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/nfs/uninstall.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.320382 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/odf-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/odf-operator/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/odf-operator/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/odf-operator/nad_cluster.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/odf-operator/nad_public.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/odf-operator/post.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/odf-operator/pre.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.320382 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/serverless-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/serverless-operator/cr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/serverless-operator/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/serverless-operator/post.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.324382 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/users/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/users/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/users/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/users/oauth.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/users/oauth_hypershift.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/apps/users/uninstall.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/autoapprovercron.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/autorules.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/bootstrap.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/calico.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/chrony.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/cilium.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/cloud_bootstrap.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/cloud_ctlplanes.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/cloud_dns.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/cloud_lb_api.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/cloud_lb_apps.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/cloud_workers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/cluster-ingress-02-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/cluster-scheduler-02-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/config.hcl.templ
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/ctlplanes.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.324382 kcli-99.0.202404020921/kvirt/cluster/openshift/customisation/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/customisation/00-kcli-namespace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/customisation/97-autoapprovercron-sa.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/customisation/98-autoapprovercron-binding.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/customisation/99-autoapprovercron-cronjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/customisation/99-ingress-controller.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/customisation/99-iptables.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/customisation/99-monitoring.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/customisation/99-registry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/dhcp.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/dhcp.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/dhcp.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.324382 kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.324382 kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      357 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected/bin/sync_image.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected/haproxy.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected/registry.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.324382 kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      201 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected/scripts/01_get_oc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      243 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected/scripts/02_packages.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2412 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected/scripts/03_mirror.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2101 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected/scripts/03_registry.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      331 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected/scripts/04_extras.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2349 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected/scripts/05_olm.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      197 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected/scripts/06_web.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      841 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected/scripts/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected/scripts/mirror-config.yaml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/fake_kubeconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/fake_pull.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/haproxy.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/haproxy.cfg.kubevirt
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/httpd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/icsp.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/ignition.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/install-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/iso.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/kcli-ipv6.conf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/kcli_default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/keepalived.conf
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/nonlocalbind.conf
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/openshift-workload-pinning
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/patch_ipv6.json
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/relocate-ip-bootstrap.service
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/relocate-ip-bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/relocate-ip.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/sno-finish.service
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/sno-finish.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/sno.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/sno_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.324382 kcli-99.0.202404020921/kvirt/cluster/openshift/staticpods/
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/staticpods/coredns.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/staticpods/haproxy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/staticpods/keepalived.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/staticpods/mdns.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/openshift/workers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.328382 kcli-99.0.202404020921/kvirt/cluster/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/profiles/sample-kubeadm-default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/profiles/sample-openshift-compact.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/profiles/sample-openshift-contrail.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/profiles/sample-openshift-ipv6.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/profiles/sample-openshift-sno-bm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/profiles/sample-openshift-sno.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/cluster/sampleprovider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.328382 kcli-99.0.202404020921/kvirt/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/common/Jenkinsfile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)   105808 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/common/autoscale.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/common/fake_kubeconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/common/ignition.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/common/kubevirt_kcli_conf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/common/local_kcli_conf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/common/pipeline.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/common/pipeline_kube.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/common/playbook.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/common/storage.sh.aws
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/common/storage.sh.gcp
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/common/storage.sh.ibmcloud
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/common/vm.ovf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/common/workflow.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/common/workflow_script.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)   190877 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.328382 kcli-99.0.202404020921/kvirt/container/
+-rw-r--r--   0 runner    (1001) docker     (127)    14188 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/containerconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/defaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1475 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/ekstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25462 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.328382 kcli-99.0.202404020921/kvirt/expose/
+-rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.276382 kcli-99.0.202404020921/kvirt/expose/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.328382 kcli-99.0.202404020921/kvirt/expose/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/static/css/bootstrap-notify.css
+-rw-r--r--   0 runner    (1001) docker     (127)   121125 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/static/css/dataTables.checkboxes.css
+-rw-r--r--   0 runner    (1001) docker     (127)    13587 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/static/css/jquery.dataTables.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/static/css/kcli.css
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/static/css/wheel.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.332382 kcli-99.0.202404020921/kvirt/expose/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/static/images/sort_asc.png
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/static/images/sort_both.png
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/static/images/sort_desc.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/static/images/wheel.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.332382 kcli-99.0.202404020921/kvirt/expose/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/static/js/dataTables.checkboxes.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/static/js/exposeactions.js
+-rw-r--r--   0 runner    (1001) docker     (127)    83059 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/static/js/jquery.dataTables.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    89795 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/static/js/list.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/swagger.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.332382 kcli-99.0.202404020921/kvirt/expose/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/templates/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/templates/infoplan.html
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/templates/planstable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/expose/templates/result.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/gketoken.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4333 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/ignitionmerger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.332382 kcli-99.0.202404020921/kvirt/internalplans/
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/internalplans/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.332382 kcli-99.0.202404020921/kvirt/jinjafilters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/jinjafilters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/jinjafilters/jinjafilters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/keywords.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.332382 kcli-99.0.202404020921/kvirt/kfish/
+-rw-r--r--   0 runner    (1001) docker     (127)    12858 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/kfish/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3395 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/klist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.332382 kcli-99.0.202404020921/kvirt/ksushy/
+-rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/ksushy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      121 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/ksushy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.336382 kcli-99.0.202404020921/kvirt/ksushy/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/ksushy/templates/bios.json
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/ksushy/templates/interface.json
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/ksushy/templates/interfaces.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/ksushy/templates/manager.json
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/ksushy/templates/managers.json
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/ksushy/templates/root.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/ksushy/templates/system.json
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/ksushy/templates/systems.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/ksushy/templates/virtualmedia_cd.json
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/ksushy/templates/virtualmedias.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.336382 kcli-99.0.202404020921/kvirt/miniconsole/
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/miniconsole/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.336382 kcli-99.0.202404020921/kvirt/nameutils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/nameutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.336382 kcli-99.0.202404020921/kvirt/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.336382 kcli-99.0.202404020921/kvirt/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)   106119 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/aws/assume_policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/aws/ctlplane_policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/aws/worker_policy.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.336382 kcli-99.0.202404020921/kvirt/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)    78530 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.336382 kcli-99.0.202404020921/kvirt/providers/fake/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/fake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.336382 kcli-99.0.202404020921/kvirt/providers/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)    99391 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/gcp/gcp-hack.service
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/gcp/gcp-hack.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.336382 kcli-99.0.202404020921/kvirt/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)    65793 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/ibm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.336382 kcli-99.0.202404020921/kvirt/providers/kubevirt/
+-rw-r--r--   0 runner    (1001) docker     (127)    86428 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/kubevirt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.336382 kcli-99.0.202404020921/kvirt/providers/kvm/
+-rw-r--r--   0 runner    (1001) docker     (127)   186412 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/kvm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/kvm/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.336382 kcli-99.0.202404020921/kvirt/providers/openstack/
+-rw-r--r--   0 runner    (1001) docker     (127)    58301 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/openstack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.336382 kcli-99.0.202404020921/kvirt/providers/ovirt/
+-rw-r--r--   0 runner    (1001) docker     (127)    63291 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/ovirt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.340382 kcli-99.0.202404020921/kvirt/providers/packet/
+-rw-r--r--   0 runner    (1001) docker     (127)    31823 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/packet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.340382 kcli-99.0.202404020921/kvirt/providers/proxmox/
+-rw-r--r--   0 runner    (1001) docker     (127)    35211 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/proxmox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/sampleprovider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.340382 kcli-99.0.202404020921/kvirt/providers/vsphere/
+-rw-r--r--   0 runner    (1001) docker     (127)    73908 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/vsphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13503 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/vsphere/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/vsphere/tagging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.340382 kcli-99.0.202404020921/kvirt/providers/web/
+-rw-r--r--   0 runner    (1001) docker     (127)    22043 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/providers/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.340382 kcli-99.0.202404020921/kvirt/version/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 09:21:58.000000 kcli-99.0.202404020921/kvirt/version/git
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.340382 kcli-99.0.202404020921/kvirt/web/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46680 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.276382 kcli-99.0.202404020921/kvirt/web/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.340382 kcli-99.0.202404020921/kvirt/web/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/css/bootstrap-notify.css
+-rw-r--r--   0 runner    (1001) docker     (127)    23409 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/css/bootstrap-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   121125 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/css/dataTables.checkboxes.css
+-rw-r--r--   0 runner    (1001) docker     (127)    13587 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/css/jquery.dataTables.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/css/kcli.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/css/navbar.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/css/spice.css
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/css/wheel.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.340382 kcli-99.0.202404020921/kvirt/web/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.344382 kcli-99.0.202404020921/kvirt/web/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/images/Centos.png
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/images/Debian.png
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/images/Fedora.png
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/images/Redhat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/images/Suse.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/images/Tux.png
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/images/Ubuntu.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/images/delete.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    23320 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/images/kcli-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27185 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/images/kcli.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   113928 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/images/kcli.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48809 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/images/logo-header.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    48809 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/images/logo-main.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/images/sort_asc.png
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/images/sort_both.png
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/images/sort_desc.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/images/start.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/images/stop.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/images/wheel.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.348382 kcli-99.0.202404020921/kvirt/web/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/bootstrap-notify.js
+-rw-r--r--   0 runner    (1001) docker     (127)    37045 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/containeraction.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/dataTables.checkboxes.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/hostaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/imageaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)    83059 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/jquery.dataTables.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    87462 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/kcli.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/kubeaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/list.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/networkaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/planaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/poolaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/productaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/refresh.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/repoaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/snapshotaction.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.352382 kcli-99.0.202404020921/kvirt/web/static/js/spice/
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/atKeynames.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/bitmap.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/cursor.js
+-rw-r--r--   0 runner    (1001) docker     (127)    49214 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/display.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/enums.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/filexfer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/inputs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/lz.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18370 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/playback.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/png.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/port.js
+-rw-r--r--   0 runner    (1001) docker     (127)    44531 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/quic.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/resize.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/simulatecursor.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/spicearraybuffer.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18202 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/spiceconn.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/spicedataview.js
+-rw-r--r--   0 runner    (1001) docker     (127)    33015 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/spicemsg.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12767 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/spicetype.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.352382 kcli-99.0.202404020921/kvirt/web/static/js/spice/thirdparty/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.352382 kcli-99.0.202404020921/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/.npmignore
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/rollup.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.352382 kcli-99.0.202404020921/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/babel-worker.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/browser-es-module-loader.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/thirdparty/jsbn.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/thirdparty/prng4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/thirdparty/rng.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/thirdparty/rsa.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/thirdparty/sha1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/ticket.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13628 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/utils.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21577 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/webm.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/spice/wire.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/vmaction.js
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/js/wheel.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.280382 kcli-99.0.202404020921/kvirt/web/static/vnc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.352382 kcli-99.0.202404020921/kvirt/web/static/vnc/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/error-handler.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.356382 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/alt.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/clipboard.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/connect.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/ctrl.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/ctrlaltdel.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/disconnect.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/drag.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/error.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/esc.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/expander.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/fullscreen.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/handle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/handle_bg.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.360382 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-152x152.png
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-24x24.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-48x48.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-60x60.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-64x64.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-76x76.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-icon-sm.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/info.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/keyboard.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/mouse_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/mouse_middle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/mouse_none.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/mouse_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/power.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/tab.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/toggleextrakeys.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/warning.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/windows.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.360382 kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/cs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/de.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/el.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/es.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/ja.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/ko.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/nl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/pl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/ru.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/sv.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/tr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/zh_CN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/zh_TW.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/localization.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.360382 kcli-99.0.202404020921/kvirt/web/static/vnc/app/sounds/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/sounds/CREDITS
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/sounds/bell.mp3
+-rw-r--r--   0 runner    (1001) docker     (127)     8495 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/sounds/bell.oga
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.360382 kcli-99.0.202404020921/kvirt/web/static/vnc/app/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)    38580 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/styles/Orbitron700.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    17472 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/styles/Orbitron700.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18450 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/styles/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)    56845 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/ui.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/app/webutil.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.364382 kcli-99.0.202404020921/kvirt/web/static/vnc/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/base64.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.364382 kcli-99.0.202404020921/kvirt/web/static/vnc/core/decoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/decoders/copyrect.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/decoders/hextile.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/decoders/raw.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/decoders/rre.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/decoders/tight.js
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/decoders/tightpng.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/des.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20381 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/display.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/encodings.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/inflator.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.364382 kcli-99.0.202404020921/kvirt/web/static/vnc/core/input/
+-rw-r--r--   0 runner    (1001) docker     (127)    11438 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/input/domkeytable.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/input/fixedkeys.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13090 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/input/keyboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34609 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/input/keysym.js
+-rw-r--r--   0 runner    (1001) docker     (127)    25374 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/input/keysymdef.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/input/mouse.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/input/util.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/input/vkeys.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/input/xtscancodes.js
+-rw-r--r--   0 runner    (1001) docker     (127)    74196 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/rfb.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.364382 kcli-99.0.202404020921/kvirt/web/static/vnc/core/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/util/browser.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/util/cursor.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/util/events.js
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/util/eventtarget.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/util/logging.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/util/polyfill.js
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/util/strings.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/core/websock.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.364382 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.368382 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/browser-es-module-loader/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/browser-es-module-loader/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/browser-es-module-loader/rollup.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.368382 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/babel-worker.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/browser-es-module-loader.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.368382 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.280382 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.368382 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/utils/common.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.368382 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/adler32.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/constants.js
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/crc32.js
+-rw-r--r--   0 runner    (1001) docker     (127)    60016 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/deflate.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/gzheader.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11690 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/inffast.js
+-rw-r--r--   0 runner    (1001) docker     (127)    47128 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/inflate.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/inftrees.js
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/messages.js
+-rw-r--r--   0 runner    (1001) docker     (127)    38767 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/trees.js
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/zstream.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/promise.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.376382 kcli-99.0.202404020921/kvirt/web/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/bootstrap.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14595 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/console.html
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/containercreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/containerprofiles.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/containerprofilestable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/containers.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/containerstable.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/hosts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/hoststable.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/imagecreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/images.html
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/imagestable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/isos.html
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/isostable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/kubecreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/kubeinfo.html
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/kubeprofiles.html
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/kubeprofilestable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/kubes.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/kubestable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/networkcreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/networks.html
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/networkstable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/plancreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/plans.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/planstable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/poolcreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/pools.html
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/poolstable.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/productcreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/products.html
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/productstable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/repocreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/repos.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/repostable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/vmcreate.html
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/vmprofiles.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/vmprofilestable.html
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/vms.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/kvirt/web/templates/vmstable.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.376382 kcli-99.0.202404020921/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/samples/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/samples/profiles.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 09:21:59.376382 kcli-99.0.202404020921/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-02 09:21:58.000000 kcli-99.0.202404020921/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:21:59.376382 kcli-99.0.202404020921/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-02 09:18:00.000000 kcli-99.0.202404020921/tests/test_kvirt.py
```

### Comparing `kcli-99.0.202404011739/LICENSE` & `kcli-99.0.202404020921/LICENSE`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/MANIFEST.in` & `kcli-99.0.202404020921/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/PKG-INFO` & `kcli-99.0.202404020921/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kcli
-Version: 99.0.202404011739
+Version: 99.0.202404020921
 Summary: Provisioner/Manager for Libvirt/Vsphere/Aws/Gcp/Kubevirt/Ovirt/Openstack/IBM Cloud and containers
 Home-page: http://github.com/karmab/kcli
 Author: Karim Boumedhel
 Author-email: karimboumedhel@gmail.com
 License: ASL
 Platform: UNKNOWN
 Provides-Extra: all
```

### Comparing `kcli-99.0.202404011739/README.md` & `kcli-99.0.202404020921/README.md`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/extras/autoscale.yml` & `kcli-99.0.202404020921/extras/autoscale.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/extras/aws_peering.py` & `kcli-99.0.202404020921/extras/aws_peering.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/extras/aws_peering_cleaning.py` & `kcli-99.0.202404020921/extras/aws_peering_cleaning.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/extras/controller/README.md` & `kcli-99.0.202404020921/extras/controller/README.md`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/extras/controller/crd.yml` & `kcli-99.0.202404020921/extras/controller/crd.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/extras/controller/deploy.yml` & `kcli-99.0.202404020921/extras/controller/deploy.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/extras/controller/examples/plan_complex.yml` & `kcli-99.0.202404020921/extras/controller/examples/plan_complex.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/extras/controller/handlers.py` & `kcli-99.0.202404020921/extras/controller/handlers.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/extras/controller/stress_test.yml` & `kcli-99.0.202404020921/extras/controller/stress_test.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/extras/debian` & `kcli-99.0.202404020921/extras/debian`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/extras/haproxy.cfg` & `kcli-99.0.202404020921/extras/haproxy.cfg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/extras/haproxy_multiple_clusters.cfg` & `kcli-99.0.202404020921/extras/haproxy_multiple_clusters.cfg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/extras/k8sdeploy.yml` & `kcli-99.0.202404020921/extras/k8sdeploy.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/extras/kfish.md` & `kcli-99.0.202404020921/extras/kfish.md`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/extras/kfish.png` & `kcli-99.0.202404020921/extras/kfish.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/extras/openstack.py` & `kcli-99.0.202404020921/extras/openstack.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/extras/openstack.sh.sample` & `kcli-99.0.202404020921/extras/openstack.sh.sample`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/extras/zerotier.service` & `kcli-99.0.202404020921/extras/zerotier.service`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kcli.egg-info/PKG-INFO` & `kcli-99.0.202404020921/kcli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kcli
-Version: 99.0.202404011739
+Version: 99.0.202404020921
 Summary: Provisioner/Manager for Libvirt/Vsphere/Aws/Gcp/Kubevirt/Ovirt/Openstack/IBM Cloud and containers
 Home-page: http://github.com/karmab/kcli
 Author: Karim Boumedhel
 Author-email: karimboumedhel@gmail.com
 License: ASL
 Platform: UNKNOWN
 Provides-Extra: all
```

### Comparing `kcli-99.0.202404011739/kcli.egg-info/SOURCES.txt` & `kcli-99.0.202404020921/kcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kcli.egg-info/requires.txt` & `kcli-99.0.202404020921/kcli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/ansibleutils/__init__.py` & `kcli-99.0.202404020921/kvirt/ansibleutils/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/baseconfig.py` & `kcli-99.0.202404020921/kvirt/baseconfig.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/bottle.py` & `kcli-99.0.202404020921/kvirt/bottle.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cli.py` & `kcli-99.0.202404020921/kvirt/cli.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/aks/__init__.py` & `kcli-99.0.202404020921/kvirt/cluster/aks/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/eks/__init__.py` & `kcli-99.0.202404020921/kvirt/cluster/eks/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/gke/__init__.py` & `kcli-99.0.202404020921/kvirt/cluster/gke/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/99-apps.yaml` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/99-apps.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/99-forcedns` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/99-forcedns`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/99-notifications.yaml` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/99-notifications.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/Corefile` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/Corefile`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/__init__.py` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/assisted_infra.yml` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/assisted_infra.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/assisted_ingress.yml` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/assisted_ingress.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/autoapprovercron.yml` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/autoapprovercron.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/bmc.yml.j2` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/bmc.yml.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/calico.sh.j2` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/calico.sh.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/cilium.sh.j2` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/cilium.sh.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/disconnected.sh` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/disconnected.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/extras.sh` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/extras.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/hostedcluster.yaml` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/hostedcluster.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/httpd.yaml` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/httpd.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/ignition.sh` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/ignition.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/kcli_plan.yml` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/kcli_plan.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/kcli_plan_default.yml` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/kcli_plan_default.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/nmstateconfig.yml.j2` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/nmstateconfig.yml.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/nodepool.yaml` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/nodepool.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/staticpods/coredns.yml` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/staticpods/coredns.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/staticpods/keepalived.yml` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/staticpods/keepalived.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/hypershift/staticpods/mdns.yml` & `kcli-99.0.202404020921/kvirt/cluster/hypershift/staticpods/mdns.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/k3s/__init__.py` & `kcli-99.0.202404020921/kvirt/cluster/k3s/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/k3s/bootstrap.sh` & `kcli-99.0.202404020921/kvirt/cluster/k3s/bootstrap.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/k3s/bootstrap.yml` & `kcli-99.0.202404020921/kvirt/cluster/k3s/bootstrap.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/k3s/ctlplanes.sh` & `kcli-99.0.202404020921/kvirt/cluster/k3s/ctlplanes.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/k3s/ctlplanes.yml` & `kcli-99.0.202404020921/kvirt/cluster/k3s/ctlplanes.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/k3s/kcli_default.yml` & `kcli-99.0.202404020921/kvirt/cluster/k3s/kcli_default.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/k3s/workers.yml` & `kcli-99.0.202404020921/kvirt/cluster/k3s/workers.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/__init__.py` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/argocd/install.sh` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/argocd/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/dashboard/install.sh` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/dashboard/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/falco/install.sh` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/falco/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/istio/istio-minimal-operator.yaml` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/istio/istio-minimal-operator.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/katacontainer/install.sh` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/katacontainer/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/katacontainer/uninstall.sh` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/katacontainer/uninstall.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/kubevirt/install.sh` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/kubevirt/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/metallb/install.sh` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/metallb/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/metallb/metallb_advertisement.yml` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/metallb/metallb_advertisement.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/rancher/install.sh` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/rancher/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/apps/rook/install.sh` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/apps/rook/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/bootstrap.sh` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/bootstrap.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/bootstrap.yml` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/bootstrap.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/ctlplanes.yml` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/ctlplanes.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/join.sh` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/join.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/kcli_default.yml` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/kcli_default.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/keepalived.conf` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/keepalived.conf`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/nfs.sh` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/nfs.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/pre_el.sh` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/pre_el.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/pre_ubuntu.sh` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/pre_ubuntu.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/registry.yml` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/registry.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubeadm/workers.yml` & `kcli-99.0.202404020921/kvirt/cluster/kubeadm/workers.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubecommon/__init__.py` & `kcli-99.0.202404020921/kvirt/cluster/kubecommon/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/kubernetes/__init__.py` & `kcli-99.0.202404020921/kvirt/cluster/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/microshift/__init__.py` & `kcli-99.0.202404020921/kvirt/cluster/microshift/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/microshift/kcli_plan.yml` & `kcli-99.0.202404020921/kvirt/cluster/microshift/kcli_plan.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/microshift/kcli_plan_default.yml` & `kcli-99.0.202404020921/kvirt/cluster/microshift/kcli_plan_default.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/microshift/scripts/01_clients.sh` & `kcli-99.0.202404020921/kvirt/cluster/microshift/scripts/01_clients.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/microshift/scripts/03_microshift.sh` & `kcli-99.0.202404020921/kvirt/cluster/microshift/scripts/03_microshift.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/microshift/scripts/05_acm.sh` & `kcli-99.0.202404020921/kvirt/cluster/microshift/scripts/05_acm.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/microshift/scripts/deploy.sh` & `kcli-99.0.202404020921/kvirt/cluster/microshift/scripts/deploy.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/10-node-ip-hint.yaml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/10-node-ip-hint.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/20-localhost-fix.yaml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/20-localhost-fix.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/99-apps.yaml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/99-apps.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/99-autologin.yaml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/99-autologin.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/99-bootstrap-deletion-2.yaml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/99-bootstrap-deletion-2.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/99-bootstrap-deletion.yaml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/99-bootstrap-deletion.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/99-chrony.yaml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/99-chrony.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/99-forcedns` & `kcli-99.0.202404020921/kvirt/cluster/openshift/99-forcedns`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/99-kubevirt-fix.yaml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/99-kubevirt-fix.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/99-notifications.yaml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/99-notifications.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/99-sno.yaml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/99-sno.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/Corefile` & `kcli-99.0.202404020921/kvirt/cluster/openshift/Corefile`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/__init__.py` & `kcli-99.0.202404020921/kvirt/cluster/openshift/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 def update_disconnected_registry(config, plandir, cluster, data):
     disconnected_url = data['disconnected_url']
     pull_secret = data['pull_secret']
     version = data['version']
     tag = data.get('ori_tag') or data.get('tag')
     arch = data.get('arch', 'x86_64')
     clusterdir = os.path.expanduser(f"~/.kcli/clusters/{cluster}") if cluster is not None else '.'
-    if 'ca' not in data:
+    if data.get('ca') is None:
         pprint(f"Trying to gather registry ca cert from {disconnected_url}")
         cacmd = f"openssl s_client -showcerts -connect {disconnected_url} </dev/null 2>/dev/null|"
         cacmd += "openssl x509 -outform PEM"
         data['ca'] = os.popen(cacmd).read()
     with open(f'{clusterdir}/ca.crt', 'w') as f:
         f.write(data['ca'])
     call(f'sudo cp {clusterdir}/ca.crt /etc/pki/ca-trust/source/anchors ; sudo update-ca-trust extract',
```

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sample.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sample.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sh` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/advanced-cluster-management/gen_registries.py` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/advanced-cluster-management/gen_registries.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/advanced-cluster-management/post.sh` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/advanced-cluster-management/post.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/argocd/configmap.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/argocd/configmap.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/argocd/install.sh` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/argocd/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/autolabeller/cr.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/autolabeller/cr.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/autolabeller/install.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/autolabeller/install.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/cluster-logging/cr.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/cluster-logging/cr.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/install.yml.j2` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/install.yml.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/cr.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/kubevirt-hyperconverged/cr.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/local-storage-operator/cr.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/local-storage-operator/cr.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/local-storage-operator/post.sh` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/local-storage-operator/post.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/lvms-operator/cr.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/lvms-operator/cr.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/lvms-operator/post.sh` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/lvms-operator/post.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/metallb-operator/cr.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/metallb-operator/cr.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sample.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sample.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sh` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/multicluster-engine/gen_registries.py` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/multicluster-engine/gen_registries.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/nfs/install.sh` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/nfs/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/odf-operator/cr.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/odf-operator/cr.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/odf-operator/post.sh` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/odf-operator/post.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/odf-operator/pre.sh` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/odf-operator/pre.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/apps/users/install.sh` & `kcli-99.0.202404020921/kvirt/cluster/openshift/apps/users/install.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/autoapprovercron.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/autoapprovercron.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/autorules.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/autorules.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/bootstrap.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/bootstrap.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/cilium.sh.j2` & `kcli-99.0.202404020921/kvirt/cluster/openshift/cilium.sh.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/cloud_bootstrap.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/cloud_bootstrap.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/cloud_ctlplanes.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/cloud_ctlplanes.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/cloud_workers.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/cloud_workers.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/ctlplanes.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/ctlplanes.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/customisation/99-autoapprovercron-cronjob.yaml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/customisation/99-autoapprovercron-cronjob.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/customisation/99-iptables.yaml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/customisation/99-iptables.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/dhcp.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/dhcp.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected/haproxy.cfg` & `kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected/haproxy.cfg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected/scripts/03_mirror.sh` & `kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected/scripts/03_mirror.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected/scripts/03_registry.sh` & `kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected/scripts/03_registry.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected/scripts/05_olm.sh` & `kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected/scripts/05_olm.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected/scripts/deploy.sh` & `kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected/scripts/deploy.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected/scripts/mirror-config.yaml.sample` & `kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected/scripts/mirror-config.yaml.sample`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/disconnected.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/disconnected.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/fake_kubeconfig.json` & `kcli-99.0.202404020921/kvirt/cluster/openshift/fake_kubeconfig.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/haproxy.cfg` & `kcli-99.0.202404020921/kvirt/cluster/openshift/haproxy.cfg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/haproxy.cfg.kubevirt` & `kcli-99.0.202404020921/kvirt/cluster/openshift/haproxy.cfg.kubevirt`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/httpd.yaml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/httpd.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/ignition.j2` & `kcli-99.0.202404020921/kvirt/cluster/openshift/ignition.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/install-config.yaml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/install-config.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/iso.sh` & `kcli-99.0.202404020921/kvirt/cluster/openshift/iso.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/kcli_default.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/kcli_default.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/keepalived.conf` & `kcli-99.0.202404020921/kvirt/cluster/openshift/keepalived.conf`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/relocate-ip.sh` & `kcli-99.0.202404020921/kvirt/cluster/openshift/relocate-ip.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/sno-finish.sh` & `kcli-99.0.202404020921/kvirt/cluster/openshift/sno-finish.sh`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/sno.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/sno.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/sno_default.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/sno_default.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/staticpods/coredns.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/staticpods/coredns.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/staticpods/haproxy.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/staticpods/haproxy.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/staticpods/keepalived.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/staticpods/keepalived.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/staticpods/mdns.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/staticpods/mdns.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/cluster/openshift/workers.yml` & `kcli-99.0.202404020921/kvirt/cluster/openshift/workers.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/common/Jenkinsfile.j2` & `kcli-99.0.202404020921/kvirt/common/Jenkinsfile.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/common/__init__.py` & `kcli-99.0.202404020921/kvirt/common/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/common/autoscale.yaml.j2` & `kcli-99.0.202404020921/kvirt/common/autoscale.yaml.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/common/fake_kubeconfig.json` & `kcli-99.0.202404020921/kvirt/common/fake_kubeconfig.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/common/ignition.j2` & `kcli-99.0.202404020921/kvirt/common/ignition.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/common/pipeline.yml.j2` & `kcli-99.0.202404020921/kvirt/common/pipeline.yml.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/common/pipeline_kube.yml.j2` & `kcli-99.0.202404020921/kvirt/common/pipeline_kube.yml.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/common/playbook.j2` & `kcli-99.0.202404020921/kvirt/common/playbook.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/common/storage.sh.aws` & `kcli-99.0.202404020921/kvirt/common/storage.sh.aws`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/common/storage.sh.gcp` & `kcli-99.0.202404020921/kvirt/common/storage.sh.gcp`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/common/vm.ovf.j2` & `kcli-99.0.202404020921/kvirt/common/vm.ovf.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/common/workflow.yml.j2` & `kcli-99.0.202404020921/kvirt/common/workflow.yml.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/common/workflow_script.yml.j2` & `kcli-99.0.202404020921/kvirt/common/workflow_script.yml.j2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/config.py` & `kcli-99.0.202404020921/kvirt/config.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/container/__init__.py` & `kcli-99.0.202404020921/kvirt/container/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/containerconfig.py` & `kcli-99.0.202404020921/kvirt/containerconfig.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/defaults.py` & `kcli-99.0.202404020921/kvirt/defaults.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/ekstoken.py` & `kcli-99.0.202404020921/kvirt/ekstoken.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/examples.py` & `kcli-99.0.202404020921/kvirt/examples.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/expose/__init__.py` & `kcli-99.0.202404020921/kvirt/expose/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/expose/static/css/bootstrap.min.css` & `kcli-99.0.202404020921/kvirt/expose/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/expose/static/css/jquery.dataTables.min.css` & `kcli-99.0.202404020921/kvirt/expose/static/css/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/expose/static/css/kcli.css` & `kcli-99.0.202404020921/kvirt/expose/static/css/kcli.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/expose/static/images/favicon.ico` & `kcli-99.0.202404020921/kvirt/expose/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/expose/static/images/wheel.gif` & `kcli-99.0.202404020921/kvirt/expose/static/images/wheel.gif`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/expose/static/js/dataTables.checkboxes.min.js` & `kcli-99.0.202404020921/kvirt/expose/static/js/dataTables.checkboxes.min.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/expose/static/js/jquery.dataTables.min.js` & `kcli-99.0.202404020921/kvirt/expose/static/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/expose/static/js/jquery.min.js` & `kcli-99.0.202404020921/kvirt/expose/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/expose/swagger.yml` & `kcli-99.0.202404020921/kvirt/expose/swagger.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/expose/templates/form.html` & `kcli-99.0.202404020921/kvirt/expose/templates/form.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/expose/templates/head.html` & `kcli-99.0.202404020921/kvirt/expose/templates/head.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/expose/templates/infoplan.html` & `kcli-99.0.202404020921/kvirt/expose/templates/infoplan.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/expose/templates/planstable.html` & `kcli-99.0.202404020921/kvirt/expose/templates/planstable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/expose/templates/result.html` & `kcli-99.0.202404020921/kvirt/expose/templates/result.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/gketoken.py` & `kcli-99.0.202404020921/kvirt/gketoken.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/ignitionmerger.py` & `kcli-99.0.202404020921/kvirt/ignitionmerger.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/internalplans/__init__.py` & `kcli-99.0.202404020921/kvirt/internalplans/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/jinjafilters/jinjafilters.py` & `kcli-99.0.202404020921/kvirt/jinjafilters/jinjafilters.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/keywords.yaml` & `kcli-99.0.202404020921/kvirt/keywords.yaml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/kfish/__init__.py` & `kcli-99.0.202404020921/kvirt/kfish/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/klist.py` & `kcli-99.0.202404020921/kvirt/klist.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/ksushy/__init__.py` & `kcli-99.0.202404020921/kvirt/ksushy/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/ksushy/templates/bios.json` & `kcli-99.0.202404020921/kvirt/ksushy/templates/bios.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/ksushy/templates/manager.json` & `kcli-99.0.202404020921/kvirt/ksushy/templates/manager.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/ksushy/templates/managers.json` & `kcli-99.0.202404020921/kvirt/ksushy/templates/managers.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/ksushy/templates/root.json` & `kcli-99.0.202404020921/kvirt/ksushy/templates/root.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/ksushy/templates/system.json` & `kcli-99.0.202404020921/kvirt/ksushy/templates/system.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/ksushy/templates/virtualmedia_cd.json` & `kcli-99.0.202404020921/kvirt/ksushy/templates/virtualmedia_cd.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/ksushy/templates/virtualmedias.json` & `kcli-99.0.202404020921/kvirt/ksushy/templates/virtualmedias.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/miniconsole/__init__.py` & `kcli-99.0.202404020921/kvirt/miniconsole/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/nameutils/__init__.py` & `kcli-99.0.202404020921/kvirt/nameutils/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/providers/aws/__init__.py` & `kcli-99.0.202404020921/kvirt/providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/providers/aws/ctlplane_policy.json` & `kcli-99.0.202404020921/kvirt/providers/aws/ctlplane_policy.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/providers/azure/__init__.py` & `kcli-99.0.202404020921/kvirt/providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/providers/gcp/__init__.py` & `kcli-99.0.202404020921/kvirt/providers/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/providers/ibm/__init__.py` & `kcli-99.0.202404020921/kvirt/providers/ibm/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/providers/kubevirt/__init__.py` & `kcli-99.0.202404020921/kvirt/providers/kubevirt/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/providers/kvm/__init__.py` & `kcli-99.0.202404020921/kvirt/providers/kvm/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/providers/kvm/helpers.py` & `kcli-99.0.202404020921/kvirt/providers/kvm/helpers.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/providers/openstack/__init__.py` & `kcli-99.0.202404020921/kvirt/providers/openstack/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/providers/ovirt/__init__.py` & `kcli-99.0.202404020921/kvirt/providers/ovirt/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/providers/packet/__init__.py` & `kcli-99.0.202404020921/kvirt/providers/packet/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/providers/proxmox/__init__.py` & `kcli-99.0.202404020921/kvirt/providers/proxmox/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/providers/sampleprovider.py` & `kcli-99.0.202404020921/kvirt/providers/sampleprovider.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/providers/vsphere/__init__.py` & `kcli-99.0.202404020921/kvirt/providers/vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/providers/vsphere/helpers.py` & `kcli-99.0.202404020921/kvirt/providers/vsphere/helpers.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/providers/vsphere/tagging.py` & `kcli-99.0.202404020921/kvirt/providers/vsphere/tagging.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/providers/web/__init__.py` & `kcli-99.0.202404020921/kvirt/providers/web/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/__init__.py` & `kcli-99.0.202404020921/kvirt/web/__init__.py`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/css/bootstrap-theme.min.css` & `kcli-99.0.202404020921/kvirt/web/static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/css/bootstrap.min.css` & `kcli-99.0.202404020921/kvirt/web/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/css/jquery.dataTables.min.css` & `kcli-99.0.202404020921/kvirt/web/static/css/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/css/kcli.css` & `kcli-99.0.202404020921/kvirt/web/static/css/kcli.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/css/navbar.css` & `kcli-99.0.202404020921/kvirt/web/static/css/navbar.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/css/spice.css` & `kcli-99.0.202404020921/kvirt/web/static/css/spice.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/fonts/glyphicons-halflings-regular.woff2` & `kcli-99.0.202404020921/kvirt/web/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/images/Centos.png` & `kcli-99.0.202404020921/kvirt/web/static/images/Centos.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/images/Fedora.png` & `kcli-99.0.202404020921/kvirt/web/static/images/Fedora.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/images/Redhat.png` & `kcli-99.0.202404020921/kvirt/web/static/images/Redhat.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/images/Suse.png` & `kcli-99.0.202404020921/kvirt/web/static/images/Suse.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/images/Tux.png` & `kcli-99.0.202404020921/kvirt/web/static/images/Tux.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/images/Ubuntu.png` & `kcli-99.0.202404020921/kvirt/web/static/images/Ubuntu.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/images/delete.png` & `kcli-99.0.202404020921/kvirt/web/static/images/delete.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/images/favicon.ico` & `kcli-99.0.202404020921/kvirt/web/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/images/kcli-small.png` & `kcli-99.0.202404020921/kvirt/web/static/images/kcli-small.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/images/kcli.jpg` & `kcli-99.0.202404020921/kvirt/web/static/images/kcli.jpg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/images/kcli.png` & `kcli-99.0.202404020921/kvirt/web/static/images/kcli.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/images/logo-header.svg` & `kcli-99.0.202404020921/kvirt/web/static/images/logo-header.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/images/logo-main.svg` & `kcli-99.0.202404020921/kvirt/web/static/images/logo-main.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/images/start.png` & `kcli-99.0.202404020921/kvirt/web/static/images/start.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/images/stop.png` & `kcli-99.0.202404020921/kvirt/web/static/images/stop.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/images/wheel.gif` & `kcli-99.0.202404020921/kvirt/web/static/images/wheel.gif`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/bootstrap-notify.js` & `kcli-99.0.202404020921/kvirt/web/static/js/bootstrap-notify.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/bootstrap.min.js` & `kcli-99.0.202404020921/kvirt/web/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/containeraction.js` & `kcli-99.0.202404020921/kvirt/web/static/js/containeraction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/dataTables.checkboxes.min.js` & `kcli-99.0.202404020921/kvirt/web/static/js/dataTables.checkboxes.min.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/hostaction.js` & `kcli-99.0.202404020921/kvirt/web/static/js/hostaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/imageaction.js` & `kcli-99.0.202404020921/kvirt/web/static/js/imageaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/jquery.dataTables.min.js` & `kcli-99.0.202404020921/kvirt/web/static/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/jquery.min.js` & `kcli-99.0.202404020921/kvirt/web/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/kcli.js` & `kcli-99.0.202404020921/kvirt/web/static/js/kcli.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/kubeaction.js` & `kcli-99.0.202404020921/kvirt/web/static/js/kubeaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/list.js` & `kcli-99.0.202404020921/kvirt/web/static/js/list.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/networkaction.js` & `kcli-99.0.202404020921/kvirt/web/static/js/networkaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/planaction.js` & `kcli-99.0.202404020921/kvirt/web/static/js/planaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/poolaction.js` & `kcli-99.0.202404020921/kvirt/web/static/js/poolaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/productaction.js` & `kcli-99.0.202404020921/kvirt/web/static/js/productaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/repoaction.js` & `kcli-99.0.202404020921/kvirt/web/static/js/repoaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/snapshotaction.js` & `kcli-99.0.202404020921/kvirt/web/static/js/snapshotaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/atKeynames.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/atKeynames.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/bitmap.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/bitmap.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/cursor.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/cursor.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/display.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/display.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/enums.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/enums.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/filexfer.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/filexfer.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/inputs.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/inputs.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/lz.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/lz.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/main.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/main.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/playback.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/playback.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/png.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/png.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/port.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/port.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/quic.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/quic.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/resize.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/resize.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/simulatecursor.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/simulatecursor.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/spicearraybuffer.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/spicearraybuffer.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/spiceconn.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/spiceconn.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/spicedataview.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/spicedataview.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/spicemsg.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/spicemsg.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/spicetype.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/spicetype.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/babel-worker.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/babel-worker.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/browser-es-module-loader.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/browser-es-module-loader.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/thirdparty/jsbn.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/thirdparty/jsbn.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/thirdparty/prng4.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/thirdparty/prng4.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/thirdparty/rng.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/thirdparty/rng.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/thirdparty/rsa.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/thirdparty/rsa.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/thirdparty/sha1.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/thirdparty/sha1.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/ticket.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/ticket.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/utils.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/utils.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/webm.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/webm.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/spice/wire.js` & `kcli-99.0.202404020921/kvirt/web/static/js/spice/wire.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/js/vmaction.js` & `kcli-99.0.202404020921/kvirt/web/static/js/vmaction.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/error-handler.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/error-handler.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/alt.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/alt.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/clipboard.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/clipboard.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/connect.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/connect.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/ctrl.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/ctrl.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/ctrlaltdel.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/ctrlaltdel.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/disconnect.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/disconnect.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/drag.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/drag.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/error.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/error.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/esc.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/esc.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/expander.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/expander.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/fullscreen.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/fullscreen.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/handle.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/handle.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/handle_bg.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/handle_bg.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/Makefile` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/Makefile`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-120x120.png` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-120x120.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-144x144.png` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-144x144.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-152x152.png` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-152x152.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-16x16.png` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-16x16.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-192x192.png` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-192x192.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-24x24.png` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-24x24.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-32x32.png` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-32x32.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-48x48.png` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-48x48.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-60x60.png` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-60x60.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-64x64.png` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-64x64.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-72x72.png` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-72x72.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-76x76.png` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-76x76.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-96x96.png` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-96x96.png`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-icon-sm.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-icon-sm.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/icons/novnc-icon.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/icons/novnc-icon.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/info.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/info.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/keyboard.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/keyboard.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/mouse_left.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/mouse_left.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/mouse_middle.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/mouse_middle.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/mouse_none.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/mouse_none.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/mouse_right.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/mouse_right.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/power.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/power.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/settings.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/settings.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/tab.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/tab.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/toggleextrakeys.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/toggleextrakeys.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/warning.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/warning.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/images/windows.svg` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/images/windows.svg`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/cs.json` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/cs.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/de.json` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/de.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/el.json` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/el.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/es.json` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/es.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/ja.json` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/ja.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/ko.json` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/ko.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/nl.json` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/nl.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/pl.json` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/pl.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/ru.json` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/ru.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/sv.json` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/sv.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/tr.json` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/tr.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/zh_CN.json` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/zh_CN.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/locale/zh_TW.json` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/locale/zh_TW.json`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/localization.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/localization.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/sounds/bell.mp3` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/sounds/bell.mp3`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/sounds/bell.oga` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/sounds/bell.oga`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/styles/Orbitron700.ttf` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/styles/Orbitron700.ttf`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/styles/Orbitron700.woff` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/styles/Orbitron700.woff`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/styles/base.css` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/styles/base.css`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/ui.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/ui.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/app/webutil.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/app/webutil.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/base64.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/base64.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/decoders/copyrect.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/decoders/copyrect.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/decoders/hextile.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/decoders/hextile.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/decoders/raw.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/decoders/raw.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/decoders/rre.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/decoders/rre.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/decoders/tight.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/decoders/tight.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/decoders/tightpng.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/decoders/tightpng.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/des.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/des.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/display.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/display.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/encodings.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/encodings.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/inflator.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/inflator.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/input/domkeytable.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/input/domkeytable.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/input/fixedkeys.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/input/fixedkeys.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/input/keyboard.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/input/keyboard.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/input/keysym.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/input/keysym.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/input/keysymdef.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/input/keysymdef.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/input/mouse.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/input/mouse.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/input/util.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/input/util.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/input/vkeys.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/input/vkeys.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/input/xtscancodes.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/input/xtscancodes.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/rfb.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/rfb.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/util/browser.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/util/browser.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/util/cursor.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/util/cursor.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/util/events.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/util/events.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/util/eventtarget.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/util/eventtarget.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/util/logging.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/util/logging.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/util/polyfill.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/util/polyfill.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/core/websock.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/core/websock.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/babel-worker.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/babel-worker.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/browser-es-module-loader.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/browser-es-module-loader/src/browser-es-module-loader.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/LICENSE` & `kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/LICENSE`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/utils/common.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/utils/common.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/adler32.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/adler32.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/constants.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/constants.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/crc32.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/crc32.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/deflate.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/deflate.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/gzheader.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/gzheader.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/inffast.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/inffast.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/inflate.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/inflate.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/inftrees.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/inftrees.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/messages.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/messages.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/trees.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/trees.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/pako/lib/zlib/zstream.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/pako/lib/zlib/zstream.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/static/vnc/vendor/promise.js` & `kcli-99.0.202404020921/kvirt/web/static/vnc/vendor/promise.js`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/bootstrap.html` & `kcli-99.0.202404020921/kvirt/web/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/console.html` & `kcli-99.0.202404020921/kvirt/web/templates/console.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/containercreate.html` & `kcli-99.0.202404020921/kvirt/web/templates/containercreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/containerprofilestable.html` & `kcli-99.0.202404020921/kvirt/web/templates/containerprofilestable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/containerstable.html` & `kcli-99.0.202404020921/kvirt/web/templates/containerstable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/head.html` & `kcli-99.0.202404020921/kvirt/web/templates/head.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/hoststable.html` & `kcli-99.0.202404020921/kvirt/web/templates/hoststable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/imagecreate.html` & `kcli-99.0.202404020921/kvirt/web/templates/imagecreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/imagestable.html` & `kcli-99.0.202404020921/kvirt/web/templates/imagestable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/kubecreate.html` & `kcli-99.0.202404020921/kvirt/web/templates/kubecreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/kubeinfo.html` & `kcli-99.0.202404020921/kvirt/web/templates/kubeinfo.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/kubeprofilestable.html` & `kcli-99.0.202404020921/kvirt/web/templates/kubeprofilestable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/kubestable.html` & `kcli-99.0.202404020921/kvirt/web/templates/kubestable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/navbar.html` & `kcli-99.0.202404020921/kvirt/web/templates/navbar.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/networkcreate.html` & `kcli-99.0.202404020921/kvirt/web/templates/networkcreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/networks.html` & `kcli-99.0.202404020921/kvirt/web/templates/networks.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/networkstable.html` & `kcli-99.0.202404020921/kvirt/web/templates/networkstable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/plancreate.html` & `kcli-99.0.202404020921/kvirt/web/templates/plancreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/planstable.html` & `kcli-99.0.202404020921/kvirt/web/templates/planstable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/poolcreate.html` & `kcli-99.0.202404020921/kvirt/web/templates/poolcreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/poolstable.html` & `kcli-99.0.202404020921/kvirt/web/templates/poolstable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/productcreate.html` & `kcli-99.0.202404020921/kvirt/web/templates/productcreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/productstable.html` & `kcli-99.0.202404020921/kvirt/web/templates/productstable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/repocreate.html` & `kcli-99.0.202404020921/kvirt/web/templates/repocreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/repostable.html` & `kcli-99.0.202404020921/kvirt/web/templates/repostable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/vmcreate.html` & `kcli-99.0.202404020921/kvirt/web/templates/vmcreate.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/vmprofilestable.html` & `kcli-99.0.202404020921/kvirt/web/templates/vmprofilestable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/kvirt/web/templates/vmstable.html` & `kcli-99.0.202404020921/kvirt/web/templates/vmstable.html`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/samples/config.yml` & `kcli-99.0.202404020921/samples/config.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/samples/profiles.yml` & `kcli-99.0.202404020921/samples/profiles.yml`

 * *Files identical despite different names*

### Comparing `kcli-99.0.202404011739/setup.py` & `kcli-99.0.202404020921/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 description = 'Provisioner/Manager for Libvirt/Vsphere/Aws/Gcp/Kubevirt/Ovirt/Openstack/IBM Cloud and containers'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='kcli',
-    version='99.0.202404011739',
+    version='99.0.202404020921',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/kcli',
     author='Karim Boumedhel',
```

### Comparing `kcli-99.0.202404011739/tests/test_kvirt.py` & `kcli-99.0.202404020921/tests/test_kvirt.py`

 * *Files identical despite different names*

