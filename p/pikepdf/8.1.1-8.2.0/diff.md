# Comparing `tmp/pikepdf-8.1.1.tar.gz` & `tmp/pikepdf-8.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikepdf-8.1.1.tar", last modified: Fri Jul 14 21:36:10 2023, max compression
+gzip compressed data, was "pikepdf-8.2.0.tar", last modified: Fri Jul 21 23:42:03 2023, max compression
```

## Comparing `pikepdf-8.1.1.tar` & `pikepdf-8.2.0.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 21:36:10.378609 pikepdf-8.1.1/
--rw-r--r--   0 runner    (1001) docker     (122)    16725 2023-07-14 21:33:09.000000 pikepdf-8.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-07-14 21:33:09.000000 pikepdf-8.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7294 2023-07-14 21:36:10.378609 pikepdf-8.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-07-14 21:33:09.000000 pikepdf-8.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     5889 2023-07-14 21:33:09.000000 pikepdf-8.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-14 21:36:10.378609 pikepdf-8.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3856 2023-07-14 21:33:09.000000 pikepdf-8.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 21:36:10.354609 pikepdf-8.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 21:36:10.358609 pikepdf-8.1.1/src/core/
--rw-r--r--   0 runner    (1001) docker     (122)     4478 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/annotation.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7216 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/embeddedfiles.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3953 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/jbig2-inl.h
--rw-r--r--   0 runner    (1001) docker     (122)     5806 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/job.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/logger.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/mmap_inputsource-inl.h
--rw-r--r--   0 runner    (1001) docker     (122)     3621 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/nametree.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3001 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/numbertree.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    42071 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/object.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/object_convert.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    10569 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/object_repr.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    14256 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/page.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    11199 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/parsers.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/parsers.h
--rw-r--r--   0 runner    (1001) docker     (122)     8201 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/pikepdf.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5700 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/pikepdf.h
--rw-r--r--   0 runner    (1001) docker     (122)     1274 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/pipeline.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/pipeline.h
--rw-r--r--   0 runner    (1001) docker     (122)    37394 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/qpdf.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5594 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/qpdf_inputsource-inl.h
--rw-r--r--   0 runner    (1001) docker     (122)    15512 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/qpdf_pagelist.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/qpdf_pagelist.h
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/rectangle.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/tokenfilter.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/core/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 21:36:10.362609 pikepdf-8.1.1/src/pikepdf/
--rw-r--r--   0 runner    (1001) docker     (122)     2972 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/pikepdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6161 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/pikepdf/_augments.py
--rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/pikepdf/_cpphelpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/pikepdf/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/pikepdf/_io.py
--rw-r--r--   0 runner    (1001) docker     (122)    57484 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/pikepdf/_methods.py
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/pikepdf/_qpdf.py
--rw-r--r--   0 runner    (1001) docker     (122)      879 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/pikepdf/_xml.py
--rw-r--r--   0 runner    (1001) docker     (122)     5952 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/pikepdf/codec.py
--rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/pikepdf/jbig2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 21:36:10.366609 pikepdf-8.1.1/src/pikepdf/models/
--rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/pikepdf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/pikepdf/models/_content_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     8204 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/pikepdf/models/_transcoding.py
--rw-r--r--   0 runner    (1001) docker     (122)     5499 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/pikepdf/models/encryption.py
--rw-r--r--   0 runner    (1001) docker     (122)    36349 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/pikepdf/models/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     5979 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/pikepdf/models/matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    32038 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/pikepdf/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)    15420 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/pikepdf/models/outlines.py
--rw-r--r--   0 runner    (1001) docker     (122)    10415 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/pikepdf/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/pikepdf/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      369 2023-07-14 21:33:09.000000 pikepdf-8.1.1/src/pikepdf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 21:36:10.362609 pikepdf-8.1.1/src/pikepdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7294 2023-07-14 21:36:10.000000 pikepdf-8.1.1/src/pikepdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3097 2023-07-14 21:36:10.000000 pikepdf-8.1.1/src/pikepdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 21:36:10.000000 pikepdf-8.1.1/src/pikepdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      661 2023-07-14 21:36:10.000000 pikepdf-8.1.1/src/pikepdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-14 21:36:10.000000 pikepdf-8.1.1/src/pikepdf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 21:36:10.370609 pikepdf-8.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1731 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 21:36:10.378609 pikepdf-8.1.1/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (122)     5661 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/1biticc.pdf
--rw-r--r--   0 runner    (1001) docker     (122)      420 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/Gray.icc
--rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/aquamarine-cie.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/aquamarine-cie.png
--rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/cmyk-jpeg.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    97969 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/congress-gray.pdf
--rw-r--r--   0 runner    (1001) docker     (122)   193947 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/congress.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2889 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/content-stream-errors.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    10876 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/form.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2713 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/formxobject.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/fourpages.pdf
--rw-r--r--   0 runner    (1001) docker     (122)   296661 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/graph-encrypted.pdf
--rw-r--r--   0 runner    (1001) docker     (122)   296322 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/graph.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/image-mono-inline.pdf
--rw-r--r--   0 runner    (1001) docker     (122)      965 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/invalid_creationdate.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    20306 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/jbig2.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    60332 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/jbig2global.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     6994 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/outlines.pdf
--rw-r--r--   0 runner    (1001) docker     (122)      931 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/pal-1bit-rgb.pdf
--rw-r--r--   0 runner    (1001) docker     (122)      931 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/pal-1bit-trivial.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/pal.pdf
--rwxr-xr-x   0 runner    (1001) docker     (122)   533953 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/pdfx.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    18471 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/pike-flate-jp2.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    18152 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/pike-jp2.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/pink-palette-icc.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/pink-palette-icc.png
--rw-r--r--   0 runner    (1001) docker     (122)     5432 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/rle.pdf
--rw-r--r--   0 runner    (1001) docker     (122)   115546 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/sandwich.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    10049 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/veraPDF test suite 6-2-10-t02-pass-a.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/resources/veraPDF test suite 6-2-3-3-t01-fail-c.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_annotation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4721 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_attachments.py
--rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_augments.py
--rw-r--r--   0 runner    (1001) docker     (122)     4516 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_codec.py
--rw-r--r--   0 runner    (1001) docker     (122)     1961 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_decimal.py
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (122)     5610 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     3404 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3135 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_foreign.py
--rw-r--r--   0 runner    (1001) docker     (122)     1988 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_formxobject.py
--rw-r--r--   0 runner    (1001) docker     (122)    36923 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_image_access.py
--rw-r--r--   0 runner    (1001) docker     (122)     9944 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_ipython.py
--rw-r--r--   0 runner    (1001) docker     (122)     2036 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    25215 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_nametree.py
--rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_numbertree.py
--rw-r--r--   0 runner    (1001) docker     (122)    22294 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_object.py
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_objectlist.py
--rw-r--r--   0 runner    (1001) docker     (122)    17256 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_outlines.py
--rw-r--r--   0 runner    (1001) docker     (122)     9131 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_page.py
--rw-r--r--   0 runner    (1001) docker     (122)    15569 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_pages.py
--rw-r--r--   0 runner    (1001) docker     (122)     9522 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (122)    13773 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_pdf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3956 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_pdfa.py
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_private_pdfs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_refcount.py
--rw-r--r--   0 runner    (1001) docker     (122)     3744 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (122)     4682 2023-07-14 21:33:09.000000 pikepdf-8.1.1/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:42:03.612349 pikepdf-8.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    16725 2023-07-21 23:39:17.000000 pikepdf-8.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-07-21 23:39:17.000000 pikepdf-8.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7294 2023-07-21 23:42:03.612349 pikepdf-8.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-07-21 23:39:17.000000 pikepdf-8.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     5924 2023-07-21 23:39:17.000000 pikepdf-8.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-21 23:42:03.612349 pikepdf-8.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3856 2023-07-21 23:39:17.000000 pikepdf-8.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:42:03.592349 pikepdf-8.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:42:03.596349 pikepdf-8.2.0/src/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     4478 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/annotation.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7216 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/embeddedfiles.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3953 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/jbig2-inl.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5806 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/job.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/logger.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/mmap_inputsource-inl.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3621 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/nametree.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3001 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/numbertree.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    42072 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/object.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/object_convert.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10569 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/object_repr.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    14256 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/page.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11199 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/parsers.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/parsers.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8253 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/pikepdf.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5700 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/pikepdf.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1274 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/pipeline.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/pipeline.h
+-rw-r--r--   0 runner    (1001) docker     (122)    37394 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/qpdf.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5594 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/qpdf_inputsource-inl.h
+-rw-r--r--   0 runner    (1001) docker     (122)    15512 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/qpdf_pagelist.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/qpdf_pagelist.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3901 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/rectangle.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/tokenfilter.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/core/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:42:03.600349 pikepdf-8.2.0/src/pikepdf/
+-rw-r--r--   0 runner    (1001) docker     (122)     3001 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/pikepdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6161 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/pikepdf/_augments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/pikepdf/_cpphelpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/pikepdf/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/pikepdf/_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57488 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/pikepdf/_methods.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/pikepdf/_qpdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      879 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/pikepdf/_xml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5952 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/pikepdf/codec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/pikepdf/jbig2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:42:03.600349 pikepdf-8.2.0/src/pikepdf/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/pikepdf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/pikepdf/models/_content_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8204 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/pikepdf/models/_transcoding.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5499 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/pikepdf/models/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36349 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/pikepdf/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5979 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/pikepdf/models/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32023 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/pikepdf/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15420 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/pikepdf/models/outlines.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10415 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/pikepdf/objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/pikepdf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      369 2023-07-21 23:39:17.000000 pikepdf-8.2.0/src/pikepdf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:42:03.600349 pikepdf-8.2.0/src/pikepdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7294 2023-07-21 23:42:03.000000 pikepdf-8.2.0/src/pikepdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3097 2023-07-21 23:42:03.000000 pikepdf-8.2.0/src/pikepdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 23:42:03.000000 pikepdf-8.2.0/src/pikepdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-07-21 23:42:03.000000 pikepdf-8.2.0/src/pikepdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-21 23:42:03.000000 pikepdf-8.2.0/src/pikepdf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:42:03.604349 pikepdf-8.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1731 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:42:03.612349 pikepdf-8.2.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)     5661 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/1biticc.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)      420 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/Gray.icc
+-rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/aquamarine-cie.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/aquamarine-cie.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/cmyk-jpeg.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    97969 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/congress-gray.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)   193947 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/congress.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     2889 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/content-stream-errors.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    10876 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/form.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     2713 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/formxobject.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/fourpages.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)   296661 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/graph-encrypted.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)   296322 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/graph.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/image-mono-inline.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)      965 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/invalid_creationdate.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    20306 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/jbig2.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    60332 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/jbig2global.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     6994 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/outlines.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)      931 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/pal-1bit-rgb.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)      931 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/pal-1bit-trivial.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/pal.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (122)   533953 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/pdfx.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    18471 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/pike-flate-jp2.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    18152 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/pike-jp2.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/pink-palette-icc.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/pink-palette-icc.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5432 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/rle.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)   115546 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/sandwich.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    10049 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/veraPDF test suite 6-2-10-t02-pass-a.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/resources/veraPDF test suite 6-2-3-3-t01-fail-c.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4721 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_augments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4453 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_codec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1961 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5610 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3404 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3135 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_foreign.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1988 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_formxobject.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36948 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_image_access.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9944 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_ipython.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2036 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25184 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_nametree.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_numbertree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22294 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_objectlist.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17177 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_outlines.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9131 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_page.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15569 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_pages.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9522 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13773 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3956 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_pdfa.py
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_private_pdfs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_refcount.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3744 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4682 2023-07-21 23:39:17.000000 pikepdf-8.2.0/tests/test_sanity.py
```

### Comparing `pikepdf-8.1.1/LICENSE.txt` & `pikepdf-8.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/PKG-INFO` & `pikepdf-8.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pikepdf
-Version: 8.1.1
+Version: 8.2.0
 Summary: Read and write PDFs with Python, powered by qpdf
 Author-email: "James R. Barlow" <james@purplerock.ca>
 License: MPL-2.0
 Project-URL: documentation, https://pikepdf.readthedocs.io/
 Project-URL: repository, https://github.com/pikepdf/pikepdf
 Project-URL: changelog, https://pikepdf.readthedocs.io/en/latest/releasenotes/index.html
 Keywords: PDF
```

### Comparing `pikepdf-8.1.1/README.md` & `pikepdf-8.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/pyproject.toml` & `pikepdf-8.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "wheel >= 0.37",
   "pybind11 >= 2.10.1",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pikepdf"
-version = "8.1.1"
+version = "8.2.0"
 description = "Read and write PDFs with Python, powered by qpdf"
 readme = "README.md"
 requires-python = ">= 3.8"
 keywords = ["PDF"]
 authors = [
   { name = "James R. Barlow", email= "james@purplerock.ca"}
 ]
@@ -30,15 +30,15 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Multimedia :: Graphics",
     "Topic :: Software Development :: Libraries",
 ]
 dependencies = [
     "Pillow>=9.0",
-    "Pillow<10; platform_python_implementation == 'PyPy'",
+    "Pillow<10; platform_python_implementation == 'PyPy' and python_version < '3.9'",
     "deprecation",
     "lxml>=4.8",
     "packaging",
 ]
 
 [project.urls]
 documentation = "https://pikepdf.readthedocs.io/"
@@ -119,15 +119,15 @@
 test-extras = "test"
 # cp36: ancient
 # pp37: discontinued by Pillow - https://pypi.org/project/Pillow/#files
 # pp310: no Pillow wheels yet
 # Reminder:
 #   build.yml sets CIBW_BUILD to select what can be built
 #   this file sets skip to deselect what cannot be built
-skip = ["cp36-*", "cp37-*", "pp37-*", "pp310-*", "*-win32", "*musllinux*", "pp*-manylinux*_aarch64"]
+skip = ["cp36-*", "cp37-*", "pp37-*", "*-win32", "*musllinux*", "pp*-manylinux*_aarch64", "pp310-win_amd64"]
 test-skip = "*_universal2:arm64"
 
 [tool.cibuildwheel.environment]
 QPDF_MIN_VERSION = "11.5.0"
 QPDF_VERSION = "11.5.0"
 QPDF_PATTERN = "https://github.com/qpdf/qpdf/releases/download/vVERSION/qpdf-VERSION.tar.gz"
```

### Comparing `pikepdf-8.1.1/setup.py` & `pikepdf-8.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/annotation.cpp` & `pikepdf-8.2.0/src/core/annotation.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/embeddedfiles.cpp` & `pikepdf-8.2.0/src/core/embeddedfiles.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/jbig2-inl.h` & `pikepdf-8.2.0/src/core/jbig2-inl.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/job.cpp` & `pikepdf-8.2.0/src/core/job.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/logger.cpp` & `pikepdf-8.2.0/src/core/logger.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/mmap_inputsource-inl.h` & `pikepdf-8.2.0/src/core/mmap_inputsource-inl.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/nametree.cpp` & `pikepdf-8.2.0/src/core/nametree.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/numbertree.cpp` & `pikepdf-8.2.0/src/core/numbertree.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/object.cpp` & `pikepdf-8.2.0/src/core/object.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -359,15 +359,15 @@
                 that is owned by *other*'s owner. If this object is a direct object
                 (no owner), then an indirect object is created that is owned by
                 *other*. An exception is thrown if *other* is a direct object.
 
                 This method may be convenient when a reference to the Pdf is not
                 available.
 
-                ..versionadded:: 2.14
+                .. versionadded:: 2.14
             )~~~")
         .def_property_readonly("is_indirect", &QPDFObjectHandle::isIndirect)
         .def("__repr__", &objecthandle_repr)
         .def("__hash__",
             [](QPDFObjectHandle &self) -> py::int_ {
                 // Objects which compare equal must have the same hash value
                 switch (self.getTypeCode()) {
@@ -851,16 +851,16 @@
         .def(
             "to_json",
             [](QPDFObjectHandle &h,
                 bool dereference   = false,
                 int schema_version = 2) -> py::bytes {
                 return h.getJSON(schema_version, dereference).unparse();
             },
-            py::arg("schema_version") = 2,
             py::arg("dereference")    = false,
+            py::arg("schema_version") = 2,
             R"~~~(
             Convert to a QPDF JSON representation of the object.
 
             See the QPDF manual for a description of its JSON representation.
             https://qpdf.readthedocs.io/en/stable/json.html#qpdf-json-format
 
             Not necessarily compatible with other PDF-JSON representations that
```

### Comparing `pikepdf-8.1.1/src/core/object_convert.cpp` & `pikepdf-8.2.0/src/core/object_convert.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/object_repr.cpp` & `pikepdf-8.2.0/src/core/object_repr.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/page.cpp` & `pikepdf-8.2.0/src/core/page.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/parsers.cpp` & `pikepdf-8.2.0/src/core/parsers.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/parsers.h` & `pikepdf-8.2.0/src/core/parsers.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/pikepdf.cpp` & `pikepdf-8.2.0/src/core/pikepdf.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -110,16 +110,16 @@
 }
 
 PYBIND11_MODULE(_core, m)
 {
     // py::options options;
     // options.disable_function_signatures();
 
-    m.doc() = "pikepdf provides a Pythonic interface for QPDF";
-
+    m.doc()            = "pikepdf provides a Pythonic interface for QPDF";
+    m.attr("__name__") = "pikepdf._core";
     m.def("qpdf_version", &QPDF::QPDFVersion, "Get libqpdf version");
 
     // -- Core objects --
     init_logger(m);
     init_qpdf(m);
     init_pagelist(m);
     init_object(m);
```

### Comparing `pikepdf-8.1.1/src/core/pikepdf.h` & `pikepdf-8.2.0/src/core/pikepdf.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/pipeline.cpp` & `pikepdf-8.2.0/src/core/pipeline.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/pipeline.h` & `pikepdf-8.2.0/src/core/pipeline.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/qpdf.cpp` & `pikepdf-8.2.0/src/core/qpdf.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/qpdf_inputsource-inl.h` & `pikepdf-8.2.0/src/core/qpdf_inputsource-inl.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/qpdf_pagelist.cpp` & `pikepdf-8.2.0/src/core/qpdf_pagelist.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/qpdf_pagelist.h` & `pikepdf-8.2.0/src/core/qpdf_pagelist.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/rectangle.cpp` & `pikepdf-8.2.0/src/core/rectangle.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             Rectangles in PDF are encoded as :class:`pikepdf.Array` with exactly
             four numeric elements, ordered as ``llx lly urx ury``.
             See |pdfrm| section 7.9.5.
 
             The rectangle may be considered degenerate if the lower left corner
             is not strictly less than the upper right corner.
 
-            .. versionadded: 2.14
+            .. versionadded:: 2.14
         )~~~")
         .def(py::init<double, double, double, double>())
         .def(py::init([](QPDFObjectHandle &h) {
             if (!h.isArray()) {
                 throw py::type_error(
                     "Object is not an array; cannot convert to Rectangle");
             }
```

### Comparing `pikepdf-8.1.1/src/core/tokenfilter.cpp` & `pikepdf-8.2.0/src/core/tokenfilter.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/utils.cpp` & `pikepdf-8.2.0/src/core/utils.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/core/utils.h` & `pikepdf-8.2.0/src/core/utils.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/pikepdf/__init__.py` & `pikepdf-8.2.0/src/pikepdf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """A library for manipulating PDFs."""
 
 # isort:skip_file
 
 from __future__ import annotations
 
-__version__ = "8.1.1"
+__version__ = "8.2.0"
 
 try:
     from . import _core
 except ImportError as _e:  # pragma: no cover
     _msg = "pikepdf's extension library failed to import"
     raise ImportError(_msg) from _e
 
@@ -67,18 +67,18 @@
 )
 
 # Importing these will monkeypatch classes defined in C++ and register a new
 # pdfdoc codec
 # While _cpphelpers is intended to be called from our C++ code only, explicitly
 # importing helps introspection tools like PyInstaller figure out that the module
 # is necessary.
-from . import _cpphelpers, _methods, codec  # noqa: unused-import
+from . import _cpphelpers, _methods, codec  # noqa: F401, F841
 from . import settings
 
-__libqpdf_version__ = _core.qpdf_version()
+__libqpdf_version__: str = _core.qpdf_version()
 
 # Provide pikepdf.{open, new} -> pikepdf.Pdf.{open, new}
 open = Pdf.open  # pylint: disable=redefined-builtin
 new = Pdf.new
 
 # Exclude .open, .new here from to make sure from pikepdf import * does not clobber
 # builtins.open()
@@ -129,9 +129,10 @@
     'PdfMatrix',
     'Permissions',
     'UnsupportedImageTypeError',
     'make_page_destination',
     'parse_content_stream',
     'unparse_content_stream',
     'settings',
+    '__libqpdf_version__',
     '__version__',
 ]
```

### Comparing `pikepdf-8.1.1/src/pikepdf/_augments.py` & `pikepdf-8.2.0/src/pikepdf/_augments.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/pikepdf/_cpphelpers.py` & `pikepdf-8.2.0/src/pikepdf/_cpphelpers.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/pikepdf/_io.py` & `pikepdf-8.2.0/src/pikepdf/_io.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/pikepdf/_methods.py` & `pikepdf-8.2.0/src/pikepdf/_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
         like ``pdf.docinfo[Name.Title] = "Title"`` will work when the dictionary
         does not exist at all.)
 
         You can delete the document information dictionary by deleting this property,
         ``del pdf.docinfo``. Note that accessing the property after deleting it
         will re-create with a new, empty dictionary.
 
-        .. versionchanged: 2.4
+        .. versionchanged:: 2.4
             Added support for ``del pdf.docinfo``.
         """
         if Name.Info not in self.trailer:
             self.trailer.Info = self.make_indirect(Dictionary())
         return self.trailer.Info
 
     @docinfo.setter
@@ -675,15 +675,15 @@
 
         .. versionchanged:: 3.0
             Keyword arguments now mandatory for everything except the first
             argument.
 
         .. versionchanged:: 8.1
             If filename_or_stream is a filename and that file exists, the new file
-            written to a temporary file in the same directory and then moved into
+            is written to a temporary file in the same directory and then moved into
             place. This prevents the existing destination file from being corrupted
             if the process is interrupted during writing; previously, corrupting the
             destination file was possible. If no file exists at the destination, output
             is written directly to the destination, but the destination will be deleted
             if errors occur during writing. Prior to 8.1, the file was always written
             directly to the destination, which could result in a corrupt destination
             file if the process was interrupted during writing.
```

### Comparing `pikepdf-8.1.1/src/pikepdf/_qpdf.py` & `pikepdf-8.2.0/src/pikepdf/_qpdf.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/pikepdf/_xml.py` & `pikepdf-8.2.0/src/pikepdf/_xml.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/pikepdf/codec.py` & `pikepdf-8.2.0/src/pikepdf/codec.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/pikepdf/jbig2.py` & `pikepdf-8.2.0/src/pikepdf/jbig2.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/pikepdf/models/__init__.py` & `pikepdf-8.2.0/src/pikepdf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/pikepdf/models/_content_stream.py` & `pikepdf-8.2.0/src/pikepdf/models/_content_stream.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/pikepdf/models/_transcoding.py` & `pikepdf-8.2.0/src/pikepdf/models/_transcoding.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/pikepdf/models/encryption.py` & `pikepdf-8.2.0/src/pikepdf/models/encryption.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/pikepdf/models/image.py` & `pikepdf-8.2.0/src/pikepdf/models/image.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/pikepdf/models/matrix.py` & `pikepdf-8.2.0/src/pikepdf/models/matrix.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/pikepdf/models/metadata.py` & `pikepdf-8.2.0/src/pikepdf/models/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from __future__ import annotations
 
 import logging
 import re
 import sys
 from abc import ABC, abstractmethod
-from datetime import datetime
+from datetime import datetime, timezone
 from functools import wraps
 from io import BytesIO
 from typing import TYPE_CHECKING, Any, Callable, NamedTuple, Set
 from warnings import warn
 
 from lxml import etree
 from lxml.etree import QName, XMLSyntaxError
@@ -564,15 +564,15 @@
 
         Depending how we are initialized, leave our metadata mark and producer.
         """
         if self.mark:
             # We were asked to mark the file as being edited by pikepdf
             self._setitem(
                 QName(XMP_NS_XMP, 'MetadataDate'),
-                datetime.now(datetime.utcnow().astimezone().tzinfo).isoformat(),
+                datetime.now(timezone.utc).isoformat(),
                 applying_mark=True,
             )
             self._setitem(
                 QName(XMP_NS_PDF, 'Producer'),
                 'pikepdf ' + pikepdf_version,
                 applying_mark=True,
             )
```

### Comparing `pikepdf-8.1.1/src/pikepdf/models/outlines.py` & `pikepdf-8.2.0/src/pikepdf/models/outlines.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/pikepdf/objects.py` & `pikepdf-8.2.0/src/pikepdf/objects.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/pikepdf.egg-info/PKG-INFO` & `pikepdf-8.2.0/src/pikepdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pikepdf
-Version: 8.1.1
+Version: 8.2.0
 Summary: Read and write PDFs with Python, powered by qpdf
 Author-email: "James R. Barlow" <james@purplerock.ca>
 License: MPL-2.0
 Project-URL: documentation, https://pikepdf.readthedocs.io/
 Project-URL: repository, https://github.com/pikepdf/pikepdf
 Project-URL: changelog, https://pikepdf.readthedocs.io/en/latest/releasenotes/index.html
 Keywords: PDF
```

### Comparing `pikepdf-8.1.1/src/pikepdf.egg-info/SOURCES.txt` & `pikepdf-8.2.0/src/pikepdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/src/pikepdf.egg-info/requires.txt` & `pikepdf-8.2.0/src/pikepdf.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Pillow>=9.0
 deprecation
 lxml>=4.8
 packaging
 
-[:platform_python_implementation == "PyPy"]
+[:platform_python_implementation == "PyPy" and python_version < "3.9"]
 Pillow<10
 
 [dev]
 pre-commit
 typer[all]
 
 [docs]
```

### Comparing `pikepdf-8.1.1/tests/conftest.py` & `pikepdf-8.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/1biticc.pdf` & `pikepdf-8.2.0/tests/resources/1biticc.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/aquamarine-cie.pdf` & `pikepdf-8.2.0/tests/resources/aquamarine-cie.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/aquamarine-cie.png` & `pikepdf-8.2.0/tests/resources/aquamarine-cie.png`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/cmyk-jpeg.pdf` & `pikepdf-8.2.0/tests/resources/cmyk-jpeg.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/congress-gray.pdf` & `pikepdf-8.2.0/tests/resources/congress-gray.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/congress.pdf` & `pikepdf-8.2.0/tests/resources/congress.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/content-stream-errors.pdf` & `pikepdf-8.2.0/tests/resources/content-stream-errors.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/form.pdf` & `pikepdf-8.2.0/tests/resources/form.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/formxobject.pdf` & `pikepdf-8.2.0/tests/resources/formxobject.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/fourpages.pdf` & `pikepdf-8.2.0/tests/resources/fourpages.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/graph-encrypted.pdf` & `pikepdf-8.2.0/tests/resources/graph-encrypted.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/graph.pdf` & `pikepdf-8.2.0/tests/resources/graph.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/image-mono-inline.pdf` & `pikepdf-8.2.0/tests/resources/image-mono-inline.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/invalid_creationdate.pdf` & `pikepdf-8.2.0/tests/resources/invalid_creationdate.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/jbig2.pdf` & `pikepdf-8.2.0/tests/resources/jbig2.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/jbig2global.pdf` & `pikepdf-8.2.0/tests/resources/jbig2global.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/outlines.pdf` & `pikepdf-8.2.0/tests/resources/outlines.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/pal-1bit-rgb.pdf` & `pikepdf-8.2.0/tests/resources/pal-1bit-rgb.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/pal-1bit-trivial.pdf` & `pikepdf-8.2.0/tests/resources/pal-1bit-trivial.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/pal.pdf` & `pikepdf-8.2.0/tests/resources/pal.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/pdfx.pdf` & `pikepdf-8.2.0/tests/resources/pdfx.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/pike-flate-jp2.pdf` & `pikepdf-8.2.0/tests/resources/pike-flate-jp2.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/pike-jp2.pdf` & `pikepdf-8.2.0/tests/resources/pike-jp2.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/pink-palette-icc.pdf` & `pikepdf-8.2.0/tests/resources/pink-palette-icc.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/pink-palette-icc.png` & `pikepdf-8.2.0/tests/resources/pink-palette-icc.png`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/rle.pdf` & `pikepdf-8.2.0/tests/resources/rle.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/sandwich.pdf` & `pikepdf-8.2.0/tests/resources/sandwich.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/veraPDF test suite 6-2-10-t02-pass-a.pdf` & `pikepdf-8.2.0/tests/resources/veraPDF test suite 6-2-10-t02-pass-a.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/resources/veraPDF test suite 6-2-3-3-t01-fail-c.pdf` & `pikepdf-8.2.0/tests/resources/veraPDF test suite 6-2-3-3-t01-fail-c.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_annotation.py` & `pikepdf-8.2.0/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_attachments.py` & `pikepdf-8.2.0/tests/test_attachments.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_augments.py` & `pikepdf-8.2.0/tests/test_augments.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_codec.py` & `pikepdf-8.2.0/tests/test_codec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # SPDX-FileCopyrightText: 2022 James R. Barlow
 # SPDX-License-Identifier: CC0-1.0
 
 from __future__ import annotations
 
-from datetime import timedelta
 from io import BytesIO
 from pathlib import Path
 
 import pytest
 from hypothesis import example, given, settings
 from hypothesis.strategies import binary, characters, text
 
@@ -93,28 +92,28 @@
 )
 
 
 @given(pdfdoc_text)
 @example('\r\n')
 @example('\r')
 @example('\n')
-@settings(deadline=timedelta(seconds=4))  # CI workers can be flakey
+@settings(deadline=4000)  # CI workers can be flakey
 def test_open_encoding_pdfdoc_write(tmp_path_factory, s):
     folder = tmp_path_factory.mktemp('pdfdoc')
     txt = folder / 'pdfdoc.txt'
     with open(txt, 'w', encoding='pdfdoc', newline='') as f:
         try:
             f.write(s)
         except UnicodeEncodeError:
             return
     assert txt.read_bytes() == s.encode('pdfdoc')
 
 
 @given(pdfdoc_text)
-@settings(deadline=timedelta(seconds=4))  # CI workers can be flakey
+@settings(deadline=4000)  # CI workers can be flakey
 @example('\r\n')
 @example('\r')
 @example('\n')
 def test_open_encoding_pdfdoc_read(tmp_path_factory, s: str):
     folder = tmp_path_factory.mktemp('pdfdoc')
     txt: Path = folder / 'pdfdoc.txt'
     with open(txt, 'w', encoding='pdfdoc', newline='') as f:
```

### Comparing `pikepdf-8.1.1/tests/test_decimal.py` & `pikepdf-8.2.0/tests/test_decimal.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_dictionary.py` & `pikepdf-8.2.0/tests/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_encrypt.py` & `pikepdf-8.2.0/tests/test_encrypt.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_errors.py` & `pikepdf-8.2.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_filters.py` & `pikepdf-8.2.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_foreign.py` & `pikepdf-8.2.0/tests/test_foreign.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_formxobject.py` & `pikepdf-8.2.0/tests/test_formxobject.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_image_access.py` & `pikepdf-8.2.0/tests/test_image_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -546,14 +546,15 @@
     outpng = tmpdir / 'pdfimage-000.png'
     assert outpng.exists()
     with Image.open(outpng) as im:
         yield im
 
 
 @given(spec=valid_random_palette_image_spec())
+@settings(deadline=2000)
 def test_image_palette2(spec, tmp_path_factory):
     pdf = pdf_from_palette_image_spec(spec)
     pim = PdfImage(pdf.pages[0].Resources.XObject['/Im0'])
 
     im1 = pim.as_pil_image()
 
     with first_image_from_pdfimages(
```

### Comparing `pikepdf-8.1.1/tests/test_io.py` & `pikepdf-8.2.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_ipython.py` & `pikepdf-8.2.0/tests/test_ipython.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_job.py` & `pikepdf-8.2.0/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_matrix.py` & `pikepdf-8.2.0/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_metadata.py` & `pikepdf-8.2.0/tests/test_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -550,15 +550,15 @@
     with pikepdf.open(outpdf) as pdf:
         assert pdf.pdf_version == '1.7' and pdf.extension_level == 42
 
     with pytest.raises(TypeError):
         trivial.save(outpdf, force_version=('1.7', 'invalid extension level'))
 
 
-@settings(deadline=500.0)
+@settings(deadline=500)
 @given(
     st.dictionaries(
         keys=st.sampled_from(
             [
                 "/Author",
                 "/Subject",
                 "/Title",
@@ -676,25 +676,22 @@
     ):
         xmp['dc:title'] = {'Title 1', 'Title 2'}
     with trivial.open_metadata(update_docinfo=False) as xmp:
         assert b'Title 1; Title 2</rdf:li></rdf:Alt></dc:title>' in xmp._get_xml_bytes()
 
 
 def test_xmp_metadatadate_timezone(sandwich, outpdf):
-    with sandwich.open_metadata():
+    with sandwich.open_metadata(set_pikepdf_as_editor=True):
         pass
     sandwich.save(outpdf)
-
-    machine_tz = datetime.utcnow().astimezone().tzinfo
-
     with Pdf.open(outpdf) as pdf:
         with pdf.open_metadata() as m:
             dt = datetime.fromisoformat(m['xmp:MetadataDate'])
             assert dt.tzinfo is not None
-            assert dt.tzinfo == machine_tz
+            assert dt.tzinfo == timezone.utc
 
 
 def test_modify_not_opened(graph):
     m = graph.open_metadata()
     with pytest.raises(RuntimeError, match='not opened for editing'):
         m['pdf:Producer'] = 'pytest'
```

### Comparing `pikepdf-8.1.1/tests/test_nametree.py` & `pikepdf-8.2.0/tests/test_nametree.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_numbertree.py` & `pikepdf-8.2.0/tests/test_numbertree.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_object.py` & `pikepdf-8.2.0/tests/test_object.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_objectlist.py` & `pikepdf-8.2.0/tests/test_objectlist.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_outlines.py` & `pikepdf-8.2.0/tests/test_outlines.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # SPDX-FileCopyrightText: 2022 James R. Barlow
 # SPDX-License-Identifier: CC0-1.0
 
 from __future__ import annotations
 
-from datetime import timedelta
 from itertools import repeat
 
 import pytest
 from hypothesis import example, given, settings
 from hypothesis import strategies as st
 
 from pikepdf import (
@@ -388,15 +387,15 @@
         first = outline.root[0]
         first.action = Dictionary(D=first.destination, S=Name.GoTo)
         first.destination = None
     assert first_obj.A.D == [first_page.obj, Name.Fit]
     assert '/Dest' not in first_obj
 
 
-@settings(deadline=timedelta(milliseconds=750))
+@settings(deadline=750)
 @given(
     page_num=st.integers(0, 1),
     page_loc=st.sampled_from(list(PageLocation) + ['invalid']),  # type: ignore
     kwargs=st.dictionaries(
         st.sampled_from(list(sorted(ALL_PAGE_LOCATION_KWARGS))), st.integers(0, 10000)
     ),
 )
@@ -436,15 +435,15 @@
         else:
             args = ()
         expected_dest = [page_ref.obj, Name(f'/{loc_str}')]
         expected_dest.extend(kwargs.get(k, 0) for k in args)
         assert dest == expected_dest
 
 
-@settings(deadline=timedelta(milliseconds=750))
+@settings(deadline=750)
 @given(
     title=st.text(),
     page_num=st.integers(0, 1),
     page_loc=st.sampled_from(PageLocation),
 )
 @example(
     title='',
```

### Comparing `pikepdf-8.1.1/tests/test_page.py` & `pikepdf-8.2.0/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_pages.py` & `pikepdf-8.2.0/tests/test_pages.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_parsers.py` & `pikepdf-8.2.0/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_pdf.py` & `pikepdf-8.2.0/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_pdfa.py` & `pikepdf-8.2.0/tests/test_pdfa.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_private_pdfs.py` & `pikepdf-8.2.0/tests/test_private_pdfs.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_rectangle.py` & `pikepdf-8.2.0/tests/test_rectangle.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_refcount.py` & `pikepdf-8.2.0/tests/test_refcount.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_repr.py` & `pikepdf-8.2.0/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.1.1/tests/test_sanity.py` & `pikepdf-8.2.0/tests/test_sanity.py`

 * *Files identical despite different names*

