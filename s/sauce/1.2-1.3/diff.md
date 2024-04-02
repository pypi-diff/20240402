# Comparing `tmp/sauce-1.2.tar.gz` & `tmp/sauce-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sauce-1.2.tar", last modified: Mon Jun  6 13:19:18 2016, max compression
+gzip compressed data, was "sauce-1.3.tar", last modified: Tue Apr  2 14:17:41 2024, max compression
```

## Comparing `sauce-1.2.tar` & `sauce-1.3.tar`

### file list

```diff
@@ -1,6 +1,12 @@
-drwxr-xr-x   0 wijnand    (501) staff       (20)        0 2016-06-06 13:19:18.000000 sauce-1.2/
--rw-r--r--   0 wijnand    (501) staff       (20)      240 2016-06-06 13:19:18.000000 sauce-1.2/PKG-INFO
--rw-r--r--   0 wijnand    (501) staff       (20)     1915 2016-06-06 13:18:18.000000 sauce-1.2/README.txt
-drwxr-xr-x   0 wijnand    (501) staff       (20)        0 2016-06-06 13:19:18.000000 sauce-1.2/sauce/
--rw-r--r--   0 wijnand    (501) staff       (20)    15415 2016-06-06 13:18:40.000000 sauce-1.2/sauce/__init__.py
--rw-r--r--   0 wijnand    (501) staff       (20)      286 2016-06-06 13:18:26.000000 sauce-1.2/setup.py
+drwxr-xr-x   0 jq         (501) staff       (20)        0 2024-04-02 14:17:41.250922 sauce-1.3/
+-rw-r--r--   0 jq         (501) staff       (20)      184 2024-04-02 14:17:41.250741 sauce-1.3/PKG-INFO
+-rw-r--r--   0 jq         (501) staff       (20)     2801 2024-04-02 14:15:55.000000 sauce-1.3/README.rst
+drwxr-xr-x   0 jq         (501) staff       (20)        0 2024-04-02 14:17:41.250036 sauce-1.3/sauce/
+-rw-r--r--   0 jq         (501) staff       (20)    15396 2024-04-02 13:56:03.000000 sauce-1.3/sauce/__init__.py
+drwxr-xr-x   0 jq         (501) staff       (20)        0 2024-04-02 14:17:41.250555 sauce-1.3/sauce.egg-info/
+-rw-r--r--   0 jq         (501) staff       (20)      184 2024-04-02 14:17:41.000000 sauce-1.3/sauce.egg-info/PKG-INFO
+-rw-r--r--   0 jq         (501) staff       (20)      153 2024-04-02 14:17:41.000000 sauce-1.3/sauce.egg-info/SOURCES.txt
+-rw-r--r--   0 jq         (501) staff       (20)        1 2024-04-02 14:17:41.000000 sauce-1.3/sauce.egg-info/dependency_links.txt
+-rw-r--r--   0 jq         (501) staff       (20)        6 2024-04-02 14:17:41.000000 sauce-1.3/sauce.egg-info/top_level.txt
+-rw-r--r--   0 jq         (501) staff       (20)       38 2024-04-02 14:17:41.250961 sauce-1.3/setup.cfg
+-rw-r--r--   0 jq         (501) staff       (20)      286 2024-04-02 13:56:39.000000 sauce-1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sauce-1.2/sauce/__init__.py` & `sauce-1.3/sauce/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,25 +13,22 @@
 '''
 Parser for SAUCE or Standard Architecture for Universal Comment Extensions.
 '''
 
 __author__    = 'Wijnand Modderman-Lenstra <maze@pyth0n.org>'
 __copyright__ = '(C) 2006-2012 Wijnand Modderman-Lenstra'
 __license__   = 'LGPL'
-__version__   = '1.2'
+__version__   = '1.3'
 __url__       = 'https://github.com/tehmaze/sauce'
 
 import datetime
 import os
 import struct
-try:
-    from cStringIO import StringIO
-except ImportError:
-    from StringIO import StringIO
-
+from io import StringIO
+from io import IOBase
 
 class SAUCE(object):
     '''
     Parser for SAUCE or Standard Architecture for Universal Comment Extensions,
     as defined in http://www.acid.org/info/sauce/s_spec.htm.
 
     :param filename:    file name or file handle
@@ -133,15 +130,15 @@
         },
     }
 
     def __init__(self, filename='', data=''):
         assert (filename or data), 'Need either filename or record'
 
         if filename:
-            if type(filename) == file:
+            if isinstance(filename, IOBase):
                 self.filehand = filename
             else:
                 self.filehand = open(filename, 'rb')
             self._size = os.path.getsize(self.filehand.name)
         else:
             self._size = len(data)
             self.filehand = StringIO(data)
@@ -156,39 +153,39 @@
         # record.
         self.filehand.seek(0)
         # Check if we have SAUCE data
         if self.record:
             reads, rest = divmod(self._size - 128, 1024)
         else:
             reads, rest = divmod(self._size, 1024)
-        for x in xrange(0, reads):
+        for x in range(0, reads):
             yield self.filehand.read(1024)
         if rest:
             yield self.filehand.read(rest)
 
     def _read(self):
         if self._size >= 128:
             self.filehand.seek(self._size - 128)
             record = self.filehand.read(128)
-            if record.startswith('SAUCE'):
+            if record.startswith(b'SAUCE'):
                 self.filehand.seek(0)
                 return record, self.filehand.read(self._size - 128)
 
         self.filehand.seek(0)
         return None, self.filehand.read()
 
     def _gets(self, key):
         if self.record is None:
             return None
 
         name, default, offset, size, stype = self._template(key)
         data = self.record[offset:offset + size]
         data = struct.unpack(stype, data)
         if stype[-1] in 'cs':
-            return ''.join(data)
+            return b''.join(data)
         elif stype[-1] in 'BI' and len(stype) == 1:
             return data[0]
         else:
             return data
 
     def _puts(self, key, data):
         name, default, offset, size, stype = self._template(key)
@@ -201,15 +198,15 @@
             self.record[offset + size:]
         ])
         return self.record
 
     def _template(self, key):
         index = self.templates.index(key)
         name, default, size, stype = self.template[index]
-        offset = sum([self.template[x][2] for x in xrange(0, index)])
+        offset = sum([self.template[x][2] for x in range(0, index)])
         return name, default, offset, size, stype
 
     def sauce(self):
         '''
         Get the raw SAUCE record.
         '''
         if self.record:
@@ -295,15 +292,15 @@
         return self._gets('Filler')
 
     def get_filler_str(self):
         filler = self._gets('Filler')
         if filler is None:
             return ''
         else:
-            return filler.rstrip('\x00')
+            return filler.rstrip(b'\x00')
 
     def get_filetype(self):
         return self._gets('FileType')
 
     def get_filetype_str(self):
         datatype = self.datatype_str
         filetype = self.filetype
@@ -445,35 +442,35 @@
     title        = property(get_title,    set_title)
     version      = property(get_version)
 
 
 if __name__ == '__main__':
     import sys
     if len(sys.argv) != 2:
-        print >>sys.stderr, '%s <file>' % (sys.argv[0],)
+        print('{} <file>'.format(sys.argv[0]), file=sys.stderr)
         sys.exit(1)
     else:
         test = SAUCE(sys.argv[1])
 
         def show(sauce):
-            print 'Version.:', sauce.version
-            print 'Title...:', sauce.title
-            print 'Author..:', sauce.author
-            print 'Group...:', sauce.group
-            print 'Date....:', sauce.date
-            print 'FileSize:', sauce.filesize
-            print 'DataType:', sauce.datatype, sauce.datatype_str
-            print 'FileType:', sauce.filetype, sauce.filetype_str
-            print 'TInfo1..:', sauce.tinfo1
-            print 'TInfo2..:', sauce.tinfo2
-            print 'TInfo3..:', sauce.tinfo3
-            print 'TInfo4..:', sauce.tinfo4
-            print 'Flags...:', sauce.flags, sauce.flags_str
-            print 'Record..:', len(sauce.record), repr(sauce.record)
-            print 'Filler..:', sauce.filler_str
+            print('Version.:', sauce.version)
+            print('Title...:', sauce.title)
+            print('Author..:', sauce.author)
+            print('Group...:', sauce.group)
+            print('Date....:', sauce.date)
+            print('FileSize:', sauce.filesize)
+            print('DataType:', sauce.datatype, sauce.datatype_str)
+            print('FileType:', sauce.filetype, sauce.filetype_str)
+            print('TInfo1..:', sauce.tinfo1)
+            print('TInfo2..:', sauce.tinfo2)
+            print('TInfo3..:', sauce.tinfo3)
+            print('TInfo4..:', sauce.tinfo4)
+            print('Flags...:', sauce.flags, sauce.flags_str)
+            print('Record..:', len(sauce.record), repr(sauce.record))
+            print('Filler..:', sauce.filler_str)
 
         if test.record:
             show(test)
         else:
-            print 'No SAUCE record found'
+            print('No SAUCE record found')
             test = SAUCE(data=test.sauce())
             show(test)
```

