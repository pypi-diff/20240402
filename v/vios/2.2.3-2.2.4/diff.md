# Comparing `tmp/vios-2.2.3-py3-none-any.whl.zip` & `tmp/vios-2.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 48174 bytes, number of entries: 25
+Zip file size: 48178 bytes, number of entries: 25
 -rw-rw-rw-  2.0 fat     2858 b- defN 24-Mar-19 11:19 quark/__main__.py
--rw-rw-rw-  2.0 fat    24025 b- defN 24-Mar-31 14:07 quark/proxy.py
+-rw-rw-rw-  2.0 fat    24139 b- defN 24-Apr-01 15:29 quark/proxy.py
 -rw-rw-rw-  2.0 fat    18861 b- defN 24-Mar-21 10:46 quark/app/__init__.py
 -rw-rw-rw-  2.0 fat     2575 b- defN 24-Mar-19 11:19 quark/app/_data.py
 -rw-rw-rw-  2.0 fat    10205 b- defN 24-Mar-19 11:19 quark/app/demo.py
 -rw-rw-rw-  2.0 fat     9043 b- defN 24-Mar-19 11:19 quark/app/task.py
 -rw-rw-rw-  2.0 fat     5876 b- defN 24-Mar-19 11:19 quark/app/uapi.py
 -rw-rw-rw-  2.0 fat     7914 b- defN 24-Mar-19 11:19 quark/driver/VirtualDevice.py
 -rw-rw-rw-  2.0 fat      386 b- defN 24-Mar-19 11:19 quark/driver/__init__.py
@@ -15,13 +15,13 @@
 -rw-rw-rw-  2.0 fat     1188 b- defN 24-Mar-19 11:19 quark/envelope/__init__.py
 -rw-rw-rw-  2.0 fat    15111 b- defN 24-Mar-19 11:19 quark/envelope/assembler.py
 -rw-rw-rw-  2.0 fat     4322 b- defN 24-Mar-19 11:19 quark/envelope/calculator.py
 -rw-rw-rw-  2.0 fat     1106 b- defN 24-Mar-19 11:19 quark/envelope/device.py
 -rw-rw-rw-  2.0 fat     3758 b- defN 24-Mar-23 03:45 quark/envelope/processor.py
 -rw-rw-rw-  2.0 fat     4128 b- defN 24-Mar-31 13:58 quark/envelope/router.py
 -rw-rw-rw-  2.0 fat     2841 b- defN 24-Mar-21 12:16 quark/envelope/systemq.py
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Mar-31 14:08 vios-2.2.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1211 b- defN 24-Mar-31 14:08 vios-2.2.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-31 14:08 vios-2.2.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Mar-31 14:08 vios-2.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1995 b- defN 24-Mar-31 14:08 vios-2.2.3.dist-info/RECORD
-25 files, 133376 bytes uncompressed, 44998 bytes compressed:  66.3%
+-rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-01 22:22 vios-2.2.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1211 b- defN 24-Apr-01 22:22 vios-2.2.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-01 22:22 vios-2.2.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-01 22:22 vios-2.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1995 b- defN 24-Apr-01 22:22 vios-2.2.4.dist-info/RECORD
+25 files, 133490 bytes uncompressed, 45002 bytes compressed:  66.3%
```

## zipnote {}

```diff
@@ -54,23 +54,23 @@
 
 Filename: quark/envelope/router.py
 Comment: 
 
 Filename: quark/envelope/systemq.py
 Comment: 
 
-Filename: vios-2.2.3.dist-info/LICENSE
+Filename: vios-2.2.4.dist-info/LICENSE
 Comment: 
 
-Filename: vios-2.2.3.dist-info/METADATA
+Filename: vios-2.2.4.dist-info/METADATA
 Comment: 
 
-Filename: vios-2.2.3.dist-info/WHEEL
+Filename: vios-2.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: vios-2.2.3.dist-info/top_level.txt
+Filename: vios-2.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: vios-2.2.3.dist-info/RECORD
+Filename: vios-2.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## quark/proxy.py

```diff
@@ -349,23 +349,22 @@
         if self.update():
             self.progress.display()
             return
         self.handles[self.tid] = asyncio.get_running_loop(
         ).call_later(interval, self.refresh, *(interval,))
 
 
-class QuarkProxy(object):
+class QuarkCloud(object):
     """负载均衡，代理分发
     """
 
     # TABLE = {'#8': {'host': '127.0.0.1', 'port': 20888}}
 
     SHOTS = 1024
     router = {}
-    syscon = {}
 
     perf = """| CHIP: {chip:<10} | CPU: {cpu:<6}% | MEM: {mem:<6}% | SPS: {sps:<10.1f}KB/s | RPS: {rps:<10.1f}KB/s |"""
 
     def __init__(self) -> None:
         setlog()
         from .app import sql
 
@@ -389,164 +388,254 @@
         router = Path.home()/'Desktop/home/router.json'
         if not router.exists():
             router.parent.mkdir(parents=True, exist_ok=True)
             with open(router, 'w') as f:
                 f.write(json.dumps({}))
 
         with open(router, 'r') as f:
-            table = json.loads(f.read())
-            for chip, value in table.items():
+            self._router = json.loads(f.read())
+            for chip, value in self._router.items():
                 self.router[chip] = connect('QuarkProxy',
                                             host=value['host'],
-                                            port=value.get('port', 3088))
+                                            port=value.get('port', 3087))
 
         logger.info(f'server list:\r\n{self.router}')
 
-        if self.router:
-            logger.info('Start to collect system info!')
-            self.lock = Lock()
-            self.tracer = {}
-            mth = Thread(target=self.sysinfo, daemon=True)
-            mth.start()
+        self.lock = Lock()
+        self.tracer = {}
+        mth = Thread(target=self.sysinfo, daemon=True)
+        mth.start()
 
-    def submit(self, task: dict, block: bool = False):
+    def submit(self, task: dict):
         from .app import submit
 
+        # by master
+        chip, name = task['metainfo']['name'].split(':/')
+        backend = self.router[chip]
+        eid = task['metainfo']['quafu']['tid']  # external id
+        with self.lock:
+            t: Task = submit(task, block=False, backend=backend)
+        ctime = time.strftime('%Y-%m-%d-%H-%M-%S')
         try:
-            # by master
-            chip, name = task['metainfo']['name'].split(':/')
-            backend = self.router[chip]
-            eid = task['metainfo']['quafu']['tid']  # external id
-            with self.lock:
-                t: Task = submit(task, block=False, backend=backend)
-            ctime = time.strftime('%Y-%m-%d-%H-%M-%S')
-            try:
-                sql = f'''INSERT INTO proxy (TID, EID, NAME, SYSTEM, CREATED) VALUES (
-                    "{t.tid}","{eid}","{name}","{chip}","{ctime}")'''
-                self.dbcon.execute(sql)
-                self.dbcon.commit()
-            except Exception as e:
-                logger.critical(
-                    f'Failed to add record[{sql}] to proxy table: {e}!')
-                import traceback
-                traceback.print_exc()
-            logger.info(f'task will be executed on {chip}!')
-        except KeyError as e:
-            # by server
-            # logger.info(f'task will be executed on local machine: {chip}!')
-            logger.warning(f'\n\n\n{"#"*80} task start to run ...\n')
-
-            try:
-                from home.ylfeng.cloud import get_bias_of_coupler
-                bias = get_bias_of_coupler()
-            except Exception as e:
-                bias = []
-                logger.error(f'Failed to get bias of coupler, {e}!')
-            circuit = [bias+c for c in task['taskinfo']['CIRQ']]
-            task['taskinfo']['CIRQ'] = circuit
-
-            qlisp = ',\n'.join([str(op) for op in circuit[0]])
-            qasm = task['metainfo']['quafu']['qasm']
-            logger.info(f"\n{'>'*36}qasm:\n{qasm}\n{'>'*36}qlisp:\n[{qlisp}]")
-
-            t: Task = submit(task, block=block)  # local machine
-            if block:
-                t.bar(0.2, disable=False)  # if block is True
-            eid = task['metainfo']['quafu']['tid']
-            logger.warning(f'task {t.tid}[{eid}] will be executed on {chip}!')
+            sql = f'''INSERT INTO proxy (TID, EID, NAME, SYSTEM, CREATED) VALUES (
+                "{t.tid}","{eid}","{name}","{chip}","{ctime}")'''
+            self.dbcon.execute(sql)
+            self.dbcon.commit()
+        except Exception as e:
+            logger.critical(
+                f'Failed to add record[{sql}] to proxy table: {e}!')
+            import traceback
+            traceback.print_exc()
+        logger.info(f'task will be executed on {chip}!')
         return t.tid
-        # t.bar(0.1, True)
-
-        # ret = {}
-        # for kv in t.result()['count']:
-        #     base = tuple(kv[:-1])
-        #     ret[base] = ret.get(base, 0)+kv[-1]
-
-        # return ret, t.status()['status']
 
     def run(self, task: dict, block: bool = False):
         """提交任务，并生成固定格式任务
 
         Args:
             task (dict): 任务描述，详见例子.
 
         Example: task例子
             ``` {.py3 linenumb="1"}
             {
-                'chip':'SCQ136', # chip name
-                'name': 'MyJob', # task name
+                'chip':'SCQ136', # required, chip name
+                'name': 'MyJob', # required, task name
+                'shots':1024, # required, shots
 
                 'tid':'', # task id from quafu
                 'token':'', # quafu token
                 'qasm': '',
-                'systemid':6, # systemid for quafu
-                'circuit':[(('Measure', 0), 'Q1001')],# qlisp
-                'shots':1024,
+                'qlisp':[(('Measure', 0), 'Q1001')], # required,  qlisp
 
             }
             ```
         """
         # transpile the circiut here and run
         # transpile(task)
+        try:
+            systemid = self._router[task['chip']]['ssid']
+        except KeyError as e:
+            return f'chip not found, {e}!'
+
         shots = task['shots']
 
         measure = []
-        for ops in task['circuit']:
+        for ops in task['qlisp']:
             if isinstance(ops[0], tuple) and ops[0][0] == 'Measure':
                 measure.append((ops[0][1], ops[1]))
-        circuit = [task['circuit']]
+        circuit = [task['qlisp']]
         repeat = 1 if shots <= 1000 else (shots+self.SHOTS-1)//self.SHOTS
 
         cloud = {'metainfo': {'name': f'{task["chip"]}:/{task["name"]}',
                               'priority': 1,
                               'other': {'shots': 1024,
                                         'signal': 'count',
                                         'standby': True,
                                         'measure': measure},
                               'quafu': {'tid': task.get('tid', ''),  # int('task_id', 16),  # 42229EA0373A3AB2
                                         'token': task.get('token', ''),
                                         'qasm': task.get('qasm', ''),
-                                        'qlisp': circuit[0],
-                                        'systemid': task.get('systemid', '')}
+                                        'qlisp': '['+',\n'.join([str(op) for op in circuit[0]])+']',
+                                        'systemid': systemid}
                               },
                  'taskinfo': {'STEP': {'main': ['WRITE', ('repeat',)],
                                        'trigger': ['WRITE', 'trig'],
                                        'READ': ['READ', 'read']},
                               'CIRQ': circuit*repeat,
                               'LOOP': {'repeat': [('repeat', np.arange(repeat), '1')]}
                               },
                  }
-        return self.submit(cloud, block)
+        return self.submit(cloud)
 
     def status(self, tid: int):
         pass
 
-    def result(self, tid: int, raw: bool = False):
+    def result(self, tid: int, circuit: bool = False):
         """根据任务id获取结果
 
         Args:
             tid (int): 任务id
 
         Returns:
             dict: 数据及任务元信息
         """
-        from .app import get_data_by_tid, get_record_by_tid
+        from .app import get_record_by_tid
         try:
-            if self.router:  # proxy
-                record = get_record_by_tid(tid, 'proxy')
+            record = get_record_by_tid(tid, 'proxy')
+            with self.lock:
+                result: dict = self.router[record[-2]].result(record[1])
+            return result
+        except Exception as e:
+            return f'No data found for {tid}!'
+
+    def update(self, backend: str, info: dict):
+        quafuos = str(Path.home()/'Desktop/qusteed0.1.1')
+        if quafuos not in sys.path:
+            print('adding quafuos', quafuos)
+            sys.path.append(quafuos)
+        with open(f'{backend}.json', 'w') as f:
+            f.write(json.dumps(info, indent=4))
+        from qusteedAPIs import call_local_backend_api
+        call_local_backend_api(backend=backend, chip_info_dict=info)
+        logger.warning(f'database of {backend} updated!')
+        return f'database of {backend} updated!'
+
+    def iterate(self):
+        pass
+
+    def getid(self, name: str, start: str, stop: str):
+        """根据名字获取所有在指定时间范围内的任务id列表
+
+        Args:
+            name (str): 任务名字
+            start (str): 起始时间，格式为2000-01-01-12-34-56，至少包含年月
+            stop (str): 结束时间，格式为2000-01-01-12-34-56，至少包含年月
+
+        Returns:
+            list: 所有任务的id
+        """
+        from .app import get_record_list_by_name
+        records = get_record_list_by_name(name, start, stop, 'proxy')
+        return [r[1] for r in records]
+
+    def sysinfo(self):
+        while True:
+            print('='*94)
+            info = self.tracer[time.strftime('%Y-%m-%d %H:%M:%S')] = {}
+            for chip, conn in self.router.items():
+                # if chip != 'Baiwang':
+                #     continue
                 with self.lock:
-                    result: dict = self.router[record[-2]].result(record[1])
-                return result if raw else self.process(result)
-            else:  # local
-                return get_data_by_tid(tid, 'count')
+                    info[chip] = conn.sysinfo()
+                try:
+                    print(self.perf.format(
+                        **({'chip': chip} | info[chip])))
+                except Exception as e:
+                    logger.error(f'Failed to print perf info, {e}!')
+            # print(info)
+            print('='*94)
+            time.sleep(5)
+            if len(self.tracer) > 1000:
+                ts = time.strftime('%Y%m%d%H%M%S')
+                pf = Path.home()/f'Desktop/home/log/proxy/perf/{ts}.json'
+                pf.parent.mkdir(parents=True, exist_ok=True)
+                with open(pf, 'w') as f:
+                    f.write(json.dumps(self.tracer, indent=4))
+                    self.tracer.clear()
+
+    def snr(self, data):
+        return data
+
+
+class QuarkProxy(object):
+    """云客户端
+    """
+
+    def __init__(self) -> None:
+        from .app import login
+
+        self.server = login()
+        setlog()
+
+    def submit(self, task: dict, block: bool = False):
+        from .app import submit
+
+        # by server
+        # logger.info(f'task will be executed on local machine: {chip}!')
+        logger.warning(f'\n\n\n{"#"*80} task start to run ...\n')
+
+        try:
+            from home.ylfeng.cloud import get_bias_of_coupler
+            bias = get_bias_of_coupler()
+        except Exception as e:
+            bias = []
+            logger.error(f'Failed to get bias of coupler, {e}!')
+        circuit = [bias+c for c in task['taskinfo']['CIRQ']]
+        task['taskinfo']['CIRQ'] = circuit
+
+        qlisp = ',\n'.join([str(op) for op in circuit[0]])
+        qasm = task['metainfo']['quafu']['qasm']
+        logger.info(f"\n{'>'*36}qasm:\n{qasm}\n{'>'*36}qlisp:\n[{qlisp}]")
+
+        t: Task = submit(task, block=block)  # local machine
+        if block:
+            t.bar(0.2, disable=False)  # if block is True
+        eid = task['metainfo']['quafu']['tid']
+        logger.warning(f'task {t.tid}[{eid}] will be executed!')
+
+        return t.tid
+        # t.bar(0.1, True)
+
+        # ret = {}
+        # for kv in t.result()['count']:
+        #     base = tuple(kv[:-1])
+        #     ret[base] = ret.get(base, 0)+kv[-1]
+
+        # return ret, t.status()['status']
+
+    def status(self, tid: int):
+        pass
+
+    def result(self, tid: int):
+        """根据任务id获取结果
+
+        Args:
+            tid (int): 任务id
+
+        Returns:
+            dict: 数据及任务元信息
+        """
+        from .app import get_data_by_tid
+        try:
+            return self.process(get_data_by_tid(tid, 'count'))
         except Exception as e:
             return f'No data found for {tid}!'
 
     @classmethod
-    def process(cls, result: dict):
+    def process(cls, result: dict, circuit: bool = False):
         def _delete_dict(ret: dict, num: int = 0):
             while num > 0:
                 tmp = np.cumsum(list(ret.values()))
                 ran_num = np.random.randint(tmp[-1]+1)
                 ran_pos = np.searchsorted(tmp, ran_num)
                 ret[list(ret.keys())[ran_pos]] -= 1
                 if ret[list(ret.keys())[ran_pos]] == 0:
@@ -579,85 +668,22 @@
                 shots = meta['other']['shots'] * \
                     len(meta['axis']['repeat']['repeat'])
                 _delete_dict(dres, shots - (shots//1000)*1000)
             except Exception as e:
                 logger.error(f'Failed to dropout: {e}')
 
             try:
-                if not cls.router:
-                    from home.ylfeng.cloud import correct_readout
-                    cdres = correct_readout(dres, meta['other']['measure'])
-                else:
-                    cdres = dres
+                from home.ylfeng.cloud import correct_readout
+                cdres = correct_readout(dres, meta['other']['measure'])
             except Exception as e:
                 cdres = dres
                 logger.error(f'Failed to correct readout, {e}!')
 
             for k, v in cdres.items():
                 hist[''.join((str(i) for i in k))] = v
-
         return status, hist
 
-    def update(self, backend: str, info: dict):
-        quafuos = str(Path.home()/'Desktop/qusteed0.1.1')
-        if quafuos not in sys.path:
-            print('adding quafuos', quafuos)
-            sys.path.append(quafuos)
-        with open(f'{backend}.json', 'w') as f:
-            f.write(json.dumps(info, indent=4))
-        from qusteedAPIs import call_local_backend_api
-        call_local_backend_api(backend=backend, chip_info_dict=info)
-        logger.warning(f'database of {backend} updated!')
-        return f'database of {backend} updated!'
-
-    def iterate(self):
-        pass
-
-    def getid(self, name: str, start: str, stop: str):
-        """根据名字获取所有在指定时间范围内的任务id列表
-
-        Args:
-            name (str): 任务名字
-            start (str): 起始时间，格式为2000-01-01-12-34-56，至少包含年月
-            stop (str): 结束时间，格式为2000-01-01-12-34-56，至少包含年月
-
-        Returns:
-            list: 所有任务的id
-        """
-        from .app import get_record_list_by_name
-        records = get_record_list_by_name(name, start, stop, 'proxy')
-        return [r[1] for r in records]
-
     def sysinfo(self):
-        while True:
-            if self.router:
-                print('='*94)
-                info = self.tracer[time.strftime('%Y-%m-%d %H:%M:%S')] = {}
-                for chip, conn in self.router.items():
-                    if chip != 'Baiwang':
-                        continue
-                    with self.lock:
-                        info[chip] = conn.sysinfo()
-                    try:
-                        print(self.perf.format(
-                            **({'chip': chip} | info[chip])))
-                    except Exception as e:
-                        logger.error(f'Failed to print perf info, {e}!')
-                # print(info)
-                print('='*94)
-                time.sleep(5)
-                if len(self.tracer) > 1000:
-                    ts = time.strftime('%Y%m%d%H%M%S')
-                    pf = Path.home()/f'Desktop/home/log/proxy/perf/{ts}.json'
-                    pf.parent.mkdir(parents=True, exist_ok=True)
-                    with open(pf, 'w') as f:
-                        f.write(json.dumps(self.tracer, indent=4))
-                        self.tracer.clear()
-
-            else:
-                if not hasattr(self, 'server'):
-                    from .app import login
-                    self.server = login()
-                return self.server.sysinfo(False)
+        return self.server.sysinfo(False)
 
     def snr(self, data):
         return data
```

## Comparing `vios-2.2.3.dist-info/LICENSE` & `vios-2.2.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vios-2.2.3.dist-info/METADATA` & `vios-2.2.4.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vios
-Version: 2.2.3
+Version: 2.2.4
 Summary: runtime requirements for systemq
 Author-email: YL Feng <fengyl@baqis.ac.cn>
 Project-URL: homepage, https://gitee.com
 Project-URL: bugs, https://gitee.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

## Comparing `vios-2.2.3.dist-info/RECORD` & `vios-2.2.4.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 quark/__main__.py,sha256=ky318p_RHmGRdMyzIL2meu-JOgqzRrH-hWfFvhceZGE,2858
-quark/proxy.py,sha256=CUkpnhSKBdjJ53eUZeG_su2YoTK07Sby7sU9DduEHWQ,24025
+quark/proxy.py,sha256=0rTaLgDGwePtWgDykY0JbwfVWw6tu5bX7mezMGNIzXo,24139
 quark/app/__init__.py,sha256=MjOh4mkjvwFzEEfPNv-dMOcoktAtYCBtl-P5_UA7MzQ,18861
 quark/app/_data.py,sha256=EGGTD2FrZ8vlbMh4jlmWhYk4fEG3FolGoWaQ26qxoss,2575
 quark/app/demo.py,sha256=eod5vSXKB0XI-Rr8UVKkNc9tOUfWCjI109Imd8bKmuo,10205
 quark/app/task.py,sha256=QEZuNia59sLEWa8pl2XIjItx2NismSTPZFnFt8-90HM,9043
 quark/app/uapi.py,sha256=itjEa89SUXozZqBGLH-3o4mKtRssNQODDj60knC-cGE,5876
 quark/driver/VirtualDevice.py,sha256=Cswl_ykFhIsocGV6Okh_YS1b48FeLm2fh1ruXqmNoyw,7914
 quark/driver/__init__.py,sha256=p1pVx1xTulBT8-qdp_zJ859tdIsA92XdvwrkqcVHL4s,386
@@ -14,12 +14,12 @@
 quark/envelope/__init__.py,sha256=5_cs0tZ7mV4GjOsY2isx8sUQu4u6Y3WN-9DUGG27SQM,1188
 quark/envelope/assembler.py,sha256=ENwX7FutJvpg6_Wcm42_Zx-ddq40JozuYqHPwJp09ZA,15111
 quark/envelope/calculator.py,sha256=0rZAA46sWh_X8wOBmpBvmljqCV53ID4VHPX1cE_abEc,4322
 quark/envelope/device.py,sha256=5E3oWZ84IYnQdzlmzltgPyayYz_au7p7UIbFVpJUa0Q,1106
 quark/envelope/processor.py,sha256=uMIwu83a4SDZVM3OE5_WrBya_4jxtdcXPd6pYa0osrk,3758
 quark/envelope/router.py,sha256=soUBYYMymYOCEruOsGogoXLGQxUoLBDkSmvLWLNcAVg,4128
 quark/envelope/systemq.py,sha256=QAaHLv68C9UjMp9qHt9t-HJkOTpCkbHZTlNVOsAzIBc,2841
-vios-2.2.3.dist-info/LICENSE,sha256=B_BP5ebph3-SqRxXvo-6Bh7vzPL2nPY5qSFQfr7xM_s,1085
-vios-2.2.3.dist-info/METADATA,sha256=NuGj7WFiyPMK5qkEucdLzwr36BAQJhcv6I6FWsONxxs,1211
-vios-2.2.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-vios-2.2.3.dist-info/top_level.txt,sha256=7SspgYXMW_50_NVkPj0EbFg4jFlGVsaIDfpqNsA1IMY,6
-vios-2.2.3.dist-info/RECORD,,
+vios-2.2.4.dist-info/LICENSE,sha256=B_BP5ebph3-SqRxXvo-6Bh7vzPL2nPY5qSFQfr7xM_s,1085
+vios-2.2.4.dist-info/METADATA,sha256=bkgceJFDGh90F8dYvSQQTcKzWueh1LRx_81a1HwxAe0,1211
+vios-2.2.4.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+vios-2.2.4.dist-info/top_level.txt,sha256=7SspgYXMW_50_NVkPj0EbFg4jFlGVsaIDfpqNsA1IMY,6
+vios-2.2.4.dist-info/RECORD,,
```

