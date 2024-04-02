# Comparing `tmp/ydiff-1.2.tar.gz` & `tmp/ydiff-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ydiff-1.2.tar", last modified: Sat Aug  8 10:40:44 2020, max compression
+gzip compressed data, was "ydiff-1.3.tar", last modified: Tue Apr  2 09:10:59 2024, max compression
```

## Comparing `ydiff-1.2.tar` & `ydiff-1.3.tar`

### file list

```diff
@@ -1,122 +1,131 @@
-drwxrwxr-x   0 ymattw    (1001) ymattw    (1003)        0 2020-08-08 10:40:44.000000 ydiff-1.2/
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)    15784 2020-08-08 10:40:44.000000 ydiff-1.2/PKG-INFO
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1331 2019-10-20 12:14:41.000000 ydiff-1.2/Makefile
--rwxrwxr-x   0 ymattw    (1001) ymattw    (1003)     1350 2019-10-20 12:14:41.000000 ydiff-1.2/setup.py
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1584 2020-08-08 10:16:33.000000 ydiff-1.2/LICENSE
-drwxrwxr-x   0 ymattw    (1001) ymattw    (1003)        0 2020-08-08 10:40:44.000000 ydiff-1.2/tests/
-drwxrwxr-x   0 ymattw    (1001) ymattw    (1003)        0 2020-08-08 10:40:44.000000 ydiff-1.2/tests/crlf/
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1358 2019-10-20 12:14:41.000000 ydiff-1.2/tests/crlf/out.normal
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     3580 2019-10-20 12:14:41.000000 ydiff-1.2/tests/crlf/out.w70
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     3744 2019-10-20 12:14:41.000000 ydiff-1.2/tests/crlf/out.side-by-side
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1041 2019-10-20 12:14:41.000000 ydiff-1.2/tests/crlf/in.diff
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     4151 2019-10-20 12:14:41.000000 ydiff-1.2/tests/crlf/out.w70.wrap
-drwxrwxr-x   0 ymattw    (1001) ymattw    (1003)        0 2020-08-08 10:40:44.000000 ydiff-1.2/tests/strange/
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      639 2019-10-20 12:14:41.000000 ydiff-1.2/tests/strange/out.normal
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      937 2019-10-20 12:14:41.000000 ydiff-1.2/tests/strange/out.w70
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      967 2019-10-20 12:14:41.000000 ydiff-1.2/tests/strange/out.side-by-side
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      456 2019-10-20 12:14:41.000000 ydiff-1.2/tests/strange/in.diff
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      937 2019-10-20 12:14:41.000000 ydiff-1.2/tests/strange/out.w70.wrap
-drwxrwxr-x   0 ymattw    (1001) ymattw    (1003)        0 2020-08-08 10:40:44.000000 ydiff-1.2/tests/diff-of-diff/
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1625 2019-10-20 12:14:41.000000 ydiff-1.2/tests/diff-of-diff/out.normal
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     4506 2020-08-08 09:54:53.000000 ydiff-1.2/tests/diff-of-diff/out.w70
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     4786 2020-08-08 09:54:53.000000 ydiff-1.2/tests/diff-of-diff/out.side-by-side
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1141 2019-10-20 12:14:41.000000 ydiff-1.2/tests/diff-of-diff/in.diff
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     4506 2020-08-08 09:54:53.000000 ydiff-1.2/tests/diff-of-diff/out.w70.wrap
--rwxrwxr-x   0 ymattw    (1001) ymattw    (1003)     2123 2020-08-04 19:44:52.000000 ydiff-1.2/tests/regression.sh
-drwxrwxr-x   0 ymattw    (1001) ymattw    (1003)        0 2020-08-08 10:40:44.000000 ydiff-1.2/tests/diff-ru-bin/
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1019 2019-10-20 12:14:41.000000 ydiff-1.2/tests/diff-ru-bin/out.normal
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1721 2019-10-20 12:14:41.000000 ydiff-1.2/tests/diff-ru-bin/out.w70
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1786 2019-10-20 12:14:41.000000 ydiff-1.2/tests/diff-ru-bin/out.side-by-side
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      708 2019-10-20 12:14:41.000000 ydiff-1.2/tests/diff-ru-bin/in.diff
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1891 2019-10-20 12:14:41.000000 ydiff-1.2/tests/diff-ru-bin/out.w70.wrap
-drwxrwxr-x   0 ymattw    (1001) ymattw    (1003)        0 2020-08-08 10:40:44.000000 ydiff-1.2/tests/git/
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     2308 2019-10-20 12:14:41.000000 ydiff-1.2/tests/git/out.normal
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     4771 2019-10-20 12:14:41.000000 ydiff-1.2/tests/git/out.w70
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     5012 2019-10-20 12:14:41.000000 ydiff-1.2/tests/git/out.side-by-side
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1683 2019-10-20 12:14:41.000000 ydiff-1.2/tests/git/in.diff
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     5265 2019-10-20 12:14:41.000000 ydiff-1.2/tests/git/out.w70.wrap
-drwxrwxr-x   0 ymattw    (1001) ymattw    (1003)        0 2020-08-08 10:40:44.000000 ydiff-1.2/tests/hg-log/
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     2662 2019-10-20 12:14:41.000000 ydiff-1.2/tests/hg-log/out.normal
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     5593 2019-10-20 12:14:41.000000 ydiff-1.2/tests/hg-log/out.w70
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     5883 2019-10-20 12:14:41.000000 ydiff-1.2/tests/hg-log/out.side-by-side
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     2085 2019-10-20 12:14:41.000000 ydiff-1.2/tests/hg-log/in.diff
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     5593 2019-10-20 12:14:41.000000 ydiff-1.2/tests/hg-log/out.w70.wrap
--rwxrwxr-x   0 ymattw    (1001) ymattw    (1003)      553 2019-10-20 12:14:41.000000 ydiff-1.2/tests/profile.sh
-drwxrwxr-x   0 ymattw    (1001) ymattw    (1003)        0 2020-08-08 10:40:44.000000 ydiff-1.2/tests/git-log/
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1308 2019-10-20 12:14:41.000000 ydiff-1.2/tests/git-log/out.normal
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     2466 2019-10-20 12:14:41.000000 ydiff-1.2/tests/git-log/out.w70
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     2558 2019-10-20 12:14:41.000000 ydiff-1.2/tests/git-log/out.side-by-side
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      972 2019-10-20 12:14:41.000000 ydiff-1.2/tests/git-log/in.diff
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     2800 2019-10-20 12:14:41.000000 ydiff-1.2/tests/git-log/out.w70.wrap
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      330 2019-10-20 12:14:41.000000 ydiff-1.2/tests/README
--rwxrwxr-x   0 ymattw    (1001) ymattw    (1003)    27137 2020-08-04 19:44:52.000000 ydiff-1.2/tests/test_ydiff.py
-drwxrwxr-x   0 ymattw    (1001) ymattw    (1003)        0 2020-08-08 10:40:44.000000 ydiff-1.2/tests/perforce/
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     2656 2019-10-20 12:14:41.000000 ydiff-1.2/tests/perforce/out.normal
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     5458 2019-10-20 12:14:41.000000 ydiff-1.2/tests/perforce/out.w70
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     5745 2019-10-20 12:14:41.000000 ydiff-1.2/tests/perforce/out.side-by-side
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1824 2019-10-20 12:14:41.000000 ydiff-1.2/tests/perforce/in.diff
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     5752 2019-10-20 12:14:41.000000 ydiff-1.2/tests/perforce/out.w70.wrap
-drwxrwxr-x   0 ymattw    (1001) ymattw    (1003)        0 2020-08-08 10:40:44.000000 ydiff-1.2/tests/evil-udiff/
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      710 2019-10-20 12:14:41.000000 ydiff-1.2/tests/evil-udiff/out.normal
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1814 2019-10-20 12:14:41.000000 ydiff-1.2/tests/evil-udiff/out.w70
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1934 2019-10-20 12:14:41.000000 ydiff-1.2/tests/evil-udiff/out.side-by-side
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      423 2019-10-20 12:14:41.000000 ydiff-1.2/tests/evil-udiff/in.diff
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1814 2019-10-20 12:14:41.000000 ydiff-1.2/tests/evil-udiff/out.w70.wrap
-drwxrwxr-x   0 ymattw    (1001) ymattw    (1003)        0 2020-08-08 10:40:44.000000 ydiff-1.2/tests/svn-property/
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      220 2019-10-20 12:14:41.000000 ydiff-1.2/tests/svn-property/out.normal
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      220 2019-10-20 12:14:41.000000 ydiff-1.2/tests/svn-property/out.w70
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      220 2019-10-20 12:14:41.000000 ydiff-1.2/tests/svn-property/out.side-by-side
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      166 2019-10-20 12:14:41.000000 ydiff-1.2/tests/svn-property/in.diff
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      220 2019-10-20 12:14:41.000000 ydiff-1.2/tests/svn-property/out.w70.wrap
-drwxrwxr-x   0 ymattw    (1001) ymattw    (1003)        0 2020-08-08 10:40:44.000000 ydiff-1.2/tests/diff-ru/
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1128 2019-10-20 12:14:41.000000 ydiff-1.2/tests/diff-ru/out.normal
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1726 2019-10-20 12:14:41.000000 ydiff-1.2/tests/diff-ru/out.w70
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1781 2020-08-04 18:59:46.000000 ydiff-1.2/tests/diff-ru/out.side-by-side
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      744 2019-10-20 12:14:41.000000 ydiff-1.2/tests/diff-ru/in.diff
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1896 2019-10-20 12:14:41.000000 ydiff-1.2/tests/diff-ru/out.w70.wrap
-drwxrwxr-x   0 ymattw    (1001) ymattw    (1003)        0 2020-08-08 10:40:44.000000 ydiff-1.2/tests/svn/
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1328 2019-10-20 12:14:41.000000 ydiff-1.2/tests/svn/out.normal
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     3573 2019-10-20 12:14:41.000000 ydiff-1.2/tests/svn/out.w70
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     3737 2019-10-20 12:14:41.000000 ydiff-1.2/tests/svn/out.side-by-side
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1039 2019-10-20 12:14:41.000000 ydiff-1.2/tests/svn/in.diff
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     4144 2019-10-20 12:14:41.000000 ydiff-1.2/tests/svn/out.w70.wrap
-drwxrwxr-x   0 ymattw    (1001) ymattw    (1003)        0 2020-08-08 10:40:44.000000 ydiff-1.2/tests/svn-log/
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1928 2019-10-20 12:14:41.000000 ydiff-1.2/tests/svn-log/out.normal
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     3389 2019-10-20 12:14:41.000000 ydiff-1.2/tests/svn-log/out.w70
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     3539 2019-10-20 12:14:41.000000 ydiff-1.2/tests/svn-log/out.side-by-side
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1480 2019-10-20 12:14:41.000000 ydiff-1.2/tests/svn-log/in.diff
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     3389 2019-10-20 12:14:41.000000 ydiff-1.2/tests/svn-log/out.w70.wrap
-drwxrwxr-x   0 ymattw    (1001) ymattw    (1003)        0 2020-08-08 10:40:44.000000 ydiff-1.2/tests/context/
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1975 2019-10-20 12:14:41.000000 ydiff-1.2/tests/context/out.normal
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     4907 2019-10-20 12:14:41.000000 ydiff-1.2/tests/context/out.w70
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     5196 2019-10-20 12:14:41.000000 ydiff-1.2/tests/context/out.side-by-side
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     2097 2019-10-20 12:14:41.000000 ydiff-1.2/tests/context/in.diff
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     5019 2019-10-20 12:14:41.000000 ydiff-1.2/tests/context/out.w70.wrap
-drwxrwxr-x   0 ymattw    (1001) ymattw    (1003)        0 2020-08-08 10:40:44.000000 ydiff-1.2/tests/git-bin/
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      957 2019-10-20 12:14:41.000000 ydiff-1.2/tests/git-bin/out.normal
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1830 2019-10-20 12:14:41.000000 ydiff-1.2/tests/git-bin/out.w70
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1914 2019-10-20 12:14:41.000000 ydiff-1.2/tests/git-bin/out.side-by-side
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      633 2019-10-20 12:14:41.000000 ydiff-1.2/tests/git-bin/in.diff
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     1924 2019-10-20 12:14:41.000000 ydiff-1.2/tests/git-bin/out.w70.wrap
-drwxrwxr-x   0 ymattw    (1001) ymattw    (1003)        0 2020-08-08 10:40:44.000000 ydiff-1.2/tests/svn-merge/
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      434 2019-10-20 12:14:41.000000 ydiff-1.2/tests/svn-merge/out.normal
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      434 2019-10-20 12:14:41.000000 ydiff-1.2/tests/svn-merge/out.w70
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      434 2019-10-20 12:14:41.000000 ydiff-1.2/tests/svn-merge/out.side-by-side
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      326 2019-10-20 12:14:41.000000 ydiff-1.2/tests/svn-merge/in.diff
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      434 2019-10-20 12:14:41.000000 ydiff-1.2/tests/svn-merge/out.w70.wrap
-drwxrwxr-x   0 ymattw    (1001) ymattw    (1003)        0 2020-08-08 10:40:44.000000 ydiff-1.2/tests/latin1/
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      259 2019-10-20 12:14:41.000000 ydiff-1.2/tests/latin1/out.normal
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      600 2019-10-20 12:14:41.000000 ydiff-1.2/tests/latin1/out.w70
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      630 2019-10-20 12:14:41.000000 ydiff-1.2/tests/latin1/out.side-by-side
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      176 2019-10-20 12:14:41.000000 ydiff-1.2/tests/latin1/in.diff
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      666 2019-10-20 12:14:41.000000 ydiff-1.2/tests/latin1/out.w70.wrap
-drwxrwxr-x   0 ymattw    (1001) ymattw    (1003)        0 2020-08-08 10:40:44.000000 ydiff-1.2/tests/git-perm/
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      196 2019-10-20 12:14:41.000000 ydiff-1.2/tests/git-perm/out.normal
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      196 2019-10-20 12:14:41.000000 ydiff-1.2/tests/git-perm/out.w70
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      196 2019-10-20 12:14:41.000000 ydiff-1.2/tests/git-perm/out.side-by-side
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      124 2019-10-20 12:14:41.000000 ydiff-1.2/tests/git-perm/in.diff
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)      196 2019-10-20 12:14:41.000000 ydiff-1.2/tests/git-perm/out.w70.wrap
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     3886 2020-08-08 10:15:17.000000 ydiff-1.2/CHANGES.rst
--rwxrwxr-x   0 ymattw    (1001) ymattw    (1003)      127 2019-10-20 12:14:41.000000 ydiff-1.2/ydiff
--rwxrwxr-x   0 ymattw    (1001) ymattw    (1003)    34532 2020-08-08 09:56:57.000000 ydiff-1.2/ydiff.py
--rw-rw-r--   0 ymattw    (1001) ymattw    (1003)     8008 2020-08-08 09:57:32.000000 ydiff-1.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.386186 ydiff-1.3/
+-rw-rw-r--   0 root         (0) root         (0)     4159 2024-04-02 09:09:22.000000 ydiff-1.3/CHANGES.rst
+-rw-rw-r--   0 root         (0) root         (0)     1584 2022-09-10 09:28:40.000000 ydiff-1.3/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      106 2022-09-10 09:28:40.000000 ydiff-1.3/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)     1399 2024-04-02 08:00:52.000000 ydiff-1.3/Makefile
+-rw-r--r--   0 root         (0) root         (0)    12805 2024-04-02 09:10:59.386186 ydiff-1.3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     7861 2024-04-02 08:59:17.000000 ydiff-1.3/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 09:10:59.386186 ydiff-1.3/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1284 2024-04-02 07:39:48.000000 ydiff-1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.314185 ydiff-1.3/tests/
+-rw-rw-r--   0 root         (0) root         (0)      350 2022-10-05 10:28:51.000000 ydiff-1.3/tests/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.314185 ydiff-1.3/tests/crlf/
+-rw-rw-r--   0 root         (0) root         (0)     1041 2022-09-10 09:28:40.000000 ydiff-1.3/tests/crlf/in.diff
+-rw-rw-r--   0 root         (0) root         (0)     1358 2022-09-10 09:28:40.000000 ydiff-1.3/tests/crlf/out.normal
+-rw-rw-r--   0 root         (0) root         (0)     3744 2022-09-10 09:28:40.000000 ydiff-1.3/tests/crlf/out.side-by-side
+-rw-rw-r--   0 root         (0) root         (0)     3580 2022-09-10 09:28:40.000000 ydiff-1.3/tests/crlf/out.w70
+-rw-rw-r--   0 root         (0) root         (0)     4151 2022-09-10 09:28:40.000000 ydiff-1.3/tests/crlf/out.w70.wrap
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.318184 ydiff-1.3/tests/diff-of-diff/
+-rw-rw-r--   0 root         (0) root         (0)     1141 2022-09-10 09:28:40.000000 ydiff-1.3/tests/diff-of-diff/in.diff
+-rw-rw-r--   0 root         (0) root         (0)     1625 2022-09-10 09:28:40.000000 ydiff-1.3/tests/diff-of-diff/out.normal
+-rw-rw-r--   0 root         (0) root         (0)     4786 2022-09-10 09:28:40.000000 ydiff-1.3/tests/diff-of-diff/out.side-by-side
+-rw-rw-r--   0 root         (0) root         (0)     4506 2022-09-10 09:28:40.000000 ydiff-1.3/tests/diff-of-diff/out.w70
+-rw-rw-r--   0 root         (0) root         (0)     4506 2022-09-10 09:28:40.000000 ydiff-1.3/tests/diff-of-diff/out.w70.wrap
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.322185 ydiff-1.3/tests/diff-ru/
+-rw-rw-r--   0 root         (0) root         (0)      744 2022-09-10 09:28:40.000000 ydiff-1.3/tests/diff-ru/in.diff
+-rw-rw-r--   0 root         (0) root         (0)     1128 2022-09-10 09:28:40.000000 ydiff-1.3/tests/diff-ru/out.normal
+-rw-rw-r--   0 root         (0) root         (0)     1781 2022-09-10 09:28:40.000000 ydiff-1.3/tests/diff-ru/out.side-by-side
+-rw-rw-r--   0 root         (0) root         (0)     1726 2022-09-10 09:28:40.000000 ydiff-1.3/tests/diff-ru/out.w70
+-rw-rw-r--   0 root         (0) root         (0)     1896 2022-09-10 09:28:40.000000 ydiff-1.3/tests/diff-ru/out.w70.wrap
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.322185 ydiff-1.3/tests/diff-ru-bin/
+-rw-rw-r--   0 root         (0) root         (0)      708 2022-09-10 09:28:40.000000 ydiff-1.3/tests/diff-ru-bin/in.diff
+-rw-rw-r--   0 root         (0) root         (0)     1019 2022-09-10 09:28:40.000000 ydiff-1.3/tests/diff-ru-bin/out.normal
+-rw-rw-r--   0 root         (0) root         (0)     1786 2022-09-10 09:28:40.000000 ydiff-1.3/tests/diff-ru-bin/out.side-by-side
+-rw-rw-r--   0 root         (0) root         (0)     1721 2022-09-10 09:28:40.000000 ydiff-1.3/tests/diff-ru-bin/out.w70
+-rw-rw-r--   0 root         (0) root         (0)     1891 2022-09-10 09:28:40.000000 ydiff-1.3/tests/diff-ru-bin/out.w70.wrap
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.322185 ydiff-1.3/tests/evil-udiff/
+-rw-rw-r--   0 root         (0) root         (0)      423 2022-09-10 09:28:40.000000 ydiff-1.3/tests/evil-udiff/in.diff
+-rw-rw-r--   0 root         (0) root         (0)      710 2022-09-10 09:28:40.000000 ydiff-1.3/tests/evil-udiff/out.normal
+-rw-rw-r--   0 root         (0) root         (0)     1934 2022-09-10 09:28:40.000000 ydiff-1.3/tests/evil-udiff/out.side-by-side
+-rw-rw-r--   0 root         (0) root         (0)     1814 2022-09-10 09:28:40.000000 ydiff-1.3/tests/evil-udiff/out.w70
+-rw-rw-r--   0 root         (0) root         (0)     1814 2022-09-10 09:28:40.000000 ydiff-1.3/tests/evil-udiff/out.w70.wrap
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.322185 ydiff-1.3/tests/git/
+-rw-rw-r--   0 root         (0) root         (0)     1683 2022-09-10 09:28:40.000000 ydiff-1.3/tests/git/in.diff
+-rw-rw-r--   0 root         (0) root         (0)     2308 2022-09-10 09:28:40.000000 ydiff-1.3/tests/git/out.normal
+-rw-rw-r--   0 root         (0) root         (0)     5012 2022-09-10 09:28:40.000000 ydiff-1.3/tests/git/out.side-by-side
+-rw-rw-r--   0 root         (0) root         (0)     4771 2022-09-10 09:28:40.000000 ydiff-1.3/tests/git/out.w70
+-rw-rw-r--   0 root         (0) root         (0)     5265 2022-09-10 09:28:40.000000 ydiff-1.3/tests/git/out.w70.wrap
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.326185 ydiff-1.3/tests/git-bin/
+-rw-rw-r--   0 root         (0) root         (0)      633 2022-09-10 09:28:40.000000 ydiff-1.3/tests/git-bin/in.diff
+-rw-rw-r--   0 root         (0) root         (0)      957 2022-09-10 09:28:40.000000 ydiff-1.3/tests/git-bin/out.normal
+-rw-rw-r--   0 root         (0) root         (0)     1914 2022-09-10 09:28:40.000000 ydiff-1.3/tests/git-bin/out.side-by-side
+-rw-rw-r--   0 root         (0) root         (0)     1830 2022-09-10 09:28:40.000000 ydiff-1.3/tests/git-bin/out.w70
+-rw-rw-r--   0 root         (0) root         (0)     1924 2022-09-10 09:28:40.000000 ydiff-1.3/tests/git-bin/out.w70.wrap
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.326185 ydiff-1.3/tests/git-log/
+-rw-rw-r--   0 root         (0) root         (0)      972 2022-09-10 09:28:40.000000 ydiff-1.3/tests/git-log/in.diff
+-rw-rw-r--   0 root         (0) root         (0)     1308 2022-09-10 09:28:40.000000 ydiff-1.3/tests/git-log/out.normal
+-rw-rw-r--   0 root         (0) root         (0)     2558 2022-09-10 09:28:40.000000 ydiff-1.3/tests/git-log/out.side-by-side
+-rw-rw-r--   0 root         (0) root         (0)     2466 2022-09-10 09:28:40.000000 ydiff-1.3/tests/git-log/out.w70
+-rw-rw-r--   0 root         (0) root         (0)     2800 2022-09-10 09:28:40.000000 ydiff-1.3/tests/git-log/out.w70.wrap
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.326185 ydiff-1.3/tests/git-perm/
+-rw-rw-r--   0 root         (0) root         (0)      124 2022-09-10 09:28:40.000000 ydiff-1.3/tests/git-perm/in.diff
+-rw-rw-r--   0 root         (0) root         (0)      196 2022-09-10 09:28:40.000000 ydiff-1.3/tests/git-perm/out.normal
+-rw-rw-r--   0 root         (0) root         (0)      196 2022-09-10 09:28:40.000000 ydiff-1.3/tests/git-perm/out.side-by-side
+-rw-rw-r--   0 root         (0) root         (0)      196 2022-09-10 09:28:40.000000 ydiff-1.3/tests/git-perm/out.w70
+-rw-rw-r--   0 root         (0) root         (0)      196 2022-09-10 09:28:40.000000 ydiff-1.3/tests/git-perm/out.w70.wrap
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.326185 ydiff-1.3/tests/hg-log/
+-rw-rw-r--   0 root         (0) root         (0)     2085 2022-09-10 09:28:40.000000 ydiff-1.3/tests/hg-log/in.diff
+-rw-rw-r--   0 root         (0) root         (0)     2662 2022-09-10 09:28:40.000000 ydiff-1.3/tests/hg-log/out.normal
+-rw-rw-r--   0 root         (0) root         (0)     5883 2022-09-10 09:28:40.000000 ydiff-1.3/tests/hg-log/out.side-by-side
+-rw-rw-r--   0 root         (0) root         (0)     5593 2022-09-10 09:28:40.000000 ydiff-1.3/tests/hg-log/out.w70
+-rw-rw-r--   0 root         (0) root         (0)     5593 2022-09-10 09:28:40.000000 ydiff-1.3/tests/hg-log/out.w70.wrap
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.326185 ydiff-1.3/tests/large-hunk/
+-rw-rw-r--   0 root         (0) root         (0)    86485 2022-09-10 09:28:40.000000 ydiff-1.3/tests/large-hunk/tao.diff
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.330185 ydiff-1.3/tests/latin1/
+-rw-rw-r--   0 root         (0) root         (0)      176 2022-09-10 09:28:40.000000 ydiff-1.3/tests/latin1/in.diff
+-rw-rw-r--   0 root         (0) root         (0)      259 2022-09-10 09:28:40.000000 ydiff-1.3/tests/latin1/out.normal
+-rw-rw-r--   0 root         (0) root         (0)      630 2022-09-10 09:28:40.000000 ydiff-1.3/tests/latin1/out.side-by-side
+-rw-rw-r--   0 root         (0) root         (0)      600 2022-09-10 09:28:40.000000 ydiff-1.3/tests/latin1/out.w70
+-rw-rw-r--   0 root         (0) root         (0)      666 2022-09-10 09:28:40.000000 ydiff-1.3/tests/latin1/out.w70.wrap
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.330185 ydiff-1.3/tests/perforce/
+-rw-rw-r--   0 root         (0) root         (0)     1824 2022-09-10 09:28:40.000000 ydiff-1.3/tests/perforce/in.diff
+-rw-rw-r--   0 root         (0) root         (0)     2656 2022-09-10 09:28:40.000000 ydiff-1.3/tests/perforce/out.normal
+-rw-rw-r--   0 root         (0) root         (0)     5745 2022-09-10 09:28:40.000000 ydiff-1.3/tests/perforce/out.side-by-side
+-rw-rw-r--   0 root         (0) root         (0)     5458 2022-09-10 09:28:40.000000 ydiff-1.3/tests/perforce/out.w70
+-rw-rw-r--   0 root         (0) root         (0)     5752 2022-09-10 09:28:40.000000 ydiff-1.3/tests/perforce/out.w70.wrap
+-rwxrwxr-x   0 root         (0) root         (0)      561 2024-03-30 15:41:43.000000 ydiff-1.3/tests/profile.sh
+-rwxrwxr-x   0 root         (0) root         (0)     1938 2024-03-30 15:41:46.000000 ydiff-1.3/tests/regression.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.330185 ydiff-1.3/tests/strange/
+-rw-rw-r--   0 root         (0) root         (0)      456 2022-09-10 09:28:40.000000 ydiff-1.3/tests/strange/in.diff
+-rw-rw-r--   0 root         (0) root         (0)      639 2022-09-10 09:28:40.000000 ydiff-1.3/tests/strange/out.normal
+-rw-rw-r--   0 root         (0) root         (0)      967 2022-09-10 09:28:40.000000 ydiff-1.3/tests/strange/out.side-by-side
+-rw-rw-r--   0 root         (0) root         (0)      937 2022-09-10 09:28:40.000000 ydiff-1.3/tests/strange/out.w70
+-rw-rw-r--   0 root         (0) root         (0)      937 2022-09-10 09:28:40.000000 ydiff-1.3/tests/strange/out.w70.wrap
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.330185 ydiff-1.3/tests/svn/
+-rw-rw-r--   0 root         (0) root         (0)     1039 2022-09-10 09:28:40.000000 ydiff-1.3/tests/svn/in.diff
+-rw-rw-r--   0 root         (0) root         (0)     1328 2022-09-10 09:28:40.000000 ydiff-1.3/tests/svn/out.normal
+-rw-rw-r--   0 root         (0) root         (0)     3737 2022-09-10 09:28:40.000000 ydiff-1.3/tests/svn/out.side-by-side
+-rw-rw-r--   0 root         (0) root         (0)     3573 2022-09-10 09:28:40.000000 ydiff-1.3/tests/svn/out.w70
+-rw-rw-r--   0 root         (0) root         (0)     4144 2022-09-10 09:28:40.000000 ydiff-1.3/tests/svn/out.w70.wrap
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.334185 ydiff-1.3/tests/svn-log/
+-rw-rw-r--   0 root         (0) root         (0)     1480 2022-09-10 09:28:40.000000 ydiff-1.3/tests/svn-log/in.diff
+-rw-rw-r--   0 root         (0) root         (0)     1928 2022-09-10 09:28:40.000000 ydiff-1.3/tests/svn-log/out.normal
+-rw-rw-r--   0 root         (0) root         (0)     3539 2022-09-10 09:28:40.000000 ydiff-1.3/tests/svn-log/out.side-by-side
+-rw-rw-r--   0 root         (0) root         (0)     3389 2022-09-10 09:28:40.000000 ydiff-1.3/tests/svn-log/out.w70
+-rw-rw-r--   0 root         (0) root         (0)     3389 2022-09-10 09:28:40.000000 ydiff-1.3/tests/svn-log/out.w70.wrap
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.382186 ydiff-1.3/tests/svn-merge/
+-rw-rw-r--   0 root         (0) root         (0)      326 2022-09-10 09:28:40.000000 ydiff-1.3/tests/svn-merge/in.diff
+-rw-rw-r--   0 root         (0) root         (0)      434 2022-09-10 09:28:40.000000 ydiff-1.3/tests/svn-merge/out.normal
+-rw-rw-r--   0 root         (0) root         (0)      434 2022-09-10 09:28:40.000000 ydiff-1.3/tests/svn-merge/out.side-by-side
+-rw-rw-r--   0 root         (0) root         (0)      434 2022-09-10 09:28:40.000000 ydiff-1.3/tests/svn-merge/out.w70
+-rw-rw-r--   0 root         (0) root         (0)      434 2022-09-10 09:28:40.000000 ydiff-1.3/tests/svn-merge/out.w70.wrap
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.382186 ydiff-1.3/tests/svn-property/
+-rw-rw-r--   0 root         (0) root         (0)      166 2022-09-10 09:28:40.000000 ydiff-1.3/tests/svn-property/in.diff
+-rw-rw-r--   0 root         (0) root         (0)      220 2022-09-10 09:28:40.000000 ydiff-1.3/tests/svn-property/out.normal
+-rw-rw-r--   0 root         (0) root         (0)      220 2022-09-10 09:28:40.000000 ydiff-1.3/tests/svn-property/out.side-by-side
+-rw-rw-r--   0 root         (0) root         (0)      220 2022-09-10 09:28:40.000000 ydiff-1.3/tests/svn-property/out.w70
+-rw-rw-r--   0 root         (0) root         (0)      220 2022-09-10 09:28:40.000000 ydiff-1.3/tests/svn-property/out.w70.wrap
+-rwxrwxr-x   0 root         (0) root         (0)    24304 2024-03-30 15:42:01.000000 ydiff-1.3/tests/test_ydiff.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.382186 ydiff-1.3/tests/wide-chars/
+-rw-rw-r--   0 root         (0) root         (0)      271 2022-10-05 10:31:18.000000 ydiff-1.3/tests/wide-chars/in.diff
+-rw-rw-r--   0 root         (0) root         (0)      424 2022-10-05 10:31:18.000000 ydiff-1.3/tests/wide-chars/out.normal
+-rw-rw-r--   0 root         (0) root         (0)      908 2022-10-05 10:31:18.000000 ydiff-1.3/tests/wide-chars/out.side-by-side
+-rw-rw-r--   0 root         (0) root         (0)      868 2022-10-05 10:31:18.000000 ydiff-1.3/tests/wide-chars/out.w70
+-rw-rw-r--   0 root         (0) root         (0)      965 2022-10-05 10:31:18.000000 ydiff-1.3/tests/wide-chars/out.w70.wrap
+-rwxrwxr-x   0 root         (0) root         (0)      128 2024-03-30 15:40:59.000000 ydiff-1.3/ydiff
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 09:10:59.382186 ydiff-1.3/ydiff.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12805 2024-04-02 09:10:59.000000 ydiff-1.3/ydiff.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2628 2024-04-02 09:10:59.000000 ydiff-1.3/ydiff.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 09:10:59.000000 ydiff-1.3/ydiff.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-02 09:10:59.000000 ydiff-1.3/ydiff.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)    29765 2024-04-02 09:03:47.000000 ydiff-1.3/ydiff.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ydiff-1.2/PKG-INFO` & `ydiff-1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,405 +1,407 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: ydiff
-Version: 1.2
+Version: 1.3
 Summary: View colored, incremental diff in a workspace or from stdin, with side by side and auto pager support
 Home-page: https://github.com/ymattw/ydiff
 Author: Matt Wang
-Author-email: mattwyl@gmail.com
 License: BSD-3
-Description: Ydiff
-        =====
-        
-        .. image:: https://travis-ci.org/ymattw/ydiff.png?branch=master
-           :target: https://travis-ci.org/ymattw/ydiff
-           :alt: Build status
-        
-        Term based tool to view *colored*, *incremental* diff in a version controlled
-        workspace (supports Git, Mercurial, Perforce and Svn so far) or from stdin,
-        with *side by side* (similar to ``diff -y``) and *auto pager* support. Requires
-        python (>= 2.5.0) and ``less``.
-        
-        .. image:: https://raw.github.com/ymattw/ydiff/gh-pages/img/default.png
-           :alt: default
-           :align: center
-        
-        .. image:: https://raw.github.com/ymattw/ydiff/gh-pages/img/side-by-side.png
-           :alt: side by side
-           :align: center
-           :width: 900 px
-        
-        Installation
-        ------------
-        
-        Install with pip
-        ~~~~~~~~~~~~~~~~
-        
-        Ydiff is already listed on `PyPI`_, you can install with ``pip`` if you have
-        the tool.
-        
-        .. _PyPI: http://pypi.python.org/pypi/ydiff
-        
-        .. code-block:: bash
-        
-            pip install --upgrade ydiff
-        
-        Install with setup.py
-        ~~~~~~~~~~~~~~~~~~~~~
-        
-        You can also run the setup.py from the source if you don't have ``pip``.
-        
-        .. code-block:: bash
-        
-            git clone https://github.com/ymattw/ydiff.git
-            cd ydiff
-            ./setup.py install
-        
-        Install with Homebrew
-        ~~~~~~~~~~~~~~~~~~~~~
-        
-        You can also install with Homebrew on Mac. (Thanks to `@josa42`_,
-        `@bfontaine`_, `@hivehand`_ and `@nijikon`_ for contributing to the Homebrew
-        `Formula`_).
-        
-        .. _`@josa42`: https://github.com/josa42
-        .. _`@bfontaine`: https://github.com/bfontaine
-        .. _`@hivehand`: https://github.com/hivehand
-        .. _`@nijikon`: https://github.com/nijikon
-        .. _`Formula`: https://github.com/Homebrew/homebrew-core/blob/master/Formula/ydiff.rb
-        
-        .. code-block:: bash
-        
-            brew install ydiff
-        
-        
-        Install on Fedora
-        ~~~~~~~~~~~~~~~~~
-        
-        On Fedora, you can install ydiff with dnf.
-        
-        .. code-block:: bash
-        
-            dnf install ydiff
-        
-        Install on FreeBSD
-        ~~~~~~~~~~~~~~~~~~
-        
-        On FreeBSD, you can install ydiff with pkg.
-        
-        .. code-block:: bash
-        
-            pkg install ydiff
-        
-        Download directly
-        ~~~~~~~~~~~~~~~~~
-        
-        Just save `ydiff.py`_ to whatever directory which is in your ``$PATH``, for
-        example, ``$HOME/bin`` is in my ``$PATH``, so I save the script there and name
-        as ``ydiff``.
-        
-        .. _`ydiff.py`: https://raw.github.com/ymattw/ydiff/master/ydiff.py
-        
-        .. code-block:: bash
-        
-            curl -ksSL https://raw.github.com/ymattw/ydiff/master/ydiff.py > ~/bin/ydiff
-            chmod +x ~/bin/ydiff
-        
-        Usage
-        -----
-        
-        Type ``ydiff -h`` to show usage::
-        
-            $ ydiff -h
-            Usage: ydiff [options] [file|dir ...]
-        
-            View colored, incremental diff in a workspace or from stdin, with side by side
-            and auto pager support
-        
-            Options:
-              --version            show program's version number and exit
-              -h, --help           show this help message and exit
-              -s, --side-by-side   enable side-by-side mode
-              -w N, --width=N      set text width for side-by-side mode, 0 for auto
-                                   detection, default is 80
-              -l, --log            show log with changes from revision control
-              -c M, --color=M      colorize mode 'auto' (default), 'always', or 'never'
-              -t N, --tab-width=N  convert tab characters to this many spaces (default: 8)
-              --wrap               wrap long lines in side-by-side view
-              -p M, --pager=M      pager application, suggested values are 'less' or 'cat'
-              -o M, --pager-options=M
-                                   options to supply to pager application
-        
-              Note:
-                Option parser will stop on first unknown option and pass them down to
-                underneath revision control. Environment variable YDIFF_OPTIONS may be
-                used to specify default options that will be placed at the beginning
-                of the argument list.
-        
-        Read diff from local modification in a *Git/Mercurial/Perforce/Svn* workspace
-        (output from e.g. ``git diff``, ``svn diff``):
-        
-        .. code-block:: bash
-        
-            cd proj-workspace
-            ydiff                         # view colored incremental diff
-            ydiff -s                      # view side by side, use default text width 80
-            ydiff -s -w 90                # use text width 90 other than default 80
-            ydiff -s -w 0                 # auto set text width based on terminal size
-            ydiff -s -w 0 --wrap          # same as before, but also wrap long lines
-            ydiff -s file1 dir2           # view modification of given files/dirs only
-            ydiff -s -w90 --wrap -- -U10  # pass '-U10' to underneath revision diff tool
-            ydiff -s -w90 --wrap -U10     # '--' is optional as it's unknown to ydiff
-            ydiff -s --cached             # show git staged diff (git diff --cached)
-            ydiff -s -r1234               # show svn diff to revision 1234
-        
-        Read log with changes in a *Git/Mercurial/Svn* workspace (output from e.g.
-        ``git log -p``, ``svn log --diff``), note *--diff* option is new in svn 1.7.0:
-        
-        .. code-block:: bash
-        
-            cd proj-workspace
-            ydiff -l                    # read log along with changes
-            ydiff -ls                   # equivalent to ydiff -l -s, view side by side
-            ydiff -ls -w90 --wrap       # set text width 90 and enable wrapping as well
-            ydiff -ls file1 dir2        # see log with changes of given files/dirs only
-        
-        Utilize a specific pager application:
-        
-        .. code-block:: bash
-        
-            ydiff                           # default pager - less
-            LESS_OPTS='-FRSX --shift 1'
-            ydiff -p less -o "${LESS_OPTS}" # emulate default pager
-            ydiff -p /usr/bin/less          # custom pager
-            ydiff -p cat                    # non-paging ANSI processor for colorizing
-        
-        Pipe in a diff:
-        
-        .. code-block:: bash
-        
-            git log -p -2 | ydiff       # view git log with changes of last 2 commits
-            git show 15bfa | ydiff -s   # view a given git commit, side by side
-            svn diff -r1234 | ydiff -s  # view svn diff comparing to given revision
-            diff -u file1 file2 | ydiff # view diff between two files (note the '-u')
-            diff -ur dir1 dir2 | ydiff  # view diff between two dirs
-        
-            # View diff in a GitHub pull request, side by side
-            curl https://github.com/ymattw/ydiff/pull/11.diff | ydiff -s
-        
-            # View a patch file in unified or context format, the latter depends on
-            # command `filterdiff` from package `patchutils` which is available in
-            # major Linux distros and MacPorts.
-            #
-            ydiff -s < foo.patch
-        
-        Redirect output to another patch file is safe:
-        
-        .. code-block:: bash
-        
-            svn diff -r PREV | ydiff -s > my.patch
-        
-        Environment variable
-        --------------------
-        
-        Environment variable ``YDIFF_OPTIONS`` may be used to specify default options
-        that will be placed at the beginning of the argument list, for example:
-        
-        .. code-block:: bash
-        
-            export YDIFF_OPTIONS='-s -w0 --wrap'
-            ydiff foo                   # equivalent to "ydiff -s -w0 --wrap foo"
-        
-        Note the default pager ``less`` takes options from the environment variable
-        ``LESS``.
-        
-        Notes
-        -----
-        
-        If you feel more comfortable with a command such as ``git ydiff`` to trigger
-        the ydiff command, you may symlink the executable to one named ``git-ydiff``
-        as follows:
-        
-        .. code-block:: bash
-        
-            ydiff_dir=$(dirname $(which ydiff))
-            ln -s "${ydiff_dir}/ydiff" "${ydiff_dir}/git-ydiff"
-        
-        Known issues
-        ------------
-        
-        Ydiff has following known issues:
-        
-        - Does not recognize `normal` diff, and depends on ``filterdiff`` (patchutils)
-          to read `context` diff
-        - Side by side mode has alignment problem for wide chars
-        - Terminal might be in a mess on exception (type ``reset`` can fix it)
-        
-        Pull requests are very welcome, please make sure your changes can pass unit
-        tests and regression tests by run ``make test`` (required tool *coverage* can
-        be installed with ``pip install coverage``).  Also watch out `travis build`_
-        after push, make sure it passes as well.
-        
-        .. _`travis build`: https://travis-ci.org/ymattw/ydiff/pull_requests
-        
-        See also
-        --------
-        
-        I have another tool `coderev`_ which generates side-by-side diff pages for code
-        review from two given files or directories, I found it's not easy to extend to
-        support git so invented `ydiff`.  Idea of ansi color markup is also from
-        project `colordiff`_.
-        
-        .. _coderev: https://github.com/ymattw/coderev
-        .. _colordiff: https://github.com/daveewart/colordiff
-        
-        .. vim:set ft=rst et sw=4 sts=4 tw=79:
-        
-        Change log
-        ==========
-        
-        Version 1.2 (2020-08-08)
-        
-          - Support perforce workspaces
-          - Support pager customization via --pager and --pager_options
-          - Support running on Windows (requires ``less`` which is offered by git-bash)
-          - Fix a bug where reading stdin does not work outside a CVS workspace
-          - Fix tab expansion, expands to the next stop modulo tab width
-          - Performance improvement
-        
-        Version 1.1 (2018-06-05)
-        
-          - Rename from ``cdiff`` to ``ydiff`` to avoid binary name conflict on major
-            distributions, ``CDIFF_OPTIONS`` still works but will be deprepated soon
-          - New option ``--wrap`` to wrap long lines in side-by-side view
-        
-        Version 1.0 (2016-12-31)
-        
-          - Use environment variable ``CDIFF_OPTIONS`` to hold default options
-        
-        Version 0.9.8 (2016-01-16)
-        
-          - More robust parser to tolerate evil unified diff
-        
-        Version 0.9.7 (2015-04-24)
-        
-          - Fix unexpected side-by-side output for diff of diff
-          - Better color to work with solarized color scheme
-        
-        Version 0.9.6 (2014-06-20)
-        
-          - Fix TypeError exception in auto width logic
-        
-        Version 0.9.5 (2014-06-19)
-        
-          - Option ``--width 0`` now fits terminal size automatically
-          - Enable smooth horizontal scrolling with less option ``--shift 1``
-        
-        Version 0.9.4 (2014-06-04)
-        
-          - Respect the ``LESS`` environment variable
-          - Support python 3.4
-          - Fix curl options in document
-        
-        Version 0.9.3 (2013-09-28)
-        
-          - Moved screenshots to 'gh-pages' branch
-          - Handle all keyboard interrupts more completely
-          - Explicitly set default encoding to utf-8
-          - Fixed broken output diff when I/O with filterdiff in nonblocking mode
-        
-        Version 0.9.2 (2013-06-21)
-        
-          - Enahanced option parser now pass unknown option to underneath revision
-            control, user can use ``cdiff --cached``, ``cdiff -U5`` directly
-        
-        Version 0.9.1 (2013-05-20)
-        
-          - Use ``--no-ext-diff`` to disable GIT_EXTERNAL_DIFF and diff.external which
-            might break cdiff output
-        
-        Version 0.9 (2013-03-23)
-        
-          - Supports reading context diff via ``filterdiff`` (patchutils)
-          - Fixed a diff parser bug which misread git commit message as common line
-          - Lots of code refactor
-        
-        Version 0.8 (2013-03-13)
-        
-          - Parser is now robust enough to handle dangling headers and short patch
-          - PEP8 (with minor own flavors) and other code lint
-          - Change 'Development Status' to stable
-        
-        Version 0.7.1 (2013-02-25)
-        
-          - Handle 'Binary files ... differ'
-          - Document update for known issues
-        
-        Version 0.7 (2013-02-23)
-        
-          - Support reading diff or log for given files/dirs in workspace
-          - Support diff generated from ``diff -ru dir1 dir2``
-          - Usage change: reading a patch and comparing two files need stdin redirect
-        
-        Version 0.6 (2013-02-20)
-        
-          - A few performance tuning and code clean up
-          - Add unit test cases with coverage 70%
-          - Show merge history in svn log
-        
-        Version 0.5.1 (2013-02-19)
-        
-          - Fixed incorrect yield on diff missing eof
-          - Fixed a bug in diff format probe
-          - Handle keyboard interrupt and large diffs in non-color mode
-          - Code clean up
-        
-        Version 0.5 (2013-02-18)
-        
-          - Support read output from ``svn diff --log`` and ``hg log -p``
-          - Streamline reading large patch set
-          - New ``--log (-l)`` option to read revision control diff log (thanks to
-            `Steven Myint`_)
-        
-        Version 0.4 (2013-02-16)
-        
-          - New option *-c WHEN* (*--color WHEN*) to support auto test
-          - Auto regression test now on Travis
-        
-        Version 0.3 (2013-02-07)
-        
-          - Support compare two files (wrapper of diff)
-        
-        Version 0.2 (2013-02-06)
-        
-          - Move cdiff.py to top dir for better meta info management
-        
-        Version 0.1 (2013-02-05)
-        
-          - New --version option
-          - setup.py now read version from source code
-        
-        Version 0.0.4 (2013-02-04)
-        
-          - Add CHANGES for history track and better versioning
-        
-        Version 0.0.3 (2013-02-04)
-        
-          - Publish on PyPI, supports read patch from file, pipe and diff output from
-            revision tools (thanks to `Steven Myint`_)
-        
-        .. _Steven Myint: https://github.com/myint
-        
-        .. vim:set ft=rst et sw=4 sts=4 tw=79:
-        
 Keywords: colored incremental side-by-side diff
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+
+Ydiff
+=====
+
+.. image:: https://github.com/ymattw/ydiff/actions/workflows/test.yml/badge.svg
+   :alt: Tests status
+   :target: https://github.com/ymattw/ydiff/actions
+
+Term based tool to view *colored*, *incremental* diff in a version controlled
+workspace (supports Git, Mercurial, Perforce and Svn so far) or from stdin,
+with *side by side* (similar to ``diff -y``) and *auto pager* support. Requires
+python (>= 2.6.0) and ``less``.
+
+.. image:: https://raw.github.com/ymattw/ydiff/gh-pages/img/default.png
+   :alt: default
+   :align: center
+
+.. image:: https://raw.github.com/ymattw/ydiff/gh-pages/img/side-by-side.png
+   :alt: side by side
+   :align: center
+   :width: 900 px
+
+Ydiff only supports diff in `Unified Format`_. This is default in most version
+control system except Perforce, which needs an environment variable
+``P4DIFF="diff -u"`` to output unified diff.
+
+.. _`Unified Format`: https://en.wikipedia.org/wiki/Diff#Unified_format
+
+Installation
+------------
+
+Ydiff only depends on Python built-in libraries, so you can just download the
+source and run without worrying about any installation.
+
+Git tagged `releases`_ will be packaged and uploaded to PyPI timely, however,
+packages hosted elsewhere are not (please note they are not managed by the
+author `@ymattw`_).
+
+.. _`@ymattw`: https://github.com/ymattw
+.. _`releases`: https://github.com/ymattw/ydiff/releases
+
+Download directly
+~~~~~~~~~~~~~~~~~
+
+Just save `ydiff.py`_ to whatever directory which is in your ``$PATH``, for
+example, ``$HOME/bin`` is in my ``$PATH``, so I save the script there and name
+as ``ydiff``.
+
+.. _`ydiff.py`: https://raw.github.com/ymattw/ydiff/master/ydiff.py
+
+.. code-block:: bash
+
+    curl -ksSL https://raw.github.com/ymattw/ydiff/master/ydiff.py > ~/bin/ydiff
+    chmod +x ~/bin/ydiff
+
+Install with pip
+~~~~~~~~~~~~~~~~
+
+Ydiff is already listed on `PyPI`_, you can install with ``pip`` if you have
+the tool.
+
+.. _PyPI: http://pypi.python.org/pypi/ydiff
+
+.. code-block:: bash
+
+    pip install --upgrade ydiff
+
+Install with setup.py
+~~~~~~~~~~~~~~~~~~~~~
+
+You can also run the setup.py from the source if you don't have ``pip``.
+
+.. code-block:: bash
+
+    git clone https://github.com/ymattw/ydiff.git
+    cd ydiff
+    ./setup.py install
+
+Install with Homebrew
+~~~~~~~~~~~~~~~~~~~~~
+
+You can also install with Homebrew on Mac. (Thanks to `@josa42`_,
+`@bfontaine`_, `@hivehand`_ and `@nijikon`_ for contributing to the Homebrew
+`Formula`_).
+
+.. _`@josa42`: https://github.com/josa42
+.. _`@bfontaine`: https://github.com/bfontaine
+.. _`@hivehand`: https://github.com/hivehand
+.. _`@nijikon`: https://github.com/nijikon
+.. _`Formula`: https://github.com/Homebrew/homebrew-core/blob/master/Formula/y/ydiff.rb
+
+.. code-block:: bash
+
+    brew install ydiff
+
+
+Install on Fedora
+~~~~~~~~~~~~~~~~~
+
+On Fedora, you can install ydiff with dnf.
+
+.. code-block:: bash
+
+    dnf install ydiff
+
+Install on FreeBSD
+~~~~~~~~~~~~~~~~~~
+
+On FreeBSD, you can install ydiff with pkg.
+
+.. code-block:: bash
+
+    pkg install ydiff
+
+Usage
+-----
+
+Type ``ydiff -h`` to show usage::
+
+    $ ydiff -h
+    Usage: ydiff [options] [file|dir ...]
+
+    View colored, incremental diff in a workspace or from stdin, with side by side
+    and auto pager support
+
+    Options:
+      --version            show program's version number and exit
+      -h, --help           show this help message and exit
+      -s, --side-by-side   enable side-by-side mode
+      -w N, --width=N      set text width for side-by-side mode, 0 for auto
+                           detection, default is 80
+      -l, --log            show log with changes from revision control
+      -c M, --color=M      colorize mode 'auto' (default), 'always', or 'never'
+      -t N, --tab-width=N  convert tab characters to this many spaces (default: 8)
+      --wrap               wrap long lines in side-by-side view
+      -p M, --pager=M      pager application, suggested values are 'less' or 'cat'
+      -o M, --pager-options=M
+                           options to supply to pager application
+
+      Note:
+        Option parser will stop on first unknown option and pass them down to
+        underneath revision control. Environment variable YDIFF_OPTIONS may be
+        used to specify default options that will be placed at the beginning
+        of the argument list.
+
+Read diff from local modification in a *Git/Mercurial/Perforce/Svn* workspace
+(output from e.g. ``git diff``, ``svn diff``):
+
+.. code-block:: bash
+
+    cd proj-workspace
+    ydiff                         # view colored incremental diff
+    ydiff -s                      # view side by side, use default text width 80
+    ydiff -s -w 90                # use text width 90 other than default 80
+    ydiff -s -w 0                 # auto set text width based on terminal size
+    ydiff -s -w 0 --wrap          # same as before, but also wrap long lines
+    ydiff -s file1 dir2           # view modification of given files/dirs only
+    ydiff -s -w90 --wrap -- -U10  # pass '-U10' to underneath revision diff tool
+    ydiff -s -w90 --wrap -U10     # '--' is optional as it's unknown to ydiff
+    ydiff -s --cached             # show git staged diff (git diff --cached)
+    ydiff -s -r1234               # show svn diff to revision 1234
+
+Read log with changes in a *Git/Mercurial/Svn* workspace (output from e.g.
+``git log -p``, ``svn log --diff``), note *--diff* option is new in svn 1.7.0:
+
+.. code-block:: bash
+
+    cd proj-workspace
+    ydiff -l                    # read log along with changes
+    ydiff -ls                   # equivalent to ydiff -l -s, view side by side
+    ydiff -ls -w90 --wrap       # set text width 90 and enable wrapping as well
+    ydiff -ls file1 dir2        # see log with changes of given files/dirs only
+
+Utilize a specific pager application:
+
+.. code-block:: bash
+
+    ydiff                           # default pager - less
+    LESS_OPTS='-FRSX --shift 1'
+    ydiff -p less -o "${LESS_OPTS}" # emulate default pager
+    ydiff -p /usr/bin/less          # custom pager
+    ydiff -p cat                    # non-paging ANSI processor for colorizing
+
+Pipe in a diff:
+
+.. code-block:: bash
+
+    git log -p -2 | ydiff       # view git log with changes of last 2 commits
+    git show 15bfa | ydiff -s   # view a given git commit, side by side
+    svn diff -r1234 | ydiff -s  # view svn diff comparing to given revision
+    diff -u file1 file2 | ydiff # view diff between two files (note the '-u')
+    diff -ur dir1 dir2 | ydiff  # view diff between two dirs
+
+    # View diff in a GitHub pull request, side by side
+    curl https://github.com/ymattw/ydiff/pull/11.diff | ydiff -s
+
+    # View a patch file in unified format.
+    ydiff -s < foo.patch
+
+Redirect output to another patch file is safe:
+
+.. code-block:: bash
+
+    svn diff -r PREV | ydiff -s > my.patch
+
+Environment variable
+--------------------
+
+Environment variable ``YDIFF_OPTIONS`` may be used to specify default options
+that will be placed at the beginning of the argument list, for example:
+
+.. code-block:: bash
+
+    export YDIFF_OPTIONS='-s -w0 --wrap'
+    ydiff foo                   # equivalent to "ydiff -s -w0 --wrap foo"
+
+Note the default pager ``less`` takes options from the environment variable
+``LESS``.
+
+Notes
+-----
+
+If you feel more comfortable with a command such as ``git ydiff`` to trigger
+the ydiff command, you may symlink the executable to one named ``git-ydiff``
+as follows:
+
+.. code-block:: bash
+
+    ydiff_dir=$(dirname $(which ydiff))
+    ln -s "${ydiff_dir}/ydiff" "${ydiff_dir}/git-ydiff"
+
+Known issues
+------------
+
+Ydiff has following known issues:
+
+- Side by side mode has alignment problem for wide chars
+- Terminal might be in a mess on exception (type ``reset`` can fix it)
+
+Pull requests are very welcome, please make sure your changes can pass unit
+tests and regression tests by run ``make docker-test``.
+
+.. vim:set ft=rst et sw=4 sts=4 tw=79:
+
+Change log
+==========
+
+Version 1.3 (2024-04-02)
+
+  - Dropped context diff support
+  - Handle East Asian wide characters (thanks to @roy2220)
+  - Fix SIGPIPE issue on Windows (unofficial support, thanks to @kingsamchen)
+  - Bump Python requirement to >=2.6 (Python 2 support is no longer tested)
+
+Version 1.2 (2020-08-08)
+
+  - Support perforce workspaces
+  - Support pager customization via --pager and --pager_options
+  - Support running on Windows (requires ``less`` which is offered by git-bash)
+  - Fix a bug where reading stdin does not work outside a CVS workspace
+  - Fix tab expansion, expands to the next stop modulo tab width
+  - Performance improvement
+
+Version 1.1 (2018-06-05)
+
+  - Rename from ``cdiff`` to ``ydiff`` to avoid binary name conflict on major
+    distributions, ``CDIFF_OPTIONS`` still works but will be deprepated soon
+  - New option ``--wrap`` to wrap long lines in side-by-side view
+
+Version 1.0 (2016-12-31)
+
+  - Use environment variable ``CDIFF_OPTIONS`` to hold default options
+
+Version 0.9.8 (2016-01-16)
+
+  - More robust parser to tolerate evil unified diff
+
+Version 0.9.7 (2015-04-24)
+
+  - Fix unexpected side-by-side output for diff of diff
+  - Better color to work with solarized color scheme
+
+Version 0.9.6 (2014-06-20)
+
+  - Fix TypeError exception in auto width logic
+
+Version 0.9.5 (2014-06-19)
+
+  - Option ``--width 0`` now fits terminal size automatically
+  - Enable smooth horizontal scrolling with less option ``--shift 1``
+
+Version 0.9.4 (2014-06-04)
+
+  - Respect the ``LESS`` environment variable
+  - Support python 3.4
+  - Fix curl options in document
+
+Version 0.9.3 (2013-09-28)
+
+  - Moved screenshots to 'gh-pages' branch
+  - Handle all keyboard interrupts more completely
+  - Explicitly set default encoding to utf-8
+  - Fixed broken output diff when I/O with filterdiff in nonblocking mode
+
+Version 0.9.2 (2013-06-21)
+
+  - Enahanced option parser now pass unknown option to underneath revision
+    control, user can use ``cdiff --cached``, ``cdiff -U5`` directly
+
+Version 0.9.1 (2013-05-20)
+
+  - Use ``--no-ext-diff`` to disable GIT_EXTERNAL_DIFF and diff.external which
+    might break cdiff output
+
+Version 0.9 (2013-03-23)
+
+  - Supports reading context diff via ``filterdiff`` (patchutils)
+  - Fixed a diff parser bug which misread git commit message as common line
+  - Lots of code refactor
+
+Version 0.8 (2013-03-13)
+
+  - Parser is now robust enough to handle dangling headers and short patch
+  - PEP8 (with minor own flavors) and other code lint
+  - Change 'Development Status' to stable
+
+Version 0.7.1 (2013-02-25)
+
+  - Handle 'Binary files ... differ'
+  - Document update for known issues
+
+Version 0.7 (2013-02-23)
+
+  - Support reading diff or log for given files/dirs in workspace
+  - Support diff generated from ``diff -ru dir1 dir2``
+  - Usage change: reading a patch and comparing two files need stdin redirect
+
+Version 0.6 (2013-02-20)
+
+  - A few performance tuning and code clean up
+  - Add unit test cases with coverage 70%
+  - Show merge history in svn log
+
+Version 0.5.1 (2013-02-19)
+
+  - Fixed incorrect yield on diff missing eof
+  - Fixed a bug in diff format probe
+  - Handle keyboard interrupt and large diffs in non-color mode
+  - Code clean up
+
+Version 0.5 (2013-02-18)
+
+  - Support read output from ``svn diff --log`` and ``hg log -p``
+  - Streamline reading large patch set
+  - New ``--log (-l)`` option to read revision control diff log (thanks to
+    `Steven Myint`_)
+
+Version 0.4 (2013-02-16)
+
+  - New option *-c WHEN* (*--color WHEN*) to support auto test
+  - Auto regression test now on Travis
+
+Version 0.3 (2013-02-07)
+
+  - Support compare two files (wrapper of diff)
+
+Version 0.2 (2013-02-06)
+
+  - Move cdiff.py to top dir for better meta info management
+
+Version 0.1 (2013-02-05)
+
+  - New --version option
+  - setup.py now read version from source code
+
+Version 0.0.4 (2013-02-04)
+
+  - Add CHANGES for history track and better versioning
+
+Version 0.0.3 (2013-02-04)
+
+  - Publish on PyPI, supports read patch from file, pipe and diff output from
+    revision tools (thanks to `Steven Myint`_)
+
+.. _Steven Myint: https://github.com/myint
+
+.. vim:set ft=rst et sw=4 sts=4 tw=79:
```

### Comparing `ydiff-1.2/setup.py` & `ydiff-1.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from __future__ import with_statement
 import sys
 from distutils.core import setup
 from ydiff import META_INFO as _meta
 
-if sys.hexversion < 0x02050000:
-    raise SystemExit("*** Requires python >= 2.5.0")
+if sys.hexversion < 0x02060000:
+    raise SystemExit("*** Requires python >= 2.6.0")
 
 with open('README.rst') as doc:
     long_description = doc.read()
 with open('CHANGES.rst') as changes:
     long_description += changes.read()
 
 setup(
     name='ydiff',
     version=_meta['version'],
     author=_meta['author'],
-    author_email=_meta['email'].replace('(', '').replace(')', ''),
     license=_meta['license'],
     description=_meta['description'],
     long_description=long_description,
     keywords=_meta['keywords'],
     url=_meta['url'],
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
```

### Comparing `ydiff-1.2/LICENSE` & `ydiff-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/crlf/out.normal` & `ydiff-1.3/tests/crlf/out.normal`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/crlf/out.w70` & `ydiff-1.3/tests/crlf/out.w70`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/crlf/out.side-by-side` & `ydiff-1.3/tests/crlf/out.side-by-side`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/crlf/in.diff` & `ydiff-1.3/tests/crlf/in.diff`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/crlf/out.w70.wrap` & `ydiff-1.3/tests/crlf/out.w70.wrap`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/strange/out.normal` & `ydiff-1.3/tests/strange/out.normal`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/strange/out.w70` & `ydiff-1.3/tests/strange/out.w70`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/strange/out.side-by-side` & `ydiff-1.3/tests/strange/out.side-by-side`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/strange/out.w70.wrap` & `ydiff-1.3/tests/strange/out.w70.wrap`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/diff-of-diff/out.normal` & `ydiff-1.3/tests/diff-of-diff/out.normal`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/diff-of-diff/out.w70` & `ydiff-1.3/tests/diff-of-diff/out.w70`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/diff-of-diff/out.side-by-side` & `ydiff-1.3/tests/diff-of-diff/out.side-by-side`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/diff-of-diff/in.diff` & `ydiff-1.3/tests/diff-of-diff/in.diff`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/diff-of-diff/out.w70.wrap` & `ydiff-1.3/tests/diff-of-diff/out.w70.wrap`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/diff-ru-bin/out.normal` & `ydiff-1.3/tests/diff-ru-bin/out.normal`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/diff-ru-bin/out.w70` & `ydiff-1.3/tests/diff-ru-bin/out.w70`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/diff-ru-bin/out.side-by-side` & `ydiff-1.3/tests/diff-ru-bin/out.side-by-side`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/diff-ru-bin/in.diff` & `ydiff-1.3/tests/diff-ru-bin/in.diff`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/diff-ru-bin/out.w70.wrap` & `ydiff-1.3/tests/diff-ru-bin/out.w70.wrap`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/git/out.normal` & `ydiff-1.3/tests/git/out.normal`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/git/out.w70` & `ydiff-1.3/tests/git/out.w70`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/git/out.side-by-side` & `ydiff-1.3/tests/git/out.side-by-side`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/git/in.diff` & `ydiff-1.3/tests/git/in.diff`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/git/out.w70.wrap` & `ydiff-1.3/tests/git/out.w70.wrap`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/hg-log/out.normal` & `ydiff-1.3/tests/hg-log/out.normal`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/hg-log/out.w70` & `ydiff-1.3/tests/hg-log/out.w70`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/hg-log/out.side-by-side` & `ydiff-1.3/tests/hg-log/out.side-by-side`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/hg-log/in.diff` & `ydiff-1.3/tests/hg-log/in.diff`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/hg-log/out.w70.wrap` & `ydiff-1.3/tests/hg-log/out.w70.wrap`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/git-log/out.normal` & `ydiff-1.3/tests/git-log/out.normal`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/git-log/out.w70` & `ydiff-1.3/tests/git-log/out.w70`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/git-log/out.side-by-side` & `ydiff-1.3/tests/git-log/out.side-by-side`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/git-log/in.diff` & `ydiff-1.3/tests/git-log/in.diff`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/git-log/out.w70.wrap` & `ydiff-1.3/tests/git-log/out.w70.wrap`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/test_ydiff.py` & `ydiff-1.3/tests/test_ydiff.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,77 +1,22 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """Unit test for ydiff"""
 
 import sys
 import unittest
 import tempfile
 import subprocess
 import os
 
 sys.path.insert(0, '')
 import ydiff  # nopep8
 
 
-class Sequential(object):
-    """A non-seekable iterator, mock of file object"""
-
-    def __init__(self, items):
-        self._items = items
-        self._index = 0
-
-    def __iter__(self):
-        while True:
-            try:
-                item = self._items[self._index]
-            except IndexError:
-                raise StopIteration
-            yield item
-            self._index += 1
-
-    def readline(self):
-        try:
-            item = self._items[self._index]
-        except IndexError:
-            return ''
-        self._index += 1
-        return item
-
-
-class PatchStreamTest(unittest.TestCase):
-
-    def test_is_empty(self):
-        stream = ydiff.PatchStream(Sequential([]))
-        self.assertTrue(stream.is_empty())
-
-        stream = ydiff.PatchStream(Sequential(['hello', 'world']))
-        self.assertFalse(stream.is_empty())
-
-    def test_read_stream_header(self):
-        stream = ydiff.PatchStream(Sequential([]))
-        self.assertEqual(stream.read_stream_header(1), [])
-
-        items = ['hello', 'world', 'again']
-
-        stream = ydiff.PatchStream(Sequential(items))
-        self.assertEqual(stream.read_stream_header(2), items[:2])
-
-        stream = ydiff.PatchStream(Sequential(items))
-        self.assertEqual(stream.read_stream_header(4), items[:])
-
-    def test_iter_after_read_stream_header(self):
-        items = ['hello', 'world', 'again', 'and', 'again']
-        stream = ydiff.PatchStream(Sequential(items))
-
-        _ = stream.read_stream_header(2)
-        out = list(stream)
-        self.assertEqual(out, items)
-
-
 class DecodeTest(unittest.TestCase):
 
     def test_normal(self):
         utext = 'hello'.encode('utf-8')
         self.assertEqual('hello', ydiff.decode(utext))
 
     def test_latin_1(self):
@@ -506,80 +451,39 @@
 
     def test_is_new_neg(self):
         self.assertFalse(self.diff.is_new('+++ considered as new path'))
 
 
 class DiffParserTest(unittest.TestCase):
 
-    def test_type_detect_unified(self):
-        patch = """\
-spam
---- a
-+++ b
-@@ -1,2 +1,2 @@
-"""
-        items = patch.splitlines(True)
-        stream = ydiff.PatchStream(Sequential(items))
-        parser = ydiff.DiffParser(stream)
-        self.assertEqual(parser._type, 'unified')
-
-    @unittest.skipIf(os.name == 'nt', 'patchutils (filterdiff) unavailable')
-    def test_type_detect_context(self):
-        patch = """\
-*** /path/to/original timestamp
---- /path/to/new timestamp
-***************
-*** 1,1 ****
---- 1,2 ----
-+ This is an important
-  This part of the
-"""
-        items = patch.splitlines(True)
-        stream = ydiff.PatchStream(Sequential(items))
-        parser = ydiff.DiffParser(stream)
-        self.assertEqual(parser._type, 'context')
-
-    def test_type_detect_neg(self):
-        patch = """\
-spam
---- a
-spam
-+++ b
-
-"""
-        items = patch.splitlines(True)
-        stream = ydiff.PatchStream(Sequential(items))
-        parser = ydiff.DiffParser(stream)
-        self.assertEqual(parser._type, 'unified')
-
     def test_parse_invalid_hunk_meta(self):
         patch = """\
 spam
 --- a
 +++ b
 spam
 @@ -a,a +0 @@
 """
         items = patch.splitlines(True)
-        stream = ydiff.PatchStream(Sequential(items))
+        stream = iter(items)
         parser = ydiff.DiffParser(stream)
         self.assertRaises(RuntimeError, list, parser.get_diff_generator())
 
     def test_parse_dangling_header(self):
         patch = """\
 --- a
 +++ b
 @@ -1,2 +1,2 @@
 -foo
 +bar
  common
 spam
 """
         items = patch.splitlines(True)
-        stream = ydiff.PatchStream(Sequential(items))
+        stream = iter(items)
         parser = ydiff.DiffParser(stream)
 
         out = list(parser.get_diff_generator())
         self.assertEqual(len(out), 2)
         self.assertEqual(len(out[1]._headers), 1)
         self.assertEqual(out[1]._headers[0], 'spam\n')
         self.assertEqual(out[1]._old_path, '')
@@ -593,15 +497,15 @@
 @@ -1,2 +1,2 @@
 -foo
 +bar
  common
 --- c
 """
         items = patch.splitlines(True)
-        stream = ydiff.PatchStream(Sequential(items))
+        stream = iter(items)
         parser = ydiff.DiffParser(stream)
         self.assertRaises(AssertionError, list, parser.get_diff_generator())
 
     def test_parse_missing_hunk_meta(self):
         patch = """\
 --- a
 +++ b
@@ -609,15 +513,15 @@
 -foo
 +bar
  common
 --- c
 +++ d
 """
         items = patch.splitlines(True)
-        stream = ydiff.PatchStream(Sequential(items))
+        stream = iter(items)
         parser = ydiff.DiffParser(stream)
 
         out = list(parser.get_diff_generator())
         self.assertEqual(len(out), 2)
         self.assertEqual(len(out[1]._headers), 0)
         self.assertEqual(out[1]._old_path, '--- c\n')
         self.assertEqual(out[1]._new_path, '+++ d\n')
@@ -632,15 +536,15 @@
 +bar
  common
 --- c
 +++ d
 @@ -1,2 +1,2 @@
 """
         items = patch.splitlines(True)
-        stream = ydiff.PatchStream(Sequential(items))
+        stream = iter(items)
         parser = ydiff.DiffParser(stream)
         self.assertRaises(AssertionError, list, parser.get_diff_generator())
 
     def test_parse_only_in_dir(self):
         patch = """\
 --- a
 +++ b
@@ -653,15 +557,15 @@
 +++ d
 @@ -1,2 +1,2 @@
 -foo
 +bar
  common
 """
         items = patch.splitlines(True)
-        stream = ydiff.PatchStream(Sequential(items))
+        stream = iter(items)
         parser = ydiff.DiffParser(stream)
 
         out = list(parser.get_diff_generator())
         self.assertEqual(len(out), 3)
         self.assertEqual(len(out[1]._hunks), 0)
         self.assertEqual(out[1]._headers, ['Only in foo: foo\n'])
         self.assertEqual(len(out[2]._hunks), 1)
@@ -674,15 +578,15 @@
 @@ -1,2 +1,2 @@
 -foo
 +bar
  common
 Only in foo: foo
 """
         items = patch.splitlines(True)
-        stream = ydiff.PatchStream(Sequential(items))
+        stream = iter(items)
         parser = ydiff.DiffParser(stream)
 
         out = list(parser.get_diff_generator())
         self.assertEqual(len(out), 2)
         self.assertEqual(len(out[1]._hunks), 0)
         self.assertEqual(out[1]._headers, ['Only in foo: foo\n'])
 
@@ -699,15 +603,15 @@
 +++ d
 @@ -1,2 +1,2 @@
 -foo
 +bar
  common
 """
         items = patch.splitlines(True)
-        stream = ydiff.PatchStream(Sequential(items))
+        stream = iter(items)
         parser = ydiff.DiffParser(stream)
 
         out = list(parser.get_diff_generator())
         self.assertEqual(len(out), 3)
         self.assertEqual(len(out[1]._hunks), 0)
         self.assertEqual(out[1]._old_path, '')
         self.assertEqual(out[1]._new_path, '')
@@ -735,15 +639,15 @@
 +++ b/bar
 @@ -1,2 +1,2 @@
 -foo
 +bar
  common
 """
         items = patch.splitlines(True)
-        stream = ydiff.PatchStream(Sequential(items))
+        stream = iter(items)
         parser = ydiff.DiffParser(stream)
 
         out = list(parser.get_diff_generator())
         self.assertEqual(len(out), 3)
         self.assertEqual(len(out[1]._hunks), 0)
         self.assertEqual(out[1]._old_path, '')
         self.assertEqual(out[1]._new_path, '')
@@ -761,15 +665,15 @@
 +*
 \\ No newline at end of property
 Added: svn:keywords
 ## -0,0 +1 ##
 +Id
 """
         items = patch.splitlines(True)
-        stream = ydiff.PatchStream(Sequential(items))
+        stream = iter(items)
         parser = ydiff.DiffParser(stream)
         out = list(parser.get_diff_generator())
         self.assertEqual(len(out), 1)
         self.assertEqual(len(out[0]._hunks), 2)
 
         hunk = out[0]._hunks[1]
         self.assertEqual(hunk._hunk_headers, ['Added: svn:keywords\n'])
```

### Comparing `ydiff-1.2/tests/perforce/out.normal` & `ydiff-1.3/tests/perforce/out.normal`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/perforce/out.w70` & `ydiff-1.3/tests/perforce/out.w70`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/perforce/out.side-by-side` & `ydiff-1.3/tests/perforce/out.side-by-side`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/perforce/in.diff` & `ydiff-1.3/tests/perforce/in.diff`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/perforce/out.w70.wrap` & `ydiff-1.3/tests/perforce/out.w70.wrap`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/evil-udiff/out.normal` & `ydiff-1.3/tests/evil-udiff/out.normal`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/evil-udiff/out.w70` & `ydiff-1.3/tests/evil-udiff/out.w70`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/evil-udiff/out.side-by-side` & `ydiff-1.3/tests/evil-udiff/out.side-by-side`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/evil-udiff/out.w70.wrap` & `ydiff-1.3/tests/evil-udiff/out.w70.wrap`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/diff-ru/out.normal` & `ydiff-1.3/tests/diff-ru/out.normal`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/diff-ru/out.w70` & `ydiff-1.3/tests/diff-ru/out.w70`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/diff-ru/out.side-by-side` & `ydiff-1.3/tests/diff-ru/out.side-by-side`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/diff-ru/in.diff` & `ydiff-1.3/tests/diff-ru/in.diff`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/diff-ru/out.w70.wrap` & `ydiff-1.3/tests/diff-ru/out.w70.wrap`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/svn/out.normal` & `ydiff-1.3/tests/svn/out.normal`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/svn/out.w70` & `ydiff-1.3/tests/svn/out.w70`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/svn/out.side-by-side` & `ydiff-1.3/tests/svn/out.side-by-side`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/svn/in.diff` & `ydiff-1.3/tests/svn/in.diff`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/svn/out.w70.wrap` & `ydiff-1.3/tests/svn/out.w70.wrap`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/svn-log/out.normal` & `ydiff-1.3/tests/svn-log/out.normal`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/svn-log/out.w70` & `ydiff-1.3/tests/svn-log/out.w70`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/svn-log/out.side-by-side` & `ydiff-1.3/tests/svn-log/out.side-by-side`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/svn-log/in.diff` & `ydiff-1.3/tests/svn-log/in.diff`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/svn-log/out.w70.wrap` & `ydiff-1.3/tests/svn-log/out.w70.wrap`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/git-bin/out.normal` & `ydiff-1.3/tests/git-bin/out.normal`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/git-bin/out.w70` & `ydiff-1.3/tests/git-bin/out.w70`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/git-bin/out.side-by-side` & `ydiff-1.3/tests/git-bin/out.side-by-side`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/git-bin/in.diff` & `ydiff-1.3/tests/git-bin/in.diff`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/git-bin/out.w70.wrap` & `ydiff-1.3/tests/git-bin/out.w70.wrap`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/latin1/out.w70` & `ydiff-1.3/tests/latin1/out.w70`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/latin1/out.side-by-side` & `ydiff-1.3/tests/latin1/out.side-by-side`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/tests/latin1/out.w70.wrap` & `ydiff-1.3/tests/latin1/out.w70.wrap`

 * *Files identical despite different names*

### Comparing `ydiff-1.2/CHANGES.rst` & `ydiff-1.3/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 
 Change log
 ==========
 
+Version 1.3 (2024-04-02)
+
+  - Dropped context diff support
+  - Handle East Asian wide characters (thanks to @roy2220)
+  - Fix SIGPIPE issue on Windows (unofficial support, thanks to @kingsamchen)
+  - Bump Python requirement to >=2.6 (Python 2 support is no longer tested)
+
 Version 1.2 (2020-08-08)
 
   - Support perforce workspaces
   - Support pager customization via --pager and --pager_options
   - Support running on Windows (requires ``less`` which is offered by git-bash)
   - Fix a bug where reading stdin does not work outside a CVS workspace
   - Fix tab expansion, expands to the next stop modulo tab width
```

### Comparing `ydiff-1.2/ydiff.py` & `ydiff-1.3/ydiff.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,37 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 Term based tool to view *colored*, *incremental* diff in a *Git/Mercurial/Svn*
 workspace or from stdin, with *side by side* and *auto pager* support. Requires
-python (>= 2.5.0) and ``less``.
+python (>= 2.6.0) and ``less``.
 """
 
 import sys
 import os
 import re
 import signal
 import subprocess
-import select
 import difflib
+import unicodedata
 
 META_INFO = {
-    'version'     : '1.2',
+    'version'     : '1.3',
     'license'     : 'BSD-3',
     'author'      : 'Matt Wang',
-    'email'       : 'mattwyl(@)gmail(.)com',
     'url'         : 'https://github.com/ymattw/ydiff',
     'keywords'    : 'colored incremental side-by-side diff',
     'description' : ('View colored, incremental diff in a workspace or from '
                      'stdin, with side by side and auto pager support')
 }
 
-if sys.hexversion < 0x02050000:
-    raise SystemExit('*** Requires python >= 2.5.0')    # pragma: no cover
+if sys.hexversion < 0x02060000:
+    raise SystemExit('*** Requires python >= 2.6.0')    # pragma: no cover
 
-# Python < 2.6 does not have next()
-try:
-    next
-except NameError:
-    def next(obj):
-        return obj.next()
 
 try:
     unicode
 except NameError:
     unicode = str
 
 COLORS = {
@@ -115,38 +108,41 @@
     It returns 3-tuple: (first string, second string, number of visible chars
     in the first string).
 
     If some color was active at the splitting point, then the first string is
     appended with the resetting sequence, and the second string is prefixed
     with all active colors.
     """
-    first = ""
-    second = ""
-    found_colors = ""
+    first = ''
+    second = ''
+    found_colors = ''
     chars_cnt = 0
     bytes_cnt = 0
     while text:
         append_len = 0
-        if text[0] == "\x1b":
-            color_end = text.find("m")
+        if text[0] == '\x1b':
+            color_end = text.find('m')
             if color_end != -1:
                 color = text[:color_end + 1]
-                if color == COLORS["reset"]:
-                    found_colors = ""
+                if color == COLORS['reset']:
+                    found_colors = ''
                 else:
                     found_colors += color
                 append_len = len(color)
 
         if append_len == 0:
             # Current string does not start with any escape sequence, so,
             # either add one more visible char to the "first" string, or
             # break if that string is already large enough.
             if chars_cnt >= width:
                 break
-            chars_cnt += 1
+            if unicodedata.east_asian_width(unicode(text[0])) in ("W", "F"):
+                chars_cnt += 2
+            else:
+                chars_cnt += 1
             append_len = 1
 
         first += text[:append_len]
         text = text[append_len:]
         bytes_cnt += append_len
 
     second = text
@@ -285,142 +281,32 @@
     def is_only_in_dir(self, line):
         return line.startswith('Only in ')
 
     def is_binary_differ(self, line):
         return re.match('^Binary files .* differ$', line.rstrip())
 
 
-class PatchStream(object):
-
-    def __init__(self, diff_hdl):
-        self._diff_hdl = diff_hdl
-        self._stream_header_size = 0
-        self._stream_header = []
-
-        # Test whether stream is empty by read 1 line
-        line = self._diff_hdl.readline()
-        if not line:
-            self._is_empty = True
-        else:
-            self._stream_header.append(line)
-            self._stream_header_size += 1
-            self._is_empty = False
-
-    def is_empty(self):
-        return self._is_empty
-
-    def read_stream_header(self, stream_header_size):
-        """Returns a small chunk for patch type detect, suppose to call once"""
-        for i in range(1, stream_header_size):
-            line = self._diff_hdl.readline()
-            if not line:
-                break
-            self._stream_header.append(line)
-            self._stream_header_size += 1
-        return self._stream_header
-
-    def __iter__(self):
-        for line in self._stream_header:
-            yield line
-        try:
-            for line in self._diff_hdl:
-                yield line
-        except RuntimeError:
-            return
-
-
-class PatchStreamForwarder(object):
-    """A blocking stream forwarder use `select` and line buffered mode.  Feed
-    input stream to a diff format translator and read output stream from it.
-    Note input stream is non-seekable, and upstream has eaten some lines.
-    """
-    def __init__(self, istream, translator):
-        assert isinstance(istream, PatchStream)
-        assert isinstance(translator, subprocess.Popen)
-        self._istream = iter(istream)
-        self._in = translator.stdin
-        self._out = translator.stdout
-
-    def _can_read(self, timeout=0):
-        return select.select([self._out.fileno()], [], [], timeout)[0]
-
-    def _forward_line(self):
-        try:
-            line = next(self._istream)
-            self._in.write(line)
-        except StopIteration:
-            self._in.close()
-
-    def __iter__(self):
-        while True:
-            if self._can_read():
-                line = self._out.readline()
-                if line:
-                    yield line
-                else:
-                    return
-            elif not self._in.closed:
-                self._forward_line()
-
-
 class DiffParser(object):
 
     def __init__(self, stream):
-
-        header = [decode(line) for line in stream.read_stream_header(100)]
-        size = len(header)
-
-        if size >= 4 and (header[0].startswith('*** ') and
-                          header[1].startswith('--- ') and
-                          header[2].rstrip() == '***************' and
-                          header[3].startswith('*** ') and
-                          header[3].rstrip().endswith(' ****')):
-            # For context diff, try use `filterdiff` to translate it to unified
-            # format and provide a new stream
-            #
-            self._type = 'context'
-            try:
-                # Use line buffered mode so that to readline() in block mode
-                self._translator = subprocess.Popen(
-                    ['filterdiff', '--format=unified'], stdin=subprocess.PIPE,
-                    stdout=subprocess.PIPE, bufsize=1)
-            except OSError:
-                raise SystemExit('*** Context diff support depends on '
-                                 'filterdiff')
-            self._stream = PatchStreamForwarder(stream, self._translator)
-            return
-
-        for n in range(size):
-            if (header[n].startswith('--- ') and (n < size - 1) and
-                    header[n + 1].startswith('+++ ')):
-                self._type = 'unified'
-                self._stream = stream
-                break
-        else:
-            # `filterdiff` translates unknown diff to nothing, fall through to
-            # unified diff give ydiff a chance to show everything as headers
-            #
-            sys.stderr.write("*** unknown format, fall through to 'unified'\n")
-            self._type = 'unified'
-            self._stream = stream
+        self._stream = stream
 
     def get_diff_generator(self):
         """parse all diff lines, construct a list of UnifiedDiff objects"""
         diff = UnifiedDiff([], None, None, [])
         headers = []
 
         for line in self._stream:
             line = decode(line)
 
             if diff.is_old_path(line):
                 # This is a new diff when current hunk is not yet genreated or
                 # is completed.  We yield previous diff if exists and construct
                 # a new one for this case.  Otherwise it's acutally an 'old'
                 # line starts with '--- '.
-                #
                 if (not diff._hunks or diff._hunks[-1].is_completed()):
                     if diff._old_path and diff._new_path and diff._hunks:
                         yield diff
                     diff = UnifiedDiff(headers, line, None, [])
                     headers = []
                 else:
                     diff._hunks[-1].append(diff.parse_hunk_line(line))
@@ -449,41 +335,38 @@
             elif diff.is_eof(line):
                 # ignore
                 pass
 
             elif diff.is_only_in_dir(line) or diff.is_binary_differ(line):
                 # 'Only in foo:' and 'Binary files ... differ' are considered
                 # as separate diffs, so yield current diff, then this line
-                #
                 if diff._old_path and diff._new_path and diff._hunks:
                     # Current diff is comppletely constructed
                     yield diff
                 headers.append(line)
                 yield UnifiedDiff(headers, '', '', [])
                 headers = []
                 diff = UnifiedDiff([], None, None, [])
 
             else:
                 # All other non-recognized lines are considered as headers or
                 # hunk headers respectively
-                #
                 headers.append(line)
 
         # Validate and yield the last patch set if it is not yielded yet
         if diff._old_path:
             assert diff._new_path is not None
             if diff._hunks:
                 assert len(diff._hunks[-1]._hunk_meta) > 0
                 assert len(diff._hunks[-1]._hunk_list) > 0
             yield diff
 
         if headers:
             # Tolerate dangling headers, just yield a UnifiedDiff object with
             # only header lines
-            #
             yield UnifiedDiff(headers, '', '', [])
 
 
 class DiffMarker(object):
 
     def __init__(self, side_by_side=False, width=0, tab_width=8, wrap=False):
         self._side_by_side = side_by_side
@@ -544,17 +427,15 @@
                     break
                 # ignore special codes
                 offset = (line.count('\x00', 0, index) * 2 +
                           line.count('\x01', 0, index))
                 # next stop modulo tab width
                 width = self._tab_width - (index - offset) % self._tab_width
                 line = line[:index] + ' ' * width + line[(index + 1):]
-            return (line
-                    .replace('\n', '')
-                    .replace('\r', ''))
+            return line.replace('\n', '').replace('\r', '')
 
         def _fit_with_marker_mix(text, base_color):
             """Wrap input text which contains mdiff tags, markup at the
             meantime
             """
             out = [COLORS[base_color]]
             tag_re = re.compile(r'\x00[+^-]|\x01')
@@ -574,20 +455,18 @@
                         out.append(COLORS['reset'] + COLORS[base_color])
                     text = text[1:]
                 else:
                     # FIXME: utf-8 wchar might break the rule here, e.g.
                     # u'\u554a' takes double width of a single letter, also
                     # this depends on your terminal font.  I guess audience of
                     # this tool never put that kind of symbol in their code :-)
-                    #
                     out.append(text[0])
                     text = text[1:]
 
             out.append(COLORS['reset'])
-
             return ''.join(out)
 
         # Set up number width, note last hunk might be empty
         try:
             (start, offset) = diff._hunks[-1]._old_addr
             max1 = start + offset - 1
             (start, offset) = diff._hunks[-1]._new_addr
@@ -600,15 +479,14 @@
         width = self._width
         if width <= 0:
             # Autodetection of text width according to terminal size
             try:
                 # Each line is like 'nnn TEXT nnn TEXT\n', so width is half of
                 # [terminal size minus the line number columns and 3 separating
                 # spaces
-                #
                 width = (terminal_size()[0] - num_width * 2 - 3) // 2
             except Exception:
                 # If terminal detection failed, set back to default
                 width = 80
 
         # Setup lineno and line format
         left_num_fmt = colorize('%%(left_num)%ds' % num_width, 'yellow')
@@ -735,25 +613,15 @@
         line = line.replace('\x00+', add_code)
         line = line.replace('\x00^', chg_code)
         line = line.replace('\x01', rst_code)
         return colorize(line, base_color)
 
 
 def markup_to_pager(stream, opts):
-    """Pipe unified diff stream to pager (less).
-
-    Note: have to create pager Popen object before the translator Popen object
-    in PatchStreamForwarder, otherwise the `stdin=subprocess.PIPE` would cause
-    trouble to the translator pipe (select() never see EOF after input stream
-    ended), most likely python bug 12607 (http://bugs.python.org/issue12607)
-    which was fixed in python 2.7.3.
-
-    See issue #30 (https://github.com/ymattw/ydiff/issues/30) for more
-    information.
-    """
+    """Pipe unified diff stream to pager (less)."""
     pager_cmd = [opts.pager]
     pager_opts = (opts.pager_options.split(' ')
                   if opts.pager_options is not None
                   else None)
 
     if opts.pager is None:
         pager_cmd = ['less']
@@ -815,19 +683,33 @@
         x = fcntl.ioctl(1, termios.TIOCGWINSZ, s)
         height, width = struct.unpack('HHHH', x)[0:2]
     except (IOError, AttributeError):
         pass
     return width, height
 
 
-def main():
-    if sys.platform != 'win32':
-        signal.signal(signal.SIGPIPE, signal.SIG_DFL)
-    signal.signal(signal.SIGINT, signal.SIG_DFL)
+def trap_interrupts(entry_fn):
+    def entry_wrapper():
+        signal.signal(signal.SIGINT, signal.SIG_DFL)
+        if sys.platform != 'win32':
+            signal.signal(signal.SIGPIPE, signal.SIG_DFL)
+            return entry_fn()
+        else:
+            import errno
+            try:
+                return entry_fn()
+            except IOError as e:
+                if e.errno not in [errno.EPIPE, errno.EINVAL]:
+                    raise
+                return 0
+    return entry_wrapper
+
 
+@trap_interrupts
+def main():
     from optparse import (OptionParser, BadOptionError, AmbiguousOptionError,
                           OptionGroup)
 
     class PassThroughOptionParser(OptionParser):
         """Stop parsing on first unknown option (e.g. --cached, -U10) and pass
         them down.  Note the `opt_str` in exception object does not give us
         chance to take the full option back, e.g. for '-U10' it will only
@@ -883,66 +765,48 @@
                          'Environment variable YDIFF_OPTIONS may be used to '
                          'specify default options that will be placed at the '
                          'beginning of the argument list.'))
     parser.add_option_group(option_group)
 
     # Place possible options defined in YDIFF_OPTIONS at the beginning of argv
     ydiff_opts = [x for x in os.getenv('YDIFF_OPTIONS', '').split(' ') if x]
-
-    # TODO: Deprecate CDIFF_OPTIONS. Fall back to it and warn (for now).
-    if not ydiff_opts:
-        cdiff_opts = [x for x in os.getenv('CDIFF_OPTIONS', '').split(' ')
-                      if x]
-        if cdiff_opts:
-            sys.stderr.write('*** CDIFF_OPTIONS will be depreated soon, '
-                             'please use YDIFF_OPTIONS instead\n')
-            ydiff_opts = cdiff_opts
-
     opts, args = parser.parse_args(ydiff_opts + sys.argv[1:])
 
+    stream = None
     if not sys.stdin.isatty():
-        diff_hdl = (sys.stdin.buffer if hasattr(sys.stdin, 'buffer')
-                    else sys.stdin)
+        stream = getattr(sys.stdin, 'buffer', sys.stdin)
     else:
         vcs_name = revision_control_probe()
         if vcs_name is None:
             supported_vcs = ', '.join(sorted(VCS_INFO.keys()))
             sys.stderr.write('*** Not in a supported workspace, supported are:'
                              ' %s\n' % supported_vcs)
             return 1
 
         if opts.log:
-            diff_hdl = revision_control_log(vcs_name, args)
-            if diff_hdl is None:
+            stream = revision_control_log(vcs_name, args)
+            if stream is None:
                 sys.stderr.write('*** %s does not support log command.\n' %
                                  vcs_name)
                 return 1
         else:
             # 'diff' is a must have feature.
-            diff_hdl = revision_control_diff(vcs_name, args)
-
-    stream = PatchStream(diff_hdl)
-
-    # Don't let empty diff pass thru
-    if stream.is_empty():
-        return 0
+            stream = revision_control_diff(vcs_name, args)
 
     if (opts.color == 'always' or
             (opts.color == 'auto' and sys.stdout.isatty())):
         markup_to_pager(stream, opts)
     else:
         # pipe out stream untouched to make sure it is still a patch
-        byte_output = (sys.stdout.buffer if hasattr(sys.stdout, 'buffer')
-                       else sys.stdout)
+        byte_output = getattr(sys.stdout, 'buffer', sys.stdout)
         for line in stream:
             byte_output.write(line)
 
-    if diff_hdl is not sys.stdin:
-        diff_hdl.close()
-
+    if stream is not None:
+        stream.close()
     return 0
 
 
 if __name__ == '__main__':
     sys.exit(main())
 
 # vim:set et sts=4 sw=4 tw=79:
```

### Comparing `ydiff-1.2/README.rst` & `ydiff-1.3/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,61 @@
 Ydiff
 =====
 
-.. image:: https://travis-ci.org/ymattw/ydiff.png?branch=master
-   :target: https://travis-ci.org/ymattw/ydiff
-   :alt: Build status
+.. image:: https://github.com/ymattw/ydiff/actions/workflows/test.yml/badge.svg
+   :alt: Tests status
+   :target: https://github.com/ymattw/ydiff/actions
 
 Term based tool to view *colored*, *incremental* diff in a version controlled
 workspace (supports Git, Mercurial, Perforce and Svn so far) or from stdin,
 with *side by side* (similar to ``diff -y``) and *auto pager* support. Requires
-python (>= 2.5.0) and ``less``.
+python (>= 2.6.0) and ``less``.
 
 .. image:: https://raw.github.com/ymattw/ydiff/gh-pages/img/default.png
    :alt: default
    :align: center
 
 .. image:: https://raw.github.com/ymattw/ydiff/gh-pages/img/side-by-side.png
    :alt: side by side
    :align: center
    :width: 900 px
 
+Ydiff only supports diff in `Unified Format`_. This is default in most version
+control system except Perforce, which needs an environment variable
+``P4DIFF="diff -u"`` to output unified diff.
+
+.. _`Unified Format`: https://en.wikipedia.org/wiki/Diff#Unified_format
+
 Installation
 ------------
 
+Ydiff only depends on Python built-in libraries, so you can just download the
+source and run without worrying about any installation.
+
+Git tagged `releases`_ will be packaged and uploaded to PyPI timely, however,
+packages hosted elsewhere are not (please note they are not managed by the
+author `@ymattw`_).
+
+.. _`@ymattw`: https://github.com/ymattw
+.. _`releases`: https://github.com/ymattw/ydiff/releases
+
+Download directly
+~~~~~~~~~~~~~~~~~
+
+Just save `ydiff.py`_ to whatever directory which is in your ``$PATH``, for
+example, ``$HOME/bin`` is in my ``$PATH``, so I save the script there and name
+as ``ydiff``.
+
+.. _`ydiff.py`: https://raw.github.com/ymattw/ydiff/master/ydiff.py
+
+.. code-block:: bash
+
+    curl -ksSL https://raw.github.com/ymattw/ydiff/master/ydiff.py > ~/bin/ydiff
+    chmod +x ~/bin/ydiff
+
 Install with pip
 ~~~~~~~~~~~~~~~~
 
 Ydiff is already listed on `PyPI`_, you can install with ``pip`` if you have
 the tool.
 
 .. _PyPI: http://pypi.python.org/pypi/ydiff
@@ -52,15 +82,15 @@
 `@bfontaine`_, `@hivehand`_ and `@nijikon`_ for contributing to the Homebrew
 `Formula`_).
 
 .. _`@josa42`: https://github.com/josa42
 .. _`@bfontaine`: https://github.com/bfontaine
 .. _`@hivehand`: https://github.com/hivehand
 .. _`@nijikon`: https://github.com/nijikon
-.. _`Formula`: https://github.com/Homebrew/homebrew-core/blob/master/Formula/ydiff.rb
+.. _`Formula`: https://github.com/Homebrew/homebrew-core/blob/master/Formula/y/ydiff.rb
 
 .. code-block:: bash
 
     brew install ydiff
 
 
 Install on Fedora
@@ -77,28 +107,14 @@
 
 On FreeBSD, you can install ydiff with pkg.
 
 .. code-block:: bash
 
     pkg install ydiff
 
-Download directly
-~~~~~~~~~~~~~~~~~
-
-Just save `ydiff.py`_ to whatever directory which is in your ``$PATH``, for
-example, ``$HOME/bin`` is in my ``$PATH``, so I save the script there and name
-as ``ydiff``.
-
-.. _`ydiff.py`: https://raw.github.com/ymattw/ydiff/master/ydiff.py
-
-.. code-block:: bash
-
-    curl -ksSL https://raw.github.com/ymattw/ydiff/master/ydiff.py > ~/bin/ydiff
-    chmod +x ~/bin/ydiff
-
 Usage
 -----
 
 Type ``ydiff -h`` to show usage::
 
     $ ydiff -h
     Usage: ydiff [options] [file|dir ...]
@@ -173,18 +189,15 @@
     svn diff -r1234 | ydiff -s  # view svn diff comparing to given revision
     diff -u file1 file2 | ydiff # view diff between two files (note the '-u')
     diff -ur dir1 dir2 | ydiff  # view diff between two dirs
 
     # View diff in a GitHub pull request, side by side
     curl https://github.com/ymattw/ydiff/pull/11.diff | ydiff -s
 
-    # View a patch file in unified or context format, the latter depends on
-    # command `filterdiff` from package `patchutils` which is available in
-    # major Linux distros and MacPorts.
-    #
+    # View a patch file in unified format.
     ydiff -s < foo.patch
 
 Redirect output to another patch file is safe:
 
 .. code-block:: bash
 
     svn diff -r PREV | ydiff -s > my.patch
@@ -216,31 +229,14 @@
     ln -s "${ydiff_dir}/ydiff" "${ydiff_dir}/git-ydiff"
 
 Known issues
 ------------
 
 Ydiff has following known issues:
 
-- Does not recognize `normal` diff, and depends on ``filterdiff`` (patchutils)
-  to read `context` diff
 - Side by side mode has alignment problem for wide chars
 - Terminal might be in a mess on exception (type ``reset`` can fix it)
 
 Pull requests are very welcome, please make sure your changes can pass unit
-tests and regression tests by run ``make test`` (required tool *coverage* can
-be installed with ``pip install coverage``).  Also watch out `travis build`_
-after push, make sure it passes as well.
-
-.. _`travis build`: https://travis-ci.org/ymattw/ydiff/pull_requests
-
-See also
---------
-
-I have another tool `coderev`_ which generates side-by-side diff pages for code
-review from two given files or directories, I found it's not easy to extend to
-support git so invented `ydiff`.  Idea of ansi color markup is also from
-project `colordiff`_.
-
-.. _coderev: https://github.com/ymattw/coderev
-.. _colordiff: https://github.com/daveewart/colordiff
+tests and regression tests by run ``make docker-test``.
 
 .. vim:set ft=rst et sw=4 sts=4 tw=79:
```

