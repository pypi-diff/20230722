# Comparing `tmp/django_tableaux-0.2.tar.gz` & `tmp/django_tableaux-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tableaux-0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_tableaux-0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_tableaux-0.2.tar` & `django_tableaux-0.3.tar`

### file list

```diff
@@ -1,48 +1,42 @@
--rw-r--r--   0        0        0     1809 2023-07-15 17:35:02.160341 django_tableaux-0.2/.gitignore
--rw-r--r--   0        0        0     1099 2023-07-15 17:10:11.497764 django_tableaux-0.2/LICENSE
--rw-r--r--   0        0        0     1113 2023-07-15 16:59:49.675807 django_tableaux-0.2/README.rst
--rw-r--r--   0        0        0     1121 2023-07-16 08:01:26.633734 django_tableaux-0.2/django_tableaux/__init__.py
--rw-r--r--   0        0        0      167 2023-07-15 11:12:22.980744 django_tableaux-0.2/django_tableaux/apps.py
--rw-r--r--   0        0        0      820 2023-07-15 11:12:22.980744 django_tableaux-0.2/django_tableaux/buttons.py
--rw-r--r--   0        0        0     2557 2023-07-15 11:12:22.981744 django_tableaux-0.2/django_tableaux/columns.py
--rw-r--r--   0        0        0     7282 2023-07-15 11:12:22.982745 django_tableaux-0.2/django_tableaux/static/django_tableaux/js/django_tableaux.js
--rw-r--r--   0        0        0      194 2023-07-15 11:12:22.982745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/_alert.html
--rw-r--r--   0        0        0      717 2023-07-15 11:12:22.983745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/block_content.html
--rw-r--r--   0        0        0      990 2023-07-15 11:12:22.983745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/block_head.html
--rw-r--r--   0        0        0      614 2023-07-15 11:12:22.983745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/block_table.html
--rw-r--r--   0        0        0     3308 2023-07-15 11:12:22.984745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/bootstrap4.html
--rw-r--r--   0        0        0     1103 2023-07-15 11:12:22.984745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/bootstrap5_base.html
--rw-r--r--   0        0        0       86 2023-07-15 11:12:22.984745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/button.html
--rw-r--r--   0        0        0      118 2023-07-15 11:12:22.984745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/cell_error.html
--rw-r--r--   0        0        0      345 2023-07-15 11:12:22.984745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/cell_form.html
--rw-r--r--   0        0        0     1355 2023-07-15 11:12:22.985745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/custom_bootstrap4.html
--rw-r--r--   0        0        0      331 2023-07-15 11:12:22.985745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/filter_settings.html
--rw-r--r--   0        0        0     1005 2023-07-15 11:12:22.985745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/filter_toolbar.html
--rw-r--r--   0        0        0     1348 2023-07-15 11:12:22.985745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/modal_base.html
--rw-r--r--   0        0        0      745 2023-07-15 11:12:22.986745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/modal_filter.html
--rw-r--r--   0        0        0      542 2023-07-15 11:12:22.986745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/modal_form.html
--rw-r--r--   0        0        0     1727 2023-07-15 11:12:22.986745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/paginator.html
--rw-r--r--   0        0        0        0 2023-07-15 11:12:22.986745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/render_row_mobile.html
--rw-r--r--   0        0        0     3103 2023-07-15 11:12:22.987744 django_tableaux-0.2/django_tableaux/templates/django_tableaux/render_rows.html
--rw-r--r--   0        0        0      105 2023-07-15 11:12:22.987744 django_tableaux-0.2/django_tableaux/templates/django_tableaux/render_table_data.html
--rw-r--r--   0        0        0      102 2023-07-15 11:12:22.987744 django_tableaux-0.2/django_tableaux/templates/django_tableaux/select_checkbox.html
--rw-r--r--   0        0        0     1136 2023-07-15 11:12:22.987744 django_tableaux-0.2/django_tableaux/templates/django_tableaux/tables_pro.html
--rw-r--r--   0        0        0     1151 2023-07-15 11:12:22.988745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/toolbar/_actions.html
--rw-r--r--   0        0        0      150 2023-07-15 11:12:22.988745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/toolbar/_buttons.html
--rw-r--r--   0        0        0     1095 2023-07-15 11:12:22.988745 django_tableaux-0.2/django_tableaux/templates/django_tableaux/toolbar/_columns.html
--rw-r--r--   0        0        0      579 2023-07-15 11:12:22.989744 django_tableaux-0.2/django_tableaux/templates/django_tableaux/toolbar/_rows.html
--rw-r--r--   0        0        0      514 2023-07-15 11:12:22.989744 django_tableaux-0.2/django_tableaux/templates/django_tableaux/toolbar/main.html
--rw-r--r--   0        0        0      317 2023-07-15 11:12:22.989744 django_tableaux-0.2/django_tableaux/templates/django_tableaux/width_request.html
--rw-r--r--   0        0        0        0 2023-07-15 11:12:22.989744 django_tableaux-0.2/django_tableaux/templatetags/__init__.py
--rw-r--r--   0        0        0      626 2023-07-15 11:12:22.990745 django_tableaux-0.2/django_tableaux/templatetags/django_tableaux.py
--rw-r--r--   0        0        0     6529 2023-07-15 11:45:29.907566 django_tableaux-0.2/django_tableaux/tests.py
--rw-r--r--   0        0        0     3697 2023-07-15 11:12:22.991745 django_tableaux-0.2/django_tableaux/utils.py
--rw-r--r--   0        0        0    18303 2023-07-15 11:12:22.991745 django_tableaux-0.2/django_tableaux/views.py
--rw-r--r--   0        0        0      414 2023-07-15 17:10:11.497764 django_tableaux-0.2/pyproject.toml
--rw-r--r--   0        0        0      684 2023-07-16 07:29:21.544621 django_tableaux-0.2/tables/manage.py
--rw-r--r--   0        0        0        0 2023-07-16 07:29:20.892757 django_tableaux-0.2/tables/tables/__init__.py
--rw-r--r--   0        0        0      405 2023-07-16 07:29:21.547623 django_tableaux-0.2/tables/tables/asgi.py
--rw-r--r--   0        0        0     3376 2023-07-16 07:29:31.315465 django_tableaux-0.2/tables/tables/settings.py
--rw-r--r--   0        0        0      784 2023-07-16 07:29:21.554622 django_tableaux-0.2/tables/tables/urls.py
--rw-r--r--   0        0        0      405 2023-07-16 07:29:21.554622 django_tableaux-0.2/tables/tables/wsgi.py
--rw-r--r--   0        0        0     1416 1970-01-01 00:00:00.000000 django_tableaux-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1809 2023-07-15 17:35:02.160341 django_tableaux-0.3/.gitignore
+-rw-r--r--   0        0        0     1099 2023-07-15 17:10:11.497764 django_tableaux-0.3/LICENSE
+-rw-r--r--   0        0        0     1177 2023-07-22 11:05:37.932487 django_tableaux-0.3/README.rst
+-rw-r--r--   0        0        0     1170 2023-07-22 11:07:08.948124 django_tableaux-0.3/django_tableaux/__init__.py
+-rw-r--r--   0        0        0      167 2023-07-15 11:12:22.980744 django_tableaux-0.3/django_tableaux/apps.py
+-rw-r--r--   0        0        0      820 2023-07-15 11:12:22.980744 django_tableaux-0.3/django_tableaux/buttons.py
+-rw-r--r--   0        0        0     2557 2023-07-15 11:12:22.981744 django_tableaux-0.3/django_tableaux/columns.py
+-rw-r--r--   0        0        0     7871 2023-07-21 17:57:23.538305 django_tableaux-0.3/django_tableaux/static/django_tableaux/js/django_tableaux.js
+-rw-r--r--   0        0        0      194 2023-07-15 11:12:22.982745 django_tableaux-0.3/django_tableaux/templates/django_tableaux/_alert.html
+-rw-r--r--   0        0        0      761 2023-07-22 07:33:55.960073 django_tableaux-0.3/django_tableaux/templates/django_tableaux/block_content.html
+-rw-r--r--   0        0        0     1120 2023-07-22 07:20:37.370978 django_tableaux-0.3/django_tableaux/templates/django_tableaux/block_head.html
+-rw-r--r--   0        0        0     3079 2023-07-22 07:37:36.360226 django_tableaux-0.3/django_tableaux/templates/django_tableaux/bootstrap4.html
+-rw-r--r--   0        0        0     1103 2023-07-15 11:12:22.984745 django_tableaux-0.3/django_tableaux/templates/django_tableaux/bootstrap5_base.html
+-rw-r--r--   0        0        0       86 2023-07-15 11:12:22.984745 django_tableaux-0.3/django_tableaux/templates/django_tableaux/button.html
+-rw-r--r--   0        0        0      118 2023-07-15 11:12:22.984745 django_tableaux-0.3/django_tableaux/templates/django_tableaux/cell_error.html
+-rw-r--r--   0        0        0      512 2023-07-20 16:48:22.764631 django_tableaux-0.3/django_tableaux/templates/django_tableaux/cell_form.html
+-rw-r--r--   0        0        0     1343 2023-07-21 07:21:05.700143 django_tableaux-0.3/django_tableaux/templates/django_tableaux/custom_bootstrap4.html
+-rw-r--r--   0        0        0      331 2023-07-15 11:12:22.985745 django_tableaux-0.3/django_tableaux/templates/django_tableaux/filter_settings.html
+-rw-r--r--   0        0        0      890 2023-07-19 18:19:28.419384 django_tableaux-0.3/django_tableaux/templates/django_tableaux/filter_toolbar.html
+-rw-r--r--   0        0        0     1348 2023-07-15 11:12:22.985745 django_tableaux-0.3/django_tableaux/templates/django_tableaux/modal_base.html
+-rw-r--r--   0        0        0      745 2023-07-15 11:12:22.986745 django_tableaux-0.3/django_tableaux/templates/django_tableaux/modal_filter.html
+-rw-r--r--   0        0        0      542 2023-07-15 11:12:22.986745 django_tableaux-0.3/django_tableaux/templates/django_tableaux/modal_form.html
+-rw-r--r--   0        0        0     1727 2023-07-15 11:12:22.986745 django_tableaux-0.3/django_tableaux/templates/django_tableaux/paginator.html
+-rw-r--r--   0        0        0     3041 2023-07-20 11:04:24.826254 django_tableaux-0.3/django_tableaux/templates/django_tableaux/render_rows.html
+-rw-r--r--   0        0        0      105 2023-07-15 11:12:22.987744 django_tableaux-0.3/django_tableaux/templates/django_tableaux/render_table_data.html
+-rw-r--r--   0        0        0      102 2023-07-15 11:12:22.987744 django_tableaux-0.3/django_tableaux/templates/django_tableaux/select_checkbox.html
+-rw-r--r--   0        0        0     1427 2023-07-18 16:36:22.512989 django_tableaux-0.3/django_tableaux/templates/django_tableaux/tableaux.html
+-rw-r--r--   0        0        0     1240 2023-07-20 12:33:33.463750 django_tableaux-0.3/django_tableaux/templates/django_tableaux/toolbar/_actions.html
+-rw-r--r--   0        0        0      181 2023-07-18 17:02:14.573795 django_tableaux-0.3/django_tableaux/templates/django_tableaux/toolbar/_buttons.html
+-rw-r--r--   0        0        0     1095 2023-07-15 11:12:22.988745 django_tableaux-0.3/django_tableaux/templates/django_tableaux/toolbar/_columns.html
+-rw-r--r--   0        0        0      607 2023-07-20 06:27:42.647795 django_tableaux-0.3/django_tableaux/templates/django_tableaux/toolbar/_filter_field.html
+-rw-r--r--   0        0        0      336 2023-07-19 16:09:11.116448 django_tableaux-0.3/django_tableaux/templates/django_tableaux/toolbar/_filter_pills.html
+-rw-r--r--   0        0        0      579 2023-07-15 11:12:22.989744 django_tableaux-0.3/django_tableaux/templates/django_tableaux/toolbar/_rows.html
+-rw-r--r--   0        0        0      469 2023-07-19 18:38:33.235037 django_tableaux-0.3/django_tableaux/templates/django_tableaux/toolbar/main.html
+-rw-r--r--   0        0        0      317 2023-07-15 11:12:22.989744 django_tableaux-0.3/django_tableaux/templates/django_tableaux/width_request.html
+-rw-r--r--   0        0        0        0 2023-07-15 11:12:22.989744 django_tableaux-0.3/django_tableaux/templatetags/__init__.py
+-rw-r--r--   0        0        0     1161 2023-07-20 16:25:29.346745 django_tableaux-0.3/django_tableaux/templatetags/django_tableaux.py
+-rw-r--r--   0        0        0     6529 2023-07-15 11:45:29.907566 django_tableaux-0.3/django_tableaux/tests.py
+-rw-r--r--   0        0        0     3697 2023-07-17 18:44:03.199442 django_tableaux-0.3/django_tableaux/utils.py
+-rw-r--r--   0        0        0    19866 2023-07-21 17:37:13.151709 django_tableaux-0.3/django_tableaux/views.py
+-rw-r--r--   0        0        0      414 2023-07-15 17:10:11.497764 django_tableaux-0.3/pyproject.toml
+-rw-r--r--   0        0        0     1462 1970-01-01 00:00:00.000000 django_tableaux-0.3/PKG-INFO
```

### Comparing `django_tableaux-0.2/.gitignore` & `django_tableaux-0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.2/LICENSE` & `django_tableaux-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.2/README.rst` & `django_tableaux-0.3/django_tableaux/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
+"""
+Django tables with Advanced User eXperience
 ===============
-django_tableaux
-===============
-**Django tables with Advanced User eXperience**
-
 This project builds upon two well-established django apps: `django_tables2 <https://github.com/jieter/django-tables2>`_
 and `django_filter <https://github.com/carltongibson/django-filter>`_ and enhances their functionality through a
 sprinkling of `htmx <https://htmx.org>`_ magic. It provides a single class-based view in which you can enable multiple
 features to deliver a customised user experience that embodies the best practice for interactive tables.
 
 Key features
 ============
 * The columns to display can be user-defined
 * Fully responsive: Define different column layouts for mobile, tablet and desktop
 * Bulk actions on selected rows or on all (possibly filtered) rows
 * Infinite scroll
 * Infinite load-more data
 * Position filters in a toolbar, in a modal or embed them within the table header
+* Show active filters with ability to clear individual filters
 * Edit specific fields directly inside the table
 * Easy integration with generic views for CRUD operations
 
 The project is still in beta but is fully usable.
 
-Full documentation to follow.
+Full documentation to follow.
+"""
+__version__ = "0.3"
```

### Comparing `django_tableaux-0.2/django_tableaux/__init__.py` & `django_tableaux-0.3/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-"""
-Django_tableaux: Django tables with Advanced User eXperience
 ===============
+django_tableaux
+===============
+**Django tables with Advanced User eXperience**
+
 This project builds upon two well-established django apps: `django_tables2 <https://github.com/jieter/django-tables2>`_
 and `django_filter <https://github.com/carltongibson/django-filter>`_ and enhances their functionality through a
 sprinkling of `htmx <https://htmx.org>`_ magic. It provides a single class-based view in which you can enable multiple
 features to deliver a customised user experience that embodies the best practice for interactive tables.
 
 Key features
 ============
 * The columns to display can be user-defined
 * Fully responsive: Define different column layouts for mobile, tablet and desktop
 * Bulk actions on selected rows or on all (possibly filtered) rows
 * Infinite scroll
 * Infinite load-more data
 * Position filters in a toolbar, in a modal or embed them within the table header
+* Show active filters with ability to clear individual filters
 * Edit specific fields directly inside the table
 * Easy integration with generic views for CRUD operations
 
 The project is still in beta but is fully usable.
 
-Full documentation to follow.
-"""
-__version__ = "0.2"
+Full documentation to follow.
```

### Comparing `django_tableaux-0.2/django_tableaux/buttons.py` & `django_tableaux-0.3/django_tableaux/buttons.py`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.2/django_tableaux/columns.py` & `django_tableaux-0.3/django_tableaux/columns.py`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.2/django_tableaux/static/django_tableaux/js/django_tableaux.js` & `django_tableaux-0.3/django_tableaux/static/django_tableaux/js/django_tableaux.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,212 +1,231 @@
 // Handle checkboxes in tables, and modal forms
 'use strict';
 let tablesPro = (function() {
-        let tb = {};
-        let lastChecked = null
-        let selAll = null
-        let selAllPage = null
-        tb.init = function() {
-            let url = new URL(window.location.href)
-            const w = url.searchParams.get("_width")
-            if (w !== null) {
-                if (parseInt(w) !== window.outerWidth) {
-                    window.location.href = window.location.href.replace(`_width=${w}`, `_width=${window.outerWidth}`)
-                }
-            }
-            selAll = document.getElementById('select_all')
-            selAllPage = document.getElementById('select_all_page')
-            if (selAllPage) {
-                selAllPage.addEventListener("click", selectAllPage)
-                selectAllPage()
-            }
-            if (selAll) {
-                selAll.addEventListener("click", selectAll)
-                selectAll()
-            }
-
-            // document.getElementById('select_all_page').addEventListener("click", selectAllPage )
-            Array.from(document.getElementsByTagName("table")).forEach(e => e.addEventListener("click", tableClick));
-            Array.from(document.querySelectorAll(".auto-submit")).forEach(e => e.addEventListener("change", function() {
-                document.getElementById("id_filter_form").submit()
-            }));
-
-            Array.from(document.querySelectorAll(".form-group.hx-get")).forEach(e => e.addEventListener("change", filterChanged))
-            countChecked()
-            document.body.addEventListener("trigger", function(evt) {
-                window.htmx.ajax('GET', evt.detail.url, {
-                    source: '#table_data',
-                    'target': '#table_data'
-                });
-            })
-        }
+            let tb = {};
+            let lastChecked = null
+            let selAll = null
+            let selAllPage = null
+            tb.init = function() {
+                let url = new URL(window.location.href)
+                const w = url.searchParams.get("_width")
+                if (w !== null) {
+                    if (parseInt(w) !== window.outerWidth) {
+                        window.location.href = window.location.href.replace(`_width=${w}`, `_width=${window.outerWidth}`)
+                    }
+                }
+                selAll = document.getElementById('select_all')
+                selAllPage = document.getElementById('select_all_page')
+                if (selAllPage) {
+                    selAllPage.addEventListener("click", selectAllPage)
+                    selectAllPage()
+                }
+                if (selAll) {
+                    selAll.addEventListener("click", selectAll)
+                    selectAll()
+                }
+                Array.from(document.querySelectorAll(".select-checkbox")).forEach(e => e.addEventListener("click", chkBoxClick));
+                Array.from(document.querySelectorAll("td")).forEach(e => e.addEventListener("click", tdClick));
+                Array.from(document.querySelectorAll(".auto-submit")).forEach(e => e.addEventListener("change", function() {
+                    document.getElementById("id_filter_form").submit()
+                }));
+                Array.from(document.querySelectorAll(".filter-clear")).forEach(e => e.addEventListener("click", filterClear))
+                Array.from(document.querySelectorAll(".form-group.hx-get")).forEach(e => e.addEventListener("change", filterChanged))
+                document.body.addEventListener("trigger", function(evt) {
+                    window.htmx.ajax('GET', evt.detail.url, {
+                        source: '#table_data',
+                        'target': '#table_data'
+                    });
+                })
+                // When editing a cell inline enter key triggers blur
+                if (document.querySelector(".td_editing")) {
+                    this.addEventListener("keypress", loseFocus)
+                }
+                countChecked()
+            }
 
-        function filterChanged() {
-            window.htmx.ajax('GET', '', {
-                source: '#' + this.lastChild.id,
-                target: '#table_data'
-            });
-        }
+            function loseFocus(e) {
+                if (e.key == "Enter") {
+                    document.activeElement.blur();
+                }
+            }
 
-        function checkBoxes() {
-            return Array.from(document.getElementsByClassName("select-checkbox"))
-        }
+            function filterChanged() {
+                // filter within header changed
+                window.htmx.ajax('GET', '', {
+                    source: '#' + this.firstChild.getAttribute("for"),
+                    target: '#table_data'
+                });
+            }
 
-        function selectAllPage() {
-            // Click on 'Select all on page' highlights all rows
-            if (selAllPage) {
-                let checked = selAllPage.checked
-                if (selAll) {
-                    if (checked) {
-                        selAll.parentElement.style.display = 'block';
-                    } else {
-                        selAll.parentElement.style.display = 'none';
+            function filterClear(e) {
+                let input = window.htmx.closest(e.target, ".input-group").firstChild
+                window.htmx.ajax('GET', '', {
+                    source: input,
+                    target: input
+                });
+            }
+
+            function selectAllPage() {
+                // Click on 'Select all on page' highlights all rows
+                if (selAllPage) {
+                    let checked = selAllPage.checked
+                    if (selAll) {
+                        if (checked) {
+                            selAll.parentElement.style.display = 'block';
+                        } else {
+                            selAll.parentElement.style.display = 'none';
+                        }
                     }
+                    Array.from(document.getElementsByClassName("select-checkbox")).forEach(function(box) {
+                        box.checked = checked
+                        //box.disabled = false;
+                        highlightRow(box)
+                    })
+                    countChecked()
+                    lastChecked = null
+                }
+            }
+
+            function selectAll() {
+                // Click on Select all highlights all rows and disables checkboxes
+                let checked = selAll.checked
+                if (checked) {
+                    document.getElementById('count').innerText = 'All';
+                    if (selAllPage) {
+                        selAllPage.disabled = true
+                    };
+                } else {
+                    if (selAllPage) {
+                        selAllPage.disabled = false
+                    };
+                    //sslAllPage.checked = false;
                 }
                 Array.from(document.getElementsByClassName("select-checkbox")).forEach(function(box) {
-                    box.checked = checked
-                    //box.disabled = false;
-                    highlightRow(box)
+                    box.disabled = checked;
                 })
-                countChecked()
-                lastChecked = null
+                countChecked();
+                lastChecked = null;
             }
-        }
 
-        function selectAll() {
-            // Click on Select all highlights all rows and disables checkboxes
-            let checked = selAll.checked
-            if (checked) {
-                document.getElementById('count').innerText = 'All';
-                if (selAllPage) {
-                    selAllPage.disabled = true
-                };
-            } else {
+            function chkBoxClick(e) {
+                // Click on row's select checkbox - handle using shift to select multiple rows
                 if (selAllPage) {
-                    selAllPage.disabled = false
-                };
-                //sslAllPage.checked = false;
-            }
-            Array.from(document.getElementsByClassName("select-checkbox")).forEach(function(box) {
-                box.disabled = checked;
-            })
-            countChecked();
-            lastChecked = null;
-        }
+                    selAllPage.checked = false
+                }
+                let chkBox = e.target
+                highlightRow(chkBox)
+                if (!lastChecked) {
+                    lastChecked = chkBox
+                } else if (e.shiftKey) {
+                    let chkBoxes = Array.from(document.getElementsByClassName("select-checkbox"))
+                    let start = chkBoxes.indexOf(chkBox)
+                    let end = chkBoxes.indexOf(lastChecked)
+                    chkBoxes.slice(Math.min(start, end), Math.max(start, end) + 1).forEach(function(box) {
+                        box.checked = chkBox.checked;
+                    });
+                    lastChecked = chkBox;
+                } else {
+                    lastChecked = chkBox;
+                }
+                countChecked();
+            }
 
-        function tableClick(e) {
-            // ignore clicks in td holding select checkbox
-            if (e.target.innerHTML.search('select-checkbox') < 0) {
-                if (e.target.name === 'select-checkbox') {
-                    // Click on row's select checkbox - handle using shift to select multiple rows
-                    if (selAllPage) {
-                        selAllPage.checked = false
+            function tdClick(e) {
+                let editing = document.getElementsByClassName("td-editing");
+                if (editing.length > 0) {
+                    if (e.target === editing[0]) {
+                        return
                     }
-                    let chkBox = e.target
-                    highlightRow(chkBox)
-                    if (!lastChecked) {
-                        lastChecked = chkBox
-                    } else if (e.shiftKey) {
-                        let chkBoxes = checkBoxes()
-                        let start = chkBoxes.indexOf(chkBox)
-                        let end = chkBoxes.indexOf(lastChecked)
-                        chkBoxes.slice(Math.min(start, end), Math.max(start, end) + 1).forEach(function(box) {
-                            box.checked = chkBox.checked;
-                        });
-                        lastChecked = chkBox;
-                    } else {
-                        lastChecked = chkBox;
+                    // click on a cell when editing another causes Put
+                    let el = editing[0].parentNode
+                    window.htmx.ajax('PUT', "", {
+                        source: "#" + el.id,
+                        target: "#" + el.id,
+                        values: window.htmx.closest(el, 'tr')
+                    })
+                } else {
+                    let row = e.target.parentNode;
+                    let pk = row.id.slice(3);
+                    let table = row.parentNode.parentNode;
+                    let col = 0;
+                    let previous = e.target.previousElementSibling;
+                    while (previous) {
+                        previous = previous.previousElementSibling;
+                        col += 1;
                     }
-                    countChecked();
-
-                } else if (e.target.tagName === 'TD') {
-                    let editing = document.getElementsByClassName("td_editing");
-                    if (editing.length > 0) {
-                        // click on a cell when editing another causes put
-                        let el = editing[0].parentNode
-                        window.htmx.ajax('PUT', "", {
-                            source: "#" + el.id,
-                            target: "#" + el.id,
-                            values: window.htmx.closest(el, 'tr')
-                        })
-                    } else {
-                        let row = e.target.parentNode;
-                        let pk = row.id.slice(3);
-                        let table = row.parentNode.parentNode;
-                        let col = 0;
-                        let previous = e.target.previousElementSibling;
-                        while (previous) {
-                            previous = previous.previousElementSibling;
-                            col += 1;
+                    let idSuffix = "_" + pk + "_" + col + "_" + window.outerWidth;
+                    if (e.target.classList.contains("td-edit")) {
+                        // fetch template for editable cell
+                        e.target.setAttribute("id", "cell" + idSuffix);
+                        window.htmx.ajax('GET', "", {
+                            source: '#cell' + idSuffix,
+                            target: '#cell' + idSuffix
+                        });
+                    } else if (table.dataset.url) {
+                        let url = table.dataset.url;
+                        if (table.dataset.pk) {
+                            url += pk;
                         }
-                        let tdId = ("td" + "_" + pk + "_" + col + "_" + window.outerWidth);
-                        if (e.target.classList.contains("td_edit")) {
-                            // fetch template for editable cell
-                            e.target.setAttribute("id", tdId);
-                            window.htmx.ajax('GET', "", {
-                                source: '#' + tdId,
-                                target: '#' + tdId
-                            });
-                        } else if (table.dataset.url) {
-                            let url = table.dataset.url;
-                            if (table.dataset.pk) {
-                                url += pk;
-                            }
-                            //url += "?return=" +encodeURIComponent(window.location.pathname + window.location.search)
-                            if (table.dataset.method === "get") {
-                                window.document.location.assign(url)
-                            } else if (table.dataset.method === "hxget") {
-                                window.htmx.ajax('GET', url, {
-                                    source: '#' + row.id,
-                                    target: table.dataset.target
-                                });
-                            }
-                        } else {
-                            window.htmx.ajax('GET', "", {
+                        //url += "?return=" +encodeURIComponent(window.location.pathname + window.location.search)
+                        if (table.dataset.click === "ClickAction.GET") {
+                            window.document.location.assign(url)
+                        } else if (table.dataset.click === "ClickAction.HX_GET") {
+                            window.htmx.ajax('GET', url, {
                                 source: '#' + row.id,
-                                target: '#' + row.id,
-                                values: {
-                                    col: col,
-                                    width: window.outerWidth
-                                }
+                                target: table.dataset.target
                             });
                         }
+                    } else if (table.dataset.click === "ClickAction.CUSTOM") {
+                        e.target.setAttribute("id", "td" + idSuffix);
+                        window.htmx.ajax('GET', "", {
+                            source: '#td' + idSuffix,
+                            target: '#td' + idSuffix,
+                        });
                     }
                 }
             }
-        }
 
-        function highlightRow(box) {
-            let row = box.parentElement.parentElement;
-            let cls = (("selected" in row.dataset) ? row.dataset.selected : "table-active");
-            if (box.checked) {
-                row.classList.add(cls)
-            } else {
-                row.classList.remove(cls)
+            function highlightRow(box) {
+                let row = box.parentElement.parentElement;
+                let cls = (("selected" in row.dataset) ? row.dataset.selected : "table-active");
+                if (box.checked) {
+                    row.classList.add(cls)
+                } else {
+                    row.classList.remove(cls)
+                }
             }
-        }
 
-        // Count the number of checked rows and nake sure they are highlighted
-        function countChecked() {
-            if (selAll && selAll.checked) {
-                return
-            }
-            let checked = Array.from(document.querySelectorAll(".select-checkbox:checked"));
-            checked.forEach(function(e) {
-                let row = e.parentElement.parentElement
-                row.classList.add((("selected" in row.dataset) ? row.dataset.selected : "table-active"))
-            });
-            let count = checked.length;
-            let countField = document.getElementById('count');
-            if (countField) {
-                countField.innerText = count.toString();
-            }
-            let actionMenu = document.getElementById('selectActionMenu');
-            if (actionMenu) {
-                actionMenu.disabled = (count === 0);
-                actionMenu.enabled = (count > 0 || selAll.checked);
+            // Count the number of checked rows and nake sure they are highlighted
+            function countChecked() {
+                if (selAll && selAll.checked) {
+                    return
+                }
+                let checked = Array.from(document.querySelectorAll(".select-checkbox:checked"));
+                let ids = []
+                checked.forEach(function(el) {
+                    let row = el.parentElement.parentElement
+                    row.classList.add((("selected" in row.dataset) ? row.dataset.selected : "table-active"))
+                    ids.push(el.value)
+                });
+                let hiddenInput = document.querySelector("input[name='selected_ids']")
+                if (hiddenInput) {
+                    hiddenInput.value = ids.toString();
+                }
+                let count = checked.length;
+                let countField = document.getElementById('count');
+                if (countField) {
+                    countField.innerText = count.toString();
+                }
+                let actionMenu = document.getElementById('selectActionMenu');
+                if (actionMenu) {
+                    actionMenu.disabled = (count === 0);
+                    actionMenu.enabled = (count > 0 || selAll.checked);
+                }
             }
+
+            return tb
         }
-        return tb
-    })
+
+    )
     ();
 window.addEventListener("load", tablesPro.init)
```

### Comparing `django_tableaux-0.2/django_tableaux/templates/django_tableaux/block_content.html` & `django_tableaux-0.3/django_tableaux/templates/django_tableaux/block_content.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 {% load static django_tableaux %}
 <div id="block_content">
   {% if view.filterset_class and view.filter_style == 1 %}
     <div class="{{ css_toolbar }}">
       {% include "django_tableaux/filter_toolbar.html" %}
     </div>
   {% endif %}
-  <form hx-post="" hx-target="#modals-here">
-    {% csrf_token %}
-    {% if actions or buttons or table.column_states or view.filterset_class and view.filter_modal %}
-      <div class="{{ css_toolbar }}">
-        {% include "django_tableaux/toolbar/main.html" %}
-      </div>
-    {% endif %}
-    <div id="table_data" class="{{ css_table }}">
-      {% include "django_tableaux/render_table_data.html" %}
+  {% if filters %}
+    <div class="d-flex">
+      {% include "django_tableaux/toolbar/_filter_pills.html" %}
     </div>
-  </form>
+  {% endif %}
+  {% if actions or buttons or table.column_states or view.filterset_class and view.filter_modal %}
+    <div class="{{ css_toolbar }}">
+      {% include "django_tableaux/toolbar/main.html" %}
+    </div>
+  {% endif %}
+  <div id="table_data" class="{{ css_table }}">
+    {% include "django_tableaux/render_table_data.html" %}
+  </div>
   <div id="modals-here"></div>
 </div>
```

### Comparing `django_tableaux-0.2/django_tableaux/templates/django_tableaux/bootstrap4.html` & `django_tableaux-0.3/django_tableaux/templates/django_tableaux/render_rows.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,207 +1,191 @@
 00000000: 7b25 206c 6f61 6420 646a 616e 676f 5f74  {% load django_t
-00000010: 6162 6c65 7332 2062 6f6f 7473 7472 6170  ables2 bootstrap
-00000020: 3420 257d 0d0a 7b25 206c 6f61 6420 6931  4 %}..{% load i1
-00000030: 386e 2025 7d0d 0a7b 2520 626c 6f63 6b20  8n %}..{% block 
-00000040: 7461 626c 652d 7772 6170 7065 7220 257d  table-wrapper %}
-00000050: 0d0a 2020 3c64 6976 2063 6c61 7373 3d22  ..  <div class="
-00000060: 7461 626c 652d 636f 6e74 6169 6e65 7222  table-container"
-00000070: 3e0d 0a20 2020 207b 2520 626c 6f63 6b20  >..    {% block 
-00000080: 7461 626c 6520 257d 0d0a 2020 2020 2020  table %}..      
-00000090: 3c74 6162 6c65 207b 2520 7265 6e64 6572  <table {% render
-000000a0: 5f61 7474 7273 2074 6162 6c65 2e61 7474  _attrs table.att
-000000b0: 7273 2063 6c61 7373 3d22 7461 626c 6522  rs class="table"
-000000c0: 2025 7d0d 0a20 2020 2020 2020 2020 207b   %}..          {
-000000d0: 2320 6164 6420 7461 626c 6520 6461 7461  # add table data
-000000e0: 237d 0d0a 2020 2020 2020 2020 2020 6461  #}..          da
-000000f0: 7461 2d6d 6574 686f 643d 227b 7b20 7461  ta-method="{{ ta
-00000100: 626c 652e 6d65 7468 6f64 207d 7d22 2064  ble.method }}" d
-00000110: 6174 612d 7572 6c3d 227b 7b20 7461 626c  ata-url="{{ tabl
-00000120: 652e 7572 6c20 7d7d 220d 0a20 2020 2020  e.url }}"..     
-00000130: 2020 2020 2064 6174 612d 706b 3d7b 7b20       data-pk={{ 
-00000140: 7461 626c 652e 706b 207d 7d20 6461 7461  table.pk }} data
-00000150: 2d74 6172 6765 743d 227b 7b20 7461 626c  -target="{{ tabl
-00000160: 652e 7461 7267 6574 207d 7d22 3e0d 0a20  e.target }}">.. 
-00000170: 2020 2020 2020 207b 2520 626c 6f63 6b20         {% block 
-00000180: 7461 626c 652e 7468 6561 6420 257d 0d0a  table.thead %}..
-00000190: 2020 2020 2020 2020 2020 7b25 2069 6620            {% if 
-000001a0: 7461 626c 652e 7368 6f77 5f68 6561 6465  table.show_heade
-000001b0: 7220 257d 0d0a 2020 2020 2020 2020 2020  r %}..          
-000001c0: 2020 7b23 2020 736f 7274 2061 7474 7269    {#  sort attri
-000001d0: 6275 7465 7320 616e 6420 6669 6c74 6572  butes and filter
-000001e0: 2072 6f77 2023 7d0d 0a20 2020 2020 2020   row #}..       
-000001f0: 2020 2020 203c 7468 6561 6420 7b7b 2074       <thead {{ t
-00000200: 6162 6c65 2e61 7474 7273 2e74 6865 6164  able.attrs.thead
-00000210: 2e61 735f 6874 6d6c 207d 7d20 7374 796c  .as_html }} styl
-00000220: 653d 226d 6172 6769 6e3a 2030 7078 223e  e="margin: 0px">
-00000230: 0d0a 2020 2020 2020 2020 2020 2020 3c74  ..            <t
-00000240: 7220 636c 6173 733d 2262 672d 7768 6974  r class="bg-whit
-00000250: 6522 3e0d 0a20 2020 2020 2020 2020 2020  e">..           
-00000260: 2020 207b 2520 666f 7220 636f 6c75 6d6e     {% for column
-00000270: 2069 6e20 7461 626c 652e 636f 6c75 6d6e   in table.column
-00000280: 7320 257d 0d0a 2020 2020 2020 2020 2020  s %}..          
-00000290: 2020 2020 2020 7b25 2069 6620 636f 6c75        {% if colu
-000002a0: 6d6e 2e6e 616d 6520 696e 2074 6162 6c65  mn.name in table
-000002b0: 2e63 6f6c 756d 6e73 5f76 6973 6962 6c65  .columns_visible
-000002c0: 2025 7d0d 0a20 2020 2020 2020 2020 2020   %}..           
-000002d0: 2020 2020 2020 203c 7468 207b 7b20 636f         <th {{ co
-000002e0: 6c75 6d6e 2e61 7474 7273 2e74 682e 6173  lumn.attrs.th.as
-000002f0: 5f68 746d 6c20 7d7d 2073 7479 6c65 3d22  _html }} style="
-00000300: 6d61 7267 696e 3a20 3070 7822 3e0d 0a20  margin: 0px">.. 
-00000310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000320: 2020 207b 2520 6966 2063 6f6c 756d 6e2e     {% if column.
-00000330: 6e61 6d65 203d 3d20 2273 656c 6563 7469  name == "selecti
-00000340: 6f6e 2220 257d 0d0a 2020 2020 2020 2020  on" %}..        
-00000350: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
-00000360: 6e70 7574 2074 7970 653d 2263 6865 636b  nput type="check
-00000370: 626f 7822 2069 643d 2273 656c 6563 745f  box" id="select_
-00000380: 616c 6c5f 7061 6765 2220 6e61 6d65 3d22  all_page" name="
-00000390: 7365 6c65 6374 5f61 6c6c 5f70 6167 6522  select_all_page"
-000003a0: 2063 6c61 7373 3d22 6d6c 2d32 223e 0d0a   class="ml-2">..
-000003b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003c0: 2020 2020 7b25 2065 6c73 6520 257d 0d0a      {% else %}..
-000003d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003e0: 2020 2020 2020 7b25 2069 6620 636f 6c75        {% if colu
-000003f0: 6d6e 2e6f 7264 6572 6162 6c65 2025 7d0d  mn.orderable %}.
-00000400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000410: 2020 2020 2020 2020 203c 6120 6872 6566           <a href
-00000420: 3d22 7b25 2071 7565 7279 7374 7269 6e67  ="{% querystring
-00000430: 2074 6162 6c65 2e70 7265 6669 7865 645f   table.prefixed_
-00000440: 6f72 6465 725f 6279 5f66 6965 6c64 3d63  order_by_field=c
-00000450: 6f6c 756d 6e2e 6f72 6465 725f 6279 5f61  olumn.order_by_a
-00000460: 6c69 6173 2e6e 6578 7420 257d 223e 0d0a  lias.next %}">..
-00000470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000480: 2020 2020 2020 2020 2020 7b23 2020 2020            {#    
-00000490: 2020 2020 2020 2020 3c73 7061 6e20 636c          <span cl
-000004a0: 6173 733d 2266 6c6f 6174 2d72 6967 6874  ass="float-right
-000004b0: 2074 6578 742d 7768 6974 6522 3e7b 2520   text-white">{% 
-000004c0: 6966 2022 2d22 2069 6e20 636f 6c75 6d6e  if "-" in column
-000004d0: 2e6f 7264 6572 5f62 792e 3020 257d 2623  .order_by.0 %}&#
-000004e0: 3936 3531 3b7b 2520 656c 7365 2025 7d26  9651;{% else %}&
-000004f0: 2339 3636 313b 7b25 2065 6e64 6966 2025  #9661;{% endif %
-00000500: 7d3c 2f73 7061 6e3e 237d 0d0a 2020 2020  }</span>#}..    
-00000510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000520: 2020 2020 2020 7b7b 2063 6f6c 756d 6e2e        {{ column.
-00000530: 6865 6164 6572 207d 7d0d 0a20 2020 2020  header }}..     
-00000540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000550: 2020 203c 2f61 3e0d 0a20 2020 2020 2020     </a>..       
-00000560: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00000570: 2520 656c 7365 2025 7d0d 0a20 2020 2020  % else %}..     
-00000580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000590: 2020 207b 7b20 636f 6c75 6d6e 2e68 6561     {{ column.hea
-000005a0: 6465 7220 7d7d 0d0a 2020 2020 2020 2020  der }}..        
-000005b0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-000005c0: 2065 6e64 6966 2025 7d0d 0a20 2020 2020   endif %}..     
-000005d0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000005e0: 2520 656e 6469 6620 257d 0d0a 2020 2020  % endif %}..    
-000005f0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00000600: 7468 3e0d 0a20 2020 2020 2020 2020 2020  th>..           
-00000610: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
-00000620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000630: 7b25 2065 6e64 666f 7220 257d 0d0a 2020  {% endfor %}..  
-00000640: 2020 2020 2020 2020 2020 3c2f 7472 3e0d            </tr>.
-00000650: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
-00000660: 6966 2074 6162 6c65 2e66 696c 7465 722e  if table.filter.
-00000670: 7374 796c 6520 3d3d 2074 6162 6c65 2e66  style == table.f
-00000680: 696c 7465 722e 7374 796c 652e 4845 4144  ilter.style.HEAD
-00000690: 4552 2025 7d0d 0a20 2020 2020 2020 2020  ER %}..         
-000006a0: 2020 2020 203c 7472 2063 6c61 7373 3d22       <tr class="
-000006b0: 6267 2d6c 6967 6874 223e 0d0a 2020 2020  bg-light">..    
-000006c0: 2020 2020 2020 2020 2020 2020 7b25 2066              {% f
-000006d0: 6f72 2066 6965 6c64 2069 6e20 7461 626c  or field in tabl
-000006e0: 652e 6865 6164 6572 5f66 6965 6c64 7320  e.header_fields 
-000006f0: 257d 0d0a 2020 2020 2020 2020 2020 2020  %}..            
-00000700: 2020 2020 2020 3c74 683e 0d0a 2020 2020        <th>..    
-00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000720: 7b25 2069 6620 6669 656c 6420 257d 0d0a  {% if field %}..
-00000730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000740: 2020 2020 2020 7b25 2062 6f6f 7473 7472        {% bootstr
-00000750: 6170 5f66 6965 6c64 2066 6965 6c64 2073  ap_field field s
-00000760: 686f 775f 6c61 6265 6c3d 4661 6c73 6520  how_label=False 
-00000770: 666f 726d 5f67 726f 7570 5f63 6c61 7373  form_group_class
-00000780: 3d22 666f 726d 2d67 726f 7570 2068 782d  ="form-group hx-
-00000790: 6765 7420 6d2d 3020 702d 3022 2025 7d0d  get m-0 p-0" %}.
-000007a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000007b0: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
-000007c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000007d0: 2020 2020 3c2f 7468 3e0d 0a20 2020 2020      </th>..     
-000007e0: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
-000007f0: 6466 6f72 2025 7d0d 0a20 2020 2020 2020  dfor %}..       
-00000800: 2020 2020 2020 203c 2f74 723e 0d0a 2020         </tr>..  
-00000810: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-00000820: 6966 2025 7d0d 0a20 2020 2020 2020 2020  if %}..         
-00000830: 2020 203c 2f74 6865 6164 3e0d 0a20 2020     </thead>..   
-00000840: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
-00000850: 257d 0d0a 2020 2020 2020 2020 7b25 2065  %}..        {% e
-00000860: 6e64 626c 6f63 6b20 7461 626c 652e 7468  ndblock table.th
-00000870: 6561 6420 257d 0d0a 2020 2020 2020 2020  ead %}..        
-00000880: 7b25 2062 6c6f 636b 2074 6162 6c65 2e74  {% block table.t
-00000890: 626f 6479 2025 7d0d 0a20 2020 2020 2020  body %}..       
-000008a0: 2020 203c 7462 6f64 7920 7b7b 2074 6162     <tbody {{ tab
-000008b0: 6c65 2e61 7474 7273 2e74 626f 6479 2e61  le.attrs.tbody.a
-000008c0: 735f 6874 6d6c 207d 7d3e 0d0a 2020 2020  s_html }}>..    
-000008d0: 2020 2020 2020 7b25 2069 6e63 6c75 6465        {% include
-000008e0: 2022 646a 616e 676f 5f74 6162 6c65 6175   "django_tableau
-000008f0: 782f 7265 6e64 6572 5f72 6f77 732e 6874  x/render_rows.ht
-00000900: 6d6c 2220 257d 0d0a 2020 2020 2020 2020  ml" %}..        
-00000910: 2020 3c2f 7462 6f64 793e 0d0a 2020 2020    </tbody>..    
-00000920: 2020 2020 7b25 2065 6e64 626c 6f63 6b20      {% endblock 
-00000930: 7461 626c 652e 7462 6f64 7920 257d 0d0a  table.tbody %}..
-00000940: 2020 2020 2020 2020 7b25 2062 6c6f 636b          {% block
-00000950: 2074 6162 6c65 2e74 666f 6f74 2025 7d0d   table.tfoot %}.
-00000960: 0a20 2020 2020 2020 2020 207b 2520 6966  .          {% if
-00000970: 2074 6162 6c65 2e68 6173 5f66 6f6f 7465   table.has_foote
-00000980: 7220 257d 0d0a 2020 2020 2020 2020 2020  r %}..          
-00000990: 2020 3c74 666f 6f74 207b 7b20 7461 626c    <tfoot {{ tabl
-000009a0: 652e 6174 7472 732e 7466 6f6f 742e 6173  e.attrs.tfoot.as
-000009b0: 5f68 746d 6c20 7d7d 3e0d 0a20 2020 2020  _html }}>..     
-000009c0: 2020 2020 2020 203c 7472 3e0d 0a20 2020         <tr>..   
-000009d0: 2020 2020 2020 2020 2020 207b 2520 666f             {% fo
-000009e0: 7220 636f 6c75 6d6e 2069 6e20 7461 626c  r column in tabl
-000009f0: 652e 636f 6c75 6d6e 7320 257d 0d0a 2020  e.columns %}..  
-00000a00: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00000a10: 2069 6620 636f 6c75 6d6e 2e6e 616d 6520   if column.name 
-00000a20: 696e 2074 6162 6c65 2e63 6f6c 756d 6e73  in table.columns
-00000a30: 5f76 6973 6962 6c65 2025 7d0d 0a20 2020  _visible %}..   
-00000a40: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000a50: 7464 207b 7b20 636f 6c75 6d6e 2e61 7474  td {{ column.att
-00000a60: 7273 2e74 662e 6173 5f68 746d 6c20 7d7d  rs.tf.as_html }}
-00000a70: 3e7b 7b20 636f 6c75 6d6e 2e66 6f6f 7465  >{{ column.foote
-00000a80: 7220 7d7d 3c2f 7464 3e0d 0a20 2020 2020  r }}</td>..     
-00000a90: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
-00000aa0: 6469 6620 257d 0d0a 2020 2020 2020 2020  dif %}..        
-00000ab0: 2020 2020 2020 7b25 2065 6e64 666f 7220        {% endfor 
-00000ac0: 257d 0d0a 2020 2020 2020 2020 2020 2020  %}..            
-00000ad0: 3c2f 7472 3e0d 0a20 2020 2020 2020 2020  </tr>..         
-00000ae0: 2020 203c 2f74 666f 6f74 3e0d 0a20 2020     </tfoot>..   
-00000af0: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
-00000b00: 257d 0d0a 2020 2020 2020 2020 7b25 2065  %}..        {% e
-00000b10: 6e64 626c 6f63 6b20 7461 626c 652e 7466  ndblock table.tf
-00000b20: 6f6f 7420 257d 0d0a 2020 2020 2020 3c2f  oot %}..      </
-00000b30: 7461 626c 653e 0d0a 2020 2020 7b25 2065  table>..    {% e
-00000b40: 6e64 626c 6f63 6b20 7461 626c 6520 257d  ndblock table %}
-00000b50: 0d0a 2020 2020 7b25 2062 6c6f 636b 2070  ..    {% block p
-00000b60: 6167 696e 6174 696f 6e20 257d 0d0a 2020  agination %}..  
-00000b70: 2020 2020 7b25 2069 6620 6e6f 7420 7461      {% if not ta
-00000b80: 626c 652e 696e 6669 6e69 7465 5f73 6372  ble.infinite_scr
-00000b90: 6f6c 6c20 616e 6420 6e6f 7420 7461 626c  oll and not tabl
-00000ba0: 652e 696e 6669 6e69 7465 5f6c 6f61 6420  e.infinite_load 
-00000bb0: 257d 0d0a 2020 2020 2020 2020 7b25 2069  %}..        {% i
-00000bc0: 6e63 6c75 6465 2022 646a 616e 676f 5f74  nclude "django_t
-00000bd0: 6162 6c65 6175 782f 7061 6769 6e61 746f  ableaux/paginato
-00000be0: 722e 6874 6d6c 2220 257d 0d0a 2020 2020  r.html" %}..    
-00000bf0: 2020 7b25 2065 6e64 6966 2025 7d0d 0a20    {% endif %}.. 
-00000c00: 2020 207b 2520 656e 6462 6c6f 636b 2070     {% endblock p
-00000c10: 6167 696e 6174 696f 6e20 257d 0d0a 2020  agination %}..  
-00000c20: 3c2f 6469 763e 0d0a 2020 3c64 6976 2069  </div>..  <div i
-00000c30: 643d 2266 6965 6c64 2220 6172 6961 2d64  d="field" aria-d
-00000c40: 6573 6372 6962 6564 6279 3d22 746f 6f6c  escribedby="tool
-00000c50: 7469 7022 3e3c 2f64 6976 3e0d 0a20 203c  tip"></div>..  <
-00000c60: 6469 7620 6964 3d22 746f 6f6c 7469 7022  div id="tooltip"
-00000c70: 2072 6f6c 653d 2274 6f6f 6c74 6970 223e   role="tooltip">
-00000c80: 0d0a 2020 2020 4572 726f 7220 696e 2066  ..    Error in f
-00000c90: 6965 6c64 0d0a 2020 2020 3c64 6976 2069  ield..    <div i
-00000ca0: 643d 2261 7272 6f77 2220 6461 7461 2d70  d="arrow" data-p
-00000cb0: 6f70 7065 722d 6172 726f 773e 3c2f 6469  opper-arrow></di
-00000cc0: 763e 0d0a 2020 3c2f 6469 763e 0d0a 7b25  v>..  </div>..{%
-00000cd0: 2065 6e64 626c 6f63 6b20 7461 626c 652d   endblock table-
-00000ce0: 7772 6170 7065 7220 257d 0d0a            wrapper %}..
+00000010: 6162 6c65 7332 2064 6a61 6e67 6f5f 7461  ables2 django_ta
+00000020: 626c 6561 7578 2025 7d0d 0a7b 2520 6c6f  bleaux %}..{% lo
+00000030: 6164 2069 3138 6e20 257d 0d0a 7b25 2066  ad i18n %}..{% f
+00000040: 6f72 2072 6f77 2069 6e20 7461 626c 652e  or row in table.
+00000050: 7061 6769 6e61 7465 645f 726f 7773 2025  paginated_rows %
+00000060: 7d0d 0a20 207b 2520 626c 6f63 6b20 7461  }..  {% block ta
+00000070: 626c 652e 7462 6f64 792e 726f 7720 257d  ble.tbody.row %}
+00000080: 0d0a 2020 2020 7b25 2069 6620 666f 726c  ..    {% if forl
+00000090: 6f6f 702e 6c61 7374 2061 6e64 2074 6162  oop.last and tab
+000000a0: 6c65 2e69 6e66 696e 6974 655f 7363 726f  le.infinite_scro
+000000b0: 6c6c 2061 6e64 2074 6162 6c65 2e70 6167  ll and table.pag
+000000c0: 652e 6e75 6d62 6572 203c 2074 6162 6c65  e.number < table
+000000d0: 2e70 6167 652e 7061 6769 6e61 746f 722e  .page.paginator.
+000000e0: 6e75 6d5f 7061 6765 7320 257d 0d0a 2020  num_pages %}..  
+000000f0: 2020 2020 3c74 7220 7b7b 2072 6f77 2e61      <tr {{ row.a
+00000100: 7474 7273 2e61 735f 6874 6d6c 207d 7d20  ttrs.as_html }} 
+00000110: 6964 3d22 7472 5f7b 7b20 726f 772e 7265  id="tr_{{ row.re
+00000120: 636f 7264 2e69 6420 7d7d 220d 0a20 2020  cord.id }}"..   
+00000130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000140: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+00000150: 782d 6765 743d 227b 2520 7175 6572 7973  x-get="{% querys
+00000160: 7472 696e 6720 7461 626c 652e 7072 6566  tring table.pref
+00000170: 6978 6564 5f70 6167 655f 6669 656c 643d  ixed_page_field=
+00000180: 7461 626c 652e 7061 6765 2e6e 6578 745f  table.page.next_
+00000190: 7061 6765 5f6e 756d 6265 7220 7769 7468  page_number with
+000001a0: 6f75 7420 225f 7363 726f 6c6c 2220 257d  out "_scroll" %}
+000001b0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+000001c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001d0: 2020 2020 2068 782d 7461 7267 6574 3d22       hx-target="
+000001e0: 2374 725f 7b7b 2072 6f77 2e72 6563 6f72  #tr_{{ row.recor
+000001f0: 642e 6964 207d 7d22 0d0a 2020 2020 2020  d.id }}"..      
+00000200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000210: 2020 2020 2020 2020 2020 2020 6878 2d74              hx-t
+00000220: 7269 6767 6572 3d22 696e 7465 7273 6563  rigger="intersec
+00000230: 7420 6f6e 6365 2220 6878 2d73 7761 703d  t once" hx-swap=
+00000240: 2261 6674 6572 656e 6422 2068 782d 7661  "afterend" hx-va
+00000250: 6c73 3d27 7b22 5f73 6372 6f6c 6c22 3a20  ls='{"_scroll": 
+00000260: 2274 7275 6522 7d27 3e0d 0a20 2020 2020  "true"}'>..     
+00000270: 2020 207b 2520 656c 7365 2025 7d0d 0a20     {% else %}.. 
+00000280: 2020 2020 203c 7472 207b 7b20 726f 772e       <tr {{ row.
+00000290: 6174 7472 732e 6173 5f68 746d 6c20 7d7d  attrs.as_html }}
+000002a0: 2069 643d 2274 725f 7b7b 2072 6f77 2e72   id="tr_{{ row.r
+000002b0: 6563 6f72 642e 6964 207d 7d22 3e0d 0a20  ecord.id }}">.. 
+000002c0: 2020 207b 2520 656e 6469 6620 257d 0d0a     {% endif %}..
+000002d0: 2020 7b25 2066 6f72 2063 6f6c 756d 6e2c    {% for column,
+000002e0: 2063 656c 6c20 696e 2072 6f77 2e69 7465   cell in row.ite
+000002f0: 6d73 2025 7d0d 0a20 2020 207b 2520 6966  ms %}..    {% if
+00000300: 2063 6f6c 756d 6e2e 6e61 6d65 2069 6e20   column.name in 
+00000310: 7461 626c 652e 636f 6c75 6d6e 735f 7669  table.columns_vi
+00000320: 7369 626c 6520 257d 0d0a 2020 2020 2020  sible %}..      
+00000330: 3c74 6420 7b7b 2063 6f6c 756d 6e7c 7464  <td {{ column|td
+00000340: 5f61 7474 723a 7461 626c 6520 7d7d 3e0d  _attr:table }}>.
+00000350: 0a20 2020 2020 2020 207b 2520 6966 2063  .        {% if c
+00000360: 6f6c 756d 6e2e 6c6f 6361 6c69 7a65 203d  olumn.localize =
+00000370: 3d20 4e6f 6e65 2025 7d7b 7b20 6365 6c6c  = None %}{{ cell
+00000380: 207d 7d7b 2520 656c 7365 2025 7d7b 2520   }}{% else %}{% 
+00000390: 6966 2063 6f6c 756d 6e2e 6c6f 6361 6c69  if column.locali
+000003a0: 7a65 2025 7d7b 7b20 6365 6c6c 7c6c 6f63  ze %}{{ cell|loc
+000003b0: 616c 697a 6520 7d7d 0d0a 2020 2020 2020  alize }}..      
+000003c0: 2020 7b25 2065 6c73 6520 257d 0d0a 2020    {% else %}..  
+000003d0: 2020 2020 2020 2020 7b7b 2063 656c 6c7c          {{ cell|
+000003e0: 756e 6c6f 6361 6c69 7a65 207d 7d7b 2520  unlocalize }}{% 
+000003f0: 656e 6469 6620 257d 0d0a 2020 2020 2020  endif %}..      
+00000400: 2020 7b25 2065 6e64 6966 2025 7d0d 0a20    {% endif %}.. 
+00000410: 2020 2020 203c 2f74 643e 0d0a 2020 2020       </td>..    
+00000420: 7b25 2065 6e64 6966 2025 7d0d 0a20 207b  {% endif %}..  {
+00000430: 2520 656e 6466 6f72 2025 7d0d 0a20 203c  % endfor %}..  <
+00000440: 2f74 723e 0d0a 2020 2020 7b25 2069 6620  /tr>..    {% if 
+00000450: 7461 626c 652e 6d6f 6269 6c65 2025 7d0d  table.mobile %}.
+00000460: 0a20 2020 2020 207b 2520 666f 7220 636f  .      {% for co
+00000470: 6c75 6d6e 2c20 6365 6c6c 2069 6e20 726f  lumn, cell in ro
+00000480: 772e 6974 656d 7320 257d 0d0a 2020 2020  w.items %}..    
+00000490: 2020 2020 7b25 2069 6620 636f 6c75 6d6e      {% if column
+000004a0: 2e6e 616d 6520 696e 2074 6162 6c65 2e63  .name in table.c
+000004b0: 6f6c 756d 6e73 5f6f 7074 696f 6e61 6c20  olumns_optional 
+000004c0: 257d 0d0a 2020 2020 2020 2020 2020 3c74  %}..          <t
+000004d0: 723e 0d0a 2020 2020 2020 2020 2020 2020  r>..            
+000004e0: 3c74 6420 7374 796c 653d 2262 6f72 6465  <td style="borde
+000004f0: 722d 746f 703a 2030 7078 3b22 3e3c 2f74  r-top: 0px;"></t
+00000500: 643e 0d0a 2020 2020 2020 2020 2020 2020  d>..            
+00000510: 3c74 6420 7374 796c 653d 2262 6f72 6465  <td style="borde
+00000520: 722d 746f 703a 2030 7078 3b22 3e7b 7b20  r-top: 0px;">{{ 
+00000530: 636f 6c75 6d6e 207d 7d3c 2f74 643e 0d0a  column }}</td>..
+00000540: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
+00000550: 7374 796c 653d 2262 6f72 6465 722d 746f  style="border-to
+00000560: 703a 2030 7078 3b20 7465 7874 2d61 6c69  p: 0px; text-ali
+00000570: 676e 3a20 7269 6768 743b 223e 0d0a 2020  gn: right;">..  
+00000580: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
+00000590: 6620 636f 6c75 6d6e 2e6c 6f63 616c 697a  f column.localiz
+000005a0: 6520 3d3d 204e 6f6e 6520 257d 7b7b 2063  e == None %}{{ c
+000005b0: 656c 6c20 7d7d 7b25 2065 6c73 6520 257d  ell }}{% else %}
+000005c0: 7b25 2069 6620 636f 6c75 6d6e 2e6c 6f63  {% if column.loc
+000005d0: 616c 697a 6520 257d 7b7b 2063 656c 6c7c  alize %}{{ cell|
+000005e0: 6c6f 6361 6c69 7a65 207d 7d0d 0a20 2020  localize }}..   
+000005f0: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
+00000600: 7365 2025 7d0d 0a20 2020 2020 2020 2020  se %}..         
+00000610: 2020 2020 2020 207b 7b20 6365 6c6c 7c75         {{ cell|u
+00000620: 6e6c 6f63 616c 697a 6520 7d7d 7b25 2065  nlocalize }}{% e
+00000630: 6e64 6966 2025 7d0d 0a20 2020 2020 2020  ndif %}..       
+00000640: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+00000650: 257d 0d0a 2020 2020 2020 2020 2020 2020  %}..            
+00000660: 3c2f 7464 3e0d 0a20 2020 2020 2020 2020  </td>..         
+00000670: 203c 2f74 723e 0d0a 2020 2020 2020 2020   </tr>..        
+00000680: 7b25 2065 6e64 6966 2025 7d0d 0a20 2020  {% endif %}..   
+00000690: 2020 207b 2520 656e 6466 6f72 2025 7d0d     {% endfor %}.
+000006a0: 0a20 2020 207b 2520 656e 6469 6620 257d  .    {% endif %}
+000006b0: 0d0a 0d0a 2020 2020 7b25 2069 6620 666f  ....    {% if fo
+000006c0: 726c 6f6f 702e 6c61 7374 2061 6e64 2074  rloop.last and t
+000006d0: 6162 6c65 2e69 6e66 696e 6974 655f 7363  able.infinite_sc
+000006e0: 726f 6c6c 2061 6e64 2074 6162 6c65 2e70  roll and table.p
+000006f0: 6167 652e 6e75 6d62 6572 203e 3d20 7461  age.number >= ta
+00000700: 626c 652e 7061 6765 2e70 6167 696e 6174  ble.page.paginat
+00000710: 6f72 2e6e 756d 5f70 6167 6573 2025 7d0d  or.num_pages %}.
+00000720: 0a20 2020 2020 203c 7472 3e0d 0a20 2020  .      <tr>..   
+00000730: 2020 2020 203c 7464 2063 6f6c 7370 616e       <td colspan
+00000740: 3d22 7b7b 2074 6162 6c65 2e63 6f6c 756d  ="{{ table.colum
+00000750: 6e73 7c6c 656e 6774 6820 7d7d 2220 7374  ns|length }}" st
+00000760: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00000770: 2063 656e 7465 7222 3e0d 0a20 2020 2020   center">..     
+00000780: 2020 2020 202d 2d20 456e 6420 6f66 2064       -- End of d
+00000790: 6174 6120 2d2d 0d0a 2020 2020 2020 2020  ata --..        
+000007a0: 3c2f 7464 3e0d 0a20 2020 2020 203c 2f74  </td>..      </t
+000007b0: 723e 0d0a 2020 2020 7b25 2065 6e64 6966  r>..    {% endif
+000007c0: 2025 7d0d 0a20 207b 2520 656e 6462 6c6f   %}..  {% endblo
+000007d0: 636b 2074 6162 6c65 2e74 626f 6479 2e72  ck table.tbody.r
+000007e0: 6f77 2025 7d0d 0a20 207b 2520 6966 2066  ow %}..  {% if f
+000007f0: 6f72 6c6f 6f70 2e6c 6173 7420 616e 6420  orloop.last and 
+00000800: 7461 626c 652e 696e 6669 6e69 7465 5f6c  table.infinite_l
+00000810: 6f61 6420 257d 0d0a 2020 2020 7b25 2069  oad %}..    {% i
+00000820: 6620 7461 626c 652e 7061 6765 2e6e 756d  f table.page.num
+00000830: 6265 7220 3c20 7461 626c 652e 7061 6765  ber < table.page
+00000840: 2e70 6167 696e 6174 6f72 2e6e 756d 5f70  .paginator.num_p
+00000850: 6167 6573 2025 7d0d 0a20 2020 2020 203c  ages %}..      <
+00000860: 7472 2069 643d 2274 725f 6c61 7374 220d  tr id="tr_last".
+00000870: 0a20 2020 2020 2020 2020 2068 782d 7461  .          hx-ta
+00000880: 7267 6574 3d22 2374 725f 6c61 7374 220d  rget="#tr_last".
+00000890: 0a20 2020 2020 2020 2020 2068 782d 7377  .          hx-sw
+000008a0: 6170 3d22 6f75 7465 7248 544d 4c22 0d0a  ap="outerHTML"..
+000008b0: 2020 2020 2020 2020 2020 6878 2d67 6574            hx-get
+000008c0: 3d22 7b25 2071 7565 7279 7374 7269 6e67  ="{% querystring
+000008d0: 2074 6162 6c65 2e70 7265 6669 7865 645f   table.prefixed_
+000008e0: 7061 6765 5f66 6965 6c64 3d74 6162 6c65  page_field=table
+000008f0: 2e70 6167 652e 6e65 7874 5f70 6167 655f  .page.next_page_
+00000900: 6e75 6d62 6572 2077 6974 686f 7574 2022  number without "
+00000910: 5f73 6372 6f6c 6c22 2025 7d22 0d0a 2020  _scroll" %}"..  
+00000920: 2020 2020 2020 2020 6878 2d76 616c 733d          hx-vals=
+00000930: 277b 225f 7363 726f 6c6c 223a 2022 7472  '{"_scroll": "tr
+00000940: 7565 227d 273e 0d0a 2020 2020 2020 2020  ue"}'>..        
+00000950: 3c74 6420 636f 6c73 7061 6e3d 227b 7b20  <td colspan="{{ 
+00000960: 7461 626c 652e 636f 6c75 6d6e 737c 6c65  table.columns|le
+00000970: 6e67 7468 207d 7d22 2073 7479 6c65 3d22  ngth }}" style="
+00000980: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
+00000990: 6572 223e 0d0a 2020 2020 2020 2020 2020  er">..          
+000009a0: 3c62 7574 746f 6e20 7479 7065 3d22 6275  <button type="bu
+000009b0: 7474 6f6e 2220 636c 6173 733d 2262 746e  tton" class="btn
+000009c0: 2062 746e 2d70 7269 6d61 7279 2220 6e61   btn-primary" na
+000009d0: 6d65 3d22 6c6f 6164 5f6d 6f72 6522 3e7b  me="load_more">{
+000009e0: 2520 7472 616e 7320 274c 6f61 6420 6d6f  % trans 'Load mo
+000009f0: 7265 2720 257d 3c2f 6275 7474 6f6e 3e0d  re' %}</button>.
+00000a00: 0a20 2020 2020 2020 203c 2f74 643e 0d0a  .        </td>..
+00000a10: 2020 2020 2020 3c2f 7472 3e0d 0a20 2020        </tr>..   
+00000a20: 207b 2520 656c 7365 2025 7d0d 0a20 2020   {% else %}..   
+00000a30: 2020 203c 7472 3e0d 0a20 2020 2020 2020     <tr>..       
+00000a40: 203c 7464 2063 6f6c 7370 616e 3d22 7b7b   <td colspan="{{
+00000a50: 2074 6162 6c65 2e63 6f6c 756d 6e73 7c6c   table.columns|l
+00000a60: 656e 6774 6820 7d7d 2220 7374 796c 653d  ength }}" style=
+00000a70: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
+00000a80: 7465 7222 3e0d 0a20 2020 2020 2020 2020  ter">..         
+00000a90: 202d 2d20 456e 6420 6f66 2064 6174 6120   -- End of data 
+00000aa0: 2d2d 0d0a 2020 2020 2020 2020 3c2f 7464  --..        </td
+00000ab0: 3e0d 0a20 2020 2020 203c 2f74 723e 0d0a  >..      </tr>..
+00000ac0: 2020 2020 7b25 2065 6e64 6966 2025 7d0d      {% endif %}.
+00000ad0: 0a20 207b 2520 656e 6469 6620 257d 0d0a  .  {% endif %}..
+00000ae0: 7b25 2065 6d70 7479 2025 7d0d 0a20 207b  {% empty %}..  {
+00000af0: 2520 6966 2074 6162 6c65 2e65 6d70 7479  % if table.empty
+00000b00: 5f74 6578 7420 257d 0d0a 2020 2020 7b25  _text %}..    {%
+00000b10: 2062 6c6f 636b 2074 6162 6c65 2e74 626f   block table.tbo
+00000b20: 6479 2e65 6d70 7479 5f74 6578 7420 257d  dy.empty_text %}
+00000b30: 0d0a 2020 2020 2020 3c74 723e 0d0a 2020  ..      <tr>..  
+00000b40: 2020 2020 2020 3c74 6420 636f 6c73 7061        <td colspa
+00000b50: 6e3d 227b 7b20 7461 626c 652e 636f 6c75  n="{{ table.colu
+00000b60: 6d6e 737c 6c65 6e67 7468 207d 7d22 3e7b  mns|length }}">{
+00000b70: 7b20 7461 626c 652e 656d 7074 795f 7465  { table.empty_te
+00000b80: 7874 207d 7d3c 2f74 643e 0d0a 2020 2020  xt }}</td>..    
+00000b90: 2020 3c2f 7472 3e0d 0a20 2020 207b 2520    </tr>..    {% 
+00000ba0: 656e 6462 6c6f 636b 2074 6162 6c65 2e74  endblock table.t
+00000bb0: 626f 6479 2e65 6d70 7479 5f74 6578 7420  body.empty_text 
+00000bc0: 257d 0d0a 2020 7b25 2065 6e64 6966 2025  %}..  {% endif %
+00000bd0: 7d0d 0a7b 2520 656e 6466 6f72 2025 7d0d  }..{% endfor %}.
+00000be0: 0a                                       .
```

### Comparing `django_tableaux-0.2/django_tableaux/templates/django_tableaux/bootstrap5_base.html` & `django_tableaux-0.3/django_tableaux/templates/django_tableaux/bootstrap5_base.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.2/django_tableaux/templates/django_tableaux/custom_bootstrap4.html` & `django_tableaux-0.3/django_tableaux/templates/django_tableaux/custom_bootstrap4.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 {% extends 'django_tableaux/bootstrap4.html' %}
-{% load django_tables2 bootstrap4 %}
-{% load i18n %}
+{% load django_tables2 bootstrap4 i18n %}
 {% block table.thead %}
   {% if table.show_header %}
     <thead {{ table.attrs.thead.as_html }}>
     <tr>
       {% for column in table.columns %}
         <th {{ column.attrs.th.as_html }}>
           {% if column.name == "selection" %}
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
 {% extends 'django_tableaux/bootstrap4.html' %} {% load django_tables2
-bootstrap4 %} {% load i18n %} {% block table.thead %} {% if table.show_header
-%}
+bootstrap4 i18n %} {% block table.thead %} {% if table.show_header %}
 { table.attrs.thead.as_html }}>
 {% for column in table.columns %}
 { column.attrs.th.as_html }}> {% if column.name == "selection" %} ⁰ {% else %}
 {% if column.orderable %} {#_{%_if_"-"_in_column.order_by.0_%}△{%_else_%}▽{%
 endif_%}#}_{{_column.header_}} {% else %} {{ column.header }} {% endif %} {%
 endif %}
 {% endfor %}
```

### Comparing `django_tableaux-0.2/django_tableaux/templates/django_tableaux/filter_toolbar.html` & `django_tableaux-0.3/django_tableaux/templates/django_tableaux/filter_toolbar.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 {% load bootstrap4 %}
 {% if filter.style == filter.style.TOOLBAR %}
   <form id="id_filter_form" hx-target="#table_data">
     {{ filter.form.media }}
     <input type="hidden" name="per_page" value="{{ per_page }}">
     <div class="d-flex">
       {% for field in filter.form.visible_fields %}
-        {% if filter_button %}
-          {% bootstrap_field field form_group_class="form-group pl-2 pt-2" label_class="small mb-0" placeholder="" %}
-        {% else %}
-          {% bootstrap_field field form_group_class="form-group pl-2 pt-2 auto-submit" label_class="small mb-0" placeholder="" %}
-        {% endif %}
+        {% include "django_tableaux/toolbar/_filter_field.html" with toolbar=True field=field filter_button=filter_button %}
       {% endfor %}
       {% if filter_button %}
         <div class="form-group pl-2 pt-2">
           <label for="id_filter_button"></label>
           <button type="submit" class="form-control btn btn-primary" style="width:150px; display: block;" id="id_filter_button">
             Filter
           </button>
         </div>
       {% endif %}
+  <span name="clr_all" hx-get="" class="filter-clear mt-3 p-3"> Clear</span></p>
     </div>
   </form>
 {% endif %}
```

### Comparing `django_tableaux-0.2/django_tableaux/templates/django_tableaux/modal_base.html` & `django_tableaux-0.3/django_tableaux/templates/django_tableaux/modal_base.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.2/django_tableaux/templates/django_tableaux/modal_filter.html` & `django_tableaux-0.3/django_tableaux/templates/django_tableaux/modal_filter.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.2/django_tableaux/templates/django_tableaux/modal_form.html` & `django_tableaux-0.3/django_tableaux/templates/django_tableaux/modal_form.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.2/django_tableaux/templates/django_tableaux/paginator.html` & `django_tableaux-0.3/django_tableaux/templates/django_tableaux/paginator.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.2/django_tableaux/templates/django_tableaux/toolbar/_actions.html` & `django_tableaux-0.3/django_tableaux/templates/django_tableaux/toolbar/_actions.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 {% load querystring from django_tables2 %}
 {% if actions %}
-  <div>
+<form id="action_form" hx-target="#modals-here">{% csrf_token %}
     <input type="hidden" name="query" value={% querystring without "page" "per_page" %}>
+    <input type="hidden" name="selected_ids">
     <div class="d-flex">
       <div class="mb-0 pb-0 px-2" style="width:200px;">
         <div id="selected"><span id="count">0</span> of {{ table.rows|length }} rows selected</div>
         <div style="display: none;">
           <input type="checkbox" id="select_all" name="select_all" class="py-0" value="Select all">
           <label class="form-check-label ml-2 py-0" for="select_all">Select all</label>
         </div>
@@ -13,15 +14,15 @@
       <div class="my-2">
         <div class="dropdown float-right">
           <button class="btn btn-primary btn-sm dropdown-toggle" type="button" id="selectActionMenu" data-toggle="dropdown">
             Select action
           </button>
           <div class="dropdown-menu">
             {% for action in actions %}
-                <button class="dropdown-item" type="submit" name="{{ action.0 }}" hx-post>{{ action.1 }}</button>
+                <button class="dropdown-item" name="{{ action.0 }}" hx-post>{{ action.1 }}</button>
             {% endfor %}
           </div>
         </div>
       </div>
     </div>
-  </div>
+</form>
 {% endif %}
```

### Comparing `django_tableaux-0.2/django_tableaux/templates/django_tableaux/toolbar/_columns.html` & `django_tableaux-0.3/django_tableaux/templates/django_tableaux/toolbar/_columns.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.2/django_tableaux/templates/django_tableaux/toolbar/_rows.html` & `django_tableaux-0.3/django_tableaux/templates/django_tableaux/toolbar/_rows.html`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.2/django_tableaux/tests.py` & `django_tableaux-0.3/django_tableaux/tests.py`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.2/django_tableaux/utils.py` & `django_tableaux-0.3/django_tableaux/utils.py`

 * *Files identical despite different names*

### Comparing `django_tableaux-0.2/django_tableaux/views.py` & `django_tableaux-0.3/django_tableaux/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,20 @@
 class DjangoTableauxView(SingleTableMixin, FilterView):
     class FilterStyle(IntEnum):
         NONE = 0
         TOOLBAR = 1
         MODAL = 2
         HEADER = 3
 
+    class ClickAction(IntEnum):
+        NONE = 0
+        GET = 1
+        HX_GET = 2
+        CUSTOM = 3
+
     title = ""
     template_name = "django_tableaux/django_tableaux.html"
     templates = {
         "filter": "django_tableaux/modal_filter.html",
         "table_data": "django_tableaux/render_table_data.html",
         "rows": "django_tableaux/render_rows.html",
         "cell_form": "django_tableaux/cell_form.html",
@@ -58,29 +64,30 @@
     #
     context_filter_name = "filter"
     filter_style = FilterStyle.TOOLBAR
     filter_button = False  # only relevant for TOOLBAR style
     #
     column_settings = False
     row_settings = False
-    #
-    click_method = "get"
+
+    click_action = ClickAction.NONE
     click_url_name = ""
     click_target = "#modals-here"
     #
     sticky_header = False
     buttons = []
     object_name = ""
     #
     export_format = "csv"
     export_class = TableExport
     export_name = "table"
     dataset_kwargs = None
 
     export_formats = (TableExport.CSV,)
+    ALLOWED_PARAMS = ["page", "per_page", "sort", "_width"]
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.table = None
         self.width = 0
         self.selected_objects = None
         self.selected_ids = None
@@ -135,80 +142,113 @@
                 exclude_columns=exclude_columns,
                 dataset_kwargs=self.get_dataset_kwargs(),
             )
             return exporter.response(filename=f"{filename}.{export_format}")
         return super().get(request, *args, **kwargs)
 
     def get_htmx(self, request, *args, **kwargs):
+        # Some actions depend on trigger_name; others on trigger
+        trigger_name = request.htmx.trigger_name
+        trigger = request.htmx.trigger
+        if trigger_name:
+            if trigger_name == "filter" and self.filterset_class:
+                # show filter modal
+                context = {"filter": self.filterset_class(request.GET)}
+                return render(request, self.templates["filter"], context)
+
+            elif trigger_name == "filter_form":
+                # a filter value was changed
+                return self.render_template(
+                    self.templates["table_data"], *args, **kwargs
+                )
 
-        if request.htmx.trigger == "table_data":
-            # triggered refresh of table data after create or update
-            return self.render_template(self.templates["table_data"], *args, **kwargs)
-
-        elif request.htmx.trigger_name == "filter" and self.filterset_class:
-            # show filter modal
-            context = {"filter": self.filterset_class(request.GET)}
-            return render(request, self.templates["filter"], context)
+            elif "clr_" in trigger_name:
+                # cancel a filter
+                filter = trigger_name.split("_")[1]
+                qd = request.GET.copy()
+                if filter == "all":
+                    keys = list(qd.keys())
+                    for key in keys:
+                        if key not in self.ALLOWED_PARAMS:
+                            qd.pop(key)
+                else:
+                    qd.pop(filter)
+                return HttpResponseClientRedirect(f"{request.path}?{qd.urlencode()}")
 
-        elif request.htmx.trigger_name == "filter_form":
-            # a filter value was changed
+        if trigger == "table_data":
+            # triggered refresh of table data after create or update
             return self.render_template(self.templates["table_data"], *args, **kwargs)
 
-        elif "id_row" in request.htmx.trigger:
+        elif "id_row" in trigger:
             # change number of rows to display
-            rows = request.htmx.trigger_name
+            rows = trigger_name
             save_per_page(request, rows)
             url = self._update_parameter(request, "per_page", rows)
             return HttpResponseClientRedirect(url)
 
-        elif "tr_" in request.htmx.trigger:
+        elif "tr_" in trigger:
             # infinite scroll/load_more or click on row
             if "_scroll" in request.GET:
                 return self.render_template(self.templates["rows"], *args, **kwargs)
 
             return self.row_clicked(
-                pk=request.htmx.trigger.split("_")[1],
+                pk=trigger.split("_")[1],
                 target=request.htmx.target,
                 return_url=request.htmx.current_url,
             )
 
-        elif "td_" in request.htmx.trigger:
+        elif "cell_" in trigger:
             # cell clicked
-            bits = request.htmx.trigger.split("_")
+            bits = trigger.split("_")
+            return self.edit_cell(
+                pk=bits[1],
+                column_name=visible_columns(request, self.table_class, self.width)[
+                    int(bits[2])
+                ],
+                target=request.htmx.target,
+            )
+
+        elif "td_" in trigger:
+            # cell clicked
+            bits = trigger.split("_")
             return self.cell_clicked(
                 pk=bits[1],
                 column_name=visible_columns(request, self.table_class, self.width)[
                     int(bits[2])
                 ],
                 target=request.htmx.target,
             )
 
         # Column handling
-        elif "id_col_reset" in request.htmx.trigger:
+        elif "id_col_reset" in trigger:
             # Reset default columns settings.
             # To make sure the column drop down is correctly updated we do a client refresh,
             table = self.table_class([])
             define_columns(table, self.width)
             save_columns(request, self.width, table.columns_default)
             return HttpResponseClientRefresh()
 
-        elif "id_col" in request.htmx.trigger:
+        elif "id_col" in trigger:
             # Click on a column checkbox in the dropdown re-renders the table data with new column settings.
             # The column dropdown does not need to be rendered because the checkboxes are in the correct state,
-            col_name = request.htmx.trigger_name[5:]
-            checked = request.htmx.trigger_name in request.GET
+            col_name = trigger_name[5:]
+            checked = trigger_name in request.GET
             set_column(request, self.width, col_name, checked)
             return self.render_template(self.templates["table_data"], *args, **kwargs)
 
-        elif "id_" in request.htmx.trigger:
+        elif "id_" in trigger:
+            if trigger == request.htmx.target:
+                # Clear filter value triggered by  click on X in input-prepend
+                qd = request.GET.copy()
+                qd.pop(trigger_name)
+                return HttpResponseClientRedirect(f"{request.path}?{qd.urlencode()}")
+            #
             # Filter value changed
             url = self._update_parameter(
-                request,
-                request.htmx.trigger_name,
-                request.GET.get(request.htmx.trigger_name, ""),
+                request, trigger_name, request.GET.get(trigger_name, "")
             )
             return HttpResponseClientRedirect(url)
         raise ValueError("Bad htmx get request")
 
     def rows_list(self):
         return [10, 15, 20, 25, 50, 100]
 
@@ -229,46 +269,51 @@
             actions=self.get_actions(),
             rows=self.rows_list(),
             per_page=self.request.GET.get(
                 "per_page", self.table_pagination.get("per_page", 25)
             ),
             breakpoints=breakpoints(self.table),
             width=self.width,
-            filters=[]
+            filters=[],
         )
         if "_width" in self.request.GET:
             context["breakpoints"] = None
+
         for key, value in self.request.GET.items():
-            if key not in ["page", "sort", "_width"] and value:
-                context['filters'].append(key)
+            if key not in self.ALLOWED_PARAMS and value:
+                context["filters"].append((key, value))
         return context
 
     def put(self, request, *args, **kwargs):
         # PUT is used to update a cell after inline editing
         params = QueryDict(request.body)
         bits = request.htmx.target.split("_")
         column_name = visible_columns(request, self.table_class, int(bits[3]))[
             int(bits[2])
         ]
-        return self.cell_changed(
-            record_pk=bits[1],
-            column_name=column_name,
-            value=params[column_name],
-            target=request.htmx.target,
-        )
+        value = params.get(column_name, None)
+        print(bits[1], value)
+        if value:
+            return self.cell_changed(
+                record_pk=bits[1],
+                column_name=column_name,
+                value=params[column_name],
+                target=request.htmx.target,
+            )
+        return HttpResponse("x")
 
     def post(self, request, *args, **kwargs):
         # Posts are an action performed on a queryset
         if "select_all" in request.POST:
             subset = "all"
             self.selected_ids = []
             self.selected_objects = self.filtered_query_set(request)
         else:
             subset = "selected"
-            self.selected_ids = request.POST.getlist("select-checkbox")
+            self.selected_ids = request.POST["selected_ids"].split(",")
             self.selected_objects = self.get_queryset().filter(pk__in=self.selected_ids)
 
         if request.htmx.trigger_name:
             if "export" in request.htmx.trigger_name:
                 # Export is a special case which must redirect to a regular GET that returns the file
                 request.session["selected_ids"] = self.selected_ids
                 bits = request.htmx.trigger_name.split("_")
@@ -323,19 +368,19 @@
         self.selected_ids is a list of model ids that were selected, empty for 'All rows'
         Possible return values:
         - None: (default) - reloads the last path
         - HttpResponse to be returned
         """
         return None
 
-    def row_clicked(self, pk, target, return_url):
-        """User clicked on a row without defining a click_url"""
+    def cell_clicked(self, pk, column_name, target, return_url):
+        """User clicked on a cell with custom action"""
         return HttpResponseClientRefresh()
 
-    def cell_clicked(self, pk, column_name, target):
+    def edit_cell(self, pk, column_name, target):
         """User clicked on an editable cell"""
         if not self.model:
             raise ConfigurationError(
                 "Model must be specified or cell_clicked must be overriden for editable cells",
             )
         if not self.form_class:
             raise ConfigurationError(
@@ -368,15 +413,15 @@
         Add extra attributes needed for rendering to the table
         """
         table.filter = _filter
         table.infinite_scroll = self.infinite_scroll
         table.infinite_load = self.infinite_load
         table.sticky_header = self.sticky_header
         # variables that control action when table is clicked
-        table.method = self.click_method
+        table.click_action = self.click_action
         table.url = ""
         table.pk = False
         if self.click_url_name:
             # handle case when there is no PK passed (create)
             try:
                 table.url = reverse(self.click_url_name)
             except NoReverseMatch:
```

### Comparing `django_tableaux-0.2/PKG-INFO` & `django_tableaux-0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django_tableaux
-Version: 0.2
-Summary: Django_tableaux: Django tables with Advanced User eXperience
+Version: 0.3
+Summary: Django tables with Advanced User eXperience
 Author-email: Ian Stewart <is@iskt.co.uk>
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/ianastewart/django_tableaux/
 
 ===============
 django_tableaux
@@ -21,13 +21,14 @@
 ============
 * The columns to display can be user-defined
 * Fully responsive: Define different column layouts for mobile, tablet and desktop
 * Bulk actions on selected rows or on all (possibly filtered) rows
 * Infinite scroll
 * Infinite load-more data
 * Position filters in a toolbar, in a modal or embed them within the table header
+* Show active filters with ability to clear individual filters
 * Edit specific fields directly inside the table
 * Easy integration with generic views for CRUD operations
 
 The project is still in beta but is fully usable.
 
 Full documentation to follow.
```

