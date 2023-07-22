# Comparing `tmp/angreal-2.0.6.tar.gz` & `tmp/angreal-2.0.7.tar.gz`

## Comparing `angreal-2.0.6.tar` & `angreal-2.0.7.tar`

### file list

```diff
@@ -1,198 +1,206 @@
--rw-r--r--   0        0        0     1333 1970-01-01 00:00:00.000000 angreal-2.0.6/Cargo.toml
--rw-r--r--   0      501       20      563 2023-03-02 18:18:44.000000 angreal-2.0.6/.angreal/task_echo.py
--rw-r--r--   0      501       20     1461 2023-03-02 18:18:45.000000 angreal-2.0.6/.angreal/task_run_tests.py
--rw-r--r--   0      501       20      371 2023-03-02 18:18:45.000000 angreal-2.0.6/.angreal/task_setup.py
--rw-r--r--   0      501       20     1782 2023-03-02 18:18:45.000000 angreal-2.0.6/.github/workflows/docs.yaml
--rw-r--r--   0      501       20     7718 2023-03-02 18:18:45.000000 angreal-2.0.6/.github/workflows/release.yaml
--rw-r--r--   0      501       20     3661 2023-03-02 18:18:45.000000 angreal-2.0.6/.github/workflows/test.yaml
--rw-r--r--   0      501       20     5668 2023-03-02 18:18:45.000000 angreal-2.0.6/.gitignore
--rw-r--r--   0      501       20     2565 2023-03-02 18:18:45.000000 angreal-2.0.6/README.md
--rw-r--r--   0      501       20      826 2023-03-02 18:18:45.000000 angreal-2.0.6/docs/_draft/how_to/include-jinja-templates.rst.md
--rw-r--r--   0      501       20      365 2023-03-02 18:18:45.000000 angreal-2.0.6/docs/_draft/how_to/use-docker-integration.rst.md
--rw-r--r--   0      501       20      548 2023-03-02 18:18:45.000000 angreal-2.0.6/docs/_draft/how_to/use-git-integration.rst.md
--rw-r--r--   0      501       20      864 2023-03-02 18:18:45.000000 angreal-2.0.6/docs/_draft/how_to/work_with_virtual_environments.rst.md
--rw-r--r--   0      501       20       84 2023-03-02 18:18:45.000000 angreal-2.0.6/docs/archetypes/default.md
--rw-r--r--   0      501       20     2788 2023-03-02 18:18:45.000000 angreal-2.0.6/docs/config.toml
--rw-r--r--   0      501       20     2554 2023-03-02 18:18:45.000000 angreal-2.0.6/docs/content/_index.md
--rw-r--r--   0      501       20      492 2023-03-02 18:18:46.000000 angreal-2.0.6/docs/content/api_reference/_index.md
--rw-r--r--   0      501       20     3008 2023-03-02 18:18:46.000000 angreal-2.0.6/docs/content/api_reference/py_angreal.md
--rw-r--r--   0      501       20       63 2023-03-02 18:18:46.000000 angreal-2.0.6/docs/content/available_templates/_index.md
--rw-r--r--   0      501       20     3212 2023-03-02 18:18:46.000000 angreal-2.0.6/docs/content/code_of_conduct/_index.md
--rw-r--r--   0      501       20     1314 2023-03-02 18:18:46.000000 angreal-2.0.6/docs/content/contributing/_index.md
--rw-r--r--   0      501       20       55 2023-03-02 18:18:46.000000 angreal-2.0.6/docs/content/discussions/_index.md
--rw-r--r--   0      501       20       58 2023-03-02 18:18:46.000000 angreal-2.0.6/docs/content/how-to/_index.md
--rw-r--r--   0      501       20     4387 2023-03-02 18:18:46.000000 angreal-2.0.6/docs/content/how-to/add_arguments.md
--rw-r--r--   0      501       20      324 2023-03-02 18:18:46.000000 angreal-2.0.6/docs/content/how-to/create_a_task.md
--rw-r--r--   0      501       20       62 2023-03-02 18:18:46.000000 angreal-2.0.6/docs/content/tutorials/_index.md
--rw-r--r--   0      501       20       68 2023-03-02 18:18:46.000000 angreal-2.0.6/docs/content/tutorials/meeting_notes.files/angreal.toml
--rw-r--r--   0      501       20       62 2023-03-02 18:18:46.000000 angreal-2.0.6/docs/content/tutorials/meeting_notes.files/{{ name }}/.angreal/init.py
--rw-r--r--   0      501       20     1254 2023-03-02 18:18:46.000000 angreal-2.0.6/docs/content/tutorials/meeting_notes.files/{{ name }}/.angreal/task_take_notes.py
--rw-r--r--   0      501       20       84 2023-03-02 18:18:46.000000 angreal-2.0.6/docs/content/tutorials/meeting_notes.files/{{ name }}/README.md
--rw-r--r--   0      501       20     5403 2023-03-02 18:18:46.000000 angreal-2.0.6/docs/content/tutorials/your-first-angreal.md
--rw-r--r--   0      501       20     5806 2023-03-02 18:18:46.000000 angreal-2.0.6/docs/content/why/_index.md
--rw-r--r--   0      501       20      198 2023-03-02 18:18:47.000000 angreal-2.0.6/docs/layouts/partials/logo.html
--rw-r--r--   0      501       20     6445 2023-03-02 18:18:47.000000 angreal-2.0.6/docs/static/images/wheel.png
--rw-r--r--   0      501       20     1139 2023-03-02 18:18:47.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/LICENSE.md
--rw-r--r--   0      501       20      168 2023-03-02 18:18:47.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/archetypes/chapter.md
--rw-r--r--   0      501       20       98 2023-03-02 18:18:47.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/archetypes/default.md
--rw-r--r--   0      501       20      585 2023-03-02 18:18:47.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/i18n/ar.toml
--rw-r--r--   0      501       20      507 2023-03-02 18:18:47.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/i18n/de.toml
--rw-r--r--   0      501       20      487 2023-03-02 18:18:47.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/i18n/en.toml
--rw-r--r--   0      501       20      484 2023-03-02 18:18:47.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/i18n/es.toml
--rw-r--r--   0      501       20      531 2023-03-02 18:18:47.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/i18n/fr.toml
--rw-r--r--   0      501       20      726 2023-03-02 18:18:47.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/i18n/hi.toml
--rw-r--r--   0      501       20      499 2023-03-02 18:18:47.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/i18n/id.toml
--rw-r--r--   0      501       20      514 2023-03-02 18:18:47.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/i18n/ja.toml
--rw-r--r--   0      501       20      499 2023-03-02 18:18:47.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/i18n/nl.toml
--rw-r--r--   0      501       20      490 2023-03-02 18:18:47.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/i18n/pt.toml
--rw-r--r--   0      501       20      623 2023-03-02 18:18:47.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/i18n/ru.toml
--rw-r--r--   0      501       20      495 2023-03-02 18:18:47.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/i18n/tr.toml
--rw-r--r--   0      501       20      710 2023-03-02 18:18:47.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/i18n/vn.toml
--rw-r--r--   0      501       20      484 2023-03-02 18:18:47.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/i18n/zh-cn.toml
--rw-r--r--   0      501       20   284162 2023-03-02 18:18:47.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/images/screenshot.png
--rw-r--r--   0      501       20   143335 2023-03-02 18:18:48.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/images/tn.png
--rw-r--r--   0      501       20     2263 2023-03-02 18:18:48.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/404.html
--rw-r--r--   0      501       20      549 2023-03-02 18:18:48.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/_default/list.html
--rw-r--r--   0      501       20      354 2023-03-02 18:18:48.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/_default/single.html
--rw-r--r--   0      501       20     1399 2023-03-02 18:18:48.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/index.html
--rw-r--r--   0      501       20      428 2023-03-02 18:18:48.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/index.json
--rw-r--r--   0      501       20       79 2023-03-02 18:18:48.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/partials/custom-comments.html
--rw-r--r--   0      501       20      181 2023-03-02 18:18:48.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/partials/custom-footer.html
--rw-r--r--   0      501       20      147 2023-03-02 18:18:48.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/partials/custom-header.html
--rw-r--r--   0      501       20       76 2023-03-02 18:18:48.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/partials/favicon.html
--rw-r--r--   0      501       20     4539 2023-03-02 18:18:48.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/partials/footer.html
--rw-r--r--   0      501       20     5312 2023-03-02 18:18:48.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/partials/header.html
--rw-r--r--   0      501       20      137 2023-03-02 18:18:48.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/partials/logo.html
--rw-r--r--   0      501       20      193 2023-03-02 18:18:48.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/partials/menu-footer.html
--rw-r--r--   0      501       20     6236 2023-03-02 18:18:48.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/partials/menu.html
--rw-r--r--   0      501       20      215 2023-03-02 18:18:48.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/partials/meta.html
--rw-r--r--   0      501       20      911 2023-03-02 18:18:48.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/partials/search.html
--rw-r--r--   0      501       20      171 2023-03-02 18:18:48.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/partials/tags.html
--rw-r--r--   0      501       20       90 2023-03-02 18:18:48.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/partials/toc.html
--rw-r--r--   0      501       20     1176 2023-03-02 18:18:48.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/shortcodes/attachments.html
--rw-r--r--   0      501       20      452 2023-03-02 18:18:48.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/shortcodes/button.html
--rw-r--r--   0      501       20     4462 2023-03-02 18:18:49.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/shortcodes/children.html
--rw-r--r--   0      501       20      729 2023-03-02 18:18:49.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/shortcodes/expand.html
--rw-r--r--   0      501       20      164 2023-03-02 18:18:49.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/shortcodes/mermaid.html
--rw-r--r--   0      501       20      151 2023-03-02 18:18:49.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/shortcodes/notice.html
--rw-r--r--   0      501       20      440 2023-03-02 18:18:49.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/shortcodes/ref.html
--rw-r--r--   0      501       20      440 2023-03-02 18:18:49.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/shortcodes/relref.html
--rw-r--r--   0      501       20      190 2023-03-02 18:18:49.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/shortcodes/siteparam.html
--rw-r--r--   0      501       20      370 2023-03-02 18:18:49.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/shortcodes/tab.html
--rw-r--r--   0      501       20      793 2023-03-02 18:18:49.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/shortcodes/tabs.html
--rw-r--r--   0      501       20     1588 2023-03-02 18:18:49.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/atom-one-dark-reasonable.css
--rw-r--r--   0      501       20      894 2023-03-02 18:18:49.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/auto-complete.css
--rw-r--r--   0      501       20     1868 2023-03-02 18:18:49.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/featherlight.min.css
--rw-r--r--   0      501       20   101894 2023-03-02 18:18:49.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/fontawesome-all.min.css
--rw-r--r--   0      501       20     4755 2023-03-02 18:18:49.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/hugo-theme.css
--rw-r--r--   0      501       20     1342 2023-03-02 18:18:49.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/hybrid.css
--rw-r--r--   0      501       20    11887 2023-03-02 18:18:49.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/nucleus.css
--rw-r--r--   0      501       20     4629 2023-03-02 18:18:50.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/perfect-scrollbar.min.css
--rw-r--r--   0      501       20      859 2023-03-02 18:18:50.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/tabs.css
--rw-r--r--   0      501       20     1046 2023-03-02 18:18:50.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/tags.css
--rw-r--r--   0      501       20     4087 2023-03-02 18:18:50.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/theme-blue.css
--rw-r--r--   0      501       20     4087 2023-03-02 18:18:50.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/theme-green.css
--rw-r--r--   0      501       20     4084 2023-03-02 18:18:50.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/theme-red.css
--rw-r--r--   0      501       20    24719 2023-03-02 18:18:50.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/theme.css
--rw-r--r--   0      501       20    35620 2023-03-02 18:18:50.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.eot
--rw-r--r--   0      501       20    61990 2023-03-02 18:18:50.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.svg
--rw-r--r--   0      501       20    63184 2023-03-02 18:18:50.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.ttf
--rw-r--r--   0      501       20    38248 2023-03-02 18:18:50.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.woff
--rw-r--r--   0      501       20    22446 2023-03-02 18:18:50.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.eot
--rw-r--r--   0      501       20    98609 2023-03-02 18:18:51.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.svg
--rw-r--r--   0      501       20    56884 2023-03-02 18:18:51.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.ttf
--rw-r--r--   0      501       20    24772 2023-03-02 18:18:51.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.woff
--rw-r--r--   0      501       20    19760 2023-03-02 18:18:51.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.woff2
--rw-r--r--   0      501       20    21080 2023-03-02 18:18:51.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.eot
--rw-r--r--   0      501       20    91968 2023-03-02 18:18:51.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.svg
--rw-r--r--   0      501       20    55600 2023-03-02 18:18:51.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.ttf
--rw-r--r--   0      501       20    23476 2023-03-02 18:18:51.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.woff
--rw-r--r--   0      501       20    18716 2023-03-02 18:18:51.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.woff2
--rw-r--r--   0      501       20    24290 2023-03-02 18:18:51.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.eot
--rw-r--r--   0      501       20    54838 2023-03-02 18:18:51.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.svg
--rw-r--r--   0      501       20    49752 2023-03-02 18:18:51.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.ttf
--rw-r--r--   0      501       20    25896 2023-03-02 18:18:51.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.woff
--rw-r--r--   0      501       20    21128 2023-03-02 18:18:51.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.woff2
--rw-r--r--   0      501       20    24817 2023-03-02 18:18:51.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.eot
--rw-r--r--   0      501       20    54786 2023-03-02 18:18:51.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.svg
--rw-r--r--   0      501       20    50784 2023-03-02 18:18:51.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.ttf
--rw-r--r--   0      501       20    26392 2023-03-02 18:18:52.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.woff
--rw-r--r--   0      501       20    21548 2023-03-02 18:18:52.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.woff2
--rw-r--r--   0      501       20    26481 2023-03-02 18:18:52.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.eot
--rw-r--r--   0      501       20    54421 2023-03-02 18:18:52.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.svg
--rw-r--r--   0      501       20    54232 2023-03-02 18:18:52.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.ttf
--rw-r--r--   0      501       20    27900 2023-03-02 18:18:52.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.woff
--rw-r--r--   0      501       20    22884 2023-03-02 18:18:52.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.woff2
--rw-r--r--   0      501       20      509 2023-03-02 18:18:52.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/images/clippy.svg
--rw-r--r--   0      501       20      608 2023-03-02 18:18:52.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/images/favicon.png
--rw-r--r--   0      501       20   206249 2023-03-02 18:18:52.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/images/gopher-404.jpg
--rw-r--r--   0      501       20     5328 2023-03-02 18:18:52.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/auto-complete.js
--rw-r--r--   0      501       20    10754 2023-03-02 18:18:52.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/clipboard.min.js
--rw-r--r--   0      501       20     9295 2023-03-02 18:18:52.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/featherlight.min.js
--rw-r--r--   0      501       20    95349 2023-03-02 18:18:52.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/highlight.pack.js
--rw-r--r--   0      501       20     2847 2023-03-02 18:18:52.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/hugo-learn.js
--rw-r--r--   0      501       20    86927 2023-03-02 18:18:52.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/jquery-3.3.1.min.js
--rwxr-xr-x   0      501       20    10085 2023-03-02 18:18:53.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/jquery.sticky.js
--rw-r--r--   0      501       20    16771 2023-03-02 18:18:53.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/learn.js
--rw-r--r--   0      501       20    29527 2023-03-02 18:18:53.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/lunr.min.js
--rw-r--r--   0      501       20     7546 2023-03-02 18:18:53.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/modernizr.custom-3.6.0.js
--rw-r--r--   0      501       20    25333 2023-03-02 18:18:53.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/perfect-scrollbar.jquery.min.js
--rw-r--r--   0      501       20    25012 2023-03-02 18:18:53.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/perfect-scrollbar.min.js
--rw-r--r--   0      501       20     3451 2023-03-02 18:18:53.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/search.js
--rw-r--r--   0      501       20   832982 2023-03-02 18:18:53.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/mermaid/mermaid.js
--rw-r--r--   0      501       20   134396 2023-03-02 18:18:53.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.eot
--rw-r--r--   0      501       20   739402 2023-03-02 18:18:53.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.svg
--rw-r--r--   0      501       20   186124 2023-03-02 18:18:53.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0      501       20    87048 2023-03-02 18:18:53.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.woff
--rw-r--r--   0      501       20   107656 2023-03-02 18:18:53.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0      501       20    40308 2023-03-02 18:18:53.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.eot
--rw-r--r--   0      501       20   135804 2023-03-02 18:18:53.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.svg
--rw-r--r--   0      501       20    62320 2023-03-02 18:18:53.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0      501       20    18164 2023-03-02 18:18:54.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.woff
--rw-r--r--   0      501       20    25236 2023-03-02 18:18:54.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0      501       20   209012 2023-03-02 18:18:54.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.eot
--rw-r--r--   0      501       20   771697 2023-03-02 18:18:54.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.svg
--rw-r--r--   0      501       20   397420 2023-03-02 18:18:54.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0      501       20   102224 2023-03-02 18:18:54.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.woff
--rw-r--r--   0      501       20   150516 2023-03-02 18:18:54.000000 angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.woff2
--rw-r--r--   0      501       20        0 2023-03-02 18:18:54.000000 angreal-2.0.6/py_tests/__init__.py
--rw-r--r--   0      501       20     2053 2023-03-02 18:18:54.000000 angreal-2.0.6/py_tests/integrations/test_docker.py
--rw-r--r--   0      501       20      843 2023-03-02 18:18:54.000000 angreal-2.0.6/py_tests/integrations/test_git.py
--rw-r--r--   0      501       20        5 2023-03-02 18:18:54.000000 angreal-2.0.6/py_tests/integrations/test_r.txt
--rw-r--r--   0      501       20     2407 2023-03-02 18:18:54.000000 angreal-2.0.6/py_tests/integrations/test_venv.py
--rw-r--r--   0      501       20     2473 2023-03-02 18:18:54.000000 angreal-2.0.6/py_tests/test_angreal.py
--rw-r--r--   0      501       20      933 2023-03-02 18:18:54.000000 angreal-2.0.6/pyproject.toml
--rw-r--r--   0      501       20     3030 2023-03-02 18:18:54.000000 angreal-2.0.6/python/angreal/__init__.py
--rw-r--r--   0      501       20       43 2023-03-02 18:18:54.000000 angreal-2.0.6/python/angreal/integrations/docker/__init__.py
--rw-r--r--   0      501       20       71 2023-03-02 18:18:54.000000 angreal-2.0.6/python/angreal/integrations/docker/container.py
--rw-r--r--   0      501       20       60 2023-03-02 18:18:54.000000 angreal-2.0.6/python/angreal/integrations/docker/image.py
--rw-r--r--   0      501       20       66 2023-03-02 18:18:54.000000 angreal-2.0.6/python/angreal/integrations/docker/network.py
--rw-r--r--   0      501       20       63 2023-03-02 18:18:54.000000 angreal-2.0.6/python/angreal/integrations/docker/volume.py
--rw-r--r--   0      501       20     2664 2023-03-02 18:18:54.000000 angreal-2.0.6/python/angreal/integrations/git.py
--rw-r--r--   0      501       20     4786 2023-03-02 18:18:54.000000 angreal-2.0.6/python/angreal/integrations/venv.py
--rw-r--r--   0      501       20       30 2023-03-02 18:18:54.000000 angreal-2.0.6/rust-toolchain.toml
--rw-r--r--   0      501       20     3278 2023-03-02 18:18:54.000000 angreal-2.0.6/src/builder.rs
--rw-r--r--   0      501       20     3817 2023-03-02 18:18:54.000000 angreal-2.0.6/src/git.rs
--rw-r--r--   0      501       20    14146 2023-03-02 18:18:54.000000 angreal-2.0.6/src/init.rs
--rw-r--r--   0      501       20     6995 2023-03-02 18:18:54.000000 angreal-2.0.6/src/lib.rs
--rw-r--r--   0      501       20     1284 2023-03-02 18:18:54.000000 angreal-2.0.6/src/logger.rs
--rw-r--r--   0      501       20     1039 2023-03-02 18:18:54.000000 angreal-2.0.6/src/macros.rs
--rw-r--r--   0      501       20     3290 2023-03-02 18:18:54.000000 angreal-2.0.6/src/py_logger.rs
--rw-r--r--   0      501       20     6338 2023-03-02 18:18:54.000000 angreal-2.0.6/src/task.rs
--rw-r--r--   0      501       20     6929 2023-03-02 18:18:54.000000 angreal-2.0.6/src/utils.rs
--rw-r--r--   0      501       20      672 2023-03-02 18:18:54.000000 angreal-2.0.6/tests/common/mod.rs
--rw-r--r--   0      501       20       28 2023-03-02 18:18:54.000000 angreal-2.0.6/tests/common/test_assets/bad_import_init.py
--rw-r--r--   0      501       20       28 2023-03-02 18:18:54.000000 angreal-2.0.6/tests/common/test_assets/bad_import_task.py
--rw-r--r--   0      501       20       34 2023-03-02 18:18:54.000000 angreal-2.0.6/tests/common/test_assets/exception_init.py
--rw-r--r--   0      501       20       32 2023-03-02 18:18:54.000000 angreal-2.0.6/tests/common/test_assets/exception_task.py
--rw-r--r--   0      501       20        0 2023-03-02 18:18:54.000000 angreal-2.0.6/tests/common/test_assets/good_init.py
--rw-r--r--   0      501       20      130 2023-03-02 18:18:54.000000 angreal-2.0.6/tests/common/test_assets/good_task.py
--rw-r--r--   0      501       20        0 2023-03-02 18:18:54.000000 angreal-2.0.6/tests/common/test_assets/internal_module/__init__.py
--rw-r--r--   0      501       20       30 2023-03-02 18:18:54.000000 angreal-2.0.6/tests/common/test_assets/no_func_init.py
--rw-r--r--   0      501       20       30 2023-03-02 18:18:54.000000 angreal-2.0.6/tests/common/test_assets/no_func_task.py
--rw-r--r--   0      501       20        0 2023-03-02 18:18:54.000000 angreal-2.0.6/tests/common/test_assets/test_template/.wee
--rw-r--r--   0      501       20      115 2023-03-02 18:18:54.000000 angreal-2.0.6/tests/common/test_assets/test_template/angreal.toml
--rw-r--r--   0      501       20       21 2023-03-02 18:18:54.000000 angreal-2.0.6/tests/common/test_assets/test_template/{{ folder_variable }}/.angreal/init.py
--rw-r--r--   0      501       20       19 2023-03-02 18:18:54.000000 angreal-2.0.6/tests/common/test_assets/test_template/{{ folder_variable }}/README.rst
--rw-r--r--   0      501       20    60345 2023-03-02 18:22:16.000000 angreal-2.0.6/Cargo.lock
--rw-r--r--   0        0        0     3740 1970-01-01 00:00:00.000000 angreal-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 angreal-2.0.7/Cargo.toml
+-rw-r--r--   0      501       20     1461 2023-07-22 20:15:55.000000 angreal-2.0.7/.angreal/task_run_tests.py
+-rw-r--r--   0      501       20      394 2023-07-22 20:15:55.000000 angreal-2.0.7/.angreal/task_setup.py
+-rw-r--r--   0      501       20     1778 2023-07-22 20:15:55.000000 angreal-2.0.7/.github/workflows/docs.yaml
+-rw-r--r--   0      501       20     7958 2023-07-22 20:15:55.000000 angreal-2.0.7/.github/workflows/release.yaml
+-rw-r--r--   0      501       20     3698 2023-07-22 20:15:55.000000 angreal-2.0.7/.github/workflows/test.yaml
+-rw-r--r--   0      501       20     5668 2023-07-22 20:15:55.000000 angreal-2.0.7/.gitignore
+-rw-r--r--   0      501       20     1176 2023-07-22 20:15:55.000000 angreal-2.0.7/.pre-commit-config.yaml
+-rw-r--r--   0      501       20        6 2023-07-22 20:15:55.000000 angreal-2.0.7/.spelling_wordlist.txt
+-rw-r--r--   0      501       20      887 2023-07-22 20:15:55.000000 angreal-2.0.7/.yamllint-config.yml
+-rw-r--r--   0      501       20     2563 2023-07-22 20:15:55.000000 angreal-2.0.7/README.md
+-rw-r--r--   0      501       20      825 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/_draft/how_to/include-jinja-templates.rst.md
+-rw-r--r--   0      501       20      365 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/_draft/how_to/use-docker-integration.rst.md
+-rw-r--r--   0      501       20      548 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/_draft/how_to/use-git-integration.rst.md
+-rw-r--r--   0      501       20      864 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/_draft/how_to/work_with_virtual_environments.rst.md
+-rw-r--r--   0      501       20       83 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/archetypes/default.md
+-rw-r--r--   0      501       20     2787 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/config.toml
+-rw-r--r--   0      501       20     2551 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/_index.md
+-rw-r--r--   0      501       20      493 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/api_reference/_index.md
+-rw-r--r--   0      501       20       55 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/api_reference/py_angreal/_index.md
+-rw-r--r--   0      501       20     2122 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/api_reference/py_angreal/argument_decorator.md
+-rw-r--r--   0      501       20      645 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/api_reference/py_angreal/command_decorator.md
+-rw-r--r--   0      501       20     1125 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/api_reference/py_angreal/command_group.md
+-rw-r--r--   0      501       20      318 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/api_reference/py_angreal/get_root.md
+-rw-r--r--   0      501       20      473 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/api_reference/py_angreal/required_version.md
+-rw-r--r--   0      501       20       64 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/available_templates/_index.md
+-rw-r--r--   0      501       20     3212 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/code_of_conduct/_index.md
+-rw-r--r--   0      501       20     1311 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/contributing/_index.md
+-rw-r--r--   0      501       20       56 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/discussions/_index.md
+-rw-r--r--   0      501       20       58 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/how-to/_index.md
+-rw-r--r--   0      501       20     4380 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/how-to/add_arguments.md
+-rw-r--r--   0      501       20      321 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/how-to/create_a_task.md
+-rw-r--r--   0      501       20      560 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/how-to/create_task_group.md
+-rw-r--r--   0      501       20       63 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/tutorials/_index.md
+-rw-r--r--   0      501       20       69 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/tutorials/meeting_notes.files/angreal.toml
+-rw-r--r--   0      501       20       62 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/tutorials/meeting_notes.files/{{ name }}/.angreal/init.py
+-rw-r--r--   0      501       20     1254 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/tutorials/meeting_notes.files/{{ name }}/.angreal/task_take_notes.py
+-rw-r--r--   0      501       20       85 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/tutorials/meeting_notes.files/{{ name }}/README.md
+-rw-r--r--   0      501       20     5274 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/tutorials/your-first-angreal.md
+-rw-r--r--   0      501       20     5660 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/content/why/_index.md
+-rw-r--r--   0      501       20      198 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/layouts/partials/logo.html
+-rw-r--r--   0      501       20     6445 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/static/images/wheel.png
+-rw-r--r--   0      501       20     1139 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/LICENSE.md
+-rw-r--r--   0      501       20      169 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/archetypes/chapter.md
+-rw-r--r--   0      501       20       99 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/archetypes/default.md
+-rw-r--r--   0      501       20      585 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/i18n/ar.toml
+-rw-r--r--   0      501       20      507 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/i18n/de.toml
+-rw-r--r--   0      501       20      487 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/i18n/en.toml
+-rw-r--r--   0      501       20      484 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/i18n/es.toml
+-rw-r--r--   0      501       20      531 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/i18n/fr.toml
+-rw-r--r--   0      501       20      726 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/i18n/hi.toml
+-rw-r--r--   0      501       20      499 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/i18n/id.toml
+-rw-r--r--   0      501       20      514 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/i18n/ja.toml
+-rw-r--r--   0      501       20      499 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/i18n/nl.toml
+-rw-r--r--   0      501       20      490 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/i18n/pt.toml
+-rw-r--r--   0      501       20      623 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/i18n/ru.toml
+-rw-r--r--   0      501       20      495 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/i18n/tr.toml
+-rw-r--r--   0      501       20      710 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/i18n/vn.toml
+-rw-r--r--   0      501       20      484 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/i18n/zh-cn.toml
+-rw-r--r--   0      501       20   284162 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/images/screenshot.png
+-rw-r--r--   0      501       20   143335 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/images/tn.png
+-rw-r--r--   0      501       20     2263 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/404.html
+-rw-r--r--   0      501       20      550 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/_default/list.html
+-rw-r--r--   0      501       20      354 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/_default/single.html
+-rw-r--r--   0      501       20     1384 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/index.html
+-rw-r--r--   0      501       20      429 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/index.json
+-rw-r--r--   0      501       20       78 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/partials/custom-comments.html
+-rw-r--r--   0      501       20      180 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/partials/custom-footer.html
+-rw-r--r--   0      501       20      148 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/partials/custom-header.html
+-rw-r--r--   0      501       20       76 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/partials/favicon.html
+-rw-r--r--   0      501       20     4539 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/partials/footer.html
+-rw-r--r--   0      501       20     5312 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/partials/header.html
+-rw-r--r--   0      501       20      137 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/partials/logo.html
+-rw-r--r--   0      501       20      193 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/partials/menu-footer.html
+-rw-r--r--   0      501       20     6236 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/partials/menu.html
+-rw-r--r--   0      501       20      215 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/partials/meta.html
+-rw-r--r--   0      501       20      911 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/partials/search.html
+-rw-r--r--   0      501       20      172 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/partials/tags.html
+-rw-r--r--   0      501       20       90 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/partials/toc.html
+-rw-r--r--   0      501       20     1176 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/shortcodes/attachments.html
+-rw-r--r--   0      501       20      452 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/shortcodes/button.html
+-rw-r--r--   0      501       20     4463 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/shortcodes/children.html
+-rw-r--r--   0      501       20      730 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/shortcodes/expand.html
+-rw-r--r--   0      501       20      164 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/shortcodes/mermaid.html
+-rw-r--r--   0      501       20      151 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/shortcodes/notice.html
+-rw-r--r--   0      501       20      441 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/shortcodes/ref.html
+-rw-r--r--   0      501       20      441 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/shortcodes/relref.html
+-rw-r--r--   0      501       20      191 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/shortcodes/siteparam.html
+-rw-r--r--   0      501       20      369 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/shortcodes/tab.html
+-rw-r--r--   0      501       20      793 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/shortcodes/tabs.html
+-rw-r--r--   0      501       20     1588 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/atom-one-dark-reasonable.css
+-rw-r--r--   0      501       20      890 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/auto-complete.css
+-rw-r--r--   0      501       20     1869 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/featherlight.min.css
+-rw-r--r--   0      501       20   101895 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/fontawesome-all.min.css
+-rw-r--r--   0      501       20     4755 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/hugo-theme.css
+-rw-r--r--   0      501       20     1342 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/hybrid.css
+-rw-r--r--   0      501       20    11887 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/nucleus.css
+-rw-r--r--   0      501       20     4629 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/perfect-scrollbar.min.css
+-rw-r--r--   0      501       20      859 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/tabs.css
+-rw-r--r--   0      501       20     1010 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/tags.css
+-rw-r--r--   0      501       20     4088 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/theme-blue.css
+-rw-r--r--   0      501       20     4088 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/theme-green.css
+-rw-r--r--   0      501       20     4085 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/theme-red.css
+-rw-r--r--   0      501       20    24719 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/theme.css
+-rw-r--r--   0      501       20    35620 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.eot
+-rw-r--r--   0      501       20    61991 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.svg
+-rw-r--r--   0      501       20    63184 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.ttf
+-rw-r--r--   0      501       20    38248 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.woff
+-rw-r--r--   0      501       20    22446 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.eot
+-rw-r--r--   0      501       20    98610 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.svg
+-rw-r--r--   0      501       20    56884 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.ttf
+-rw-r--r--   0      501       20    24772 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.woff
+-rw-r--r--   0      501       20    19760 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.woff2
+-rw-r--r--   0      501       20    21080 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.eot
+-rw-r--r--   0      501       20    91969 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.svg
+-rw-r--r--   0      501       20    55600 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.ttf
+-rw-r--r--   0      501       20    23476 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.woff
+-rw-r--r--   0      501       20    18716 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.woff2
+-rw-r--r--   0      501       20    24290 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.eot
+-rw-r--r--   0      501       20    54839 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.svg
+-rw-r--r--   0      501       20    49752 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.ttf
+-rw-r--r--   0      501       20    25896 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.woff
+-rw-r--r--   0      501       20    21128 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.woff2
+-rw-r--r--   0      501       20    24817 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.eot
+-rw-r--r--   0      501       20    54787 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.svg
+-rw-r--r--   0      501       20    50784 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.ttf
+-rw-r--r--   0      501       20    26392 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.woff
+-rw-r--r--   0      501       20    21548 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.woff2
+-rw-r--r--   0      501       20    26481 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.eot
+-rw-r--r--   0      501       20    54422 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.svg
+-rw-r--r--   0      501       20    54232 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.ttf
+-rw-r--r--   0      501       20    27900 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.woff
+-rw-r--r--   0      501       20    22884 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.woff2
+-rw-r--r--   0      501       20      510 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/images/clippy.svg
+-rw-r--r--   0      501       20      608 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/images/favicon.png
+-rw-r--r--   0      501       20   206249 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/images/gopher-404.jpg
+-rw-r--r--   0      501       20     5328 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/auto-complete.js
+-rw-r--r--   0      501       20    10754 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/clipboard.min.js
+-rw-r--r--   0      501       20     9296 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/featherlight.min.js
+-rw-r--r--   0      501       20    95350 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/highlight.pack.js
+-rw-r--r--   0      501       20     2847 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/hugo-learn.js
+-rw-r--r--   0      501       20    86927 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/jquery-3.3.1.min.js
+-rwxr-xr-x   0      501       20    10085 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/jquery.sticky.js
+-rw-r--r--   0      501       20    16771 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/learn.js
+-rw-r--r--   0      501       20    29528 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/lunr.min.js
+-rw-r--r--   0      501       20     7547 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/modernizr.custom-3.6.0.js
+-rw-r--r--   0      501       20    25333 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/perfect-scrollbar.jquery.min.js
+-rw-r--r--   0      501       20    25012 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/perfect-scrollbar.min.js
+-rw-r--r--   0      501       20     3443 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/search.js
+-rw-r--r--   0      501       20   832983 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/mermaid/mermaid.js
+-rw-r--r--   0      501       20   134396 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.eot
+-rw-r--r--   0      501       20   739403 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.svg
+-rw-r--r--   0      501       20   186124 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0      501       20    87048 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.woff
+-rw-r--r--   0      501       20   107656 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0      501       20    40308 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.eot
+-rw-r--r--   0      501       20   135805 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.svg
+-rw-r--r--   0      501       20    62320 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0      501       20    18164 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.woff
+-rw-r--r--   0      501       20    25236 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0      501       20   209012 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.eot
+-rw-r--r--   0      501       20   771698 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.svg
+-rw-r--r--   0      501       20   397420 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0      501       20   102224 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.woff
+-rw-r--r--   0      501       20   150516 2023-07-22 20:15:55.000000 angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.woff2
+-rw-r--r--   0      501       20        0 2023-07-22 20:15:55.000000 angreal-2.0.7/py_tests/__init__.py
+-rw-r--r--   0      501       20     2053 2023-07-22 20:15:55.000000 angreal-2.0.7/py_tests/integrations/test_docker.py
+-rw-r--r--   0      501       20      831 2023-07-22 20:15:55.000000 angreal-2.0.7/py_tests/integrations/test_git.py
+-rw-r--r--   0      501       20        6 2023-07-22 20:15:55.000000 angreal-2.0.7/py_tests/integrations/test_r.txt
+-rw-r--r--   0      501       20     2385 2023-07-22 20:15:55.000000 angreal-2.0.7/py_tests/integrations/test_venv.py
+-rw-r--r--   0      501       20     3547 2023-07-22 20:15:55.000000 angreal-2.0.7/py_tests/test_angreal.py
+-rw-r--r--   0      501       20      930 2023-07-22 20:15:55.000000 angreal-2.0.7/pyproject.toml
+-rw-r--r--   0      501       20     5041 2023-07-22 20:15:55.000000 angreal-2.0.7/python/angreal/__init__.py
+-rw-r--r--   0      501       20       68 2023-07-22 20:15:55.000000 angreal-2.0.7/python/angreal/integrations/docker/__init__.py
+-rw-r--r--   0      501       20       85 2023-07-22 20:15:55.000000 angreal-2.0.7/python/angreal/integrations/docker/container.py
+-rw-r--r--   0      501       20       74 2023-07-22 20:15:55.000000 angreal-2.0.7/python/angreal/integrations/docker/image.py
+-rw-r--r--   0      501       20       80 2023-07-22 20:15:55.000000 angreal-2.0.7/python/angreal/integrations/docker/network.py
+-rw-r--r--   0      501       20       77 2023-07-22 20:15:55.000000 angreal-2.0.7/python/angreal/integrations/docker/volume.py
+-rw-r--r--   0      501       20     2664 2023-07-22 20:15:55.000000 angreal-2.0.7/python/angreal/integrations/git.py
+-rw-r--r--   0      501       20     4782 2023-07-22 20:15:55.000000 angreal-2.0.7/python/angreal/integrations/venv.py
+-rw-r--r--   0      501       20       31 2023-07-22 20:15:55.000000 angreal-2.0.7/rust-toolchain.toml
+-rw-r--r--   0      501       20     6270 2023-07-22 20:15:55.000000 angreal-2.0.7/src/builder.rs
+-rw-r--r--   0      501       20     6547 2023-07-22 20:15:55.000000 angreal-2.0.7/src/git/mod.rs
+-rw-r--r--   0      501       20    15338 2023-07-22 20:15:55.000000 angreal-2.0.7/src/init.rs
+-rw-r--r--   0      501       20     7817 2023-07-22 20:15:55.000000 angreal-2.0.7/src/lib.rs
+-rw-r--r--   0      501       20     1284 2023-07-22 20:15:55.000000 angreal-2.0.7/src/logger.rs
+-rw-r--r--   0      501       20     1039 2023-07-22 20:15:55.000000 angreal-2.0.7/src/macros.rs
+-rw-r--r--   0      501       20     3290 2023-07-22 20:15:55.000000 angreal-2.0.7/src/py_logger.rs
+-rw-r--r--   0      501       20     8423 2023-07-22 20:15:55.000000 angreal-2.0.7/src/task.rs
+-rw-r--r--   0      501       20     7510 2023-07-22 20:15:55.000000 angreal-2.0.7/src/utils.rs
+-rw-r--r--   0      501       20      672 2023-07-22 20:15:55.000000 angreal-2.0.7/tests/common/mod.rs
+-rw-r--r--   0      501       20       41 2023-07-22 20:15:55.000000 angreal-2.0.7/tests/common/test_assets/bad_import_init.py
+-rw-r--r--   0      501       20       41 2023-07-22 20:15:55.000000 angreal-2.0.7/tests/common/test_assets/bad_import_task.py
+-rw-r--r--   0      501       20       34 2023-07-22 20:15:55.000000 angreal-2.0.7/tests/common/test_assets/exception_init.py
+-rw-r--r--   0      501       20       32 2023-07-22 20:15:55.000000 angreal-2.0.7/tests/common/test_assets/exception_task.py
+-rw-r--r--   0      501       20        0 2023-07-22 20:15:55.000000 angreal-2.0.7/tests/common/test_assets/good_init.py
+-rw-r--r--   0      501       20      109 2023-07-22 20:15:55.000000 angreal-2.0.7/tests/common/test_assets/good_task.py
+-rw-r--r--   0      501       20        0 2023-07-22 20:15:55.000000 angreal-2.0.7/tests/common/test_assets/internal_module/__init__.py
+-rw-r--r--   0      501       20       30 2023-07-22 20:15:55.000000 angreal-2.0.7/tests/common/test_assets/no_func_init.py
+-rw-r--r--   0      501       20       30 2023-07-22 20:15:55.000000 angreal-2.0.7/tests/common/test_assets/no_func_task.py
+-rw-r--r--   0      501       20        0 2023-07-22 20:15:55.000000 angreal-2.0.7/tests/common/test_assets/test_template/.wee
+-rw-r--r--   0      501       20      116 2023-07-22 20:15:55.000000 angreal-2.0.7/tests/common/test_assets/test_template/angreal.toml
+-rw-r--r--   0      501       20       21 2023-07-22 20:15:55.000000 angreal-2.0.7/tests/common/test_assets/test_template/{{ folder_variable }}/.angreal/init.py
+-rw-r--r--   0      501       20       20 2023-07-22 20:15:55.000000 angreal-2.0.7/tests/common/test_assets/test_template/{{ folder_variable }}/README.rst
+-rw-r--r--   0      501       20    72292 2023-07-22 20:15:55.000000 angreal-2.0.7/Cargo.lock
+-rw-r--r--   0        0        0     3738 1970-01-01 00:00:00.000000 angreal-2.0.7/PKG-INFO
```

### Comparing `angreal-2.0.6/.angreal/task_run_tests.py` & `angreal-2.0.7/.angreal/task_run_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,19 @@
     """
     Run tests for both cargo test and pytest
     """
     print(green + "====================" + end)
     print(green + "building" + end)
     print(green + "====================" + end)
 
-    build = subprocess.run(
+    subprocess.run(
         ["maturin build"], cwd=cwd, shell=True
     )
 
-    build = subprocess.run(
+    subprocess.run(
         ["pip install ."], cwd=cwd, shell=True
     )
 
     print(green + "====================" + end)
     print(green + "Starting Cargo tests" + end)
     print(green + "====================" + end)
 
@@ -39,13 +39,14 @@
             "cargo test -v -- --nocapture --test-threads=1",
         ], cwd=cwd, shell=True
     )
 
     print(green + "=====================" + end)
     print(green + "Starting python tests" + end)
     print(green + "=====================" + end)
-    pytest_rv = subprocess.run(["python -m pytest -svv"], cwd=cwd, shell=True)
+    pytest_rv = subprocess.run(["python3 -m pytest -svv"], cwd=cwd, shell=True)
 
     if cargo_rv.returncode or pytest_rv.returncode:
         raise RuntimeError(
-            f"Tests failed with status codes : {cargo_rv} (cargo) and {pytest_rv}(pytest)"
+            f"Tests failed with status codes : {cargo_rv}"
+            " (cargo) and {pytest_rv}(pytest)"
         )
```

### Comparing `angreal-2.0.6/.github/workflows/docs.yaml` & `angreal-2.0.7/.github/workflows/docs.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+---
 # Sample workflow for building and deploying a Hugo site to GitHub Pages
 name: "Angreal Docs Deploy"
 
-on:
+on:  # yamllint disable-line rule:truthy
   # Runs on pushes targeting the default branch
   push:
     branches: ["main"]
 
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
@@ -25,20 +26,19 @@
   run:
     shell: bash
 
 jobs:
   # Build job
   build:
     runs-on: ubuntu-latest
-    env:
-      HUGO_VERSION: 0.108.0
     steps:
       - name: Install Hugo CLI
-        run: |
-          wget -O ${{ runner.temp }}/hugo.deb https://github.com/gohugoio/hugo/releases/download/v${HUGO_VERSION}/hugo_${HUGO_VERSION}_linux-amd64.deb \
+        run: >
+          wget -O ${{ runner.temp }}/hugo.deb
+          https://github.com/gohugoio/hugo/releases/download/v0.111.3/hugo_0.111.3_linux-amd64.deb
           && sudo dpkg -i ${{ runner.temp }}/hugo.deb
       - name: Install Dart Sass Embedded
         run: sudo snap install dart-sass-embedded
       - name: Checkout
         uses: actions/checkout@v3
         with:
           fetch-depth: 0
```

### Comparing `angreal-2.0.6/.github/workflows/release.yaml` & `angreal-2.0.7/.github/workflows/release.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+---
 name: "Angreal Release"
 
-on:
+on:  # yamllint disable-line rule:truthy
   release:
     types: [published]
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 jobs:
@@ -17,15 +18,15 @@
           python-version: '3.11'
           architecture: x64
       - uses: dtolnay/rust-toolchain@stable
       - name: Build wheels - x86_64
         uses: PyO3/maturin-action@v1
         with:
           target: x86_64
-          args: --release --out dist --sdist -i 3.7 3.8 3.9 3.10 3.11 
+          args: --release --out dist --sdist -i 3.7 3.8 3.9 3.10 3.11
       - name: Install built wheel - x86_64
         run: |
           pip install angreal --no-index --find-links dist --force-reinstall
           pip install pytest
           pytest
       - name: Upload wheels
         uses: actions/upload-artifact@v3
@@ -41,15 +42,15 @@
         with:
           python-version: '3.11'
           architecture: x64
       - uses: dtolnay/rust-toolchain@stable
       - name: Build wheels - universal2
         uses: PyO3/maturin-action@v1
         with:
-          args: --release --universal2 --out dist -i 3.8 3.9 3.10 3.11 
+          args: --release --universal2 --out dist -i 3.8 3.9 3.10 3.11
       - name: Install built wheel - universal2
         run: |
           pip install angreal --no-index --find-links dist --force-reinstall
           pip install pytest
           pytest
       - name: Upload wheels
         uses: actions/upload-artifact@v3
@@ -60,15 +61,15 @@
   windows:
     runs-on: windows-latest
     name: windows (${{ matrix.platform.target }})
     strategy:
       matrix:
         platform:
           - target: x64
-            interpreter: 3.7 3.8 3.9 3.10 3.11 
+            interpreter: 3.7 3.8 3.9 3.10 3.11
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: '3.11'
           architecture: ${{ matrix.platform.target }}
       - uses: dtolnay/rust-toolchain@stable
@@ -90,150 +91,150 @@
 
   linux:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         target: [x86_64, i686]
     steps:
-    - uses: actions/checkout@v3
-    - uses: actions/setup-python@v4
-      with:
-        python-version: '3.11'
-        architecture: x64
-    - name: Build wheels
-      uses: PyO3/maturin-action@v1
-      with:
-        rust-toolchain: stable
-        target: ${{ matrix.target }}
-        manylinux: auto
-        args: --release --out dist -i 3.7 3.8 3.9 3.10 3.11 
-    - name: Install built wheel
-      if: matrix.target == 'x86_64'
-      run: |
-        pip install angreal --no-index --find-links dist --force-reinstall
-        pip install pytest
-        pytest
-    - name: Upload wheels
-      uses: actions/upload-artifact@v3
-      with:
-        name: wheels
-        path: dist
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
+        with:
+          python-version: '3.11'
+          architecture: x64
+      - name: Build wheels
+        uses: PyO3/maturin-action@v1
+        with:
+          rust-toolchain: stable
+          target: ${{ matrix.target }}
+          manylinux: auto
+          args: --release --out dist -i 3.7 3.8 3.9 3.10 3.11
+      - name: Install built wheel
+        if: matrix.target == 'x86_64'
+        run: |
+          pip install angreal --no-index --find-links dist --force-reinstall
+          pip install pytest
+          pytest
+      - name: Upload wheels
+        uses: actions/upload-artifact@v3
+        with:
+          name: wheels
+          path: dist
 
   linux-cross:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         target: [aarch64, armv7, s390x, ppc64le]
     steps:
-    - uses: actions/checkout@v3
-    - uses: actions/setup-python@v4
-      with:
-        python-version: '3.11'
-    - name: Build wheels
-      uses: PyO3/maturin-action@v1
-      with:
-        rust-toolchain: stable
-        target: ${{ matrix.target }}
-        manylinux: auto
-        args: --release --out dist -i 3.7 3.8 3.9 3.10 3.11 
-    - uses: uraimo/run-on-arch-action@v2.3.0
-      if: matrix.target != 'ppc64'
-      name: Install built wheel
-      with:
-        arch: ${{ matrix.target }}
-        distro: ubuntu20.04
-        githubToken: ${{ github.token }}
-        install: |
-          apt-get update
-          apt-get install -y --no-install-recommends python3 python3-pip python3-venv git
-          pip3 install -U pip pytest
-        run: |
-          pip3 install angreal --no-index --find-links dist/ --force-reinstall
-          pytest
-    - name: Upload wheels
-      uses: actions/upload-artifact@v3
-      with:
-        name: wheels
-        path: dist
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
+        with:
+          python-version: '3.11'
+      - name: Build wheels
+        uses: PyO3/maturin-action@v1
+        with:
+          rust-toolchain: stable
+          target: ${{ matrix.target }}
+          manylinux: auto
+          args: --release --out dist -i 3.7 3.8 3.9 3.10 3.11
+      - uses: uraimo/run-on-arch-action@v2.3.0
+        if: matrix.target != 'ppc64'
+        name: Install built wheel
+        with:
+          arch: ${{ matrix.target }}
+          distro: ubuntu20.04
+          githubToken: ${{ github.token }}
+          install: |
+            apt-get update
+            apt-get install -y --no-install-recommends python3 python3-pip python3-venv git
+            pip3 install -U pip pytest
+          run: |
+            pip3 install angreal --no-index --find-links dist/ --force-reinstall
+            pytest
+      - name: Upload wheels
+        uses: actions/upload-artifact@v3
+        with:
+          name: wheels
+          path: dist
 
   musllinux:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         target:
           - x86_64-unknown-linux-musl
           - i686-unknown-linux-musl
     steps:
-    - uses: actions/checkout@v3
-    - uses: actions/setup-python@v4
-      with:
-        python-version: '3.11'
-        architecture: x64
-    - name: Build wheels
-      uses: PyO3/maturin-action@v1
-      with:
-        rust-toolchain: stable
-        target: ${{ matrix.target }}
-        manylinux: musllinux_1_2
-        args: --release --out dist -i 3.7 3.8 3.9 3.10 3.11
-    - name: Install built wheel
-      if: matrix.target == 'x86_64-unknown-linux-musl'
-      uses: addnab/docker-run-action@v3
-      with:
-        image: alpine:latest
-        options: -v ${{ github.workspace }}:/io -w /io
-        run: |
-          apk add py3-pip
-          pip3 install -U pip pytest
-          pip3 install angreal --no-index --find-links /io/dist/ --force-reinstall
-          
-    - name: Upload wheels
-      uses: actions/upload-artifact@v3
-      with:
-        name: wheels
-        path: dist
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
+        with:
+          python-version: '3.11'
+          architecture: x64
+      - name: Build wheels
+        uses: PyO3/maturin-action@v1
+        with:
+          rust-toolchain: stable
+          target: ${{ matrix.target }}
+          manylinux: musllinux_1_2
+          args: --release --out dist -i 3.7 3.8 3.9 3.10 3.11
+      - name: Install built wheel
+        if: matrix.target == 'x86_64-unknown-linux-musl'
+        uses: addnab/docker-run-action@v3
+        with:
+          image: alpine:latest
+          options: -v ${{ github.workspace }}:/io -w /io
+          run: |
+            apk add py3-pip
+            pip3 install -U pip pytest
+            pip3 install angreal --no-index --find-links /io/dist/ --force-reinstall
+
+      - name: Upload wheels
+        uses: actions/upload-artifact@v3
+        with:
+          name: wheels
+          path: dist
 
   musllinux-cross:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         platform:
           - target: aarch64-unknown-linux-musl
             arch: aarch64
           - target: armv7-unknown-linux-musleabihf
             arch: armv7
     steps:
-    - uses: actions/checkout@v3
-    - uses: actions/setup-python@v4
-      with:
-        python-version: '3.11'
-    - name: Build wheels
-      uses: PyO3/maturin-action@v1
-      with:
-        rust-toolchain: stable
-        target: ${{ matrix.platform.target }}
-        manylinux: musllinux_1_2
-        args: --release --out dist -i 3.7 3.8 3.9 3.10 3.11
-    - uses: uraimo/run-on-arch-action@v2.3.0
-      name: Install built wheel
-      with:
-        arch: ${{ matrix.platform.arch }}
-        distro: alpine_latest
-        githubToken: ${{ github.token }}
-        install: |
-          apk add py3-pip
-          pip3 install -U pip pytest
-        run: |
-          pip3 install angreal --no-index --find-links dist/ --force-reinstall
-          
-    - name: Upload wheels
-      uses: actions/upload-artifact@v3
-      with:
-        name: wheels
-        path: dist
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
+        with:
+          python-version: '3.11'
+      - name: Build wheels
+        uses: PyO3/maturin-action@v1
+        with:
+          rust-toolchain: stable
+          target: ${{ matrix.platform.target }}
+          manylinux: musllinux_1_2
+          args: --release --out dist -i 3.7 3.8 3.9 3.10 3.11
+      - uses: uraimo/run-on-arch-action@v2.3.0
+        name: Install built wheel
+        with:
+          arch: ${{ matrix.platform.arch }}
+          distro: alpine_latest
+          githubToken: ${{ github.token }}
+          install: |
+            apk add py3-pip
+            pip3 install -U pip pytest
+          run: |
+            pip3 install angreal --no-index --find-links dist/ --force-reinstall
+
+      - name: Upload wheels
+        uses: actions/upload-artifact@v3
+        with:
+          name: wheels
+          path: dist
 
   release-pypi:
     name: Release
     runs-on: ubuntu-latest
     needs:
       - macos-universal
       - macos-x86_64
@@ -265,15 +266,15 @@
       - windows
       - linux
       - linux-cross
       - musllinux
       - musllinux-cross
     if: "startsWith(github.ref, 'refs/tags/')"
     steps:
-    - uses: actions/checkout@v3
-    - uses: actions-rs/toolchain@v1
-      with:
+      - uses: actions/checkout@v3
+      - uses: actions-rs/toolchain@v1
+        with:
           toolchain: stable
           override: true
-    - uses: katyo/publish-crates@v2
-      with:
+      - uses: katyo/publish-crates@v2
+        with:
           registry-token: ${{ secrets.CARGO_REGISTRY_TOKEN }}
```

### Comparing `angreal-2.0.6/.github/workflows/test.yaml` & `angreal-2.0.7/.github/workflows/test.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,98 +1,93 @@
+---
 name: "Angreal Tests"
 
-on:
+on:  # yamllint disable-line rule:truthy
   push:
     branches:
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref_name }}-${{ github.event.pull_request.number || github.sha }}
   cancel-in-progress: true
 
 env:
   CARGO_INCREMENTAL: 0
   CARGO_NET_RETRY: 10
   RUSTUP_MAX_RETRIES: 10
 
 jobs:
-  cargo-build:
-    name: "cargo build"
+  pre-commit:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - name: Checkout
+        uses: actions/checkout@v3
       - uses: actions-rs/toolchain@v1
         with:
           profile: minimal
           toolchain: nightly-2022-11-01
           override: true
-      - uses: Swatinem/rust-cache@v1
-      - run: cargo build --all
-
-  cargo-fmt:
-    name: "cargo fmt"
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v3
-      - uses: actions-rs/toolchain@v1
+          components: rustfmt, clippy
+      - uses: pre-commit/action@v3.0.0
         with:
-          profile: minimal
-          toolchain: nightly-2022-11-01
-          override: true
-          components: rustfmt
-      - run: cargo fmt --all --check
+          extra_args: --all-files
 
-  cargo_clippy:
-    name: "cargo clippy"
+  cargo-build:
+    name: "cargo build"
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions-rs/toolchain@v1
         with:
           profile: minimal
           toolchain: nightly-2022-11-01
           override: true
-          components: clippy
       - uses: Swatinem/rust-cache@v1
-      - run: cargo clippy --workspace --all-targets --all-features
-  
+      - run: cargo build --all
+
   angreal-tests-linux:
     name: "angreal run-tests linux"
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions-rs/toolchain@v1
         with:
           profile: minimal
           toolchain: 1.65.0
           override: true
       - uses: Swatinem/rust-cache@v1
+      - uses: webfactory/ssh-agent@v0.7.0
+        with:
+          ssh-private-key: ${{ secrets.SSH_PRIVATE_KEY }}
       - uses: actions/setup-python@v4
         with:
           python-version: "3.11"
-      - run: pip install maturin pytest 
-      - run: maturin build 
+      - run: pip install maturin pytest
+      - run: maturin build
       - run: pip install .
       - run: angreal run-tests
 
   angreal-tests-windows:
     name: "angreal run-tests windows"
     runs-on: windows-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions-rs/toolchain@v1
         with:
           profile: minimal
           toolchain: 1.65.0
           override: true
       - uses: Swatinem/rust-cache@v1
+      - uses: webfactory/ssh-agent@v0.7.0
+        with:
+          ssh-private-key: ${{ secrets.SSH_PRIVATE_KEY }}
       - uses: actions/setup-python@v4
         with:
           python-version: "3.11"
-      - run: pip install maturin pytest 
-      - run: maturin build 
+      - run: pip install maturin pytest
+      - run: maturin build
       - run: pip install .
       - run: cargo test -v -- --nocapture --test-threads=1
       - run: python -m pytest -svv
 
   angreal-tests-macosx:
     name: "angreal run-tests macos"
     runs-on: macos-11
@@ -100,42 +95,45 @@
       - uses: actions/checkout@v3
       - uses: actions-rs/toolchain@v1
         with:
           profile: minimal
           toolchain: 1.65.0
           override: true
       - uses: Swatinem/rust-cache@v1
+      - uses: webfactory/ssh-agent@v0.7.0
+        with:
+          ssh-private-key: ${{ secrets.SSH_PRIVATE_KEY }}
       - uses: actions/setup-python@v4
         with:
           python-version: "3.11"
-      - run: pip install maturin pytest 
-      - run: maturin build 
+      - run: pip install maturin pytest
+      - run: maturin build
       - run: pip install .
-      # - run: cargo test -v -- --nocapture --test-threads=1 ## the linking thing is messing with cargo test
+      - run: cargo test -v -- --nocapture --test-threads=1
       - run: python -m pytest -svv
-  
+
   typos:
     name: Spell Check with Typos
     runs-on: ubuntu-latest
     steps:
-    - name: Checkout Actions Repository
-      uses: actions/checkout@v2
-    - name: Spell Check
-      uses: crate-ci/typos@master
-      with:
-        files: ./src
-    - name: Spell Check
-      uses: crate-ci/typos@master
-      with:
-        files: ./docs/content
-    - name: Spell Check
-      uses: crate-ci/typos@master
-      with:
-        files: ./python
-    - name: Spell Check
-      uses: crate-ci/typos@master
-      with:
-        files: ./py_tests
-    - name: Spell Check
-      uses: crate-ci/typos@master
-      with:
-        files: ./tests
+      - name: Checkout Actions Repository
+        uses: actions/checkout@v2
+      - name: Spell Check
+        uses: crate-ci/typos@master
+        with:
+          files: ./src
+      - name: Spell Check
+        uses: crate-ci/typos@master
+        with:
+          files: ./docs/content
+      - name: Spell Check
+        uses: crate-ci/typos@master
+        with:
+          files: ./python
+      - name: Spell Check
+        uses: crate-ci/typos@master
+        with:
+          files: ./py_tests
+      - name: Spell Check
+        uses: crate-ci/typos@master
+        with:
+          files: ./tests
```

### Comparing `angreal-2.0.6/.gitignore` & `angreal-2.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/README.md` & `angreal-2.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [![image](https://img.shields.io/pypi/v/angreal.svg)](https://pypi.python.org/pypi/angreal)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/angreal)
 [![image](https://img.shields.io/pypi/l/angreal.svg)](https://pypi.python.org/pypi/angreal)
 [![Angreal Tests](https://github.com/angreal/angreal/actions/workflows/test.yaml/badge.svg?branch=main)](https://github.com/angreal/angreal/actions/workflows/test.yaml)
 [![Angreal Docs Deploy](https://github.com/angreal/angreal/actions/workflows/docs.yaml/badge.svg)](https://github.com/angreal/angreal/actions/workflows/docs.yaml)
 [![Angreal Release](https://github.com/angreal/angreal/actions/workflows/release.yaml/badge.svg?event=release)](https://github.com/angreal/angreal/actions/workflows/release.yaml)
 ---
-[Docs are available here.](https://angreal.github.io/angreal/) 
+[Docs are available here.](https://angreal.github.io/angreal/)
 
 ## Angreal is meant to:
 - allow the consistent creation of projects
 - provide consistent methods for interacting with projects
 
 ### Quick Start
 
@@ -18,15 +18,15 @@
 2.  Initialize a project from a template
 3.  Use the template
 
 ```bash
 $: pip install 'angreal>=2' #pip install angreal will also work
 $: angreal init https://github.com/angreal/python
 ```
---- 
+---
 
 
 ## What is it?
 
 Angreal is an attempt to solve two problems that I was running into in
 both my personal and professional life as a data scientist and software
 developer. I do things often enough that they needed automation, I
@@ -41,14 +41,14 @@
 of executing methods for interacting with that project in a consistent
 manner. These methods (called tasks) travel with the project so while
 templated initially, they\'re customizable to the project - allowing some
 level of flexibility in how a task functions between projects.
 
 ### Why 2.0 ?
 
-The original angreal was built ontop of a number of python modules that
+The original angreal was built on top of a number of python modules that
 were under active development and used by a number of other projects.
 The nature of the application itself meant that core application found
 itself in dependency hell regularly - and became rather annoying to use.
 The 2.0.0 release is a complete rewrite that uses
-[Rust](https://www.rust-lang.org/) to provide a compiled binary with the goal that it will 
+[Rust](https://www.rust-lang.org/) to provide a compiled binary with the goal that it will
 require no external python dependencies.
```

### Comparing `angreal-2.0.6/docs/_draft/how_to/include-jinja-templates.rst.md` & `angreal-2.0.7/docs/_draft/how_to/include-jinja-templates.rst.md`

 * *Files 0% similar despite different names*

```diff
@@ -36,9 +36,9 @@
 will render as
 
 ``` {.sourceCode .bash}
 ├── README.md
 ├── VERSION
 ├── angreal.json
 ├── setup.py
-└── {{ angreal.name }} 
+└── {{ angreal.name }}
 ```
```

### Comparing `angreal-2.0.6/docs/_draft/how_to/use-git-integration.rst.md` & `angreal-2.0.7/docs/_draft/how_to/use-git-integration.rst.md`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/_draft/how_to/work_with_virtual_environments.rst.md` & `angreal-2.0.7/docs/_draft/how_to/work_with_virtual_environments.rst.md`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/config.toml` & `angreal-2.0.7/docs/config.toml`

 * *Files 0% similar despite different names*

```diff
@@ -69,8 +69,7 @@
 weight = 10
 
 
 [[menu.shortcuts]]
 name = "<i class='fa fa-download'></i> Download"
 url = "https://github.com/angreal/angreal/archive/refs/heads/main.zip"
 weight = 20
-
```

### Comparing `angreal-2.0.6/docs/content/_index.md` & `angreal-2.0.7/docs/content/_index.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ---
 title: Angreal Home
 type: page
 ---
 
 # Angreal
---- 
+---
 
 ## Angreal is meant to:
 - allow the consistent creation of projects
 - provide consistent methods for interacting with projects
 
 ### Quick Start
 
@@ -16,15 +16,15 @@
 2.  Initialize a project from a template
 3.  Use the template
 
 ```bash
 $: pip install 'angreal>=2' #pip install angreal will also work
 $: angreal init https://github.com/angreal/python.git
 ```
---- 
+---
 
 ## What is it?
 
 Angreal is an attempt to solve two problems that I was running into in
 both my personal and professional life as a data scientist and software
 developer. I do things often enough that they needed automation, I
 don\'t do things so often that I remember all of the steps/commands I
@@ -38,23 +38,23 @@
 of executing methods for interacting with that project in a consistent
 manner. These methods (called tasks) travel with the project so while
 templated initially, they\'re customizable to the project - allowing some
 level of flexibility in how a task functions between projects.
 
 ### Why 2.0 ?
 
-The original angreal was built ontop of a number of python modules that
+The original angreal was built on top of a number of python modules that
 were under active development and used by a number of other projects.
 The nature of the application itself meant that core application found
 itself in dependency hell regularly - and became rather annoying to use.
 The 2.0.0 release is a complete rewrite that uses
-[Rust](https://www.rust-lang.org/) to provide a compiled binary with the goal that it will 
+[Rust](https://www.rust-lang.org/) to provide a compiled binary with the goal that it will
 require no external python dependencies.
 
 
 <!-- [![image](https://img.shields.io/pypi/v/angreal.svg)](https://pypi.python.org/pypi/angreal)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/angreal) 
+![PyPI - Downloads](https://img.shields.io/pypi/dm/angreal)
 [![image](https://img.shields.io/pypi/l/angreal.svg)](https://pypi.python.org/pypi/angreal)
 [![Angreal Tests](https://github.com/angreal/angreal/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/angreal/angreal/actions/workflows/ci.yaml)
 [![Angreal Docs Deploy](https://github.com/angreal/angreal/actions/workflows/docs.yaml/badge.svg)](https://github.com/angreal/angreal/actions/workflows/docs.yaml)
 [![Angreal Release](https://github.com/angreal/angreal/actions/workflows/release.yaml/badge.svg?event=release)](https://github.com/angreal/angreal/actions/workflows/release.yaml)
  -->
```

### Comparing `angreal-2.0.6/docs/content/code_of_conduct/_index.md` & `angreal-2.0.7/docs/content/code_of_conduct/_index.md`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/content/contributing/_index.md` & `angreal-2.0.7/docs/content/contributing/_index.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 1. `pip install angreal`, install angreal for executing our defined tasks
 1. `angreal bootstrap-dev`, setup your environment
 1. `angreal run-tests`, run our test suite
 
 
 ### Windows Development Support
 
-I did not have windows in mind when writing initial angreal tasks, they may (probably) won't work 
+I did not have windows in mind when writing initial angreal tasks, they may (probably) won't work
 well out of the box.
 
 1. When running `maturin develop` you may see failures in the build chain due to OpenSSL not being installed. Installing [StrawberryPerl](https://strawberryperl.com/)
-SHOULD take care of that for you. 
+SHOULD take care of that for you.
 
 2. Tests can be run via `cargo test` and `pytest`.
-
```

### Comparing `angreal-2.0.6/docs/content/how-to/add_arguments.md` & `angreal-2.0.7/docs/content/how-to/add_arguments.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,40 +6,40 @@
 First, all control mechanisms for commands are managed by a single decorator called `@argument`. The full signature for this decorator is:
 
 - __name__: the argument name, must match the provided arg/kwarg in the wrapped python function (_Required_)
 - __python_type__: the python type to apply when passing to the wrapped function. Must be one of ("str", "int", "float"), __default__ "str"
 - __takes_value__: does the argument consumer a trailing value, __default__ True
 - __default_value__: the default value to apply if none is provided, __default__ None
 - __require_equals__: the applied value requires an equal sign (i.e. `--arg=value` ), __default__ None
-- __multiple_values__: the argument takes multiple values, __default__ None 
+- __multiple_values__: the argument takes multiple values, __default__ None
 - __number_of_values__: the argument takes a specific number of values, __default__ None
 - __max_values__: the argument takes at most X values, __default__ None
-- __min_values__: the argument takes at min X values, __default__ None 
+- __min_values__: the argument takes at min X values, __default__ None
 - __short__: the short name for the argument, a single character (i.e. `-i` in the CLI would be 'i'), __default__ None
 - __long__: the long name for the argument, a single word (i.e. `--information` in the CLI would be 'information'), __default__ None
 - __long_help__: the help message to show when a long help message is requested via `--help`, __default__ None
 - __help__: the short help message to show during failure or when `-h` is requested, __default__ None
 - __required__: whether this argument is required at run time, __default__ None
 
 
-## Arguments 
+## Arguments
 
 Arguments are positional after the defined command.
 
 ```python
 import angreal
 
 @angreal.command(name="echo", about="an echo replacement")
 @angreal.argument(name="phrase", help="the phrase to echo", required=True)
 def task_echo(phrase):
     print(phrase)
 ```
 
 ```bash
-angreal echo --help                                                                                                                           ─╯ 
+angreal echo --help                                                                                                                           ─╯
 echo
 an echo replacement
 
 USAGE:
     echo <phrase>
 
 ARGS:
@@ -71,17 +71,17 @@
     if color=="green":
         print(green + phrase + end )
         return
     print(phrase)
 ```
 
 ```bash
-$ angreal echo --help                                                                                                                           ─╯ 
+$ angreal echo --help                                                                                                                           ─╯
 
-echo 
+echo
 an echo replacement
 
 USAGE:
     echo [OPTIONS] <phrase>
 
 ARGS:
     <phrase>    the phrase to echo
@@ -89,15 +89,15 @@
 OPTIONS:
     -c, --color <color>    apply a color to the echo phrase
     -h, --help             Print help information
 ```
 
 ## Flags
 
-A flag is just a binary value that will set a resulting value to True without taking a value. 
+A flag is just a binary value that will set a resulting value to True without taking a value.
 
 ```python
 import angreal
 
 green = "\33[32m"
 red = "\33[31m"
 end = "\33[0m"
@@ -117,23 +117,23 @@
     if color=="green":
         print(green + phrase + end )
         return
     print(phrase)
 ```
 
 ```bash
-$ angreal echo --help                                                                                                                           ─╯ 
+$ angreal echo --help                                                                                                                           ─╯
 
 echo
 an echo replacement
 
 USAGE:
     echo [OPTIONS] <phrase>
 
 ARGS:
     <phrase>    the phrase to echo
 
 OPTIONS:
     -c, --color <color>    apply a color to the echo phrase
     -h, --help             Print help information
     -y, --yell             yell it from the tree tops
-```
+```
```

### Comparing `angreal-2.0.6/docs/content/tutorials/meeting_notes.files/{{ name }}/.angreal/task_take_notes.py` & `angreal-2.0.7/docs/content/tutorials/meeting_notes.files/{{ name }}/.angreal/task_take_notes.py`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/content/tutorials/your-first-angreal.md` & `angreal-2.0.7/docs/content/tutorials/your-first-angreal.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 -   on creation a folder with the meeting name will be created
 -   on creation a file that introduces us to the reason the meetings
     exist as an initial README.
 -   a task to take minutes using an editor
 
 ## Template Layout
 
-Based on the above planned requirements we'll need files and folders created as follows : 
+Based on the above planned requirements we'll need files and folders created as follows :
 
 ```bash
 meeting_notes
 ├── angreal.toml
 └── {{ name }}
     ├── .angreal
     │   ├── init.py
     │   └── task_take_notes.py
     └── README.md
 ```
 ## `angreal.toml`
 
-The `angreal.toml` file tells angreal what variables it needs to template and provides default values for them. 
-Our template will have the following variables: 
+The `angreal.toml` file tells angreal what variables it needs to template and provides default values for them.
+Our template will have the following variables:
 - name
 - cadence
 - standing_agenda
 
 ```toml
 name="another_meeting"
 cadence="weekly"
@@ -58,15 +58,15 @@
 
 {{ standing_agenda }}
 ```
 
 
 ## `init.py`
 {{% notice info %}}
-**Optional:** In this very trivial example, not much happens after the folder structure is created so the init isn't required. 
+**Optional:** In this very trivial example, not much happens after the folder structure is created so the init isn't required.
 {{% /notice %}}
 
 ```python
 def init():
     print("Initializing {{ name }} !")
     return
 ```
@@ -91,18 +91,18 @@
 @angreal.argument(name='now',long='now', takes_value=False)
 def angreal_cmd(now=False):
     """
     create a file for taking minutes
     """
     file_name = datetime.datetime.today().strftime('%Y-%m-%d-%H-%M')
 
-    # We're going to assume that you're running on ubuntu 
-    # which has a binary called "editor" that will launch your 
+    # We're going to assume that you're running on ubuntu
+    # which has a binary called "editor" that will launch your
     # default terminal editor. If you need something else - set the environment
-    # variable "EDITOR" to the appropriate command 
+    # variable "EDITOR" to the appropriate command
     editor = os.environ.get('EDITOR','editor')
 
     # Create our default file template using the current time as a header
     (fd, path) = tempfile.mkstemp()
     with open(fd, 'w') as default:
         print('# {}'.format(file_name), file=default)
 
@@ -115,28 +115,28 @@
     with open(file_name+'.md', 'a') as dst:
         with open(path,'r') as src:
             print(src.read(),file=dst)
 
     # Clean up behind our selves
     os.unlink(path)
 ```
-A brief explanation of this code: 
-    - import angreal and other libraries 
+A brief explanation of this code:
+    - import angreal and other libraries
     - decorate a function with the `command`
     - we decorate the same function with an `argument`
 
-The function itself: 
+The function itself:
 - determines the current date/time
 - tries to get an EDITOR variable from the environment, falling back to the `editor` command from Ubuntu
 - if you pass the `--now` argument, opens a temporary file using your editor
 - saves the notes taken to a file with the date and time the minutes were started.
 
 ## Using our Angreal
 
-1. Initialize our template. 
+1. Initialize our template.
 ```bash
 $ angreal init docs/content/tutorials/meeting_notes
 
 cadence? ["weekly"]
 >
 name? ["another_meeting"]
 > Hall of the Tower
@@ -148,15 +148,15 @@
 ```bash
 $ tree 'Hall of the Tower'
 Hall of the Tower
 └── README.md
 ```
 
 ```bash
-$ cat Hall\ of\ the\ Tower/README.md                                                                                                            ─╯ 
+$ cat Hall\ of\ the\ Tower/README.md                                                                                                            ─╯
 # Hall of the Tower
 
 
 ## Cadence
 
 Weekly
 
@@ -167,15 +167,15 @@
 
 ```
 
 2. What commands do i have access to ?
 
 ```bash
 $ cd 'Hall of the Tower'
-$ angreal 
+$ angreal
 
 angreal 2.0.0-rc.1
 
 USAGE:
     angreal <SUBCOMMAND>
 
 OPTIONS:
@@ -188,15 +188,15 @@
     take-notes    Take notes for our meeting
 
 ```
 
 3. How do i use `take-notes` ?
 
 ```bash
-$ angreal take-notes --help                                                                                                                  
+$ angreal take-notes --help
 
 take-notes
 
     create a file for taking minutes
 
 
 USAGE:
@@ -216,11 +216,10 @@
 $ export EDITOR='vim'
 $ angreal take-minutes --now
 ```
 
 This will open an editor (vim if you set the `EDITOR` variable) write a note.
 
 ```
-$ ls                                                                                                                                            ─╯ 
+$ ls                                                                                                                                            ─╯
 2023-01-19-09-19.md  README.md
 ```
-
```

### Comparing `angreal-2.0.6/docs/content/why/_index.md` & `angreal-2.0.7/docs/content/why/_index.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     described template into a usable form. Templates can exist in one of
     three locations : local directories, remote git repositories, or
     pypi modules. Where an angreal template is distributed from is
     decided by whomever made that particular template.
 
 ```bash
 # initialize and render the template angreal at the remote URI
-$: angreal init https://github.com/angreal/python.git   
+$: angreal init https://github.com/angreal/python.git
 # If you've used this template before you simply need to ...
-$: angreal init python 
+$: angreal init python
 ```
 
 2.  **Execution** : Executing an angreal task through the `angreal`
     command line interface. This can only happen after the template has
     been rendered.
 
 ```bash
@@ -56,15 +56,15 @@
 
 You identify that the python3 angreal fits your needs well and choose to
 use it.
 
 1.  You initialize the project with :
 
 ```bash
-$: angreal init https://github.com/angreal/python.git   
+$: angreal init https://github.com/angreal/python.git
 ```
 
 2.  You provide values for template variables with the interactive CLI :
 
 ```bash
 author_name? ["Your name"]
 Dylan Storey
@@ -75,15 +75,15 @@
 project_name? ["Name of the project (will be shown e.g. as the title in the readme)"]
 Angreal Python Demo
 project_slug? ["angreal-python-demo"] #enter accepts the provided devault value
 
 package_name? ["angreal_python_demo"]
 
 project_short_description? ["A short description of the project"]
-A demo project 
+A demo project
 ```
 
 3.  Angreal creates a project for you, using your provided variables to
     fill in some of the blanks.
 
 ```bash
 cd angreal-python-demo && tree
@@ -107,15 +107,15 @@
 
 4 directories, 12 files
 ```
 
 4.  Next lets find out what tasks come with the template
 
 ```bash
-$: angreal                                                                                                                                       ─╯ 
+$: angreal                                                                                                                                       ─╯
 angreal 2.0.0-rc.1
 
 USAGE:
     angreal [OPTIONS] <SUBCOMMAND>
 
 OPTIONS:
     -h, --help       Print help information
@@ -138,16 +138,16 @@
 ```bash
 $: angreal run-tests --open
 
 ================================================================ test session starts ================================================================platform linux -- Python 3.8.10, pytest-7.2.0, pluggy-1.0.0 -- /home/dstorey/.venvs/angreal-2/bin/python3
 cachedir: .pytest_cache
 rootdir: /home/dstorey/angreal-python-demo, configfile: setup.cfg
 plugins: cov-4.0.0
-collected 0 items                                                                                                                                    
-/home/dstorey/.venvs/angreal-2/lib/python3.8/site-packages/coverage/control.py:836: CoverageWarning: No data was collected. (no-data-collected)      
+collected 0 items
+/home/dstorey/.venvs/angreal-2/lib/python3.8/site-packages/coverage/control.py:836: CoverageWarning: No data was collected. (no-data-collected)
   self._warn("No data was collected.", slug="no-data-collected")
 
 
 ---------- coverage: platform linux, python 3.8.10-final-0 -----------
 Name                              Stmts   Miss  Cover
 -----------------------------------------------------
 angreal_python_demo/__init__.py       1      1     0%
@@ -164,8 +164,8 @@
     make sure you\'re setup :
 
 ```bash
 $: pip install angreal
 $: git clone https://github.com/dylanbstorey/angreal-test-project
 $: cd angreal-test-project
 $: angreal dev-setup
-```
+```
```

### Comparing `angreal-2.0.6/docs/static/images/wheel.png` & `angreal-2.0.7/docs/static/images/wheel.png`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/LICENSE.md` & `angreal-2.0.7/docs/themes/hugo-theme-learn/LICENSE.md`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/i18n/ar.toml` & `angreal-2.0.7/docs/themes/hugo-theme-learn/i18n/ar.toml`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/i18n/fr.toml` & `angreal-2.0.7/docs/themes/hugo-theme-learn/i18n/fr.toml`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/i18n/hi.toml` & `angreal-2.0.7/docs/themes/hugo-theme-learn/i18n/hi.toml`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/i18n/ja.toml` & `angreal-2.0.7/docs/themes/hugo-theme-learn/i18n/ja.toml`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/i18n/ru.toml` & `angreal-2.0.7/docs/themes/hugo-theme-learn/i18n/ru.toml`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/i18n/vn.toml` & `angreal-2.0.7/docs/themes/hugo-theme-learn/i18n/vn.toml`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/images/screenshot.png` & `angreal-2.0.7/docs/themes/hugo-theme-learn/images/screenshot.png`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/images/tn.png` & `angreal-2.0.7/docs/themes/hugo-theme-learn/images/tn.png`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/404.html` & `angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/404.html`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/_default/list.html` & `angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/_default/list.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 <footer class=" footline" >
 	{{with .Params.LastModifierDisplayName}}
 	    <i class='fas fa-user'></i> <a href="mailto:{{ $.Params.LastModifierEmail }}">{{ . }}</a> {{with $.Date}} <i class='fas fa-calendar'></i> {{ .Format "02/01/2006" }}{{end}}
 	    </div>
 	{{end}}
 </footer>
 
-{{ partial "footer.html" . }}
+{{ partial "footer.html" . }}
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/index.html` & `angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {{ partial "header.html" . }}
 <span id="sidebar-toggle-span">
 <a href="#" id="sidebar-toggle" data-sidebar-toggle=""><i class="fas fa-bars"></i> navigation</a>
 </span>
 
-{{if .Site.Home.Content }} 
-{{.Site.Home.Content}}	
-{{else}}           
+{{if .Site.Home.Content }}
+{{.Site.Home.Content}}
+{{else}}
 	{{if eq .Site.Language.Lang "fr"}}
 		<h1>Personaliser la page d'accueil</h1>
 		<p>
 		  Le site fonctionne. Ne pas oublier de personaliser cette page avec votre propre contenu. 3 manières de faire :
 		</p>
 		<ul>
 			<li><b>1. </b> Créer un fichier _index.md dans le dossier <b>content</b> et le remplir de Markdown</li>
@@ -23,9 +23,9 @@
 		</p>
 		<ul>
 			<li><b>1. </b> Create an _index.md document in <b>content</b> folder and fill it with Markdown content</li>
 			<li><b>2. </b> Create an <b>index.html</b> file in the <b>static</b> folder and fill the file with HTML content</li>
 		  <li><b>3. </b> Configure your server to automatically redirect home page to one your documentation page</li>
 		</ul>
 	{{end}}
-{{ end }}  
+{{ end }}
 {{ partial "footer.html" . }}
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/partials/footer.html` & `angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/partials/footer.html`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/partials/header.html` & `angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/partials/header.html`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/partials/menu.html` & `angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/partials/menu.html`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/partials/search.html` & `angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/partials/search.html`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/shortcodes/attachments.html` & `angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/shortcodes/attachments.html`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/shortcodes/children.html` & `angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/shortcodes/children.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -92,8 +92,8 @@
 
 				{{if eq $.style "li"}}
 </ul>
 				{{end}}
 			{{end}}
 		{{end}}
 	{{end}}
-{{end}}
+{{end}}
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/shortcodes/expand.html` & `angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/shortcodes/expand.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
     	{{.Get 0 | default $expandMessage}}
     	{{end}}
     	</span>
     </div>
     <div class="expand-content" style="display: none;">
         {{.Inner | safeHTML}}
     </div>
-</div>
+</div>
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/layouts/shortcodes/tabs.html` & `angreal-2.0.7/docs/themes/hugo-theme-learn/layouts/shortcodes/tabs.html`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/atom-one-dark-reasonable.css` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/atom-one-dark-reasonable.css`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/auto-complete.css` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/auto-complete.css`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     position: absolute;
     display: none;
     z-index: 9999;
     max-height: 254px;
     overflow: hidden;
     overflow-y: auto;
     box-sizing: border-box;
-    
+
 }
 .autocomplete-suggestion {
     position: relative;
     cursor: pointer;
     padding: 7px;
     line-height: 23px;
     white-space: nowrap;
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/featherlight.min.css` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/featherlight.min.css`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 /**
  * Featherlight - ultra slim jQuery lightbox
  * Version 1.7.13 - http://noelboss.github.io/featherlight/
  *
  * Copyright 2018, Noël Raoul Bossart (http://www.noelboss.com)
  * MIT Licensed.
 **/
-html.with-featherlight{overflow:hidden}.featherlight{display:none;position:fixed;top:0;right:0;bottom:0;left:0;z-index:2147483647;text-align:center;white-space:nowrap;cursor:pointer;background:#333;background:rgba(0,0,0,0)}.featherlight:last-of-type{background:rgba(0,0,0,.8)}.featherlight:before{content:'';display:inline-block;height:100%;vertical-align:middle}.featherlight .featherlight-content{position:relative;text-align:left;vertical-align:middle;display:inline-block;overflow:auto;padding:25px 25px 0;border-bottom:25px solid transparent;margin-left:5%;margin-right:5%;max-height:95%;background:#fff;cursor:auto;white-space:normal}.featherlight .featherlight-inner{display:block}.featherlight link.featherlight-inner,.featherlight script.featherlight-inner,.featherlight style.featherlight-inner{display:none}.featherlight .featherlight-close-icon{position:absolute;z-index:9999;top:0;right:0;line-height:25px;width:25px;cursor:pointer;text-align:center;font-family:Arial,sans-serif;background:#fff;background:rgba(255,255,255,.3);color:#000;border:0;padding:0}.featherlight .featherlight-close-icon::-moz-focus-inner{border:0;padding:0}.featherlight .featherlight-image{width:100%}.featherlight-iframe .featherlight-content{border-bottom:0;padding:0;-webkit-overflow-scrolling:touch}.featherlight iframe{border:0}.featherlight *{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}@media only screen and (max-width:1024px){.featherlight .featherlight-content{margin-left:0;margin-right:0;max-height:98%;padding:10px 10px 0;border-bottom:10px solid transparent}}@media print{html.with-featherlight>*>:not(.featherlight){display:none}}
+html.with-featherlight{overflow:hidden}.featherlight{display:none;position:fixed;top:0;right:0;bottom:0;left:0;z-index:2147483647;text-align:center;white-space:nowrap;cursor:pointer;background:#333;background:rgba(0,0,0,0)}.featherlight:last-of-type{background:rgba(0,0,0,.8)}.featherlight:before{content:'';display:inline-block;height:100%;vertical-align:middle}.featherlight .featherlight-content{position:relative;text-align:left;vertical-align:middle;display:inline-block;overflow:auto;padding:25px 25px 0;border-bottom:25px solid transparent;margin-left:5%;margin-right:5%;max-height:95%;background:#fff;cursor:auto;white-space:normal}.featherlight .featherlight-inner{display:block}.featherlight link.featherlight-inner,.featherlight script.featherlight-inner,.featherlight style.featherlight-inner{display:none}.featherlight .featherlight-close-icon{position:absolute;z-index:9999;top:0;right:0;line-height:25px;width:25px;cursor:pointer;text-align:center;font-family:Arial,sans-serif;background:#fff;background:rgba(255,255,255,.3);color:#000;border:0;padding:0}.featherlight .featherlight-close-icon::-moz-focus-inner{border:0;padding:0}.featherlight .featherlight-image{width:100%}.featherlight-iframe .featherlight-content{border-bottom:0;padding:0;-webkit-overflow-scrolling:touch}.featherlight iframe{border:0}.featherlight *{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}@media only screen and (max-width:1024px){.featherlight .featherlight-content{margin-left:0;margin-right:0;max-height:98%;padding:10px 10px 0;border-bottom:10px solid transparent}}@media print{html.with-featherlight>*>:not(.featherlight){display:none}}
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/fontawesome-all.min.css` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/fontawesome-all.min.css`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 /*!
  * Font Awesome Free 6.2.1 by @fontawesome - https://fontawesome.com
  * License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License)
  * Copyright 2022 Fonticons, Inc.
  */
-.fa{font-family:var(--fa-style-family,"Font Awesome 6 Free");font-weight:var(--fa-style,900)}.fa,.fa-brands,.fa-classic,.fa-regular,.fa-sharp,.fa-solid,.fab,.far,.fas{-moz-osx-font-smoothing:grayscale;-webkit-font-smoothing:antialiased;display:var(--fa-display,inline-block);font-style:normal;font-variant:normal;line-height:1;text-rendering:auto}.fa-classic,.fa-regular,.fa-solid,.far,.fas{font-family:"Font Awesome 6 Free"}.fa-brands,.fab{font-family:"Font Awesome 6 Brands"}.fa-1x{font-size:1em}.fa-2x{font-size:2em}.fa-3x{font-size:3em}.fa-4x{font-size:4em}.fa-5x{font-size:5em}.fa-6x{font-size:6em}.fa-7x{font-size:7em}.fa-8x{font-size:8em}.fa-9x{font-size:9em}.fa-10x{font-size:10em}.fa-2xs{font-size:.625em;line-height:.1em;vertical-align:.225em}.fa-xs{font-size:.75em;line-height:.08333em;vertical-align:.125em}.fa-sm{font-size:.875em;line-height:.07143em;vertical-align:.05357em}.fa-lg{font-size:1.25em;line-height:.05em;vertical-align:-.075em}.fa-xl{font-size:1.5em;line-height:.04167em;vertical-align:-.125em}.fa-2xl{font-size:2em;line-height:.03125em;vertical-align:-.1875em}.fa-fw{text-align:center;width:1.25em}.fa-ul{list-style-type:none;margin-left:var(--fa-li-margin,2.5em);padding-left:0}.fa-ul>li{position:relative}.fa-li{left:calc(var(--fa-li-width, 2em)*-1);position:absolute;text-align:center;width:var(--fa-li-width,2em);line-height:inherit}.fa-border{border-radius:var(--fa-border-radius,.1em);border:var(--fa-border-width,.08em) var(--fa-border-style,solid) var(--fa-border-color,#eee);padding:var(--fa-border-padding,.2em .25em .15em)}.fa-pull-left{float:left;margin-right:var(--fa-pull-margin,.3em)}.fa-pull-right{float:right;margin-left:var(--fa-pull-margin,.3em)}.fa-beat{-webkit-animation-name:fa-beat;animation-name:fa-beat;-webkit-animation-delay:var(--fa-animation-delay,0s);animation-delay:var(--fa-animation-delay,0s);-webkit-animation-direction:var(--fa-animation-direction,normal);animation-direction:var(--fa-animation-direction,normal);-webkit-animation-duration:var(--fa-animation-duration,1s);animation-duration:var(--fa-animation-duration,1s);-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,ease-in-out);animation-timing-function:var(--fa-animation-timing,ease-in-out)}.fa-bounce{-webkit-animation-name:fa-bounce;animation-name:fa-bounce;-webkit-animation-delay:var(--fa-animation-delay,0s);animation-delay:var(--fa-animation-delay,0s);-webkit-animation-direction:var(--fa-animation-direction,normal);animation-direction:var(--fa-animation-direction,normal);-webkit-animation-duration:var(--fa-animation-duration,1s);animation-duration:var(--fa-animation-duration,1s);-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,cubic-bezier(.28,.84,.42,1));animation-timing-function:var(--fa-animation-timing,cubic-bezier(.28,.84,.42,1))}.fa-fade{-webkit-animation-name:fa-fade;animation-name:fa-fade;-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,cubic-bezier(.4,0,.6,1));animation-timing-function:var(--fa-animation-timing,cubic-bezier(.4,0,.6,1))}.fa-beat-fade,.fa-fade{-webkit-animation-delay:var(--fa-animation-delay,0s);animation-delay:var(--fa-animation-delay,0s);-webkit-animation-direction:var(--fa-animation-direction,normal);animation-direction:var(--fa-animation-direction,normal);-webkit-animation-duration:var(--fa-animation-duration,1s);animation-duration:var(--fa-animation-duration,1s)}.fa-beat-fade{-webkit-animation-name:fa-beat-fade;animation-name:fa-beat-fade;-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,cubic-bezier(.4,0,.6,1));animation-timing-function:var(--fa-animation-timing,cubic-bezier(.4,0,.6,1))}.fa-flip{-webkit-animation-name:fa-flip;animation-name:fa-flip;-webkit-animation-delay:var(--fa-animation-delay,0s);animation-delay:var(--fa-animation-delay,0s);-webkit-animation-direction:var(--fa-animation-direction,normal);animation-direction:var(--fa-animation-direction,normal);-webkit-animation-duration:var(--fa-animation-duration,1s);animation-duration:var(--fa-animation-duration,1s);-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,ease-in-out);animation-timing-function:var(--fa-animation-timing,ease-in-out)}.fa-shake{-webkit-animation-name:fa-shake;animation-name:fa-shake;-webkit-animation-duration:var(--fa-animation-duration,1s);animation-duration:var(--fa-animation-duration,1s);-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,linear);animation-timing-function:var(--fa-animation-timing,linear)}.fa-shake,.fa-spin{-webkit-animation-delay:var(--fa-animation-delay,0s);animation-delay:var(--fa-animation-delay,0s);-webkit-animation-direction:var(--fa-animation-direction,normal);animation-direction:var(--fa-animation-direction,normal)}.fa-spin{-webkit-animation-name:fa-spin;animation-name:fa-spin;-webkit-animation-duration:var(--fa-animation-duration,2s);animation-duration:var(--fa-animation-duration,2s);-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,linear);animation-timing-function:var(--fa-animation-timing,linear)}.fa-spin-reverse{--fa-animation-direction:reverse}.fa-pulse,.fa-spin-pulse{-webkit-animation-name:fa-spin;animation-name:fa-spin;-webkit-animation-direction:var(--fa-animation-direction,normal);animation-direction:var(--fa-animation-direction,normal);-webkit-animation-duration:var(--fa-animation-duration,1s);animation-duration:var(--fa-animation-duration,1s);-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,steps(8));animation-timing-function:var(--fa-animation-timing,steps(8))}@media (prefers-reduced-motion:reduce){.fa-beat,.fa-beat-fade,.fa-bounce,.fa-fade,.fa-flip,.fa-pulse,.fa-shake,.fa-spin,.fa-spin-pulse{-webkit-animation-delay:-1ms;animation-delay:-1ms;-webkit-animation-duration:1ms;animation-duration:1ms;-webkit-animation-iteration-count:1;animation-iteration-count:1;transition-delay:0s;transition-duration:0s}}@-webkit-keyframes fa-beat{0%,90%{-webkit-transform:scale(1);transform:scale(1)}45%{-webkit-transform:scale(var(--fa-beat-scale,1.25));transform:scale(var(--fa-beat-scale,1.25))}}@keyframes fa-beat{0%,90%{-webkit-transform:scale(1);transform:scale(1)}45%{-webkit-transform:scale(var(--fa-beat-scale,1.25));transform:scale(var(--fa-beat-scale,1.25))}}@-webkit-keyframes fa-bounce{0%{-webkit-transform:scale(1) translateY(0);transform:scale(1) translateY(0)}10%{-webkit-transform:scale(var(--fa-bounce-start-scale-x,1.1),var(--fa-bounce-start-scale-y,.9)) translateY(0);transform:scale(var(--fa-bounce-start-scale-x,1.1),var(--fa-bounce-start-scale-y,.9)) translateY(0)}30%{-webkit-transform:scale(var(--fa-bounce-jump-scale-x,.9),var(--fa-bounce-jump-scale-y,1.1)) translateY(var(--fa-bounce-height,-.5em));transform:scale(var(--fa-bounce-jump-scale-x,.9),var(--fa-bounce-jump-scale-y,1.1)) translateY(var(--fa-bounce-height,-.5em))}50%{-webkit-transform:scale(var(--fa-bounce-land-scale-x,1.05),var(--fa-bounce-land-scale-y,.95)) translateY(0);transform:scale(var(--fa-bounce-land-scale-x,1.05),var(--fa-bounce-land-scale-y,.95)) translateY(0)}57%{-webkit-transform:scale(1) translateY(var(--fa-bounce-rebound,-.125em));transform:scale(1) translateY(var(--fa-bounce-rebound,-.125em))}64%{-webkit-transform:scale(1) translateY(0);transform:scale(1) translateY(0)}to{-webkit-transform:scale(1) translateY(0);transform:scale(1) translateY(0)}}@keyframes fa-bounce{0%{-webkit-transform:scale(1) translateY(0);transform:scale(1) translateY(0)}10%{-webkit-transform:scale(var(--fa-bounce-start-scale-x,1.1),var(--fa-bounce-start-scale-y,.9)) translateY(0);transform:scale(var(--fa-bounce-start-scale-x,1.1),var(--fa-bounce-start-scale-y,.9)) translateY(0)}30%{-webkit-transform:scale(var(--fa-bounce-jump-scale-x,.9),var(--fa-bounce-jump-scale-y,1.1)) translateY(var(--fa-bounce-height,-.5em));transform:scale(var(--fa-bounce-jump-scale-x,.9),var(--fa-bounce-jump-scale-y,1.1)) translateY(var(--fa-bounce-height,-.5em))}50%{-webkit-transform:scale(var(--fa-bounce-land-scale-x,1.05),var(--fa-bounce-land-scale-y,.95)) translateY(0);transform:scale(var(--fa-bounce-land-scale-x,1.05),var(--fa-bounce-land-scale-y,.95)) translateY(0)}57%{-webkit-transform:scale(1) translateY(var(--fa-bounce-rebound,-.125em));transform:scale(1) translateY(var(--fa-bounce-rebound,-.125em))}64%{-webkit-transform:scale(1) translateY(0);transform:scale(1) translateY(0)}to{-webkit-transform:scale(1) translateY(0);transform:scale(1) translateY(0)}}@-webkit-keyframes fa-fade{50%{opacity:var(--fa-fade-opacity,.4)}}@keyframes fa-fade{50%{opacity:var(--fa-fade-opacity,.4)}}@-webkit-keyframes fa-beat-fade{0%,to{opacity:var(--fa-beat-fade-opacity,.4);-webkit-transform:scale(1);transform:scale(1)}50%{opacity:1;-webkit-transform:scale(var(--fa-beat-fade-scale,1.125));transform:scale(var(--fa-beat-fade-scale,1.125))}}@keyframes fa-beat-fade{0%,to{opacity:var(--fa-beat-fade-opacity,.4);-webkit-transform:scale(1);transform:scale(1)}50%{opacity:1;-webkit-transform:scale(var(--fa-beat-fade-scale,1.125));transform:scale(var(--fa-beat-fade-scale,1.125))}}@-webkit-keyframes fa-flip{50%{-webkit-transform:rotate3d(var(--fa-flip-x,0),var(--fa-flip-y,1),var(--fa-flip-z,0),var(--fa-flip-angle,-180deg));transform:rotate3d(var(--fa-flip-x,0),var(--fa-flip-y,1),var(--fa-flip-z,0),var(--fa-flip-angle,-180deg))}}@keyframes fa-flip{50%{-webkit-transform:rotate3d(var(--fa-flip-x,0),var(--fa-flip-y,1),var(--fa-flip-z,0),var(--fa-flip-angle,-180deg));transform:rotate3d(var(--fa-flip-x,0),var(--fa-flip-y,1),var(--fa-flip-z,0),var(--fa-flip-angle,-180deg))}}@-webkit-keyframes fa-shake{0%{-webkit-transform:rotate(-15deg);transform:rotate(-15deg)}4%{-webkit-transform:rotate(15deg);transform:rotate(15deg)}8%,24%{-webkit-transform:rotate(-18deg);transform:rotate(-18deg)}12%,28%{-webkit-transform:rotate(18deg);transform:rotate(18deg)}16%{-webkit-transform:rotate(-22deg);transform:rotate(-22deg)}20%{-webkit-transform:rotate(22deg);transform:rotate(22deg)}32%{-webkit-transform:rotate(-12deg);transform:rotate(-12deg)}36%{-webkit-transform:rotate(12deg);transform:rotate(12deg)}40%,to{-webkit-transform:rotate(0deg);transform:rotate(0deg)}}@keyframes fa-shake{0%{-webkit-transform:rotate(-15deg);transform:rotate(-15deg)}4%{-webkit-transform:rotate(15deg);transform:rotate(15deg)}8%,24%{-webkit-transform:rotate(-18deg);transform:rotate(-18deg)}12%,28%{-webkit-transform:rotate(18deg);transform:rotate(18deg)}16%{-webkit-transform:rotate(-22deg);transform:rotate(-22deg)}20%{-webkit-transform:rotate(22deg);transform:rotate(22deg)}32%{-webkit-transform:rotate(-12deg);transform:rotate(-12deg)}36%{-webkit-transform:rotate(12deg);transform:rotate(12deg)}40%,to{-webkit-transform:rotate(0deg);transform:rotate(0deg)}}@-webkit-keyframes fa-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}}@keyframes fa-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}}.fa-rotate-90{-webkit-transform:rotate(90deg);transform:rotate(90deg)}.fa-rotate-180{-webkit-transform:rotate(180deg);transform:rotate(180deg)}.fa-rotate-270{-webkit-transform:rotate(270deg);transform:rotate(270deg)}.fa-flip-horizontal{-webkit-transform:scaleX(-1);transform:scaleX(-1)}.fa-flip-vertical{-webkit-transform:scaleY(-1);transform:scaleY(-1)}.fa-flip-both,.fa-flip-horizontal.fa-flip-vertical{-webkit-transform:scale(-1);transform:scale(-1)}.fa-rotate-by{-webkit-transform:rotate(var(--fa-rotate-angle,none));transform:rotate(var(--fa-rotate-angle,none))}.fa-stack{display:inline-block;height:2em;line-height:2em;position:relative;vertical-align:middle;width:2.5em}.fa-stack-1x,.fa-stack-2x{left:0;position:absolute;text-align:center;width:100%;z-index:var(--fa-stack-z-index,auto)}.fa-stack-1x{line-height:inherit}.fa-stack-2x{font-size:2em}.fa-inverse{color:var(--fa-inverse,#fff)}.fa-0:before{content:"\30"}.fa-1:before{content:"\31"}.fa-2:before{content:"\32"}.fa-3:before{content:"\33"}.fa-4:before{content:"\34"}.fa-5:before{content:"\35"}.fa-6:before{content:"\36"}.fa-7:before{content:"\37"}.fa-8:before{content:"\38"}.fa-9:before{content:"\39"}.fa-fill-drip:before{content:"\f576"}.fa-arrows-to-circle:before{content:"\e4bd"}.fa-chevron-circle-right:before,.fa-circle-chevron-right:before{content:"\f138"}.fa-at:before{content:"\40"}.fa-trash-alt:before,.fa-trash-can:before{content:"\f2ed"}.fa-text-height:before{content:"\f034"}.fa-user-times:before,.fa-user-xmark:before{content:"\f235"}.fa-stethoscope:before{content:"\f0f1"}.fa-comment-alt:before,.fa-message:before{content:"\f27a"}.fa-info:before{content:"\f129"}.fa-compress-alt:before,.fa-down-left-and-up-right-to-center:before{content:"\f422"}.fa-explosion:before{content:"\e4e9"}.fa-file-alt:before,.fa-file-lines:before,.fa-file-text:before{content:"\f15c"}.fa-wave-square:before{content:"\f83e"}.fa-ring:before{content:"\f70b"}.fa-building-un:before{content:"\e4d9"}.fa-dice-three:before{content:"\f527"}.fa-calendar-alt:before,.fa-calendar-days:before{content:"\f073"}.fa-anchor-circle-check:before{content:"\e4aa"}.fa-building-circle-arrow-right:before{content:"\e4d1"}.fa-volleyball-ball:before,.fa-volleyball:before{content:"\f45f"}.fa-arrows-up-to-line:before{content:"\e4c2"}.fa-sort-desc:before,.fa-sort-down:before{content:"\f0dd"}.fa-circle-minus:before,.fa-minus-circle:before{content:"\f056"}.fa-door-open:before{content:"\f52b"}.fa-right-from-bracket:before,.fa-sign-out-alt:before{content:"\f2f5"}.fa-atom:before{content:"\f5d2"}.fa-soap:before{content:"\e06e"}.fa-heart-music-camera-bolt:before,.fa-icons:before{content:"\f86d"}.fa-microphone-alt-slash:before,.fa-microphone-lines-slash:before{content:"\f539"}.fa-bridge-circle-check:before{content:"\e4c9"}.fa-pump-medical:before{content:"\e06a"}.fa-fingerprint:before{content:"\f577"}.fa-hand-point-right:before{content:"\f0a4"}.fa-magnifying-glass-location:before,.fa-search-location:before{content:"\f689"}.fa-forward-step:before,.fa-step-forward:before{content:"\f051"}.fa-face-smile-beam:before,.fa-smile-beam:before{content:"\f5b8"}.fa-flag-checkered:before{content:"\f11e"}.fa-football-ball:before,.fa-football:before{content:"\f44e"}.fa-school-circle-exclamation:before{content:"\e56c"}.fa-crop:before{content:"\f125"}.fa-angle-double-down:before,.fa-angles-down:before{content:"\f103"}.fa-users-rectangle:before{content:"\e594"}.fa-people-roof:before{content:"\e537"}.fa-people-line:before{content:"\e534"}.fa-beer-mug-empty:before,.fa-beer:before{content:"\f0fc"}.fa-diagram-predecessor:before{content:"\e477"}.fa-arrow-up-long:before,.fa-long-arrow-up:before{content:"\f176"}.fa-burn:before,.fa-fire-flame-simple:before{content:"\f46a"}.fa-male:before,.fa-person:before{content:"\f183"}.fa-laptop:before{content:"\f109"}.fa-file-csv:before{content:"\f6dd"}.fa-menorah:before{content:"\f676"}.fa-truck-plane:before{content:"\e58f"}.fa-record-vinyl:before{content:"\f8d9"}.fa-face-grin-stars:before,.fa-grin-stars:before{content:"\f587"}.fa-bong:before{content:"\f55c"}.fa-pastafarianism:before,.fa-spaghetti-monster-flying:before{content:"\f67b"}.fa-arrow-down-up-across-line:before{content:"\e4af"}.fa-spoon:before,.fa-utensil-spoon:before{content:"\f2e5"}.fa-jar-wheat:before{content:"\e517"}.fa-envelopes-bulk:before,.fa-mail-bulk:before{content:"\f674"}.fa-file-circle-exclamation:before{content:"\e4eb"}.fa-circle-h:before,.fa-hospital-symbol:before{content:"\f47e"}.fa-pager:before{content:"\f815"}.fa-address-book:before,.fa-contact-book:before{content:"\f2b9"}.fa-strikethrough:before{content:"\f0cc"}.fa-k:before{content:"\4b"}.fa-landmark-flag:before{content:"\e51c"}.fa-pencil-alt:before,.fa-pencil:before{content:"\f303"}.fa-backward:before{content:"\f04a"}.fa-caret-right:before{content:"\f0da"}.fa-comments:before{content:"\f086"}.fa-file-clipboard:before,.fa-paste:before{content:"\f0ea"}.fa-code-pull-request:before{content:"\e13c"}.fa-clipboard-list:before{content:"\f46d"}.fa-truck-loading:before,.fa-truck-ramp-box:before{content:"\f4de"}.fa-user-check:before{content:"\f4fc"}.fa-vial-virus:before{content:"\e597"}.fa-sheet-plastic:before{content:"\e571"}.fa-blog:before{content:"\f781"}.fa-user-ninja:before{content:"\f504"}.fa-person-arrow-up-from-line:before{content:"\e539"}.fa-scroll-torah:before,.fa-torah:before{content:"\f6a0"}.fa-broom-ball:before,.fa-quidditch-broom-ball:before,.fa-quidditch:before{content:"\f458"}.fa-toggle-off:before{content:"\f204"}.fa-archive:before,.fa-box-archive:before{content:"\f187"}.fa-person-drowning:before{content:"\e545"}.fa-arrow-down-9-1:before,.fa-sort-numeric-desc:before,.fa-sort-numeric-down-alt:before{content:"\f886"}.fa-face-grin-tongue-squint:before,.fa-grin-tongue-squint:before{content:"\f58a"}.fa-spray-can:before{content:"\f5bd"}.fa-truck-monster:before{content:"\f63b"}.fa-w:before{content:"\57"}.fa-earth-africa:before,.fa-globe-africa:before{content:"\f57c"}.fa-rainbow:before{content:"\f75b"}.fa-circle-notch:before{content:"\f1ce"}.fa-tablet-alt:before,.fa-tablet-screen-button:before{content:"\f3fa"}.fa-paw:before{content:"\f1b0"}.fa-cloud:before{content:"\f0c2"}.fa-trowel-bricks:before{content:"\e58a"}.fa-face-flushed:before,.fa-flushed:before{content:"\f579"}.fa-hospital-user:before{content:"\f80d"}.fa-tent-arrow-left-right:before{content:"\e57f"}.fa-gavel:before,.fa-legal:before{content:"\f0e3"}.fa-binoculars:before{content:"\f1e5"}.fa-microphone-slash:before{content:"\f131"}.fa-box-tissue:before{content:"\e05b"}.fa-motorcycle:before{content:"\f21c"}.fa-bell-concierge:before,.fa-concierge-bell:before{content:"\f562"}.fa-pen-ruler:before,.fa-pencil-ruler:before{content:"\f5ae"}.fa-people-arrows-left-right:before,.fa-people-arrows:before{content:"\e068"}.fa-mars-and-venus-burst:before{content:"\e523"}.fa-caret-square-right:before,.fa-square-caret-right:before{content:"\f152"}.fa-cut:before,.fa-scissors:before{content:"\f0c4"}.fa-sun-plant-wilt:before{content:"\e57a"}.fa-toilets-portable:before{content:"\e584"}.fa-hockey-puck:before{content:"\f453"}.fa-table:before{content:"\f0ce"}.fa-magnifying-glass-arrow-right:before{content:"\e521"}.fa-digital-tachograph:before,.fa-tachograph-digital:before{content:"\f566"}.fa-users-slash:before{content:"\e073"}.fa-clover:before{content:"\e139"}.fa-mail-reply:before,.fa-reply:before{content:"\f3e5"}.fa-star-and-crescent:before{content:"\f699"}.fa-house-fire:before{content:"\e50c"}.fa-minus-square:before,.fa-square-minus:before{content:"\f146"}.fa-helicopter:before{content:"\f533"}.fa-compass:before{content:"\f14e"}.fa-caret-square-down:before,.fa-square-caret-down:before{content:"\f150"}.fa-file-circle-question:before{content:"\e4ef"}.fa-laptop-code:before{content:"\f5fc"}.fa-swatchbook:before{content:"\f5c3"}.fa-prescription-bottle:before{content:"\f485"}.fa-bars:before,.fa-navicon:before{content:"\f0c9"}.fa-people-group:before{content:"\e533"}.fa-hourglass-3:before,.fa-hourglass-end:before{content:"\f253"}.fa-heart-broken:before,.fa-heart-crack:before{content:"\f7a9"}.fa-external-link-square-alt:before,.fa-square-up-right:before{content:"\f360"}.fa-face-kiss-beam:before,.fa-kiss-beam:before{content:"\f597"}.fa-film:before{content:"\f008"}.fa-ruler-horizontal:before{content:"\f547"}.fa-people-robbery:before{content:"\e536"}.fa-lightbulb:before{content:"\f0eb"}.fa-caret-left:before{content:"\f0d9"}.fa-circle-exclamation:before,.fa-exclamation-circle:before{content:"\f06a"}.fa-school-circle-xmark:before{content:"\e56d"}.fa-arrow-right-from-bracket:before,.fa-sign-out:before{content:"\f08b"}.fa-chevron-circle-down:before,.fa-circle-chevron-down:before{content:"\f13a"}.fa-unlock-alt:before,.fa-unlock-keyhole:before{content:"\f13e"}.fa-cloud-showers-heavy:before{content:"\f740"}.fa-headphones-alt:before,.fa-headphones-simple:before{content:"\f58f"}.fa-sitemap:before{content:"\f0e8"}.fa-circle-dollar-to-slot:before,.fa-donate:before{content:"\f4b9"}.fa-memory:before{content:"\f538"}.fa-road-spikes:before{content:"\e568"}.fa-fire-burner:before{content:"\e4f1"}.fa-flag:before{content:"\f024"}.fa-hanukiah:before{content:"\f6e6"}.fa-feather:before{content:"\f52d"}.fa-volume-down:before,.fa-volume-low:before{content:"\f027"}.fa-comment-slash:before{content:"\f4b3"}.fa-cloud-sun-rain:before{content:"\f743"}.fa-compress:before{content:"\f066"}.fa-wheat-alt:before,.fa-wheat-awn:before{content:"\e2cd"}.fa-ankh:before{content:"\f644"}.fa-hands-holding-child:before{content:"\e4fa"}.fa-asterisk:before{content:"\2a"}.fa-check-square:before,.fa-square-check:before{content:"\f14a"}.fa-peseta-sign:before{content:"\e221"}.fa-header:before,.fa-heading:before{content:"\f1dc"}.fa-ghost:before{content:"\f6e2"}.fa-list-squares:before,.fa-list:before{content:"\f03a"}.fa-phone-square-alt:before,.fa-square-phone-flip:before{content:"\f87b"}.fa-cart-plus:before{content:"\f217"}.fa-gamepad:before{content:"\f11b"}.fa-circle-dot:before,.fa-dot-circle:before{content:"\f192"}.fa-dizzy:before,.fa-face-dizzy:before{content:"\f567"}.fa-egg:before{content:"\f7fb"}.fa-house-medical-circle-xmark:before{content:"\e513"}.fa-campground:before{content:"\f6bb"}.fa-folder-plus:before{content:"\f65e"}.fa-futbol-ball:before,.fa-futbol:before,.fa-soccer-ball:before{content:"\f1e3"}.fa-paint-brush:before,.fa-paintbrush:before{content:"\f1fc"}.fa-lock:before{content:"\f023"}.fa-gas-pump:before{content:"\f52f"}.fa-hot-tub-person:before,.fa-hot-tub:before{content:"\f593"}.fa-map-location:before,.fa-map-marked:before{content:"\f59f"}.fa-house-flood-water:before{content:"\e50e"}.fa-tree:before{content:"\f1bb"}.fa-bridge-lock:before{content:"\e4cc"}.fa-sack-dollar:before{content:"\f81d"}.fa-edit:before,.fa-pen-to-square:before{content:"\f044"}.fa-car-side:before{content:"\f5e4"}.fa-share-alt:before,.fa-share-nodes:before{content:"\f1e0"}.fa-heart-circle-minus:before{content:"\e4ff"}.fa-hourglass-2:before,.fa-hourglass-half:before{content:"\f252"}.fa-microscope:before{content:"\f610"}.fa-sink:before{content:"\e06d"}.fa-bag-shopping:before,.fa-shopping-bag:before{content:"\f290"}.fa-arrow-down-z-a:before,.fa-sort-alpha-desc:before,.fa-sort-alpha-down-alt:before{content:"\f881"}.fa-mitten:before{content:"\f7b5"}.fa-person-rays:before{content:"\e54d"}.fa-users:before{content:"\f0c0"}.fa-eye-slash:before{content:"\f070"}.fa-flask-vial:before{content:"\e4f3"}.fa-hand-paper:before,.fa-hand:before{content:"\f256"}.fa-om:before{content:"\f679"}.fa-worm:before{content:"\e599"}.fa-house-circle-xmark:before{content:"\e50b"}.fa-plug:before{content:"\f1e6"}.fa-chevron-up:before{content:"\f077"}.fa-hand-spock:before{content:"\f259"}.fa-stopwatch:before{content:"\f2f2"}.fa-face-kiss:before,.fa-kiss:before{content:"\f596"}.fa-bridge-circle-xmark:before{content:"\e4cb"}.fa-face-grin-tongue:before,.fa-grin-tongue:before{content:"\f589"}.fa-chess-bishop:before{content:"\f43a"}.fa-face-grin-wink:before,.fa-grin-wink:before{content:"\f58c"}.fa-deaf:before,.fa-deafness:before,.fa-ear-deaf:before,.fa-hard-of-hearing:before{content:"\f2a4"}.fa-road-circle-check:before{content:"\e564"}.fa-dice-five:before{content:"\f523"}.fa-rss-square:before,.fa-square-rss:before{content:"\f143"}.fa-land-mine-on:before{content:"\e51b"}.fa-i-cursor:before{content:"\f246"}.fa-stamp:before{content:"\f5bf"}.fa-stairs:before{content:"\e289"}.fa-i:before{content:"\49"}.fa-hryvnia-sign:before,.fa-hryvnia:before{content:"\f6f2"}.fa-pills:before{content:"\f484"}.fa-face-grin-wide:before,.fa-grin-alt:before{content:"\f581"}.fa-tooth:before{content:"\f5c9"}.fa-v:before{content:"\56"}.fa-bangladeshi-taka-sign:before{content:"\e2e6"}.fa-bicycle:before{content:"\f206"}.fa-rod-asclepius:before,.fa-rod-snake:before,.fa-staff-aesculapius:before,.fa-staff-snake:before{content:"\e579"}.fa-head-side-cough-slash:before{content:"\e062"}.fa-ambulance:before,.fa-truck-medical:before{content:"\f0f9"}.fa-wheat-awn-circle-exclamation:before{content:"\e598"}.fa-snowman:before{content:"\f7d0"}.fa-mortar-pestle:before{content:"\f5a7"}.fa-road-barrier:before{content:"\e562"}.fa-school:before{content:"\f549"}.fa-igloo:before{content:"\f7ae"}.fa-joint:before{content:"\f595"}.fa-angle-right:before{content:"\f105"}.fa-horse:before{content:"\f6f0"}.fa-q:before{content:"\51"}.fa-g:before{content:"\47"}.fa-notes-medical:before{content:"\f481"}.fa-temperature-2:before,.fa-temperature-half:before,.fa-thermometer-2:before,.fa-thermometer-half:before{content:"\f2c9"}.fa-dong-sign:before{content:"\e169"}.fa-capsules:before{content:"\f46b"}.fa-poo-bolt:before,.fa-poo-storm:before{content:"\f75a"}.fa-face-frown-open:before,.fa-frown-open:before{content:"\f57a"}.fa-hand-point-up:before{content:"\f0a6"}.fa-money-bill:before{content:"\f0d6"}.fa-bookmark:before{content:"\f02e"}.fa-align-justify:before{content:"\f039"}.fa-umbrella-beach:before{content:"\f5ca"}.fa-helmet-un:before{content:"\e503"}.fa-bullseye:before{content:"\f140"}.fa-bacon:before{content:"\f7e5"}.fa-hand-point-down:before{content:"\f0a7"}.fa-arrow-up-from-bracket:before{content:"\e09a"}.fa-folder-blank:before,.fa-folder:before{content:"\f07b"}.fa-file-medical-alt:before,.fa-file-waveform:before{content:"\f478"}.fa-radiation:before{content:"\f7b9"}.fa-chart-simple:before{content:"\e473"}.fa-mars-stroke:before{content:"\f229"}.fa-vial:before{content:"\f492"}.fa-dashboard:before,.fa-gauge-med:before,.fa-gauge:before,.fa-tachometer-alt-average:before{content:"\f624"}.fa-magic-wand-sparkles:before,.fa-wand-magic-sparkles:before{content:"\e2ca"}.fa-e:before{content:"\45"}.fa-pen-alt:before,.fa-pen-clip:before{content:"\f305"}.fa-bridge-circle-exclamation:before{content:"\e4ca"}.fa-user:before{content:"\f007"}.fa-school-circle-check:before{content:"\e56b"}.fa-dumpster:before{content:"\f793"}.fa-shuttle-van:before,.fa-van-shuttle:before{content:"\f5b6"}.fa-building-user:before{content:"\e4da"}.fa-caret-square-left:before,.fa-square-caret-left:before{content:"\f191"}.fa-highlighter:before{content:"\f591"}.fa-key:before{content:"\f084"}.fa-bullhorn:before{content:"\f0a1"}.fa-globe:before{content:"\f0ac"}.fa-synagogue:before{content:"\f69b"}.fa-person-half-dress:before{content:"\e548"}.fa-road-bridge:before{content:"\e563"}.fa-location-arrow:before{content:"\f124"}.fa-c:before{content:"\43"}.fa-tablet-button:before{content:"\f10a"}.fa-building-lock:before{content:"\e4d6"}.fa-pizza-slice:before{content:"\f818"}.fa-money-bill-wave:before{content:"\f53a"}.fa-area-chart:before,.fa-chart-area:before{content:"\f1fe"}.fa-house-flag:before{content:"\e50d"}.fa-person-circle-minus:before{content:"\e540"}.fa-ban:before,.fa-cancel:before{content:"\f05e"}.fa-camera-rotate:before{content:"\e0d8"}.fa-air-freshener:before,.fa-spray-can-sparkles:before{content:"\f5d0"}.fa-star:before{content:"\f005"}.fa-repeat:before{content:"\f363"}.fa-cross:before{content:"\f654"}.fa-box:before{content:"\f466"}.fa-venus-mars:before{content:"\f228"}.fa-arrow-pointer:before,.fa-mouse-pointer:before{content:"\f245"}.fa-expand-arrows-alt:before,.fa-maximize:before{content:"\f31e"}.fa-charging-station:before{content:"\f5e7"}.fa-shapes:before,.fa-triangle-circle-square:before{content:"\f61f"}.fa-random:before,.fa-shuffle:before{content:"\f074"}.fa-person-running:before,.fa-running:before{content:"\f70c"}.fa-mobile-retro:before{content:"\e527"}.fa-grip-lines-vertical:before{content:"\f7a5"}.fa-spider:before{content:"\f717"}.fa-hands-bound:before{content:"\e4f9"}.fa-file-invoice-dollar:before{content:"\f571"}.fa-plane-circle-exclamation:before{content:"\e556"}.fa-x-ray:before{content:"\f497"}.fa-spell-check:before{content:"\f891"}.fa-slash:before{content:"\f715"}.fa-computer-mouse:before,.fa-mouse:before{content:"\f8cc"}.fa-arrow-right-to-bracket:before,.fa-sign-in:before{content:"\f090"}.fa-shop-slash:before,.fa-store-alt-slash:before{content:"\e070"}.fa-server:before{content:"\f233"}.fa-virus-covid-slash:before{content:"\e4a9"}.fa-shop-lock:before{content:"\e4a5"}.fa-hourglass-1:before,.fa-hourglass-start:before{content:"\f251"}.fa-blender-phone:before{content:"\f6b6"}.fa-building-wheat:before{content:"\e4db"}.fa-person-breastfeeding:before{content:"\e53a"}.fa-right-to-bracket:before,.fa-sign-in-alt:before{content:"\f2f6"}.fa-venus:before{content:"\f221"}.fa-passport:before{content:"\f5ab"}.fa-heart-pulse:before,.fa-heartbeat:before{content:"\f21e"}.fa-people-carry-box:before,.fa-people-carry:before{content:"\f4ce"}.fa-temperature-high:before{content:"\f769"}.fa-microchip:before{content:"\f2db"}.fa-crown:before{content:"\f521"}.fa-weight-hanging:before{content:"\f5cd"}.fa-xmarks-lines:before{content:"\e59a"}.fa-file-prescription:before{content:"\f572"}.fa-weight-scale:before,.fa-weight:before{content:"\f496"}.fa-user-friends:before,.fa-user-group:before{content:"\f500"}.fa-arrow-up-a-z:before,.fa-sort-alpha-up:before{content:"\f15e"}.fa-chess-knight:before{content:"\f441"}.fa-face-laugh-squint:before,.fa-laugh-squint:before{content:"\f59b"}.fa-wheelchair:before{content:"\f193"}.fa-arrow-circle-up:before,.fa-circle-arrow-up:before{content:"\f0aa"}.fa-toggle-on:before{content:"\f205"}.fa-person-walking:before,.fa-walking:before{content:"\f554"}.fa-l:before{content:"\4c"}.fa-fire:before{content:"\f06d"}.fa-bed-pulse:before,.fa-procedures:before{content:"\f487"}.fa-shuttle-space:before,.fa-space-shuttle:before{content:"\f197"}.fa-face-laugh:before,.fa-laugh:before{content:"\f599"}.fa-folder-open:before{content:"\f07c"}.fa-heart-circle-plus:before{content:"\e500"}.fa-code-fork:before{content:"\e13b"}.fa-city:before{content:"\f64f"}.fa-microphone-alt:before,.fa-microphone-lines:before{content:"\f3c9"}.fa-pepper-hot:before{content:"\f816"}.fa-unlock:before{content:"\f09c"}.fa-colon-sign:before{content:"\e140"}.fa-headset:before{content:"\f590"}.fa-store-slash:before{content:"\e071"}.fa-road-circle-xmark:before{content:"\e566"}.fa-user-minus:before{content:"\f503"}.fa-mars-stroke-up:before,.fa-mars-stroke-v:before{content:"\f22a"}.fa-champagne-glasses:before,.fa-glass-cheers:before{content:"\f79f"}.fa-clipboard:before{content:"\f328"}.fa-house-circle-exclamation:before{content:"\e50a"}.fa-file-arrow-up:before,.fa-file-upload:before{content:"\f574"}.fa-wifi-3:before,.fa-wifi-strong:before,.fa-wifi:before{content:"\f1eb"}.fa-bath:before,.fa-bathtub:before{content:"\f2cd"}.fa-underline:before{content:"\f0cd"}.fa-user-edit:before,.fa-user-pen:before{content:"\f4ff"}.fa-signature:before{content:"\f5b7"}.fa-stroopwafel:before{content:"\f551"}.fa-bold:before{content:"\f032"}.fa-anchor-lock:before{content:"\e4ad"}.fa-building-ngo:before{content:"\e4d7"}.fa-manat-sign:before{content:"\e1d5"}.fa-not-equal:before{content:"\f53e"}.fa-border-style:before,.fa-border-top-left:before{content:"\f853"}.fa-map-location-dot:before,.fa-map-marked-alt:before{content:"\f5a0"}.fa-jedi:before{content:"\f669"}.fa-poll:before,.fa-square-poll-vertical:before{content:"\f681"}.fa-mug-hot:before{content:"\f7b6"}.fa-battery-car:before,.fa-car-battery:before{content:"\f5df"}.fa-gift:before{content:"\f06b"}.fa-dice-two:before{content:"\f528"}.fa-chess-queen:before{content:"\f445"}.fa-glasses:before{content:"\f530"}.fa-chess-board:before{content:"\f43c"}.fa-building-circle-check:before{content:"\e4d2"}.fa-person-chalkboard:before{content:"\e53d"}.fa-mars-stroke-h:before,.fa-mars-stroke-right:before{content:"\f22b"}.fa-hand-back-fist:before,.fa-hand-rock:before{content:"\f255"}.fa-caret-square-up:before,.fa-square-caret-up:before{content:"\f151"}.fa-cloud-showers-water:before{content:"\e4e4"}.fa-bar-chart:before,.fa-chart-bar:before{content:"\f080"}.fa-hands-bubbles:before,.fa-hands-wash:before{content:"\e05e"}.fa-less-than-equal:before{content:"\f537"}.fa-train:before{content:"\f238"}.fa-eye-low-vision:before,.fa-low-vision:before{content:"\f2a8"}.fa-crow:before{content:"\f520"}.fa-sailboat:before{content:"\e445"}.fa-window-restore:before{content:"\f2d2"}.fa-plus-square:before,.fa-square-plus:before{content:"\f0fe"}.fa-torii-gate:before{content:"\f6a1"}.fa-frog:before{content:"\f52e"}.fa-bucket:before{content:"\e4cf"}.fa-image:before{content:"\f03e"}.fa-microphone:before{content:"\f130"}.fa-cow:before{content:"\f6c8"}.fa-caret-up:before{content:"\f0d8"}.fa-screwdriver:before{content:"\f54a"}.fa-folder-closed:before{content:"\e185"}.fa-house-tsunami:before{content:"\e515"}.fa-square-nfi:before{content:"\e576"}.fa-arrow-up-from-ground-water:before{content:"\e4b5"}.fa-glass-martini-alt:before,.fa-martini-glass:before{content:"\f57b"}.fa-rotate-back:before,.fa-rotate-backward:before,.fa-rotate-left:before,.fa-undo-alt:before{content:"\f2ea"}.fa-columns:before,.fa-table-columns:before{content:"\f0db"}.fa-lemon:before{content:"\f094"}.fa-head-side-mask:before{content:"\e063"}.fa-handshake:before{content:"\f2b5"}.fa-gem:before{content:"\f3a5"}.fa-dolly-box:before,.fa-dolly:before{content:"\f472"}.fa-smoking:before{content:"\f48d"}.fa-compress-arrows-alt:before,.fa-minimize:before{content:"\f78c"}.fa-monument:before{content:"\f5a6"}.fa-snowplow:before{content:"\f7d2"}.fa-angle-double-right:before,.fa-angles-right:before{content:"\f101"}.fa-cannabis:before{content:"\f55f"}.fa-circle-play:before,.fa-play-circle:before{content:"\f144"}.fa-tablets:before{content:"\f490"}.fa-ethernet:before{content:"\f796"}.fa-eur:before,.fa-euro-sign:before,.fa-euro:before{content:"\f153"}.fa-chair:before{content:"\f6c0"}.fa-check-circle:before,.fa-circle-check:before{content:"\f058"}.fa-circle-stop:before,.fa-stop-circle:before{content:"\f28d"}.fa-compass-drafting:before,.fa-drafting-compass:before{content:"\f568"}.fa-plate-wheat:before{content:"\e55a"}.fa-icicles:before{content:"\f7ad"}.fa-person-shelter:before{content:"\e54f"}.fa-neuter:before{content:"\f22c"}.fa-id-badge:before{content:"\f2c1"}.fa-marker:before{content:"\f5a1"}.fa-face-laugh-beam:before,.fa-laugh-beam:before{content:"\f59a"}.fa-helicopter-symbol:before{content:"\e502"}.fa-universal-access:before{content:"\f29a"}.fa-chevron-circle-up:before,.fa-circle-chevron-up:before{content:"\f139"}.fa-lari-sign:before{content:"\e1c8"}.fa-volcano:before{content:"\f770"}.fa-person-walking-dashed-line-arrow-right:before{content:"\e553"}.fa-gbp:before,.fa-pound-sign:before,.fa-sterling-sign:before{content:"\f154"}.fa-viruses:before{content:"\e076"}.fa-square-person-confined:before{content:"\e577"}.fa-user-tie:before{content:"\f508"}.fa-arrow-down-long:before,.fa-long-arrow-down:before{content:"\f175"}.fa-tent-arrow-down-to-line:before{content:"\e57e"}.fa-certificate:before{content:"\f0a3"}.fa-mail-reply-all:before,.fa-reply-all:before{content:"\f122"}.fa-suitcase:before{content:"\f0f2"}.fa-person-skating:before,.fa-skating:before{content:"\f7c5"}.fa-filter-circle-dollar:before,.fa-funnel-dollar:before{content:"\f662"}.fa-camera-retro:before{content:"\f083"}.fa-arrow-circle-down:before,.fa-circle-arrow-down:before{content:"\f0ab"}.fa-arrow-right-to-file:before,.fa-file-import:before{content:"\f56f"}.fa-external-link-square:before,.fa-square-arrow-up-right:before{content:"\f14c"}.fa-box-open:before{content:"\f49e"}.fa-scroll:before{content:"\f70e"}.fa-spa:before{content:"\f5bb"}.fa-location-pin-lock:before{content:"\e51f"}.fa-pause:before{content:"\f04c"}.fa-hill-avalanche:before{content:"\e507"}.fa-temperature-0:before,.fa-temperature-empty:before,.fa-thermometer-0:before,.fa-thermometer-empty:before{content:"\f2cb"}.fa-bomb:before{content:"\f1e2"}.fa-registered:before{content:"\f25d"}.fa-address-card:before,.fa-contact-card:before,.fa-vcard:before{content:"\f2bb"}.fa-balance-scale-right:before,.fa-scale-unbalanced-flip:before{content:"\f516"}.fa-subscript:before{content:"\f12c"}.fa-diamond-turn-right:before,.fa-directions:before{content:"\f5eb"}.fa-burst:before{content:"\e4dc"}.fa-house-laptop:before,.fa-laptop-house:before{content:"\e066"}.fa-face-tired:before,.fa-tired:before{content:"\f5c8"}.fa-money-bills:before{content:"\e1f3"}.fa-smog:before{content:"\f75f"}.fa-crutch:before{content:"\f7f7"}.fa-cloud-arrow-up:before,.fa-cloud-upload-alt:before,.fa-cloud-upload:before{content:"\f0ee"}.fa-palette:before{content:"\f53f"}.fa-arrows-turn-right:before{content:"\e4c0"}.fa-vest:before{content:"\e085"}.fa-ferry:before{content:"\e4ea"}.fa-arrows-down-to-people:before{content:"\e4b9"}.fa-seedling:before,.fa-sprout:before{content:"\f4d8"}.fa-arrows-alt-h:before,.fa-left-right:before{content:"\f337"}.fa-boxes-packing:before{content:"\e4c7"}.fa-arrow-circle-left:before,.fa-circle-arrow-left:before{content:"\f0a8"}.fa-group-arrows-rotate:before{content:"\e4f6"}.fa-bowl-food:before{content:"\e4c6"}.fa-candy-cane:before{content:"\f786"}.fa-arrow-down-wide-short:before,.fa-sort-amount-asc:before,.fa-sort-amount-down:before{content:"\f160"}.fa-cloud-bolt:before,.fa-thunderstorm:before{content:"\f76c"}.fa-remove-format:before,.fa-text-slash:before{content:"\f87d"}.fa-face-smile-wink:before,.fa-smile-wink:before{content:"\f4da"}.fa-file-word:before{content:"\f1c2"}.fa-file-powerpoint:before{content:"\f1c4"}.fa-arrows-h:before,.fa-arrows-left-right:before{content:"\f07e"}.fa-house-lock:before{content:"\e510"}.fa-cloud-arrow-down:before,.fa-cloud-download-alt:before,.fa-cloud-download:before{content:"\f0ed"}.fa-children:before{content:"\e4e1"}.fa-blackboard:before,.fa-chalkboard:before{content:"\f51b"}.fa-user-alt-slash:before,.fa-user-large-slash:before{content:"\f4fa"}.fa-envelope-open:before{content:"\f2b6"}.fa-handshake-alt-slash:before,.fa-handshake-simple-slash:before{content:"\e05f"}.fa-mattress-pillow:before{content:"\e525"}.fa-guarani-sign:before{content:"\e19a"}.fa-arrows-rotate:before,.fa-refresh:before,.fa-sync:before{content:"\f021"}.fa-fire-extinguisher:before{content:"\f134"}.fa-cruzeiro-sign:before{content:"\e152"}.fa-greater-than-equal:before{content:"\f532"}.fa-shield-alt:before,.fa-shield-halved:before{content:"\f3ed"}.fa-atlas:before,.fa-book-atlas:before{content:"\f558"}.fa-virus:before{content:"\e074"}.fa-envelope-circle-check:before{content:"\e4e8"}.fa-layer-group:before{content:"\f5fd"}.fa-arrows-to-dot:before{content:"\e4be"}.fa-archway:before{content:"\f557"}.fa-heart-circle-check:before{content:"\e4fd"}.fa-house-chimney-crack:before,.fa-house-damage:before{content:"\f6f1"}.fa-file-archive:before,.fa-file-zipper:before{content:"\f1c6"}.fa-square:before{content:"\f0c8"}.fa-glass-martini:before,.fa-martini-glass-empty:before{content:"\f000"}.fa-couch:before{content:"\f4b8"}.fa-cedi-sign:before{content:"\e0df"}.fa-italic:before{content:"\f033"}.fa-church:before{content:"\f51d"}.fa-comments-dollar:before{content:"\f653"}.fa-democrat:before{content:"\f747"}.fa-z:before{content:"\5a"}.fa-person-skiing:before,.fa-skiing:before{content:"\f7c9"}.fa-road-lock:before{content:"\e567"}.fa-a:before{content:"\41"}.fa-temperature-arrow-down:before,.fa-temperature-down:before{content:"\e03f"}.fa-feather-alt:before,.fa-feather-pointed:before{content:"\f56b"}.fa-p:before{content:"\50"}.fa-snowflake:before{content:"\f2dc"}.fa-newspaper:before{content:"\f1ea"}.fa-ad:before,.fa-rectangle-ad:before{content:"\f641"}.fa-arrow-circle-right:before,.fa-circle-arrow-right:before{content:"\f0a9"}.fa-filter-circle-xmark:before{content:"\e17b"}.fa-locust:before{content:"\e520"}.fa-sort:before,.fa-unsorted:before{content:"\f0dc"}.fa-list-1-2:before,.fa-list-numeric:before,.fa-list-ol:before{content:"\f0cb"}.fa-person-dress-burst:before{content:"\e544"}.fa-money-check-alt:before,.fa-money-check-dollar:before{content:"\f53d"}.fa-vector-square:before{content:"\f5cb"}.fa-bread-slice:before{content:"\f7ec"}.fa-language:before{content:"\f1ab"}.fa-face-kiss-wink-heart:before,.fa-kiss-wink-heart:before{content:"\f598"}.fa-filter:before{content:"\f0b0"}.fa-question:before{content:"\3f"}.fa-file-signature:before{content:"\f573"}.fa-arrows-alt:before,.fa-up-down-left-right:before{content:"\f0b2"}.fa-house-chimney-user:before{content:"\e065"}.fa-hand-holding-heart:before{content:"\f4be"}.fa-puzzle-piece:before{content:"\f12e"}.fa-money-check:before{content:"\f53c"}.fa-star-half-alt:before,.fa-star-half-stroke:before{content:"\f5c0"}.fa-code:before{content:"\f121"}.fa-glass-whiskey:before,.fa-whiskey-glass:before{content:"\f7a0"}.fa-building-circle-exclamation:before{content:"\e4d3"}.fa-magnifying-glass-chart:before{content:"\e522"}.fa-arrow-up-right-from-square:before,.fa-external-link:before{content:"\f08e"}.fa-cubes-stacked:before{content:"\e4e6"}.fa-krw:before,.fa-won-sign:before,.fa-won:before{content:"\f159"}.fa-virus-covid:before{content:"\e4a8"}.fa-austral-sign:before{content:"\e0a9"}.fa-f:before{content:"\46"}.fa-leaf:before{content:"\f06c"}.fa-road:before{content:"\f018"}.fa-cab:before,.fa-taxi:before{content:"\f1ba"}.fa-person-circle-plus:before{content:"\e541"}.fa-chart-pie:before,.fa-pie-chart:before{content:"\f200"}.fa-bolt-lightning:before{content:"\e0b7"}.fa-sack-xmark:before{content:"\e56a"}.fa-file-excel:before{content:"\f1c3"}.fa-file-contract:before{content:"\f56c"}.fa-fish-fins:before{content:"\e4f2"}.fa-building-flag:before{content:"\e4d5"}.fa-face-grin-beam:before,.fa-grin-beam:before{content:"\f582"}.fa-object-ungroup:before{content:"\f248"}.fa-poop:before{content:"\f619"}.fa-location-pin:before,.fa-map-marker:before{content:"\f041"}.fa-kaaba:before{content:"\f66b"}.fa-toilet-paper:before{content:"\f71e"}.fa-hard-hat:before,.fa-hat-hard:before,.fa-helmet-safety:before{content:"\f807"}.fa-eject:before{content:"\f052"}.fa-arrow-alt-circle-right:before,.fa-circle-right:before{content:"\f35a"}.fa-plane-circle-check:before{content:"\e555"}.fa-face-rolling-eyes:before,.fa-meh-rolling-eyes:before{content:"\f5a5"}.fa-object-group:before{content:"\f247"}.fa-chart-line:before,.fa-line-chart:before{content:"\f201"}.fa-mask-ventilator:before{content:"\e524"}.fa-arrow-right:before{content:"\f061"}.fa-map-signs:before,.fa-signs-post:before{content:"\f277"}.fa-cash-register:before{content:"\f788"}.fa-person-circle-question:before{content:"\e542"}.fa-h:before{content:"\48"}.fa-tarp:before{content:"\e57b"}.fa-screwdriver-wrench:before,.fa-tools:before{content:"\f7d9"}.fa-arrows-to-eye:before{content:"\e4bf"}.fa-plug-circle-bolt:before{content:"\e55b"}.fa-heart:before{content:"\f004"}.fa-mars-and-venus:before{content:"\f224"}.fa-home-user:before,.fa-house-user:before{content:"\e1b0"}.fa-dumpster-fire:before{content:"\f794"}.fa-house-crack:before{content:"\e3b1"}.fa-cocktail:before,.fa-martini-glass-citrus:before{content:"\f561"}.fa-face-surprise:before,.fa-surprise:before{content:"\f5c2"}.fa-bottle-water:before{content:"\e4c5"}.fa-circle-pause:before,.fa-pause-circle:before{content:"\f28b"}.fa-toilet-paper-slash:before{content:"\e072"}.fa-apple-alt:before,.fa-apple-whole:before{content:"\f5d1"}.fa-kitchen-set:before{content:"\e51a"}.fa-r:before{content:"\52"}.fa-temperature-1:before,.fa-temperature-quarter:before,.fa-thermometer-1:before,.fa-thermometer-quarter:before{content:"\f2ca"}.fa-cube:before{content:"\f1b2"}.fa-bitcoin-sign:before{content:"\e0b4"}.fa-shield-dog:before{content:"\e573"}.fa-solar-panel:before{content:"\f5ba"}.fa-lock-open:before{content:"\f3c1"}.fa-elevator:before{content:"\e16d"}.fa-money-bill-transfer:before{content:"\e528"}.fa-money-bill-trend-up:before{content:"\e529"}.fa-house-flood-water-circle-arrow-right:before{content:"\e50f"}.fa-poll-h:before,.fa-square-poll-horizontal:before{content:"\f682"}.fa-circle:before{content:"\f111"}.fa-backward-fast:before,.fa-fast-backward:before{content:"\f049"}.fa-recycle:before{content:"\f1b8"}.fa-user-astronaut:before{content:"\f4fb"}.fa-plane-slash:before{content:"\e069"}.fa-trademark:before{content:"\f25c"}.fa-basketball-ball:before,.fa-basketball:before{content:"\f434"}.fa-satellite-dish:before{content:"\f7c0"}.fa-arrow-alt-circle-up:before,.fa-circle-up:before{content:"\f35b"}.fa-mobile-alt:before,.fa-mobile-screen-button:before{content:"\f3cd"}.fa-volume-high:before,.fa-volume-up:before{content:"\f028"}.fa-users-rays:before{content:"\e593"}.fa-wallet:before{content:"\f555"}.fa-clipboard-check:before{content:"\f46c"}.fa-file-audio:before{content:"\f1c7"}.fa-burger:before,.fa-hamburger:before{content:"\f805"}.fa-wrench:before{content:"\f0ad"}.fa-bugs:before{content:"\e4d0"}.fa-rupee-sign:before,.fa-rupee:before{content:"\f156"}.fa-file-image:before{content:"\f1c5"}.fa-circle-question:before,.fa-question-circle:before{content:"\f059"}.fa-plane-departure:before{content:"\f5b0"}.fa-handshake-slash:before{content:"\e060"}.fa-book-bookmark:before{content:"\e0bb"}.fa-code-branch:before{content:"\f126"}.fa-hat-cowboy:before{content:"\f8c0"}.fa-bridge:before{content:"\e4c8"}.fa-phone-alt:before,.fa-phone-flip:before{content:"\f879"}.fa-truck-front:before{content:"\e2b7"}.fa-cat:before{content:"\f6be"}.fa-anchor-circle-exclamation:before{content:"\e4ab"}.fa-truck-field:before{content:"\e58d"}.fa-route:before{content:"\f4d7"}.fa-clipboard-question:before{content:"\e4e3"}.fa-panorama:before{content:"\e209"}.fa-comment-medical:before{content:"\f7f5"}.fa-teeth-open:before{content:"\f62f"}.fa-file-circle-minus:before{content:"\e4ed"}.fa-tags:before{content:"\f02c"}.fa-wine-glass:before{content:"\f4e3"}.fa-fast-forward:before,.fa-forward-fast:before{content:"\f050"}.fa-face-meh-blank:before,.fa-meh-blank:before{content:"\f5a4"}.fa-parking:before,.fa-square-parking:before{content:"\f540"}.fa-house-signal:before{content:"\e012"}.fa-bars-progress:before,.fa-tasks-alt:before{content:"\f828"}.fa-faucet-drip:before{content:"\e006"}.fa-cart-flatbed:before,.fa-dolly-flatbed:before{content:"\f474"}.fa-ban-smoking:before,.fa-smoking-ban:before{content:"\f54d"}.fa-terminal:before{content:"\f120"}.fa-mobile-button:before{content:"\f10b"}.fa-house-medical-flag:before{content:"\e514"}.fa-basket-shopping:before,.fa-shopping-basket:before{content:"\f291"}.fa-tape:before{content:"\f4db"}.fa-bus-alt:before,.fa-bus-simple:before{content:"\f55e"}.fa-eye:before{content:"\f06e"}.fa-face-sad-cry:before,.fa-sad-cry:before{content:"\f5b3"}.fa-audio-description:before{content:"\f29e"}.fa-person-military-to-person:before{content:"\e54c"}.fa-file-shield:before{content:"\e4f0"}.fa-user-slash:before{content:"\f506"}.fa-pen:before{content:"\f304"}.fa-tower-observation:before{content:"\e586"}.fa-file-code:before{content:"\f1c9"}.fa-signal-5:before,.fa-signal-perfect:before,.fa-signal:before{content:"\f012"}.fa-bus:before{content:"\f207"}.fa-heart-circle-xmark:before{content:"\e501"}.fa-home-lg:before,.fa-house-chimney:before{content:"\e3af"}.fa-window-maximize:before{content:"\f2d0"}.fa-face-frown:before,.fa-frown:before{content:"\f119"}.fa-prescription:before{content:"\f5b1"}.fa-shop:before,.fa-store-alt:before{content:"\f54f"}.fa-floppy-disk:before,.fa-save:before{content:"\f0c7"}.fa-vihara:before{content:"\f6a7"}.fa-balance-scale-left:before,.fa-scale-unbalanced:before{content:"\f515"}.fa-sort-asc:before,.fa-sort-up:before{content:"\f0de"}.fa-comment-dots:before,.fa-commenting:before{content:"\f4ad"}.fa-plant-wilt:before{content:"\e5aa"}.fa-diamond:before{content:"\f219"}.fa-face-grin-squint:before,.fa-grin-squint:before{content:"\f585"}.fa-hand-holding-dollar:before,.fa-hand-holding-usd:before{content:"\f4c0"}.fa-bacterium:before{content:"\e05a"}.fa-hand-pointer:before{content:"\f25a"}.fa-drum-steelpan:before{content:"\f56a"}.fa-hand-scissors:before{content:"\f257"}.fa-hands-praying:before,.fa-praying-hands:before{content:"\f684"}.fa-arrow-right-rotate:before,.fa-arrow-rotate-forward:before,.fa-arrow-rotate-right:before,.fa-redo:before{content:"\f01e"}.fa-biohazard:before{content:"\f780"}.fa-location-crosshairs:before,.fa-location:before{content:"\f601"}.fa-mars-double:before{content:"\f227"}.fa-child-dress:before{content:"\e59c"}.fa-users-between-lines:before{content:"\e591"}.fa-lungs-virus:before{content:"\e067"}.fa-face-grin-tears:before,.fa-grin-tears:before{content:"\f588"}.fa-phone:before{content:"\f095"}.fa-calendar-times:before,.fa-calendar-xmark:before{content:"\f273"}.fa-child-reaching:before{content:"\e59d"}.fa-head-side-virus:before{content:"\e064"}.fa-user-cog:before,.fa-user-gear:before{content:"\f4fe"}.fa-arrow-up-1-9:before,.fa-sort-numeric-up:before{content:"\f163"}.fa-door-closed:before{content:"\f52a"}.fa-shield-virus:before{content:"\e06c"}.fa-dice-six:before{content:"\f526"}.fa-mosquito-net:before{content:"\e52c"}.fa-bridge-water:before{content:"\e4ce"}.fa-person-booth:before{content:"\f756"}.fa-text-width:before{content:"\f035"}.fa-hat-wizard:before{content:"\f6e8"}.fa-pen-fancy:before{content:"\f5ac"}.fa-digging:before,.fa-person-digging:before{content:"\f85e"}.fa-trash:before{content:"\f1f8"}.fa-gauge-simple-med:before,.fa-gauge-simple:before,.fa-tachometer-average:before{content:"\f629"}.fa-book-medical:before{content:"\f7e6"}.fa-poo:before{content:"\f2fe"}.fa-quote-right-alt:before,.fa-quote-right:before{content:"\f10e"}.fa-shirt:before,.fa-t-shirt:before,.fa-tshirt:before{content:"\f553"}.fa-cubes:before{content:"\f1b3"}.fa-divide:before{content:"\f529"}.fa-tenge-sign:before,.fa-tenge:before{content:"\f7d7"}.fa-headphones:before{content:"\f025"}.fa-hands-holding:before{content:"\f4c2"}.fa-hands-clapping:before{content:"\e1a8"}.fa-republican:before{content:"\f75e"}.fa-arrow-left:before{content:"\f060"}.fa-person-circle-xmark:before{content:"\e543"}.fa-ruler:before{content:"\f545"}.fa-align-left:before{content:"\f036"}.fa-dice-d6:before{content:"\f6d1"}.fa-restroom:before{content:"\f7bd"}.fa-j:before{content:"\4a"}.fa-users-viewfinder:before{content:"\e595"}.fa-file-video:before{content:"\f1c8"}.fa-external-link-alt:before,.fa-up-right-from-square:before{content:"\f35d"}.fa-table-cells:before,.fa-th:before{content:"\f00a"}.fa-file-pdf:before{content:"\f1c1"}.fa-bible:before,.fa-book-bible:before{content:"\f647"}.fa-o:before{content:"\4f"}.fa-medkit:before,.fa-suitcase-medical:before{content:"\f0fa"}.fa-user-secret:before{content:"\f21b"}.fa-otter:before{content:"\f700"}.fa-female:before,.fa-person-dress:before{content:"\f182"}.fa-comment-dollar:before{content:"\f651"}.fa-briefcase-clock:before,.fa-business-time:before{content:"\f64a"}.fa-table-cells-large:before,.fa-th-large:before{content:"\f009"}.fa-book-tanakh:before,.fa-tanakh:before{content:"\f827"}.fa-phone-volume:before,.fa-volume-control-phone:before{content:"\f2a0"}.fa-hat-cowboy-side:before{content:"\f8c1"}.fa-clipboard-user:before{content:"\f7f3"}.fa-child:before{content:"\f1ae"}.fa-lira-sign:before{content:"\f195"}.fa-satellite:before{content:"\f7bf"}.fa-plane-lock:before{content:"\e558"}.fa-tag:before{content:"\f02b"}.fa-comment:before{content:"\f075"}.fa-birthday-cake:before,.fa-cake-candles:before,.fa-cake:before{content:"\f1fd"}.fa-envelope:before{content:"\f0e0"}.fa-angle-double-up:before,.fa-angles-up:before{content:"\f102"}.fa-paperclip:before{content:"\f0c6"}.fa-arrow-right-to-city:before{content:"\e4b3"}.fa-ribbon:before{content:"\f4d6"}.fa-lungs:before{content:"\f604"}.fa-arrow-up-9-1:before,.fa-sort-numeric-up-alt:before{content:"\f887"}.fa-litecoin-sign:before{content:"\e1d3"}.fa-border-none:before{content:"\f850"}.fa-circle-nodes:before{content:"\e4e2"}.fa-parachute-box:before{content:"\f4cd"}.fa-indent:before{content:"\f03c"}.fa-truck-field-un:before{content:"\e58e"}.fa-hourglass-empty:before,.fa-hourglass:before{content:"\f254"}.fa-mountain:before{content:"\f6fc"}.fa-user-doctor:before,.fa-user-md:before{content:"\f0f0"}.fa-circle-info:before,.fa-info-circle:before{content:"\f05a"}.fa-cloud-meatball:before{content:"\f73b"}.fa-camera-alt:before,.fa-camera:before{content:"\f030"}.fa-square-virus:before{content:"\e578"}.fa-meteor:before{content:"\f753"}.fa-car-on:before{content:"\e4dd"}.fa-sleigh:before{content:"\f7cc"}.fa-arrow-down-1-9:before,.fa-sort-numeric-asc:before,.fa-sort-numeric-down:before{content:"\f162"}.fa-hand-holding-droplet:before,.fa-hand-holding-water:before{content:"\f4c1"}.fa-water:before{content:"\f773"}.fa-calendar-check:before{content:"\f274"}.fa-braille:before{content:"\f2a1"}.fa-prescription-bottle-alt:before,.fa-prescription-bottle-medical:before{content:"\f486"}.fa-landmark:before{content:"\f66f"}.fa-truck:before{content:"\f0d1"}.fa-crosshairs:before{content:"\f05b"}.fa-person-cane:before{content:"\e53c"}.fa-tent:before{content:"\e57d"}.fa-vest-patches:before{content:"\e086"}.fa-check-double:before{content:"\f560"}.fa-arrow-down-a-z:before,.fa-sort-alpha-asc:before,.fa-sort-alpha-down:before{content:"\f15d"}.fa-money-bill-wheat:before{content:"\e52a"}.fa-cookie:before{content:"\f563"}.fa-arrow-left-rotate:before,.fa-arrow-rotate-back:before,.fa-arrow-rotate-backward:before,.fa-arrow-rotate-left:before,.fa-undo:before{content:"\f0e2"}.fa-hard-drive:before,.fa-hdd:before{content:"\f0a0"}.fa-face-grin-squint-tears:before,.fa-grin-squint-tears:before{content:"\f586"}.fa-dumbbell:before{content:"\f44b"}.fa-list-alt:before,.fa-rectangle-list:before{content:"\f022"}.fa-tarp-droplet:before{content:"\e57c"}.fa-house-medical-circle-check:before{content:"\e511"}.fa-person-skiing-nordic:before,.fa-skiing-nordic:before{content:"\f7ca"}.fa-calendar-plus:before{content:"\f271"}.fa-plane-arrival:before{content:"\f5af"}.fa-arrow-alt-circle-left:before,.fa-circle-left:before{content:"\f359"}.fa-subway:before,.fa-train-subway:before{content:"\f239"}.fa-chart-gantt:before{content:"\e0e4"}.fa-indian-rupee-sign:before,.fa-indian-rupee:before,.fa-inr:before{content:"\e1bc"}.fa-crop-alt:before,.fa-crop-simple:before{content:"\f565"}.fa-money-bill-1:before,.fa-money-bill-alt:before{content:"\f3d1"}.fa-left-long:before,.fa-long-arrow-alt-left:before{content:"\f30a"}.fa-dna:before{content:"\f471"}.fa-virus-slash:before{content:"\e075"}.fa-minus:before,.fa-subtract:before{content:"\f068"}.fa-chess:before{content:"\f439"}.fa-arrow-left-long:before,.fa-long-arrow-left:before{content:"\f177"}.fa-plug-circle-check:before{content:"\e55c"}.fa-street-view:before{content:"\f21d"}.fa-franc-sign:before{content:"\e18f"}.fa-volume-off:before{content:"\f026"}.fa-american-sign-language-interpreting:before,.fa-asl-interpreting:before,.fa-hands-american-sign-language-interpreting:before,.fa-hands-asl-interpreting:before{content:"\f2a3"}.fa-cog:before,.fa-gear:before{content:"\f013"}.fa-droplet-slash:before,.fa-tint-slash:before{content:"\f5c7"}.fa-mosque:before{content:"\f678"}.fa-mosquito:before{content:"\e52b"}.fa-star-of-david:before{content:"\f69a"}.fa-person-military-rifle:before{content:"\e54b"}.fa-cart-shopping:before,.fa-shopping-cart:before{content:"\f07a"}.fa-vials:before{content:"\f493"}.fa-plug-circle-plus:before{content:"\e55f"}.fa-place-of-worship:before{content:"\f67f"}.fa-grip-vertical:before{content:"\f58e"}.fa-arrow-turn-up:before,.fa-level-up:before{content:"\f148"}.fa-u:before{content:"\55"}.fa-square-root-alt:before,.fa-square-root-variable:before{content:"\f698"}.fa-clock-four:before,.fa-clock:before{content:"\f017"}.fa-backward-step:before,.fa-step-backward:before{content:"\f048"}.fa-pallet:before{content:"\f482"}.fa-faucet:before{content:"\e005"}.fa-baseball-bat-ball:before{content:"\f432"}.fa-s:before{content:"\53"}.fa-timeline:before{content:"\e29c"}.fa-keyboard:before{content:"\f11c"}.fa-caret-down:before{content:"\f0d7"}.fa-clinic-medical:before,.fa-house-chimney-medical:before{content:"\f7f2"}.fa-temperature-3:before,.fa-temperature-three-quarters:before,.fa-thermometer-3:before,.fa-thermometer-three-quarters:before{content:"\f2c8"}.fa-mobile-android-alt:before,.fa-mobile-screen:before{content:"\f3cf"}.fa-plane-up:before{content:"\e22d"}.fa-piggy-bank:before{content:"\f4d3"}.fa-battery-3:before,.fa-battery-half:before{content:"\f242"}.fa-mountain-city:before{content:"\e52e"}.fa-coins:before{content:"\f51e"}.fa-khanda:before{content:"\f66d"}.fa-sliders-h:before,.fa-sliders:before{content:"\f1de"}.fa-folder-tree:before{content:"\f802"}.fa-network-wired:before{content:"\f6ff"}.fa-map-pin:before{content:"\f276"}.fa-hamsa:before{content:"\f665"}.fa-cent-sign:before{content:"\e3f5"}.fa-flask:before{content:"\f0c3"}.fa-person-pregnant:before{content:"\e31e"}.fa-wand-sparkles:before{content:"\f72b"}.fa-ellipsis-v:before,.fa-ellipsis-vertical:before{content:"\f142"}.fa-ticket:before{content:"\f145"}.fa-power-off:before{content:"\f011"}.fa-long-arrow-alt-right:before,.fa-right-long:before{content:"\f30b"}.fa-flag-usa:before{content:"\f74d"}.fa-laptop-file:before{content:"\e51d"}.fa-teletype:before,.fa-tty:before{content:"\f1e4"}.fa-diagram-next:before{content:"\e476"}.fa-person-rifle:before{content:"\e54e"}.fa-house-medical-circle-exclamation:before{content:"\e512"}.fa-closed-captioning:before{content:"\f20a"}.fa-hiking:before,.fa-person-hiking:before{content:"\f6ec"}.fa-venus-double:before{content:"\f226"}.fa-images:before{content:"\f302"}.fa-calculator:before{content:"\f1ec"}.fa-people-pulling:before{content:"\e535"}.fa-n:before{content:"\4e"}.fa-cable-car:before,.fa-tram:before{content:"\f7da"}.fa-cloud-rain:before{content:"\f73d"}.fa-building-circle-xmark:before{content:"\e4d4"}.fa-ship:before{content:"\f21a"}.fa-arrows-down-to-line:before{content:"\e4b8"}.fa-download:before{content:"\f019"}.fa-face-grin:before,.fa-grin:before{content:"\f580"}.fa-backspace:before,.fa-delete-left:before{content:"\f55a"}.fa-eye-dropper-empty:before,.fa-eye-dropper:before,.fa-eyedropper:before{content:"\f1fb"}.fa-file-circle-check:before{content:"\e5a0"}.fa-forward:before{content:"\f04e"}.fa-mobile-android:before,.fa-mobile-phone:before,.fa-mobile:before{content:"\f3ce"}.fa-face-meh:before,.fa-meh:before{content:"\f11a"}.fa-align-center:before{content:"\f037"}.fa-book-dead:before,.fa-book-skull:before{content:"\f6b7"}.fa-drivers-license:before,.fa-id-card:before{content:"\f2c2"}.fa-dedent:before,.fa-outdent:before{content:"\f03b"}.fa-heart-circle-exclamation:before{content:"\e4fe"}.fa-home-alt:before,.fa-home-lg-alt:before,.fa-home:before,.fa-house:before{content:"\f015"}.fa-calendar-week:before{content:"\f784"}.fa-laptop-medical:before{content:"\f812"}.fa-b:before{content:"\42"}.fa-file-medical:before{content:"\f477"}.fa-dice-one:before{content:"\f525"}.fa-kiwi-bird:before{content:"\f535"}.fa-arrow-right-arrow-left:before,.fa-exchange:before{content:"\f0ec"}.fa-redo-alt:before,.fa-rotate-forward:before,.fa-rotate-right:before{content:"\f2f9"}.fa-cutlery:before,.fa-utensils:before{content:"\f2e7"}.fa-arrow-up-wide-short:before,.fa-sort-amount-up:before{content:"\f161"}.fa-mill-sign:before{content:"\e1ed"}.fa-bowl-rice:before{content:"\e2eb"}.fa-skull:before{content:"\f54c"}.fa-broadcast-tower:before,.fa-tower-broadcast:before{content:"\f519"}.fa-truck-pickup:before{content:"\f63c"}.fa-long-arrow-alt-up:before,.fa-up-long:before{content:"\f30c"}.fa-stop:before{content:"\f04d"}.fa-code-merge:before{content:"\f387"}.fa-upload:before{content:"\f093"}.fa-hurricane:before{content:"\f751"}.fa-mound:before{content:"\e52d"}.fa-toilet-portable:before{content:"\e583"}.fa-compact-disc:before{content:"\f51f"}.fa-file-arrow-down:before,.fa-file-download:before{content:"\f56d"}.fa-caravan:before{content:"\f8ff"}.fa-shield-cat:before{content:"\e572"}.fa-bolt:before,.fa-zap:before{content:"\f0e7"}.fa-glass-water:before{content:"\e4f4"}.fa-oil-well:before{content:"\e532"}.fa-vault:before{content:"\e2c5"}.fa-mars:before{content:"\f222"}.fa-toilet:before{content:"\f7d8"}.fa-plane-circle-xmark:before{content:"\e557"}.fa-cny:before,.fa-jpy:before,.fa-rmb:before,.fa-yen-sign:before,.fa-yen:before{content:"\f157"}.fa-rouble:before,.fa-rub:before,.fa-ruble-sign:before,.fa-ruble:before{content:"\f158"}.fa-sun:before{content:"\f185"}.fa-guitar:before{content:"\f7a6"}.fa-face-laugh-wink:before,.fa-laugh-wink:before{content:"\f59c"}.fa-horse-head:before{content:"\f7ab"}.fa-bore-hole:before{content:"\e4c3"}.fa-industry:before{content:"\f275"}.fa-arrow-alt-circle-down:before,.fa-circle-down:before{content:"\f358"}.fa-arrows-turn-to-dots:before{content:"\e4c1"}.fa-florin-sign:before{content:"\e184"}.fa-arrow-down-short-wide:before,.fa-sort-amount-desc:before,.fa-sort-amount-down-alt:before{content:"\f884"}.fa-less-than:before{content:"\3c"}.fa-angle-down:before{content:"\f107"}.fa-car-tunnel:before{content:"\e4de"}.fa-head-side-cough:before{content:"\e061"}.fa-grip-lines:before{content:"\f7a4"}.fa-thumbs-down:before{content:"\f165"}.fa-user-lock:before{content:"\f502"}.fa-arrow-right-long:before,.fa-long-arrow-right:before{content:"\f178"}.fa-anchor-circle-xmark:before{content:"\e4ac"}.fa-ellipsis-h:before,.fa-ellipsis:before{content:"\f141"}.fa-chess-pawn:before{content:"\f443"}.fa-first-aid:before,.fa-kit-medical:before{content:"\f479"}.fa-person-through-window:before{content:"\e5a9"}.fa-toolbox:before{content:"\f552"}.fa-hands-holding-circle:before{content:"\e4fb"}.fa-bug:before{content:"\f188"}.fa-credit-card-alt:before,.fa-credit-card:before{content:"\f09d"}.fa-automobile:before,.fa-car:before{content:"\f1b9"}.fa-hand-holding-hand:before{content:"\e4f7"}.fa-book-open-reader:before,.fa-book-reader:before{content:"\f5da"}.fa-mountain-sun:before{content:"\e52f"}.fa-arrows-left-right-to-line:before{content:"\e4ba"}.fa-dice-d20:before{content:"\f6cf"}.fa-truck-droplet:before{content:"\e58c"}.fa-file-circle-xmark:before{content:"\e5a1"}.fa-temperature-arrow-up:before,.fa-temperature-up:before{content:"\e040"}.fa-medal:before{content:"\f5a2"}.fa-bed:before{content:"\f236"}.fa-h-square:before,.fa-square-h:before{content:"\f0fd"}.fa-podcast:before{content:"\f2ce"}.fa-temperature-4:before,.fa-temperature-full:before,.fa-thermometer-4:before,.fa-thermometer-full:before{content:"\f2c7"}.fa-bell:before{content:"\f0f3"}.fa-superscript:before{content:"\f12b"}.fa-plug-circle-xmark:before{content:"\e560"}.fa-star-of-life:before{content:"\f621"}.fa-phone-slash:before{content:"\f3dd"}.fa-paint-roller:before{content:"\f5aa"}.fa-hands-helping:before,.fa-handshake-angle:before{content:"\f4c4"}.fa-location-dot:before,.fa-map-marker-alt:before{content:"\f3c5"}.fa-file:before{content:"\f15b"}.fa-greater-than:before{content:"\3e"}.fa-person-swimming:before,.fa-swimmer:before{content:"\f5c4"}.fa-arrow-down:before{content:"\f063"}.fa-droplet:before,.fa-tint:before{content:"\f043"}.fa-eraser:before{content:"\f12d"}.fa-earth-america:before,.fa-earth-americas:before,.fa-earth:before,.fa-globe-americas:before{content:"\f57d"}.fa-person-burst:before{content:"\e53b"}.fa-dove:before{content:"\f4ba"}.fa-battery-0:before,.fa-battery-empty:before{content:"\f244"}.fa-socks:before{content:"\f696"}.fa-inbox:before{content:"\f01c"}.fa-section:before{content:"\e447"}.fa-gauge-high:before,.fa-tachometer-alt-fast:before,.fa-tachometer-alt:before{content:"\f625"}.fa-envelope-open-text:before{content:"\f658"}.fa-hospital-alt:before,.fa-hospital-wide:before,.fa-hospital:before{content:"\f0f8"}.fa-wine-bottle:before{content:"\f72f"}.fa-chess-rook:before{content:"\f447"}.fa-bars-staggered:before,.fa-reorder:before,.fa-stream:before{content:"\f550"}.fa-dharmachakra:before{content:"\f655"}.fa-hotdog:before{content:"\f80f"}.fa-blind:before,.fa-person-walking-with-cane:before{content:"\f29d"}.fa-drum:before{content:"\f569"}.fa-ice-cream:before{content:"\f810"}.fa-heart-circle-bolt:before{content:"\e4fc"}.fa-fax:before{content:"\f1ac"}.fa-paragraph:before{content:"\f1dd"}.fa-check-to-slot:before,.fa-vote-yea:before{content:"\f772"}.fa-star-half:before{content:"\f089"}.fa-boxes-alt:before,.fa-boxes-stacked:before,.fa-boxes:before{content:"\f468"}.fa-chain:before,.fa-link:before{content:"\f0c1"}.fa-assistive-listening-systems:before,.fa-ear-listen:before{content:"\f2a2"}.fa-tree-city:before{content:"\e587"}.fa-play:before{content:"\f04b"}.fa-font:before{content:"\f031"}.fa-rupiah-sign:before{content:"\e23d"}.fa-magnifying-glass:before,.fa-search:before{content:"\f002"}.fa-ping-pong-paddle-ball:before,.fa-table-tennis-paddle-ball:before,.fa-table-tennis:before{content:"\f45d"}.fa-diagnoses:before,.fa-person-dots-from-line:before{content:"\f470"}.fa-trash-can-arrow-up:before,.fa-trash-restore-alt:before{content:"\f82a"}.fa-naira-sign:before{content:"\e1f6"}.fa-cart-arrow-down:before{content:"\f218"}.fa-walkie-talkie:before{content:"\f8ef"}.fa-file-edit:before,.fa-file-pen:before{content:"\f31c"}.fa-receipt:before{content:"\f543"}.fa-pen-square:before,.fa-pencil-square:before,.fa-square-pen:before{content:"\f14b"}.fa-suitcase-rolling:before{content:"\f5c1"}.fa-person-circle-exclamation:before{content:"\e53f"}.fa-chevron-down:before{content:"\f078"}.fa-battery-5:before,.fa-battery-full:before,.fa-battery:before{content:"\f240"}.fa-skull-crossbones:before{content:"\f714"}.fa-code-compare:before{content:"\e13a"}.fa-list-dots:before,.fa-list-ul:before{content:"\f0ca"}.fa-school-lock:before{content:"\e56f"}.fa-tower-cell:before{content:"\e585"}.fa-down-long:before,.fa-long-arrow-alt-down:before{content:"\f309"}.fa-ranking-star:before{content:"\e561"}.fa-chess-king:before{content:"\f43f"}.fa-person-harassing:before{content:"\e549"}.fa-brazilian-real-sign:before{content:"\e46c"}.fa-landmark-alt:before,.fa-landmark-dome:before{content:"\f752"}.fa-arrow-up:before{content:"\f062"}.fa-television:before,.fa-tv-alt:before,.fa-tv:before{content:"\f26c"}.fa-shrimp:before{content:"\e448"}.fa-list-check:before,.fa-tasks:before{content:"\f0ae"}.fa-jug-detergent:before{content:"\e519"}.fa-circle-user:before,.fa-user-circle:before{content:"\f2bd"}.fa-user-shield:before{content:"\f505"}.fa-wind:before{content:"\f72e"}.fa-car-burst:before,.fa-car-crash:before{content:"\f5e1"}.fa-y:before{content:"\59"}.fa-person-snowboarding:before,.fa-snowboarding:before{content:"\f7ce"}.fa-shipping-fast:before,.fa-truck-fast:before{content:"\f48b"}.fa-fish:before{content:"\f578"}.fa-user-graduate:before{content:"\f501"}.fa-adjust:before,.fa-circle-half-stroke:before{content:"\f042"}.fa-clapperboard:before{content:"\e131"}.fa-circle-radiation:before,.fa-radiation-alt:before{content:"\f7ba"}.fa-baseball-ball:before,.fa-baseball:before{content:"\f433"}.fa-jet-fighter-up:before{content:"\e518"}.fa-diagram-project:before,.fa-project-diagram:before{content:"\f542"}.fa-copy:before{content:"\f0c5"}.fa-volume-mute:before,.fa-volume-times:before,.fa-volume-xmark:before{content:"\f6a9"}.fa-hand-sparkles:before{content:"\e05d"}.fa-grip-horizontal:before,.fa-grip:before{content:"\f58d"}.fa-share-from-square:before,.fa-share-square:before{content:"\f14d"}.fa-child-combatant:before,.fa-child-rifle:before{content:"\e4e0"}.fa-gun:before{content:"\e19b"}.fa-phone-square:before,.fa-square-phone:before{content:"\f098"}.fa-add:before,.fa-plus:before{content:"\2b"}.fa-expand:before{content:"\f065"}.fa-computer:before{content:"\e4e5"}.fa-close:before,.fa-multiply:before,.fa-remove:before,.fa-times:before,.fa-xmark:before{content:"\f00d"}.fa-arrows-up-down-left-right:before,.fa-arrows:before{content:"\f047"}.fa-chalkboard-teacher:before,.fa-chalkboard-user:before{content:"\f51c"}.fa-peso-sign:before{content:"\e222"}.fa-building-shield:before{content:"\e4d8"}.fa-baby:before{content:"\f77c"}.fa-users-line:before{content:"\e592"}.fa-quote-left-alt:before,.fa-quote-left:before{content:"\f10d"}.fa-tractor:before{content:"\f722"}.fa-trash-arrow-up:before,.fa-trash-restore:before{content:"\f829"}.fa-arrow-down-up-lock:before{content:"\e4b0"}.fa-lines-leaning:before{content:"\e51e"}.fa-ruler-combined:before{content:"\f546"}.fa-copyright:before{content:"\f1f9"}.fa-equals:before{content:"\3d"}.fa-blender:before{content:"\f517"}.fa-teeth:before{content:"\f62e"}.fa-ils:before,.fa-shekel-sign:before,.fa-shekel:before,.fa-sheqel-sign:before,.fa-sheqel:before{content:"\f20b"}.fa-map:before{content:"\f279"}.fa-rocket:before{content:"\f135"}.fa-photo-film:before,.fa-photo-video:before{content:"\f87c"}.fa-folder-minus:before{content:"\f65d"}.fa-store:before{content:"\f54e"}.fa-arrow-trend-up:before{content:"\e098"}.fa-plug-circle-minus:before{content:"\e55e"}.fa-sign-hanging:before,.fa-sign:before{content:"\f4d9"}.fa-bezier-curve:before{content:"\f55b"}.fa-bell-slash:before{content:"\f1f6"}.fa-tablet-android:before,.fa-tablet:before{content:"\f3fb"}.fa-school-flag:before{content:"\e56e"}.fa-fill:before{content:"\f575"}.fa-angle-up:before{content:"\f106"}.fa-drumstick-bite:before{content:"\f6d7"}.fa-holly-berry:before{content:"\f7aa"}.fa-chevron-left:before{content:"\f053"}.fa-bacteria:before{content:"\e059"}.fa-hand-lizard:before{content:"\f258"}.fa-notdef:before{content:"\e1fe"}.fa-disease:before{content:"\f7fa"}.fa-briefcase-medical:before{content:"\f469"}.fa-genderless:before{content:"\f22d"}.fa-chevron-right:before{content:"\f054"}.fa-retweet:before{content:"\f079"}.fa-car-alt:before,.fa-car-rear:before{content:"\f5de"}.fa-pump-soap:before{content:"\e06b"}.fa-video-slash:before{content:"\f4e2"}.fa-battery-2:before,.fa-battery-quarter:before{content:"\f243"}.fa-radio:before{content:"\f8d7"}.fa-baby-carriage:before,.fa-carriage-baby:before{content:"\f77d"}.fa-traffic-light:before{content:"\f637"}.fa-thermometer:before{content:"\f491"}.fa-vr-cardboard:before{content:"\f729"}.fa-hand-middle-finger:before{content:"\f806"}.fa-percent:before,.fa-percentage:before{content:"\25"}.fa-truck-moving:before{content:"\f4df"}.fa-glass-water-droplet:before{content:"\e4f5"}.fa-display:before{content:"\e163"}.fa-face-smile:before,.fa-smile:before{content:"\f118"}.fa-thumb-tack:before,.fa-thumbtack:before{content:"\f08d"}.fa-trophy:before{content:"\f091"}.fa-person-praying:before,.fa-pray:before{content:"\f683"}.fa-hammer:before{content:"\f6e3"}.fa-hand-peace:before{content:"\f25b"}.fa-rotate:before,.fa-sync-alt:before{content:"\f2f1"}.fa-spinner:before{content:"\f110"}.fa-robot:before{content:"\f544"}.fa-peace:before{content:"\f67c"}.fa-cogs:before,.fa-gears:before{content:"\f085"}.fa-warehouse:before{content:"\f494"}.fa-arrow-up-right-dots:before{content:"\e4b7"}.fa-splotch:before{content:"\f5bc"}.fa-face-grin-hearts:before,.fa-grin-hearts:before{content:"\f584"}.fa-dice-four:before{content:"\f524"}.fa-sim-card:before{content:"\f7c4"}.fa-transgender-alt:before,.fa-transgender:before{content:"\f225"}.fa-mercury:before{content:"\f223"}.fa-arrow-turn-down:before,.fa-level-down:before{content:"\f149"}.fa-person-falling-burst:before{content:"\e547"}.fa-award:before{content:"\f559"}.fa-ticket-alt:before,.fa-ticket-simple:before{content:"\f3ff"}.fa-building:before{content:"\f1ad"}.fa-angle-double-left:before,.fa-angles-left:before{content:"\f100"}.fa-qrcode:before{content:"\f029"}.fa-clock-rotate-left:before,.fa-history:before{content:"\f1da"}.fa-face-grin-beam-sweat:before,.fa-grin-beam-sweat:before{content:"\f583"}.fa-arrow-right-from-file:before,.fa-file-export:before{content:"\f56e"}.fa-shield-blank:before,.fa-shield:before{content:"\f132"}.fa-arrow-up-short-wide:before,.fa-sort-amount-up-alt:before{content:"\f885"}.fa-house-medical:before{content:"\e3b2"}.fa-golf-ball-tee:before,.fa-golf-ball:before{content:"\f450"}.fa-chevron-circle-left:before,.fa-circle-chevron-left:before{content:"\f137"}.fa-house-chimney-window:before{content:"\e00d"}.fa-pen-nib:before{content:"\f5ad"}.fa-tent-arrow-turn-left:before{content:"\e580"}.fa-tents:before{content:"\e582"}.fa-magic:before,.fa-wand-magic:before{content:"\f0d0"}.fa-dog:before{content:"\f6d3"}.fa-carrot:before{content:"\f787"}.fa-moon:before{content:"\f186"}.fa-wine-glass-alt:before,.fa-wine-glass-empty:before{content:"\f5ce"}.fa-cheese:before{content:"\f7ef"}.fa-yin-yang:before{content:"\f6ad"}.fa-music:before{content:"\f001"}.fa-code-commit:before{content:"\f386"}.fa-temperature-low:before{content:"\f76b"}.fa-biking:before,.fa-person-biking:before{content:"\f84a"}.fa-broom:before{content:"\f51a"}.fa-shield-heart:before{content:"\e574"}.fa-gopuram:before{content:"\f664"}.fa-earth-oceania:before,.fa-globe-oceania:before{content:"\e47b"}.fa-square-xmark:before,.fa-times-square:before,.fa-xmark-square:before{content:"\f2d3"}.fa-hashtag:before{content:"\23"}.fa-expand-alt:before,.fa-up-right-and-down-left-from-center:before{content:"\f424"}.fa-oil-can:before{content:"\f613"}.fa-t:before{content:"\54"}.fa-hippo:before{content:"\f6ed"}.fa-chart-column:before{content:"\e0e3"}.fa-infinity:before{content:"\f534"}.fa-vial-circle-check:before{content:"\e596"}.fa-person-arrow-down-to-line:before{content:"\e538"}.fa-voicemail:before{content:"\f897"}.fa-fan:before{content:"\f863"}.fa-person-walking-luggage:before{content:"\e554"}.fa-arrows-alt-v:before,.fa-up-down:before{content:"\f338"}.fa-cloud-moon-rain:before{content:"\f73c"}.fa-calendar:before{content:"\f133"}.fa-trailer:before{content:"\e041"}.fa-bahai:before,.fa-haykal:before{content:"\f666"}.fa-sd-card:before{content:"\f7c2"}.fa-dragon:before{content:"\f6d5"}.fa-shoe-prints:before{content:"\f54b"}.fa-circle-plus:before,.fa-plus-circle:before{content:"\f055"}.fa-face-grin-tongue-wink:before,.fa-grin-tongue-wink:before{content:"\f58b"}.fa-hand-holding:before{content:"\f4bd"}.fa-plug-circle-exclamation:before{content:"\e55d"}.fa-chain-broken:before,.fa-chain-slash:before,.fa-link-slash:before,.fa-unlink:before{content:"\f127"}.fa-clone:before{content:"\f24d"}.fa-person-walking-arrow-loop-left:before{content:"\e551"}.fa-arrow-up-z-a:before,.fa-sort-alpha-up-alt:before{content:"\f882"}.fa-fire-alt:before,.fa-fire-flame-curved:before{content:"\f7e4"}.fa-tornado:before{content:"\f76f"}.fa-file-circle-plus:before{content:"\e494"}.fa-book-quran:before,.fa-quran:before{content:"\f687"}.fa-anchor:before{content:"\f13d"}.fa-border-all:before{content:"\f84c"}.fa-angry:before,.fa-face-angry:before{content:"\f556"}.fa-cookie-bite:before{content:"\f564"}.fa-arrow-trend-down:before{content:"\e097"}.fa-feed:before,.fa-rss:before{content:"\f09e"}.fa-draw-polygon:before{content:"\f5ee"}.fa-balance-scale:before,.fa-scale-balanced:before{content:"\f24e"}.fa-gauge-simple-high:before,.fa-tachometer-fast:before,.fa-tachometer:before{content:"\f62a"}.fa-shower:before{content:"\f2cc"}.fa-desktop-alt:before,.fa-desktop:before{content:"\f390"}.fa-m:before{content:"\4d"}.fa-table-list:before,.fa-th-list:before{content:"\f00b"}.fa-comment-sms:before,.fa-sms:before{content:"\f7cd"}.fa-book:before{content:"\f02d"}.fa-user-plus:before{content:"\f234"}.fa-check:before{content:"\f00c"}.fa-battery-4:before,.fa-battery-three-quarters:before{content:"\f241"}.fa-house-circle-check:before{content:"\e509"}.fa-angle-left:before{content:"\f104"}.fa-diagram-successor:before{content:"\e47a"}.fa-truck-arrow-right:before{content:"\e58b"}.fa-arrows-split-up-and-left:before{content:"\e4bc"}.fa-fist-raised:before,.fa-hand-fist:before{content:"\f6de"}.fa-cloud-moon:before{content:"\f6c3"}.fa-briefcase:before{content:"\f0b1"}.fa-person-falling:before{content:"\e546"}.fa-image-portrait:before,.fa-portrait:before{content:"\f3e0"}.fa-user-tag:before{content:"\f507"}.fa-rug:before{content:"\e569"}.fa-earth-europe:before,.fa-globe-europe:before{content:"\f7a2"}.fa-cart-flatbed-suitcase:before,.fa-luggage-cart:before{content:"\f59d"}.fa-rectangle-times:before,.fa-rectangle-xmark:before,.fa-times-rectangle:before,.fa-window-close:before{content:"\f410"}.fa-baht-sign:before{content:"\e0ac"}.fa-book-open:before{content:"\f518"}.fa-book-journal-whills:before,.fa-journal-whills:before{content:"\f66a"}.fa-handcuffs:before{content:"\e4f8"}.fa-exclamation-triangle:before,.fa-triangle-exclamation:before,.fa-warning:before{content:"\f071"}.fa-database:before{content:"\f1c0"}.fa-arrow-turn-right:before,.fa-mail-forward:before,.fa-share:before{content:"\f064"}.fa-bottle-droplet:before{content:"\e4c4"}.fa-mask-face:before{content:"\e1d7"}.fa-hill-rockslide:before{content:"\e508"}.fa-exchange-alt:before,.fa-right-left:before{content:"\f362"}.fa-paper-plane:before{content:"\f1d8"}.fa-road-circle-exclamation:before{content:"\e565"}.fa-dungeon:before{content:"\f6d9"}.fa-align-right:before{content:"\f038"}.fa-money-bill-1-wave:before,.fa-money-bill-wave-alt:before{content:"\f53b"}.fa-life-ring:before{content:"\f1cd"}.fa-hands:before,.fa-sign-language:before,.fa-signing:before{content:"\f2a7"}.fa-calendar-day:before{content:"\f783"}.fa-ladder-water:before,.fa-swimming-pool:before,.fa-water-ladder:before{content:"\f5c5"}.fa-arrows-up-down:before,.fa-arrows-v:before{content:"\f07d"}.fa-face-grimace:before,.fa-grimace:before{content:"\f57f"}.fa-wheelchair-alt:before,.fa-wheelchair-move:before{content:"\e2ce"}.fa-level-down-alt:before,.fa-turn-down:before{content:"\f3be"}.fa-person-walking-arrow-right:before{content:"\e552"}.fa-envelope-square:before,.fa-square-envelope:before{content:"\f199"}.fa-dice:before{content:"\f522"}.fa-bowling-ball:before{content:"\f436"}.fa-brain:before{content:"\f5dc"}.fa-band-aid:before,.fa-bandage:before{content:"\f462"}.fa-calendar-minus:before{content:"\f272"}.fa-circle-xmark:before,.fa-times-circle:before,.fa-xmark-circle:before{content:"\f057"}.fa-gifts:before{content:"\f79c"}.fa-hotel:before{content:"\f594"}.fa-earth-asia:before,.fa-globe-asia:before{content:"\f57e"}.fa-id-card-alt:before,.fa-id-card-clip:before{content:"\f47f"}.fa-magnifying-glass-plus:before,.fa-search-plus:before{content:"\f00e"}.fa-thumbs-up:before{content:"\f164"}.fa-user-clock:before{content:"\f4fd"}.fa-allergies:before,.fa-hand-dots:before{content:"\f461"}.fa-file-invoice:before{content:"\f570"}.fa-window-minimize:before{content:"\f2d1"}.fa-coffee:before,.fa-mug-saucer:before{content:"\f0f4"}.fa-brush:before{content:"\f55d"}.fa-mask:before{content:"\f6fa"}.fa-magnifying-glass-minus:before,.fa-search-minus:before{content:"\f010"}.fa-ruler-vertical:before{content:"\f548"}.fa-user-alt:before,.fa-user-large:before{content:"\f406"}.fa-train-tram:before{content:"\e5b4"}.fa-user-nurse:before{content:"\f82f"}.fa-syringe:before{content:"\f48e"}.fa-cloud-sun:before{content:"\f6c4"}.fa-stopwatch-20:before{content:"\e06f"}.fa-square-full:before{content:"\f45c"}.fa-magnet:before{content:"\f076"}.fa-jar:before{content:"\e516"}.fa-note-sticky:before,.fa-sticky-note:before{content:"\f249"}.fa-bug-slash:before{content:"\e490"}.fa-arrow-up-from-water-pump:before{content:"\e4b6"}.fa-bone:before{content:"\f5d7"}.fa-user-injured:before{content:"\f728"}.fa-face-sad-tear:before,.fa-sad-tear:before{content:"\f5b4"}.fa-plane:before{content:"\f072"}.fa-tent-arrows-down:before{content:"\e581"}.fa-exclamation:before{content:"\21"}.fa-arrows-spin:before{content:"\e4bb"}.fa-print:before{content:"\f02f"}.fa-try:before,.fa-turkish-lira-sign:before,.fa-turkish-lira:before{content:"\e2bb"}.fa-dollar-sign:before,.fa-dollar:before,.fa-usd:before{content:"\24"}.fa-x:before{content:"\58"}.fa-magnifying-glass-dollar:before,.fa-search-dollar:before{content:"\f688"}.fa-users-cog:before,.fa-users-gear:before{content:"\f509"}.fa-person-military-pointing:before{content:"\e54a"}.fa-bank:before,.fa-building-columns:before,.fa-institution:before,.fa-museum:before,.fa-university:before{content:"\f19c"}.fa-umbrella:before{content:"\f0e9"}.fa-trowel:before{content:"\e589"}.fa-d:before{content:"\44"}.fa-stapler:before{content:"\e5af"}.fa-masks-theater:before,.fa-theater-masks:before{content:"\f630"}.fa-kip-sign:before{content:"\e1c4"}.fa-hand-point-left:before{content:"\f0a5"}.fa-handshake-alt:before,.fa-handshake-simple:before{content:"\f4c6"}.fa-fighter-jet:before,.fa-jet-fighter:before{content:"\f0fb"}.fa-share-alt-square:before,.fa-square-share-nodes:before{content:"\f1e1"}.fa-barcode:before{content:"\f02a"}.fa-plus-minus:before{content:"\e43c"}.fa-video-camera:before,.fa-video:before{content:"\f03d"}.fa-graduation-cap:before,.fa-mortar-board:before{content:"\f19d"}.fa-hand-holding-medical:before{content:"\e05c"}.fa-person-circle-check:before{content:"\e53e"}.fa-level-up-alt:before,.fa-turn-up:before{content:"\f3bf"}.fa-sr-only,.fa-sr-only-focusable:not(:focus),.sr-only,.sr-only-focusable:not(:focus){position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);white-space:nowrap;border-width:0}:host,:root{--fa-style-family-brands:"Font Awesome 6 Brands";--fa-font-brands:normal 400 1em/1 "Font Awesome 6 Brands"}@font-face{font-family:"Font Awesome 6 Brands";font-style:normal;font-weight:400;font-display:block;src:url(../webfonts/fa-brands-400.woff2) format("woff2"),url(../webfonts/fa-brands-400.ttf) format("truetype")}.fa-brands,.fab{font-weight:400}.fa-monero:before{content:"\f3d0"}.fa-hooli:before{content:"\f427"}.fa-yelp:before{content:"\f1e9"}.fa-cc-visa:before{content:"\f1f0"}.fa-lastfm:before{content:"\f202"}.fa-shopware:before{content:"\f5b5"}.fa-creative-commons-nc:before{content:"\f4e8"}.fa-aws:before{content:"\f375"}.fa-redhat:before{content:"\f7bc"}.fa-yoast:before{content:"\f2b1"}.fa-cloudflare:before{content:"\e07d"}.fa-ups:before{content:"\f7e0"}.fa-wpexplorer:before{content:"\f2de"}.fa-dyalog:before{content:"\f399"}.fa-bity:before{content:"\f37a"}.fa-stackpath:before{content:"\f842"}.fa-buysellads:before{content:"\f20d"}.fa-first-order:before{content:"\f2b0"}.fa-modx:before{content:"\f285"}.fa-guilded:before{content:"\e07e"}.fa-vnv:before{content:"\f40b"}.fa-js-square:before,.fa-square-js:before{content:"\f3b9"}.fa-microsoft:before{content:"\f3ca"}.fa-qq:before{content:"\f1d6"}.fa-orcid:before{content:"\f8d2"}.fa-java:before{content:"\f4e4"}.fa-invision:before{content:"\f7b0"}.fa-creative-commons-pd-alt:before{content:"\f4ed"}.fa-centercode:before{content:"\f380"}.fa-glide-g:before{content:"\f2a6"}.fa-drupal:before{content:"\f1a9"}.fa-hire-a-helper:before{content:"\f3b0"}.fa-creative-commons-by:before{content:"\f4e7"}.fa-unity:before{content:"\e049"}.fa-whmcs:before{content:"\f40d"}.fa-rocketchat:before{content:"\f3e8"}.fa-vk:before{content:"\f189"}.fa-untappd:before{content:"\f405"}.fa-mailchimp:before{content:"\f59e"}.fa-css3-alt:before{content:"\f38b"}.fa-reddit-square:before,.fa-square-reddit:before{content:"\f1a2"}.fa-vimeo-v:before{content:"\f27d"}.fa-contao:before{content:"\f26d"}.fa-square-font-awesome:before{content:"\e5ad"}.fa-deskpro:before{content:"\f38f"}.fa-sistrix:before{content:"\f3ee"}.fa-instagram-square:before,.fa-square-instagram:before{content:"\e055"}.fa-battle-net:before{content:"\f835"}.fa-the-red-yeti:before{content:"\f69d"}.fa-hacker-news-square:before,.fa-square-hacker-news:before{content:"\f3af"}.fa-edge:before{content:"\f282"}.fa-napster:before{content:"\f3d2"}.fa-snapchat-square:before,.fa-square-snapchat:before{content:"\f2ad"}.fa-google-plus-g:before{content:"\f0d5"}.fa-artstation:before{content:"\f77a"}.fa-markdown:before{content:"\f60f"}.fa-sourcetree:before{content:"\f7d3"}.fa-google-plus:before{content:"\f2b3"}.fa-diaspora:before{content:"\f791"}.fa-foursquare:before{content:"\f180"}.fa-stack-overflow:before{content:"\f16c"}.fa-github-alt:before{content:"\f113"}.fa-phoenix-squadron:before{content:"\f511"}.fa-pagelines:before{content:"\f18c"}.fa-algolia:before{content:"\f36c"}.fa-red-river:before{content:"\f3e3"}.fa-creative-commons-sa:before{content:"\f4ef"}.fa-safari:before{content:"\f267"}.fa-google:before{content:"\f1a0"}.fa-font-awesome-alt:before,.fa-square-font-awesome-stroke:before{content:"\f35c"}.fa-atlassian:before{content:"\f77b"}.fa-linkedin-in:before{content:"\f0e1"}.fa-digital-ocean:before{content:"\f391"}.fa-nimblr:before{content:"\f5a8"}.fa-chromecast:before{content:"\f838"}.fa-evernote:before{content:"\f839"}.fa-hacker-news:before{content:"\f1d4"}.fa-creative-commons-sampling:before{content:"\f4f0"}.fa-adversal:before{content:"\f36a"}.fa-creative-commons:before{content:"\f25e"}.fa-watchman-monitoring:before{content:"\e087"}.fa-fonticons:before{content:"\f280"}.fa-weixin:before{content:"\f1d7"}.fa-shirtsinbulk:before{content:"\f214"}.fa-codepen:before{content:"\f1cb"}.fa-git-alt:before{content:"\f841"}.fa-lyft:before{content:"\f3c3"}.fa-rev:before{content:"\f5b2"}.fa-windows:before{content:"\f17a"}.fa-wizards-of-the-coast:before{content:"\f730"}.fa-square-viadeo:before,.fa-viadeo-square:before{content:"\f2aa"}.fa-meetup:before{content:"\f2e0"}.fa-centos:before{content:"\f789"}.fa-adn:before{content:"\f170"}.fa-cloudsmith:before{content:"\f384"}.fa-pied-piper-alt:before{content:"\f1a8"}.fa-dribbble-square:before,.fa-square-dribbble:before{content:"\f397"}.fa-codiepie:before{content:"\f284"}.fa-node:before{content:"\f419"}.fa-mix:before{content:"\f3cb"}.fa-steam:before{content:"\f1b6"}.fa-cc-apple-pay:before{content:"\f416"}.fa-scribd:before{content:"\f28a"}.fa-openid:before{content:"\f19b"}.fa-instalod:before{content:"\e081"}.fa-expeditedssl:before{content:"\f23e"}.fa-sellcast:before{content:"\f2da"}.fa-square-twitter:before,.fa-twitter-square:before{content:"\f081"}.fa-r-project:before{content:"\f4f7"}.fa-delicious:before{content:"\f1a5"}.fa-freebsd:before{content:"\f3a4"}.fa-vuejs:before{content:"\f41f"}.fa-accusoft:before{content:"\f369"}.fa-ioxhost:before{content:"\f208"}.fa-fonticons-fi:before{content:"\f3a2"}.fa-app-store:before{content:"\f36f"}.fa-cc-mastercard:before{content:"\f1f1"}.fa-itunes-note:before{content:"\f3b5"}.fa-golang:before{content:"\e40f"}.fa-kickstarter:before{content:"\f3bb"}.fa-grav:before{content:"\f2d6"}.fa-weibo:before{content:"\f18a"}.fa-uncharted:before{content:"\e084"}.fa-firstdraft:before{content:"\f3a1"}.fa-square-youtube:before,.fa-youtube-square:before{content:"\f431"}.fa-wikipedia-w:before{content:"\f266"}.fa-rendact:before,.fa-wpressr:before{content:"\f3e4"}.fa-angellist:before{content:"\f209"}.fa-galactic-republic:before{content:"\f50c"}.fa-nfc-directional:before{content:"\e530"}.fa-skype:before{content:"\f17e"}.fa-joget:before{content:"\f3b7"}.fa-fedora:before{content:"\f798"}.fa-stripe-s:before{content:"\f42a"}.fa-meta:before{content:"\e49b"}.fa-laravel:before{content:"\f3bd"}.fa-hotjar:before{content:"\f3b1"}.fa-bluetooth-b:before{content:"\f294"}.fa-sticker-mule:before{content:"\f3f7"}.fa-creative-commons-zero:before{content:"\f4f3"}.fa-hips:before{content:"\f452"}.fa-behance:before{content:"\f1b4"}.fa-reddit:before{content:"\f1a1"}.fa-discord:before{content:"\f392"}.fa-chrome:before{content:"\f268"}.fa-app-store-ios:before{content:"\f370"}.fa-cc-discover:before{content:"\f1f2"}.fa-wpbeginner:before{content:"\f297"}.fa-confluence:before{content:"\f78d"}.fa-mdb:before{content:"\f8ca"}.fa-dochub:before{content:"\f394"}.fa-accessible-icon:before{content:"\f368"}.fa-ebay:before{content:"\f4f4"}.fa-amazon:before{content:"\f270"}.fa-unsplash:before{content:"\e07c"}.fa-yarn:before{content:"\f7e3"}.fa-square-steam:before,.fa-steam-square:before{content:"\f1b7"}.fa-500px:before{content:"\f26e"}.fa-square-vimeo:before,.fa-vimeo-square:before{content:"\f194"}.fa-asymmetrik:before{content:"\f372"}.fa-font-awesome-flag:before,.fa-font-awesome-logo-full:before,.fa-font-awesome:before{content:"\f2b4"}.fa-gratipay:before{content:"\f184"}.fa-apple:before{content:"\f179"}.fa-hive:before{content:"\e07f"}.fa-gitkraken:before{content:"\f3a6"}.fa-keybase:before{content:"\f4f5"}.fa-apple-pay:before{content:"\f415"}.fa-padlet:before{content:"\e4a0"}.fa-amazon-pay:before{content:"\f42c"}.fa-github-square:before,.fa-square-github:before{content:"\f092"}.fa-stumbleupon:before{content:"\f1a4"}.fa-fedex:before{content:"\f797"}.fa-phoenix-framework:before{content:"\f3dc"}.fa-shopify:before{content:"\e057"}.fa-neos:before{content:"\f612"}.fa-hackerrank:before{content:"\f5f7"}.fa-researchgate:before{content:"\f4f8"}.fa-swift:before{content:"\f8e1"}.fa-angular:before{content:"\f420"}.fa-speakap:before{content:"\f3f3"}.fa-angrycreative:before{content:"\f36e"}.fa-y-combinator:before{content:"\f23b"}.fa-empire:before{content:"\f1d1"}.fa-envira:before{content:"\f299"}.fa-gitlab-square:before,.fa-square-gitlab:before{content:"\e5ae"}.fa-studiovinari:before{content:"\f3f8"}.fa-pied-piper:before{content:"\f2ae"}.fa-wordpress:before{content:"\f19a"}.fa-product-hunt:before{content:"\f288"}.fa-firefox:before{content:"\f269"}.fa-linode:before{content:"\f2b8"}.fa-goodreads:before{content:"\f3a8"}.fa-odnoklassniki-square:before,.fa-square-odnoklassniki:before{content:"\f264"}.fa-jsfiddle:before{content:"\f1cc"}.fa-sith:before{content:"\f512"}.fa-themeisle:before{content:"\f2b2"}.fa-page4:before{content:"\f3d7"}.fa-hashnode:before{content:"\e499"}.fa-react:before{content:"\f41b"}.fa-cc-paypal:before{content:"\f1f4"}.fa-squarespace:before{content:"\f5be"}.fa-cc-stripe:before{content:"\f1f5"}.fa-creative-commons-share:before{content:"\f4f2"}.fa-bitcoin:before{content:"\f379"}.fa-keycdn:before{content:"\f3ba"}.fa-opera:before{content:"\f26a"}.fa-itch-io:before{content:"\f83a"}.fa-umbraco:before{content:"\f8e8"}.fa-galactic-senate:before{content:"\f50d"}.fa-ubuntu:before{content:"\f7df"}.fa-draft2digital:before{content:"\f396"}.fa-stripe:before{content:"\f429"}.fa-houzz:before{content:"\f27c"}.fa-gg:before{content:"\f260"}.fa-dhl:before{content:"\f790"}.fa-pinterest-square:before,.fa-square-pinterest:before{content:"\f0d3"}.fa-xing:before{content:"\f168"}.fa-blackberry:before{content:"\f37b"}.fa-creative-commons-pd:before{content:"\f4ec"}.fa-playstation:before{content:"\f3df"}.fa-quinscape:before{content:"\f459"}.fa-less:before{content:"\f41d"}.fa-blogger-b:before{content:"\f37d"}.fa-opencart:before{content:"\f23d"}.fa-vine:before{content:"\f1ca"}.fa-paypal:before{content:"\f1ed"}.fa-gitlab:before{content:"\f296"}.fa-typo3:before{content:"\f42b"}.fa-reddit-alien:before{content:"\f281"}.fa-yahoo:before{content:"\f19e"}.fa-dailymotion:before{content:"\e052"}.fa-affiliatetheme:before{content:"\f36b"}.fa-pied-piper-pp:before{content:"\f1a7"}.fa-bootstrap:before{content:"\f836"}.fa-odnoklassniki:before{content:"\f263"}.fa-nfc-symbol:before{content:"\e531"}.fa-ethereum:before{content:"\f42e"}.fa-speaker-deck:before{content:"\f83c"}.fa-creative-commons-nc-eu:before{content:"\f4e9"}.fa-patreon:before{content:"\f3d9"}.fa-avianex:before{content:"\f374"}.fa-ello:before{content:"\f5f1"}.fa-gofore:before{content:"\f3a7"}.fa-bimobject:before{content:"\f378"}.fa-facebook-f:before{content:"\f39e"}.fa-google-plus-square:before,.fa-square-google-plus:before{content:"\f0d4"}.fa-mandalorian:before{content:"\f50f"}.fa-first-order-alt:before{content:"\f50a"}.fa-osi:before{content:"\f41a"}.fa-google-wallet:before{content:"\f1ee"}.fa-d-and-d-beyond:before{content:"\f6ca"}.fa-periscope:before{content:"\f3da"}.fa-fulcrum:before{content:"\f50b"}.fa-cloudscale:before{content:"\f383"}.fa-forumbee:before{content:"\f211"}.fa-mizuni:before{content:"\f3cc"}.fa-schlix:before{content:"\f3ea"}.fa-square-xing:before,.fa-xing-square:before{content:"\f169"}.fa-bandcamp:before{content:"\f2d5"}.fa-wpforms:before{content:"\f298"}.fa-cloudversify:before{content:"\f385"}.fa-usps:before{content:"\f7e1"}.fa-megaport:before{content:"\f5a3"}.fa-magento:before{content:"\f3c4"}.fa-spotify:before{content:"\f1bc"}.fa-optin-monster:before{content:"\f23c"}.fa-fly:before{content:"\f417"}.fa-aviato:before{content:"\f421"}.fa-itunes:before{content:"\f3b4"}.fa-cuttlefish:before{content:"\f38c"}.fa-blogger:before{content:"\f37c"}.fa-flickr:before{content:"\f16e"}.fa-viber:before{content:"\f409"}.fa-soundcloud:before{content:"\f1be"}.fa-digg:before{content:"\f1a6"}.fa-tencent-weibo:before{content:"\f1d5"}.fa-symfony:before{content:"\f83d"}.fa-maxcdn:before{content:"\f136"}.fa-etsy:before{content:"\f2d7"}.fa-facebook-messenger:before{content:"\f39f"}.fa-audible:before{content:"\f373"}.fa-think-peaks:before{content:"\f731"}.fa-bilibili:before{content:"\e3d9"}.fa-erlang:before{content:"\f39d"}.fa-cotton-bureau:before{content:"\f89e"}.fa-dashcube:before{content:"\f210"}.fa-42-group:before,.fa-innosoft:before{content:"\e080"}.fa-stack-exchange:before{content:"\f18d"}.fa-elementor:before{content:"\f430"}.fa-pied-piper-square:before,.fa-square-pied-piper:before{content:"\e01e"}.fa-creative-commons-nd:before{content:"\f4eb"}.fa-palfed:before{content:"\f3d8"}.fa-superpowers:before{content:"\f2dd"}.fa-resolving:before{content:"\f3e7"}.fa-xbox:before{content:"\f412"}.fa-searchengin:before{content:"\f3eb"}.fa-tiktok:before{content:"\e07b"}.fa-facebook-square:before,.fa-square-facebook:before{content:"\f082"}.fa-renren:before{content:"\f18b"}.fa-linux:before{content:"\f17c"}.fa-glide:before{content:"\f2a5"}.fa-linkedin:before{content:"\f08c"}.fa-hubspot:before{content:"\f3b2"}.fa-deploydog:before{content:"\f38e"}.fa-twitch:before{content:"\f1e8"}.fa-ravelry:before{content:"\f2d9"}.fa-mixer:before{content:"\e056"}.fa-lastfm-square:before,.fa-square-lastfm:before{content:"\f203"}.fa-vimeo:before{content:"\f40a"}.fa-mendeley:before{content:"\f7b3"}.fa-uniregistry:before{content:"\f404"}.fa-figma:before{content:"\f799"}.fa-creative-commons-remix:before{content:"\f4ee"}.fa-cc-amazon-pay:before{content:"\f42d"}.fa-dropbox:before{content:"\f16b"}.fa-instagram:before{content:"\f16d"}.fa-cmplid:before{content:"\e360"}.fa-facebook:before{content:"\f09a"}.fa-gripfire:before{content:"\f3ac"}.fa-jedi-order:before{content:"\f50e"}.fa-uikit:before{content:"\f403"}.fa-fort-awesome-alt:before{content:"\f3a3"}.fa-phabricator:before{content:"\f3db"}.fa-ussunnah:before{content:"\f407"}.fa-earlybirds:before{content:"\f39a"}.fa-trade-federation:before{content:"\f513"}.fa-autoprefixer:before{content:"\f41c"}.fa-whatsapp:before{content:"\f232"}.fa-slideshare:before{content:"\f1e7"}.fa-google-play:before{content:"\f3ab"}.fa-viadeo:before{content:"\f2a9"}.fa-line:before{content:"\f3c0"}.fa-google-drive:before{content:"\f3aa"}.fa-servicestack:before{content:"\f3ec"}.fa-simplybuilt:before{content:"\f215"}.fa-bitbucket:before{content:"\f171"}.fa-imdb:before{content:"\f2d8"}.fa-deezer:before{content:"\e077"}.fa-raspberry-pi:before{content:"\f7bb"}.fa-jira:before{content:"\f7b1"}.fa-docker:before{content:"\f395"}.fa-screenpal:before{content:"\e570"}.fa-bluetooth:before{content:"\f293"}.fa-gitter:before{content:"\f426"}.fa-d-and-d:before{content:"\f38d"}.fa-microblog:before{content:"\e01a"}.fa-cc-diners-club:before{content:"\f24c"}.fa-gg-circle:before{content:"\f261"}.fa-pied-piper-hat:before{content:"\f4e5"}.fa-kickstarter-k:before{content:"\f3bc"}.fa-yandex:before{content:"\f413"}.fa-readme:before{content:"\f4d5"}.fa-html5:before{content:"\f13b"}.fa-sellsy:before{content:"\f213"}.fa-sass:before{content:"\f41e"}.fa-wirsindhandwerk:before,.fa-wsh:before{content:"\e2d0"}.fa-buromobelexperte:before{content:"\f37f"}.fa-salesforce:before{content:"\f83b"}.fa-octopus-deploy:before{content:"\e082"}.fa-medapps:before{content:"\f3c6"}.fa-ns8:before{content:"\f3d5"}.fa-pinterest-p:before{content:"\f231"}.fa-apper:before{content:"\f371"}.fa-fort-awesome:before{content:"\f286"}.fa-waze:before{content:"\f83f"}.fa-cc-jcb:before{content:"\f24b"}.fa-snapchat-ghost:before,.fa-snapchat:before{content:"\f2ab"}.fa-fantasy-flight-games:before{content:"\f6dc"}.fa-rust:before{content:"\e07a"}.fa-wix:before{content:"\f5cf"}.fa-behance-square:before,.fa-square-behance:before{content:"\f1b5"}.fa-supple:before{content:"\f3f9"}.fa-rebel:before{content:"\f1d0"}.fa-css3:before{content:"\f13c"}.fa-staylinked:before{content:"\f3f5"}.fa-kaggle:before{content:"\f5fa"}.fa-space-awesome:before{content:"\e5ac"}.fa-deviantart:before{content:"\f1bd"}.fa-cpanel:before{content:"\f388"}.fa-goodreads-g:before{content:"\f3a9"}.fa-git-square:before,.fa-square-git:before{content:"\f1d2"}.fa-square-tumblr:before,.fa-tumblr-square:before{content:"\f174"}.fa-trello:before{content:"\f181"}.fa-creative-commons-nc-jp:before{content:"\f4ea"}.fa-get-pocket:before{content:"\f265"}.fa-perbyte:before{content:"\e083"}.fa-grunt:before{content:"\f3ad"}.fa-weebly:before{content:"\f5cc"}.fa-connectdevelop:before{content:"\f20e"}.fa-leanpub:before{content:"\f212"}.fa-black-tie:before{content:"\f27e"}.fa-themeco:before{content:"\f5c6"}.fa-python:before{content:"\f3e2"}.fa-android:before{content:"\f17b"}.fa-bots:before{content:"\e340"}.fa-free-code-camp:before{content:"\f2c5"}.fa-hornbill:before{content:"\f592"}.fa-js:before{content:"\f3b8"}.fa-ideal:before{content:"\e013"}.fa-git:before{content:"\f1d3"}.fa-dev:before{content:"\f6cc"}.fa-sketch:before{content:"\f7c6"}.fa-yandex-international:before{content:"\f414"}.fa-cc-amex:before{content:"\f1f3"}.fa-uber:before{content:"\f402"}.fa-github:before{content:"\f09b"}.fa-php:before{content:"\f457"}.fa-alipay:before{content:"\f642"}.fa-youtube:before{content:"\f167"}.fa-skyatlas:before{content:"\f216"}.fa-firefox-browser:before{content:"\e007"}.fa-replyd:before{content:"\f3e6"}.fa-suse:before{content:"\f7d6"}.fa-jenkins:before{content:"\f3b6"}.fa-twitter:before{content:"\f099"}.fa-rockrms:before{content:"\f3e9"}.fa-pinterest:before{content:"\f0d2"}.fa-buffer:before{content:"\f837"}.fa-npm:before{content:"\f3d4"}.fa-yammer:before{content:"\f840"}.fa-btc:before{content:"\f15a"}.fa-dribbble:before{content:"\f17d"}.fa-stumbleupon-circle:before{content:"\f1a3"}.fa-internet-explorer:before{content:"\f26b"}.fa-telegram-plane:before,.fa-telegram:before{content:"\f2c6"}.fa-old-republic:before{content:"\f510"}.fa-square-whatsapp:before,.fa-whatsapp-square:before{content:"\f40c"}.fa-node-js:before{content:"\f3d3"}.fa-edge-legacy:before{content:"\e078"}.fa-slack-hash:before,.fa-slack:before{content:"\f198"}.fa-medrt:before{content:"\f3c8"}.fa-usb:before{content:"\f287"}.fa-tumblr:before{content:"\f173"}.fa-vaadin:before{content:"\f408"}.fa-quora:before{content:"\f2c4"}.fa-reacteurope:before{content:"\f75d"}.fa-medium-m:before,.fa-medium:before{content:"\f23a"}.fa-amilia:before{content:"\f36d"}.fa-mixcloud:before{content:"\f289"}.fa-flipboard:before{content:"\f44d"}.fa-viacoin:before{content:"\f237"}.fa-critical-role:before{content:"\f6c9"}.fa-sitrox:before{content:"\e44a"}.fa-discourse:before{content:"\f393"}.fa-joomla:before{content:"\f1aa"}.fa-mastodon:before{content:"\f4f6"}.fa-airbnb:before{content:"\f834"}.fa-wolf-pack-battalion:before{content:"\f514"}.fa-buy-n-large:before{content:"\f8a6"}.fa-gulp:before{content:"\f3ae"}.fa-creative-commons-sampling-plus:before{content:"\f4f1"}.fa-strava:before{content:"\f428"}.fa-ember:before{content:"\f423"}.fa-canadian-maple-leaf:before{content:"\f785"}.fa-teamspeak:before{content:"\f4f9"}.fa-pushed:before{content:"\f3e1"}.fa-wordpress-simple:before{content:"\f411"}.fa-nutritionix:before{content:"\f3d6"}.fa-wodu:before{content:"\e088"}.fa-google-pay:before{content:"\e079"}.fa-intercom:before{content:"\f7af"}.fa-zhihu:before{content:"\f63f"}.fa-korvue:before{content:"\f42f"}.fa-pix:before{content:"\e43a"}.fa-steam-symbol:before{content:"\f3f6"}:host,:root{--fa-font-regular:normal 400 1em/1 "Font Awesome 6 Free"}@font-face{font-family:"Font Awesome 6 Free";font-style:normal;font-weight:400;font-display:block;src:url(../webfonts/fa-regular-400.woff2) format("woff2"),url(../webfonts/fa-regular-400.ttf) format("truetype")}.fa-regular,.far{font-weight:400}:host,:root{--fa-style-family-classic:"Font Awesome 6 Free";--fa-font-solid:normal 900 1em/1 "Font Awesome 6 Free"}@font-face{font-family:"Font Awesome 6 Free";font-style:normal;font-weight:900;font-display:block;src:url(../webfonts/fa-solid-900.woff2) format("woff2"),url(../webfonts/fa-solid-900.ttf) format("truetype")}.fa-solid,.fas{font-weight:900}@font-face{font-family:"Font Awesome 5 Brands";font-display:block;font-weight:400;src:url(../webfonts/fa-brands-400.woff2) format("woff2"),url(../webfonts/fa-brands-400.ttf) format("truetype")}@font-face{font-family:"Font Awesome 5 Free";font-display:block;font-weight:900;src:url(../webfonts/fa-solid-900.woff2) format("woff2"),url(../webfonts/fa-solid-900.ttf) format("truetype")}@font-face{font-family:"Font Awesome 5 Free";font-display:block;font-weight:400;src:url(../webfonts/fa-regular-400.woff2) format("woff2"),url(../webfonts/fa-regular-400.ttf) format("truetype")}@font-face{font-family:"FontAwesome";font-display:block;src:url(../webfonts/fa-solid-900.woff2) format("woff2"),url(../webfonts/fa-solid-900.ttf) format("truetype")}@font-face{font-family:"FontAwesome";font-display:block;src:url(../webfonts/fa-brands-400.woff2) format("woff2"),url(../webfonts/fa-brands-400.ttf) format("truetype")}@font-face{font-family:"FontAwesome";font-display:block;src:url(../webfonts/fa-regular-400.woff2) format("woff2"),url(../webfonts/fa-regular-400.ttf) format("truetype");unicode-range:u+f003,u+f006,u+f014,u+f016-f017,u+f01a-f01b,u+f01d,u+f022,u+f03e,u+f044,u+f046,u+f05c-f05d,u+f06e,u+f070,u+f087-f088,u+f08a,u+f094,u+f096-f097,u+f09d,u+f0a0,u+f0a2,u+f0a4-f0a7,u+f0c5,u+f0c7,u+f0e5-f0e6,u+f0eb,u+f0f6-f0f8,u+f10c,u+f114-f115,u+f118-f11a,u+f11c-f11d,u+f133,u+f147,u+f14e,u+f150-f152,u+f185-f186,u+f18e,u+f190-f192,u+f196,u+f1c1-f1c9,u+f1d9,u+f1db,u+f1e3,u+f1ea,u+f1f7,u+f1f9,u+f20a,u+f247-f248,u+f24a,u+f24d,u+f255-f25b,u+f25d,u+f271-f274,u+f278,u+f27b,u+f28c,u+f28e,u+f29c,u+f2b5,u+f2b7,u+f2ba,u+f2bc,u+f2be,u+f2c0-f2c1,u+f2c3,u+f2d0,u+f2d2,u+f2d4,u+f2dc}@font-face{font-family:"FontAwesome";font-display:block;src:url(../webfonts/fa-v4compatibility.woff2) format("woff2"),url(../webfonts/fa-v4compatibility.ttf) format("truetype");unicode-range:u+f041,u+f047,u+f065-f066,u+f07d-f07e,u+f080,u+f08b,u+f08e,u+f090,u+f09a,u+f0ac,u+f0ae,u+f0b2,u+f0d0,u+f0d6,u+f0e4,u+f0ec,u+f10a-f10b,u+f123,u+f13e,u+f148-f149,u+f14c,u+f156,u+f15e,u+f160-f161,u+f163,u+f175-f178,u+f195,u+f1f8,u+f219,u+f27a}
+.fa{font-family:var(--fa-style-family,"Font Awesome 6 Free");font-weight:var(--fa-style,900)}.fa,.fa-brands,.fa-classic,.fa-regular,.fa-sharp,.fa-solid,.fab,.far,.fas{-moz-osx-font-smoothing:grayscale;-webkit-font-smoothing:antialiased;display:var(--fa-display,inline-block);font-style:normal;font-variant:normal;line-height:1;text-rendering:auto}.fa-classic,.fa-regular,.fa-solid,.far,.fas{font-family:"Font Awesome 6 Free"}.fa-brands,.fab{font-family:"Font Awesome 6 Brands"}.fa-1x{font-size:1em}.fa-2x{font-size:2em}.fa-3x{font-size:3em}.fa-4x{font-size:4em}.fa-5x{font-size:5em}.fa-6x{font-size:6em}.fa-7x{font-size:7em}.fa-8x{font-size:8em}.fa-9x{font-size:9em}.fa-10x{font-size:10em}.fa-2xs{font-size:.625em;line-height:.1em;vertical-align:.225em}.fa-xs{font-size:.75em;line-height:.08333em;vertical-align:.125em}.fa-sm{font-size:.875em;line-height:.07143em;vertical-align:.05357em}.fa-lg{font-size:1.25em;line-height:.05em;vertical-align:-.075em}.fa-xl{font-size:1.5em;line-height:.04167em;vertical-align:-.125em}.fa-2xl{font-size:2em;line-height:.03125em;vertical-align:-.1875em}.fa-fw{text-align:center;width:1.25em}.fa-ul{list-style-type:none;margin-left:var(--fa-li-margin,2.5em);padding-left:0}.fa-ul>li{position:relative}.fa-li{left:calc(var(--fa-li-width, 2em)*-1);position:absolute;text-align:center;width:var(--fa-li-width,2em);line-height:inherit}.fa-border{border-radius:var(--fa-border-radius,.1em);border:var(--fa-border-width,.08em) var(--fa-border-style,solid) var(--fa-border-color,#eee);padding:var(--fa-border-padding,.2em .25em .15em)}.fa-pull-left{float:left;margin-right:var(--fa-pull-margin,.3em)}.fa-pull-right{float:right;margin-left:var(--fa-pull-margin,.3em)}.fa-beat{-webkit-animation-name:fa-beat;animation-name:fa-beat;-webkit-animation-delay:var(--fa-animation-delay,0s);animation-delay:var(--fa-animation-delay,0s);-webkit-animation-direction:var(--fa-animation-direction,normal);animation-direction:var(--fa-animation-direction,normal);-webkit-animation-duration:var(--fa-animation-duration,1s);animation-duration:var(--fa-animation-duration,1s);-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,ease-in-out);animation-timing-function:var(--fa-animation-timing,ease-in-out)}.fa-bounce{-webkit-animation-name:fa-bounce;animation-name:fa-bounce;-webkit-animation-delay:var(--fa-animation-delay,0s);animation-delay:var(--fa-animation-delay,0s);-webkit-animation-direction:var(--fa-animation-direction,normal);animation-direction:var(--fa-animation-direction,normal);-webkit-animation-duration:var(--fa-animation-duration,1s);animation-duration:var(--fa-animation-duration,1s);-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,cubic-bezier(.28,.84,.42,1));animation-timing-function:var(--fa-animation-timing,cubic-bezier(.28,.84,.42,1))}.fa-fade{-webkit-animation-name:fa-fade;animation-name:fa-fade;-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,cubic-bezier(.4,0,.6,1));animation-timing-function:var(--fa-animation-timing,cubic-bezier(.4,0,.6,1))}.fa-beat-fade,.fa-fade{-webkit-animation-delay:var(--fa-animation-delay,0s);animation-delay:var(--fa-animation-delay,0s);-webkit-animation-direction:var(--fa-animation-direction,normal);animation-direction:var(--fa-animation-direction,normal);-webkit-animation-duration:var(--fa-animation-duration,1s);animation-duration:var(--fa-animation-duration,1s)}.fa-beat-fade{-webkit-animation-name:fa-beat-fade;animation-name:fa-beat-fade;-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,cubic-bezier(.4,0,.6,1));animation-timing-function:var(--fa-animation-timing,cubic-bezier(.4,0,.6,1))}.fa-flip{-webkit-animation-name:fa-flip;animation-name:fa-flip;-webkit-animation-delay:var(--fa-animation-delay,0s);animation-delay:var(--fa-animation-delay,0s);-webkit-animation-direction:var(--fa-animation-direction,normal);animation-direction:var(--fa-animation-direction,normal);-webkit-animation-duration:var(--fa-animation-duration,1s);animation-duration:var(--fa-animation-duration,1s);-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,ease-in-out);animation-timing-function:var(--fa-animation-timing,ease-in-out)}.fa-shake{-webkit-animation-name:fa-shake;animation-name:fa-shake;-webkit-animation-duration:var(--fa-animation-duration,1s);animation-duration:var(--fa-animation-duration,1s);-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,linear);animation-timing-function:var(--fa-animation-timing,linear)}.fa-shake,.fa-spin{-webkit-animation-delay:var(--fa-animation-delay,0s);animation-delay:var(--fa-animation-delay,0s);-webkit-animation-direction:var(--fa-animation-direction,normal);animation-direction:var(--fa-animation-direction,normal)}.fa-spin{-webkit-animation-name:fa-spin;animation-name:fa-spin;-webkit-animation-duration:var(--fa-animation-duration,2s);animation-duration:var(--fa-animation-duration,2s);-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,linear);animation-timing-function:var(--fa-animation-timing,linear)}.fa-spin-reverse{--fa-animation-direction:reverse}.fa-pulse,.fa-spin-pulse{-webkit-animation-name:fa-spin;animation-name:fa-spin;-webkit-animation-direction:var(--fa-animation-direction,normal);animation-direction:var(--fa-animation-direction,normal);-webkit-animation-duration:var(--fa-animation-duration,1s);animation-duration:var(--fa-animation-duration,1s);-webkit-animation-iteration-count:var(--fa-animation-iteration-count,infinite);animation-iteration-count:var(--fa-animation-iteration-count,infinite);-webkit-animation-timing-function:var(--fa-animation-timing,steps(8));animation-timing-function:var(--fa-animation-timing,steps(8))}@media (prefers-reduced-motion:reduce){.fa-beat,.fa-beat-fade,.fa-bounce,.fa-fade,.fa-flip,.fa-pulse,.fa-shake,.fa-spin,.fa-spin-pulse{-webkit-animation-delay:-1ms;animation-delay:-1ms;-webkit-animation-duration:1ms;animation-duration:1ms;-webkit-animation-iteration-count:1;animation-iteration-count:1;transition-delay:0s;transition-duration:0s}}@-webkit-keyframes fa-beat{0%,90%{-webkit-transform:scale(1);transform:scale(1)}45%{-webkit-transform:scale(var(--fa-beat-scale,1.25));transform:scale(var(--fa-beat-scale,1.25))}}@keyframes fa-beat{0%,90%{-webkit-transform:scale(1);transform:scale(1)}45%{-webkit-transform:scale(var(--fa-beat-scale,1.25));transform:scale(var(--fa-beat-scale,1.25))}}@-webkit-keyframes fa-bounce{0%{-webkit-transform:scale(1) translateY(0);transform:scale(1) translateY(0)}10%{-webkit-transform:scale(var(--fa-bounce-start-scale-x,1.1),var(--fa-bounce-start-scale-y,.9)) translateY(0);transform:scale(var(--fa-bounce-start-scale-x,1.1),var(--fa-bounce-start-scale-y,.9)) translateY(0)}30%{-webkit-transform:scale(var(--fa-bounce-jump-scale-x,.9),var(--fa-bounce-jump-scale-y,1.1)) translateY(var(--fa-bounce-height,-.5em));transform:scale(var(--fa-bounce-jump-scale-x,.9),var(--fa-bounce-jump-scale-y,1.1)) translateY(var(--fa-bounce-height,-.5em))}50%{-webkit-transform:scale(var(--fa-bounce-land-scale-x,1.05),var(--fa-bounce-land-scale-y,.95)) translateY(0);transform:scale(var(--fa-bounce-land-scale-x,1.05),var(--fa-bounce-land-scale-y,.95)) translateY(0)}57%{-webkit-transform:scale(1) translateY(var(--fa-bounce-rebound,-.125em));transform:scale(1) translateY(var(--fa-bounce-rebound,-.125em))}64%{-webkit-transform:scale(1) translateY(0);transform:scale(1) translateY(0)}to{-webkit-transform:scale(1) translateY(0);transform:scale(1) translateY(0)}}@keyframes fa-bounce{0%{-webkit-transform:scale(1) translateY(0);transform:scale(1) translateY(0)}10%{-webkit-transform:scale(var(--fa-bounce-start-scale-x,1.1),var(--fa-bounce-start-scale-y,.9)) translateY(0);transform:scale(var(--fa-bounce-start-scale-x,1.1),var(--fa-bounce-start-scale-y,.9)) translateY(0)}30%{-webkit-transform:scale(var(--fa-bounce-jump-scale-x,.9),var(--fa-bounce-jump-scale-y,1.1)) translateY(var(--fa-bounce-height,-.5em));transform:scale(var(--fa-bounce-jump-scale-x,.9),var(--fa-bounce-jump-scale-y,1.1)) translateY(var(--fa-bounce-height,-.5em))}50%{-webkit-transform:scale(var(--fa-bounce-land-scale-x,1.05),var(--fa-bounce-land-scale-y,.95)) translateY(0);transform:scale(var(--fa-bounce-land-scale-x,1.05),var(--fa-bounce-land-scale-y,.95)) translateY(0)}57%{-webkit-transform:scale(1) translateY(var(--fa-bounce-rebound,-.125em));transform:scale(1) translateY(var(--fa-bounce-rebound,-.125em))}64%{-webkit-transform:scale(1) translateY(0);transform:scale(1) translateY(0)}to{-webkit-transform:scale(1) translateY(0);transform:scale(1) translateY(0)}}@-webkit-keyframes fa-fade{50%{opacity:var(--fa-fade-opacity,.4)}}@keyframes fa-fade{50%{opacity:var(--fa-fade-opacity,.4)}}@-webkit-keyframes fa-beat-fade{0%,to{opacity:var(--fa-beat-fade-opacity,.4);-webkit-transform:scale(1);transform:scale(1)}50%{opacity:1;-webkit-transform:scale(var(--fa-beat-fade-scale,1.125));transform:scale(var(--fa-beat-fade-scale,1.125))}}@keyframes fa-beat-fade{0%,to{opacity:var(--fa-beat-fade-opacity,.4);-webkit-transform:scale(1);transform:scale(1)}50%{opacity:1;-webkit-transform:scale(var(--fa-beat-fade-scale,1.125));transform:scale(var(--fa-beat-fade-scale,1.125))}}@-webkit-keyframes fa-flip{50%{-webkit-transform:rotate3d(var(--fa-flip-x,0),var(--fa-flip-y,1),var(--fa-flip-z,0),var(--fa-flip-angle,-180deg));transform:rotate3d(var(--fa-flip-x,0),var(--fa-flip-y,1),var(--fa-flip-z,0),var(--fa-flip-angle,-180deg))}}@keyframes fa-flip{50%{-webkit-transform:rotate3d(var(--fa-flip-x,0),var(--fa-flip-y,1),var(--fa-flip-z,0),var(--fa-flip-angle,-180deg));transform:rotate3d(var(--fa-flip-x,0),var(--fa-flip-y,1),var(--fa-flip-z,0),var(--fa-flip-angle,-180deg))}}@-webkit-keyframes fa-shake{0%{-webkit-transform:rotate(-15deg);transform:rotate(-15deg)}4%{-webkit-transform:rotate(15deg);transform:rotate(15deg)}8%,24%{-webkit-transform:rotate(-18deg);transform:rotate(-18deg)}12%,28%{-webkit-transform:rotate(18deg);transform:rotate(18deg)}16%{-webkit-transform:rotate(-22deg);transform:rotate(-22deg)}20%{-webkit-transform:rotate(22deg);transform:rotate(22deg)}32%{-webkit-transform:rotate(-12deg);transform:rotate(-12deg)}36%{-webkit-transform:rotate(12deg);transform:rotate(12deg)}40%,to{-webkit-transform:rotate(0deg);transform:rotate(0deg)}}@keyframes fa-shake{0%{-webkit-transform:rotate(-15deg);transform:rotate(-15deg)}4%{-webkit-transform:rotate(15deg);transform:rotate(15deg)}8%,24%{-webkit-transform:rotate(-18deg);transform:rotate(-18deg)}12%,28%{-webkit-transform:rotate(18deg);transform:rotate(18deg)}16%{-webkit-transform:rotate(-22deg);transform:rotate(-22deg)}20%{-webkit-transform:rotate(22deg);transform:rotate(22deg)}32%{-webkit-transform:rotate(-12deg);transform:rotate(-12deg)}36%{-webkit-transform:rotate(12deg);transform:rotate(12deg)}40%,to{-webkit-transform:rotate(0deg);transform:rotate(0deg)}}@-webkit-keyframes fa-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}}@keyframes fa-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}}.fa-rotate-90{-webkit-transform:rotate(90deg);transform:rotate(90deg)}.fa-rotate-180{-webkit-transform:rotate(180deg);transform:rotate(180deg)}.fa-rotate-270{-webkit-transform:rotate(270deg);transform:rotate(270deg)}.fa-flip-horizontal{-webkit-transform:scaleX(-1);transform:scaleX(-1)}.fa-flip-vertical{-webkit-transform:scaleY(-1);transform:scaleY(-1)}.fa-flip-both,.fa-flip-horizontal.fa-flip-vertical{-webkit-transform:scale(-1);transform:scale(-1)}.fa-rotate-by{-webkit-transform:rotate(var(--fa-rotate-angle,none));transform:rotate(var(--fa-rotate-angle,none))}.fa-stack{display:inline-block;height:2em;line-height:2em;position:relative;vertical-align:middle;width:2.5em}.fa-stack-1x,.fa-stack-2x{left:0;position:absolute;text-align:center;width:100%;z-index:var(--fa-stack-z-index,auto)}.fa-stack-1x{line-height:inherit}.fa-stack-2x{font-size:2em}.fa-inverse{color:var(--fa-inverse,#fff)}.fa-0:before{content:"\30"}.fa-1:before{content:"\31"}.fa-2:before{content:"\32"}.fa-3:before{content:"\33"}.fa-4:before{content:"\34"}.fa-5:before{content:"\35"}.fa-6:before{content:"\36"}.fa-7:before{content:"\37"}.fa-8:before{content:"\38"}.fa-9:before{content:"\39"}.fa-fill-drip:before{content:"\f576"}.fa-arrows-to-circle:before{content:"\e4bd"}.fa-chevron-circle-right:before,.fa-circle-chevron-right:before{content:"\f138"}.fa-at:before{content:"\40"}.fa-trash-alt:before,.fa-trash-can:before{content:"\f2ed"}.fa-text-height:before{content:"\f034"}.fa-user-times:before,.fa-user-xmark:before{content:"\f235"}.fa-stethoscope:before{content:"\f0f1"}.fa-comment-alt:before,.fa-message:before{content:"\f27a"}.fa-info:before{content:"\f129"}.fa-compress-alt:before,.fa-down-left-and-up-right-to-center:before{content:"\f422"}.fa-explosion:before{content:"\e4e9"}.fa-file-alt:before,.fa-file-lines:before,.fa-file-text:before{content:"\f15c"}.fa-wave-square:before{content:"\f83e"}.fa-ring:before{content:"\f70b"}.fa-building-un:before{content:"\e4d9"}.fa-dice-three:before{content:"\f527"}.fa-calendar-alt:before,.fa-calendar-days:before{content:"\f073"}.fa-anchor-circle-check:before{content:"\e4aa"}.fa-building-circle-arrow-right:before{content:"\e4d1"}.fa-volleyball-ball:before,.fa-volleyball:before{content:"\f45f"}.fa-arrows-up-to-line:before{content:"\e4c2"}.fa-sort-desc:before,.fa-sort-down:before{content:"\f0dd"}.fa-circle-minus:before,.fa-minus-circle:before{content:"\f056"}.fa-door-open:before{content:"\f52b"}.fa-right-from-bracket:before,.fa-sign-out-alt:before{content:"\f2f5"}.fa-atom:before{content:"\f5d2"}.fa-soap:before{content:"\e06e"}.fa-heart-music-camera-bolt:before,.fa-icons:before{content:"\f86d"}.fa-microphone-alt-slash:before,.fa-microphone-lines-slash:before{content:"\f539"}.fa-bridge-circle-check:before{content:"\e4c9"}.fa-pump-medical:before{content:"\e06a"}.fa-fingerprint:before{content:"\f577"}.fa-hand-point-right:before{content:"\f0a4"}.fa-magnifying-glass-location:before,.fa-search-location:before{content:"\f689"}.fa-forward-step:before,.fa-step-forward:before{content:"\f051"}.fa-face-smile-beam:before,.fa-smile-beam:before{content:"\f5b8"}.fa-flag-checkered:before{content:"\f11e"}.fa-football-ball:before,.fa-football:before{content:"\f44e"}.fa-school-circle-exclamation:before{content:"\e56c"}.fa-crop:before{content:"\f125"}.fa-angle-double-down:before,.fa-angles-down:before{content:"\f103"}.fa-users-rectangle:before{content:"\e594"}.fa-people-roof:before{content:"\e537"}.fa-people-line:before{content:"\e534"}.fa-beer-mug-empty:before,.fa-beer:before{content:"\f0fc"}.fa-diagram-predecessor:before{content:"\e477"}.fa-arrow-up-long:before,.fa-long-arrow-up:before{content:"\f176"}.fa-burn:before,.fa-fire-flame-simple:before{content:"\f46a"}.fa-male:before,.fa-person:before{content:"\f183"}.fa-laptop:before{content:"\f109"}.fa-file-csv:before{content:"\f6dd"}.fa-menorah:before{content:"\f676"}.fa-truck-plane:before{content:"\e58f"}.fa-record-vinyl:before{content:"\f8d9"}.fa-face-grin-stars:before,.fa-grin-stars:before{content:"\f587"}.fa-bong:before{content:"\f55c"}.fa-pastafarianism:before,.fa-spaghetti-monster-flying:before{content:"\f67b"}.fa-arrow-down-up-across-line:before{content:"\e4af"}.fa-spoon:before,.fa-utensil-spoon:before{content:"\f2e5"}.fa-jar-wheat:before{content:"\e517"}.fa-envelopes-bulk:before,.fa-mail-bulk:before{content:"\f674"}.fa-file-circle-exclamation:before{content:"\e4eb"}.fa-circle-h:before,.fa-hospital-symbol:before{content:"\f47e"}.fa-pager:before{content:"\f815"}.fa-address-book:before,.fa-contact-book:before{content:"\f2b9"}.fa-strikethrough:before{content:"\f0cc"}.fa-k:before{content:"\4b"}.fa-landmark-flag:before{content:"\e51c"}.fa-pencil-alt:before,.fa-pencil:before{content:"\f303"}.fa-backward:before{content:"\f04a"}.fa-caret-right:before{content:"\f0da"}.fa-comments:before{content:"\f086"}.fa-file-clipboard:before,.fa-paste:before{content:"\f0ea"}.fa-code-pull-request:before{content:"\e13c"}.fa-clipboard-list:before{content:"\f46d"}.fa-truck-loading:before,.fa-truck-ramp-box:before{content:"\f4de"}.fa-user-check:before{content:"\f4fc"}.fa-vial-virus:before{content:"\e597"}.fa-sheet-plastic:before{content:"\e571"}.fa-blog:before{content:"\f781"}.fa-user-ninja:before{content:"\f504"}.fa-person-arrow-up-from-line:before{content:"\e539"}.fa-scroll-torah:before,.fa-torah:before{content:"\f6a0"}.fa-broom-ball:before,.fa-quidditch-broom-ball:before,.fa-quidditch:before{content:"\f458"}.fa-toggle-off:before{content:"\f204"}.fa-archive:before,.fa-box-archive:before{content:"\f187"}.fa-person-drowning:before{content:"\e545"}.fa-arrow-down-9-1:before,.fa-sort-numeric-desc:before,.fa-sort-numeric-down-alt:before{content:"\f886"}.fa-face-grin-tongue-squint:before,.fa-grin-tongue-squint:before{content:"\f58a"}.fa-spray-can:before{content:"\f5bd"}.fa-truck-monster:before{content:"\f63b"}.fa-w:before{content:"\57"}.fa-earth-africa:before,.fa-globe-africa:before{content:"\f57c"}.fa-rainbow:before{content:"\f75b"}.fa-circle-notch:before{content:"\f1ce"}.fa-tablet-alt:before,.fa-tablet-screen-button:before{content:"\f3fa"}.fa-paw:before{content:"\f1b0"}.fa-cloud:before{content:"\f0c2"}.fa-trowel-bricks:before{content:"\e58a"}.fa-face-flushed:before,.fa-flushed:before{content:"\f579"}.fa-hospital-user:before{content:"\f80d"}.fa-tent-arrow-left-right:before{content:"\e57f"}.fa-gavel:before,.fa-legal:before{content:"\f0e3"}.fa-binoculars:before{content:"\f1e5"}.fa-microphone-slash:before{content:"\f131"}.fa-box-tissue:before{content:"\e05b"}.fa-motorcycle:before{content:"\f21c"}.fa-bell-concierge:before,.fa-concierge-bell:before{content:"\f562"}.fa-pen-ruler:before,.fa-pencil-ruler:before{content:"\f5ae"}.fa-people-arrows-left-right:before,.fa-people-arrows:before{content:"\e068"}.fa-mars-and-venus-burst:before{content:"\e523"}.fa-caret-square-right:before,.fa-square-caret-right:before{content:"\f152"}.fa-cut:before,.fa-scissors:before{content:"\f0c4"}.fa-sun-plant-wilt:before{content:"\e57a"}.fa-toilets-portable:before{content:"\e584"}.fa-hockey-puck:before{content:"\f453"}.fa-table:before{content:"\f0ce"}.fa-magnifying-glass-arrow-right:before{content:"\e521"}.fa-digital-tachograph:before,.fa-tachograph-digital:before{content:"\f566"}.fa-users-slash:before{content:"\e073"}.fa-clover:before{content:"\e139"}.fa-mail-reply:before,.fa-reply:before{content:"\f3e5"}.fa-star-and-crescent:before{content:"\f699"}.fa-house-fire:before{content:"\e50c"}.fa-minus-square:before,.fa-square-minus:before{content:"\f146"}.fa-helicopter:before{content:"\f533"}.fa-compass:before{content:"\f14e"}.fa-caret-square-down:before,.fa-square-caret-down:before{content:"\f150"}.fa-file-circle-question:before{content:"\e4ef"}.fa-laptop-code:before{content:"\f5fc"}.fa-swatchbook:before{content:"\f5c3"}.fa-prescription-bottle:before{content:"\f485"}.fa-bars:before,.fa-navicon:before{content:"\f0c9"}.fa-people-group:before{content:"\e533"}.fa-hourglass-3:before,.fa-hourglass-end:before{content:"\f253"}.fa-heart-broken:before,.fa-heart-crack:before{content:"\f7a9"}.fa-external-link-square-alt:before,.fa-square-up-right:before{content:"\f360"}.fa-face-kiss-beam:before,.fa-kiss-beam:before{content:"\f597"}.fa-film:before{content:"\f008"}.fa-ruler-horizontal:before{content:"\f547"}.fa-people-robbery:before{content:"\e536"}.fa-lightbulb:before{content:"\f0eb"}.fa-caret-left:before{content:"\f0d9"}.fa-circle-exclamation:before,.fa-exclamation-circle:before{content:"\f06a"}.fa-school-circle-xmark:before{content:"\e56d"}.fa-arrow-right-from-bracket:before,.fa-sign-out:before{content:"\f08b"}.fa-chevron-circle-down:before,.fa-circle-chevron-down:before{content:"\f13a"}.fa-unlock-alt:before,.fa-unlock-keyhole:before{content:"\f13e"}.fa-cloud-showers-heavy:before{content:"\f740"}.fa-headphones-alt:before,.fa-headphones-simple:before{content:"\f58f"}.fa-sitemap:before{content:"\f0e8"}.fa-circle-dollar-to-slot:before,.fa-donate:before{content:"\f4b9"}.fa-memory:before{content:"\f538"}.fa-road-spikes:before{content:"\e568"}.fa-fire-burner:before{content:"\e4f1"}.fa-flag:before{content:"\f024"}.fa-hanukiah:before{content:"\f6e6"}.fa-feather:before{content:"\f52d"}.fa-volume-down:before,.fa-volume-low:before{content:"\f027"}.fa-comment-slash:before{content:"\f4b3"}.fa-cloud-sun-rain:before{content:"\f743"}.fa-compress:before{content:"\f066"}.fa-wheat-alt:before,.fa-wheat-awn:before{content:"\e2cd"}.fa-ankh:before{content:"\f644"}.fa-hands-holding-child:before{content:"\e4fa"}.fa-asterisk:before{content:"\2a"}.fa-check-square:before,.fa-square-check:before{content:"\f14a"}.fa-peseta-sign:before{content:"\e221"}.fa-header:before,.fa-heading:before{content:"\f1dc"}.fa-ghost:before{content:"\f6e2"}.fa-list-squares:before,.fa-list:before{content:"\f03a"}.fa-phone-square-alt:before,.fa-square-phone-flip:before{content:"\f87b"}.fa-cart-plus:before{content:"\f217"}.fa-gamepad:before{content:"\f11b"}.fa-circle-dot:before,.fa-dot-circle:before{content:"\f192"}.fa-dizzy:before,.fa-face-dizzy:before{content:"\f567"}.fa-egg:before{content:"\f7fb"}.fa-house-medical-circle-xmark:before{content:"\e513"}.fa-campground:before{content:"\f6bb"}.fa-folder-plus:before{content:"\f65e"}.fa-futbol-ball:before,.fa-futbol:before,.fa-soccer-ball:before{content:"\f1e3"}.fa-paint-brush:before,.fa-paintbrush:before{content:"\f1fc"}.fa-lock:before{content:"\f023"}.fa-gas-pump:before{content:"\f52f"}.fa-hot-tub-person:before,.fa-hot-tub:before{content:"\f593"}.fa-map-location:before,.fa-map-marked:before{content:"\f59f"}.fa-house-flood-water:before{content:"\e50e"}.fa-tree:before{content:"\f1bb"}.fa-bridge-lock:before{content:"\e4cc"}.fa-sack-dollar:before{content:"\f81d"}.fa-edit:before,.fa-pen-to-square:before{content:"\f044"}.fa-car-side:before{content:"\f5e4"}.fa-share-alt:before,.fa-share-nodes:before{content:"\f1e0"}.fa-heart-circle-minus:before{content:"\e4ff"}.fa-hourglass-2:before,.fa-hourglass-half:before{content:"\f252"}.fa-microscope:before{content:"\f610"}.fa-sink:before{content:"\e06d"}.fa-bag-shopping:before,.fa-shopping-bag:before{content:"\f290"}.fa-arrow-down-z-a:before,.fa-sort-alpha-desc:before,.fa-sort-alpha-down-alt:before{content:"\f881"}.fa-mitten:before{content:"\f7b5"}.fa-person-rays:before{content:"\e54d"}.fa-users:before{content:"\f0c0"}.fa-eye-slash:before{content:"\f070"}.fa-flask-vial:before{content:"\e4f3"}.fa-hand-paper:before,.fa-hand:before{content:"\f256"}.fa-om:before{content:"\f679"}.fa-worm:before{content:"\e599"}.fa-house-circle-xmark:before{content:"\e50b"}.fa-plug:before{content:"\f1e6"}.fa-chevron-up:before{content:"\f077"}.fa-hand-spock:before{content:"\f259"}.fa-stopwatch:before{content:"\f2f2"}.fa-face-kiss:before,.fa-kiss:before{content:"\f596"}.fa-bridge-circle-xmark:before{content:"\e4cb"}.fa-face-grin-tongue:before,.fa-grin-tongue:before{content:"\f589"}.fa-chess-bishop:before{content:"\f43a"}.fa-face-grin-wink:before,.fa-grin-wink:before{content:"\f58c"}.fa-deaf:before,.fa-deafness:before,.fa-ear-deaf:before,.fa-hard-of-hearing:before{content:"\f2a4"}.fa-road-circle-check:before{content:"\e564"}.fa-dice-five:before{content:"\f523"}.fa-rss-square:before,.fa-square-rss:before{content:"\f143"}.fa-land-mine-on:before{content:"\e51b"}.fa-i-cursor:before{content:"\f246"}.fa-stamp:before{content:"\f5bf"}.fa-stairs:before{content:"\e289"}.fa-i:before{content:"\49"}.fa-hryvnia-sign:before,.fa-hryvnia:before{content:"\f6f2"}.fa-pills:before{content:"\f484"}.fa-face-grin-wide:before,.fa-grin-alt:before{content:"\f581"}.fa-tooth:before{content:"\f5c9"}.fa-v:before{content:"\56"}.fa-bangladeshi-taka-sign:before{content:"\e2e6"}.fa-bicycle:before{content:"\f206"}.fa-rod-asclepius:before,.fa-rod-snake:before,.fa-staff-aesculapius:before,.fa-staff-snake:before{content:"\e579"}.fa-head-side-cough-slash:before{content:"\e062"}.fa-ambulance:before,.fa-truck-medical:before{content:"\f0f9"}.fa-wheat-awn-circle-exclamation:before{content:"\e598"}.fa-snowman:before{content:"\f7d0"}.fa-mortar-pestle:before{content:"\f5a7"}.fa-road-barrier:before{content:"\e562"}.fa-school:before{content:"\f549"}.fa-igloo:before{content:"\f7ae"}.fa-joint:before{content:"\f595"}.fa-angle-right:before{content:"\f105"}.fa-horse:before{content:"\f6f0"}.fa-q:before{content:"\51"}.fa-g:before{content:"\47"}.fa-notes-medical:before{content:"\f481"}.fa-temperature-2:before,.fa-temperature-half:before,.fa-thermometer-2:before,.fa-thermometer-half:before{content:"\f2c9"}.fa-dong-sign:before{content:"\e169"}.fa-capsules:before{content:"\f46b"}.fa-poo-bolt:before,.fa-poo-storm:before{content:"\f75a"}.fa-face-frown-open:before,.fa-frown-open:before{content:"\f57a"}.fa-hand-point-up:before{content:"\f0a6"}.fa-money-bill:before{content:"\f0d6"}.fa-bookmark:before{content:"\f02e"}.fa-align-justify:before{content:"\f039"}.fa-umbrella-beach:before{content:"\f5ca"}.fa-helmet-un:before{content:"\e503"}.fa-bullseye:before{content:"\f140"}.fa-bacon:before{content:"\f7e5"}.fa-hand-point-down:before{content:"\f0a7"}.fa-arrow-up-from-bracket:before{content:"\e09a"}.fa-folder-blank:before,.fa-folder:before{content:"\f07b"}.fa-file-medical-alt:before,.fa-file-waveform:before{content:"\f478"}.fa-radiation:before{content:"\f7b9"}.fa-chart-simple:before{content:"\e473"}.fa-mars-stroke:before{content:"\f229"}.fa-vial:before{content:"\f492"}.fa-dashboard:before,.fa-gauge-med:before,.fa-gauge:before,.fa-tachometer-alt-average:before{content:"\f624"}.fa-magic-wand-sparkles:before,.fa-wand-magic-sparkles:before{content:"\e2ca"}.fa-e:before{content:"\45"}.fa-pen-alt:before,.fa-pen-clip:before{content:"\f305"}.fa-bridge-circle-exclamation:before{content:"\e4ca"}.fa-user:before{content:"\f007"}.fa-school-circle-check:before{content:"\e56b"}.fa-dumpster:before{content:"\f793"}.fa-shuttle-van:before,.fa-van-shuttle:before{content:"\f5b6"}.fa-building-user:before{content:"\e4da"}.fa-caret-square-left:before,.fa-square-caret-left:before{content:"\f191"}.fa-highlighter:before{content:"\f591"}.fa-key:before{content:"\f084"}.fa-bullhorn:before{content:"\f0a1"}.fa-globe:before{content:"\f0ac"}.fa-synagogue:before{content:"\f69b"}.fa-person-half-dress:before{content:"\e548"}.fa-road-bridge:before{content:"\e563"}.fa-location-arrow:before{content:"\f124"}.fa-c:before{content:"\43"}.fa-tablet-button:before{content:"\f10a"}.fa-building-lock:before{content:"\e4d6"}.fa-pizza-slice:before{content:"\f818"}.fa-money-bill-wave:before{content:"\f53a"}.fa-area-chart:before,.fa-chart-area:before{content:"\f1fe"}.fa-house-flag:before{content:"\e50d"}.fa-person-circle-minus:before{content:"\e540"}.fa-ban:before,.fa-cancel:before{content:"\f05e"}.fa-camera-rotate:before{content:"\e0d8"}.fa-air-freshener:before,.fa-spray-can-sparkles:before{content:"\f5d0"}.fa-star:before{content:"\f005"}.fa-repeat:before{content:"\f363"}.fa-cross:before{content:"\f654"}.fa-box:before{content:"\f466"}.fa-venus-mars:before{content:"\f228"}.fa-arrow-pointer:before,.fa-mouse-pointer:before{content:"\f245"}.fa-expand-arrows-alt:before,.fa-maximize:before{content:"\f31e"}.fa-charging-station:before{content:"\f5e7"}.fa-shapes:before,.fa-triangle-circle-square:before{content:"\f61f"}.fa-random:before,.fa-shuffle:before{content:"\f074"}.fa-person-running:before,.fa-running:before{content:"\f70c"}.fa-mobile-retro:before{content:"\e527"}.fa-grip-lines-vertical:before{content:"\f7a5"}.fa-spider:before{content:"\f717"}.fa-hands-bound:before{content:"\e4f9"}.fa-file-invoice-dollar:before{content:"\f571"}.fa-plane-circle-exclamation:before{content:"\e556"}.fa-x-ray:before{content:"\f497"}.fa-spell-check:before{content:"\f891"}.fa-slash:before{content:"\f715"}.fa-computer-mouse:before,.fa-mouse:before{content:"\f8cc"}.fa-arrow-right-to-bracket:before,.fa-sign-in:before{content:"\f090"}.fa-shop-slash:before,.fa-store-alt-slash:before{content:"\e070"}.fa-server:before{content:"\f233"}.fa-virus-covid-slash:before{content:"\e4a9"}.fa-shop-lock:before{content:"\e4a5"}.fa-hourglass-1:before,.fa-hourglass-start:before{content:"\f251"}.fa-blender-phone:before{content:"\f6b6"}.fa-building-wheat:before{content:"\e4db"}.fa-person-breastfeeding:before{content:"\e53a"}.fa-right-to-bracket:before,.fa-sign-in-alt:before{content:"\f2f6"}.fa-venus:before{content:"\f221"}.fa-passport:before{content:"\f5ab"}.fa-heart-pulse:before,.fa-heartbeat:before{content:"\f21e"}.fa-people-carry-box:before,.fa-people-carry:before{content:"\f4ce"}.fa-temperature-high:before{content:"\f769"}.fa-microchip:before{content:"\f2db"}.fa-crown:before{content:"\f521"}.fa-weight-hanging:before{content:"\f5cd"}.fa-xmarks-lines:before{content:"\e59a"}.fa-file-prescription:before{content:"\f572"}.fa-weight-scale:before,.fa-weight:before{content:"\f496"}.fa-user-friends:before,.fa-user-group:before{content:"\f500"}.fa-arrow-up-a-z:before,.fa-sort-alpha-up:before{content:"\f15e"}.fa-chess-knight:before{content:"\f441"}.fa-face-laugh-squint:before,.fa-laugh-squint:before{content:"\f59b"}.fa-wheelchair:before{content:"\f193"}.fa-arrow-circle-up:before,.fa-circle-arrow-up:before{content:"\f0aa"}.fa-toggle-on:before{content:"\f205"}.fa-person-walking:before,.fa-walking:before{content:"\f554"}.fa-l:before{content:"\4c"}.fa-fire:before{content:"\f06d"}.fa-bed-pulse:before,.fa-procedures:before{content:"\f487"}.fa-shuttle-space:before,.fa-space-shuttle:before{content:"\f197"}.fa-face-laugh:before,.fa-laugh:before{content:"\f599"}.fa-folder-open:before{content:"\f07c"}.fa-heart-circle-plus:before{content:"\e500"}.fa-code-fork:before{content:"\e13b"}.fa-city:before{content:"\f64f"}.fa-microphone-alt:before,.fa-microphone-lines:before{content:"\f3c9"}.fa-pepper-hot:before{content:"\f816"}.fa-unlock:before{content:"\f09c"}.fa-colon-sign:before{content:"\e140"}.fa-headset:before{content:"\f590"}.fa-store-slash:before{content:"\e071"}.fa-road-circle-xmark:before{content:"\e566"}.fa-user-minus:before{content:"\f503"}.fa-mars-stroke-up:before,.fa-mars-stroke-v:before{content:"\f22a"}.fa-champagne-glasses:before,.fa-glass-cheers:before{content:"\f79f"}.fa-clipboard:before{content:"\f328"}.fa-house-circle-exclamation:before{content:"\e50a"}.fa-file-arrow-up:before,.fa-file-upload:before{content:"\f574"}.fa-wifi-3:before,.fa-wifi-strong:before,.fa-wifi:before{content:"\f1eb"}.fa-bath:before,.fa-bathtub:before{content:"\f2cd"}.fa-underline:before{content:"\f0cd"}.fa-user-edit:before,.fa-user-pen:before{content:"\f4ff"}.fa-signature:before{content:"\f5b7"}.fa-stroopwafel:before{content:"\f551"}.fa-bold:before{content:"\f032"}.fa-anchor-lock:before{content:"\e4ad"}.fa-building-ngo:before{content:"\e4d7"}.fa-manat-sign:before{content:"\e1d5"}.fa-not-equal:before{content:"\f53e"}.fa-border-style:before,.fa-border-top-left:before{content:"\f853"}.fa-map-location-dot:before,.fa-map-marked-alt:before{content:"\f5a0"}.fa-jedi:before{content:"\f669"}.fa-poll:before,.fa-square-poll-vertical:before{content:"\f681"}.fa-mug-hot:before{content:"\f7b6"}.fa-battery-car:before,.fa-car-battery:before{content:"\f5df"}.fa-gift:before{content:"\f06b"}.fa-dice-two:before{content:"\f528"}.fa-chess-queen:before{content:"\f445"}.fa-glasses:before{content:"\f530"}.fa-chess-board:before{content:"\f43c"}.fa-building-circle-check:before{content:"\e4d2"}.fa-person-chalkboard:before{content:"\e53d"}.fa-mars-stroke-h:before,.fa-mars-stroke-right:before{content:"\f22b"}.fa-hand-back-fist:before,.fa-hand-rock:before{content:"\f255"}.fa-caret-square-up:before,.fa-square-caret-up:before{content:"\f151"}.fa-cloud-showers-water:before{content:"\e4e4"}.fa-bar-chart:before,.fa-chart-bar:before{content:"\f080"}.fa-hands-bubbles:before,.fa-hands-wash:before{content:"\e05e"}.fa-less-than-equal:before{content:"\f537"}.fa-train:before{content:"\f238"}.fa-eye-low-vision:before,.fa-low-vision:before{content:"\f2a8"}.fa-crow:before{content:"\f520"}.fa-sailboat:before{content:"\e445"}.fa-window-restore:before{content:"\f2d2"}.fa-plus-square:before,.fa-square-plus:before{content:"\f0fe"}.fa-torii-gate:before{content:"\f6a1"}.fa-frog:before{content:"\f52e"}.fa-bucket:before{content:"\e4cf"}.fa-image:before{content:"\f03e"}.fa-microphone:before{content:"\f130"}.fa-cow:before{content:"\f6c8"}.fa-caret-up:before{content:"\f0d8"}.fa-screwdriver:before{content:"\f54a"}.fa-folder-closed:before{content:"\e185"}.fa-house-tsunami:before{content:"\e515"}.fa-square-nfi:before{content:"\e576"}.fa-arrow-up-from-ground-water:before{content:"\e4b5"}.fa-glass-martini-alt:before,.fa-martini-glass:before{content:"\f57b"}.fa-rotate-back:before,.fa-rotate-backward:before,.fa-rotate-left:before,.fa-undo-alt:before{content:"\f2ea"}.fa-columns:before,.fa-table-columns:before{content:"\f0db"}.fa-lemon:before{content:"\f094"}.fa-head-side-mask:before{content:"\e063"}.fa-handshake:before{content:"\f2b5"}.fa-gem:before{content:"\f3a5"}.fa-dolly-box:before,.fa-dolly:before{content:"\f472"}.fa-smoking:before{content:"\f48d"}.fa-compress-arrows-alt:before,.fa-minimize:before{content:"\f78c"}.fa-monument:before{content:"\f5a6"}.fa-snowplow:before{content:"\f7d2"}.fa-angle-double-right:before,.fa-angles-right:before{content:"\f101"}.fa-cannabis:before{content:"\f55f"}.fa-circle-play:before,.fa-play-circle:before{content:"\f144"}.fa-tablets:before{content:"\f490"}.fa-ethernet:before{content:"\f796"}.fa-eur:before,.fa-euro-sign:before,.fa-euro:before{content:"\f153"}.fa-chair:before{content:"\f6c0"}.fa-check-circle:before,.fa-circle-check:before{content:"\f058"}.fa-circle-stop:before,.fa-stop-circle:before{content:"\f28d"}.fa-compass-drafting:before,.fa-drafting-compass:before{content:"\f568"}.fa-plate-wheat:before{content:"\e55a"}.fa-icicles:before{content:"\f7ad"}.fa-person-shelter:before{content:"\e54f"}.fa-neuter:before{content:"\f22c"}.fa-id-badge:before{content:"\f2c1"}.fa-marker:before{content:"\f5a1"}.fa-face-laugh-beam:before,.fa-laugh-beam:before{content:"\f59a"}.fa-helicopter-symbol:before{content:"\e502"}.fa-universal-access:before{content:"\f29a"}.fa-chevron-circle-up:before,.fa-circle-chevron-up:before{content:"\f139"}.fa-lari-sign:before{content:"\e1c8"}.fa-volcano:before{content:"\f770"}.fa-person-walking-dashed-line-arrow-right:before{content:"\e553"}.fa-gbp:before,.fa-pound-sign:before,.fa-sterling-sign:before{content:"\f154"}.fa-viruses:before{content:"\e076"}.fa-square-person-confined:before{content:"\e577"}.fa-user-tie:before{content:"\f508"}.fa-arrow-down-long:before,.fa-long-arrow-down:before{content:"\f175"}.fa-tent-arrow-down-to-line:before{content:"\e57e"}.fa-certificate:before{content:"\f0a3"}.fa-mail-reply-all:before,.fa-reply-all:before{content:"\f122"}.fa-suitcase:before{content:"\f0f2"}.fa-person-skating:before,.fa-skating:before{content:"\f7c5"}.fa-filter-circle-dollar:before,.fa-funnel-dollar:before{content:"\f662"}.fa-camera-retro:before{content:"\f083"}.fa-arrow-circle-down:before,.fa-circle-arrow-down:before{content:"\f0ab"}.fa-arrow-right-to-file:before,.fa-file-import:before{content:"\f56f"}.fa-external-link-square:before,.fa-square-arrow-up-right:before{content:"\f14c"}.fa-box-open:before{content:"\f49e"}.fa-scroll:before{content:"\f70e"}.fa-spa:before{content:"\f5bb"}.fa-location-pin-lock:before{content:"\e51f"}.fa-pause:before{content:"\f04c"}.fa-hill-avalanche:before{content:"\e507"}.fa-temperature-0:before,.fa-temperature-empty:before,.fa-thermometer-0:before,.fa-thermometer-empty:before{content:"\f2cb"}.fa-bomb:before{content:"\f1e2"}.fa-registered:before{content:"\f25d"}.fa-address-card:before,.fa-contact-card:before,.fa-vcard:before{content:"\f2bb"}.fa-balance-scale-right:before,.fa-scale-unbalanced-flip:before{content:"\f516"}.fa-subscript:before{content:"\f12c"}.fa-diamond-turn-right:before,.fa-directions:before{content:"\f5eb"}.fa-burst:before{content:"\e4dc"}.fa-house-laptop:before,.fa-laptop-house:before{content:"\e066"}.fa-face-tired:before,.fa-tired:before{content:"\f5c8"}.fa-money-bills:before{content:"\e1f3"}.fa-smog:before{content:"\f75f"}.fa-crutch:before{content:"\f7f7"}.fa-cloud-arrow-up:before,.fa-cloud-upload-alt:before,.fa-cloud-upload:before{content:"\f0ee"}.fa-palette:before{content:"\f53f"}.fa-arrows-turn-right:before{content:"\e4c0"}.fa-vest:before{content:"\e085"}.fa-ferry:before{content:"\e4ea"}.fa-arrows-down-to-people:before{content:"\e4b9"}.fa-seedling:before,.fa-sprout:before{content:"\f4d8"}.fa-arrows-alt-h:before,.fa-left-right:before{content:"\f337"}.fa-boxes-packing:before{content:"\e4c7"}.fa-arrow-circle-left:before,.fa-circle-arrow-left:before{content:"\f0a8"}.fa-group-arrows-rotate:before{content:"\e4f6"}.fa-bowl-food:before{content:"\e4c6"}.fa-candy-cane:before{content:"\f786"}.fa-arrow-down-wide-short:before,.fa-sort-amount-asc:before,.fa-sort-amount-down:before{content:"\f160"}.fa-cloud-bolt:before,.fa-thunderstorm:before{content:"\f76c"}.fa-remove-format:before,.fa-text-slash:before{content:"\f87d"}.fa-face-smile-wink:before,.fa-smile-wink:before{content:"\f4da"}.fa-file-word:before{content:"\f1c2"}.fa-file-powerpoint:before{content:"\f1c4"}.fa-arrows-h:before,.fa-arrows-left-right:before{content:"\f07e"}.fa-house-lock:before{content:"\e510"}.fa-cloud-arrow-down:before,.fa-cloud-download-alt:before,.fa-cloud-download:before{content:"\f0ed"}.fa-children:before{content:"\e4e1"}.fa-blackboard:before,.fa-chalkboard:before{content:"\f51b"}.fa-user-alt-slash:before,.fa-user-large-slash:before{content:"\f4fa"}.fa-envelope-open:before{content:"\f2b6"}.fa-handshake-alt-slash:before,.fa-handshake-simple-slash:before{content:"\e05f"}.fa-mattress-pillow:before{content:"\e525"}.fa-guarani-sign:before{content:"\e19a"}.fa-arrows-rotate:before,.fa-refresh:before,.fa-sync:before{content:"\f021"}.fa-fire-extinguisher:before{content:"\f134"}.fa-cruzeiro-sign:before{content:"\e152"}.fa-greater-than-equal:before{content:"\f532"}.fa-shield-alt:before,.fa-shield-halved:before{content:"\f3ed"}.fa-atlas:before,.fa-book-atlas:before{content:"\f558"}.fa-virus:before{content:"\e074"}.fa-envelope-circle-check:before{content:"\e4e8"}.fa-layer-group:before{content:"\f5fd"}.fa-arrows-to-dot:before{content:"\e4be"}.fa-archway:before{content:"\f557"}.fa-heart-circle-check:before{content:"\e4fd"}.fa-house-chimney-crack:before,.fa-house-damage:before{content:"\f6f1"}.fa-file-archive:before,.fa-file-zipper:before{content:"\f1c6"}.fa-square:before{content:"\f0c8"}.fa-glass-martini:before,.fa-martini-glass-empty:before{content:"\f000"}.fa-couch:before{content:"\f4b8"}.fa-cedi-sign:before{content:"\e0df"}.fa-italic:before{content:"\f033"}.fa-church:before{content:"\f51d"}.fa-comments-dollar:before{content:"\f653"}.fa-democrat:before{content:"\f747"}.fa-z:before{content:"\5a"}.fa-person-skiing:before,.fa-skiing:before{content:"\f7c9"}.fa-road-lock:before{content:"\e567"}.fa-a:before{content:"\41"}.fa-temperature-arrow-down:before,.fa-temperature-down:before{content:"\e03f"}.fa-feather-alt:before,.fa-feather-pointed:before{content:"\f56b"}.fa-p:before{content:"\50"}.fa-snowflake:before{content:"\f2dc"}.fa-newspaper:before{content:"\f1ea"}.fa-ad:before,.fa-rectangle-ad:before{content:"\f641"}.fa-arrow-circle-right:before,.fa-circle-arrow-right:before{content:"\f0a9"}.fa-filter-circle-xmark:before{content:"\e17b"}.fa-locust:before{content:"\e520"}.fa-sort:before,.fa-unsorted:before{content:"\f0dc"}.fa-list-1-2:before,.fa-list-numeric:before,.fa-list-ol:before{content:"\f0cb"}.fa-person-dress-burst:before{content:"\e544"}.fa-money-check-alt:before,.fa-money-check-dollar:before{content:"\f53d"}.fa-vector-square:before{content:"\f5cb"}.fa-bread-slice:before{content:"\f7ec"}.fa-language:before{content:"\f1ab"}.fa-face-kiss-wink-heart:before,.fa-kiss-wink-heart:before{content:"\f598"}.fa-filter:before{content:"\f0b0"}.fa-question:before{content:"\3f"}.fa-file-signature:before{content:"\f573"}.fa-arrows-alt:before,.fa-up-down-left-right:before{content:"\f0b2"}.fa-house-chimney-user:before{content:"\e065"}.fa-hand-holding-heart:before{content:"\f4be"}.fa-puzzle-piece:before{content:"\f12e"}.fa-money-check:before{content:"\f53c"}.fa-star-half-alt:before,.fa-star-half-stroke:before{content:"\f5c0"}.fa-code:before{content:"\f121"}.fa-glass-whiskey:before,.fa-whiskey-glass:before{content:"\f7a0"}.fa-building-circle-exclamation:before{content:"\e4d3"}.fa-magnifying-glass-chart:before{content:"\e522"}.fa-arrow-up-right-from-square:before,.fa-external-link:before{content:"\f08e"}.fa-cubes-stacked:before{content:"\e4e6"}.fa-krw:before,.fa-won-sign:before,.fa-won:before{content:"\f159"}.fa-virus-covid:before{content:"\e4a8"}.fa-austral-sign:before{content:"\e0a9"}.fa-f:before{content:"\46"}.fa-leaf:before{content:"\f06c"}.fa-road:before{content:"\f018"}.fa-cab:before,.fa-taxi:before{content:"\f1ba"}.fa-person-circle-plus:before{content:"\e541"}.fa-chart-pie:before,.fa-pie-chart:before{content:"\f200"}.fa-bolt-lightning:before{content:"\e0b7"}.fa-sack-xmark:before{content:"\e56a"}.fa-file-excel:before{content:"\f1c3"}.fa-file-contract:before{content:"\f56c"}.fa-fish-fins:before{content:"\e4f2"}.fa-building-flag:before{content:"\e4d5"}.fa-face-grin-beam:before,.fa-grin-beam:before{content:"\f582"}.fa-object-ungroup:before{content:"\f248"}.fa-poop:before{content:"\f619"}.fa-location-pin:before,.fa-map-marker:before{content:"\f041"}.fa-kaaba:before{content:"\f66b"}.fa-toilet-paper:before{content:"\f71e"}.fa-hard-hat:before,.fa-hat-hard:before,.fa-helmet-safety:before{content:"\f807"}.fa-eject:before{content:"\f052"}.fa-arrow-alt-circle-right:before,.fa-circle-right:before{content:"\f35a"}.fa-plane-circle-check:before{content:"\e555"}.fa-face-rolling-eyes:before,.fa-meh-rolling-eyes:before{content:"\f5a5"}.fa-object-group:before{content:"\f247"}.fa-chart-line:before,.fa-line-chart:before{content:"\f201"}.fa-mask-ventilator:before{content:"\e524"}.fa-arrow-right:before{content:"\f061"}.fa-map-signs:before,.fa-signs-post:before{content:"\f277"}.fa-cash-register:before{content:"\f788"}.fa-person-circle-question:before{content:"\e542"}.fa-h:before{content:"\48"}.fa-tarp:before{content:"\e57b"}.fa-screwdriver-wrench:before,.fa-tools:before{content:"\f7d9"}.fa-arrows-to-eye:before{content:"\e4bf"}.fa-plug-circle-bolt:before{content:"\e55b"}.fa-heart:before{content:"\f004"}.fa-mars-and-venus:before{content:"\f224"}.fa-home-user:before,.fa-house-user:before{content:"\e1b0"}.fa-dumpster-fire:before{content:"\f794"}.fa-house-crack:before{content:"\e3b1"}.fa-cocktail:before,.fa-martini-glass-citrus:before{content:"\f561"}.fa-face-surprise:before,.fa-surprise:before{content:"\f5c2"}.fa-bottle-water:before{content:"\e4c5"}.fa-circle-pause:before,.fa-pause-circle:before{content:"\f28b"}.fa-toilet-paper-slash:before{content:"\e072"}.fa-apple-alt:before,.fa-apple-whole:before{content:"\f5d1"}.fa-kitchen-set:before{content:"\e51a"}.fa-r:before{content:"\52"}.fa-temperature-1:before,.fa-temperature-quarter:before,.fa-thermometer-1:before,.fa-thermometer-quarter:before{content:"\f2ca"}.fa-cube:before{content:"\f1b2"}.fa-bitcoin-sign:before{content:"\e0b4"}.fa-shield-dog:before{content:"\e573"}.fa-solar-panel:before{content:"\f5ba"}.fa-lock-open:before{content:"\f3c1"}.fa-elevator:before{content:"\e16d"}.fa-money-bill-transfer:before{content:"\e528"}.fa-money-bill-trend-up:before{content:"\e529"}.fa-house-flood-water-circle-arrow-right:before{content:"\e50f"}.fa-poll-h:before,.fa-square-poll-horizontal:before{content:"\f682"}.fa-circle:before{content:"\f111"}.fa-backward-fast:before,.fa-fast-backward:before{content:"\f049"}.fa-recycle:before{content:"\f1b8"}.fa-user-astronaut:before{content:"\f4fb"}.fa-plane-slash:before{content:"\e069"}.fa-trademark:before{content:"\f25c"}.fa-basketball-ball:before,.fa-basketball:before{content:"\f434"}.fa-satellite-dish:before{content:"\f7c0"}.fa-arrow-alt-circle-up:before,.fa-circle-up:before{content:"\f35b"}.fa-mobile-alt:before,.fa-mobile-screen-button:before{content:"\f3cd"}.fa-volume-high:before,.fa-volume-up:before{content:"\f028"}.fa-users-rays:before{content:"\e593"}.fa-wallet:before{content:"\f555"}.fa-clipboard-check:before{content:"\f46c"}.fa-file-audio:before{content:"\f1c7"}.fa-burger:before,.fa-hamburger:before{content:"\f805"}.fa-wrench:before{content:"\f0ad"}.fa-bugs:before{content:"\e4d0"}.fa-rupee-sign:before,.fa-rupee:before{content:"\f156"}.fa-file-image:before{content:"\f1c5"}.fa-circle-question:before,.fa-question-circle:before{content:"\f059"}.fa-plane-departure:before{content:"\f5b0"}.fa-handshake-slash:before{content:"\e060"}.fa-book-bookmark:before{content:"\e0bb"}.fa-code-branch:before{content:"\f126"}.fa-hat-cowboy:before{content:"\f8c0"}.fa-bridge:before{content:"\e4c8"}.fa-phone-alt:before,.fa-phone-flip:before{content:"\f879"}.fa-truck-front:before{content:"\e2b7"}.fa-cat:before{content:"\f6be"}.fa-anchor-circle-exclamation:before{content:"\e4ab"}.fa-truck-field:before{content:"\e58d"}.fa-route:before{content:"\f4d7"}.fa-clipboard-question:before{content:"\e4e3"}.fa-panorama:before{content:"\e209"}.fa-comment-medical:before{content:"\f7f5"}.fa-teeth-open:before{content:"\f62f"}.fa-file-circle-minus:before{content:"\e4ed"}.fa-tags:before{content:"\f02c"}.fa-wine-glass:before{content:"\f4e3"}.fa-fast-forward:before,.fa-forward-fast:before{content:"\f050"}.fa-face-meh-blank:before,.fa-meh-blank:before{content:"\f5a4"}.fa-parking:before,.fa-square-parking:before{content:"\f540"}.fa-house-signal:before{content:"\e012"}.fa-bars-progress:before,.fa-tasks-alt:before{content:"\f828"}.fa-faucet-drip:before{content:"\e006"}.fa-cart-flatbed:before,.fa-dolly-flatbed:before{content:"\f474"}.fa-ban-smoking:before,.fa-smoking-ban:before{content:"\f54d"}.fa-terminal:before{content:"\f120"}.fa-mobile-button:before{content:"\f10b"}.fa-house-medical-flag:before{content:"\e514"}.fa-basket-shopping:before,.fa-shopping-basket:before{content:"\f291"}.fa-tape:before{content:"\f4db"}.fa-bus-alt:before,.fa-bus-simple:before{content:"\f55e"}.fa-eye:before{content:"\f06e"}.fa-face-sad-cry:before,.fa-sad-cry:before{content:"\f5b3"}.fa-audio-description:before{content:"\f29e"}.fa-person-military-to-person:before{content:"\e54c"}.fa-file-shield:before{content:"\e4f0"}.fa-user-slash:before{content:"\f506"}.fa-pen:before{content:"\f304"}.fa-tower-observation:before{content:"\e586"}.fa-file-code:before{content:"\f1c9"}.fa-signal-5:before,.fa-signal-perfect:before,.fa-signal:before{content:"\f012"}.fa-bus:before{content:"\f207"}.fa-heart-circle-xmark:before{content:"\e501"}.fa-home-lg:before,.fa-house-chimney:before{content:"\e3af"}.fa-window-maximize:before{content:"\f2d0"}.fa-face-frown:before,.fa-frown:before{content:"\f119"}.fa-prescription:before{content:"\f5b1"}.fa-shop:before,.fa-store-alt:before{content:"\f54f"}.fa-floppy-disk:before,.fa-save:before{content:"\f0c7"}.fa-vihara:before{content:"\f6a7"}.fa-balance-scale-left:before,.fa-scale-unbalanced:before{content:"\f515"}.fa-sort-asc:before,.fa-sort-up:before{content:"\f0de"}.fa-comment-dots:before,.fa-commenting:before{content:"\f4ad"}.fa-plant-wilt:before{content:"\e5aa"}.fa-diamond:before{content:"\f219"}.fa-face-grin-squint:before,.fa-grin-squint:before{content:"\f585"}.fa-hand-holding-dollar:before,.fa-hand-holding-usd:before{content:"\f4c0"}.fa-bacterium:before{content:"\e05a"}.fa-hand-pointer:before{content:"\f25a"}.fa-drum-steelpan:before{content:"\f56a"}.fa-hand-scissors:before{content:"\f257"}.fa-hands-praying:before,.fa-praying-hands:before{content:"\f684"}.fa-arrow-right-rotate:before,.fa-arrow-rotate-forward:before,.fa-arrow-rotate-right:before,.fa-redo:before{content:"\f01e"}.fa-biohazard:before{content:"\f780"}.fa-location-crosshairs:before,.fa-location:before{content:"\f601"}.fa-mars-double:before{content:"\f227"}.fa-child-dress:before{content:"\e59c"}.fa-users-between-lines:before{content:"\e591"}.fa-lungs-virus:before{content:"\e067"}.fa-face-grin-tears:before,.fa-grin-tears:before{content:"\f588"}.fa-phone:before{content:"\f095"}.fa-calendar-times:before,.fa-calendar-xmark:before{content:"\f273"}.fa-child-reaching:before{content:"\e59d"}.fa-head-side-virus:before{content:"\e064"}.fa-user-cog:before,.fa-user-gear:before{content:"\f4fe"}.fa-arrow-up-1-9:before,.fa-sort-numeric-up:before{content:"\f163"}.fa-door-closed:before{content:"\f52a"}.fa-shield-virus:before{content:"\e06c"}.fa-dice-six:before{content:"\f526"}.fa-mosquito-net:before{content:"\e52c"}.fa-bridge-water:before{content:"\e4ce"}.fa-person-booth:before{content:"\f756"}.fa-text-width:before{content:"\f035"}.fa-hat-wizard:before{content:"\f6e8"}.fa-pen-fancy:before{content:"\f5ac"}.fa-digging:before,.fa-person-digging:before{content:"\f85e"}.fa-trash:before{content:"\f1f8"}.fa-gauge-simple-med:before,.fa-gauge-simple:before,.fa-tachometer-average:before{content:"\f629"}.fa-book-medical:before{content:"\f7e6"}.fa-poo:before{content:"\f2fe"}.fa-quote-right-alt:before,.fa-quote-right:before{content:"\f10e"}.fa-shirt:before,.fa-t-shirt:before,.fa-tshirt:before{content:"\f553"}.fa-cubes:before{content:"\f1b3"}.fa-divide:before{content:"\f529"}.fa-tenge-sign:before,.fa-tenge:before{content:"\f7d7"}.fa-headphones:before{content:"\f025"}.fa-hands-holding:before{content:"\f4c2"}.fa-hands-clapping:before{content:"\e1a8"}.fa-republican:before{content:"\f75e"}.fa-arrow-left:before{content:"\f060"}.fa-person-circle-xmark:before{content:"\e543"}.fa-ruler:before{content:"\f545"}.fa-align-left:before{content:"\f036"}.fa-dice-d6:before{content:"\f6d1"}.fa-restroom:before{content:"\f7bd"}.fa-j:before{content:"\4a"}.fa-users-viewfinder:before{content:"\e595"}.fa-file-video:before{content:"\f1c8"}.fa-external-link-alt:before,.fa-up-right-from-square:before{content:"\f35d"}.fa-table-cells:before,.fa-th:before{content:"\f00a"}.fa-file-pdf:before{content:"\f1c1"}.fa-bible:before,.fa-book-bible:before{content:"\f647"}.fa-o:before{content:"\4f"}.fa-medkit:before,.fa-suitcase-medical:before{content:"\f0fa"}.fa-user-secret:before{content:"\f21b"}.fa-otter:before{content:"\f700"}.fa-female:before,.fa-person-dress:before{content:"\f182"}.fa-comment-dollar:before{content:"\f651"}.fa-briefcase-clock:before,.fa-business-time:before{content:"\f64a"}.fa-table-cells-large:before,.fa-th-large:before{content:"\f009"}.fa-book-tanakh:before,.fa-tanakh:before{content:"\f827"}.fa-phone-volume:before,.fa-volume-control-phone:before{content:"\f2a0"}.fa-hat-cowboy-side:before{content:"\f8c1"}.fa-clipboard-user:before{content:"\f7f3"}.fa-child:before{content:"\f1ae"}.fa-lira-sign:before{content:"\f195"}.fa-satellite:before{content:"\f7bf"}.fa-plane-lock:before{content:"\e558"}.fa-tag:before{content:"\f02b"}.fa-comment:before{content:"\f075"}.fa-birthday-cake:before,.fa-cake-candles:before,.fa-cake:before{content:"\f1fd"}.fa-envelope:before{content:"\f0e0"}.fa-angle-double-up:before,.fa-angles-up:before{content:"\f102"}.fa-paperclip:before{content:"\f0c6"}.fa-arrow-right-to-city:before{content:"\e4b3"}.fa-ribbon:before{content:"\f4d6"}.fa-lungs:before{content:"\f604"}.fa-arrow-up-9-1:before,.fa-sort-numeric-up-alt:before{content:"\f887"}.fa-litecoin-sign:before{content:"\e1d3"}.fa-border-none:before{content:"\f850"}.fa-circle-nodes:before{content:"\e4e2"}.fa-parachute-box:before{content:"\f4cd"}.fa-indent:before{content:"\f03c"}.fa-truck-field-un:before{content:"\e58e"}.fa-hourglass-empty:before,.fa-hourglass:before{content:"\f254"}.fa-mountain:before{content:"\f6fc"}.fa-user-doctor:before,.fa-user-md:before{content:"\f0f0"}.fa-circle-info:before,.fa-info-circle:before{content:"\f05a"}.fa-cloud-meatball:before{content:"\f73b"}.fa-camera-alt:before,.fa-camera:before{content:"\f030"}.fa-square-virus:before{content:"\e578"}.fa-meteor:before{content:"\f753"}.fa-car-on:before{content:"\e4dd"}.fa-sleigh:before{content:"\f7cc"}.fa-arrow-down-1-9:before,.fa-sort-numeric-asc:before,.fa-sort-numeric-down:before{content:"\f162"}.fa-hand-holding-droplet:before,.fa-hand-holding-water:before{content:"\f4c1"}.fa-water:before{content:"\f773"}.fa-calendar-check:before{content:"\f274"}.fa-braille:before{content:"\f2a1"}.fa-prescription-bottle-alt:before,.fa-prescription-bottle-medical:before{content:"\f486"}.fa-landmark:before{content:"\f66f"}.fa-truck:before{content:"\f0d1"}.fa-crosshairs:before{content:"\f05b"}.fa-person-cane:before{content:"\e53c"}.fa-tent:before{content:"\e57d"}.fa-vest-patches:before{content:"\e086"}.fa-check-double:before{content:"\f560"}.fa-arrow-down-a-z:before,.fa-sort-alpha-asc:before,.fa-sort-alpha-down:before{content:"\f15d"}.fa-money-bill-wheat:before{content:"\e52a"}.fa-cookie:before{content:"\f563"}.fa-arrow-left-rotate:before,.fa-arrow-rotate-back:before,.fa-arrow-rotate-backward:before,.fa-arrow-rotate-left:before,.fa-undo:before{content:"\f0e2"}.fa-hard-drive:before,.fa-hdd:before{content:"\f0a0"}.fa-face-grin-squint-tears:before,.fa-grin-squint-tears:before{content:"\f586"}.fa-dumbbell:before{content:"\f44b"}.fa-list-alt:before,.fa-rectangle-list:before{content:"\f022"}.fa-tarp-droplet:before{content:"\e57c"}.fa-house-medical-circle-check:before{content:"\e511"}.fa-person-skiing-nordic:before,.fa-skiing-nordic:before{content:"\f7ca"}.fa-calendar-plus:before{content:"\f271"}.fa-plane-arrival:before{content:"\f5af"}.fa-arrow-alt-circle-left:before,.fa-circle-left:before{content:"\f359"}.fa-subway:before,.fa-train-subway:before{content:"\f239"}.fa-chart-gantt:before{content:"\e0e4"}.fa-indian-rupee-sign:before,.fa-indian-rupee:before,.fa-inr:before{content:"\e1bc"}.fa-crop-alt:before,.fa-crop-simple:before{content:"\f565"}.fa-money-bill-1:before,.fa-money-bill-alt:before{content:"\f3d1"}.fa-left-long:before,.fa-long-arrow-alt-left:before{content:"\f30a"}.fa-dna:before{content:"\f471"}.fa-virus-slash:before{content:"\e075"}.fa-minus:before,.fa-subtract:before{content:"\f068"}.fa-chess:before{content:"\f439"}.fa-arrow-left-long:before,.fa-long-arrow-left:before{content:"\f177"}.fa-plug-circle-check:before{content:"\e55c"}.fa-street-view:before{content:"\f21d"}.fa-franc-sign:before{content:"\e18f"}.fa-volume-off:before{content:"\f026"}.fa-american-sign-language-interpreting:before,.fa-asl-interpreting:before,.fa-hands-american-sign-language-interpreting:before,.fa-hands-asl-interpreting:before{content:"\f2a3"}.fa-cog:before,.fa-gear:before{content:"\f013"}.fa-droplet-slash:before,.fa-tint-slash:before{content:"\f5c7"}.fa-mosque:before{content:"\f678"}.fa-mosquito:before{content:"\e52b"}.fa-star-of-david:before{content:"\f69a"}.fa-person-military-rifle:before{content:"\e54b"}.fa-cart-shopping:before,.fa-shopping-cart:before{content:"\f07a"}.fa-vials:before{content:"\f493"}.fa-plug-circle-plus:before{content:"\e55f"}.fa-place-of-worship:before{content:"\f67f"}.fa-grip-vertical:before{content:"\f58e"}.fa-arrow-turn-up:before,.fa-level-up:before{content:"\f148"}.fa-u:before{content:"\55"}.fa-square-root-alt:before,.fa-square-root-variable:before{content:"\f698"}.fa-clock-four:before,.fa-clock:before{content:"\f017"}.fa-backward-step:before,.fa-step-backward:before{content:"\f048"}.fa-pallet:before{content:"\f482"}.fa-faucet:before{content:"\e005"}.fa-baseball-bat-ball:before{content:"\f432"}.fa-s:before{content:"\53"}.fa-timeline:before{content:"\e29c"}.fa-keyboard:before{content:"\f11c"}.fa-caret-down:before{content:"\f0d7"}.fa-clinic-medical:before,.fa-house-chimney-medical:before{content:"\f7f2"}.fa-temperature-3:before,.fa-temperature-three-quarters:before,.fa-thermometer-3:before,.fa-thermometer-three-quarters:before{content:"\f2c8"}.fa-mobile-android-alt:before,.fa-mobile-screen:before{content:"\f3cf"}.fa-plane-up:before{content:"\e22d"}.fa-piggy-bank:before{content:"\f4d3"}.fa-battery-3:before,.fa-battery-half:before{content:"\f242"}.fa-mountain-city:before{content:"\e52e"}.fa-coins:before{content:"\f51e"}.fa-khanda:before{content:"\f66d"}.fa-sliders-h:before,.fa-sliders:before{content:"\f1de"}.fa-folder-tree:before{content:"\f802"}.fa-network-wired:before{content:"\f6ff"}.fa-map-pin:before{content:"\f276"}.fa-hamsa:before{content:"\f665"}.fa-cent-sign:before{content:"\e3f5"}.fa-flask:before{content:"\f0c3"}.fa-person-pregnant:before{content:"\e31e"}.fa-wand-sparkles:before{content:"\f72b"}.fa-ellipsis-v:before,.fa-ellipsis-vertical:before{content:"\f142"}.fa-ticket:before{content:"\f145"}.fa-power-off:before{content:"\f011"}.fa-long-arrow-alt-right:before,.fa-right-long:before{content:"\f30b"}.fa-flag-usa:before{content:"\f74d"}.fa-laptop-file:before{content:"\e51d"}.fa-teletype:before,.fa-tty:before{content:"\f1e4"}.fa-diagram-next:before{content:"\e476"}.fa-person-rifle:before{content:"\e54e"}.fa-house-medical-circle-exclamation:before{content:"\e512"}.fa-closed-captioning:before{content:"\f20a"}.fa-hiking:before,.fa-person-hiking:before{content:"\f6ec"}.fa-venus-double:before{content:"\f226"}.fa-images:before{content:"\f302"}.fa-calculator:before{content:"\f1ec"}.fa-people-pulling:before{content:"\e535"}.fa-n:before{content:"\4e"}.fa-cable-car:before,.fa-tram:before{content:"\f7da"}.fa-cloud-rain:before{content:"\f73d"}.fa-building-circle-xmark:before{content:"\e4d4"}.fa-ship:before{content:"\f21a"}.fa-arrows-down-to-line:before{content:"\e4b8"}.fa-download:before{content:"\f019"}.fa-face-grin:before,.fa-grin:before{content:"\f580"}.fa-backspace:before,.fa-delete-left:before{content:"\f55a"}.fa-eye-dropper-empty:before,.fa-eye-dropper:before,.fa-eyedropper:before{content:"\f1fb"}.fa-file-circle-check:before{content:"\e5a0"}.fa-forward:before{content:"\f04e"}.fa-mobile-android:before,.fa-mobile-phone:before,.fa-mobile:before{content:"\f3ce"}.fa-face-meh:before,.fa-meh:before{content:"\f11a"}.fa-align-center:before{content:"\f037"}.fa-book-dead:before,.fa-book-skull:before{content:"\f6b7"}.fa-drivers-license:before,.fa-id-card:before{content:"\f2c2"}.fa-dedent:before,.fa-outdent:before{content:"\f03b"}.fa-heart-circle-exclamation:before{content:"\e4fe"}.fa-home-alt:before,.fa-home-lg-alt:before,.fa-home:before,.fa-house:before{content:"\f015"}.fa-calendar-week:before{content:"\f784"}.fa-laptop-medical:before{content:"\f812"}.fa-b:before{content:"\42"}.fa-file-medical:before{content:"\f477"}.fa-dice-one:before{content:"\f525"}.fa-kiwi-bird:before{content:"\f535"}.fa-arrow-right-arrow-left:before,.fa-exchange:before{content:"\f0ec"}.fa-redo-alt:before,.fa-rotate-forward:before,.fa-rotate-right:before{content:"\f2f9"}.fa-cutlery:before,.fa-utensils:before{content:"\f2e7"}.fa-arrow-up-wide-short:before,.fa-sort-amount-up:before{content:"\f161"}.fa-mill-sign:before{content:"\e1ed"}.fa-bowl-rice:before{content:"\e2eb"}.fa-skull:before{content:"\f54c"}.fa-broadcast-tower:before,.fa-tower-broadcast:before{content:"\f519"}.fa-truck-pickup:before{content:"\f63c"}.fa-long-arrow-alt-up:before,.fa-up-long:before{content:"\f30c"}.fa-stop:before{content:"\f04d"}.fa-code-merge:before{content:"\f387"}.fa-upload:before{content:"\f093"}.fa-hurricane:before{content:"\f751"}.fa-mound:before{content:"\e52d"}.fa-toilet-portable:before{content:"\e583"}.fa-compact-disc:before{content:"\f51f"}.fa-file-arrow-down:before,.fa-file-download:before{content:"\f56d"}.fa-caravan:before{content:"\f8ff"}.fa-shield-cat:before{content:"\e572"}.fa-bolt:before,.fa-zap:before{content:"\f0e7"}.fa-glass-water:before{content:"\e4f4"}.fa-oil-well:before{content:"\e532"}.fa-vault:before{content:"\e2c5"}.fa-mars:before{content:"\f222"}.fa-toilet:before{content:"\f7d8"}.fa-plane-circle-xmark:before{content:"\e557"}.fa-cny:before,.fa-jpy:before,.fa-rmb:before,.fa-yen-sign:before,.fa-yen:before{content:"\f157"}.fa-rouble:before,.fa-rub:before,.fa-ruble-sign:before,.fa-ruble:before{content:"\f158"}.fa-sun:before{content:"\f185"}.fa-guitar:before{content:"\f7a6"}.fa-face-laugh-wink:before,.fa-laugh-wink:before{content:"\f59c"}.fa-horse-head:before{content:"\f7ab"}.fa-bore-hole:before{content:"\e4c3"}.fa-industry:before{content:"\f275"}.fa-arrow-alt-circle-down:before,.fa-circle-down:before{content:"\f358"}.fa-arrows-turn-to-dots:before{content:"\e4c1"}.fa-florin-sign:before{content:"\e184"}.fa-arrow-down-short-wide:before,.fa-sort-amount-desc:before,.fa-sort-amount-down-alt:before{content:"\f884"}.fa-less-than:before{content:"\3c"}.fa-angle-down:before{content:"\f107"}.fa-car-tunnel:before{content:"\e4de"}.fa-head-side-cough:before{content:"\e061"}.fa-grip-lines:before{content:"\f7a4"}.fa-thumbs-down:before{content:"\f165"}.fa-user-lock:before{content:"\f502"}.fa-arrow-right-long:before,.fa-long-arrow-right:before{content:"\f178"}.fa-anchor-circle-xmark:before{content:"\e4ac"}.fa-ellipsis-h:before,.fa-ellipsis:before{content:"\f141"}.fa-chess-pawn:before{content:"\f443"}.fa-first-aid:before,.fa-kit-medical:before{content:"\f479"}.fa-person-through-window:before{content:"\e5a9"}.fa-toolbox:before{content:"\f552"}.fa-hands-holding-circle:before{content:"\e4fb"}.fa-bug:before{content:"\f188"}.fa-credit-card-alt:before,.fa-credit-card:before{content:"\f09d"}.fa-automobile:before,.fa-car:before{content:"\f1b9"}.fa-hand-holding-hand:before{content:"\e4f7"}.fa-book-open-reader:before,.fa-book-reader:before{content:"\f5da"}.fa-mountain-sun:before{content:"\e52f"}.fa-arrows-left-right-to-line:before{content:"\e4ba"}.fa-dice-d20:before{content:"\f6cf"}.fa-truck-droplet:before{content:"\e58c"}.fa-file-circle-xmark:before{content:"\e5a1"}.fa-temperature-arrow-up:before,.fa-temperature-up:before{content:"\e040"}.fa-medal:before{content:"\f5a2"}.fa-bed:before{content:"\f236"}.fa-h-square:before,.fa-square-h:before{content:"\f0fd"}.fa-podcast:before{content:"\f2ce"}.fa-temperature-4:before,.fa-temperature-full:before,.fa-thermometer-4:before,.fa-thermometer-full:before{content:"\f2c7"}.fa-bell:before{content:"\f0f3"}.fa-superscript:before{content:"\f12b"}.fa-plug-circle-xmark:before{content:"\e560"}.fa-star-of-life:before{content:"\f621"}.fa-phone-slash:before{content:"\f3dd"}.fa-paint-roller:before{content:"\f5aa"}.fa-hands-helping:before,.fa-handshake-angle:before{content:"\f4c4"}.fa-location-dot:before,.fa-map-marker-alt:before{content:"\f3c5"}.fa-file:before{content:"\f15b"}.fa-greater-than:before{content:"\3e"}.fa-person-swimming:before,.fa-swimmer:before{content:"\f5c4"}.fa-arrow-down:before{content:"\f063"}.fa-droplet:before,.fa-tint:before{content:"\f043"}.fa-eraser:before{content:"\f12d"}.fa-earth-america:before,.fa-earth-americas:before,.fa-earth:before,.fa-globe-americas:before{content:"\f57d"}.fa-person-burst:before{content:"\e53b"}.fa-dove:before{content:"\f4ba"}.fa-battery-0:before,.fa-battery-empty:before{content:"\f244"}.fa-socks:before{content:"\f696"}.fa-inbox:before{content:"\f01c"}.fa-section:before{content:"\e447"}.fa-gauge-high:before,.fa-tachometer-alt-fast:before,.fa-tachometer-alt:before{content:"\f625"}.fa-envelope-open-text:before{content:"\f658"}.fa-hospital-alt:before,.fa-hospital-wide:before,.fa-hospital:before{content:"\f0f8"}.fa-wine-bottle:before{content:"\f72f"}.fa-chess-rook:before{content:"\f447"}.fa-bars-staggered:before,.fa-reorder:before,.fa-stream:before{content:"\f550"}.fa-dharmachakra:before{content:"\f655"}.fa-hotdog:before{content:"\f80f"}.fa-blind:before,.fa-person-walking-with-cane:before{content:"\f29d"}.fa-drum:before{content:"\f569"}.fa-ice-cream:before{content:"\f810"}.fa-heart-circle-bolt:before{content:"\e4fc"}.fa-fax:before{content:"\f1ac"}.fa-paragraph:before{content:"\f1dd"}.fa-check-to-slot:before,.fa-vote-yea:before{content:"\f772"}.fa-star-half:before{content:"\f089"}.fa-boxes-alt:before,.fa-boxes-stacked:before,.fa-boxes:before{content:"\f468"}.fa-chain:before,.fa-link:before{content:"\f0c1"}.fa-assistive-listening-systems:before,.fa-ear-listen:before{content:"\f2a2"}.fa-tree-city:before{content:"\e587"}.fa-play:before{content:"\f04b"}.fa-font:before{content:"\f031"}.fa-rupiah-sign:before{content:"\e23d"}.fa-magnifying-glass:before,.fa-search:before{content:"\f002"}.fa-ping-pong-paddle-ball:before,.fa-table-tennis-paddle-ball:before,.fa-table-tennis:before{content:"\f45d"}.fa-diagnoses:before,.fa-person-dots-from-line:before{content:"\f470"}.fa-trash-can-arrow-up:before,.fa-trash-restore-alt:before{content:"\f82a"}.fa-naira-sign:before{content:"\e1f6"}.fa-cart-arrow-down:before{content:"\f218"}.fa-walkie-talkie:before{content:"\f8ef"}.fa-file-edit:before,.fa-file-pen:before{content:"\f31c"}.fa-receipt:before{content:"\f543"}.fa-pen-square:before,.fa-pencil-square:before,.fa-square-pen:before{content:"\f14b"}.fa-suitcase-rolling:before{content:"\f5c1"}.fa-person-circle-exclamation:before{content:"\e53f"}.fa-chevron-down:before{content:"\f078"}.fa-battery-5:before,.fa-battery-full:before,.fa-battery:before{content:"\f240"}.fa-skull-crossbones:before{content:"\f714"}.fa-code-compare:before{content:"\e13a"}.fa-list-dots:before,.fa-list-ul:before{content:"\f0ca"}.fa-school-lock:before{content:"\e56f"}.fa-tower-cell:before{content:"\e585"}.fa-down-long:before,.fa-long-arrow-alt-down:before{content:"\f309"}.fa-ranking-star:before{content:"\e561"}.fa-chess-king:before{content:"\f43f"}.fa-person-harassing:before{content:"\e549"}.fa-brazilian-real-sign:before{content:"\e46c"}.fa-landmark-alt:before,.fa-landmark-dome:before{content:"\f752"}.fa-arrow-up:before{content:"\f062"}.fa-television:before,.fa-tv-alt:before,.fa-tv:before{content:"\f26c"}.fa-shrimp:before{content:"\e448"}.fa-list-check:before,.fa-tasks:before{content:"\f0ae"}.fa-jug-detergent:before{content:"\e519"}.fa-circle-user:before,.fa-user-circle:before{content:"\f2bd"}.fa-user-shield:before{content:"\f505"}.fa-wind:before{content:"\f72e"}.fa-car-burst:before,.fa-car-crash:before{content:"\f5e1"}.fa-y:before{content:"\59"}.fa-person-snowboarding:before,.fa-snowboarding:before{content:"\f7ce"}.fa-shipping-fast:before,.fa-truck-fast:before{content:"\f48b"}.fa-fish:before{content:"\f578"}.fa-user-graduate:before{content:"\f501"}.fa-adjust:before,.fa-circle-half-stroke:before{content:"\f042"}.fa-clapperboard:before{content:"\e131"}.fa-circle-radiation:before,.fa-radiation-alt:before{content:"\f7ba"}.fa-baseball-ball:before,.fa-baseball:before{content:"\f433"}.fa-jet-fighter-up:before{content:"\e518"}.fa-diagram-project:before,.fa-project-diagram:before{content:"\f542"}.fa-copy:before{content:"\f0c5"}.fa-volume-mute:before,.fa-volume-times:before,.fa-volume-xmark:before{content:"\f6a9"}.fa-hand-sparkles:before{content:"\e05d"}.fa-grip-horizontal:before,.fa-grip:before{content:"\f58d"}.fa-share-from-square:before,.fa-share-square:before{content:"\f14d"}.fa-child-combatant:before,.fa-child-rifle:before{content:"\e4e0"}.fa-gun:before{content:"\e19b"}.fa-phone-square:before,.fa-square-phone:before{content:"\f098"}.fa-add:before,.fa-plus:before{content:"\2b"}.fa-expand:before{content:"\f065"}.fa-computer:before{content:"\e4e5"}.fa-close:before,.fa-multiply:before,.fa-remove:before,.fa-times:before,.fa-xmark:before{content:"\f00d"}.fa-arrows-up-down-left-right:before,.fa-arrows:before{content:"\f047"}.fa-chalkboard-teacher:before,.fa-chalkboard-user:before{content:"\f51c"}.fa-peso-sign:before{content:"\e222"}.fa-building-shield:before{content:"\e4d8"}.fa-baby:before{content:"\f77c"}.fa-users-line:before{content:"\e592"}.fa-quote-left-alt:before,.fa-quote-left:before{content:"\f10d"}.fa-tractor:before{content:"\f722"}.fa-trash-arrow-up:before,.fa-trash-restore:before{content:"\f829"}.fa-arrow-down-up-lock:before{content:"\e4b0"}.fa-lines-leaning:before{content:"\e51e"}.fa-ruler-combined:before{content:"\f546"}.fa-copyright:before{content:"\f1f9"}.fa-equals:before{content:"\3d"}.fa-blender:before{content:"\f517"}.fa-teeth:before{content:"\f62e"}.fa-ils:before,.fa-shekel-sign:before,.fa-shekel:before,.fa-sheqel-sign:before,.fa-sheqel:before{content:"\f20b"}.fa-map:before{content:"\f279"}.fa-rocket:before{content:"\f135"}.fa-photo-film:before,.fa-photo-video:before{content:"\f87c"}.fa-folder-minus:before{content:"\f65d"}.fa-store:before{content:"\f54e"}.fa-arrow-trend-up:before{content:"\e098"}.fa-plug-circle-minus:before{content:"\e55e"}.fa-sign-hanging:before,.fa-sign:before{content:"\f4d9"}.fa-bezier-curve:before{content:"\f55b"}.fa-bell-slash:before{content:"\f1f6"}.fa-tablet-android:before,.fa-tablet:before{content:"\f3fb"}.fa-school-flag:before{content:"\e56e"}.fa-fill:before{content:"\f575"}.fa-angle-up:before{content:"\f106"}.fa-drumstick-bite:before{content:"\f6d7"}.fa-holly-berry:before{content:"\f7aa"}.fa-chevron-left:before{content:"\f053"}.fa-bacteria:before{content:"\e059"}.fa-hand-lizard:before{content:"\f258"}.fa-notdef:before{content:"\e1fe"}.fa-disease:before{content:"\f7fa"}.fa-briefcase-medical:before{content:"\f469"}.fa-genderless:before{content:"\f22d"}.fa-chevron-right:before{content:"\f054"}.fa-retweet:before{content:"\f079"}.fa-car-alt:before,.fa-car-rear:before{content:"\f5de"}.fa-pump-soap:before{content:"\e06b"}.fa-video-slash:before{content:"\f4e2"}.fa-battery-2:before,.fa-battery-quarter:before{content:"\f243"}.fa-radio:before{content:"\f8d7"}.fa-baby-carriage:before,.fa-carriage-baby:before{content:"\f77d"}.fa-traffic-light:before{content:"\f637"}.fa-thermometer:before{content:"\f491"}.fa-vr-cardboard:before{content:"\f729"}.fa-hand-middle-finger:before{content:"\f806"}.fa-percent:before,.fa-percentage:before{content:"\25"}.fa-truck-moving:before{content:"\f4df"}.fa-glass-water-droplet:before{content:"\e4f5"}.fa-display:before{content:"\e163"}.fa-face-smile:before,.fa-smile:before{content:"\f118"}.fa-thumb-tack:before,.fa-thumbtack:before{content:"\f08d"}.fa-trophy:before{content:"\f091"}.fa-person-praying:before,.fa-pray:before{content:"\f683"}.fa-hammer:before{content:"\f6e3"}.fa-hand-peace:before{content:"\f25b"}.fa-rotate:before,.fa-sync-alt:before{content:"\f2f1"}.fa-spinner:before{content:"\f110"}.fa-robot:before{content:"\f544"}.fa-peace:before{content:"\f67c"}.fa-cogs:before,.fa-gears:before{content:"\f085"}.fa-warehouse:before{content:"\f494"}.fa-arrow-up-right-dots:before{content:"\e4b7"}.fa-splotch:before{content:"\f5bc"}.fa-face-grin-hearts:before,.fa-grin-hearts:before{content:"\f584"}.fa-dice-four:before{content:"\f524"}.fa-sim-card:before{content:"\f7c4"}.fa-transgender-alt:before,.fa-transgender:before{content:"\f225"}.fa-mercury:before{content:"\f223"}.fa-arrow-turn-down:before,.fa-level-down:before{content:"\f149"}.fa-person-falling-burst:before{content:"\e547"}.fa-award:before{content:"\f559"}.fa-ticket-alt:before,.fa-ticket-simple:before{content:"\f3ff"}.fa-building:before{content:"\f1ad"}.fa-angle-double-left:before,.fa-angles-left:before{content:"\f100"}.fa-qrcode:before{content:"\f029"}.fa-clock-rotate-left:before,.fa-history:before{content:"\f1da"}.fa-face-grin-beam-sweat:before,.fa-grin-beam-sweat:before{content:"\f583"}.fa-arrow-right-from-file:before,.fa-file-export:before{content:"\f56e"}.fa-shield-blank:before,.fa-shield:before{content:"\f132"}.fa-arrow-up-short-wide:before,.fa-sort-amount-up-alt:before{content:"\f885"}.fa-house-medical:before{content:"\e3b2"}.fa-golf-ball-tee:before,.fa-golf-ball:before{content:"\f450"}.fa-chevron-circle-left:before,.fa-circle-chevron-left:before{content:"\f137"}.fa-house-chimney-window:before{content:"\e00d"}.fa-pen-nib:before{content:"\f5ad"}.fa-tent-arrow-turn-left:before{content:"\e580"}.fa-tents:before{content:"\e582"}.fa-magic:before,.fa-wand-magic:before{content:"\f0d0"}.fa-dog:before{content:"\f6d3"}.fa-carrot:before{content:"\f787"}.fa-moon:before{content:"\f186"}.fa-wine-glass-alt:before,.fa-wine-glass-empty:before{content:"\f5ce"}.fa-cheese:before{content:"\f7ef"}.fa-yin-yang:before{content:"\f6ad"}.fa-music:before{content:"\f001"}.fa-code-commit:before{content:"\f386"}.fa-temperature-low:before{content:"\f76b"}.fa-biking:before,.fa-person-biking:before{content:"\f84a"}.fa-broom:before{content:"\f51a"}.fa-shield-heart:before{content:"\e574"}.fa-gopuram:before{content:"\f664"}.fa-earth-oceania:before,.fa-globe-oceania:before{content:"\e47b"}.fa-square-xmark:before,.fa-times-square:before,.fa-xmark-square:before{content:"\f2d3"}.fa-hashtag:before{content:"\23"}.fa-expand-alt:before,.fa-up-right-and-down-left-from-center:before{content:"\f424"}.fa-oil-can:before{content:"\f613"}.fa-t:before{content:"\54"}.fa-hippo:before{content:"\f6ed"}.fa-chart-column:before{content:"\e0e3"}.fa-infinity:before{content:"\f534"}.fa-vial-circle-check:before{content:"\e596"}.fa-person-arrow-down-to-line:before{content:"\e538"}.fa-voicemail:before{content:"\f897"}.fa-fan:before{content:"\f863"}.fa-person-walking-luggage:before{content:"\e554"}.fa-arrows-alt-v:before,.fa-up-down:before{content:"\f338"}.fa-cloud-moon-rain:before{content:"\f73c"}.fa-calendar:before{content:"\f133"}.fa-trailer:before{content:"\e041"}.fa-bahai:before,.fa-haykal:before{content:"\f666"}.fa-sd-card:before{content:"\f7c2"}.fa-dragon:before{content:"\f6d5"}.fa-shoe-prints:before{content:"\f54b"}.fa-circle-plus:before,.fa-plus-circle:before{content:"\f055"}.fa-face-grin-tongue-wink:before,.fa-grin-tongue-wink:before{content:"\f58b"}.fa-hand-holding:before{content:"\f4bd"}.fa-plug-circle-exclamation:before{content:"\e55d"}.fa-chain-broken:before,.fa-chain-slash:before,.fa-link-slash:before,.fa-unlink:before{content:"\f127"}.fa-clone:before{content:"\f24d"}.fa-person-walking-arrow-loop-left:before{content:"\e551"}.fa-arrow-up-z-a:before,.fa-sort-alpha-up-alt:before{content:"\f882"}.fa-fire-alt:before,.fa-fire-flame-curved:before{content:"\f7e4"}.fa-tornado:before{content:"\f76f"}.fa-file-circle-plus:before{content:"\e494"}.fa-book-quran:before,.fa-quran:before{content:"\f687"}.fa-anchor:before{content:"\f13d"}.fa-border-all:before{content:"\f84c"}.fa-angry:before,.fa-face-angry:before{content:"\f556"}.fa-cookie-bite:before{content:"\f564"}.fa-arrow-trend-down:before{content:"\e097"}.fa-feed:before,.fa-rss:before{content:"\f09e"}.fa-draw-polygon:before{content:"\f5ee"}.fa-balance-scale:before,.fa-scale-balanced:before{content:"\f24e"}.fa-gauge-simple-high:before,.fa-tachometer-fast:before,.fa-tachometer:before{content:"\f62a"}.fa-shower:before{content:"\f2cc"}.fa-desktop-alt:before,.fa-desktop:before{content:"\f390"}.fa-m:before{content:"\4d"}.fa-table-list:before,.fa-th-list:before{content:"\f00b"}.fa-comment-sms:before,.fa-sms:before{content:"\f7cd"}.fa-book:before{content:"\f02d"}.fa-user-plus:before{content:"\f234"}.fa-check:before{content:"\f00c"}.fa-battery-4:before,.fa-battery-three-quarters:before{content:"\f241"}.fa-house-circle-check:before{content:"\e509"}.fa-angle-left:before{content:"\f104"}.fa-diagram-successor:before{content:"\e47a"}.fa-truck-arrow-right:before{content:"\e58b"}.fa-arrows-split-up-and-left:before{content:"\e4bc"}.fa-fist-raised:before,.fa-hand-fist:before{content:"\f6de"}.fa-cloud-moon:before{content:"\f6c3"}.fa-briefcase:before{content:"\f0b1"}.fa-person-falling:before{content:"\e546"}.fa-image-portrait:before,.fa-portrait:before{content:"\f3e0"}.fa-user-tag:before{content:"\f507"}.fa-rug:before{content:"\e569"}.fa-earth-europe:before,.fa-globe-europe:before{content:"\f7a2"}.fa-cart-flatbed-suitcase:before,.fa-luggage-cart:before{content:"\f59d"}.fa-rectangle-times:before,.fa-rectangle-xmark:before,.fa-times-rectangle:before,.fa-window-close:before{content:"\f410"}.fa-baht-sign:before{content:"\e0ac"}.fa-book-open:before{content:"\f518"}.fa-book-journal-whills:before,.fa-journal-whills:before{content:"\f66a"}.fa-handcuffs:before{content:"\e4f8"}.fa-exclamation-triangle:before,.fa-triangle-exclamation:before,.fa-warning:before{content:"\f071"}.fa-database:before{content:"\f1c0"}.fa-arrow-turn-right:before,.fa-mail-forward:before,.fa-share:before{content:"\f064"}.fa-bottle-droplet:before{content:"\e4c4"}.fa-mask-face:before{content:"\e1d7"}.fa-hill-rockslide:before{content:"\e508"}.fa-exchange-alt:before,.fa-right-left:before{content:"\f362"}.fa-paper-plane:before{content:"\f1d8"}.fa-road-circle-exclamation:before{content:"\e565"}.fa-dungeon:before{content:"\f6d9"}.fa-align-right:before{content:"\f038"}.fa-money-bill-1-wave:before,.fa-money-bill-wave-alt:before{content:"\f53b"}.fa-life-ring:before{content:"\f1cd"}.fa-hands:before,.fa-sign-language:before,.fa-signing:before{content:"\f2a7"}.fa-calendar-day:before{content:"\f783"}.fa-ladder-water:before,.fa-swimming-pool:before,.fa-water-ladder:before{content:"\f5c5"}.fa-arrows-up-down:before,.fa-arrows-v:before{content:"\f07d"}.fa-face-grimace:before,.fa-grimace:before{content:"\f57f"}.fa-wheelchair-alt:before,.fa-wheelchair-move:before{content:"\e2ce"}.fa-level-down-alt:before,.fa-turn-down:before{content:"\f3be"}.fa-person-walking-arrow-right:before{content:"\e552"}.fa-envelope-square:before,.fa-square-envelope:before{content:"\f199"}.fa-dice:before{content:"\f522"}.fa-bowling-ball:before{content:"\f436"}.fa-brain:before{content:"\f5dc"}.fa-band-aid:before,.fa-bandage:before{content:"\f462"}.fa-calendar-minus:before{content:"\f272"}.fa-circle-xmark:before,.fa-times-circle:before,.fa-xmark-circle:before{content:"\f057"}.fa-gifts:before{content:"\f79c"}.fa-hotel:before{content:"\f594"}.fa-earth-asia:before,.fa-globe-asia:before{content:"\f57e"}.fa-id-card-alt:before,.fa-id-card-clip:before{content:"\f47f"}.fa-magnifying-glass-plus:before,.fa-search-plus:before{content:"\f00e"}.fa-thumbs-up:before{content:"\f164"}.fa-user-clock:before{content:"\f4fd"}.fa-allergies:before,.fa-hand-dots:before{content:"\f461"}.fa-file-invoice:before{content:"\f570"}.fa-window-minimize:before{content:"\f2d1"}.fa-coffee:before,.fa-mug-saucer:before{content:"\f0f4"}.fa-brush:before{content:"\f55d"}.fa-mask:before{content:"\f6fa"}.fa-magnifying-glass-minus:before,.fa-search-minus:before{content:"\f010"}.fa-ruler-vertical:before{content:"\f548"}.fa-user-alt:before,.fa-user-large:before{content:"\f406"}.fa-train-tram:before{content:"\e5b4"}.fa-user-nurse:before{content:"\f82f"}.fa-syringe:before{content:"\f48e"}.fa-cloud-sun:before{content:"\f6c4"}.fa-stopwatch-20:before{content:"\e06f"}.fa-square-full:before{content:"\f45c"}.fa-magnet:before{content:"\f076"}.fa-jar:before{content:"\e516"}.fa-note-sticky:before,.fa-sticky-note:before{content:"\f249"}.fa-bug-slash:before{content:"\e490"}.fa-arrow-up-from-water-pump:before{content:"\e4b6"}.fa-bone:before{content:"\f5d7"}.fa-user-injured:before{content:"\f728"}.fa-face-sad-tear:before,.fa-sad-tear:before{content:"\f5b4"}.fa-plane:before{content:"\f072"}.fa-tent-arrows-down:before{content:"\e581"}.fa-exclamation:before{content:"\21"}.fa-arrows-spin:before{content:"\e4bb"}.fa-print:before{content:"\f02f"}.fa-try:before,.fa-turkish-lira-sign:before,.fa-turkish-lira:before{content:"\e2bb"}.fa-dollar-sign:before,.fa-dollar:before,.fa-usd:before{content:"\24"}.fa-x:before{content:"\58"}.fa-magnifying-glass-dollar:before,.fa-search-dollar:before{content:"\f688"}.fa-users-cog:before,.fa-users-gear:before{content:"\f509"}.fa-person-military-pointing:before{content:"\e54a"}.fa-bank:before,.fa-building-columns:before,.fa-institution:before,.fa-museum:before,.fa-university:before{content:"\f19c"}.fa-umbrella:before{content:"\f0e9"}.fa-trowel:before{content:"\e589"}.fa-d:before{content:"\44"}.fa-stapler:before{content:"\e5af"}.fa-masks-theater:before,.fa-theater-masks:before{content:"\f630"}.fa-kip-sign:before{content:"\e1c4"}.fa-hand-point-left:before{content:"\f0a5"}.fa-handshake-alt:before,.fa-handshake-simple:before{content:"\f4c6"}.fa-fighter-jet:before,.fa-jet-fighter:before{content:"\f0fb"}.fa-share-alt-square:before,.fa-square-share-nodes:before{content:"\f1e1"}.fa-barcode:before{content:"\f02a"}.fa-plus-minus:before{content:"\e43c"}.fa-video-camera:before,.fa-video:before{content:"\f03d"}.fa-graduation-cap:before,.fa-mortar-board:before{content:"\f19d"}.fa-hand-holding-medical:before{content:"\e05c"}.fa-person-circle-check:before{content:"\e53e"}.fa-level-up-alt:before,.fa-turn-up:before{content:"\f3bf"}.fa-sr-only,.fa-sr-only-focusable:not(:focus),.sr-only,.sr-only-focusable:not(:focus){position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);white-space:nowrap;border-width:0}:host,:root{--fa-style-family-brands:"Font Awesome 6 Brands";--fa-font-brands:normal 400 1em/1 "Font Awesome 6 Brands"}@font-face{font-family:"Font Awesome 6 Brands";font-style:normal;font-weight:400;font-display:block;src:url(../webfonts/fa-brands-400.woff2) format("woff2"),url(../webfonts/fa-brands-400.ttf) format("truetype")}.fa-brands,.fab{font-weight:400}.fa-monero:before{content:"\f3d0"}.fa-hooli:before{content:"\f427"}.fa-yelp:before{content:"\f1e9"}.fa-cc-visa:before{content:"\f1f0"}.fa-lastfm:before{content:"\f202"}.fa-shopware:before{content:"\f5b5"}.fa-creative-commons-nc:before{content:"\f4e8"}.fa-aws:before{content:"\f375"}.fa-redhat:before{content:"\f7bc"}.fa-yoast:before{content:"\f2b1"}.fa-cloudflare:before{content:"\e07d"}.fa-ups:before{content:"\f7e0"}.fa-wpexplorer:before{content:"\f2de"}.fa-dyalog:before{content:"\f399"}.fa-bity:before{content:"\f37a"}.fa-stackpath:before{content:"\f842"}.fa-buysellads:before{content:"\f20d"}.fa-first-order:before{content:"\f2b0"}.fa-modx:before{content:"\f285"}.fa-guilded:before{content:"\e07e"}.fa-vnv:before{content:"\f40b"}.fa-js-square:before,.fa-square-js:before{content:"\f3b9"}.fa-microsoft:before{content:"\f3ca"}.fa-qq:before{content:"\f1d6"}.fa-orcid:before{content:"\f8d2"}.fa-java:before{content:"\f4e4"}.fa-invision:before{content:"\f7b0"}.fa-creative-commons-pd-alt:before{content:"\f4ed"}.fa-centercode:before{content:"\f380"}.fa-glide-g:before{content:"\f2a6"}.fa-drupal:before{content:"\f1a9"}.fa-hire-a-helper:before{content:"\f3b0"}.fa-creative-commons-by:before{content:"\f4e7"}.fa-unity:before{content:"\e049"}.fa-whmcs:before{content:"\f40d"}.fa-rocketchat:before{content:"\f3e8"}.fa-vk:before{content:"\f189"}.fa-untappd:before{content:"\f405"}.fa-mailchimp:before{content:"\f59e"}.fa-css3-alt:before{content:"\f38b"}.fa-reddit-square:before,.fa-square-reddit:before{content:"\f1a2"}.fa-vimeo-v:before{content:"\f27d"}.fa-contao:before{content:"\f26d"}.fa-square-font-awesome:before{content:"\e5ad"}.fa-deskpro:before{content:"\f38f"}.fa-sistrix:before{content:"\f3ee"}.fa-instagram-square:before,.fa-square-instagram:before{content:"\e055"}.fa-battle-net:before{content:"\f835"}.fa-the-red-yeti:before{content:"\f69d"}.fa-hacker-news-square:before,.fa-square-hacker-news:before{content:"\f3af"}.fa-edge:before{content:"\f282"}.fa-napster:before{content:"\f3d2"}.fa-snapchat-square:before,.fa-square-snapchat:before{content:"\f2ad"}.fa-google-plus-g:before{content:"\f0d5"}.fa-artstation:before{content:"\f77a"}.fa-markdown:before{content:"\f60f"}.fa-sourcetree:before{content:"\f7d3"}.fa-google-plus:before{content:"\f2b3"}.fa-diaspora:before{content:"\f791"}.fa-foursquare:before{content:"\f180"}.fa-stack-overflow:before{content:"\f16c"}.fa-github-alt:before{content:"\f113"}.fa-phoenix-squadron:before{content:"\f511"}.fa-pagelines:before{content:"\f18c"}.fa-algolia:before{content:"\f36c"}.fa-red-river:before{content:"\f3e3"}.fa-creative-commons-sa:before{content:"\f4ef"}.fa-safari:before{content:"\f267"}.fa-google:before{content:"\f1a0"}.fa-font-awesome-alt:before,.fa-square-font-awesome-stroke:before{content:"\f35c"}.fa-atlassian:before{content:"\f77b"}.fa-linkedin-in:before{content:"\f0e1"}.fa-digital-ocean:before{content:"\f391"}.fa-nimblr:before{content:"\f5a8"}.fa-chromecast:before{content:"\f838"}.fa-evernote:before{content:"\f839"}.fa-hacker-news:before{content:"\f1d4"}.fa-creative-commons-sampling:before{content:"\f4f0"}.fa-adversal:before{content:"\f36a"}.fa-creative-commons:before{content:"\f25e"}.fa-watchman-monitoring:before{content:"\e087"}.fa-fonticons:before{content:"\f280"}.fa-weixin:before{content:"\f1d7"}.fa-shirtsinbulk:before{content:"\f214"}.fa-codepen:before{content:"\f1cb"}.fa-git-alt:before{content:"\f841"}.fa-lyft:before{content:"\f3c3"}.fa-rev:before{content:"\f5b2"}.fa-windows:before{content:"\f17a"}.fa-wizards-of-the-coast:before{content:"\f730"}.fa-square-viadeo:before,.fa-viadeo-square:before{content:"\f2aa"}.fa-meetup:before{content:"\f2e0"}.fa-centos:before{content:"\f789"}.fa-adn:before{content:"\f170"}.fa-cloudsmith:before{content:"\f384"}.fa-pied-piper-alt:before{content:"\f1a8"}.fa-dribbble-square:before,.fa-square-dribbble:before{content:"\f397"}.fa-codiepie:before{content:"\f284"}.fa-node:before{content:"\f419"}.fa-mix:before{content:"\f3cb"}.fa-steam:before{content:"\f1b6"}.fa-cc-apple-pay:before{content:"\f416"}.fa-scribd:before{content:"\f28a"}.fa-openid:before{content:"\f19b"}.fa-instalod:before{content:"\e081"}.fa-expeditedssl:before{content:"\f23e"}.fa-sellcast:before{content:"\f2da"}.fa-square-twitter:before,.fa-twitter-square:before{content:"\f081"}.fa-r-project:before{content:"\f4f7"}.fa-delicious:before{content:"\f1a5"}.fa-freebsd:before{content:"\f3a4"}.fa-vuejs:before{content:"\f41f"}.fa-accusoft:before{content:"\f369"}.fa-ioxhost:before{content:"\f208"}.fa-fonticons-fi:before{content:"\f3a2"}.fa-app-store:before{content:"\f36f"}.fa-cc-mastercard:before{content:"\f1f1"}.fa-itunes-note:before{content:"\f3b5"}.fa-golang:before{content:"\e40f"}.fa-kickstarter:before{content:"\f3bb"}.fa-grav:before{content:"\f2d6"}.fa-weibo:before{content:"\f18a"}.fa-uncharted:before{content:"\e084"}.fa-firstdraft:before{content:"\f3a1"}.fa-square-youtube:before,.fa-youtube-square:before{content:"\f431"}.fa-wikipedia-w:before{content:"\f266"}.fa-rendact:before,.fa-wpressr:before{content:"\f3e4"}.fa-angellist:before{content:"\f209"}.fa-galactic-republic:before{content:"\f50c"}.fa-nfc-directional:before{content:"\e530"}.fa-skype:before{content:"\f17e"}.fa-joget:before{content:"\f3b7"}.fa-fedora:before{content:"\f798"}.fa-stripe-s:before{content:"\f42a"}.fa-meta:before{content:"\e49b"}.fa-laravel:before{content:"\f3bd"}.fa-hotjar:before{content:"\f3b1"}.fa-bluetooth-b:before{content:"\f294"}.fa-sticker-mule:before{content:"\f3f7"}.fa-creative-commons-zero:before{content:"\f4f3"}.fa-hips:before{content:"\f452"}.fa-behance:before{content:"\f1b4"}.fa-reddit:before{content:"\f1a1"}.fa-discord:before{content:"\f392"}.fa-chrome:before{content:"\f268"}.fa-app-store-ios:before{content:"\f370"}.fa-cc-discover:before{content:"\f1f2"}.fa-wpbeginner:before{content:"\f297"}.fa-confluence:before{content:"\f78d"}.fa-mdb:before{content:"\f8ca"}.fa-dochub:before{content:"\f394"}.fa-accessible-icon:before{content:"\f368"}.fa-ebay:before{content:"\f4f4"}.fa-amazon:before{content:"\f270"}.fa-unsplash:before{content:"\e07c"}.fa-yarn:before{content:"\f7e3"}.fa-square-steam:before,.fa-steam-square:before{content:"\f1b7"}.fa-500px:before{content:"\f26e"}.fa-square-vimeo:before,.fa-vimeo-square:before{content:"\f194"}.fa-asymmetrik:before{content:"\f372"}.fa-font-awesome-flag:before,.fa-font-awesome-logo-full:before,.fa-font-awesome:before{content:"\f2b4"}.fa-gratipay:before{content:"\f184"}.fa-apple:before{content:"\f179"}.fa-hive:before{content:"\e07f"}.fa-gitkraken:before{content:"\f3a6"}.fa-keybase:before{content:"\f4f5"}.fa-apple-pay:before{content:"\f415"}.fa-padlet:before{content:"\e4a0"}.fa-amazon-pay:before{content:"\f42c"}.fa-github-square:before,.fa-square-github:before{content:"\f092"}.fa-stumbleupon:before{content:"\f1a4"}.fa-fedex:before{content:"\f797"}.fa-phoenix-framework:before{content:"\f3dc"}.fa-shopify:before{content:"\e057"}.fa-neos:before{content:"\f612"}.fa-hackerrank:before{content:"\f5f7"}.fa-researchgate:before{content:"\f4f8"}.fa-swift:before{content:"\f8e1"}.fa-angular:before{content:"\f420"}.fa-speakap:before{content:"\f3f3"}.fa-angrycreative:before{content:"\f36e"}.fa-y-combinator:before{content:"\f23b"}.fa-empire:before{content:"\f1d1"}.fa-envira:before{content:"\f299"}.fa-gitlab-square:before,.fa-square-gitlab:before{content:"\e5ae"}.fa-studiovinari:before{content:"\f3f8"}.fa-pied-piper:before{content:"\f2ae"}.fa-wordpress:before{content:"\f19a"}.fa-product-hunt:before{content:"\f288"}.fa-firefox:before{content:"\f269"}.fa-linode:before{content:"\f2b8"}.fa-goodreads:before{content:"\f3a8"}.fa-odnoklassniki-square:before,.fa-square-odnoklassniki:before{content:"\f264"}.fa-jsfiddle:before{content:"\f1cc"}.fa-sith:before{content:"\f512"}.fa-themeisle:before{content:"\f2b2"}.fa-page4:before{content:"\f3d7"}.fa-hashnode:before{content:"\e499"}.fa-react:before{content:"\f41b"}.fa-cc-paypal:before{content:"\f1f4"}.fa-squarespace:before{content:"\f5be"}.fa-cc-stripe:before{content:"\f1f5"}.fa-creative-commons-share:before{content:"\f4f2"}.fa-bitcoin:before{content:"\f379"}.fa-keycdn:before{content:"\f3ba"}.fa-opera:before{content:"\f26a"}.fa-itch-io:before{content:"\f83a"}.fa-umbraco:before{content:"\f8e8"}.fa-galactic-senate:before{content:"\f50d"}.fa-ubuntu:before{content:"\f7df"}.fa-draft2digital:before{content:"\f396"}.fa-stripe:before{content:"\f429"}.fa-houzz:before{content:"\f27c"}.fa-gg:before{content:"\f260"}.fa-dhl:before{content:"\f790"}.fa-pinterest-square:before,.fa-square-pinterest:before{content:"\f0d3"}.fa-xing:before{content:"\f168"}.fa-blackberry:before{content:"\f37b"}.fa-creative-commons-pd:before{content:"\f4ec"}.fa-playstation:before{content:"\f3df"}.fa-quinscape:before{content:"\f459"}.fa-less:before{content:"\f41d"}.fa-blogger-b:before{content:"\f37d"}.fa-opencart:before{content:"\f23d"}.fa-vine:before{content:"\f1ca"}.fa-paypal:before{content:"\f1ed"}.fa-gitlab:before{content:"\f296"}.fa-typo3:before{content:"\f42b"}.fa-reddit-alien:before{content:"\f281"}.fa-yahoo:before{content:"\f19e"}.fa-dailymotion:before{content:"\e052"}.fa-affiliatetheme:before{content:"\f36b"}.fa-pied-piper-pp:before{content:"\f1a7"}.fa-bootstrap:before{content:"\f836"}.fa-odnoklassniki:before{content:"\f263"}.fa-nfc-symbol:before{content:"\e531"}.fa-ethereum:before{content:"\f42e"}.fa-speaker-deck:before{content:"\f83c"}.fa-creative-commons-nc-eu:before{content:"\f4e9"}.fa-patreon:before{content:"\f3d9"}.fa-avianex:before{content:"\f374"}.fa-ello:before{content:"\f5f1"}.fa-gofore:before{content:"\f3a7"}.fa-bimobject:before{content:"\f378"}.fa-facebook-f:before{content:"\f39e"}.fa-google-plus-square:before,.fa-square-google-plus:before{content:"\f0d4"}.fa-mandalorian:before{content:"\f50f"}.fa-first-order-alt:before{content:"\f50a"}.fa-osi:before{content:"\f41a"}.fa-google-wallet:before{content:"\f1ee"}.fa-d-and-d-beyond:before{content:"\f6ca"}.fa-periscope:before{content:"\f3da"}.fa-fulcrum:before{content:"\f50b"}.fa-cloudscale:before{content:"\f383"}.fa-forumbee:before{content:"\f211"}.fa-mizuni:before{content:"\f3cc"}.fa-schlix:before{content:"\f3ea"}.fa-square-xing:before,.fa-xing-square:before{content:"\f169"}.fa-bandcamp:before{content:"\f2d5"}.fa-wpforms:before{content:"\f298"}.fa-cloudversify:before{content:"\f385"}.fa-usps:before{content:"\f7e1"}.fa-megaport:before{content:"\f5a3"}.fa-magento:before{content:"\f3c4"}.fa-spotify:before{content:"\f1bc"}.fa-optin-monster:before{content:"\f23c"}.fa-fly:before{content:"\f417"}.fa-aviato:before{content:"\f421"}.fa-itunes:before{content:"\f3b4"}.fa-cuttlefish:before{content:"\f38c"}.fa-blogger:before{content:"\f37c"}.fa-flickr:before{content:"\f16e"}.fa-viber:before{content:"\f409"}.fa-soundcloud:before{content:"\f1be"}.fa-digg:before{content:"\f1a6"}.fa-tencent-weibo:before{content:"\f1d5"}.fa-symfony:before{content:"\f83d"}.fa-maxcdn:before{content:"\f136"}.fa-etsy:before{content:"\f2d7"}.fa-facebook-messenger:before{content:"\f39f"}.fa-audible:before{content:"\f373"}.fa-think-peaks:before{content:"\f731"}.fa-bilibili:before{content:"\e3d9"}.fa-erlang:before{content:"\f39d"}.fa-cotton-bureau:before{content:"\f89e"}.fa-dashcube:before{content:"\f210"}.fa-42-group:before,.fa-innosoft:before{content:"\e080"}.fa-stack-exchange:before{content:"\f18d"}.fa-elementor:before{content:"\f430"}.fa-pied-piper-square:before,.fa-square-pied-piper:before{content:"\e01e"}.fa-creative-commons-nd:before{content:"\f4eb"}.fa-palfed:before{content:"\f3d8"}.fa-superpowers:before{content:"\f2dd"}.fa-resolving:before{content:"\f3e7"}.fa-xbox:before{content:"\f412"}.fa-searchengin:before{content:"\f3eb"}.fa-tiktok:before{content:"\e07b"}.fa-facebook-square:before,.fa-square-facebook:before{content:"\f082"}.fa-renren:before{content:"\f18b"}.fa-linux:before{content:"\f17c"}.fa-glide:before{content:"\f2a5"}.fa-linkedin:before{content:"\f08c"}.fa-hubspot:before{content:"\f3b2"}.fa-deploydog:before{content:"\f38e"}.fa-twitch:before{content:"\f1e8"}.fa-ravelry:before{content:"\f2d9"}.fa-mixer:before{content:"\e056"}.fa-lastfm-square:before,.fa-square-lastfm:before{content:"\f203"}.fa-vimeo:before{content:"\f40a"}.fa-mendeley:before{content:"\f7b3"}.fa-uniregistry:before{content:"\f404"}.fa-figma:before{content:"\f799"}.fa-creative-commons-remix:before{content:"\f4ee"}.fa-cc-amazon-pay:before{content:"\f42d"}.fa-dropbox:before{content:"\f16b"}.fa-instagram:before{content:"\f16d"}.fa-cmplid:before{content:"\e360"}.fa-facebook:before{content:"\f09a"}.fa-gripfire:before{content:"\f3ac"}.fa-jedi-order:before{content:"\f50e"}.fa-uikit:before{content:"\f403"}.fa-fort-awesome-alt:before{content:"\f3a3"}.fa-phabricator:before{content:"\f3db"}.fa-ussunnah:before{content:"\f407"}.fa-earlybirds:before{content:"\f39a"}.fa-trade-federation:before{content:"\f513"}.fa-autoprefixer:before{content:"\f41c"}.fa-whatsapp:before{content:"\f232"}.fa-slideshare:before{content:"\f1e7"}.fa-google-play:before{content:"\f3ab"}.fa-viadeo:before{content:"\f2a9"}.fa-line:before{content:"\f3c0"}.fa-google-drive:before{content:"\f3aa"}.fa-servicestack:before{content:"\f3ec"}.fa-simplybuilt:before{content:"\f215"}.fa-bitbucket:before{content:"\f171"}.fa-imdb:before{content:"\f2d8"}.fa-deezer:before{content:"\e077"}.fa-raspberry-pi:before{content:"\f7bb"}.fa-jira:before{content:"\f7b1"}.fa-docker:before{content:"\f395"}.fa-screenpal:before{content:"\e570"}.fa-bluetooth:before{content:"\f293"}.fa-gitter:before{content:"\f426"}.fa-d-and-d:before{content:"\f38d"}.fa-microblog:before{content:"\e01a"}.fa-cc-diners-club:before{content:"\f24c"}.fa-gg-circle:before{content:"\f261"}.fa-pied-piper-hat:before{content:"\f4e5"}.fa-kickstarter-k:before{content:"\f3bc"}.fa-yandex:before{content:"\f413"}.fa-readme:before{content:"\f4d5"}.fa-html5:before{content:"\f13b"}.fa-sellsy:before{content:"\f213"}.fa-sass:before{content:"\f41e"}.fa-wirsindhandwerk:before,.fa-wsh:before{content:"\e2d0"}.fa-buromobelexperte:before{content:"\f37f"}.fa-salesforce:before{content:"\f83b"}.fa-octopus-deploy:before{content:"\e082"}.fa-medapps:before{content:"\f3c6"}.fa-ns8:before{content:"\f3d5"}.fa-pinterest-p:before{content:"\f231"}.fa-apper:before{content:"\f371"}.fa-fort-awesome:before{content:"\f286"}.fa-waze:before{content:"\f83f"}.fa-cc-jcb:before{content:"\f24b"}.fa-snapchat-ghost:before,.fa-snapchat:before{content:"\f2ab"}.fa-fantasy-flight-games:before{content:"\f6dc"}.fa-rust:before{content:"\e07a"}.fa-wix:before{content:"\f5cf"}.fa-behance-square:before,.fa-square-behance:before{content:"\f1b5"}.fa-supple:before{content:"\f3f9"}.fa-rebel:before{content:"\f1d0"}.fa-css3:before{content:"\f13c"}.fa-staylinked:before{content:"\f3f5"}.fa-kaggle:before{content:"\f5fa"}.fa-space-awesome:before{content:"\e5ac"}.fa-deviantart:before{content:"\f1bd"}.fa-cpanel:before{content:"\f388"}.fa-goodreads-g:before{content:"\f3a9"}.fa-git-square:before,.fa-square-git:before{content:"\f1d2"}.fa-square-tumblr:before,.fa-tumblr-square:before{content:"\f174"}.fa-trello:before{content:"\f181"}.fa-creative-commons-nc-jp:before{content:"\f4ea"}.fa-get-pocket:before{content:"\f265"}.fa-perbyte:before{content:"\e083"}.fa-grunt:before{content:"\f3ad"}.fa-weebly:before{content:"\f5cc"}.fa-connectdevelop:before{content:"\f20e"}.fa-leanpub:before{content:"\f212"}.fa-black-tie:before{content:"\f27e"}.fa-themeco:before{content:"\f5c6"}.fa-python:before{content:"\f3e2"}.fa-android:before{content:"\f17b"}.fa-bots:before{content:"\e340"}.fa-free-code-camp:before{content:"\f2c5"}.fa-hornbill:before{content:"\f592"}.fa-js:before{content:"\f3b8"}.fa-ideal:before{content:"\e013"}.fa-git:before{content:"\f1d3"}.fa-dev:before{content:"\f6cc"}.fa-sketch:before{content:"\f7c6"}.fa-yandex-international:before{content:"\f414"}.fa-cc-amex:before{content:"\f1f3"}.fa-uber:before{content:"\f402"}.fa-github:before{content:"\f09b"}.fa-php:before{content:"\f457"}.fa-alipay:before{content:"\f642"}.fa-youtube:before{content:"\f167"}.fa-skyatlas:before{content:"\f216"}.fa-firefox-browser:before{content:"\e007"}.fa-replyd:before{content:"\f3e6"}.fa-suse:before{content:"\f7d6"}.fa-jenkins:before{content:"\f3b6"}.fa-twitter:before{content:"\f099"}.fa-rockrms:before{content:"\f3e9"}.fa-pinterest:before{content:"\f0d2"}.fa-buffer:before{content:"\f837"}.fa-npm:before{content:"\f3d4"}.fa-yammer:before{content:"\f840"}.fa-btc:before{content:"\f15a"}.fa-dribbble:before{content:"\f17d"}.fa-stumbleupon-circle:before{content:"\f1a3"}.fa-internet-explorer:before{content:"\f26b"}.fa-telegram-plane:before,.fa-telegram:before{content:"\f2c6"}.fa-old-republic:before{content:"\f510"}.fa-square-whatsapp:before,.fa-whatsapp-square:before{content:"\f40c"}.fa-node-js:before{content:"\f3d3"}.fa-edge-legacy:before{content:"\e078"}.fa-slack-hash:before,.fa-slack:before{content:"\f198"}.fa-medrt:before{content:"\f3c8"}.fa-usb:before{content:"\f287"}.fa-tumblr:before{content:"\f173"}.fa-vaadin:before{content:"\f408"}.fa-quora:before{content:"\f2c4"}.fa-reacteurope:before{content:"\f75d"}.fa-medium-m:before,.fa-medium:before{content:"\f23a"}.fa-amilia:before{content:"\f36d"}.fa-mixcloud:before{content:"\f289"}.fa-flipboard:before{content:"\f44d"}.fa-viacoin:before{content:"\f237"}.fa-critical-role:before{content:"\f6c9"}.fa-sitrox:before{content:"\e44a"}.fa-discourse:before{content:"\f393"}.fa-joomla:before{content:"\f1aa"}.fa-mastodon:before{content:"\f4f6"}.fa-airbnb:before{content:"\f834"}.fa-wolf-pack-battalion:before{content:"\f514"}.fa-buy-n-large:before{content:"\f8a6"}.fa-gulp:before{content:"\f3ae"}.fa-creative-commons-sampling-plus:before{content:"\f4f1"}.fa-strava:before{content:"\f428"}.fa-ember:before{content:"\f423"}.fa-canadian-maple-leaf:before{content:"\f785"}.fa-teamspeak:before{content:"\f4f9"}.fa-pushed:before{content:"\f3e1"}.fa-wordpress-simple:before{content:"\f411"}.fa-nutritionix:before{content:"\f3d6"}.fa-wodu:before{content:"\e088"}.fa-google-pay:before{content:"\e079"}.fa-intercom:before{content:"\f7af"}.fa-zhihu:before{content:"\f63f"}.fa-korvue:before{content:"\f42f"}.fa-pix:before{content:"\e43a"}.fa-steam-symbol:before{content:"\f3f6"}:host,:root{--fa-font-regular:normal 400 1em/1 "Font Awesome 6 Free"}@font-face{font-family:"Font Awesome 6 Free";font-style:normal;font-weight:400;font-display:block;src:url(../webfonts/fa-regular-400.woff2) format("woff2"),url(../webfonts/fa-regular-400.ttf) format("truetype")}.fa-regular,.far{font-weight:400}:host,:root{--fa-style-family-classic:"Font Awesome 6 Free";--fa-font-solid:normal 900 1em/1 "Font Awesome 6 Free"}@font-face{font-family:"Font Awesome 6 Free";font-style:normal;font-weight:900;font-display:block;src:url(../webfonts/fa-solid-900.woff2) format("woff2"),url(../webfonts/fa-solid-900.ttf) format("truetype")}.fa-solid,.fas{font-weight:900}@font-face{font-family:"Font Awesome 5 Brands";font-display:block;font-weight:400;src:url(../webfonts/fa-brands-400.woff2) format("woff2"),url(../webfonts/fa-brands-400.ttf) format("truetype")}@font-face{font-family:"Font Awesome 5 Free";font-display:block;font-weight:900;src:url(../webfonts/fa-solid-900.woff2) format("woff2"),url(../webfonts/fa-solid-900.ttf) format("truetype")}@font-face{font-family:"Font Awesome 5 Free";font-display:block;font-weight:400;src:url(../webfonts/fa-regular-400.woff2) format("woff2"),url(../webfonts/fa-regular-400.ttf) format("truetype")}@font-face{font-family:"FontAwesome";font-display:block;src:url(../webfonts/fa-solid-900.woff2) format("woff2"),url(../webfonts/fa-solid-900.ttf) format("truetype")}@font-face{font-family:"FontAwesome";font-display:block;src:url(../webfonts/fa-brands-400.woff2) format("woff2"),url(../webfonts/fa-brands-400.ttf) format("truetype")}@font-face{font-family:"FontAwesome";font-display:block;src:url(../webfonts/fa-regular-400.woff2) format("woff2"),url(../webfonts/fa-regular-400.ttf) format("truetype");unicode-range:u+f003,u+f006,u+f014,u+f016-f017,u+f01a-f01b,u+f01d,u+f022,u+f03e,u+f044,u+f046,u+f05c-f05d,u+f06e,u+f070,u+f087-f088,u+f08a,u+f094,u+f096-f097,u+f09d,u+f0a0,u+f0a2,u+f0a4-f0a7,u+f0c5,u+f0c7,u+f0e5-f0e6,u+f0eb,u+f0f6-f0f8,u+f10c,u+f114-f115,u+f118-f11a,u+f11c-f11d,u+f133,u+f147,u+f14e,u+f150-f152,u+f185-f186,u+f18e,u+f190-f192,u+f196,u+f1c1-f1c9,u+f1d9,u+f1db,u+f1e3,u+f1ea,u+f1f7,u+f1f9,u+f20a,u+f247-f248,u+f24a,u+f24d,u+f255-f25b,u+f25d,u+f271-f274,u+f278,u+f27b,u+f28c,u+f28e,u+f29c,u+f2b5,u+f2b7,u+f2ba,u+f2bc,u+f2be,u+f2c0-f2c1,u+f2c3,u+f2d0,u+f2d2,u+f2d4,u+f2dc}@font-face{font-family:"FontAwesome";font-display:block;src:url(../webfonts/fa-v4compatibility.woff2) format("woff2"),url(../webfonts/fa-v4compatibility.ttf) format("truetype");unicode-range:u+f041,u+f047,u+f065-f066,u+f07d-f07e,u+f080,u+f08b,u+f08e,u+f090,u+f09a,u+f0ac,u+f0ae,u+f0b2,u+f0d0,u+f0d6,u+f0e4,u+f0ec,u+f10a-f10b,u+f123,u+f13e,u+f148-f149,u+f14c,u+f156,u+f15e,u+f160-f161,u+f163,u+f175-f178,u+f195,u+f1f8,u+f219,u+f27a}
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/hugo-theme.css` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/hugo-theme.css`

 * *Files 1% similar despite different names*

```diff
@@ -233,9 +233,9 @@
 @media only all and (max-width: 47.938em) {
   #breadcrumbs .links, #top-github-link-text {
       display: none;
   }
 }
 
 .is-sticky #top-bar {
-  box-shadow: -1px 2px 5px 1px rgba(0, 0, 0, 0.1); 
-}
+  box-shadow: -1px 2px 5px 1px rgba(0, 0, 0, 0.1);
+}
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/hybrid.css` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/hybrid.css`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/nucleus.css` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/nucleus.css`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/perfect-scrollbar.min.css` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/perfect-scrollbar.min.css`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/tabs.css` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/tabs.css`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/tags.css` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/tags.css`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 /* Tags */
 
 #head-tags{
-    margin-left:1em;  
+    margin-left:1em;
     margin-top:1em;
 }
-  
+
 #body .tags a.tag-link {
     display: inline-block;
     line-height: 2em;
     font-size: 0.8em;
     position: relative;
     margin: 0 16px 8px 0;
     padding: 0 10px 0 12px;
-    background: #8451a1;    
-    
-    -webkit-border-bottom-right-radius: 3px;    
+    background: #8451a1;
+
+    -webkit-border-bottom-right-radius: 3px;
     border-bottom-right-radius: 3px;
-    -webkit-border-top-right-radius: 3px;    
+    -webkit-border-top-right-radius: 3px;
     border-top-right-radius: 3px;
 
     -webkit-box-shadow: 0 1px 2px rgba(0,0,0,0.2);
     box-shadow: 0 1px 2px rgba(0,0,0,0.2);
     color: #fff;
 }
-  
+
 #body .tags a.tag-link:before {
     content: "";
     position: absolute;
     top:0;
     left: -1em;
     width: 0;
     height: 0;
     border-color: transparent #8451a1 transparent transparent;
     border-style: solid;
-    border-width: 1em 1em 1em 0;        
+    border-width: 1em 1em 1em 0;
 }
-  
+
 #body .tags a.tag-link:after {
     content: "";
     position: absolute;
     top: 10px;
     left: 1px;
     width: 5px;
     height: 5px;
     -webkit-border-radius: 50%;
     border-radius: 100%;
-    background: #fff;    
+    background: #fff;
 }
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/theme-blue.css` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/theme-blue.css`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -121,8 +121,8 @@
 
 #homelinks a {
   color: var(--MENU-HOME-LINK-color);
 }
 
 #homelinks a:hover {
   color: var(--MENU-HOME-LINK-HOVERED-color);
-}
+}
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/theme-green.css` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/theme-green.css`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -121,8 +121,8 @@
 
 #homelinks a {
   color: var(--MENU-HOME-LINK-color);
 }
 
 #homelinks a:hover {
   color: var(--MENU-HOME-LINK-HOVERED-color);
-}
+}
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/theme-red.css` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/theme-red.css`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -121,8 +121,8 @@
 
 #homelinks a {
   color: var(--MENU-HOME-LINK-color);
 }
 
 #homelinks a:hover {
   color: var(--MENU-HOME-LINK-HOVERED-color);
-}
+}
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/css/theme.css` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/css/theme.css`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.eot` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.eot`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.svg` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.svg`

 * *Files 0% similar despite different names*

```diff
@@ -3868,8 +3868,8 @@
 0000f1b0: 3031 4c32 3733 2032 3431 4c31 3532 2033  01L273 241L152 3
 0000f1c0: 3539 4c31 3931 2034 3030 4c33 3433 2032  59L191 400L343 2
 0000f1d0: 3533 5a22 2067 6c79 7068 2d6e 616d 653d  53Z" glyph-name=
 0000f1e0: 2267 7569 6c73 696e 676c 7269 6768 7422  "guilsinglright"
 0000f1f0: 2068 6f72 697a 2d61 6476 2d78 3d22 3530   horiz-adv-x="50
 0000f200: 3022 2075 6e69 636f 6465 3d22 e280 ba22  0" unicode="..."
 0000f210: 2f3e 3c2f 666f 6e74 3e3c 2f64 6566 733e  /></font></defs>
-0000f220: 3c2f 7376 673e                           </svg>
+0000f220: 3c2f 7376 673e 0a                        </svg>.
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.ttf` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.ttf`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.woff` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Inconsolata.woff`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.eot` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.eot`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.svg` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.svg`

 * *Files 0% similar despite different names*

```diff
@@ -6157,8 +6157,8 @@
 000180c0: 2271 756f 7465 6462 6c2c 7175 6f74 6573  "quotedbl,quotes
 000180d0: 696e 676c 652c 7175 6f74 656c 6566 742c  ingle,quoteleft,
 000180e0: 7175 6f74 6572 6967 6874 2c71 756f 7465  quoteright,quote
 000180f0: 6462 6c6c 6566 742c 7175 6f74 6564 626c  dblleft,quotedbl
 00018100: 7269 6768 7422 2067 323d 2264 6f6c 6c61  right" g2="dolla
 00018110: 722c 7322 206b 3d22 3530 222f 3e3c 2f66  r,s" k="50"/></f
 00018120: 6f6e 743e 3c2f 6465 6673 3e3c 2f73 7667  ont></defs></svg
-00018130: 3e                                       >
+00018130: 3e0a                                     >.
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.ttf` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.ttf`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.woff` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.woff`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.woff2` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-Normal-webfont.woff2`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.eot` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.eot`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.svg` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.svg`

 * *Files 0% similar despite different names*

```diff
@@ -5742,7 +5742,8 @@
 000166d0: 7175 6f74 6564 626c 2c71 756f 7465 7369  quotedbl,quotesi
 000166e0: 6e67 6c65 2c71 756f 7465 6c65 6674 2c71  ngle,quoteleft,q
 000166f0: 756f 7465 7269 6768 742c 7175 6f74 6564  uoteright,quoted
 00016700: 626c 6c65 6674 2c71 756f 7465 6462 6c72  blleft,quotedblr
 00016710: 6967 6874 2220 6732 3d22 646f 6c6c 6172  ight" g2="dollar
 00016720: 2c73 2220 6b3d 2235 3022 2f3e 3c2f 666f  ,s" k="50"/></fo
 00016730: 6e74 3e3c 2f64 6566 733e 3c2f 7376 673e  nt></defs></svg>
+00016740: 0a                                       .
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.ttf` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.ttf`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.woff` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.woff`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.woff2` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Novecentosanswide-UltraLight-webfont.woff2`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.eot` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.eot`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.svg` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.svg`

 * *Files 0% similar despite different names*

```diff
@@ -3421,8 +3421,8 @@
 0000d5c0: 3232 3420 3236 354c 3834 2036 3948 3530  224 265L84 69H50
 0000d5d0: 4c31 3932 2032 3635 4c35 3020 3436 3148  L192 265L50 461H
 0000d5e0: 3834 5a22 2067 6c79 7068 2d6e 616d 653d  84Z" glyph-name=
 0000d5f0: 2267 7569 6c73 696e 676c 7269 6768 7422  "guilsinglright"
 0000d600: 2068 6f72 697a 2d61 6476 2d78 3d22 3237   horiz-adv-x="27
 0000d610: 3122 2075 6e69 636f 6465 3d22 e280 ba22  1" unicode="..."
 0000d620: 2f3e 3c2f 666f 6e74 3e3c 2f64 6566 733e  /></font></defs>
-0000d630: 3c2f 7376 673e                           </svg>
+0000d630: 3c2f 7376 673e 0a                        </svg>.
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.ttf` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.ttf`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.woff` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.woff`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.woff2` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_200.woff2`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.eot` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.eot`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.svg` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.svg`

 * *Files 0% similar despite different names*

```diff
@@ -3418,8 +3418,8 @@
 0000d590: 354c 3130 3720 3639 4835 314c 3138 3720  5L107 69H51L187 
 0000d5a0: 3236 354c 3531 2034 3631 4831 3037 5a22  265L51 461H107Z"
 0000d5b0: 2067 6c79 7068 2d6e 616d 653d 2267 7569   glyph-name="gui
 0000d5c0: 6c73 696e 676c 7269 6768 7422 2068 6f72  lsinglright" hor
 0000d5d0: 697a 2d61 6476 2d78 3d22 3239 3022 2075  iz-adv-x="290" u
 0000d5e0: 6e69 636f 6465 3d22 e280 ba22 2f3e 3c2f  nicode="..."/></
 0000d5f0: 666f 6e74 3e3c 2f64 6566 733e 3c2f 7376  font></defs></sv
-0000d600: 673e                                     g>
+0000d600: 673e 0a                                  g>.
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.ttf` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.ttf`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.woff` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.woff`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.woff2` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_300.woff2`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.eot` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.eot`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.svg` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.svg`

 * *Files 0% similar despite different names*

```diff
@@ -3395,8 +3395,8 @@
 0000d420: 2032 3635 4c31 3532 2036 3948 3437 4c31   265L152 69H47L1
 0000d430: 3733 2032 3635 4c34 3720 3436 3148 3135  73 265L47 461H15
 0000d440: 325a 2220 676c 7970 682d 6e61 6d65 3d22  2Z" glyph-name="
 0000d450: 6775 696c 7369 6e67 6c72 6967 6874 2220  guilsinglright" 
 0000d460: 686f 7269 7a2d 6164 762d 783d 2233 3234  horiz-adv-x="324
 0000d470: 2220 756e 6963 6f64 653d 22e2 80ba 222f  " unicode="..."/
 0000d480: 3e3c 2f66 6f6e 743e 3c2f 6465 6673 3e3c  ></font></defs><
-0000d490: 2f73 7667 3e                             /svg>
+0000d490: 2f73 7667 3e0a                           /svg>.
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.ttf` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.ttf`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.woff` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.woff`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.woff2` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/fonts/Work_Sans_500.woff2`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/images/favicon.png` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/images/favicon.png`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/images/gopher-404.jpg` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/images/gopher-404.jpg`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/auto-complete.js` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/auto-complete.js`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/clipboard.min.js` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/clipboard.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 /*!
  * clipboard.js v2.0.4
  * https://zenorocha.github.io/clipboard.js
- * 
+ *
  * Licensed MIT © Zeno Rocha
  */
 ! function(t, e) {
     "object" == typeof exports && "object" == typeof module ? module.exports = e() : "function" == typeof define && define.amd ? define([], e) : "object" == typeof exports ? exports.ClipboardJS = e() : t.ClipboardJS = e()
 }(this, function() {
     return function(n) {
         var o = {};
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/featherlight.min.js` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/featherlight.min.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, Unicode text, UTF-8 text, with very long lines (9024)*

 * *Files 0% similar despite different names*

```diff
@@ -574,8 +574,8 @@
 000023d0: 7374 616e 6365 6f66 2063 2929 7b76 6172  stanceof c)){var
 000023e0: 206e 3d6e 6577 2063 2865 2c74 293b 7265   n=new c(e,t);re
 000023f0: 7475 726e 206e 2e6f 7065 6e28 292c 6e7d  turn n.open(),n}
 00002400: 7468 6973 2e69 643d 632e 6964 2b2b 2c74  this.id=c.id++,t
 00002410: 6869 732e 7365 7475 7028 652c 7429 2c74  his.setup(e,t),t
 00002420: 6869 732e 6368 6169 6e43 616c 6c62 6163  his.chainCallbac
 00002430: 6b73 2863 2e5f 6361 6c6c 6261 636b 4368  ks(c._callbackCh
-00002440: 6169 6e29 7d7d 286a 5175 6572 7929 3b    ain)}}(jQuery);
+00002440: 6169 6e29 7d7d 286a 5175 6572 7929 3b0a  ain)}}(jQuery);.
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/highlight.pack.js` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/highlight.pack.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff.*

 * *Files 0% similar despite different names*

```diff
@@ -5953,8 +5953,8 @@
 00017400: 6177 4465 6669 6e69 7469 6f6e 2829 3b72  awDefinition();r
 00017410: 6574 7572 6e20 742e 6469 7361 626c 6541  eturn t.disableA
 00017420: 7574 6f64 6574 6563 743d 2131 2c74 2e6e  utodetect=!1,t.n
 00017430: 616d 653d 2243 2b2b 222c 742e 616c 6961  ame="C++",t.alia
 00017440: 7365 733d 5b22 6363 222c 2263 2b2b 222c  ses=["cc","c++",
 00017450: 2268 2b2b 222c 2268 7070 222c 2268 6822  "h++","hpp","hh"
 00017460: 2c22 6878 7822 2c22 6378 7822 5d2c 747d  ,"hxx","cxx"],t}
-00017470: 7d28 2929 3b                             }());
+00017470: 7d28 2929 3b0a                           }());.
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/hugo-learn.js` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/hugo-learn.js`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/jquery-3.3.1.min.js` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/jquery.sticky.js` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/jquery.sticky.js`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/learn.js` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/learn.js`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/lunr.min.js` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/lunr.min.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text, with very long lines (29372)*

 * *Files 0% similar despite different names*

```diff
@@ -1839,8 +1839,8 @@
 000072e0: 2829 7b72 6574 7572 6e20 7a7d 2c22 6675  (){return z},"fu
 000072f0: 6e63 7469 6f6e 223d 3d74 7970 656f 6620  nction"==typeof 
 00007300: 6465 6669 6e65 2626 6465 6669 6e65 2e61  define&&define.a
 00007310: 6d64 3f64 6566 696e 6528 7329 3a22 6f62  md?define(s):"ob
 00007320: 6a65 6374 223d 3d74 7970 656f 6620 6578  ject"==typeof ex
 00007330: 706f 7274 733f 6d6f 6475 6c65 2e65 7870  ports?module.exp
 00007340: 6f72 7473 3d73 2829 3a6e 2e6c 756e 723d  orts=s():n.lunr=
-00007350: 7328 297d 2829 3b                        s()}();
+00007350: 7328 297d 2829 3b0a                      s()}();.
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/modernizr.custom-3.6.0.js` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/modernizr.custom-3.6.0.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text, with very long lines (7377)*

 * *Files 0% similar despite different names*

```diff
@@ -465,8 +465,8 @@
 00001d00: 6573 742c 6465 6c65 7465 2045 2e61 6464  est,delete E.add
 00001d10: 4173 796e 6354 6573 743b 666f 7228 7661  AsyncTest;for(va
 00001d20: 7220 463d 303b 463c 4d6f 6465 726e 697a  r F=0;F<Moderniz
 00001d30: 722e 5f71 2e6c 656e 6774 683b 462b 2b29  r._q.length;F++)
 00001d40: 4d6f 6465 726e 697a 722e 5f71 5b46 5d28  Modernizr._q[F](
 00001d50: 293b 652e 4d6f 6465 726e 697a 723d 4d6f  );e.Modernizr=Mo
 00001d60: 6465 726e 697a 727d 2877 696e 646f 772c  dernizr}(window,
-00001d70: 646f 6375 6d65 6e74 293b                 document);
+00001d70: 646f 6375 6d65 6e74 293b 0a              document);.
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/perfect-scrollbar.jquery.min.js` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/perfect-scrollbar.jquery.min.js`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/perfect-scrollbar.min.js` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/perfect-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/js/search.js` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/js/search.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, Unicode text, UTF-8 text*

 * *Files 4% similar despite different names*

```diff
@@ -46,171 +46,171 @@
 000002d0: 7b0a 0909 2020 2020 626f 6f73 743a 2031  {...    boost: 1
 000002e0: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
 000002f0: 2020 7d29 3b0a 2020 2020 2020 2020 2020    });.          
 00000300: 2020 2020 2020 7468 6973 2e66 6965 6c64        this.field
 00000310: 2822 636f 6e74 656e 7422 2c20 7b0a 0909  ("content", {...
 00000320: 2020 2020 626f 6f73 743a 2035 0a20 2020      boost: 5.   
 00000330: 2020 2020 2020 2020 2020 2020 207d 293b               });
-00000340: 0a09 0909 090a 2020 2020 2020 2020 2020  ......          
-00000350: 2020 2020 2020 7468 6973 2e70 6970 656c        this.pipel
-00000360: 696e 652e 7265 6d6f 7665 286c 756e 722e  ine.remove(lunr.
-00000370: 7374 656d 6d65 7229 3b0a 2020 2020 2020  stemmer);.      
-00000380: 2020 2020 2020 2020 2020 7468 6973 2e73            this.s
-00000390: 6561 7263 6850 6970 656c 696e 652e 7265  earchPipeline.re
-000003a0: 6d6f 7665 286c 756e 722e 7374 656d 6d65  move(lunr.stemme
-000003b0: 7229 3b0a 0909 0909 0a20 2020 2020 2020  r);......       
-000003c0: 2020 2020 2020 2020 202f 2f20 4665 6564           // Feed
-000003d0: 206c 756e 7220 7769 7468 2065 6163 6820   lunr with each 
-000003e0: 6669 6c65 2061 6e64 206c 6574 206c 756e  file and let lun
-000003f0: 7220 6163 7475 616c 6c79 2069 6e64 6578  r actually index
-00000400: 2074 6865 6d0a 2020 2020 2020 2020 2020   them.          
-00000410: 2020 2020 2020 7061 6765 7349 6e64 6578        pagesIndex
-00000420: 2e66 6f72 4561 6368 2866 756e 6374 696f  .forEach(functio
-00000430: 6e28 7061 6765 2920 7b0a 0909 2020 2020  n(page) {...    
-00000440: 7468 6973 2e61 6464 2870 6167 6529 3b0a  this.add(page);.
-00000450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000460: 7d2c 2074 6869 7329 3b0a 2020 2020 2020  }, this);.      
-00000470: 2020 2020 2020 7d29 0a20 2020 2020 2020        }).       
-00000480: 207d 290a 2020 2020 2020 2020 2e66 6169   }).        .fai
-00000490: 6c28 6675 6e63 7469 6f6e 286a 7178 6872  l(function(jqxhr
-000004a0: 2c20 7465 7874 5374 6174 7573 2c20 6572  , textStatus, er
-000004b0: 726f 7229 207b 0a20 2020 2020 2020 2020  ror) {.         
-000004c0: 2020 2076 6172 2065 7272 203d 2074 6578     var err = tex
-000004d0: 7453 7461 7475 7320 2b20 222c 2022 202b  tStatus + ", " +
-000004e0: 2065 7272 6f72 3b0a 2020 2020 2020 2020   error;.        
-000004f0: 2020 2020 636f 6e73 6f6c 652e 6572 726f      console.erro
-00000500: 7228 2245 7272 6f72 2067 6574 7469 6e67  r("Error getting
-00000510: 2048 7567 6f20 696e 6465 7820 6669 6c65   Hugo index file
-00000520: 3a22 2c20 6572 7229 3b0a 2020 2020 2020  :", err);.      
-00000530: 2020 7d29 3b0a 7d0a 0a2f 2a2a 0a20 2a20    });.}../**. * 
-00000540: 5472 6967 6765 7220 6120 7365 6172 6368  Trigger a search
-00000550: 2069 6e20 6c75 6e72 2061 6e64 2074 7261   in lunr and tra
-00000560: 6e73 666f 726d 2074 6865 2072 6573 756c  nsform the resul
-00000570: 740a 202a 0a20 2a20 4070 6172 616d 2020  t. *. * @param  
-00000580: 7b53 7472 696e 677d 2071 7565 7279 0a20  {String} query. 
-00000590: 2a20 4072 6574 7572 6e20 7b41 7272 6179  * @return {Array
-000005a0: 7d20 2072 6573 756c 7473 0a20 2a2f 0a66  }  results. */.f
-000005b0: 756e 6374 696f 6e20 7365 6172 6368 2871  unction search(q
-000005c0: 7565 7279 5465 726d 2920 7b0a 2020 2020  ueryTerm) {.    
-000005d0: 2f2f 2046 696e 6420 7468 6520 6974 656d  // Find the item
-000005e0: 2069 6e20 6f75 7220 696e 6465 7820 636f   in our index co
-000005f0: 7272 6573 706f 6e64 696e 6720 746f 2074  rresponding to t
-00000600: 6865 206c 756e 7220 6f6e 6520 746f 2068  he lunr one to h
-00000610: 6176 6520 6d6f 7265 2069 6e66 6f0a 2020  ave more info.  
-00000620: 2020 7265 7475 726e 206c 756e 7249 6e64    return lunrInd
-00000630: 6578 2e73 6561 7263 6828 7175 6572 7954  ex.search(queryT
-00000640: 6572 6d2b 225e 3130 3022 2b22 2022 2b71  erm+"^100"+" "+q
-00000650: 7565 7279 5465 726d 2b22 2a5e 3130 222b  ueryTerm+"*^10"+
-00000660: 2220 222b 222a 222b 7175 6572 7954 6572  " "+"*"+queryTer
-00000670: 6d2b 225e 3130 222b 2220 222b 7175 6572  m+"^10"+" "+quer
-00000680: 7954 6572 6d2b 227e 325e 3122 292e 6d61  yTerm+"~2^1").ma
-00000690: 7028 6675 6e63 7469 6f6e 2872 6573 756c  p(function(resul
-000006a0: 7429 207b 0a20 2020 2020 2020 2020 2020  t) {.           
-000006b0: 2072 6574 7572 6e20 7061 6765 7349 6e64   return pagesInd
-000006c0: 6578 2e66 696c 7465 7228 6675 6e63 7469  ex.filter(functi
-000006d0: 6f6e 2870 6167 6529 207b 0a20 2020 2020  on(page) {.     
-000006e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000006f0: 6e20 7061 6765 2e75 7269 203d 3d3d 2072  n page.uri === r
-00000700: 6573 756c 742e 7265 663b 0a20 2020 2020  esult.ref;.     
-00000710: 2020 2020 2020 207d 295b 305d 3b0a 2020         })[0];.  
-00000720: 2020 2020 2020 7d29 3b0a 7d0a 0a2f 2f20        });.}..// 
-00000730: 4c65 7427 7320 6765 7420 7374 6172 7465  Let's get starte
-00000740: 640a 696e 6974 4c75 6e72 2829 3b0a 2428  d.initLunr();.$(
-00000750: 2064 6f63 756d 656e 7420 292e 7265 6164   document ).read
-00000760: 7928 6675 6e63 7469 6f6e 2829 207b 0a20  y(function() {. 
-00000770: 2020 2076 6172 2073 6561 7263 684c 6973     var searchLis
-00000780: 7420 3d20 6e65 7720 6175 746f 436f 6d70  t = new autoComp
-00000790: 6c65 7465 287b 0a20 2020 2020 2020 202f  lete({.        /
-000007a0: 2a20 7365 6c65 6374 6f72 2066 6f72 2074  * selector for t
-000007b0: 6865 2073 6561 7263 6820 626f 7820 656c  he search box el
-000007c0: 656d 656e 7420 2a2f 0a20 2020 2020 2020  ement */.       
-000007d0: 2073 656c 6563 746f 723a 2024 2822 2373   selector: $("#s
-000007e0: 6561 7263 682d 6279 2229 2e67 6574 2830  earch-by").get(0
-000007f0: 292c 0a20 2020 2020 2020 202f 2a20 736f  ),.        /* so
-00000800: 7572 6365 2069 7320 7468 6520 6361 6c6c  urce is the call
-00000810: 6261 636b 2074 6f20 7065 7266 6f72 6d20  back to perform 
-00000820: 7468 6520 7365 6172 6368 202a 2f0a 2020  the search */.  
-00000830: 2020 2020 2020 736f 7572 6365 3a20 6675        source: fu
-00000840: 6e63 7469 6f6e 2874 6572 6d2c 2072 6573  nction(term, res
-00000850: 706f 6e73 6529 207b 0a20 2020 2020 2020  ponse) {.       
-00000860: 2020 2020 2072 6573 706f 6e73 6528 7365       response(se
-00000870: 6172 6368 2874 6572 6d29 293b 0a20 2020  arch(term));.   
-00000880: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00000890: 2f2a 2072 656e 6465 7249 7465 6d20 6469  /* renderItem di
-000008a0: 7370 6c61 7973 2069 6e64 6976 6964 7561  splays individua
-000008b0: 6c20 7365 6172 6368 2072 6573 756c 7473  l search results
-000008c0: 202a 2f0a 2020 2020 2020 2020 7265 6e64   */.        rend
-000008d0: 6572 4974 656d 3a20 6675 6e63 7469 6f6e  erItem: function
-000008e0: 2869 7465 6d2c 2074 6572 6d29 207b 0a20  (item, term) {. 
-000008f0: 2020 2020 2020 2020 2020 2076 6172 206e             var n
-00000900: 756d 436f 6e74 6578 7457 6f72 6473 203d  umContextWords =
-00000910: 2032 3b0a 2020 2020 2020 2020 2020 2020   2;.            
-00000920: 7661 7220 7465 7874 203d 2069 7465 6d2e  var text = item.
-00000930: 636f 6e74 656e 742e 6d61 7463 6828 0a20  content.match(. 
-00000940: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000950: 283f 3a5c 5c73 3f28 3f3a 5b5c 5c77 5d2b  (?:\\s?(?:[\\w]+
-00000960: 295c 5c73 3f29 7b30 2c22 2b6e 756d 436f  )\\s?){0,"+numCo
-00000970: 6e74 6578 7457 6f72 6473 2b22 7d22 202b  ntextWords+"}" +
-00000980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000990: 2020 2020 2074 6572 6d2b 2228 3f3a 5c5c       term+"(?:\\
-000009a0: 733f 283f 3a5b 5c5c 775d 2b29 5c5c 733f  s?(?:[\\w]+)\\s?
-000009b0: 297b 302c 222b 6e75 6d43 6f6e 7465 7874  ){0,"+numContext
-000009c0: 576f 7264 732b 227d 2229 3b0a 2020 2020  Words+"}");.    
-000009d0: 2020 2020 2020 2020 6974 656d 2e63 6f6e          item.con
-000009e0: 7465 7874 203d 2074 6578 743b 0a20 2020  text = text;.   
-000009f0: 2020 2020 2020 2020 2076 6172 2064 6976           var div
-00000a00: 636f 6e74 6578 7420 3d20 646f 6375 6d65  context = docume
-00000a10: 6e74 2e63 7265 6174 6545 6c65 6d65 6e74  nt.createElement
-00000a20: 2822 6469 7622 293b 0a20 2020 2020 2020  ("div");.       
-00000a30: 2020 2020 2064 6976 636f 6e74 6578 742e       divcontext.
-00000a40: 636c 6173 734e 616d 6520 3d20 2263 6f6e  className = "con
-00000a50: 7465 7874 223b 0a20 2020 2020 2020 2020  text";.         
-00000a60: 2020 2064 6976 636f 6e74 6578 742e 696e     divcontext.in
-00000a70: 6e65 7254 6578 7420 3d20 2869 7465 6d2e  nerText = (item.
-00000a80: 636f 6e74 6578 7420 7c7c 2027 2729 3b0a  context || '');.
-00000a90: 2020 2020 2020 2020 2020 2020 7661 7220              var 
-00000aa0: 6469 7673 7567 6765 7374 696f 6e20 3d20  divsuggestion = 
-00000ab0: 646f 6375 6d65 6e74 2e63 7265 6174 6545  document.createE
-00000ac0: 6c65 6d65 6e74 2822 6469 7622 293b 0a20  lement("div");. 
-00000ad0: 2020 2020 2020 2020 2020 2064 6976 7375             divsu
-00000ae0: 6767 6573 7469 6f6e 2e63 6c61 7373 4e61  ggestion.classNa
-00000af0: 6d65 203d 2022 6175 746f 636f 6d70 6c65  me = "autocomple
-00000b00: 7465 2d73 7567 6765 7374 696f 6e22 3b0a  te-suggestion";.
-00000b10: 2020 2020 2020 2020 2020 2020 6469 7673              divs
-00000b20: 7567 6765 7374 696f 6e2e 7365 7441 7474  uggestion.setAtt
-00000b30: 7269 6275 7465 2822 6461 7461 2d74 6572  ribute("data-ter
-00000b40: 6d22 2c20 7465 726d 293b 0a20 2020 2020  m", term);.     
-00000b50: 2020 2020 2020 2064 6976 7375 6767 6573         divsugges
-00000b60: 7469 6f6e 2e73 6574 4174 7472 6962 7574  tion.setAttribut
-00000b70: 6528 2264 6174 612d 7469 746c 6522 2c20  e("data-title", 
-00000b80: 6974 656d 2e74 6974 6c65 293b 0a20 2020  item.title);.   
-00000b90: 2020 2020 2020 2020 2064 6976 7375 6767           divsugg
-00000ba0: 6573 7469 6f6e 2e73 6574 4174 7472 6962  estion.setAttrib
-00000bb0: 7574 6528 2264 6174 612d 7572 6922 2c20  ute("data-uri", 
-00000bc0: 6974 656d 2e75 7269 293b 0a20 2020 2020  item.uri);.     
-00000bd0: 2020 2020 2020 2064 6976 7375 6767 6573         divsugges
-00000be0: 7469 6f6e 2e73 6574 4174 7472 6962 7574  tion.setAttribut
-00000bf0: 6528 2264 6174 612d 636f 6e74 6578 7422  e("data-context"
-00000c00: 2c20 6974 656d 2e63 6f6e 7465 7874 293b  , item.context);
-00000c10: 0a20 2020 2020 2020 2020 2020 2064 6976  .            div
-00000c20: 7375 6767 6573 7469 6f6e 2e69 6e6e 6572  suggestion.inner
-00000c30: 5465 7874 203d 2027 c2bb 2027 202b 2069  Text = '.. ' + i
-00000c40: 7465 6d2e 7469 746c 653b 0a20 2020 2020  tem.title;.     
-00000c50: 2020 2020 2020 2064 6976 7375 6767 6573         divsugges
-00000c60: 7469 6f6e 2e61 7070 656e 6443 6869 6c64  tion.appendChild
-00000c70: 2864 6976 636f 6e74 6578 7429 3b0a 2020  (divcontext);.  
-00000c80: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00000c90: 2064 6976 7375 6767 6573 7469 6f6e 2e6f   divsuggestion.o
-00000ca0: 7574 6572 4854 4d4c 3b0a 2020 2020 2020  uterHTML;.      
-00000cb0: 2020 7d2c 0a20 2020 2020 2020 202f 2a20    },.        /* 
-00000cc0: 6f6e 5365 6c65 6374 2063 616c 6c62 6163  onSelect callbac
-00000cd0: 6b20 6669 7265 7320 7768 656e 2061 2073  k fires when a s
-00000ce0: 6561 7263 6820 7375 6767 6573 7469 6f6e  earch suggestion
-00000cf0: 2069 7320 6368 6f73 656e 202a 2f0a 2020   is chosen */.  
-00000d00: 2020 2020 2020 6f6e 5365 6c65 6374 3a20        onSelect: 
-00000d10: 6675 6e63 7469 6f6e 2865 2c20 7465 726d  function(e, term
-00000d20: 2c20 6974 656d 2920 7b0a 2020 2020 2020  , item) {.      
-00000d30: 2020 2020 2020 6c6f 6361 7469 6f6e 2e68        location.h
-00000d40: 7265 6620 3d20 6974 656d 2e67 6574 4174  ref = item.getAt
-00000d50: 7472 6962 7574 6528 2764 6174 612d 7572  tribute('data-ur
-00000d60: 6927 293b 0a20 2020 2020 2020 207d 0a20  i');.        }. 
-00000d70: 2020 207d 293b 0a7d 293b 0a                 });.});.
+00000340: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000350: 2020 7468 6973 2e70 6970 656c 696e 652e    this.pipeline.
+00000360: 7265 6d6f 7665 286c 756e 722e 7374 656d  remove(lunr.stem
+00000370: 6d65 7229 3b0a 2020 2020 2020 2020 2020  mer);.          
+00000380: 2020 2020 2020 7468 6973 2e73 6561 7263        this.searc
+00000390: 6850 6970 656c 696e 652e 7265 6d6f 7665  hPipeline.remove
+000003a0: 286c 756e 722e 7374 656d 6d65 7229 3b0a  (lunr.stemmer);.
+000003b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000003c0: 202f 2f20 4665 6564 206c 756e 7220 7769   // Feed lunr wi
+000003d0: 7468 2065 6163 6820 6669 6c65 2061 6e64  th each file and
+000003e0: 206c 6574 206c 756e 7220 6163 7475 616c   let lunr actual
+000003f0: 6c79 2069 6e64 6578 2074 6865 6d0a 2020  ly index them.  
+00000400: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00000410: 6765 7349 6e64 6578 2e66 6f72 4561 6368  gesIndex.forEach
+00000420: 2866 756e 6374 696f 6e28 7061 6765 2920  (function(page) 
+00000430: 7b0a 0909 2020 2020 7468 6973 2e61 6464  {...    this.add
+00000440: 2870 6167 6529 3b0a 2020 2020 2020 2020  (page);.        
+00000450: 2020 2020 2020 2020 7d2c 2074 6869 7329          }, this)
+00000460: 3b0a 2020 2020 2020 2020 2020 2020 7d29  ;.            })
+00000470: 0a20 2020 2020 2020 207d 290a 2020 2020  .        }).    
+00000480: 2020 2020 2e66 6169 6c28 6675 6e63 7469      .fail(functi
+00000490: 6f6e 286a 7178 6872 2c20 7465 7874 5374  on(jqxhr, textSt
+000004a0: 6174 7573 2c20 6572 726f 7229 207b 0a20  atus, error) {. 
+000004b0: 2020 2020 2020 2020 2020 2076 6172 2065             var e
+000004c0: 7272 203d 2074 6578 7453 7461 7475 7320  rr = textStatus 
+000004d0: 2b20 222c 2022 202b 2065 7272 6f72 3b0a  + ", " + error;.
+000004e0: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
+000004f0: 6f6c 652e 6572 726f 7228 2245 7272 6f72  ole.error("Error
+00000500: 2067 6574 7469 6e67 2048 7567 6f20 696e   getting Hugo in
+00000510: 6465 7820 6669 6c65 3a22 2c20 6572 7229  dex file:", err)
+00000520: 3b0a 2020 2020 2020 2020 7d29 3b0a 7d0a  ;.        });.}.
+00000530: 0a2f 2a2a 0a20 2a20 5472 6967 6765 7220  ./**. * Trigger 
+00000540: 6120 7365 6172 6368 2069 6e20 6c75 6e72  a search in lunr
+00000550: 2061 6e64 2074 7261 6e73 666f 726d 2074   and transform t
+00000560: 6865 2072 6573 756c 740a 202a 0a20 2a20  he result. *. * 
+00000570: 4070 6172 616d 2020 7b53 7472 696e 677d  @param  {String}
+00000580: 2071 7565 7279 0a20 2a20 4072 6574 7572   query. * @retur
+00000590: 6e20 7b41 7272 6179 7d20 2072 6573 756c  n {Array}  resul
+000005a0: 7473 0a20 2a2f 0a66 756e 6374 696f 6e20  ts. */.function 
+000005b0: 7365 6172 6368 2871 7565 7279 5465 726d  search(queryTerm
+000005c0: 2920 7b0a 2020 2020 2f2f 2046 696e 6420  ) {.    // Find 
+000005d0: 7468 6520 6974 656d 2069 6e20 6f75 7220  the item in our 
+000005e0: 696e 6465 7820 636f 7272 6573 706f 6e64  index correspond
+000005f0: 696e 6720 746f 2074 6865 206c 756e 7220  ing to the lunr 
+00000600: 6f6e 6520 746f 2068 6176 6520 6d6f 7265  one to have more
+00000610: 2069 6e66 6f0a 2020 2020 7265 7475 726e   info.    return
+00000620: 206c 756e 7249 6e64 6578 2e73 6561 7263   lunrIndex.searc
+00000630: 6828 7175 6572 7954 6572 6d2b 225e 3130  h(queryTerm+"^10
+00000640: 3022 2b22 2022 2b71 7565 7279 5465 726d  0"+" "+queryTerm
+00000650: 2b22 2a5e 3130 222b 2220 222b 222a 222b  +"*^10"+" "+"*"+
+00000660: 7175 6572 7954 6572 6d2b 225e 3130 222b  queryTerm+"^10"+
+00000670: 2220 222b 7175 6572 7954 6572 6d2b 227e  " "+queryTerm+"~
+00000680: 325e 3122 292e 6d61 7028 6675 6e63 7469  2^1").map(functi
+00000690: 6f6e 2872 6573 756c 7429 207b 0a20 2020  on(result) {.   
+000006a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000006b0: 7061 6765 7349 6e64 6578 2e66 696c 7465  pagesIndex.filte
+000006c0: 7228 6675 6e63 7469 6f6e 2870 6167 6529  r(function(page)
+000006d0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+000006e0: 2020 2072 6574 7572 6e20 7061 6765 2e75     return page.u
+000006f0: 7269 203d 3d3d 2072 6573 756c 742e 7265  ri === result.re
+00000700: 663b 0a20 2020 2020 2020 2020 2020 207d  f;.            }
+00000710: 295b 305d 3b0a 2020 2020 2020 2020 7d29  )[0];.        })
+00000720: 3b0a 7d0a 0a2f 2f20 4c65 7427 7320 6765  ;.}..// Let's ge
+00000730: 7420 7374 6172 7465 640a 696e 6974 4c75  t started.initLu
+00000740: 6e72 2829 3b0a 2428 2064 6f63 756d 656e  nr();.$( documen
+00000750: 7420 292e 7265 6164 7928 6675 6e63 7469  t ).ready(functi
+00000760: 6f6e 2829 207b 0a20 2020 2076 6172 2073  on() {.    var s
+00000770: 6561 7263 684c 6973 7420 3d20 6e65 7720  earchList = new 
+00000780: 6175 746f 436f 6d70 6c65 7465 287b 0a20  autoComplete({. 
+00000790: 2020 2020 2020 202f 2a20 7365 6c65 6374         /* select
+000007a0: 6f72 2066 6f72 2074 6865 2073 6561 7263  or for the searc
+000007b0: 6820 626f 7820 656c 656d 656e 7420 2a2f  h box element */
+000007c0: 0a20 2020 2020 2020 2073 656c 6563 746f  .        selecto
+000007d0: 723a 2024 2822 2373 6561 7263 682d 6279  r: $("#search-by
+000007e0: 2229 2e67 6574 2830 292c 0a20 2020 2020  ").get(0),.     
+000007f0: 2020 202f 2a20 736f 7572 6365 2069 7320     /* source is 
+00000800: 7468 6520 6361 6c6c 6261 636b 2074 6f20  the callback to 
+00000810: 7065 7266 6f72 6d20 7468 6520 7365 6172  perform the sear
+00000820: 6368 202a 2f0a 2020 2020 2020 2020 736f  ch */.        so
+00000830: 7572 6365 3a20 6675 6e63 7469 6f6e 2874  urce: function(t
+00000840: 6572 6d2c 2072 6573 706f 6e73 6529 207b  erm, response) {
+00000850: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00000860: 706f 6e73 6528 7365 6172 6368 2874 6572  ponse(search(ter
+00000870: 6d29 293b 0a20 2020 2020 2020 207d 2c0a  m));.        },.
+00000880: 2020 2020 2020 2020 2f2a 2072 656e 6465          /* rende
+00000890: 7249 7465 6d20 6469 7370 6c61 7973 2069  rItem displays i
+000008a0: 6e64 6976 6964 7561 6c20 7365 6172 6368  ndividual search
+000008b0: 2072 6573 756c 7473 202a 2f0a 2020 2020   results */.    
+000008c0: 2020 2020 7265 6e64 6572 4974 656d 3a20      renderItem: 
+000008d0: 6675 6e63 7469 6f6e 2869 7465 6d2c 2074  function(item, t
+000008e0: 6572 6d29 207b 0a20 2020 2020 2020 2020  erm) {.         
+000008f0: 2020 2076 6172 206e 756d 436f 6e74 6578     var numContex
+00000900: 7457 6f72 6473 203d 2032 3b0a 2020 2020  tWords = 2;.    
+00000910: 2020 2020 2020 2020 7661 7220 7465 7874          var text
+00000920: 203d 2069 7465 6d2e 636f 6e74 656e 742e   = item.content.
+00000930: 6d61 7463 6828 0a20 2020 2020 2020 2020  match(.         
+00000940: 2020 2020 2020 2022 283f 3a5c 5c73 3f28         "(?:\\s?(
+00000950: 3f3a 5b5c 5c77 5d2b 295c 5c73 3f29 7b30  ?:[\\w]+)\\s?){0
+00000960: 2c22 2b6e 756d 436f 6e74 6578 7457 6f72  ,"+numContextWor
+00000970: 6473 2b22 7d22 202b 0a20 2020 2020 2020  ds+"}" +.       
+00000980: 2020 2020 2020 2020 2020 2020 2074 6572               ter
+00000990: 6d2b 2228 3f3a 5c5c 733f 283f 3a5b 5c5c  m+"(?:\\s?(?:[\\
+000009a0: 775d 2b29 5c5c 733f 297b 302c 222b 6e75  w]+)\\s?){0,"+nu
+000009b0: 6d43 6f6e 7465 7874 576f 7264 732b 227d  mContextWords+"}
+000009c0: 2229 3b0a 2020 2020 2020 2020 2020 2020  ");.            
+000009d0: 6974 656d 2e63 6f6e 7465 7874 203d 2074  item.context = t
+000009e0: 6578 743b 0a20 2020 2020 2020 2020 2020  ext;.           
+000009f0: 2076 6172 2064 6976 636f 6e74 6578 7420   var divcontext 
+00000a00: 3d20 646f 6375 6d65 6e74 2e63 7265 6174  = document.creat
+00000a10: 6545 6c65 6d65 6e74 2822 6469 7622 293b  eElement("div");
+00000a20: 0a20 2020 2020 2020 2020 2020 2064 6976  .            div
+00000a30: 636f 6e74 6578 742e 636c 6173 734e 616d  context.classNam
+00000a40: 6520 3d20 2263 6f6e 7465 7874 223b 0a20  e = "context";. 
+00000a50: 2020 2020 2020 2020 2020 2064 6976 636f             divco
+00000a60: 6e74 6578 742e 696e 6e65 7254 6578 7420  ntext.innerText 
+00000a70: 3d20 2869 7465 6d2e 636f 6e74 6578 7420  = (item.context 
+00000a80: 7c7c 2027 2729 3b0a 2020 2020 2020 2020  || '');.        
+00000a90: 2020 2020 7661 7220 6469 7673 7567 6765      var divsugge
+00000aa0: 7374 696f 6e20 3d20 646f 6375 6d65 6e74  stion = document
+00000ab0: 2e63 7265 6174 6545 6c65 6d65 6e74 2822  .createElement("
+00000ac0: 6469 7622 293b 0a20 2020 2020 2020 2020  div");.         
+00000ad0: 2020 2064 6976 7375 6767 6573 7469 6f6e     divsuggestion
+00000ae0: 2e63 6c61 7373 4e61 6d65 203d 2022 6175  .className = "au
+00000af0: 746f 636f 6d70 6c65 7465 2d73 7567 6765  tocomplete-sugge
+00000b00: 7374 696f 6e22 3b0a 2020 2020 2020 2020  stion";.        
+00000b10: 2020 2020 6469 7673 7567 6765 7374 696f      divsuggestio
+00000b20: 6e2e 7365 7441 7474 7269 6275 7465 2822  n.setAttribute("
+00000b30: 6461 7461 2d74 6572 6d22 2c20 7465 726d  data-term", term
+00000b40: 293b 0a20 2020 2020 2020 2020 2020 2064  );.            d
+00000b50: 6976 7375 6767 6573 7469 6f6e 2e73 6574  ivsuggestion.set
+00000b60: 4174 7472 6962 7574 6528 2264 6174 612d  Attribute("data-
+00000b70: 7469 746c 6522 2c20 6974 656d 2e74 6974  title", item.tit
+00000b80: 6c65 293b 0a20 2020 2020 2020 2020 2020  le);.           
+00000b90: 2064 6976 7375 6767 6573 7469 6f6e 2e73   divsuggestion.s
+00000ba0: 6574 4174 7472 6962 7574 6528 2264 6174  etAttribute("dat
+00000bb0: 612d 7572 6922 2c20 6974 656d 2e75 7269  a-uri", item.uri
+00000bc0: 293b 0a20 2020 2020 2020 2020 2020 2064  );.            d
+00000bd0: 6976 7375 6767 6573 7469 6f6e 2e73 6574  ivsuggestion.set
+00000be0: 4174 7472 6962 7574 6528 2264 6174 612d  Attribute("data-
+00000bf0: 636f 6e74 6578 7422 2c20 6974 656d 2e63  context", item.c
+00000c00: 6f6e 7465 7874 293b 0a20 2020 2020 2020  ontext);.       
+00000c10: 2020 2020 2064 6976 7375 6767 6573 7469       divsuggesti
+00000c20: 6f6e 2e69 6e6e 6572 5465 7874 203d 2027  on.innerText = '
+00000c30: c2bb 2027 202b 2069 7465 6d2e 7469 746c  .. ' + item.titl
+00000c40: 653b 0a20 2020 2020 2020 2020 2020 2064  e;.            d
+00000c50: 6976 7375 6767 6573 7469 6f6e 2e61 7070  ivsuggestion.app
+00000c60: 656e 6443 6869 6c64 2864 6976 636f 6e74  endChild(divcont
+00000c70: 6578 7429 3b0a 2020 2020 2020 2020 2020  ext);.          
+00000c80: 2020 7265 7475 726e 2064 6976 7375 6767    return divsugg
+00000c90: 6573 7469 6f6e 2e6f 7574 6572 4854 4d4c  estion.outerHTML
+00000ca0: 3b0a 2020 2020 2020 2020 7d2c 0a20 2020  ;.        },.   
+00000cb0: 2020 2020 202f 2a20 6f6e 5365 6c65 6374       /* onSelect
+00000cc0: 2063 616c 6c62 6163 6b20 6669 7265 7320   callback fires 
+00000cd0: 7768 656e 2061 2073 6561 7263 6820 7375  when a search su
+00000ce0: 6767 6573 7469 6f6e 2069 7320 6368 6f73  ggestion is chos
+00000cf0: 656e 202a 2f0a 2020 2020 2020 2020 6f6e  en */.        on
+00000d00: 5365 6c65 6374 3a20 6675 6e63 7469 6f6e  Select: function
+00000d10: 2865 2c20 7465 726d 2c20 6974 656d 2920  (e, term, item) 
+00000d20: 7b0a 2020 2020 2020 2020 2020 2020 6c6f  {.            lo
+00000d30: 6361 7469 6f6e 2e68 7265 6620 3d20 6974  cation.href = it
+00000d40: 656d 2e67 6574 4174 7472 6962 7574 6528  em.getAttribute(
+00000d50: 2764 6174 612d 7572 6927 293b 0a20 2020  'data-uri');.   
+00000d60: 2020 2020 207d 0a20 2020 207d 293b 0a7d       }.    });.}
+00000d70: 293b 0a                                  );.
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/mermaid/mermaid.js` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/mermaid/mermaid.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text, with very long lines (65536), with no line terminators*

 * *Files 0% similar despite different names*

```diff
@@ -52055,8 +52055,8 @@
 000cb560: 642e 6874 6d6c 4c61 6265 6c73 2929 2c4c  d.htmlLabels)),L
 000cb570: 6f2e 696e 6974 6961 6c69 7a65 2874 297d  o.initialize(t)}
 000cb580: 2c63 6f6e 7465 6e74 4c6f 6164 6564 3a46  ,contentLoaded:F
 000cb590: 6f7d 3b65 2e64 6566 6175 6c74 3d50 6f7d  o};e.default=Po}
 000cb5a0: 5d29 2e64 6566 6175 6c74 7d29 293b 0a2f  ]).default}));./
 000cb5b0: 2f23 2073 6f75 7263 654d 6170 7069 6e67  /# sourceMapping
 000cb5c0: 5552 4c3d 6d65 726d 6169 642e 6d69 6e2e  URL=mermaid.min.
-000cb5d0: 6a73 2e6d 6170                           js.map
+000cb5d0: 6a73 2e6d 6170 0a                        js.map.
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.eot` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.svg` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.svg`

 * *Files 0% similar despite different names*

```diff
@@ -46206,8 +46206,8 @@
 000b47d0: 3920 3136 352e 3836 2036 3339 2e39 3720  9 165.86 639.97 
 000b47e0: 3138 392e 3634 2036 3339 2e39 3720 3138  189.64 639.97 18
 000b47f0: 392e 3634 4c36 3430 2031 3839 2e36 357a  9.64L640 189.65z
 000b4800: 2220 676c 7970 682d 6e61 6d65 3d22 7a68  " glyph-name="zh
 000b4810: 6968 7522 2068 6f72 697a 2d61 6476 2d78  ihu" horiz-adv-x
 000b4820: 3d22 3634 3022 2075 6e69 636f 6465 3d22  ="640" unicode="
 000b4830: ef98 bf22 2f3e 3c2f 666f 6e74 3e3c 2f64  ..."/></font></d
-000b4840: 6566 733e 3c2f 7376 673e                 efs></svg>
+000b4840: 6566 733e 3c2f 7376 673e 0a              efs></svg>.
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.ttf` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.woff` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.woff2` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.eot` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.svg` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.svg`

 * *Files 0% similar despite different names*

```diff
@@ -8481,8 +8481,8 @@
 00021200: 3620 3333 302e 3520 3339 342e 3520 3335  6 330.5 394.5 35
 00021210: 3220 3336 3820 3335 3248 3134 3456 3430  2 368 352H144V40
 00021220: 3048 3436 3456 3830 7a22 2067 6c79 7068  0H464V80z" glyph
 00021230: 2d6e 616d 653d 2277 696e 646f 772d 7265  -name="window-re
 00021240: 7374 6f72 6522 2068 6f72 697a 2d61 6476  store" horiz-adv
 00021250: 2d78 3d22 3531 3222 2075 6e69 636f 6465  -x="512" unicode
 00021260: 3d22 ef8b 9222 2f3e 3c2f 666f 6e74 3e3c  ="..."/></font><
-00021270: 2f64 6566 733e 3c2f 7376 673e            /defs></svg>
+00021270: 2f64 6566 733e 3c2f 7376 673e 0a         /defs></svg>.
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.ttf` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.woff` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.woff2` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.eot` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.svg` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.svg`

 * *Files 0% similar despite different names*

```diff
@@ -48225,8 +48225,8 @@
 000bc600: 3030 3030 3030 3031 2032 3830 2032 3838  00000001 280 288
 000bc610: 5332 3635 2e36 3720 3332 3020 3234 3820  S265.67 320 248 
 000bc620: 3332 307a 2220 676c 7970 682d 6e61 6d65  320z" glyph-name
 000bc630: 3d22 7969 6e2d 7961 6e67 2220 686f 7269  ="yin-yang" hori
 000bc640: 7a2d 6164 762d 783d 2234 3936 2220 756e  z-adv-x="496" un
 000bc650: 6963 6f64 653d 22ef 9aad 222f 3e3c 2f66  icode="..."/></f
 000bc660: 6f6e 743e 3c2f 6465 6673 3e3c 2f73 7667  ont></defs></svg
-000bc670: 3e                                       >
+000bc670: 3e0a                                     >.
```

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.ttf` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.woff` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.woff2` & `angreal-2.0.7/docs/themes/hugo-theme-learn/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/py_tests/integrations/test_docker.py` & `angreal-2.0.7/py_tests/integrations/test_docker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pytest 
+import pytest
 import sys
 
 from angreal.integrations.docker import Docker
 from angreal.integrations.docker.container import Containers, Container
 from angreal.integrations.docker.network   import Network, Networks
 from angreal.integrations.docker.image     import Image, Images
 from angreal.integrations.docker.volume    import Volume, Volumes
@@ -69,8 +69,8 @@
 @pytest.mark.skipif(
     sys.platform == 'win32', reason="windows tests are flaky"
 )
 def test_network():
     """volumes interface exists"""
     d = Docker()
     assert isinstance(d.networks(), Networks)
-    assert isinstance(Network(d,'id'), Network)
+    assert isinstance(Network(d,'id'), Network)
```

### Comparing `angreal-2.0.6/py_tests/integrations/test_git.py` & `angreal-2.0.7/py_tests/integrations/test_git.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from angreal.integrations.git import Git, GitException
 
 
 def test_git_no_path():
     """
     test git object fails with no path
     """
-    git = Git(git_path=None)
+    Git(git_path=None)
 
 
 def test_git_bad_path():
     """
     test git object fails with bad path
     """
     with pytest.raises(OSError):
-        git = Git(git_path="not git")
+        Git(git_path="not git")
 
 
 def test_git_bad_subcommand():
     """
     test that object fails with bad sub-command
     """
```

### Comparing `angreal-2.0.6/py_tests/integrations/test_venv.py` & `angreal-2.0.7/py_tests/integrations/test_venv.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 def test_venv_required():
     """
     test venv required good
     """
 
     @venv_required("__angreal", requirements='flask')
     def test(a, b):
-        import flask
         return a + b
 
     try:
         assert test(1, 2) == 3
     except:
         raise
     finally:
@@ -34,70 +33,71 @@
     assert os.path.exists(test_requirements)
     # activation edits sys.prefix, save and reset it when this test passes
     initial_sys_prefix = sys.prefix
 
     this_venv = "__test_venv_1"
     assert not os.path.isdir(this_venv)
 
-    venv = VirtualEnv(path=this_venv, requirements=test_requirements, now=True).install_requirements()
+    VirtualEnv(path=this_venv, requirements=test_requirements,
+                now=True).install_requirements()
+
 
-    
 
     try:
-        import flask
+        pass
     except (ImportError, AssertionError):
         raise
     finally:
         try:
             shutil.rmtree(this_venv)
             sys.prefix = initial_sys_prefix
-        except:
+        except Exception:
             pass
-            
 
 
-def test_requirements_load():
+
+def test_requirements_load_string():
     """
     testing load from "string"
     """
 
     # activation edits sys.prefix, save and reset it when this test passes
     initial_sys_prefix = sys.prefix
 
     this_venv = "__test_venv_2"
     assert not os.path.isdir(this_venv)
 
-    venv = VirtualEnv(path=this_venv, requirements=flask, now=True).install_requirements()
+    VirtualEnv(path=this_venv, requirements="flask", now=True).install_requirements()
 
     try:
-        import flask
+        pass
     except (ImportError, AssertionError):
         raise
     finally:
         try:
             shutil.rmtree(this_venv)
             sys.prefix = initial_sys_prefix
-        except:
+        except Exception:
             pass
 
 
-def test_requirements_load():
+def test_requirements_load_list():
     """
     test load requirements from list
     """
     # activation edits sys.prefix, save and reset it when this test passes
     initial_sys_prefix = sys.prefix
     this_venv = "__test_venv_3"
     assert not os.path.isdir(this_venv)
 
-    venv = VirtualEnv(path=this_venv, requirements=["flask"], now=True).install_requirements()
+    VirtualEnv(path=this_venv, requirements=["flask"], now=True).install_requirements()
 
     try:
-        import flask
+        pass
     except (ImportError, AssertionError):
         raise
     finally:
         try:
             shutil.rmtree(this_venv)
             sys.prefix = initial_sys_prefix
-        except:
+        except Exception:
             pass
```

### Comparing `angreal-2.0.6/pyproject.toml` & `angreal-2.0.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -16,17 +16,17 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
-    "Topic :: Software Development :: Libraries :: Python Modules",    
+    "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 
 
 [project.scripts]
 angreal = "angreal:main"
 
 [tool.maturin]
-features = ["pyo3/extension-module"]
+features = ["pyo3/extension-module"]
```

### Comparing `angreal-2.0.6/python/angreal/integrations/git.py` & `angreal-2.0.7/python/angreal/integrations/git.py`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/python/angreal/integrations/venv.py` & `angreal-2.0.7/python/angreal/integrations/venv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 """
     angreal.integrations.virtual_env
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     Integration to virtualenv
 
 """
-import logging
 import functools
 import os
 import subprocess
 import sys
 import venv
-import site
 
-from shutil import which
 
 
 def venv_required(path,requirements=None):
     """wrap a function in a virtual environment before execution
 
     Args:
-        path (str): The path to the virtual environment (or where the environment should be created if it doesn't exist)
-        requirements (_type_, optional): A string containing a single module, a list of module names, or a string containing a file path. Defaults to None.
+        path (str): The path to the virtual environment (or where the environment
+          should be created if it doesn't exist)
+        requirements (_type_, optional): A string containing a single module, a
+          list of module names, or a string containing a file path. Defaults to None.
     """
-    
+
     def decorator(f):
 
         @functools.wraps(f)
         def wrapper(*args, **kwargs):
             initial_sys_prefix = sys.prefix
             venv = VirtualEnv(path=path, now=True,requirements=requirements)
             venv.install_requirements()
@@ -37,22 +36,24 @@
 
         return wrapper
 
     return decorator
 
 
 class VirtualEnv(object):
-    
+
     """
     Interacting with virtual environments from within a currently running script.
 
     Args:
         path (str): the path to the virtual environment
-        requirements ([str,List[str]]), optional): A string containing a single module, a list of module names, or a string containing a file path. Defaults to None.
-        now (bool, optional): should the environment be created/activated on initialization. Defaults to True
+        requirements ([str,List[str]]), optional): A string containing a single module,
+          a list of module names, or a string containing a file path. Defaults to None.
+        now (bool, optional): should the environment be created/activated
+          on initialization. Defaults to True
     """
 
     base_path = os.path.expanduser(os.path.join("~", ".venv"))
 
     @property
     def exists(self):
         """
@@ -86,40 +87,42 @@
             self._activate()
 
 
     def install_requirements(self):
         """
         install requirements the requirements set during initialization.
 
-        :param requirements: path to a requirements file, single requirement, or list of requirements
+        :param requirements: path to a requirements file, single requirement,
+          or list of requirements
         """
 
         if not self.requirements:
             return
 
         args = [self.ensure_directories.env_exe, "-m", "pip", "install"]
 
-        
+
         if isinstance(self.requirements, list):
             args = args + self.requirements
         elif os.path.exists(self.requirements):
             args = args + ["-r", self.requirements]
         elif isinstance(self.requirements, str):
             args = args + [self.requirements]
         else:
             raise TypeError(
-                f"requirements should be one of : file, list, or string got {type(self.requirements)}"
+                "requirements should be one of : file, list, or string got "
+                "{type(self.requirements)}"
             )
 
         rc = subprocess.call(args, stdout=self.devnull, stderr=self.devnull)
         if rc != 0:
             raise EnvironmentError(
                 "{} failed to install requirements file.".format(self.path)
             )
-    
+
 
     def __str__(self):
         return self.path
 
     def _create(self):
         """
         Create the described environment.
```

### Comparing `angreal-2.0.6/src/init.rs` & `angreal-2.0.7/src/init.rs`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 use std::fs::File;
 use std::io::Write;
 use std::ops::Not;
 use std::path::{Path, PathBuf};
 use std::process::exit;
 use tera::{Context, Tera};
 use text_io::read;
-use toml::{Table, Value};
+use toml::{map::Map, Table, Value};
 use walkdir::WalkDir;
 
 /// Initialize a new project by rendering a template.
 pub fn init(template: &str, force: bool, take_inputs: bool) {
     let angreal_home = create_home_dot_angreal();
     let template_type = get_scheme(template).unwrap();
     debug!("Got template type {:?} for {:?}.", template_type, template);
@@ -116,14 +116,15 @@
                 .unwrap();
 
             let function: Py<PyAny> = PyModule::from_code(py, &init_contents, "", "")
                 .unwrap()
                 .getattr("init")
                 .unwrap()
                 .into();
+
             function.call0(py).unwrap();
         });
     }
 
     println!(
         "Angreal template ({}) successfully rendered !",
         template.to_string_lossy()
@@ -177,14 +178,15 @@
             exit(1);
         }
     };
 
     // build our tera context from toml file.
     let extract = file_contents.parse::<Table>().unwrap();
     let mut context = Context::new();
+    let mut toml_values = Map::new();
     for (k, v) in extract.iter() {
         let value = if v.is_str()
             && v.as_str().unwrap().starts_with("{{")
             && v.as_str().unwrap().contains("}}")
         {
             let temp_value = v.clone();
             let rendered_value =
@@ -200,36 +202,50 @@
         } else {
             String::new()
         };
 
         if input.trim().is_empty() | take_input.not() {
             if value.is_str() {
                 context.insert(k, &value.as_str().unwrap());
+                toml_values.insert(k.into(), value.clone());
             }
             if value.is_integer() {
                 context.insert(k, &value.as_integer().unwrap());
+                toml_values.insert(k.into(), value.clone());
             }
             if value.is_bool() {
                 context.insert(k, &value.as_bool().unwrap());
+                toml_values.insert(k.into(), value.clone());
             }
             if value.is_float() {
                 context.insert(k, &value.as_float().unwrap());
+                toml_values.insert(k.into(), value.clone());
             }
         } else {
             if value.is_str() {
                 context.insert(k, &input.trim());
+                toml_values.insert(k.into(), Value::String(input.trim().to_string()));
             }
             if value.is_integer() {
                 context.insert(k, &input.trim().parse::<i32>().unwrap());
+                toml_values.insert(
+                    k.into(),
+                    Value::Integer(input.trim().parse::<i64>().unwrap()),
+                );
             }
             if value.is_bool() {
                 context.insert(k, &input.trim());
+                toml_values.insert(
+                    k.into(),
+                    Value::Boolean(input.trim().parse::<bool>().unwrap()),
+                );
             }
             if value.is_float() {
                 context.insert(k, &input.trim().parse::<f64>().unwrap());
+                toml_values.insert(k.into(), Value::Float(input.trim().parse::<f64>().unwrap()));
             }
         }
     }
 
     // first we create a Tera instance from an empty directory so we can extend it
     let mut tmp_dir = env::temp_dir();
     tmp_dir.push(Path::new("angreal_tmp"));
@@ -307,26 +323,34 @@
         if template == "angreal.toml" {
             // never render the angreal.toml
             // todo: exclusion glob
             continue;
         }
 
         if template.starts_with('.') {
-            // we don't render dot files eiterh
+            // we don't render dot files either
             // todo: exclusion glob
             continue;
         }
 
         let rendered = tera.render(template, &context).unwrap();
         let path = Tera::one_off(template, &context, false).unwrap();
         debug!("Rendering file at {:?}", path);
         let mut output = File::create(path).unwrap();
         write!(output, "{}", rendered.as_str()).unwrap();
     }
 
+    let toml_string = toml::to_string(&Value::Table(toml_values.clone())).unwrap();
+    let mut value_path = PathBuf::new();
+    value_path.push(angreal_path.as_str());
+    value_path.push("angreal.toml");
+
+    let mut output = File::create(&value_path).unwrap();
+    write!(output, "{}", toml_string.as_str()).unwrap();
+    debug!("Storing initialization values to {}", &value_path.display());
     angreal_path
 
     // return path to .angreal
 }
 
 #[cfg(test)]
 #[path = "../tests"]
```

### Comparing `angreal-2.0.6/src/lib.rs` & `angreal-2.0.7/src/lib.rs`

 * *Files 11% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 fn main() -> PyResult<()> {
     let handle = logger::init_logger();
     // we have to do this because we're calling the main function through python - when lib+bin build support is available, we can factor away
     let mut argvs: Vec<String> = std::env::args().collect();
     argvs.remove(0);
     argvs.remove(0);
 
+    utils::check_up_to_date();
+
     // env_logger::Builder::from_env(env_logger::Env::default().default_filter_or("warning"))
     // .init();
 
     // Load any angreal task assets that are available to us
     let in_angreal_project = utils::is_angreal_project().is_ok();
 
     if in_angreal_project {
@@ -59,15 +61,15 @@
 
         // load the files , IF a file has command or task decorators - they'll register themselves now
         for task in _angreal_tasks_to_load.iter() {
             utils::load_python(task.clone()).unwrap_or(());
         }
     }
 
-    let app = build_app();
+    let app = build_app(in_angreal_project);
     let mut app_copy = app.clone();
     let sub_command = app.get_matches_from(&argvs);
 
     // Get our asked for verbosity and set the logger up. TODO: find a way to initialize earlier and reset after.
     let verbosity = sub_command.get_count("verbose");
 
     logger::update_verbosity(&handle, verbosity);
@@ -79,20 +81,43 @@
             _sub_matches.is_present("defaults").not(),
         ),
         Some((task, sub_m)) => {
             if !in_angreal_project {
                 error!("This doesn't appear to be an angreal project.");
                 exit(1)
             }
+
+            let mut command_groups: Vec<String> = Vec::new();
+            command_groups.push(task.to_string());
+
+            let mut next = sub_m.subcommand();
+
+            while next.is_some() {
+                let cmd = next.unwrap();
+                command_groups.push(cmd.0.to_string());
+                next = cmd.1.subcommand();
+            }
+
+            let task = command_groups.pop().unwrap();
+
             let some_command = ANGREAL_TASKS.lock().unwrap().clone();
-            let some_command = some_command.iter().find(|&x| x.name == task);
+            let some_command = some_command.iter().find(|&x| {
+                x.name == task.as_str()
+                    && x.group
+                        .clone()
+                        .unwrap()
+                        .iter()
+                        .map(|x| x.name.to_string())
+                        .collect::<Vec<String>>()
+                        == command_groups
+            });
 
             let command = match some_command {
                 None => {
-                    error!("Task {}, not found.", <&str>::clone(&task));
+                    error!("Task {}, not found.", task.as_str());
                     app_copy.print_help().unwrap_or(());
                     exit(1)
                 }
                 Some(some_command) => some_command,
             };
 
             let args = builder::select_args(task.to_string());
@@ -141,14 +166,16 @@
     }
 
     Ok(())
 }
 
 #[pymodule]
 fn angreal(_py: Python, m: &PyModule) -> PyResult<()> {
+    m.add("__version__", env!("CARGO_PKG_VERSION"))?;
+
     py_logger::register();
     m.add_function(wrap_pyfunction!(main, m)?)?;
     task::register(_py, m)?;
     utils::register(_py, m)?;
 
     m.add_wrapped(wrap_pymodule!(_integrations))?;
```

### Comparing `angreal-2.0.6/src/logger.rs` & `angreal-2.0.7/src/logger.rs`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/src/macros.rs` & `angreal-2.0.7/src/macros.rs`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/src/py_logger.rs` & `angreal-2.0.7/src/py_logger.rs`

 * *Files 1% similar despite different names*

```diff
@@ -78,23 +78,24 @@
     logging.setattr("host_log", wrap_pyfunction!(host_log, logging)?)?;
 
     py.run(
         r#"
 class HostHandler(Handler):
 	def __init__(self, level=0):
 		super().__init__(level=level)
-	
+
 	def emit(self, record):
 		host_log(record)
 
 oldBasicConfig = basicConfig
 def basicConfig(*pargs, **kwargs):
 	if "handlers" not in kwargs:
 		kwargs["handlers"] = [HostHandler()]
 	return oldBasicConfig(*pargs, **kwargs)
+
 "#,
         Some(logging.dict()),
         None,
     )?;
 
     let all = logging.index()?;
     all.append("HostHandler")?;
```

### Comparing `angreal-2.0.6/src/task.rs` & `angreal-2.0.7/src/task.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,57 @@
 //! Core structures for describing tasks and arguments
 //!
 
 use once_cell::sync::Lazy;
 use pyo3::prelude::*;
+use pyo3::types::PyModule;
 use std::sync::Mutex;
 
 /// Registers the Command and Arg structs to the python api in the `angreal` module
 pub fn register(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
     m.add_class::<AngrealCommand>()?;
     m.add_class::<AngrealArg>()?;
+    m.add_class::<AngrealGroup>()?;
     Ok(())
 }
 
 /// A long lived structure that stores AngrealCommands upon registration
 pub static ANGREAL_TASKS: Lazy<Mutex<Vec<AngrealCommand>>> = Lazy::new(|| Mutex::new(vec![]));
 
 /// A long lived structure that stores AngrealArgs for commands upon registration
 pub static ANGREAL_ARGS: Lazy<Mutex<Vec<AngrealArg>>> = Lazy::new(|| Mutex::new(vec![]));
 
+/// A long lived structure that stores Angreal Groups for commands upon registration
+pub static ANGREAL_GROUPS: Lazy<Mutex<Vec<AngrealGroup>>> = Lazy::new(|| Mutex::new(vec![]));
+
+/// A group is just a special type of sub-command
+#[derive(Clone, Debug)]
+#[pyclass(name = "Group")]
+pub struct AngrealGroup {
+    /// The name of the command group
+    #[pyo3(get)]
+    pub name: String,
+    /// The about of the command group
+    #[pyo3(get)]
+    pub about: Option<String>,
+}
+/// Methods exposed in the python API
+#[pymethods]
+impl AngrealGroup {
+    #[new]
+    fn __new__(name: &str, about: Option<&str>) -> Self {
+        let group = AngrealGroup {
+            name: name.to_string(),
+            about: about.map(|i| i.to_string()),
+        };
+        ANGREAL_GROUPS.lock().unwrap().push(group.clone());
+        group
+    }
+}
+
 /// A command describes a subcommand to be registered with the CLI
 #[derive(Clone, Debug)]
 #[pyclass(name = "Command")]
 pub struct AngrealCommand {
     /// The name of the sub command
     #[pyo3(get)]
     pub name: String,
@@ -30,14 +60,17 @@
     pub about: Option<String>,
     /// A longer description of what the command does
     #[pyo3(get)]
     pub long_about: Option<String>,
     /// The actual function that is executed when the command is run
     #[pyo3(get)]
     pub func: Py<PyAny>,
+    /// The group this command belongs to
+    #[pyo3(get)]
+    pub group: Option<Vec<AngrealGroup>>,
 }
 
 /// Methods exposed to the python API
 #[pymethods]
 impl AngrealCommand {
     /// Initialization method for the object. The command is registered to `ANGREAL_TASKS` upon instantiation from the python api
     ///
@@ -59,24 +92,61 @@
     /// def test-message():
     ///     pass
     ///
     /// angreal.Command(name='test',about='a short message',
     /// long_about='a much longer message`, func=test-message)
     /// ```
     #[new]
-    fn __new__(name: &str, func: Py<PyAny>, about: Option<&str>, long_about: Option<&str>) -> Self {
+    fn __new__(
+        name: &str,
+        func: Py<PyAny>,
+        about: Option<&str>,
+        long_about: Option<&str>,
+        group: Option<Vec<AngrealGroup>>,
+    ) -> Self {
         let cmd = AngrealCommand {
             name: name.to_string(),
             about: about.map(|i| i.to_string()),
             long_about: long_about.map(|i| i.to_string()),
+            group,
             func,
         };
         ANGREAL_TASKS.lock().unwrap().push(cmd.clone());
         cmd
     }
+
+    pub fn add_group(&mut self, group: AngrealGroup) -> PyResult<()> {
+        let this_command_pos = ANGREAL_TASKS.lock().unwrap().iter().position(|x| {
+            x.name == self.name.as_str()
+                && x.group
+                    .clone()
+                    .unwrap()
+                    .iter()
+                    .map(|x| x.name.to_string())
+                    .collect::<Vec<String>>()
+                    == self
+                        .group
+                        .clone()
+                        .unwrap()
+                        .iter()
+                        .map(|x| x.name.to_string())
+                        .collect::<Vec<String>>()
+        });
+
+        if self.group.is_none() {
+            self.group = Some(Vec::new());
+        }
+
+        let mut g = self.group.as_mut().unwrap().clone();
+
+        g.insert(0, group);
+        self.group = Some(g.clone());
+        ANGREAL_TASKS.lock().unwrap()[this_command_pos.unwrap()] = self.clone();
+        Ok(())
+    }
 }
 
 /// An argument to augment the behavior of an angreal command
 #[derive(Clone, Debug)]
 #[pyclass(name = "Arg")]
 pub struct AngrealArg {
     /// The name of the argument, required to match the name in the function being executed by the command
```

### Comparing `angreal-2.0.6/src/utils.rs` & `angreal-2.0.7/src/utils.rs`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,34 @@
 use std::vec::Vec;
 
 use pyo3::prelude::*;
 use pyo3::types::{PyList, PyModule};
 use pyo3::PyResult;
 use std::fs;
 
+use reqwest;
+use version_compare::Version;
+
+pub fn check_up_to_date() {
+    let body = reqwest::blocking::get("https://pypi.org/pypi/angreal/json")
+        .unwrap()
+        .json::<serde_json::Value>()
+        .unwrap();
+
+    let upstream = body["info"]["version"].as_str().unwrap();
+
+    let current = env!("CARGO_PKG_VERSION");
+    let current = Version::from(current).unwrap();
+    let upstream = Version::from(upstream).unwrap();
+
+    if upstream > current {
+        println!("A newer version of angreal is available, use pip install --upgrade angreal to upgrade.")
+    };
+}
+
 /// Get a list of task files in given a path
 ///
 /// # Examples
 ///
 /// ```
 /// use angreal::utils::get_task_files;
 /// use std::path::PathBuf;
```

### Comparing `angreal-2.0.6/tests/common/mod.rs` & `angreal-2.0.7/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `angreal-2.0.6/Cargo.lock` & `angreal-2.0.7/Cargo.lock`

 * *Files 8% similar despite different names*

```diff
@@ -33,32 +33,37 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "angreal"
-version = "2.0.6"
+version = "2.0.7"
 dependencies = [
  "clap",
  "docker-pyo3",
  "git-url-parse",
  "git2",
+ "git2_credentials",
  "glob",
  "home",
  "log",
  "log4rs",
  "once_cell",
  "openssl",
  "pyo3",
  "rand",
+ "reqwest",
+ "same-file",
+ "serde_json",
  "tera",
  "text_io",
  "toml",
  "version",
+ "version-compare",
  "walkdir",
 ]
 
 [[package]]
 name = "anyhow"
 version = "1.0.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -118,14 +123,20 @@
 [[package]]
 name = "base64"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
 
 [[package]]
+name = "base64"
+version = "0.21.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
+
+[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "block-buffer"
@@ -275,14 +286,27 @@
  "once_cell",
  "owo-colors",
  "tracing-core",
  "tracing-error",
 ]
 
 [[package]]
+name = "console"
+version = "0.15.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c926e00cc70edefdc64d3a5ff31cc65bb97a3460097762bd23afb4d8145fccf8"
+dependencies = [
+ "encode_unicode",
+ "lazy_static",
+ "libc",
+ "unicode-width",
+ "windows-sys 0.45.0",
+]
+
+[[package]]
 name = "containers-api"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56082e32f18a6d60f06c736b49e234deffb93b13cb87091a39e0dec053d03819"
 dependencies = [
  "chrono",
  "flate2",
@@ -299,14 +323,24 @@
  "tar",
  "thiserror",
  "tokio",
  "url",
 ]
 
 [[package]]
+name = "core-foundation"
+version = "0.9.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "194a7a9e6de53fa55116934067c844d9d749312f75c6f6d0980e8c252f8c2146"
+dependencies = [
+ "core-foundation-sys",
+ "libc",
+]
+
+[[package]]
 name = "core-foundation-sys"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
 
 [[package]]
 name = "cpufeatures"
@@ -435,31 +469,63 @@
 [[package]]
 name = "deunicode"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "850878694b7933ca4c9569d30a34b55031b9b139ee1fc7b94a527c4ef960d690"
 
 [[package]]
+name = "dialoguer"
+version = "0.10.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "59c6f2989294b9a498d3ad5491a79c6deb604617378e1cdc4bfc1c1361fe2f87"
+dependencies = [
+ "console",
+ "shell-words",
+ "tempfile",
+ "zeroize",
+]
+
+[[package]]
 name = "digest"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
 dependencies = [
  "block-buffer",
  "crypto-common",
 ]
 
 [[package]]
+name = "dirs"
+version = "4.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca3aa72a6f96ea37bbc5aa912f6788242832f75369bdfdadcb0e38423f100059"
+dependencies = [
+ "dirs-sys",
+]
+
+[[package]]
+name = "dirs-sys"
+version = "0.3.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1b1d1d91c932ef41c0f2663aa8b0ca0342d444d842c06914aa0a7e352d0bada6"
+dependencies = [
+ "libc",
+ "redox_users",
+ "winapi",
+]
+
+[[package]]
 name = "docker-api"
 version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "522a3ae33cf4fc165de192eb9c563b755bc43cda9bd6f442b2d511b84514b917"
 dependencies = [
  "asynchronous-codec",
- "base64",
+ "base64 0.13.1",
  "byteorder",
  "bytes",
  "chrono",
  "containers-api",
  "docker-api-stubs",
  "futures-util",
  "http",
@@ -499,33 +565,78 @@
  "pythonize",
  "serde",
  "tar",
  "tokio",
 ]
 
 [[package]]
+name = "encode_unicode"
+version = "0.3.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a357d28ed41a50f9c765dbfe56cbc04a64e53e5fc58ba79fbc34c10ef3df831f"
+
+[[package]]
+name = "encoding_rs"
+version = "0.8.32"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "071a31f4ee85403370b58aca746f01041ede6f0da2730960ad001edc2b71b394"
+dependencies = [
+ "cfg-if",
+]
+
+[[package]]
+name = "errno"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
+dependencies = [
+ "errno-dragonfly",
+ "libc",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "errno-dragonfly"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
+dependencies = [
+ "cc",
+ "libc",
+]
+
+[[package]]
 name = "eyre"
 version = "0.6.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c2b6b5a29c02cdc822728b7d7b8ae1bab3e3b05d44522770ddd49722eeac7eb"
 dependencies = [
  "indenter",
  "once_cell",
 ]
 
 [[package]]
+name = "fastrand"
+version = "1.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
+dependencies = [
+ "instant",
+]
+
+[[package]]
 name = "filetime"
 version = "0.2.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a3de6e8d11b22ff9edc6d916f890800597d60f8b2da1caf2955c274638d6412"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
- "windows-sys",
+ "redox_syscall 0.2.16",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "flate2"
 version = "1.0.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8a2db397cb1c8772f31494cb8917e48cd1e64f0fa7efac59fbd741a0a8ce841"
@@ -677,14 +788,28 @@
  "log",
  "openssl-probe",
  "openssl-sys",
  "url",
 ]
 
 [[package]]
+name = "git2_credentials"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32dcdcdc9d3a11a13e707af87bdd130ad6b3878ff64ae0053e95e0f42e3a7bcb"
+dependencies = [
+ "dialoguer",
+ "dirs",
+ "git2",
+ "pest",
+ "pest_derive",
+ "regex",
+]
+
+[[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "globset"
@@ -707,14 +832,33 @@
 dependencies = [
  "bitflags",
  "ignore",
  "walkdir",
 ]
 
 [[package]]
+name = "h2"
+version = "0.3.20"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "97ec8491ebaf99c8eaa73058b045fe58073cd6be7f596ac993ced0b0a0c01049"
+dependencies = [
+ "bytes",
+ "fnv",
+ "futures-core",
+ "futures-sink",
+ "futures-util",
+ "http",
+ "indexmap",
+ "slab",
+ "tokio",
+ "tokio-util",
+ "tracing",
+]
+
+[[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
 name = "heck"
@@ -737,14 +881,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "hermit-abi"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
+
+[[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
 name = "home"
@@ -807,28 +957,42 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5e011372fa0b68db8350aa7a248930ecc7839bf46d8485577d69f117a75f164c"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
+ "h2",
  "http",
  "http-body",
  "httparse",
  "httpdate",
  "itoa",
  "pin-project-lite",
  "socket2",
  "tokio",
  "tower-service",
  "tracing",
  "want",
 ]
 
 [[package]]
+name = "hyper-tls"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d6183ddfa99b85da61a140bea0efc93fdf56ceaa041b37d553518030827f9905"
+dependencies = [
+ "bytes",
+ "hyper",
+ "native-tls",
+ "tokio",
+ "tokio-native-tls",
+]
+
+[[package]]
 name = "hyperlocal"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fafdf7b2b2de7c9784f76e02c0935e65a8117ec3b768644379983ab333ac98c"
 dependencies = [
  "futures-util",
  "hex",
@@ -914,14 +1078,40 @@
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
+name = "instant"
+version = "0.1.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
+dependencies = [
+ "cfg-if",
+]
+
+[[package]]
+name = "io-lifetimes"
+version = "1.0.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
+dependencies = [
+ "hermit-abi 0.3.2",
+ "libc",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "ipnet"
+version = "2.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "28b29a3cd74f0f4598934efe3aeba42bae0eb4680554128851ebbecb02af14e6"
+
+[[package]]
 name = "itoa"
 version = "1.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fad582f4b9e86b6caa621cabeb0963332d92eea04729ab12892c2533951e6440"
 
 [[package]]
 name = "jobserver"
@@ -945,17 +1135,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "libgit2-sys"
 version = "0.14.2+1.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f3d95f6b51075fe9810a7ae22c7095f12b98005ab364d8544797a825ce946a4"
 dependencies = [
@@ -1005,14 +1195,20 @@
 [[package]]
 name = "linked-hash-map"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
 
 [[package]]
+name = "linux-raw-sys"
+version = "0.3.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
+
+[[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
  "autocfg",
  "scopeguard",
@@ -1095,15 +1291,33 @@
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b9d9a46eff5b4ff64b45a9e316a6d1e0bc719ef429cbec4dc630684212bfdf9"
 dependencies = [
  "libc",
  "log",
  "wasi 0.11.0+wasi-snapshot-preview1",
- "windows-sys",
+ "windows-sys 0.45.0",
+]
+
+[[package]]
+name = "native-tls"
+version = "0.2.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "07226173c32f2926027b63cce4bcd8076c3552846cbe7925f3aaffeac0a3b92e"
+dependencies = [
+ "lazy_static",
+ "libc",
+ "log",
+ "openssl",
+ "openssl-probe",
+ "openssl-sys",
+ "schannel",
+ "security-framework",
+ "security-framework-sys",
+ "tempfile",
 ]
 
 [[package]]
 name = "nom8"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ae01545c9c7fc4486ab7debaf2aad7003ac19431791868fb2e8066df97fad2f8"
@@ -1153,17 +1367,17 @@
 name = "once_cell"
 version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "openssl"
-version = "0.10.45"
+version = "0.10.55"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b102428fd03bc5edf97f62620f7298614c45cedf287c271e7ed450bbaf83f2e1"
+checksum = "345df152bc43501c5eb9e4654ff05f794effb78d4efe3d53abc158baddc0703d"
 dependencies = [
  "bitflags",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
@@ -1194,19 +1408,18 @@
 checksum = "1ef9a9cc6ea7d9d5e7c4a913dc4b48d0e359eddf01af1dfec96ba7064b4aba10"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.80"
+version = "0.9.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23bbbf7854cd45b83958ebe919f0e8e516793727652e27fda10a8384cfc790b7"
+checksum = "374533b0e45f3a7ced10fcaeccca020e66656bc03dac384f852e4e5a7a8104a6"
 dependencies = [
- "autocfg",
  "cc",
  "libc",
  "openssl-src",
  "pkg-config",
  "vcpkg",
 ]
 
@@ -1245,17 +1458,17 @@
 name = "parking_lot_core"
 version = "0.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "smallvec",
- "windows-sys",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "parse-zoneinfo"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c705f256449c60da65e11ff6626e0c16a0a0b96aaa348de61376b249bc340f41"
@@ -1527,14 +1740,34 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+dependencies = [
+ "bitflags",
+]
+
+[[package]]
+name = "redox_users"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
+dependencies = [
+ "getrandom",
+ "redox_syscall 0.2.16",
+ "thiserror",
+]
+
+[[package]]
 name = "regex"
 version = "1.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "48aaa5748ba571fb95cd2c85c09f629215d3a6ece942baa100950af03a34f733"
 dependencies = [
  "aho-corasick",
  "memchr",
@@ -1544,20 +1777,71 @@
 [[package]]
 name = "regex-syntax"
 version = "0.6.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
 
 [[package]]
+name = "reqwest"
+version = "0.11.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cde824a14b7c14f85caff81225f411faacc04a2013f41670f41443742b1c1c55"
+dependencies = [
+ "base64 0.21.2",
+ "bytes",
+ "encoding_rs",
+ "futures-core",
+ "futures-util",
+ "h2",
+ "http",
+ "http-body",
+ "hyper",
+ "hyper-tls",
+ "ipnet",
+ "js-sys",
+ "log",
+ "mime",
+ "native-tls",
+ "once_cell",
+ "percent-encoding",
+ "pin-project-lite",
+ "serde",
+ "serde_json",
+ "serde_urlencoded",
+ "tokio",
+ "tokio-native-tls",
+ "tower-service",
+ "url",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "web-sys",
+ "winreg",
+]
+
+[[package]]
 name = "rustc-demangle"
 version = "0.1.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ef03e0a2b150c7a90d01faf6254c9c48a41e95fb2a8c2ac1c6f0d2b9aefc342"
 
 [[package]]
+name = "rustix"
+version = "0.37.23"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4d69718bf81c6127a49dc64e44a742e8bb9213c0ff8869a22c308f84c1d4ab06"
+dependencies = [
+ "bitflags",
+ "errno",
+ "io-lifetimes",
+ "libc",
+ "linux-raw-sys",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "rustversion"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5583e89e108996506031660fe09baa5011b9dd0341b89029313006d1fb508d70"
 
 [[package]]
 name = "ryu"
@@ -1571,26 +1855,58 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
+name = "schannel"
+version = "0.1.22"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0c3733bf4cf7ea0880754e19cb5a462007c4a8c1914bff372ccc95b464f1df88"
+dependencies = [
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "scratch"
 version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ddccb15bcce173023b3fedd9436f882a0739b8dfb45e4f6b6002bee5929f61b2"
 
 [[package]]
+name = "security-framework"
+version = "2.9.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1fc758eb7bffce5b308734e9b0c1468893cae9ff70ebf13e7090be8dcbcc83a8"
+dependencies = [
+ "bitflags",
+ "core-foundation",
+ "core-foundation-sys",
+ "libc",
+ "security-framework-sys",
+]
+
+[[package]]
+name = "security-framework-sys"
+version = "2.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f51d0c0d83bec45f16480d0ce0058397a69e48fcdc52d1dc8855fb68acbd31a7"
+dependencies = [
+ "core-foundation-sys",
+ "libc",
+]
+
+[[package]]
 name = "serde"
 version = "1.0.152"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bb7d1f0d3021d347a83e556fc4683dea2ea09d87bccdf88ff5c12545d89d5efb"
 dependencies = [
  "serde_derive",
 ]
@@ -1633,20 +1949,32 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0efd8caf556a6cebd3b285caf480045fcc1ac04f6bd786b09a6f11af30c4fcf4"
 dependencies = [
  "serde",
 ]
 
 [[package]]
+name = "serde_urlencoded"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d3491c14715ca2294c4d6a88f15e84739788c1d030eed8c110436aafdaa2f3fd"
+dependencies = [
+ "form_urlencoded",
+ "itoa",
+ "ryu",
+ "serde",
+]
+
+[[package]]
 name = "serde_with"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "30d904179146de381af4c93d3af6ca4984b3152db687dacb9c3c35e86f39809c"
 dependencies = [
- "base64",
+ "base64 0.13.1",
  "chrono",
  "hex",
  "indexmap",
  "serde",
  "serde_json",
  "serde_with_macros",
  "time 0.3.20",
@@ -1693,14 +2021,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "900fba806f70c630b0a382d0d825e17a0f19fcd059a2ade1ff237bcddf446b31"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
+name = "shell-words"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "24188a676b6ae68c3b2cb3a01be17fbf7240ce009799bb56d5b1409051e78fde"
+
+[[package]]
 name = "siphasher"
 version = "0.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7bd3e3206899af3f8b12af284fafc038cc1dc2b41d1b89dd17297221c5d225de"
 
 [[package]]
 name = "slab"
@@ -1786,14 +2120,28 @@
 [[package]]
 name = "target-lexicon"
 version = "0.12.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
 
 [[package]]
+name = "tempfile"
+version = "3.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
+dependencies = [
+ "autocfg",
+ "cfg-if",
+ "fastrand",
+ "redox_syscall 0.3.5",
+ "rustix",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "tera"
 version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3df578c295f9ec044ff1c829daf31bb7581d5b3c2a7a3d87419afe1f2531438c"
 dependencies = [
  "chrono",
  "chrono-tz",
@@ -1855,15 +2203,15 @@
 [[package]]
 name = "thread-id"
 version = "4.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5fdfe0627923f7411a43ec9ec9c39c3a9b4151be313e0922042581fb6c9b717f"
 dependencies = [
  "libc",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "winapi",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1929,35 +2277,61 @@
 [[package]]
 name = "tokio"
 version = "1.26.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "03201d01c3c27a29c8a5cee5b55a93ddae1ccf6f08f65365c2c918f8c1b76f64"
 dependencies = [
  "autocfg",
+ "bytes",
  "libc",
+ "memchr",
  "mio",
  "num_cpus",
  "pin-project-lite",
  "socket2",
  "tokio-macros",
- "windows-sys",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "tokio-macros"
 version = "1.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d266c00fde287f55d3f1c3e96c500c362a2b8c695076ec180f27918820bc6df8"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
+name = "tokio-native-tls"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
+dependencies = [
+ "native-tls",
+ "tokio",
+]
+
+[[package]]
+name = "tokio-util"
+version = "0.7.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "806fe8c2c87eccc8b3267cbae29ed3ab2d0bd37fca70ab622e46aaa9375ddb7d"
+dependencies = [
+ "bytes",
+ "futures-core",
+ "futures-sink",
+ "pin-project-lite",
+ "tokio",
+ "tracing",
+]
+
+[[package]]
 name = "toml"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fb9d890e4dc9298b70f740f615f2e05b9db37dce531f6b24fb77ac993f9f217"
 dependencies = [
  "indexmap",
  "serde",
@@ -2202,14 +2576,20 @@
 [[package]]
 name = "version"
 version = "3.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3a449064fee414fcc201356a3e6c1510f6c8829ed28bb06b91c54ebe208ce065"
 
 [[package]]
+name = "version-compare"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "579a42fc0b8e0c63b76519a339be31bed574929511fa53c1a3acae26eb258f29"
+
+[[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walkdir"
@@ -2266,14 +2646,26 @@
  "proc-macro2",
  "quote",
  "syn",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
+name = "wasm-bindgen-futures"
+version = "0.4.34"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f219e0d211ba40266969f6dbdd90636da12f75bee4fc9d6c23d1260dadb51454"
+dependencies = [
+ "cfg-if",
+ "js-sys",
+ "wasm-bindgen",
+ "web-sys",
+]
+
+[[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c21f77c0bedc37fd5dc21f897894a5ca01e7bb159884559461862ae90c0b4c5"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
@@ -2295,14 +2687,24 @@
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0046fef7e28c3804e5e38bfa31ea2a0f73905319b677e57ebe37e49358989b5d"
 
 [[package]]
+name = "web-sys"
+version = "0.3.61"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e33b99f4b23ba3eec1a53ac264e35a755f00e966e0065077d6027c0f575b0b97"
+dependencies = [
+ "js-sys",
+ "wasm-bindgen",
+]
+
+[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
@@ -2331,75 +2733,150 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.42.1",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.1",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e2522491fbfcd58cc84d47aeb2958948c4b8982e9a2d8a2a35bbaed431390e7"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.1",
+ "windows_aarch64_msvc 0.42.1",
+ "windows_i686_gnu 0.42.1",
+ "windows_i686_msvc 0.42.1",
+ "windows_x86_64_gnu 0.42.1",
+ "windows_x86_64_gnullvm 0.42.1",
+ "windows_x86_64_msvc 0.42.1",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.42.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.42.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
 
 [[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
+name = "winreg"
+version = "0.10.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "80d0f4e272c85def139476380b12f9ac60926689dd2e01d4923222f40580869d"
+dependencies = [
+ "winapi",
+]
+
+[[package]]
 name = "xattr"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d1526bbe5aaeb5eb06885f4d987bcdfa5e23187055de9b83fe00156a821fabc"
 dependencies = [
  "libc",
 ]
@@ -2408,7 +2885,13 @@
 name = "yaml-rust"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56c1936c4cc7a1c9ab21a1ebb602eb942ba868cbd44a99cb7cdc5892335e1c85"
 dependencies = [
  "linked-hash-map",
 ]
+
+[[package]]
+name = "zeroize"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
```

### Comparing `angreal-2.0.6/PKG-INFO` & `angreal-2.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angreal
-Version: 2.0.6
+Version: 2.0.7
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
@@ -27,15 +27,15 @@
 [![image](https://img.shields.io/pypi/v/angreal.svg)](https://pypi.python.org/pypi/angreal)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/angreal)
 [![image](https://img.shields.io/pypi/l/angreal.svg)](https://pypi.python.org/pypi/angreal)
 [![Angreal Tests](https://github.com/angreal/angreal/actions/workflows/test.yaml/badge.svg?branch=main)](https://github.com/angreal/angreal/actions/workflows/test.yaml)
 [![Angreal Docs Deploy](https://github.com/angreal/angreal/actions/workflows/docs.yaml/badge.svg)](https://github.com/angreal/angreal/actions/workflows/docs.yaml)
 [![Angreal Release](https://github.com/angreal/angreal/actions/workflows/release.yaml/badge.svg?event=release)](https://github.com/angreal/angreal/actions/workflows/release.yaml)
 ---
-[Docs are available here.](https://angreal.github.io/angreal/) 
+[Docs are available here.](https://angreal.github.io/angreal/)
 
 ## Angreal is meant to:
 - allow the consistent creation of projects
 - provide consistent methods for interacting with projects
 
 ### Quick Start
 
@@ -43,15 +43,15 @@
 2.  Initialize a project from a template
 3.  Use the template
 
 ```bash
 $: pip install 'angreal>=2' #pip install angreal will also work
 $: angreal init https://github.com/angreal/python
 ```
---- 
+---
 
 
 ## What is it?
 
 Angreal is an attempt to solve two problems that I was running into in
 both my personal and professional life as a data scientist and software
 developer. I do things often enough that they needed automation, I
@@ -66,15 +66,15 @@
 of executing methods for interacting with that project in a consistent
 manner. These methods (called tasks) travel with the project so while
 templated initially, they\'re customizable to the project - allowing some
 level of flexibility in how a task functions between projects.
 
 ### Why 2.0 ?
 
-The original angreal was built ontop of a number of python modules that
+The original angreal was built on top of a number of python modules that
 were under active development and used by a number of other projects.
 The nature of the application itself meant that core application found
 itself in dependency hell regularly - and became rather annoying to use.
 The 2.0.0 release is a complete rewrite that uses
-[Rust](https://www.rust-lang.org/) to provide a compiled binary with the goal that it will 
+[Rust](https://www.rust-lang.org/) to provide a compiled binary with the goal that it will
 require no external python dependencies.
```

