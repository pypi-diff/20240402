# Comparing `tmp/pybts-1.2.1.tar.gz` & `tmp/pybts-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybts-1.2.1.tar", last modified: Mon Apr  1 13:56:44 2024, max compression
+gzip compressed data, was "pybts-1.3.0.tar", max compression
```

## Comparing `pybts-1.2.1.tar` & `pybts-1.3.0.tar`

### file list

```diff
@@ -1,39 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:56:44.529909 pybts-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-01 13:56:40.000000 pybts-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-04-01 13:56:44.529909 pybts-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-01 13:56:40.000000 pybts-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:56:44.525909 pybts-1.2.1/pybts/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-01 13:56:40.000000 pybts-1.2.1/pybts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-01 13:56:40.000000 pybts-1.2.1/pybts/board.py
--rw-r--r--   0 runner    (1001) docker     (127)    11046 2024-04-01 13:56:40.000000 pybts-1.2.1/pybts/board_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-01 13:56:40.000000 pybts-1.2.1/pybts/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:56:44.525909 pybts-1.2.1/pybts/composites/
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-01 13:56:40.000000 pybts-1.2.1/pybts/composites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-04-01 13:56:40.000000 pybts-1.2.1/pybts/composites/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-01 13:56:40.000000 pybts-1.2.1/pybts/composites/condition_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-04-01 13:56:40.000000 pybts-1.2.1/pybts/composites/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-01 13:56:40.000000 pybts-1.2.1/pybts/composites/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-01 13:56:40.000000 pybts-1.2.1/pybts/composites/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-01 13:56:40.000000 pybts-1.2.1/pybts/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:56:44.525909 pybts-1.2.1/pybts/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-01 13:56:40.000000 pybts-1.2.1/pybts/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17159 2024-04-01 13:56:40.000000 pybts-1.2.1/pybts/decorators/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-01 13:56:40.000000 pybts-1.2.1/pybts/node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:56:44.525909 pybts-1.2.1/pybts/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    16958 2024-04-01 13:56:40.000000 pybts-1.2.1/pybts/templates/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-01 13:56:40.000000 pybts-1.2.1/pybts/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:56:44.529909 pybts-1.2.1/pybts/templates/static/
--rw-r--r--   0 runner    (1001) docker     (127)  1966405 2024-04-01 13:56:40.000000 pybts-1.2.1/pybts/templates/static/index-BUWP2os5.js
--rw-r--r--   0 runner    (1001) docker     (127)   320362 2024-04-01 13:56:40.000000 pybts-1.2.1/pybts/templates/static/index-BXdrQGHp.css
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-01 13:56:40.000000 pybts-1.2.1/pybts/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-01 13:56:40.000000 pybts-1.2.1/pybts/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:56:44.529909 pybts-1.2.1/pybts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-04-01 13:56:44.000000 pybts-1.2.1/pybts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-01 13:56:44.000000 pybts-1.2.1/pybts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 13:56:44.000000 pybts-1.2.1/pybts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-01 13:56:44.000000 pybts-1.2.1/pybts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-01 13:56:44.000000 pybts-1.2.1/pybts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 13:56:44.000000 pybts-1.2.1/pybts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-01 13:56:40.000000 pybts-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 13:56:44.529909 pybts-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-01 13:56:40.000000 pybts-1.2.1/setup.py
+-rw-r--r--   0        0        0   157658 2024-04-02 06:31:57.977077 pybts-1.3.0/README.assets/DEMO_Sequence  10-10 _ 100.png
+-rw-r--r--   0        0        0   189323 2024-04-02 06:31:57.977077 pybts-1.3.0/README.assets/image-20240329031220580.png
+-rw-r--r--   0        0        0   208202 2024-04-02 06:31:57.981077 pybts-1.3.0/README.assets/image-20240329031233459.png
+-rw-r--r--   0        0        0   255608 2024-04-02 06:31:57.981077 pybts-1.3.0/README.assets/image-20240401211552611.png
+-rw-r--r--   0        0        0   202283 2024-04-02 06:31:57.981077 pybts-1.3.0/README.assets/image-20240401211609525.png
+-rw-r--r--   0        0        0     5830 2024-04-02 06:31:57.981077 pybts-1.3.0/README.md
+-rw-r--r--   0        0        0      420 2024-04-02 06:31:57.981077 pybts-1.3.0/pybts/__init__.py
+-rw-r--r--   0        0        0     2355 2024-04-02 06:31:57.981077 pybts-1.3.0/pybts/board.py
+-rw-r--r--   0        0        0    10108 2024-04-02 06:31:57.981077 pybts-1.3.0/pybts/board_server.py
+-rw-r--r--   0        0        0     4001 2024-04-02 06:31:57.981077 pybts-1.3.0/pybts/builder.py
+-rw-r--r--   0        0        0      473 2024-04-02 06:31:57.985077 pybts-1.3.0/pybts/composites/__init__.py
+-rw-r--r--   0        0        0     8710 2024-04-02 06:31:57.985077 pybts-1.3.0/pybts/composites/composite.py
+-rw-r--r--   0        0        0     2420 2024-04-02 06:31:57.985077 pybts-1.3.0/pybts/composites/condition_branch.py
+-rw-r--r--   0        0        0     5970 2024-04-02 06:31:57.985077 pybts-1.3.0/pybts/composites/parallel.py
+-rw-r--r--   0        0        0     2317 2024-04-02 06:31:57.985077 pybts-1.3.0/pybts/composites/selector.py
+-rw-r--r--   0        0        0     2541 2024-04-02 06:31:57.985077 pybts-1.3.0/pybts/composites/sequence.py
+-rw-r--r--   0        0        0     3220 2024-04-02 06:31:57.985077 pybts-1.3.0/pybts/constants.py
+-rw-r--r--   0        0        0      121 2024-04-02 06:31:57.985077 pybts-1.3.0/pybts/decorators/__init__.py
+-rw-r--r--   0        0        0    17159 2024-04-02 06:31:57.985077 pybts-1.3.0/pybts/decorators/nodes.py
+-rw-r--r--   0        0        0     1145 2024-04-02 06:31:57.985077 pybts-1.3.0/pybts/main.py
+-rw-r--r--   0        0        0     5112 2024-04-02 06:31:57.985077 pybts-1.3.0/pybts/node.py
+-rw-r--r--   0        0        0    16958 2024-04-02 06:31:57.985077 pybts-1.3.0/pybts/templates/favicon.ico
+-rw-r--r--   0        0        0      433 2024-04-02 06:31:57.985077 pybts-1.3.0/pybts/templates/index.html
+-rw-r--r--   0        0        0  1966405 2024-04-02 06:31:57.993077 pybts-1.3.0/pybts/templates/static/index-BUWP2os5.js
+-rw-r--r--   0        0        0   320362 2024-04-02 06:31:57.997077 pybts-1.3.0/pybts/templates/static/index-BXdrQGHp.css
+-rw-r--r--   0        0        0      506 2024-04-02 06:31:57.997077 pybts-1.3.0/pybts/tree.py
+-rw-r--r--   0        0        0     7683 2024-04-02 06:31:57.997077 pybts-1.3.0/pybts/utility.py
+-rw-r--r--   0        0        0      610 2024-04-02 06:31:57.997077 pybts-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6551 1970-01-01 00:00:00.000000 pybts-1.3.0/PKG-INFO
```

### Comparing `pybts-1.2.1/PKG-INFO` & `pybts-1.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 Metadata-Version: 2.1
 Name: pybts
-Version: 1.2.1
-Summary: pybts is a Python library for creating, managing, and visualizing behavior trees. It supports loading and exporting behavior trees from JSON and XML files, enables real-time visualization of execution processes, and allows for analysis of historical data
+Version: 1.3.0
+Summary: 
 Home-page: https://github.com/wangtong2015/pybts
-Author: Wang Tong
-Author-email: astroboythu@gmail.com
-License: MIT
-Keywords: Behavior Tree Reinforcement Learning
-Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Games/Entertainment :: Simulation
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Keywords: BehaviorTree,AI
+Author: 王童
+Author-email: 785271992@qq.com
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: flask (>=3.0.2,<4.0.0)
+Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: py-trees (>=2.2.3,<3.0.0)
+Project-URL: Repository, https://github.com/wangtong2015/pybts
 Description-Content-Type: text/markdown
-Requires-Dist: py-trees>=2.2.3
-Requires-Dist: jinja2>=3.1.2
-Requires-Dist: PyYAML>=6.0.1
-Requires-Dist: flask~=3.0.2
-Requires-Dist: jsonpickle~=3.0.3
-Requires-Dist: numpy
 
 # PYBTS - Python Behavior Tree
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pybts.svg)](https://pypi.org/project/pybts/)
 [![License](https://img.shields.io/pypi/l/pybts.svg)](https://github.com/wangtong2015/pybts)
 [![Package Status](https://img.shields.io/pypi/status/pybts.svg)](https://pypi.org/project/pybts/)
 
@@ -148,7 +144,8 @@
 For more information about `py_trees` and to access its source code, visit the official GitHub repository: [py_trees on GitHub](https://github.com/splintered-reality/py_trees).
 
 We appreciate the effort and expertise that has gone into `py_trees`, making it possible for us to develop advanced features in pybts and offer a comprehensive behavior tree solution in the Python ecosystem.
 
 ## Development and Contributions
 
 Contributions to pybts are welcome! You can contribute by submitting issues, providing updates to documentation, or submitting pull requests with new features or bug fixes.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pybts-1.2.1/README.md` & `pybts-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pybts-1.2.1/pybts/board.py` & `pybts-1.3.0/pybts/board.py`

 * *Files identical despite different names*

### Comparing `pybts-1.2.1/pybts/board_server.py` & `pybts-1.3.0/pybts/board_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -257,35 +257,9 @@
             'title'   : f"{project}  {log_data['round']}-{log_data['step']} / {log_data['id']}",
             'id'      : log_data['id'],
             'page'    : log_data['id'],
             'total'   : pybts_data['id']
         })
 
 
-def directory_type(path):
-    if not os.path.isdir(path):
-        raise argparse.ArgumentTypeError(f"{path} is not a valid directory")
-    return path
 
 
-def main():
-    # 创建 ArgumentParser 对象
-    parser = argparse.ArgumentParser(description="A simple program to demonstrate argparse")
-
-    # 添加选项标志
-    parser.add_argument("--dir", type=directory_type, help="Path to the log directory", required=True)
-    # 添加debug参数
-    parser.add_argument("--debug", action="store_true", help="Enable debug mode")
-    # 添加host参数
-    parser.add_argument("--host", default="localhost", help="Host address")
-    # 添加port参数
-    parser.add_argument("--port", type=int, default=10000, help="Port number")
-
-    # 解析命令行参数
-    args = parser.parse_args()
-
-    server = BoardServer(log_dir=args.dir, debug=args.debug, host=args.host, port=args.port)
-    server.run()
-
-
-if __name__ == '__main__':
-    main()
```

### Comparing `pybts-1.2.1/pybts/builder.py` & `pybts-1.3.0/pybts/builder.py`

 * *Files identical despite different names*

### Comparing `pybts-1.2.1/pybts/composites/composite.py` & `pybts-1.3.0/pybts/composites/composite.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         child.parent = self
         return child.id
 
 
 def _SEQ_SEL_tick(self: Composite, tick_again_status: list[Status], continue_status: list[Status],
                   no_child_status: Status):
     """Sequence/Selector的tick逻辑"""
-    self._tick_count += 1
+    self._debug_info['tick_count'] += 1
     self.logger.debug("%s.tick()" % (self.__class__.__name__))
 
     if self.status in tick_again_status:
         # 重新执行上次执行的子节点
         assert self.current_child is not None
         index = self.children.index(self.current_child)
     else:
```

### Comparing `pybts-1.2.1/pybts/composites/condition_branch.py` & `pybts-1.3.0/pybts/composites/condition_branch.py`

 * *Files identical despite different names*

### Comparing `pybts-1.2.1/pybts/composites/parallel.py` & `pybts-1.3.0/pybts/composites/parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             - 如果有子节点返回 RUNNING 状态，节点本身返回 RUNNING
             - 子节点的执行不依赖于其它子节点的状态；每个子节点独立执行
             - 如果达到或超过指定的成功阈值（success_threshold），则返回 SUCCESS
             - 如果未达到成功阈值，即使所有子节点都已完成执行，也返回 FAILURE
             - RUNNING 状态的子节点在下一次tick时会继续执行，非RUNNING状态的子节点在下一次tick时会重置并重新开始
             - success_threshold 设置为 -1 表示所有子节点都必须成功才算总体成功
             """
-        self._tick_count += 1
+        self._debug_info['tick_count'] += 1
         self.logger.debug("%s.tick()" % (self.__class__.__name__))
 
         self.current_child = None
 
         for i, child in enumerate(self.children):
             self.current_child = child
             yield from child.tick()
```

### Comparing `pybts-1.2.1/pybts/composites/selector.py` & `pybts-1.3.0/pybts/composites/selector.py`

 * *Files identical despite different names*

### Comparing `pybts-1.2.1/pybts/composites/sequence.py` & `pybts-1.3.0/pybts/composites/sequence.py`

 * *Files identical despite different names*

### Comparing `pybts-1.2.1/pybts/constants.py` & `pybts-1.3.0/pybts/constants.py`

 * *Files identical despite different names*

### Comparing `pybts-1.2.1/pybts/decorators/nodes.py` & `pybts-1.3.0/pybts/decorators/nodes.py`

 * *Files identical despite different names*

### Comparing `pybts-1.2.1/pybts/node.py` & `pybts-1.3.0/pybts/node.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,46 +29,59 @@
     下一次tick的时候状态一开始是RUNNING，则直接调用
     update
 
     """
 
     def __init__(self, name: str = ''):
         super().__init__(name=name or self.__class__.__name__)
-        self._terminate_count = 0
-        self._update_count = 0
-        self._tick_count = 0
-        self._initialise_count = 0
-        self._reset_count = 0
+        self._updater_iter = None
+        self._debug_info = {
+            'tick_count'      : 0,
+            'update_count'    : 0,
+            'reset_count'     : 0,
+            'terminate_count' : 0,
+            'initialise_count': 0
+        }
 
     def reset(self):
-        self._reset_count += 1
+        self._debug_info['reset_count'] += 1
+        self._updater_iter = None
         if self.status != Status.INVALID:
             self.stop(Status.INVALID)
 
     @classmethod
     def creator(cls, d: dict, c: list):
         return cls(name=d['name'])
 
     def to_data(self):
         # 在board上查看的信息
         return {
-            '_reset_count'     : self._reset_count,
-            '_initialise_count': self._initialise_count,
-            '_tick_count'      : self._tick_count,
-            '_update_count'    : self._update_count,
-            '_terminate_count' : self._terminate_count
+            '_debug_info': self._debug_info,
         }
 
     def update(self) -> Status:
         self.logger.debug("%s.update()" % (self.__class__.__name__))
-        self._update_count += 1
-        return Status.INVALID
+        self._debug_info['update_count'] += 1
+        if self._updater_iter is None:
+            self._updater_iter = self.updater()
+        new_status = Status.INVALID
+        for _ in range(2):
+            try:
+                new_status = next(self._updater_iter)
+                break
+            except:
+                self._updater_iter = self.updater()
+        return new_status
+
+    def updater(self) -> typing.Iterator[Status]:
+        yield Status.INVALID
+        return
 
     def tick(self) -> typing.Iterator[Behaviour]:
-        self._tick_count += 1
+        self._debug_info['tick_count'] += 1
         self.logger.debug("%s.tick()" % (self.__class__.__name__))
 
         if self.status != Status.RUNNING:
             # 开始的状态不是RUNNING
             self.initialise()
 
         # don't set self.status yet, terminate() may need to check what the current state is first
@@ -111,21 +124,20 @@
         self.logger.debug(
                 "%s.terminate(%s)"
                 % (
                     self.__class__.__name__,
                     "%s->%s" % (self.status, new_status)
                 )
         )
-        self._terminate_count += 1
+        self._debug_info['terminate_count'] += 1
 
     def initialise(self) -> None:
         super().initialise()
         self.logger.debug("%s.initialise()" % (self.__class__.__name__))
-        self._initialise_count += 1
-
+        self._debug_info['initialise_count'] += 1
 
 
 class Action(Node, ABC):
     """
     行为节点
     """
```

### Comparing `pybts-1.2.1/pybts/templates/favicon.ico` & `pybts-1.3.0/pybts/templates/favicon.ico`

 * *Files identical despite different names*

### Comparing `pybts-1.2.1/pybts/templates/static/index-BUWP2os5.js` & `pybts-1.3.0/pybts/templates/static/index-BUWP2os5.js`

 * *Files identical despite different names*

### Comparing `pybts-1.2.1/pybts/templates/static/index-BXdrQGHp.css` & `pybts-1.3.0/pybts/templates/static/index-BXdrQGHp.css`

 * *Files identical despite different names*

### Comparing `pybts-1.2.1/pybts/utility.py` & `pybts-1.3.0/pybts/utility.py`

 * *Files identical despite different names*

