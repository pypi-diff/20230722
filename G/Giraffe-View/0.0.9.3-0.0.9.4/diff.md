# Comparing `tmp/Giraffe_View-0.0.9.3.tar.gz` & `tmp/Giraffe_View-0.0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Giraffe_View-0.0.9.3.tar", last modified: Fri Jul 21 10:04:50 2023, max compression
+gzip compressed data, was "Giraffe_View-0.0.9.4.tar", last modified: Sat Jul 22 12:04:04 2023, max compression
```

## Comparing `Giraffe_View-0.0.9.3.tar` & `Giraffe_View-0.0.9.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-21 10:04:50.670559 Giraffe_View-0.0.9.3/
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-21 10:04:50.670559 Giraffe_View-0.0.9.3/Giraffe_View/
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       57 2023-07-21 09:58:31.000000 Giraffe_View-0.0.9.3/Giraffe_View/__init__.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2835 2023-07-21 09:58:31.000000 Giraffe_View-0.0.9.3/Giraffe_View/estimated_read_accuracy.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4539 2023-07-21 09:58:31.000000 Giraffe_View-0.0.9.3/Giraffe_View/function.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3288 2023-07-21 09:58:31.000000 Giraffe_View-0.0.9.3/Giraffe_View/gc_bias.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4357 2023-07-21 09:58:31.000000 Giraffe_View-0.0.9.3/Giraffe_View/giraffe
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4721 2023-07-21 09:58:31.000000 Giraffe_View-0.0.9.3/Giraffe_View/homopolymer.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     2944 2023-07-21 09:58:31.000000 Giraffe_View-0.0.9.3/Giraffe_View/observed_read_accuracy.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4591 2023-07-21 09:57:39.000000 Giraffe_View-0.0.9.3/Giraffe_View/plot.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2156 2023-07-21 09:58:31.000000 Giraffe_View-0.0.9.3/Giraffe_View/regional_modification.py
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-21 10:04:50.670559 Giraffe_View-0.0.9.3/Giraffe_View.egg-info/
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5057 2023-07-21 10:04:50.000000 Giraffe_View-0.0.9.3/Giraffe_View.egg-info/PKG-INFO
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      466 2023-07-21 10:04:50.000000 Giraffe_View-0.0.9.3/Giraffe_View.egg-info/SOURCES.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2023-07-21 10:04:50.000000 Giraffe_View-0.0.9.3/Giraffe_View.egg-info/dependency_links.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       71 2023-07-21 10:04:50.000000 Giraffe_View-0.0.9.3/Giraffe_View.egg-info/requires.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       13 2023-07-21 10:04:50.000000 Giraffe_View-0.0.9.3/Giraffe_View.egg-info/top_level.txt
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1064 2023-07-21 09:58:42.000000 Giraffe_View-0.0.9.3/LICENSE
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5057 2023-07-21 10:04:50.670559 Giraffe_View-0.0.9.3/PKG-INFO
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     4662 2023-07-21 09:58:42.000000 Giraffe_View-0.0.9.3/README.md
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2023-07-21 10:04:50.670559 Giraffe_View-0.0.9.3/setup.cfg
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)      940 2023-07-21 09:59:40.000000 Giraffe_View-0.0.9.3/setup.py
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-22 12:04:04.872175 Giraffe_View-0.0.9.4/
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-22 12:04:04.868175 Giraffe_View-0.0.9.4/Giraffe_View/
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       57 2023-07-22 06:47:12.000000 Giraffe_View-0.0.9.4/Giraffe_View/__init__.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2838 2023-07-22 11:58:17.000000 Giraffe_View-0.0.9.4/Giraffe_View/estimated_read_accuracy.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4755 2023-07-22 11:58:35.000000 Giraffe_View-0.0.9.4/Giraffe_View/function.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3287 2023-07-22 11:58:52.000000 Giraffe_View-0.0.9.4/Giraffe_View/gc_bias.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5819 2023-07-22 12:00:28.000000 Giraffe_View-0.0.9.4/Giraffe_View/giraffe
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4752 2023-07-22 12:01:18.000000 Giraffe_View-0.0.9.4/Giraffe_View/homopolymer.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     2953 2023-07-22 07:03:46.000000 Giraffe_View-0.0.9.4/Giraffe_View/observed_read_accuracy.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     8167 2023-07-22 10:55:54.000000 Giraffe_View-0.0.9.4/Giraffe_View/plot.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2157 2023-07-22 09:24:19.000000 Giraffe_View-0.0.9.4/Giraffe_View/regional_modification.py
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-22 12:04:04.872175 Giraffe_View-0.0.9.4/Giraffe_View.egg-info/
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5285 2023-07-22 12:04:04.000000 Giraffe_View-0.0.9.4/Giraffe_View.egg-info/PKG-INFO
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      466 2023-07-22 12:04:04.000000 Giraffe_View-0.0.9.4/Giraffe_View.egg-info/SOURCES.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2023-07-22 12:04:04.000000 Giraffe_View-0.0.9.4/Giraffe_View.egg-info/dependency_links.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       88 2023-07-22 12:04:04.000000 Giraffe_View-0.0.9.4/Giraffe_View.egg-info/requires.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       13 2023-07-22 12:04:04.000000 Giraffe_View-0.0.9.4/Giraffe_View.egg-info/top_level.txt
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1064 2023-07-22 06:47:12.000000 Giraffe_View-0.0.9.4/LICENSE
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5285 2023-07-22 12:04:04.872175 Giraffe_View-0.0.9.4/PKG-INFO
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     4875 2023-07-22 11:56:21.000000 Giraffe_View-0.0.9.4/README.md
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2023-07-22 12:04:04.872175 Giraffe_View-0.0.9.4/setup.cfg
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)      965 2023-07-22 12:03:15.000000 Giraffe_View-0.0.9.4/setup.py
```

### Comparing `Giraffe_View-0.0.9.3/Giraffe_View/estimated_read_accuracy.py` & `Giraffe_View-0.0.9.4/Giraffe_View/estimated_read_accuracy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,45 @@
 import numpy as np
 import math
 import multiprocessing
 
 def calculate_read_accuracy(string):
     """
     Calculate the estimated accuracy for a given string.
-
     Parameters:
     string (str): A string of bases in ASCII format.
-
     Returns:
     list: A list containing the estimated accuracy, error proportion, and Q-value.
     """
     error_list = []
     for base_value in string:
         ascii_value = ord(base_value) - 33
         error_proporation = math.pow(10, (-1) * int(ascii_value) / 10)
         error_list.append(error_proporation)
     error_mean = np.mean(error_list)
     return [1 - error_mean, error_mean, (-10) * math.log10(error_mean)]
 
 def process_chunk(chunk):
     """
     Process a chunk of reads.
-
     Parameters:
     chunk (list): A list of reads.
-
     Returns:
     list: A list containing the estimated accuracy, error proportion, and Q-value for each read in the chunk.
     """
     results = []
     for line in chunk:
         read_id, quality = line
         quality = calculate_read_accuracy(quality)
         results.append([read_id, quality[0], quality[1], quality[2]])
     return results
 
 def calculate_estimated_accuracy(input_file, num_processes, chunk_size=1000):
     """
     Calculate the estimated accuracy for each read in an input file and write the results to an output file.
-
     Parameters:
     input_file (str): The path to the input file.
     output_file (str): The path to the output file.
     num_processes (int): The number of processes to use for multiprocessing.
     chunk_size (int): The size of the chunks to split the input file into.
     """
     pool = multiprocessing.Pool(processes=num_processes)
@@ -69,14 +64,14 @@
                 results.append(pool.apply_async(process_chunk, (chunk,)))
                 chunk = []
         if len(chunk) > 0:
             results.append(pool.apply_async(process_chunk, (chunk,)))
     pool.close()
     pool.join()
 
-    output_file = open("results/estimated/final_estimated_accuracy.txt", "w")
+    output_file = open("results/estimated_quality/final_estimated_accuracy.txt", "w")
     # with open("result/estimated/estimated_accuracy.txt", "w") as output_file:
     output_file.write("ID\tacc\terror\tQ_value\n")
     for result in results:
         for line in result.get():
             message = f"{line[0]}\t{line[1]}\t{line[2]}\t{line[3]}"
             output_file.write(message + "\n")
```

### Comparing `Giraffe_View-0.0.9.3/Giraffe_View/function.py` & `Giraffe_View-0.0.9.4/Giraffe_View/function.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 import subprocess
 import re
 import os
+from termcolor import colored
 from subprocess import Popen, PIPE
 
+def print_with_color(input_string):
+    print(colored(input_string, "green"))
+
+def error_with_color(input_string):
+    print(colored(input_string, "red"))
 
 def cmd_shell(cammands, string):
     process = Popen(cammands.split(' '), stdout=subprocess.DEVNULL, universal_newlines=True)
     process.wait()
     err = process.communicate()
 
     if process.returncode == 0:
-        print('{} SUCCESS'.format(string))
+        # print('{} SUCCESS'.format(string))
+        pass
     else:
-        print('{} FAILED'.format(string))
-        print(err)
+        # print('{} FAILED'.format(string))
+        error_with_color(err)
 
 def Data_process(read, ref, threads=10):
     # Define the commands as a list of strings to avoid issues with spaces
     # in file names or command arguments
     # path =  os.getcwd()
-    cmd0 = ["mkdir", "-p", "results/quality"]
-    cmd1 = ["seqkit", "seq", read, "-m", "200", "-Q", "7", "-g", "-j", str(threads), "-o", "results/quality/clean.fastq"]
-    cmd2 = ["minimap2", "-ax", "map-ont", "-o", "results/quality/tmp.sam", "--MD", "--secondary=no", "-L", "-t", str(threads), ref, "results/quality/clean.fastq"]
-    cmd3 = ["samtools", "view", "-bS", "-F4", "-@", str(threads), "-o", "results/quality/tmp.bam", "results/quality/tmp.sam"]
-    cmd4 = ["samtools", "sort", "-@", str(threads), "-o", "results/quality/tmp.sort.bam", "results/quality/tmp.bam"]
-    cmd5 = ["samtools", "index", "-@", str(threads), "results/quality/tmp.sort.bam"]
-    cmd6 = ["rm", "-rf", "results/quality/tmp.sam", "results/quality/tmp.bam"]
+    cmd0 = ["mkdir", "-p", "results/observed_quality"]
+    cmd1 = ["seqkit", "seq", read, "-m", "200", "-Q", "7", "-g", "-j", str(threads), "-o", "results/observed_quality/clean.fastq"]
+    cmd2 = ["minimap2", "-ax", "map-ont", "-o", "results/observed_quality/tmp.sam", "--MD", "--secondary=no", "-L", "-t", str(threads), ref, "results/observed_quality/clean.fastq"]
+    cmd3 = ["samtools", "view", "-bS", "-F4", "-@", str(threads), "-o", "results/observed_quality/tmp.bam", "results/observed_quality/tmp.sam"]
+    cmd4 = ["samtools", "sort", "-@", str(threads), "-o", "results/observed_quality/tmp.sort.bam", "results/observed_quality/tmp.bam"]
+    cmd5 = ["samtools", "index", "-@", str(threads), "results/observed_quality/tmp.sort.bam"]
+    cmd6 = ["rm", "-rf", "results/observed_quality/tmp.sam", "results/observed_quality/tmp.bam"]
 
     # Run each command and check the return code
     for i, cmd in enumerate([cmd0, cmd1, cmd2, cmd3, cmd4, cmd5, cmd6]):
         try:
             subprocess.run(cmd, check=True)
-            print("Command {} succeeded".format(i + 1))
+            # print("Command {} succeeded".format(i + 1))
         except subprocess.CalledProcessError as e:
             print("Command {} failed with error code {}".format(i + 1, e.returncode))
             print(e.output)
             # Raise an exception to indicate that processing failed
             raise Exception("Data processing failed")
 
 def mkdir_d(input_name):
@@ -76,16 +83,14 @@
     elif (len(remove_cigarstring) == 1) and (input_cigar[-1] != "S") or ((len(remove_cigarstring) == 2) and (remove_cigarstring[0][-1] == "S") and (remove_cigarstring[1][-1] == "H")):
         remove_start_site = int(remove_cigarstring[0][:-1])
         valid_pairs = input_pairs[remove_start_site:]
     else:
         print(str(input_ID) + ", please recheck this CIGAR and MD!")
     return(valid_pairs)
 
-
-
 """
 only for base A T G C
 (read_position, ref_position, "ref_base")
 none    √   √   Deletion(D)
 √   none    none Insertion(I)
 √   √   N(A,T,G,C)  Match(M)
 √   √   n(a,t,g,c)  Substitution(S)
@@ -99,13 +104,8 @@
         if input_list[1] == None:
             result = "I" # I = insertion
         else:
             if input_list[2] in map_list:
                 result = "M" # M = match
             else:
                 result =  "S" # S = substitution
-    return result
-
-
-# def Rplot(plotR):
-#     cmd = ["Rscript", str(plotR)]
-#     subprocess.run(cmd, check=True)
+    return result
```

### Comparing `Giraffe_View-0.0.9.3/Giraffe_View/gc_bias.py` & `Giraffe_View-0.0.9.4/Giraffe_View/gc_bias.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -108,8 +108,8 @@
 				start -= 1
 				end += 1
 				continue
 
 	# normalization
 	ave_dp = nor_df["dp"].mean()
 	nor_df["nor_dp"] = nor_df.apply(lambda row: row["dp"]/ave_dp, axis=1)
-	nor_df.to_csv("results/GC_bias/final_GC_bias_nor.txt", sep="\t", index=False)
+	nor_df.to_csv("results/GC_bias/final_GC_bias_nor.txt", sep="\t", index=False)
```

### Comparing `Giraffe_View-0.0.9.3/Giraffe_View/giraffe` & `Giraffe_View-0.0.9.4/Giraffe_View/giraffe`

 * *Files 23% similar despite different names*

```diff
@@ -1,103 +1,134 @@
 #!/usr/bin/env python
 import sys
 import argparse
+import pathlib
+
 from Giraffe_View.function import *
 from Giraffe_View.homopolymer import *
 from Giraffe_View.observed_read_accuracy import *
 from Giraffe_View.gc_bias import *
 from Giraffe_View.estimated_read_accuracy import *
 from Giraffe_View.regional_modification import *
 from Giraffe_View.plot import *
 
+working_path = pathlib.Path().resolve()
+
 def observed(args):
+    print_with_color("Start data processing!")
     Data_process(args.input, args.ref, args.cpu)
-    print("Start observed accuracy analysis!")
-    observed_accuracy("results/quality/tmp.sort.bam")
-    print("Start homopolymer identification!")
-
-    homopolymer_from_bam("results/quality/tmp.sort.bam")
-    homopolymer_summary_1("results/quality/homo.txt")
+    
+    print_with_color("Start observed accuracy analysis!")
+    observed_accuracy("results/observed_quality/tmp.sort.bam")
+    
+    print_with_color("Start homopolymer identification!")
+    homopolymer_from_bam("results/observed_quality/tmp.sort.bam")
+    homopolymer_summary_1("results/observed_quality/homo.txt")
     homopolymer_summary_2()
     
     if args.plot:
-        print("Start plotting!")
+        print_with_color("Start plotting!")
         plot_observe()
-        print("Analysis finished!")
+        print_with_color("Observe read quality analysis finished!")
     else:
-        print("Analysis finished!")
-
+        print_with_color("Observe read quality analysis finished!")
+    
+    mes = "The results are available at " + str(working_path) + "/results/observed_quality!"
+    print_with_color(str(mes))
 
-def methylation(args):
-    mkdir_d("regional_modification")
-    methylation_calculation(args.input, args.ref, args.cpu)
+def estimated(args):
+    mkdir_d("estimated_quality")
 
+    print_with_color("Start estimated read accuracy analysis!")
+    calculate_estimated_accuracy(args.input, args.cpu)
+    
+    if args.plot:
+        print_with_color("Start plotting!")
+        plot_estimate()
+        print_with_color("Analysis finished!")
+    else:
+        print_with_color("Analysis finished!")
+    
+    mes = "The results are available at " + str(working_path) + "/results/estimated_quality!"
+    print_with_color(str(mes))
 
 def GC_bias(args):
     mkdir_d("GC_bias")
+    print_with_color("Start GC bias analysis!")
     compute_GC_bias(args.ref, args.input, args.binsize)
     merge_CG_content_and_depth(args.binsize)
 
     if args.plot:
-        print("Start plotting!")
+        print_with_color("Start plotting!")
         plot_GC_bias()
-        print("Analysis finished!")
+        print_with_color("Analysis finished!")
     else:
-        print("Analysis finished!")
-
-def estimated(args):
-    mkdir_d("estimated")
-    calculate_estimated_accuracy(args.input, args.cpu)
+        print_with_color("Analysis finished!")
     
+    mes = "The results are available at " + str(working_path) + "/results/GC_bias!"
+    print_with_color(str(mes))
+
+def methylation(args):
+    mkdir_d("regional_modification")
+    print_with_color("Start calculating the modification bin analysis!")
+    methylation_calculation(args.input, args.ref, args.cpu)
+
     if args.plot:
-        print("Start plotting!")
-        plot_estimate()
-        print("Analysis finished!")
+        print_with_color("Start plotting!")
+        plot_modi_bin(args.input, args.ref)
+        print_with_color("Analysis finished!")
     else:
-        print("Analysis finished!")
+        print_with_color("Analysis finished!")
+
+    mes = "The results are available at " + str(working_path) + "/results/regional_modification!"
+    print_with_color(str(mes))
+
+
+
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(prog="giraffe", description="A tool to help you assess quality of ONT data.")
 
     # Define subparsers
     subparsers = parser.add_subparsers(dest='function', help="")
-    observed_parser = subparsers.add_parser('observe', help='Observed quality in accuracy, mismatch, and homopolymer')
+    observed_parser = subparsers.add_parser('observe', help='Observed quality in accuracy, mismatch, and homopolymer identification')
     observed_parser.add_argument("--input", type=str, metavar="<fastq>", required=True, help="input reads")
     observed_parser.add_argument("--ref", type=str, metavar="<reference>", required=True, help="input reference")
     observed_parser.add_argument("--cpu", type=int, metavar="<number>", required=False, help="number of cpu (default:10)", default=10)
     observed_parser.add_argument("--plot", required=False, help="Results visualization", action='store_true')
 
     estimated_parser = subparsers.add_parser('estimate', help='Estimated read accuracy')
     estimated_parser.add_argument("--input", type=str, metavar="<fastq>", required=True, help="input reads")
     estimated_parser.add_argument("--cpu", type=int, metavar="<number>", required=False, help="number of cpu (default:10)", default=10)
     estimated_parser.add_argument("--plot", required=False, help="Results visualization", action='store_true')
 
-    methylation_parser = subparsers.add_parser('modi', help='Average modification proportion of regions')
-    methylation_parser.add_argument("--input", type=str, metavar="<bed>", required=True, help="input bed file")
-    methylation_parser.add_argument("--ref", type=str, metavar="<reference>", required=True, help="input reference")
-    methylation_parser.add_argument("--cpu", type=int, metavar="<number>", required=False, help="number of cpu (default:10)", default=10)
-
     GC_bias_parser = subparsers.add_parser('gc_bias', help='Relationship between GC content and depth')
     GC_bias_parser.add_argument("--ref", type=str, metavar="<reference>", required=True, help="input reference file")
     GC_bias_parser.add_argument("--input", type=str, metavar="<sam/bam>", required=True, help="input bam/sam file")
     GC_bias_parser.add_argument("--binsize", type=int, metavar="", required=False, help="input bin size (default:1000)", default=1000)
     GC_bias_parser.add_argument("--plot", required=False, help="Results visualization", action='store_true')
 
+    methylation_parser = subparsers.add_parser('modi_bin', help='Average modification proportion of bins')
+    methylation_parser.add_argument("--input", type=str, metavar="<bed>", required=True, help="input modificated bed file, please use the .bed as the file suffix")
+    methylation_parser.add_argument("--ref", type=str, metavar="<reference>", required=True, help="input position file with CSV format, please use the .csv as the file suffix")
+    methylation_parser.add_argument("--cpu", type=int, metavar="<number>", required=False, help="number of cpu (default:10)", default=10)
+    methylation_parser.add_argument("--plot", required=False, help="Results visualization", action='store_true')
+
     # Add function to print help if no arguments are provided
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
         sys.exit(1)
 
     args = parser.parse_args()
 
     # Call the appropriate function based on the subparser used
     if args.function == "observe":
         observed(args)
 
-    elif args.function == "modi":
+    elif args.function == "modi_bin":
         methylation(args)
 
     elif args.function == "gc_bias":
         GC_bias(args)
 
     elif args.function == "estimate":
-        estimated(args)
+        estimated(args)
```

### Comparing `Giraffe_View-0.0.9.3/Giraffe_View/homopolymer.py` & `Giraffe_View-0.0.9.4/Giraffe_View/homopolymer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import pandas as pd
 import pysam
 import re
-from Giraffe_View.function import *
 import multiprocessing
-
+from Giraffe_View.function import *
 
 def homopolymer_from_bam(input_bamfile):
 	bamfile = pysam.AlignmentFile(input_bamfile, threads=4)
 	dir_polymer = {}
 
 	for read in bamfile:
 		read_ID = read.query_name
@@ -47,15 +46,15 @@
 							count += 1
 						del homoploymer_ref_pos[:]
 						homoploymer_ref = str(base[2]).upper()
 						homoploymer_read = str(get_base_alignment(base))
 						homoploymer_ref_pos.append(base[1])
 	bamfile.close()
 
-	ff = open("results/quality/homo.txt", "w")
+	ff = open("results/observed_quality/homo.txt", "w")
 	for read in dir_polymer.keys():
 		for n in dir_polymer[read].keys():
 			stat_info = count_indel_and_snv(str(dir_polymer[read][n][1]))
 
 			if "M" not in stat_info.keys():
 				stat_info["M"] = 0
 			if "D" not in stat_info.keys():
@@ -68,16 +67,14 @@
 			mes = str(dir_polymer[read][n][2]) + "\t" +  str(dir_polymer[read][n][3]) + "\t" + str(dir_polymer[read][n][-1]) + "\t" # chr start end
 			mes += str(dir_polymer[read][n][0][:-1]) + "\t" + str(dir_polymer[read][n][0][-1]) + "\t"  #  4 A
 			mes += str(stat_info["M"]) + "\t" + str(stat_info["D"]) + "\t" + str(stat_info["I"]) + "\t" + str(stat_info["S"])  + "\t"  # map del ins sub
 			mes += str(read)
 			ff.write(mes + "\n")
 	ff.close()
 
-
-
 def homopolymer_summary_1(input_file):
 	data = {}
 	with open(input_file) as ff:
 		for line in ff:
 			line = line.replace("\n", "")
 			line = line.split("\t")
 			position = line[0] + "_" + line[1] + "_" + line[2]
@@ -93,29 +90,28 @@
 
 			elif position in data.keys():
 				data[position]["depth"] += 1
 				if int(line[3]) == int(line[5]):
 					data[position]["mat"] += 1
 	ff.close()
 
-	ff = open("results/quality/homo_tmp.txt", "w")
+	ff = open("results/observed_quality/homo_tmp.txt", "w")
 	ff.write("pos\tnum_of_mat\tdepth\ttype\n")   
 
 	for i in data.keys():
 		mes = str(i) + "\t" + str(data[i]["mat"]) + "\t" + str(data[i]["depth"]) + "\t" + data[i]["type"]
 		ff.write(mes + "\n")
 	ff.close()
 
-
 def homopolymer_summary_2():
-	data = pd.read_table("results/quality/homo_tmp.txt", sep="\t")	
+	data = pd.read_table("results/observed_quality/homo_tmp.txt", sep="\t")	
 	valid = data[data["depth"] >= 3].copy()
 
 	if len(valid) != 0:
-		ff = open("results/quality/final_homo_summary.txt", "w")
+		ff = open("results/observed_quality/final_homo_summary.txt", "w")
 		ff.write("base\tvalue\n")
 
 		valid["rate"] = valid["num_of_mat"] / valid["depth"]
 		
 		def Abase(x):
 			if re.search(".*A", x): 
 				return(True)
@@ -142,8 +138,8 @@
 		
 		ff.write("T\t" + str(valid[valid["type"].apply(Tbase)]["rate"].mean()) + "\n")
 		ff.write("G\t" + str(valid[valid["type"].apply(Gbase)]["rate"].mean()) + "\n")
 		ff.write("A\t" + str(valid[valid["type"].apply(Abase)]["rate"].mean()) + "\n")
 		ff.write("C\t" + str(valid[valid["type"].apply(Cbase)]["rate"].mean()) + "\n")
 		ff.close()
 	else:
-		print("The read coverage of data was shallow, homopolymer analysis failed!!!")
+		print("The read coverage of data was shallow, homopolymer analysis failed!!!")
```

### Comparing `Giraffe_View-0.0.9.3/Giraffe_View/observed_read_accuracy.py` & `Giraffe_View-0.0.9.4/Giraffe_View/observed_read_accuracy.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 def observed_accuracy(bam_file):
     """
     Calculates the observed accuracy, insertion, deletion, substitution, match,
     and identity rates for each read in a BAM file.
     """
     quality = {}
-    with open("results/quality/final_observed_accuracy.txt", "w") as outfile:  
+    with open("results/observed_quality/final_observed_accuracy.txt", "w") as outfile:  
         outfile.write("ID\tIns\tDel\tSub\tMat\tIden\tAcc\n")
 
         bamfile= pysam.AlignmentFile(bam_file, 'rb')
         for read in bamfile:
                 # Skip reads with unmapped or secondary alignments
                 # if int(read.flag) not in [0, 16]:
                 #     continue
```

### Comparing `Giraffe_View-0.0.9.3/Giraffe_View/regional_modification.py` & `Giraffe_View-0.0.9.4/Giraffe_View/regional_modification.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         for l in ff:
             inqueue.put(l.strip())
 
     for i in range(process_num):
         inqueue.put("STOP")
 
     stop_count = 0
-    with tqdm(total=total, desc=input_file) as pbar, open(f"results/regional_modification/{input_file.replace('.bed', '')}_{input_ref.replace('.db', '')}.bed", "w") as of:
+    with tqdm(total=total, desc=input_file) as pbar, open(f"results/regional_modification/{input_file.replace('.bed', '')}_{input_ref.replace('.csv', '')}.bed", "w") as of:
         while stop_count < process_num:
             pbar.update()
             result = outqueue.get()
             if len(result) == 2:
                 of.write(f"{result[0]}\t{result[1]}\n")
             elif result[-4:] == "BYE!":
                 stop_count += 1
```

### Comparing `Giraffe_View-0.0.9.3/Giraffe_View.egg-info/PKG-INFO` & `Giraffe_View-0.0.9.4/Giraffe_View.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Giraffe-View
-Version: 0.0.9.3
+Version: 0.0.9.4
 Summary: A small tool help assess and visualize the accuracy of a sequencing dataset,   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.
 Home-page: https://github.com/lxd98/Giraffe_View
 Author: Xudong Liu
 Author-email: xudongliu98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,170 +15,155 @@
 # Giraffe_View 
 
 **Giraffe_View** is designed to help assess and visualize the accuracy of a sequencing dataset, specifically for Oxford Nanopore Technologies (ONT) long-read sequencing including DNA and RNA data. There are four main functions to validate the read quality.
 
 - `observe`  calculates the observed read accuracy, mismatches porportion, and homopolymer identification.
 - `estimate`  calculates the estimated read accuracy, which is equal to Quality Score.
 - `gc_bias`  compares the relationship between GC content and read coverage.
-- `modi` perform statistics on the distribution of modification based on the bed file.
+- `modi_bin` perform statistics on the distribution of modification based on the bed file.
 
 
 
 ## Install
 
-To use this software, you need to install additional dependencies including samtools, minimap2, and seqkit for read processing and ggplot2 and patchwork for figure plotting.
-
-The following commands can help you to install the package  and dependencies.
+To use this software, you need to install additional dependencies including samtools, minimap2, seqkit, and bedtools for read processing. The following commands can help you to install the package  and dependencies.
 
 ```shell
 pip install Giraffe-View
-
 conda install -c bioconda -c conda-forge samtools minimap2 seqkit bedtools -y
-conda install -c conda-forge r-ggplot2 r-patchwork -y
 ```
 
 
 
 ## General Usage
 
 Giraffe View is run simply with fllowing commands:
 
-```shell
-giraffe -h
 ```
+giraffe -h
+usage: giraffe [-h] {observe,estimate,gc_bias,modi_bin} ...
 
-```shell
-usage: giraffe [-h] {observe,modi,gc_bias,estimate} ...
-
-A tool to help you assess quality of your ONT data.
+A tool to help you assess quality of ONT data.
 
 positional arguments:
-  {observe,modi,gc_bias,estimate}
-    observe             Observed quality in accuracy, mismatch, and homopolymer
-    modi                Average modification proportion of regions
-    gc_bias             Relationship between GC content and depth
+  {observe,estimate,gc_bias,modi_bin}
+    observe             Observed quality in accuracy, mismatch, and homopolymer identification
     estimate            Estimated read accuracy
+    gc_bias             Relationship between GC content and depth
+    modi_bin            Average modification proportion of bins
 
 optional arguments:
   -h, --help            show this help message and exit
 ```
 
 
 
 The available sub-commands are:
 
-### observe
+#### observe
 
-```shell
-giraffe observe -h
 ```
-
-```xshell
-usage: giraffe observe [-h] --input <fastq> --ref <reference> [--cpu <number>]
+giraffe observe -h
+usage: giraffe observe [-h] --input <fastq> --ref <reference> [--cpu <number>] [--plot]
 
 optional arguments:
   -h, --help         show this help message and exit
   --input <fastq>    input reads
   --ref <reference>  input reference
   --cpu <number>     number of cpu (default:10)
+  --plot             Results visualization
 ```
 
 - `fastq` - the raw fastq data, some filter steps will be conducted including short read ( < 200 bp) and low quality read ( < 7 ) removal.
 - `reference` - the reference file in fasta format.
 - `cpu` - the number of CPUs will be used during processing.
 
 
 
-### estimate  
+#### estimate  
 
-```shell
-giraffe estimate -h
 ```
-
-```shell
-usage: giraffe estimate [-h] --input <fastq> [--cpu <number>]
+giraffe estimate -h
+usage: giraffe estimate [-h] --input <fastq> [--cpu <number>] [--plot]
 
 optional arguments:
   -h, --help       show this help message and exit
   --input <fastq>  input reads
   --cpu <number>   number of cpu (default:10)
+  --plot           Results visualization
 ```
 
 
 
-### gc_bias
+#### gc_bias
 
-```shell
-giraffe gc_bias -h
 ```
-
-```shell
-usage: giraffe gc_bias [-h] --ref <reference> --input <sam/bam> [--binsize]
+giraffe gc_bias -h
+usage: giraffe gc_bias [-h] --ref <reference> --input <sam/bam> [--binsize] [--plot]
 
 optional arguments:
   -h, --help         show this help message and exit
   --ref <reference>  input reference file
   --input <sam/bam>  input bam/sam file
   --binsize          input bin size (default:1000)
+  --plot             Results visualization
 ```
 
 - `reference` - the reference file in fasta format.
 - `sam` / `bam` - the result of mapping in sam/bam file. If you have used the observe function to process your data, the resulting `tmp.sort.bam` file can be used as the input.
 - `binsize` - the length of bin. A bin is the smallest unit to count the read coverage and GC content.
 
 
 
-### modi
+#### modi_bin
 
-```shell
-giraffe modi -h
 ```
-
-```shell
-usage: giraffe modi [-h] --input <bed> --ref <reference> [--cpu <number>]
+giraffe modi_bin -h
+usage: giraffe modi_bin [-h] --input <bed> --ref <reference> [--cpu <number>] [--plot]
 
 optional arguments:
   -h, --help         show this help message and exit
-  --input <bed>      input bed file
-  --ref <reference>  input reference
+  --input <bed>      input modificated bed file, please use the .bed as the file suffix
+  --ref <reference>  input position file with CSV format, please use the .csv as the file suffix
   --cpu <number>     number of cpu (default:10)
+  --plot             Results visualization
 ```
 
-- `bed` -  a bed file with four columns (three columns for position, one for methylation proportion).  Please use the tab ("\t") to gap the column instead of the space (" ").
+- `bed` -  a BED file with four columns (three columns for position, one for methylation proportion).  Please use the tab ("\t") to gap the column instead of the space (" ").
 
-   ```shell
+   ```
    #chrom	start	end	value
    chr1	81	83	0.8
    chr1	21314	21315	0.3
    chr1	32421	32422	0.85
    ```
 
-- `reference` - a csv file with target regions.
+- `reference` - a CSV file with target regions.
 
-   ```shell
+   ```
    chr1,0,100000,1_0_100000
    chr1,100000,200000,1_100000_200000
    ```
 
 
 
 ## Workflow
 
 ```mermaid
 graph TD
-raw_data --> |Quality control| clean_data
-raw_data --> |Basecall| modification_file
-modification_file --> modification_distribution
-clean_data --> Estimated_accuracy
-clean_data --> |Reference| aligned_file
-aligned_file --> Homopolymer_analysis
-aligned_file --> GC_bias 
-aligned_file --> Observed_accuracy
+	A(raw signal) -.-> |Basecall| B(FASTA)
+	A(raw signal) -.-> |Basecall| C(modificated BED)
+	C(modificated BED) --> |modi_bin| D(modification distribution)
+	B(FASTA) --> |estimate|e(estimated accuracy)
+	B(FASTA) --> |observe| f(clean reads)
+	f(clean reads) --> |observe| g(aligned BAM)
+	
+	g(aligned BAM) --> |observe|h(homopolymer identification)
+ 	g(aligned BAM) --> |observe|i(observed accuracy)
+	g(aligned BAM) --> |gc_bias|j(GC bias) 
 ```
 
 
 
 ## Developing
 
-- A example to show how to run
-- polish the result figures
 - run the homopolymer identification with multi-processed
```

### Comparing `Giraffe_View-0.0.9.3/LICENSE` & `Giraffe_View-0.0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.9.3/PKG-INFO` & `Giraffe_View-0.0.9.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Giraffe_View
-Version: 0.0.9.3
+Version: 0.0.9.4
 Summary: A small tool help assess and visualize the accuracy of a sequencing dataset,   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.
 Home-page: https://github.com/lxd98/Giraffe_View
 Author: Xudong Liu
 Author-email: xudongliu98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,170 +15,155 @@
 # Giraffe_View 
 
 **Giraffe_View** is designed to help assess and visualize the accuracy of a sequencing dataset, specifically for Oxford Nanopore Technologies (ONT) long-read sequencing including DNA and RNA data. There are four main functions to validate the read quality.
 
 - `observe`  calculates the observed read accuracy, mismatches porportion, and homopolymer identification.
 - `estimate`  calculates the estimated read accuracy, which is equal to Quality Score.
 - `gc_bias`  compares the relationship between GC content and read coverage.
-- `modi` perform statistics on the distribution of modification based on the bed file.
+- `modi_bin` perform statistics on the distribution of modification based on the bed file.
 
 
 
 ## Install
 
-To use this software, you need to install additional dependencies including samtools, minimap2, and seqkit for read processing and ggplot2 and patchwork for figure plotting.
-
-The following commands can help you to install the package  and dependencies.
+To use this software, you need to install additional dependencies including samtools, minimap2, seqkit, and bedtools for read processing. The following commands can help you to install the package  and dependencies.
 
 ```shell
 pip install Giraffe-View
-
 conda install -c bioconda -c conda-forge samtools minimap2 seqkit bedtools -y
-conda install -c conda-forge r-ggplot2 r-patchwork -y
 ```
 
 
 
 ## General Usage
 
 Giraffe View is run simply with fllowing commands:
 
-```shell
-giraffe -h
 ```
+giraffe -h
+usage: giraffe [-h] {observe,estimate,gc_bias,modi_bin} ...
 
-```shell
-usage: giraffe [-h] {observe,modi,gc_bias,estimate} ...
-
-A tool to help you assess quality of your ONT data.
+A tool to help you assess quality of ONT data.
 
 positional arguments:
-  {observe,modi,gc_bias,estimate}
-    observe             Observed quality in accuracy, mismatch, and homopolymer
-    modi                Average modification proportion of regions
-    gc_bias             Relationship between GC content and depth
+  {observe,estimate,gc_bias,modi_bin}
+    observe             Observed quality in accuracy, mismatch, and homopolymer identification
     estimate            Estimated read accuracy
+    gc_bias             Relationship between GC content and depth
+    modi_bin            Average modification proportion of bins
 
 optional arguments:
   -h, --help            show this help message and exit
 ```
 
 
 
 The available sub-commands are:
 
-### observe
+#### observe
 
-```shell
-giraffe observe -h
 ```
-
-```xshell
-usage: giraffe observe [-h] --input <fastq> --ref <reference> [--cpu <number>]
+giraffe observe -h
+usage: giraffe observe [-h] --input <fastq> --ref <reference> [--cpu <number>] [--plot]
 
 optional arguments:
   -h, --help         show this help message and exit
   --input <fastq>    input reads
   --ref <reference>  input reference
   --cpu <number>     number of cpu (default:10)
+  --plot             Results visualization
 ```
 
 - `fastq` - the raw fastq data, some filter steps will be conducted including short read ( < 200 bp) and low quality read ( < 7 ) removal.
 - `reference` - the reference file in fasta format.
 - `cpu` - the number of CPUs will be used during processing.
 
 
 
-### estimate  
+#### estimate  
 
-```shell
-giraffe estimate -h
 ```
-
-```shell
-usage: giraffe estimate [-h] --input <fastq> [--cpu <number>]
+giraffe estimate -h
+usage: giraffe estimate [-h] --input <fastq> [--cpu <number>] [--plot]
 
 optional arguments:
   -h, --help       show this help message and exit
   --input <fastq>  input reads
   --cpu <number>   number of cpu (default:10)
+  --plot           Results visualization
 ```
 
 
 
-### gc_bias
+#### gc_bias
 
-```shell
-giraffe gc_bias -h
 ```
-
-```shell
-usage: giraffe gc_bias [-h] --ref <reference> --input <sam/bam> [--binsize]
+giraffe gc_bias -h
+usage: giraffe gc_bias [-h] --ref <reference> --input <sam/bam> [--binsize] [--plot]
 
 optional arguments:
   -h, --help         show this help message and exit
   --ref <reference>  input reference file
   --input <sam/bam>  input bam/sam file
   --binsize          input bin size (default:1000)
+  --plot             Results visualization
 ```
 
 - `reference` - the reference file in fasta format.
 - `sam` / `bam` - the result of mapping in sam/bam file. If you have used the observe function to process your data, the resulting `tmp.sort.bam` file can be used as the input.
 - `binsize` - the length of bin. A bin is the smallest unit to count the read coverage and GC content.
 
 
 
-### modi
+#### modi_bin
 
-```shell
-giraffe modi -h
 ```
-
-```shell
-usage: giraffe modi [-h] --input <bed> --ref <reference> [--cpu <number>]
+giraffe modi_bin -h
+usage: giraffe modi_bin [-h] --input <bed> --ref <reference> [--cpu <number>] [--plot]
 
 optional arguments:
   -h, --help         show this help message and exit
-  --input <bed>      input bed file
-  --ref <reference>  input reference
+  --input <bed>      input modificated bed file, please use the .bed as the file suffix
+  --ref <reference>  input position file with CSV format, please use the .csv as the file suffix
   --cpu <number>     number of cpu (default:10)
+  --plot             Results visualization
 ```
 
-- `bed` -  a bed file with four columns (three columns for position, one for methylation proportion).  Please use the tab ("\t") to gap the column instead of the space (" ").
+- `bed` -  a BED file with four columns (three columns for position, one for methylation proportion).  Please use the tab ("\t") to gap the column instead of the space (" ").
 
-   ```shell
+   ```
    #chrom	start	end	value
    chr1	81	83	0.8
    chr1	21314	21315	0.3
    chr1	32421	32422	0.85
    ```
 
-- `reference` - a csv file with target regions.
+- `reference` - a CSV file with target regions.
 
-   ```shell
+   ```
    chr1,0,100000,1_0_100000
    chr1,100000,200000,1_100000_200000
    ```
 
 
 
 ## Workflow
 
 ```mermaid
 graph TD
-raw_data --> |Quality control| clean_data
-raw_data --> |Basecall| modification_file
-modification_file --> modification_distribution
-clean_data --> Estimated_accuracy
-clean_data --> |Reference| aligned_file
-aligned_file --> Homopolymer_analysis
-aligned_file --> GC_bias 
-aligned_file --> Observed_accuracy
+	A(raw signal) -.-> |Basecall| B(FASTA)
+	A(raw signal) -.-> |Basecall| C(modificated BED)
+	C(modificated BED) --> |modi_bin| D(modification distribution)
+	B(FASTA) --> |estimate|e(estimated accuracy)
+	B(FASTA) --> |observe| f(clean reads)
+	f(clean reads) --> |observe| g(aligned BAM)
+	
+	g(aligned BAM) --> |observe|h(homopolymer identification)
+ 	g(aligned BAM) --> |observe|i(observed accuracy)
+	g(aligned BAM) --> |gc_bias|j(GC bias) 
 ```
 
 
 
 ## Developing
 
-- A example to show how to run
-- polish the result figures
 - run the homopolymer identification with multi-processed
```

### Comparing `Giraffe_View-0.0.9.3/README.md` & `Giraffe_View-0.0.9.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,170 +1,155 @@
 # Giraffe_View 
 
 **Giraffe_View** is designed to help assess and visualize the accuracy of a sequencing dataset, specifically for Oxford Nanopore Technologies (ONT) long-read sequencing including DNA and RNA data. There are four main functions to validate the read quality.
 
 - `observe`  calculates the observed read accuracy, mismatches porportion, and homopolymer identification.
 - `estimate`  calculates the estimated read accuracy, which is equal to Quality Score.
 - `gc_bias`  compares the relationship between GC content and read coverage.
-- `modi` perform statistics on the distribution of modification based on the bed file.
+- `modi_bin` perform statistics on the distribution of modification based on the bed file.
 
 
 
 ## Install
 
-To use this software, you need to install additional dependencies including samtools, minimap2, and seqkit for read processing and ggplot2 and patchwork for figure plotting.
-
-The following commands can help you to install the package  and dependencies.
+To use this software, you need to install additional dependencies including samtools, minimap2, seqkit, and bedtools for read processing. The following commands can help you to install the package  and dependencies.
 
 ```shell
 pip install Giraffe-View
-
 conda install -c bioconda -c conda-forge samtools minimap2 seqkit bedtools -y
-conda install -c conda-forge r-ggplot2 r-patchwork -y
 ```
 
 
 
 ## General Usage
 
 Giraffe View is run simply with fllowing commands:
 
-```shell
-giraffe -h
 ```
+giraffe -h
+usage: giraffe [-h] {observe,estimate,gc_bias,modi_bin} ...
 
-```shell
-usage: giraffe [-h] {observe,modi,gc_bias,estimate} ...
-
-A tool to help you assess quality of your ONT data.
+A tool to help you assess quality of ONT data.
 
 positional arguments:
-  {observe,modi,gc_bias,estimate}
-    observe             Observed quality in accuracy, mismatch, and homopolymer
-    modi                Average modification proportion of regions
-    gc_bias             Relationship between GC content and depth
+  {observe,estimate,gc_bias,modi_bin}
+    observe             Observed quality in accuracy, mismatch, and homopolymer identification
     estimate            Estimated read accuracy
+    gc_bias             Relationship between GC content and depth
+    modi_bin            Average modification proportion of bins
 
 optional arguments:
   -h, --help            show this help message and exit
 ```
 
 
 
 The available sub-commands are:
 
-### observe
+#### observe
 
-```shell
-giraffe observe -h
 ```
-
-```xshell
-usage: giraffe observe [-h] --input <fastq> --ref <reference> [--cpu <number>]
+giraffe observe -h
+usage: giraffe observe [-h] --input <fastq> --ref <reference> [--cpu <number>] [--plot]
 
 optional arguments:
   -h, --help         show this help message and exit
   --input <fastq>    input reads
   --ref <reference>  input reference
   --cpu <number>     number of cpu (default:10)
+  --plot             Results visualization
 ```
 
 - `fastq` - the raw fastq data, some filter steps will be conducted including short read ( < 200 bp) and low quality read ( < 7 ) removal.
 - `reference` - the reference file in fasta format.
 - `cpu` - the number of CPUs will be used during processing.
 
 
 
-### estimate  
+#### estimate  
 
-```shell
-giraffe estimate -h
 ```
-
-```shell
-usage: giraffe estimate [-h] --input <fastq> [--cpu <number>]
+giraffe estimate -h
+usage: giraffe estimate [-h] --input <fastq> [--cpu <number>] [--plot]
 
 optional arguments:
   -h, --help       show this help message and exit
   --input <fastq>  input reads
   --cpu <number>   number of cpu (default:10)
+  --plot           Results visualization
 ```
 
 
 
-### gc_bias
+#### gc_bias
 
-```shell
-giraffe gc_bias -h
 ```
-
-```shell
-usage: giraffe gc_bias [-h] --ref <reference> --input <sam/bam> [--binsize]
+giraffe gc_bias -h
+usage: giraffe gc_bias [-h] --ref <reference> --input <sam/bam> [--binsize] [--plot]
 
 optional arguments:
   -h, --help         show this help message and exit
   --ref <reference>  input reference file
   --input <sam/bam>  input bam/sam file
   --binsize          input bin size (default:1000)
+  --plot             Results visualization
 ```
 
 - `reference` - the reference file in fasta format.
 - `sam` / `bam` - the result of mapping in sam/bam file. If you have used the observe function to process your data, the resulting `tmp.sort.bam` file can be used as the input.
 - `binsize` - the length of bin. A bin is the smallest unit to count the read coverage and GC content.
 
 
 
-### modi
+#### modi_bin
 
-```shell
-giraffe modi -h
 ```
-
-```shell
-usage: giraffe modi [-h] --input <bed> --ref <reference> [--cpu <number>]
+giraffe modi_bin -h
+usage: giraffe modi_bin [-h] --input <bed> --ref <reference> [--cpu <number>] [--plot]
 
 optional arguments:
   -h, --help         show this help message and exit
-  --input <bed>      input bed file
-  --ref <reference>  input reference
+  --input <bed>      input modificated bed file, please use the .bed as the file suffix
+  --ref <reference>  input position file with CSV format, please use the .csv as the file suffix
   --cpu <number>     number of cpu (default:10)
+  --plot             Results visualization
 ```
 
-- `bed` -  a bed file with four columns (three columns for position, one for methylation proportion).  Please use the tab ("\t") to gap the column instead of the space (" ").
+- `bed` -  a BED file with four columns (three columns for position, one for methylation proportion).  Please use the tab ("\t") to gap the column instead of the space (" ").
 
-   ```shell
+   ```
    #chrom	start	end	value
    chr1	81	83	0.8
    chr1	21314	21315	0.3
    chr1	32421	32422	0.85
    ```
 
-- `reference` - a csv file with target regions.
+- `reference` - a CSV file with target regions.
 
-   ```shell
+   ```
    chr1,0,100000,1_0_100000
    chr1,100000,200000,1_100000_200000
    ```
 
 
 
 ## Workflow
 
 ```mermaid
 graph TD
-raw_data --> |Quality control| clean_data
-raw_data --> |Basecall| modification_file
-modification_file --> modification_distribution
-clean_data --> Estimated_accuracy
-clean_data --> |Reference| aligned_file
-aligned_file --> Homopolymer_analysis
-aligned_file --> GC_bias 
-aligned_file --> Observed_accuracy
+	A(raw signal) -.-> |Basecall| B(FASTA)
+	A(raw signal) -.-> |Basecall| C(modificated BED)
+	C(modificated BED) --> |modi_bin| D(modification distribution)
+	B(FASTA) --> |estimate|e(estimated accuracy)
+	B(FASTA) --> |observe| f(clean reads)
+	f(clean reads) --> |observe| g(aligned BAM)
+	
+	g(aligned BAM) --> |observe|h(homopolymer identification)
+ 	g(aligned BAM) --> |observe|i(observed accuracy)
+	g(aligned BAM) --> |gc_bias|j(GC bias) 
 ```
 
 
 
 ## Developing
 
-- A example to show how to run
-- polish the result figures
 - run the homopolymer identification with multi-processed
```

### Comparing `Giraffe_View-0.0.9.3/setup.py` & `Giraffe_View-0.0.9.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="Giraffe_View",
-  version="0.0.9.3",
+  version="0.0.9.4",
   author="Xudong Liu",
   author_email="xudongliu98@gmail.com",
   description="A small tool help assess and visualize the accuracy of a sequencing dataset, \
   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/lxd98/Giraffe_View",
@@ -21,11 +21,12 @@
   ],
   python_requires = '>=3.7, <=3.10',
   install_requires=[
   'pysam >= 0.17.0',
   'plotnine >= 0.12.1',
   'numpy >= 1.7.0',
   'pandas >= 1.5.0',
-  'tqdm == 4.64.0'
+  'tqdm >= 4.64.0',
+  'termcolor >= 2.2.0'
   ],
   scripts = ["Giraffe_View/giraffe"]
 )
```

