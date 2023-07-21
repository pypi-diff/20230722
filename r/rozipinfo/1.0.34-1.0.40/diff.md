# Comparing `tmp/rozipinfo-1.0.34.tar.gz` & `tmp/rozipinfo-1.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rozipinfo-1.0.34.tar", last modified: Sun Jul  3 22:01:41 2022, max compression
+gzip compressed data, was "dist/rozipinfo-1.0.40.tar", last modified: Fri Jul 21 22:58:46 2023, max compression
```

## Comparing `rozipinfo-1.0.34.tar` & `rozipinfo-1.0.40.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 charles    (502) staff       (20)        0 2022-07-03 22:01:41.000000 rozipinfo-1.0.34/
--rw-rw-r--   0 charles    (502) staff       (20)     6747 2022-07-03 22:01:41.000000 rozipinfo-1.0.34/PKG-INFO
--rw-rw-r--   0 charles    (502) staff       (20)    54068 2022-07-03 20:37:25.000000 rozipinfo-1.0.34/rozipinfo.py
--rwxrwxr-x   0 charles    (502) staff       (20)    17803 2022-07-03 21:54:23.000000 rozipinfo-1.0.34/rozipfile.py
--rw-rw-r--   0 charles    (502) staff       (20)     5087 2022-07-03 20:49:30.000000 rozipinfo-1.0.34/README.md
--rwxrwxr-x   0 charles    (502) staff       (20)     1584 2022-07-03 22:01:40.000000 rozipinfo-1.0.34/setup.py
--rw-rw-r--   0 charles    (502) staff       (20)       38 2022-07-03 22:01:41.000000 rozipinfo-1.0.34/setup.cfg
-drwxrwxr-x   0 charles    (502) staff       (20)        0 2022-07-03 22:01:41.000000 rozipinfo-1.0.34/rozipinfo.egg-info/
--rw-rw-r--   0 charles    (502) staff       (20)     6747 2022-07-03 22:01:41.000000 rozipinfo-1.0.34/rozipinfo.egg-info/PKG-INFO
--rw-rw-r--   0 charles    (502) staff       (20)      176 2022-07-03 22:01:41.000000 rozipinfo-1.0.34/rozipinfo.egg-info/SOURCES.txt
--rw-rw-r--   0 charles    (502) staff       (20)       20 2022-07-03 22:01:41.000000 rozipinfo-1.0.34/rozipinfo.egg-info/top_level.txt
--rw-rw-r--   0 charles    (502) staff       (20)        1 2022-07-03 22:01:41.000000 rozipinfo-1.0.34/rozipinfo.egg-info/dependency_links.txt
+drwxrwxr-x   0 charles    (502) staff       (20)        0 2023-07-21 22:58:46.000000 rozipinfo-1.0.40/
+-rw-rw-r--   0 charles    (502) staff       (20)     6939 2023-07-21 22:58:46.000000 rozipinfo-1.0.40/PKG-INFO
+-rw-rw-r--   0 charles    (502) staff       (20)    54448 2023-04-02 13:38:30.000000 rozipinfo-1.0.40/rozipinfo.py
+-rwxrwxr-x   0 charles    (502) staff       (20)    20344 2023-07-21 22:43:48.000000 rozipinfo-1.0.40/rozipfile.py
+-rw-rw-r--   0 charles    (502) staff       (20)     5239 2023-04-02 13:37:16.000000 rozipinfo-1.0.40/README.md
+-rwxrwxr-x   0 charles    (502) staff       (20)     1584 2023-07-21 22:58:45.000000 rozipinfo-1.0.40/setup.py
+-rw-rw-r--   0 charles    (502) staff       (20)       38 2023-07-21 22:58:46.000000 rozipinfo-1.0.40/setup.cfg
+drwxrwxr-x   0 charles    (502) staff       (20)        0 2023-07-21 22:58:46.000000 rozipinfo-1.0.40/rozipinfo.egg-info/
+-rw-rw-r--   0 charles    (502) staff       (20)     6939 2023-07-21 22:58:46.000000 rozipinfo-1.0.40/rozipinfo.egg-info/PKG-INFO
+-rw-rw-r--   0 charles    (502) staff       (20)      176 2023-07-21 22:58:46.000000 rozipinfo-1.0.40/rozipinfo.egg-info/SOURCES.txt
+-rw-rw-r--   0 charles    (502) staff       (20)       20 2023-07-21 22:58:46.000000 rozipinfo-1.0.40/rozipinfo.egg-info/top_level.txt
+-rw-rw-r--   0 charles    (502) staff       (20)        1 2023-07-21 22:58:46.000000 rozipinfo-1.0.40/rozipinfo.egg-info/dependency_links.txt
```

### Comparing `rozipinfo-1.0.34/PKG-INFO` & `rozipinfo-1.0.40/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rozipinfo
-Version: 1.0.34
+Version: 1.0.40
 Summary: Managing Zip archives with RISC OS filetype information present
 Home-page: https://github.com/gerph/python-zipinfo-riscos
 Author: Charles Ferguson
 Author-email: gerph@gerph.org
 License: BSD
 Description: # Python ZipInfo processing for RISC OS archives
         
@@ -114,14 +114,19 @@
         
             python -m rozipfile [--chdir <dir>] --create <archive> <files>*
         
         Extracting an archive:
         
             python -m rozipfile [--chdir <dir>] --extract <archive> <files>*
         
+        Producing a list of *SetType commands to restore filetypes from a badly extracted file:
+        
+            python -m rozipfile [--chdir <dir>] --settypes <archive>
+        
+        
         ### Default filetype
         
         The default filetype for files that don't have any RISC OS extension information present (either as NFS-encoding or RISC OS extensions) is &FFD (Data). However, the switch `--default-filetype` can be used to default to a different type. Most commonly you may wish to set the default filetype to Text with `--default-filetype text`.
         
         
         ## Tests
```

### Comparing `rozipinfo-1.0.34/rozipinfo.py` & `rozipinfo-1.0.40/rozipinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,14 +383,20 @@
             for field in zipinfo.__class__.__slots__:
                 if field != 'extra' and field != 'filename':
                     setattr(self, field, getattr(zipinfo, field, None))
             # Always populate the extra field last, as this modifies the existing fields
             # based on what the RISC OS extra field contains.
             self.extra = zipinfo.extra
 
+            # Some archive tools have written the filename ending in a '/' but not marked the
+            # file as being a directory. This causes problems when we try to extract because we
+            # create a 0 length file, which then cannot be a directory.
+            if self.filename.endswith('/'):
+                self.external_attr |= self.external_attr_msdos_directory
+
         self._nfs_encoding = nfs_encoding
         self.create_system = 13  # RISC OS
 
     def __repr__(self):
         try:
             ro_load = '&{:08x}({})'.format(self.riscos_loadaddr, 'inferred' if self._riscos_loadaddr is None else 'set')
             ro_exec = '&{:08x}({})'.format(self.riscos_execaddr, 'inferred' if self._riscos_execaddr is None else 'set')
```

### Comparing `rozipinfo-1.0.34/rozipfile.py` & `rozipinfo-1.0.40/rozipfile.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 import re
 import sys
 import zipfile
 
 import rozipinfo
 
 
+# Whether the Python zipfile module supports compression levels.
+has_compression_level = sys.version_info > (3, 7)
+
+
 class RISCOSZipFileError(Exception):
     pass
 
 
 class RISCOSZipFile(object):
     named_types = {
             0xFFF: 'Text',
@@ -82,18 +86,20 @@
             0x132: 'ICO',
         }
     inv_named_types = dict((name.lower(), filetype) for filetype, name in named_types.items())
     cls_zipinfo = rozipinfo.ZipInfoRISCOS
 
     escapable_re = re.compile(br'[\x00-\x1f\x7f-\xff]')
 
-    def __init__(self, zip_filename, mode='r', base_dir='.', default_filetype=None):
+    def __init__(self, zip_filename, mode='r', compression=zipfile.ZIP_STORED,
+                 base_dir='.', default_filetype=None):
         self.zip_filename = zip_filename
+        self.compression = compression
         self.mode = mode
-        self.zh = zipfile.ZipFile(zip_filename, mode)
+        self.zh = zipfile.ZipFile(zip_filename, mode, compression)
         if default_filetype:
             if default_filetype in self.inv_named_types:
                 # It's a named type
                 default_filetype = self.inv_named_types[default_filetype.lower()]
             else:
                 if default_filetype[0] == '&':
                     default_filetype = default_filetype[1:]
@@ -137,46 +143,51 @@
                     filetype += ' ({})'.format(type_name)
             else:
                 filetype = 'load/exec &{:08X}/&{:08X}'.format(zi.riscos_loadaddr, zi.riscos_execaddr)
             self.verbose("File {!r}, size {} bytes, {}".format(zi.riscos_filename,
                                                                zi.file_size,
                                                                filetype))
 
-    def add_file(self, filename, verbose=False):
+    def add_file(self, filename, verbose=False, compresslevel=None):
         zipname = os.path.relpath(filename, self.base_dir)
         zi = self.cls_zipinfo.from_file(filename=filename, arcname=zipname, nfs_encoding=True)
+        zi.compress_type = self.compression
         zi.nfs_encoding = False
         if verbose:
             self.verbose_object(zi)
         with open(filename, 'rb') as fh:
             data = fh.read()
-        self.zh.writestr(zi, data)
+        #print("Compression: %r"% (compresslevel,))
+        if compresslevel is None or not has_compression_level:
+            self.zh.writestr(zi, data)
+        else:
+            self.zh.writestr(zi, data, compresslevel=compresslevel)
 
-    def add_dir(self, filename, verbose=False):
+    def add_dir(self, filename, verbose=False, compresslevel=None):
         zipname = os.path.relpath(filename, self.base_dir)
         zi = self.cls_zipinfo.from_file(filename=filename, arcname=zipname, nfs_encoding=True)
         zi.nfs_encoding = False
         self.zh.writestr(zi, b'')
 
         if verbose:
             self.verbose_object(zi)
 
         # Having written this directory, we now need to write each of the objects within it.
         for name in os.listdir(filename):
             new_filename = os.path.join(filename, name)
-            self.add_to_zipfile(new_filename, verbose=verbose)
+            self.add_to_zipfile(new_filename, verbose=verbose, compresslevel=compresslevel)
 
-    def add_to_zipfile(self, filename, verbose=False):
+    def add_to_zipfile(self, filename, verbose=False, compresslevel=None):
         if os.path.isfile(filename):
             # This is a simple file
-            self.add_file(filename, verbose=verbose)
+            self.add_file(filename, verbose=verbose, compresslevel=compresslevel)
 
         elif os.path.isdir(filename):
             # This is a directory, so we want to add everything within it
-            self.add_dir(filename, verbose=verbose)
+            self.add_dir(filename, verbose=verbose, compresslevel=compresslevel)
 
         else:
             raise RuntimeError("Cannot add '{}' as it is not a file or directory".format(filename.encode('utf-8')))
 
     def __enter__(self):
         return self
 
@@ -381,15 +392,15 @@
         if isinstance(member, str):
             zi = self.getinfo(member)
         else:
             zi = member
         return self.zh.read(zi)
 
     def extract(self, member, path=None, verbose=False):
-        if isinstance(member, str):
+        if isinstance(member, (str, bytes)):
             zi = self.getinfo(member)
         else:
             if isinstance(member, rozipinfo.ZipInfoRISCOS):
                 zi = member
             else:
                 zi = rozipinfo.ZipInfoRISCOS(zipinfo=member)
 
@@ -427,59 +438,91 @@
 
         for member in members:
             self.extract(member, path, verbose=verbose)
 
 
 def main():
     parser = argparse.ArgumentParser()
+    parser.add_argument('-0', '--store',      dest='compression', action='store_const', const=0, default=6,
+                        help="Compression level: Store")
+    if has_compression_level:
+        parser.add_argument('-1', '--faster', dest='compression', action='store_const', const=1,
+                            help="Compression level: Deflate level 1 (faster)")
+    parser.add_argument('-6', '--deflate',    dest='compression', action='store_const', const=6,
+                        help="Compression level: Deflate level 6 (default)")
+    if has_compression_level:
+        parser.add_argument('-9', '--better', dest='compression', action='store_const', const=9,
+                            help="Compression level: Deflate level 9 (best)")
     parser.add_argument('-v', '--verbose', action='store_true',
                         help="Output more information during processing")
     parser.add_argument('-T', '--default-filetype', default=None,
                         help="Default filetype to use for files without type")
     parser.add_argument('-C', '--chdir', default='.',
                         help="Base directory for the reading or writing files")
     parser.add_argument('-c', '--create', action='store_true',
                         help="Create a RISC OS zip archive, from files with NFS encoding")
     parser.add_argument('-e', '--extract', action='store_true',
                         help="Extract files from a RISC OS zip archive, to files with NFS encoding")
     parser.add_argument('-l', '--list', action='store_true',
                         help="List the contents of a RISC OS zip archive")
+    parser.add_argument('-t', '--settypes', action='store_true',
+                        help="Output *SetType commands to restore filetypes on an incorrectly extracted file")
     parser.add_argument('zipfile',
                         help="Zip archive to create")
     parser.add_argument('content', nargs='*',
                         help="Files/directories to add to the archive")
 
     options = parser.parse_args()
 
     zip_filename = os.path.abspath(options.zipfile)
 
+    compression = zipfile.ZIP_DEFLATED if options.compression else zipfile.ZIP_STORED
+    #print("Compression %r/%r" % (compression, options.compression))
+
     try:
         if options.create:
-            with RISCOSZipFile(zip_filename, 'w', base_dir=options.chdir, default_filetype=options.default_filetype) as rzh:
+            with RISCOSZipFile(zip_filename, 'w', compression=compression,
+                               base_dir=options.chdir, default_filetype=options.default_filetype) as rzh:
 
                 options.chdir = os.path.abspath(options.chdir)
                 for filename in options.content:
-                    rzh.add_to_zipfile(filename, verbose=options.verbose)
+                    rzh.add_to_zipfile(filename,
+                                       verbose=options.verbose,
+                                       compresslevel=options.compression)
 
         elif options.list:
             with RISCOSZipFile(zip_filename, 'r', default_filetype=options.default_filetype) as zh:
                 if options.verbose:
                     zh.printdir_verbose()
                 else:
                     zh.printdir()
 
+        elif options.settypes:
+            with RISCOSZipFile(zip_filename, 'r',
+                               default_filetype=options.default_filetype) as zh:
+                for zi in zh.infolist():
+                    if zi.riscos_objtype == 1:
+                        name = zi.riscos_filename.decode(zi.filename_encoding_name)
+                        print("*SetType {} &{:3X}".format(name, zi.riscos_filetype))
+
         elif options.extract:
-            with RISCOSZipFile(zip_filename, 'r', default_filetype=options.default_filetype) as zh:
+            with RISCOSZipFile(zip_filename, 'r',
+                               default_filetype=options.default_filetype) as zh:
                 zh.extractall(path=options.chdir, verbose=options.verbose,
                               members=options.content if options.content else None)
 
         else:
             sys.stderr.write("No action specified\n")
             sys.exit(1)
 
+    except IOError as exc:
+        # If the file doesn't exist, is inaccessible, or fails to read, we report as an IO error.
+        sys.stderr.write("Failed: IO error: {}\n".format(exc))
+        sys.exit(1)
+
     except RISCOSZipFileError as exc:
-        sys.stderr.write("Failed: {}\n".format(exc))
+        sys.stderr.write("Failed: Zip error {}\n".format(exc))
         sys.exit(1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `rozipinfo-1.0.34/README.md` & `rozipinfo-1.0.40/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,19 @@
 
     python -m rozipfile [--chdir <dir>] --create <archive> <files>*
 
 Extracting an archive:
 
     python -m rozipfile [--chdir <dir>] --extract <archive> <files>*
 
+Producing a list of *SetType commands to restore filetypes from a badly extracted file:
+
+    python -m rozipfile [--chdir <dir>] --settypes <archive>
+
+
 ### Default filetype
 
 The default filetype for files that don't have any RISC OS extension information present (either as NFS-encoding or RISC OS extensions) is &FFD (Data). However, the switch `--default-filetype` can be used to default to a different type. Most commonly you may wish to set the default filetype to Text with `--default-filetype text`.
 
 
 ## Tests
```

### Comparing `rozipinfo-1.0.34/setup.py` & `rozipinfo-1.0.40/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name = 'rozipinfo',
     py_modules = ['rozipfile', 'rozipinfo'],
-    version = '1.0.34',
+    version = '1.0.40',
     license='BSD',
     description = 'Managing Zip archives with RISC OS filetype information present',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     author = 'Charles Ferguson',
     author_email = 'gerph@gerph.org',
     url = 'https://github.com/gerph/python-zipinfo-riscos',
```

### Comparing `rozipinfo-1.0.34/rozipinfo.egg-info/PKG-INFO` & `rozipinfo-1.0.40/rozipinfo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rozipinfo
-Version: 1.0.34
+Version: 1.0.40
 Summary: Managing Zip archives with RISC OS filetype information present
 Home-page: https://github.com/gerph/python-zipinfo-riscos
 Author: Charles Ferguson
 Author-email: gerph@gerph.org
 License: BSD
 Description: # Python ZipInfo processing for RISC OS archives
         
@@ -114,14 +114,19 @@
         
             python -m rozipfile [--chdir <dir>] --create <archive> <files>*
         
         Extracting an archive:
         
             python -m rozipfile [--chdir <dir>] --extract <archive> <files>*
         
+        Producing a list of *SetType commands to restore filetypes from a badly extracted file:
+        
+            python -m rozipfile [--chdir <dir>] --settypes <archive>
+        
+        
         ### Default filetype
         
         The default filetype for files that don't have any RISC OS extension information present (either as NFS-encoding or RISC OS extensions) is &FFD (Data). However, the switch `--default-filetype` can be used to default to a different type. Most commonly you may wish to set the default filetype to Text with `--default-filetype text`.
         
         
         ## Tests
```

