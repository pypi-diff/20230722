# Comparing `tmp/udn_songbook-1.1.6.tar.gz` & `tmp/udn_songbook-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udn_songbook-1.1.6.tar", max compression
+gzip compressed data, was "udn_songbook-1.1.8.tar", max compression
```

## Comparing `udn_songbook-1.1.6.tar` & `udn_songbook-1.1.8.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1662 2023-06-13 21:42:22.016696 udn_songbook-1.1.6/CHANGELOG.md
--rw-r--r--   0        0        0    35150 2023-05-03 20:57:17.787425 udn_songbook-1.1.6/LICENSE.txt
--rw-r--r--   0        0        0     1731 2023-05-03 20:57:17.787425 udn_songbook-1.1.6/README.md
--rw-r--r--   0        0        0     1500 2023-06-13 21:44:59.278514 udn_songbook-1.1.6/pyproject.toml
--rw-r--r--   0        0        0       91 2023-06-13 21:42:22.018696 udn_songbook-1.1.6/udn_songbook/__init__.py
--rw-r--r--   0        0        0     6944 2023-06-13 21:16:36.156515 udn_songbook-1.1.6/udn_songbook/book.py
--rw-r--r--   0        0        0     1043 2023-05-05 10:02:10.536805 udn_songbook-1.1.6/udn_songbook/filters.py
--rw-r--r--   0        0        0     3629 2023-05-25 22:09:08.574890 udn_songbook-1.1.6/udn_songbook/renderer.py
--rw-r--r--   0        0        0    19925 2023-06-13 21:42:22.018696 udn_songbook-1.1.6/udn_songbook/song.py
--rw-r--r--   0        0        0     2771 2023-05-05 10:02:10.537804 udn_songbook-1.1.6/udn_songbook/stylesheets/pdf.css
--rw-r--r--   0        0        0     3517 2023-05-05 10:02:10.537804 udn_songbook-1.1.6/udn_songbook/stylesheets/responsive.css
--rw-r--r--   0        0        0     1270 2023-05-05 10:02:10.538804 udn_songbook-1.1.6/udn_songbook/stylesheets/ukedown_elements.css
--rw-r--r--   0        0        0     1517 2023-06-13 21:16:36.156515 udn_songbook-1.1.6/udn_songbook/templates/base.html.j2
--rw-r--r--   0        0        0     1062 2023-06-13 21:42:22.018696 udn_songbook-1.1.6/udn_songbook/templates/index.html.j2
--rw-r--r--   0        0        0     1298 2023-06-13 21:42:22.018696 udn_songbook-1.1.6/udn_songbook/templates/song.html.j2
--rwxr-xr-x   0        0        0     2778 2023-06-13 21:42:22.018696 udn_songbook-1.1.6/udn_songbook/tools/makesheet.py
--rwxr-xr-x   0        0        0     1990 2023-06-13 21:42:22.018696 udn_songbook-1.1.6/udn_songbook/tools/transpose.py
--rw-r--r--   0        0        0     1037 2023-06-13 21:16:36.157514 udn_songbook-1.1.6/udn_songbook/utils.py
--rw-r--r--   0        0        0     2967 1970-01-01 00:00:00.000000 udn_songbook-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     2114 2023-07-20 21:32:37.419198 udn_songbook-1.1.8/CHANGELOG.md
+-rw-r--r--   0        0        0    35150 2023-05-03 20:57:17.787425 udn_songbook-1.1.8/LICENSE.txt
+-rw-r--r--   0        0        0     2428 2023-07-20 21:28:31.360844 udn_songbook-1.1.8/README.md
+-rw-r--r--   0        0        0     1532 2023-07-20 21:32:50.348426 udn_songbook-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0       91 2023-06-13 21:42:22.018696 udn_songbook-1.1.8/udn_songbook/__init__.py
+-rw-r--r--   0        0        0     6944 2023-06-13 21:16:36.156515 udn_songbook-1.1.8/udn_songbook/book.py
+-rw-r--r--   0        0        0     1043 2023-05-05 10:02:10.536805 udn_songbook-1.1.8/udn_songbook/filters.py
+-rw-r--r--   0        0        0     3629 2023-05-25 22:09:08.574890 udn_songbook-1.1.8/udn_songbook/renderer.py
+-rw-r--r--   0        0        0    20049 2023-07-20 21:28:58.530325 udn_songbook-1.1.8/udn_songbook/song.py
+-rw-r--r--   0        0        0     3080 2023-07-20 21:29:12.388570 udn_songbook-1.1.8/udn_songbook/stylesheets/landscape.css
+-rw-r--r--   0        0        0     2771 2023-07-20 21:28:50.132176 udn_songbook-1.1.8/udn_songbook/stylesheets/portrait.css
+-rw-r--r--   0        0        0     2713 2023-07-20 21:29:12.388570 udn_songbook-1.1.8/udn_songbook/stylesheets/responsive.css
+-rw-r--r--   0        0        0     1270 2023-05-05 10:02:10.538804 udn_songbook-1.1.8/udn_songbook/stylesheets/ukedown_elements.css
+-rw-r--r--   0        0        0     1517 2023-06-13 21:16:36.156515 udn_songbook-1.1.8/udn_songbook/templates/base.html.j2
+-rw-r--r--   0        0        0     1087 2023-07-20 21:29:26.396818 udn_songbook-1.1.8/udn_songbook/templates/index.html.j2
+-rw-r--r--   0        0        0     1298 2023-06-13 21:42:22.018696 udn_songbook-1.1.8/udn_songbook/templates/song.html.j2
+-rwxr-xr-x   0        0        0     3011 2023-07-20 21:29:05.249444 udn_songbook-1.1.8/udn_songbook/tools/makesheet.py
+-rwxr-xr-x   0        0        0     1997 2023-07-20 21:28:31.361844 udn_songbook-1.1.8/udn_songbook/tools/transpose.py
+-rw-r--r--   0        0        0     1401 2023-07-20 21:28:58.530325 udn_songbook-1.1.8/udn_songbook/utils.py
+-rw-r--r--   0        0        0    40930 1970-01-01 00:00:00.000000 udn_songbook-1.1.8/PKG-INFO
```

### Comparing `udn_songbook-1.1.6/CHANGELOG.md` & `udn_songbook-1.1.8/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,30 @@
 # CHANGELOG for udn_songbook
 
 This project attempts to adhere to [semantic versioning](https://semver.org)
 
+## 1.1.8
+
+- Fix template for index generation
+- Add latest CSS from ukebook-md
+- Fix singers options in makesheet
+- Unpunctuate song._index_entry for better sorting
+- Rename default stylesheet to 'portrait.css'
+
+## 1.1.7
+
+- README updated with new udn_songbook.Song features
+
+- BUGFIX: default metadata to empty dict if not present in songsheet
+- BUGFIX: use absolute import for Song in transpose.py
+
+## 1.1.6
+
+- Adds README to project files for PyPi
+
 ## 1.1.5
 
 - rename udn_render to udn_songsheet (script entry point)
 - BUGFIX: stop wiping metadata after parsing songsheets
 
 ## 1.1.4
```

### Comparing `udn_songbook-1.1.6/LICENSE.txt` & `udn_songbook-1.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.6/README.md` & `udn_songbook-1.1.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -25,29 +25,49 @@
 How to use the current functionality
 
 (it only does basic things at the moment)
 
 ```python
 from udn_songbook import Song
 s = song('/path/to/filename')
+
+# list the unique chords in the song
+s.chords
+
+# save it to disk
+s.save(outputfile)
+
+# transpose by an arbitrary number of semitones
+s.transpose(semitones)
+
+# generate a PDF from the current song, using built-in templates
+s.pdf()
 ```
 
-And to generate a songbook, use the SongBook class, with a directory of UDN-format songsheets
+And to build a songbook, use the SongBook class, with a directory of UDN-format songsheets
 
 ```python
 from udn_songbook import SongBook
 mybook = SongBook(inputs=['directory1', 'directory2', 'someotherfile.udn'])
 ```
 
 Songbooks have an index auto-generated, and do not support mutiple songs with the same ID (which is essentially "Title - Artist").
-If your inputs include multiple songs in this way, the last one imported will be used. So name them carefully.
 
+If your inputs include multiple songs in this way, the last one imported will be used. So name them carefully.
 
 A Songbook in this context is a collection of song objects with additional metadata, such as an index.
 
+## Tools
+
+The pip package also installs 2 commandline tools, aimed at managing individual songsheets:
+
+`udn_transpose`, which allows in-place (or optionally to a new file) transposing of an existing  songsheet by an arbitrary number of semitones. The transposition is added to metadata
+
+`udn_songsheet`, which renders a UDN songsheet to a file in either PDF (default) or HTML format. it also supports in-place transposition, without affecting the original input file.
+
 ## what you need to use this:
 
 * a directory full of UDN-format files.
 * templates:
   * index.html.j2
   * song.html.j2
 * stylesheets (up to you, you can pass their names and location to the methods)
```

### Comparing `udn_songbook-1.1.6/pyproject.toml` & `udn_songbook-1.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "udn-songbook"
-version = "1.1.6"
+version = "1.1.8"
 description = "songbook and songsheet management for songsheets in ukedown format"
 authors = ["Stuart Sears <stuart@sjsears.com>"]
 include = ["CHANGELOG.md"]
 license = "GPL-3.0-or-later"
 repository = "https://github.com/lanky/udn-songbook"
-readme = [ "README.md" ]
+readme = [ "README.md", "LICENSE.txt", "CHANGELOG.md" ]
+
 [tool.poetry.scripts]
 udn_transpose = "udn_songbook.tools.transpose:main"
 udn_songsheet = "udn_songbook.tools.makesheet:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 ukedown = "^2.0.0"
```

### Comparing `udn_songbook-1.1.6/udn_songbook/book.py` & `udn_songbook-1.1.8/udn_songbook/book.py`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.6/udn_songbook/filters.py` & `udn_songbook-1.1.8/udn_songbook/filters.py`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.6/udn_songbook/renderer.py` & `udn_songbook-1.1.8/udn_songbook/renderer.py`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.6/udn_songbook/song.py` & `udn_songbook-1.1.8/udn_songbook/song.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 # PDF rendering
 from weasyprint import HTML, CSS
 from weasyprint.text.fonts import FontConfiguration
 
 # jinja filters and general utils
 from .filters import custom_filters
-from .utils import safe_filename
+from .utils import unpunctuate, safe_filename
 
 # a slightly doctored version of the ukedown chord pattern, which separates
 # '*' (and any other non-standard chord 'qualities' so we can still transpose
 CHORD = r"\(([A-G][adgijmnsu0-9#b\/A-G]*)([*\+])?\)"
 CRDPATT = re.compile(CHORD)
 
 
@@ -81,14 +81,15 @@
                              headers
         """
         self._checksum = None
         self._load_time = datetime.datetime.now()
         self._mod_time = None
         self._index_entry = None
         self._id = 0
+        self._sort_name = ""
         self.styles_dir = os.path.join(os.path.dirname(__file__), "stylesheets")
         self.location = os.path.dirname(__file__)
         if hasattr(src, "read"):
             # if we're operating on a filehandle
             # or another class that implements 'read'
             self._markup = src.read()
             if hasattr(src, "name"):
@@ -118,18 +119,18 @@
         self.__parse(markup=self._markup)
 
         # update with any parameters...
         for key, val in kwargs.items():
             setattr(self, key, val)
 
         if self._filename is None:
-            self._filename = ("{0.title}_-_{0.artist}.udn".format(self)).lower()
+            self._filename = f"{self.title}_-_{self.artist}.udn".lower()
 
         if self._index_entry is None:
-            self._index_entry = "{0.title} - {0.artist}".format(self)
+            self._index_entry = f"{unpunctuate(self.title)} - {self.artist}"
 
         self.__checksum()
 
     def __unicode__(self):
         return self.songid
 
     def __str__(self):
@@ -195,15 +196,18 @@
         for line in markup.splitlines():
             res = metap.match(line)
             if res is not None:
                 metadata.append(res.group(1))
             else:
                 content.append(line)
         self._markup = "\n".join(content)
-        self._meta = yaml.safe_load("\n".join(metadata))
+        if len(metadata):
+            self._meta = yaml.safe_load("\n".join(metadata))
+        else:
+            self._meta = {}
 
     def __parse(self, **kwargs):
         """
         parses ukedown to set attrs and properties
         processes metadata entries in file, converts markup content to HTML
 
         kwargs:
@@ -341,15 +345,15 @@
         if environment is None:
             environment = self.__get_render_env()
 
         tpl = environment.get_template(template)
         return tpl.render(songbook={}, song=self, output="html", **context)
 
     def pdf(
-        self, stylesheet: str = "pdf.css", destfile: Optional[str] = None, **context
+        self, stylesheet: str = "portrait.css", destfile: Optional[str] = None, **context
     ):
         """
         Generate a PDF songsheet from this song
         This will require weasyprint and a stylesheet
 
         Stylesheets are loaded from the udn_songbook installation dir
         by default, but you can provide a path to a stylesheet of your
@@ -372,15 +376,15 @@
 
         NB at this time, chord diagrams are not generated - this will use the
         external python-fretboard diagram library
         """
         # try the stylesheet provided, as follows:
         # load it as an absolute path
         # load it from the included stylesheets
-        # fall back to the default "pdf.css"
+        # fall back to the default "portrait.css"
 
         stylesdir = os.path.join(self.location, "stylesheets")
 
         fontcfg = FontConfiguration()
         # figure out the stylesheet location
         styles = None
         for sheet in [
@@ -388,15 +392,15 @@
             os.path.join(stylesdir, stylesheet),
         ]:
             if os.path.exists(sheet):
                 styles = CSS(filename=sheet, font_config=fontcfg)
                 break
         if styles is None:
             styles = CSS(
-                filename=os.path.join(stylesdir, "pdf.css"), font_config=fontcfg
+                filename=os.path.join(stylesdir, stylesheet), font_config=fontcfg
             )
 
         content = HTML(string=self.html(**context))
         pdfdoc = content.render(
             stylesheets=[styles],
             presentational_hints=True,
             font_config=fontcfg,
```

### Comparing `udn_songbook-1.1.6/udn_songbook/stylesheets/pdf.css` & `udn_songbook-1.1.8/udn_songbook/stylesheets/portrait.css`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.6/udn_songbook/stylesheets/responsive.css` & `udn_songbook-1.1.8/udn_songbook/stylesheets/responsive.css`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 @charset "utf-8";
+@import 'ukedown_elements.css';
 
-body: {
+body {
     font-family: verdana, sans-serif;
     width: 100%;
-    font-size 0.8em;
+    font-size: 0.8em;
 }
 
 a {
     font-family: verdana, sans-serif;
     font-style: normal;
     font-size: 80%;
 }
@@ -29,15 +30,15 @@
     float: right;
     display: block;
 }
 
 h1 {
     font-family: verdana, sans-serif;
     font-weight: bold;
-    font=size: 0.7em;
+    font-size: 0.7em;
     text-align: center;
     float: top
 }
 
 div.header {
     top: 0;
     left: 0;
@@ -68,83 +69,14 @@
 
 p {
     font-family: verdana, sans-serif;
     font-weight: normal;
     padding: 0px;
 }
 
-/* Box call-outs (repeated chorus etc) */
-.box {
-    padding: 2px;
-    margin: 1px;
-    border: 2px solid black;
-    width: auto
-}
-
-div.box {
-    display: inline-block;
-    padding: 5px;
-}
-
-.box > p {
-    margin-top: 0;
-    margin-bottom: 1em;
-}
-
-.box > p:last-child {
-    margin-bottom: 0;
-}
-
-.box > h2 {
-    margin-top: 0;
-    padding-top: 0;
-}
-
-/* End box definitions*/
-
-/* chord styling - auto bold and enclose in ()*/
-.chord {
-    font-weight: bold;
-}
-.chord:before {
-    content: "("
-}
-.chord:after {
-    content: ")"
-}
-
-/* End  chord definitions*/
-
-
-/* Performance notes etc */
-.notes {
-    font-weight: bold;
-}
-
-.notes:before {
-    content: "["
-}
-
-.notes:after {
-    content: "]";
-}
-
-
-/* Backing vox, italic with () around them */
-.vox {
-    font-style: italic;
-    font-weight: normal;
-}
-.vox:before {
-    content: '(';
-}
-.vox:after {
-    content: ')';
-}
-
 div.footer {
     position: fixed;
     bottom: 0;
     left: 0;
     width: 100%;
     max-height: 10%;
     height: 5;
@@ -200,15 +132,15 @@
 /*
 Responsive design for scaling and columns
 Allows zoom and rotation etc
 uses em-widths which are approx
 1em =~16px
 */
 /* max-width here is approx 991px*/
-@media screen and (min-width: 62em) {
+@media screen and (min-width: 62em) and (orientation: landscape) {
     div.chords {
         width: 100%;
         height: 0;
         max-height: 10vmin;
         position: absolute;
         bottom: 0;
         left: 0;
```

### Comparing `udn_songbook-1.1.6/udn_songbook/stylesheets/ukedown_elements.css` & `udn_songbook-1.1.8/udn_songbook/stylesheets/ukedown_elements.css`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.6/udn_songbook/templates/base.html.j2` & `udn_songbook-1.1.8/udn_songbook/templates/base.html.j2`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.6/udn_songbook/templates/index.html.j2` & `udn_songbook-1.1.8/udn_songbook/templates/index.html.j2`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 <html xmlns="http://www.w3.org/1999/xhtml">
 <head>
     <meta name="viewport" content="width=device-width, initial-scale=1"/>
-    <link rel="stylesheet" type="text/css" href="css/{{ book_css }}.css" />
+    <link rel="stylesheet" type="text/css" href="css/{{ stylesheet }}.css" />
     <title>{{ Songbook }}</title>
     <!-- # also import javascript stuff here if needed -->
 </head>
 <body>
-<div class="header" id="title_index"><h1>{{ song.book.title }} Index</h1></div>
+<div class="header" id="title_index"><h1>{{ songbook.title }} Index</h1></div>
 <div class="index">
-{% for song in songs %}
+{% for title, song in songbook.index.items() %}
     {% if output == "html" %}
         {% set target='songs/%s'| format(song.filename) %}
     {% else %}
         {% set target='#title_%03d'| format(song.id) %}
     {% endif %}
 <a class="indexlink" id="song_{{ song.id}}" href="{{ target }}" alt="{{ song.title }} - {{ song.artist }}">{{ song.title }} - {{ song.artist }}</a><br/>
 {% endfor %}
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
 
-****** {{ song.book.title }} Index ******
-{% for song in songs %} {% if output == "html" %} {% set target='songs/%s'|
-format(song.filename) %} {% else %} {% set target='#title_%03d'| format
-(song.id) %} {% endif %} {{_song.title_}}_-_{{_song.artist_}}
+****** {{ songbook.title }} Index ******
+{% for title, song in songbook.index.items() %} {% if output == "html" %} {%
+set target='songs/%s'| format(song.filename) %} {% else %} {% set
+target='#title_%03d'| format(song.id) %} {% endif %} {{_song.title_}}_-_{
+{_song.artist_}}
 {% endfor %}
 [footer image with social media links]
```

### Comparing `udn_songbook-1.1.6/udn_songbook/templates/song.html.j2` & `udn_songbook-1.1.8/udn_songbook/templates/song.html.j2`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.6/udn_songbook/tools/makesheet.py` & `udn_songbook-1.1.8/udn_songbook/tools/makesheet.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,22 +40,22 @@
         "-v",
         "--verbose",
         action="store_true",
         default=False,
         help="Actually tell me what is being done",
     )
 
-
-    outgrp = parser.add_argument_group("Customised Output", "Options for changing default output")
+    outgrp = parser.add_argument_group(
+        "Customised Output", "Options for changing default output"
+    )
 
     outgrp.add_argument(
         "--singers",
-        action="store_false",
-        default=True,
-        dest="chords",
+        action="store_true",
+        default=False,
         help="Generate a singer's sheet (no chords)",
     )
 
     outgrp.add_argument(
         "--html",
         action="store_true",
         default=False,
@@ -76,22 +76,30 @@
     if opts.output:
         opts.output = Path(opts.output)
     else:
         opts.output = Path(
             Path(opts.filename).with_suffix(".html" if opts.html else ".pdf").name
         )
 
+    if opts.singers:
+        opts.chords = False
+        opts.notes = False
+    else:
+        opts.chords = True
+        opts.notes = True
+
     return opts
 
 
 def main():
     """
     Main functionality
     """
     opts = parse_cmdline(sys.argv[1:])
+    print(opts)
 
     song = Song(opts.filename)
 
     if opts.transpose:
         if opts.verbose:
             print(f"transposing song by {opts.transpose} semitones")
         song.transpose(opts.transpose)
@@ -101,14 +109,17 @@
         sys.exit(1)
 
     if opts.verbose:
         print(f"Writing output to {opts.output}")
 
     if opts.html:
         with open(opts.output, "w") as dest:
-            dest.write(song.html(standalone=True))
+            dest.write(
+                song.html(standalone=True, chords=opts.chords, notes=opts.notes)
+            )
+
     else:
-        song.pdf(destfile=opts.output, chords=opts.chords)
+        song.pdf(destfile=opts.output, chords=opts.chords, notes=opts.notes)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `udn_songbook-1.1.6/udn_songbook/tools/transpose.py` & `udn_songbook-1.1.8/udn_songbook/tools/transpose.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # vim: set ts=4 sts=4 sw=4 et ci nu ft=python:
 import argparse
 import sys
 from typing import List
 
-from .song import Song
+from udn_songbook import Song
 
 """
 A tool using the `udn_songbook` mechanisms to transpose songs by a given number of semitones
 """
 
 
 def parse_cmdline(argv: List[str] = []) -> argparse.Namespace:
```

### Comparing `udn_songbook-1.1.6/udn_songbook/utils.py` & `udn_songbook-1.1.8/udn_songbook/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,24 @@
         try:
             os.makedirs(destdir)
             return True
         except (IOError, OSError) as E:
             logger.exception(f"Unable to create output dir {E.filename} - {E.strerror}")
             raise
 
+def unpunctuate(name: str, replacement: str = "") -> str:
+    """
+    Simply removes punctuation from the given name, for ease of sorting.
+    Args:
+        name(str): the name you want to unpunctuate
+        replacement(str): what to replace punctuation with.
+    """
+    TRANS = {ord(char): replacement for char in punctuation}
+    return name.translate(TRANS)
+
 
 def safe_filename(filename: str) -> str:
     """
     Just simple string translation to remove UNIX-unfriendly characters from filenames
     removes the following characters from filenames:
 
     """
```

