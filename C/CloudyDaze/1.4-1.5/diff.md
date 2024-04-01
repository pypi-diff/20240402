# Comparing `tmp/CloudyDaze-1.4.tar.gz` & `tmp/CloudyDaze-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CloudyDaze-1.4.tar", last modified: Wed Apr 26 00:55:10 2023, max compression
+gzip compressed data, was "CloudyDaze-1.5.tar", last modified: Mon Apr  1 22:38:53 2024, max compression
```

## Comparing `CloudyDaze-1.4.tar` & `CloudyDaze-1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-04-26 00:55:10.224612 CloudyDaze-1.4/
-drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-04-26 00:55:10.209612 CloudyDaze-1.4/CloudyDaze/
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)     1015 2022-11-14 06:55:17.000000 CloudyDaze-1.4/CloudyDaze/MyAWS.py
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)     2940 2022-11-14 06:55:17.000000 CloudyDaze-1.4/CloudyDaze/MyEC2.py
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)    16340 2022-11-14 06:55:17.000000 CloudyDaze-1.4/CloudyDaze/MySCP.py
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)     4834 2023-04-26 00:52:57.000000 CloudyDaze-1.4/CloudyDaze/MySG.py
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)     2697 2022-11-14 06:55:17.000000 CloudyDaze-1.4/CloudyDaze/MySSH.py
-drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-04-26 00:55:10.217612 CloudyDaze-1.4/CloudyDaze.egg-info/
--rwxrwx---   0 eddo8    (197610) eddo8    (197610)     3557 2023-04-26 00:55:10.000000 CloudyDaze-1.4/CloudyDaze.egg-info/PKG-INFO
--rwxrwx---   0 eddo8    (197610) eddo8    (197610)      347 2023-04-26 00:55:10.000000 CloudyDaze-1.4/CloudyDaze.egg-info/SOURCES.txt
--rwxrwx---   0 eddo8    (197610) eddo8    (197610)        1 2023-04-26 00:55:10.000000 CloudyDaze-1.4/CloudyDaze.egg-info/dependency_links.txt
--rwxrwx---   0 eddo8    (197610) eddo8    (197610)      100 2023-04-26 00:55:10.000000 CloudyDaze-1.4/CloudyDaze.egg-info/requires.txt
--rwxrwx---   0 eddo8    (197610) eddo8    (197610)       11 2023-04-26 00:55:10.000000 CloudyDaze-1.4/CloudyDaze.egg-info/top_level.txt
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)     3557 2023-04-26 00:55:10.225612 CloudyDaze-1.4/PKG-INFO
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)     3241 2022-11-14 06:55:17.000000 CloudyDaze-1.4/README.md
-drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-04-26 00:55:10.223612 CloudyDaze-1.4/bin/
--rwxrwx---   0 eddo8    (197610) eddo8    (197610)      143 2021-08-08 23:42:06.000000 CloudyDaze-1.4/bin/myEC2.py
--rwxrwx---   0 eddo8    (197610) eddo8    (197610)      156 2021-08-08 23:42:06.000000 CloudyDaze-1.4/bin/mySCP.py
--rwxr-xr-x   0 eddo8    (197610) eddo8    (197610)      183 2022-11-14 06:55:17.000000 CloudyDaze-1.4/bin/mySG.py
--rwxrwx---   0 eddo8    (197610) eddo8    (197610)      156 2021-08-08 23:42:06.000000 CloudyDaze-1.4/bin/mySSH.py
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)       79 2023-04-26 00:55:10.225612 CloudyDaze-1.4/setup.cfg
--rwxrwx---   0 eddo8    (197610) eddo8    (197610)      892 2023-04-26 00:53:46.000000 CloudyDaze-1.4/setup.py
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2024-04-01 22:38:53.687730 CloudyDaze-1.5/
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2024-04-01 22:38:53.650647 CloudyDaze-1.5/CloudyDaze/
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     1015 2024-04-01 22:37:00.000000 CloudyDaze-1.5/CloudyDaze/MyAWS.py
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     2940 2024-04-01 22:37:00.000000 CloudyDaze-1.5/CloudyDaze/MyEC2.py
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)    16375 2024-04-01 22:37:00.000000 CloudyDaze-1.5/CloudyDaze/MySCP.py
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     4826 2024-04-01 22:37:31.000000 CloudyDaze-1.5/CloudyDaze/MySG.py
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     2732 2024-04-01 22:37:00.000000 CloudyDaze-1.5/CloudyDaze/MySSH.py
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2024-04-01 22:38:53.669202 CloudyDaze-1.5/CloudyDaze.egg-info/
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     3520 2024-04-01 22:38:53.000000 CloudyDaze-1.5/CloudyDaze.egg-info/PKG-INFO
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)      347 2024-04-01 22:38:53.000000 CloudyDaze-1.5/CloudyDaze.egg-info/SOURCES.txt
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)        1 2024-04-01 22:38:53.000000 CloudyDaze-1.5/CloudyDaze.egg-info/dependency_links.txt
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)      100 2024-04-01 22:38:53.000000 CloudyDaze-1.5/CloudyDaze.egg-info/requires.txt
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)       11 2024-04-01 22:38:53.000000 CloudyDaze-1.5/CloudyDaze.egg-info/top_level.txt
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     3520 2024-04-01 22:38:53.688707 CloudyDaze-1.5/PKG-INFO
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     3241 2022-11-14 06:55:17.000000 CloudyDaze-1.5/README.md
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2024-04-01 22:38:53.684801 CloudyDaze-1.5/bin/
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      143 2021-08-08 23:42:06.000000 CloudyDaze-1.5/bin/myEC2.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      156 2021-08-08 23:42:06.000000 CloudyDaze-1.5/bin/mySCP.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      183 2022-11-14 06:55:17.000000 CloudyDaze-1.5/bin/mySG.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      156 2021-08-08 23:42:06.000000 CloudyDaze-1.5/bin/mySSH.py
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)       79 2024-04-01 22:38:53.690660 CloudyDaze-1.5/setup.cfg
+-rwxr-xr-x   0 eddo8    (197610) eddo8    (197610)      892 2024-04-01 22:38:26.000000 CloudyDaze-1.5/setup.py
```

### Comparing `CloudyDaze-1.4/CloudyDaze/MyAWS.py` & `CloudyDaze-1.5/CloudyDaze/MyAWS.py`

 * *Files identical despite different names*

### Comparing `CloudyDaze-1.4/CloudyDaze/MyEC2.py` & `CloudyDaze-1.5/CloudyDaze/MyEC2.py`

 * *Files 17% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 		
 	@args.operation
 	@args.parameter(name='ids', short='i', nargs='*', help='aws ec2 id list')
 	def list(self, ids=[]):
 		status = dict()
 		for reservation in self.conn.get_all_reservations():
-			logger.debug('reservation: %s'%reservation.id)
+			print('reservation: %s'%reservation.id)
 			for instance in reservation.instances:
 				if len(ids) > 0 and instance.id not in ids: continue
 				if self.verbose:
 					printp(json.dumps(dir(instance),indent=4))
 					print(instance.ip_address)
 				if str(instance.state) not in status.keys():
 					status[str(instance.state)] = list()
@@ -65,37 +65,39 @@
 
 		
 	@args.operation
 	@args.parameter(name='ids', short='i', nargs='*', help='aws ec2 id list')
 	def start(self, ids=[]):
 		status = dict()
 		for reservation in self.conn.get_all_reservations():
-			logger.debug('reservation: %s'%reservation.id)
+			print('reservation: %s'%reservation.id)
 			for instance in reservation.instances:
-				logger.info(instance)
+				print(instance)
 				if len(ids) > 0 and instance.id not in ids: continue
 				if instance.state not in [ u'pending', u'starting', u'running' ]:
 					instance.start()
-					logger.info(instance)
+					print(instance)
 				if str(instance.state) not in status.keys():
 					status[str(instance.state)] = list()
 				status[str(instance.state)].append(str(instance.id))
 		return status
 
 		
 	@args.operation
 	@args.parameter(name='ids', short='i', nargs='*', help='aws ec2 id list')
 	def stop(self, ids=[]):
 		status = dict()
 		for reservation in self.conn.get_all_reservations():
-			logger.debug('reservation: %s'%reservation.id)
+			print('reservation: %s'%reservation.id)
 			for instance in reservation.instances:
-				logger.info(instance)
+				print(instance)
 				if len(ids) > 0 and instance.id not in ids: continue
 				if instance.state not in [ u'pending', u'stopping', u'stopped' ]:
 					instance.stop()
-					logger.info(instance)
+					print(instance)
 				if str(instance.state) not in status.keys():
 					status[str(instance.state)] = list()
 				status[str(instance.state)].append(str(instance.id))
 		return status
 		
+		
+if __name__ == '__main__': args.execute()
```

### Comparing `CloudyDaze-1.4/CloudyDaze/MySCP.py` & `CloudyDaze-1.5/CloudyDaze/MySCP.py`

 * *Files 1% similar despite different names*

```diff
@@ -610,7 +610,9 @@
 		output.write(now.strftime('%Y-%m-%d %H:%M:%S'))
 
 	mySCP.connect()
 	print(mySCP.put(local, remote))
 	print(mySCP.get(remote, local.replace('.txt', '.new.txt')))
 	mySCP.close()
 
+
+if __name__ == '__main__': test()
```

### Comparing `CloudyDaze-1.4/CloudyDaze/MySG.py` & `CloudyDaze-1.5/CloudyDaze/MySG.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 	ports = {
 		22: 'tcp',
 		1521: 'tcp',
 		1883: 'tcp',
 		3389: 'tcp',
 		8888: 'tcp',
 		9999: 'tcp',
+		61616: 'tcp',
 	}
 	
 	types=[
 		'tcp',
 		'udp',
 		'icmp',
 		-1
@@ -79,15 +80,15 @@
 
 	#_________________________________________________
 	@args.operation
 	def myip(self):
 		if not self._myip:
 			results = requests.get(self.url).json()
 			self._myip = results['ip']
-			logger.info('myip = %s'%self._myip)
+			print('myip = %s'%self._myip)
 		return self._myip
 
 
 	#_________________________________________________
 	def __security_group(self):
 		for sg in self.conn.get_all_security_groups():
 			if sg.id != self.security_group: 
@@ -105,15 +106,15 @@
 			for grant in rule.grants:
 				_grant = dict(
 					ip_protocol=str(rule.ip_protocol),
 					cidr_ip=str(grant),
 					from_port=int(rule.from_port),
 					to_port=int(rule.to_port),
 				)
-				logger.info('= %s'%self.dictate(_grant))
+				print('= %s'%self.dictate(_grant))
 				_granted.append(_grant)
 				ip = str(grant).replace('/32','')
 		return _granted
 	
 
 	#_________________________________________________
 	@args.operation
@@ -150,15 +151,15 @@
 				if all(test):
 					logger.debug('authorised = %s'%self.dictate(_do))
 					_enabled.append(_do)
 					del _todo[t]
 
 		# process the remaing todo items
 		for _do in _todo:
-			logger.info('+ %s'%self.dictate(_do))
+			print('+ %s'%self.dictate(_do))
 			_enabled.append(_do)
 			sg.authorize(src_group=None,**_do)
 			
 		return _enabled
 
 
 	#_________________________________________________
@@ -171,15 +172,15 @@
 		sg = self.__security_group()
 		_granted = self.granted()
 		_revoked = []
 		for ip in ips:
 			for _grant in _granted:
 				if forall or ip == _grant['cidr_ip'].split('/')[0]:
 					_revoked.append(_grant)
-					logger.info('- %s'%self.dictate(_grant))
+					print('- %s'%self.dictate(_grant))
 					sg.revoke(
 						ip_protocol=_grant['ip_protocol'],
 						from_port=_grant['from_port'],
 						to_port=_grant['to_port'],
 						cidr_ip=_grant['cidr_ip'],
 						src_group=None
 					)
```

### Comparing `CloudyDaze-1.4/CloudyDaze/MySSH.py` & `CloudyDaze-1.5/CloudyDaze/MySSH.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,7 +116,9 @@
 	mySSH.key = '~/.ssh/id_rsa'
 
 	mySSH.connect()
 	print(mySSH.execute('whoami'))
 	print(mySSH.execute('uptime'))
 	mySSH.close()
 
+if __name__ == '__main__': test()
+
```

### Comparing `CloudyDaze-1.4/CloudyDaze.egg-info/PKG-INFO` & `CloudyDaze-1.5/CloudyDaze.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: CloudyDaze
-Version: 1.4
-Summary: UNKNOWN
+Version: 1.5
 Home-page: https://github.com/eddo888/CloudyDaze
+Download-URL: https://github.com/eddo888/CloudyDaze/archive/1.5.tar.gz
 Author: David Edson
 Author-email: eddo888@tpg.com.au
 License: MIT
-Download-URL: https://github.com/eddo888/CloudyDaze/archive/1.4.tar.gz
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # CloudyDaze
 
 bunch of usefull scripts for managing your cloud
 
 please note that these use the most excellent credstash library for python,
@@ -137,9 +135,7 @@
   -v, --verbose         verbose logging
 ```
 
 ---
 ## acknowledgements
 
 code graciously borrowed from [StaSh for Pythonista](https://github.com/ywangd/stash)
-
-
```

### Comparing `CloudyDaze-1.4/PKG-INFO` & `CloudyDaze-1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: CloudyDaze
-Version: 1.4
-Summary: UNKNOWN
+Version: 1.5
 Home-page: https://github.com/eddo888/CloudyDaze
+Download-URL: https://github.com/eddo888/CloudyDaze/archive/1.5.tar.gz
 Author: David Edson
 Author-email: eddo888@tpg.com.au
 License: MIT
-Download-URL: https://github.com/eddo888/CloudyDaze/archive/1.4.tar.gz
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # CloudyDaze
 
 bunch of usefull scripts for managing your cloud
 
 please note that these use the most excellent credstash library for python,
@@ -137,9 +135,7 @@
   -v, --verbose         verbose logging
 ```
 
 ---
 ## acknowledgements
 
 code graciously borrowed from [StaSh for Pythonista](https://github.com/ywangd/stash)
-
-
```

### Comparing `CloudyDaze-1.4/README.md` & `CloudyDaze-1.5/README.md`

 * *Files identical despite different names*

### Comparing `CloudyDaze-1.4/setup.py` & `CloudyDaze-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 pwd = path.abspath(path.dirname(__file__))
 with codecs.open(path.join(pwd, 'README.md'), 'r', encoding='utf8') as input:
     long_description = input.read()
 
 name='CloudyDaze'
-version='1.4'
+version='1.5'
 
 setup(
 	name=name,
 	version=version,
 	license='MIT',
 	long_description=long_description,
 	long_description_content_type="text/markdown",
```

