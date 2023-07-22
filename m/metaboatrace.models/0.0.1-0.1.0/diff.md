# Comparing `tmp/metaboatrace.models-0.0.1.tar.gz` & `tmp/metaboatrace_models-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaboatrace.models-0.0.1.tar", last modified: Sun Mar 26 05:30:08 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `metaboatrace.models-0.0.1.tar` & `metaboatrace_models-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,24 @@
-drwxr-xr-x   0 k0kishima   (501) staff       (20)        0 2023-03-26 05:30:08.684041 metaboatrace.models-0.0.1/
--rw-r--r--   0 k0kishima   (501) staff       (20)     1074 2023-03-26 05:12:47.000000 metaboatrace.models-0.0.1/LICENSE.txt
--rw-r--r--   0 k0kishima   (501) staff       (20)      730 2023-03-26 05:30:08.684099 metaboatrace.models-0.0.1/PKG-INFO
--rw-r--r--   0 k0kishima   (501) staff       (20)       96 2023-03-26 05:29:52.000000 metaboatrace.models-0.0.1/README.md
-drwxr-xr-x   0 k0kishima   (501) staff       (20)        0 2023-03-26 05:30:08.681946 metaboatrace.models-0.0.1/metaboatrace/
--rw-r--r--   0 k0kishima   (501) staff       (20)       65 2023-03-26 05:29:52.000000 metaboatrace.models-0.0.1/metaboatrace/__init__.py
-drwxr-xr-x   0 k0kishima   (501) staff       (20)        0 2023-03-26 05:30:08.683924 metaboatrace.models-0.0.1/metaboatrace/models/
--rw-r--r--   0 k0kishima   (501) staff       (20)      531 2023-03-26 05:29:52.000000 metaboatrace.models-0.0.1/metaboatrace/models/__init__.py
--rw-r--r--   0 k0kishima   (501) staff       (20)       79 2023-03-26 05:29:52.000000 metaboatrace.models-0.0.1/metaboatrace/models/betting_method.py
--rw-r--r--   0 k0kishima   (501) staff       (20)      342 2023-03-26 05:29:52.000000 metaboatrace.models-0.0.1/metaboatrace/models/branch.py
--rw-r--r--   0 k0kishima   (501) staff       (20)      350 2023-03-26 05:29:52.000000 metaboatrace.models-0.0.1/metaboatrace/models/disqualification.py
--rw-r--r--   0 k0kishima   (501) staff       (20)       88 2023-03-26 05:29:52.000000 metaboatrace.models-0.0.1/metaboatrace/models/gender.py
--rw-r--r--   0 k0kishima   (501) staff       (20)      249 2023-03-26 05:29:52.000000 metaboatrace.models-0.0.1/metaboatrace/models/motor_parts.py
--rw-r--r--   0 k0kishima   (501) staff       (20)      935 2023-03-26 05:29:52.000000 metaboatrace.models-0.0.1/metaboatrace/models/prefecture.py
--rw-r--r--   0 k0kishima   (501) staff       (20)      129 2023-03-26 05:29:52.000000 metaboatrace.models-0.0.1/metaboatrace/models/race_grade.py
--rw-r--r--   0 k0kishima   (501) staff       (20)      213 2023-03-26 05:29:52.000000 metaboatrace.models-0.0.1/metaboatrace/models/race_kind.py
--rw-r--r--   0 k0kishima   (501) staff       (20)      233 2023-03-26 05:29:52.000000 metaboatrace.models-0.0.1/metaboatrace/models/race_laps.py
--rw-r--r--   0 k0kishima   (501) staff       (20)      103 2023-03-26 05:29:52.000000 metaboatrace.models-0.0.1/metaboatrace/models/racer_rank.py
--rw-r--r--   0 k0kishima   (501) staff       (20)      458 2023-03-26 05:29:52.000000 metaboatrace.models-0.0.1/metaboatrace/models/stadium_tel_code.py
--rw-r--r--   0 k0kishima   (501) staff       (20)      165 2023-03-26 05:29:52.000000 metaboatrace.models-0.0.1/metaboatrace/models/weather.py
--rw-r--r--   0 k0kishima   (501) staff       (20)      178 2023-03-26 05:29:52.000000 metaboatrace.models-0.0.1/metaboatrace/models/winning_trick.py
-drwxr-xr-x   0 k0kishima   (501) staff       (20)        0 2023-03-26 05:30:08.682452 metaboatrace.models-0.0.1/metaboatrace.models.egg-info/
--rw-r--r--   0 k0kishima   (501) staff       (20)      730 2023-03-26 05:30:08.000000 metaboatrace.models-0.0.1/metaboatrace.models.egg-info/PKG-INFO
--rw-r--r--   0 k0kishima   (501) staff       (20)      718 2023-03-26 05:30:08.000000 metaboatrace.models-0.0.1/metaboatrace.models.egg-info/SOURCES.txt
--rw-r--r--   0 k0kishima   (501) staff       (20)        1 2023-03-26 05:30:08.000000 metaboatrace.models-0.0.1/metaboatrace.models.egg-info/dependency_links.txt
--rw-r--r--   0 k0kishima   (501) staff       (20)       13 2023-03-26 05:30:08.000000 metaboatrace.models-0.0.1/metaboatrace.models.egg-info/top_level.txt
--rw-r--r--   0 k0kishima   (501) staff       (20)      126 2023-03-26 05:30:08.684255 metaboatrace.models-0.0.1/setup.cfg
--rw-r--r--   0 k0kishima   (501) staff       (20)      863 2023-03-26 05:29:52.000000 metaboatrace.models-0.0.1/setup.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/requirements-dev.lock
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/requirements.lock
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/metaboatrace/models/__init__.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/metaboatrace/models/boat.py
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/metaboatrace/models/race.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/metaboatrace/models/racer.py
+-rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/metaboatrace/models/region.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/metaboatrace/models/stadium.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/tests/metaboatrace/models/test_boat.py
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/tests/metaboatrace/models/test_racer.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/tests/metaboatrace/models/test_region.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/tests/metaboatrace/models/test_stadium.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/tests/metaboatrace/models/race/test_bettings.py
+-rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/tests/metaboatrace/models/race/test_race_entries.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/tests/metaboatrace/models/race/test_races.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/README.md
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 metaboatrace_models-0.1.0/PKG-INFO
```

### Comparing `metaboatrace.models-0.0.1/LICENSE.txt` & `metaboatrace_models-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

