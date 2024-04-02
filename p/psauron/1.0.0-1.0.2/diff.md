# Comparing `tmp/psauron-1.0.0.tar.gz` & `tmp/psauron-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psauron-1.0.0.tar", last modified: Tue Feb 27 20:10:19 2024, max compression
+gzip compressed data, was "psauron-1.0.2.tar", last modified: Tue Apr  2 19:13:10 2024, max compression
```

## Comparing `psauron-1.0.0.tar` & `psauron-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0 markus    (1000) markus    (1000)        0 2024-02-27 20:10:19.991913 psauron-1.0.0/
--rwxrwxrwx   0 markus    (1000) markus    (1000)       38 2024-01-18 19:50:03.000000 psauron-1.0.0/MANIFEST.in
--rwxrwxrwx   0 markus    (1000) markus    (1000)      953 2024-02-27 20:10:19.989913 psauron-1.0.0/PKG-INFO
--rwxrwxrwx   0 markus    (1000) markus    (1000)      316 2024-02-27 20:04:01.000000 psauron-1.0.0/README.md
-drwxrwxrwx   0 markus    (1000) markus    (1000)        0 2024-02-27 20:10:19.772913 psauron-1.0.0/app/
--rwxrwxrwx   0 markus    (1000) markus    (1000)     5934 2024-02-27 19:28:41.000000 psauron-1.0.0/app/TCN_model.py
--rwxrwxrwx   0 markus    (1000) markus    (1000)        0 2024-01-18 19:59:40.000000 psauron-1.0.0/app/__init__.py
-drwxrwxrwx   0 markus    (1000) markus    (1000)        0 2024-02-27 20:10:19.806913 psauron-1.0.0/app/data/
--rwxrwxrwx   0 markus    (1000) markus    (1000)        0 2024-01-17 22:05:05.000000 psauron-1.0.0/app/data/__init__.py
--rwxrwxrwx   0 markus    (1000) markus    (1000)   792554 2024-01-17 22:22:11.000000 psauron-1.0.0/app/data/model_state_dict.pt
--rwxrwxrwx   0 markus    (1000) markus    (1000)    24352 2024-02-27 20:08:59.000000 psauron-1.0.0/app/psauron.py
-drwxrwxrwx   0 markus    (1000) markus    (1000)        0 2024-02-27 20:10:19.911916 psauron-1.0.0/psauron.egg-info/
--rwxrwxrwx   0 markus    (1000) markus    (1000)      953 2024-02-27 20:10:18.000000 psauron-1.0.0/psauron.egg-info/PKG-INFO
--rwxrwxrwx   0 markus    (1000) markus    (1000)      421 2024-02-27 20:10:18.000000 psauron-1.0.0/psauron.egg-info/SOURCES.txt
--rwxrwxrwx   0 markus    (1000) markus    (1000)        1 2024-02-27 20:10:18.000000 psauron-1.0.0/psauron.egg-info/dependency_links.txt
--rwxrwxrwx   0 markus    (1000) markus    (1000)       56 2024-02-27 20:10:18.000000 psauron-1.0.0/psauron.egg-info/entry_points.txt
--rwxrwxrwx   0 markus    (1000) markus    (1000)      195 2024-02-27 20:10:18.000000 psauron-1.0.0/psauron.egg-info/requires.txt
--rwxrwxrwx   0 markus    (1000) markus    (1000)       10 2024-02-27 20:10:18.000000 psauron-1.0.0/psauron.egg-info/top_level.txt
--rwxrwxrwx   0 markus    (1000) markus    (1000)       38 2024-02-27 20:10:19.992914 psauron-1.0.0/setup.cfg
--rwxrwxrwx   0 markus    (1000) markus    (1000)     1457 2024-02-27 20:08:13.000000 psauron-1.0.0/setup.py
-drwxrwxrwx   0 markus    (1000) markus    (1000)        0 2024-02-27 20:10:19.974912 psauron-1.0.0/tests/
--rwxrwxrwx   0 markus    (1000) markus    (1000)        0 2024-01-18 19:59:40.000000 psauron-1.0.0/tests/__init__.py
--rwxrwxrwx   0 markus    (1000) markus    (1000)     2628 2024-02-27 19:43:19.000000 psauron-1.0.0/tests/test_eye_of_psauron.py
--rwxrwxrwx   0 markus    (1000) markus    (1000)       90 2024-02-27 19:09:05.000000 psauron-1.0.0/tests/test_load_model.py
--rwxrwxrwx   0 markus    (1000) markus    (1000)      278 2024-02-27 18:58:13.000000 psauron-1.0.0/tests/test_reverse_complement.py
+drwxrwxrwx   0 markus    (1000) markus    (1000)        0 2024-04-02 19:13:10.622275 psauron-1.0.2/
+-rwxrwxrwx   0 markus    (1000) markus    (1000)     1092 2024-03-21 17:58:55.000000 psauron-1.0.2/LICENSE.txt
+-rwxrwxrwx   0 markus    (1000) markus    (1000)       38 2024-03-21 17:58:55.000000 psauron-1.0.2/MANIFEST.in
+-rwxrwxrwx   0 markus    (1000) markus    (1000)     4708 2024-04-02 19:13:10.617275 psauron-1.0.2/PKG-INFO
+-rwxrwxrwx   0 markus    (1000) markus    (1000)     3772 2024-03-21 17:58:55.000000 psauron-1.0.2/README.md
+drwxrwxrwx   0 markus    (1000) markus    (1000)        0 2024-04-02 19:13:10.467941 psauron-1.0.2/app/
+-rwxrwxrwx   0 markus    (1000) markus    (1000)     5934 2024-03-21 17:58:55.000000 psauron-1.0.2/app/TCN_model.py
+-rwxrwxrwx   0 markus    (1000) markus    (1000)        0 2024-03-21 17:58:55.000000 psauron-1.0.2/app/__init__.py
+drwxrwxrwx   0 markus    (1000) markus    (1000)        0 2024-04-02 19:13:10.493559 psauron-1.0.2/app/data/
+-rwxrwxrwx   0 markus    (1000) markus    (1000)        0 2024-03-21 17:58:55.000000 psauron-1.0.2/app/data/__init__.py
+-rwxrwxrwx   0 markus    (1000) markus    (1000)   792554 2024-03-21 17:58:55.000000 psauron-1.0.2/app/data/model_state_dict.pt
+-rwxrwxrwx   0 markus    (1000) markus    (1000)    28558 2024-04-02 19:00:29.000000 psauron-1.0.2/app/psauron.py
+drwxrwxrwx   0 markus    (1000) markus    (1000)        0 2024-04-02 19:13:10.567192 psauron-1.0.2/psauron.egg-info/
+-rwxrwxrwx   0 markus    (1000) markus    (1000)     4708 2024-04-02 19:13:09.000000 psauron-1.0.2/psauron.egg-info/PKG-INFO
+-rwxrwxrwx   0 markus    (1000) markus    (1000)      433 2024-04-02 19:13:09.000000 psauron-1.0.2/psauron.egg-info/SOURCES.txt
+-rwxrwxrwx   0 markus    (1000) markus    (1000)        1 2024-04-02 19:13:09.000000 psauron-1.0.2/psauron.egg-info/dependency_links.txt
+-rwxrwxrwx   0 markus    (1000) markus    (1000)       55 2024-04-02 19:13:09.000000 psauron-1.0.2/psauron.egg-info/entry_points.txt
+-rwxrwxrwx   0 markus    (1000) markus    (1000)      212 2024-04-02 19:13:09.000000 psauron-1.0.2/psauron.egg-info/requires.txt
+-rwxrwxrwx   0 markus    (1000) markus    (1000)       10 2024-04-02 19:13:09.000000 psauron-1.0.2/psauron.egg-info/top_level.txt
+-rwxrwxrwx   0 markus    (1000) markus    (1000)       38 2024-04-02 19:13:10.623277 psauron-1.0.2/setup.cfg
+-rwxrwxrwx   0 markus    (1000) markus    (1000)     1503 2024-04-02 19:00:05.000000 psauron-1.0.2/setup.py
+drwxrwxrwx   0 markus    (1000) markus    (1000)        0 2024-04-02 19:13:10.605769 psauron-1.0.2/tests/
+-rwxrwxrwx   0 markus    (1000) markus    (1000)        0 2024-03-21 17:58:55.000000 psauron-1.0.2/tests/__init__.py
+-rwxrwxrwx   0 markus    (1000) markus    (1000)     2854 2024-04-02 18:59:35.000000 psauron-1.0.2/tests/test_eye_of_psauron.py
+-rwxrwxrwx   0 markus    (1000) markus    (1000)       90 2024-03-21 17:58:55.000000 psauron-1.0.2/tests/test_load_model.py
+-rwxrwxrwx   0 markus    (1000) markus    (1000)      278 2024-03-21 17:58:55.000000 psauron-1.0.2/tests/test_reverse_complement.py
```

### Comparing `psauron-1.0.0/app/TCN_model.py` & `psauron-1.0.2/app/TCN_model.py`

 * *Files identical despite different names*

### Comparing `psauron-1.0.0/app/data/model_state_dict.pt` & `psauron-1.0.2/app/data/model_state_dict.pt`

 * *Files identical despite different names*

### Comparing `psauron-1.0.0/app/psauron.py` & `psauron-1.0.2/app/psauron.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     parser.add_argument("-m", "--minimum-length", type=int, required=False, help="OPTIONAL exclude all proteins shorter than m amino acids, default=5", default=5)
     parser.add_argument("-e", "--exclude", type=str, help="OPTIONAL exclude any CDS where FASTA description contains given text (case invariant), e.g. \"hypothetical\", default=None", default="")
     parser.add_argument("--inframe", type=float, required=False, help="OPTIONAL probability threshold used to determine final psauron score, in-frame, higher number decreases sensitivity and increases specificity, default=0.5, range=[0,1]", default=0.5)
     parser.add_argument("--outframe", type=float, required=False, help="OPTIONAL probability threshold used to determine final psauron score, out-of-frame, higher number increases sensitivity and decreases specificity, default=0.5, range=[0,1]", default=0.5)
     parser.add_argument("-c", "--use-cpu", action='store_true', help="OPTIONAL set -c to force usage of CPU instead of GPU, default=False", default=False)
     parser.add_argument("-s", "--single-frame", action='store_true', help="OPTIONAL set -s to score only the in-frame CDS, which may lower accuracy of the model, default=False", default=False)
     parser.add_argument("-p", "--protein", action='store_true', help="OPTIONAL set -p if your FASTA contains amino acid protein sequence, which may lower accuracy of the model, default=False", default=False)
+    parser.add_argument("-a", "--all-prob", action='store_true', help="OPTIONAL set -a to output per-amino-acid predicted probabilities, NOTE: these may not behave as expected due to receptive field size, default=False", default=False)
     parser.add_argument("-v", "--verbose", action='store_true', help="OPTIONAL set -v for verbose output with progress bars etc., default=False", default=False)
 
     args = parser.parse_args()
     return args
     
 def get_data_path():
     # gets correct path to model weight data for installed package
@@ -84,81 +85,95 @@
             torch.cuda.empty_cache()
         else:
             X_enc = F.one_hot(X, 21).permute(0,2,1).float()
             probs = expit(model(X_enc).cpu())
 
     return probs
     
-def score_seq(aa_seq_list, model, use_cpu, verbose, gene_batch_size=100):
+def score_seq(aa_seq_list, model, use_cpu, allprob, verbose, gene_batch_size=100):
     # format seqs
     ORF_seq_enc = [tokenize_aa_seq(str(x)) for x in aa_seq_list]
 
     # sort by length to minimize impact of batch padding
     ORF_lengths = np.asarray([len(x) for x in ORF_seq_enc])
     length_idx = np.argsort(ORF_lengths)
     ORF_seq_sorted = [ORF_seq_enc[i] for i in length_idx]
 
     # pad to allow creation of batch matrix
     prob_list = []
+    prob_list_allprob = []
     if verbose:
         for i in tqdm(range(0, len(ORF_seq_sorted), gene_batch_size), unit=" batch"):
             batch = ORF_seq_sorted[i:i+gene_batch_size]
             seq_lengths = torch.LongTensor(list(map(len, batch)))
             seq_tensor = torch.zeros((len(batch), seq_lengths.max())).long()
             for idx, (seq, seqlen) in enumerate(zip(batch, seq_lengths)):
                 seq_tensor[idx, :seqlen] = torch.LongTensor(seq)
             pred_all = predict(seq_tensor, model, use_cpu)
             pred = []
+            pred_allprob = []
             for j, length in enumerate(seq_lengths):
                 subseq = pred_all[j, 0, 0:int(length)]
                 idx = min(100, int(length) - 1) # avoids NaNs
                 predprob = float(expit(torch.mean(logit(subseq[idx:]))))
                 pred.append(predprob)
+                pred_allprob.append(subseq.tolist())
             prob_list.extend(pred)
+            prob_list_allprob.extend(pred_allprob)
         prob_arr = np.asarray(prob_list, dtype=float)
     else:
         for i in range(0, len(ORF_seq_sorted), gene_batch_size):
             batch = ORF_seq_sorted[i:i+gene_batch_size]
             seq_lengths = torch.LongTensor(list(map(len, batch)))
             seq_tensor = torch.zeros((len(batch), seq_lengths.max())).long()
             for idx, (seq, seqlen) in enumerate(zip(batch, seq_lengths)):
                 seq_tensor[idx, :seqlen] = torch.LongTensor(seq)
             pred_all = predict(seq_tensor, model, use_cpu)
             pred = []
+            pred_allprob = []
             for j, length in enumerate(seq_lengths):
                 subseq = pred_all[j, 0, 0:int(length)]
                 idx = min(100, int(length) - 1) # avoids NaNs
                 predprob = float(expit(torch.mean(logit(subseq[idx:]))))
                 pred.append(predprob)
+                pred_allprob.append(subseq.tolist())
             prob_list.extend(pred)
+            prob_list_allprob.extend(pred_allprob)
         prob_arr = np.asarray(prob_list, dtype=float)
 
     # unsort
     unsort_idx = np.argsort(length_idx)
     ORF_prob = prob_arr[unsort_idx]
-
-    return ORF_prob
+    
+    # unsort allprob, differing lengths mean this can't be a np array
+    ORF_prob_allprob = []
+    if allprob:
+        for idx in unsort_idx:
+            ORF_prob_allprob.append(prob_list_allprob[idx])
+    
+    return ORF_prob, ORF_prob_allprob
     
 def eye_of_psauron():
     # supress annoying warnings
     warnings.filterwarnings('ignore')
     
     # print PSAURON version
-    version = "1.0.0"
+    version = "1.0.2"
     print("PSAURON version", version)
     
     # parse command line arguments
     try:
         args = get_args()
     except:
         print("\n -i INPUT_FASTA, REQUIRED path to FASTA with spliced CDS sequence. This fasta can be created from a GTF/GFF and a reference FASTA by using gffread. \n\nExample gffread commands to get CDS FASTA:\ngffread -x CDS_FASTA.fa -g genome.fa input.gff\ngffread -x CDS_FASTA.fa -g genome.fa input.gtf\n")
         sys.exit()
     min_len_aa = args.minimum_length
     p_fasta = args.input_fasta
     use_cpu = args.use_cpu
+    allprob = args.all_prob
     verbose = args.verbose
     single_frame = args.single_frame
     protein = args.protein
     print("System info")
     print(sys.version, "\n")
     
     # check args
@@ -293,18 +308,19 @@
                 if not use_cpu:
                     print("Running TCN model on GPU...")
                 else:
                     print("Detected GPU, but running TCN model on CPU due to -c argument")
             else:
                 print("No GPU detected, running TCN model on CPU...")
             print("Scoring in-frame sequence...")
-            ORF_prob = score_seq(ORF_list_aa_flat_clean, model, use_cpu, verbose)
+            ORF_prob, ORF_prob_allprob = score_seq(ORF_list_aa_flat_clean, model, use_cpu, allprob, verbose)
             print("Scoring out-of-frame sequence...")
-            ARF_prob = score_seq(ARF_list_aa_flat_clean, model, use_cpu, verbose)
+            ARF_prob, ARF_prob_allprob = score_seq(ARF_list_aa_flat_clean, model, use_cpu, allprob, verbose)
             ARF_prob = [ARF_prob[i:i+5] for i in range(0, len(ARF_prob), 5)]    
+            ARF_prob_allprob = [ARF_prob_allprob[i:i+5] for i in range(0, len(ARF_prob_allprob), 5)]
             
             # create meta-score for each CDS
             ORF_bound = args.inframe # ORF must be >= ORF_bound
             ARF_bound = args.outframe # mean ARFs must be <= ARF_bound
             is_protein = []
             ORF_score_all = []
             ARF_score_all = []
@@ -356,15 +372,15 @@
                 if not use_cpu:
                     print("Running TCN model on GPU...")
                 else:
                     print("Detected GPU, but running TCN model on CPU due to -c argument")
             else:
                 print("No GPU detected, running TCN model on CPU...")
             print("Scoring in-frame sequence...")
-            ORF_prob = score_seq(ORF_list_aa_flat_clean, model, use_cpu, verbose)
+            ORF_prob, ORF_prob_allprob = score_seq(ORF_list_aa_flat_clean, model, use_cpu, allprob, verbose)
             
             # create score for each CDS
             ORF_bound = args.inframe # ORF must be >= ORF_bound
             is_protein = []
             ORF_score_all = []
             for i in range(0, len(ORF_prob)):
                 ORF_score = ORF_prob[i]
@@ -429,15 +445,15 @@
             if not use_cpu:
                 print("Running TCN model on GPU...")
             else:
                 print("Detected GPU, but running TCN model on CPU due to -c argument")
         else:
             print("No GPU detected, running TCN model on CPU...")
         print("Scoring in-frame sequence...")
-        ORF_prob = score_seq(ORF_list_aa_flat_clean, model, use_cpu, verbose)
+        ORF_prob, ORF_prob_allprob = score_seq(ORF_list_aa_flat_clean, model, use_cpu, allprob, verbose)
         
         # create score for each CDS
         ORF_bound = args.inframe # ORF must be >= ORF_bound
         is_protein = []
         ORF_score_all = []
         for i in range(0, len(ORF_prob)):
             ORF_score = ORF_prob[i]
@@ -453,45 +469,87 @@
     # print final score
     ss = round(sum(is_protein)/len(is_protein) * 100, 1)
     
     # ALL FRAMES, DEFAULT BEHAVIOR
     if not single_frame and not protein:
         print("\npsauron score:", ss)
         print("\nWriting detailed output file to", p_out)
+        if allprob:
+            print("NOTE: all_prob cells in .csv output may exceed Microsoft Excel max cell size limit")
+
         cols = ["description", "psauron_is_protein", "in_frame_score",
                 "forward_frame2_score", "forward_frame3_score", 
                 "reverse_frame1_score", "reverse_frame2_score", 
                 "reverse_frame3_score", "mean_out_of_frame_score"]
+        if allprob:
+            cols.extend(["in_frame_all_prob", "forward_frame2_all_prob",
+                         "forward_frame3_all_prob", "reverse_frame1_all_prob",
+                         "reverse_frame2_all_prob", "reverse_frame3_all_prob"])   
+             
         header = " ".join(sys.argv) + "\n" + "psauron score: " + str(ss) + "\nNOTE: alternate reading frames may not contain valid ORFs"
         with open(p_out, "wt") as f:
             f.write(header + "\n")
             f.write(",".join(cols) + "\n")
             for i, desc in enumerate(description_list_clean):
-                # removes all "," in data to avoid .csv errors
-                f.write(",".join([str(x).replace(",", "") for x in [desc, 
-                                                                    is_protein[i],
-                                                                    round(ORF_score_all[i], 5),
-                                                                    round(ARF_score_all[i][0], 5),
-                                                                    round(ARF_score_all[i][1], 5),
-                                                                    round(ARF_score_all[i][2], 5),
-                                                                    round(ARF_score_all[i][3], 5),
-                                                                    round(ARF_score_all[i][4], 5),
-                                                                    round(ARF_score_mean_all[i], 5)]]))
-                f.write("\n")
+                if allprob:
+                    # remove all "," in data to avoid .csv errors
+                    f.write(",".join([str(x).replace(",", "") for x in [desc, 
+                                                                        is_protein[i],
+                                                                        round(ORF_score_all[i], 5),
+                                                                        round(ARF_score_all[i][0], 5),
+                                                                        round(ARF_score_all[i][1], 5),
+                                                                        round(ARF_score_all[i][2], 5),
+                                                                        round(ARF_score_all[i][3], 5),
+                                                                        round(ARF_score_all[i][4], 5),
+                                                                        round(ARF_score_mean_all[i], 5),
+                                                                        ";".join([str(round(x,2)) for x in ORF_prob_allprob[i]]),
+                                                                        ";".join([str(round(x,2)) for x in ARF_prob_allprob[i][0]]),
+                                                                        ";".join([str(round(x,2)) for x in ARF_prob_allprob[i][1]]),
+                                                                        ";".join([str(round(x,2)) for x in ARF_prob_allprob[i][2]]),
+                                                                        ";".join([str(round(x,2)) for x in ARF_prob_allprob[i][3]]),
+                                                                        ";".join([str(round(x,2)) for x in ARF_prob_allprob[i][4]]),
+                                                                        ]]))
+                    f.write("\n")
+                else:
+                    # remove all "," in data to avoid .csv errors
+                    f.write(",".join([str(x).replace(",", "") for x in [desc, 
+                                                                        is_protein[i],
+                                                                        round(ORF_score_all[i], 5),
+                                                                        round(ARF_score_all[i][0], 5),
+                                                                        round(ARF_score_all[i][1], 5),
+                                                                        round(ARF_score_all[i][2], 5),
+                                                                        round(ARF_score_all[i][3], 5),
+                                                                        round(ARF_score_all[i][4], 5),
+                                                                        round(ARF_score_mean_all[i], 5)]]))
+                    f.write("\n")
     
     else:
         print("\npsauron score:", ss)
         print("\nWriting detailed output file to", p_out)
+        if allprob:
+            print("NOTE: all_prob cells in .csv output may exceed Microsoft Excel max cell size limit")
+        
         cols = ["description", "psauron_is_protein", "in-frame_score"]
+        if allprob:
+            cols.extend(["in_frame_all_prob"])
+                         
         header = " ".join(sys.argv) + "\n" + "psauron score: " + str(ss)
         with open(p_out, "wt") as f:
             f.write(header + "\n")
             f.write(",".join(cols) + "\n")
             for i, desc in enumerate(description_list_clean):
-                # removes all "," in data to avoid .csv errors
-                f.write(",".join([str(x).replace(",", "") for x in [desc, 
-                                                                    is_protein[i],
-                                                                    round(ORF_score_all[i], 5)]]))
-                f.write("\n")
+                if allprob:
+                    # removes all "," in data to avoid .csv errors
+                    f.write(",".join([str(x).replace(",", "") for x in [desc, 
+                                                                        is_protein[i],
+                                                                        round(ORF_score_all[i], 5),
+                                                                        ";".join([str(round(x,2)) for x in ORF_prob_allprob[i]])]]))
+                    f.write("\n")
+                else:
+                    # removes all "," in data to avoid .csv errors
+                    f.write(",".join([str(x).replace(",", "") for x in [desc, 
+                                                                        is_protein[i],
+                                                                        round(ORF_score_all[i], 5)]]))
+                    f.write("\n")
     
     print("Done")
```

### Comparing `psauron-1.0.0/setup.py` & `psauron-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
     
 setup(
     name="psauron",
-    version="1.0.0",
+    version="1.0.2",
     description="A tool to assess protein coding gene annotation",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Markusjsommer/psauron",
     author="markus",
     author_email = "markusjsommer@gmail.com",
@@ -24,17 +24,18 @@
                       "torchvision>=0.16.2",
                       "torchaudio>=2.1.2",
                       "typing-extensions>=4.9.0",
                       "tqdm>=4.66.1",
                       "scipy>=1.10.1",
                       "biopython>=1.83",
                       "numpy>=1.24.4",
-                      "pandas>=2.0.3"],
+                      "pandas>=2.0.3",
+                      "setuptools"],
     extras_require={
-        "dev": ["pytest>=7.0", "twine>=4.0.2", "pytest-cov>=4.0"],
+        "dev": ["pytest>=7.0", "twine>=4.0.2", "pytest-cov>=4.0", "wheel"],
     },
     python_requires=">=3.8",
     entry_points={
         'console_scripts': [
             'psauron = app.psauron:eye_of_psauron',
         ],
     },
```

### Comparing `psauron-1.0.0/tests/test_eye_of_psauron.py` & `psauron-1.0.2/tests/test_eye_of_psauron.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,8 +56,13 @@
     with unittest.mock.patch('sys.argv', ['psauron']):
         with pytest.raises(SystemExit):
             eye_of_psauron()
             
 def test_eye_of_psauron_badargs2():
     with unittest.mock.patch('sys.argv', ['psauron', '-i', 'tests/seq_test_CDS.fa', '-p', '-s']):
         with pytest.raises(SystemExit):
+            eye_of_psauron()
+            
+def test_eye_of_psauron_allprob():
+    with unittest.mock.patch('sys.argv', ['psauron', '-i', 'tests/seq_test_CDS.fa', '-p', '-s', '-a']):
+        with pytest.raises(SystemExit):
             eye_of_psauron()
```

