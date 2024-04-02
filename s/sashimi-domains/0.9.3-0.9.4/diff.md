# Comparing `tmp/sashimi_domains-0.9.3.tar.gz` & `tmp/sashimi_domains-0.9.4.tar.gz`

## Comparing `sashimi_domains-0.9.3.tar` & `sashimi_domains-0.9.4.tar`

### file list

```diff
@@ -1,50 +1,49 @@
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/TODO
--rw-r--r--   0        0        0   441328 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/doc/domain topic map.png
--rw-r--r--   0        0        0    26080 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/limbo/blockology.py
--rw-r--r--   0        0        0     4308 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/limbo/corporalogy.py
--rw-r--r--   0        0        0    15646 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/limbo/graphology.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/__init__.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/config.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/entropies.py
--rw-r--r--   0        0        0     9758 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/ioio.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/misc.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/naming.py
--rw-r--r--   0        0        0    18265 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/scorology.py
--rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/vectorology.py
--rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/w2v_score.py
--rw-r--r--   0        0        0    16237 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/#annotations.py#
--rw-r--r--   0        0        0    13901 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/__init__.py
--rw-r--r--   0        0        0    16246 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/annotations.py
--rw-r--r--   0        0        0     8885 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/area_rank_chart.py
--rw-r--r--   0        0        0    11244 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/block_ext_map.py
--rw-r--r--   0        0        0    44214 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/hierarchical_block_map.py
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/hierarchical_block_map_help.html
--rw-r--r--   0        0        0     8002 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/link_maps.py
--rw-r--r--   0        0        0    11670 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/network_map.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/util.py
--rw-r--r--   0        0        0     8937 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/zmethods.py
--rw-r--r--   0        0        0    10540 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/tables/__init__.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/tables/tables.css
--rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/tables/tables_html.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/blocks/tables/tables_plots.py
--rw-r--r--   0        0        0    37282 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/corpus/__init__.py
--rw-r--r--   0        0        0     6200 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/corpus/nlp.py
--rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/corpus/parsers.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/corpus/wos.py
--rw-r--r--   0        0        0    20413 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/graph_models/__init__.py
--rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/graph_models/domain_chained_model.py
--rw-r--r--   0        0        0     6602 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/graph_models/domain_topic_model.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/graph_models/util.py
--rwxr-xr-x   0        0        0     1746 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/util/asco_clean.py
--rwxr-xr-x   0        0        0      451 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/util/pubmed_clean.py
--rwxr-xr-x   0        0        0      612 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/util/pubmed_get.sh
--rwxr-xr-x   0        0        0     6667 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/util/scan_bugtrap.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/util/wos_lam/__init__.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/src/sashimi/util/wos_lam/wos_api_request.tpl
--rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/tests/test_basic_usage.py
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/tests/test_pclabel_bfield.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/.gitignore
--rw-r--r--   0        0        0    35061 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/LICENSE
--rw-r--r--   0        0        0     8175 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/README.md
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     9516 2020-02-02 00:00:00.000000 sashimi_domains-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0    26090 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/limbo/blockology.py
+-rw-r--r--   0        0        0     4308 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/limbo/corporalogy.py
+-rw-r--r--   0        0        0    15649 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/limbo/graphology.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/__init__.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/config.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/entropies.py
+-rw-r--r--   0        0        0     9758 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/ioio.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/misc.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/naming.py
+-rw-r--r--   0        0        0    18265 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/scorology.py
+-rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/vectorology.py
+-rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/w2v_score.py
+-rw-r--r--   0        0        0    14986 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/__init__.py
+-rw-r--r--   0        0        0    17831 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/annotations.py
+-rw-r--r--   0        0        0     9676 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/area_rank_chart.py
+-rw-r--r--   0        0        0    14781 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/better_network_map.py
+-rw-r--r--   0        0        0    11244 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/block_ext_map.py
+-rw-r--r--   0        0        0    55053 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/hierarchical_block_map.py
+-rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/hierarchical_block_map_help.html
+-rw-r--r--   0        0        0     8002 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/link_maps.py
+-rw-r--r--   0        0        0    11655 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/network_map.py
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/util.py
+-rw-r--r--   0        0        0     8946 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/zmethods.py
+-rw-r--r--   0        0        0    10565 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/tables/__init__.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/tables/tables.css
+-rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/tables/tables_html.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/blocks/tables/tables_plots.py
+-rw-r--r--   0        0        0    37395 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/corpus/__init__.py
+-rw-r--r--   0        0        0     6200 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/corpus/nlp.py
+-rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/corpus/parsers.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/corpus/wos.py
+-rw-r--r--   0        0        0    14648 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/graph_models/__init__.py
+-rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/graph_models/blockstate_to_dataframes.py
+-rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/graph_models/domain_chained_model.py
+-rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/graph_models/domain_topic_model.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/graph_models/util.py
+-rwxr-xr-x   0        0        0     1746 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/util/asco_clean.py
+-rwxr-xr-x   0        0        0      451 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/util/pubmed_clean.py
+-rwxr-xr-x   0        0        0      612 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/util/pubmed_get.sh
+-rwxr-xr-x   0        0        0     6667 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/util/scan_bugtrap.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/util/wos_lam/__init__.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/src/sashimi/util/wos_lam/wos_api_request.tpl
+-rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/tests/test_basic_usage.py
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/tests/test_pclabel_bfield.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/.gitignore
+-rw-r--r--   0        0        0    35061 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/LICENSE
+-rw-r--r--   0        0        0     8187 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/README.md
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     9528 2020-02-02 00:00:00.000000 sashimi_domains-0.9.4/PKG-INFO
```

### Comparing `sashimi_domains-0.9.3/src/limbo/blockology.py` & `sashimi_domains-0.9.4/src/limbo/blockology.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
         for level in reversed(levels):
             print("Processing level {}".format(level))
             columns = tuple(
                 sorted(
                     [
                         tuple(reversed(x))
-                        for x in blocks[levels[level - 1 :]]
+                        for x in blocks[levels[levels.index(level) :]]
                         .groupby(level)
                         .first()
                         .itertuples()
                     ]
                 )
             )
             m = pandas.DataFrame(
```

### Comparing `sashimi_domains-0.9.3/src/limbo/corporalogy.py` & `sashimi_domains-0.9.4/src/limbo/corporalogy.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/src/limbo/graphology.py` & `sashimi_domains-0.9.4/src/limbo/graphology.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,15 +338,15 @@
     ######################
 
     def calc_nested_blockstate_mcmc(self, name_args=[]):
         for irun in count():
             fname = naming.gen(
                 "blockstate",
                 [("step", "aneq")] + name_args + [("run", irun)],
-                self.ext_nbs,
+                self.suffix_nbs,
             )
             try:
                 (self.graph_dir / fname).mkdir(exist_ok=False)
                 print("Reserving name: {}".format(fname))
                 break
             except OSError:
                 pass
```

### Comparing `sashimi_domains-0.9.3/src/sashimi/__init__.py` & `sashimi_domains-0.9.4/src/sashimi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 # Contributions are welcome, get in touch with the author(s).
 
 """
 See README.md for usage information.
 """
 
 __author__ = "Alexandre Hannud Abdo <abdo@member.fsf.org>"
-__copyright__ = "Copyright 2016-2023 Alexandre Hannud Abdo"
+__copyright__ = "Copyright 2016-2024 Alexandre Hannud Abdo"
 __license__ = "GNU GPL version 3 or above"
 __URL__ = "https://gitlab.com/solstag/sashimi/"
 
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 
 __all__ = ["Corpus", "GraphModels", "Vectorology"]
 
 import graph_tool  # to avoid import order issues with pandas # noqa
 
 #######################
 # Expose main classes #
```

### Comparing `sashimi_domains-0.9.3/src/sashimi/config.py` & `sashimi_domains-0.9.4/src/sashimi/config.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/src/sashimi/entropies.py` & `sashimi_domains-0.9.4/src/sashimi/entropies.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/src/sashimi/ioio.py` & `sashimi_domains-0.9.4/src/sashimi/ioio.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/src/sashimi/misc.py` & `sashimi_domains-0.9.4/src/sashimi/misc.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/src/sashimi/naming.py` & `sashimi_domains-0.9.4/src/sashimi/naming.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,14 @@
     @classmethod
     def check(cls, *args):
         forbidden = (cls.esc, path.sep, cls.itemsep, cls.valsep)
         if any(y in x for x in args for y in forbidden):
             raise ValueError
 
     @classmethod
-    def gen(cls, base, params, ext):
+    def gen(cls, base, params, suffix):
         params = [tuple(map(str, x)) for x in params]
-        cls.check(*chain(*params), ext)
+        cls.check(*chain(*params), suffix)
         base = cls.escape(base)
         params = (map(cls.escape, x) for x in params)
         name = cls.itemsep.join(chain([base], map(cls.valsep.join, params)))
-        return path.extsep.join([name, ext.lstrip(path.extsep)])
+        return path.extsep.join([name, suffix.lstrip(path.extsep)])
```

### Comparing `sashimi_domains-0.9.3/src/sashimi/scorology.py` & `sashimi_domains-0.9.4/src/sashimi/scorology.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/src/sashimi/vectorology.py` & `sashimi_domains-0.9.4/src/sashimi/vectorology.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/src/sashimi/w2v_score.py` & `sashimi_domains-0.9.4/src/sashimi/w2v_score.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/src/sashimi/blocks/#annotations.py#` & `sashimi_domains-0.9.4/src/sashimi/blocks/annotations.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,37 +7,43 @@
 # [GNU-GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html)
 #
 # Project:
 # <https://en.wikiversity.org/wiki/The_dynamics_and_social_organization_of
 #  _innovation_in_the_field_of_oncology>
 #
 # Reference repository for this file:
-# <https://gitlab.com/solstag/abstractology>
+# <https://gitlab.com/solstag/sashimi>
 #
 # Contributions are welcome, get in touch with the author(s).
 
+from __future__ import annotations
+import typing
+
 from heapq import nsmallest as heapq_nsmallest
 import html
 import random
 
 import pandas
 from tqdm import tqdm
 
 from ..naming import naming
 from ..ioio import ioio
 from ..entropies import make_nested_specificity, make_nested_commonality
 
+if typing.TYPE_CHECKING:
+    from ..graph_models import GraphModels
+
 
 ##############################
 # xblock yblocks annotations #
 ##############################
 
 
 def get_xblock_yblocks(
-    corpus, xbtype, xlevel, xb, ybtype, ylevel, num=None, anti=False
+    corpus: GraphModels, xbtype, xlevel, xb, ybtype, ylevel, num=None, anti=False
 ):
     """
     Returns
     =======
     [(yblock, yblock_entropy), ...]
     """
     hxb = corpus.level_block_to_hblock(xlevel, xb, xbtype)
@@ -51,15 +57,23 @@
     def sortkeyf(x):
         return -x[1]
 
     return nsmallest(num, ((x, nested_specificity(x)) for x in ybs), key=sortkeyf)
 
 
 def get_xblock_yblocks_elements(
-    corpus, xbtype, xlevel, xb, ybtype, ylevel, num=10, ent_frac=0.5, anti=False
+    corpus: GraphModels,
+    xbtype,
+    xlevel,
+    xb,
+    ybtype,
+    ylevel,
+    num=10,
+    ent_frac=0.5,
+    anti=False,
 ):
     """
     Given a domain block, returns a list containing, for each pertinent level 1 topic,
     a list of pertinent terms.
 
     After ordering topics by pointwise topic-level relative entropy, takes enough topics
     to account for half of the positive part of the topic-level relative entropy between
@@ -124,30 +138,30 @@
         "ent": (cum_ent, float(total_ent)),
         "blocks": yblocks_elements,
         "btypes": (xbtype, ybtype),
         "levels": (xlevel, ylevel),
     }
 
 
-def get_xblock_docs(corpus, xbtype, xlevel, xb, order="sample", n=10):
+def get_xblock_docs(corpus: GraphModels, xbtype, xlevel, xb, order="sample", n=10):
     xdc = corpus.get_xblock_yblocks_counts(xbtype, xlevel, xb, "doc", None)
     xdc = dict((k, v) for k, v in xdc.items() if v)
     docs = corpus.data.index.intersection(xdc).to_list()
     n = len(docs) if n is None else min(n, len(docs))
     if order == "sample":
         return random.sample(docs, n)
 
 
 ###############################
 # xblocks yblocks annotations #
 ###############################
 
 
 def get_xblocks_yblocks(
-    corpus, xbtype, xlevelblocks, ybtype, ylevel, n=None, ent_frac=0.5
+    corpus: GraphModels, xbtype, xlevelblocks, ybtype, ylevel, n=None, ent_frac=0.5
 ):
     yblocks = {}
     for xlevel, xb in xlevelblocks:
         xblock_yblocks = get_xblock_yblocks(corpus, xbtype, xlevel, xb, ybtype, ylevel)
         for k, v in xblock_yblocks:
             yblocks[k] = yblocks.setdefault(k, 0.0) + v
     return list(yield_values_fraction(yblocks.items(), ent_frac))
@@ -158,15 +172,15 @@
         xblock_yblocks = get_xblock_yblocks(corpus, xbtype, xlevel, xb, ybtype, ylevel)
         for k, v in yield_values_fraction(xblock_yblocks, ent_frac):
             yblocks[k] = yblocks.setdefault(k, 0.0) + v
     return list(yblocks.items())
 
 
 def get_yblocks_xblocks(
-    corpus, xbtype, xlevel, ybtype, ylevel, ybs, n=None, ent_frac=0.5
+    corpus: GraphModels, xbtype, xlevel, ybtype, ylevel, ybs, n=None, ent_frac=0.5
 ):
     ybs = set(ybs)
     xblocks = []
 
     for xb in tqdm(corpus.get_blocks_levels(xbtype)[0][xlevel].unique()):
         xb_yblocks = get_xblock_yblocks(corpus, xbtype, xlevel, xb, ybtype, ylevel)
         for _, ent_low in yield_values_fraction(xb_yblocks, ent_frac):
@@ -179,25 +193,25 @@
 
 #################################
 # subxblock yblocks annotations #
 #################################
 
 
 def get_subxblocks_yblocks(
-    corpus, xbtype, xlevel, xb, ybtype, ylevel, num=None, anti=False
+    corpus: GraphModels, xbtype, xlevel, xb, ybtype, ylevel, num=None, anti=False
 ):
     get_counts = make_get_counts(corpus, xbtype, ybtype, ylevel)
     hxb = corpus.level_block_to_hblock(xlevel, xb, xbtype)
     yb_counts, _ = get_counts(hxb)
     upx_yb_counts = [get_counts(hxb[:i]) for i in range(1, len(hxb))]
 
     if xlevel == 1:
         sxlevel = "v"
     else:
-        sxlevel = xlevel - 1  # = 1
+        sxlevel = corpus.get_sublevel(xlevel, xbtype)
 
     xblocks, _ = corpus.get_blocks_levels(xbtype)
     subxblocks = xblocks[xblocks[xlevel].eq(xb)].groupby(sxlevel)
     subx_yb_counts = []
     for subxb, group in subxblocks:
         hsubxb = corpus.level_block_to_hblock(sxlevel, subxb, xbtype)
         subx_yb_counts.append(get_counts(hsubxb))
@@ -210,15 +224,23 @@
     def sortkeyf(x):
         return -x[1]
 
     return nsmallest(num, yblocks, key=sortkeyf)
 
 
 def get_subxblocks_yblocks_elements(
-    corpus, xbtype, xlevel, xb, ybtype, ylevel, num=5, ent_frac=0.5, anti=False
+    corpus: GraphModels,
+    xbtype,
+    xlevel,
+    xb,
+    ybtype,
+    ylevel,
+    num=5,
+    ent_frac=0.5,
+    anti=False,
 ):
     xblocks, xlevels = corpus.get_blocks_levels(xbtype)
     yblocks, ylevels = corpus.get_blocks_levels(ybtype)
 
     get_counts = make_get_counts(corpus, xbtype, ybtype, None)
     hxb = corpus.level_block_to_hblock(xlevel, xb, xbtype)
     upx_y_counts = [get_counts(hxb[:i]) for i in range(1, len(hxb))]
@@ -226,15 +248,15 @@
     subxblocks_yblocks = get_subxblocks_yblocks(
         corpus, xbtype, xlevel, xb, ybtype, ylevel
     )
 
     if xlevel == 1:
         return {"ent": (0.0, 0.0), "blocks": {}}
     # sxlevel = 1 # too expensive
-    sxlevel = xlevel - 1
+    sxlevel = corpus.get_sublevel(xlevel, xbtype)
     subxblocks = xblocks[xblocks[xlevel].eq(xb)].groupby(sxlevel)
     subx_y_counts = []
     for subxb, group in subxblocks:
         hsubxb = corpus.level_block_to_hblock(sxlevel, subxb, xbtype)
         subx_y_counts.append(get_counts(hsubxb))
 
     yblocks_elements = {}
@@ -271,15 +293,15 @@
 
 ######################
 # xblock annotations #
 ######################
 
 
 def get_xblock_xelements(
-    corpus, xbtype, xlevel, xb, order, ybtype=None, num=None, sxblocks=None
+    corpus: GraphModels, xbtype, xlevel, xb, order, ybtype=None, num=None, sxblocks=None
 ):
     xblocks, _ = (
         corpus.get_blocks_levels(xbtype) if sxblocks is None else (sxblocks, None)
     )
     if ybtype:
         xelement_yelements = corpus.get_xelement_yelements(xbtype, ybtype)
     xelements = xblocks[xblocks[xlevel].eq(xb)]
@@ -324,15 +346,15 @@
 
 
 ########
 # misc #
 ########
 
 
-def make_get_counts(corpus, xbtype, ybtype, ylevel):
+def make_get_counts(corpus: GraphModels, xbtype, ybtype, ylevel):
     _, xlevels = corpus.get_blocks_levels(xbtype)
 
     def get_regular_counts(hxb):
         xlevel_, xb_ = corpus.hblock_to_level_block(hxb, xbtype)
         xyc = corpus.get_xblock_yblocks_counts(xbtype, xlevel_, xb_, ybtype, ylevel)
         return xyc, sum(xyc.values())
 
@@ -413,15 +435,15 @@
 def make_get_title(key_title, key_url=None, key_time=None):
     """
     `get_title(row)` used e.g. in `corpus.data.agg(get_title, axis=1)`.
     """
 
     def get_title(row):
         """
-        Returns a title for a row of data.
+        Returns an enriched title for a row of data.
         """
         # pandas bug: .agg(get_title) → if access row[_] → result df not series
         if row.empty:
             return None
 
         title = html.escape(str(row[key_title]))
         if key_time:
@@ -445,54 +467,93 @@
 
 #########
 # cache #
 #########
 
 
 def load_annotations(
-    corpus, annotation_function, xbtype, ybtype, ylevel=1, num=5, ent_frac=0.5
+    corpus: GraphModels,
+    annotation_function,
+    xbtype,
+    ybtype,
+    ylevel=1,
+    num=5,
+    ent_frac=0.5,
 ):
+    btypes = {"xbtype": xbtype, "ybtype": ybtype}
     use_cache = corpus.use_cached_annotations
-    use_cache_sample = corpus.use_cached_annotations_sampled
+    sample_hash = corpus.get_sample_hash(
+        **{x: x in btypes.values() for x in ["doc", "ter", "ext"]}
+    )
+    fdir = corpus.chained_dir if "ext" in btypes.values() else corpus.blocks_dir
+    use_sample = corpus.use_sampled_annotations or f"sample={sample_hash};" in fdir.stem
     if use_cache:
-        if all(t in ("doc", "ter") for t in (xbtype, ybtype)):
-            fdir = corpus.blocks_dir
-        else:
-            fdir = corpus.chained_dir
         fname_params = (
-            ("xbtype", xbtype),
-            ("ybtype", ybtype),
+            *btypes.items(),
             ("ylevel", ylevel),
             ("num", num),
             ("ent_frac", ent_frac),
         )
-        sample_hash = corpus.get_sample_hash(
-                **{x: x in {xbtype, ybtype} for x in ["doc", "ter", "ext"]}
-        ) if use_cache_sample else None
-        if sample_hash := :
-                fname_params = [("sample", sample_hash), *fname_params]
+        if use_sample and sample_hash:
+            fname_params = [("sample", sample_hash), *fname_params]
         fpath = (
             fdir
             / "cache"
             / naming.gen(
                 annotation_function.__name__,
                 fname_params,
                 ".pickle.xz",
             )
         )
         if fpath.exists():
-            print(f"Loading cached {'sampled' if sample_hash else ''} annotations!")
+            print(
+                f"Loading cached "
+                f"{'sampled ' if (use_sample and sample_hash) else ''}"
+                f"annotations: {fpath}"
+            )
             return ioio.load(fpath)
 
+    if not use_sample and sample_hash:
+        raise ValueError("No cached unsampled annotations found!")
     annotations = {}
     xblocks, xlevels = corpus.get_blocks_levels(xbtype)
     for xlevel in tqdm(xlevels):
         annotations[xlevel] = {}
         for xb in tqdm(xblocks[xlevel].unique()):
             annotations[xlevel][xb] = annotation_function(
                 corpus, xbtype, xlevel, xb, ybtype, ylevel, num, ent_frac
             )
 
     if use_cache:
         ioio.store(annotations, fpath)
 
     return annotations
+
+
+def make_get_annotations(corpus: GraphModels):
+    """
+    By using this function one can cache results in-place like
+    `annotations = cache(make_get_annotations(corpus))`
+    """
+
+    def get_annotations(xbtype, xlevel, ybtype, ylevel, edges, **kwargs):
+        """
+        Usage:
+        ```
+        annotations = get_annotations("doc", 2, "ter", 1, "specific")
+        annotations[xb]["blocks"][yb]["elements"]` -> [(element, relent), ...]
+        ```
+        """
+        if edges == "specific":
+            annotation_function = get_xblock_yblocks_elements
+        elif edges == "common" and xlevel > 1:
+            annotation_function = get_subxblocks_yblocks_elements
+        elif edges == "common" and xlevel == 1:
+            raise ValueError('`edges="common"` requires xlevel > 1')
+        else:
+            raise ValueError("`edges` must be one of ['specific', 'common']")
+        annotations = load_annotations(
+            corpus, annotation_function, xbtype, ybtype, ylevel, **kwargs
+        )[xlevel]
+        return annotations
+
+    return get_annotations
```

### Comparing `sashimi_domains-0.9.3/src/sashimi/blocks/__init__.py` & `sashimi_domains-0.9.4/src/sashimi/blocks/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from collections import Counter
 from functools import cache
 
 import pandas as pd
 
 from ..corpus import Corpus
+from ..graph_models import blockstate_to_dataframes
 from .hierarchical_block_map import composite_hierarchical_block_map
 from . import zmethods
 from .tables import subxblocks_report, xblocks_report
 from .network_map import network_map
 
 
 class Blocks:
@@ -34,101 +35,121 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         if self.col_title is None:
             print("Warning: `col_title` is not set")
 
-    def get_blocks_levels(self, btype=None):
+    @property
+    def dblocks_levels(self):
+        return [x for x in self.dblocks if isinstance(x, int)]
+
+    @property
+    def tblocks_levels(self):
+        return [x for x in self.tblocks if isinstance(x, int)]
+
+    @property
+    def eblocks_levels(self):
+        return [x for x in self.eblocks if isinstance(x, int)]
+
+    def get_blocks_levels(self, btype=None, *, orig=False) -> tuple[pd.DataFrame, list]:
         """
         Parameters
         ----------
         btype: the type of block to return ('doc', 'ter' or 'ext')
 
         Returns
         -------
         blocks: the original blocks
         levels: the levels
         """
+        bprefix = "_orig_" if orig else ""
         if btype is None:
             return {
-                "doc": (self.dblocks, self.dblocks_levels),
-                "ter": (self.tblocks, self.tblocks_levels),
-                "ext": (self.eblocks, self.eblocks_levels),
+                "doc": (
+                    getattr(self, f"{bprefix}dblocks", self.dblocks),
+                    self.dblocks_levels,
+                ),
+                "ter": (
+                    getattr(self, f"{bprefix}tblocks", self.tblocks),
+                    self.tblocks_levels,
+                ),
+                "ext": (
+                    getattr(self, f"{bprefix}eblocks", self.eblocks),
+                    self.eblocks_levels,
+                ),
             }
         elif btype == "doc":
-            return self.dblocks, self.dblocks_levels
+            return getattr(self, f"{bprefix}dblocks", self.dblocks), self.dblocks_levels
         elif btype == "ter":
-            return self.tblocks, self.tblocks_levels
+            return getattr(self, f"{bprefix}tblocks", self.tblocks), self.tblocks_levels
         elif btype == "ext":
-            return self.eblocks, self.eblocks_levels
+            return getattr(self, f"{bprefix}eblocks", self.eblocks), self.eblocks_levels
         else:
             raise ValueError("Unrecognized `btype`.")
 
-    def get_blocks_levels_sample(self, btype):
-        """
-        If data is sampled, we need to sample the corresponding entries
-        from the blocks as well.
-
-        Parameters
-        ----------
-        btype: the type of block to return ('doc', 'ter' or 'ext')
-
-        Returns
-        -------
-        blocks: the original blocks
-        levels: the levels
-        sblocks: the blocks restricted to the data sample
-        """
-        blocks, levels = self.get_blocks_levels(btype)
-        if btype == "doc":
-            sblocks = self.dblocks.loc[self.data.index]
-        elif btype == "ter":
-            sblocks = self.tblocks.loc[
-                self.tblocks.index.intersection(self.get_vocab())
-            ]
-        elif btype == "ext":
-            sblocks = blocks  # TODO actually sample eblocks
-        return blocks, levels, sblocks
-
     def hblock_to_level_block(self, hb, btype):
-        _, levels = self.get_blocks_levels(btype)
-        level = len(levels) - len(hb) + 1
-        return ("v" if level == 0 else level), hb[-1]
+        blocks, levels = self.get_blocks_levels(btype)
+        levels = ["v", *levels]
+        level, block = levels[-len(hb)], hb[-1]
+        true_hb = self.level_block_to_hblock(level, block, btype)
+        if hb == true_hb:
+            return level, block
+        else:
+            raise ValueError(f"False hblock: {hb}")
 
     def level_block_to_hblock(self, level, block, btype):
         blocks, levels = self.get_blocks_levels(btype)
         if level == "v":
-            levels = levels.copy()
-            levels.insert(0, "v")
+            levels = ["v", *levels]
         b = blocks.loc[blocks[level].eq(block), levels[levels.index(level) :]]
         return tuple(reversed(b.iloc[0].tolist()))
 
+    def get_sublevel(self, level, btype):
+        _, levels = self.get_blocks_levels(btype)
+        return levels[levels.index(level) - 1]
+
     def domain_labels_to_selection(self, labels):
         level_blocks = {}
         for label in labels:
-            for level, block in [
-                self.hblock_to_level_block(self.label_to_hblock[label], "doc")
-            ]:
-                level_blocks.setdefault(level, []).append(block)
+            _, level, block = self.label_to_tlblock[label]
+            level_blocks.setdefault(level, []).append(block)
         sel = pd.Series(False, self.data.index)
         for level, blocks in level_blocks.items():
             sel |= self.dblocks[level].isin(blocks)
         return sel
 
-    def set_sample(self, sample, keep=False):
+    def set_sample(self, sample, keep=False, trim=True):
         Corpus.set_sample(self, sample=sample, keep=keep)
-        if hasattr(self, "dblocks"):
-            if not hasattr(self, "_orig_dblocks"):
-                self._orig_dblocks = self.dblocks
-            if keep:
-                self.dblocks = self.dblocks.loc[self.data.index]
-            else:
-                self.dblocks = self._orig_dblocks.loc[self.data.index]
-            self.gen_mapindex()
+        if trim:
+            self.trim_to_sample()
+
+    def trim_to_sample(self):
+        self.cache_clear(clear_static=True)
+        if not hasattr(self, "dblocks"):
+            return
+        if not hasattr(self, "_orig_dblocks"):
+            self._orig_dblocks = self.dblocks.copy()
+        self.dblocks = self._orig_dblocks.loc[self.data.index].copy()
+        if hasattr(self, "tblocks") and not self.tblocks.empty:
+            self.load_ter_documents()
+            if not hasattr(self, "_orig_tblocks"):
+                self._orig_tblocks = self.tblocks.copy()
+            self.tblocks = self._orig_tblocks[
+                self._orig_tblocks.index.isin(self.ter_documents)
+            ].copy()
+        if hasattr(self, "eblocks") and not self.eblocks.empty:
+            self.load_ext_documents()
+            if not hasattr(self, "_orig_eblocks"):
+                self._orig_eblocks = self.eblocks.copy()
+            self.eblocks = self._orig_eblocks[
+                self._orig_eblocks.index.isin(self.ext_documents)
+            ].copy()
+        blockstate_to_dataframes.remove_redundant_levels(self)
+        blockstate_to_dataframes.gen_mapindex(self)
 
     def find_blocks(self, lscape, finder):
         """
         Returns the blocks that correspond to features defined in finder.
         For example, blocks with the highest or lowest values, or with
         the highest or lowest differences in values across the landscape.
 
@@ -302,15 +323,21 @@
             antixlevel_xblock_containing_xb = xblocks.loc[~xsel, antixlevel].iloc[0]
             antixsel = xblocks[antixlevel].eq(antixlevel_xblock_containing_xb)
             xsel = xsel & antixsel
         return xsel
 
     @cache
     def get_antixblock_yblocks_counts(
-            self, xbtype, xlevel, xb, antixlevel=None, ybtype="ter", ylevel=1,
+        self,
+        xbtype,
+        xlevel,
+        xb,
+        antixlevel=None,
+        ybtype="ter",
+        ylevel=1,
     ):
         xsel = self.get_antixblock_sel(xbtype, xlevel, xb, antixlevel)
         return self.get_xsel_yblocks_counts(xbtype, xsel, ybtype, ylevel)
 
     def get_xblock_yblocks_stat(
         self, stat, xbtype, xlevel, xb, ybtype, ylevel, ybs=None
     ):
```

### Comparing `sashimi_domains-0.9.3/src/sashimi/blocks/area_rank_chart.py` & `sashimi_domains-0.9.4/src/sashimi/blocks/area_rank_chart.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,69 +1,93 @@
 import math
 from numpy import linspace, cos, pi
 
-import colorcet as cc
+import colorcet
 import bokeh.models as bkm
 from bokeh.io import output_file, show
 from bokeh.layouts import row, column  # , Spacer
 from bokeh.models import ColumnDataSource
 from bokeh.plotting import figure
 import pandas as pd
 
-from .reports import get_subxblocks, get_labels
+from .tables import get_subxblocks, get_labels
 
 
 ################
 # Domain plots #
 ################
 
 
-def subdomain_graphics(corpus, xlevel, xb, sxlevel=None, outfile="evoplot.html"):
+def domain_charts(corpus, domain_labels, outfile="evoplot.html"):
+    fig = build_graphics(
+        corpus,
+        [
+            corpus.level_block_to_hblock(level, block, btype)
+            for dlabel in domain_labels
+            for btype, level, block in [corpus.label_to_tlblock(dlabel)]
+        ],
+    )
+    if outfile is None:
+        return fig
+    output_file(outfile)
+    show(fig)
+
+
+def subdomain_charts(corpus, xlevel, xb, sxlevel=None, outfile="evoplot.html"):
     layout = column(
         build_graphics(corpus, [corpus.level_block_to_hblock(xlevel, xb, "doc")]),
         build_graphics(
             corpus, get_subxblocks(corpus, "doc", xlevel, xb, sxlevel=sxlevel)
         ),
         # rank_graphics(),
     )
+    if outfile is None:
+        return layout
     output_file(outfile)
     show(layout)
 
 
 def build_graphics(corpus, dhblocks):
     """
-    Graphic showing the comparative evolution of domains.
+    Stacked charts showing the comparative evolution of domains.
     """
-    dhlevels = [corpus.hblock_to_level_block(dhb, "doc")[0] for dhb in dhblocks]
+    x = sorted(corpus.data[corpus.col_time].unique())
+
+    def get_sizes(level_block):
+        level, block = level_block
+        return (
+            corpus.data[corpus.dblocks[level] == block]
+            .groupby(corpus.col_time)
+            .size()
+            .reindex(x)
+            .fillna(0)
+        )
+
+    dlevels = [corpus.hblock_to_level_block(dhb, "doc")[0] for dhb in dhblocks]
     labels = get_labels(corpus)
 
-    cats_data = list(reversed(list(zip(dhblocks, dhlevels))))
+    cats_data = list(reversed(list(zip(dhblocks, dlevels))))
+    cats_data = sorted(
+        cats_data, key=lambda x: get_sizes((x[1], x[0][-1])).sum(), reverse=True
+    )
     cats = [corpus.lblock_to_label[level, dhb[-1]] for dhb, level in cats_data]
     cats = [f"{x}: {labels.get(x, '[no label]')}" for x in cats]
 
-    x = sorted(corpus.data[corpus.col_time].unique())
-
-    palette = cc.rainbow[:: (len(cc.rainbow) - 1) // len(cats) + 1]
-
-    in_size = sum(
-        corpus.data[corpus.dblocks[level] == dhb[-1]]
-        .groupby(corpus.col_time)
-        .size()
-        .reindex(x)
-        .fillna(0)
-        for (dhb, level) in cats_data
-    )
     out_size = corpus.data.groupby(corpus.col_time).size().reindex(x)
+    in_size = sum(get_sizes((level, dhb[-1])) for (dhb, level) in cats_data).astype(int)
+    has_in_size = not out_size.equals(in_size)
+
+    palette = colorcet.glasbey_dark[1 : 1 + len(cats_data)]
 
     def make_plot(norm, scale, title, labels):
         p = figure(
             title=title,
             y_range=cats + [""],
-            frame_width=450,
-            plot_height=900,
+            width=1920 // (3 if has_in_size else 2),
+            height=1080,
             x_range=(min(x), max(x)),
             toolbar_location=None,
             tools="",
         )
 
         def ridge(category, data):
             return [(category, dat * scale * len(dhblocks) / 2) for dat in data]
@@ -88,15 +112,15 @@
             source.add(norm, "norm")
 
             p.varea(
                 x="x",
                 y1=f"{cat}_zero",
                 y2=cat,
                 color=palette[i],
-                alpha=0.6,
+                alpha=0.5,
                 source=source,
             )
             line = p.line(
                 x="x",
                 y=cat,
                 color="black",
                 source=source,
@@ -123,35 +147,38 @@
             p.yaxis.major_label_text_font_size = "0px"
 
         return p
 
     layout = row(
         make_plot(pd.Series(1, index=x), 1 / in_size.mean(), "Absolute", True),
         make_plot(out_size, out_size.sum() / in_size.sum(), "Corpus relative", False),
-        make_plot(in_size, 1, "Ensemble relative", False),
         align="end",
     )
+    if has_in_size:
+        layout.append(make_plot(in_size, 1, "Ensemble relative", False))
 
     return layout
 
 
 ###################
 # Area rank chart #
 ###################
 
 
-def area_rank_chart(corpus, selector, grouper, averager, level, labels=None, rel=True):
+def area_rank_chart(
+    corpus, selector, grouper, averager, level, labels=None, rel=True, outfile=None
+):
     """
-    Restricts corpus to a `.loc` selector
-    then group by grouper and block level
-    get the group's sizes
-    then average on averager (e.g. grouper is period, averager is year).
+    Plots an area rank chart of domains, with the grouper dimension on the
+    x-axis and domain sizes on the y-axis.
 
-    Finally, plots an area bump chart of domains with size on y-axis
-    and the grouper's dimension on the x-axis.
+    Restricts corpus to given selector, then group by grouper and by blocks of
+    the given level. Get the group's sizes, then average on averager. For
+    example, if grouper corresponds to periods with variable number of years,
+    then averager should be the year, so that larger periods aren't inflated.
     """
     if labels is None:
         labels = get_labels(corpus)
 
     def get_label(b):
         label = corpus.lblock_to_label[level, b]
         return f"{label}: {labels.get(label, '[no label]')}"
@@ -170,53 +197,56 @@
     for y_abs_o in y_abs[1:]:
         y_range = y_range.union(y_abs_o.index)
     msize_abs = max(yi.max() for yi in y_abs)
     if rel:
         y_rel = [x / x.sum() for x in y_abs]
         msize_rel = max(yi.max() for yi in y_rel)
     points_in_unit_width = 900 // len(y_abs)
-    p = figure(
+    fig = figure(
         # title=title,
-        frame_width=900,
-        frame_height=900,
+        width=1920,
+        height=1080,
         x_range=(0, len(y_abs) - 1),
         x_axis_location="above",
         y_range=(len(y_range), 0),
         toolbar_location="above",
         # tools="",
     )
-    p.axis.major_label_text_font_size = "17px"
-    p.xaxis.minor_tick_line_color = None
-    p.xaxis.major_label_orientation = math.pi / 4
-    p.xaxis.ticker = list(range(len(y_counts.index.levels[0])))
-    p.xaxis.major_label_overrides = {
+    fig.axis.major_label_text_font_size = "17px"
+    fig.xaxis.minor_tick_line_color = None
+    fig.xaxis.major_label_orientation = math.pi / 4
+    fig.xaxis.ticker = list(range(len(y_counts.index.levels[0])))
+    fig.xaxis.major_label_overrides = {
         i: str(j) for i, j in enumerate(y_counts.index.levels[0])
     }
-    p.ygrid.visible = False
-    p.yaxis.ticker = yticker = [i + 1 / 2 for i in range(len(y_abs[0]))]
-    p.yaxis.major_label_overrides = {
+    fig.ygrid.visible = False
+    fig.yaxis.ticker = yticker = [i + 1 / 2 for i in range(len(y_abs[0]))]
+    fig.yaxis.major_label_overrides = {
         i: str(j) for i, j in zip(yticker, y_abs[0].index.map(get_label))
     }
 
     # add end ticks and labels
     ryaxis = bkm.LinearAxis(ticker=bkm.FixedTicker())
-    p.add_layout(ryaxis, "right")
+    fig.add_layout(ryaxis, "right")
     ryaxis.major_label_text_font_size = "17px"
     ryaxis.ticker = ryticker = [i + 1 / 2 for i in range(len(y_abs[-1]))]
     ryaxis.major_label_overrides = {
         i: str(j) for i, j in zip(ryticker, y_abs[-1].index.map(get_label))
     }
 
-    palette = pd.Series(cc.glasbey[: len(y_range)], index=y_range)
+    palette = pd.Series(colorcet.glasbey[: len(y_range)], index=y_range)
 
-    plot_connections(p, y_abs, msize_abs, "solid", palette, points_in_unit_width)
+    plot_connections(fig, y_abs, msize_abs, "solid", palette, points_in_unit_width)
     if rel:
-        plot_connections(p, y_rel, msize_rel, "dotted", palette, points_in_unit_width)
+        plot_connections(fig, y_rel, msize_rel, "dotted", palette, points_in_unit_width)
 
-    return p
+    if outfile is None:
+        return fig
+    output_file(outfile)
+    show(fig)
 
 
 def plot_connections(fig, y_data, msize_data, line_dash, palette, points_in_unit_width):
     def plot():
         fig.varea(xs, y0s, y1s, color=palette[idx], alpha=0.5)
         fig.line(xs, y0s, color="black", line_dash=line_dash)
         fig.line(xs, y1s, color="black", line_dash=line_dash)
@@ -266,19 +296,7 @@
         return s0 * (1 - x) + s1 * x
 
     xs = linspace(start, start + length, int(abs(length) * points_in_unit_width))
     nxs = linspace(0, 1, int(abs(length) * points_in_unit_width))
     y0s = [connect(x) - spread(x) / 2 for x in nxs]
     y1s = [connect(x) + spread(x) / 2 for x in nxs]
     return xs, y0s, y1s
-
-
-##########
-# Unused #
-##########
-
-
-def block_diff_level(block0, block1, levels):
-    for i, (b1, b2) in enumerate(zip(block0, block1)):
-        if b1 != b2:
-            return len(levels) - i
-    return len(levels) - i - 1
```

### Comparing `sashimi_domains-0.9.3/src/sashimi/blocks/block_ext_map.py` & `sashimi_domains-0.9.4/src/sashimi/blocks/block_ext_map.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/src/sashimi/blocks/hierarchical_block_map.py` & `sashimi_domains-0.9.4/src/sashimi/blocks/hierarchical_block_map.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,27 +19,35 @@
 
 import colorcet
 import numpy as np
 import pandas
 from tqdm import tqdm
 
 # bokeh
-from bokeh import plotting as bkp, models as bkm, layouts as bkl, events as bke
+from bokeh import (
+    plotting as bkp,
+    models as bkm,
+    layouts as bkl,
+    events as bke,
+    io as bio,
+)
 from bokeh.models.callbacks import CustomJS
 from bokeh.transform import transform
 from bokeh.models.transforms import CustomJSTransform
 from bokeh.models.formatters import DatetimeTickFormatter
 
 from ..naming import naming
 from . import zmethods
 from .util import (
     sorted_hierarchical_block_index,
-    try_datetime,
-    try_period_get_range,
+    try_time_index,
+    is_time_type,
     make_normalization_factor,
+    btype_to_name,
+    phi,
 )
 from .annotations import (
     load_annotations,
     get_xblock_xelements,
     get_xblock_docs,
     get_xblock_yblocks_elements,
     get_subxblocks_yblocks_elements,
@@ -53,33 +61,26 @@
 def composite_hierarchical_block_map(
     corpus,
     btype,
     zmethod=None,
     norm=None,
     scale="linear",
     bheight="hierarchical",
-    annotate=True,
     link_p_func=None,
     page_title=None,
+    disable_features={},
 ):
     """
-    Colormap to display aggregates at different levels.
-    Colors can represent, for example, journals/authors/institutions
-    within, or crossing, blocks at that given level.
-
-    Colors are taken from the z axis, which is calculated from
-    'zmethod', a member of the abstract Zmethod class. See the
-    documentation for that class for more information and to define
-    your own functions.
-
-    When sampling the data with 'set_sample()':
-    * the block structure is not affected
-    * displayed value, color, terms and titles are affected
-    * when calling 'zmethod', 'blocks' is affected but 'index' is not
-    * displayed count shows both sample and total as a fraction
+    Colormap to display multimodal aggregates at different levels.
+    Elements are documents and terms, but also journals, authors, institutions, years.
+    Colors can represent volume within or connections between different agregates.
+
+    Colors reflect the z axis, which is calculated from 'zmethod', a member of the
+    abstract Zmethod class. See the documentation for that class for more information
+    and to define your own functions.
 
     You may pass a list of two or more btypes, in this case multiple
     colormaps will be displayed using the options given. Options that
     are also lists will then be applied to the corresponing map.
     """
 
     def as_list(arg):
@@ -89,17 +90,18 @@
     btype = [btype] if isinstance(btype, str) else btype
     maps_args = [
         {
             "zmethod": zmethods.count if (x := as_list(zmethod)[i]) is None else x,
             "norm": as_list(norm)[i],
             "scale": as_list(scale)[i],
             "bheight": as_list(bheight)[i],
-            "annotate": as_list(annotate)[i],
+            "annotate": as_list("annotations" not in disable_features)[i],
+            "other_btype": next(o_btype for o_btype in btype if o_btype != i_btype),
         }
-        for i in range(len(btype))
+        for i, i_btype in enumerate(btype)
     ]
     zname = [map_args["zmethod"].__name__ for map_args in maps_args]
 
     if page_title is None:
         page_title = f'{"|".join(corpus.loaded["data"])}: {len(corpus.data)} documents'
 
     name_args = "norm", "scale", "bheight"
@@ -124,70 +126,94 @@
         }
     )
     for map_args in maps_args:
         map_args["document_data"] = document_data
 
     # Produce the hierarchical_block_map for each individual set of parameters
     corpus.cache_clear()
-    figs, cbars, infos, nav_buttons = zip(
+    figs, cbars, nav_buttons, infos = zip(
         *(
             get_hierarchical_block_map(corpus, btype[i], **maps_args[i])
             for i in range(len(btype))
         )
     )
 
     # Lay out the Bokeh document and save it to disk
-    figlabels = {"doc": "Domain", "ter": "Topic", "ext": "Chained"}
     map_layouts = []
-    selection_mode = bkm.Select(
-        value="single",
-        options=["single", "multi AND", "multi OR"],
-        align="center",
-    )
-    doc_fig = figs[btype.index("doc")] if "doc" in btype else None
-    for i_btype, i_fig, i_bar, i_nav_buttons in zip(btype, figs, cbars, nav_buttons):
-        map_row_0 = bkl.row(
+    info_layouts = []
+    for i, (i_btype, i_fig, i_bar, i_nav_buttons, i_info) in enumerate(
+        zip(btype, figs, cbars, nav_buttons, infos)
+    ):
+        map_row = bkl.row(
             i_fig,
             bkl.column(i_nav_buttons, i_bar, sizing_mode="stretch_height"),
-            sizing_mode="stretch_width",
+            sizing_mode="stretch_both",
         )
-        if i_btype == "doc":
+        map_layouts.append(map_row)
+        info_column = []
+        if i_btype == "doc" and "doc_histogram" not in disable_features:
+            print("Building doc histogram")
             try:
-                map_row_1 = bkl.row(
-                    get_doc_histogram(corpus, i_fig),
-                    bkl.Spacer(width=90),
-                    sizing_mode="stretch_width",
+                info_column.append(
+                    get_doc_histogram(get_doc_histogram_data(corpus), i_fig),
                 )
             except Exception as e:
-                print(f"Failed to build doc histogram: {e}")
-                map_row_1 = bkl.row(sizing_mode="stretch_width")
-        if i_btype != "doc":
-            map_row_1 = bkl.row(
-                bkl.Spacer(width=23),
-                get_search_widget(corpus, i_btype, i_fig, doc_fig, selection_mode),
-                bkl.Spacer(width=90),
-                sizing_mode="stretch_width",
-            )
-        map_layouts.append(
-            bkl.column(
-                map_row_0,
-                map_row_1,
-                sizing_mode="stretch_width",
-            )
+                print(f"Failed to build doc histogram: {repr(e)}")
+        if i_btype == "doc" and "multi_histogram" not in disable_features:
+            print("Building multi histogram")
+            try:
+                info_column.append(
+                    get_multi_histogram(
+                        get_multi_histogram_data(
+                            corpus,
+                            maps_args[i]["other_btype"],
+                        ),
+                        i_fig,
+                    ),
+                )
+            except Exception as e:
+                print(f"Failed to build term histogram: {repr(e)}")
+        info_column.append(bkm.ScrollBox(child=i_info, sizing_mode="stretch_both"))
+        info_vbox_rows = {1: ["100%"], 2: ["20%", "80%"], 3: ["19%", "21%", "60%"]}[
+            len(info_column)
+        ]
+        info_vbox = bkm.VBox(
+            children=info_column, rows=info_vbox_rows, sizing_mode="stretch_both"
         )
+        info_layouts.append(info_vbox)
 
-    help = bkm.Div(
-        text=(
-            '<div style="width:49lvw; max-height:92lvh; overflow:auto;">'
-            + Path(__file__).with_name("hierarchical_block_map_help.html").read_text()
-            + "</div>"
+    help_div = bkm.Div(
+        text=(Path(__file__).with_name("hierarchical_block_map_help.html").read_text()),
+        sizing_mode="stretch_both",
+    )
+
+    selection_mode = bkm.Select(
+        value="single",
+        options=["single", "multi AND", "multi OR"],
+        align="center",
+    )
+    if "search" not in disable_features:
+        doc_fig = figs[btype.index("doc")] if "doc" in btype else None
+        print("Building the search box")
+        search_widget = get_search_widget(
+            corpus, i_btype, i_fig, doc_fig, selection_mode
         )
+    else:
+        search_widget = bkl.Spacer()
+    search_row = bkm.HBox(
+        children=[
+            bkl.Spacer(),
+            search_widget,
+            bkl.Spacer(),
+        ],
+        cols=["25%", "50%", "25%"],
+        sizing_mode="stretch_width",
     )
 
-    if len(btype) in (1, 2):
+    if len(btype) in (1, 2) and "link_maps" not in disable_features:
         # link figures
         if btype in (["doc", "ter"], ["doc", "ext"]):
             map_d = ["doc", figs[0], corpus.dblocks, corpus.dblocks_levels]
             if btype[1] == "ter":
                 map_x = ["ter", figs[1], corpus.tblocks, corpus.tblocks_levels]
                 values_x = zmethods.get_cross_counts(corpus, "ter", "link")
             if btype[1] == "ext":
@@ -198,97 +224,105 @@
                     corpus,
                     *map_s,
                     *map_t,
                     values=values_x,
                     selection_mode=selection_mode,
                     pfunc=link_p_func,
                 )
+    figlabels = {"doc": "Domain", "ter": "Topic", "ext": "Chained"}
+    if len(btype) in (1, 2):
         # two column single row layout
         mapinfo_row = [
             bkm.Tabs(
-                sizing_mode="stretch_width",
+                sizing_mode="stretch_both",
                 tabs=[
                     bkm.TabPanel(
-                        child=map_layouts[i], title="{} map".format(figlabels[btype[i]])
+                        child=map_layouts[i],
+                        title="{} map".format(figlabels[btype[i]]),
                     ),
                     bkm.TabPanel(
-                        child=infos[j], title="{} info".format(figlabels[btype[j]])
+                        child=info_layouts[j],
+                        title="{} info".format(figlabels[btype[j]]),
                     ),
                     bkm.TabPanel(
-                        child=help,
+                        child=bkm.ScrollBox(child=help_div, sizing_mode="stretch_both"),
                         title="Help",
                     ),
                 ],
             )
             for i, j in (([0, 1], [1, 0]) if len(btype) == 2 else ([0, 0],))
         ]
-        layout = [
+        layout_col = [
+            search_row,
             mapinfo_row,
         ]
     else:
         # multicolumn two rows layout
         map_row = [
             bkm.TabPanel(child=i_figcol, title="{} map".format(figlabels[i_btype]))
             for i_btype, i_figcol in zip(btype, map_layouts)
         ]
         info_row = [
             bkm.TabPanel(child=i_info, title="{} info".format(figlabels[i_btype]))
-            for i_btype, i_info in zip(btype, infos)
+            for i_btype, i_info in zip(btype, info_layouts)
         ]
-        layout = [map_row, info_row, help]
+        layout_col = [search_row, map_row, info_row, help_div]
 
     fdir = corpus.chained_adir if "ext" in btype else corpus.blocks_adir
-    bkp.output_file(fdir / fname, title=page_title, mode="inline")
-    return bkp.save(bkl.layout(layout, sizing_mode="stretch_width"))
+    bokehjs = dict(mode="inline")
+    bkp.output_file(fdir / fname, title=page_title, **bokehjs)
+
+    return bkp.save(bkl.layout(layout_col, sizing_mode="stretch_both"))
 
 
 def get_hierarchical_block_map(
     corpus,
     btype,
     zmethod,
     norm=None,
     scale="linear",
     bheight="hierarchical",
     annotate=True,
     document_data=None,
+    other_btype=None,
 ):
     """
     This method returns a bokeh.figure and other objects to be further processed.
     """
-    blocks, levels, sblocks = corpus.get_blocks_levels_sample(btype)
+    blocks, levels = corpus.get_blocks_levels(btype)
     lscape = get_block_level_landscape(corpus, btype, zmethod)
 
     source = dict(
         (k, [])
         for k in (
             "label",  # block label to display
-            "x",  # horizontal position of center (the block's level)
+            "level",  # the block's level
+            "x",  # horizontal position of center
             "y",  # vertical position of center
             "height",  # heigth of block
             "z",  # colorscale position of block
             "o_z",  # original colorscale position of block
             "value",  # value to be scaled/normalized into z
             "o_value",  # original value to be scaled/normalized into z
             "doc_terms",  # if 'doc': a list of terms
             "doc_exts",  # if 'doc': a list of elements
             "xb_elements",  # if not 'doc': elements and their occurrences
             "documents",  # list of integers representing document for block
-            "line_width",  # borders must shrink on lower levels
             "count",  # number of elements in block
-            "scount",  # number of elements in block accounting for sampling
         )
     )
     b2h = {(): 1}  # maps hblock to height, used when bheight=="hierarchical"
     color_p = get_color_params(btype)
 
-    # Load annotations for "doc" xbtype
-    annotations = get_hbm_annotations(corpus, btype) if annotate else {}
+    # Load document annotations
+    if annotate:
+        doc_annotations = get_doc_annotations(corpus) if btype == "doc" else None
 
     for level in tqdm(
-        reversed(levels[:]), total=len(levels), desc=f"{btype.capitalize()} level"
+        reversed(levels), total=len(levels), desc=f"{btype.capitalize()} level"
     ):
         # level total height
         if bheight == "procount":
             h_sum = len(blocks[level])
         elif bheight == "proval":
             h_sum = lscape[level].sum()
         else:
@@ -296,18 +330,17 @@
         h_cum = 0
 
         # level nomalization factor
         lscape_scaled = lscape[level].apply(np.log) if scale == "log" else lscape[level]
         znorm = make_normalization_factor(norm)(lscape_scaled)
 
         hxbindex = sorted_hierarchical_block_index(blocks, levels, level)
-        for hxb in tqdm(hxbindex, desc=f" L{level}{btype[0].upper()} block"):
+        for hxb in tqdm(hxbindex, desc=f" L{level}{btype[0].upper()} blocks"):
             xb = hxb[-1]
             count = (blocks[level] == xb).sum()
-            scount = (sblocks[level] == xb).sum()
             val = lscape[level].loc[xb]
             if np.isnan(val):  # happens in some 0/0 cases so put 1
                 val = 1
             zval = (
                 np.log(val) / znorm if scale == "log" else val / znorm
             )  # scale and normalize val
 
@@ -316,72 +349,83 @@
                 h_block = count / h_sum
             elif bheight == "proval":
                 h_block = val / h_sum
             elif bheight == "hierarchical":
                 num_same_parent = (
                     1
                     if len(hxb) == 1
-                    else blocks.loc[blocks[level + 1].eq(hxb[-2]), level].unique().size
+                    else blocks.loc[
+                        blocks[levels[levels.index(level) + 1]].eq(hxb[-2]), level
+                    ]
+                    .unique()
+                    .size
                 )
                 h_block = b2h[hxb[:-1]] / num_same_parent
                 b2h[hxb] = h_block
 
             # data for this block
-            source["x"].append(level)
+            source["level"].append(level)
+            source["x"].append(levels.index(level) + 1)
             source["y"].append(h_cum + h_block / 2)
             source["height"].append(h_block)
-            source["label"].append(f"{corpus.lblock_to_label[level, xb]} {hxb}")
+            source["label"].append(f"{corpus.lblock_to_label[level, xb]}")
             source["count"].append(count)
-            source["scount"].append(scount)
             source["value"].append(val)
             source["z"].append(zval)
             h_cum += h_block
 
             # add block annotations
             if annotate:
-                annotate_block(corpus, btype, level, xb, source, sblocks, annotations)
+                annotate_block(
+                    corpus, btype, level, xb, source, blocks, doc_annotations
+                )
 
     fig, colorbar, labels = get_hbm_figure_and_colorbar(btype, source, color_p)
-    infobox = get_infobox(
-        btype, fig, annotate, hasattr(corpus, "ext_documents"), document_data
+    info_box = get_info_box(
+        btype,
+        fig,
+        document_data,
+        other_btype,
+        annotate,
+        hasattr(corpus, "ext_documents"),
     )
     nav_buttons = get_hbm_nav_buttons(fig, btype, labels)
     hbm_add_wheel_zoom(btype, fig, labels)
     hbm_add_pan_tool(fig, labels)
     fig.add_tools(bkm.TapTool(behavior="select"))
 
-    return fig, colorbar, infobox, nav_buttons
+    return fig, colorbar, nav_buttons, info_box
 
 
-def get_hbm_annotations(corpus, btype):
+def get_doc_annotations(corpus):
     annotations = {}
-    if btype == "doc":
-        if hasattr(corpus, "ter_documents"):
-            annotations["ter"] = {
-                "block": load_annotations(
-                    corpus, get_xblock_yblocks_elements, "doc", "ter"
-                ),
-                "subblocks": load_annotations(
-                    corpus, get_subxblocks_yblocks_elements, "doc", "ter"
-                ),
-            }
-        if hasattr(corpus, "ext_documents"):
-            annotations["ext"] = {
-                "block": load_annotations(
-                    corpus, get_xblock_yblocks_elements, "doc", "ext"
-                ),
-                "subblocks": load_annotations(
-                    corpus, get_subxblocks_yblocks_elements, "doc", "ext"
-                ),
-            }
+    if hasattr(corpus, "ter_documents"):
+        annotations["ter"] = {
+            "specific": load_annotations(
+                corpus, get_xblock_yblocks_elements, "doc", "ter"
+            ),
+            "common": load_annotations(
+                corpus, get_subxblocks_yblocks_elements, "doc", "ter"
+            ),
+        }
+    if hasattr(corpus, "ext_documents"):
+        annotations["ext"] = {
+            "specific": load_annotations(
+                corpus, get_xblock_yblocks_elements, "doc", "ext"
+            ),
+            "common": load_annotations(
+                corpus, get_subxblocks_yblocks_elements, "doc", "ext"
+            ),
+        }
     return annotations
 
 
 def get_hbm_transforms(source, fig):
     transforms = {}
+
     # trivial
     transforms["format_number"] = CustomJSTransform(  # field: value
         v_func="""
         return xs.map(value => value.toPrecision(2) + " ")
         """
     )
 
@@ -397,17 +441,20 @@
         """
     )
     transforms["y_block_bottom"] = CustomJSTransform(  # field: y
         args=dict(source=source, fig=fig),
         v_func="""
         const h = source.data["height"]
         const delta = fig.y_range.end - fig.y_range.start
+        const pixels_in_line = fig.frame_height / 41
+        const lines_in_frame = fig.frame_height / pixels_in_line
+        const lines_per_height = lines_in_frame / delta
         return xs.map(function (y, i) {
             if ((y - h[i] / 2 < fig.y_range.start)
-                && (y + h[i] / 2 > fig.y_range.start + (delta * 550 / (fig.frame_height * 30)))) {
+                && (y + h[i] / 2 > fig.y_range.start + 1 / lines_per_height)) {
                 return fig.y_range.start + 0.005 * delta
             }
             return y - h[i] / 2 + 0.005 * delta
         })
         """,
     )
     transforms["y_block_top"] = CustomJSTransform(  # field: y
@@ -420,62 +467,75 @@
                 return fig.y_range.end - 0.005 * delta
             }
             return y + h[i] / 2 - 0.005 * delta
         })
         """,
     )
 
-    # font size
+    # sizes and colors
     transforms["font_size_height_threshold"] = CustomJSTransform(  # field: height
         args=dict(fig=fig),
         v_func="""
         const delta = fig.y_range.end - fig.y_range.start
         return xs.map(height => fig.frame_height * height / delta > 13 ? "1em" : "0em")
         """,
     )
     transforms["contents_font_size"] = CustomJSTransform(  # field: height
         args=dict(fig=fig),
         v_func="""
         const delta = fig.y_range.end - fig.y_range.start
         return xs.map(height => fig.frame_height * height / delta > 30 ? "1em" : "0em")
         """,
     )
+    transforms["line_width"] = CustomJSTransform(  # field: height
+        args=dict(fig=fig),
+        v_func="""
+        return xs.map(height => (fig.frame_height * height > 39) ? 1 : 0.001)
+        """,
+    )
     transforms["map_text_color"] = CustomJSTransform(  # field: z
         v_func="""
         return xs.map(z => (isFinite(z) || z > 0) ? "black" : "grey")
         """,
     )
+
     # contents
     transforms["label_text"] = CustomJSTransform(  # field: label
+        # TODO: no longer needed since removal of hxb from label
         v_func="""
-        return xs.map(label => label.split(" ")[0])
+        return xs.map(label => label)
         """
     )
     transforms["count_text"] = CustomJSTransform(  # field: count
-        args=dict(source=source),
         v_func="""
-        const scount = source.data["scount"]
-        return xs.map(
-            (count, i) => (scount[i] == count) ? scount[i] + " " : scount[i] + "/" + count
-        )
+        return xs.map(count => count + " ")
         """,
     )
     process_items_js = """ // args: xs, source, fig
         const h = source.data["height"]
         const y = source.data["y"]
         const delta = fig.y_range.end - fig.y_range.start
-        const a = (fig.frame_height * 30 / 550) / delta
-        const b = (fig.frame_height * 30 / 550) * (1 / 30)
+        const pixels_in_line = fig.frame_height / 41
+        const lines_in_frame = fig.frame_height / pixels_in_line
+        const lines_per_height = lines_in_frame / delta
+        const height_taken = 1 / lines_per_height + 2 * 0.005 * delta
+//        const a = (fig.frame_height * 30 / 650) / delta
+//        const b = (fig.frame_height * 30 / 650) * (1 / 30)
         function process_items (items, i) {
-            const h_in_i = Math.max(
+            const height_in_frame = Math.max(
                0,
                Math.min(y[i] + h[i] / 2, fig.y_range.end)
                - Math.max(y[i] - h[i] / 2, fig.y_range.start)
             )
-            const num_elements = h_in_i ? Math.max(0, Math.round(h_in_i * a - b)) : 0
+            const num_elements = (
+                height_in_frame
+                ? Math.max(
+                    0, Math.round((height_in_frame - height_taken) * lines_per_height))
+                : 0
+            )
             const sel = (
                 items.slice(0, num_elements).map(
                     ([x0, ...x_rest], i) =>
                     x_rest.length > 1 ? (x0[0] == "L" ? "　" + x0 : x0)
                     : (x0.length > 17 ? x0.slice(0, 17) + "…" : x0)
                 )
             )
@@ -495,15 +555,15 @@
     transforms["short_contents_doc_text"] = CustomJSTransform(  # field: doc_terms
         args=dict(source=source, fig=fig),
         v_func=process_items_js
         + """
         function preprocess_items (_items, i) {
             const items = [..._items]
             const [btype, ent] = items[0]
-            const level_is_1 = source.data["x"][i] == 1
+            const level_is_1 = source.data["level"][i] == 1
             const title = `${level_is_1 ? "≏" : "⋂"} ${Math.pow(2, ent).toPrecision(2)}`
             if (items.length > 1) {
                 items.shift()
                 items[0] = [`${title}　⁄　${items[0][0]}`, ...items[0].slice(1)]
             } else {
                 items[0] = [`${title}`, ...items[0].slice(1)]
             }
@@ -516,58 +576,55 @@
         }
         return res.map(process_items)
         """,
     )
     return transforms
 
 
-def get_hbm_figure_and_colorbar(btype, source_d, color_p):
-    levels = sorted(set(source_d["x"]))
-    fig_frame_height = 850  # TODO: stretch vertically
+def get_hbm_figure_and_colorbar(btype, source_data, color_p):
     fig = bkp.figure(
         toolbar_location=None,
         tools="",
         sizing_mode="stretch_width",
-        frame_height=fig_frame_height,
+        frame_height=900,  # TODO: stretch vertically
         min_border_right=0,
-        x_range=(max(levels) + 0.5, min(levels) - 0.5),
+        x_range=(max(source_data["x"]) + 0.5, min(source_data["x"]) - 0.5),
         y_range=bkm.Range1d(0, 1, bounds="auto", max_interval=1),
         x_axis_label="level",
         y_axis_label=(get_btype_name(btype) + " blocks").strip(),
     )
     fig.grid.visible = False
-    fig.xaxis[0].ticker.desired_num_ticks = len(levels)
+    fig.xaxis[0].ticker.desired_num_ticks = len(set(source_data["x"]))
+    fig.xaxis[0].major_label_overrides = dict(
+        zip(source_data["x"], (str(x) for x in source_data["level"]))
+    )
     fig.xaxis.minor_tick_line_color = None
     fig.yaxis.major_label_text_font_size = "0px"
     fig.yaxis.major_tick_line_color = None
     fig.yaxis.minor_tick_line_color = None
 
-    # TODO move to a transform?
-    source_d["line_width"] = [
-        1 if fig_frame_height * x > 39 else 0.001 for x in source_d["height"]
-    ]
     # Used in link_maps()
-    source_d["o_z"] = source_d["z"].copy()
-    source_d["o_value"] = source_d["value"].copy()
+    source_data["o_z"] = source_data["z"].copy()
+    source_data["o_value"] = source_data["value"].copy()
 
     # remove unused columns and instantiate datasource
-    for key in [k for k in source_d if not len(source_d[k])]:
-        source_d.pop(key)
-    source = bkm.ColumnDataSource(data=source_d, name="{}_map_data".format(btype))
+    for key in [k for k in source_data if not len(source_data[k])]:
+        source_data.pop(key)
+    source = bkm.ColumnDataSource(data=source_data, name="{}_map_data".format(btype))
 
     transforms = get_hbm_transforms(source, fig)
 
     # plot the glyphs
     fig.rect(
         "x",
         "y",
         width=1,
         height="height",
         source=source,
-        line_width="line_width",
+        line_width={"field": "height", "transform": transforms["line_width"]},
         line_color=color_p["line_color"],
         fill_color={"field": "z", "transform": color_p["cmap"]},
         selection_line_width=4.0,
         selection_line_color=color_p["selection_line_color"],
         nonselection_alpha=1.0,
     )
     fig.add_layout(
@@ -690,59 +747,61 @@
         Extra arguments passed to `zmethod`.
 
     Returns
     -------
     lscape: dict of pandas.DataFrames
         for each level, the series of values over its blocks.
     """
-    blocks, levels, sblocks = corpus.get_blocks_levels_sample(btype)
+    blocks, levels = corpus.get_blocks_levels(btype)
 
     lscape = dict()
 
     if zrel is not None:
         for level in levels:
             lidx = blocks[level].unique()
             lscape[level] = zmethod(zrel[0], zrel[1], **zargs)(
-                corpus, sblocks, level, lidx
+                corpus, blocks, level, lidx
             )
         return lscape
 
     elif zby is not None:
         idxs = []
         for gname, g in corpus.data.groupby(zby):
             g.index.name = gname
             idxs.append(g.index)
         for level in levels:
             lscape[level] = pandas.DataFrame(index=blocks[level].unique())
             for idx0, idx1 in zip(idxs[1:], idxs):
                 lscape[level][(idx0.name, idx1.name)] = zmethod(idx0, idx1, **zargs)(
-                    corpus, sblocks, level, lscape[level].index
+                    corpus, blocks, level, lscape[level].index
                 )
         return lscape
 
     else:
         for level in levels:
             lidx = blocks[level].unique()
-            lscape[level] = zmethod(corpus, sblocks, level, lidx)
+            lscape[level] = zmethod(corpus, blocks, level, lidx)
         return lscape
 
 
-def annotate_block(corpus, xbtype, xlevel, xb, source, sblocks, annotations):
-    data = corpus.data.reset_index()  # reset to match bokeh datasource index
-    if xbtype == "doc":  # doc_terms and doc_exts
-        kind = "block" if xlevel == 1 else "subblocks"
+def annotate_block(corpus, xbtype, xlevel, xb, source, sblocks, doc_annotations):
+    # reset index to match bokeh datasource index
+    data = corpus.data.reset_index()
+    if xbtype == "doc":
+        # doc_terms and doc_exts
+        kind = "specific" if xlevel == 1 else "common"
         source["doc_terms"].append(
             prepare_xblock_yblocks_elements(
-                corpus.lblock_to_label, annotations["ter"][kind][xlevel][xb]
+                corpus.lblock_to_label, doc_annotations["ter"][kind][xlevel][xb]
             )
         )
         if hasattr(corpus, "ext_documents"):
             source["doc_exts"].append(
                 prepare_xblock_yblocks_elements(
-                    corpus.lblock_to_label, annotations["ext"][kind][xlevel][xb]
+                    corpus.lblock_to_label, doc_annotations["ext"][kind][xlevel][xb]
                 )
             )
         documents = data.loc[sblocks[xlevel].eq(xb).values].index.to_series()
         num_documents = len(documents) if xlevel == 1 else min(len(documents), 23)
         documents = documents.sample(num_documents)
     else:  # xb_elements
         num_elements = None if xlevel == 1 else 23
@@ -787,73 +846,78 @@
     return dict(
         cmap=cmap,
         line_color=line_color,
         selection_line_color=selection_line_color,
     )
 
 
-def get_infobox(btype, fig, annotate, has_chained_elements, document_data):
+def get_info_box(
+    btype, fig, document_data, other_btype, annotate, has_chained_elements
+):
     source = fig.select_one("{}_map_data".format(btype))
 
     # HTML templates
-    head_html = """<span style="color:#3333dd">block:</span> {label}"""
-    # Numbers
-    info_num_html = """
-    <div style="display:flex; justify-content: space-between">
-        <div><span style="color:#3333dd">value:</span> {value}</div>
-        <div><span style="color:#3333dd">color:</span> {z}</div>
-        <div><span style="color:#3333dd">count:</span> {scount} / {count}</div>
+    # Label and numbers
+    head_html = f"""
+    <div style="display: flex; justify-content: space-between">
+        <div><span style="color:#3333dd">block:</span> {{label}}</div>
+        <div><span style="color:#3333dd">{btype_to_name(btype, plural=True)}:</span>
+             {{count}}</div>
+        <div><span style="color:#3333dd">map value:</span> {{value}}</div>
+        <!-- <div><span style="color:#3333dd">color:</span> {{z}}</div> -->
     </div>
     """
     # Terms and other
-    info_term_html = """
-    <div>
-    """
+    info_term_html = """<div>"""
     if btype == "doc":
-        info_term_html += """{doc_terms}"""
+        doc_ybtypes = ["""<div>{doc_terms}</div>"""]
         if has_chained_elements:
-            info_term_html += """<br />{doc_exts}"""
+            doc_ybtypes.extend(["""<br />""", """<div>{doc_exts}</div>"""])
+        if other_btype == "ext":
+            doc_ybtypes = reversed(doc_ybtypes)
+        info_term_html += """\n""".join(doc_ybtypes)
     else:
         element_label = get_btype_name(btype, True)
         info_term_html += f"""
-            <span style="color:#3333dd">{{top}} {element_label} (occurrences):</span><br />
-            <div style="max-height:40lvh; overflow:auto;">
-            {{xb_elements}}</div>"""
+            <div style="color:#3333dd">{{top}} {element_label} (occurrences):</div>
+            <div>{{xb_elements}}</div>
+        """
     info_term_html += "</div>"
     # Titles
     title_html = """
     <div>
         <span style="color:#3333dd">{sample} titles:</span><br />{titles}
     </div>
     """
 
     if not annotate:
         info_term_html = title_html = ""
-    infobox_wrap = """
-    <div style="font-size: 1.3em">{}
-        <div style="max-height:92lvh; overflow:auto"><br />{}<br />{}<br />{}</div>
-    </div>
-    """
-    infobox_html = infobox_wrap.format(
-        head_html, info_num_html, info_term_html, title_html
+    info_box_wrap = """{}<br />{}<br />{}"""
+    info_box_html = info_box_wrap.format(head_html, info_term_html, title_html)
+    info_box = bkm.Div(
+        text="<br />I suggest you try clicking on a block. 😉",
+        sizing_mode="stretch_both",
+        styles={"font-size": "1.3em"},
+        stylesheets=[bkm.InlineStyleSheet(css=".bk-clearfix {width: 100%};")],
     )
-    infobox = bkm.Div(text="<big>I suggest you try clicking on a block. 😉</big>")
-    infobox_cb = CustomJS(
+    info_box_cb = CustomJS(
         args=dict(
             btype=btype,
             source=source,
-            infobox=infobox,
-            infobox_html=infobox_html,
+            info_box=info_box,
+            info_box_html=info_box_html,
             document_data=document_data,
+            colors=colorcet.glasbey_dark[1:],
+            other_btype=other_btype,
         ),
         code=r"""
     const texts = []
     for (const index of source.selected.indices) {
-        const level_is_1 = source.data["x"][index] == 1
-        const infobox_text = infobox_html.replace(
+        const level_is_1 = source.data["level"][index] == 1
+        const info_box_text = info_box_html.replace(
             /{[\A-z ]*}/g,
             function(key) {
                 key = key.slice(1, -1)
                 if (key == "sample") {
                     return ((btype == "doc") && level_is_1) ? "All" : "Sample"
                 }
                 if (key == "top") {
@@ -866,18 +930,26 @@
                 } else if (['value', 'z'].includes(key)) {
                     const val = source.data[key][index]
                     const y = String(val).match(/-?\d+\.\d{4}/)
                     if (y) { return y[0] }
                 } else if (key == "xb_elements") {
                     const val = source.data[key][index]
                     return (
-                        val.map(x => x[0] + " <small>(" + x[1] + ")</small>").join(", ") + "."
+                        val.map(x => x[0] + " <small>(" + x[1] + ")</small>")
+                        .join(", ") + "."
                     )
                 } else if (["doc_terms", "doc_exts"].includes(key)) {
-                    const val = [...source.data[key][index]]
+                    let val = [...source.data[key][index]]
+                    let label_n = 0
+                    val = val.map(v =>
+                        v.length == 3 && label_n < 5
+                          && key.slice(4, 7) == other_btype
+                        ? [`<span style="color: ${colors[label_n++]}; `
+                          + `font-weight: bold">${v[0]}</span>`, v[1], v[2]]
+                        : v)
                     const [btype, ent] = val.shift()
                     const btype_name = (btype == "ter") ? "terms" : "elements"
                     let title = (level_is_1 ? "≏ Specific " : "⋂ Common ") + btype_name
                     title = `<span style="color:#3333dd">${title}</span>
                              <small>(${Math.pow(2, ent).toPrecision(2)})</small> `
                     return val.reduce(
                         (a, v) => (
@@ -885,45 +957,41 @@
                         ),
                         title,
                     ).slice(0, -1)
                 }
                 return source.data[key][index]
             }
         )
-        texts.push(infobox_text)
+        texts.push(info_box_text)
     }
     if (texts.length){
-        infobox.text = (
-            '<div style="width:49.25lvw; max-height:95lvh; overflow:auto">'
-            + texts.join("<hr>")
-            + "</div>"
-        )
+        info_box.text = texts.join("<hr>")
     }
     else {
-        infobox.text = "<big>I suggest you try clicking on a block. 😉</big>"
+        info_box.text = "<br />I suggest you try clicking on a block. 😉"
     }
         """,
     )
-    source.selected.js_on_change("change:indices", infobox_cb)
-    source.js_on_change("change:data", infobox_cb)
+    source.selected.js_on_change("change:indices", info_box_cb)
+    source.js_on_change("change:data", info_box_cb)
 
-    return infobox
+    return info_box
 
 
 def hbm_add_hover_tool(btype, fig, annotate, has_chained_elements):
     """
     Unused as we now display the same information on top of the blocks
     """
 
     head_html = """<span style="color:#3333dd">block:</span> {label}"""
 
     tooltip_num_html = """
         <span style="color:#3333dd">value:</span> @value{{0,0.0[00]}}
         <span style="color:#3333dd">color:</span> @z{{0,0.0[00]}}
-        <span style="color:#3333dd">count:</span> @scount / @count"""
+        <span style="color:#3333dd">count:</span> @count"""
     if btype == "doc":
         tooltip_term_html = """{doc_terms}"""
         if has_chained_elements:
             tooltip_term_html += """<br />{doc_exts}"""
     else:
         element_label = get_btype_name(btype, True)
         tooltip_term_html = f"""
@@ -1009,18 +1077,21 @@
 
 def get_search_widget(corpus, xbtype, xfig, dfig, selection_mode):
     # Block search tool
     xsource = xfig.select_one("{}_map_data".format(xbtype))
     dsource = dfig.select_one("doc_map_data")
     xblocks, _ = corpus.get_blocks_levels(xbtype)
     dblocks, _ = corpus.get_blocks_levels("doc")
+
+    # Build completion list
+    completions = []
     term_to_mapindex = {
         k: corpus.lblock_to_mapindex[(1, v)] for k, v in xblocks[1].items()
     }
-    completions = sorted(term_to_mapindex)
+    completions.extend(f"/ {term}" for term in sorted(term_to_mapindex))
     # doc_to_mapindex = {
     #     k: corpus.lblock_to_mapindex[(1, v)]
     #     for k, v in dblocks[1].items()
     # }
     # completions.extend(f"/i {id_}" for id_ in sorted(doc_to_mapindex))
     title_to_mapindices = {
         title: [corpus.lblock_to_mapindex[(1, dblocks.loc[idx, 1])] for idx in idxs]
@@ -1032,19 +1103,23 @@
         for _btype in (xbtype, "doc")
         for _blocks, _levels in [corpus.get_blocks_levels(_btype)]
         for _level in _levels
         for _block in _blocks[_level].unique()
     )
 
     searchbox = bkm.AutocompleteInput(
-        placeholder="🔍 Enter a term, or /b followed by a block label,"
-        " or /d followed by a document title (ESC to unselect all)",
+        placeholder=(
+            "🔍 Find blocks: enter text to see choices,"
+            " shown preceded by '/' for terms, '/b' for labels, '/d' for titles"
+            "(Press ESC to unselect all)"
+        ),
         completions=sorted(completions),
-        max_completions=1024,
+        max_completions=128,
         case_sensitive=False,
+        search_strategy="includes",
         sizing_mode="stretch_width",
         align="center",
     )
     searchbox_cb = CustomJS(
         args=dict(
             xsource=xsource,
             term_to_mapindex=term_to_mapindex,
@@ -1052,56 +1127,63 @@
             label_to_mapindex=corpus.label_to_mapindex,
             title_to_mapindices=title_to_mapindices,
             selection_mode=selection_mode,
         ),
         code=r"""
         if (this.value == "") return;
         let indices, _source, _level, _btype, _block
-        const term = this.value;
-        let match = term.match(/\/b (L\d+([DTE])\d+)/)
+        const text = this.value;
+        let match = text.match(/\/b (L\d+([DTE])\d+)/)
         if (match) {
             _btype = match[2];
             indices = [label_to_mapindex[match[1]]]
             if (_btype == "D") { _source = dsource; } else { _source = xsource; }
         }
         else {
-            match = term.match(/\/d (.+)/)
+            match = text.match(/\/d (.+)/)
             if (match) {
                 indices = title_to_mapindices[match[1]]
                 _source = dsource
             }
         }
         if (!match) {
-            indices = [term_to_mapindex[term]]
+            indices = [term_to_mapindex[text.slice(2)]]
             _source = xsource
         }
         if (indices != undefined) {
             if (selection_mode.value == "single") {
                 _source.selected.indices = indices;
             } else {
-                _source.selected.indices = [...new Set(_source.selected.indices.concat(indices))];
+                _source.selected.indices = [
+                    ...new Set(_source.selected.indices.concat(indices))
+                ];
             }
         } else {
             _source.selected.indices = [];
         }
         this.value = "";
         """,
     )
     searchbox.js_on_change("change:value", searchbox_cb)
 
-    return bkl.Row(
+    return bkl.row(
         searchbox, selection_mode, align="center", sizing_mode="stretch_width"
     )
 
 
 def get_hbm_nav_buttons(fig, btype, labels):
     source = fig.select_one("{}_map_data".format(btype))
-    up_button = bkm.Button(label="▲", width=70, margin=(5, 10, 0, 10))
-    down_button = bkm.Button(label="▼", width=70, margin=(0, 10, 0, 10))
-    button_js = """
+    width = 70
+    height = int(width / phi)
+
+    up_button = bkm.Button(label="▲", width=width, height=height, margin=(5, 10, 1, 10))
+    down_button = bkm.Button(
+        label="▼", width=width, height=height, margin=(1, 10, 5, 10)
+    )
+    move_buttons_js = """
     let enact_move = false;
     let old_index
     let new_index
     const data = source.data
     if (source.selected.indices.length == 0) {
         if (move == -1) {
             new_index = data.x.length - 1;
@@ -1141,103 +1223,336 @@
         CustomJS(
             args={
                 "fig": fig,
                 "source": source,
                 "labels": [*labels.values()],
                 "move": 1,
             },
-            code=button_js,
+            code=move_buttons_js,
         )
     )
     down_button.js_on_click(
         CustomJS(
             args={
                 "fig": fig,
                 "source": source,
                 "labels": [*labels.values()],
                 "move": -1,
             },
-            code=button_js,
+            code=move_buttons_js,
         )
     )
-    return bkl.Column(up_button, down_button, sizing_mode="stretch_width")
 
+    zoom_button = bkm.Button(
+        label="⇳",  # ⬍ or ⇳ or ⇕ or 🖽
+        width=width,
+        height=height,
+        margin=(5, 10, 0, 10),
+        stylesheets=[bkm.InlineStyleSheet(css=".bk-btn {font-size: 17px};")],
+    )
+    zoom_button_js = """
+    let new_start
+    let new_end
+    const data = source.data
+    const indices = source.selected.indices
+    if (indices.length == 0) {
+        new_start = 0
+        new_end = 1
+    }
+    else {
+        const old_start = fig.y_range.start
+        const old_end = fig.y_range.end
+        new_start = Math.min(...indices.map(x => data.y[x] - data.height[x] / 2))
+        new_end = Math.max(...indices.map(x => data.y[x] + data.height[x] / 2))
+        if (old_start == new_start && old_end == new_end) {
+            new_start = 0
+            new_end = 1
+        }
+    }
+    fig.y_range.start = new_start;
+    fig.y_range.end = new_end;
+    for (const label of labels) { label.change.emit() }
+    """
+    zoom_button.js_on_click(
+        CustomJS(
+            args={
+                "fig": fig,
+                "source": source,
+                "labels": [*labels.values()],
+            },
+            code=zoom_button_js,
+        )
+    )
 
-def get_doc_histogram(corpus, tap_fig, series: pandas.Series = None):
-    if series is None:
-        series = corpus.data[corpus.col_time]
-        is_datetime, series = try_datetime(series)
-    else:
-        is_datetime = issubclass(series.dtype.type, (np.datetime64, pandas.Period))
+    return bkl.Column(up_button, down_button, zoom_button, sizing_mode="stretch_width")
 
-    if is_datetime:
-        series, xindex = try_period_get_range(series)
-    else:
-        xindex = series.drop_duplicates().sort_values()
 
-    blocks, levels, _ = corpus.get_blocks_levels_sample("doc")
-    tap_vals = []
-    tap_vals_rel = []
-    for tap_level in list(reversed(levels)):
-        tap_hbindex = sorted_hierarchical_block_index(blocks, levels, tap_level)
-        for tap_hb in tap_hbindex:
-            bdata = corpus.data[blocks[tap_level] == tap_hb[-1]]
+def get_doc_histogram_data(corpus, series: pandas.Series = None):
+    series = corpus.data[corpus.col_time] if series is None else series
+    series, xindex = try_time_index(series)
+    blocks, levels = corpus.get_blocks_levels("doc")
+    choice_vals = []
+    for map_level in list(reversed(levels)):
+        map_hbindex = sorted_hierarchical_block_index(blocks, levels, map_level)
+        for map_hb in map_hbindex:
+            bdata = corpus.data[blocks[map_level] == map_hb[-1]]
             val = bdata.groupby(series).size().reindex(xindex).fillna(0)
-            tap_vals.append(val)
-            tap_vals_rel.append(tap_vals[-1] / tap_vals[0].where(tap_vals[0] != 0, 1))
+            choice_vals.append(val)
+    choice_vals[0].index.name = series.name
+    return choice_vals
+
+
+def get_doc_histogram(choice_vals, tap_fig):
+    xaxis = choice_vals[0].index
+    is_time = is_time_type(xaxis)
     source = bkm.ColumnDataSource(
-        {"x": xindex, "y": tap_vals[0], "yrel": tap_vals_rel[0], "ytot": tap_vals[0]}
+        {
+            "x": xaxis,
+            "y": [0] * len(xaxis),
+            "yrel": [0] * len(xaxis),
+            "ytot": choice_vals[0],
+        }
     )
 
     fig = bkp.figure(
         toolbar_location=None,
         tools="",
-        sizing_mode="stretch_width",
-        height=140,
-        x_axis_type="datetime" if is_datetime else "linear",
-        x_axis_label=f"{series.name}",
+        min_height=150,
+        sizing_mode="stretch_both",
+        x_axis_type="datetime" if is_time else "linear",
+        # x_axis_label=f"{xaxis.name}",
         y_axis_label="documents",
-        align="end",
     )
-    if is_datetime:
+
+    if is_time:
         fig.xaxis.formatter = DatetimeTickFormatter(days="%d %b")
 
     rel_rend = fig.line(
         "x", "yrel", source=source, color="red", y_range_name="rel", legend_label="rel"
     )
     fig.line("x", "y", source=source, color="grey", legend_label="abs")
 
     fig.y_range.start = 0.0
     fig.extra_y_ranges = {"rel": bkm.DataRange1d(renderers=[rel_rend], start=0.0)}
     fig.add_layout(
         bkm.LinearAxis(y_range_name="rel", major_label_text_color="red"), "right"
     )
     fig.legend.location = "top_left"
-    tap_source = tap_fig.select_one("doc_map_data")
+    fig.x_range.bounds = "auto"
     dochist_cb = CustomJS(
         args=dict(
+            fig=fig,
             source=source,
-            tap_vals=tap_vals,
-            tap_vals_rel=tap_vals_rel,
+            choice_vals=choice_vals,
         ),
         code="""
-        let index = cb_obj.indices[0]
-        if (index == undefined) { index = 0 }
+        const index = (
+            cb_obj.indices === undefined || cb_obj.indices[0] === undefined ?
+            0 : cb_obj.indices[0]
+        )
         const data = {...source.data}
-        data.y = tap_vals[index]
-        data.yrel = tap_vals_rel[index]
+        data.y = choice_vals[index]
+        data.yrel = new Float64Array(data.y).map((val, i) => val ? val / data.ytot[i] : val)
         source.data = data
         """,
     )
+    bio.curdoc().js_on_event("document_ready", dochist_cb)
+    tap_source = tap_fig.select_one("doc_map_data")
     tap_source.selected.js_on_change("change:indices", dochist_cb)
 
-    fig.add_tools(
-        bkm.HoverTool(
-            tooltips=[("", ("@x{%F}" if is_datetime else "@x") + " (@y / @ytot)")],
-            formatters={"@x": "datetime"} if is_datetime else {},
-            mode="vline",
-            attachment="right",
-            renderers=[rel_rend],
-        )
+    wheelzoom_tool = bkm.WheelZoomTool(
+        dimensions="width",
+        maintain_focus=False,
+        zoom_on_axis=True,
+    )
+    pan_tool = bkm.PanTool(dimensions="width")
+    hover_tool = bkm.HoverTool(
+        tooltips=[("", ("@x{%F}" if is_time else "@x") + " (@y / @ytot)")],
+        formatters={"@x": "datetime"} if is_time else {},
+        mode="vline",
+        attachment="right",
+        renderers=[rel_rend],
     )
+    fig.add_tools(wheelzoom_tool, pan_tool, hover_tool)
+    fig.toolbar.active_scroll = wheelzoom_tool
+    fig.toolbar.active_drag = pan_tool
+
+    return fig
+
+
+def get_multi_histogram_data(corpus, ybtype, series: pandas.Series = None):
+    annotations_spe = load_annotations(
+        corpus, get_xblock_yblocks_elements, "doc", ybtype
+    )
+    annotations_com = load_annotations(
+        corpus, get_subxblocks_yblocks_elements, "doc", ybtype
+    )
+
+    lblock_to_label = corpus.lblock_to_label
+    yblocks, ylevels = corpus.get_blocks_levels(ybtype)
+    y_element_to_block = yblocks[1]
+    if ybtype == "ext":
+        doc_exts = corpus.get_doc_exts()
+
+    def counting_f(domain_data, level, xblock):
+        annotations = annotations_spe if level == 1 else annotations_com
+
+        xblock_yblocks = annotations[level][xblock]["blocks"]
+        # number of terms in domain_data belonging to each yblock
+        yblocks_count = {lblock_to_label[1, yb]: 0 for yb in xblock_yblocks}
+        if ybtype == "ter":
+            for doc in domain_data[corpus.column]:
+                for yb in {
+                    yb
+                    for sen in doc
+                    for ter in sen
+                    if (yb := y_element_to_block[ter]) in xblock_yblocks
+                }:
+                    yblocks_count[lblock_to_label[1, yb]] += 1
+        else:
+            for doc_idx in domain_data.index:
+                for yb in {
+                    yb
+                    for ext in doc_exts[doc_idx]
+                    if (yb := y_element_to_block[ext]) in xblock_yblocks
+                }:
+                    yblocks_count[lblock_to_label[1, yb]] += 1
+        yblocks_count = pandas.Series(yblocks_count, dtype="float64").fillna(0)
+        return yblocks_count
+
+    series = corpus.data[corpus.col_time] if series is None else series
+    series, xindex = try_time_index(series)
+
+    dblocks, dlevels = corpus.get_blocks_levels("doc")
+    choice_vals = []
+    for level in list(reversed(dlevels)):
+        hbindex = sorted_hierarchical_block_index(dblocks, dlevels, level)
+        for hb in hbindex:
+            domain_data = corpus.data[dblocks[level] == hb[-1]]
+            df_sums = domain_data.groupby(series).apply(counting_f, level, hb[-1])
+            val = df_sums.reindex(xindex).fillna(0)
+            choice_vals.append(val)
+    choice_vals[0].index.name = xindex.name
+    return choice_vals
+
+
+def get_multi_histogram(dfs, tap_fig):
+    xaxis = dfs[0].index
+    is_time = is_time_type(xaxis)
+    fig = bkp.figure(
+        toolbar_location=None,
+        tools="",
+        sizing_mode="stretch_both",
+        x_axis_type="datetime" if is_time else "linear",
+        x_axis_label=f"{xaxis.name}",
+        y_axis_label="occurrences",
+    )
+
+    if is_time:
+        fig.xaxis.formatter = DatetimeTickFormatter(days="%d %b")
+    fig.y_range.start = 0.0
+    tap_source = tap_fig.select_one("doc_map_data")
+    multihist_cb = CustomJS(
+        args=dict(
+            tap_source=tap_source.selected,
+            xaxis=xaxis.to_list(),
+            choice_yaxis=[df.to_dict(orient="list") for df in dfs],
+            fig=fig,
+            colors=colorcet.glasbey_dark[1:],
+        ),
+        code="""
+        const ColumnDataSource = Bokeh.Models.get("ColumnDataSource")
+        const Line = Bokeh.Models.get("Line")
+        const VAreaStep = Bokeh.Models.get("VAreaStep")
+        const index = tap_source.indices === undefined ? undefined : tap_source.indices[0]
+        fig.x_range.bounds = "auto"
+        fig.renderers = []
+        let cur_y, prev_y
+        cur_y = prev_y = xaxis.map(x => 0)
+        const block2yaxis = index === undefined ? {} : choice_yaxis[index]
+        let num = 0
+        for (const yname in block2yaxis) {
+            const y_diff = block2yaxis[yname]
+            cur_y = prev_y.map((x, i) => x + y_diff[i])
+            const source = new ColumnDataSource(
+                {data: {x: xaxis, y1: prev_y, y2: cur_y, y: y_diff}}
+            )
+            /* Old style using VAreaStep
+            const varea = new VAreaStep({
+                x: { field: "x" },
+                y1: { field: "y1" },
+                y2: { field: "y2" },
+                fill_color: colors[num],
+                step_mode: "center",
+            });
+            fig.add_glyph(varea, source)
+            */
+            const line = new Line({
+                x: { field: "x" },
+                y: { field: "y" },
+                line_color: colors[num],
+            });
+            fig.add_glyph(line, source)
+            prev_y = cur_y
+            num += 1
+            if (num === 5) { break }
+        }
+        if (num == 0) {
+            const source = new ColumnDataSource({data: {x: xaxis, y: cur_y}})
+            const line = new Line({x: { field: "x" }, y: { field: "y" }});
+            fig.add_glyph(line, source)
+            // fig.x_range.reset()
+            // fig.y_range.reset()
+            fig.renderers[0].visible = false
+        }
+        fig.x_range.reset()
+        fig.y_range.reset()
+        """,
+    )
+    bio.curdoc().js_on_event("document_ready", multihist_cb)
+    tap_source.selected.js_on_change("change:indices", multihist_cb)
+
+    relative_mode = bkm.Select(value="absolute", options=["absolute", "relative"])
+    fig.js_on_event(
+        bke.Tap,
+        CustomJS(
+            args=dict(relative_mode=relative_mode, reload_data=multihist_cb),
+            code="""
+        const renderers = cb_obj.origin.renderers
+        if (!renderers[0].data_source.data.hasOwnProperty("y")) return
+        if (relative_mode.value == "absolute") {
+            let total = renderers[0].data_source.data.y.map(x => 0)
+            for (const rend of renderers) {
+                const data = rend.data_source.data
+                total = total.map((x, i) => x + data.y[i])
+            }
+            for (const rend of renderers) {
+                const data = {...rend.data_source.data}
+                data.y = data.y.map((x, i) => x ? x / total[i] : 0)
+                rend.data_source.data = data
+            }
+            relative_mode.value = "relative"
+        } else {
+            reload_data.execute()
+            relative_mode.value = "absolute"
+        }
+    """,
+        ),
+    )
+
+    wheelzoom_tool = bkm.WheelZoomTool(
+        dimensions="width",
+        maintain_focus=False,
+        zoom_on_axis=True,
+    )
+    pan_tool = bkm.PanTool(dimensions="width")
+    hover_tool = bkm.HoverTool(
+        tooltips=[("", ("@x{%F}" if is_time else "@x") + " (@y)")],
+        formatters={"@x": "datetime"} if is_time else {},
+        mode="mouse",
+        attachment="left",
+    )
+    fig.add_tools(wheelzoom_tool, pan_tool, hover_tool)
+    fig.toolbar.active_scroll = wheelzoom_tool
+    fig.toolbar.active_drag = pan_tool
 
     return fig
```

### Comparing `sashimi_domains-0.9.3/src/sashimi/blocks/hierarchical_block_map_help.html` & `sashimi_domains-0.9.4/src/sashimi/blocks/hierarchical_block_map_help.html`

 * *Files 6% similar despite different names*

```diff
@@ -41,35 +41,33 @@
   </ul>
 </p>
 <p>Block contents for topics/other:
   <ol>
     <li><em>frequent elements</em>: top terms from the topic, ordered by highest frequency in the corpus.
   </ol>
 </p>
-<p>
-  Last, in case a line plot appears below the domain map, it represents the distribution of documents along some dimension, usually time. The red line corresponds to the fraction of documents at that point, and the grey line to the absolute number of documents. When a domain is selected, the plot gets restricted to the documents it contains.
-</p>
 
 <h2>My cursor, <i>maihashi</i></h2>
 <p>
   <strong>Scroll</strong> down and up to zoom in and out of blocks. To help navigate the hierarchy, zooming in on a block stops when the block fills the frame. Move the cursor lower in the hierarchy (to the right) to continue zooming. Zooming on a block that is partially hidden immediately brings it entirely into the frame.
 </p>
 <p>
   <strong>Click</strong> on a block to select and learn more about it: on the opposite side, the Map and the Info tab will be updated with information on the selected block. <em>Shift-click</em> allows selecting multiple blocks, and <em>Ctrl-Shift-click</em> allows deselecting individual blocks. You may deselect all selected blocks in a map with a <em>Control-click</em> elsewhere on the map, or deselect everything in all maps by pressing <em>Escape</em> on the keyboard.
 </p>
 
 <h3>Upon selecting a domain</h3>
 <p>
   The color and values of the Topic map will be updated to show, for each topic, the logarithm of the ratio between how much the topic is used in the selected domain(s) against how much it gets used overall. This quantity represents how much a topic is over (positive) or under (negative) represented in the selected domain, with shades of grey standing for negative values.
 </p>
+<h4>The <em>Domain info</em> tab</h4>
 <p>
-  The document distribution plot, if present, will be updated to show the distribution of documents belonging to the (first chosen) domain.
+  Two line plots may appear on top of the tab. The first represents the distribution of documents along some dimension, usually time. It concerns the documents belonging to the (first chosen) domain. The red line corresponds to the fraction of documents at that point, and the grey line to the absolute number of documents. When a domain is selected, the plot gets restricted to the documents it contains. The second shows multiple colored lines, one for each characteristic topic, representing the distribution along the same dimension of documents using that topic.
 </p>
 <p>
-  The <em>Domain info</em> tab, in addition to the full information seen on top of the domain block(s), will provide a list of <em>titles</em> from documents in the domain, with links to those documents' URLs if that was provided when building the map.
+  Furthermore, the tab displays the full information partially seen on top of the domain block(s), plus a list of <em>titles</em> from documents in the domain, with links to those documents' URLs if that was provided when building the map.
 </p>
 <p>When selecting multiple domains, the Topic map's color and value will depend on the choice presented in the selector (below it and to the right of the Search bar):
   <ul>
     <li>Single: keeps those of the first chosen domain.
     <li>Multi AND: for each topic, picks the minimum among the chosen domains.
     <li>Multi OR: for each topic, picks the maximum among the chosen domains.
   </ul>
@@ -82,13 +80,14 @@
 <p>
   The <em>Topic info</em> tab, in addition to the full information seen on top of the topic block(s), will provide a list of <em>titles</em> from documents that contain any terms from the topic. At level 1, <em>frequent terms</em> displays the full list of terms in the topic.
 </p>
 <p>When selecting multiple topics, the Topic map's color and value behave in a manner analogous to multiple domains.</p>
 
 <h3>Searching</h3>
 
-You'll find a Search bar below the Topic/other map. Use it wisely.
+You'll find a Search bar on top of the maps. It recognizes partial matches, and allows searching blocks by label (i.e. "L2D3", "L4T2"), by term (i.e. "green", "yellow") wihch will select the containing topic, and by title (i.e. "A study of wonderful things") which will select the containing domain. Use it wisely.
 
 <h2>Au revoir, <em>またいつか</em></h2>
+<h3>Bibliography (also to credit where appropriate)</h3>
 <p>
   Hannud Abdo, A., Cointet, J.-P., Bourret, P., & Cambrosio, A. (2022). Domain-topic models with chained dimensions: Charting an emergent domain of a major oncology conference. Journal of the Association for Information Science and Technology, 73( 7), 992– 1011. <a href="https://doi.org/10.1002/asi.24606">https://doi.org/10.1002/asi.24606</a>
 </p>
```

### Comparing `sashimi_domains-0.9.3/src/sashimi/blocks/link_maps.py` & `sashimi_domains-0.9.4/src/sashimi/blocks/link_maps.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/src/sashimi/blocks/network_map.py` & `sashimi_domains-0.9.4/src/sashimi/blocks/network_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,27 +26,28 @@
     get_xblock_yblocks_elements,
     get_subxblocks_yblocks_elements,
     load_annotations,
 )
 from ..misc import get_hash
 
 
+def first_element(yb_info_elements):
+    return yb_info_elements[0][0] if yb_info_elements else ""
+
+
 def dblock_terext_graph(
     corpus,
     xbtype,
     doc_level,
     ter_level,
     ext_level,
     *,
     xb_selection=None,
     edges="specific",
 ):
-    def first_element(yb_info_elements):
-        return yb_info_elements[0][0] if yb_info_elements else ""
-
     xlevel = {"doc": doc_level, "ter": ter_level, "ext": ext_level}[xbtype]
     if edges == "specific":
         annotation_function = get_xblock_yblocks_elements
     elif edges == "common":
         if xlevel == 1:
             raise ValueError(
                 f"`edges=common` requires xbtype (here `{xbtype}`) level > 1 (here `{xlevel}`)."
@@ -153,15 +154,15 @@
         xb_selection=xb_selection,
         edges=edges,
     )
     vp_label = g.vp["label"]
 
     vp_block = g.new_vertex_property("int")
     for v in g.vertices():
-        vp_block[v] = corpus.label_to_hblock[vp_label[v]][-1]
+        vp_block[v] = corpus.label_to_tlblock[vp_label[v]][-1]
 
     vp_type = g.vp["type"]
 
     g.vp["shape"] = g.new_vertex_property(
         "string",
         [
             "square" if t == "D" else "circle" if t == "T" else "hexagon"
@@ -196,15 +197,15 @@
     vp_fill_color = g.vp["fill_color"] = g.new_vertex_property("vector<float>")
     for v in g.vertices():
         vp_size[v] = 100 if vp_type[v] == "D" else 80
         vp_fill_color[v] = [
             1,
             0,
             0,
-            0.85 * size[vp_block[v]] if vp_type[v] == "D" else 0,
+            0.8 * size[vp_block[v]] if vp_type[v] == "D" else 0,
         ]
         if vp_type[v] == "D" and split_on is not None:
             color = period_color_scalar[vp_block[v]]
             vp_color[v] = [0, color > 0, color < 0, np.abs(color)]
         elif vp_type[v] == "E":
             vp_color[v] = [0, 0, 0, 1]
         else:
@@ -236,24 +237,24 @@
     fpath_graphml = target_dir / naming.gen("network_map", fname_params, "graphml")
     fpath_pdf = target_dir / naming.gen("network_map", fname_params, "pdf")
     fpath_svg = target_dir / naming.gen("network_map", fname_params, "svg")
     g.save(str(fpath_graphml))
     draw(g, str(fpath_pdf))
     draw(g, str(fpath_svg))
 
-    if False:  # Disable improved layout for now
-        gv = improve_layout(g)
+    if False:  # Disable circular layout for now
+        gv = circular_layout(g)
         gv.save(
             str(
-                target_dir / naming.gen("network_map_improved", fname_params, "graphml")
+                target_dir / naming.gen("network_map_circular", fname_params, "graphml")
             )
         )
         draw(
             gv,
-            str(target_dir / naming.gen("network_map_improved", fname_params, "pdf")),
+            str(target_dir / naming.gen("network_map_circular", fname_params, "pdf")),
         )
 
     return {"graphml": fpath_graphml, "pdf": fpath_pdf, "svg": fpath_svg}
 
 
 def get_split_fraction_diff_rel(
     corpus, dlevel, dblocks_selection, split_on, split_list
@@ -264,15 +265,15 @@
     (split_on) series of values based on which to split
     (split_list) values from split series to consider positive
 
     Example:
     get_split_fraction_diff_rel(
         ...,
         split_on=corpus.data[corpus.col_time],
-        split_list=corpus.data[corpus.col_time].pipe(lambda x: x[x.ge(2002)])
+        split_list=set(corpus.data[corpus.col_time][lambda x: x.ge(2002)])
     )
     """
     index = split_on.index.intersection(
         corpus.dblocks.index[corpus.dblocks[dlevel].isin(set(dblocks_selection))]
     )
     split_on = split_on[index]
     split_on.name = "split_on"
@@ -292,15 +293,15 @@
 
 
 def area2radius(area):
     """Domain area, currently squares"""
     return np.sqrt(area)  # np.sqrt(area / np.pi)
 
 
-def improve_layout(g):
+def circular_layout(g):
     vp_pos = g.vp["position"]
     vp_type = g.vp["type"]
     vp_pin = g.new_vertex_property("bool", (vp_type[v] == "D" for v in g.vertices()))
     center_x = (lambda x: np.mean([x.max(), x.min()]))(vp_pos.get_2d_array([0])[0])
     center_y = (lambda x: np.mean([x.max(), x.min()]))(vp_pos.get_2d_array([1])[0])
     for v in g.vertices():  # Put origin at center
         vp_pos[v] = [vp_pos[v][0] - center_x, vp_pos[v][1] - center_y]
@@ -322,31 +323,27 @@
                     vp_pos[w] = 1.5 * vp_pos[w].a
     # Redo sfdp with frozen domains
     vp_pos = g.vp["position"] = gt.sfdp_layout(g, pos=vp_pos, pin=vp_pin)
     return gt.GraphView(g, vfilt=lambda v: vp_type[v] != "T" or v.in_degree() > 1)
 
 
 def draw(g, output_file=None):
+    vp = {**g.vp}
+    ep = {**g.ep}
+    if "weight" in vp:
+        vp["pen_width"] = vp["weight"]
+    if "label" in vp:
+        vp["text"] = vp["label"]
+    if "weight" in ep:
+        ep["pen_width"] = ep["weight"]
+    if "label" in g.ep:
+        ep["text"] = ep["label"]
     gt.graph_draw(
         g,
-        pos=g.vp["position"],
-        vprops=dict(
-            size=g.vp["size"],
-            shape=g.vp["shape"],
-            color=g.vp["color"],
-            pen_width=g.vp["weight"],
-            fill_color=g.vp["fill_color"],
-            text=g.vp["label"],
-            text_position=-2,
-            text_color="black",
-            font_size=15,
-        ),
-        eprops=dict(
-            text=g.ep["label"],
-            font_size=12,
-            pen_width=g.ep["weight"],
-        ),
+        pos=g.vp.get("position", None),
+        vprops={"text_position": -2, "text_color": "black", "font_size": 15, **vp},
+        eprops={"font_size": 12, "text_color": "blue", "text_parallel": True, **ep},
         output_size=(3 * 1920, 3 * 1080),
         adjust_aspect=False,
         bg_color="white",
         output=output_file,
     )
```

### Comparing `sashimi_domains-0.9.3/src/sashimi/blocks/util.py` & `sashimi_domains-0.9.4/src/sashimi/blocks/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 # <https://gitlab.com/solstag/abstractology>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 import numpy as np
 import pandas
 
+phi = (1 + 5**0.5) / 2  # the golden ratio
+
 
 def sorted_hierarchical_block_index(blocks, levels, level):
     return sorted(
         tuple(reversed(x))
         for x in (
             blocks[list(levels[levels.index(level) :])]  # list() in case passed a tuple
             .groupby(level)
@@ -56,65 +58,88 @@
         } else {
             return value => 1
         }
     }
     """
 
 
+def try_time_index(series):
+    is_time, series = try_datetime(series)
+    if is_time:
+        series, xindex = try_period_get_range(series)
+    else:
+        xindex = series.drop_duplicates().sort_values()
+    return series, xindex
+
+
+def is_time_type(series):
+    return issubclass(series.dtype.type, (np.datetime64, pandas.Period))
+
+
 def try_datetime(series):
-    is_datetime = issubclass(series.dtype.type, (np.datetime64, pandas.Period))
-    if is_datetime:
-        return is_datetime, series
+    is_time = is_time_type(series)
+    if is_time:
+        return is_time, series
     if series.dropna().map(lambda x: isinstance(x, str)).all():
         try:
             series = to_datetimeindex(series)
-            is_datetime = True
+            is_time = True
         except Exception:
             pass
-    if is_datetime:
-        return is_datetime, series
+    if is_time:
+        return is_time, series
     if not issubclass(series.dtype.type, np.number):
         try:
             series = series.astype(int)
         except Exception:
             series = series.astype(float)
         except Exception:
             pass
     if issubclass(series.dtype.type, np.number):
         try:
             if series.min().ge(1678) and series.max().le(2262):
                 series.loc[series.notna()] = series.dropna().astype(int).astype(str)
                 series = to_datetimeindex(series)
             elif series.min() < 0 or series.max() > 999999:
                 series = to_datetimeindex(series, unit="s")
-            is_datetime = True
+            is_time = True
         except Exception:
             pass
-    return is_datetime, series
+    return is_time, series
 
 
 def to_datetimeindex(series, **kwargs):
     return pandas.DatetimeIndex(pandas.to_datetime(series, dayfirst=True, **kwargs))
 
 
 def try_period_get_range(series):
     if issubclass(series.dtype.type, pandas.Period):
         full_range = pandas.period_range(series.min(), series.max())
     elif issubclass(series.dtype.type, np.datetime64) and (freq := get_freq(series)):
         full_range = pandas.period_range(series.min(), series.max(), freq=freq)
         series = series.to_period(freq=freq)
     else:
         full_range = series.drop_duplicates().sort_values()
+    full_range.name = series.name
     return series, full_range
 
 
 def get_freq(series):
     valid = series.dropna()
     return (
         "A"
         if (valid.is_year_start.all() or valid.is_year_end.all())
         else "M"
         if (valid.is_month_start.all() or valid.is_month_end.all())
         else "D"
         if valid.is_normalized
         else False
     )
+
+
+def btype_to_name(btype, plural=False):
+    if btype == "doc":
+        return "documents" if plural else "document"
+    if btype == "ter":
+        return "terms" if plural else "term"
+    if btype == "ext":
+        return "elements" if plural else "element"
```

### Comparing `sashimi_domains-0.9.3/src/sashimi/blocks/zmethods.py` & `sashimi_domains-0.9.4/src/sashimi/blocks/zmethods.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,26 +185,28 @@
     Result
     ------
     A pandas.Series with MultiIndex:
     (domain level, domain, cross level, cross block)
     """
     use_cache = corpus.use_cached_cross_counts
     dblocks = corpus.dblocks
-    yblocks, yblocks_levels, _ = corpus.get_blocks_levels_sample(ybtype)
+    yblocks, yblocks_levels = corpus.get_blocks_levels(ybtype)
     y_documents = corpus.get_xelement_yelements(ybtype, "doc")
     fname_params = [("ybtype", ybtype), ("ltype", ltype)]
     if sample_hash := corpus.get_sample_hash(
         **{x: x in {"doc", ybtype} for x in ["doc", "ter", "ext"]}
     ):
         fname_params = [("sample", sample_hash), *fname_params]
     if ybtype == "ter":
         fdir = corpus.blocks_dir
     elif ybtype == "ext":
         fdir = corpus.chained_dir
-    fpath = fdir / "cache" / naming.gen("cross_counts", fname_params, corpus.ext_data)
+    fpath = (
+        fdir / "cache" / naming.gen("cross_counts", fname_params, corpus.suffix_data)
+    )
 
     if use_cache:
         try:
             values = ioio.load(fpath)
             if isinstance(values, dict):
                 values = pandas.Series(
                     index=pandas.MultiIndex.from_tuples(values["index"]),
```

### Comparing `sashimi_domains-0.9.3/src/sashimi/blocks/tables/__init__.py` & `sashimi_domains-0.9.4/src/sashimi/blocks/tables/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,15 +280,15 @@
 ####################
 # Helper functions #
 ####################
 
 
 def get_subxblocks(corpus, xbtype, xlevel, xb, sxlevel=None):
     if sxlevel is None:
-        sxlevel = xlevel - 1
+        sxlevel = corpus.get_sublevel(xlevel, xbtype)
     xblocks, xlevels = corpus.get_blocks_levels(xbtype)
     xblocks = xblocks[xblocks[xlevel].eq(xb)]
     return [
         corpus.hblock_to_level_block(x, xbtype)
         for x in sorted_hierarchical_block_index(xblocks, xlevels, level=sxlevel)
     ]
```

### Comparing `sashimi_domains-0.9.3/src/sashimi/blocks/tables/tables.css` & `sashimi_domains-0.9.4/src/sashimi/blocks/tables/tables.css`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/src/sashimi/blocks/tables/tables_html.py` & `sashimi_domains-0.9.4/src/sashimi/blocks/tables/tables_html.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/src/sashimi/blocks/tables/tables_plots.py` & `sashimi_domains-0.9.4/src/sashimi/blocks/tables/tables_plots.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/src/sashimi/corpus/__init__.py` & `sashimi_domains-0.9.4/src/sashimi/corpus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         if config_path is not None:
             self.config_path = config_path
         to_load = load_config(get_config_path(config_path, analysis_dir, storage_dir))
 
         # Load properties
         prop_defaults = {
             STORAGE_DIR_KEY: STORAGE_DIR_DEFAULT,
-            "ext_data": ".json.xz",
+            "suffix_data": ".json.xz",
             "column": None,
             "token_sources": [],
             "text_sources": [],
         }
         self._load_properties(wargs, to_load, prop_defaults)
 
         # Load directory structure
@@ -204,15 +204,15 @@
             self._column = column
         else:
             raise KeyError("`column` must be a valid key in the data.")
 
     column = makep("column", True, _set_column, None)
     token_sources = makep("token_sources")
     text_sources = makep("text_sources")
-    ext_data = makep("ext_data")
+    suffix_data = makep("suffix_data")
     _column_label_keys = {
         "affiliations",
         "authors",
         "id",
         "time",
         "title",
         "url",
@@ -225,15 +225,15 @@
 
     storage_dir = makep(STORAGE_DIR_KEY, True, _fset_dir(STORAGE_DIR_KEY), None)
     analysis_dir = makep(ANALYSIS_DIR_KEY, True, _fset_dir(ANALYSIS_DIR_KEY), None)
     resources_dir = makep(RESOURCES_DIR_KEY, True, _fset_dir(RESOURCES_DIR_KEY), None)
     data_store = property_getfuncdir(lambda self: self.storage_dir / "data")
 
     def _gen_data_name(self, names):
-        return naming.gen("|".join(names), [], self.ext_data)
+        return naming.gen("|".join(names), [], self.suffix_data)
 
     data_name = property(
         lambda self: self._gen_data_name(self.loaded["data"])
         if self.loaded["data"]
         else None
     )
     data_dir = property_getfuncdir(lambda self: self.data_store / self.data_name)
@@ -308,18 +308,18 @@
         data = ioio.load_pandas(self.data_store / name_in_store / name_in_store)
         if return_not_load:
             return data
         self.load_data(data, name=name)
 
     def list_datasets(self):
         return [
-            fpath.name[: -len(self.ext_data)]
+            fpath.name[: -len(self.suffix_data)]
             for fpath in self.data_store.iterdir()
             if ioio.uncompressed_suffix(fpath)
-            == ioio.uncompressed_suffix(Path(f"_{self.ext_data}"))
+            == ioio.uncompressed_suffix(Path(f"_{self.suffix_data}"))
         ]
 
     ################
     # Data methods #
     ################
 
     def check_column(self, default_name="_tokens"):
@@ -568,27 +568,17 @@
     def clear_data(self):
         self.cache_clear(clear_static=True)
         self.data, self.odata = pandas.DataFrame(), pandas.DataFrame()
         self.loaded["data"] = []
 
     def cache_clear(self, clear_static=False):
         if clear_static and clear_static != "ext":
-            clearattrs(
-                self,
-                [
-                    "ter_documents",
-                ],
-            )
+            clearattrs(self, ["ter_documents"])
         if clear_static and clear_static != "ter":
-            clearattrs(
-                self,
-                [
-                    "ext_documents",
-                ],
-            )
+            clearattrs(self, ["ext_documents"])
         for m in dir(type(self)):
             m = getattr(type(self), m)
             if hasattr(m, "cache_clear"):
                 m.cache_clear()
 
     ###################
     # Data derivation #
@@ -627,28 +617,32 @@
         for i_doc, doc in tqdm(docs.items(), total=len(docs), desc="Doc"):
             for element in doc:
                 d[element][i_doc] += 1
         setattr(self, f"{btype}_documents", d)
 
     def make_matcher(self, extend=None, multi=False, na_action="ignore"):
         """
-        (extend) prop and matcher, if not self.graph_extend.
-        (multi) allow multiple matches if `prop` values are a list.
+        (extend) None | {"prop": [str], "matcher": [None|str]}
+            If None, uses `corpus.extended` otherwise `corpus.graph_extend`.
+            `prop` is the column whose values will be used to form new nodes.
+            If all values are lists, they get exploded before matching.
+            `matcher` can be:
+            - None: edges link documents to items found in `prop`.
+            - str: file in resources dir containing a dictionary mapping node names to
+            regular expressions to be applied at `prop` to connect keys to documents.
 
-        `prop` is the column whose values will be used to form new nodes.
-        `matcher` can be:
-        - None: edges link documents to items found in `prop`.
-        - str: file in resources dir containing a dictionary mapping node names to
-        regular expressions to be applied at `prop` to connect keys to documents.
+        (multi) `get_matches()` keeps duplicates when an exploded value matches more than once
 
         :match_keys: nodes of the extended dimension
         :get_matches: given a node, returns the corresponding documents
 
         Usage:
         match_keys, get_matches = self.make_matcher()
+
+        TODO: move multi and na_action into graph_extend?
         """
         extend = extend or self.extended or self.graph_extend
         prop = self.data[extend["prop"]]
         if prop.dropna().map(lambda x: isinstance(x, list)).all():
             prop = prop.explode()
         if na_action == "ignore":
             prop = prop.dropna()  # dropna after explode() as []→nan
@@ -699,17 +693,17 @@
     def set_sample(self, sample, keep=False):
         if keep:
             new_data = self.data.loc[self.samplify(sample, self.data)]
         else:
             new_data = self.odata.loc[self.samplify(sample, self.odata)]
         if not self.data.index.equals(new_data.index):
             self.cache_clear()
-        self.data = new_data
+        self.data = new_data.copy()
 
-    def get_sample_hash(self, doc, ter=False, ext=False):
+    def get_sample_hash(self, *, doc, ter=False, ext=False):
         hashes = {}
         if doc and not self.data.index.equals(self.odata.index):
             hashes["D"] = get_hash(self.data.index)
         if ter and hasattr(self, "_orig_tblocks"):
             if not self.tblocks.index.equals(self._orig_tblocks.index):
                 hashes["T"] = get_hash(self.tblocks.index)
         if ext and hasattr(self, "_orig_eblocks"):
```

### Comparing `sashimi_domains-0.9.3/src/sashimi/corpus/nlp.py` & `sashimi_domains-0.9.4/src/sashimi/corpus/nlp.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/src/sashimi/corpus/parsers.py` & `sashimi_domains-0.9.4/src/sashimi/corpus/parsers.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/src/sashimi/corpus/wos.py` & `sashimi_domains-0.9.4/src/sashimi/corpus/wos.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from ..util.wos_lam import WosLam
 
 
 def load_wos_citations(self, user=None, password=None, pmids=None):
     if pmids is None:
         pmids = self.data.pmid
-    fpath = Path(self.data_dir, f"wos_citations{self.ext_data}")
+    fpath = Path(self.data_dir, f"wos_citations{self.suffix_data}")
     try:
         wos_citations = ioio.load_pandas(fpath)
     except FileNotFoundError:
         wos_citations = pandas.Series()
     new_pmids = pmids[~pmids.isin(wos_citations.index)]
     print(
         "Found {} stored, downloading {} new citation counts".format(
```

### Comparing `sashimi_domains-0.9.3/src/sashimi/graph_models/__init__.py` & `sashimi_domains-0.9.4/src/sashimi/graph_models/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,25 +14,24 @@
 # <https://gitlab.com/solstag/abstractology>
 #
 # Contributions are welcome, get in touch with the author(s).
 
 
 import graph_tool.all as gt
 import numpy
-import pandas
 from pathlib import Path
 import shutil
 
 from ..misc import clearattrs, makep_fromdict, property_getfuncdir
 from ..ioio import ioio
 from ..corpus import Corpus
 from ..scorology import Scorology
-from ..blocks import Blocks, zmethods
-from ..blocks.util import sorted_hierarchical_block_index
+from ..blocks import Blocks
 
+from . import blockstate_to_dataframes
 from .domain_topic_model import create_docter_graph, calc_nested_blockstate
 from .domain_chained_model import (
     extend_graph,
     gen_doc_graph,
     calc_chained_nested_blockstate,
 )
 
@@ -52,19 +51,19 @@
         self.set_blockstate(self._to_load.pop("blockstate", None))
         self.loaded["chainedbstates"] = self._to_load.pop("chainedbstates", {})
         if graph_extend := self._to_load.pop("graph_extend", None):
             self.set_chain(**graph_extend, strict=False)
         else:
             self.unset_chain()
         self.use_cached_annotations = True
-        self.use_cached_annotations_sampled = False
+        self.use_sampled_annotations = False
         self.use_cached_cross_counts = True
 
-    ext_g = ".gt.xz"
-    ext_nbs = ".json.xz"
+    suffix_g = ".gt.xz"
+    suffix_nbs = ".json.xz"
 
     graph_name = makep_fromdict("loaded", "graph", True, None, None)
     graph_dir = property_getfuncdir(lambda self: self.data_dir / self.graph_name)
     graph_adir = property_getfuncdir(lambda self: self.data_adir / self.graph_name)
     blocks_name = makep_fromdict("loaded", "blockstate", True, None, None)
     blocks_dir = property_getfuncdir(lambda self: self.graph_dir / self.blocks_name)
     blocks_adir = property_getfuncdir(lambda self: self.graph_adir / self.blocks_name)
@@ -80,55 +79,41 @@
 
     def load_domain_topic_model(self, load=True):
         """"""
         self.cache_clear(clear_static=True)
         if not self.column:
             raise ValueError
         if not self.blocks_name or not load:
-            if not self.graph_name:
-                create_docter_graph(self)
+            create_docter_graph(self)
             self.load_graph()
             calc_nested_blockstate(self)
         self.load_blockstate()
         self.blockstate_to_dataframes()
+        if self.get_sample_hash(doc=True):
+            self.trim_to_sample()
         self.load_ter_documents()
 
-    def load_domain_chained_model(self, load=True, bext="max", anneal=False):
+    def load_domain_chained_model(
+        self, load=True, bext="max", strategy=["anneal", "sweep"]
+    ):
         """"""
         self.cache_clear(clear_static=True)
         if not (self.graph_extend and (load or self.blocks_name)):
             raise ValueError
         self.load_blockstate()
         self.blockstate_to_dataframes()
+        if self.get_sample_hash(doc=True):
+            self.trim_to_sample()
         if not self.chained_name or not load:
-            calc_chained_nested_blockstate(self, bext=bext, anneal=anneal)
+            calc_chained_nested_blockstate(self, bext=bext, strategy=strategy)
         self.load_blockstate(chained=True, keep_blocks=True)
         self.blockstate_to_dataframes()
         self.load_ter_documents()
         self.load_ext_documents()
 
-    def trim_to_sample(self):
-        self.cache_clear(clear_static=True)
-        self.use_cached_annotations = False
-        if not self.tblocks.empty:
-            self.load_ter_documents()
-            if not hasattr(self, "_orig_tblocks"):
-                self._orig_tblocks = self.tblocks.copy()
-            self.tblocks = self._orig_tblocks[
-                self._orig_tblocks.index.isin(self.ter_documents)
-            ]
-        if not self.eblocks.empty:
-            self.load_ext_documents()
-            if not hasattr(self, "_orig_eblocks"):
-                self._orig_eblocks = self.eblocks.copy()
-            self.eblocks = self._orig_eblocks[
-                self._orig_eblocks.index.isin(self.ext_documents)
-            ]
-        self.gen_mapindex()
-
     ################################################
     # Graph and blockstate methods (TODO move out) #
     ################################################
 
     def from_corpus_to_convoc(self):
         """
         Builds a bipartite undirected graph of terms connecting to the contexts
@@ -199,15 +184,15 @@
     # Graph
 
     def list_graphs(self):
         return [
             str(fpath.name)
             for fpath in self.data_dir.iterdir()
             if ioio.uncompressed_suffix(fpath)
-            == ioio.uncompressed_suffix(Path(f"_{self.ext_g}"))
+            == ioio.uncompressed_suffix(Path(f"_{self.suffix_g}"))
         ]
 
     def set_graph(self, name=None, strict=True):
         """
         Set graph to be loaded to `name`. Doesn't load the graph.
 
         name) `str` or `None` (default)
@@ -304,14 +289,15 @@
         else:
             obj = ioio.load(fpath, fmt="json")
             args = obj["args"]
             args["bs"] = list(map(numpy.array, args["bs"]))
             if chained:
                 graph = gen_doc_graph(self)
                 extend_graph(self, graph, obj["graph"]["extended"])
+                # We used to store bs data for terms and they would come first in the list
                 args["bs"][0] = args["bs"][0][-graph.num_vertices() :]
             else:
                 graph = gt.load_graph(str(self.graph_dir / obj["graph"]["name"]))
             for key, val in obj["vp_args"].items():
                 if val is not None:
                     args[key] = graph.vp[val]
             for key, val in obj["ep_args"].items():
@@ -357,17 +343,14 @@
                 [
                     "dblocks",
                     "tblocks",
                     "eblocks",
                     "_orig_dblocks",
                     "_orig_tblocks",
                     "_orig_eblocks",
-                    "dblocks_levels",
-                    "tblocks_levels",
-                    "eblocks_levels",
                 ],
             )
         clearattrs(self, ["state"])
 
     def delete_blockstate(self, blocks_name):
         if blocks_name.startswith("blockstate; "):
             blocks_dir = self.graph_dir / blocks_name
@@ -408,136 +391,24 @@
         """
         if state_list is None:
             state_list = (
                 self.list_chainedbstates() if chained else self.list_blockstates()
             )
         state_ent = {}
         for state in state_list:
-            self.set_blockstate(state, chained)
-            self.load_blockstate(chained=chained)
-            state_ent[state] = self.state.entropy()
+            try:
+                self.set_blockstate(state, chained)
+                self.load_blockstate(chained=chained)
+                state_ent[state] = self.state.entropy()
+            except Exception:
+                print(f"Invalid state: {state}")
         state_ent = dict(sorted(state_ent.items(), key=lambda x: x[1]))
         chosen_state = [*state_ent][index]
         self.set_blockstate(chosen_state, chained)
         self.clear_blockstate()
         if delete_non_best:
             for state in [state for state in state_list if state != chosen_state]:
                 self.delete_blockstate(state)
         return state_ent
 
-    # Conversion
-
     def blockstate_to_dataframes(self, nbstate=None):
-        """
-        state: the blockstate instance to be turned into dataframes indexed at
-        documents and terms
-        """
-        if nbstate is None:
-            nbstate = self.state
-        g = nbstate.g
-
-        df = pandas.DataFrame(index=[g.vp["name"][v] for v in g.vertices()])
-        df["v"] = [int(v) for v in g.vertices()]
-        df["type"] = [g.vp["type"][v] for v in g.vertices()]
-        for blevel in range(len(nbstate.levels) - 1):  # treat top blevel later
-            blocks = nbstate.project_level(blevel).get_blocks()
-            df[blevel + 1] = [blocks[v] for v in g.vertices()]
-        # include top blevel if it's vertices don't correspond to "type"
-        if len(df[blevel + 1].unique()) > 2:
-            blevel += 1
-            blocks = nbstate.project_level(blevel).get_blocks()
-            df[blevel + 1] = [blocks[v] for v in g.vertices()]
-
-        # make sure highest level matches type then replace it
-        level = blevel + 1
-        if not df.groupby("type")[level].agg(set).map(len).eq(1).all():
-            raise ValueError("multiple top level blocks for type!")
-        if not df.groupby(level)["type"].agg(set).map(len).eq(1).all():
-            raise ValueError("multiple types for top level block!")
-        df[level] = df["type"]
-
-        dblocks = df[df["type"].eq(0)]
-        tblocks = df[df["type"].eq(1)]
-        eblocks = df[df["type"].gt(1)].copy()
-
-        if tblocks.empty and not eblocks.empty:
-            # chained state: only load eblocks, with index starting after other blocks
-            self_dblocks = getattr(self, "_orig_dblocks", self.dblocks)
-            for dblocks_l, tblocks_l, eblocks_l in zip(
-                self_dblocks, self.tblocks, eblocks
-            ):
-                assert dblocks_l == tblocks_l == eblocks_l
-                eblocks_start_num = (
-                    max(
-                        self_dblocks[dblocks_l].max(),
-                        self.tblocks[tblocks_l].max(),
-                    )
-                    - eblocks[eblocks_l].min()
-                    + 1
-                )
-                eblocks[eblocks_l] = eblocks[eblocks_l].map(
-                    lambda x: x + eblocks_start_num
-                )
-            self.eblocks = eblocks
-            self.eblocks_levels = [x for x in self.eblocks if isinstance(x, int)]
-        else:
-            # align dblocks with data
-            document_ids = self.get_document_ids()
-            self.dblocks = dblocks.reindex(document_ids)
-            self.dblocks.index = self.data.index
-            self.dblocks.dropna(inplace=True)
-            # if sampled, also keep _orig_dblocks aligned with original data
-            if len(self.dblocks) < len(dblocks):
-                odata_document_ids = self.get_document_ids(self.odata)
-                if not document_ids.equals(odata_document_ids):
-                    self._orig_dblocks = dblocks.reindex(odata_document_ids)
-                    self._orig_dblocks.index = self.odata.index
-                    self._orig_dblocks.dropna(inplace=True)
-            # assign remaining blocks and block_levels
-            self.tblocks, self.eblocks = (tblocks, eblocks)
-            self.dblocks_levels, self.tblocks_levels, self.eblocks_levels = (
-                [x for x in blocks if isinstance(x, int)]
-                for blocks in (dblocks, tblocks, eblocks)
-            )
-        self.gen_block_label_correspondence()
-        self.gen_mapindex()
-
-    def gen_block_label_correspondence(self):
-        self.hblock_to_label = {}
-        self.label_to_hblock = {}
-        self.label_to_tlblock = {}
-        self.lblock_to_label = {}
-        self_dblocks = getattr(self, "_orig_dblocks", self.dblocks)
-        for blocks, levels, btype in [
-            (self_dblocks, self.dblocks_levels, "doc"),
-            (self.tblocks, self.tblocks_levels, "ter"),
-            (self.eblocks, self.eblocks_levels, "ext"),
-        ]:
-            for level in reversed(levels):
-                for i, hblock in enumerate(
-                    sorted_hierarchical_block_index(blocks, levels, level)
-                ):
-                    lblock = (level, hblock[-1])
-                    label = "L{}{}{}".format(level, btype[0].upper(), i)
-                    self.hblock_to_label[hblock] = label
-                    self.label_to_hblock[label] = hblock
-                    self.label_to_tlblock[label] = (btype, *lblock)
-                    self.lblock_to_label[(level, hblock[-1])] = label
-
-    def gen_mapindex(self):
-        self.label_to_mapindex = {}
-        self.lblock_to_mapindex = {}
-        for blocks, levels, btype in [
-            (self.dblocks, self.dblocks_levels, "doc"),
-            (self.tblocks, self.tblocks_levels, "ter"),
-            (self.eblocks, self.eblocks_levels, "ext"),
-        ]:
-            mapindex = 0
-            for level in reversed(levels):
-                for i, hblock in enumerate(
-                    sorted_hierarchical_block_index(blocks, levels, level)
-                ):
-                    lblock = (level, hblock[-1])
-                    label = self.lblock_to_label[lblock]
-                    self.label_to_mapindex[label] = mapindex
-                    self.lblock_to_mapindex[lblock] = mapindex
-                    mapindex += 1
+        return blockstate_to_dataframes.blockstate_to_dataframes(self, nbstate)
```

### Comparing `sashimi_domains-0.9.3/src/sashimi/graph_models/domain_chained_model.py` & `sashimi_domains-0.9.4/src/sashimi/graph_models/domain_chained_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,86 +19,99 @@
 from itertools import count
 import graph_tool.all as gt
 
 from ..naming import naming
 from .util import contiguous_map_nested_blockstate
 
 
-def calc_chained_nested_blockstate(corpus, bext="max", niter=10, anneal=False):
+def calc_chained_nested_blockstate(
+    corpus, bext="max", niter=10, strategy=["anneal", "sweep"]
+):
     """
     Calculates a chained nested blockstate for vertices derived from
     values of some property of the documents.
     Only works for NestedBlockState without layers or overlapping.
     (corpus)
     (niter) number of times the optimization procedure is run
     (anneal) use annealing for optimization
     :str: file name of stored state
     """
     name_args = []
     if sample := corpus.get_sample_hash(doc=True, ext=True):
-        name_args += [("sample", sample)]
+        name_args = [*name_args, ("sample", sample)]
 
     for irun in count():
         fname = naming.gen(
             "chainedbstate",
             [
                 ("prop", corpus.graph_extend["prop"]),
                 ("matcher", corpus.graph_extend["matcher"]),
                 *name_args,
                 ("run", irun),
             ],
-            corpus.ext_nbs,
+            corpus.suffix_nbs,
         )
         try:
             (corpus.blocks_dir / fname).mkdir(exist_ok=False)
             print(f"Reserved name: {fname}\n")
             break
         except OSError:
             pass
 
     print("Generating initial block state\n")
+    pclabel = "type"
+    nbstate = gen_nbstate(corpus, pclabel, bext)
+
+    print("Starting minimization from initial state:\n", nbstate)
+    nbstate = minimize_nbstate(nbstate, strategy)
+
+    fpath = corpus.blocks_dir / fname / fname
+    corpus.store_blockstate(fpath, state=nbstate, pclabel=pclabel)
+    print("Saved chained state: {}".format(fname))
+    corpus.set_blockstate(str(fname), chained=True)
+    return fpath
+
+
+def gen_nbstate(corpus, pclabel, bext):
     g = gen_doc_graph(corpus)
     extend_graph(corpus, g)
     doc_bs = gen_doc_blocks(corpus)
-    pclabel = "type"
     nbstate = gen_chained_nested_blockstate(g, doc_bs, pclabel=pclabel, bext=bext)
+    return nbstate
 
-    # WARNING: nbstate copies lose hbfields, do not optimize or get entropy on them
 
-    print("Starting minimization from initial state:\n", nbstate)
+def minimize_nbstate(nbstate, strategy):
     ent = nbstate.entropy()
+    # WARNING: nbstate copies lose hbfields, do not optimize or get entropy on them
     best_nbstate = nbstate.copy()
-    for _ in range(niter):
-        if not anneal:
+    for method in strategy:
+        if method == "sweep":
+            print("Sweeping...")
             for i in range(1000):  # this should be sufficiently large
                 nbstate.multiflip_mcmc_sweep(
                     beta=numpy.inf,
                     niter=10,
                     ls=[*range(len(nbstate.levels) - 1)],
                 )
-        else:
+        if method == "anneal":
+            print("Annealing...")
             gt.mcmc_anneal(
                 nbstate,
                 beta_range=(1, 10),
                 niter=1000,
                 mcmc_equilibrate_args=dict(
                     force_niter=10,
                     mcmc_args=dict(ls=[*range(len(nbstate.levels) - 1)]),
                 ),
             )
         if nbstate.entropy() < ent:
             ent = nbstate.entropy()
             best_nbstate = nbstate.copy()
     nbstate = contiguous_map_nested_blockstate(best_nbstate)
-
-    fpath = corpus.blocks_dir / fname / fname
-    corpus.store_blockstate(fpath, state=nbstate, pclabel=pclabel)
-    print("Saved chained state: {}".format(fname))
-    corpus.set_blockstate(str(fname), chained=True)
-    return fpath
+    return nbstate
 
 
 def gen_chained_nested_blockstate(g, bs, pclabel, bext="max"):
     """
     (g) Graph: extended graph
     (bs) Sequence[Sequence]: blockstates of doc graph
     (pclabel) Name of vertex property passed down and frozen at < 2
```

### Comparing `sashimi_domains-0.9.3/src/sashimi/graph_models/domain_topic_model.py` & `sashimi_domains-0.9.4/src/sashimi/graph_models/domain_topic_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             else by.__name__
         )
         if not name_by:
             raise ValueError
 
     def get_graph_name(name_args, group_name):
         name_args += [] if by is None else [("by", (name_by, group_name))]
-        return naming.gen("graph", name_args, corpus.ext_g)
+        return naming.gen("graph", name_args, corpus.suffix_g)
 
     graph_names = []
     for group_name, group in (
         [("all", corpus.data)] if by is None else corpus.data.groupby(by)
     ):
         print(f"Generating doc ter graph for {group_name}")
         graph_name = get_graph_name(name_args, group_name)
@@ -92,19 +92,14 @@
     return graph_names
 
 
 def gen_docter_graph(doc_tokens, doc_ids):
     """
     Builds a bipartite undirected graph of documents connecting to the terms
     they contain.
-
-    Parameters
-    ----------
-    sample: anything consumable by `samplify`
-      use the full vocabulary but only a sample of the documents
     """
     vocab = {w for d in doc_tokens for s in d for w in s}
     print("Vocab size: {}".format(len(vocab)))
     vocabindex = dict((w, n) for n, w in enumerate(vocab))
 
     g = gt.Graph(directed=False)
     g.vp["type"] = g.new_vertex_property("int")  # type = 0: document, 1: term
@@ -126,15 +121,15 @@
                     if w in vocab:
                         yield (vi, vocabindex[w])
 
     g.add_edge_list(gen_docter_edges())
     return g
 
 
-def calc_nested_blockstate(corpus, name_args=[], state_args={}):
+def calc_nested_blockstate(corpus, name_args=(), state_args={}):
     """
     Calculate and save a nested blockstate for the graph, using
     `graph_tool.inference.minimize.minimize_nested_blockmodel_dl()`.
 
     Parameters
     ----------
     g: a `graph_tool.Graph` instance
@@ -143,21 +138,21 @@
       Extra arguments to add to the blockstate filename.
     state_args: `dict`
       Passed downstream. For key "ec", value is passed as `g.ep[value]`.
     """
     state_args = state_args.copy()
 
     if sample := corpus.get_sample_hash(doc=True, ter=True):
-        name_args += [("sample", sample)]
+        name_args = [*name_args, ("sample", sample)]
 
     for irun in count():
         fname = naming.gen(
             "blockstate",
-            name_args + [("step", "mnbdl")] + [("run", irun)],
-            corpus.ext_nbs,
+            [*name_args, ("step", "mnbdl"), ("run", irun)],
+            corpus.suffix_nbs,
         )
         try:
             (corpus.graph_dir / fname).mkdir(exist_ok=False)
             print(f"Reserving name: {fname}")
             break
         except OSError:
             pass
@@ -183,14 +178,17 @@
     corpus.store_blockstate(state=state, **store_blockstate_args)
     print("Saved state: {}".format(fname))
     corpus.loaded["blockstate"] = str(fname)
     return fname
 
 
 def refine_state(state, strategy="sweep"):
+    """
+    For the "bestest" results go with ["anneal", "sweep"]
+    """
     print("Refining state...")
     if isinstance(strategy, str):
         strategy = [strategy]
     for method in strategy:
         if method == "sweep":
             for i in range(1000):
                 state.multiflip_mcmc_sweep(beta=np.inf, niter=10)
```

### Comparing `sashimi_domains-0.9.3/src/sashimi/graph_models/util.py` & `sashimi_domains-0.9.4/src/sashimi/graph_models/util.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/src/sashimi/util/asco_clean.py` & `sashimi_domains-0.9.4/src/sashimi/util/asco_clean.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/src/sashimi/util/pubmed_get.sh` & `sashimi_domains-0.9.4/src/sashimi/util/pubmed_get.sh`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/src/sashimi/util/scan_bugtrap.py` & `sashimi_domains-0.9.4/src/sashimi/util/scan_bugtrap.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/src/sashimi/util/wos_lam/__init__.py` & `sashimi_domains-0.9.4/src/sashimi/util/wos_lam/__init__.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/src/sashimi/util/wos_lam/wos_api_request.tpl` & `sashimi_domains-0.9.4/src/sashimi/util/wos_lam/wos_api_request.tpl`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/tests/test_basic_usage.py` & `sashimi_domains-0.9.4/tests/test_basic_usage.py`

 * *Files 6% similar despite different names*

```diff
@@ -142,29 +142,35 @@
     dns = corpus.domain_network(doc_level=1, ext_level=1, edges="specific")
     dnc = None
     if 2 in corpus.dblocks_levels:
         dnc = corpus.domain_network(doc_level=2, ext_level=1, edges="common")
     return dm, dns, dnc
 
 
-def load_test_corpus(name):
-    return sashimi.GraphModels(name)
+def load_test_corpus(number, kind="dtm"):
+    name = f"{number}.json.xz-{kind}.json"
+    corpus = sashimi.GraphModels(name)
+    if kind == "dtm":
+        corpus.load_domain_topic_model()
+    else:
+        corpus.load_domain_chained_model()
+    return corpus
 
 
 def cache_clear():
-    num, den = 0, 0
+    cleared, caching = 0, 0
     names_obj = globals()
     for name, obj in names_obj.items():
         if name.startswith("test_") or name.startswith("example_"):
             if hasattr(obj, "cache_clear"):
                 if obj.cache_info().currsize:
                     obj.cache_clear()
-                    num += 1
-                den += 1
-    return num, den
+                    cleared += 1
+                caching += 1
+    return {"cleared": cleared, "caching": caching}
 
 
 def gen_name_test():
     names_obj = globals()
     for name, obj in names_obj.items():
         if name.startswith("test_"):
             yield name, obj
```

### Comparing `sashimi_domains-0.9.3/tests/test_pclabel_bfield.py` & `sashimi_domains-0.9.4/tests/test_pclabel_bfield.py`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/LICENSE` & `sashimi_domains-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sashimi_domains-0.9.3/README.md` & `sashimi_domains-0.9.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 - [pandas](https://pandas.pydata.org/)
 - [spacy](https://spacy.io/) (for tokenization)
 - [gensim](https://radimrehurek.com/gensim/) (for ngram detection)
 - [bokeh](https://bokeh.org/) (for building hierarchical block maps and other plots)
 - [lxml](https://lxml.de/) (for building domain tables)
 - [matplotlib](https://matplotlib.org/) (for plotting simple corpus statistics)
 
-With the exception of graph-tool, they'll be automatically handled by `pip`.
+With the exception of graph-tool, dependencies will be automatically installed by `pip`.
 
 ## Basic usage
 
 ```python
 from sashimi import GraphModels
 import pandas as pd
 
@@ -162,22 +162,22 @@
 - Calls to `Corpus.set_chain` may pass in the `matcher` parameter a path to a json file containing a dictionary. Nodes of the chained dimension will then correspond to the keys in the dictionary, and links will be established by searching for a key's value, as a regular expression, in the column passed as the first parameter.
 
 Development
 -----------
 
 This module provides four main classes:
 
+`class Corpus`
+
+Provides loading and preprocessing corpora, plus some descriptive statistics.
+
 `class GraphModels` (user-facing class, inherits Corpus and Blocks)
 
 Provides Stochastic Block Models of corpora from their document-term and document-metadata graphs, yielding domain-topic and domain-chained models, respectively.
 
 `class Blocks`
 
 Provides interactive domain maps, networks, tables, and other interfaces.
 
-`class Corpus`
-
-Provides loading and preprocessing corpora, plus some descriptive statistics.
-
 `class Vectorology` [currently deprecated]
 
 Provides models of corpora using word embedding and produces reports, statistics and visualisations.
```

### Comparing `sashimi_domains-0.9.3/pyproject.toml` & `sashimi_domains-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -67,7 +67,9 @@
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
+
+[tool.black]
```

### Comparing `sashimi_domains-0.9.3/PKG-INFO` & `sashimi_domains-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: sashimi-domains
-Version: 0.9.3
+Version: 0.9.4
 Summary: Sashimi is a Python module that provides tailored mathematical models and corresponding interactive visualisations for exploratory and confirmatory mixed-methods analysis of large textual or token corpora. It can detect textual and metadata structures and shifts, by employing stochastic block modeling (SBM) from graph-tool or [currently deprecated] word embedding from Gensim.
 Project-URL: Documentation, https://gitlab.com/solstag/sashimi/
 Project-URL: Issues, https://gitlab.com/solstag/sashimi/-/issues
 Project-URL: Source, https://gitlab.com/solstag/sashimi/
 Author-email: Ale Abdo <abdo@member.fsf.org>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
@@ -67,15 +67,15 @@
 - [pandas](https://pandas.pydata.org/)
 - [spacy](https://spacy.io/) (for tokenization)
 - [gensim](https://radimrehurek.com/gensim/) (for ngram detection)
 - [bokeh](https://bokeh.org/) (for building hierarchical block maps and other plots)
 - [lxml](https://lxml.de/) (for building domain tables)
 - [matplotlib](https://matplotlib.org/) (for plotting simple corpus statistics)
 
-With the exception of graph-tool, they'll be automatically handled by `pip`.
+With the exception of graph-tool, dependencies will be automatically installed by `pip`.
 
 ## Basic usage
 
 ```python
 from sashimi import GraphModels
 import pandas as pd
 
@@ -190,22 +190,22 @@
 - Calls to `Corpus.set_chain` may pass in the `matcher` parameter a path to a json file containing a dictionary. Nodes of the chained dimension will then correspond to the keys in the dictionary, and links will be established by searching for a key's value, as a regular expression, in the column passed as the first parameter.
 
 Development
 -----------
 
 This module provides four main classes:
 
+`class Corpus`
+
+Provides loading and preprocessing corpora, plus some descriptive statistics.
+
 `class GraphModels` (user-facing class, inherits Corpus and Blocks)
 
 Provides Stochastic Block Models of corpora from their document-term and document-metadata graphs, yielding domain-topic and domain-chained models, respectively.
 
 `class Blocks`
 
 Provides interactive domain maps, networks, tables, and other interfaces.
 
-`class Corpus`
-
-Provides loading and preprocessing corpora, plus some descriptive statistics.
-
 `class Vectorology` [currently deprecated]
 
 Provides models of corpora using word embedding and produces reports, statistics and visualisations.
```

