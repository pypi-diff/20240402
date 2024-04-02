# Comparing `tmp/blindschleiche-0.2.4.tar.gz` & `tmp/blindschleiche-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blindschleiche-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "blindschleiche-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `blindschleiche-0.2.4.tar` & `blindschleiche-0.2.5.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     3129 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/README.md
--rw-r--r--   0        0        0     3323 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/__init__.py
--rw-r--r--   0        0        0      323 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/__main__.py
--rw-r--r--   0        0        0      651 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/_utils.py
--rw-r--r--   0        0        0     3574 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/deepclust2fa.py
--rw-r--r--   0        0        0     1390 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/ebiosra2rl2s.py
--rw-r--r--   0        0        0     1913 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/equalbestblast.py
--rw-r--r--   0        0        0     3377 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/esearchandfetch.py
--rw-r--r--   0        0        0      848 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/falen.py
--rw-r--r--   0        0        0      764 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/farename.py
--rw-r--r--   0        0        0     3943 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/fastasanitiser.py
--rw-r--r--   0        0        0     1366 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/galhist.py
--rw-r--r--   0        0        0     5818 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/genigvjs.py
--rw-r--r--   0        0        0     1905 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/gffcat.py
--rwxr-xr-x   0        0        0     1651 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/gffcsqify.py
--rw-r--r--   0        0        0    12118 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/gffparse.py
--rw-r--r--   0        0        0      946 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/gfftagsane.py
--rw-r--r--   0        0        0     4555 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/gg2k.py
--rw-r--r--   0        0        0     6264 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/ildemux.py
--rw-r--r--   0        0        0     1336 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/ilsample.py
--rw-r--r--   0        0        0     3882 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/liftoff_gff3.py
--rw-r--r--   0        0        0     1981 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/mask2bed.py
--rw-r--r--   0        0        0     1170 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/n50.py
--rw-r--r--   0        0        0     1905 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/nstitch.py
--rw-r--r--   0        0        0     1045 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/pairslash.py
--rw-r--r--   0        0        0     5143 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/pansn_rename.py
--rw-r--r--   0        0        0     1372 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/regionbed.py
--rw-r--r--   0        0        0     2161 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/shannon.py
--rw-r--r--   0        0        0     1845 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/tabcat.py
--rw-r--r--   0        0        0     3189 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/telogrep.py
--rw-r--r--   0        0        0     1290 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/uniref_accessionmap.py
--rwxr-xr-x   0        0        0     6030 2024-02-20 08:16:27.781287 blindschleiche-0.2.4/blsl/vcfparallel.py
--rw-r--r--   0        0        0     3287 2024-02-20 08:16:27.785287 blindschleiche-0.2.4/blsl/vcfstats.py
--rw-r--r--   0        0        0      534 2024-02-20 08:16:27.785287 blindschleiche-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3451 1970-01-01 00:00:00.000000 blindschleiche-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     3129 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/README.md
+-rw-r--r--   0        0        0     3405 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/__init__.py
+-rw-r--r--   0        0        0      323 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/__main__.py
+-rw-r--r--   0        0        0      651 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/_utils.py
+-rw-r--r--   0        0        0     3574 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/deepclust2fa.py
+-rw-r--r--   0        0        0     1366 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/ebiosra2rl2s.py
+-rw-r--r--   0        0        0     1913 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/equalbestblast.py
+-rw-r--r--   0        0        0     3377 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/esearchandfetch.py
+-rw-r--r--   0        0        0      832 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/falen.py
+-rw-r--r--   0        0        0      748 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/farename.py
+-rw-r--r--   0        0        0     3943 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/fastasanitiser.py
+-rw-r--r--   0        0        0     1366 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/galhist.py
+-rw-r--r--   0        0        0     5818 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/genigvjs.py
+-rw-r--r--   0        0        0     1905 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/gffcat.py
+-rw-r--r--   0        0        0     1651 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/gffcsqify.py
+-rw-r--r--   0        0        0    12355 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/gffparse.py
+-rw-r--r--   0        0        0      946 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/gfftagsane.py
+-rw-r--r--   0        0        0     4555 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/gg2k.py
+-rw-r--r--   0        0        0     6264 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/ildemux.py
+-rw-r--r--   0        0        0     1341 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/ilsample.py
+-rw-r--r--   0        0        0     2083 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/jsonl2csv.py
+-rw-r--r--   0        0        0     3882 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/liftoff_gff3.py
+-rw-r--r--   0        0        0     1981 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/mask2bed.py
+-rw-r--r--   0        0        0     1170 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/n50.py
+-rw-r--r--   0        0        0     1905 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/nstitch.py
+-rw-r--r--   0        0        0     1045 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/pairslash.py
+-rw-r--r--   0        0        0     5143 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/pansn_rename.py
+-rw-r--r--   0        0        0     1372 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/regionbed.py
+-rw-r--r--   0        0        0     2161 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/shannon.py
+-rw-r--r--   0        0        0     1845 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/tabcat.py
+-rw-r--r--   0        0        0     3189 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/telogrep.py
+-rw-r--r--   0        0        0     1290 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/uniref_accessionmap.py
+-rw-r--r--   0        0        0     6030 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/vcfparallel.py
+-rw-r--r--   0        0        0     3025 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/blsl/vcfstats.py
+-rw-r--r--   0        0        0      534 2024-04-02 16:57:02.783231 blindschleiche-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3451 1970-01-01 00:00:00.000000 blindschleiche-0.2.5/PKG-INFO
```

### Comparing `blindschleiche-0.2.4/README.md` & `blindschleiche-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/__init__.py` & `blindschleiche-0.2.5/blsl/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 from sys import argv, exit, stderr
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 
 cmds = {}
 
+
 from .telogrep import telogrep_main
 cmds["telogrep"] = telogrep_main
 
 from .n50 import n50_main
 cmds["n50"] = n50_main
 
 from .falen import falen_main
 cmds["falen"] = falen_main
 
 from .mask2bed import mask2bed_main
 cmds["mask2bed"] = mask2bed_main
 
-from .genigvjs import genigvjs_main
-cmds["genigvjs"] = genigvjs_main
-
-
 from .pansn_rename import main as pansn_rename_main
 cmds["pansn-rename"] = pansn_rename_main
 
+from .genigvjs import genigvjs_main
+cmds["genigvjs"] = genigvjs_main
+
 from .ildemux import main as ildemux_main
 cmds["ildemux"] = ildemux_main
 
 from .ilsample import main as ilsample_main
 cmds["ilsample"] = ilsample_main
 
 from .regionbed import main as regionbed_main
@@ -58,40 +58,39 @@
 
 from .deepclust2fa import deepclust2fa_main
 cmds["deepclust2fa"] = deepclust2fa_main
 
 from .farename import farename_main
 cmds["farename"] = farename_main
 
-from .ebiosra2rl2s import main as rl2s_main
-cmds["ebiosra2rl2s"] = rl2s_main
-
-from .galhist import main as galhist_main
-cmds["galhist"] = galhist_main
-
 from .gffcat import gffcat_main
 cmds["gffcat"] = gffcat_main
 
 from .gffparse import gffparse_main
 cmds["gffparse"] = gffparse_main
 
-
 from .gffcsqify import main as gffcsqify_main
 cmds["gffcsqify"] = gffcsqify_main
 
+from .gfftagsane import main as gfftagsane_main
+cmds["gfftagsane"] = gfftagsane_main
+
 from .liftoff_gff3 import liftoff_gff3_main
 cmds["liftoff-gff3"] = liftoff_gff3_main
 
-from .gfftagsane import main as gfftagsane_main
-cmds["gfftagsane"] = gfftagsane_main
+from .ebiosra2rl2s import main as rl2s_main
+cmds["ebiosra2rl2s"] = rl2s_main
 
+from .galhist import main as galhist_main
+cmds["galhist"] = galhist_main
 
 from .pairslash import main as pairslash_main
 cmds["pairslash"] = pairslash_main
 
+
 try:
     from .vcfstats import main as vcfstats_main
     cmds["vcfstats"] = vcfstats_main
 
     from .vcfparallel import main as vcfparallel_main
     cmds["vcfparallel"] = vcfparallel_main
 except ImportError as exc:
@@ -100,14 +99,18 @@
 
 from .shannon import main as shannon_main
 cmds["shannon-entropy"] = shannon_main
 
 from .fastasanitiser import main as fastasanitiser_main
 cmds["fastasanitiser"] = fastasanitiser_main
 
+from .jsonl2csv import main as jsonl2csv_main
+cmds["jsonl2csv"] = jsonl2csv_main
+
+
 def mainhelp(argv=None):
     """Print this help message"""
     print("USAGE: blsl <subtool> [options...]\n\n")
     print("Where <subtool> is one of:\n")
     for tool, func in cmds.items():
         print("  {:<19}".format(tool + ":"), " ", func.__doc__.split("\n")[0])
     print("\n\nUse blsl subtool --help to get help about a specific tool")
```

### Comparing `blindschleiche-0.2.4/blsl/_utils.py` & `blindschleiche-0.2.5/blsl/_utils.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/deepclust2fa.py` & `blindschleiche-0.2.5/blsl/deepclust2fa.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/ebiosra2rl2s.py` & `blindschleiche-0.2.5/blsl/ebiosra2rl2s.py`

 * *Files 27% similar despite different names*

```diff
@@ -18,16 +18,15 @@
             path, sample, run, read = m.groups()
             if sample not in samples:
                 samples[sample] = {run: {read: path}}
             elif run not in samples[sample]:
                 samples[sample][run] = {read: path}
             else:
                 samples[sample][run][read] = path
-    #json.dump(samples, stdout, indent=2)
-    print("library", "run", "read1_uri", "read2_uri", file=stdout, sep='\t')
+    print("library", "run", "sample", "read1_uri", "read2_uri", file=stdout, sep='\t')
     for sample, dat in samples.items():
         for run, reads in dat.items():
-            print(sample, run, reads["R1"], reads["R2"], file=stdout, sep='\t')
+            print(sample, run, sample, reads["R1"], reads["R2"], file=stdout, sep='\t')
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `blindschleiche-0.2.4/blsl/equalbestblast.py` & `blindschleiche-0.2.5/blsl/equalbestblast.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/esearchandfetch.py` & `blindschleiche-0.2.5/blsl/esearchandfetch.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/falen.py` & `blindschleiche-0.2.5/blsl/farename.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 #!/usr/bin/env python3
-from sys import argv
 import argparse
 
 from Bio import SeqIO
 
-def falen_main(argv):
-    """Tabulate the lengths of sequences in a FASTA file"""
+def farename_main(argv=None):
+    """Rename sequences in a fasta file sequentially"""
     ap = argparse.ArgumentParser()
-    ap.add_argument("-t", "--total", action="store_true",
-            help="Output only a total length per file")
+    ap.add_argument("-p", "--prefix", type=str, default="",
+            help="Prefix for each sequence ID (e.g. SEQ_ -> SEQ_1, SEQ_2 etc)")
     ap.add_argument("fastas", help="FASTA file of contigs", nargs="+")
     args = ap.parse_args(argv)
     
     for infile in args.fastas:
+        i = 0
         with open(infile) as fh:
-            file_total = 0
             for seq in SeqIO.parse(fh, 'fasta'):
-                file_total += len(seq.seq)
-                if not args.total:
-                    print(infile, seq.name, len(seq.seq), sep="\t")
-            if args.total:
-                print(infile, file_total, sep="\t")
+                i += 1
+                print(f">{args.prefix}{i} {seq.id} {seq.description}")
+                print(seq.seq)
+
                 
 if __name__ == "__main__":
-    falen_main()
+    farename_main()
```

### Comparing `blindschleiche-0.2.4/blsl/fastasanitiser.py` & `blindschleiche-0.2.5/blsl/fastasanitiser.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/galhist.py` & `blindschleiche-0.2.5/blsl/galhist.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/genigvjs.py` & `blindschleiche-0.2.5/blsl/genigvjs.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/gffcat.py` & `blindschleiche-0.2.5/blsl/gffcat.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/gffcsqify.py` & `blindschleiche-0.2.5/blsl/gffcsqify.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/gffparse.py` & `blindschleiche-0.2.5/blsl/gffparse.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 #Initialized GeneInfo named tuple. Note: namedtuple is immutable
 gffInfoFields = ["seqid", "source", "type", "start", "end", "score", "strand", "phase", "attributes"]
 GFFRecord = namedtuple("GFFRecord", gffInfoFields)
 
 ontological_order = [
     "chromosome", "gene", "pseudogene", "pseudogenic_region", "mRNA", "transcript", "pseudogenic_transcript",
-    "exon", "pseudogenic_exon", "five_prime_UTR", "three_prime_UTR", "CDS", "pseudogenic_CDS",
+    "intron", "exon", "pseudogenic_exon", "five_prime_UTR", "three_prime_UTR", "CDS", "pseudogenic_CDS",
 ]
 
 def parseGFFAttributes(attributeString, lax=False):
     """Parse the GFF3 attribute column and return a dict"""#
     if attributeString == ".": return {}
     ret = {}
     if lax:
@@ -101,14 +101,15 @@
         "transposable_element_gene": "l1",
         "gene": "l1",
         "tRNA": "l2",
         "pseudogenic_transcript": "l2",
         "tmRNA": "l2",
         "mRNA": "l2",
         "exon": "l3",
+        "intron": "l3",
         "CDS": "l3",
         "five_prime_UTR": "l3",
         "three_prime_UTR": "l3",
     }
     ignore = {
         "source",
         "stop_codon",
@@ -164,26 +165,30 @@
                 else:
                     parent = None
             l2l1[id] = parent
             record["children"] = {}
             try:
                 records[parent]["children"][id] = record
             except KeyError:
-                print(f"L2 entry {id} parent {parent} not in records? {record}")
+                if "missing_l2" not in warned:
+                    print(f"L2 entry {id} parent {parent} not in records? {record}")
+                    warned.add("missing_l2")
         else:
             try:
                 parent = record["attributes"].get("Parent", record["attributes"].get("transcript_id", None))
                 top = l2l1[parent]
                 if id in records[top]["children"][parent]["children"]:
                     i += 1
                     id = f"{id}_{i}"
                     record["attributes"]["ID"] = id
                 records[top]["children"][parent]["children"][id] = record
             except KeyError:
-                print(f"L3 entry {id} parent not in records? {record}")
+                if "missing_l3" not in warned:
+                    print(f"L3 entry {id} parent '{parent}' not in GFF?")
+                    warned.add("missing_l3")
     return records
 
 
 def attr2line(attrs):
     from urllib.parse import quote as Q
     return ";".join("=".join((Q(k), Q(v))) for k, v in attrs.items())
 
@@ -302,15 +307,15 @@
     ap.add_argument("-g", "--make-missing-genes", action="store_true",
             help="Invent Fake L1 'gene' entries for any L2 lacking an L1 parent")
     ap.add_argument("input", help="Input GFF")
     args = ap.parse_args(argv)
 
     with open(args.output, "w") as fh:
         if args.tabular:
-            records =  list(tqdm(parseGFF3(args.input, return_as=dict), desc="Parse GFF"))
+            records =  list(tqdm(parseGFF3(args.input, return_as=dict), desc="Parse GFF", item="line"))
             fields = set()
             for line in records:
                 fields.update(line["attributes"].keys())
             print(*gffInfoFields[:-1], *fields, sep="\t", file=fh)
             for line in tqdm(records, desc="Tabularise"):
                 cols = [line[x] for x in gffInfoFields[:-1]] + [line["attributes"].get(x) for x in fields]
                 cols = [x if x is not None else "" for x in cols]
```

### Comparing `blindschleiche-0.2.4/blsl/gfftagsane.py` & `blindschleiche-0.2.5/blsl/gfftagsane.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/gg2k.py` & `blindschleiche-0.2.5/blsl/gg2k.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/ildemux.py` & `blindschleiche-0.2.5/blsl/ildemux.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/ilsample.py` & `blindschleiche-0.2.5/blsl/ilsample.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         fqp.append(line)
         if len(fqp) == 8:
             yield fqp
             fqp = list()
     if len(fqp) == 8:
         yield fqp
 
-def main(argv):
+def main(argv=None):
     """Sample a fraction of read pairs from an interleaved fastq file
     """
     import argparse
     ap = argparse.ArgumentParser()
     ap.add_argument("-o", "--out", default="/dev/fd/1", type=argparse.FileType("wb"),
             help="Output file")
     ap.add_argument("-f", "--frac", default=0.1, type=float,
```

### Comparing `blindschleiche-0.2.4/blsl/liftoff_gff3.py` & `blindschleiche-0.2.5/blsl/liftoff_gff3.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/mask2bed.py` & `blindschleiche-0.2.5/blsl/mask2bed.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/n50.py` & `blindschleiche-0.2.5/blsl/n50.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/nstitch.py` & `blindschleiche-0.2.5/blsl/nstitch.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/pairslash.py` & `blindschleiche-0.2.5/blsl/pairslash.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/pansn_rename.py` & `blindschleiche-0.2.5/blsl/pansn_rename.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/regionbed.py` & `blindschleiche-0.2.5/blsl/regionbed.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/shannon.py` & `blindschleiche-0.2.5/blsl/shannon.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/tabcat.py` & `blindschleiche-0.2.5/blsl/tabcat.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/telogrep.py` & `blindschleiche-0.2.5/blsl/telogrep.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/uniref_accessionmap.py` & `blindschleiche-0.2.5/blsl/uniref_accessionmap.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/vcfparallel.py` & `blindschleiche-0.2.5/blsl/vcfparallel.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/blsl/vcfstats.py` & `blindschleiche-0.2.5/blsl/vcfstats.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,97 +1,84 @@
 #!/usr/bin/env python3
 from tqdm import tqdm
 from cyvcf2 import VCF
-import pandas as pd
 
 import sys
 from sys import stdin, stdout, stderr
 from subprocess import Popen, PIPE
 import argparse
 import math
+import json
 from concurrent.futures import ProcessPoolExecutor, as_completed
 
 def parallel_regions(vcf, cores=1):
     V = VCF(vcf)
     # 10 chunks per chrom per core
-    chunks = len(V.seqlens)*10*cores
+    chunks = len(V.seqlens)*100*cores
     for cname, clen in zip(V.seqnames, V.seqlens):
-        chunk = int(math.ceil(clen/chunks))
+        chunk = 10000#int(math.ceil(clen/chunks))
         for start in range(0, clen, chunk):
             s = start+1
             e = start+chunk+1
             yield f"{cname}:{s}-{e}"
 
-def variant2dict(v):
+def variant2dict(v, fields=None):
     for i, alt in enumerate(v.ALT):
         dat = {"CHROM": v.CHROM, "POS": v.POS, "REF": v.REF, "ALT": alt, "QUAL": v.QUAL}
         dat["call_rate"] = v.call_rate
         for key, val  in v.INFO:
             if isinstance(val, str) and "," in val:
                 val = val.split(',')
             if isinstance(val, tuple) or isinstance(val, list):
                 val = val[i]
             dat[f"INFO_{key}"] = val
-        yield dat
+        if fields:
+            dat = {K:V for K, V in dat.items() if K in fields}
+        yield json.dumps(dat)
 
-def bcftools_info_with_tags(vbcf):
-    res = []
-    cmd=f"bcftools +fill-tags {vbcf} -Ou -- -d -t all,F_MISSING"
-    with Popen(cmd, shell=True, stdout=PIPE) as proc:
-        for v in tqdm(VCF(proc.stdout)):
-            for r in variant2dict(v):
-                res.append(r)
-    return res
-
-def one_chunk_stats(vcf, chunk, fill=True):
+def one_chunk_stats(vcf, chunk, fill=True, fields=None):
     cmd=f"bcftools view -r {chunk} {vcf} -Ou"
     if fill:
         cmd = f"{cmd} | bcftools +fill-tags - -Ou -- -d -t all,F_MISSING"
     res = []
     with Popen(cmd, shell=True, stdout=PIPE) as proc:
-        for v in VCF(proc.stdout):
-            for r in variant2dict(v):
+        vcf = VCF(proc.stdout)
+        for v in vcf:
+            for r in variant2dict(v, fields=fields):
                 res.append(r)
+        del vcf
     return res
 
 def chunkwise_bcfools_stats(args):
-    res = []
-    with ProcessPoolExecutor(args.threads) as exc:
-        jobs = []
-        for region in parallel_regions(args.vcf):
-            jobs.append(exc.submit(one_chunk_stats, args.vcf, region, fill=args.fill_tags_first))
-        for job in tqdm(as_completed(jobs), total=len(jobs), unit="chunk"):
-            res.extend(job.result())
-    return res
+    regions = list(parallel_regions(args.vcf))
+    with tqdm(total=len(regions), unit="chunk") as pbar:
+        for i in range(0, len(regions), 10000):
+            to=min(len(regions), i+10000)
+            with ProcessPoolExecutor(args.threads) as exc:
+                jobs = (exc.submit(one_chunk_stats, args.vcf, region, fill=args.fill_tags_first, fields=args.fields) for region in regions[i:to])
+                for job in as_completed(jobs):
+                    pbar.update(1)
+                    for res in job.result():
+                        args.output.write(res)
+                        args.output.write("\n")
 
-def filter_fields(dat, fields=None):
-    if fields is None:
-        return dat
-    return {k: dat[k] for k in fields if k in dat}
 
 def main(argv=None):
     """Use bcftools to calculate various statistics, outputing an R-ready table"""
     ap = argparse.ArgumentParser()
     ap.add_argument("-o", "--output", default=stdout, type=argparse.FileType("wt"),
-            help="Output TSV file")
+            help="Output jsonlines file")
     ap.add_argument("-f", "--fields", nargs="+",
             help="Use only these fields")
     ap.add_argument("-F", "--fill-tags-first", action="store_true",
             help="Use bcftools +fill-tags to pre-fill more fields (forces no parallelism)")
     ap.add_argument("-t", "--threads", default=1, type=int,
             help="Number of parallel threads")
 
     ap.add_argument("vcf")
     args = ap.parse_args(argv)
 
-    #if args.fill_tags_first:
-    #    variants = bcftools_info_with_tags(args.vcf)
-    #else:
-    variants = chunkwise_bcfools_stats(args)
-    if args.fields:
-        variants = [filter_fields(x, args.fields) for x in variants]
+    chunkwise_bcfools_stats(args)
 
-    df = pd.DataFrame(variants)
-    df.to_csv(args.output, sep="\t", index=False)
 
 if __name__ == "__main__":
     main()
```

### Comparing `blindschleiche-0.2.4/pyproject.toml` & `blindschleiche-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.2.4/PKG-INFO` & `blindschleiche-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blindschleiche
-Version: 0.2.4
+Version: 0.2.5
 Summary: Miscelanelous python-based bioinformatics utils
 Author-email: "Dr. K. D. Murray" <info@gekkonid.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: tqdm
 Requires-Dist: biopython
 Requires-Dist: cyvcf2
```

