# Comparing `tmp/big-0.9.1.tar.gz` & `tmp/big-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "big-0.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "big-0.9.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `big-0.9.1.tar` & `big-0.9.2.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0       50 2022-12-06 08:53:33.203521 big-0.9.1/.gitignore
--rw-r--r--   0        0        0     1084 2023-06-16 06:39:59.562319 big-0.9.1/LICENSE
--rw-r--r--   0        0        0   150629 2023-06-28 11:25:56.173595 big-0.9.1/README.md
--rw-r--r--   0        0        0     1242 2023-06-28 11:25:56.173595 big-0.9.1/big/__init__.py
--rw-r--r--   0        0        0     2007 2023-06-28 11:25:56.173595 big-0.9.1/big/all.py
--rw-r--r--   0        0        0     7825 2023-06-18 07:30:42.346660 big-0.9.1/big/boundinnerclass.py
--rw-r--r--   0        0        0     3274 2023-06-18 07:30:42.346660 big-0.9.1/big/builtin.py
--rw-r--r--   0        0        0    11015 2023-06-18 07:30:42.346660 big-0.9.1/big/file.py
--rw-r--r--   0        0        0    25350 2023-06-18 07:30:42.346660 big-0.9.1/big/graph.py
--rw-r--r--   0        0        0     5347 2023-06-18 07:30:42.346660 big-0.9.1/big/heap.py
--rw-r--r--   0        0        0     2499 2023-06-28 10:08:06.167307 big-0.9.1/big/itertools.py
--rw-r--r--   0        0        0     6358 2023-06-28 11:25:56.173595 big-0.9.1/big/log.py
--rw-r--r--   0        0        0    12574 2023-06-18 07:30:42.346660 big-0.9.1/big/scheduler.py
--rw-r--r--   0        0        0   108729 2023-06-18 07:30:42.346660 big-0.9.1/big/text.py
--rw-r--r--   0        0        0     7163 2023-06-18 07:30:42.346660 big-0.9.1/big/time.py
--rw-r--r--   0        0        0      613 2023-06-16 06:39:59.562319 big-0.9.1/pyproject.toml
--rw-r--r--   0        0        0       16 2022-12-06 08:53:33.203521 big-0.9.1/requirements.txt
--rw-r--r--   0        0        0   174313 2022-05-27 04:32:07.000000 big-0.9.1/resources/experiments/alice.in.wonderland.txt
--rw-r--r--   0        0        0     6060 2023-06-16 06:39:59.562319 big-0.9.1/resources/experiments/time_multisplit.py
--rw-r--r--   0        0        0  1391641 2022-06-02 13:08:28.000000 big-0.9.1/resources/images/big.header.png
--rw-r--r--   0        0        0     3531 2023-06-24 07:13:15.776575 big-0.9.1/tests/bigtestlib.py
--rw-r--r--   0        0        0       50 2023-06-16 06:39:59.562319 big-0.9.1/tests/grepfile
--rw-r--r--   0        0        0     1468 2023-06-28 11:25:56.173595 big-0.9.1/tests/test_all.py
--rw-r--r--   0        0        0     8721 2023-06-16 06:39:59.562319 big-0.9.1/tests/test_boundinnerclass.py
--rw-r--r--   0        0        0     6517 2023-06-28 11:25:56.173595 big-0.9.1/tests/test_builtin.py
--rw-r--r--   0        0        0     8363 2023-06-16 06:39:59.566320 big-0.9.1/tests/test_file.py
--rw-r--r--   0        0        0    12333 2023-06-16 06:39:59.566320 big-0.9.1/tests/test_graph.py
--rw-r--r--   0        0        0     5007 2023-06-16 06:39:59.566320 big-0.9.1/tests/test_heap.py
--rw-r--r--   0        0        0     3403 2023-06-16 06:39:59.566320 big-0.9.1/tests/test_itertools.py
--rw-r--r--   0        0        0     4259 2023-06-28 11:25:56.173595 big-0.9.1/tests/test_log.py
--rw-r--r--   0        0        0    11473 2023-06-16 06:39:59.566320 big-0.9.1/tests/test_scheduler.py
--rw-r--r--   0        0        0   140256 2023-06-16 06:39:59.566320 big-0.9.1/tests/test_text.py
--rw-r--r--   0        0        0     6101 2023-06-16 06:39:59.566320 big-0.9.1/tests/test_time.py
--rw-r--r--   0        0        0   151234 1970-01-01 00:00:00.000000 big-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1191 2023-07-21 22:29:18.288177 big-0.9.2/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     1373 2023-07-21 22:29:18.288177 big-0.9.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0       50 2022-12-06 08:53:33.203521 big-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1084 2023-06-16 06:39:59.562319 big-0.9.2/LICENSE
+-rw-r--r--   0        0        0   152672 2023-07-21 22:35:32.367627 big-0.9.2/README.md
+-rw-r--r--   0        0        0     1242 2023-07-21 22:29:18.292177 big-0.9.2/big/__init__.py
+-rw-r--r--   0        0        0     2007 2023-06-28 11:25:56.173595 big-0.9.2/big/all.py
+-rw-r--r--   0        0        0     7825 2023-06-18 07:30:42.346660 big-0.9.2/big/boundinnerclass.py
+-rw-r--r--   0        0        0     3274 2023-06-18 07:30:42.346660 big-0.9.2/big/builtin.py
+-rw-r--r--   0        0        0    11015 2023-06-18 07:30:42.346660 big-0.9.2/big/file.py
+-rw-r--r--   0        0        0    25350 2023-06-18 07:30:42.346660 big-0.9.2/big/graph.py
+-rw-r--r--   0        0        0     5347 2023-06-18 07:30:42.346660 big-0.9.2/big/heap.py
+-rw-r--r--   0        0        0     2499 2023-06-28 10:08:06.167307 big-0.9.2/big/itertools.py
+-rw-r--r--   0        0        0     6806 2023-07-21 14:24:39.316289 big-0.9.2/big/log.py
+-rw-r--r--   0        0        0    12675 2023-06-28 11:52:01.906550 big-0.9.2/big/scheduler.py
+-rw-r--r--   0        0        0   108729 2023-06-18 07:30:42.346660 big-0.9.2/big/text.py
+-rw-r--r--   0        0        0     7163 2023-06-18 07:30:42.346660 big-0.9.2/big/time.py
+-rw-r--r--   0        0        0      936 2023-07-21 22:33:08.810303 big-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0       16 2022-12-06 08:53:33.203521 big-0.9.2/requirements.txt
+-rw-r--r--   0        0        0   174313 2022-05-27 04:32:07.000000 big-0.9.2/resources/experiments/alice.in.wonderland.txt
+-rw-r--r--   0        0        0     6060 2023-06-16 06:39:59.562319 big-0.9.2/resources/experiments/time_multisplit.py
+-rw-r--r--   0        0        0  1391641 2022-06-02 13:08:28.000000 big-0.9.2/resources/images/big.header.png
+-rw-r--r--   0        0        0     3531 2023-06-24 07:13:15.776575 big-0.9.2/tests/bigtestlib.py
+-rw-r--r--   0        0        0       50 2023-06-16 06:39:59.562319 big-0.9.2/tests/grepfile
+-rw-r--r--   0        0        0     1468 2023-06-28 11:25:56.173595 big-0.9.2/tests/test_all.py
+-rw-r--r--   0        0        0     8721 2023-06-16 06:39:59.562319 big-0.9.2/tests/test_boundinnerclass.py
+-rw-r--r--   0        0        0     6517 2023-06-28 11:25:56.173595 big-0.9.2/tests/test_builtin.py
+-rw-r--r--   0        0        0     8363 2023-06-16 06:39:59.566320 big-0.9.2/tests/test_file.py
+-rw-r--r--   0        0        0    12333 2023-06-16 06:39:59.566320 big-0.9.2/tests/test_graph.py
+-rw-r--r--   0        0        0     5007 2023-06-16 06:39:59.566320 big-0.9.2/tests/test_heap.py
+-rw-r--r--   0        0        0     3403 2023-06-16 06:39:59.566320 big-0.9.2/tests/test_itertools.py
+-rw-r--r--   0        0        0     4016 2023-07-21 14:51:27.631753 big-0.9.2/tests/test_log.py
+-rw-r--r--   0        0        0    11473 2023-06-16 06:39:59.566320 big-0.9.2/tests/test_scheduler.py
+-rw-r--r--   0        0        0   140256 2023-06-16 06:39:59.566320 big-0.9.2/tests/test_text.py
+-rw-r--r--   0        0        0     6101 2023-06-16 06:39:59.566320 big-0.9.2/tests/test_time.py
+-rw-r--r--   0        0        0   153687 1970-01-01 00:00:00.000000 big-0.9.2/PKG-INFO
```

### Comparing `big-0.9.1/LICENSE` & `big-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `big-0.9.1/README.md` & `big-0.9.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 ![# big](https://raw.githubusercontent.com/larryhastings/big/master/resources/images/big.header.png)
 
 ##### Copyright 2022-2023 by Larry Hastings
 
+[![# test badge](https://img.shields.io/github/actions/workflow/status/larryhastings/big/test.yml?branch=master&label=test)](https://github.com/larryhastings/big/actions/workflows/test.yml)
+[![# coverage badge](https://img.shields.io/github/actions/workflow/status/larryhastings/big/coverage.yml?branch=master&label=coverage)](https://github.com/larryhastings/big/actions/workflows/coverage.yml)
+[![# python versions badge](https://img.shields.io/pypi/pyversions/big.svg?logo=python&logoColor=FBE072)](https://pypi.org/project/big/)
+
+
 **big** is a Python package, a grab-bag of useful technology
 I always want to have handy.
 
 Finally!  For years, I've copied-and-pasted all my little
 helper functions between projects--we've all done it.
 But now I've finally taken the time to consolidate all those
 useful little functions into one big package, so they're always
@@ -57,17 +62,18 @@
 
 ```Python
 from big.all import *
 ```
 
 but that's up to you.
 
-**big** is licensed using the [MIT license.](https://opensource.org/licenses/MIT)
-You're free to use it and even ship it in your own programs, as long as you leave my copyright
-notice on the source code.
+**big** is licensed using the
+[MIT license.](https://opensource.org/licenses/MIT)
+You're free to use it and even ship it in your own programs,
+as long as you leave my copyright notice on the source code.
 
 # Index
 
 [`ascii_newlines`](#newlines)
 
 [`ascii_newlines_without_dos`](#newlines)
 
@@ -167,21 +173,21 @@
 
 [`lines_strip(li)`](#lines_stripli)
 
 [`lines_strip_comments(li, comment_separators, *, quotes=('"', "'"), backslash='\\', rstrip=True, triple_quotes=True)`](#lines_strip_commentsli-comment_separators--quotes--backslash-rstriptrue-triple_quotestrue)
 
 [`lines_strip_indent(li)`](#lines_strip_indentli)
 
-[`Log`](#log)
+[`Log`](#log-clocknone)
 
 [`Log.enter(subsystem)`](#logentersubsystem)
 
 [`Log.exit()`](#logexit)
 
-[`Log.print(*, print=None, title="[event log]", headings=True, indent=2, seconds_width=2, fractional_width=9)`](#logprint--printnone-titleeventlog-headingstrue-indent2-seconds_width2-fractional_width9)
+[`Log.print(*, print=None, title="[event log]", headings=True, indent=2, seconds_width=2, fractional_width=9)`](#logprint-printnone-titleevent-log-headingstrue-indent2-seconds_width2-fractional_width9)
 
 [`Log.reset()`](#logreset)
 
 [`merge_columns(*columns, column_separator=" ", overflow_response=OverflowResponse.RAISE, overflow_before=0, overflow_after=0)`](#merge_columnscolumns-column_separator--overflow_responseoverflowresponseraise-overflow_before0-overflow_after0)
 
 [`multipartition(s, separators, count=1, *, reverse=False, separate=True)`](#multipartitions-separators-count1--reverseFalse-separateTrue)
 
@@ -297,15 +303,15 @@
 
 [`whitespace`](#whitespace)
 
 [`whitespace_without_dos`](#whitespace)
 
 [`wrap_words(words, margin=79, *, two_spaces=True)`](#wrap_wordswords-margin79--two_spacestrue)
 
-[**The `multi-` family of functions**](#The-multi--family-of-functions)
+[**The `multi-` family of string functions**](#The-multi--family-of-string-functions)
 
 [**`lines` and lines modifier functions**](#lines-and-lines-modifier-functions)
 
 [**Word wrapping and formatting**](#word-wrapping-and-formatting)
 
 [**Bound inner classes**](#bound-inner-classes)
 
@@ -823,21 +829,24 @@
 
 A simple and lightweight logging class, useful for performance analysis.
 Not intended as a full-fledged logging facility like Python's
 [`logging`](https://docs.python.org/3/library/logging.html) module.
 
 #### `default_clock()`
 
-> The default clock function used by the `Log` class.
+> The default clock function used by the [`Log`](#log-clocknone) class.
 > This function returns elapsed time in nanoseconds,
 > expressed as an integer.
 >
 > In Python 3.7+,
-> this is `time.monotonic_ns`; in Python 3.6 this is
-> a custom function that calls `time.perf_counter`,
+> this is
+> [`time.monotonic_ns`](https://docs.python.org/3/library/time.html#time.monotonic_ns);
+> in Python 3.6 this is
+> a custom function that calls
+> [`time.perf_counter`](https://docs.python.org/3/library/time.html#time.perf_counter),
 > then converts that time to requisite format.
 
 #### `Log(*, clock=None)`
 
 > A simple and lightweight logging class, useful for performance analysis.
 > Not intended as a full-fledged logging facility like Python's
 > [`logging`](https://docs.python.org/3/library/logging.html) module.
@@ -869,14 +878,28 @@
 >
 >     log.print()
 >
 > You can also iterate over the log events using `iter(log)`.
 > This yields 4-tuples:
 >
 >     (start_time, elapsed_time, event, depth)
+>
+> `start_time` and `elapsed_time` are times, expressed as
+> an integer number of nanoseconds.  The first event
+> is at `start_time` 0, and all subsequent start times are
+> relative to that time.
+>
+> `event` is the event string you
+> passed in to `log()` (or `"<subsystem> start"` or
+> `"<subsystem> end"`).
+>
+> `depth` is an integer indicating
+> how many subsystems the event is nested in; larger
+> numbers indicate deeper nesting.
+
 
 #### `Log.enter(subsystem)`
 
 > Notifies the log that you've entered a subsystem.
 > The `subsystem` parameter should be a string describing the subsystem.
 >
 > This is really just a presentation
@@ -944,16 +967,16 @@
 > Python API design--its design predates many common modern
 > Python conventions.  Its events are callbacks, which it
 > calls directly.  `Scheduler` fixes this: its events are
 > objects, and you iterate over the `Scheduler` object to receive
 > events as they become due.
 >
 > `Scheduler` also benefits from thirty years of improvements
-> to `sched.scheduler`.  In particular, big reimplements the
-> bulk of the `sched.scheduler` test suite, to ensure that
+> to `sched.scheduler`.  In particular, **big** reimplements the
+> relevant parts of the `sched.scheduler` test suite, to ensure that
 > `Scheduler` never repeats the historical problems discovered
 > over the lifetime of `sched.scheduler`.
 
 #### `Event(scheduler, event, time, priority, sequence)`
 
 > An object representing a scheduled event in a `Scheduler`.
 > You shouldn't need to create them manually; `Event` objects
@@ -1123,15 +1146,15 @@
 ## `big.text`
 
 Functions for working with text strings.  There are
 several families of functions inside the `text` module;
 for a higher-level view of those families, read the
 following deep-dives:
 
-* [**The `multi-` family of functions**](#The-multi--family-of-functions)
+* [**The `multi-` family of string functions**](#The-multi--family-of-string-functions)
 * [**`lines` and lines modifier functions**](#lines-and-lines-modifier-functions)
 * [**Word wrapping and formatting**](#word-wrapping-and-formatting)
 
 All the functions in `big.text` will work with either
 `str` or `bytes` objects, except the three
 [**Word wrapping and formatting**](#word-wrapping-and-formatting)
 functions.  When working with `bytes`,
@@ -1556,15 +1579,15 @@
 >     big.text.multipartition('aXYbYXc', ('X', 'Y',), count=2, separate=True ) => ('a', 'X', '', 'Y', 'bYXc')
 >
 > If `reverse` is true, multipartition behaves like `str.rpartition`.
 > It partitions starting on the right, scanning backwards through s
 > looking for separators.
 >
 > For more information, see the deep-dive on
-> [**The `multi-` family of functions.**](#The-multi--family-of-functions)
+> [**The `multi-` family of string functions.**](#The-multi--family-of-string-functions)
 
 #### `multisplit(s, separators, *, keep=False, maxsplit=-1, reverse=False, separate=False, strip=False)`
 
 > Splits strings like `str.split`, but with multiple separators and options.
 >
 > `s` can be `str` or `bytes`.
 >
@@ -1617,15 +1640,15 @@
 >            are one big separator.
 >        true
 >            Don't group separators together.  Each separator should
 >            split the string individually, even if there are no
 >            characters between two separators.
 >
 > `strip` indicates whether multisplit should strip separators from
-> the beginning and/or end of `s`.  It supports six values:
+> the beginning and/or end of `s`.  It supports five values:
 >
 >        false (the default)
 >            Don't strip separators from the beginning or end of "s".
 >        true (apart from LEFT, RIGHT, and PROGRESSIVE)
 >            Strip separators from the beginning and end of "s"
 >            (similarly to `str.strip`).
 >        LEFT
@@ -1670,15 +1693,15 @@
 >
 >    If you pass in a true value for `reverse`, `multisplit` will prefer
 >    the rightmost overlapping separator:
 >
 >        multisplit("A x x Z", (" x ",), keep=big.ALTERNATING, reverse=True) => "A x", " x ", "Z"
 >
 > For more information, see the deep-dive on
-> [**The `multi-` family of functions.**](#The-multi--family-of-functions)
+> [**The `multi-` family of string functions.**](#The-multi--family-of-string-functions)
 
 #### `multistrip(s, separators, left=True, right=True)`
 
 > Like `str.strip`, but supports stripping multiple substrings from `s`.
 >
 > Strips from the string `s` all leading and trailing instances of strings
 > found in `separators`.
@@ -1698,15 +1721,15 @@
 > doesn't match one of the separators.
 >
 > Returns a copy of `s` with the leading and/or trailing
 > separators stripped.  (If `left` and `right` are both
 > false, returns `s` unchanged.)
 >
 > For more information, see the deep-dive on
-> [**The `multi-` family of functions.**](#The-multi--family-of-functions)
+> [**The `multi-` family of string functions.**](#The-multi--family-of-string-functions)
 
 #### `newlines`
 
 > A list of all newline characters recognized by Python.
 > Includes many Unicode newline characters, like `'\u2029'`
 > (a paragraph separator).  Useful as a list of separator
 > strings for
@@ -2084,27 +2107,28 @@
 > ends with microseconds if the type of `t` can represent
 > fractional seconds: a float, a `datetime` object, or the
 > value `None`.
 
 
 # Topic deep-dives
 
-## The `multi-` family of functions
+## The `multi-` family of string functions
 
-This family of functions was inspired by Python's `str.strip`,
+This family of string functions was inspired by Python's `str.strip`,
 `str.rstrip`, and `str.splitlines` functions.  These functions
 are well-designed, and often do what you want.  But they're
 surprisingly opinionated.  And... what if your use case doesn't
 fit exactly into their narrow functionality?  `str.strip`
 supports two specific modes of operation; if you want
 to split your string in a slightly different way, you
 probably can't use `str.strip`.
 
-So what *can* you use?  There's `re.strip`, but it can be
-hard to use.  Now there's a new answer:
+So what *can* you use?  There's `re.strip`, but that can be
+hard to use.<sup id=back_to_re_strip><a href=#re_strip_footnote>1</a></sup>
+Now there's a new answer:
 [`multisplit`.](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse)
 
 [`multisplit`'s](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse)
 goal is to be the be-all end-all string splitting function.
 It's designed to replace every mode of operation for
 `str.split`, `str.rstrip`, and `str.splitlines`, and it
 can even replace `str.partition` and `str.rpartition`.
@@ -2122,16 +2146,15 @@
 format.
 
 The cornerstone of [`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse)
 is the `separators` argument.
 This is an iterable of strings, of the same type (`str` or `bytes`)
 as the string you want to split (`s`).  `multisplit` will split
 the string at *each* non-overlapping instance of any string
-specified in `separators`.  Internally, `multisplit` is
-implemented using `re.split` for speed.
+specified in `separators`.
 
 [`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse)
 also let you fine-tune how it splits, through five keyword-only
 parameters:
 
 * `keep` lets you include the separator strings in the output,
   in a number of different formats.
@@ -2329,15 +2352,15 @@
     >>> list(big.multisplit('appleXYbananaYXYcookie', ('X', 'Y'), separate=True, keep=big.AS_PAIRS))
     [('apple', 'X'), ('', 'Y'), ('banana', 'Y'), ('', 'X'), ('', 'Y'), ('cookie', '')]
 ```
 
 #### `strip`
 
 `strip` indicates whether multisplit should strip separators from
-the beginning and/or end of `s`.  It supports six values:
+the beginning and/or end of `s`.  It supports five values:
 false, true, `big.LEFT`, `big.RIGHT`, and `big.PROGRESSIVE`.
 
 By default, `strip` is false, which means it doesn't strip any
 leading or trailing separators:
 
 ```Python
     >>> list(big.multisplit('XYappleXbananaYcookieYXY', ('X', 'Y'))) # strip defaults to False
@@ -2796,15 +2819,15 @@
 
 The output of [`lines`](#liness-separatorsnone--line_number1-column_number1-tab_width8-kwargs) can be modified by "lines modifier"
 functions.  These are functions that iterate over a lines
 iterator and re-yield the values, possibly modifying or
 discarding them along the way.  For example, passing
 a [`lines`](#liness-separatorsnone--line_number1-column_number1-tab_width8-kwargs) iterator into `lines_filter_empty_lines` results
 in an iterator that skips over the empty lines.
-All the lines modifier functions that ship with big
+All the lines modifier functions that ship with **big**
 start with the string `lines_`.
 
 Actually there are additional constraints on lines modifier
 function names.  The second word in the function name,
 immediately after `lines_`, may denote the lines modifier's
 category.  Some examples:
 
@@ -3480,17 +3503,36 @@
   class from the `__init__` of the outer class, which should allow
   the code to cache the bound inner class instance before a second
   thread could ever get a reference to the outer object.
 
 
 ## Release history
 
-**0.9.1** *2023/0628*
+**0.9.2** *2023/07/22*
+
+Extremely minor release.  No new features or bug fixes.
 
-* Added the new [`big.log`](#biglog) module, with its new [`Log`](#log) class!
+* Fixed coverage, now back to the usual 100%.
+  (This just required changing the tests, which
+  *didn't* find any new bugs.)
+* Made the tests for [`Log`](#log-clocknone)
+  deterministic.  They now use a fake clock
+  that always returns the same values.
+* Added GitHub Actions integration.  Tests and
+  coverage are run in the cloud after every checkin.
+  Thanks to [Dan Pope](https://github.com/lordmauve)
+  for gently walking me through this!
+* Fixed metadata in the `pyproject.toml` file.
+* Added badges for testing, coverage,
+  and supported Python versions.
+
+**0.9.1** *2023/06/28*
+
+* Added the new [`big.log`](#biglog) module, with its new
+  [`Log`](#log-clocknone) class!
   I wrote this for another project--but it turned out so nice
   I just had to add it to **big**!
 
 **0.9** *2023/06/15*
 
 * Bugfix!  If an outer class `Outer` had an inner class `Inner`
   decorated with `@BoundInnerClass`, and `o` is an instance of
@@ -3840,15 +3882,15 @@
 * Completely retooled and upgraded
   [`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse),
   and added
   [`multistrip`](#multistrips-separators-leftTrue-rightTrue)
   and
   [`multipartition`,](#multipartitions-separators-count1--reverseFalse-separateTrue)
   collectively called
-  [**The `multi-` family of functions.**](#The-multi--family-of-functions)
+  [**The `multi-` family of string functions.**](#The-multi--family-of-string-functions)
   (Thanks to Eric Smith for suggesting
   [`multipartition`!](#multipartitions-separators-count1--reverseFalse-separateTrue)
   Well, sort of.)
   * `[`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse)`
     now supports five (!) keyword-only parameters, allowing the caller
     to tune its behavior to an amazing degree.
   * Also, the original implementation of
@@ -3915,7 +3957,14 @@
   If the colon is not followed by a space, turns the colon into `'-'`.
   This is good for tiresome modern gobbledygook like `'Re:code'`, which
   will now be translated to `'Re-code'`.
 
 **0.5** *2022/06/12*
 
 * Initial release.
+
+
+------------------------
+
+<ol><li id="re_strip_footnote"><p>
+I should know, `multisplit` is implemented using `re.split`!
+</p></li></ol>
```

### Comparing `big-0.9.1/big/__init__.py` & `big-0.9.2/big/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR
 THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
```

### Comparing `big-0.9.1/big/all.py` & `big-0.9.2/big/all.py`

 * *Files identical despite different names*

### Comparing `big-0.9.1/big/boundinnerclass.py` & `big-0.9.2/big/boundinnerclass.py`

 * *Files identical despite different names*

### Comparing `big-0.9.1/big/builtin.py` & `big-0.9.2/big/builtin.py`

 * *Files identical despite different names*

### Comparing `big-0.9.1/big/file.py` & `big-0.9.2/big/file.py`

 * *Files identical despite different names*

### Comparing `big-0.9.1/big/graph.py` & `big-0.9.2/big/graph.py`

 * *Files identical despite different names*

### Comparing `big-0.9.1/big/heap.py` & `big-0.9.2/big/heap.py`

 * *Files identical despite different names*

### Comparing `big-0.9.1/big/itertools.py` & `big-0.9.2/big/itertools.py`

 * *Files identical despite different names*

### Comparing `big-0.9.1/big/log.py` & `big-0.9.2/big/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 
 import builtins
 
 try:
     # new in 3.7
     from time import monotonic_ns as default_clock
-except ImportError:
+except ImportError: # pragma: no cover
     from time import perf_counter
     def default_clock():
         return int(perf_counter() * 1000000000.0)
 
 
 class Log:
     """
@@ -62,14 +62,22 @@
         log.exit()
     And finally print the log:
         log.print()
 
     You can also iterate over the log events using iter(log).
     This yields 4-tuples:
         (start_time, elapsed_time, event, depth)
+    start_time and elapsed_time are times, expressed as
+    an integer number of nanoseconds.  The first event
+    is at start_time 0, and all subsequent start times are
+    relative to that time.  event is the event string you
+    passed in to log() (or "<subsystem> start" or
+    "<subsystem> end").  depth is an integer indicating
+    how many subsystems the event is nested in; larger
+    numbers indicate deeper nesting.
     """
 
     # Internally, all times are stored relative to
     # the logging start time.
     # Writing this any other way was *madness.*
     # (You're dealing with 15-digit numbers that change
     # randomly in the last... seven? digits.  You'll go blind!)
@@ -162,15 +170,15 @@
             print = builtins.print
 
         indent = " " * indent
         column_width = seconds_width + 1 + fractional_width
 
         def format_time(t):
             assert t is not None
-            seconds = t // 1000000000
+            seconds = t // 1_000_000_000
             nanoseconds = f"{t - seconds:>09}"
             nanoseconds = nanoseconds[:fractional_width]
             return f"{seconds:0{seconds_width}}.{nanoseconds}"
 
         if title:
             print(title)
```

### Comparing `big-0.9.1/big/scheduler.py` & `big-0.9.2/big/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,16 +238,18 @@
     Also, sched.scheduler is thirty years behind the times in
     Python API design.  Its events are callbacks, which it
     calls.  Scheduler fixes this: its events are objects,
     and you iterate over the Scheduler object to receive
     events as they become due.
 
     Scheduler also benefits from thirty years of improvements
-    to sched.scheduler, and in particular reimplements the
-    entire (relevant portion of the) sched.scheduler test suite.
+    to sched.scheduler.  In particular, big reimplements the
+    bulk of the sched.scheduler test suite, to ensure that
+    Scheduler never repeats the historical problems discovered
+    over the lifetime of sched.scheduler.
 
     The only argument to Scheduler is an instance of Regulator,
     that provides time and thread-safety to the Scheduler.
     By default Scheduler uses an instance of
     SingleThreadedRegulator, which is not thread-safe.
 
     (If you need the scheduler to be thread-safe, pass in
```

### Comparing `big-0.9.1/big/text.py` & `big-0.9.2/big/text.py`

 * *Files identical despite different names*

### Comparing `big-0.9.1/big/time.py` & `big-0.9.2/big/time.py`

 * *Files identical despite different names*

### Comparing `big-0.9.1/resources/experiments/alice.in.wonderland.txt` & `big-0.9.2/resources/experiments/alice.in.wonderland.txt`

 * *Files identical despite different names*

### Comparing `big-0.9.1/resources/experiments/time_multisplit.py` & `big-0.9.2/resources/experiments/time_multisplit.py`

 * *Files identical despite different names*

### Comparing `big-0.9.1/resources/images/big.header.png` & `big-0.9.2/resources/images/big.header.png`

 * *Files identical despite different names*

### Comparing `big-0.9.1/tests/bigtestlib.py` & `big-0.9.2/tests/bigtestlib.py`

 * *Files identical despite different names*

### Comparing `big-0.9.1/tests/test_all.py` & `big-0.9.2/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `big-0.9.1/tests/test_boundinnerclass.py` & `big-0.9.2/tests/test_boundinnerclass.py`

 * *Files identical despite different names*

### Comparing `big-0.9.1/tests/test_builtin.py` & `big-0.9.2/tests/test_builtin.py`

 * *Files identical despite different names*

### Comparing `big-0.9.1/tests/test_file.py` & `big-0.9.2/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `big-0.9.1/tests/test_graph.py` & `big-0.9.2/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `big-0.9.1/tests/test_heap.py` & `big-0.9.2/tests/test_heap.py`

 * *Files identical despite different names*

### Comparing `big-0.9.1/tests/test_itertools.py` & `big-0.9.2/tests/test_itertools.py`

 * *Files identical despite different names*

### Comparing `big-0.9.1/tests/test_log.py` & `big-0.9.2/tests/test_log.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,95 +23,98 @@
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR
 THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 import bigtestlib
 bigtestlib.preload_local_big()
 
+import builtins
 import big.all as big
 import unittest
 import time
 
+def fake_clock():
+    def fake_clock():
+        time = 0
+        while True:
+            yield time
+            time += 12_000_000 # add twelve milliseconds
+    return fake_clock().__next__
+
 class BigTestLog(unittest.TestCase):
 
     maxDiff=None
 
     def test_smoke_test_log(self):
-        sleep = time.sleep
-
-        # perform all the lookups first
-        # so that the actual logging is as efficient as possible
-        log = big.Log()
-        log_enter = log.enter
-        log_exit = log.exit
-        log_print = log.print
-        got = []
-        got_append = got.append
+        clock = fake_clock()
+        log = big.Log(clock=clock)
 
         log.reset()
-        log_enter("subsystem")
-        sleep(0.01)
+        log.enter("subsystem")
         log('event 1')
-        sleep(0.02)
+        clock()
         log('event 2')
-        sleep(0.03)
-        log_exit()
-        log_print(print=got_append, fractional_width=3)
+        log.exit()
+        got = []
+        log.print(print=got.append, fractional_width=3)
 
         expected = """
 [event log]
   start   elapsed  event
   ------  ------  ---------------
-  00.000  00.000  log start
-  00.000  00.010  subsystem start
-  00.010  00.020    event 1
-  00.030  00.030    event 2
+  00.000  00.012  log start
+  00.012  00.012  subsystem start
+  00.024  00.024    event 1
+  00.048  00.012    event 2
   00.060  00.000  subsystem end
         """.strip().split('\n')
 
-        # we can't simply compare text strings.
-        # maybe your computer is slow!
-        # maybe the scheduler paused the test program for a moment!
-        # the final time might be 00.061!
-        #
-        # so, do this the hard way.
+        self.assertEqual(expected, got)
 
         i_got = iter(got)
         i_expected = iter(expected)
 
-        self.assertEqual(next(i_expected), next(i_got), "error on log line 1: [event log] line didn't match!")
-        self.assertEqual(next(i_expected), next(i_got), "error on log line 2: column heading text line didn't match!")
-        self.assertEqual(next(i_expected), next(i_got), "error on log line 3: column heading dashes line didn't match!")
-
-        # time should pass by *at least* this much.
         per_line_elapsed = [
-            0,
-            0.01,
-            0.02,
-            0.03,
+            0.012,
+            0.012,
+            0.024,
+            0.012,
             0.0
             ]
 
         def split_line(s):
             s = s.strip()
             start_time, _, s = s.partition("  ")
             assert _
             elapsed_time, _, s = s.partition("  ")
             assert _
             return (float(start_time), float(elapsed_time), s)
 
         expected_start_time = 0
-        for line_number, (expected, got, expected_elapsed_time) in enumerate(zip(i_expected, i_got, per_line_elapsed), 4):
+        for line_number, (expected, got, expected_elapsed_time) in enumerate(zip(i_expected, i_got, per_line_elapsed)):
+            if line_number < 3:
+                self.assertEqual(expected, got)
+                continue
             _, _, expected_event = split_line(expected)
             got_start_time, got_elapsed_time, got_event = split_line(got)
             self.assertEqual(got_start_time, expected_start_time, f"error on log line {line_number}: start time didn't match! expected {expected_start_time}, got {got_start_time}")
             self.assertGreaterEqual(got_elapsed_time, expected_elapsed_time, f"error on log line {line_number}: elapsed time didn't match! expected {expected_elapsed_time}, got {got_elapsed_time}")
             self.assertEqual(got_event, expected_event, f"error on log line {line_number}: event didn't match! expected {expected_event!r}, got {got_event!r}")
             expected_start_time += got_elapsed_time
 
+    def test_default_settings(self):
+        log = big.Log()
+        log('event 1')
+        buffer = []
+        real_print = builtins.print
+        builtins.print = buffer.append
+        log.print()
+        builtins.print = real_print
+        got = "\n".join(buffer)
+        self.assertIn("event 1", got)
 
 
 def run_tests():
     bigtestlib.run(name="big.log", module=__name__)
 
 if __name__ == "__main__": # pragma: no cover
     run_tests()
```

### Comparing `big-0.9.1/tests/test_scheduler.py` & `big-0.9.2/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `big-0.9.1/tests/test_text.py` & `big-0.9.2/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `big-0.9.1/tests/test_time.py` & `big-0.9.2/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `big-0.9.1/PKG-INFO` & `big-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 Metadata-Version: 2.1
 Name: big
-Version: 0.9.1
+Version: 0.9.2
 Summary: The big package is a grab-bag of cool code for use in your programs.
 Author-email: Larry Hastings <larry@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: python-dateutil ; extra == "test"
 Requires-Dist: regex ; extra == "test"
+Requires-Dist: inflect ; extra == "test"
 Requires-Dist: python-dateutil ; extra == "time"
 Project-URL: Source, https://github.com/larryhastings/big/
 Provides-Extra: test
 Provides-Extra: time
 
 ![# big](https://raw.githubusercontent.com/larryhastings/big/master/resources/images/big.header.png)
 
 ##### Copyright 2022-2023 by Larry Hastings
 
+[![# test badge](https://img.shields.io/github/actions/workflow/status/larryhastings/big/test.yml?branch=master&label=test)](https://github.com/larryhastings/big/actions/workflows/test.yml)
+[![# coverage badge](https://img.shields.io/github/actions/workflow/status/larryhastings/big/coverage.yml?branch=master&label=coverage)](https://github.com/larryhastings/big/actions/workflows/coverage.yml)
+[![# python versions badge](https://img.shields.io/pypi/pyversions/big.svg?logo=python&logoColor=FBE072)](https://pypi.org/project/big/)
+
+
 **big** is a Python package, a grab-bag of useful technology
 I always want to have handy.
 
 Finally!  For years, I've copied-and-pasted all my little
 helper functions between projects--we've all done it.
 But now I've finally taken the time to consolidate all those
 useful little functions into one big package, so they're always
@@ -73,17 +87,18 @@
 
 ```Python
 from big.all import *
 ```
 
 but that's up to you.
 
-**big** is licensed using the [MIT license.](https://opensource.org/licenses/MIT)
-You're free to use it and even ship it in your own programs, as long as you leave my copyright
-notice on the source code.
+**big** is licensed using the
+[MIT license.](https://opensource.org/licenses/MIT)
+You're free to use it and even ship it in your own programs,
+as long as you leave my copyright notice on the source code.
 
 # Index
 
 [`ascii_newlines`](#newlines)
 
 [`ascii_newlines_without_dos`](#newlines)
 
@@ -183,21 +198,21 @@
 
 [`lines_strip(li)`](#lines_stripli)
 
 [`lines_strip_comments(li, comment_separators, *, quotes=('"', "'"), backslash='\\', rstrip=True, triple_quotes=True)`](#lines_strip_commentsli-comment_separators--quotes--backslash-rstriptrue-triple_quotestrue)
 
 [`lines_strip_indent(li)`](#lines_strip_indentli)
 
-[`Log`](#log)
+[`Log`](#log-clocknone)
 
 [`Log.enter(subsystem)`](#logentersubsystem)
 
 [`Log.exit()`](#logexit)
 
-[`Log.print(*, print=None, title="[event log]", headings=True, indent=2, seconds_width=2, fractional_width=9)`](#logprint--printnone-titleeventlog-headingstrue-indent2-seconds_width2-fractional_width9)
+[`Log.print(*, print=None, title="[event log]", headings=True, indent=2, seconds_width=2, fractional_width=9)`](#logprint-printnone-titleevent-log-headingstrue-indent2-seconds_width2-fractional_width9)
 
 [`Log.reset()`](#logreset)
 
 [`merge_columns(*columns, column_separator=" ", overflow_response=OverflowResponse.RAISE, overflow_before=0, overflow_after=0)`](#merge_columnscolumns-column_separator--overflow_responseoverflowresponseraise-overflow_before0-overflow_after0)
 
 [`multipartition(s, separators, count=1, *, reverse=False, separate=True)`](#multipartitions-separators-count1--reverseFalse-separateTrue)
 
@@ -313,15 +328,15 @@
 
 [`whitespace`](#whitespace)
 
 [`whitespace_without_dos`](#whitespace)
 
 [`wrap_words(words, margin=79, *, two_spaces=True)`](#wrap_wordswords-margin79--two_spacestrue)
 
-[**The `multi-` family of functions**](#The-multi--family-of-functions)
+[**The `multi-` family of string functions**](#The-multi--family-of-string-functions)
 
 [**`lines` and lines modifier functions**](#lines-and-lines-modifier-functions)
 
 [**Word wrapping and formatting**](#word-wrapping-and-formatting)
 
 [**Bound inner classes**](#bound-inner-classes)
 
@@ -839,21 +854,24 @@
 
 A simple and lightweight logging class, useful for performance analysis.
 Not intended as a full-fledged logging facility like Python's
 [`logging`](https://docs.python.org/3/library/logging.html) module.
 
 #### `default_clock()`
 
-> The default clock function used by the `Log` class.
+> The default clock function used by the [`Log`](#log-clocknone) class.
 > This function returns elapsed time in nanoseconds,
 > expressed as an integer.
 >
 > In Python 3.7+,
-> this is `time.monotonic_ns`; in Python 3.6 this is
-> a custom function that calls `time.perf_counter`,
+> this is
+> [`time.monotonic_ns`](https://docs.python.org/3/library/time.html#time.monotonic_ns);
+> in Python 3.6 this is
+> a custom function that calls
+> [`time.perf_counter`](https://docs.python.org/3/library/time.html#time.perf_counter),
 > then converts that time to requisite format.
 
 #### `Log(*, clock=None)`
 
 > A simple and lightweight logging class, useful for performance analysis.
 > Not intended as a full-fledged logging facility like Python's
 > [`logging`](https://docs.python.org/3/library/logging.html) module.
@@ -885,14 +903,28 @@
 >
 >     log.print()
 >
 > You can also iterate over the log events using `iter(log)`.
 > This yields 4-tuples:
 >
 >     (start_time, elapsed_time, event, depth)
+>
+> `start_time` and `elapsed_time` are times, expressed as
+> an integer number of nanoseconds.  The first event
+> is at `start_time` 0, and all subsequent start times are
+> relative to that time.
+>
+> `event` is the event string you
+> passed in to `log()` (or `"<subsystem> start"` or
+> `"<subsystem> end"`).
+>
+> `depth` is an integer indicating
+> how many subsystems the event is nested in; larger
+> numbers indicate deeper nesting.
+
 
 #### `Log.enter(subsystem)`
 
 > Notifies the log that you've entered a subsystem.
 > The `subsystem` parameter should be a string describing the subsystem.
 >
 > This is really just a presentation
@@ -960,16 +992,16 @@
 > Python API design--its design predates many common modern
 > Python conventions.  Its events are callbacks, which it
 > calls directly.  `Scheduler` fixes this: its events are
 > objects, and you iterate over the `Scheduler` object to receive
 > events as they become due.
 >
 > `Scheduler` also benefits from thirty years of improvements
-> to `sched.scheduler`.  In particular, big reimplements the
-> bulk of the `sched.scheduler` test suite, to ensure that
+> to `sched.scheduler`.  In particular, **big** reimplements the
+> relevant parts of the `sched.scheduler` test suite, to ensure that
 > `Scheduler` never repeats the historical problems discovered
 > over the lifetime of `sched.scheduler`.
 
 #### `Event(scheduler, event, time, priority, sequence)`
 
 > An object representing a scheduled event in a `Scheduler`.
 > You shouldn't need to create them manually; `Event` objects
@@ -1139,15 +1171,15 @@
 ## `big.text`
 
 Functions for working with text strings.  There are
 several families of functions inside the `text` module;
 for a higher-level view of those families, read the
 following deep-dives:
 
-* [**The `multi-` family of functions**](#The-multi--family-of-functions)
+* [**The `multi-` family of string functions**](#The-multi--family-of-string-functions)
 * [**`lines` and lines modifier functions**](#lines-and-lines-modifier-functions)
 * [**Word wrapping and formatting**](#word-wrapping-and-formatting)
 
 All the functions in `big.text` will work with either
 `str` or `bytes` objects, except the three
 [**Word wrapping and formatting**](#word-wrapping-and-formatting)
 functions.  When working with `bytes`,
@@ -1572,15 +1604,15 @@
 >     big.text.multipartition('aXYbYXc', ('X', 'Y',), count=2, separate=True ) => ('a', 'X', '', 'Y', 'bYXc')
 >
 > If `reverse` is true, multipartition behaves like `str.rpartition`.
 > It partitions starting on the right, scanning backwards through s
 > looking for separators.
 >
 > For more information, see the deep-dive on
-> [**The `multi-` family of functions.**](#The-multi--family-of-functions)
+> [**The `multi-` family of string functions.**](#The-multi--family-of-string-functions)
 
 #### `multisplit(s, separators, *, keep=False, maxsplit=-1, reverse=False, separate=False, strip=False)`
 
 > Splits strings like `str.split`, but with multiple separators and options.
 >
 > `s` can be `str` or `bytes`.
 >
@@ -1633,15 +1665,15 @@
 >            are one big separator.
 >        true
 >            Don't group separators together.  Each separator should
 >            split the string individually, even if there are no
 >            characters between two separators.
 >
 > `strip` indicates whether multisplit should strip separators from
-> the beginning and/or end of `s`.  It supports six values:
+> the beginning and/or end of `s`.  It supports five values:
 >
 >        false (the default)
 >            Don't strip separators from the beginning or end of "s".
 >        true (apart from LEFT, RIGHT, and PROGRESSIVE)
 >            Strip separators from the beginning and end of "s"
 >            (similarly to `str.strip`).
 >        LEFT
@@ -1686,15 +1718,15 @@
 >
 >    If you pass in a true value for `reverse`, `multisplit` will prefer
 >    the rightmost overlapping separator:
 >
 >        multisplit("A x x Z", (" x ",), keep=big.ALTERNATING, reverse=True) => "A x", " x ", "Z"
 >
 > For more information, see the deep-dive on
-> [**The `multi-` family of functions.**](#The-multi--family-of-functions)
+> [**The `multi-` family of string functions.**](#The-multi--family-of-string-functions)
 
 #### `multistrip(s, separators, left=True, right=True)`
 
 > Like `str.strip`, but supports stripping multiple substrings from `s`.
 >
 > Strips from the string `s` all leading and trailing instances of strings
 > found in `separators`.
@@ -1714,15 +1746,15 @@
 > doesn't match one of the separators.
 >
 > Returns a copy of `s` with the leading and/or trailing
 > separators stripped.  (If `left` and `right` are both
 > false, returns `s` unchanged.)
 >
 > For more information, see the deep-dive on
-> [**The `multi-` family of functions.**](#The-multi--family-of-functions)
+> [**The `multi-` family of string functions.**](#The-multi--family-of-string-functions)
 
 #### `newlines`
 
 > A list of all newline characters recognized by Python.
 > Includes many Unicode newline characters, like `'\u2029'`
 > (a paragraph separator).  Useful as a list of separator
 > strings for
@@ -2100,27 +2132,28 @@
 > ends with microseconds if the type of `t` can represent
 > fractional seconds: a float, a `datetime` object, or the
 > value `None`.
 
 
 # Topic deep-dives
 
-## The `multi-` family of functions
+## The `multi-` family of string functions
 
-This family of functions was inspired by Python's `str.strip`,
+This family of string functions was inspired by Python's `str.strip`,
 `str.rstrip`, and `str.splitlines` functions.  These functions
 are well-designed, and often do what you want.  But they're
 surprisingly opinionated.  And... what if your use case doesn't
 fit exactly into their narrow functionality?  `str.strip`
 supports two specific modes of operation; if you want
 to split your string in a slightly different way, you
 probably can't use `str.strip`.
 
-So what *can* you use?  There's `re.strip`, but it can be
-hard to use.  Now there's a new answer:
+So what *can* you use?  There's `re.strip`, but that can be
+hard to use.<sup id=back_to_re_strip><a href=#re_strip_footnote>1</a></sup>
+Now there's a new answer:
 [`multisplit`.](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse)
 
 [`multisplit`'s](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse)
 goal is to be the be-all end-all string splitting function.
 It's designed to replace every mode of operation for
 `str.split`, `str.rstrip`, and `str.splitlines`, and it
 can even replace `str.partition` and `str.rpartition`.
@@ -2138,16 +2171,15 @@
 format.
 
 The cornerstone of [`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse)
 is the `separators` argument.
 This is an iterable of strings, of the same type (`str` or `bytes`)
 as the string you want to split (`s`).  `multisplit` will split
 the string at *each* non-overlapping instance of any string
-specified in `separators`.  Internally, `multisplit` is
-implemented using `re.split` for speed.
+specified in `separators`.
 
 [`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse)
 also let you fine-tune how it splits, through five keyword-only
 parameters:
 
 * `keep` lets you include the separator strings in the output,
   in a number of different formats.
@@ -2345,15 +2377,15 @@
     >>> list(big.multisplit('appleXYbananaYXYcookie', ('X', 'Y'), separate=True, keep=big.AS_PAIRS))
     [('apple', 'X'), ('', 'Y'), ('banana', 'Y'), ('', 'X'), ('', 'Y'), ('cookie', '')]
 ```
 
 #### `strip`
 
 `strip` indicates whether multisplit should strip separators from
-the beginning and/or end of `s`.  It supports six values:
+the beginning and/or end of `s`.  It supports five values:
 false, true, `big.LEFT`, `big.RIGHT`, and `big.PROGRESSIVE`.
 
 By default, `strip` is false, which means it doesn't strip any
 leading or trailing separators:
 
 ```Python
     >>> list(big.multisplit('XYappleXbananaYcookieYXY', ('X', 'Y'))) # strip defaults to False
@@ -2812,15 +2844,15 @@
 
 The output of [`lines`](#liness-separatorsnone--line_number1-column_number1-tab_width8-kwargs) can be modified by "lines modifier"
 functions.  These are functions that iterate over a lines
 iterator and re-yield the values, possibly modifying or
 discarding them along the way.  For example, passing
 a [`lines`](#liness-separatorsnone--line_number1-column_number1-tab_width8-kwargs) iterator into `lines_filter_empty_lines` results
 in an iterator that skips over the empty lines.
-All the lines modifier functions that ship with big
+All the lines modifier functions that ship with **big**
 start with the string `lines_`.
 
 Actually there are additional constraints on lines modifier
 function names.  The second word in the function name,
 immediately after `lines_`, may denote the lines modifier's
 category.  Some examples:
 
@@ -3496,17 +3528,36 @@
   class from the `__init__` of the outer class, which should allow
   the code to cache the bound inner class instance before a second
   thread could ever get a reference to the outer object.
 
 
 ## Release history
 
-**0.9.1** *2023/0628*
+**0.9.2** *2023/07/22*
+
+Extremely minor release.  No new features or bug fixes.
 
-* Added the new [`big.log`](#biglog) module, with its new [`Log`](#log) class!
+* Fixed coverage, now back to the usual 100%.
+  (This just required changing the tests, which
+  *didn't* find any new bugs.)
+* Made the tests for [`Log`](#log-clocknone)
+  deterministic.  They now use a fake clock
+  that always returns the same values.
+* Added GitHub Actions integration.  Tests and
+  coverage are run in the cloud after every checkin.
+  Thanks to [Dan Pope](https://github.com/lordmauve)
+  for gently walking me through this!
+* Fixed metadata in the `pyproject.toml` file.
+* Added badges for testing, coverage,
+  and supported Python versions.
+
+**0.9.1** *2023/06/28*
+
+* Added the new [`big.log`](#biglog) module, with its new
+  [`Log`](#log-clocknone) class!
   I wrote this for another project--but it turned out so nice
   I just had to add it to **big**!
 
 **0.9** *2023/06/15*
 
 * Bugfix!  If an outer class `Outer` had an inner class `Inner`
   decorated with `@BoundInnerClass`, and `o` is an instance of
@@ -3856,15 +3907,15 @@
 * Completely retooled and upgraded
   [`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse),
   and added
   [`multistrip`](#multistrips-separators-leftTrue-rightTrue)
   and
   [`multipartition`,](#multipartitions-separators-count1--reverseFalse-separateTrue)
   collectively called
-  [**The `multi-` family of functions.**](#The-multi--family-of-functions)
+  [**The `multi-` family of string functions.**](#The-multi--family-of-string-functions)
   (Thanks to Eric Smith for suggesting
   [`multipartition`!](#multipartitions-separators-count1--reverseFalse-separateTrue)
   Well, sort of.)
   * `[`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse)`
     now supports five (!) keyword-only parameters, allowing the caller
     to tune its behavior to an amazing degree.
   * Also, the original implementation of
@@ -3932,7 +3983,14 @@
   This is good for tiresome modern gobbledygook like `'Re:code'`, which
   will now be translated to `'Re-code'`.
 
 **0.5** *2022/06/12*
 
 * Initial release.
 
+
+------------------------
+
+<ol><li id="re_strip_footnote"><p>
+I should know, `multisplit` is implemented using `re.split`!
+</p></li></ol>
+
```

