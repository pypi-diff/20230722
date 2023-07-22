# Comparing `tmp/BookerPdfTool-2023.7.19.1.tar.gz` & `tmp/BookerPdfTool-2023.7.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BookerPdfTool-2023.7.19.1.tar", last modified: Wed Jul 19 15:14:15 2023, max compression
+gzip compressed data, was "BookerPdfTool-2023.7.22.0.tar", last modified: Sat Jul 22 16:00:41 2023, max compression
```

## Comparing `BookerPdfTool-2023.7.19.1.tar` & `BookerPdfTool-2023.7.22.0.tar`

### file list

```diff
@@ -1,29 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 15:14:15.972668 BookerPdfTool-2023.7.19.1/
-drwxrwxrwx   0        0        0        0 2023-07-19 15:14:15.953671 BookerPdfTool-2023.7.19.1/BookerPdfTool/
--rw-rw-rw-   0        0        0      228 2023-07-19 15:13:51.000000 BookerPdfTool-2023.7.19.1/BookerPdfTool/__init__.py
--rw-rw-rw-   0        0        0     4672 2023-07-19 14:33:49.000000 BookerPdfTool-2023.7.19.1/BookerPdfTool/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 15:14:15.970667 BookerPdfTool-2023.7.19.1/BookerPdfTool/assets/
--rw-rw-rw-   0        0        0  1799680 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.19.1/BookerPdfTool/assets/7z.dll
--rwxrwxrwx   0        0        0   545280 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.19.1/BookerPdfTool/assets/7z.exe
--rw-rw-rw-   0        0        0   657262 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.19.1/BookerPdfTool/assets/PwdDic.txt
--rw-rw-rw-   0        0        0        0 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.19.1/BookerPdfTool/assets/__init__.py
--rw-rw-rw-   0        0        0    16896 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.19.1/BookerPdfTool/assets/jbig2enc.dll
--rwxrwxrwx   0        0        0   786446 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.19.1/BookerPdfTool/assets/jbig2enc.exe
--rwxrwxrwx   0        0        0   413336 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.19.1/BookerPdfTool/assets/unrar.exe
--rw-rw-rw-   0        0        0     6173 2023-07-19 15:11:10.000000 BookerPdfTool-2023.7.19.1/BookerPdfTool/img2jb2pdf.py
--rw-rw-rw-   0        0        0    16075 2023-07-19 14:38:40.000000 BookerPdfTool-2023.7.19.1/BookerPdfTool/pdf_tool.py
--rw-rw-rw-   0        0        0     1174 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.19.1/BookerPdfTool/toggle_bw.py
--rw-rw-rw-   0        0        0     4840 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.19.1/BookerPdfTool/util.py
--rw-rw-rw-   0        0        0     1716 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.19.1/BookerPdfTool/zip_tool.py
-drwxrwxrwx   0        0        0        0 2023-07-19 15:14:15.956669 BookerPdfTool-2023.7.19.1/BookerPdfTool.egg-info/
--rw-rw-rw-   0        0        0     1905 2023-07-19 15:14:15.000000 BookerPdfTool-2023.7.19.1/BookerPdfTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      651 2023-07-19 15:14:15.000000 BookerPdfTool-2023.7.19.1/BookerPdfTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 15:14:15.000000 BookerPdfTool-2023.7.19.1/BookerPdfTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2023-07-19 15:14:15.000000 BookerPdfTool-2023.7.19.1/BookerPdfTool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       69 2023-07-19 15:14:15.000000 BookerPdfTool-2023.7.19.1/BookerPdfTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-19 15:14:15.000000 BookerPdfTool-2023.7.19.1/BookerPdfTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1837 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.19.1/LICENSE
--rw-rw-rw-   0        0        0     1905 2023-07-19 15:14:15.972668 BookerPdfTool-2023.7.19.1/PKG-INFO
--rw-rw-rw-   0        0        0      708 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.19.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-19 15:14:15.972668 BookerPdfTool-2023.7.19.1/setup.cfg
--rw-rw-rw-   0        0        0     1975 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.19.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 16:00:41.651461 BookerPdfTool-2023.7.22.0/
+drwxrwxrwx   0        0        0        0 2023-07-22 16:00:41.637580 BookerPdfTool-2023.7.22.0/BookerPdfTool/
+-rw-rw-rw-   0        0        0      228 2023-07-22 15:58:27.000000 BookerPdfTool-2023.7.22.0/BookerPdfTool/__init__.py
+-rw-rw-rw-   0        0        0     4652 2023-07-22 13:05:54.000000 BookerPdfTool-2023.7.22.0/BookerPdfTool/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-22 16:00:41.645460 BookerPdfTool-2023.7.22.0/BookerPdfTool/assets/
+-rw-rw-rw-   0        0        0  1799680 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.22.0/BookerPdfTool/assets/7z.dll
+-rwxrwxrwx   0        0        0   545280 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.22.0/BookerPdfTool/assets/7z.exe
+-rw-rw-rw-   0        0        0   657262 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.22.0/BookerPdfTool/assets/PwdDic.txt
+-rw-rw-rw-   0        0        0        0 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.22.0/BookerPdfTool/assets/__init__.py
+-rwxrwxrwx   0        0        0   413336 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.22.0/BookerPdfTool/assets/unrar.exe
+-rw-rw-rw-   0        0        0    16018 2023-07-22 15:52:47.000000 BookerPdfTool-2023.7.22.0/BookerPdfTool/pdf_tool.py
+-rw-rw-rw-   0        0        0     1174 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.22.0/BookerPdfTool/toggle_bw.py
+-rw-rw-rw-   0        0        0     4840 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.22.0/BookerPdfTool/util.py
+-rw-rw-rw-   0        0        0     1716 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.22.0/BookerPdfTool/zip_tool.py
+drwxrwxrwx   0        0        0        0 2023-07-22 16:00:41.640576 BookerPdfTool-2023.7.22.0/BookerPdfTool.egg-info/
+-rw-rw-rw-   0        0        0     1905 2023-07-22 16:00:41.000000 BookerPdfTool-2023.7.22.0/BookerPdfTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2023-07-22 16:00:41.000000 BookerPdfTool-2023.7.22.0/BookerPdfTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 16:00:41.000000 BookerPdfTool-2023.7.22.0/BookerPdfTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2023-07-22 16:00:41.000000 BookerPdfTool-2023.7.22.0/BookerPdfTool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       80 2023-07-22 16:00:41.000000 BookerPdfTool-2023.7.22.0/BookerPdfTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-22 16:00:41.000000 BookerPdfTool-2023.7.22.0/BookerPdfTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1837 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.22.0/LICENSE
+-rw-rw-rw-   0        0        0     1905 2023-07-22 16:00:41.646461 BookerPdfTool-2023.7.22.0/PKG-INFO
+-rw-rw-rw-   0        0        0      708 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.22.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-22 16:00:41.651461 BookerPdfTool-2023.7.22.0/setup.cfg
+-rw-rw-rw-   0        0        0     1975 2023-07-19 13:57:52.000000 BookerPdfTool-2023.7.22.0/setup.py
```

### Comparing `BookerPdfTool-2023.7.19.1/BookerPdfTool/__main__.py` & `BookerPdfTool-2023.7.22.0/BookerPdfTool/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,41 +11,41 @@
 def main():
     parser = argparse.ArgumentParser(prog="BookerPdfTool", description="iBooker PDF tool", formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument("-v", "--version", action="version", version=f"BookerPdfTool version: {__version__}")
     parser.set_defaults(func=lambda x: parser.print_help())
     subparsers = parser.add_subparsers()
     
    
-    office2pdf_parser = subparsers.add_parser("office2pdf", help="doc/xls/ppt to pdf")
+    office2pdf_parser = subparsers.add_parser("fm-office", help="doc/xls/ppt to pdf")
     office2pdf_parser.add_argument("fname", help="file name")
     office2pdf_parser.set_defaults(func=office2pdf_handle)
     
-    comp_pdf_parser = subparsers.add_parser("comp-pdf", help="compress pdf")
+    comp_pdf_parser = subparsers.add_parser("comp", help="compress pdf")
     comp_pdf_parser.add_argument("fname", help="file name")
     comp_pdf_parser.set_defaults(func=comp_pdf)
 
 
-    ext_pdf_parser = subparsers.add_parser("ext-pdf", help="extract odf into images")
+    ext_pdf_parser = subparsers.add_parser("ext", help="extract odf into images")
     ext_pdf_parser.add_argument("fname", help="file name")
     ext_pdf_parser.add_argument("-d", "--dir", default='.', help="path to save")
     ext_pdf_parser.add_argument("-w", "--whole", action='store_true', default=False, help="whether to clip the whole page")
     ext_pdf_parser.set_defaults(func=ext_pdf)
 
-    pdf2html_parser = subparsers.add_parser("pdf2html", help="convert pdf page to html")
+    pdf2html_parser = subparsers.add_parser("2html", help="convert pdf page to html")
     pdf2html_parser.add_argument("fname", help="file name")
     pdf2html_parser.add_argument("-d", "--dir", default='.', help="path to save")
     pdf2html_parser.set_defaults(func=pdf2html)
 
     anime4k_auto_parser = subparsers.add_parser("anime4k-auto", help="process imgs with waifu2x")
     anime4k_auto_parser.add_argument("fname", help="file or dir name")
     anime4k_auto_parser.add_argument("-G", "--gpu", action='store_true', help="whether to use GPU")
     anime4k_auto_parser.add_argument("-t", "--threads", help="num of threads", type=int, default=8)
     anime4k_auto_parser.set_defaults(func=anime4k_auto_handle)
 
-    pack_pdf_parser = subparsers.add_parser("pack-pdf", help="package images into pdf")
+    pack_pdf_parser = subparsers.add_parser("pack", help="package images into pdf")
     pack_pdf_parser.add_argument("dir", help="dir name")
     pack_pdf_parser.add_argument("-r", "--regex", help="regex of keyword for grouping")
     pack_pdf_parser.add_argument("--jb2", action='store_true', help="rwhether to generate jb2 encoding pdf")
     pack_pdf_parser.set_defaults(func=pack_pdf)
 
 
     toggle_bw_parser = subparsers.add_parser("tog-bw", help="check if image colors reversed and then toggle them")
@@ -57,15 +57,15 @@
     ck_zip_parser = subparsers.add_parser("crack-zip", help="crack encrypted zip")
     ck_zip_parser.add_argument("fname", help="ZIP fname")
     ck_zip_parser.add_argument("-p", "--pw", default=asset('PwdDic.txt'), help="password dict")
     ck_zip_parser.add_argument("-t", "--threads", type=int, default=8, help="num of threads")
     ck_zip_parser.set_defaults(func=crack_zip)
 
 
-    pdf_auto_parser = subparsers.add_parser("pdf-auto", help="auto process pdf")
+    pdf_auto_parser = subparsers.add_parser("auto", help="auto process pdf")
     pdf_auto_parser.add_argument("fname", help="pdf fname or dirname")
     pdf_auto_parser.add_argument("-t", "--threads", type=int, default=8, help="num of threads")
     pdf_auto_parser.add_argument("-G", "--gpu", action='store_true', help="whether to use GPU")
     pdf_auto_parser.add_argument("-w", "--whole", action='store_true', default=False, help="whether to clip the whole page")
     pdf_auto_parser.set_defaults(func=pdf_auto_handle)
 
     pick_scan_parser = subparsers.add_parser("pick-scan", help="pick scanned pdf")
```

### Comparing `BookerPdfTool-2023.7.19.1/BookerPdfTool/assets/7z.dll` & `BookerPdfTool-2023.7.22.0/BookerPdfTool/assets/7z.dll`

 * *Files identical despite different names*

### Comparing `BookerPdfTool-2023.7.19.1/BookerPdfTool/assets/7z.exe` & `BookerPdfTool-2023.7.22.0/BookerPdfTool/assets/7z.exe`

 * *Files identical despite different names*

### Comparing `BookerPdfTool-2023.7.19.1/BookerPdfTool/assets/PwdDic.txt` & `BookerPdfTool-2023.7.22.0/BookerPdfTool/assets/PwdDic.txt`

 * *Files identical despite different names*

### Comparing `BookerPdfTool-2023.7.19.1/BookerPdfTool/assets/unrar.exe` & `BookerPdfTool-2023.7.22.0/BookerPdfTool/assets/unrar.exe`

 * *Files identical despite different names*

### Comparing `BookerPdfTool-2023.7.19.1/BookerPdfTool/pdf_tool.py` & `BookerPdfTool-2023.7.22.0/BookerPdfTool/pdf_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import platform
 import traceback
 from PIL import Image, ImageFile
 from multiprocessing import Pool
 from imgyaso import pngquant_bts, adathres_bts
 from .img2jb2pdf import img_to_jb2_pdf
 import img2pdf
+from img2jb2pdf import img2jb2pdf
 from io import BytesIO
 from .util import *
 
 ImageFile.LOAD_TRUNCATED_IMAGES = True
 fitz.Document.is_image = fitz.Document.xref_is_image
 
 app_map = {
@@ -244,18 +245,14 @@
         return 1
     elif wid < 4200:
         return 0.75
     else:
         return 0.5
 
 def pack_pdf(args):
-    if args.jb2 and platform.system() != 'Windows':
-        print('JBIG2 模式只支持 Windows')
-        return
-
     dir, rgx = args.dir, args.regex
     if dir.endswith('/') or \
         dir.endswith('\\'):
         dir = dir[:-1]
     
     fnames = filter(is_pic, os.listdir(dir))
     if not rgx:
@@ -276,15 +273,15 @@
         kw = m.group(0)
         d.setdefault(kw, [])
         d[kw].append(fname)
         
     for kw, fnames in d.items():
         fnames = [path.join(dir, f) for f in fnames]
         if args.jb2:
-            pdf = img_to_jb2_pdf(fnames)
+            pdf = img2jb2pdf(fnames)
         else:
             pdf = img2pdf.convert(fnames)
         fname = path.join(dir, kw + '.pdf')
         print(fname)
         open(fname, 'wb').write(pdf)
 
 def office2pdf(fname, ofname):
@@ -447,23 +444,24 @@
         print('请提供 PDF 文件')
         return
     print(f'file: {fname}')
     tmpdir = path.join(tempfile.gettempdir(), uuid.uuid4().hex)
     safe_mkdir(tmpdir)
     
     cmds = [
-        ['pdf-tool', 'ext-pdf', '-d', tmpdir, fname],
+        ['pdf-tool', 'ext', '-d', tmpdir, fname],
         ['pdf-tool', 'tog-bw', '-t', str(threads), tmpdir],
         ['pdf-tool', 'anime4k-auto', '-t', str(threads), tmpdir],
         ['imgyaso', '-m', 'thres', '-t', str(threads), tmpdir],
-        ['pdf-tool', 'pack-pdf', tmpdir],
+        ['pdf-tool', 'pack', tmpdir, '--jb2'],
     ]
     if args.gpu: cmds[2].append('-G')
     if args.whole: cmds[0].append('-w')
     for cmd in cmds:
+        print(f'cmd: {cmd}')
         subp.Popen(cmd, shell=True).communicate()
     if path.isfile(fname + '.bak'): os.unlink(fname + '.bak')
     shutil.move(fname, fname + '.bak')
     shutil.move(path.abspath(tmpdir) + '.pdf', fname)
     
     safe_rmdir(tmpdir)
```

### Comparing `BookerPdfTool-2023.7.19.1/BookerPdfTool/toggle_bw.py` & `BookerPdfTool-2023.7.22.0/BookerPdfTool/toggle_bw.py`

 * *Files identical despite different names*

### Comparing `BookerPdfTool-2023.7.19.1/BookerPdfTool/util.py` & `BookerPdfTool-2023.7.22.0/BookerPdfTool/util.py`

 * *Files identical despite different names*

### Comparing `BookerPdfTool-2023.7.19.1/BookerPdfTool/zip_tool.py` & `BookerPdfTool-2023.7.22.0/BookerPdfTool/zip_tool.py`

 * *Files identical despite different names*

### Comparing `BookerPdfTool-2023.7.19.1/BookerPdfTool.egg-info/PKG-INFO` & `BookerPdfTool-2023.7.22.0/BookerPdfTool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BookerPdfTool
-Version: 2023.7.19.1
+Version: 2023.7.22.0
 Summary: iBooker/ApacheCN 知识库抓取工具
 Home-page: https://github.com/apachecn/BookerPdfTool
 Author: wizardforcel
 Author-email: wizard.z@qq.com
 Keywords: wiki,知识库,document,文档,crawler,爬虫
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `BookerPdfTool-2023.7.19.1/BookerPdfTool.egg-info/SOURCES.txt` & `BookerPdfTool-2023.7.22.0/BookerPdfTool.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 LICENSE
 README.md
 setup.py
 BookerPdfTool/__init__.py
 BookerPdfTool/__main__.py
-BookerPdfTool/img2jb2pdf.py
 BookerPdfTool/pdf_tool.py
 BookerPdfTool/toggle_bw.py
 BookerPdfTool/util.py
 BookerPdfTool/zip_tool.py
 BookerPdfTool.egg-info/PKG-INFO
 BookerPdfTool.egg-info/SOURCES.txt
 BookerPdfTool.egg-info/dependency_links.txt
 BookerPdfTool.egg-info/entry_points.txt
 BookerPdfTool.egg-info/requires.txt
 BookerPdfTool.egg-info/top_level.txt
 BookerPdfTool/assets/7z.dll
 BookerPdfTool/assets/7z.exe
 BookerPdfTool/assets/PwdDic.txt
 BookerPdfTool/assets/__init__.py
-BookerPdfTool/assets/jbig2enc.dll
-BookerPdfTool/assets/jbig2enc.exe
 BookerPdfTool/assets/unrar.exe
```

### Comparing `BookerPdfTool-2023.7.19.1/LICENSE` & `BookerPdfTool-2023.7.22.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BookerPdfTool-2023.7.19.1/PKG-INFO` & `BookerPdfTool-2023.7.22.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BookerPdfTool
-Version: 2023.7.19.1
+Version: 2023.7.22.0
 Summary: iBooker/ApacheCN 知识库抓取工具
 Home-page: https://github.com/apachecn/BookerPdfTool
 Author: wizardforcel
 Author-email: wizard.z@qq.com
 Keywords: wiki,知识库,document,文档,crawler,爬虫
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `BookerPdfTool-2023.7.19.1/README.md` & `BookerPdfTool-2023.7.22.0/README.md`

 * *Files identical despite different names*

### Comparing `BookerPdfTool-2023.7.19.1/setup.py` & `BookerPdfTool-2023.7.22.0/setup.py`

 * *Files identical despite different names*

