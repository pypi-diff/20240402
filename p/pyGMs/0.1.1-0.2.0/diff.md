# Comparing `tmp/pyGMs-0.1.1.tar.gz` & `tmp/pyGMs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGMs-0.1.1.tar", last modified: Wed Apr  6 17:30:03 2022, max compression
+gzip compressed data, was "pyGMs-0.2.0.tar", last modified: Tue Apr  2 00:45:18 2024, max compression
```

## Comparing `pyGMs-0.1.1.tar` & `pyGMs-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,49 @@
-drwxrwxr-x   0 ihler     (1000) ihler     (1000)        0 2022-04-06 17:30:03.015893 pyGMs-0.1.1/
--rw-rw-r--   0 ihler     (1000) ihler     (1000)     1392 2022-04-06 17:30:03.015893 pyGMs-0.1.1/PKG-INFO
-drwxrwxr-x   0 ihler     (1000) ihler     (1000)        0 2022-04-06 17:30:03.015893 pyGMs-0.1.1/pyGMs/
--rw-rw-r--   0 ihler     (1000) ihler     (1000)      644 2022-04-06 17:29:03.000000 pyGMs-0.1.1/pyGMs/__init__.py
--rw-rw-r--   0 ihler     (1000) ihler     (1000)    11296 2022-04-06 17:29:03.000000 pyGMs-0.1.1/pyGMs/draw.py
--rw-rw-r--   0 ihler     (1000) ihler     (1000)    28567 2022-04-06 17:29:03.000000 pyGMs-0.1.1/pyGMs/factor.py
--rw-rw-r--   0 ihler     (1000) ihler     (1000)    27188 2022-04-06 17:29:03.000000 pyGMs-0.1.1/pyGMs/factorSparse.py
--rw-rw-r--   0 ihler     (1000) ihler     (1000)    27032 2022-04-06 17:29:03.000000 pyGMs-0.1.1/pyGMs/filetypes.py
--rw-rw-r--   0 ihler     (1000) ihler     (1000)    39584 2022-04-06 17:29:03.000000 pyGMs-0.1.1/pyGMs/graphmodel.py
--rw-rw-r--   0 ihler     (1000) ihler     (1000)    28147 2022-04-06 17:29:03.000000 pyGMs-0.1.1/pyGMs/ising.py
--rw-rw-r--   0 ihler     (1000) ihler     (1000)    10764 2021-02-10 02:10:13.000000 pyGMs-0.1.1/pyGMs/messagepass.py
--rw-rw-r--   0 ihler     (1000) ihler     (1000)     8572 2022-04-06 17:29:03.000000 pyGMs-0.1.1/pyGMs/misc.py
--rw-rw-r--   0 ihler     (1000) ihler     (1000)     8766 2022-04-06 17:29:03.000000 pyGMs-0.1.1/pyGMs/montecarlo.py
--rw-rw-r--   0 ihler     (1000) ihler     (1000)    10135 2021-02-10 00:24:22.000000 pyGMs-0.1.1/pyGMs/search.py
--rw-rw-r--   0 ihler     (1000) ihler     (1000)     2569 2022-04-06 17:29:03.000000 pyGMs-0.1.1/pyGMs/varset_py.py
--rw-rw-r--   0 ihler     (1000) ihler     (1000)    17832 2021-02-10 00:24:22.000000 pyGMs-0.1.1/pyGMs/weighted.py
--rw-r--r--   0 ihler     (1000) ihler     (1000)    30094 2020-06-11 19:15:54.000000 pyGMs-0.1.1/pyGMs/wmb.py
--rw-rw-r--   0 ihler     (1000) ihler     (1000)    13545 2022-04-06 17:29:03.000000 pyGMs-0.1.1/pyGMs/wogm.py
-drwxrwxr-x   0 ihler     (1000) ihler     (1000)        0 2022-04-06 17:30:03.015893 pyGMs-0.1.1/pyGMs.egg-info/
--rw-rw-r--   0 ihler     (1000) ihler     (1000)     1392 2022-04-06 17:30:02.000000 pyGMs-0.1.1/pyGMs.egg-info/PKG-INFO
--rw-rw-r--   0 ihler     (1000) ihler     (1000)      383 2022-04-06 17:30:03.000000 pyGMs-0.1.1/pyGMs.egg-info/SOURCES.txt
--rw-rw-r--   0 ihler     (1000) ihler     (1000)        1 2022-04-06 17:30:02.000000 pyGMs-0.1.1/pyGMs.egg-info/dependency_links.txt
--rw-rw-r--   0 ihler     (1000) ihler     (1000)        6 2022-04-06 17:30:02.000000 pyGMs-0.1.1/pyGMs.egg-info/top_level.txt
--rw-rw-r--   0 ihler     (1000) ihler     (1000)       38 2022-04-06 17:30:03.015893 pyGMs-0.1.1/setup.cfg
--rw-rw-r--   0 ihler     (1000) ihler     (1000)      685 2022-04-06 17:29:03.000000 pyGMs-0.1.1/setup.py
+drwxrwxr-x   0 ihler     (1000) ihler     (1000)        0 2024-04-02 00:45:18.502948 pyGMs-0.2.0/
+-rw-r--r--   0 ihler     (1000) ihler     (1000)     1357 2024-04-02 00:45:18.498948 pyGMs-0.2.0/PKG-INFO
+drwxrwxr-x   0 ihler     (1000) ihler     (1000)        0 2024-04-02 00:45:18.494948 pyGMs-0.2.0/pyGMs/
+-rw-rw-r--   0 ihler     (1000) ihler     (1000)      644 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/__init__.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)     1108 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/_profile.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)    12746 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/_rbm.py
+-rw-rw-r--   0 ihler     (1000) ihler     (1000)     1214 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/causal.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)    17205 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/csp.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)    14063 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/draw.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)    28718 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/factor.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)    11524 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/factorGauss.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)    27378 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/factorSparse.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)    27698 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/filetypes.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)    34629 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/graphmodel.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)     4032 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/indexedheap.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)    31037 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/ising.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)     9930 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/jupyter.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)     8302 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/learning.py
+-rw-rw-r--   0 ihler     (1000) ihler     (1000)    10785 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/messagepass.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)     9808 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/misc.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)    11627 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/montecarlo.py
+-rw-rw-r--   0 ihler     (1000) ihler     (1000)     7976 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/regiongraph.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)    10768 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/search.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)    27279 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/search1.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)    12269 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/search2.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)    10830 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/search_sum.py
+-rw-rw-r--   0 ihler     (1000) ihler     (1000)     2570 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/varset_py.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)     6510 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/varset_py2.py
+-rw-rw-r--   0 ihler     (1000) ihler     (1000)    17837 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/weighted.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)    34246 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/wmb.py
+-rw-rw-r--   0 ihler     (1000) ihler     (1000)    13545 2024-04-02 00:43:20.000000 pyGMs-0.2.0/pyGMs/wogm.py
+drwxrwxr-x   0 ihler     (1000) ihler     (1000)        0 2024-04-02 00:45:18.498948 pyGMs-0.2.0/pyGMs.egg-info/
+-rw-r--r--   0 ihler     (1000) ihler     (1000)     1357 2024-04-02 00:45:18.000000 pyGMs-0.2.0/pyGMs.egg-info/PKG-INFO
+-rw-rw-r--   0 ihler     (1000) ihler     (1000)      812 2024-04-02 00:45:18.000000 pyGMs-0.2.0/pyGMs.egg-info/SOURCES.txt
+-rw-rw-r--   0 ihler     (1000) ihler     (1000)        1 2024-04-02 00:45:18.000000 pyGMs-0.2.0/pyGMs.egg-info/dependency_links.txt
+-rw-rw-r--   0 ihler     (1000) ihler     (1000)        6 2024-04-02 00:45:18.000000 pyGMs-0.2.0/pyGMs.egg-info/top_level.txt
+-rw-rw-r--   0 ihler     (1000) ihler     (1000)       38 2024-04-02 00:45:18.502948 pyGMs-0.2.0/setup.cfg
+-rw-rw-r--   0 ihler     (1000) ihler     (1000)      685 2024-04-02 00:45:07.000000 pyGMs-0.2.0/setup.py
+drwxrwxr-x   0 ihler     (1000) ihler     (1000)        0 2024-04-02 00:45:18.498948 pyGMs-0.2.0/tests/
+-rw-rw-r--   0 ihler     (1000) ihler     (1000)     1998 2022-04-06 17:25:50.000000 pyGMs-0.2.0/tests/testDraw.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)    32665 2022-04-06 17:25:50.000000 pyGMs-0.2.0/tests/testFactor.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)    32701 2022-04-06 17:25:50.000000 pyGMs-0.2.0/tests/testFactorSp.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)    18194 2023-08-29 17:58:57.000000 pyGMs-0.2.0/tests/testGraphModel.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)     8812 2022-04-06 17:25:50.000000 pyGMs-0.2.0/tests/testIsing.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)      981 2022-04-06 17:25:50.000000 pyGMs-0.2.0/tests/testJG.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)     5697 2022-04-06 17:25:50.000000 pyGMs-0.2.0/tests/testLimid.py
+-rw-rw-r--   0 ihler     (1000) ihler     (1000)     3528 2022-04-06 17:25:50.000000 pyGMs-0.2.0/tests/testMisc.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)     2051 2022-04-06 17:25:50.000000 pyGMs-0.2.0/tests/testNotebooks.py
+-rw-r--r--   0 ihler     (1000) ihler     (1000)     2376 2022-04-06 17:25:50.000000 pyGMs-0.2.0/tests/testWmb.py
```

### Comparing `pyGMs-0.1.1/PKG-INFO` & `pyGMs-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: pyGMs
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python Graphical Models Toolbox
 Author: Alexander Ihler
 Author-email: ihler@ics.uci.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-pyGM : A Python toolbox for Graphical Models
+pyGMs : A Python toolbox for Graphical Models
 ================
 
 This code provides a simple Python-based interface for defining probabilistic
 graphical models (Bayesian networks, factor graphs, etc.) over discrete random
 variables, along with a number of routines for approximate inference.  It is
 being developed for use in teaching, as well as prototyping for research.
 
@@ -24,21 +22,19 @@
 operating on the table-based representation of discrete factors, and
 [SortedContainers](https://pypi.python.org/pypi/sortedcontainers) for some
 internal representations.  Smaller portions use [networkx](https://networkx.org/)
 and [scipy](https://www.scipy.org/) as well.
 
 ## Installation
 
-Simply download or clone the repository to a directory *pyGM*, and add its
+Simply download or clone the repository to a directory *pyGMs*, and add its
 parent directory to your Python path, either:
 ```
 $ export PYTHONPATH=${PYTHONPATH}:/directory/containing/
 ```
 or in Python
 ```
 import sys
 sys.path.append('/directory/containing/')
 ```
 
 
-
-
```

### Comparing `pyGMs-0.1.1/pyGMs/__init__.py` & `pyGMs-0.2.0/pyGMs/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 pyGMs: Python Graphical Model code
 
 A simple graphical model class for learning about, testing, and developing algorithms
 for graphical models.
 
-Version 0.1.1 (2022-04-06)
-Version 0.1.1 (2022-04-06)
+Version 0.2.0 (2024-04-01)
+Version 0.2.0 (2024-04-01)
 
 (c) 2015- Alexander Ihler under the FreeBSD license; see license.txt for details.
 """
 
 import numpy as np;
 from sortedcontainers import SortedSet as sset;
```

### Comparing `pyGMs-0.1.1/pyGMs/draw.py` & `pyGMs-0.2.0/pyGMs/draw.py`

 * *Files 24% similar despite different names*

```diff
@@ -180,24 +180,24 @@
     >>> gm.drawBayesNet(model, labels={0:'0', ... } )    # keyword args passed to networkx.draw()
     """
     import networkx as nx
     import copy
     kwargs = copy.copy(kwargs)    # make a copy of the arguments dict for mutation
     topo_order = bnOrder(model)                              # TODO: allow user-provided order?
     if topo_order is None: raise ValueError('Topo order not found; model is not a Bayes Net?')
-    pri = np.zeros((len(topo_order),))-1
+    pri = np.zeros((max(topo_order)+1,))-1
     pri[topo_order] = np.arange(len(topo_order))
     G = nx.DiGraph()
     G.add_nodes_from( [v.label for v in model.X if v.states > 1] )  # only non-trivial vars
     for f in model.factors:
       v2label = topo_order[ int(max(pri[v.label] for v in f.vars)) ]
       for v1 in f.vars:
         if (v1.label != v2label): G.add_edge(v1.label,v2label)
 
-    kwargs['var_labels'] = kwargs.get('var_labels',{n:n for n in [v.label for v in model.X]})
+    kwargs['var_labels'] = kwargs.get('var_labels',{n:n for n in [v.label for v in model.X if v.states>1]})
     kwargs['labels'] = kwargs.get('labels', kwargs.get('var_labels',{}) )
     kwargs.pop('var_labels',None)   # remove artificial "var_labels" entry)
     kwargs['arrowstyle'] = kwargs.get('arrowstyle','->')
     kwargs['arrowsize'] = kwargs.get('arrowsize',10)
     kwargs['edgecolors'] = kwargs.get('edgecolors','k')
     nx.draw(G,**kwargs)
     return G
@@ -219,15 +219,15 @@
     decisions = [d[-1] for d in D]                       # list the decision variables
     model = GraphModel( C + [Factor(d,1.) for d in D] )  # get all chance & decision vars, arcs
     chance = [c for c in model.X if c not in decisions]
     util = [-i-1 for i,u in enumerate(U)]
     cpd_edges, util_edges, info_edges = [],[],[]
     topo_order = bnOrder(model)
     if topo_order is None: raise ValueError('Topo order not found; graph is not a Bayes Net?')
-    pri = np.zeros((len(topo_order),))-1
+    pri = np.zeros((max(topo_order)+1,))-1
     pri[topo_order] = np.arange(len(topo_order))
     G = nx.DiGraph()
     G.add_nodes_from( [v.label for v in model.X if v.states > 1] )  # only non-trivial vars
     G.add_nodes_from( util )                                       # add utility nodes
     for f in model.factors:
       v2label = topo_order[ int(max(pri[v.label] for v in f.vars)) ]
       for v1 in f.vars:
@@ -253,7 +253,73 @@
 
 
 
 #def drawJGraph(
 
 
 
+#### TODO: fix & test
+#def drawSearchTree(root):
+#    """G, pos = drawSearchTree(root) :  return nxGraph of a current search tree, and position information."""
+#    nodes = [[(-root.value,root)],[]]
+#    while True:
+#        for n in nodes[-2]:
+#            nodes[-1] += n[1].children
+#        if len(nodes[-1])==0: break
+#        nodes.append([])
+#    pos = {}
+#    for d in range(len(nodes)-1,-1,-1):
+#        p = 0.
+#        for vn,n in nodes[d]:
+#            if len(n.children)>0:
+#                p = np.mean([pos[c][0] for vc,c in n.children])
+#                pos[n] = (p, -d*1.)
+#                p = np.max([pos[c] for vc,c in n.children]) + 1.
+#            else:
+#                pos[n] = (p,-d*1.)
+#                p += 1
+#    G = nx.Graph(); G.add_nodes_from([n for ns in nodes for n in ns]);
+#    G.add_edges_from([(p,n) for ns in nodes[:-1] for p in ns for n in p.children])
+#    return G,pos
+
+def nxTreeLayout(G):
+    """pos = nxTreeLayout(G) :  return positions for root-down layout of a tree."""
+    depth = {}; by_depth = {}
+    for n in G.nodes: 
+        dn = n.count(',')+n.count('.')  # number of variables & number of values    
+        depth[n] = dn
+        by_depth[dn] = [n] if dn not in by_depth else by_depth[dn]+[n]
+
+    pos = {}
+    leaves = sorted([n for n in G.nodes if len(G.out_edges(n))==0])
+    max_depth = max(by_depth.keys());
+    x = -1.
+    for i,l in enumerate(leaves): 
+        if i>0:
+            x += 1. + np.log2(depth[l] - depth[nx.lowest_common_ancestor(G,l,leaves[i-1])])
+        else: x += 1. + 0*np.log2(max_depth - depth[l]+1)
+        pos[l] = (x,-depth[l]);
+        
+    for d in range(max_depth,-1,-1):
+        if d not in by_depth: continue
+        for n in by_depth[d]: 
+            if n not in pos: pos[n] = (np.mean([pos[c[1]][0] for c in G.out_edges(n)]), -depth[n])
+    return pos
+
+## TODO: nxTuneTreeLayout? Make tree layout look nicer?
+
+
+
+def nx2tikz(G,pos, precision=1, use_names=True):
+    latex = "\\begin{tikzpicture} \n"
+    latex+= "  \\tikzset{var/.style = {shape=circle,draw,minimum size=1.2em}} \n"
+    latex+= "  \\tikzset{edge/.style = {->,> = latex,line width=0.5mm}} \n"
+    nodes = list(G.nodes)
+    id = lambda n: n if use_names else nodes.index(n)
+    locat = np.array([pos[key] for key in nodes]).reshape(-1,2).round(precision)
+    latex += "  \\foreach \\name/\\pos in {"+",".join(["{"+"{}/({},{})".format(id(nodes[i]),locat[i,0],locat[i,1])+"}" for i in range(len(locat))])+"}\n"
+    latex += "    \\node[var] (\\name) at \\pos {$\\name$}; \n"
+    latex += "  \\foreach \\pa/\\ch in {"+",".join(["{"+"{}/{}".format(id(e[0]),id(e[1]))+"}" for e in G.edges])+"}\n"
+    latex += "    \\draw[edge] (\\pa) to (\\ch); \n"
+    latex += "\\end{tikzpicture} \n"
+    return latex
+
```

### Comparing `pyGMs-0.1.1/pyGMs/factor.py` & `pyGMs-0.2.0/pyGMs/factor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 factor.py
 
 Defines variables, variable sets, and dense factors over discrete variables (tables) for graphical models
 
-Version 0.1.1 (2022-04-06)
+Version 0.2.0 (2024-04-01)
 (c) 2015-2021 Alexander Ihler under the FreeBSD license; see license.txt for details.
 """
 
 import numpy as np
 #import autograd.numpy as np
 from sortedcontainers import SortedSet as sset
 
@@ -19,14 +19,18 @@
   from pyGMs.varset_py import Var,VarSet    # sortedcontainers version
   #from .varset_py2 import Var,VarSet  # numpy array version
 
 
 
 inf = float('inf')
 
+def _cfg2str(cfg,X=None): 
+  if X is None: X = range(max(cfg.keys())+1)
+  return ''.join(str(cfg[i]) if i in cfg else '-' for i in X);
+
 
 orderMethod = 'F'   # TODO: currently stores in fortran order (as Matlab); should be trivially changable
 #orderMethod = 'C'  #   Can we make this "seamless" to the user, and/or force them to do something consistent?
 
 # Notes: column-major (order=F) puts last index sequentially ("big endian"): t[0 0 0], t[0 0 1], t[0 1 0] ...
 #        row major (order=C) puts 1st index sequentially ("little endian"): t[0 0 0], t[1 0 0], t[0 1 0], ...
 
@@ -95,15 +99,15 @@
   def changeVars(self, vars, copy=True):
     """Copy a factor but change its arguments (scope).
  
        >>> f = Factor([X0,X1], table)      
        >>> g = changeVars( f, [X7,X5])   # now,  g(X5=b,X7=a) = f(X0=a,X1=b)
     """
     v = VarSet(vars)
-    newOrder = map(lambda x:vars.index(x), v)
+    newOrder = tuple(map(lambda x:vars.index(x), v))
     if copy: ret = Factor(v, self.t.transpose(newOrder))
     else:    ret = Factor().__build(v, self.t.transpose(newOrder))  # try not to copy if possible
     return ret
 
   def __repr__(self):
     """Detailed representation: scope (varset) + table memory location"""
     return 'Factor({:s},[0x{:x}])'.format(str(self.v),self.t.ctypes.data)
@@ -389,61 +393,61 @@
     with np.errstate(divide='ignore'):
       return self.__opExpand2(that,np.divide, out=self)
 
   __itruediv__ = __idiv__
 
   #### ELIMINATION OPERATIONS ####
   def sum(self, elim=None, out=None):
-    """Eliminate via sum on F, e.g., f(X_2) = \sum_{x_1} F(x_1,X_2) = F.sum([X1])"""
+    """Eliminate via sum on F, e.g., f(X_2) = \\sum_{x_1} F(x_1,X_2) = F.sum([X1])"""
     if (elim is None): elim = self.v
     return self.__opReduce2(self.v & elim,np.sum, out=out)
 
   def marginal(self, target, out=None):
-    """Compute the marginal of F, e.g., f(X_2) = \sum_{x_1} F(x_1,X_2) = F.marginal([X2])"""
+    """Compute the marginal of F, e.g., f(X_2) = \\sum_{x_1} F(x_1,X_2) = F.marginal([X2])"""
     return self.__opReduce2(self.v - target,np.sum, out=out)
 
   def sumPower(self, elim=None, power=1.0, out=None):
     """Eliminate via powered sum, e.g., f(X_2) =  \\root^{1/p}{ sum_{x_1} F(x_1,X_2)^p } = F.sumPower([X1],p)"""
     if (elim is None): elim = self.v
     tmp = (self ** power).sum(elim)
     tmp **= (1.0/power)
     return tmp
 
   def lse(self, elim=None, out=None):
-    """Eliminate via log-sum-exp on F, e.g., f(X_2) = log \sum_{x_1} exp F(x_1,X_2) = F.lse([X1])"""
+    """Eliminate via log-sum-exp on F, e.g., f(X_2) = log \\sum_{x_1} exp F(x_1,X_2) = F.lse([X1])"""
     if (elim is None): elim = self.v
     return self.__opReduce3(self.v & elim, np.logaddexp.reduce, out=out)
 
   def lsePower(self, elim=None, power=1.0, out=None):
-    """Eliminate via powered log-sum-exp, e.g., f(X_2) = 1/p log \sum_{x_1} exp F(x_1,X_2)*p = F.lsePower([X_1],p)"""
+    """Eliminate via powered log-sum-exp, e.g., f(X_2) = 1/p log \\sum_{x_1} exp F(x_1,X_2)*p = F.lsePower([X_1],p)"""
     if (elim is None): elim = self.v
     if   power == inf: return self.max(elim)
     elif power == -inf: return self.min(elim)
     elif power == 1.0:  return self.lse(elim)
     else:
       tmp = (self*power).lse(elim)
       tmp *= (1.0/power)
       return tmp
 
   def max(self, elim=None, out=None):
-    """Eliminate via max on F, e.g., f(X_2) = \max_{x_1} F(x_1,X_2) = F.max([X1])"""
+    """Eliminate via max on F, e.g., f(X_2) = \\max_{x_1} F(x_1,X_2) = F.max([X1])"""
     if (elim is None): elim = self.v
     return self.__opReduce2(self.v & elim,np.max, out=out)
 
   def maxmarginal(self, target, out=None):
-    """Compute the max-marginal of F, e.g., f(X_2) = \max_{x_1} F(x_1,X_2) = F.maxmarginal([X2])"""
+    """Compute the max-marginal of F, e.g., f(X_2) = \\max_{x_1} F(x_1,X_2) = F.maxmarginal([X2])"""
     return self.__opReduce2(self.v - target,np.max, out=out)
 
   def min(self, elim=None, out=None):
-    """Eliminate via min on F, e.g., f(X_2) = \min_{x_1} F(x_1,X_2) = F.min([X1])"""
+    """Eliminate via min on F, e.g., f(X_2) = \\min_{x_1} F(x_1,X_2) = F.min([X1])"""
     if (elim is None): elim = self.v
     return self.__opReduce2(self.v & elim,np.min, out=out)
 
   def minmarginal(self, target, out=None):
-    """Compute the min-marginal of F, e.g., f(X_2) = \min_{x_1} F(x_1,X_2) = F.minmarginal([X2])"""
+    """Compute the min-marginal of F, e.g., f(X_2) = \\min_{x_1} F(x_1,X_2) = F.minmarginal([X2])"""
     return self.__opReduce2(self.v - target,np.min, out=out)
 
 
     # use ufunc.reduceat?  reduce etc seem not good?
     # frompyfunc to make ufunc from python function?
     # use "externalloop" flag?
     #return t.max(axis=None,out=None) # use axis to specific dimensions to eliminate; out for IP version
```

### Comparing `pyGMs-0.1.1/pyGMs/factorSparse.py` & `pyGMs-0.2.0/pyGMs/factorSparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 factorSparse.py
 
 Defines sparse factors over discrete variables (tables) for graphical models
 
-Version 0.1.1 (2022-04-06)
+Version 0.2.0 (2024-04-01)
 (c) 2019 Alexander Ihler under the FreeBSD license; see license.txt for details.
 """
 
 import numpy as np
 #import autograd.numpy as np
 from sortedcontainers import SortedSet as sset
 
@@ -70,25 +70,28 @@
     except TypeError:                                   # if not iterable (e.g. single variable)
       self.v = VarSet()                                 #   try just adding it
       self.v.add(vars)
     #assert( self.v.nrStates() > 0)
     #if self.v.nrStatesDouble() > 1e8: raise ValueError("Too big!");
 
     self.t = {}
-    try:
-      tmp_t = np.empty(self.v.dims(), float, orderMethod);
-      tmp_t[:] = vals
-      for i in np.ndindex( tuple(self.v.dims()) ):
-        if tmp_t[i] != 0.0: self.t[i] = tmp_t[i]
-    except ValueError:
-      tmp_t = np.reshape(np.array(vals, float), self.v.dims(), orderMethod)  # try again using reshape
-      for i in np.ndindex( tuple(self.v.dims()) ):
-        if tmp_t[i] != 0.0: self.t[i] = tmp_t[i]
-    except TypeError:
-      self.t = dict(vals)
+    if type(vals) is dict:
+      self.t = vals
+    elif not (type(vals) is float and vals==0.):
+      try:	
+        tmp_t = np.empty(self.v.dims(), float, orderMethod);
+        tmp_t[:] = vals
+        for i in np.ndindex( tuple(self.v.dims()) ):
+          if tmp_t[i] != 0.0: self.t[i] = tmp_t[i]
+      except ValueError:
+        tmp_t = np.reshape(np.array(vals, float), self.v.dims(), orderMethod)  # try again using reshape
+        for i in np.ndindex( tuple(self.v.dims()) ):
+          if tmp_t[i] != 0.0: self.t[i] = tmp_t[i]
+      except TypeError:
+        self.t = dict(vals)
 
 
   def __build(self,vs,table):
     """Internal build function from numpy ndarray"""
     self.v = vs
     self.t = table
     return self
@@ -354,62 +357,62 @@
     with np.errstate(divide='ignore'):
       return self.__opExpand2(that,np.divide, out=self)
 
   __itruediv__ = __idiv__
 
   #### ELIMINATION OPERATIONS ####
   def sum(self, elim=None, out=None):
-    """Eliminate via sum on F, e.g., f(X_2) = \sum_{x_1} F(x_1,X_2) = F.sum([X1])"""
+    """Eliminate via sum on F, e.g., f(X_2) = \\sum_{x_1} F(x_1,X_2) = F.sum([X1])"""
     if (elim is None): elim = self.v
     return self.__opReduce2(self.v & elim,np.sum, out=out)
 
   def marginal(self, target, out=None):
-    """Compute the marginal of F, e.g., f(X_2) = \sum_{x_1} F(x_1,X_2) = F.marginal([X2])"""
+    """Compute the marginal of F, e.g., f(X_2) = \\sum_{x_1} F(x_1,X_2) = F.marginal([X2])"""
     return self.__opReduce2(self.v - target,np.sum, out=out)
 
   def sumPower(self, elim=None, power=1.0, out=None):
     """Eliminate via powered sum, e.g., f(X_2) =  \\root^{1/p}{ sum_{x_1} F(x_1,X_2)^p } = F.sumPower([X1],p)"""
     if (elim is None): elim = self.v
     tmp = (self ** power).sum(elim)
     tmp **= (1.0/power)
     return tmp
 
   def lse(self, elim=None, out=None):
-    """Eliminate via log-sum-exp on F, e.g., f(X_2) = log \sum_{x_1} exp F(x_1,X_2) = F.lse([X1])"""
+    """Eliminate via log-sum-exp on F, e.g., f(X_2) = log \\sum_{x_1} exp F(x_1,X_2) = F.lse([X1])"""
     if (elim is None): elim = self.v
     return self.__opReduce2(self.v & elim, np.logaddexp.reduce, out=out)
     #return self.__opReduce3(self.v & elim, np.logaddexp.reduce, out=out)
 
   def lsePower(self, elim=None, power=1.0, out=None):
-    """Eliminate via powered log-sum-exp, e.g., f(X_2) = 1/p log \sum_{x_1} exp F(x_1,X_2)*p = F.lsePower([X_1],p)"""
+    """Eliminate via powered log-sum-exp, e.g., f(X_2) = 1/p log \\sum_{x_1} exp F(x_1,X_2)*p = F.lsePower([X_1],p)"""
     if (elim is None): elim = self.v
     if   power == inf: return self.max(elim)
     elif power == -inf: return self.min(elim)
     elif power == 1.0:  return self.lse(elim)
     else:
       tmp = (self*power).lse(elim)
       tmp *= (1.0/power)
       return tmp
 
   def max(self, elim=None, out=None):
-    """Eliminate via max on F, e.g., f(X_2) = \max_{x_1} F(x_1,X_2) = F.max([X1])"""
+    """Eliminate via max on F, e.g., f(X_2) = \\max_{x_1} F(x_1,X_2) = F.max([X1])"""
     if (elim is None): elim = self.v
     return self.__opReduce2(self.v & elim,np.max, out=out)
 
   def maxmarginal(self, target, out=None):
-    """Compute the max-marginal of F, e.g., f(X_2) = \max_{x_1} F(x_1,X_2) = F.maxmarginal([X2])"""
+    """Compute the max-marginal of F, e.g., f(X_2) = \\max_{x_1} F(x_1,X_2) = F.maxmarginal([X2])"""
     return self.__opReduce2(self.v - target,np.max, out=out)
 
   def min(self, elim=None, out=None):
-    """Eliminate via min on F, e.g., f(X_2) = \min_{x_1} F(x_1,X_2) = F.min([X1])"""
+    """Eliminate via min on F, e.g., f(X_2) = \\min_{x_1} F(x_1,X_2) = F.min([X1])"""
     if (elim is None): elim = self.v
     return self.__opReduce2(self.v & elim,np.min, out=out)
 
   def minmarginal(self, target, out=None):
-    """Compute the min-marginal of F, e.g., f(X_2) = \min_{x_1} F(x_1,X_2) = F.minmarginal([X2])"""
+    """Compute the min-marginal of F, e.g., f(X_2) = \\min_{x_1} F(x_1,X_2) = F.minmarginal([X2])"""
     return self.__opReduce2(self.v - target,np.min, out=out)
 
 
     # use ufunc.reduceat?  reduce etc seem not good?
     # frompyfunc to make ufunc from python function?
     # use "externalloop" flag?
     #return t.max(axis=None,out=None) # use axis to specific dimensions to eliminate; out for IP version
@@ -485,15 +488,16 @@
     return out
 
   def condition(self, evidence):
     """Create a clamped (or "sliced") factor using partial conditioning (dict version)
 
     >>> F.condition({0:a,2:b})   # returns  f(X_1,X_3) = F(X_0=a, X_1, X_2=b, X_3)
     """
-    ax = tuple(evidence[v] if  v in evidence else None for x in self.v)
+    ax = tuple(evidence[vi] if  vi in evidence else None for vi in self.v)
+    cvars = VarSet([vi for vi in self.v if vi in evidence])
     out = FactorSparse(self.v - cvars, {})
     for l,x in self.t.items():
       if (cvars is None) or all(ax[i]==None or ax[i]==l[i] for i in range(len(l))):
         out.t[ tuple(li for li,ai in zip(l,ax) if ai is None) ] = x
     return out
 
   slice2 = condition2   # alternate, libDAI-like names
```

### Comparing `pyGMs-0.1.1/pyGMs/filetypes.py` & `pyGMs-0.2.0/pyGMs/filetypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,47 +4,53 @@
 Read / write methods for graphical model file types (UAI, WCSP, etc.)
 
 readUai  /  writeUai            : read/write UAI competition file format
 readEvidence10, readEvidence14  : read/write UAI, Ergo evidence formats (14: single evidence)
 readErgo                        : read Ergo Bayes Net format
 readWCSP /  writeWCSP           : read/write WCSP weighted CSP format
 
-Version 0.1.1 (2022-04-06)
+Version 0.2.0 (2024-04-01)
 (c) 2015 Alexander Ihler under the FreeBSD license; see license.txt for details.
 """
 
 import numpy as np;
 from sortedcontainers import SortedSet as sset;
 from pyGMs.factor import *
 from builtins import range
 
 
 
-def readFileByTokens(path, specials=[]):
-  """Helper function for parsing pyGMs file formats"""
+def readFileByTokens(path, specials=[], escape=True):
+  """Helper function for parsing pyGMs file formats
+    specials : list of tokens to split on (in addition to whitespace, '\s')
+    escape   : escape any specials; if False, interpret specials directly as regular expressions
+  """
   import re
-  spliton = '([\s'+''.join(specials)+'])'
+  if escape: specials = [re.escape(s) for s in specials]
+  spliton = '([\s])'
+  if len(specials): spliton += '|'+'|'.join(['('+s+')' for s in specials])
   with open(path, 'r') as fp:
     for line in fp:
-      #if line[-1]=='\n': line = line[:-1]
       tok = [t.strip() for t in re.split(spliton,line) if t and not t.isspace()]
       for t in tok: yield t
-        #t = t.strip()
-        #if t != '':
-        #  yield t
 
 
 def stripComments(gen, start=['/*'],end=['*/']):
+  """Helper function for removing comment sub-sequences from a stream
+    start/end : list of tokens marking start and end of subsequences to remove 
+  """
   while True:
-    t = next(gen)
+    try: t = next(gen)
+    except StopIteration: return
     if t not in start: 
       yield t
     else:
       while t not in end: 
-        t = next(gen) 
+        try: t = next(gen) 
+        except StopIteration: return
 
 
 ################################################################################################
 # Temporary functions for testing file parse speed, etc.
 ################################################################################################
 def readFileByTokensNEW(path, specials=[]):
   """Helper function for parsing pyGMs file formats"""
@@ -387,28 +393,28 @@
       for tup in np.ndindex(f.dims()):          # then the value of each tuple
         if f[tup] != default_value:
           fp.write(" ".join(map(str,tup)))
           if use_float: fp.write(" {:f}\n".format(f[tup]))
           else:         fp.write(" {:d}\n".format(int(f[tup])))
 
 
-def readDSL(filename):
+def readDSL(filename, verbose=False):
   """Read GeNIe XML DSL format Bayesian network"""
   # TODO: check table entry order
   import xml.etree.ElementTree as ET
   tree = ET.parse(filename)
   root = tree.getroot()
   nodes = root.findall('nodes')[0]   # extract list of nodes in the model
   X = {}
   F,D,U,names,labels = [],[],[],[],[]
   for node in list(nodes):     # get all the variable def's
     if node.tag == 'cpt' or node.tag == 'decision':  # cpts & decisions define a variable:
       name = node.attrib['id']
       states = node.findall('state')
-      print("{} ({}): {} states".format(name,len(X),len(states)))
+      if verbose: print("{} ({}): {} states".format(name,len(X),len(states)))
       X[name] = Var(len(X), len(states)) 
       names.append(name)
       labels.append([s.attrib['id'] for s in states])
     # get parents:
     par  = node.findall('parents')
     clique  = [] if len(par)==0 else [X[pname] for pname in par[0].text.split()]
     if node.tag == 'cpt' or node.tag == 'decision': clique = clique + [X[name]]
@@ -641,26 +647,30 @@
     newarr = np.ones( (tmp.vars.nrStates(),nU) )
     newarr[:,u] = tmp.table.ravel()
     U[u] = Factor( [v for v in tmp.vars]+[z], newarr.reshape( tmp.dims()+(nU,) ) )
   return C+DD+U+[fZ], Q
 
 
 
-def readOrder(filename):
+def readOrder(filename, *args,**kwargs):
     """Read an elimination order from a file
 
     Elimination orders are stored as unknown length vectors, format "[nvar] [v0] [v1] ... [vn]"
 
     Note: the same file format may also be useful for MPE configurations, etc.
+    Additional arguments passed to numpy.loadtxt (used for file read)
     """
-    with open(filename,'r') as fp:
-        lines = fp.readlines();
-    text = lines[-1].strip('\n').split(' ');
-    nvar = int(text[0]);
-    vals = [int(text[i]) for i in range(1,nvar+1)];
+    tmp = np.loadtxt(filename, dtype=int, *args, **kwargs)
+    nvar = tmp[0]
+    vals = list(tmp.squeeze()[1:nvar+1])
+    #with open(filename,'r') as fp:
+    #    lines = fp.readlines();
+    #text = lines[-1].strip('\n').split(' ');
+    #nvar = int(text[0]);
+    #vals = [int(text[i]) for i in range(1,nvar+1)];
     if len(vals) != nvar: raise ValueError("Problem with file?");
     return vals
 
 
 
 def writeOrder(filename,order):
     """ Write an elimination order (or other vector) to a file """
```

### Comparing `pyGMs-0.1.1/pyGMs/graphmodel.py` & `pyGMs-0.2.0/pyGMs/graphmodel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 graphmodel.py
 
 Defines a graphical model container class for reasoning about graphical models
 
-Version 0.1.1 (2022-04-06)
+Version 0.2.0 (2024-04-01)
 (c) 2015-2021 Alexander Ihler under the FreeBSD license; see license.txt for details.
 """
 
 import operator as operator
 import numpy as np
 from sortedcontainers import SortedSet;
 from sortedcontainers import SortedListWithKey;
@@ -32,28 +32,29 @@
   """A basic graphical model class; represents a collection of factors.
 
   Example:
 
   >>> flist = readUai('myfile.uai')  # read a list of factors from a UAI format file
   >>> model = GraphModel(flist)      # makes a copy of the factors for manipulation
 
-  The model may be stored in an exponential, product of factors form:  f(X) = \prod_r f_r(X_r),
-  or in a log-probability, sum of factors form:  \theta(X) = \sum_r \theta_r(X_r).
+  The model may be stored in an exponential, product of factors form:  f(X) = \\prod_r f_r(X_r),
+  or in a log-probability, sum of factors form:  \theta(X) = \\sum_r \theta_r(X_r).
   
   Various accessor functions enable finding factors that depend on one or more variables, variables that
   share one or more factors (their Markov blanket), manipulations to the graph (such as eliminating one
   or more variables), and visualization (through networkx).
   """
 
   X            = []            # variables model defined over
   factors      = factorSet()   # collection of factors that make up the model, sorted by scope size, lex
   factorsByVar = []            # factor lookup by variable:  var -> factor list 
  
   #TODO: useful stuff for algorithm objects interacting with the graph
   lock         = False         # are factors "locked", or are reparameterization changes OK?
+  ## TODO: change to structure lock & parameter lock, separate?
   sig          = 0;            # "signature" of factor cliques; changes if model structure (cliques) changes
  
   isLog = False                # flag: additive (log probability) model vs multiplicative (probability) model 
 
 
   def __repr__(self):
     # TODO: add any details?
@@ -71,14 +72,61 @@
     self.factors = factorSet()
     self.factorsByVar = []
     self.lock = False
     self.sig = 0
     self.isLog = isLog
     if not (factorList is None): self.addFactors(factorList, copy=copy)
   
+  ###################################################
+  ## Basic accessors: what variables are in the model?
+
+  @property
+  def vars(self):
+    """List of variables in the graphical model; equals model.X"""
+    return self.X
+
+  @property
+  def vars_nontrivial(self):
+    """List of "nontrivial" variables (more than one state) in the graphical model"""
+    return [x for x in self.X if x.states>1]
+
+  def var(self,i):   # TODO: change to property to access (read only?) X?
+    """Return a variable object (with # states) for id 'i'; equals model.X[i]"""
+    return self.X[i]
+
+  @property
+  def nvar(self):
+    """The number of variables ( = largest variable id) in the model"""
+    return len(self.X)
+
+  @property
+  def nfactors(self): 
+    """The number of factors in the model"""
+    return len(self.factors)
+
+  ###################################################
+  ## (Partial) configurations of the model variables can be represented as dicts or tuples:
+
+  def as_tuple(self, config, X=None):
+    """Convert a (partial) configuration represented as a dict into a tuple.
+      Variables in self.X missing from config are represented as NaN.
+    """
+    if X is None: X = self.X
+    return tuple(config[x] if x in config else np.nan for x in X)
+
+  def as_dict(self, config, X=None):
+    """Convert a (partial) configuration represented as a tuple into a dict.
+      Config entries specified by NaN are excluded.
+    """
+    if X is None: X=self.X
+    return {x:config[x] for x in X if not np.isnan(config[x])}
+
+  ###################################################
+  ## Basic model transforms. "Log" model => additive cliques, "Exp" model => multiplicative cliques
+
   def toLog(self):
     """Convert internal factors to log form (if not already).  May use 'isLog' to check."""
     if not self.isLog:
       for f in self.factors: f.logIP()
       self.isLog = True
     return self
 
@@ -90,62 +138,98 @@
     return self
  
   def copy(self):
     """Return a (deep) copy of the graphical model"""
     import copy as pcopy
     return pcopy.deepcopy(self)
 
+  def makePositive(self,eps=1e-8):
+    """Force factors / model to be positive (non-zero)"""
+    if self.isLog(): eps = np.log(eps)
+    for f in self.factors:
+      f.table = np.maximum( f.table, eps )
+
+  def value(self,x,subset=None):
+    """Evaluate F(x) = \\prod_r f_r(x_r) for some (full) configuration x.
+         If optional subset != None, uses *only* the factors in the Markov blanket of subset.
+    """
+    if not _is2D(x): x=[x]
+    factors = self.factors if subset==None else self.factorsWithAny(subset)
+    if self.isLog: return np.exp( np.sum( [[ f.valueMap(xx) for f in factors ] for xx in x] ,1) )
+    else:          return np.product( [[ f.valueMap(xx) for f in factors ] for xx in x] ,1)
+
+  def logValue(self,x,subset=None): 
+    """Evaluate log F(x) = \\sum_r log f_r(x_r) for some (full) configuration x.
+         If optional subset != None, uses *only* the factors in the Markov blanket of subset.
+    """
+    if not _is2D(x): x=[x]
+    factors = self.factors if subset==None else self.factorsWithAny(subset)
+    if self.isLog: return np.sum( [[ f.valueMap(xx) for f in factors ] for xx in x] ,1)
+    else:          return np.sum( [[ np.log(f.valueMap(xx)) for f in factors] for xx in x] ,1)
+
+  ###################################################
+  ## Modifying graph structure & cliques
+
   def addFactors(self,flist,copy=True):
     """Add a list of factors to the model; factors are copied locally unless copy = False"""
     import copy as pcopy
     if (copy): flist = pcopy.deepcopy(flist)  # create new factor copies that this model "owns"
     self.factors.update(flist);   # add factor to set of all factors, and to by-variable indexing
     for f in flist:
       # TODO: if constant do something else?  (Currently just leave it in factors list)
       for v in reversed(f.vars):
         if (v.label >= len(self.X)): 
           self.X.extend( [Var(i,1) for i in range(len(self.X),v.label+1) ] )
           self.factorsByVar.extend( [ factorSet() for i in range(len(self.factorsByVar),v.label+1) ] )
         if self.X[v].states <= 1: self.X[v] = v   # copy variable info if undefined, then check:
         if self.X[v].states != v.states: raise ValueError('Incorrect # of states',v,self.X[v])
         self.factorsByVar[v].add(f)
-    self.sig = np.random.rand()     # TODO: check if structure is / can be preserved?
+    self.sig = self.__clique_signature()  # track graph clique signature
 
   def removeFactors(self,flist):
     """Remove a list of factors from the model
     
     >>> model.removeFactors(model.factorsWith([0]))    # remove all factors involving X0
     """
     self.factors.difference_update(flist)
     for f in flist:
       for v in f.vars:
         self.factorsByVar[v].discard(f)
-    self.sig = np.random.rand()     # TODO: check if structure is / can be preserved?
+    self.sig = self.__clique_signature()  # track graph clique signature
 
   def makeCanonical(self):
     """Add/merge factors to make a canonical factor graph: singleton factors plus maximal cliques"""
     for f in self.factors:
       fs = self.factorsWithAll(f.vars)
       if (f.nvar > 1) & (fs[-1] != f):
         if self.isLog: fs[-1] += f
         else:          fs[-1] *= f
         self.removeFactors([f])
+    self.sig = self.__clique_signature()  # track graph clique signature
         
   def makeMinimal(self):
     """Merge factors to make a minimal factor graph: retain only factors over maximal cliques"""
     to_remove = []
     for f in self.factors:
       fs = self.factorsWithAll(f.vars)
       largest = fs[-1]
       if (fs[-1] != f):
         if self.isLog: largest += f
         else:          largest *= f
         to_remove.append(f)
     self.removeFactors(to_remove)
+    self.sig = self.__clique_signature()  # track graph clique signature
+
+  def __clique_signature(self):
+      """Generate hash value based on the graph cliques. Used to track changes in graph structure."""
+      cliquestr = ",".join( (str(f.vars) for f in self.factors) )
+      return hash(cliquestr)
 
+  ###################################################
+  ## Querying graph structure & cliques; special classes of models
 
   def factorsWith(self,v,copy=True):
     """Get the list of all factors that include variable v"""
     return self.factorsByVar[v].copy() if copy else self.factorsByVar[v]
 
   def factorsWithAny(self,vs):
     """Get the list of all factors that include any variables in the list vs"""
@@ -163,37 +247,19 @@
   def markovBlanket(self,v):
     """Get the Markov blanket of variable v (all variables involved in a factor with v)"""
     vs = VarSet()
     for f in self.factorsByVar[v]: vs |= f.vars
     vs -= [v]
     return vs
  
-  def value(self,x,subset=None):
-    """Evaluate F(x) = \prod_r f_r(x_r) for some (full) configuration x.
-         If optional subset != None, uses *only* the factors in the Markov blanket of subset.
-    """
-    if not _is2D(x): x=[x]
-    factors = self.factors if subset==None else self.factorsWithAny(subset)
-    if self.isLog: return np.exp( np.sum( [[ f.valueMap(xx) for f in factors ] for xx in x] ,1) )
-    else:          return np.product( [[ f.valueMap(xx) for f in factors ] for xx in x] ,1)
-
-  def logValue(self,x,subset=None): 
-    """Evaluate log F(x) = \sum_r log f_r(x_r) for some (full) configuration x.
-         If optional subset != None, uses *only* the factors in the Markov blanket of subset.
-    """
-    if not _is2D(x): x=[x]
-    factors = self.factors if subset==None else self.factorsWithAny(subset)
-    if self.isLog: return np.sum( [[ f.valueMap(xx) for f in factors ] for xx in x] ,1)
-    else:          return np.sum( [[ np.log(f.valueMap(xx)) for f in factors] for xx in x] ,1)
-
-  def isBinary(self):   # Check whether the model is binary (all variables binary)
+  def isBinary(self):   
     """Check whether the graphical model is binary (all variables <= 2 states)"""
     return all( [x.states <= 2 for x in self.X] )
 
-  def isPairwise(self): # Check whether the model is pairwise (all factors pairwise)
+  def isPairwise(self): 
     """Check whether the graphical model is pairwise (has maximum scope size 2)"""
     return all( [len(f.vars)<= 2 for f in self.factors] )
 
   def isCSP(self): 
     """Check whether the graphical model is a valid CSP (all zeros or ones)"""
     if self.isLog: isTableCSP = lambda t : all( (t==-np.inf) | (t==0.) ) 
     else:          isTableCSP = lambda t : all( (t==0.) | (t==1.) )   
@@ -214,36 +280,18 @@
       try:
         tmp = tmp.absIP().max()
       except:
         tmp = abs(tmp)
       if tmp > tol: return False                     # fail if not a CPT for X
     if np.prod(found)==0: return False               # fail if missing some variable's CPT
     return True
-    
-
-  @property
-  def vars(self):
-    """List of variables in the graphical model; equals model.X"""
-    return self.X
-
-  def var(self,i):   # TODO: change to property to access (read only?) X?
-    """Return a variable object (with # states) for id 'i'; equals model.X[i]"""
-    return self.X[i]
-
-  @property
-  def nvar(self):
-    """The number of variables ( = largest variable id) in the model"""
-    return len(self.X)
-
-  @property
-  def nfactors(self): 
-    """The number of factors in the model"""
-    return len(self.factors)
-
+  
 
+  ###################################################
+  ## Graph transformations: conditioning on evidence, marginalizing variables
 
   def condition(self, evidence):
     """Condition (clamp) the graphical model on a partial configuration (dict) {Xi:xi, Xj:xj, ...}"""
     # TODO: optionally, ensure re-added factor is maximal, or modify an existing one (fWithAll(vs)[-1]?)
     if len(evidence)==0: return
     for v,x in evidence.items():
       constant = 0.0
@@ -297,15 +345,15 @@
           self.addFactors([F],False)  # add factor F by reference
         except:  
           self.addFactors([Factor([],F)],False)          # scalar => add as scalar factor
           # TODO: could check for existing scalar? or leave as is to preserve independent problem correspondence?
       self.X[v] = Var(int(v),1)    # remove "concept" of variable v ( => single state)
 
   def joint(self):
-    """Compute brute-force joint function F(x) = \prod_r f_r(x_r) as a (large) factor"""
+    """Compute brute-force joint function F(x) = \\prod_r f_r(x_r) as a (large) factor"""
     F = self.factors[0].copy()
     for f in self.factors[1:]: 
       if self.isLog: F += f
       else:          F *= f   
     return F
 
   def connectedComponents(self):
@@ -329,192 +377,14 @@
         
     # Note: to split graph into connected components, use e.g.
     # >>> [GraphModel(model.factorsWithAny(vs)) for vs in model.connectedComponents()]
     # (although each model may have the full set of variables, most with 0 or 1 state...)  
     # NOTE: don't forget about any scalar factors: [f for f in model.factors where f.nvar==0]
     
     
-    
-
-
-# def nxMarkovGraph(self, all_vars=False):
-#   """Get networkx Graph object of the Markov graph of the model
-#
-#   Example:
-#   >>> G = nxMarkovGraph(model)
-#   >>> nx.draw(G)
-#   """
-#   import networkx as nx
-#    G = nx.Graph()
-#    G.add_nodes_from( [v.label for v in self.X if (all_vars or v.states > 1)] ) 
-#    for f in self.factors:
-#      for v1 in f.vars:
-#        for v2 in f.vars:
-#          if (v1 != v2) and (all_vars or (v1.states > 1 and v2.states > 1)): 
-#            G.add_edge(v1.label,v2.label)
-#    return G 
-#    """ Plotting examples:
-#    fig,ax=plt.subplots(1,2)
-#    pos = nx.spring_layout(G) # so we can use same positions multiple times...
-#    # use nodelist=[nodes-to-draw] to only show nodes in model
-#    nx.draw(G,with_labels=True,labels={0:'0',1:'1',2:'2',3:'3',4:'4',5:'5',6:'6'},
-#              node_color=[.3,.3,.3,.7,.7,.7,.7],vmin=0.0,vmax=1.0,pos=pos,ax=ax[0])
-#    nx.draw(G,with_labels=True,labels={0:'0',1:'1',2:'2',3:'3',4:'4',5:'5',6:'6'},
-#              node_color=[.3,.3,.3,.7,.7,.7,.7],vmin=0.0,vmax=1.0,pos=pos,ax=ax[1])
-#    """
-#
-#  def drawMarkovGraph(self,**kwargs):
-#    """Draw a Markov random field using networkx function calls
-#
-#    Args:
-#      ``**kwargs``: remaining keyword arguments passed to networkx.draw()
-#
-#    Example:
-#    >>> model.drawMarkovGraph( labels={0:'0', ... } )    # keyword args passed to networkx.draw()
-#    """
-#    # TODO: fix defaults; specify shape, size etc. consistent with FG version
-#    import networkx as nx
-#    G = self.nxMarkovGraph()
-#    kwargs['var_labels'] = kwargs.get('var_labels',{n:n for n in G.nodes()})
-#    kwargs['labels'] = kwargs.get('labels', kwargs.get('var_labels',{}) )
-#    nx.draw(G,**kwargs)
-#    return G
-#
-#
-#
-#  def drawFactorGraph(self,var_color='w',factor_color=[(.2,.2,.8)],**kwargs):
-#    """Draw a factorgraph using networkx function calls
-#
-#    Args:
-#      var_color (str, tuple): networkx color descriptor for drawing variable nodes
-#      factor_color (str, tuple list): networkx color for drawing factor nodes
-#      var_labels (dict): variable id to label string for variable nodes
-#      factor_labels (dict): factor id to label string for factor nodes
-#      ``**kwargs``: remaining keyword arguments passed to networkx.draw()
-#
-#    Example:
-#    >>> model.drawFactorGraph( var_labels={0:'0', ... } )    # keyword args passed to networkx.draw()
-#    """
-#    # TODO: specify var/factor shape,size, position, etc.; return G? silent mode?
-#    import networkx as nx
-#    G = nx.Graph()
-#    vNodes = [v.label for v in self.X if v.states > 1]   # list only non-trivial variables
-#    fNodes = [-i-1 for i in range(len(self.factors))]    # use negative IDs for factors
-#    G.add_nodes_from( vNodes )
-#    G.add_nodes_from( fNodes )
-#    for i,f in enumerate(self.factors):
-#      for v1 in f.vars:
-#        G.add_edge(v1.label,-i-1)
-#
-#    if not 'pos' in kwargs: kwargs['pos'] = nx.spring_layout(G) # so we can use same positions multiple times...
-#    kwargs['var_labels']  = kwargs.get('var_labels',{n:n for n in vNodes})
-#    kwargs['labels'] = kwargs.get('var_labels',{})
-#    nx.draw_networkx(G, nodelist=vNodes,node_color=var_color,**kwargs)
-#    kwargs['labels'] = kwargs.get('factor_labels',{})    # TODO: need to transform?
-#    nx.draw_networkx_nodes(G, nodelist=fNodes,node_color=factor_color,node_shape='s',**kwargs)
-#    nx.draw_networkx_edges(G,**kwargs)
-#    return G
-#
-#
-#
-#  def drawBayesNet(self,**kwargs):
-#    """Draw a Bayesian Network (directed acyclic graph) using networkx function calls
-#
-#    Args:
-#      ``**kwargs``: remaining keyword arguments passed to networkx.draw()
-#
-#    Example:
-#    >>> model.drawBayesNet( labels={0:'0', ... } )    # keyword args passed to networkx.draw()
-#    """
-#    import networkx as nx
-#    topo_order = bnOrder(self)                              # TODO: allow user-provided order?
-#    if topo_order is None: raise ValueError('Topo order not found; graph is not a Bayes Net?')
-#    pri = np.zeros((len(topo_order),))-1
-#    pri[topo_order] = np.arange(len(topo_order))
-#    G = nx.DiGraph()
-#    G.add_nodes_from( [v.label for v in self.X if v.states > 1] )  # only non-trivial vars
-#    for f in self.factors:
-#      v2label = topo_order[ int(max(pri[v.label] for v in f.vars)) ]
-#      for v1 in f.vars:
-#        if (v1.label != v2label): G.add_edge(v1.label,v2label)
-#
-#    kwargs['var_labels'] = kwargs.get('var_labels',{n:n for n in [v.label for v in self.X]})
-#    kwargs['labels'] = kwargs.get('labels', kwargs.get('var_labels',{}) )
-#    kwargs['arrowstyle'] = kwargs.get('arrowstyle','->')
-#    kwargs['arrowsize'] = kwargs.get('arrowsize',10)
-#    nx.draw(G,**kwargs)
-#    return G
-#
-#
-#  def drawLimid(self, C,D,U, **kwargs):
-#    """Draw a limited-memory influence diagram (limid) using networkx 
-#
-#    Args:
-#      ``**kwargs``: remaining keyword arguments passed to networkx.draw()
-#
-#    Example:
-#    >>> model.drawLimid(C,D,U, var_labels={0:'0', ... } )    # keyword args passed to networkx.draw()
-#    """
-#    import networkx as nx
-#    decisions = [d[-1] for d in D]                       # list the decision variables
-#    model = GraphModel( C + [Factor(d,1.) for d in D] )  # get all chance & decision vars, arcs
-#    chance = [c for c in model.X if c not in decisions]
-#    util = [-i-1 for i,u in enumerate(U)]
-#    cpd_edges, util_edges, info_edges = [],[],[]
-#    topo_order = bnOrder(model)                          
-#    if topo_order is None: raise ValueError('Topo order not found; graph is not a Bayes Net?')
-#    pri = np.zeros((len(topo_order),))-1
-#    pri[topo_order] = np.arange(len(topo_order))
-#    G = nx.DiGraph()
-#    G.add_nodes_from( [v.label for v in self.X if v.states > 1] )  # only non-trivial vars
-#    G.add_nodes_from( util )                                       # add utility nodes
-#    for f in model.factors:
-#      v2label = topo_order[ int(max(pri[v.label] for v in f.vars)) ]
-#      for v1 in f.vars:
-#        if (v1.label != v2label): 
-#          G.add_edge(v1.label,v2label)
-#          if v2label in decisions: info_edges.append((v1.label,v2label))
-#          else: cpd_edges.append((v1.label,v2label))
-#    for i,u in enumerate(U):
-#      for v1 in u.vars:
-#        G.add_edge(v1.label,-i-1)
-#        util_edges.append( (v1.label,-i-1) )
-#    if not 'pos' in kwargs: kwargs['pos'] = nx.spring_layout(G) # so we can use same positions multiple times...
-#    nx.draw_networkx_nodes(G, nodelist=decisions, node_color=[(.7,.7,.9)], node_shape='s', **kwargs)
-#    nx.draw_networkx_nodes(G, nodelist=chance, node_color=[(1.,1.,1.)], node_shape='o', **kwargs)
-#    nx.draw_networkx_nodes(G, nodelist=util, node_color=[(.7,.9,.7)], node_shape='d', **kwargs)
-#    nx.draw_networkx_edges(G, edgelist=cpd_edges+util_edges, **kwargs)
-#    tmp = nx.draw_networkx_edges(G, edgelist=info_edges, **kwargs)
-#    for line in tmp: line.set_linestyle('dashed')
-#    nx.draw_networkx_labels(G, **kwargs)
-
-
-
-#  def nxFactorGraph(self):
-#    """Get networkx Graph object of the factor graph of the model"""
-#    import networkx as nx
-#    G = nx.Graph()
-#    vNodes = [v.label for v in self.X]
-#    fNodes = [-i-1 for i in range(len(self.factors))]
-#    G.add_nodes_from( vNodes )
-#    G.add_nodes_from( fNodes )
-#    for f in self.factors:
-#      for v1 in f.vars:
-#        G.add_edge(v1.label,-self.factors.index(f)-1)
-#    return G 
-#    """ Plotting examples:
-#    pos = nx.spring_layout(G) # so we can use same positions multiple times...
-#    nx.draw_networkx(G,pos=pos, nodelist=[n for n in G.nodes() if n >= 0],node_color='w')
-#    nx.draw_networkx_nodes(G,pos=pos, nodelist=[n for n in G.nodes() if n < 0],node_color='g',node_shape='s')
-#    nx.draw_networkx_edges(G,pos=pos)
-#    nx.draw_networkx_labels(G,pos=pos,labels={n:n for n in G.nodes() if n>=0})
-#    """
-
-
-
   ############# FUNCTIONS TODO ######################
   
   # Algorithms:
   #   (CSP) AC, Backtrack, Local Search;  (GEN) gibbs, mh?, MAS, MBE, WMB, local search, other search?
   # Train:
   #   CD, ???
  
@@ -541,137 +411,143 @@
 def bnOrder(bn):
     """Return a topological order for the variables (roots to leaves), assuming 'bn' is a Bayes net
 
     Returns:
         list: variable IDs in a topological order from roots to leaves
     """
     temp = GraphModel(bn.factors, copy=False)  # slow? unnecessary?
-    topo_order = [-1]*bn.nvar
-    pri = [-1]*bn.nvar
-    for i in range(bn.nvar):
+    nvar = len(bn.vars_nontrivial)
+    topo_order = [-1]*nvar
+    for i in range(nvar):
+        #print(f"Have: {[f.vars for f in temp.factors]}")
+        # check if all remaining vars have only one state?
         if temp.factors[0].nvar != 1: return None    # if there are no root variables, not a BN
         X = temp.factors[0].vars[0]                  # otherwise, add root to the topological order
+        if X.states < 2: raise ValueError('Factor with trivial variable argument?')
         topo_order[i] = X.label
-        pri[X] = i
+        #print(f"  Root {X.label}")
         withX = temp.factorsWith(topo_order[i])      # remove it from its childrens' CPTs
         temp.removeFactors(withX)                    #  to look for the next variable in the order
         temp.addFactors( [f.condition2([X],[0]) for f in withX if f.nvar > 1] )
+        #print(f"  Now {[f.vars for f in temp.factors]}")
     return topo_order
 
 
 def bnPrune(bn, query):
   """Prune all non-ancestors of 'query' in Bayesian network 'bn'
   """
   # TODO: implement: find all ancestors of query; remove non-ancestors (do bn-check elim for safety?)
   raise NotImplementedError('Not implemented')
 
 
 def bnSample(model, order, evidence={}):
-  """Draw a sample from a Bayes net with given topological order and evidence E={ Xi: k ... }
+  """xs, lnP = bnSample(model, order, evidence)
+  Draw a sample from a Bayes net with given topological order and evidence E={ Xi: k ... }
 
   Args:
     model (GraphModel): A Bayesian network or other graphical model
     order (list): A topological ordering of the variables, e.g., from ``bnOrder(model)``
 
   Returns:
-     float : lnP, the log-probability of the sampled configuration xs 
      tuple : xs, the sampled configuration (including evidence)
+     float : lnP, the log-probability of the sampled configuration xs 
 
   Notes: lnP, the log-probability, does not include any evidence probabilities.  If `model` is not a
      Bayes net, the process and lnP will still correspond to some valid distribution over X given E.
   """
   lnP, cfg = 0.0, evidence.copy()
-  pri = np.zeros((len(order),))-1
+  pri = np.zeros((max(order)+1,))-1
   pri[order] = np.arange(len(order))
   for i in order:
     if i in evidence: continue
     F = model.factorsWith(i)
     fid = np.argmin( [ np.max(pri[f.vars.labels]) for f in F ] )  # find factor with X and earliest neighbors
     Pi = F[fid].condition(cfg)
     if model.isLog: Pi.expIP()    # if storing log-factors, exponentiate...
     Pi /= Pi.sum()
     Pi = Pi.marginal([i])     # likely not necessary, but to be safe for non BNs
     cfg[i] = Pi.sample()[0]
     lnP += np.log( Pi[cfg[i]] )
-  return lnP, tuple(cfg.get(i,0) for i in model.X) 
+  return tuple(cfg.get(i,0) for i in model.X), lnP
+  # TODO: if model.X is not 0...n-1, this does not include missing variables (?)
 
 # One-line likelihood weighting estimator:
-# np.mean( [ np.exp(model.logValue(xs)-lnP) for s in range(1000) for lnP,xs in [gm.bnSample(model,order,evid)] ] )
+# np.mean( [ np.exp(model.logValue(xs)-lnP) for s in range(1000) for xs,lnP in [gm.bnSample(model,order,evid)] ] )
 #
 #
 
 
 
-def _eliminationOrder_OLD(gm, orderMethod=None, nExtra=-1, cutoff=inf, priority=None, target=None):
-  """Find an elimination order for a graphical model
-  Args:
-    gm (GraphModel): A graphical model object
-    method (str): Heuristic method; one of {'minfill','wtminfill','minwidth','wtminwidth','random'}
-    nExtra (int): Randomly select eliminated variable from among the best plus nExtra; this adds
-        randomness to the order selection process.  0 => randomly from best; -1 => no randomness (default)
-    cutoff (float): Quit early if ``score`` exceeds a user-supplied cutoff value (returning ``target, cutoff``)
-    target (list): If the identified order is better than cutoff, write it directly into passed ``target`` list
-    priority (list, optional): Optional list of variable priorities; lowest priority variables are 
-        eliminated first.  Useful for mixed elimination models, such as marginal MAP inference tasks.
-  Returns:
-    list: The identified elimination order
-    float: The "score" of this ordering
-  Using ``target`` and ``cutoff`` one can easily search for better orderings by repeated calls:
-  >>> ord, score = eliminationOrder(model, 'minfill', nExtra=2, cutoff=score, target=ord) 
-  """
-  import bisect
-  orderMethod = 'minfill' if orderMethod is None else orderMethod.lower()
-  priority = [1 for x in gm.X] if priority is None else priority
-
-  if   orderMethod == 'minfill':    score = lambda adj,Xj: sum([0.5*len(adj[Xj]-adj[Xk]) for Xk in adj[Xj]])
-  elif orderMethod == 'wtminfill':  score = lambda adj,Xj: sum([(adj[Xj]-adj[Xk]).nrStatesDouble() for Xk in adj[Xj]])
-  elif orderMethod == 'minwidth':   score = lambda adj,Xj: len(adj[Xj])
-  elif orderMethod == 'wtminwidth': score = lambda adj,Xj: adj[Xj].nrStatesDouble()
-  elif orderMethod == 'random':     score = lambda adj,Xj: np.random.rand()
-  else: raise ValueError('Unknown ordering method: {}'.format(orderMethod))
-
-  adj = [ VarSet([Xi]) for Xi in gm.X ]
-  for Xi in gm.X: 
-    for f in gm.factorsWith(Xi, copy=False):
-      adj[Xi] |= f.vars
-
-  # initialize priority queue of scores using e.g. heapq or sort
-  scores  = [ (priority[Xi],score(adj,Xi),Xi) for Xi in gm.X ]
-  reverse = scores[:]
-  scores.sort()
-  totalSize = 0.0
-  _order = [0 for Xi in gm.X]
-
-  for idx in range(gm.nvar):
-    pick = 0
-    Pi,Si,Xi = scores[pick]
-    if nExtra >= 0:
-      mx = bisect.bisect_right(scores, (Pi,Si,gm.X[-1]))  # get one past last equal-priority & score vars
-      pick = min(mx+nExtra, len(scores))                  # then pick a random "near-best" variable
-      pick = np.random.randint(pick)
-      Pi,Si,Xi = scores[pick]
-    del scores[pick]
-    _order[idx] = Xi.label        # write into order[idx] = Xi
-    totalSize += adj[Xi].nrStatesDouble()
-    if totalSize > cutoff: return target,cutoff  # if worse than cutoff, quit with no changes to "target"
-    fix = VarSet()
-    for Xj in adj[Xi]:
-      adj[Xj] |= adj[Xi]
-      adj[Xj] -= [Xi]
-      fix |= adj[Xj]   # shouldn't need to fix as much for min-width?
-    for Xj in fix:
-      Pj,Sj,Xj = reverse[Xj]
-      jPos = bisect.bisect_left(scores, (Pj,Sj,Xj))
-      del scores[jPos]                        # erase (Pj,Sj,Xj) from heap 
-      reverse[Xj] = (Pj,score(adj,Xj),Xj)     
-      bisect.insort_left(scores, reverse[Xj]) # add (Pj,score(adj,Xj),Xj) to heap & update reverse lookup
-  if not (target is None): 
-    target.extend([None for i in range(len(target),len(_order))])  # make sure order is the right size
-    for idx in range(gm.nvar): target[idx]=_order[idx]   # copy result if completed without quitting
-  return _order,totalSize
+#def _eliminationOrder_OLD(gm, orderMethod=None, nExtra=-1, cutoff=inf, priority=None, target=None):
+#  """Find an elimination order for a graphical model
+#  Args:
+#    gm (GraphModel): A graphical model object
+#    method (str): Heuristic method; one of {'minfill','wtminfill','minwidth','wtminwidth','random'}
+#    nExtra (int): Randomly select eliminated variable from among the best plus nExtra; this adds
+#        randomness to the order selection process.  0 => randomly from best; -1 => no randomness (default)
+#    cutoff (float): Quit early if ``score`` exceeds a user-supplied cutoff value (returning ``target, cutoff``)
+#    target (list): If the identified order is better than cutoff, write it directly into passed ``target`` list
+#    priority (list, optional): Optional list of variable priorities; lowest priority variables are 
+#        eliminated first.  Useful for mixed elimination models, such as marginal MAP inference tasks.
+#  Returns:
+#    list: The identified elimination order
+#    float: The "score" of this ordering
+#  Using ``target`` and ``cutoff`` one can easily search for better orderings by repeated calls:
+#  >>> ord, score = eliminationOrder(model, 'minfill', nExtra=2, cutoff=score, target=ord) 
+#  """
+#  import bisect
+#  orderMethod = 'minfill' if orderMethod is None else orderMethod.lower()
+#  priority = [1 for x in gm.X] if priority is None else priority
+#
+#  if   orderMethod == 'minfill':    score = lambda adj,Xj: sum([0.5*len(adj[Xj]-adj[Xk]) for Xk in adj[Xj]])
+#  elif orderMethod == 'wtminfill':  score = lambda adj,Xj: sum([(adj[Xj]-adj[Xk]).nrStatesDouble() for Xk in adj[Xj]])
+#  elif orderMethod == 'minwidth':   score = lambda adj,Xj: len(adj[Xj])
+#  elif orderMethod == 'wtminwidth': score = lambda adj,Xj: adj[Xj].nrStatesDouble()
+#  elif orderMethod == 'random':     score = lambda adj,Xj: np.random.rand()
+#  else: raise ValueError('Unknown ordering method: {}'.format(orderMethod))
+#
+#  adj = [ VarSet([Xi]) for Xi in gm.X ]
+#  for Xi in gm.X: 
+#    for f in gm.factorsWith(Xi, copy=False):
+#      adj[Xi] |= f.vars
+#
+#  # initialize priority queue of scores using e.g. heapq or sort
+#  scores  = [ (priority[Xi],score(adj,Xi),Xi) for Xi in gm.X ]
+#  reverse = scores[:]
+#  scores.sort()
+#  totalSize = 0.0
+#  _order = [0 for Xi in gm.X]
+#
+#  for idx in range(gm.nvar):
+#    pick = 0
+#    Pi,Si,Xi = scores[pick]
+#    if nExtra >= 0:
+#      mx = bisect.bisect_right(scores, (Pi,Si,gm.X[-1]))  # get one past last equal-priority & score vars
+#      pick = min(mx+nExtra, len(scores))                  # then pick a random "near-best" variable
+#      pick = np.random.randint(pick)
+#      Pi,Si,Xi = scores[pick]
+#    del scores[pick]
+#    _order[idx] = Xi.label        # write into order[idx] = Xi
+#    totalSize += adj[Xi].nrStatesDouble()
+#    if totalSize > cutoff: return target,cutoff  # if worse than cutoff, quit with no changes to "target"
+#    fix = VarSet()
+#    for Xj in adj[Xi]:
+#      adj[Xj] |= adj[Xi]
+#      adj[Xj] -= [Xi]
+#      fix |= adj[Xj]   # shouldn't need to fix as much for min-width?
+#    for Xj in fix:
+#      Pj,Sj,Xj = reverse[Xj]
+#      jPos = bisect.bisect_left(scores, (Pj,Sj,Xj))
+#      del scores[jPos]                        # erase (Pj,Sj,Xj) from heap 
+#      reverse[Xj] = (Pj,score(adj,Xj),Xj)     
+#      bisect.insort_left(scores, reverse[Xj]) # add (Pj,score(adj,Xj),Xj) to heap & update reverse lookup
+#  if not (target is None): 
+#    target.extend([None for i in range(len(target),len(_order))])  # make sure order is the right size
+#    for idx in range(gm.nvar): target[idx]=_order[idx]   # copy result if completed without quitting
+#  return _order,totalSize
 
 
 def eliminationOrder(gm, orderMethod=None, nExtra=-1, cutoff=inf, priority=None, target=None):
   """Find an elimination order for a graphical model
 
   Args:
     gm (GraphModel): A graphical model object
@@ -686,20 +562,23 @@
   Returns:
     list: The identified elimination order
     float: The "score" of this ordering
 
   Using ``target`` and ``cutoff`` one can easily search for better orderings by repeated calls:
   >>> ord, score = eliminationOrder(model, 'minfill', nExtra=2, cutoff=score, target=ord) 
   """
+  import bisect
   orderMethod = 'minfill' if orderMethod is None else orderMethod.lower()
   priority = [1 for x in gm.X] if priority is None else priority
 
   if   orderMethod == 'minfill':    score = lambda adj,Xj: 0.5*sum([len(adj[Xj]-adj[Xk]) for Xk in adj[Xj]])
+  elif orderMethod == 'wtminfill1': score = lambda adj,Xj: sum([Xk.states*Xl.states for Xk in adj[Xj] for Xl in adj[Xj]-adj[Xk]])
   elif orderMethod == 'wtminfill':  score = lambda adj,Xj: sum([(adj[Xj]-adj[Xk]).nrStatesDouble() for Xk in adj[Xj]])
   elif orderMethod == 'minwidth':   score = lambda adj,Xj: len(adj[Xj])
+  elif orderMethod == 'wtminwidth1': score = lambda adj,Xj: sum([Xk.states*Xl.states for Xk in adj[Xj] for Xl in adj[Xj]-[Xk]])
   elif orderMethod == 'wtminwidth': score = lambda adj,Xj: adj[Xj].nrStatesDouble()
   elif orderMethod == 'random':     score = lambda adj,Xj: np.random.rand()
   else: raise ValueError('Unknown ordering method: {}'.format(orderMethod))
 
   adj = [ gm.markovBlanket(Xi) for Xi in gm.X ]  # build MRF
 
   # initialize priority queue of scores using e.g. heapq or sort
@@ -717,24 +596,24 @@
       pick = min(mx+nExtra, len(scores))                  # then pick a random "near-best" variable
       pick = np.random.randint(pick)
       Pi,Si,Xi = scores[pick]
     del scores[pick]
     _order[idx] = Xi.label        # write into order[idx] = Xi
     totalSize += adj[Xi].nrStatesDouble()
     if totalSize > cutoff: return target,cutoff  # if worse than cutoff, quit with no changes to "target"
-    fix = VarSet()
-    for Xj in adj[Xi]:
+    fix = adj[Xi].copy()          # fix up (at least) scores of variables adjacent to Xi
+    for Xj in adj[Xi]:            # update Markov graph to reflect removal of Xi: join Xi's neighbors
       adj[Xj] |= adj[Xi]
-      adj[Xj] -= [Xi]  # TODO adj[Xj].remove(Xi) slightly faster but still unsupported by cython version
-      fix |= adj[Xj]   # shouldn't need to fix as much for min-width?
-    for Xj in fix:
+      adj[Xj] -= [Xi,Xj]  # TODO adj[Xj].remove(Xi) slightly faster but still unsupported by cython version
+      fix |= adj[Xj]              # also fix scores of 2nd neighbors for min-fill (shouldn't need to fix as much for min-width?)
+    for Xj in fix:                # Now, update the scores of "fix" set in the priority queue:
       Pj,Sj,Xj = reverse[Xj]
       scores.remove(reverse[Xj])
-      reverse[Xj] = (Pj,score(adj,Xj),Xj)
-      scores.add(reverse[Xj]) # add (Pj,score(adj,Xj),Xj) to heap & update reverse lookup
+      reverse[Xj] = (Pj,score(adj,Xj),Xj)  # re-score Xj
+      scores.add(reverse[Xj])     # add (Pj,score(adj,Xj),Xj) to heap & update reverse lookup
   if not (target is None): 
     target.extend([None for i in range(len(target),len(_order))])  # make sure order is the right size
     for idx in range(gm.nvar): target[idx]=_order[idx]   # copy result if completed without quitting
   return _order,totalSize
     
 
 class PseudoTree(object):
@@ -846,42 +725,39 @@
 #    constructs ordered seq. of conditionals (by ref if possible) by selecting the largest
 #    factor containing only preceding vars & conditioning if reqiured.
 #    => BN + order = factor sequence for sampling
 #    => BP beliefs + order = BP BN proposal
 # ?? do without actually conditioning? condition on the fly: 
 #   compute the norm, sample, etc. manually in f'n
 
-#def forwardSample(model, varOrder, factorOrder=None):
-def sampleSequential(model, varOrder, factorOrder=None):
-  """Draw a configuration X sequentially from the model factors.
-  For a Bayes net using a valid topological order, this is equivalent to forward sampling.
- 
-  Returns logQ,xs  (tuple): the sampled config xs and its log-probability under the sampling distribution
-  """
-  if factorOrder is None: factorOrder = []
-  if len(factorOrder)==0:
-    raise NotImplementedError
-    # figure out an ordering of the factors in "model" to use & store them in factorOrder:
-    # for each xi in varOrder:
-    #   from model, get factors with xi
-    #   from small->large (?) check if args all in "done"; if so, add to factorOrder
-    #   add xi to done
-  #x = [-1 for Xi in varOrder]         # storage for sample value
-  s = {}                              # storage for sample value
-  #lnP, lnW = 0.0, 0.0                 # log p(x) of drawn sample & log w(x) = f(x)/p(x)
-  lnP = 0.0                           # log p(x) of drawn sample
-  # TODO: enumerate over varOrder instead; use factorOrder[i], then weight by factorOrd[i:] after
-  for i,f in enumerate(factorOrder):  # sample Xi from F[i | prev]:
-    xi  = varOrder[i]
-    Pxi = f.condition( s )
-    # TODO: check Pxi over one var, xi
-    Zi  = Pxi.sum()
-    s[ xi ], = Pxi.sample(Z=Zi)  # draw sample for i'th variable
-    lnP += np.log( Pxi[s[xi]] / Zi )
-  s_list = [ s[i] for i in range(len(s)) ]
-  return lnP, s_list   
+#def sampleSequential(model, varOrder, factorOrder=None):
+#  """Draw a configuration X sequentially from the model factors.
+#  For a Bayes net using a valid topological order, this is equivalent to forward sampling.
+# 
+#  Returns xs,lnQ : the sampled config xs (tuple) and its log-probability under the sampling distribution (float)
+#  """
+#  if factorOrder is None: factorOrder = []
+#  if len(factorOrder)==0:
+#    raise NotImplementedError
+#    # figure out an ordering of the factors in "model" to use & store them in factorOrder:
+#    # for each xi in varOrder:
+#    #   from model, get factors with xi
+#    #   from small->large (?) check if args all in "done"; if so, add to factorOrder
+#    #   add xi to done
+#  s = {}                              # storage for sample value
+#  lnP = 0.0                           # log p(x) of drawn sample
+#  # TODO: enumerate over varOrder instead; use factorOrder[i], then weight by factorOrd[i:] after
+#  for i,f in enumerate(factorOrder):  # sample Xi from F[i | prev]:
+#    xi  = varOrder[i]
+#    Pxi = f.condition( s )
+#    # TODO: check Pxi over one var, xi
+#    Zi  = Pxi.sum()
+#    s[ xi ], = Pxi.sample(Z=Zi)  # draw sample for i'th variable
+#    lnP += np.log( Pxi[s[xi]] / Zi )
+#  s_list = [ s[i] for i in range(len(s)) ]
+#  return s_list, lnP
```

### Comparing `pyGMs-0.1.1/pyGMs/ising.py` & `pyGMs-0.2.0/pyGMs/ising.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 ising.py
 
 Specialty graphical model class for Ising models (binary pairwise models)
 Note: uses data definition Xi in {0,1} for compatibility with other graphmodel classes
 
-Version 0.1.1 (2022-04-06)
+Version 0.2.0 (2024-04-01)
 (c) 2020 Alexander Ihler under the FreeBSD license; see license.txt for details.
 """
 
 import operator as operator
 import numpy as np
 
 inf = float('inf')
@@ -20,16 +20,18 @@
 from scipy.sparse import coo_matrix as coo
 from scipy.sparse import csr_matrix as csr
 
 from numpy import asarray as arr
 from numpy import atleast_2d as twod
 
 def toPM(x):
+    """Convert data (nparray) from values {0,1} to {-1,+1}"""
     return 2*x-1
 def to01(x):
+    """Convert data (nparray) from values {-1,+1} to {0,1}"""
     return (x>0).astype(int)
 
 class Ising(object):
   """Specialized graphical model class for representing Ising models (pairwise, binary models)
     Internal representation is as a sparse matrix, which is much more efficient than a factor list.
     NOTE: evaluations / data expect Xi = {0,1} to match GraphModel class
   """
@@ -293,15 +295,15 @@
 
   def nxMarkovGraph(self, all_vars=False):
     """Return a networkx object representing the Markov graph of the Ising model"""
     import networkx as nx
     return nx.from_scipy_sparse_matrix(self.L!=0)
     
   def pseudolikelihood(self, data):
-    """Compute the pseudo (log) likelihood, \sum_i \sum_j \log p(x^{(j)}_i | x^{(j)}_{\neg i})
+    """Compute the pseudo (log) likelihood, \\sum_i \\sum_j \\log p(x^{(j)}_i | x^{(j)}_{\neg i})
        data : (m,n) or (n,) array or dict of the values xi; values in {0,1}
     """
     if isinstance(data,dict): data = toPM(np.array([[data[i] for i in range(self.nvar)]]))
     else: data = toPM(twod(data));              # interface glue: convert {0,1} to {-1,+1}
     r = self.L.dot(data.T)
     r += self.h.reshape(-1,1) if len(data.shape)==2 else self.h
     lnp = -np.log(1+np.exp(-2*data.T*r))    # ln p(x_i^(s)|x_{-i}^(s)) for all vars i, samples s
@@ -375,14 +377,68 @@
     dL = L.tocoo()
     for k in range(dL.nnz):
         i,j = dL.row[k],dL.col[k]
         dL.data[k] = 2*np.mean((p[i]+p[j])*(x[i]*x[j]))  # avg over s if needed
     return dL.tocsr(),dh
 
 
+def refit_moments(model, data, alpha=1e-4, weights=None):
+    """Set the parameters of the model to match locally the empirical data probabilities (max likelihood for trees)
+      model : an Ising model to re-fit (will keep edge structure)
+      data: (m,n) nparray of m data points; values {0,1}
+    """
+    def moments(data, weights):
+        """Estimate mutual information between all pairs of *binary* {0,1} variables"""
+        pi = np.average(data.astype(float),axis=1,weights=weights)[np.newaxis,:]
+        pij = np.cov(data,ddof=0,aweights=weights) + (pi.T.dot(pi));
+        return pij,pi[0]
+        
+    n,m = data.shape
+    pij,pi = moments(data.T, weights)       # data should be 0/1, not -1/+1
+    factors = [Factor([Var(i,2)], [1-pi[i],pi[i]]) for i in range(n)]
+    L = coo(model.L)
+    for i,j,th in zip(L.row,L.col,L.data):
+        if j>i: continue
+        tij = [1+pij[i,j]-pi[i]-pi[j], pi[i]-pij[i,j], pi[j]-pij[i,j], pij[i,j]]
+        fij = Factor([Var(int(i),2),Var(int(j),2)],tij)+alpha;
+        fij = fij / fij.sum([i]) / fij.sum([j])
+        factors.append(fij)
+    model.__init__(factors)
+
+
+def refit_ipf(model, data, maxiter=10, stoptol=1e-4, alpha=1e-4, weights=None):
+    """Set the parameters of the model to match the empirical data probabilities (max likelihood) (slow!)
+      model : an Ising model to re-fit (will keep edge structure)
+      data: (m,n) nparray of m data points; values {0,1}
+    """
+    def moments(data, weights):
+        """Estimate mutual information between all pairs of *binary* {0,1} variables"""
+        pi = np.average(data.astype(float),axis=1,weights=weights)[np.newaxis,:]
+        pij = np.cov(data,ddof=0,aweights=weights) + (pi.T.dot(pi));
+        return pij,pi[0]
+       
+    from pyGMs.wmb import JTree
+    import random
+    n,m = data.shape
+    pij,pi = moments(data.T, weights)       # data should be 0/1, not -1/+1
+    order = eliminationOrder(model, 'minwidth')[0];
+    L = coo(model.L); edges = list([(int(i),int(j)) for i,j in zip(L.row,L.col) if i<j])
+    for it in range(maxiter):
+        random.shuffle(edges)
+        done=True
+        for i,j in edges:
+            tij = [1+pij[i,j]-pi[i]-pi[j], pi[i]-pij[i,j], pi[j]-pij[i,j], pij[i,j]]
+            fij = Factor([Var(i,2),Var(j,2)],tij)+alpha;
+            jt = JTree(model, elimOrder=order)
+            lnZ = jt.msgForward()
+            bij = jt.msgBackward( beliefs = [fij.vars] )[fij.vars]
+            if (fij-bij).abs().max() > stoptol: done=False
+            model.addFactors( [fij/bij] )
+        if done: break
+    return
 
 
 def refit_pll_sgd(model,data, initStep=.01, maxIter=1000, verbose=False):
     """Fit a fixed graph structure to optimize pseudo-log-likelihood (uses basic SGD)
       model : an Ising model to re-fit (will keep edge structure)
       data  : (m,n) array of m data points with n variables (with values {0,1})
     """
@@ -442,21 +498,25 @@
     from sklearn.linear_model import LogisticRegression
     m,n = data.shape
   
     # TODO: just build (sparse) L directly & construct with it
     # for each Xi, estimate the neighborhood of Xi using L1-reg logistic regression:
     nbrs,th_ij,th_i = [None]*n, [None]*n, np.zeros((n,))
     Xtr, Xtmp = toPM(data.T), toPM(data.T)  # make two copies so we can modify; TODO: internal (n,m) shape
+    XtrE = np.hstack( (Xtr,np.zeros((n,2))) )
+    XtmpE= np.hstack( (Xtmp,np.zeros((n,2))) )
     for i in range(n):  
-        Xtmp[i,:] = 0.        # remove ourselves
-        lr = LogisticRegression(penalty='l1',C=C,solver='liblinear').fit(Xtmp.T,Xtr[i,:])
+        XtmpE[i,:] = 0.        # remove ourselves
+        XtrE[i,-2:]=[-1,1];  # ensure at least one +1 & -1
+        lr = LogisticRegression(penalty='l1',C=C,solver='liblinear').fit(XtmpE.T,XtrE[i,:])
         nbrs[i] = np.where(np.abs(lr.coef_) > 1e-6)[1]
         th_ij[i]= lr.coef_[0,nbrs[i]]/2.
         th_i[i] = lr.intercept_/2.
-        Xtmp[i,:] = Xtr[i,:]; # & restore after
+        XtrE[:,-2:] = 0     # blank out "pseudo" data
+        XtmpE[i,:] = XtrE[i,:]; # & restore after
     
     # Collect single-variable factors
     factors = [Factor(Var(i,2),[-t,t]).exp() for i,t in enumerate(th_i)]
 
     # Collect non-zero pairwise factors
     for i in range(n):
         for jj,j in enumerate(nbrs[i]):
```

### Comparing `pyGMs-0.1.1/pyGMs/messagepass.py` & `pyGMs-0.2.0/pyGMs/messagepass.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,17 +159,17 @@
 
     def update_weights(weights,idx,dW,stepW):   # TODO only works for positive weights
       wtot = 0.0
       for j,wt,dw in zip(idx,weights,dW): wt[j] *= np.exp( - stepW * wt[j] * dw ); wtot += wt[j];
       for j,wt,dw in zip(idx,weights,dW): wt[j] /= wtot;
 
     def armijo(thetas,weights,pri,Xi,steps,threshold=1e-4,direction=+1, optTol=1e-8,progTol=1e-8):
-      import copy
+      import copy, functools
       f0,f1 = None, calc_bound(thetas,weights,pri)                       # init prev, current objective values
-      match = reduce(lambda a,b: a&b, [th.vars for th in thetas], thetas[0].vars)
+      match = functools.reduce(lambda a,b: a&b, [th.vars for th in thetas], thetas[0].vars)
       idx = [th.v.index(Xi) for th in thetas] if Xi is not None else []  # find location of Xi in var/weight vectors
       newweights = copy.deepcopy(weights) if Xi is not None else weights # copy weights if updated
       for s in range(steps):
         # compute gradients dPhi/dTheta, dPhi/dW  (wrt parameters, weights):
         dT,dW = zip(*[calc_deriv(th,wt,pri,match,Xi) for th,wt in zip(thetas,weights)])
         dT,dW = list(dT),list(dW)
         for dt in dT[1:]: dt -= dT[0]; dt *= -1;
```

### Comparing `pyGMs-0.1.1/pyGMs/misc.py` & `pyGMs-0.2.0/pyGMs/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,33 +28,43 @@
     first = next(iter(D))
     try:
         next(iter(first))
         return True
     except: 
         return False
 
+
+def np2str(nparr,precision=2):
+    return np.array_str( nparr, precision=precision)
+
+def np2str1(nparr,precision=2,maxlen=None):
+    st = np.array_str( nparr, precision=precision).replace('\n','')
+    if (maxlen is not None) and (len(st)>maxlen): st = st[:maxlen] + "..."
+    return st
+
+
 ################################################################################################
 # Estimating empirical frequencies
 #
-def empirical( cliques, data, normalize=False):
+def empirical( cliques, data, weights=None, normalize=False):
     """Compute the empirical counts of each configuration of the cliques within the data
        Data should be integer, 0...d; any missing data (`nan') skipped (per clique)
        cliques (list) : list of VarSets; which subsets of variables to examine
        data (dict or (m,n) array) : data[s,i] is the value of x^(s)_i, x_i for sample s
        normalize (bool) : divide by the number of data in each estimate?
     """
     factors = [None]*len(cliques)
     for i,vs in enumerate(cliques):
         vs = VarSet(vs)                     # make sure these are OK & sorted
         try:    vs_data = data[:,[int(v) for v in vs]]      # 2d nparray data
-        except: vs_data = np.array([data[v] for v in vs])   # dict or 1d array
+        except: vs_data = np.array([[x[v] for v in vs] for x in data])   # dict or 1d array
         factors[i] = Factor(vs, 0.)
-        for xs in vs_data:
+        for s,xs in enumerate(vs_data):
           if np.any(np.isnan(xs)): continue    # skip data with missing entries  
-          factors[i].t[ tuple(xs.astype(int)) ] += 1.
+          factors[i].t[ tuple(xs.astype(int)) ] += 1. if weights is None else weights[s]
         if normalize: factors[i].t /= factors[i].sum()
     return factors 
 
 
 ################################################################################################
 # Evaluating data likelihood of a model
 #
@@ -111,31 +121,52 @@
       if (i+1 < n): E.append( (i*n+j,(i+1)*n+j) )
       if (j+1 < n): E.append( (i*n+j,i*n+j+1) )
   fs = [Factor([x],np.exp(sigu*np.random.randn(d))) for x in X]   # unary, then binary factors:
   fs.extend( [Factor([X[i],X[j]],np.exp(sigp*(T+T.T)/np.sqrt(2))) for i,j in E for T in [np.random.randn(d,d)*(1.0-np.eye(d))]] )
   #fs.extend( [Factor([X[i],X[j]],np.exp(sigp*np.random.randn(d,d)*(1.0-np.eye(d)))) for i,j in E] )
   return fs
 
+# TODO: flag to force ising model to be ferromagnetic? "force_sign = None/+1/-1?"
 
 def boltzmann(theta_ij):
   '''Create a pairwise graphical model from a matrix of parameter values.  
      .. math::
-       p(x) \propto \exp( \sum_{i \\neq j} \\theta_{ij} xi xj + \sum_i \\theta_{ii} xi )
+       p(x) \\propto \\exp( \\sum_{i \\neq j} \\theta_{ij} xi xj + \\sum_i \\theta_{ii} xi )
      theta : (n,n) array of parameters
   '''
   n = theta_ij.shape[0]
   X = [Var(i,2) for i in range(n)]
   nzi,nzj = np.nonzero( theta_ij )
   factors = [None]*len(nzi)
   for k,i,j in enumerate(zip(nzi,nzj)):
     if i==j: factors[k] = Factor([X[i]],[0,np.exp(theta[i,i])])
     else:    factors[k] = Factor([X[i],X[j]],[0,0,0,np.exp(theta[i,j])])
   return factors
 
 
+def random3SAT(alpha,n):
+    '''Create a random 3-SAT problem in CNF form
+      alpha : float : ratio of variables to clauses
+      n     : int   : number of variables
+      Returns a list of pyGMs Factors corresponding to each clause.
+    '''
+    import random
+    p = int(round(alpha*n))
+    X = [gm.Var(i,2) for i in range(n)] 
+    factors = []
+    for i in range(p):
+        #idx = [np.random.randint(n), np.random.randint(n), np.random.randint(n)]
+        idx = random.sample(range(n),3)
+        f = gm.Factor([X[idx[0]],X[idx[1]],X[idx[2]]],1.0)
+        cfg = [np.random.randint(2), np.random.randint(2), np.random.randint(2)]
+        f[cfg[0],cfg[1],cfg[2]] = 0.0
+        factors.append(f)
+    return factors
+
+## TODO: add random spatial graph generators? (Table distributions?)
 
 
 def fit_chowliu(data, penalty=0, weights=None):
     """Select a maximum likelihood tree-structured graph & parameters
       data: (m,n) nparray of m data points (values castable to int)
     """
     # TODO: add score f'n parameter, default to empirical MI?  or too complicated?
```

### Comparing `pyGMs-0.1.1/pyGMs/montecarlo.py` & `pyGMs-0.2.0/pyGMs/montecarlo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 montecarlo.py
 
 Defines several Monte Carlo and MCMC routines for approximate inference in graphical models
 
-Version 0.1.1 (2022-04-06)
+Version 0.2.0 (2024-04-01)
 (c) 2015 Alexander Ihler under the FreeBSD license; see license.txt for details.
 """
 
 import numpy as np
 #import time as time
 from time import time
 from sortedcontainers import SortedSet;
@@ -139,14 +139,32 @@
     #
     #@property
     #def neff(self):
     #    return self.wtot**2 / self.w2tot
 
 
 
+class QuerySamples(Query):
+    """Save a circular buffer of "keep" samples, inserting every "stride" MCMC steps."""
+    def __init__(self, keep=100, stride=10):
+        self.samples = [ None for i in range(keep) ]
+        self.i = 0
+        self.n = 0
+        self.stride = stride
+    def __getitem__(self,i):
+        return self.samples[(self.i+i)%len(self.samples)]
+    def __call__(self): 
+        return [self.samples[(i+self.i)%len(self.samples)] for i in range(len(self.samples)) ]
+    def update(self,x,w):
+        if (self.n % self.stride == 0):
+            self.samples[self.i] = x
+            self.i += 1; self.i = self.i % len(self.samples)
+        self.n += 1
+
+
 
 def GibbsSampling( model, query, state=None, stopSamples=1, stopTime = inf ):
     """Gibbs sampling procedure for discrete graphical model "model" with query object "query"
     """
     state = state if state is not None else [np.random.randint(Xi.states) for Xi in model.X]
     # TODO: timing check
     for j in range(stopSamples):
@@ -181,14 +199,30 @@
             state[Xi] = p.sample()[0]
             stateMap[Xi] = state[Xi]
         j += 1 
         query.update(state, 1.0)
     return query
 
 
+def GibbsSamplingBlock( model, query, state=None, blocks=None, stopSamples=1, stopTime = inf ):
+    """Gibbs sampling procedure for discrete graphical model "model" with query object "query"
+    """
+    if state is None: state = [ np.random.randint(v.states) for v in model.X]
+    if blocks is None: blocks = [ [x] for x in model.X ]   # basic single-var Gibbs
+    j = 0; stopTime += time()
+    while (j < stopSamples) and (time() < stopTime):
+        for b in blocks:
+            Pb = np.prod( [f.condition({v:state[v] for v in f.vars-b}) for f in model.factorsWithAny(b)] )
+            xb = Pb.sample()
+            for i,xi in zip(b,xb): state[i]=xi
+        j += 1
+        query.update(state, 1.0)
+    return query
+
+
 
 
 def Metropolis( model, query, proposal, state=None, stopSamples=1, stopTime = inf ):
     """Metropolis-Hastings sampling for discrete graphical model "model" with query object "query"
        proposal : function object: newstate,logratio = proposal(oldstate) 
                   propose random transition "old -> new" and report log q(old->new)/q(new->old)
     """
@@ -231,11 +265,38 @@
 ###    Verify GM is a BN; sample Xh & eval Xe
 
 ### Importance sampling (generic form?)
 ###   f(x), q(x) draw and eval; queries
 ###   
 
 
+def ImportanceSampling(model, query, proposal, stopSamples=1, stopTime = inf):
+    j = 0; stopTime += time();
+    while (j < stopSamples) and (time() < stopTime):
+        xi,qi = proposal()
+        fi = model.logValue(xi)
+        query.update(xi,np.exp(fi-qi))   # exp? do weights in log form?
+        j += 1
+    return query
 
+def AnnealedImportanceSampling(model, query, base, K=10, stopSamples=1, stopTime=inf):
+    j = 0; stopTime += time()
+    model_eps = model.copy(); model_eps.makePositive();
+    while (j < stopSamples) and (time() < stopTime):
+        xi,ln_wi = gm.bnSample(base, gm.bnOrder(base)) # TODO: how? bnSample?  wi = 1?
+        current = base
+        for t in np.linspace(1./T,1,T):
+            annealed = GraphModel( [f**(1.-t) for f in base.factors]+[f**t for f in model_eps.factors] )
+            ln_wi += (annealed.logValue(xi) - current.logValue(xi))
+            xi = GibbsSamplingBlock(annealed, QuerySamples(1,1), state=xi, stopSamples=K)[0]
+        ln_wi += (model_eps.logValue(xi) - model.logValue(xi))
+        query.update(xi,np.exp(wi))
+    return query
 
+### Annealed IS:
+###   provide base proposal p0, target f, # temp, positivity eps, Gibbs method (cliques, # steps)
+###   sample x ~ p0, define p+ = f/Zhat+eps, pt = (p0)^(1-t)*(p+)^t, t=1/#t; w = pt(x)/f 
+###   for t=2/#t...1: MCMC(pt,x); w*=pt+1/pt;
+###   w*=f/p+
+###      ** if p0 factors like p+, we can use local ops for gibbs. what if not? (enum?) (pass GModel vs pass eval f'n)
```

### Comparing `pyGMs-0.1.1/pyGMs/search.py` & `pyGMs-0.2.0/pyGMs/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,19 @@
     self.parent = parent
     self.children = []
     #self.priority = -inf
     self.value = val
     self.heuristic = None
     self.X = X
     self.x = x   # node is for assignment X=x given ancestor assigments
-
+  def __str__(self): 
+    return(('' if self.parent is None else (str(self.parent)+',')) + 
+           ('' if self.X is None else (str(self.X)+'.')) +
+           ('' if self.x is None else str(self.x)))
+  def __lt__(self,other): return self.value < other.value
 
 
 class PrunedDFS(object):
   """Depth-first search using pruning."""
   def __init__(self, model, heuristic, weights='max', xinit={}):
     self.model = model
     self.heuristic = heuristic
@@ -81,16 +85,18 @@
             self.xhat = self.cfg.copy(); 
             if verbose: print("[{}]".format(self.L),[self.xhat[v] for v in self.model.X])
         else:                          # else, update heuristic given n.X = n.x
           n.heuristic, n.value = n.heuristic.update(self.cfg,n.X,n.x)
 
         if not self.prune(n):           # if not pruned, expand n & generate children:
           X,vals = n.heuristic.next_var(self.cfg,n.X,n.x)
-          idx = np.argsort(vals)
-          n.children = [NodeDFS(n,X,i,vals[i]) for i in idx]
+          n.children = [(-vals[i],NodeAStar(n,X,i,vals[i])) for i in idx]
+          heapq.heapify(n.children)
+          #idx = np.argsort(vals)
+          #n.children = [NodeDFS(n,X,i,vals[i]) for i in idx]
           for c in n.children: c.heuristic = n.heuristic   # point to previous heuristic
 
         # Now move on to the next node in the queue
         self.node, self.cfg = self.__next(n) 
         
 
 
@@ -99,14 +105,19 @@
     self.parent = parent
     self.children = []
     #self.priority = -inf
     self.value = val
     self.heuristic = None
     self.X = X
     self.x = x   # node is for assignment X=x given ancestor assigments
+  def __str__(self): 
+    return(('' if self.parent is None else (str(self.parent)+',')) + 
+           ('' if self.X is None else (str(self.X)+'.')) +
+           ('' if self.x is None else str(self.x)))
+  def __lt__(self,other): return self.value < other.value
 
 class AStar(object):
   """A-Star heuristic search """
   def __init__(self, model, heuristic, weights='max', xinit={}):
     self.model = model
     self.heuristic = heuristic
     if len(xinit): self.xhat = xinit; self.L = model.logValue(xinit) # use initial config
```

### Comparing `pyGMs-0.1.1/pyGMs/varset_py.py` & `pyGMs-0.2.0/pyGMs/varset_py.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Pure python implementation of variables ("id" and state size) and variable sets (sorted lists of variables
+Pure python implementation of variables ("id" and state size) and variable sets (sorted lists of variables)
 
 """
 
 import numpy as np
 from sortedcontainers import SortedSet as sset;
 from functools import reduce
```

### Comparing `pyGMs-0.1.1/pyGMs/weighted.py` & `pyGMs-0.2.0/pyGMs/weighted.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Weighted graphical model:
 A graphical model (GraphModel) augmented with an elimination order and weights (temperatures) for each Xi 
-Corresponds to an inference problem, Phi_w = \log [ ... \wsum_{x_i} ... \exp[ \sum_r \theta_r(X_r) ] ... ]
+Corresponds to an inference problem, Phi_w = \\log [ ... \\wsum_{x_i} ... \\exp[ \\sum_r \\theta_r(X_r) ] ... ]
 Always maintains factors in log form (theta_r)
 
 Constructor takes factors, order (default 1..N), weights (default 1.0)
 Can set order, weights manually
 Can "reorder" -- find new elimination order that preserves problem definition (e.g., only switch
 the order of variables with equal weights).
```

### Comparing `pyGMs-0.1.1/pyGMs/wmb.py` & `pyGMs-0.2.0/pyGMs/wmb.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,23 +20,25 @@
 
 """
 from .factor import *
 from .graphmodel import *
 
 from builtins import range
 try:
-    from itertools import izip
+    from itertools import izip    # OLD python versions required this
 except:
-    izip = zip
+    izip = zip                    # more recent versions we can just do this
 
 
 reverse_enumerate = lambda l: izip(range(len(l)-1, -1, -1), reversed(l))
 
 class WMB(object):
-    '''Class implementing weighted mini-bucket elimination inference'''
+    '''Class implementing weighted mini-bucket elimination inference.
+    See documentation and example notebooks for usage.
+    '''
 
     # Internal object / structure for representing a mini-bucket
     class Node:
         """Internal container object for mini-bucket nodes"""
         def __init__(self):
             self.clique = VarSet()
             self.theta = Factor().log()
@@ -51,21 +53,30 @@
         def __str__(self):
             return "{}".format(self.clique)
         def __lt__(self, other):
             return False         # don't care about ordering nodes
 
 
     class ConstantList:
+        """Internal helper object for treating scalars and lists interchangably"""
         def __init__(self, val):
             self.val = val
         def __getitem__(self, loc):
             return self.val
 
 
-    def __init__(self, model, elimOrder=None, iBound=0, sBound=0, weights=1.0, attach=True, **kwargs):
+    def __init__(self, model, elimOrder=None, iBound=None, sBound=None, weights=1.0, attach=True, **kwargs):
+        """Construct a mini-bucket object from a given graphical model.
+          model : GraphModel object representing the graphical model
+          elimOrder : an elimination order (list-like) or method (e.g. "minfill")
+          iBound : maximum number of variables in any mini-bucket clique
+          sBound : maximum number of state configurations for any mini-bucket clique
+          weights: weighted elimination per bucket; see setWeights()
+          attach : construct clique functions (True) or postpone until later (False)
+        """
         # TODO: check if model isLog() true
         # save a reference to our model
         self.model = model
         self.X     = model.X
         self.logValue = model.logValue
 
         # create & process elimination ordering of the model:
@@ -76,23 +87,24 @@
             elimOrder = eliminationOrder(self.model, orderMethod=elimOrder)[0];  
         self.elimOrder = elimOrder
         self.priority = [-1 for i in range(model.nvar)]  # build priority of each var
         for i,x in enumerate(elimOrder): self.priority[x] = i
 
         # now build the mini-bucket data structure
         self.buckets = [ [] for x in range(model.nvar) ]  # bucket for each var: list of minibuckets 
-        self.matches = [ [] for x in range(model.nvar) ] # matching sets for each bucket
-        self.setWeights(weights)   # TODO: duplicate to initialize (!)
+        self.matches = [ [] for x in range(model.nvar) ]  # matching sets for each bucket
+        self.weights = WMB.ConstantList(1.0)              # default to sum+ during construction
         for f in model.factors:
             if len(f.vars)==0: continue;      #TODO: should add anyway (somewhere)
             n = self.addClique(f.vars)
-            if attach: n.theta += f.log()                 # include log f(x) in node's log-factor
+            if attach: n.theta += f if model.isLog else f.log()  # include log f(x) in node's log-factor
             n.originals.append(f)              # append (pointer to) original f for later reference
-        # and set the weights of the buckets:
-        self.setWeights(weights)
+        if iBound is not None or sBound is not None:      # perform merging if criteria given at init
+            self.merge(self.scoreByScope(ibound=iBound,sbound=sBound))
+        self.setWeights(weights)                          # and set the weights of the buckets
  
     def setWeights(self,weights):
         """Set the weights of the inference problem.
         weights = 'max+' or 0.0  => upper bound the MAP configuration
                   'sum+' or 1.0  => upper bound the partition function
                   'sum-' or -1.0 => lower bound the partition function
         For more general bounds, weights = list of floats (one per variable)
@@ -119,35 +131,27 @@
         """Helper function: get identifier (bucket & location) of a given node""" 
         if not isinstance(node, WMB.Node): return None,None
         i = min([self.priority[x] for x in node.clique])  # get bucket
         j = self.buckets[i].index(node)
         return i,j
    
     def __repr__(self):     
+        """Detailed representation of the mini-bucket structure as a text string"""
         to_return = ""
         for i,b in enumerate(self.buckets):
             to_return += "{:03d}: ".format(int(self.elimOrder[i]))
             for j,mb in enumerate(b):
                 to_return += "{!s}^{:.2f} => {}; ".format(mb,mb.weight, self.__nodeID(mb.parent))
             to_return += "\n"
         return to_return
 
-#    def draw(self):
-#        import pygraphviz
-#        G = pygraphviz.AGraph()
-#        for i,b in enumerate(self.buckets):
-#            for j,mb in enumerate(b):
-#                G.add_node(self.__nodeID(mb))
-#        for i,b in enumerate(self.buckets):
-#            for j,mb in enumerate(b):
-#                G.add_edge(self.__nodeID(mb),self.__nodeID(mb.parent))
-#        G.layout()        # layout with default (neato)
-#        G.draw('wmb.png') # draw png
-
     def draw(self):
+        """Draw mini-bucket tree in networkx.  Limited usefulness without good positioning.
+        Returns the networkx DiGraph of the mini-bucket tree.
+        """
         import networkx as nx
         pos,labels = {},{}
         G = nx.DiGraph()
         for i,b in enumerate(self.buckets):
             for j,mb in enumerate(b):
                 G.add_node(str(mb))
                 pos[str(mb)] = (j,-i)
@@ -165,35 +169,35 @@
         vs = VarSet(vars)
         corder = np.argsort( [self.priority[x] for x in vars]  ) # get order in which eliminated
         corder = [vars[c] for c in corder]
         added = []
         found = False
         for x in corder:
             if found: break
-            #print "bucket ",x
+            #print("bucket ",x)
             b = self.buckets[self.priority[x]]
             to_remove = []
             for mb in b:
-                #print "  check ",mb
+                #print("  check ",mb)
                 if mb.clique < vs:
                    to_remove.append(mb)
                 if mb.clique >= vs:                # if we found a minibucket we can just join, do:
                     if len(added) > 0:             # if we've added nodes, connect them as descendants
                         mb.children.append( added[-1] )  # of the found node, and found node as parent of last
                         added[-1].parent = mb          
                     found = True                   # now, we don't need to keep generating parents
-                    #print "    Found!"
+                    #print("    Found!")
                     added.append(mb)               # not really added, but the end of the added chain
                     break
             # if we didn't find any mini-buckets we can join, we need to add one:
             if not found:                          # 
                 n = WMB.Node()
                 n.clique = VarSet(vs)
                 n.weight = -1e-3 if self.weights[x] < 0 else 1e-3;   # TODO: small non-zero weights
-                #print "adding ",n," to ",self.priority[x]
+                #print("adding ",n," to ",self.priority[x])
                 b.append(n)
                 if len(added) > 0:                 #   then, last added node is the child of this one
                     n.children.append(added[-1])
                     added[-1].parent = n
                 added.append(n)                    #   put in added list 
                 vs -= [x]                          #   next bucket is what's left after x is eliminated
                 for mb in to_remove:
@@ -219,102 +223,113 @@
             for mb in b:
                 mb.theta = Factor([],0.)
 
     def attachFactors(self):
         """Re-attach factor tables to their associated cliques for evaluation"""
         for b in self.buckets:
             for mb in b:
-                mb.theta = Factor([],0.)
-                for f in mb.originals: mb.theta += f.log()
-    # TODO: check if already in log form???
+                mb.theta = Factor([],0.)    # TODO: need to ensure Xb is there in case no factor includes it?
+                for f in mb.originals: 
+                    mb.theta += f if self.model.isLog else f.log()  # TODO: check if already in log form?
 
     def memory(self, bucket=None, use_backward=True):
-        """Compute the total memory (in MB) required for this mini-bucket approximation"""
+        """Estimate the total memory (in MB) required for this mini-bucket approximation"""
         mem = 0.
         use_buckets = self.buckets if bucket is None else [self.buckets[bucket]]
         for b in use_buckets:
             for mb in b:
                 mem += mb.clique.nrStatesDouble() * mb.theta.table.itemsize
                 # TODO: add forward & backward message costs here also
         return mem / 1024. / 1024.
 
     # TODO: convert to external function?  pass variable in; check if refinement of another?
-    #  Is score correct, or inverted?  check
     def scoreByScope(self, ibound=None, sbound=None):
       """Returns a scope-based scoring function for use in merge()"""
       def score(m1,m2):
         jt = m1.clique | m2.clique
         if ibound is not None and len(jt) > ibound: return -1
         if sbound is not None and jt.nrStates() > sbound: return -1
         # TODO: also disallow if not consistent with some specified scope sets?
         mx,mn = max([len(m1.clique),len(m2.clique)]), min([len(m1.clique),len(m2.clique)])
-        return 1.0/(float(mx)+float(mn)/mx)
+        #return 1.0/(float(mx)+float(mn)/mx)   # prefers merging smaller cliques first
+        return (float(mx)+float(mn)/(mx+1))    # prefer merging largest cliques
       # return the scoring function 
       return score
 
 
     # score = len(max)+len(min)/len(max) if union < iBound else -1 for scope
     def merge(self, score):
+        """merge(score_function) : perform score-based merging of mini-buckets
+        Merging cliques of the mini-bucket tree typically improves accuracy at a computational cost.
+        score : a function, score(m1,m2), that evaluates a pair of mini-bucket cliques,
+                determines if they can be merged, and prioritizes them.
+                Higher value pairs are merged first; a negative return value indicates an invalid merge.
+                See WMB.scoreByScope() for an example.
+        """
         from heapq import heappush,heappop
         try:
           from itertools import count
           tiebreak = count().__next__        # need tiebreaker value for priority queue (?)
         except:
           tiebreak = lambda: 0
         for b in self.buckets:
             priority = [] 
             lookup = {}
             # see not-too-efficient-looking remove_task https://docs.python.org/2/library/heapq.html
             # build scores:
             for i,m1 in enumerate(b):
                 for m2 in b[i+1:]:
                     s = score(m1,m2)
-                    if s >= 0.0:
-                        entry = [-s,tiebreak(),m1,m2]
+                    if s >= 0.0:                       # if the merge is allowed,
+                        entry = [-s,tiebreak(),m1,m2]  # add it to the priority heap
                         lookup[(m1,m2)] = entry
                         heappush(priority, entry)
             while len(priority):
-                entry = heappop(priority)
+                entry = heappop(priority)              # find the best pair to merge:
                 s,_,m1,m2 = entry[0],entry[1],entry[2],entry[3]
                 #s,m1,m2 = priority.pop()
                 if m1 is None or m2 is None: continue
                 if m1 not in b or m2 not in b: continue   ## check for removed minibuckets?
-                #print b
-                #print "Merging ",m1,"+",m2
-                for m in b:
+                #print("Merging ",m1,"+",m2)
+                for m in b:                            # mark anything involving m1 or m2 as now invalid
                     for ma,mb in [(m1,m),(m,m1),(m2,m),(m,m2)]:
                         s = -lookup.get( (ma,mb), [1,None,None] )[0]
                         if s >= 0.0: 
                             entry = lookup.pop( (ma,mb) )
                             entry[2],entry[3] = None,None  # mark as "removed"
                             #priority.remove( [s,ma,mb] )
                 m12 = self.addClique( m1.clique | m2.clique )
                 # what if others removed?  (bad check above?)
-                #print b
-                for m in b:
+                #print(b)
+                for m in b:                            # now check possible merges with new m1+m2
                     if m is m12: continue
                     s = score(m12,m)
-                    if s >= 0.0:
+                    if s >= 0.0:                       # if the merge is allowed, add it to queue
                         entry = [-s,tiebreak(),m12,m] 
                         lookup[ (m12,m) ] = entry
                         heappush(priority,entry)
         return None
 
 
-
-    def mergeScope(iBound=0, sBound=0): 
-        for Bi in self.buckets:
-            # TODO: sort bucket by size (or store sorted)
-            for mb in Bi:
-                # TODO: merge into largest clique that can fit
-                pass
+    ### Removed; equivalent to wmb.merge( wmb.scoreByScope(iB, sB) )
+    #def mergeScope(iBound=0, sBound=0): 
+    #    for Bi in self.buckets:
+    #        # TODO: sort bucket by size (or store sorted)
+    #        for mb in Bi:
+    #            # TODO: merge into largest clique that can fit
+    #            pass
 
     #@profile
     def msgForward(self, stepTheta=0.5, stepWeights=0.1):
-        """Compute a forward pass through all nodes and return the resulting bound"""
+        """Compute a forward pass through all nodes and return the resulting bound
+          stepTheta, stepWeights : step size of reparameterization updates (theta) and weights.
+            Ex: stepTheta = 1., stepWeights = 0.  => "moment matching" downward pass
+                stepTheta = 0., stepWeights = 0.  => Basic mini-bucket forward computation
+        Returns the current bound on the mini-bucket objective (lnZ or lnF, depending on weight settings)
+        """
         bound = 0.0
         for i,b in enumerate(self.buckets):
             X = self.model.vars[ self.elimOrder[i] ]
             nNodes = len(b)
             beliefs = [ None for mb in b ]
             if nNodes > 1:  # if more than one mini-bucket partition, pre-compute beliefs:
                 if stepTheta or stepWeights:
@@ -386,35 +401,38 @@
                     bound += mb.msgFwd  
         return float(bound)
 
 
     #@profile
     def msgBackward(self, stepTheta=0.0, stepWeights=0.0, beliefs=None):
         """Compute a backward pass through all nodes
-           If beliefs is a list of cliques, returns the estimated beliefs on those cliques
+           stepTheta, stepWeights : update bound using step sizes on clique functions & weights
+           beliefs : a list of cliques (VarSets) on which to estimate marginal probabilities
+           Returns a map { clique :  factor } of cliques & estimated marginals
+           Raises ValueError if a requested clique is not present anywhere in the mini-bucket.
         """
         to_save = [[] for i in range(len(self.buckets))]
         if beliefs is None:
             return_beliefs = {}
         else:
             return_beliefs = { clique: None for clique in beliefs }
             # map cliques to buckets for checking
             for clique in beliefs:
                 to_save[ min([self.priority[x] for x in clique]) ].append(VarSet(clique))
-        for i,b in reverse_enumerate(self.buckets): #reversed(list(enumerate(self.buckets))):
+        for i,b in reverse_enumerate(self.buckets): 
             X = self.model.vars[ self.elimOrder[i] ]
             nNodes = len(b)
             beliefs_b = [ None for mb in b ]
             if nNodes > 1:  # if more than one mini-bucket partition, pre-compute beliefs:
                 if stepTheta or stepWeights:
                     for j,mb in enumerate(b):
                         beliefs_b[j] = mb.theta + mb.msgBwd
                         for c in mb.children: beliefs_b[j] += c.msgFwd
                         beliefs_b[j] *= 1.0/mb.weight
-                        beliefs_b[j] -= bel[j].lse()
+                        beliefs_b[j] -= beliefs_b[j].lse()
                 # Then, update theta (parameterization) on each set in "matches"
                 if stepTheta:  
                     pass
                 if stepWeights:
                     pass
             # now, compute the backward messages:
             for j,mb in enumerate(b):
@@ -426,35 +444,42 @@
                 #else:
                 #    beliefs_b[j] -= beliefs_b[j].min()   # invert if negative? TODO?
                 beliefs_b[j] *= 1.0 / mb.weight
                 for c in mb.children:
                     c.msgBwd = beliefs_b[j].lse( mb.clique - c.clique )*c.weight - c.msgFwd
                     #c.msgBwd -= c.msgBwd.max()   # TODO normalize for convenience?
                     #c.msgBwd = (beliefs_b[j]*(1.0/mb.weight)).lse( mb.clique - c.clique )*c.weight - c.msgFwd
-                # TODO: compute marginal of any to_save[i] cliques that fit & not done
                 for c in to_save[i]:
-                    if c <= mb.clique and return_beliefs[c] is None: return_beliefs[c] = beliefs_b[j].lse( mb.clique - c )
+                    if c <= mb.clique and return_beliefs[c] is None: 
+                        return_beliefs[c] = beliefs_b[j].lse( mb.clique - c )
                 beliefs_b[j] = Factor().log() # clear out belief
         for c,f in return_beliefs.items(): 
-            f -= f.lse()
-            f.expIP()   # exponentiate and normalize beliefs before returning
-            #f /= f.sum()
+            if f is None: raise ValueError(f'Belief over {c} not available in WMB structure!')
+            f -= f.lse()      # exponentiate and normalize beliefs before returning
+            f.expIP()     
         return return_beliefs
 
 
     def reparameterize(self):
+        """reparameterize() : update the current mini-bucket clique factors to incorporate the forward messages
+          Useful for switching to a decomposition bound method after WMB message passing.
+        """
         for i,b in enumerate(self.buckets):
           for j,mb in enumerate(b):
             if mb.parent is not None:
               mb.theta -= mb.msgFwd
               mb.parent.theta += mb.msgFwd
               mb.msgFwd *= 0.0
 
 
     def gdd_update(self,maxstep=1.0,threshold=0.01):
+        """gdd_update : update the clique factors using generalized dual decomposition gradients.
+          Often slower than WMB messages, but should ensure monotonic bound changes.
+        """
+        from functools import reduce
         def wt_elim(f,w,pri):
             elim_ord = np.argsort( [pri[x] for x in f.vars] )
             tmp = f.copy();
             for i in elim_ord:
               tmp = tmp.lsePower([f.v[i]],1.0/w[i])
             return tmp
         def calc_bound( thetas, weights, pri):
@@ -535,18 +560,20 @@
         return float(bound)
 
 
 
 
     # TODO: rename greedy-assign?  Add optional partial config?
     def assignBackward(self):
-        """Perform a backward pass through all nodes, assigning the most likely value"""
+        """Perform a backward pass through all nodes, greedily assigning the most likely value.
+        If weights='max' and each bucket has only one mini-bucket, this returns the optimal model configuration.
+        """
         # TODO check & test  ; check for zero weights? (don't care?)
         x = {}
-        for i,b in reverse_enumerate(self.buckets): #reversed(list(enumerate(self.buckets))):
+        for i,b in reverse_enumerate(self.buckets):    
             X = self.model.vars[ self.elimOrder[i] ]
             bel = Factor([X],0.0)
             for j,mb in enumerate(b):
                 bel += mb.theta.condition(x)
                 for c in mb.children: bel += c.msgFwd.condition(x)
             x[X] = bel.argmax()[0]
         return x
@@ -559,32 +586,33 @@
             if mb.parent is not None:
               pi,pj = self.__nodeID(mb.parent)
               for ii in range(i+1,pi+1): self.atElim[ii].append(mb);
 
     def heuristic(self,X,config):
         """Evaluate the bound given partial assignment 'config' (including variable X and all later)"""
         return sum([mb.msgFwd.valueMap(config) for mb in self.atElim[X]])
-        #raise NotImplementedError   # TODO: fix
         # need desired pseudo-tree & track messages passing between earlier & later buckets
 
     def resolved(self,X,config):
         """Evaluate the resolved value of a partial assignment 'config' (including variable X and all later)"""
         return sum([mb.theta.valueMap(config) for b in self.buckets[self.priority[X]:] for mb in b])
 
     def newly_resolved(self,X,config):
         """Evaluate the change in resolved value of a partial assignment 'config' after clamping X"""
         return sum([mb.theta.valueMap(config) for mb in self.buckets[self.priority[X]]])
 
     def sample(self):  
-        """Draw a sample from the WMB-IS mixture proposal (assumes sum+ task)"""
+        """Draw a sample from the WMB-IS mixture proposal (assumes sum+ task)
+        Returns x,q  where x (config) is the sampled configuration and q (float) is its log-probability under the proposal.
+        """
         # TODO: add argument "x" for partial conditioning?  (return of configuration? or return tuple?)
         # TODO check for positive, unit sum weights?  (don't care?)
         x = {}
         logQx = 0.0
-        for i,b in reverse_enumerate(self.buckets): #reversed(list(enumerate(self.buckets))):
+        for i,b in reverse_enumerate(self.buckets): 
             X = self.model.vars[ self.elimOrder[i] ]
             qi = Factor([X],0.0)
             for j,mb in enumerate(b):
                 qij = mb.theta.condition(x)
                 qij -= mb.msgFwd if mb.parent is None else mb.msgFwd.condition(x)
                 for c in mb.children: qij += c.msgFwd.condition(x)
                 qij -= qij.max()
@@ -592,15 +620,15 @@
                 qij.expIP()
                 qij *= mb.weight
                 qi += qij
             qi /= qi.sum()   # normalize (should be already)
             xval = qi.sample(Z=1.0)[0]
             x[X] = xval
             logQx += np.log( qi[xval] )
-        return logQx,x
+        return x,logQx
 
 
 # functions:
 # addClique(vs) : add clique etc and [fix up structure beneath]
 #   => build = add each clique in turn => valid structure?
 # 
 
@@ -629,28 +657,47 @@
     def __init__(self, model, elimOrder=None, weights=1.0):
         super(JTree,self).__init__(model,elimOrder=elimOrder,weights=weights)
         self.merge(lambda a,b: 1.0)    # merge until exact 
         self.forwardDone = False
         self.setWeights(weights)
 
     def msgForward(self):
+        """Perform a forward pass of the junction tree.
+          Returns the inference value: partition function for `sum`, optimal value for `max`.
+        """
         return_value = super(JTree,self).msgForward()
         self.forwardDone = True
         return return_value
 
     def beliefs(self, beliefs=None):
+        """Compute a set of marginals of the junction tree.  Calls msgForward if not yet done.
+          beliefs = list of variable sets, corresponding to the desired marginals.
+          Returns a corresponding length list of marginal factors.
+        """
         if beliefs is None: return {}
         if not self.forwardDone: self.msgForward()   # or raise valueerror?
         return super(JTree,self).msgBackward(beliefs=beliefs)
 
     def argmax(self):
+        """Compute a maximizing argument of the junction tree.  Calls msgForward if not yet done."""
         if not self.forwardDone: self.msgForward()   # or raise valueerror?
         return super(JTree,self).assignBackward()
 
     def sample(self):
+        """Draw a sample from the junction tree.  Calls msgForward if not yet done."""
         if not self.forwardDone: self.msgForward()   # or raise valueerror?
         return super(JTree,self).sample()
 
-    # Smartly accommodate changes to the model?
+    def __repr__(self):
+        """Overrides WMB __repr__ method to remove unnecessary details"""
+        to_return = ""
+        for i,b in enumerate(self.buckets):
+            to_return += "{:03d}: ".format(int(self.elimOrder[i]))
+            for j,mb in enumerate(b):
+                to_return += "{!s} => ({}); ".format(mb, self._WMB__nodeID(mb.parent)[0])
+            to_return += "\n"
+        return to_return
+
+    # TODO?: Smartly accommodate changes to the model?
```

### Comparing `pyGMs-0.1.1/pyGMs/wogm.py` & `pyGMs-0.2.0/pyGMs/wogm.py`

 * *Files identical despite different names*

### Comparing `pyGMs-0.1.1/pyGMs.egg-info/PKG-INFO` & `pyGMs-0.2.0/pyGMs.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: pyGMs
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python Graphical Models Toolbox
 Author: Alexander Ihler
 Author-email: ihler@ics.uci.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-pyGM : A Python toolbox for Graphical Models
+pyGMs : A Python toolbox for Graphical Models
 ================
 
 This code provides a simple Python-based interface for defining probabilistic
 graphical models (Bayesian networks, factor graphs, etc.) over discrete random
 variables, along with a number of routines for approximate inference.  It is
 being developed for use in teaching, as well as prototyping for research.
 
@@ -24,21 +22,19 @@
 operating on the table-based representation of discrete factors, and
 [SortedContainers](https://pypi.python.org/pypi/sortedcontainers) for some
 internal representations.  Smaller portions use [networkx](https://networkx.org/)
 and [scipy](https://www.scipy.org/) as well.
 
 ## Installation
 
-Simply download or clone the repository to a directory *pyGM*, and add its
+Simply download or clone the repository to a directory *pyGMs*, and add its
 parent directory to your Python path, either:
 ```
 $ export PYTHONPATH=${PYTHONPATH}:/directory/containing/
 ```
 or in Python
 ```
 import sys
 sys.path.append('/directory/containing/')
 ```
 
 
-
-
```

### Comparing `pyGMs-0.1.1/setup.py` & `pyGMs-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open("readme.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyGMs',
     #name=pyGM.__title__,
     #version=pyGM.__version__,
-    version='0.1.1',
+    version='0.2.0',
     author='Alexander Ihler',
     author_email='ihler@ics.uci.edu',
     description='Python Graphical Models Toolbox',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     python_requires='>=3.6',
```

