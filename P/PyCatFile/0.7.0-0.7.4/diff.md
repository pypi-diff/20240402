# Comparing `tmp/PyCatFile-0.7.0.tar.gz` & `tmp/PyCatFile-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCatFile-0.7.0.tar", last modified: Fri Mar 29 19:11:34 2024, max compression
+gzip compressed data, was "PyCatFile-0.7.4.tar", last modified: Mon Apr  1 23:44:26 2024, max compression
```

## Comparing `PyCatFile-0.7.0.tar` & `PyCatFile-0.7.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:11:34.173971 PyCatFile-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-29 19:11:24.000000 PyCatFile-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-29 19:11:34.173971 PyCatFile-0.7.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:11:34.173971 PyCatFile-0.7.0/PyCatFile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-29 19:11:34.000000 PyCatFile-0.7.0/PyCatFile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-29 19:11:34.000000 PyCatFile-0.7.0/PyCatFile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 19:11:34.000000 PyCatFile-0.7.0/PyCatFile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-29 19:11:34.000000 PyCatFile-0.7.0/PyCatFile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 19:11:34.000000 PyCatFile-0.7.0/PyCatFile.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-29 19:11:24.000000 PyCatFile-0.7.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     6993 2024-03-29 19:11:24.000000 PyCatFile-0.7.0/catfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-03-29 19:11:24.000000 PyCatFile-0.7.0/neocatfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   320185 2024-03-29 19:11:24.000000 PyCatFile-0.7.0/pycatfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-29 19:11:34.173971 PyCatFile-0.7.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     5451 2024-03-29 19:11:24.000000 PyCatFile-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:44:26.191751 PyCatFile-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-01 23:44:17.000000 PyCatFile-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-01 23:44:26.191751 PyCatFile-0.7.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:44:26.191751 PyCatFile-0.7.4/PyCatFile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-01 23:44:26.000000 PyCatFile-0.7.4/PyCatFile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-01 23:44:26.000000 PyCatFile-0.7.4/PyCatFile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 23:44:26.000000 PyCatFile-0.7.4/PyCatFile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 23:44:26.000000 PyCatFile-0.7.4/PyCatFile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 23:44:26.000000 PyCatFile-0.7.4/PyCatFile.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-01 23:44:17.000000 PyCatFile-0.7.4/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6992 2024-04-01 23:44:17.000000 PyCatFile-0.7.4/catfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-01 23:44:17.000000 PyCatFile-0.7.4/neocatfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   329914 2024-04-01 23:44:17.000000 PyCatFile-0.7.4/pycatfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-01 23:44:26.191751 PyCatFile-0.7.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5450 2024-04-01 23:44:17.000000 PyCatFile-0.7.4/setup.py
```

### Comparing `PyCatFile-0.7.0/LICENSE` & `PyCatFile-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCatFile-0.7.0/PKG-INFO` & `PyCatFile-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCatFile
-Version: 0.7.0
+Version: 0.7.4
 Summary: A tar like file format name catfile after unix cat command (concatenate files) .
 Home-page: https://github.com/GameMaker2k/PyCatFile
 Download-URL: https://github.com/GameMaker2k/PyCatFile/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `PyCatFile-0.7.0/PyCatFile.egg-info/PKG-INFO` & `PyCatFile-0.7.4/PyCatFile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCatFile
-Version: 0.7.0
+Version: 0.7.4
 Summary: A tar like file format name catfile after unix cat command (concatenate files) .
 Home-page: https://github.com/GameMaker2k/PyCatFile
 Download-URL: https://github.com/GameMaker2k/PyCatFile/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `PyCatFile-0.7.0/catfile.py` & `PyCatFile-0.7.4/catfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: catfile.py - Last Update: 3/29/2024 Ver. 0.7.0 RC 1 - Author: cooldude2k $
+    $FileInfo: catfile.py - Last Update: 4/1/2024 Ver. 0.7.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import argparse, pycatfile, binascii;
 
 rarfile_support = pycatfile.rarfile_support;
```

### Comparing `PyCatFile-0.7.0/neocatfile.py` & `PyCatFile-0.7.4/neocatfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: neocatfile.py - Last Update: 3/29/2024 Ver. 0.7.0 RC 1 - Author: cooldude2k $
+    $FileInfo: neocatfile.py - Last Update: 4/1/2024 Ver. 0.7.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 import argparse
 import pycatfile
 
 # Compatibility layer for Python 2 and 3 input
```

### Comparing `PyCatFile-0.7.0/pycatfile.py` & `PyCatFile-0.7.4/pycatfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: pycatfile.py - Last Update: 3/29/2024 Ver. 0.7.0 RC 1 - Author: cooldude2k $
+    $FileInfo: pycatfile.py - Last Update: 4/1/2024 Ver. 0.7.4 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import io, os, re, sys, time, stat, zlib, base64, shutil, socket, hashlib, datetime, logging, binascii, tempfile, zipfile, platform;
 from ftplib import FTP, FTP_TLS;
 if(sys.version[0]=="2"):
  from urlparse import urlparse, urlunparse;
@@ -158,19 +158,19 @@
 __file_format_hex__ = binascii.hexlify(__file_format_magic__.encode("UTF-8")).decode("UTF-8");
 __file_format_delimiter__ = "\x00";
 __file_format_ver__ = "001";
 __use_new_style__ = True;
 __file_format_list__ = [__file_format_name__, __file_format_magic__, __file_format_lower__, __file_format_len__, __file_format_hex__, __file_format_delimiter__, __file_format_ver__, __use_new_style__];
 __project__ = __program_name__;
 __project_url__ = "https://github.com/GameMaker2k/PyCatFile";
-__version_info__ = (0, 7, 0, "RC 1", 1);
-__version_date_info__ = (2024, 3, 27, "RC 1", 1);
+__version_info__ = (0, 7, 4, "RC 1", 1);
+__version_date_info__ = (2024, 4, 1, "RC 1", 1);
 __version_date__ = str(__version_date_info__[0]) + "." + str(__version_date_info__[1]).zfill(2) + "." + str(__version_date_info__[2]).zfill(2);
 __revision__ = __version_info__[3];
-__revision_id__ = "$Id: c6be791f0f01d1c31106c1f6f8fb2e9411866361 $";
+__revision_id__ = "$Id: 330c6ce992c910537524a1f38d1f5cfc7f1b5bbd $";
 if(__version_info__[4] is not None):
  __version_date_plusrc__ = __version_date__ + "-" + str(__version_date_info__[4]);
 if(__version_info__[4] is None):
  __version_date_plusrc__ = __version_date__;
 if(__version_info__[3] is not None):
  __version__ = str(__version_info__[0]) + "." + str(__version_info__[1]) + "." + str(__version_info__[2]) + " " + str(__version_info__[3]);
 if(__version_info__[3] is None):
@@ -193,17 +193,17 @@
 geturls_ua_googlebot_google = "Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)";
 geturls_ua_googlebot_google_old = "Googlebot/2.1 (+http://www.google.com/bot.html)";
 geturls_headers_pycatfile_python = {'Referer': "http://google.com/", 'User-Agent': geturls_ua_pycatfile_python, 'Accept-Encoding': "none", 'Accept-Language': "en-US,en;q=0.8,en-CA,en-GB;q=0.6", 'Accept-Charset': "ISO-8859-1,ISO-8859-15,utf-8;q=0.7,*;q=0.7", 'Accept': "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8", 'Connection': "close", 'SEC-CH-UA': "\""+__project__+"\";v=\""+str(__version__)+"\", \"Not;A=Brand\";v=\"8\", \""+py_implementation+"\";v=\""+str(platform.release())+"\"", 'SEC-CH-UA-FULL-VERSION': str(__version__), 'SEC-CH-UA-PLATFORM': ""+py_implementation+"", 'SEC-CH-UA-ARCH': ""+platform.machine()+"", 'SEC-CH-UA-PLATFORM': str(__version__), 'SEC-CH-UA-BITNESS': str(PyBitness)};
 geturls_headers_pycatfile_python_alt = {'Referer': "http://google.com/", 'User-Agent': geturls_ua_pycatfile_python_alt, 'Accept-Encoding': "none", 'Accept-Language': "en-US,en;q=0.8,en-CA,en-GB;q=0.6", 'Accept-Charset': "ISO-8859-1,ISO-8859-15,utf-8;q=0.7,*;q=0.7", 'Accept': "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8", 'Connection': "close", 'SEC-CH-UA': "\""+__project__+"\";v=\""+str(__version__)+"\", \"Not;A=Brand\";v=\"8\", \""+py_implementation+"\";v=\""+str(platform.release())+"\"", 'SEC-CH-UA-FULL-VERSION': str(__version__), 'SEC-CH-UA-PLATFORM': ""+py_implementation+"", 'SEC-CH-UA-ARCH': ""+platform.machine()+"", 'SEC-CH-UA-PLATFORM': str(__version__), 'SEC-CH-UA-BITNESS': str(PyBitness)};
 geturls_headers_googlebot_google = {'Referer': "http://google.com/", 'User-Agent': geturls_ua_googlebot_google, 'Accept-Encoding': "none", 'Accept-Language': "en-US,en;q=0.8,en-CA,en-GB;q=0.6", 'Accept-Charset': "ISO-8859-1,ISO-8859-15,utf-8;q=0.7,*;q=0.7", 'Accept': "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8", 'Connection': "close"};
 geturls_headers_googlebot_google_old = {'Referer': "http://google.com/", 'User-Agent': geturls_ua_googlebot_google_old, 'Accept-Encoding': "none", 'Accept-Language': "en-US,en;q=0.8,en-CA,en-GB;q=0.6", 'Accept-Charset': "ISO-8859-1,ISO-8859-15,utf-8;q=0.7,*;q=0.7", 'Accept': "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8", 'Connection': "close"};
 
-compressionlist = ['auto', 'gzip', 'bzip2', 'zstd', 'xz', 'lz4', 'lzo', 'lzma'];
-outextlist = ['gz', 'bz2', 'zst', 'xz', 'lz4', 'lzo', 'lzma'];
-outextlistwd = ['.gz', '.bz2', '.zst', '.xz', '.lz4', '.lzo', '.lzma'];
+compressionlist = ['auto', 'gzip', 'bzip2', 'zstd', 'lz4', 'lzo', 'lzop', 'lzma', 'xz'];
+outextlist = ['gz', 'bz2', 'zst', 'lz4', 'lzo', 'lzop', 'lzma', 'xz'];
+outextlistwd = ['.gz', '.bz2', '.zst', '.lz4', '.lzo', '.lzop', '.lzma', '.xz'];
 
 tarfile_mimetype = "application/tar";
 tarfile_tar_mimetype = tarfile_mimetype;
 zipfile_mimetype = "application/zip";
 zipfile_zip_mimetype = zipfile_mimetype;
 rarfile_mimetype = "application/rar";
 rarfile_rar_mimetype = rarfile_mimetype;
@@ -687,15 +687,86 @@
   pyhascontents = False;
  newfccs = GetFileChecksum(fcontents, HeaderOut[-3].lower(), False, formatspecs);
  if(fccs!=newfccs and not skipchecksum and not listonly):
   VerbosePrintOut("File Content Checksum Error with file " + fname + " at offset " + str(fcontentstart));
   return False;
  fp.seek(1, 1);
  fcontentend = fp.tell() - 1;
- catlist = {'fheadersize': fheadsize, 'fhstart': fheaderstart, 'fhend': fhend, 'ftype': ftype, 'fname': fname, 'fbasedir': fbasedir, 'flinkname': flinkname, 'fsize': fsize, 'fatime': fatime, 'fmtime': fmtime, 'fctime': fctime, 'fbtime': fbtime, 'fmode': fmode, 'fchmode': fchmode, 'ftypemod': ftypemod, 'fwinattributes': fwinattributes, 'fuid': fuid, 'funame': funame, 'fgid': fgid, 'fgname': fgname, 'finode': finode, 'flinkcount': flinkcount, 'fminor': fdev_minor, 'fmajor': fdev_major, 'frminor': frdev_minor, 'frmajor': frdev_major, 'fchecksumtype': fchecksumtype, 'fnumfields': fnumfields + 2, 'frawheader': HeaderOut, 'fextrafields': fextrafields, 'fextrafieldsize': fextrasize, 'fextralist': extrafieldslist, 'fheaderchecksum': fcs, 'fcontentchecksum': fccs, 'fhascontents': pyhascontents, 'fcontentstart': fcontentstart, 'fcontentend': fcontentend, 'fcontents': fcontents}
+ catlist = {'fheadersize': fheadsize, 'fhstart': fheaderstart, 'fhend': fhend, 'ftype': ftype, 'fname': fname, 'fbasedir': fbasedir, 'flinkname': flinkname, 'fsize': fsize, 'fatime': fatime, 'fmtime': fmtime, 'fctime': fctime, 'fbtime': fbtime, 'fmode': fmode, 'fchmode': fchmode, 'ftypemod': ftypemod, 'fwinattributes': fwinattributes, 'fuid': fuid, 'funame': funame, 'fgid': fgid, 'fgname': fgname, 'finode': finode, 'flinkcount': flinkcount, 'fminor': fdev_minor, 'fmajor': fdev_major, 'frminor': frdev_minor, 'frmajor': frdev_major, 'fchecksumtype': fchecksumtype, 'fnumfields': fnumfields + 2, 'frawheader': HeaderOut, 'fextrafields': fextrafields, 'fextrafieldsize': fextrasize, 'fextralist': extrafieldslist, 'fheaderchecksum': fcs, 'fcontentchecksum': fccs, 'fhascontents': pyhascontents, 'fcontentstart': fcontentstart, 'fcontentend': fcontentend, 'fcontents': fcontents};
+ return catlist;
+
+def ReadFileHeaderDataBySizeWithContentToList(fp, listonly=False, skipchecksum=False, formatspecs=__file_format_list__):
+ delimiter = formatspecs[5];
+ fheaderstart = fp.tell();
+ if(formatspecs[7]):
+  HeaderOut = ReadFileHeaderDataBySize(fp, delimiter);
+ else:
+  HeaderOut = ReadFileHeaderDataWoSize(fp, delimiter);
+ fheadsize = int(HeaderOut[0], 16);
+ fnumfields = int(HeaderOut[1], 16);
+ ftype = int(HeaderOut[2], 16);
+ if(re.findall("^[.|/]", HeaderOut[3])):
+  fname = HeaderOut[3];
+ else:
+  fname = "./"+HeaderOut[3];
+ fbasedir = os.path.dirname(fname);
+ flinkname = HeaderOut[4];
+ fsize = int(HeaderOut[5], 16);
+ fatime = int(HeaderOut[6], 16);
+ fmtime = int(HeaderOut[7], 16);
+ fctime = int(HeaderOut[8], 16);
+ fbtime = int(HeaderOut[9], 16);
+ fmode = int(HeaderOut[10], 16);
+ fchmode = stat.S_IMODE(fmode);
+ ftypemod = stat.S_IFMT(fmode);
+ fwinattributes = int(HeaderOut[11], 16);
+ fuid = int(HeaderOut[12], 16);
+ funame = HeaderOut[13];
+ fgid = int(HeaderOut[14], 16);
+ fgname = HeaderOut[15];
+ fid = int(HeaderOut[16], 16);
+ finode = int(HeaderOut[17], 16);
+ flinkcount = int(HeaderOut[18], 16);
+ fdev_minor = int(HeaderOut[19], 16);
+ fdev_major = int(HeaderOut[20], 16);
+ frdev_minor = int(HeaderOut[21], 16);
+ frdev_major = int(HeaderOut[22], 16);
+ fextrasize = int(HeaderOut[23], 16);
+ fextrafields = int(HeaderOut[24], 16);
+ extrafieldslist = [];
+ extrastart = 25;
+ extraend = extrastart + fextrafields;
+ extrafieldslist = [];
+ if(extrastart<extraend):
+  extrafieldslist.append(HeaderOut[extrastart]);
+  extrastart = extrastart + 1;
+ fchecksumtype = HeaderOut[extrastart].lower();
+ fcs = HeaderOut[extrastart + 1].lower();
+ fccs = HeaderOut[extrastart + 2].lower();
+ newfcs = GetHeaderChecksum(HeaderOut[:-2], HeaderOut[-3].lower(), True, formatspecs);
+ if(fcs!=newfcs and not skipchecksum):
+  VerbosePrintOut("File Header Checksum Error with file " + fname + " at offset " + str(fheaderstart));
+  return False;
+ fhend = fp.tell() - 1;
+ fcontentstart = fp.tell();
+ fcontents = "".encode('UTF-8');
+ pyhascontents = False;
+ if(fsize>0 and not listonly):
+  fcontents = fp.read(fsize);
+  pyhascontents = True;
+ elif(fsize>0 and listonly):
+  fp.seek(fsize, 1);
+  pyhascontents = False;
+ newfccs = GetFileChecksum(fcontents, HeaderOut[-3].lower(), False, formatspecs);
+ if(fccs!=newfccs and not skipchecksum and not listonly):
+  VerbosePrintOut("File Content Checksum Error with file " + fname + " at offset " + str(fcontentstart));
+  return False;
+ fp.seek(1, 1);
+ fcontentend = fp.tell() - 1;
+ catlist = [ftype, fname, flinkname, fsize, fatime, fmtime, fctime, fbtime, fmode, fwinattributes, fuid, funame, fgid, fgname, fid, finode, flinkcount, fdev_minor, fdev_major, frdev_minor, frdev_major, extrafieldslist, fchecksumtype, fcontents];
  return catlist;
 
 def ReadFileDataBySizeWithContent(fp, listonly=False, skipchecksum=False, formatspecs=__file_format_list__):
  delimiter = formatspecs[5];
  catheader = ReadFileHeaderData(fp, 4, delimiter);
  headercheck = ValidateHeaderChecksum(catheader[:-1], catheader[2], catheader[3], formatspecs);
  if(not headercheck and not skipchecksum):
@@ -818,15 +889,71 @@
    catarray['filetypes']['symlinks']['filetoid'].update(filetoidarray);
    catarray['filetypes']['symlinks']['idtofile'].update(idtofilearray);
    catarray['filetypes']['devices']['filetoid'].update(filetoidarray);
    catarray['filetypes']['devices']['idtofile'].update(idtofilearray);
   lcfi = lcfi + 1;
  return catarray;
 
-def ReadInFileBySizeWithContent(infile, seekstart=0, seekend=0, listonly=False, skipchecksum=False, formatspecs=__file_format_list__):
+def ReadFileDataBySizeWithContentToList(fp, seekstart=0, seekend=0, listonly=False, skipchecksum=False, formatspecs=__file_format_list__):
+ delimiter = formatspecs[5];
+ catheader = ReadFileHeaderData(fp, 4, delimiter);
+ headercheck = ValidateHeaderChecksum(catheader[:-1], catheader[2], catheader[3], formatspecs);
+ if(not headercheck and not skipchecksum):
+  VerbosePrintOut("File Header Checksum Error with file at offset " + str(0));
+  return False;
+ catstring = catheader[0];
+ catversion = re.findall(r"([\d]+)$", catstring);
+ catversions = re.search(r'(.*?)(\d+)$', catstring).groups();
+ fprenumfiles = catheader[1];
+ fnumfiles = int(fprenumfiles, 16);
+ fprechecksumtype = catheader[2];
+ fprechecksum = catheader[3];
+ catlist = [];
+ if(seekstart<0 and seekstart>fnumfiles):
+   seekstart = 0;
+ if(seekend==0 or seekend>fnumfiles and seekend<seekstart):
+  seekend = fnumfiles;
+ elif(seekend<0 and abs(seekend)<=fnumfiles and abs(seekend)>=seekstart):
+  seekend = fnumfiles - abs(seekend);
+ if(seekstart>0):
+  il = 0;
+  while(il < seekstart):
+   prefhstart = fp.tell();
+   preheaderdata = ReadFileHeaderDataBySize(fp, formatspecs[5]);
+   prefsize = int(preheaderdata[5], 16);
+   prenewfcs = GetHeaderChecksum(preheaderdata[:-2], preheaderdata[-3].lower(), True, formatspecs);
+   prefcs = preheaderdata[-2];
+   if(prefcs!=prenewfcs and not skipchecksum):
+    VerbosePrintOut("File Header Checksum Error with file " + prefname + " at offset " + str(prefhstart));
+    return False;
+    valid_archive = False;
+    invalid_archive = True;
+   prefhend = fp.tell() - 1;
+   prefcontentstart = fp.tell();
+   prefcontents = "";
+   pyhascontents = False;
+   if(prefsize>0):
+    prefcontents = fp.read(prefsize);
+    prenewfccs = GetFileChecksum(prefcontents, preheaderdata[-3].lower(), False, formatspecs);
+    prefccs = preheaderdata[-1];
+    pyhascontents = True;
+    if(prefccs!=prenewfccs and not skipchecksum):
+     VerbosePrintOut("File Content Checksum Error with file " + prefname + " at offset " + str(prefcontentstart));
+     return False;
+   fp.seek(1, 1);
+   il = il + 1;
+ realidnum = 0;
+ countnum = seekstart;
+ while(countnum < seekend):
+  catlist.append(ReadFileHeaderDataBySizeWithContentToList(fp, listonly, skipchecksum, formatspecs));
+  countnum = countnum + 1;
+  realidnum = realidnum + 1;
+ return catlist;
+
+def ReadInFileBySizeWithContentToArray(infile, listonly=False, skipchecksum=False, formatspecs=__file_format_list__):
  delimiter = formatspecs[5];
  if(hasattr(infile, "read") or hasattr(infile, "write")):
   fp = infile;
   fp.seek(0, 0);
   fp = UncompressArchiveFile(fp, formatspecs);
   checkcompressfile = CheckCompressionSubType(fp, formatspecs);
   if(checkcompressfile!="catfile" and checkcompressfile!=formatspecs[2]):
@@ -873,17 +1000,17 @@
    elif(fextname==".lzma" or fextname==".xz"):
     compresscheck = "lzma";
    else:
     return False;
   if(not compresscheck):
    return False;
   fp = UncompressFile(infile, formatspecs, "rb");
- return ReadFileDataBySizeWithContentToArray(fp, seekstart, seekend, listonly, skipchecksum, formatspecs);
+ return ReadFileDataBySizeWithContentToArray(fp, listonly, skipchecksum, formatspecs);
 
-def ReadInFileBySizeWithContentToArray(infile, listonly=False, skipchecksum=False, formatspecs=__file_format_list__):
+def ReadInFileBySizeWithContentToList(infile, seekstart=0, seekend=0, listonly=False, skipchecksum=False, formatspecs=__file_format_list__):
  delimiter = formatspecs[5];
  if(hasattr(infile, "read") or hasattr(infile, "write")):
   fp = infile;
   fp.seek(0, 0);
   fp = UncompressArchiveFile(fp, formatspecs);
   checkcompressfile = CheckCompressionSubType(fp, formatspecs);
   if(checkcompressfile!="catfile" and checkcompressfile!=formatspecs[2]):
@@ -930,15 +1057,15 @@
    elif(fextname==".lzma" or fextname==".xz"):
     compresscheck = "lzma";
    else:
     return False;
   if(not compresscheck):
    return False;
   fp = UncompressFile(infile, formatspecs, "rb");
- return ReadFileDataBySizeWithContentToArray(fp, listonly, skipchecksum, formatspecs);
+ return ReadFileDataBySizeWithContentToList(fp, seekstart, seekend, listonly, skipchecksum, formatspecs);
 
 def ReadInFileBySizeWithContentToArrayIndex(infile, seekstart=0, seekend=0, listonly=False, skipchecksum=False, formatspecs=__file_format_list__):
  if(isinstance(infile, dict)):
   listcatfiles = infile;
  else:
   if(infile!="-" and not hasattr(infile, "read") and not hasattr(infile, "write")):
    infile = RemoveWindowsPath(infile);
@@ -1057,24 +1184,26 @@
   os.fsync(fp.fileno());
  except io.UnsupportedOperation:
   pass;
  except AttributeError:
   pass;
  return fp;
 
-def AppendFilesWithContent(infiles, fp, dirlistfromtxt=False, filevalues=[], extradata=[], followlink=False, checksumtype="crc32", formatspecs=__file_format_list__):
+def AppendFilesWithContent(infiles, fp, dirlistfromtxt=False, filevalues=[], extradata=[], followlink=False, checksumtype="crc32", formatspecs=__file_format_list__, verbose=False):
  advancedlist = True;
+ if(verbose):
+  logging.basicConfig(format="%(message)s", stream=sys.stdout, level=logging.DEBUG);
  if(infiles=="-"):
   for line in sys.stdin:
    infilelist.append(line.strip());
   infilelist = list(filter(None, infilelist));
  elif(infiles!="-" and dirlistfromtxt and os.path.exists(infiles) and (os.path.isfile(infiles) or infiles=="/dev/null" or infiles=="NUL")):
   if(not os.path.exists(infiles) or not os.path.isfile(infiles)):
    return False;
-  with open(infiles, "r") as finfile:
+  with UncompressFile(infiles, formatspecs, "r") as finfile:
    for line in finfile:
     infilelist.append(line.strip());
   infilelist = list(filter(None, infilelist));
  else:
   if(isinstance(infiles, (list, tuple, ))):
    infilelist = list(filter(None, infiles));
   elif(isinstance(infiles, (str, ))):
@@ -1096,14 +1225,16 @@
  fnumfiles = format(fnumfiles, 'x').lower();
  for curfname in GetDirList:
   catfhstart = fp.tell();
   if(re.findall("^[.|/]", curfname)):
    fname = curfname;
   else:
    fname = "./"+curfname;
+  if(verbose):
+   VerbosePrintOut(fname);
   if(not followlink or followlink is None):
    fstatinfo = os.lstat(fname);
   else:
    fstatinfo = os.stat(fname);
   fpremode = fstatinfo.st_mode;
   finode = fstatinfo.st_ino;
   flinkcount = fstatinfo.st_nlink;
@@ -1208,51 +1339,105 @@
   flinkcount = format(int(flinkcount), 'x').lower();
   if(hasattr(fstatinfo, "st_file_attributes")):
    fwinattributes = format(int(fstatinfo.st_file_attributes), 'x').lower();
   else:
    fwinattributes = format(int(0), 'x').lower();
   fcontents = "".encode('UTF-8');
   chunk_size = 1024;
-  if(ftype == 0 or ftype == 7):
+  if(ftype==0 or ftype==7):
    with open(fname, "rb") as fpc:
     while(True):
      chunk = fpc.read(chunk_size);
      if(not chunk):
       break
      fcontents += chunk;
-  if(followlink and (ftype == 1 or ftype == 2)):
+  if(followlink and (ftype==1 or ftype==2)):
    flstatinfo = os.stat(flinkname);
    with open(flinkname, "rb") as fpc:
     while(True):
      chunk = fpc.read(chunk_size);
      if(not chunk):
       break;
      fcontents += chunk;
   ftypehex = format(ftype, 'x').lower();
   catoutlist = [ftypehex, fname, flinkname, fsize, fatime, fmtime, fctime, fbtime, fmode, fwinattributes, fuid, funame, fgid, fgname, fcurfid, fcurinode, flinkcount, fdev_minor, fdev_major, frdev_minor, frdev_major];
   fp = AppendFileHeaderWithContent(fp, catoutlist, extradata, fcontents, checksumtype, formatspecs);
  fp.seek(0, 0);
  return fp;
 
-def AppendFilesWithContentToOutFile(infile, outfile, dirlistfromtxt=False, compression="auto", compressionlevel=None, filevalues=[], extradata=[], followlink=False, checksumtype="crc32", formatspecs=__file_format_list__, returnfp=False):
+def AppendListsWithContent(inlist, fp, dirlistfromtxt=False, filevalues=[], extradata=[], followlink=False, checksumtype="crc32", formatspecs=__file_format_list__, verbose=False):
+ advancedlist = True;
+ if(verbose):
+  logging.basicConfig(format="%(message)s", stream=sys.stdout, level=logging.DEBUG);
+ GetDirList = inlist;
+ if(not GetDirList):
+  return False;
+ curinode = 0;
+ curfid = 0;
+ inodelist = [];
+ inodetofile = {};
+ filetoinode = {};
+ inodetocatinode = {};
+ fnumfiles = int(len(GetDirList));
+ AppendFileHeader(fp, fnumfiles, checksumtype, formatspecs);
+ fnumfiles = format(fnumfiles, 'x').lower();
+ for curfname in GetDirList:
+  ftype = format(curfname[0], 'x').lower();
+  if(re.findall("^[.|/]", curfname[1])):
+   fname = curfname[1];
+  else:
+   fname = "./"+curfname[1];
+  fbasedir = os.path.dirname(fname);
+  flinkname = curfname[2];
+  fsize = format(curfname[3], 'x').lower();
+  fatime = format(curfname[4], 'x').lower();
+  fmtime = format(curfname[5], 'x').lower();
+  fctime = format(curfname[6], 'x').lower();
+  fbtime = format(curfname[7], 'x').lower();
+  fmode = format(curfname[8], 'x').lower();
+  fwinattributes = format(curfname[9], 'x').lower();
+  fuid = format(curfname[10], 'x').lower();
+  funame = curfname[11];
+  fgid = format(curfname[12], 'x').lower();
+  fgname = curfname[13];
+  fid = format(curfname[14], 'x').lower();
+  finode = format(curfname[15], 'x').lower();
+  flinkcount = format(curfname[16], 'x').lower();
+  fdev_minor = format(curfname[17], 'x').lower();
+  fdev_major = format(curfname[18], 'x').lower();
+  frdev_minor = format(curfname[19], 'x').lower();
+  frdev_major = format(curfname[20], 'x').lower();
+  extradata = curfname[21];
+  fchecksumtype = curfname[22];
+  fcontents = curfname[23];
+  catoutlist = [ftype, fname, flinkname, fsize, fatime, fmtime, fctime, fbtime, fmode, fwinattributes, fuid, funame, fgid, fgname, fid, finode, flinkcount, fdev_minor, fdev_major, frdev_minor, frdev_major];
+  fp = AppendFileHeaderWithContent(fp, catoutlist, extradata, fcontents, checksumtype, formatspecs);
+ fp.seek(0, 0);
+ return fp;
+
+def AppendInFileWithContent(infile, fp, dirlistfromtxt=False, filevalues=[], extradata=[], followlink=False, checksumtype="crc32", formatspecs=__file_format_list__, verbose=False):
+ inlist = ReadInFileBySizeWithContentToList(infile, 0, 0, False, False, formatspecs);
+ return AppendListsWithContent(inlist, fp, dirlistfromtxt, filevalues, extradata, followlink, checksumtype, formatspecs, verbose);
+
+def AppendFilesWithContentToOutFile(infiles, outfile, dirlistfromtxt=False, compression="auto", compressionlevel=None, filevalues=[], extradata=[], followlink=False, checksumtype="crc32", formatspecs=__file_format_list__, verbose=False, returnfp=False):
  if(outfile!="-" and not hasattr(outfile, "read") and not hasattr(outfile, "write")):
   if(os.path.exists(outfile)):
    os.unlink(outfile);
  if(outfile=="-"):
   verbose = False;
   catfpfp = BytesIO();
  elif(hasattr(outfile, "read") or hasattr(outfile, "write")):
   catfp = outfile;
  elif(re.findall(r"^(ftp|ftps|sftp)\:\/\/", str(outfile))):
   catfp = BytesIO();
  else:
   fbasename = os.path.splitext(outfile)[0];
   fextname = os.path.splitext(outfile)[1];
   catfp = CompressOpenFile(outfile, compressionlevel);
- catfp = AppendFilesWithContent(infile, catfp, dirlistfromtxt, filevalues, extradata, followlink, checksumtype, formatspecs);
+ catfp = AppendFilesWithContent(infiles, catfp, dirlistfromtxt, filevalues, extradata, followlink, checksumtype, formatspecs, verbose);
  if(outfile=="-" or hasattr(outfile, "read") or hasattr(outfile, "write")):
   catfp = CompressArchiveFile(catfp, compression, formatspecs);
   try:
    catfp.flush();
    os.fsync(catfp.fileno());
   except io.UnsupportedOperation:
    pass;
@@ -1271,14 +1456,60 @@
  if(returnfp):
   catfp.seek(0, 0);
   return catfp;
  else:
   catfp.close();
   return True;
 
+def AppendListsWithContentToOutFile(inlist, outfile, dirlistfromtxt=False, compression="auto", compressionlevel=None, filevalues=[], extradata=[], followlink=False, checksumtype="crc32", formatspecs=__file_format_list__, verbose=False, returnfp=False):
+ if(outfile!="-" and not hasattr(outfile, "read") and not hasattr(outfile, "write")):
+  if(os.path.exists(outfile)):
+   os.unlink(outfile);
+ if(outfile=="-"):
+  verbose = False;
+  catfpfp = BytesIO();
+ elif(hasattr(outfile, "read") or hasattr(outfile, "write")):
+  catfp = outfile;
+ elif(re.findall(r"^(ftp|ftps|sftp)\:\/\/", str(outfile))):
+  catfp = BytesIO();
+ else:
+  fbasename = os.path.splitext(outfile)[0];
+  fextname = os.path.splitext(outfile)[1];
+  catfp = CompressOpenFile(outfile, compressionlevel);
+ catfp = AppendListsWithContent(inlist, catfp, dirlistfromtxt, filevalues, extradata, followlink, checksumtype, formatspecs, verbose);
+ if(outfile=="-" or hasattr(outfile, "read") or hasattr(outfile, "write")):
+  catfp = CompressArchiveFile(catfp, compression, formatspecs);
+  try:
+   catfp.flush();
+   os.fsync(catfp.fileno());
+  except io.UnsupportedOperation:
+   pass;
+  except AttributeError:
+   pass;
+ if(outfile=="-"):
+  catfp.seek(0, 0);
+  if(hasattr(sys.stdout, "buffer")):
+   shutil.copyfileobj(catfp, sys.stdout.buffer);
+  else:
+   shutil.copyfileobj(catfp, sys.stdout);
+ elif(re.findall(r"^(ftp|ftps|sftp)\:\/\/", str(outfile))):
+  catfp = CompressArchiveFile(catfp, compression, formatspecs);
+  catfp.seek(0, 0);
+  upload_file_to_internet_file(catfp, outfile);
+ if(returnfp):
+  catfp.seek(0, 0);
+  return catfp;
+ else:
+  catfp.close();
+  return True;
+
+def AppendInFileWithContentToOutFile(infile, outfile, dirlistfromtxt=False, compression="auto", compressionlevel=None, filevalues=[], extradata=[], followlink=False, checksumtype="crc32", formatspecs=__file_format_list__, verbose=False, returnfp=False):
+ inlist = ReadInFileBySizeWithContentToList(infile, 0, 0, False, False, formatspecs);
+ return AppendListsWithContentToOutFile(inlist, outfile, dirlistfromtxt, compression, compressionlevel, filevalues, extradata, followlink, checksumtype, formatspecs, verbose, returnfp);
+
 def PrintPermissionString(fchmode, ftype):
  permissions = { 'access': { '0': ('---'), '1': ('--x'), '2': ('-w-'), '3': ('-wx'), '4': ('r--'), '5': ('r-x'), '6': ('rw-'), '7': ('rwx') }, 'roles': { 0: 'owner', 1: 'group', 2: 'other' } };
  permissionstr = "";
  for fmodval in str(oct(fchmode))[-3:]:
   permissionstr = permissionstr + permissions['access'].get(fmodval, '---');
  if(ftype==0 or ftype==7):
   permissionstr = "-" + permissionstr;
@@ -1746,15 +1977,14 @@
  except FileNotFoundError:
   return False;
  catdata = catfp.read();
  catfp.close();
  return catdata;
 
 def CompressArchiveFile(fp, compression="auto", compressionlevel=None, formatspecs=__file_format_list__):
- compressionlist = ['auto', 'gzip', 'bzip2', 'zstd', 'lz4', 'lzo', 'lzop', 'lzma', 'xz'];
  if(not hasattr(fp, "read") and not hasattr(fp, "write")):
   return False;
  fp.seek(0, 0);
  if(not compression or compression or compression=="catfile" or compression==formatspecs[2]):
   compression = None;
  if(compression not in compressionlist and compression is None):
   compression = "auto";
@@ -1961,17 +2191,14 @@
  checklistout = hash_list;
  if(checkfor in checklistout):
   return True;
  else:
   return False;
 
 def PackArchiveFile(infiles, outfile, dirlistfromtxt=False, compression="auto", compressionlevel=None, followlink=False, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False, returnfp=False):
- compressionlist = ['auto', 'gzip', 'bzip2', 'zstd', 'lz4', 'lzo', 'lzop', 'lzma', 'xz'];
- outextlist = ['gz', 'bz2', 'zst', 'lz4', 'lzo', 'lzop', 'lzma', 'xz'];
- outextlistwd = ['.gz', '.bz2', '.zst', '.lz4', '.lzo', '.lzop', '.lzma', '.xz'];
  advancedlist = True;
  if(outfile!="-" and not hasattr(outfile, "read") and not hasattr(outfile, "write")):
   outfile = RemoveWindowsPath(outfile);
  checksumtype = checksumtype.lower();
  if(not CheckSumSupport(checksumtype, hashlib_guaranteed)):
   checksumtype="crc32";
  if(checksumtype=="none"):
@@ -2004,15 +2231,15 @@
  if(infiles=="-"):
   for line in sys.stdin:
    infilelist.append(line.strip());
   infilelist = list(filter(None, infilelist));
  elif(infiles!="-" and dirlistfromtxt and os.path.exists(infiles) and (os.path.isfile(infiles) or infiles=="/dev/null" or infiles=="NUL")):
   if(not os.path.exists(infiles) or not os.path.isfile(infiles)):
    return False;
-  with open(infiles, "r") as finfile:
+  with UncompressFile(infiles, formatspecs, "r") as finfile:
    for line in finfile:
     infilelist.append(line.strip());
   infilelist = list(filter(None, infilelist));
  else:
   if(isinstance(infiles, (list, tuple, ))):
    infilelist = list(filter(None, infiles));
   elif(isinstance(infiles, (str, ))):
@@ -2176,22 +2403,22 @@
   flinkcount = format(int(flinkcount), 'x').lower();
   if(hasattr(fstatinfo, "st_file_attributes")):
    fwinattributes = format(int(fstatinfo.st_file_attributes), 'x').lower();
   else:
    fwinattributes = format(int(0), 'x').lower();
   fcontents = "".encode('UTF-8');
   chunk_size = 1024;
-  if(ftype == 0 or ftype == 7):
+  if(ftype==0 or ftype==7):
    with open(fname, "rb") as fpc:
     while(True):
      chunk = fpc.read(chunk_size);
      if(not chunk):
       break
      fcontents += chunk;
-  if(followlink and (ftype == 1 or ftype == 2)):
+  if(followlink and (ftype==1 or ftype==2)):
    flstatinfo = os.stat(flinkname);
    with open(flinkname, "rb") as fpc:
     while(True):
      chunk = fpc.read(chunk_size);
      if(not chunk):
       break;
      fcontents += chunk;
@@ -2311,17 +2538,14 @@
   return PackArchiveFile(source_dir, archive_name, False, "auto", None, False, "crc32", [], __file_format_delimiter__, False, False);
  create_alias_function("Pack", __file_format_name__, "Func", PackArchiveFileFunc);
 
 def PackArchiveFileFromDirList(infiles, outfile, dirlistfromtxt=False, compression="auto", compressionlevel=None, followlink=False, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False, returnfp=False):
  return PackArchiveFile(infiles, outfile, dirlistfromtxt, compression, compressionlevel, followlink, checksumtype, extradata, formatspecs, verbose, returnfp);
 
 def PackArchiveFileFromTarFile(infile, outfile, compression="auto", compressionlevel=None, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False, returnfp=False):
- compressionlist = ['auto', 'gzip', 'bzip2', 'zstd', 'lz4', 'lzo', 'lzop', 'lzma', 'xz'];
- outextlist = ['gz', 'bz2', 'zst', 'lz4', 'lzo', 'lzop', 'lzma', 'xz'];
- outextlistwd = ['.gz', '.bz2', '.zst', '.lz4', '.lzo', '.lzop', '.lzma', '.xz'];
  if(outfile!="-" and not hasattr(outfile, "read") and not hasattr(outfile, "write")):
   outfile = RemoveWindowsPath(outfile);
  checksumtype = checksumtype.lower();
  if(not CheckSumSupport(checksumtype, hashlib_guaranteed)):
   checksumtype="crc32";
  if(checksumtype=="none"):
   checksumtype = "";
@@ -2489,15 +2713,15 @@
   fgid = format(int(member.gid), 'x').lower();
   funame = member.uname;
   fgname = member.gname;
   flinkcount = format(int(flinkcount), 'x').lower();
   fwinattributes = format(int(0), 'x').lower();
   fcontents = "".encode('UTF-8');
   chunk_size = 1024;
-  if(ftype == 0 or ftype == 7):
+  if(ftype==0 or ftype==7):
    with tarfp.extractfile(member) as fpc:
     while(True):
      chunk = fpc.read(chunk_size);
      if(not chunk):
       break
      fcontents += chunk;
   ftypehex = format(ftype, 'x').lower();
@@ -2608,17 +2832,14 @@
  else:
   catfp.close();
   return True;
 
 create_alias_function("Pack", __file_format_name__, "FromTarFile", PackArchiveFileFromTarFile);
 
 def PackArchiveFileFromZipFile(infile, outfile, compression="auto", compressionlevel=None, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False, returnfp=False):
- compressionlist = ['auto', 'gzip', 'bzip2', 'zstd', 'lz4', 'lzo', 'lzop', 'lzma', 'xz'];
- outextlist = ['gz', 'bz2', 'zst', 'lz4', 'lzo', 'lzop', 'lzma', 'xz'];
- outextlistwd = ['.gz', '.bz2', '.zst', '.lz4', '.lzo', '.lzop', '.lzma', '.xz'];
  if(outfile!="-" and not hasattr(outfile, "read") and not hasattr(outfile, "write")):
   outfile = RemoveWindowsPath(outfile);
  checksumtype = checksumtype.lower();
  if(not CheckSumSupport(checksumtype, hashlib_guaranteed)):
   checksumtype="crc32";
  if(checksumtype=="none"):
   checksumtype = "";
@@ -2925,17 +3146,14 @@
 
 if(not rarfile_support):
  def PackArchiveFileFromRarFile(infile, outfile, compression="auto", compressionlevel=None, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False, returnfp=False):
   return False
 
 if(rarfile_support):
  def PackArchiveFileFromRarFile(infile, outfile, compression="auto", compressionlevel=None, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False, returnfp=False):
-  compressionlist = ['auto', 'gzip', 'bzip2', 'zstd', 'lz4', 'lzo', 'lzop', 'lzma', 'xz'];
-  outextlist = ['gz', 'bz2', 'zst', 'lz4', 'lzo', 'lzop', 'lzma', 'xz'];
-  outextlistwd = ['.gz', '.bz2', '.zst', '.lz4', '.lzo', '.lzop', '.lzma', '.xz'];
   if(outfile!="-" and not hasattr(outfile, "read") and not hasattr(outfile, "write")):
    outfile = RemoveWindowsPath(outfile);
   checksumtype = checksumtype.lower();
   if(not CheckSumSupport(checksumtype, hashlib_guaranteed)):
    checksumtype="crc32";
   if(checksumtype=="none"):
    checksumtype = "";
@@ -3007,22 +3225,22 @@
   except io.UnsupportedOperation:
    pass;
   except AttributeError:
    pass;
   for member in sorted(rarfp.infolist(), key=lambda x: x.filename):
    is_unix = False;
    is_windows = False;
-   if(member.host_os == rarfile.RAR_OS_UNIX):
+   if(member.host_os==rarfile.RAR_OS_UNIX):
     is_windows = False;
     try:
      member.external_attr
      is_unix = True;
     except AttributeError:
      is_unix = False;
-   elif(member.host_os == rarfile.RAR_OS_WIN32):
+   elif(member.host_os==rarfile.RAR_OS_WIN32):
     is_unix = False;
     try:
      member.external_attr
      is_windows = True;
     except AttributeError:
      is_windows = False;
    else:
@@ -4390,15 +4608,15 @@
  if(infiles=="-"):
   for line in sys.stdin:
    infilelist.append(line.strip());
   infilelist = list(filter(None, infilelist));
  elif(infiles!="-" and dirlistfromtxt and os.path.exists(infiles) and (os.path.isfile(infiles) or infiles=="/dev/null" or infiles=="NUL")):
   if(not os.path.exists(infiles) or not os.path.isfile(infiles)):
    return False;
-  with open(infiles, "r") as finfile:
+  with UncompressFile(infiles, formatspecs, "r") as finfile:
    for line in finfile:
     infilelist.append(line.strip());
   infilelist = list(filter(None, infilelist));
  else:
   if(isinstance(infiles, (list, tuple, ))):
    infilelist = list(filter(None, infiles));
   elif(isinstance(infiles, (str, ))):
@@ -4561,22 +4779,22 @@
   flinkcount = flinkcount;
   if(hasattr(fstatinfo, "st_file_attributes")):
    fwinattributes = fstatinfo.st_file_attributes;
   else:
    fwinattributes = 0;
   fcontents = "".encode('UTF-8');
   chunk_size = 1024;
-  if(ftype == 0 or ftype == 7):
+  if(ftype==0 or ftype==7):
    with open(fname, "rb") as fpc:
     while(True):
      chunk = fpc.read(chunk_size);
      if(not chunk):
       break
      fcontents += chunk;
-  if(followlink and (ftype == 1 or ftype == 2)):
+  if(followlink and (ftype==1 or ftype==2)):
    flstatinfo = os.stat(flinkname);
    with open(flinkname, "rb") as fpc:
     while(True):
      chunk = fpc.read(chunk_size);
      if(not chunk):
       break;
      fcontents += chunk;
@@ -4816,15 +5034,15 @@
   fgid = member.gid;
   funame = member.uname;
   fgname = member.gname;
   flinkcount = flinkcount;
   fwinattributes = int(0);
   fcontents = "".encode('UTF-8');
   chunk_size = 1024;
-  if(ftype == 0 or ftype == 7):
+  if(ftype==0 or ftype==7):
    with tarfp.extractfile(member) as fpc:
     while(True):
      chunk = fpc.read(chunk_size);
      if(not chunk):
       break
      fcontents += chunk;
   ftypehex = format(ftype, 'x').lower();
@@ -5233,22 +5451,22 @@
    catfileheadercshex = format(0, 'x').lower();
   fileheader = fileheader + AppendNullByte(catfileheadercshex, formatspecs[5]);
   fheadtell = len(fileheader);
   catlist = {'fnumfiles': fnumfiles, 'fformat': catversions[0], 'fversion': catversions[1], 'fformatspecs': formatspecs, 'fchecksumtype': checksumtype, 'fheaderchecksum': catfileheadercshex, 'ffilelist': {}};
   for member in sorted(rarfp.infolist(), key=lambda x: x.filename):
    is_unix = False;
    is_windows = False;
-   if(member.host_os == rarfile.RAR_OS_UNIX):
+   if(member.host_os==rarfile.RAR_OS_UNIX):
     is_windows = False;
     try:
      member.external_attr
      is_unix = True;
     except AttributeError:
      is_unix = False;
-   elif(member.host_os == rarfile.RAR_OS_WIN32):
+   elif(member.host_os==rarfile.RAR_OS_WIN32):
     is_unix = False;
     try:
      member.external_attr
      is_windows = True;
     except AttributeError:
      is_windows = False;
    else:
@@ -5765,17 +5983,14 @@
 def ListDirToArrayIndex(infiles, dirlistfromtxt=False, compression="auto", compressionlevel=None, followlink=False, seekstart=0, seekend=0, listonly=False, skipchecksum=False, checksumtype="crc32", formatspecs=__file_format_list__, verbose=False, returnfp=False):
  outarray = BytesIO();
  packcat = PackArchiveFile(infiles, outarray, dirlistfromtxt, compression, compressionlevel, followlink, checksumtype, formatspecs, verbose, True);
  listcatfiles = ArchiveFileToArrayIndex(outarray, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp)
  return listcatfiles;
 
 def RePackArchiveFile(infile, outfile, compression="auto", compressionlevel=None, followlink=False, seekstart=0, seekend=0, checksumtype="crc32", skipchecksum=False, extradata=[], formatspecs=__file_format_list__, verbose=False, returnfp=False):
- compressionlist = ['auto', 'gzip', 'bzip2', 'zstd', 'lz4', 'lzo', 'lzop', 'lzma', 'xz'];
- outextlist = ['gz', 'bz2', 'zst', 'lz4', 'lzop', 'lzo', 'lzma', 'xz'];
- outextlistwd = ['.gz', '.bz2', '.zst', '.lz4', 'lzop', '.lzo', '.lzma', '.xz'];
  if(isinstance(infile, dict)):
   prelistcatfiles = ArchiveFileToArrayIndex(infile, seekstart, seekend, False, skipchecksum, formatspecs, returnfp);
   listcatfiles = prelistcatfiles['list'];
  else:
   if(infile!="-" and not hasattr(infile, "read") and not hasattr(infile, "write")):
    infile = RemoveWindowsPath(infile);
   if(followlink):
@@ -5891,15 +6106,15 @@
   fwinattributes = flinkinfo['ffilelist'][reallcfi]['fwinattributes'];
   fdev_minor = format(int(listcatfiles['ffilelist'][reallcfi]['fminor']), 'x').lower();
   fdev_major = format(int(listcatfiles['ffilelist'][reallcfi]['fmajor']), 'x').lower();
   frdev_minor = format(int(listcatfiles['ffilelist'][reallcfi]['frminor']), 'x').lower();
   frdev_major = format(int(listcatfiles['ffilelist'][reallcfi]['frmajor']), 'x').lower();
   if(len(listcatfiles['ffilelist'][reallcfi]['fextralist'])>listcatfiles['ffilelist'][reallcfi]['fextrafields'] and len(listcatfiles['ffilelist'][reallcfi]['fextralist'])>0):
    listcatfiles['ffilelist'][reallcfi]['fextrafields'] = len(listcatfiles['ffilelist'][reallcfi]['fextralist']);
-  if(len(extradata) > 0):
+  if(len(extradata)>0):
    listcatfiles['ffilelist'][reallcfi]['fextrafields'] = len(extradata);
    listcatfiles['ffilelist'][reallcfi]['fextralist'] = extradata;
   extrafields = format(int(listcatfiles['ffilelist'][reallcfi]['fextrafields']), 'x').lower();
   extrasizestr = AppendNullByte(extrafields, formatspecs[5]);
   if(len(extradata)>0):
    extrasizestr = extrasizestr + AppendNullBytes(extradata, formatspecs[5]);
   extrasizelen = format(len(extrasizestr), 'x').lower();
@@ -5927,15 +6142,15 @@
     fwinattributes = flinkinfo['fwinattributes'];
     fdev_minor = format(int(flinkinfo['fminor']), 'x').lower();
     fdev_major = format(int(flinkinfo['fmajor']), 'x').lower();
     frdev_minor = format(int(flinkinfo['frminor']), 'x').lower();
     frdev_major = format(int(flinkinfo['frmajor']), 'x').lower();
     if(len(flinkinfo['fextralist'])>flinkinfo['fextrafields'] and len(flinkinfo['fextralist'])>0):
      flinkinfo['fextrafields'] = len(flinkinfo['fextralist']);
-    if(len(extradata) > 0):
+    if(len(extradata)>0):
      flinkinfo['fextrafields'] = len(extradata);
      flinkinfo['fextralist'] = extradata;
     extrafields = format(int(flinkinfo['fextrafields']), 'x').lower();
     extrasizestr = AppendNullByte(extrafields, formatspecs[5]);
     if(len(extradata)>0):
      extrasizestr = extrasizestr + AppendNullBytes(extradata, formatspecs[5]);
     extrasizelen = format(len(extrasizestr), 'x').lower();
@@ -5971,15 +6186,15 @@
   catoutlenhex = format(catoutlen, 'x').lower();
   catoutlist.insert(0, catoutlenhex);
   catfileoutstr = AppendNullBytes(catoutlist, formatspecs[5]);
   if(listcatfiles['ffilelist'][reallcfi]['fextrafields']>0):
    extrafieldslist = [];
    exi = 0;
    exil = listcatfiles['ffilelist'][reallcfi]['fextrafields'];
-   while(exi < exil):
+   while(exi<exil):
     extrafieldslist.append(listcatfiles['ffilelist'][reallcfi]['fextralist']);
     exi = exi + 1;
    catfileoutstr += AppendNullBytes([extrafieldslist], formatspecs[5]);
   catfileoutstr += AppendNullBytes([checksumtype], formatspecs[5]);
   catfhend = (catfp.tell() - 1) + len(catfileoutstr);
   catfcontentstart = catfp.tell() + len(catfileoutstr);
   if(checksumtype=="none" or checksumtype==""):
@@ -6114,15 +6329,15 @@
  fnumfiles = int(listcatfiles['fnumfiles']);
  lcfi = 0;
  lcfx = int(listcatfiles['fnumfiles']);
  if(lenlist>listcatfiles['fnumfiles'] or lenlist<listcatfiles['fnumfiles']):
   lcfx = int(lenlist);
  else:
   lcfx = int(listcatfiles['fnumfiles']);
- while(lcfi < lcfx):
+ while(lcfi<lcfx):
   if(listcatfiles['ffilelist'][lcfi]['fhascontents']):
    listcatfiles['ffilelist'][lcfi]['fcontents'] = base64.b64encode(listcatfiles['ffilelist'][lcfi]['fcontents']).decode("UTF-8");
   lcfi = lcfi + 1;
  return listcatfiles;
 
 create_alias_function("", __file_format_name__, "ArrayBase64Encode", ArchiveFileArrayBase64Encode);
 
@@ -6146,15 +6361,15 @@
  fnumfiles = int(listcatfiles['fnumfiles']);
  lcfi = 0;
  lcfx = int(listcatfiles['fnumfiles']);
  if(lenlist>listcatfiles['fnumfiles'] or lenlist<listcatfiles['fnumfiles']):
   lcfx = int(lenlist);
  else:
   lcfx = int(listcatfiles['fnumfiles']);
- while(lcfi < lcfx):
+ while(lcfi<lcfx):
   if(listcatfiles['ffilelist'][lcfi]['fhascontents']):
    listcatfiles['ffilelist'][lcfi]['fcontents'] = base64.b64decode(listcatfiles['ffilelist'][lcfi]['fcontents'].encode("UTF-8"));
   lcfi = lcfi + 1;
  return listcatfiles;
 
 create_alias_function("", __file_format_name__, "ArrayBase64Decode", ArchiveFileArrayBase64Decode);
 
@@ -6180,15 +6395,15 @@
  fnumfiles = int(listcatfiles['fnumfiles']);
  lcfi = 0;
  lcfx = int(listcatfiles['fnumfiles']);
  if(lenlist>listcatfiles['fnumfiles'] or lenlist<listcatfiles['fnumfiles']):
   lcfx = int(lenlist);
  else:
   lcfx = int(listcatfiles['fnumfiles']);
- while(lcfi < lcfx):
+ while(lcfi<lcfx):
   funame = "";
   try:
    import pwd;
    try:
     userinfo = pwd.getpwuid(listcatfiles['ffilelist'][lcfi]['fuid']);
     funame = userinfo.pw_name;
    except KeyError:
@@ -6244,15 +6459,15 @@
      try:
       groupinfo = grp.getgrgid(flinkinfo['fgid']);
       fgname = groupinfo.gr_name;
      except KeyError:
       fgname = "";
     except ImportError:
      fgname = "";
-    if(flinkinfo['ftype'] == 0 or flinkinfo['ftype'] == 7):
+    if(flinkinfo['ftype']==0 or flinkinfo['ftype']==7):
      with open(PrependPath(outdir, listcatfiles['ffilelist'][lcfi]['fname']), "wb") as fpc:
       fpc.write(flinkinfo['fcontents'])
       try:
        fpc.flush()
        os.fsync(fpc.fileno())
       except io.UnsupportedOperation:
        pass
@@ -6391,15 +6606,15 @@
  lcfi = 0;
  lcfx = int(listcatfiles['fnumfiles']);
  if(lenlist>listcatfiles['fnumfiles'] or lenlist<listcatfiles['fnumfiles']):
   lcfx = int(lenlist);
  else:
   lcfx = int(listcatfiles['fnumfiles']);
  returnval = {};
- while(lcfi < lcfx):
+ while(lcfi<lcfx):
   returnval.update({lcfi: listcatfiles['ffilelist'][lcfi]['fname']});
   if(not verbose):
    VerbosePrintOut(listcatfiles['ffilelist'][lcfi]['fname']);
   if(verbose):
    permissions = { 'access': { '0': ('---'), '1': ('--x'), '2': ('-w-'), '3': ('-wx'), '4': ('r--'), '5': ('r-x'), '6': ('rw-'), '7': ('rwx') }, 'roles': { 0: 'owner', 1: 'group', 2: 'other' } };
    printfname = listcatfiles['ffilelist'][lcfi]['fname'];
    if(listcatfiles['ffilelist'][lcfi]['ftype']==1):
@@ -6443,15 +6658,15 @@
  lcfi = 0;
  lcfx = int(listcatfiles['fnumfiles']);
  if(lenlist>listcatfiles['fnumfiles'] or lenlist<listcatfiles['fnumfiles']):
   lcfx = int(lenlist);
  else:
   lcfx = int(listcatfiles['fnumfiles']);
  returnval = {};
- while(lcfi < lcfx):
+ while(lcfi<lcfx):
   returnval.update({lcfi: listcatfiles['ffilelist'][lcfi]['fname']});
   if(not verbose):
    VerbosePrintOut(listcatfiles['ffilelist'][lcfi]['fname']);
   if(verbose):
    permissions = { 'access': { '0': ('---'), '1': ('--x'), '2': ('-w-'), '3': ('-wx'), '4': ('r--'), '5': ('r-x'), '6': ('rw-'), '7': ('rwx') }, 'roles': { 0: 'owner', 1: 'group', 2: 'other' } };
    printfname = listcatfiles['ffilelist'][lcfi]['fname'];
    if(listcatfiles['ffilelist'][lcfi]['ftype']==1):
@@ -6711,22 +6926,22 @@
   rarfp = rarfile.RarFile(infile, "r");
   rartest = rarfp.testrar();
   if(rartest):
    VerbosePrintOut("Bad file found!");
   for member in sorted(rarfp.infolist(), key=lambda x: x.filename):
    is_unix = False;
    is_windows = False;
-   if(member.host_os == rarfile.RAR_OS_UNIX):
+   if(member.host_os==rarfile.RAR_OS_UNIX):
     is_windows = False;
     try:
      member.external_attr
      is_unix = True;
     except AttributeError:
      is_unix = False;
-   elif(member.host_os == rarfile.RAR_OS_WIN32):
+   elif(member.host_os==rarfile.RAR_OS_WIN32):
     is_unix = False;
     try:
      member.external_attr
      is_windows = True;
     except AttributeError:
      is_windows = False;
    else:
@@ -7268,14 +7483,22 @@
    return download_file_from_pysftp_file(url);
   else:
    return download_file_from_sftp_file(url);
  else:
   return False;
  return False;
 
+def download_file_from_internet_uncompress_file(url, headers=geturls_headers_pycatfile_python_alt, formatspecs=__file_format_list__):
+ fp = download_file_from_internet_file(url);
+ fp = UncompressArchiveFile(fp, formatspecs);
+ fp.seek(0, 0);
+ if(not fp):
+  return False;
+ return fp;
+
 def download_file_from_internet_string(url, headers=geturls_headers_pycatfile_python_alt):
  urlparts = urlparse(url);
  if(urlparts.scheme=="http" or urlparts.scheme=="https"):
   return download_file_from_http_string(url, headers);
  elif(urlparts.scheme=="ftp" or urlparts.scheme=="ftps"):
   return download_file_from_ftp_string(url);
  elif(urlparts.scheme=="sftp"):
@@ -7283,14 +7506,22 @@
    return download_file_from_pysftp_string(url);
   else:
    return download_file_from_sftp_string(url);
  else:
   return False;
  return False;
 
+def download_file_from_internet_uncompress_string(url, headers=geturls_headers_pycatfile_python_alt, formatspecs=__file_format_list__):
+ fp = download_file_from_internet_string(url);
+ fp = UncompressArchiveFile(fp, formatspecs);
+ fp.seek(0, 0);
+ if(not fp):
+  return False;
+ return fp;
+
 def upload_file_to_internet_file(ifp, url):
  urlparts = urlparse(url);
  if(urlparts.scheme=="http" or urlparts.scheme=="https"):
   return False;
  elif(urlparts.scheme=="ftp" or urlparts.scheme=="ftps"):
   return upload_file_from_ftp_file(ifp, url);
  elif(urlparts.scheme=="sftp"):
@@ -7298,28 +7529,44 @@
    return upload_file_from_pysftp_file(ifp, url);
   else:
    return download_file_from_sftp_file(ifp, url);
  else:
   return False;
  return False;
 
+def upload_file_to_internet_compress_file(ifp, url, formatspecs=__file_format_list__):
+ catfp = CompressArchiveFile(catfp, compression, formatspecs);
+ if(not catfileout):
+  return False;
+ catfp.seek(0, 0);
+ upload_file_to_internet_file(catfp, outfile);
+ return True;
+
 def upload_file_to_internet_string(ifp, url):
  urlparts = urlparse(url);
  if(urlparts.scheme=="http" or urlparts.scheme=="https"):
   return False;
  elif(urlparts.scheme=="ftp" or urlparts.scheme=="ftps"):
   return upload_file_from_ftp_string(ifp, url);
  elif(urlparts.scheme=="sftp"):
   if(__use_pysftp__ and havepysftp):
    return upload_file_from_pysftp_string(ifp, url);
   else:
    return download_file_from_sftp_string(ifp, url);
  else:
   return False;
  return False;
+ 
+def upload_file_to_internet_compress_string(ifp, url, formatspecs=__file_format_list__):
+ catfp = CompressArchiveFile(BytesIO(ifp), compression, formatspecs);
+ if(not catfileout):
+  return False;
+ catfp.seek(0, 0);
+ upload_file_to_internet_file(catfp, outfile);
+ return True;
 
 try:
  if(hasattr(shutil, "register_archive_format")):
   # Register the packing format
   shutil.register_archive_format(__file_format_name__, PackArchiveFileFunc, description='Pack concatenated files');
 except shutil.RegistryError:
  pass;
```

### Comparing `PyCatFile-0.7.0/setup.py` & `PyCatFile-0.7.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2016-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2016-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2016-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: setup.py - Last Update: 3/29/2024 Ver. 0.7.0 RC 1 - Author: cooldude2k $
+    $FileInfo: setup.py - Last Update: 4/1/2024 Ver. 0.7.4 RC 1 - Author: cooldude2k $
 '''
 
 import os, re, sys, pkg_resources;
 from setuptools import setup;
 
 verinfofilename = os.path.realpath("."+os.path.sep+os.path.sep+"pycatfile.py");
 verinfofile = open(verinfofilename, "r");
```

