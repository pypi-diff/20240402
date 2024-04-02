# Comparing `tmp/cle-9.2.96.tar.gz` & `tmp/cle-9.2.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cle-9.2.96.tar", last modified: Tue Mar 26 17:01:45 2024, max compression
+gzip compressed data, was "cle-9.2.97.tar", last modified: Tue Apr  2 17:02:10 2024, max compression
```

## Comparing `cle-9.2.96.tar` & `cle-9.2.97.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:45.605962 cle-9.2.96/
--rw-r--r--   0 vsts      (1001) docker     (127)     1327 2024-03-26 17:00:57.000000 cle-9.2.96/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)       34 2024-03-26 17:00:57.000000 cle-9.2.96/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     6672 2024-03-26 17:01:45.605962 cle-9.2.96/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     4910 2024-03-26 17:00:57.000000 cle-9.2.96/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:45.573963 cle-9.2.96/cle/
--rw-r--r--   0 vsts      (1001) docker     (127)     2746 2024-03-26 17:01:09.000000 cle-9.2.96/cle/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2681 2024-03-26 17:00:57.000000 cle-9.2.96/cle/address_translator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:45.581962 cle-9.2.96/cle/backends/
--rw-r--r--   0 vsts      (1001) docker     (127)     1398 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21376 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9202 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/binja.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3791 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/blob.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:45.581962 cle-9.2.96/cle/backends/cgc/
--rw-r--r--   0 vsts      (1001) docker     (127)       86 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/cgc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3095 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/cgc/backedcgc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1386 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/cgc/cgc.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15781 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/coff.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:45.585962 cle-9.2.96/cle/backends/elf/
--rw-r--r--   0 vsts      (1001) docker     (127)      120 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      921 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/compilation_unit.py
--rw-r--r--   0 vsts      (1001) docker     (127)    62261 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/elf.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25130 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/elfcore.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4094 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/hashtable.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5991 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/lsda.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19998 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/metaelf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2244 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/regions.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:45.585962 cle-9.2.96/cle/backends/elf/relocation/
--rw-r--r--   0 vsts      (1001) docker     (127)     1437 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/relocation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1638 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/relocation/amd64.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18466 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/relocation/arm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3194 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/relocation/arm64.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1007 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/relocation/arm_cortex_m.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1094 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/relocation/armel.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1094 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/relocation/armhf.py
--rw-r--r--   0 vsts      (1001) docker     (127)      818 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/relocation/elfreloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7157 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/relocation/generic.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1724 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/relocation/i386.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1056 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/relocation/mips.py
--rw-r--r--   0 vsts      (1001) docker     (127)      542 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/relocation/mips64.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4612 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/relocation/pcc64.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8962 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/relocation/ppc.py
--rw-r--r--   0 vsts      (1001) docker     (127)      582 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/relocation/s390x.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1349 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/relocation/sparc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1733 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/subprogram.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2359 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/symbol.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5413 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/symbol_type.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4682 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/variable.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10205 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/elf/variable_type.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:45.589962 cle-9.2.96/cle/backends/externs/
--rw-r--r--   0 vsts      (1001) docker     (127)    10751 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/externs/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:45.589962 cle-9.2.96/cle/backends/externs/simdata/
--rw-r--r--   0 vsts      (1001) docker     (127)      180 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/externs/simdata/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3359 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/externs/simdata/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2356 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/externs/simdata/glibc_startup.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3446 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/externs/simdata/io_file.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2382 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/externs/simdata/simdata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6548 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/ihex.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:45.589962 cle-9.2.96/cle/backends/java/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/java/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4081 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/java/android_lifecycle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9929 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/java/apk.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3122 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/java/jar.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7273 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/java/soot.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:45.593962 cle-9.2.96/cle/backends/macho/
--rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/macho/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22044 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/macho/binding.py
--rw-r--r--   0 vsts      (1001) docker     (127)    47241 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/macho/macho.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7948 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/macho/macho_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3088 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/macho/section.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2150 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/macho/segment.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16766 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/macho/structs.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12844 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/macho/symbol.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:45.593962 cle-9.2.96/cle/backends/minidump/
--rw-r--r--   0 vsts      (1001) docker     (127)     6702 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/minidump/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2356 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/named_region.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:45.593962 cle-9.2.96/cle/backends/pe/
--rw-r--r--   0 vsts      (1001) docker     (127)       44 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/pe/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11994 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/pe/pe.py
--rw-r--r--   0 vsts      (1001) docker     (127)      923 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/pe/regions.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:45.593962 cle-9.2.96/cle/backends/pe/relocation/
--rw-r--r--   0 vsts      (1001) docker     (127)     1435 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/pe/relocation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      494 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/pe/relocation/amd64.py
--rw-r--r--   0 vsts      (1001) docker     (127)      629 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/pe/relocation/arm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3236 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/pe/relocation/generic.py
--rw-r--r--   0 vsts      (1001) docker     (127)      492 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/pe/relocation/i386.py
--rw-r--r--   0 vsts      (1001) docker     (127)      636 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/pe/relocation/mips.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2159 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/pe/relocation/pereloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)      691 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/pe/relocation/riscv.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1257 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/pe/symbol.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5546 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/region.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4990 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/regions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5237 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/relocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5561 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/srec.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1589 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/static_archive.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4359 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/symbol.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3357 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/te.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:45.597962 cle-9.2.96/cle/backends/tls/
--rw-r--r--   0 vsts      (1001) docker     (127)      426 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/tls/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6392 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/tls/elf_tls.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1815 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/tls/elfcore_tls.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1350 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/tls/minidump_tls.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4801 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/tls/pe_tls.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2175 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/tls/tls_object.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6432 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/uefi_firmware.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3834 2024-03-26 17:00:57.000000 cle-9.2.96/cle/backends/xbe.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1106 2024-03-26 17:00:57.000000 cle-9.2.96/cle/errors.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3603 2024-03-26 17:00:57.000000 cle-9.2.96/cle/gdb.py
--rw-r--r--   0 vsts      (1001) docker     (127)    54612 2024-03-26 17:00:57.000000 cle-9.2.96/cle/loader.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23547 2024-03-26 17:00:57.000000 cle-9.2.96/cle/memory.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1560 2024-03-26 17:00:57.000000 cle-9.2.96/cle/patched_stream.py
--rw-r--r--   0 vsts      (1001) docker     (127)        8 2024-03-26 17:00:57.000000 cle-9.2.96/cle/py.typed
--rw-r--r--   0 vsts      (1001) docker     (127)     4019 2024-03-26 17:00:57.000000 cle-9.2.96/cle/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:45.601962 cle-9.2.96/cle.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     6672 2024-03-26 17:01:45.000000 cle-9.2.96/cle.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     3890 2024-03-26 17:01:45.000000 cle-9.2.96/cle.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-26 17:01:45.000000 cle-9.2.96/cle.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      330 2024-03-26 17:01:45.000000 cle-9.2.96/cle.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        4 2024-03-26 17:01:45.000000 cle-9.2.96/cle.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      238 2024-03-26 17:01:09.000000 cle-9.2.96/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     1268 2024-03-26 17:01:45.609962 cle-9.2.96/setup.cfg
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-26 17:01:45.601962 cle-9.2.96/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)     1649 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_address_translator.py
--rw-r--r--   0 vsts      (1001) docker     (127)      735 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_arch_detect.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1387 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_arm_firmware.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1949 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_blob.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3342 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_clemory.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1031 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_coff.py
--rw-r--r--   0 vsts      (1001) docker     (127)      633 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_compiler_detection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      513 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_dwarf_resiliency.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1437 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_elfcore.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1671 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)      966 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_gdb.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1712 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_got.py
--rw-r--r--   0 vsts      (1001) docker     (127)      668 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_hex.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7802 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_macho.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20566 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_macho_bindinghelper.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7111 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_macho_dyld.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2017 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_macho_dyld_structs.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4128 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_macho_libs.py
--rw-r--r--   0 vsts      (1001) docker     (127)    42112 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_macho_reloc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1358 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_minidump.py
--rw-r--r--   0 vsts      (1001) docker     (127)      929 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_namedregion.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1012 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_overlap.py
--rw-r--r--   0 vsts      (1001) docker     (127)      887 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_patched_stream.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_pe.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7163 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_plt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1661 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_ppc64_initial_rtoc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2993 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_ppc_relocations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      549 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_preload.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7718 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_regions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3586 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_relocated.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1037 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_runpath.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_simdata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1220 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_stream.py
--rw-r--r--   0 vsts      (1001) docker     (127)      545 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_tls_resiliency.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2810 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_unpackword.py
--rw-r--r--   0 vsts      (1001) docker     (127)      844 2024-03-26 17:00:57.000000 cle-9.2.96/tests/test_xbe.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:10.886320 cle-9.2.97/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1327 2024-04-02 17:01:33.000000 cle-9.2.97/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)       34 2024-04-02 17:01:33.000000 cle-9.2.97/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     6672 2024-04-02 17:02:10.886320 cle-9.2.97/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     4910 2024-04-02 17:01:33.000000 cle-9.2.97/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:10.858320 cle-9.2.97/cle/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2746 2024-04-02 17:01:45.000000 cle-9.2.97/cle/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2681 2024-04-02 17:01:33.000000 cle-9.2.97/cle/address_translator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:10.862320 cle-9.2.97/cle/backends/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1398 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21376 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9202 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/binja.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3791 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/blob.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:10.862320 cle-9.2.97/cle/backends/cgc/
+-rw-r--r--   0 vsts      (1001) docker     (127)       86 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/cgc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3095 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/cgc/backedcgc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1386 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/cgc/cgc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15781 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/coff.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:10.866320 cle-9.2.97/cle/backends/elf/
+-rw-r--r--   0 vsts      (1001) docker     (127)      120 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      921 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/compilation_unit.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    62261 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/elf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25130 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/elfcore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4094 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/hashtable.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5991 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/lsda.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19998 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/metaelf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2244 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/regions.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:10.866320 cle-9.2.97/cle/backends/elf/relocation/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1437 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/relocation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1638 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/relocation/amd64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18466 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/relocation/arm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3194 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/relocation/arm64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1007 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/relocation/arm_cortex_m.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1094 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/relocation/armel.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1094 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/relocation/armhf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      818 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/relocation/elfreloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7157 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/relocation/generic.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1724 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/relocation/i386.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1056 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/relocation/mips.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      542 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/relocation/mips64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4612 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/relocation/pcc64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8962 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/relocation/ppc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      582 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/relocation/s390x.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1349 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/relocation/sparc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1733 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/subprogram.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2359 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/symbol.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5413 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/symbol_type.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4682 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/variable.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10205 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/elf/variable_type.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:10.870320 cle-9.2.97/cle/backends/externs/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10751 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/externs/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:10.870320 cle-9.2.97/cle/backends/externs/simdata/
+-rw-r--r--   0 vsts      (1001) docker     (127)      180 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/externs/simdata/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3359 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/externs/simdata/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2356 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/externs/simdata/glibc_startup.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3446 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/externs/simdata/io_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2382 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/externs/simdata/simdata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6548 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/ihex.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:10.870320 cle-9.2.97/cle/backends/java/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/java/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4081 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/java/android_lifecycle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9929 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/java/apk.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3122 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/java/jar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7273 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/java/soot.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:10.874320 cle-9.2.97/cle/backends/macho/
+-rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/macho/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22044 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/macho/binding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    47241 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/macho/macho.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7948 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/macho/macho_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3088 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/macho/section.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2150 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/macho/segment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16766 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/macho/structs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12844 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/macho/symbol.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:10.874320 cle-9.2.97/cle/backends/minidump/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6702 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/minidump/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2356 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/named_region.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:10.874320 cle-9.2.97/cle/backends/pe/
+-rw-r--r--   0 vsts      (1001) docker     (127)       44 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/pe/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11994 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/pe/pe.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      923 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/pe/regions.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:10.874320 cle-9.2.97/cle/backends/pe/relocation/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1435 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/pe/relocation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      494 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/pe/relocation/amd64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      629 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/pe/relocation/arm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3236 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/pe/relocation/generic.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      492 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/pe/relocation/i386.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      636 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/pe/relocation/mips.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2159 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/pe/relocation/pereloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      691 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/pe/relocation/riscv.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1257 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/pe/symbol.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5546 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4990 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/regions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5237 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/relocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5561 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/srec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1589 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/static_archive.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4359 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/symbol.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3357 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/te.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:10.874320 cle-9.2.97/cle/backends/tls/
+-rw-r--r--   0 vsts      (1001) docker     (127)      426 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/tls/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6392 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/tls/elf_tls.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1815 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/tls/elfcore_tls.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1350 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/tls/minidump_tls.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4801 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/tls/pe_tls.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2175 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/tls/tls_object.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6432 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/uefi_firmware.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3834 2024-04-02 17:01:33.000000 cle-9.2.97/cle/backends/xbe.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1106 2024-04-02 17:01:33.000000 cle-9.2.97/cle/errors.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3603 2024-04-02 17:01:33.000000 cle-9.2.97/cle/gdb.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    54612 2024-04-02 17:01:33.000000 cle-9.2.97/cle/loader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23547 2024-04-02 17:01:33.000000 cle-9.2.97/cle/memory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1560 2024-04-02 17:01:33.000000 cle-9.2.97/cle/patched_stream.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        8 2024-04-02 17:01:33.000000 cle-9.2.97/cle/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (127)     4019 2024-04-02 17:01:33.000000 cle-9.2.97/cle/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:10.882320 cle-9.2.97/cle.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6672 2024-04-02 17:02:10.000000 cle-9.2.97/cle.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     3890 2024-04-02 17:02:10.000000 cle-9.2.97/cle.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-02 17:02:10.000000 cle-9.2.97/cle.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      330 2024-04-02 17:02:10.000000 cle-9.2.97/cle.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        4 2024-04-02 17:02:10.000000 cle-9.2.97/cle.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      238 2024-04-02 17:01:45.000000 cle-9.2.97/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1268 2024-04-02 17:02:10.886320 cle-9.2.97/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 17:02:10.882320 cle-9.2.97/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1649 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_address_translator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      735 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_arch_detect.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1387 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_arm_firmware.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1949 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_blob.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3342 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_clemory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1031 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_coff.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      633 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_compiler_detection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      513 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_dwarf_resiliency.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1437 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_elfcore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1671 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      966 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_gdb.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1712 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_got.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      668 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_hex.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7802 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_macho.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20566 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_macho_bindinghelper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7111 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_macho_dyld.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2017 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_macho_dyld_structs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4128 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_macho_libs.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    42112 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_macho_reloc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1358 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_minidump.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      929 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_namedregion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1012 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_overlap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      887 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_patched_stream.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_pe.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7163 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_plt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1661 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_ppc64_initial_rtoc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2993 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_ppc_relocations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      549 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_preload.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7718 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_regions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3586 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_relocated.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1037 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_runpath.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_simdata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1220 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_stream.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      545 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_tls_resiliency.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2810 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_unpackword.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      844 2024-04-02 17:01:33.000000 cle-9.2.97/tests/test_xbe.py
```

### Comparing `cle-9.2.96/LICENSE` & `cle-9.2.97/LICENSE`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/PKG-INFO` & `cle-9.2.97/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: cle
-Version: 9.2.96
+Version: 9.2.97
 Summary: CLE Loads Everything (at least, many binary formats!) and provides a pythonic interface to analyze what they are and what they would look like in memory.
 Home-page: https://github.com/angr/cle
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: archinfo==9.2.96
+Requires-Dist: archinfo==9.2.97
 Requires-Dist: pefile
 Requires-Dist: pyelftools>=0.27
-Requires-Dist: pyvex==9.2.96
+Requires-Dist: pyvex==9.2.97
 Requires-Dist: sortedcontainers>=2.0
 Provides-Extra: ar
 Requires-Dist: arpy==1.1.1; extra == "ar"
 Provides-Extra: docs
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
```

### Comparing `cle-9.2.96/README.md` & `cle-9.2.97/README.md`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/__init__.py` & `cle-9.2.97/cle/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 CLE is an extensible binary loader. Its main goal is to take an executable program and any libraries it depends on and
 produce an address space where that program is loaded and ready to run.
 
 The primary interface to CLE is the Loader class.
 """
 
-__version__ = "9.2.96"
+__version__ = "9.2.97"
 
 from .address_translator import AT, AddressTranslator
 from .backends import (
     ALL_BACKENDS,
     CGC,
     ELF,
     PE,
```

### Comparing `cle-9.2.96/cle/address_translator.py` & `cle-9.2.97/cle/address_translator.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/__init__.py` & `cle-9.2.97/cle/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/backend.py` & `cle-9.2.97/cle/backends/backend.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/binja.py` & `cle-9.2.97/cle/backends/binja.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/blob.py` & `cle-9.2.97/cle/backends/blob.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/cgc/backedcgc.py` & `cle-9.2.97/cle/backends/cgc/backedcgc.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/cgc/cgc.py` & `cle-9.2.97/cle/backends/cgc/cgc.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/coff.py` & `cle-9.2.97/cle/backends/coff.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/compilation_unit.py` & `cle-9.2.97/cle/backends/elf/compilation_unit.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/elf.py` & `cle-9.2.97/cle/backends/elf/elf.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/elfcore.py` & `cle-9.2.97/cle/backends/elf/elfcore.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/hashtable.py` & `cle-9.2.97/cle/backends/elf/hashtable.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/lsda.py` & `cle-9.2.97/cle/backends/elf/lsda.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/metaelf.py` & `cle-9.2.97/cle/backends/elf/metaelf.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/regions.py` & `cle-9.2.97/cle/backends/elf/regions.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/relocation/__init__.py` & `cle-9.2.97/cle/backends/elf/relocation/__init__.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/relocation/amd64.py` & `cle-9.2.97/cle/backends/elf/relocation/amd64.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/relocation/arm.py` & `cle-9.2.97/cle/backends/elf/relocation/arm.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/relocation/arm64.py` & `cle-9.2.97/cle/backends/elf/relocation/arm64.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/relocation/arm_cortex_m.py` & `cle-9.2.97/cle/backends/elf/relocation/arm_cortex_m.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/relocation/armel.py` & `cle-9.2.97/cle/backends/elf/relocation/armel.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/relocation/armhf.py` & `cle-9.2.97/cle/backends/elf/relocation/armhf.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/relocation/elfreloc.py` & `cle-9.2.97/cle/backends/elf/relocation/elfreloc.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/relocation/generic.py` & `cle-9.2.97/cle/backends/elf/relocation/generic.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/relocation/i386.py` & `cle-9.2.97/cle/backends/elf/relocation/i386.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/relocation/mips.py` & `cle-9.2.97/cle/backends/elf/relocation/mips.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/relocation/mips64.py` & `cle-9.2.97/cle/backends/elf/relocation/mips64.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/relocation/pcc64.py` & `cle-9.2.97/cle/backends/elf/relocation/pcc64.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/relocation/ppc.py` & `cle-9.2.97/cle/backends/elf/relocation/ppc.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/relocation/s390x.py` & `cle-9.2.97/cle/backends/elf/relocation/s390x.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/relocation/sparc.py` & `cle-9.2.97/cle/backends/elf/relocation/sparc.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/subprogram.py` & `cle-9.2.97/cle/backends/elf/subprogram.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/symbol.py` & `cle-9.2.97/cle/backends/elf/symbol.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/symbol_type.py` & `cle-9.2.97/cle/backends/elf/symbol_type.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/variable.py` & `cle-9.2.97/cle/backends/elf/variable.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/elf/variable_type.py` & `cle-9.2.97/cle/backends/elf/variable_type.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/externs/__init__.py` & `cle-9.2.97/cle/backends/externs/__init__.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/externs/simdata/common.py` & `cle-9.2.97/cle/backends/externs/simdata/common.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/externs/simdata/glibc_startup.py` & `cle-9.2.97/cle/backends/externs/simdata/glibc_startup.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/externs/simdata/io_file.py` & `cle-9.2.97/cle/backends/externs/simdata/io_file.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/externs/simdata/simdata.py` & `cle-9.2.97/cle/backends/externs/simdata/simdata.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/ihex.py` & `cle-9.2.97/cle/backends/ihex.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/java/android_lifecycle.py` & `cle-9.2.97/cle/backends/java/android_lifecycle.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/java/apk.py` & `cle-9.2.97/cle/backends/java/apk.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/java/jar.py` & `cle-9.2.97/cle/backends/java/jar.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/java/soot.py` & `cle-9.2.97/cle/backends/java/soot.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/macho/binding.py` & `cle-9.2.97/cle/backends/macho/binding.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/macho/macho.py` & `cle-9.2.97/cle/backends/macho/macho.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/macho/macho_enums.py` & `cle-9.2.97/cle/backends/macho/macho_enums.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/macho/section.py` & `cle-9.2.97/cle/backends/macho/section.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/macho/segment.py` & `cle-9.2.97/cle/backends/macho/segment.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/macho/structs.py` & `cle-9.2.97/cle/backends/macho/structs.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/macho/symbol.py` & `cle-9.2.97/cle/backends/macho/symbol.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/minidump/__init__.py` & `cle-9.2.97/cle/backends/minidump/__init__.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/named_region.py` & `cle-9.2.97/cle/backends/named_region.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/pe/pe.py` & `cle-9.2.97/cle/backends/pe/pe.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/pe/regions.py` & `cle-9.2.97/cle/backends/pe/regions.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/pe/relocation/__init__.py` & `cle-9.2.97/cle/backends/pe/relocation/__init__.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/pe/relocation/arm.py` & `cle-9.2.97/cle/backends/pe/relocation/arm.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/pe/relocation/generic.py` & `cle-9.2.97/cle/backends/pe/relocation/generic.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/pe/relocation/mips.py` & `cle-9.2.97/cle/backends/pe/relocation/mips.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/pe/relocation/pereloc.py` & `cle-9.2.97/cle/backends/pe/relocation/pereloc.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/pe/relocation/riscv.py` & `cle-9.2.97/cle/backends/pe/relocation/riscv.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/pe/symbol.py` & `cle-9.2.97/cle/backends/pe/symbol.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/region.py` & `cle-9.2.97/cle/backends/region.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/regions.py` & `cle-9.2.97/cle/backends/regions.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/relocation.py` & `cle-9.2.97/cle/backends/relocation.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/srec.py` & `cle-9.2.97/cle/backends/srec.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/static_archive.py` & `cle-9.2.97/cle/backends/static_archive.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/symbol.py` & `cle-9.2.97/cle/backends/symbol.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/te.py` & `cle-9.2.97/cle/backends/te.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/tls/elf_tls.py` & `cle-9.2.97/cle/backends/tls/elf_tls.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/tls/elfcore_tls.py` & `cle-9.2.97/cle/backends/tls/elfcore_tls.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/tls/minidump_tls.py` & `cle-9.2.97/cle/backends/tls/minidump_tls.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/tls/pe_tls.py` & `cle-9.2.97/cle/backends/tls/pe_tls.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/tls/tls_object.py` & `cle-9.2.97/cle/backends/tls/tls_object.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/uefi_firmware.py` & `cle-9.2.97/cle/backends/uefi_firmware.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/backends/xbe.py` & `cle-9.2.97/cle/backends/xbe.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/errors.py` & `cle-9.2.97/cle/errors.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/gdb.py` & `cle-9.2.97/cle/gdb.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/loader.py` & `cle-9.2.97/cle/loader.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/memory.py` & `cle-9.2.97/cle/memory.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/patched_stream.py` & `cle-9.2.97/cle/patched_stream.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle/utils.py` & `cle-9.2.97/cle/utils.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/cle.egg-info/PKG-INFO` & `cle-9.2.97/cle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: cle
-Version: 9.2.96
+Version: 9.2.97
 Summary: CLE Loads Everything (at least, many binary formats!) and provides a pythonic interface to analyze what they are and what they would look like in memory.
 Home-page: https://github.com/angr/cle
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: archinfo==9.2.96
+Requires-Dist: archinfo==9.2.97
 Requires-Dist: pefile
 Requires-Dist: pyelftools>=0.27
-Requires-Dist: pyvex==9.2.96
+Requires-Dist: pyvex==9.2.97
 Requires-Dist: sortedcontainers>=2.0
 Provides-Extra: ar
 Requires-Dist: arpy==1.1.1; extra == "ar"
 Provides-Extra: docs
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
```

### Comparing `cle-9.2.96/cle.egg-info/SOURCES.txt` & `cle-9.2.97/cle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/setup.cfg` & `cle-9.2.97/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 
 [options]
 packages = find:
 install_requires = 
-	archinfo==9.2.96
+	archinfo==9.2.97
 	pefile
 	pyelftools>=0.27
-	pyvex==9.2.96
+	pyvex==9.2.97
 	sortedcontainers>=2.0
 python_requires = >=3.8
 tests_require = cffi
 
 [options.extras_require]
 ar = 
 	arpy==1.1.1
```

### Comparing `cle-9.2.96/tests/test_address_translator.py` & `cle-9.2.97/tests/test_address_translator.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_arch_detect.py` & `cle-9.2.97/tests/test_arch_detect.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_arm_firmware.py` & `cle-9.2.97/tests/test_arm_firmware.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_blob.py` & `cle-9.2.97/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_clemory.py` & `cle-9.2.97/tests/test_clemory.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_coff.py` & `cle-9.2.97/tests/test_coff.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_compiler_detection.py` & `cle-9.2.97/tests/test_compiler_detection.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_dwarf_resiliency.py` & `cle-9.2.97/tests/test_dwarf_resiliency.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_elfcore.py` & `cle-9.2.97/tests/test_elfcore.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_exceptions.py` & `cle-9.2.97/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_gdb.py` & `cle-9.2.97/tests/test_gdb.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_got.py` & `cle-9.2.97/tests/test_got.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_hex.py` & `cle-9.2.97/tests/test_hex.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_macho.py` & `cle-9.2.97/tests/test_macho.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_macho_bindinghelper.py` & `cle-9.2.97/tests/test_macho_bindinghelper.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_macho_dyld.py` & `cle-9.2.97/tests/test_macho_dyld.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_macho_dyld_structs.py` & `cle-9.2.97/tests/test_macho_dyld_structs.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_macho_libs.py` & `cle-9.2.97/tests/test_macho_libs.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_macho_reloc.py` & `cle-9.2.97/tests/test_macho_reloc.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_minidump.py` & `cle-9.2.97/tests/test_minidump.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_namedregion.py` & `cle-9.2.97/tests/test_namedregion.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_overlap.py` & `cle-9.2.97/tests/test_overlap.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_patched_stream.py` & `cle-9.2.97/tests/test_patched_stream.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_pe.py` & `cle-9.2.97/tests/test_pe.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_plt.py` & `cle-9.2.97/tests/test_plt.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_ppc64_initial_rtoc.py` & `cle-9.2.97/tests/test_ppc64_initial_rtoc.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_ppc_relocations.py` & `cle-9.2.97/tests/test_ppc_relocations.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_preload.py` & `cle-9.2.97/tests/test_preload.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_regions.py` & `cle-9.2.97/tests/test_regions.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_relocated.py` & `cle-9.2.97/tests/test_relocated.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_runpath.py` & `cle-9.2.97/tests/test_runpath.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_simdata.py` & `cle-9.2.97/tests/test_simdata.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_stream.py` & `cle-9.2.97/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_tls_resiliency.py` & `cle-9.2.97/tests/test_tls_resiliency.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_unpackword.py` & `cle-9.2.97/tests/test_unpackword.py`

 * *Files identical despite different names*

### Comparing `cle-9.2.96/tests/test_xbe.py` & `cle-9.2.97/tests/test_xbe.py`

 * *Files identical despite different names*

