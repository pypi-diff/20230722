# Comparing `tmp/hchacha-1.0.2.tar.gz` & `tmp/hchacha-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hchacha-1.0.2.tar", max compression
+gzip compressed data, was "hchacha-1.0.3.tar", max compression
```

## Comparing `hchacha-1.0.2.tar` & `hchacha-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,29 @@
--rw-r--r--   0        0        0     1077 2023-02-09 14:04:58.020837 hchacha-1.0.2/LICENSE.txt
--rw-r--r--   0        0        0     3744 2023-02-13 16:55:33.165808 hchacha-1.0.2/README.md
--rw-r--r--   0        0        0      900 2023-02-13 16:47:23.293962 hchacha-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       47 2023-02-06 02:52:38.085523 hchacha-1.0.2/src/hchacha/__init__.py
--rw-r--r--   0        0        0     5881 2023-02-06 02:52:38.086507 hchacha-1.0.2/src/hchacha/data/GCF_000001405.25_GRCh37.p13_assembly_report.txt.gz
--rw-r--r--   0        0        0    12451 2023-02-06 02:52:38.086909 hchacha-1.0.2/src/hchacha/data/GCF_000001405.39_GRCh38.p13_assembly_report.txt.gz
--rw-r--r--   0        0        0    14331 2023-02-06 02:52:38.087577 hchacha-1.0.2/src/hchacha/data/GCF_000001405.39_GRCh38.p14_assembly_report.txt.gz
--rwxr-xr-x   0        0        0     7601 2023-02-13 16:23:51.865083 hchacha-1.0.2/src/hchacha/hchacha.py
--rw-r--r--   0        0        0     4674 1970-01-01 00:00:00.000000 hchacha-1.0.2/setup.py
--rw-r--r--   0        0        0     4749 1970-01-01 00:00:00.000000 hchacha-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-02-09 14:04:58.020837 hchacha-1.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     3314 2023-07-21 20:38:53.317135 hchacha-1.0.3/README.md
+-rw-r--r--   0        0        0      900 2023-07-22 16:18:53.730306 hchacha-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-02-06 02:52:38.085523 hchacha-1.0.3/src/hchacha/__init__.py
+-rw-r--r--   0        0        0     5626 2016-10-13 15:30:37.000000 hchacha-1.0.3/src/hchacha/data/GRCh37.p10_assembly_report.txt.gz
+-rw-r--r--   0        0        0     5719 2016-10-13 15:30:37.000000 hchacha-1.0.3/src/hchacha/data/GRCh37.p11_assembly_report.txt.gz
+-rw-r--r--   0        0        0     5865 2016-10-13 15:30:38.000000 hchacha-1.0.3/src/hchacha/data/GRCh37.p12_assembly_report.txt.gz
+-rw-r--r--   0        0        0     6073 2022-03-12 17:43:21.000000 hchacha-1.0.3/src/hchacha/data/GRCh37.p13_assembly_report.txt.gz
+-rw-r--r--   0        0        0     3732 2016-10-13 15:30:37.000000 hchacha-1.0.3/src/hchacha/data/GRCh37.p2_assembly_report.txt.gz
+-rw-r--r--   0        0        0     4338 2016-10-13 15:30:37.000000 hchacha-1.0.3/src/hchacha/data/GRCh37.p5_assembly_report.txt.gz
+-rw-r--r--   0        0        0     5129 2016-10-13 15:30:37.000000 hchacha-1.0.3/src/hchacha/data/GRCh37.p9_assembly_report.txt.gz
+-rw-r--r--   0        0        0     2560 2016-10-13 15:30:37.000000 hchacha-1.0.3/src/hchacha/data/GRCh37_assembly_report.txt.gz
+-rw-r--r--   0        0        0    11552 2017-01-20 23:11:46.000000 hchacha-1.0.3/src/hchacha/data/GRCh38.p10_assembly_report.txt.gz
+-rw-r--r--   0        0        0    11912 2017-07-13 15:37:28.000000 hchacha-1.0.3/src/hchacha/data/GRCh38.p11_assembly_report.txt.gz
+-rw-r--r--   0        0        0    12238 2020-07-24 05:12:19.000000 hchacha-1.0.3/src/hchacha/data/GRCh38.p12_assembly_report.txt.gz
+-rw-r--r--   0        0        0    13541 2022-04-06 15:25:09.000000 hchacha-1.0.3/src/hchacha/data/GRCh38.p13_assembly_report.txt.gz
+-rw-r--r--   0        0        0    15026 2023-04-24 19:26:35.000000 hchacha-1.0.3/src/hchacha/data/GRCh38.p14_assembly_report.txt.gz
+-rw-r--r--   0        0        0    10015 2016-10-13 15:30:38.000000 hchacha-1.0.3/src/hchacha/data/GRCh38.p1_assembly_report.txt.gz
+-rw-r--r--   0        0        0    10271 2016-10-13 15:30:38.000000 hchacha-1.0.3/src/hchacha/data/GRCh38.p2_assembly_report.txt.gz
+-rw-r--r--   0        0        0    10430 2016-10-13 15:30:38.000000 hchacha-1.0.3/src/hchacha/data/GRCh38.p3_assembly_report.txt.gz
+-rw-r--r--   0        0        0    10708 2016-10-13 15:30:39.000000 hchacha-1.0.3/src/hchacha/data/GRCh38.p4_assembly_report.txt.gz
+-rw-r--r--   0        0        0    10838 2021-12-16 03:28:08.000000 hchacha-1.0.3/src/hchacha/data/GRCh38.p5_assembly_report.txt.gz
+-rw-r--r--   0        0        0    10907 2016-10-13 15:30:39.000000 hchacha-1.0.3/src/hchacha/data/GRCh38.p6_assembly_report.txt.gz
+-rw-r--r--   0        0        0    10983 2016-10-13 15:30:39.000000 hchacha-1.0.3/src/hchacha/data/GRCh38.p7_assembly_report.txt.gz
+-rw-r--r--   0        0        0    11284 2016-10-13 15:30:39.000000 hchacha-1.0.3/src/hchacha/data/GRCh38.p8_assembly_report.txt.gz
+-rw-r--r--   0        0        0    11438 2016-10-13 15:30:39.000000 hchacha-1.0.3/src/hchacha/data/GRCh38.p9_assembly_report.txt.gz
+-rw-r--r--   0        0        0     9682 2016-10-13 15:30:38.000000 hchacha-1.0.3/src/hchacha/data/GRCh38_assembly_report.txt.gz
+-rwxr-xr-x   0        0        0     7928 2023-07-21 20:33:58.384900 hchacha-1.0.3/src/hchacha/hchacha.py
+-rw-r--r--   0        0        0     4271 1970-01-01 00:00:00.000000 hchacha-1.0.3/PKG-INFO
```

### Comparing `hchacha-1.0.2/LICENSE.txt` & `hchacha-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hchacha-1.0.2/README.md` & `hchacha-1.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -38,40 +38,33 @@
 Since all you are doing is really renaming the sequences in the header (and individual BAM/CRAM records
 refer back to those sequence names by an integer index), you can do things much more quickly and with
 less CPU usage using `samtools reheader` if it is available on your system.
 
 For example:
 
 ```bash
-samtools reheader -P -c 'python3 hchacha sam -a 38 -t ucsc -s' input.bam > output.bam
+samtools reheader -P -c 'hchacha sam -a 38 -t ucsc -s' input.bam > output.bam
 ```
 
 With some clever use of the `tee` command to output the new bam file and continue the shell pipeline
 going, you can even make the new index at the same time:
 
 ```bash
-samtools reheader -P -c 'python3 hchacha.py sam -a 38 -t ucsc -s' input.bam | tee output.bam | samtools index - output.bam.bai
-```
-
+samtools reheader -P -c 'hchacha sam -a 38 -t ucsc -s' input.bam | tee output.bam | samtools index - output.bam.bai
 ```
 
 ## Data used
 
 NCBI provides a useful file (*.assembly_report.txt) for different GRCh reference versions and patch
 levels, for instance [here](https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/000/001/405/GCF_000001405.40_GRCh38.p14/GCF_000001405.40_GRCh38.p14_assembly_report.txt),
 that maps among these names. To get the data included in the repository (for GRCh versions 37 and 38), I
-did the following:
-
-```
-curl https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/000/001/405/GCF_000001405.40_GRCh38.p14/GCF_000001405.40_GRCh38.p14_assembly_report.txt | gzip -9 > src/hchacha/data/GCF_000001405.39_GRCh38.p14_assembly_report.txt.gz
-
-curl https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/000/001/405/GCF_000001405.25_GRCh37.p13/GCF_000001405.25_GRCh37.p13_assembly_report.txt | gzip -9 > src/hchacha/data/GCF_000001405.25_GRCh37.p13_assembly_report.txt.gz
-```
+ran the bash script `prepare-assembly-reports/get-assembly-reports.bash` (require wget), then moved the resulting
+files to `src/hchacha/data`.
 
-Changing the above (like for new patch levels) would also require changing the relevant filenames in the script.
+## Mapping for ensembl names
 
 The mapping to ensEMBL names is not quite as straightforward. It looks
 like they use the "short" names (like 1, 2, 3, ... X, Y) for the primary chromosomes, then RefSeq
 accessions for the others, so that is what this script does.
 
 ## License
```

### Comparing `hchacha-1.0.2/pyproject.toml` & `hchacha-1.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hchacha"
-version = "1.0.2"
+version = "1.0.3"
 description = "Human CHromosome Accession CHAnge - Convert between different human chromosome naming systems (of the same assembly/version)"
 authors = ["Bradford Powell <bpow@drpowell.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://bitbucket.org/bpow/hchacha"
 homepage = "https://bitbucket.org/bpow/hchacha"
 keywords = [ "genetics", "bam", "sam", "vcf", "variants", "bed", "fasta", "genome", "exome"]
```

### Comparing `hchacha-1.0.2/src/hchacha/hchacha.py` & `hchacha-1.0.3/src/hchacha/hchacha.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,26 +6,29 @@
 import collections
 import gzip
 import os.path
 
 contig_pattern = re.compile(r"##contig=<ID=([^,]+),(.*)")
 
 
-def make_translation(assembly="38", target="refseq", silent=False):
+def make_translation(assembly="38", patch=None, target="refseq", silent=False):
     # Read the appropriate mappings of chromosome names
     # data originally from location like:
     # https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/000/001/405/GCF_000001405.38_GRCh38.p12/GCF_000001405.38_GRCh38.p12_assembly_report.txt
-    if assembly == "37":
-        assembly_report = "data/GCF_000001405.25_GRCh37.p13_assembly_report.txt.gz"
-    elif assembly == "38":
-        assembly_report = "data/GCF_000001405.39_GRCh38.p14_assembly_report.txt.gz"
-    else:
-        raise RuntimeError("Assembly %s is not recognized" % assembly)
+    if patch is None:
+        if assembly == "37":
+            patch = "13"
+        elif assembly == "38":
+            patch = "14"
+    
+    assembly_report = os.path.join(os.path.dirname(__file__),
+                                   "data/GRCh%s%s_assembly_report.txt.gz" % (assembly, '' if patch == '0' else '.p' + patch))
 
-    assembly_report = os.path.join(os.path.dirname(__file__), assembly_report)
+    if not os.path.exists(assembly_report):
+        raise RuntimeError("Assembly %s with patch %s is not recognized" % (assembly, patch))
 
     # ensembl uses Sequence-Name for full chromosomes, otherwise Genbank-Accn
     # GenBank and RefSeq use GenBank-Accn and Refseq-Accn (of course...)
     # UCSC uses UCSC-style-name
 
     mapping = dict()
     columns = "Sequence-Name Sequence-Role Assigned-Molecule Assigned-Molecule-Location/Type GenBank-Accn Relationship RefSeq-Accn Assembly-Unit Sequence-Length UCSC-style-name".split()
@@ -60,22 +63,23 @@
 
     return translate
 
 
 def separated_values(
     inf=sys.stdin,
     assembly="38",
+    patch=None,
     target="refseq",
     silent=False,
     column=1,
     delimiter="\t",
     subformat=None,
     **kwargs,
 ):
-    translate = make_translation(assembly, target, silent)
+    translate = make_translation(assembly, patch, target, silent)
     column = int(column) - 1
     for line in inf:
         if subformat == "vcf":
             # special handling for header lines-- most pass-through, but translate the 'contig' lines
             if line.startswith("#"):
                 if line.startswith("##contig=<"):
                     m = contig_pattern.match(line)
@@ -109,16 +113,16 @@
                 row[6] = translate(row[6])
         except IndexError:
             print(line, end="")
             continue
         print(delimiter.join(row))
 
 
-def fasta(inf=sys.stdin, assembly="38", target="refseq", silent=False, **kwargs):
-    translate = make_translation(assembly, target, silent)
+def fasta(inf=sys.stdin, assembly="38", patch=None, target="refseq", silent=False, **kwargs):
+    translate = make_translation(assembly, patch, target, silent)
     for line in inf:
         if line.startswith(">"):
             old_identifier = line[1:].split()[0]
             translated_line = ">%s%s" % (
                 translate(old_identifier),
                 line[(len(old_identifier) + 1) :],
             )
@@ -139,14 +143,20 @@
         "-a",
         action="store",
         help="GRCh assembly version",
         default="38",
         choices=("37", "38"),
     )
     parent_parser.add_argument(
+        "--patch",
+        "-p",
+        action="store",
+        help="GRCh patch version (most recent if not specified, use '0' for initial release)",
+    )
+    parent_parser.add_argument(
         "--silent",
         "-s",
         action="store_true",
         help="silently pass through identifiers that are not recognized (otherwise throw exception)",
     )
     parent_parser.add_argument(
         "--target",
```

### Comparing `hchacha-1.0.2/PKG-INFO` & `hchacha-1.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hchacha
-Version: 1.0.2
+Version: 1.0.3
 Summary: Human CHromosome Accession CHAnge - Convert between different human chromosome naming systems (of the same assembly/version)
 Home-page: https://bitbucket.org/bpow/hchacha
 License: MIT
 Keywords: genetics,bam,sam,vcf,variants,bed,fasta,genome,exome
 Author: Bradford Powell
 Author-email: bpow@drpowell.org
 Requires-Python: >=3.7,<4.0
@@ -12,15 +12,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Project-URL: Repository, https://bitbucket.org/bpow/hchacha
 Description-Content-Type: text/markdown
 
 # hchacha - Human CHromosome Accession CHange
 
 Translate among the different naming systems used for human chromosomes (of the same assembly)
@@ -61,40 +60,33 @@
 Since all you are doing is really renaming the sequences in the header (and individual BAM/CRAM records
 refer back to those sequence names by an integer index), you can do things much more quickly and with
 less CPU usage using `samtools reheader` if it is available on your system.
 
 For example:
 
 ```bash
-samtools reheader -P -c 'python3 hchacha sam -a 38 -t ucsc -s' input.bam > output.bam
+samtools reheader -P -c 'hchacha sam -a 38 -t ucsc -s' input.bam > output.bam
 ```
 
 With some clever use of the `tee` command to output the new bam file and continue the shell pipeline
 going, you can even make the new index at the same time:
 
 ```bash
-samtools reheader -P -c 'python3 hchacha.py sam -a 38 -t ucsc -s' input.bam | tee output.bam | samtools index - output.bam.bai
-```
-
+samtools reheader -P -c 'hchacha sam -a 38 -t ucsc -s' input.bam | tee output.bam | samtools index - output.bam.bai
 ```
 
 ## Data used
 
 NCBI provides a useful file (*.assembly_report.txt) for different GRCh reference versions and patch
 levels, for instance [here](https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/000/001/405/GCF_000001405.40_GRCh38.p14/GCF_000001405.40_GRCh38.p14_assembly_report.txt),
 that maps among these names. To get the data included in the repository (for GRCh versions 37 and 38), I
-did the following:
-
-```
-curl https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/000/001/405/GCF_000001405.40_GRCh38.p14/GCF_000001405.40_GRCh38.p14_assembly_report.txt | gzip -9 > src/hchacha/data/GCF_000001405.39_GRCh38.p14_assembly_report.txt.gz
-
-curl https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/000/001/405/GCF_000001405.25_GRCh37.p13/GCF_000001405.25_GRCh37.p13_assembly_report.txt | gzip -9 > src/hchacha/data/GCF_000001405.25_GRCh37.p13_assembly_report.txt.gz
-```
+ran the bash script `prepare-assembly-reports/get-assembly-reports.bash` (require wget), then moved the resulting
+files to `src/hchacha/data`.
 
-Changing the above (like for new patch levels) would also require changing the relevant filenames in the script.
+## Mapping for ensembl names
 
 The mapping to ensEMBL names is not quite as straightforward. It looks
 like they use the "short" names (like 1, 2, 3, ... X, Y) for the primary chromosomes, then RefSeq
 accessions for the others, so that is what this script does.
 
 ## License
```

