# Comparing `tmp/python-gnupg-0.4.9.tar.gz` & `tmp/python-gnupg-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/disk2/vinay/projects/python-gnupg/dist/tmpwj4h5mju/python-gnupg-0.4.9.tar", last modified: Fri May 20 08:08:10 2022, max compression
+gzip compressed data, was "/disk2/vinay/projects/python-gnupg/dist/tmp5eg0wd4x/python-gnupg-0.5.0.tar", last modified: Tue Aug 23 15:52:00 2022, max compression
```

## Comparing `python-gnupg-0.4.9.tar` & `python-gnupg-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-05-20 08:08:10.000000 python-gnupg-0.4.9/
--rw-r--r--   0 vinay     (1000) vinay     (1000)     6724 2019-05-09 06:37:26.000000 python-gnupg-0.4.9/test_secring.gpg
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-05-20 08:08:10.000000 python-gnupg-0.4.9/python_gnupg.egg-info/
--rw-r--r--   0 vinay     (1000) vinay     (1000)      274 2022-05-20 08:08:10.000000 python-gnupg-0.4.9/python_gnupg.egg-info/SOURCES.txt
--rw-r--r--   0 vinay     (1000) vinay     (1000)        6 2022-05-20 08:08:10.000000 python-gnupg-0.4.9/python_gnupg.egg-info/top_level.txt
--rw-r--r--   0 vinay     (1000) vinay     (1000)     1932 2022-05-20 08:08:10.000000 python-gnupg-0.4.9/python_gnupg.egg-info/PKG-INFO
--rw-r--r--   0 vinay     (1000) vinay     (1000)        1 2022-05-20 08:08:10.000000 python-gnupg-0.4.9/python_gnupg.egg-info/dependency_links.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     1913 2022-05-20 08:08:10.000000 python-gnupg-0.4.9/setup.cfg
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    70531 2022-05-20 08:02:15.000000 python-gnupg-0.4.9/test_gnupg.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    65170 2022-05-20 08:01:43.000000 python-gnupg-0.4.9/gnupg.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     1468 2022-03-09 20:04:33.000000 python-gnupg-0.4.9/LICENSE.txt
--rw-r--r--   0 vinay     (1000) vinay     (1000)    19992 2020-04-17 06:02:24.000000 python-gnupg-0.4.9/messages.json
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     1932 2022-05-20 08:08:10.000000 python-gnupg-0.4.9/PKG-INFO
--rw-r--r--   0 vinay     (1000) vinay     (1000)      107 2020-04-17 06:50:10.000000 python-gnupg-0.4.9/MANIFEST.in
--rw-r--r--   0 vinay     (1000) vinay     (1000)     4399 2019-05-09 06:37:26.000000 python-gnupg-0.4.9/test_pubring.gpg
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      117 2022-05-09 18:48:23.000000 python-gnupg-0.4.9/pyproject.toml
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    17857 2022-05-20 07:14:52.000000 python-gnupg-0.4.9/README.rst
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-23 15:52:00.000000 python-gnupg-0.5.0/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     6724 2019-05-09 06:37:26.000000 python-gnupg-0.5.0/test_secring.gpg
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-08-23 15:52:00.000000 python-gnupg-0.5.0/python_gnupg.egg-info/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      274 2022-08-23 15:52:00.000000 python-gnupg-0.5.0/python_gnupg.egg-info/SOURCES.txt
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        6 2022-08-23 15:52:00.000000 python-gnupg-0.5.0/python_gnupg.egg-info/top_level.txt
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     1932 2022-08-23 15:52:00.000000 python-gnupg-0.5.0/python_gnupg.egg-info/PKG-INFO
+-rw-r--r--   0 vinay     (1000) vinay     (1000)        1 2022-08-23 15:52:00.000000 python-gnupg-0.5.0/python_gnupg.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     1913 2022-08-23 15:52:00.000000 python-gnupg-0.5.0/setup.cfg
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    73221 2022-08-23 15:37:02.000000 python-gnupg-0.5.0/test_gnupg.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    67038 2022-08-23 15:36:40.000000 python-gnupg-0.5.0/gnupg.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     1468 2022-03-09 20:04:33.000000 python-gnupg-0.5.0/LICENSE.txt
+-rw-r--r--   0 vinay     (1000) vinay     (1000)    19992 2020-04-17 06:02:24.000000 python-gnupg-0.5.0/messages.json
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     1932 2022-08-23 15:52:00.000000 python-gnupg-0.5.0/PKG-INFO
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      107 2020-04-17 06:50:10.000000 python-gnupg-0.5.0/MANIFEST.in
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     4399 2019-05-09 06:37:26.000000 python-gnupg-0.5.0/test_pubring.gpg
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      117 2022-05-09 18:48:23.000000 python-gnupg-0.5.0/pyproject.toml
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    18701 2022-08-23 08:08:24.000000 python-gnupg-0.5.0/README.rst
```

### Comparing `python-gnupg-0.4.9/test_secring.gpg` & `python-gnupg-0.5.0/test_secring.gpg`

 * *Files identical despite different names*

### Comparing `python-gnupg-0.4.9/python_gnupg.egg-info/PKG-INFO` & `python-gnupg-0.5.0/python_gnupg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gnupg
-Version: 0.4.9
+Version: 0.5.0
 Summary: A wrapper for the Gnu Privacy Guard (GPG or GnuPG)
 Home-page: https://github.com/vsajip/python-gnupg
 Author: Vinay Sajip
 Author-email: vinay_sajip@yahoo.co.uk
 Maintainer: Vinay Sajip
 Maintainer-email: vinay_sajip@yahoo.co.uk
 License: BSD
```

### Comparing `python-gnupg-0.4.9/setup.cfg` & `python-gnupg-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-gnupg-0.4.9/test_gnupg.py` & `python-gnupg-0.5.0/test_gnupg.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,18 +26,20 @@
         else:
             return lambda x: None
 
 
 import gnupg
 
 __author__ = 'Vinay Sajip'
-__date__ = '$20-May-2022 09:02:15$'
+__date__ = '$23-Aug-2022 16:37:02$'
 
 ALL_TESTS = True
 
+gnupg.log_everything = True
+
 logger = logging.getLogger(__name__)
 
 GPGBINARY = os.environ.get('GPGBINARY', 'gpg')
 
 KEYS_TO_IMPORT = """-----BEGIN PGP PUBLIC KEY BLOCK-----
 Version: GnuPG v1.4.9 (MingW32)
 
@@ -975,16 +977,16 @@
         data_file = open(self.test_fn, 'rb')
         sig = self.gpg.sign_file(data_file, keyid=key.fingerprint, passphrase='aable')
         self.assertEqual(0, sig.returncode, 'Non-zero return code')
         data_file.close()
         self.assertTrue(sig, 'File signing should succeed')
         self.assertTrue(sig.hash_algo)
         try:
-            file = gnupg._make_binary_stream(sig.data, self.gpg.encoding)
-            verified = self.gpg.verify_file(file)
+            stream = gnupg._make_binary_stream(sig.data, self.gpg.encoding)
+            verified = self.gpg.verify_file(stream)
         except UnicodeDecodeError:  # pragma: no cover
             # sometimes happens in Python 2.6
             from io import BytesIO
             verified = self.gpg.verify_file(BytesIO(sig.data))
         self.assertEqual(0, verified.returncode, 'Non-zero return code')
         if key.fingerprint != verified.fingerprint:  # pragma: no cover
             logger.debug('key: %r', key.fingerprint)
@@ -1008,21 +1010,21 @@
             logger.debug('key: %r', key.fingerprint)
             logger.debug('ver: %r', verified.fingerprint)
         self.assertEqual(key.fingerprint, verified.fingerprint, 'Fingerprints must match')
         # Test in-memory verification
         data_file = open(self.test_fn, 'rb')
         data = data_file.read()
         data_file.close()
-        fd, fn = tempfile.mkstemp()
+        fd, fn = tempfile.mkstemp(prefix='pygpg-test-')
         os.write(fd, sig.data)
         os.close(fd)
         try:
             verified = self.gpg.verify_data(fn, data)
         finally:
-            os.unlink(fn)
+            os.remove(fn)
         self.assertEqual(0, verified.returncode, 'Non-zero return code')
         if key.fingerprint != verified.fingerprint:  # pragma: no cover
             logger.debug('key: %r', key.fingerprint)
             logger.debug('ver: %r', verified.fingerprint)
         self.assertEqual(key.fingerprint, verified.fingerprint, 'Fingerprints must match')
 
     def test_signature_file(self):
@@ -1045,15 +1047,15 @@
         data = data_file.read()
         data_file.close()
         try:
             verified = self.gpg.verify_data(sig_file, data)
             self.assertTrue(verified.username.startswith('Andrew Able'))
             self.assertTrue(key.fingerprint.endswith(verified.key_id))
         finally:
-            os.unlink(sig_file)
+            os.remove(sig_file)
         self.assertEqual(0, verified.returncode, 'Non-zero return code')
         if key.fingerprint != verified.fingerprint:
             logger.debug('key: %r', key.fingerprint)
             logger.debug('ver: %r', verified.fingerprint)
         self.assertEqual(key.fingerprint, verified.fingerprint, 'Fingerprints must match')
 
     def test_subkey_signature_file(self):
@@ -1092,15 +1094,15 @@
         data = data_file.read()
         data_file.close()
         try:
             verified = self.gpg.verify_data(sig_file, data)
             self.assertTrue(verified.username.startswith('Charlie Clark'))
             self.assertTrue(subkey.fingerprint.endswith(verified.key_id))
         finally:
-            os.unlink(sig_file)
+            os.remove(sig_file)
         self.assertEqual(0, verified.returncode, 'Non-zero return code')
         if subkey.fingerprint != verified.fingerprint:
             logger.debug('key: %r', subkey.fingerprint)
             logger.debug('ver: %r', verified.fingerprint)
         self.assertEqual(subkey.fingerprint, verified.fingerprint, 'Fingerprints must match')
 
     def test_deletion(self):
@@ -1153,16 +1155,16 @@
             key = self.generate_key('Andrew', 'Able', 'alpha.com', passphrase='andy')
             self.assertEqual(0, key.returncode, 'Non-zero return code')
             andrew = key.fingerprint
             key = self.generate_key('Barbara', 'Brown', 'beta.com')
             self.assertEqual(0, key.returncode, 'Non-zero return code')
             barbara = key.fingerprint
             data = 'Hello, world!'
-            file = gnupg._make_binary_stream(data, self.gpg.encoding)
-            edata = self.gpg.encrypt_file(file, [andrew, barbara], armor=False, output=encfname)
+            stream = gnupg._make_binary_stream(data, self.gpg.encoding)
+            edata = self.gpg.encrypt_file(stream, [andrew, barbara], armor=False, output=encfname)
             self.assertEqual(0, edata.returncode, 'Non-zero return code')
             efile = open(encfname, 'rb')
             ddata = self.gpg.decrypt_file(efile, passphrase='bbrown', output=decfname)
             self.assertEqual(0, ddata.returncode, 'Non-zero return code')
             efile.seek(0, os.SEEK_SET)
             edata = efile.read()
             efile.close()
@@ -1192,25 +1194,25 @@
                     # mode bits we set are still in effect
                     self.assertEqual(os.stat(fn).st_mode, mode)
                 if os.path.exists(fn):
                     os.remove(fn)
 
     def test_file_encryption_and_decryption(self):
         "Test that encryption/decryption to/from file works"
-        encfno, encfname = tempfile.mkstemp()
-        decfno, decfname = tempfile.mkstemp()
+        encfno, encfname = tempfile.mkstemp(prefix='pygpg-test-')
+        decfno, decfname = tempfile.mkstemp(prefix='pygpg-test-')
         # On Windows, if the handles aren't closed, the files can't be deleted
         os.close(encfno)
         os.close(decfno)
         self.do_file_encryption_and_decryption(encfname, decfname)
 
     @skipIf(os.name == 'nt', 'Test not suitable for Windows')
     def test_invalid_outputs(self):
         "Test encrypting to invalid output files"
-        encfno, encfname = tempfile.mkstemp()
+        encfno, encfname = tempfile.mkstemp(prefix='pygpg-test-')
         os.close(encfno)
         os.chmod(encfname, 0o400)
         cases = (
             ('/dev/null/foo', 'encrypt: not a directory'),
             (encfname, 'encrypt: permission denied'),
         )
         key = self.generate_key('Barbara', 'Brown', 'beta.com')
@@ -1231,15 +1233,15 @@
                 mdata = json.load(f)
             messages = {}
             for k, v in mdata.items():
                 messages[int(k, 16)] = v
 
             self.gpg.error_map = messages
 
-            encfno, encfname = tempfile.mkstemp()
+            encfno, encfname = tempfile.mkstemp(prefix='pygpg-test-')
             os.close(encfno)
             os.chmod(encfname, 0o400)
 
             try:
                 cases = (
                     ('/dev/null/foo', 'encrypt: Not a directory'),
                     (encfname, 'encrypt: Permission denied'),
@@ -1417,17 +1419,22 @@
     def test_recv_keys_no_server(self):
         result = self.gpg.recv_keys('foo.bar.baz', '92905378')
         self.assertEqual(2, result.returncode, 'Unexpected return code')
         self.assertEqual(result.summary(), '0 imported')
 
     def test_invalid_fileobject(self):
         # accidentally on purpose pass in a filename rather than the file itself
-        with self.assertRaises(TypeError) as ec:
-            self.gpg.decrypt_file('foobar.txt', passphrase='', output='/tmp/decrypted.txt')
-        self.assertEqual(str(ec.exception), 'Not a valid file: foobar.txt')
+        bad = b'foobar.txt'
+        with self.assertRaises((TypeError, ValueError)) as ec:
+            self.gpg.decrypt_file(bad, passphrase='', output='/tmp/decrypted.txt')
+        if gnupg._py3k:
+            expected = 'Not a valid file or path: %s' % bad
+        else:
+            expected = 'No such file: %s' % bad
+        self.assertEqual(str(ec.exception), expected)
 
     def remove_all_existing_keys(self):
         for root, dirs, files in os.walk(self.homedir):
             for d in dirs:
                 p = os.path.join(root, d)
                 shutil.rmtree(p)
             for f in files:
@@ -1464,14 +1471,66 @@
         ids = gpg.get_recipients(edata.data.decode(gpg.encoding))
         self.assertGreater(len(ids), 0)
         idlen = len(ids[0])
         ids = set(ids)
         expected = set((key1.fingerprint[-idlen:], key2.fingerprint[-idlen:]))
         self.assertEqual(expected, ids)
 
+    def test_passing_paths(self):
+        key1 = self.generate_key('Andrew', 'Able', 'alpha.com', passphrase='andy')
+        self.assertEqual(0, key1.returncode, 'Non-zero return code')
+        andrew = key1.fingerprint
+        key2 = self.generate_key('Barbara', 'Brown', 'beta.com')
+        self.assertEqual(0, key2.returncode, 'Non-zero return code')
+        barbara = key2.fingerprint
+        data = b'Hello, world!'
+        fd, fn = tempfile.mkstemp(prefix='pygpg-test-')
+        os.write(fd, data)
+        os.close(fd)
+        gpg = self.gpg
+        try:
+            # Check encryption
+            edata = gpg.encrypt_file(fn, [andrew, barbara], armor=False)
+            self.assertEqual(0, edata.returncode, 'Non-zero return code')
+            self.assertEqual(edata.status, 'encryption ok')
+            with open(fn, 'wb') as f:
+                f.write(edata.data)
+            # Check getting recipients
+            ids = gpg.get_recipients_file(fn)
+            idlen = len(ids[0])
+            keys = gpg.list_keys()
+            expected = set(d['subkeys'][0][0][-idlen:] for d in keys)
+            self.assertEqual(set(ids), expected)
+            # Check decryption
+            ddata = gpg.decrypt_file(fn, passphrase='andy')
+            self.assertEqual(0, ddata.returncode, 'Non-zero return code')
+            self.assertEqual(ddata.status, 'decryption ok')
+            self.assertEqual(ddata.data, data)
+            # Check signing
+            with open(fn, 'wb') as f:
+                f.write(data)
+            sig = gpg.sign_file(fn, keyid=andrew, passphrase='andy', binary=True)
+            self.assertEqual(0, sig.returncode, 'Non-zero return code')
+            self.assertEqual(sig.status, 'signature created')
+            # Check verification
+            with open(fn, 'wb') as f:
+                f.write(sig.data)
+            verified = gpg.verify_file(fn)
+            self.assertEqual(0, verified.returncode, 'Non-zero return code')
+            self.assertEqual(verified.status, 'signature valid')
+            self.assertTrue(verified.valid)
+            # Check importing keys
+            with open(fn, 'wb') as f:
+                f.write(KEYS_TO_IMPORT.encode('ascii'))
+            result = gpg.import_keys_file(fn)
+            self.assertEqual(0, result.returncode, 'Non-zero return code')
+            self.assertEqual(result.imported, 2)
+        finally:
+            os.remove(fn)
+
 
 TEST_GROUPS = {
     'sign':
     set(['test_signature_verification', 'test_signature_file', 'test_subkey_signature_file']),
     'crypt':
     set([
         'test_encryption_and_decryption', 'test_file_encryption_and_decryption',
@@ -1490,15 +1549,15 @@
     set(['test_import_only', 'test_doctest_import_keys']),
     'basic':
     set([
         'test_environment', 'test_list_keys_initial', 'test_nogpg', 'test_make_args',
         'test_quote_with_shell'
     ]),
     'test':
-    set(['test_key_generation_failure']),
+    set(['test_passing_paths']),
 }
 
 
 def suite(args=None):
     if args is None:
         args = sys.argv[1:]
     if not args:
```

### Comparing `python-gnupg-0.4.9/gnupg.py` & `python-gnupg-0.5.0/gnupg.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,39 +38,48 @@
 import os
 import re
 import socket
 from subprocess import Popen, PIPE
 import sys
 import threading
 
-__version__ = '0.4.9'
+__version__ = '0.5.0'
 __author__ = 'Vinay Sajip'
-__date__ = '$20-May-2022 09:01:43$'
+__date__ = '$23-Aug-2022 16:36:40$'
 
 STARTUPINFO = None
 if os.name == 'nt':  # pragma: no cover
     try:
         from subprocess import STARTUPINFO, STARTF_USESHOWWINDOW, SW_HIDE
     except ImportError:
         STARTUPINFO = None
 
 try:
     unicode
     _py3k = False
     string_types = basestring
     text_type = unicode
+    path_types = (bytes, str)
 except NameError:
     _py3k = True
     string_types = str
     text_type = str
+    path_types = (str,)
 
 logger = logging.getLogger(__name__)
 if not logger.handlers:
     logger.addHandler(logging.NullHandler())
 
+# See gh-196: Logging could show sensitive data. It also produces some voluminous
+# output. Hence, split into two tiers - stuff that's always logged, and stuff that's
+# only logged if log_everything is True. (This is set by the test script.)
+#
+# For now, only debug logging of chunks falls into the optionally-logged category.
+log_everything = False
+
 # We use the test below because it works for Jython as well as CPython
 if os.path.__name__ == 'ntpath':  # pragma: no cover
     # On Windows, we don't need shell quoting, other than worrying about
     # paths with spaces in them.
     def shell_quote(s):
         return '"%s"' % s
 else:
@@ -131,26 +140,26 @@
     else:  # pragma: no cover
         enc = 'ascii'
     while True:
         # See issue #39: read can fail when e.g. a text stream is provided
         # for what is actually a binary file
         try:
             data = instream.read(1024)
-        except UnicodeError:
+        except Exception:  # pragma: no cover
             logger.warning('Exception occurred while reading', exc_info=1)
             break
         if not data:
             break
         sent += len(data)
         # logger.debug('sending chunk (%d): %r', sent, data[:256])
         try:
             outstream.write(data)
         except UnicodeError:  # pragma: no cover
             outstream.write(data.encode(enc))
-        except Exception:
+        except Exception:  # pragma: no cover
             # Can sometimes get 'broken pipe' errors even when the data has all
             # been sent
             logger.exception('Error sending data')
             break
     try:
         outstream.close()
     except IOError:  # pragma: no cover
@@ -287,35 +296,33 @@
             update_sig_info(keyid=self.key_id, username=self.username, status=self.status)
         elif key == 'GOODSIG':
             self.valid = True
             self.status = 'signature good'
             self.key_id, self.username = value.split(None, 1)
             update_sig_info(keyid=self.key_id, username=self.username, status=self.status)
         elif key == 'VALIDSIG':
-            fingerprint, creation_date, sig_ts, expire_ts = value.split()[:4]
+            parts = value.split()
+            fingerprint, creation_date, sig_ts, expire_ts = parts[:4]
             (self.fingerprint, self.creation_date, self.sig_timestamp,
              self.expire_timestamp) = (fingerprint, creation_date, sig_ts, expire_ts)
             # may be different if signature is made with a subkey
-            self.pubkey_fingerprint = value.split()[-1]
+            if len(parts) >= 10:
+                self.pubkey_fingerprint = parts[9]
             self.status = 'signature valid'
             update_sig_info(fingerprint=fingerprint,
                             creation_date=creation_date,
                             timestamp=sig_ts,
                             expiry=expire_ts,
                             pubkey_fingerprint=self.pubkey_fingerprint,
                             status=self.status)
         elif key == 'SIG_ID':
             sig_id, creation_date, timestamp = value.split()
             self.sig_info[sig_id] = {'creation_date': creation_date, 'timestamp': timestamp}
             (self.signature_id, self.creation_date, self.timestamp) = (sig_id, creation_date,
                                                                        timestamp)
-        elif key == 'DECRYPTION_FAILED':  # pragma: no cover
-            self.valid = False
-            self.key_id = value
-            self.status = 'decryption failed'
         elif key == 'NO_PUBKEY':  # pragma: no cover
             self.valid = False
             self.key_id = value
             self.status = 'no public key'
         elif key == 'NO_SECKEY':  # pragma: no cover
             self.valid = False
             self.key_id = value
@@ -328,15 +335,14 @@
                 self.key_status = 'signing key has expired'
             else:
                 self.key_status = 'signing key was revoked'
             self.status = self.key_status
             update_sig_info(status=self.status, keyid=self.key_id)
         elif key in ('UNEXPECTED', 'FAILURE'):  # pragma: no cover
             self.valid = False
-            self.key_id = value
             if key == 'UNEXPECTED':
                 self.status = 'unexpected data'
             else:
                 # N.B. there might be other reasons. For example, if an output
                 # file can't  be created - /dev/null/foo will lead to a
                 # "not a directory" error, but which is not sent as a status
                 # message with the [GNUPG:] prefix. Similarly if you try to
@@ -355,14 +361,18 @@
                             mapping = self.GPG_SYSTEM_ERROR_CODES
                         else:
                             mapping = self.GPG_ERROR_CODES
                         if code in mapping:
                             message = '%s: %s' % (operation, mapping[code])
                 if not self.status:
                     self.status = message
+        elif key == 'NODATA':
+            # See issue GH-191
+            self.valid = False
+            self.status = 'signature expected but not found'
         elif key in ('DECRYPTION_INFO', 'PLAINTEXT', 'PLAINTEXT_LENGTH', 'BEGIN_SIGNING'):
             pass
         else:  # pragma: no cover
             logger.debug('message ignored: %s, %s', key, value)
 
 
 class ImportResult(object):
@@ -378,15 +388,15 @@
         self.gpg = gpg
         self.results = []
         self.fingerprints = []
         for result in self.counts:
             setattr(self, result, 0)
 
     def __nonzero__(self):
-        if self.not_imported or not self.fingerprints:
+        if self.not_imported or not self.fingerprints:  # pragma: no cover
             return False
         return True
 
     __bool__ = __nonzero__
 
     ok_reason = {
         '0': 'Not actually changed',
@@ -402,15 +412,15 @@
         '1': 'Invalid Certificate',
         '2': 'Issuer Certificate missing',
         '3': 'Certificate Chain too long',
         '4': 'Error storing certificate',
     }
 
     def handle_status(self, key, value):
-        if key in ('WARNING', 'ERROR'):
+        if key in ('WARNING', 'ERROR'):  # pragma: no cover
             logger.warning('potential problem: %s: %s', key, value)
         elif key in ('IMPORTED', 'KEY_CONSIDERED'):
             # this duplicates info we already see in import_ok & import_problem
             pass
         elif key == 'NODATA':  # pragma: no cover
             self.results.append({
                 'fingerprint': None,
@@ -714,15 +724,16 @@
     def __str__(self):
         return self.fingerprint
 
     def handle_status(self, key, value):
         if key in ('WARNING', 'ERROR'):  # pragma: no cover
             logger.warning('potential problem: %s: %s', key, value)
         elif key == 'KEY_CREATED':
-            (self.type, self.fingerprint) = value.split()
+            parts = value.split()
+            (self.type, self.fingerprint) = parts[:2]
             self.status = 'ok'
         elif key == 'KEY_NOT_CREATED':
             self.status = key.replace('_', ' ').lower()
         elif key in ('PROGRESS', 'GOOD_PASSPHRASE'):
             pass
         else:  # pragma: no cover
             logger.debug('message ignored: %s, %s', key, value)
@@ -876,29 +887,32 @@
     def __init__(self,
                  gpgbinary='gpg',
                  gnupghome=None,
                  verbose=False,
                  use_agent=False,
                  keyring=None,
                  options=None,
-                 secret_keyring=None):
+                 secret_keyring=None,
+                 env=None):
         """Initialize a GPG process wrapper.  Options are:
 
         gpgbinary -- full pathname for GPG binary.
 
         gnupghome -- full pathname to where we can find the public and
         private keyrings.  Default is whatever gpg defaults to.
         keyring -- name of alternative keyring file to use, or list of such
         keyrings. If specified, the default keyring is not used.
         options =-- a list of additional options to pass to the GPG binary.
         secret_keyring -- name of alternative secret keyring file to use, or
         list of such keyrings.
+        env -- a dict of environment variables
         """
         self.gpgbinary = gpgbinary
         self.gnupghome = gnupghome
+        self.env = env
         # issue 112: fail if the specified value isn't a directory
         if gnupghome and not os.path.isdir(gnupghome):
             raise ValueError('gnupghome should be a directory (it isn\'t): %s' % gnupghome)
         if keyring:
             # Allow passing a string or another iterable. Make it uniformly
             # a list of keyring filenames
             if isinstance(keyring, string_types):
@@ -986,15 +1000,15 @@
             print(debug_print(cmd))
         if not STARTUPINFO:
             si = None
         else:  # pragma: no cover
             si = STARTUPINFO()
             si.dwFlags = STARTF_USESHOWWINDOW
             si.wShowWindow = SW_HIDE
-        result = Popen(cmd, shell=False, stdin=PIPE, stdout=PIPE, stderr=PIPE, startupinfo=si)
+        result = Popen(cmd, shell=False, stdin=PIPE, stdout=PIPE, stderr=PIPE, startupinfo=si, env=self.env)
         logger.debug('%s: %s', result.pid, debug_print(cmd))
         return result
 
     def _read_response(self, stream, result):
         # Internal method: reads all the stderr output from GPG, taking notice
         # only of lines that begin with the magic [GNUPG:] prefix.
         #
@@ -1027,15 +1041,16 @@
         chunks = []
         while True:
             data = stream.read(1024)
             if len(data) == 0:
                 if on_data:
                     on_data(data)
                 break
-            logger.debug('chunk: %r' % data[:256])
+            if log_everything:
+                logger.debug('chunk: %r' % data[:256])
             append = True
             if on_data:
                 append = on_data(data) is not False
             if append:
                 chunks.append(data)
         if _py3k:
             # Join using b'' or '', as appropriate
@@ -1061,15 +1076,15 @@
         dr.daemon = True
         logger.debug('stdout reader: %r', dr)
         dr.start()
 
         dr.join()
         rr.join()
         if writer is not None:
-            writer.join()
+            writer.join(0.01)
         process.wait()
         result.returncode = rc = process.returncode
         if rc != 0:
             logger.warning('gpg returned a non-zero error code: %d', rc)
         if stdin is not None:
             try:
                 stdin.close()
@@ -1081,31 +1096,45 @@
 
     def is_valid_file(self, fileobj):
         """
         Simplistic check for a file object
         """
         return hasattr(fileobj, 'read')
 
-    def _handle_io(self, args, fileobj, result, passphrase=None, binary=False):
-        "Handle a call to GPG - pass input data, collect output data"
-        # Handle a basic data call - pass data to GPG, handle the output
-        # including status information. Garbage In, Garbage Out :)
-        if not self.is_valid_file(fileobj):
-            raise TypeError('Not a valid file: %s' % fileobj)
-        p = self._open_subprocess(args, passphrase is not None)
-        if not binary:  # pragma: no cover
-            stdin = codecs.getwriter(self.encoding)(p.stdin)
+    def _get_fileobj(self, fileobj_or_path):
+        if self.is_valid_file(fileobj_or_path):
+            result = fileobj_or_path
+        elif not isinstance(fileobj_or_path, path_types):
+            raise TypeError('Not a valid file or path: %s' % fileobj_or_path)
+        elif not os.path.exists(fileobj_or_path):
+            raise ValueError('No such file: %s' % fileobj_or_path)
         else:
-            stdin = p.stdin
-        if passphrase:
-            _write_passphrase(stdin, passphrase, self.encoding)
-        writer = _threaded_copy_data(fileobj, stdin)
-        self._collect_output(p, result, writer, stdin)
+            result = open(fileobj_or_path, 'rb')
         return result
 
+    def _handle_io(self, args, fileobj_or_path, result, passphrase=None, binary=False):
+        "Handle a call to GPG - pass input data, collect output data"
+        # Handle a basic data call - pass data to GPG, handle the output
+        # including status information. Garbage In, Garbage Out :)
+        fileobj = self._get_fileobj(fileobj_or_path)
+        try:
+            p = self._open_subprocess(args, passphrase is not None)
+            if not binary:  # pragma: no cover
+                stdin = codecs.getwriter(self.encoding)(p.stdin)
+            else:
+                stdin = p.stdin
+            if passphrase:
+                _write_passphrase(stdin, passphrase, self.encoding)
+            writer = _threaded_copy_data(fileobj, stdin)
+            self._collect_output(p, result, writer, stdin)
+            return result
+        finally:
+            writer.join(0.01)
+            if fileobj is not fileobj_or_path:
+                fileobj.close()
     #
     # SIGNATURE METHODS
     #
     def sign(self, message, **kwargs):
         """sign message"""
         f = _make_binary_stream(message, self.encoding)
         result = self.sign_file(f, **kwargs)
@@ -1124,26 +1153,26 @@
         Confirm that the passphrase doesn't contain newline-type characters -
         it is passed in a pipe to gpg, and so not checking could lead to
         spoofing attacks by passing arbitrary text after passphrase and newline.
         """
         return ('\n' not in passphrase and '\r' not in passphrase and '\x00' not in passphrase)
 
     def sign_file(self,
-                  file,
+                  fileobj_or_path,
                   keyid=None,
                   passphrase=None,
                   clearsign=True,
                   detach=False,
                   binary=False,
                   output=None,
                   extra_args=None):
         """sign file"""
         if passphrase and not self.is_valid_passphrase(passphrase):
             raise ValueError('Invalid passphrase')
-        logger.debug('sign_file: %s', file)
+        logger.debug('sign_file: %s', fileobj_or_path)
         if binary:  # pragma: no cover
             args = ['-s']
         else:
             args = ['-sa']
         # You can't specify detach-sign and clearsign together: gpg ignores
         # the detach-sign in that case.
         if detach:
@@ -1156,23 +1185,29 @@
             self.set_output_without_confirmation(args, output)
 
         if extra_args:
             args.extend(extra_args)
         result = self.result_map['sign'](self)
         # We could use _handle_io here except for the fact that if the
         # passphrase is bad, gpg bails and you can't write the message.
+        fileobj = self._get_fileobj(fileobj_or_path)
         p = self._open_subprocess(args, passphrase is not None)
         try:
             stdin = p.stdin
             if passphrase:
                 _write_passphrase(stdin, passphrase, self.encoding)
-            writer = _threaded_copy_data(file, stdin)
+            writer = _threaded_copy_data(fileobj, stdin)
         except IOError:  # pragma: no cover
             logging.exception('error writing message')
             writer = None
+        finally:
+            if writer:
+                writer.join(0.01)
+            if fileobj is not fileobj_or_path:
+                fileobj.close()
         self._collect_output(p, result, writer, stdin)
         return result
 
     def verify(self, data, **kwargs):
         """Verify the signature on the contents of the string 'data'
 
         >>> GPGBINARY = os.environ.get('GPGBINARY', 'gpg')
@@ -1190,40 +1225,40 @@
 
         """
         f = _make_binary_stream(data, self.encoding)
         result = self.verify_file(f, **kwargs)
         f.close()
         return result
 
-    def verify_file(self, file, data_filename=None, close_file=True, extra_args=None):
+    def verify_file(self, fileobj_or_path, data_filename=None, close_file=True, extra_args=None):
         "Verify the signature on the contents of the file-like object 'file'"
-        logger.debug('verify_file: %r, %r', file, data_filename)
+        logger.debug('verify_file: %r, %r', fileobj_or_path, data_filename)
         result = self.result_map['verify'](self)
         args = ['--verify']
         if extra_args:
             args.extend(extra_args)
         if data_filename is None:
-            self._handle_io(args, file, result, binary=True)
+            self._handle_io(args, fileobj_or_path, result, binary=True)
         else:
             logger.debug('Handling detached verification')
             import tempfile
-            fd, fn = tempfile.mkstemp(prefix='pygpg')
-            s = file.read()
+            fd, fn = tempfile.mkstemp(prefix='pygpg-')
+            s = fileobj_or_path.read()
             if close_file:
-                file.close()
+                fileobj_or_path.close()
             logger.debug('Wrote to temp file: %r', s)
             os.write(fd, s)
             os.close(fd)
             args.append(no_quote(fn))
             args.append(no_quote(data_filename))
             try:
                 p = self._open_subprocess(args)
                 self._collect_output(p, result, stdin=p.stdin)
             finally:
-                os.unlink(fn)
+                os.remove(fn)
         return result
 
     def verify_data(self, sig_filename, data, extra_args=None):
         "Verify the signature in sig_filename against data in memory"
         logger.debug('verify_data: %r, %r ...', sig_filename, data[:16])
         result = self.result_map['verify'](self)
         args = ['--verify']
@@ -1249,14 +1284,21 @@
         if extra_args:
             args.extend(extra_args)
         self._handle_io(args, data, result, passphrase=passphrase, binary=True)
         logger.debug('import_keys result: %r', result.__dict__)
         data.close()
         return result
 
+    def import_keys_file(self, key_path, **kwargs):
+        """
+        Import the key data in key_path into our keyring.
+        """
+        with open(key_path, 'rb') as f:
+            return self.import_keys(f.read(), **kwargs)
+
     def recv_keys(self, keyserver, *keyids, **kwargs):
         """Import a key from a keyserver
 
         >>> import shutil
         >>> shutil.rmtree("keys", ignore_errors=True)
         >>> GPGBINARY = os.environ.get('GPGBINARY', 'gpg')
         >>> if not os.path.isdir('keys'): os.mkdir('keys')
@@ -1613,15 +1655,15 @@
         self._handle_io(args, f, result, passphrase=master_passphrase, binary=True)
         return result
 
     #
     # ENCRYPTION
     #
     def encrypt_file(self,
-                     file,
+                     fileobj_or_path,
                      recipients,
                      sign=None,
                      always_trust=False,
                      passphrase=None,
                      armor=True,
                      output=None,
                      symmetric=False,
@@ -1654,15 +1696,15 @@
         elif sign:  # pragma: no cover
             args.extend(['--sign', '--default-key', no_quote(sign)])
         if always_trust:  # pragma: no cover
             args.append('--always-trust')
         if extra_args:
             args.extend(extra_args)
         result = self.result_map['crypt'](self)
-        self._handle_io(args, file, result, passphrase=passphrase, binary=True)
+        self._handle_io(args, fileobj_or_path, result, passphrase=passphrase, binary=True)
         logger.debug('encrypt result[:100]: %r', result.data[:100])
         return result
 
     def encrypt(self, data, recipients, **kwargs):
         """Encrypt the message contained in the string 'data'
 
         >>> import shutil
@@ -1713,59 +1755,59 @@
     def decrypt(self, message, **kwargs):
         data = _make_binary_stream(message, self.encoding)
         result = self.decrypt_file(data, **kwargs)
         data.close()
         return result
 
     def decrypt_file(self,
-                     file,
+                     fileobj_or_path,
                      always_trust=False,
                      passphrase=None,
                      output=None,
                      extra_args=None):
         if passphrase and not self.is_valid_passphrase(passphrase):
             raise ValueError('Invalid passphrase')
         args = ['--decrypt']
         if output:  # write the output to a file with the specified name
             self.set_output_without_confirmation(args, output)
         if always_trust:  # pragma: no cover
             args.append('--always-trust')
         if extra_args:
             args.extend(extra_args)
         result = self.result_map['crypt'](self)
-        self._handle_io(args, file, result, passphrase, binary=True)
+        self._handle_io(args, fileobj_or_path, result, passphrase, binary=True)
         logger.debug('decrypt result[:100]: %r', result.data[:100])
         return result
 
     def get_recipients(self, message, **kwargs):
         data = _make_binary_stream(message, self.encoding)
         result = self.get_recipients_file(data, **kwargs)
         data.close()
         return result
 
-    def get_recipients_file(self, file, extra_args=None):
+    def get_recipients_file(self, fileobj_or_path, extra_args=None):
         args = ['--decrypt', '--list-only', '-v']
         if extra_args:
             args.extend(extra_args)
         result = self.result_map['crypt'](self)
-        self._handle_io(args, file, result, binary=True)
+        self._handle_io(args, fileobj_or_path, result, binary=True)
         ids = []
         for m in PUBLIC_KEY_RE.finditer(result.stderr):
             ids.append(m.group(1))
         return ids
 
     def trust_keys(self, fingerprints, trustlevel):
         levels = Verify.TRUST_LEVELS
         if trustlevel not in levels:
             poss = ', '.join(sorted(levels))
             raise ValueError('Invalid trust level: "%s" (must be one of %s)' % (trustlevel, poss))
         trustlevel = levels[trustlevel] + 2
         import tempfile
         try:
-            fd, fn = tempfile.mkstemp()
+            fd, fn = tempfile.mkstemp(prefix='pygpg-')
             lines = []
             if isinstance(fingerprints, string_types):
                 fingerprints = [fingerprints]
             for f in fingerprints:
                 lines.append('%s:%s:' % (f, trustlevel))
             # The trailing newline is required!
             s = os.linesep.join(lines) + os.linesep
```

### Comparing `python-gnupg-0.4.9/LICENSE.txt` & `python-gnupg-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-gnupg-0.4.9/messages.json` & `python-gnupg-0.5.0/messages.json`

 * *Files identical despite different names*

### Comparing `python-gnupg-0.4.9/PKG-INFO` & `python-gnupg-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gnupg
-Version: 0.4.9
+Version: 0.5.0
 Summary: A wrapper for the Gnu Privacy Guard (GPG or GnuPG)
 Home-page: https://github.com/vsajip/python-gnupg
 Author: Vinay Sajip
 Author-email: vinay_sajip@yahoo.co.uk
 Maintainer: Vinay Sajip
 Maintainer-email: vinay_sajip@yahoo.co.uk
 License: BSD
```

### Comparing `python-gnupg-0.4.9/test_pubring.gpg` & `python-gnupg-0.5.0/test_pubring.gpg`

 * *Files identical despite different names*

### Comparing `python-gnupg-0.4.9/README.rst` & `python-gnupg-0.5.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 |badge1| |badge2|
 
 .. |badge1| image:: https://img.shields.io/github/workflow/status/vsajip/python-gnupg/Tests
    :alt: GitHub test status
 
 .. |badge2| image:: https://img.shields.io/codecov/c/github/vsajip/python-gnupg
+   :target: https://app.codecov.io/gh/vsajip/python-gnupg
    :alt: GitHub coverage status
 
 
 What is it?
 ===========
 
 The GNU Privacy Guard (gpg, or gpg.exe on Windows) is a command-line program
@@ -67,14 +68,35 @@
 
 
 0.5.0 (future)
 --------------
 
 Released: Not yet.
 
+* Fixed #181: Added the ability to pass file paths to encrypt_file, decrypt_file,
+  sign_file, verify_file, get_recipients_file and added import_keys_file.
+
+* Fixed #183: Handle FAILURE and UNEXPECTED conditions correctly. Thanks to sebbASF for
+  the patch.
+
+* Fixed #185: Handle VALIDSIG arguments more robustly.
+
+* Fixed #188: Remove handling of DECRYPTION_FAILED from Verify code, as not required
+  there. Thanks to sebbASF for the patch.
+
+* Fixed #190: Handle KEY_CREATED more robustly.
+
+* Fixed #191: Handle NODATA messages during verification.
+
+* Fixed #196: Don't log chunk data by default, as it could contain sensitive
+  information (during decryption, for example).
+
+* Added the ability to pass an environment to the gpg executable. Thanks to Edvard
+  Rejthar for the patch.
+
 
 0.4.9
 -----
 
 Released: 2022-05-20
 
 * Fixed #161: Added a status attribute to the returned object from gen_key() which
```

