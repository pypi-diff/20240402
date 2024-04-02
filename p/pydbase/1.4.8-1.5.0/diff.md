# Comparing `tmp/pydbase-1.4.8.tar.gz` & `tmp/pydbase-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydbase-1.4.8.tar", last modified: Sat Mar  9 10:55:19 2024, max compression
+gzip compressed data, was "pydbase-1.5.0.tar", last modified: Tue Apr  2 05:36:08 2024, max compression
```

## Comparing `pydbase-1.4.8.tar` & `pydbase-1.5.0.tar`

### file list

```diff
@@ -1,43 +1,47 @@
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-03-09 10:55:19.485671 pydbase-1.4.8/
--rw-r--r--   0 peterglen  (1000) users      (100)    14847 2024-03-09 10:55:19.485671 pydbase-1.4.8/PKG-INFO
--rw-rw-r--   0 peterglen  (1000) users      (100)    14433 2024-03-09 10:52:04.000000 pydbase-1.4.8/README.md
--rwxrwxr-x   0 peterglen  (1000) users      (100)     7524 2024-03-09 09:46:44.000000 pydbase-1.4.8/chainadm.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)    10808 2024-03-08 03:12:59.000000 pydbase-1.4.8/dbaseadm.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-03-09 10:55:19.473664 pydbase-1.4.8/pydbase/
--rwxr-xr-x   0 peterglen  (1000) users      (100)        9 2023-09-25 19:38:11.000000 pydbase-1.4.8/pydbase/__init__.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     6275 2024-03-09 09:44:34.000000 pydbase-1.4.8/pydbase/dbutils.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     6118 2024-03-09 04:59:30.000000 pydbase-1.4.8/pydbase/twinbase.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    11825 2024-03-09 10:39:04.000000 pydbase-1.4.8/pydbase/twinchain.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    42259 2024-03-09 10:53:51.000000 pydbase-1.4.8/pydbase/twincore.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-03-09 10:55:19.485671 pydbase-1.4.8/pydbase.egg-info/
--rw-r--r--   0 peterglen  (1000) users      (100)    14847 2024-03-09 10:55:19.000000 pydbase-1.4.8/pydbase.egg-info/PKG-INFO
--rw-r--r--   0 peterglen  (1000) users      (100)      794 2024-03-09 10:55:19.000000 pydbase-1.4.8/pydbase.egg-info/SOURCES.txt
--rw-r--r--   0 peterglen  (1000) users      (100)        1 2024-03-09 10:55:19.000000 pydbase-1.4.8/pydbase.egg-info/dependency_links.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       76 2024-03-09 10:55:19.000000 pydbase-1.4.8/pydbase.egg-info/entry_points.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       18 2024-03-09 10:55:19.000000 pydbase-1.4.8/pydbase.egg-info/top_level.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-03-09 10:55:19.485671 pydbase-1.4.8/setup.cfg
--rw-rw-r--   0 peterglen  (1000) users      (100)     1760 2024-03-09 10:52:17.000000 pydbase-1.4.8/setup.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-03-09 10:55:19.485671 pydbase-1.4.8/tests/
--rw-rw-r--   0 peterglen  (1000) users      (100)     1476 2024-02-28 03:36:47.000000 pydbase-1.4.8/tests/test_acreate.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1471 2024-03-08 06:23:40.000000 pydbase-1.4.8/tests/test_bigdata.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1747 2024-02-28 04:12:53.000000 pydbase-1.4.8/tests/test_bindata.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1497 2024-03-07 15:25:35.000000 pydbase-1.4.8/tests/test_chain.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     2047 2024-03-07 16:36:45.000000 pydbase-1.4.8/tests/test_chain_data.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     2335 2024-03-07 16:44:33.000000 pydbase-1.4.8/tests/test_chain_link.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1189 2024-02-28 03:53:28.000000 pydbase-1.4.8/tests/test_del.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1273 2024-02-28 03:53:43.000000 pydbase-1.4.8/tests/test_dump.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1239 2024-03-05 15:27:23.000000 pydbase-1.4.8/tests/test_find.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1244 2024-03-05 15:30:09.000000 pydbase-1.4.8/tests/test_findrec.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1315 2024-03-05 15:37:16.000000 pydbase-1.4.8/tests/test_getoffs.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1567 2024-02-28 04:02:31.000000 pydbase-1.4.8/tests/test_getrec.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1762 2024-03-08 07:58:06.000000 pydbase-1.4.8/tests/test_handles.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1403 2024-03-08 06:29:52.000000 pydbase-1.4.8/tests/test_inplace.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1042 2024-02-28 04:02:50.000000 pydbase-1.4.8/tests/test_integrity.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1508 2024-02-28 04:03:32.000000 pydbase-1.4.8/tests/test_list.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1531 2024-02-28 04:03:13.000000 pydbase-1.4.8/tests/test_lockrel.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1622 2024-02-28 04:03:50.000000 pydbase-1.4.8/tests/test_multi.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1927 2024-02-28 04:05:14.000000 pydbase-1.4.8/tests/test_packer.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1429 2024-02-28 04:13:18.000000 pydbase-1.4.8/tests/test_randdata.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1846 2024-02-28 04:01:33.000000 pydbase-1.4.8/tests/test_reindex.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1431 2024-02-28 04:05:31.000000 pydbase-1.4.8/tests/test_search.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1588 2024-03-04 12:52:21.000000 pydbase-1.4.8/tests/test_vacuum.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-02 05:36:08.914493 pydbase-1.5.0/
+-rw-r--r--   0 peterglen  (1000) users      (100)    14848 2024-04-02 05:36:08.914493 pydbase-1.5.0/PKG-INFO
+-rw-rw-r--   0 peterglen  (1000) users      (100)    14434 2024-03-15 17:13:31.000000 pydbase-1.5.0/README.md
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     7869 2024-04-01 08:34:35.000000 pydbase-1.5.0/chainadm.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)    10897 2024-04-01 03:23:33.000000 pydbase-1.5.0/dbaseadm.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-02 05:36:08.902492 pydbase-1.5.0/pydbase/
+-rwxr-xr-x   0 peterglen  (1000) users      (100)        9 2023-09-25 19:38:11.000000 pydbase-1.5.0/pydbase/__init__.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     5144 2024-04-02 05:00:59.000000 pydbase-1.5.0/pydbase/dbutils.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-02 05:36:08.902492 pydbase-1.5.0/pydbase/docs/
+-rw-r--r--   0 peterglen  (1000) users      (100)    30170 2024-04-02 05:33:18.000000 pydbase-1.5.0/pydbase/docs/twinbase.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    46450 2024-04-02 05:33:17.000000 pydbase-1.5.0/pydbase/docs/twinchain.html
+-rw-r--r--   0 peterglen  (1000) users      (100)   143801 2024-04-02 05:33:18.000000 pydbase-1.5.0/pydbase/docs/twincore.html
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3453 2024-04-01 01:42:37.000000 pydbase-1.5.0/pydbase/portalocker.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     6495 2024-04-01 05:05:24.000000 pydbase-1.5.0/pydbase/twinbase.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    12457 2024-04-02 05:05:37.000000 pydbase-1.5.0/pydbase/twinchain.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    47269 2024-04-02 05:16:26.000000 pydbase-1.5.0/pydbase/twincore.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-02 05:36:08.914493 pydbase-1.5.0/pydbase.egg-info/
+-rw-r--r--   0 peterglen  (1000) users      (100)    14848 2024-04-02 05:36:08.000000 pydbase-1.5.0/pydbase.egg-info/PKG-INFO
+-rw-r--r--   0 peterglen  (1000) users      (100)      876 2024-04-02 05:36:08.000000 pydbase-1.5.0/pydbase.egg-info/SOURCES.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)        1 2024-04-02 05:36:08.000000 pydbase-1.5.0/pydbase.egg-info/dependency_links.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       76 2024-04-02 05:36:08.000000 pydbase-1.5.0/pydbase.egg-info/entry_points.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       18 2024-04-02 05:36:08.000000 pydbase-1.5.0/pydbase.egg-info/top_level.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-04-02 05:36:08.914493 pydbase-1.5.0/setup.cfg
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1926 2024-04-02 05:31:14.000000 pydbase-1.5.0/setup.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-02 05:36:08.914493 pydbase-1.5.0/tests/
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1436 2024-04-01 04:09:23.000000 pydbase-1.5.0/tests/test_acreate.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1470 2024-04-01 08:57:38.000000 pydbase-1.5.0/tests/test_bigdata.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1399 2024-04-01 07:47:06.000000 pydbase-1.5.0/tests/test_bindata.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1497 2024-03-07 15:25:35.000000 pydbase-1.5.0/tests/test_chain.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     2046 2024-04-01 02:59:49.000000 pydbase-1.5.0/tests/test_chain_data.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     2333 2024-04-01 03:03:51.000000 pydbase-1.5.0/tests/test_chain_link.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1189 2024-02-28 03:53:28.000000 pydbase-1.5.0/tests/test_del.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1273 2024-02-28 03:53:43.000000 pydbase-1.5.0/tests/test_dump.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1305 2024-04-01 04:15:24.000000 pydbase-1.5.0/tests/test_find.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1310 2024-04-01 04:09:03.000000 pydbase-1.5.0/tests/test_findrec.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1385 2024-04-01 04:21:29.000000 pydbase-1.5.0/tests/test_getoffs.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1567 2024-02-28 04:02:31.000000 pydbase-1.5.0/tests/test_getrec.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1931 2024-04-01 04:17:37.000000 pydbase-1.5.0/tests/test_handles.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1471 2024-04-01 04:18:57.000000 pydbase-1.5.0/tests/test_inplace.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1108 2024-04-01 04:23:28.000000 pydbase-1.5.0/tests/test_integrity.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1574 2024-04-01 04:20:53.000000 pydbase-1.5.0/tests/test_list.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1541 2024-03-10 04:45:43.000000 pydbase-1.5.0/tests/test_lockrel.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1799 2024-04-02 05:26:52.000000 pydbase-1.5.0/tests/test_multi.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1927 2024-02-28 04:05:14.000000 pydbase-1.5.0/tests/test_packer.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1654 2024-04-01 09:10:20.000000 pydbase-1.5.0/tests/test_reindex.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1503 2024-04-01 04:22:41.000000 pydbase-1.5.0/tests/test_search.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1676 2024-04-01 03:36:26.000000 pydbase-1.5.0/tests/test_vacuum.py
```

### Comparing `pydbase-1.4.8/PKG-INFO` & `pydbase-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydbase
-Version: 1.4.8
+Version: 1.5.0
 Summary: High speed database with key / data in python.
 Home-page: https://github.com/pglen/pydbase
 Author: Peter Glen
 Author-email: peterglen99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 #### see: blockchain functions at the end
 
  &nbsp; The motivation was to create a no frills way of saving / retrieving data.
 It is fast, and the time test shows that this is an order of magnitude
 faster than most mainstream databases. This is due to the engine's simplicity.
 It avoids expensive computations in favor of quickly saving data.
 
-### Fast data save / retrieve
+### Fast data save / retrieve 
 
  &nbsp; Mostly ready for production. All tests pass. Please use caution, as this is new.
 The command line tester can drive most aspects of this API; and it is somewhat
 complete. It is also  good way to see the API / Module in action.
 
 ## API
```

### Comparing `pydbase-1.4.8/README.md` & `pydbase-1.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #### see: blockchain functions at the end
 
  &nbsp; The motivation was to create a no frills way of saving / retrieving data.
 It is fast, and the time test shows that this is an order of magnitude
 faster than most mainstream databases. This is due to the engine's simplicity.
 It avoids expensive computations in favor of quickly saving data.
 
-### Fast data save / retrieve
+### Fast data save / retrieve 
 
  &nbsp; Mostly ready for production. All tests pass. Please use caution, as this is new.
 The command line tester can drive most aspects of this API; and it is somewhat
 complete. It is also  good way to see the API / Module in action.
 
 ## API
```

### Comparing `pydbase-1.4.8/chainadm.py` & `pydbase-1.5.0/chainadm.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,17 @@
     dkeyx   = "";   dumpx  = 0
     findrec = "";   getrec = -1
     datex = 0   ;   cntx = 1
     headx = ""  ;   gethead = -1
     getby = ""  ;   getoffs = ""
 
 def help():
+
+    ''' Deliver program usage information '''
+
     print("Usage: %s [options]" % os.path.split(sys.argv[0])[1])
     print("   Options: -a  data   append data to the end of chain")
     print("            -g recnum  get record")
     print("            -k reckey  get record by key/header")
     print("            -G recnum  get record offset by key")
     print("            -r recnum  get record header")
     print("            -n         append / show / get number of records")
@@ -137,19 +140,32 @@
 
         if aa[0] == "-c":
             _c.checkx = True
 
         if aa[0] == "-i":
             _c.integx = True
 
+    execfunc()
+
     #print("Use: pychain.py -h to see options and help")
 
+def execfunc():
+
+    ''' Execute individual function from command line '''
+
+
     # Create our database
     core = twinchain.TwinChain(_c.deffile, _c.pgdebug, _c.verbose)
 
+    core.base_quiet     = _c.quiet
+    core.base_pgdebug   = _c.pgdebug
+    core.base_showdel   = _c.sdelx
+    core.base_integrity = _c.checkx
+    core.base_pgdebug   = _c.pgdebug
+
     if _c.integx:
         #print("Integrity", _c.integx)
         errx = False; cnt = []
         sss = core.getdbsize()
         # Remember record zero is the anchor
         for aa in range(1, sss):
             ppp = core.linkintegrity(aa)
@@ -207,16 +223,16 @@
             if cnt >= end:
                 break
             hhh = core.get_header(cnt)
             ppp = core.get_payload(cnt)
             ddd = ""
             if  _c.datex:
                 ddd = dbutils.uuid2date(uuid.UUID(ppp[0]))
-            print(cnt, hhh, ddd, ppp)
-
+            if hhh:
+                print(cnt, hhh, ddd, ppp)
             cnt = cnt + 1
 
     elif _c.append:
         #print("Appending", _c.append)
         dicx = {}; arrx = []
         arrx = _c.append.split()
         if len(arrx) % 2:
```

### Comparing `pydbase-1.4.8/dbaseadm.py` & `pydbase-1.5.0/dbaseadm.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,22 +54,25 @@
 
 # ------------------------------------------------------------------------
 
 # Return a random string based upon length
 
 def randstr(lenx):
 
+    ''' Deliver a random string for testing '''
     strx = ""
     for aa in range(lenx):
         ridx = random.randint(0, len(allstr)-1)
         rr = allstr[ridx]
         strx += str(rr)
     return strx
 
 def help():
+    ''' Program usage information '''
+
     pname = os.path.split(sys.argv[0])[1]
     print("Usage: %s [options] [arg_key arg_data]" %  pname)
     print("   -h         Help (this screen)   -|-  -E         Replace record in place")
     print("   -V         Print version        -|-  -q         Quiet on, less printing")
     print("   -d         Debug level (0-10)   -|-  -v         Increment verbosity level")
     print("   -r         Randomize data       -|-  -w         Write random record(s)")
     print("   -z         Dump backwards(s)    -|-  -i         Show deleted record(s)")
@@ -292,15 +295,15 @@
         if not ddd:
             print("Record:", "'" + _m.retrx + "'", "is not found.")
         else:
             print(ddd)
     elif _m.sizex:
         print("Database size:", core.getdbsize())
     elif _m.offsx:
-        ddd = core.get_rec_offs(int(_m.offsx))
+        ddd = core.get_rec_byoffs(int(_m.offsx))
         print(ddd)
     elif _m.delx:
         ddd = core.del_rec_offs(int(_m.delx))
         print(ddd)
     elif _m.delrx2:
         ddd = core.del_rec(int(_m.delrx))
         print(ddd)
```

### Comparing `pydbase-1.4.8/pydbase/twinbase.py` & `pydbase-1.5.0/pydbase/twinbase.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 
 '''!
     twinbase -- extracted from twincore to make it eazier to read
 '''
 
 import  os, sys, getopt, signal, select, socket, time, struct
 import  random, stat, os.path, datetime, threading
-import  struct, io, traceback, fcntl, hashlib, traceback
+import  struct, io, traceback, hashlib, traceback
+
+try:
+    import fcntl
+except:
+    fcntl = None
 
 base = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(base, '..', 'pydbase'))
 
 from dbutils import *
 
 HEADSIZE        = 32
@@ -46,14 +51,15 @@
 
     def __init__(self, pgdebug = 0):
 
         self.pgdebug = pgdebug
 
         global base_pgdebug
         base_pgdebug = pgdebug
+        set_pgdebug(pgdebug)
 
         if self.pgdebug > 1:
             print("Initializing core base pgdebug =", pgdebug)
 
         # Provide placeholders
         self.fp = None
         self.ifp = None
@@ -148,31 +154,42 @@
         #    hashx = int(hashx << 8) + int(hashx >> 8)
         #    hashx &= 0xffffffff
         #print("hash32 %.3f" % ((time.time() - ttt) * 1000) )
         #print("hash32: %x" % hashx)
 
         return hashx
 
+    def _lockx(self, fp):
+        if fcntl:
+            fcntl.lockf(fp, fcntl.LOCK_EX)
+        else:
+            import msvcrt
+            fnum = fp.fileno()
+            msvcrt.locking(fnum, msvcrt.LK_LOCK, os.fstat(fnum).st_size)
+
     def softcreate(self, fname, raisex = True):
 
         ''' Open for read / write. Create if needed. '''
 
         #print("Softcreate", fname)
 
         fp = None
         try:
             fp = open(fname, "rb+")
+            #self._lockx(fp)
         except:
             try:
                 fp = open(fname, "wb+")
-                fcntl.lockf(fp, fcntl.LOCK_EX)
+                self._lockx(fp)
             except:
                 #print("Deleting lock", self.lckname)
-                dellock(self.lckname)
+                #dellock(self.lckname)
+                self.lock.unlock()  #dellock(self.lckname)
                 print("Cannot open / create ", "'" + fname + "'", sys.exc_info())
+
                 if raisex:
                     raise
                 pass
 
         return fp
 
     def create_data(self, fp):
```

### Comparing `pydbase-1.4.8/pydbase/twinchain.py` & `pydbase-1.5.0/pydbase/twinchain.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #!/usr/bin/env python3
 
 '''!
     @mainpage
 
     # Twinchain
 
-    Block chain layer on top of twincore.
+        Block chain layer on top of twincore.
 
-        prev     curr
-            record
-    |   Time Now    |   Time  Now    |  Time Now     |
-    |   hash256   | |    hash256   | |   hash256   | |
-    |   Header    | |    Header    | |   Header    | |
-    |   Payload   | |    Payload   | |   Payload   | |
-    |   Backlink  | |    Backlink  | |   Backlink  | |
-                  |----->---|      |---->---|     |------ ...
-
-    The sum of fields saved to the next backlink.
-
-    History:
-
-        0.0.0       Tue 20.Feb.2024     Initial release
-        0.0.0       Sun 26.Mar.2023     More features
-        1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
-        1.4.0       Tue 27.Feb.2024     Addedd pgdebug
-        1.4.2       Wed 28.Feb.2024     Fixed multiple instances
-        1.4.3       Wed 28.Feb.2024     ChainAdm added
+            prev     curr
+                record
+        |   Time Now    |   Time  Now    |  Time Now     |
+        |   hash256   | |    hash256   | |   hash256   | |
+        |   Header    | |    Header    | |   Header    | |
+        |   Payload   | |    Payload   | |   Payload   | |
+        |   Backlink  | |    Backlink  | |   Backlink  | |
+                      |----->---|      |---->---|     |------ ...
+
+        The sum of fields saved to the next backlink.
+
+        History:
+
+            0.0.0       Tue 20.Feb.2024     Initial release
+            0.0.0       Sun 26.Mar.2023     More features
+            1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
+            1.4.0       Tue 27.Feb.2024     Addedd pgdebug
+            1.4.2       Wed 28.Feb.2024     Fixed multiple instances
+            1.4.3       Wed 28.Feb.2024     ChainAdm added
 
 '''
 
 import  os, sys, getopt, signal, select, socket, time, struct
 import  random, stat, os.path, datetime, threading, uuid
 import  struct, io, hashlib
 
@@ -65,21 +65,20 @@
     '''
 
     def __init__(self, fname = "pydbchain.pydb", pgdebug = 0, core_verbose = 0):
 
         self.core_verbose = core_verbose
 
         # Upper lock name
-        self.ulockname = os.path.splitext(fname)[0] + ".ulock"
+        ulockname = os.path.splitext(fname)[0] + ".ulock"
+        self.ulock = FileLock(ulockname)
+        self.ulock.waitlock()    #(self.ulockname)
 
-        waitlock(self.ulockname)
         super(TwinChain, self).__init__(fname, pgdebug)
 
-        #print("TwinChain.init", self.fname, self.ulockname)
-
         self.packer = pyvpacker.packbin()
         sss = self.getdbsize()
         if sss == 0:
             payload = {"Initial": "Initial record, do not use."}
             #print("Init anchor record", payload)
 
             # Here we fake the initial backlink for the anchor record
@@ -97,15 +96,15 @@
             self.old_dicx["backlink"] =  ""
 
             aaa = self._fill_record(header, payload)
             #print(aaa)
             encoded = self.packer.encode_data("", aaa)
             self.save_data(header, encoded)
 
-        dellock(self.ulockname)
+        self.ulock.unlock() #self.ulockname)
 
     def _hashtohex(self, varx):
 
         if type(varx) == type(""):
             varx = varx.encode()
 
         hh = hashlib.new("sha256");
@@ -180,20 +179,22 @@
         return aaa
 
     def get_payload(self, recnum):
 
         ''' Return the payload on record number '''
 
         arr = self.get_rec(recnum)
+        if not arr:
+            return []
         try:
             decoded = self.packer.decode_data(arr[1])
             #print("decoded", decoded)
         except:
-            print("Cannot decode", recnum, sys.exc_info())
-            return "Bad record"
+            print("Cannot decode record at", recnum, recnum, sys.exc_info())
+            raise
         dic = self._get_fields(decoded[0])
 
         if self.core_verbose > 2:
             print(dic)
         if self.core_verbose > 0:
             print(dic['header'] + " " + dic['now'], dic['payload'])
 
@@ -247,19 +248,29 @@
                 arr.append((head, pay))
                 if len(arr) >= maxrec:
                     break
         return arr
 
     def get_header(self, recnum):
 
-        ''' Get header of record '''
+        ''' Get the header of record. '''
 
+        if self.pgdebug > 5:
+            print("get_header()", recnum)
         arr = self.get_rec(recnum)
+        if not arr:
+            if self.pgdebug > 5:
+                print("get_header(): empty/deleted record", recnum)
+
+            if self.core_verbose > 1:
+                print("get_header(): empty/deleted record", recnum)
+            return []
+
         if self.core_verbose > 1:
-            print("arr[0]", arr[0])
+            print("arr", arr)
             uuu = uuid.UUID(arr[0].decode())
             ddd = str(uuid2date(uuu))
             print("header", arr[0])
         return arr[0].decode()
 
     def linkintegrity(self, recnum):
 
@@ -280,15 +291,16 @@
             print("Cannot decode prev:", recnum, sys.exc_info())
             return
         dicold = self._get_fields(decoded[0])
         arr2 = self.get_rec(recnum)
         try:
             decoded2 = self.packer.decode_data(arr2[1])
         except:
-            print("Cannot decode curr:", recnum, sys.exc_info())
+            if self.core_verbose > 2:
+                print("Cannot decode curr:", recnum, sys.exc_info())
             return
         dic = self._get_fields(decoded2[0])
         backlink = self._build_backlink(dicold)
         hhh = self._hashtohex(backlink)
         if self.core_verbose > 2:
             print("calc      ", hhh)
             print("backlink  ", dic['backlink'])
@@ -298,15 +310,16 @@
 
         ''' Integrity check of record. '''
 
         arr = self.get_rec(recnum)
         try:
             decoded = self.packer.decode_data(arr[1])
         except:
-            print("Cannot decode:", recnum, sys.exc_info())
+            if self.core_verbose > 2:
+                print("Cannot decode:", recnum, sys.exc_info())
             return
 
         aaa = self._get_fields(decoded[0])
         sumstr = self._build_sumstr(aaa)
         hhh = self._hashtohex(sumstr)
         if self.core_verbose > 1:
             print("data", hhh)
@@ -323,35 +336,38 @@
 
         #if type(datax) != type(b""):
         #    datax = datax.encode() #errors='strict')
 
         if self.core_verbose > 0:
             print("Appendwith", header, datax)
 
-        waitlock(self.ulockname)
+        self.ulock.waitlock()    #self.ulockname)
 
         try:
             uuu = uuid.UUID(header)
         except:
             if self.core_verbose:
                 print("Header override must be a valid UUID string.")
 
-            dellock(self.ulockname)
+            self.ulock.unlock() #self.ulockname)
             raise ValueError("Header override must be a valid UUID string.")
 
         self.old_dicx = {}
         # Get last data from db
         sss = self.getdbsize()
         #print("sss", sss)
 
         if not sss:
             raise ValueError("Invalid database, must have at least one record.")
 
         ooo = self.get_rec(sss-1)
 
+        if self.pgdebug > 5:
+            print("decoding", ooo)
+
         decoded = self.packer.decode_data(ooo[1])
 
         self.old_dicx = self._get_fields(decoded[0])
 
         #print("old_fff", self.old_dicx["hash256"])
         #print("old_time", self.old_dicx["now"])
 
@@ -365,15 +381,15 @@
         self.save_data(header, encoded)
         #print("eee", self.getdbsize())
 
         if self.core_verbose > 1:
             bbb = self.packer.decode_data(encoded)
             print("Rec", bbb[0])
 
-        dellock(self.ulockname)
+        self.ulock.unlock() #self.ulockname)
         return True
 
     def append(self, datax):
 
         ''' Append data to the end of database '''
 
         if self.core_verbose > 0:
```

### Comparing `pydbase-1.4.8/pydbase/twincore.py` & `pydbase-1.5.0/pydbase/twincore.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,67 +1,75 @@
 #!/usr/bin/env python3
 
 '''!
     @mainpage
 
-    # Twincore
+        Database with two files. One for data, one for index;
 
-    Database with two files. One for data, one for index;
+        The reason for the 'twin' name is that two files are created.
+        The first contains the data, the second contains the
+        offsets (indexes) and hashes.
 
-    The reason for this name is that two files are created. The first contains
-    the data, the second contains the offsets (indexes) and hashes.
+        The second file can be re-built easily from the first
+        using the reindex option.
 
-    The second file can be re-built easily from the first using the reindex option.
+        Structure of the data:
 
-    Structure of the data:
+            32 byte header, starating with FILESIG;
 
-        32 byte header, starating with FILESIG;
+            4 bytes    4 bytes          4 bytes         Variable
+            ------------------------------------------------------------
+            RECSIG     Hash_of_key      Len_of_key      DATA_for_key
+            RECSEP     Hash_of_payload  Len_of_payload  DATA_for_payload
+                .
+                .
 
-        4 bytes    4 bytes          4 bytes         Variable
-        ------------------------------------------------------------
-        RECSIG     Hash_of_key      Len_of_key      DATA_for_key
-        RECSEP     Hash_of_payload  Len_of_payload  DATA_for_payload
+            RECSIG     Hash_of_key      Len_of_key      DATA_for_key
+            RECSEP     Hash_of_payload  Len_of_payload  DATA_for_payload
 
-            .
-            .
-            .
+        Deleted records are marked with RECSIG mutated from RECB to RECX
 
-        RECSIG     Hash_of_key      Len_of_key      DATA_for_key
-        RECSEP     Hash_of_payload  Len_of_payload  DATA_for_payload
+        New data is appended to the end, no duplicate filtering is done.
+        Retrieval is searched from reverse, the latest record with this key
+        is retrieved first.
 
-    Deleted records are marked with RECSIG mutated from RECB to RECX
+        Verbosity:    (use the '-v' option multiple times)
 
-    New data is appended to the end, no duplicate filtering is done.
-    Retrieval is searched from reverse, the latest record with this key
-    is retrieved first.
+            0 =  no output
+            1 =  normal, some items printed, short record ;
+            2 =  more detail; full record (-vv)
+            3 =  more detail + damaged records (-vvv)
 
-    Verbosity:    (use the '-v' option multiple times)
+        Debug:    (use the '-d' option with number)
 
-        0 =  no output
-        1 =  normal, some items printed, short record ;
-        2 =  more detail; full record (-vv)
-        3 =  more detail + damaged records (-vvv)
+            0 =  no output
+            1 =  normal, some items
+            2 =  more details
 
-    Debug:    (use the '-d' option with number)
+        History:
 
-        0 =  no output
-        1 =  normal, some items
-        2 =  more details
-
-    History:
-
-        Sat 04.Feb.2023     --  Converted from CURRDATA to ftell
+            1.1         Tue 20.Feb.2024     Initial release
+            1.2.0       Mon 26.Feb.2024     Moved pip home to pydbase/
+            1.4.0       Tue 27.Feb.2024     Addedd pgdebug
+            1.4.2       Wed 28.Feb.2024     Fixed multiple instances
+            1.4.3       Wed 28.Feb.2024     ChainAdm added
+            1.4.4       Fri 01.Mar.2024     Tests for chain functions
+            1.4.5       Fri 01.Mar.2024     Misc fixes
+            1.4.6       Mon 04.Mar.2024     Vacuum count on vacuumed records
+            1.4.7       Tue 05.Mar.2024     In place record update
+            1.4.8       Sat 09.Mar.2024     Added new locking mechanism
 
 '''
 
 import  os, sys, getopt, signal, select, socket, time, struct
 import  random, stat, os.path, datetime, threading
 import  struct, io
 
 base = os.path.dirname(os.path.realpath(__file__))
+sys.path.append(os.path.join(base))
 sys.path.append(os.path.join(base, '..', 'pydbase'))
 
 from twinbase import *
 
 Version = "1.4.8"
 
 # ------------------------------------------------------------------------
@@ -80,17 +88,18 @@
         self.cnt = 0
         self.fname = fname
         self.lckname  = os.path.splitext(self.fname)[0] + ".lock"
         self.idxname  = os.path.splitext(self.fname)[0] + ".pidx"
         self.pgdebug = pgdebug
         self.base_verbose  = 0
         self.devmode = devmode
+        self.lock = FileLock(self.lckname)
 
         # Make sure only one process can use this
-        waitlock(self.lckname)
+        self.lock.waitlock() #self.lckname)
 
         super(TwinCore, self).__init__(pgdebug)
 
         #print("initializing core with", fname, pgdebug)
         #self.pool = threading.BoundedSemaphore(value=1)
 
         # It was informative at one point
@@ -136,32 +145,34 @@
             indexsize = self.getsize(self.ifp)
 
             # See if valid index
             if indexsize < HEADSIZE:
                 self.create_idx(self.ifp)
                 # It was an existing data, new index needed
                 if self.base_verbose > 0:
-                        print("Reindexing")
+                    print("Reindexing")
                 self.__reindex()
 
         # Check
         if  self.getbuffstr(0, 4) != FILESIG:
-            print("Invalid data signature")
-            dellock(self.lckname)
+            if self.base_verbose > 2:
+                print("Invalid data signature")
+            self.lock.unlock()  #dellock(self.lckname)
             raise  RuntimeError("Invalid database signature.")
 
         #print("buffsize", buffsize, "indexsize", indexsize)
-        dellock(self.lckname)
+        self.lock.unlock() #dellock(self.lckname)
 
     def version(self):
+        ''' Return version sting. '''
         return Version
 
     def flush(self):
 
-        ''' Flush files to disk '''
+        ''' Flush files to disk. '''
 
         if self.pgdebug > 9:
             print("Flushing", self.fp, self.ifp)
 
         try:
             if hasattr(self, "fp"):
                 if self.fp:
@@ -169,22 +180,27 @@
             if hasattr(self, "ifp"):
                 if self.ifp:
                     self.ifp.flush()
         except:
             print("Cannot flush files", sys.exc_info())
 
     def getdbsize(self):
+
+        ''' Return the DB size in records. This includes ALL records, including
+        deleted and damaged. This number can be used to iterate all records
+        in the database. Usually from end to beginning. '''
+
         ret = self._getdbsize(self.ifp)
         if not ret:
             ret = 0
         return ret
 
     def _getdbsize(self, ifp):
 
-        ''' Return number of records. Return total including deleted / damaged '''
+        ''' Return number of records. Return total including deleted / damaged. '''
 
         try:
             #chash = self.getidxint(CURROFFS) - HEADSIZE
             chash = self.getsize(ifp) - HEADSIZE
             ret = int(chash / (2 * self.INTSIZE))
         except:
             ret = 0
@@ -244,40 +260,56 @@
         return arr
 
     # -------------------------------------------------------------------
     # Originator, dump single record
 
     def  dump_rec(self, rec, cnt):
 
-        ''' Print record to the screen '''
+        ''' Print record to the screen. '''
+
+        if self.pgdebug > 1:
+            print("Dump Rec at", rec)
 
         cnt2 = 0
         sig = self.getbuffstr(rec, self.INTSIZE)
+        if self.pgdebug > 5:
+            print("Sig ", sig, "at", rec)
 
         if sig == RECDEL:
             if base_showdel:
                 klen = self.getbuffint(rec+8)
                 kdata = self.getbuffstr(rec+12, klen)
                 rec2 = rec + 16 + klen;
                 blen = self.getbuffint(rec2+4)
                 data = self.getbuffstr(rec2+8, blen)
-
                 print(" Del at", rec, "key:", kdata, "data:", truncs(data))
+            if self.base_verbose > 1:
+                klen = self.getbuffint(rec+8)
+                kdata = self.getbuffstr(rec+12, klen)
+                rec2 = rec + 16 + klen;
+                blen = self.getbuffint(rec2+4)
+                data = self.getbuffstr(rec2+8, blen)
+                if self.base_verbose > 2:
+                    print(" Del at", rec, "key:", kdata, "data:", data)
+                else:
+                    print(" Del at", rec, "key:", kdata, "data:", truncs(data))
+
             return cnt2
 
         if sig != RECSIG:
             if self.base_verbose > 1:
                 print(" Damaged data (sig) '%s' at" % sig, rec)
             return cnt2
 
         hash = self.getbuffint(rec+4)
         blen = self.getbuffint(rec+8)
 
         if blen < 0:
-            print("Invalid key length %d at %d" % (blen, rec))
+            if self.base_verbose > 2:
+                print("Invalid key length %d at %d" % (blen, rec))
             return cnt2
 
         data = self.getbuffstr(rec+12, blen)
         if base_integrity:
             ccc = self.hash32(data)
             if self.base_verbose > 1:
                 print("rec", rec, "hash", hex(hash), "check", hex(ccc))
@@ -293,15 +325,16 @@
             return cnt2
 
         rec2 = rec + 16 + blen;
         hash2 = self.getbuffint(rec2)
         blen2 = self.getbuffint(rec2+4)
 
         if blen2 < 0:
-            print("Invalid data length %d at %d" % (blen2, rec))
+            if self.base_verbose > 1:
+                print("Invalid data length %d at %d" % (blen2, rec))
             return cnt2
 
         data2 = self.getbuffstr(rec2+8, blen2)
         if base_integrity:
             ccc2 = self.hash32(data2)
             if self.base_verbose > 1:
                 print("rec", rec, "hash2", hex(hash), "check2", hex(ccc))
@@ -330,14 +363,16 @@
         ''' Check record. Verbose to the screen. Return number of errors.'''
 
         ret = 0
         sig = self.getbuffstr(rec, self.INTSIZE)
 
         # Do not check deleted, say OK
         if sig == RECDEL:
+            if self.base_verbose > 1:
+                print(" Deleted data '%s' at %d (%d)" % (sig, rec, cnt2))
             ret = 1
             return ret
 
         if sig != RECSIG:
             if self.base_verbose > 0:
                 print(" Damaged data (sig) '%s' at %d (%d)" % (sig, rec, cnt2))
             #if self.base_verbose > 1:
@@ -352,19 +387,20 @@
             if self.base_verbose > 1:
                 print("Invalid key length %d at %d" % (blen, rec))
             return ret
 
         data = self.getbuffstr(rec+12, blen)
         ccc = self.hash32(data)
         if hash != ccc:
-            if self.base_verbose > 0:
-                print("Error on hash at rec", rec, cnt2, "hash", hex(hash), "check", hex(ccc))
-
             if self.base_verbose > 1:
                 print("Data", data)
+            elif self.base_verbose > 0:
+                print("Error on hash at rec", rec, cnt2, "hash",
+                                            hex(hash), "check", hex(ccc))
+
             return ret
 
         endd = self.getbuffstr(rec + 12 + blen, self.INTSIZE)
         if endd != RECSEP:
             if self.base_verbose > 0:
                 print(" Damaged data (sep) '%s' at %d %d %d" % (endd, rec, cnt2))
             return ret
@@ -377,89 +413,106 @@
             if self.base_verbose > 1:
                 print("Invalid data length2 %d at %d" % (blen2, rec))
             return ret
 
         data2 = self.getbuffstr(rec2+8, blen2)
         ccc2 = self.hash32(data2)
         if hash2 != ccc2:
-            if self.base_verbose > 0:
-                print("Error on hash2 at rec", rec, cnt2, "hash2", hex(hash2), "check2", hex(ccc2))
             if self.base_verbose > 1:
                 print("Data", data, "Data2", data2)
+            elif self.base_verbose > 0:
+                print("Error on hash2 at rec", rec, cnt2, "hash2",
+                                        hex(hash2), "check2", hex(ccc2))
             return ret
 
         if self.base_verbose > 2:
             print("Record at %d (%d) OK." % (rec, cnt2))
 
         ret += 1
         return ret
 
     # --------------------------------------------------------------------
     # Internal; no locking
 
     def  __dump_data(self, lim = INT_MAX, skip = 0, dirx = 0):
 
-        if self.pgdebug:
-            print("dump_data()", "lim =", hex(lim), "skip=", skip, "dirx =", dirx)
+        ''' Put all data to screen worker function. '''
 
-        ''' Put all data to screen worker function '''
+        #if self.pgdebug:
+        #    print("dump_data()", "lim =", hex(lim), "skip=", skip, "dirx =", dirx)
 
         cnt = skip; cnt2 = 0
         curr =  chash = HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
 
         # Direction sensitivity
         if dirx:
             rrr = range(HEADSIZE + skip * self.INTSIZE * 2, chash, self.INTSIZE * 2)
         else:
             rrr = range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2)
 
         for aa in rrr:
             rec = self.getidxint(aa)
+
             #print(aa, rec)
             if not base_quiet:
                 cnt2 += 1
                 ret = self.dump_rec(rec, cnt)
+
+                if not ret:
+                    if self.pgdebug > 5:
+                        print("Deleted / empty record at", cnt)
+
                 if ret:
                     cnt += 1
                     if cnt >= lim:
                         break
 
     def  dump_data(self, lim = INT_MAX, skip = 0):
 
-        ''' Put all data to screen '''
+        ''' Put all data to screen. '''
 
         self.__dump_data(lim, skip, 1)
 
     def  revdump_data(self, lim, skip = 0):
 
-        ''' Put all data to screen in reverse order '''
+        ''' Put all data to screen in reverse order. '''
 
         self.__dump_data(lim, skip)
 
     def  reindex(self):
 
-        ''' Re create index file '''
+        ''' Re create index file. '''
 
-        waitlock(self.lckname)
+        self.lock.waitlock() #self.lckname)
         ret = self.__reindex()
-        dellock(self.lckname)
+        self.lock.unlock()    #dellock(self.lckname)
         return ret
 
     # --------------------------------------------------------------------
 
     def  __reindex(self):
 
         ''' Recover index. Make sure the DB in not in session.  '''
 
         ret = 0
 
         #curr = self.getbuffint(CURROFFS) - HEADSIZE
         curr =  self._getdbsize(self.ifp) * self.INTSIZE * 2
 
         reidx = os.path.splitext(self.fname)[0]  + "_tmp_" + ".pidx"
+        relock = os.path.splitext(self.fname)[0]  + "_tmp_" + ".pidx"
+        # Make sure reidx is empty
+        try:
+            os.remove(reidx)
+        except:
+            pass
+
+        tmplock = FileLock(relock)
+        tmplock.waitlock()
+
         tempifp = self.softcreate(reidx)
         self.create_idx(tempifp)
         dlen = self.getsize(self.fp)
 
         if self.base_verbose > 2:
            print("curr", curr, "dlen", dlen)
 
@@ -467,30 +520,34 @@
         while 1:
             if aa >= dlen:
                 break
 
             sig = self.getbuffstr(aa, self.INTSIZE)
             # Check if sig is correct
             if sig != RECSIG:
-                print("Invalid sig .. resync needed")
+                if self.core_verbose > 0:
+                    print("Invalid sig .. resync needed")
                 raise
 
             #print("reind", aa)
 
             try:
                 hhh2 = self.getbuffint(aa + 4)
                 lenx = self.getbuffint(aa + 8)
                 if lenx < 0:
-                    print("Invalid key length")
+                    if self.core_verbose > 0:
+                        print("Invalid key length.")
                 sep =  self.getbuffstr(aa + 12 + lenx, self.INTSIZE)
                 len2 =  self.getbuffint(aa + 20 + lenx)
                 if len2 < 0:
-                    print("Invalid record length")
+                    if self.core_verbose > 0:
+                        print("Invalid record length")
             except:
-                print("in reindex", sys.exc_info())
+                if self.core_verbose > 2:
+                    print("in reindex", sys.exc_info())
 
             if self.base_verbose == 1:
                 print(aa, "sig", sig, "hhh2", hex(hhh2), "len", lenx, \
                     "sep", sep, "len2", len2)
             if self.base_verbose > 1:
                 data =  self.getbuffstr(aa + 12, lenx)
                 data2 =  self.getbuffstr(aa + 24 + lenx, len2)
@@ -508,29 +565,38 @@
 
             #self._putint(tempifp, hashpos, self.fp.tell())
 
             # This is dependent on the database structure
             aa += lenx + len2 + 24
             ret += 1
 
+        tempifp.flush()
+        tempifp.close()
+
         # Make it go out of scope
-        self.fp.flush()
-        self.ifp.flush();
+        #self.fp.flush()
+        #self.fp.close()
+        self.ifp.flush()
         self.ifp.close()
-        tempifp.flush();
-        tempifp.close()
 
         # Now move files
         try:
             os.remove(self.idxname)
         except:
             pass
+            #print("remove:", sys.exc_info())
 
         #print("rename", reidx, "->", self.idxname)
-        os.rename(reidx, self.idxname)
+        try:
+            os.rename(reidx, self.idxname)
+        except:
+            pass
+            #print("rename:", sys.exc_info())
+
+        tmplock.unlock()
 
         # Activate new index
         self.ifp = self.softcreate(self.idxname)
         return ret
 
     def __save_error(self, rec, vacerrfp):
 
@@ -552,21 +618,24 @@
         if not found:
             vacerrfp.write(ddd)
 
     # ----------------------------------------------------------------
 
     def  vacuum(self):
 
-        ''' Remove all deleted data. Reindex.
-            Make sure the db in not in session, and no pending
-            operations are  present (like find / retrieve cycle)'''
+        '''
+            Remove all deleted data. Reindex.
+            The db is locked while the vacuum is in operation, but
+            make sure the DB in not in session, and no pending
+            operations are present (like find / retrieve cycle).
+        '''
 
-        waitlock(self.lckname)
+        self.lock.waitlock() #self.lckname)
         ret = self._vacuum()
-        dellock(self.lckname)
+        self.lock.unlock()  #dellock(self.lckname)
         return ret
 
     def  _vacuum(self):
 
         vacname = os.path.splitext(self.fname)[0] + "_vac_" + ".pydb"
         vacerr  = os.path.splitext(self.fname)[0] +  ".perr"
         vacidx = os.path.splitext(vacname)[0]  + ".pidx"
@@ -588,15 +657,15 @@
             os.remove(vacidx)
         except:
             pass
 
         # It is used to raise the scope so vacuumed DB closes
         if 1:
             vacdb = TwinCore(vacname)
-            waitlock(vacdb.lckname)
+            vacdb.lock.waitlock()
 
             skip = 0; cnt = 0
             chash =  self._getdbsize(self.ifp) * self.INTSIZE * 2
             rrr = range(HEADSIZE + skip * self.INTSIZE * 2, chash + HEADSIZE, self.INTSIZE * 2)
             for aa in rrr:
                 rec = self.getidxint(aa)
                 sig = self.getbuffstr(rec, self.INTSIZE)
@@ -610,15 +679,15 @@
                         print("Detected error at %d" % rec)
                     ret += 1
                     self.__save_error(rec, vacerrfp)
                 else:
                     global base_integrity
                     tmpi = base_integrity
                     base_integrity = True
-                    arr = self.get_rec_offs(rec)
+                    arr = self.get_rec_byoffs(rec)
                     base_integrity = tmpi
 
                     if self.pgdebug > 1:
                         print(cnt, "vac rec", rec, arr)
 
                     if len(arr) > 1:
                         hhh2 = self.hash32(arr[0])
@@ -628,88 +697,111 @@
                     else:
                         # This could be from empty bacause of hash error
                         self.__save_error(rec, vacerrfp)
                         if self.pgdebug > 0:
                             print("Error on vac: %d" % rec)
                 cnt += 1
 
-            dellock(vacdb.lckname)
+            vacdb.fp.close()
+            vacdb.ifp.close()
+
+            vacdb.lock.unlock()  #dellock(vacdb.lckname)
 
             # if vacerr is empty
             try:
                 if os.stat(vacerr).st_size == 0:
                     #print("Vac error empty")
                     os.remove(vacerr)
             except:
-                print("vacerr", sys.exc_info())
-
-        dellock(self.lckname)
+                if self.core_verbose > 0:
+                    print("vacerr", sys.exc_info())
 
         # Any vacummed?
         if vac > 0:
             # Make it go out of scope
             self.fp.flush(); self.ifp.flush()
             self.fp.close(); self.ifp.close()
 
             # Now move files
             try:
-                os.remove(self.fname);  os.remove(self.idxname)
+                os.remove(self.fname);
             except:
+                if self.core_verbose > 0:
+                    print("vacuum remove", self.fname, sys.exc_info())
+                pass
+
+            try:
+                os.remove(self.idxname)
+            except:
+                if self.core_verbose > 2:
+                    print("vacuum idx remove", self.idxname, sys.exc_info())
                 pass
 
             if self.pgdebug > 1:
                 print("rename", vacname, "->", self.fname)
                 print("rename", vacidx, "->", self.idxname)
 
-            os.rename(vacname, self.fname)
-            os.rename(vacidx, self.idxname)
+            try:
+                os.rename(vacname, self.fname)
+            except:
+                if self.core_verbose > 2:
+                    print("vacuum rename", vacname, sys.exc_info())
+            try:
+                os.rename(vacidx, self.idxname)
+            except:
+                if self.core_verbose > 2:
+                    print("vacuum idx rename", vacidx, sys.exc_info())
 
-            waitlock(self.lckname)
+            self.lock.waitlock() #self.lckname)
             self.fp = self.softcreate(self.fname)
             self.ifp = self.softcreate(self.idxname)
-            dellock(self.lckname)
+            #self.lock.unlock()  #dellock(self.lckname)
 
         else:
             # Just remove non vacuumed files
             if self.pgdebug > 1:
                 print("deleted", vacname, vacidx)
             try:
                 os.remove(vacname)
                 os.remove(vacidx)
             except:
                 pass
 
+        #self.lock.unlock()
+        #dellock(self.lckname)
+
         #print("ended vacuum")
         return ret, vac
 
     def  get_rec(self, recnum):
 
-        ''' Get record from database; recnum is a zero based record counter '''
+        ''' Get record from database; recnum is a zero based record counter. '''
 
         if self.pgdebug:
             print("getrec()", recnum)
 
         rsize = self._getdbsize(self.ifp)
         if recnum >= rsize:
-            #print("Past end of data.");
+            if self.core_verbose > 0:
+                print("Past end of data.");
             raise  RuntimeError( \
                     "Past end of Data. Asking for %d while max is 0 .. %d records." \
                                      % (recnum, rsize-1) )
             return []
 
         chash = self.getidxint(CURROFFS)
         #print("chash", chash)
         offs = self.getidxint(HEADSIZE + recnum * self.INTSIZE * 2)
 
         #print("offs", offs)
         return self._rec2arr(offs)
 
-    def  get_rec_offs(self, recoffs):
+    def  get_rec_byoffs(self, recoffs):
 
-        ''' Return record by offset '''
+        ''' Return record by offset. '''
 
         rsize = self.getsize(self.fp)
         if recoffs >= rsize:
             #print("Past end of data.");
             raise  RuntimeError( \
                     "Past end of File. Asking for offset %d file size is %d." \
                                      % (recoffs, rsize) )
@@ -717,22 +809,23 @@
 
         sig = self.getbuffstr(recoffs, self.INTSIZE)
         if sig == RECDEL:
             if self.base_verbose:
                 print("Deleted record.")
             return []
         if sig != RECSIG:
-            print("Unlikely offset %d is not at record boundary." % recoffs, sig)
+            if self.core_verbose > 0:
+                print("Unlikely offset %d is not at record boundary." % recoffs, sig)
             return []
         #print("recoffs", recoffs)
         return self._rec2arr(recoffs)
 
     def  get_key_offs(self, recoffs):
 
-        ''' Get key by offset '''
+        ''' Get key by offset. '''
 
         rsize = self.getsize(self.fp)
         if recoffs >= rsize:
             #print("Past end of data.");
             raise  RuntimeError( \
                     "Past end of File. Asking for offset %d file size is %d." \
                                      % (recoffs, rsize) )
@@ -740,15 +833,16 @@
 
         sig = self.getbuffstr(recoffs, self.INTSIZE)
         if sig == RECDEL:
             if self.base_verbose:
                 print("Deleted record.")
             return []
         if sig != RECSIG:
-            print("Unlikely offset %d is not at record boundary." % recoffs, sig)
+            if self.core_verbose > 0:
+                print("Unlikely offset %d is not at record boundary." % recoffs, sig)
             return []
         #print("recoffs", recoffs)
         return self._rec2arr(recoffs)[0]
 
     def  del_rec(self, recnum):
 
         ''' Delete by record number.
@@ -773,96 +867,103 @@
             return False
 
         self.putbuffstr(offs, RECDEL)
         return True
 
     def  del_rec_offs(self, recoffs):
 
-        ''' Delete record by file offset '''
+        ''' Delete record by file offset. '''
 
         rsize = self.getsize(self.fp)
         if recoffs >= rsize:
             #print("Past end of data.");
             raise  RuntimeError( \
                     "Past end of File. Asking for offset %d file size is %d." \
                                      % (recoffs, rsize) )
             return False
 
         sig = self.getbuffstr(recoffs, self.INTSIZE)
         if sig != RECSIG  and sig != RECDEL:
-            print("Unlikely offset %d is not at record boundary." % recoffs, sig)
+            if self.core_verbose > 0:
+                print("Unlikely offset %d is not at record boundary." % recoffs, sig)
             return False
 
         self.putbuffstr(recoffs, RECDEL)
         return True
 
     # Check integrity
 
-    def integrity_check(self, skip = 0):
+    def integrity_check(self, skip = 0, count = 0xffffffff):
 
-        ''' check multiple record integrity Skip number of records '''
+        ''' Check record integrity for 'count' records.
+            Skip number of records.
+        '''
 
-        waitlock(self.lckname)
-        ret = 0; cnt2 = 0
+        self.lock.waitlock()    #(self.lckname)
+        ret = 0; cnt2 = 0; cnt3 = 0;
         #chash = self.getidxint(CURROFFS)        #;print("chash", chash)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         # Direction sensitivity
         rrr = range(HEADSIZE + skip * self.INTSIZE * 2, chash, self.INTSIZE * 2)
         for aa in rrr:
             rec = self.getidxint(aa)
             #print(aa, rec)
             ret += self.check_rec(rec, cnt2)
             cnt2 += 1
-        dellock(self.lckname)
+            cnt3 += 1
+            if cnt3 >= count:
+                break
+        self.lock.unlock() #dellock(self.lckname)
         return ret, cnt2
 
     def  retrieve(self, strx, limx = 1):
 
-        ''' Retrive in reverse, limit it '''
+        ''' Retrive in reverse, limit it. '''
 
         if type(strx) != type(b""):
             strx = strx.encode(errors='strict')
 
         hhhh = self.hash32(strx)
         if self.pgdebug > 2:
             print("strx", strx, hhhh)
 
         #chash = self.getidxint(CURROFFS)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
 
         #;print("chash", chash)
         arr = []
 
-        waitlock(self.lckname)
+        self.lock.waitlock() #(self.lckname)
 
         #for aa in range(HEADSIZE + self.INTSIZE * 2, chash, self.INTSIZE * 2):
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2):
             rec = self.getidxint(aa)
             sig = self.getbuffstr(rec, self.INTSIZE)
             if sig == RECDEL:
                 if self.base_verbose > 3:
                     print(" Deleted record '%s' at" % sig, rec)
             elif sig != RECSIG:
                 if self.base_verbose:
                     print(" Damaged data '%s' at" % sig, rec)
             else:
                 hhh = self.getbuffint(rec+4)
                 if hhh == hhhh:
-                    arr.append(self.get_rec_offs(rec))
+                    arr.append(self.get_rec_byoffs(rec))
                     if len(arr) >= limx:
                         break
-        dellock(self.lckname)
+        self.lock.unlock()  #dellock(self.lckname)
 
         return arr
 
     # Return record offset
 
     def  _recoffset(self, strx, limx = INT_MAX, skipx = 0):
 
-        #chash = self.getidxint(CURROFFS)            #;print("chash", chash)
+        #chash = self.getidxint(CURROFFS)
+        #;print("chash", chash)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         rec = 0; blen = 0; data = ""
         arr = []
         if type(strx) != type(b""):
             strx2 = strx.encode(errors='strict');
         else:
             strx2 = strx
@@ -890,17 +991,17 @@
                     data = self.getbuffstr(rec + 24 + blen, xlen)
                     #print("rec offset", rec + 12,  "key:", keyz, "data:", data)
                     break       # Only the last one
         return rec, rec+24 + blen, len(data)
 
     def  findrec(self, strx, limx = INT_MAX, skipx = 0):
 
-        ''' Find by string matching substring '''
+        ''' Find by string matching substring. '''
 
-        waitlock(self.lckname)
+        self.lock.waitlock()    #(self.lckname)
 
         #chash = self.getidxint(CURROFFS)            #;print("chash", chash)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
 
         arr = []
         strx2 = strx.encode(errors='strict');
 
@@ -924,23 +1025,23 @@
                 #if str(strx2) in str(data):
                 if strx2 in data:
                     arr.append(self.get_key_offs(rec))
                     #arr.append(rec)
 
                     if len(arr) >= limx:
                         break
-        dellock(self.lckname)
+        self.lock.unlock()  #dellock(self.lckname)
 
         return arr
 
     def  findrecpos(self, strx, limx = INT_MAX, skipx = 0):
 
-        ''' Find record, return array of positions '''
+        ''' Find record, return array of positions. '''
 
-        waitlock(self.lckname)
+        self.lock.waitlock()    #(self.lckname)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         arr = []
         if type(strx) != type(b""):
             strx = strx.encode(errors='strict');
 
         for aa in range(chash - self.INTSIZE * 2, HEADSIZE  - self.INTSIZE * 2, -self.INTSIZE * 2):
             rec = self.getidxint(aa)
@@ -957,23 +1058,23 @@
                 if self.base_verbose > 1:
                     print("frecpos", data)
                 if strx == data:
                     arr.append(rec)
                     if len(arr) >= limx:
                         break
 
-        dellock(self.lckname)
+        self.lock.unlock()  #dellock(self.lckname)
 
         return arr
 
     def  findrec(self, strx, limx = INT_MAX, skipx = 0):
 
-        ''' Find by string matching substring '''
+        ''' Find by string matching substring. '''
 
-        waitlock(self.lckname)
+        self.lock.waitlock()    #(self.lckname)
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         arr = []
         if type(strx) != type(b""):
             strx2 = strx.encode(errors='strict');
 
         #print("findrec", strx2)
 
@@ -995,26 +1096,26 @@
                 #if str(strx2) in str(data):
                 if strx2 in data:
                     #arr.append(self.get_key_offs(rec))
                     #arr.append(rec)
                     arr.append(self._rec2arr(rec))
                     if len(arr) >= limx:
                         break
-        dellock(self.lckname)
+        self.lock.unlock()    #dellock(self.lckname)
 
         return arr
 
     # --------------------------------------------------------------------
     # List all active records
 
     def  listall(self):
 
-        ''' List all active records. Return array id record indexes'''
+        ''' List all active records. Return array id record indexes. '''
 
-        waitlock(self.lckname)
+        self.lock.waitlock()    #(self.lckname)
         keys = []; arr = []; cnt = 0
 
         chash =  HEADSIZE  + self._getdbsize(self.ifp) * self.INTSIZE * 2
         maxrec = chash - self.INTSIZE * 2
         rsize = self._getdbsize(self.ifp) - 1
 
         rrr =  range(maxrec,
@@ -1038,23 +1139,23 @@
                         keys.append(hhh)
                         # as we are going backwards
                         arr.append(rsize - cnt)
                         #print("found", hhh)
             cnt += 1
 
         keys = []
-        dellock(self.lckname)
+        self.lock.unlock()  #dellock()self.lckname)
 
         return arr
 
     def  find_key(self, keyx, limx = 0xffffffff):
 
         ''' Find record by key Search from the end, so latest comes first. '''
 
-        waitlock(self.lckname)
+        self.lock.waitlock()   #self.lckname)
 
         skip = 0; arr = []; cnt = 0
         try:
             arg2e = keyx.encode()
         except:
             arg2e = keyx
 
@@ -1083,22 +1184,22 @@
                         break
                     arr.append(rec)
                 else:
                     pass
                     #print("no match", hex(hhh))
 
             cnt += 1
-        dellock(self.lckname)
+        self.lock.unlock()  #dellock()self.lckname)
 
         return arr
 
 
     def  del_data(self, hash, skip = 1):
 
-        ''' Delete data by hash '''
+        ''' Delete data by hash. '''
 
         cnt = skip
         hhhh = int(hash, 16)                #;print("hash", hash, hhhh)
         curr = self.getbuffint(CURROFFS)    #;print("curr", curr)
         chash = self.getidxint(CURROFFS)    #;print("chash", chash)
 
         arr = []
@@ -1122,21 +1223,31 @@
 
             cnt += 1
 
         return arr
 
     def  del_rec_bykey(self, strx, maxdelrec = 0xffffffff, skip = 0, dirx = 0):
 
-        ''' Remove record by key. Remove maxdelrec occurances '''
+        ''' Remove record by key. Remove maxdelrec occurances.
+
+                    Input:
+                        strx            key to remove
+                        maxdelrex       maximum number of records to delete
+                        skip            start scanning from offset
+                        dirx            False for scanning down, True for up
+                    Return:
+                        count of records removed
+
+            '''
 
         if self.pgdebug:
             print("del_rec_bykey()", strx)
 
         ''' Delete records by key string; needs bin str, converted
-            automatically on entry
+            automatically on entry.
         '''
 
         if type(strx) != type(b""):
             strx = strx.encode()
 
         if self.base_verbose > 1:
             print("Start delete ", strx, "skip", skip)
@@ -1173,57 +1284,62 @@
                     self.putbuffstr(rec, RECDEL)
                     cnt += 1
                     if cnt >= maxdelrec:
                         break
             cnt3 += 1
         return cnt
 
-    def  save_data(self, arg2, arg3, replace = False):
+    def  save_data(self, header, datax, replace = False):
 
         ''' Append to the end of file. If replace flag is set, try to overwrite
             in place. If new record is larger, add it as ususal. If smaller,
             the record is padded with spaces. This should not influence most ops.
             (like: int())
             This feature allows the database update wthout creating new records.
             Useful for counters or dynamically changing data.
-         '''
+
+                    Input:
+                        header     Header
+                        datax      Data
+
+                     Return:
+                        The offset of saved data
+            '''
 
         if self.pgdebug > 0:
-            print("Save_data()", arg2, arg3)
+            print("Save_data()", header, datax)
 
-        waitlock(self.lckname)
+        self.lock.waitlock()   #self.lckname)
         ret = 0
         was = False
         # Put new data in place
         if replace:
-            if type(arg3) != type(b""):
-                mrep2 = arg3.encode()
+            if type(datax) != type(b""):
+                mrep2 = datax.encode()
             else:
-                mrep2 = arg3
+                mrep2 = datax
 
-            rrr = self._recoffset(arg2, 1)
-            if rrr[2]:
-                #print("Replace rec", hex(rrr[0]), "len:", rrr[1])
-                if len(mrep2) <= rrr[2]:
-                    #print("Fit")
-                    padded = mrep2 + b' ' * (rrr[1] - len(mrep2))
-                    #print("Padded", padded)
+            rrr = self._recoffset(header, 1)
+            arr = self.get_rec_byoffs(rrr[0])
+            #print(arr)
+            if arr:
+                #print("Replace rec", arr[1], "len:", arr[1])
+                if len(mrep2) <= len(arr[1]):
+                    padded = mrep2 + b' ' * (len(arr[1]) - len(mrep2) )
+                    #print("Padded", b"'" + padded + b"'")
                     ccc = self.hash32(padded)
                     self.putbuffint(rrr[1] - 8, ccc)
                     #print("ccc", hex(ccc))
                     self.putbuffstr(rrr[1], padded)
                     was = True
-                    # This was helpful ... but more systematic approach is needed
-                    self.fp.flush()
-                    self.ifp.flush()
                     ret =  rrr[0]
         if not was:
-            ret = self._save_data2(arg2, arg3)
+            ret = self._save_data2(header, datax)
 
-        dellock(self.lckname)
+        self.lock.unlock()  #dellock()self.lckname)
 
         return ret
 
     # --------------------------------------------------------------------
     # Save data to database file
 
     def  _save_data2(self, arg2, arg3):
@@ -1231,15 +1347,15 @@
         # Prepare all args, if cannot encode, use original
         if type(arg2) != type(b""):
             arg2 = arg2.encode()
         if type(arg3) != type(b""):
             arg3 = arg3.encode()
 
         if self.pgdebug > 1:
-            print("args", arg2, "arg3", arg3)
+            print("Save_data2() args", arg2, "arg3", arg3)
 
         hhh2 = self.hash32(arg2)
         hhh3 = self.hash32(arg3)
 
         if self.pgdebug > 1:
             print("_save_data2 hhh2", hhh2, "hhh3", hhh3)
 
@@ -1292,26 +1408,28 @@
         self.fp.flush()
         self.ifp.flush()
 
         return curr
 
     def __del__(self):
 
-        ''' flush file handles and close files '''
+        ''' flush file handles and close files. '''
 
         if hasattr(self, "pgdebug"):
             if self.pgdebug > 9:
                 print("__del__ called.")
 
         #self.flush()
 
         if hasattr(self, "fp"):
                 if self.fp:
-                    self.fp.flush()
-                    self.fp.close()
+                    if not self.fp.closed:
+                        self.fp.flush()
+                        self.fp.close()
 
         if hasattr(self, "ifp"):
                 if self.ifp:
-                    self.ifp.flush()
-                    self.ifp.close()
+                    if not self.ifp.closed:
+                        self.ifp.flush()
+                        self.ifp.close()
 
 # EOF
```

### Comparing `pydbase-1.4.8/pydbase.egg-info/PKG-INFO` & `pydbase-1.5.0/pydbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydbase
-Version: 1.4.8
+Version: 1.5.0
 Summary: High speed database with key / data in python.
 Home-page: https://github.com/pglen/pydbase
 Author: Peter Glen
 Author-email: peterglen99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 #### see: blockchain functions at the end
 
  &nbsp; The motivation was to create a no frills way of saving / retrieving data.
 It is fast, and the time test shows that this is an order of magnitude
 faster than most mainstream databases. This is due to the engine's simplicity.
 It avoids expensive computations in favor of quickly saving data.
 
-### Fast data save / retrieve
+### Fast data save / retrieve 
 
  &nbsp; Mostly ready for production. All tests pass. Please use caution, as this is new.
 The command line tester can drive most aspects of this API; and it is somewhat
 complete. It is also  good way to see the API / Module in action.
 
 ## API
```

### Comparing `pydbase-1.4.8/pydbase.egg-info/SOURCES.txt` & `pydbase-1.5.0/pydbase.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 README.md
 chainadm.py
 dbaseadm.py
 setup.py
 pydbase/__init__.py
 pydbase/dbutils.py
+pydbase/portalocker.py
 pydbase/twinbase.py
 pydbase/twinchain.py
 pydbase/twincore.py
 pydbase.egg-info/PKG-INFO
 pydbase.egg-info/SOURCES.txt
 pydbase.egg-info/dependency_links.txt
 pydbase.egg-info/entry_points.txt
 pydbase.egg-info/top_level.txt
+pydbase/docs/twinbase.html
+pydbase/docs/twinchain.html
+pydbase/docs/twincore.html
 tests/test_acreate.py
 tests/test_bigdata.py
 tests/test_bindata.py
 tests/test_chain.py
 tests/test_chain_data.py
 tests/test_chain_link.py
 tests/test_del.py
@@ -27,11 +31,10 @@
 tests/test_handles.py
 tests/test_inplace.py
 tests/test_integrity.py
 tests/test_list.py
 tests/test_lockrel.py
 tests/test_multi.py
 tests/test_packer.py
-tests/test_randdata.py
 tests/test_reindex.py
 tests/test_search.py
 tests/test_vacuum.py
```

### Comparing `pydbase-1.4.8/setup.py` & `pydbase-1.5.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import setuptools
+import os, sys
 
 descx = '''
         It is an insanely simple database. Fast. If all you need is a key / value
         pair, this is the perfect solution.
         (Yes, all you need is a key / value pair, as any and every structure
         can be built out of it)
 '''
@@ -15,40 +16,46 @@
           'License :: OSI Approved :: Python Software Foundation License',
           'Operating System :: Microsoft :: Windows',
           'Operating System :: POSIX',
           'Programming Language :: Python',
           'Topic :: Databases',
         ]
 
-#includex = ["pydbase/"]
+includex = ["*", "pydbase/", ]
+versionx = "1.5.0"
+
+doclist = []; droot = "pydbase/docs/"
+doclistx = os.listdir(droot)
+for aa in doclistx:
+    doclist.append(droot + aa)
+#print(doclist)
+#sys.exit()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pydbase",
-    version="1.4.8",
+    version=versionx,
     author="Peter Glen",
     author_email="peterglen99@gmail.com",
     description="High speed database with key / data in python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pglen/pydbase",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     include_package_data=True,
-    #packages=setuptools.find_packages(include=includex),
-    packages = ["pydbase",],
+    packages=setuptools.find_packages(include=includex),
     scripts = ['dbaseadm.py', 'chainadm.py'],
     py_modules = ["pyvpacker",],
-    #package_dir = {'': '.'},
-
+    package_data = {"docs" : doclist},
     python_requires='>=3',
     entry_points={
         'console_scripts': [ "dbaseadm=dbaseadm:mainfunc",
                                 "chainadm=chainadm:mainfunc",
                            ],
     },
 )
```

### Comparing `pydbase-1.4.8/tests/test_acreate.py` & `pydbase-1.5.0/tests/test_find.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 #!/usr/bin/env python3
 
-import pytest, os, sys
-
-fff = __file__[:]
+import pytest, os, sys, random
 from mytest import *
 import twincore, pyvpacker
 
 core = None
+fname = createname(__file__)
+iname = createidxname(__file__)
 
 def setup_module(module):
     """ setup any state specific to the execution of the given module."""
     global core
-    core = create_db()
-    assert core != None
+    core = create_db(fname)
+    assert core != 0
+
+    ret = core.save_data("1111", "2222")
+    assert ret != 0
+    ret = core.save_data("11111", "22222")
+    assert ret != 0
+    ret = core.save_data("111", "222")
+    assert ret != 0
 
 def teardown_module(module):
     """ teardown any state that was previously setup with a setup_module
     method.
     """
     uncreate_db()
 
@@ -28,44 +35,28 @@
     #assert tmp_path == ""
     #assert 0, "test here, function %s" % function.__name__
     pass
 
 # ------------------------------------------------------------------------
 # Start
 
-def test_create(tmp_path):
-    global core
-    try:
-        # Fresh start
-        #os.remove("data/tests.pydb")
-        #os.remove("data/tests.pidx")
-        pass
-    except:
-        pass
-
-def test_write():
-    print("write", core)
-    ret = core.save_data("1111", "2222")
-    assert ret != 0
-    ret = core.save_data("11111", "22222")
-    assert ret != 0
-    ret = core.save_data("111", "222")
-    assert ret != 0
-
 def test_get():
     ret = core.get_rec(2)
     assert ret != 0
+    print(ret)
     assert ret == [b'111', b'222']
 
-def test_read():
-    ret = core.retrieve("111")
-    assert ret == [[b'111', b'222']]
-
-    ret = core.retrieve("1111")
-    assert ret == [[b'1111', b'2222']]
-
-def test_create_file(tmp_path):
-    #print("tmp_path", tmp_path)
-    #assert core == 0
-    pass
+def test_search():
+
+    #return
+
+    strx = "1111"
+    ret = core.findrec(strx, 1)
+    #print(ret)
+    assert ret ==[[b'11111', b'22222']]
+
+    strx = "11111"
+    ret = core.findrec(strx, 1)
+    #print(ret)
+    assert ret == [[b'11111', b'22222']]
 
 # EOF
```

### Comparing `pydbase-1.4.8/tests/test_bigdata.py` & `pydbase-1.5.0/tests/test_bigdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from mytest import *
 
 #import twincore, pyvpacker
 
 # Test for pydbase
 
 core = None
-
 fname = createname(__file__)
 iname = createidxname(__file__)
 
 bigdata = "Fill Data " * 100
 bigbigdata = "Fill Data " * 1000000
 
 def setup_module(module):
```

### Comparing `pydbase-1.4.8/tests/test_bindata.py` & `pydbase-1.5.0/tests/test_chain.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 #!/usr/bin/env python3
 
 import pytest, os, sys
 from mytest import *
-import twincore, pyvpacker
+
+import twinchain, pyvpacker
 
 core = None
 fname = createname(__file__)
 iname = createidxname(__file__)
 
+ddd = \
+ ['rput', 'vote',
+ ['1707765075.806346', '39c91dc0c9d811ee99d0eb7f258547e4',
+ {'PayLoad': {'Default': '', 'Vote': 0,
+  'UID': 'ca81f62ed5574acaa4a105192da5c631'}},
+  #{'_PowRand': b'\x84\xcd\xb2\xb3\xb9\xe9t\xcd\x15\xe2\x95\xb4'},
+  {'_Hash': 'd0b28280f5810041336982b423522d67e740692c36f7a311fdcc9fd3ef419d0f'},
+  {'_Proof': 'dfd58c2cc281cee281631d20a2032332af26d0df8a8f758043f2098ff9bae000'}
+  ]]
+
 # ------------------------------------------------------------------------
 
 def setup_module(module):
     """ setup any state specific to the execution of the given module."""
     global core
 
     try:
         # Fresh start
         os.remove(fname)
         os.remove(iname)
     except:
         #print(sys.exc_info())
         pass
 
-    core = twincore.TwinCore(fname)
+    core = twinchain.TwinChain(fname)
     assert core != 0
 
-    # Create a database of 500 random records
-    for aa in range(500):
-        key = randbin(random.randint(6, 12))
-        val = randbin(random.randint(24, 96))
-        ret = core.save_data(str(key), str(val))
-        assert ret != 0
-
 def teardown_module(module):
     """ teardown any state that was previously setup with a setup_module
     method.
     """
 
     try:
         # No dangling data
@@ -46,43 +50,18 @@
         print(sys.exc_info())
         #assert 0
         pass
 
     #assert 0
 
 
-def test_bindata(capsys):
-
-    dbsize = core.getdbsize()
-
-    ddd = []
-    for aa in range(dbsize):
-        vvv = core.get_rec(aa)
-        ddd.append(vvv)
-
-    #core.core_verbose = 2
-    core.reindex()
-    dbsize2 = core.getdbsize()
-    #core.core_verbose = 0
-    assert dbsize == dbsize2
-
-    nnn = []
-    try:
-        for aa in range(dbsize2):
-            vvv = core.get_rec(aa)
-            nnn.append(vvv)
-    except:
-        pass
+def test_data(capsys):
 
-    try:
-        # No dangling data
-        #os.remove(fname)
-        #os.remove(iname)
-        pass
-    except:
-        print(sys.exc_info())
-        #assert 0
-        pass
+    pay  = "payload string " * 10
 
-    assert nnn == ddd
+    core.append(pay)
+    dbsize = core.getdbsize()
+    payload = core.get_payload(dbsize-1)
+    #print(payload[1], pay)
+    assert payload[1] == pay
 
 # EOF
```

### Comparing `pydbase-1.4.8/tests/test_chain_data.py` & `pydbase-1.5.0/tests/test_chain_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 def teardown_module(module):
     """ teardown any state that was previously setup with a setup_module
     method.
     """
     try:
         # No dangling data
-        #os.remove(fname)
+        os.remove(fname)
         os.remove(iname)
         pass
     except:
         print(sys.exc_info())
         #assert 0
         pass
```

### Comparing `pydbase-1.4.8/tests/test_chain_link.py` & `pydbase-1.5.0/tests/test_chain_link.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 def teardown_module(module):
     """ teardown any state that was previously setup with a setup_module
     method.
     """
 
     try:
         # No dangling data
-        #os.remove(fname)
-        #os.remove(iname)
+        os.remove(fname)
+        os.remove(iname)
         pass
     except:
         print(sys.exc_info())
         #assert 0
         pass
 
     #assert 0
```

### Comparing `pydbase-1.4.8/tests/test_del.py` & `pydbase-1.5.0/tests/test_del.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.4.8/tests/test_dump.py` & `pydbase-1.5.0/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.4.8/tests/test_find.py` & `pydbase-1.5.0/tests/test_getoffs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python3
 
 import pytest, os, sys, random
 from mytest import *
 import twincore, pyvpacker
 
 core = None
+fname = createname(__file__)
+iname = createidxname(__file__)
 
 def setup_module(module):
     """ setup any state specific to the execution of the given module."""
     global core
-    core = create_db()
+    core = create_db(fname)
     assert core != 0
 
     ret = core.save_data("1111", "2222")
     assert ret != 0
     ret = core.save_data("11111", "22222")
     assert ret != 0
     ret = core.save_data("111", "222")
@@ -34,27 +36,28 @@
     #assert 0, "test here, function %s" % function.__name__
     pass
 
 # ------------------------------------------------------------------------
 # Start
 
 def test_get():
+
+    # Get record, verify
     ret = core.get_rec(2)
     assert ret != 0
-    print(ret)
     assert ret == [b'111', b'222']
 
-def test_search():
-
-    #return
+def test_getoffs():
 
-    strx = "1111"
-    ret = core.findrec(strx, 1)
-    #print(ret)
-    assert ret ==[[b'11111', b'22222']]
-
-    strx = "11111"
-    ret = core.findrec(strx, 1)
-    #print(ret)
-    assert ret == [[b'11111', b'22222']]
+    ret = core.findrecpos('1111', 1)
+    assert ret == [32]
+    ddd = core.get_rec_byoffs(ret[0])
+    assert ddd == [b'1111', b'2222']
+
+def test_getoffs2():
+
+    ret = core.findrecpos('11111', 1)
+    assert ret == [64]
+    ddd = core.get_rec_byoffs(ret[0])
+    assert ddd == [b'11111', b'22222']
 
 # EOF
```

### Comparing `pydbase-1.4.8/tests/test_findrec.py` & `pydbase-1.5.0/tests/test_findrec.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 #!/usr/bin/env python3
 
 import pytest, os, sys, random
 from mytest import *
 import twincore, pyvpacker
 
 core = None
+fname = createname(__file__)
+iname = createidxname(__file__)
 
 def setup_module(module):
     """ setup any state specific to the execution of the given module."""
     global core
-    core = create_db()
+
+    core = create_db(fname)
     assert core != 0
 
     ret = core.save_data("1111", "2222")
     assert ret != 0
     ret = core.save_data("11111", "22222")
     assert ret != 0
     ret = core.save_data("111", "222")
@@ -54,9 +57,8 @@
 
     # Not found
     strx = "11111x"
     ret = core.findrec(strx)
     print (ret)
     assert ret == []
 
-
 # EOF
```

### Comparing `pydbase-1.4.8/tests/test_getoffs.py` & `pydbase-1.5.0/tests/test_inplace.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python3
 
 import pytest, os, sys, random
 from mytest import *
 import twincore, pyvpacker
 
 core = None
+fname = createname(__file__)
+iname = createidxname(__file__)
 
 def setup_module(module):
     """ setup any state specific to the execution of the given module."""
     global core
-    core = create_db()
+    core = create_db(fname)
     assert core != 0
 
     ret = core.save_data("1111", "2222")
     assert ret != 0
     ret = core.save_data("11111", "22222")
     assert ret != 0
     ret = core.save_data("111", "222")
@@ -37,25 +39,31 @@
 # ------------------------------------------------------------------------
 # Start
 
 def test_get():
 
     # Get record, verify
     ret = core.get_rec(2)
-    assert ret != 0
     assert ret == [b'111', b'222']
 
 def test_getoffs():
 
-    ret = core.findrecpos('1111', 1)
-    assert ret == [32]
-    ddd = core.get_rec_offs(ret[0])
-    assert ddd == [b'1111', b'2222']
-
-def test_getoffs2():
-
-    ret = core.findrecpos('11111', 1)
-    assert ret == [64]
-    ddd = core.get_rec_offs(ret[0])
-    assert ddd == [b'11111', b'22222']
+    # This is in place
+    ret = core.save_data("11111", "333", True)
+    #print(ret)
+    assert ret == 64
+
+    ret4 = core.get_rec_byoffs(ret)
+    #print(ret4)
+    assert ret4 == [b'11111', b'333  ']
+
+def test_finder():
+
+    ret2 = core.findrec("11111", 1)
+    #print(ret2)
+    assert ret2 == [[b'11111', b'333  ']]
+
+    ret3 = core.get_rec(1)
+    #print(ret3)
+    assert ret3 == [b'11111', b'333  ']
 
 # EOF
```

### Comparing `pydbase-1.4.8/tests/test_getrec.py` & `pydbase-1.5.0/tests/test_getrec.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.4.8/tests/test_handles.py` & `pydbase-1.5.0/tests/test_handles.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,31 @@
 
 import pytest, os, sys
 
 fff = __file__[:]
 from mytest import *
 
 core = None
+dcore = None
+fname = createname(__file__)
+iname = createidxname(__file__)
 
 def _print_handles():
-    open_file_handles = os.listdir('/proc/self/fd')
-    print('open file handles: ' + ', '.join(map(str, open_file_handles)))
+    try:
+        import fcntl
+        open_file_handles = os.listdir('/proc/self/fd')
+        print('open file handles: ' + ', '.join(map(str, open_file_handles)))
+    except:
+        pass
+        # Windows here ...
 
 def setup_module(module):
     """ setup any state specific to the execution of the given module."""
     global core
-    core = create_db()
+    core = create_db(fname)
     assert core != None
 
 def teardown_module(module):
     """ teardown any state that was previously setup with a setup_module
     method.
     """
     uncreate_db()
```

### Comparing `pydbase-1.4.8/tests/test_inplace.py` & `pydbase-1.5.0/tests/test_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 #!/usr/bin/env python3
 
 import pytest, os, sys, random
 from mytest import *
 import twincore, pyvpacker
 
 core = None
+fname = createname(__file__)
+iname = createidxname(__file__)
 
 def setup_module(module):
     """ setup any state specific to the execution of the given module."""
     global core
-    core = create_db()
+    core = create_db(fname)
     assert core != 0
 
     ret = core.save_data("1111", "2222")
     assert ret != 0
     ret = core.save_data("11111", "22222")
     assert ret != 0
+    ret = core.save_data("11111", "333333")
+    assert ret != 0
+    ret = core.save_data("3333", "4444")
+    assert ret != 0
     ret = core.save_data("111", "222")
     assert ret != 0
+    ret = core.save_data("1111", "3333")
+    assert ret != 0
 
 def teardown_module(module):
     """ teardown any state that was previously setup with a setup_module
     method.
     """
     uncreate_db()
 
@@ -34,34 +42,28 @@
     #assert 0, "test here, function %s" % function.__name__
     pass
 
 # ------------------------------------------------------------------------
 # Start
 
 def test_get():
-
-    # Get record, verify
-    ret = core.get_rec(2)
+    ret = core.get_rec(4)
     assert ret == [b'111', b'222']
 
-def test_getoffs():
+def test_list():
 
-    # This is in place
-    ret = core.save_data("11111", "333", True)
-    #print(ret)
-    assert ret == 64
-
-    ret4 = core.get_rec_offs(ret)
-    #print(ret4)
-    assert ret4 == [b'11111', b'333  ']
-
-def test_finder():
-
-    ret2 = core.findrec("11111", 1)
-    #print(ret2)
-    assert ret2 == [[b'11111', b'333  ']]
-
-    ret3 = core.get_rec(1)
-    #print(ret3)
-    assert ret3 == [b'11111', b'333  ']
+    ret = core.del_rec_bykey("3333")
+    #print("delrec", ret)
+    assert ret == 1
+
+    ret = core.listall()
+    #print("listall", ret)
+    assert ret == [5, 4, 2]
+
+    sss = []
+    for aa in ret:
+        ret = core.get_rec(aa)
+        sss.append(ret)
+    #print(sss)
+    assert sss == [[b'1111', b'3333'], [b'111', b'222'], [b'11111', b'333333']]
 
 # EOF
```

### Comparing `pydbase-1.4.8/tests/test_integrity.py` & `pydbase-1.5.0/tests/test_integrity.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 import pytest, os, sys
 from mytest import *
 import twincore, pyvpacker
 
 # Test for pydbase
 
 core = None
+fname = createname(__file__)
+iname = createidxname(__file__)
 
 def setup_module(module):
     """ setup any state specific to the execution of the given module."""
     global core
-    core = create_db()
+    core = create_db(fname)
     assert core != 0
 
     ret = core.save_data("1111", "2222")
     assert ret != 0
     ret = core.save_data("11111", "22222")
     assert ret != 0
     ret = core.save_data("111", "222")
```

### Comparing `pydbase-1.4.8/tests/test_list.py` & `pydbase-1.5.0/tests/test_acreate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,23 @@
 #!/usr/bin/env python3
 
-import pytest, os, sys, random
+import pytest, os, sys
+
+fff = __file__[:]
 from mytest import *
-import twincore, pyvpacker
 
 core = None
+fname = createname(__file__)
+iname = createidxname(__file__)
 
 def setup_module(module):
     """ setup any state specific to the execution of the given module."""
     global core
-    core = create_db()
-    assert core != 0
-
-    ret = core.save_data("1111", "2222")
-    assert ret != 0
-    ret = core.save_data("11111", "22222")
-    assert ret != 0
-    ret = core.save_data("11111", "333333")
-    assert ret != 0
-    ret = core.save_data("3333", "4444")
-    assert ret != 0
-    ret = core.save_data("111", "222")
-    assert ret != 0
-    ret = core.save_data("1111", "3333")
-    assert ret != 0
+    core = create_db(fname)
+    assert core != None
 
 def teardown_module(module):
     """ teardown any state that was previously setup with a setup_module
     method.
     """
     uncreate_db()
 
@@ -39,29 +29,42 @@
     #assert tmp_path == ""
     #assert 0, "test here, function %s" % function.__name__
     pass
 
 # ------------------------------------------------------------------------
 # Start
 
-def test_get():
-    ret = core.get_rec(4)
+def test_awrite(capsys):
+
+    print("write", core)
+    ret = core.save_data("1111", "2222")
+    print(ret)
+    #assert ret != 0
+    ret = core.save_data("11111", "22222")
+    #assert ret != 0
+    ret = core.save_data("111", "222")
+    #assert ret != 0
+
+    #for aa in range(core.getdbsize()):
+    #    print( core.get_rec(aa))
+
+def test_get(capsys):
+
+    ret = core.get_rec(2)
+    assert ret != 0
     assert ret == [b'111', b'222']
 
-def test_list():
+def test_read(capsys):
+
+    #for aa in range(core.getdbsize()):
+    #    print( core.get_rec(aa))
+
+    ret = core.retrieve("111")
+    print(ret)
+    assert ret == [[b'111', b'222']]
+
+    ret = core.retrieve("1111")
+    assert ret == [[b'1111', b'2222']]
 
-    ret = core.del_rec_bykey("3333")
-    #print("delrec", ret)
-    assert ret == 1
-
-    ret = core.listall()
-    #print("listall", ret)
-    assert ret == [5, 4, 2]
-
-    sss = []
-    for aa in ret:
-        ret = core.get_rec(aa)
-        sss.append(ret)
-    #print(sss)
-    assert sss == [[b'1111', b'3333'], [b'111', b'222'], [b'11111', b'333333']]
 
 # EOF
+
```

### Comparing `pydbase-1.4.8/tests/test_packer.py` & `pydbase-1.5.0/tests/test_packer.py`

 * *Files identical despite different names*

### Comparing `pydbase-1.4.8/tests/test_randdata.py` & `pydbase-1.5.0/tests/test_bindata.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 #!/usr/bin/env python3
 
-import pytest, os, sys, random
+import pytest, os, sys
 from mytest import *
 import twincore, pyvpacker
 
 core = None
+fname = createname(__file__)
+iname = createidxname(__file__)
+
+orgdata = []
+
+# ------------------------------------------------------------------------
 
 def setup_module(module):
     """ setup any state specific to the execution of the given module."""
-    global core
-    core = create_db()
+    global core, orgdata
+
+    try:
+        # Fresh start
+        os.remove(fname)
+        os.remove(iname)
+    except:
+        #print("on prepare", sys.exc_info())
+        pass
+
+    core = twincore.TwinCore(fname)
     assert core != 0
 
-    # Create a database of 5000 random records
+    # Create a database of 500 random binary records
     for aa in range(500):
-        key = randstr(random.randint(6, 12))
-        val = randstr(random.randint(24, 96))
-        ret = core.save_data(str(key), str(val))
+        key = randbin(random.randint(6, 12))
+        val = randbin(random.randint(24, 96))
+        ret = core.save_data(key, val)
         assert ret != 0
+        orgdata.append([key, val])
 
 def teardown_module(module):
     """ teardown any state that was previously setup with a setup_module
     method.
     """
-    uncreate_db()
+    try:
+        # No dangling data
+        os.remove(fname)
+        os.remove(iname)
+        pass
+    except:
+        print(sys.exc_info())
+        #assert 0
+        pass
 
-def test_randdata(capsys):
+    #assert 0
+
+def test_bindata(capsys):
 
-    #core.reindex()
-    #core.dump_data(twincore.INT_MAX)
     dbsize = core.getdbsize()
-    #print("dbsize", dbsize)
-    #assert 0
 
     ddd = []
     for aa in range(dbsize):
         vvv = core.get_rec(aa)
         ddd.append(vvv)
 
-    #twincore.core_verbose = 2
-    core.reindex()
-    dbsize2 = core.getdbsize()
-    #twincore.core_verbose = 0
-
-    nnn = []
-    try:
-        for aa in range(dbsize2):
-            vvv = core.get_rec(aa)
-            nnn.append(vvv)
-    except:
-        pass
-
-    try:
-        # No dangling data
-        #os.remove("data/test_randdata.pydb")
-        #os.remove("data/test_randdata.pidx")
-        pass
-    except:
-        #print(sys.exc_info())
-        pass
+    # print(orgdata);  print(ddd)
 
-    assert dbsize == dbsize2
-    assert nnn == ddd
+    assert orgdata == ddd
 
 # EOF
```

### Comparing `pydbase-1.4.8/tests/test_reindex.py` & `pydbase-1.5.0/tests/test_reindex.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 # Test for pydbase integrity test
 
 core = None
 
 fname = createname(__file__)
 iname = createidxname(__file__)
 
+orgdata = []
+
 def setup_module(module):
     """ setup any state specific to the execution of the given module."""
 
     global core
 
     try:
         # Fresh start
@@ -24,70 +26,58 @@
     except:
         #print(sys.exc_info())
         pass
 
     core = create_db(fname)
     assert core != 0
 
-    kkk = 100; vvv = 1000; xxx = 10
+    kkk = 1000000; vvv = 1000
     # Create a database of xxx records
-    for aa in range(xxx):
+    for aa in range(500):
         ret = core.save_data(str(kkk), str(vvv))
+        orgdata.append([str(kkk).encode(), str(vvv).encode()])
         assert ret != 0
         kkk += 1; vvv += 1
-
     #assert 0
 
 def teardown_module(module):
     """ teardown any state that was previously setup with a setup_module
     method.
     """
     try:
         # Fresh start
         os.remove(fname)
         os.remove(iname)
     except:
         #print(sys.exc_info())
         pass
 
-
 def test_reindex(capsys):
 
-    #core.reindex()
-    #core.dump_data()
     dbsize = core.getdbsize()
     #print("dbsize", dbsize)
     #assert 0
 
     ddd = []
     for aa in range(dbsize):
         vvv = core.get_rec(aa)
         ddd.append(vvv)
 
-    #twincore.core_verbose = 2
+    #print(ddd); print(); print(orgdata)
+    assert ddd == orgdata
+
     core.reindex()
     dbsize2 = core.getdbsize()
-    #twincore.core_verbose = 0
 
     assert dbsize == dbsize2
 
     nnn = []
     try:
         for aa in range(dbsize2):
             vvv = core.get_rec(aa)
             nnn.append(vvv)
     except:
         pass
 
-    try:
-        # No dangling data
-        #os.remove("data/test_reindex.pydb")
-        #os.remove("data/test_reindex.pidx")
-        pass
-    except:
-        #print(sys.exc_info())
-        pass
-
-    assert dbsize == dbsize2
     assert nnn == ddd
 
 # EOF
```

### Comparing `pydbase-1.4.8/tests/test_search.py` & `pydbase-1.5.0/tests/test_search.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python3
 
 import pytest, os, sys, random
 from mytest import *
 import twincore, pyvpacker
 
 core = None
+fname = createname(__file__)
+iname = createidxname(__file__)
 
 def setup_module(module):
     """ setup any state specific to the execution of the given module."""
     global core
-    core = create_db()
+    core = create_db(fname)
     assert core != 0
 
     ret = core.save_data("1111", "2222")
     assert ret != 0
     ret = core.save_data("11111", "22222")
     assert ret != 0
     ret = core.save_data("11111", "22222")
@@ -44,21 +46,21 @@
     assert ret == [b'111', b'222']
 
 def test_search():
 
     strx = "1111"
     ret = core.find_key(strx)
     assert ret == [32]
-    arr = core.get_rec_offs(ret[0])
+    arr = core.get_rec_byoffs(ret[0])
     assert arr == [b"1111", b"2222"]
 
 def test_search2():
 
     strx = "11111"
     ret = core.find_key(strx)
     assert ret == [98, 64]
-    arr = core.get_rec_offs(ret[0])
+    arr = core.get_rec_byoffs(ret[0])
     assert arr == [b"11111", b"22222"]
-    arr = core.get_rec_offs(ret[1])
+    arr = core.get_rec_byoffs(ret[1])
     assert arr == [b"11111", b"22222"]
 
 # EOF
```

