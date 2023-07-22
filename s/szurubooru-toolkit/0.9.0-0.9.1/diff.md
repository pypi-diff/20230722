# Comparing `tmp/szurubooru_toolkit-0.9.0.tar.gz` & `tmp/szurubooru_toolkit-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "szurubooru_toolkit-0.9.0.tar", max compression
+gzip compressed data, was "szurubooru_toolkit-0.9.1.tar", max compression
```

## Comparing `szurubooru_toolkit-0.9.0.tar` & `szurubooru_toolkit-0.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2023-07-04 17:51:17.304553 szurubooru_toolkit-0.9.0/LICENSE
--rw-r--r--   0        0        0    23353 2023-07-04 17:51:17.304553 szurubooru_toolkit-0.9.0/README.md
--rw-r--r--   0        0        0     2625 2023-07-04 17:51:17.304553 szurubooru_toolkit-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1924 2023-07-04 17:51:17.304553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/__init__.py
--rw-r--r--   0        0        0     8965 2023-07-04 17:51:17.304553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/config.py
--rw-r--r--   0        0        0     5290 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/danbooru.py
--rw-r--r--   0        0        0     3716 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/deepbooru.py
--rw-r--r--   0        0        0     1604 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/gelbooru.py
--rw-r--r--   0        0        0     5773 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/saucenao.py
--rw-r--r--   0        0        0      453 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/__init__.py
--rw-r--r--   0        0        0    12824 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/auto_tagger.py
--rw-r--r--   0        0        0     7203 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/create_relations.py
--rw-r--r--   0        0        0     3544 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/create_tags.py
--rw-r--r--   0        0        0     2841 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/delete_posts.py
--rw-r--r--   0        0        0     6519 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/import_from_booru.py
--rw-r--r--   0        0        0     4044 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/import_from_twitter.py
--rw-r--r--   0        0        0     7058 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/import_from_url.py
--rw-r--r--   0        0        0     3314 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/reset_posts.py
--rw-r--r--   0        0        0     4713 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/tag_posts.py
--rw-r--r--   0        0        0    11103 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/upload_media.py
--rw-r--r--   0        0        0    12255 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/szurubooru.py
--rw-r--r--   0        0        0     7036 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/twitter.py
--rw-r--r--   0        0        0    19173 2023-07-04 17:51:17.308553 szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/utils.py
--rw-r--r--   0        0        0    24881 1970-01-01 00:00:00.000000 szurubooru_toolkit-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-22 13:45:44.687583 szurubooru_toolkit-0.9.1/LICENSE
+-rw-r--r--   0        0        0    24721 2023-07-22 13:45:44.687583 szurubooru_toolkit-0.9.1/README.md
+-rw-r--r--   0        0        0     2625 2023-07-22 13:45:44.691583 szurubooru_toolkit-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1924 2023-07-22 13:45:44.691583 szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/__init__.py
+-rw-r--r--   0        0        0     8965 2023-07-22 13:45:44.691583 szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/config.py
+-rw-r--r--   0        0        0     5414 2023-07-22 13:45:44.691583 szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/danbooru.py
+-rw-r--r--   0        0        0     3716 2023-07-22 13:45:44.691583 szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/deepbooru.py
+-rw-r--r--   0        0        0     1604 2023-07-22 13:45:44.691583 szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/gelbooru.py
+-rw-r--r--   0        0        0     6194 2023-07-22 13:45:44.691583 szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/saucenao.py
+-rw-r--r--   0        0        0      453 2023-07-22 13:45:44.691583 szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/scripts/__init__.py
+-rw-r--r--   0        0        0    12921 2023-07-22 13:45:44.691583 szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/scripts/auto_tagger.py
+-rw-r--r--   0        0        0     7174 2023-07-22 13:45:44.691583 szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/scripts/create_relations.py
+-rw-r--r--   0        0        0     3544 2023-07-22 13:45:44.691583 szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/scripts/create_tags.py
+-rw-r--r--   0        0        0     2841 2023-07-22 13:45:44.691583 szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/scripts/delete_posts.py
+-rw-r--r--   0        0        0     6519 2023-07-22 13:45:44.691583 szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/scripts/import_from_booru.py
+-rw-r--r--   0        0        0     4044 2023-07-22 13:45:44.691583 szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/scripts/import_from_twitter.py
+-rw-r--r--   0        0        0     7058 2023-07-22 13:45:44.691583 szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/scripts/import_from_url.py
+-rw-r--r--   0        0        0     3314 2023-07-22 13:45:44.691583 szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/scripts/reset_posts.py
+-rw-r--r--   0        0        0     4713 2023-07-22 13:45:44.691583 szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/scripts/tag_posts.py
+-rw-r--r--   0        0        0    11103 2023-07-22 13:45:44.691583 szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/scripts/upload_media.py
+-rw-r--r--   0        0        0    12255 2023-07-22 13:45:44.691583 szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/szurubooru.py
+-rw-r--r--   0        0        0     7036 2023-07-22 13:45:44.691583 szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/twitter.py
+-rw-r--r--   0        0        0    19600 2023-07-22 13:45:44.691583 szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/utils.py
+-rw-r--r--   0        0        0    26249 1970-01-01 00:00:00.000000 szurubooru_toolkit-0.9.1/PKG-INFO
```

### Comparing `szurubooru_toolkit-0.9.0/LICENSE` & `szurubooru_toolkit-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.9.0/README.md` & `szurubooru_toolkit-0.9.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 For Deepbooru support, download the current release [here](https://github.com/KichangKim/DeepDanbooru/releases/tag/v3-20211112-sgd-e28) (v3-20211112-sgd-e28) and extract the contents of the zip file. Specify the path of the folder with the extracted files in `deepbooru_model`.
 Please note that you have to set `deepbooru_enabled` if you want to use it.
 
 ## :page_with_curl: Scripts
 Following scripts are currently available:
 
 * `auto-tagger`: Batch tagging of posts with SauceNAO and Deepbooru
+* `create-relations`: Create relations between character and parody tag categories
 * `create-tags`: Batch creation of tags with their categories
 * `delete-posts`: Batch delete of posts
 * `import-from-booru`: Batch importing of posts with their tags from various Boorus
 * `import-from-twitter`: Batch importing of Twitter favorites
 * `import-from-url`: Batch importing of URLs based on [gallery-dl](https://github.com/mikf/gallery-dl)
 * `reset-posts`: Batch resetting of posts (remove tags and sources)
 * `upload-media`: Batch upload of media files from local source folder
@@ -160,28 +161,26 @@
 If no matches from SauceNAO were found, the script keeps the previously set tags of the post and additionally appends the tag `tagme`.
 
 You can set `deepbooru_enabled` to `true` in your config.toml file. In that case, the script falls back to tag posts with the supplied Deepbooru model.
 If you only want to use Deepbooru, set `deepbooru_enabled` to `true` and `saucenao_enabled` to `false`. If you want to use SauceNAO and Deepbooru, set following options to `true`: `saucenao_enabled`, `deepbooru_enabled` and `deepbooru_forced`.
 
 __Usage__
 ```
-usage: auto-tagger [-h] [--sankaku_url SANKAKU_URL] [--add-tags ADD_TAGS] [--remove-tags REMOVE_TAGS] query
+usage: auto-tagger [-h] [--add-tags ADD_TAGS] [--remove-tags REMOVE_TAGS] query
 
 This script will automagically tag your szurubooru posts based on your input query.
 
 positional arguments:
   query                 Specify a single post id to tag or a szuru query. E.g. "date:today tag-count:0"
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
-  --sankaku_url SANKAKU_URL
-                        Fetch tags from specified Sankaku URL instead of searching SauceNAO.
-  --add-tags ADD_TAGS   Specify tags, separated by a comma, which will be added to all posts matching your query
+  --add-tags ADD_TAGS   Specify tags, separated by a comma, which will be added to all posts matching your query.
   --remove-tags REMOVE_TAGS
-                        Specify tags, separated by a comma, which will be removed from all posts matching your query
+                        Specify tags, separated by a comma, which will be removed from all posts matching your query.
 ```
 
 __Examples__
 * `auto-tagger "date:today tag-count:0"`
 * `auto-tagger "date:2021-04-07"`
 * `auto-tagger "tagme"`
 * `auto-tagger "id:100..111"`
@@ -244,49 +243,56 @@
 * max_similarity
 * convert_to_jpg
 * convert_threshold
 * shrink
 * shrink_threshold
 * shrink_dimensions
 
-:information_source:️ **Following Boorus are currently supported:**
+:information_source:️ **The source URL will be generated for following sites:**
 * Gelbooru
 * Danbooru
-* Sankaku
+* E-Hentai
 * Konachan
+* Kemono
+* Sankaku
 * Yandere
 
 Credentials in your `config.toml` file will be passed to the gallery-dl script if you use a single input URL to this script.
 
+However, it's recommended to use the `--cookie` flag for authentication, check https://github.com/mikf/gallery-dl#cookies for details.
+
 __Usage__
 ```
-usage: import-from-url [-h] [--range RANGE] [--input-file INPUT_FILE] [url ...]
+usage: import-from-url [-h] [--range RANGE] [--input-file INPUT_FILE] [--cookies COOKIES] [urls ...]
 
 This script downloads and tags posts from various Boorus based on your input query.
 
 positional arguments:
-  url                   The URL for the posts you want to download and tag
+  urls                  One or multiple URLs to the posts you want to download and tag
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --range RANGE         Index range(s) specifying which files to download. These can be either a constant value, range, or slice (e.g. '5', '8-20', or '1:24:3')
   --input-file INPUT_FILE
                         Download URLs found in FILE.
-
+  --cookies COOKIES     Path to a cookies file for gallery-dl to consume. Used for authentication.
 ```
 
 __Examples__
 * `import-from-url "https://danbooru.donmai.us/posts?tags=foo"`
 * `import-from-url "https://chan.sankakucomplex.com/?tags=foo"`
 * `import-from-url "https://beta.sankakucomplex.com/post/show/<id>"`
+* `import-from-url --cookies "~/cookies.txt" --range ":100" ""https://twitter.com/<USERNAME>/likes"`
 * `import-from-url --input-file urls.txt "https://danbooru.donmai.us/posts?tags=foo" "https://beta.sankakucomplex.com/post/show/<id>"`
 
-### :dove: import-from-twitter
+### :dove: import-from-twitter (Deprecated)
 This script fetches media files from your Twitter likes, uploads and optionally tags them.
 
+:warning: __This script is deprecated. Use `import-from-url` instead.__
+
 :warning: __OAuth 1.0a credentials are required to read the likes from a user. See https://developer.twitter.com/en/docs/authentication/oauth-1-0a on how to generate them.__
 
 The `user_id` can be converted on sites like https://tweeterid.com/. If you configured above credentials, you can also get your own ID from the `access_token`, which is in following format: `<user_id>-<random_string>`
 
 In the `config.toml` file, you can set if the post should be additionally tagged with SauceNAO or Deepbooru and if the progress bar should be shown.
 Since this script is using the `upload-media` script to upload the post, following settings apply from the `upload-media` section:
 * max_similarity
@@ -420,9 +426,31 @@
 The category has to be created beforehand manually (e.g. default, artist, series, character and meta).
 
 __Examples__
 * `create-tags`
 * `create-tags --query genshin* --overwrite`
 * `create-tags --tag-file tags.txt`
 
+### :label: create-relations
+__Usage__
+```
+usage: create-relations [-h] [--hide-progress HIDE_PROGRESS] query
+
+Create relations between character and parody tag categories
+
+positional arguments:
+  query                 Search for specific tags (default: "*").
+
+options:
+  -h, --help            show this help message and exit
+  --hide-progress HIDE_PROGRESS
+                        Hide the progress bar.
+```
+
+__Examples__
+* `create-relations hitori_bocchi`
+  * Will create the implication _bocchi_the_rock_ for tag _hitori_bocchi_ if other posts are found with query _hitori_bocchi_ containing _bocchi_the_rock_ as the parody (tag has to be of category _series_ or _parody_)
+  * Will also add _hitori_bocchi_ as a suggestion to the parody tag _bocchi_the_rock_
+  * These relations will only get generated if at least X posts are found containing the tags _bocchi_the_rock_ and _hitori_bocchi_. Control X with `threshold` under `[create-relations]` in `config.toml`.
+
 ## :information_source:	Image credit
 GitHub repo icon: <a href="https://www.flaticon.com/free-icons/code" title="code icons">Code icons created by Smashicons - Flaticon</a>
```

### Comparing `szurubooru_toolkit-0.9.0/pyproject.toml` & `szurubooru_toolkit-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 check_untyped_defs = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 
 
 [tool.poetry]
 name = "szurubooru-toolkit"
-version = "0.9.0"
+version = "0.9.1"
 description = "Python package and script collection to manage szurubooru."
 authors = ["reluce <reluce@fkosquad.moe>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/reluce/szurubooru-toolkit"
 documentation = "https://github.com/reluce/szurubooru-toolkit"
 keywords = ["szurubooru", "szuru", "booru", "saucenao", "deepbooru"]
```

### Comparing `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/__init__.py` & `szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/config.py` & `szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/config.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/danbooru.py` & `szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/danbooru.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,17 +79,20 @@
 
         for _ in range(1, 12):
             try:
                 result = self.client.artist_list(artist.lower())
                 if result:
                     artist = result[0]['name']
                 else:
-                    artist = self.session.get(
-                        f'https://danbooru.donmai.us/artists.json?search[any_other_name_like]={artist.lower()}',
-                    ).json()[0]['name']
+                    search_url = (
+                        'https://danbooru.donmai.us/artists.json?'
+                        f'search[any_other_name_like]={artist.lower()}'
+                        '&search[is_deleted]=false'
+                    )
+                    artist = self.session.get(search_url).json()[0]['name']
                     self.session.close()
 
                 logger.debug(f'Returning artist: {artist}')
 
                 break
             except (IndexError, KeyError):
                 logger.debug(f'Could not find artist "{artist.lower()}"')
```

### Comparing `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/deepbooru.py` & `szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/deepbooru.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/gelbooru.py` & `szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/gelbooru.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/saucenao.py` & `szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/saucenao.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,44 +74,55 @@
             'gelbooru': None,
             'yande': None,
             'konachan': None,
             'sankakucomplex': None,
             'pixiv': None,
         }
 
-        if response and not response == 'Limit reached':
+        if response and response != 'Limit reached':
             site_keys = {
                 'pixiv': 'pixiv',
                 'donmai': 'danbooru',
                 'gelbooru': 'gelbooru',
                 'yande': 'yandere',
                 'konachan': 'konachan',
                 'sankakucomplex': 'sankaku',
             }
 
             for result in response:
-                for url in result.urls:
-                    site = self.get_base_domain(url)
-                    post_id = re.findall(r'\b\d+\b', url)
-                    if site in matches and not matches[site]:
-                        logger.debug(f'Found result on {site.capitalize()}')
-                        if site == 'pixiv':
-                            matches[site] = result
-                        elif site in site_keys:
-                            matches[site] = {'site': site_keys[site], 'post_id': int(post_id[0])} if post_id else None
-                        else:
-                            continue
+                if result.urls:
+                    for url in result.urls:
+                        site = self.get_base_domain(url)
+                        post_id = re.findall(r'\b\d+\b', url)
+                        if site in matches and not matches[site]:
+                            logger.debug(f'Found result on {site.capitalize()}')
+                            if site == 'pixiv':
+                                matches[site] = result
+                            elif site in site_keys:
+                                matches[site] = (
+                                    {'site': site_keys[site], 'post_id': int(post_id[0])} if post_id else None
+                                )
+                            else:
+                                continue
 
             logger.debug(f'Limit short: {response.short_remaining}')
             logger.debug(f'Limit long: {response.long_remaining}')
 
+        # Even if response evaluates to False, it can still contain the limits
+        try:
+            short_remaining = response.short_remaining
+            long_remaining = response.long_remaining
+        except AttributeError:
+            short_remaining = 1
+            long_remaining = 1
+
         if response == 'Limit reached':
             response.long_remaining = 0
 
-        return matches, response.short_remaining, response.long_remaining
+        return matches, short_remaining, long_remaining
 
     async def get_result(self, content_url: str, image: bytes = None) -> Coroutine | None:
         for attempt in range(self.retry_attempts):
             try:
                 if image:
                     logger.debug('Trying to get result from uploaded file...')
                     response = await self.pysaucenao.from_file(BytesIO(image))
```

### Comparing `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/auto_tagger.py` & `szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/scripts/auto_tagger.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,34 +278,35 @@
                 if result is None:
                     continue
 
                 tags_by_deepbooru, post.safety = result
 
                 # Deepbooru detects characters, but not the parody.
                 # Set the parody based on the character if configured.
-                if (not config.auto_tagger['saucenao_enabled'] or limit_reached) and config.auto_tagger[
-                    'update_relations'
-                ]:
+                # Only do this if no previous tags where found as this operation takes quite some time
+                if not tags_by_md5 and not tags_by_sauce and config.auto_tagger['update_relations']:
                     for tag in tags_by_deepbooru:
                         szuru_tag = szuru.api.getTag(tag)
                         for implication in szuru_tag.implications:
                             szuru_implication = szuru.api.getTag(implication)
                             if szuru_implication not in post.tags:
                                 post.tags.append(szuru_implication.primary_name)
 
                 if post.relations:
                     set_tags_from_relations(post)
             else:
                 tags_by_deepbooru = []
 
             # Keep previous tags and add user tags if configured
             if add_tags:
-                post.tags = list(set().union(post.tags, tags_by_md5, tags_by_sauce, tags_by_deepbooru, add_tags))
+                tags = list(set().union(post.tags, tags_by_md5, tags_by_sauce, tags_by_deepbooru, add_tags))
             else:
-                post.tags = list(set().union(post.tags, tags_by_md5, tags_by_sauce, tags_by_deepbooru))
+                tags = list(set().union(post.tags, tags_by_md5, tags_by_sauce, tags_by_deepbooru))
+
+            post.tags = [tag for tag in tags if tag is not None]
 
             if remove_tags:
                 [post.tags.remove(tag) for tag in remove_tags if tag in post.tags]
 
             # If any tags were collected, remove tagme and deepbooru tag
             if tags_by_md5 or tags_by_sauce or tags_by_deepbooru:
                 [post.tags.remove(tag) for tag in post.tags if tag == 'tagme']
```

### Comparing `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/create_relations.py` & `szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/scripts/create_relations.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,20 +63,20 @@
     Returns:
         None
     """
 
     # Add parody/series tag as an implication for character tags
     if tag.category == 'character' and relation.category in ['parody', 'series']:
         if relation.primary_name not in [implication.primary_name for implication in tag.implications]:
-            tag.implications = tag.implications + [relation]
+            tag.implications.append(relation)
             tag.push()
     # Add character tags as a suggestion to parody/series tags
     elif tag.category in ['parody', 'series'] and relation.category == 'character':
         if relation.primary_name not in [suggestion.primary_name for suggestion in tag.suggestions]:
-            tag.suggestions = tag.suggestions + [relation]
+            tag.suggestions.append(relation)
             tag.push()
 
 
 def evaluate_relations(tag: Tag, relation: Tag, found_relations: dict) -> None:
     """Evaluate if the tag relation is valid.
 
     This is done by searching the possible relation of two tags on szurubooru.
```

### Comparing `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/create_tags.py` & `szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/scripts/create_tags.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/delete_posts.py` & `szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/scripts/delete_posts.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/import_from_booru.py` & `szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/scripts/import_from_booru.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/import_from_twitter.py` & `szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/scripts/import_from_twitter.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/import_from_url.py` & `szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/scripts/import_from_url.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/reset_posts.py` & `szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/scripts/reset_posts.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/tag_posts.py` & `szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/scripts/tag_posts.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/scripts/upload_media.py` & `szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/scripts/upload_media.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/szurubooru.py` & `szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/szurubooru.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/twitter.py` & `szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/twitter.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.9.0/src/szurubooru_toolkit/utils.py` & `szurubooru_toolkit-0.9.1/src/szurubooru_toolkit/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -552,17 +552,29 @@
     pixiv_artist = result.author_name
     source = result.url
     from szurubooru_toolkit import config
     from szurubooru_toolkit import danbooru_client
     from szurubooru_toolkit import szuru
 
     if pixiv_artist:
-        artist = danbooru_client.search_artist(pixiv_artist)
-        if not artist and config.auto_tagger['use_pixiv_artist']:
-            artist = pixiv_artist.lower().replace(' ', '_')
+        artist_danbooru = danbooru_client.search_artist(pixiv_artist)
+
+        artist_pixiv_sanitized = pixiv_artist.lower().replace(' ', '_')
+        # Sometimes \3000 gets appended from the result for whatever reason
+        artist_pixiv_sanitized = artist_pixiv_sanitized.replace('\u3000', '')
+
+        if not artist_danbooru:
+            artist_danbooru = danbooru_client.search_artist(artist_pixiv_sanitized)
+
+        if artist_danbooru:
+            artist = artist_danbooru
+        else:
+            artist = artist_pixiv_sanitized
+
+        if not artist_danbooru and config.auto_tagger['use_pixiv_artist']:
             try:
                 szuru.create_tag(artist, category='artist', overwrite=True)
             except Exception as e:
                 logger.debug(f'Could not create pixiv artist {pixiv_artist}: {e}')
     else:
         artist = None
```

### Comparing `szurubooru_toolkit-0.9.0/PKG-INFO` & `szurubooru_toolkit-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: szurubooru-toolkit
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python package and script collection to manage szurubooru.
 Home-page: https://github.com/reluce/szurubooru-toolkit
 License: GPL-3.0-only
 Keywords: szurubooru,szuru,booru,saucenao,deepbooru
 Author: reluce
 Author-email: reluce@fkosquad.moe
 Requires-Python: >=3.11,<3.12
@@ -172,14 +172,15 @@
 For Deepbooru support, download the current release [here](https://github.com/KichangKim/DeepDanbooru/releases/tag/v3-20211112-sgd-e28) (v3-20211112-sgd-e28) and extract the contents of the zip file. Specify the path of the folder with the extracted files in `deepbooru_model`.
 Please note that you have to set `deepbooru_enabled` if you want to use it.
 
 ## :page_with_curl: Scripts
 Following scripts are currently available:
 
 * `auto-tagger`: Batch tagging of posts with SauceNAO and Deepbooru
+* `create-relations`: Create relations between character and parody tag categories
 * `create-tags`: Batch creation of tags with their categories
 * `delete-posts`: Batch delete of posts
 * `import-from-booru`: Batch importing of posts with their tags from various Boorus
 * `import-from-twitter`: Batch importing of Twitter favorites
 * `import-from-url`: Batch importing of URLs based on [gallery-dl](https://github.com/mikf/gallery-dl)
 * `reset-posts`: Batch resetting of posts (remove tags and sources)
 * `upload-media`: Batch upload of media files from local source folder
@@ -197,28 +198,26 @@
 If no matches from SauceNAO were found, the script keeps the previously set tags of the post and additionally appends the tag `tagme`.
 
 You can set `deepbooru_enabled` to `true` in your config.toml file. In that case, the script falls back to tag posts with the supplied Deepbooru model.
 If you only want to use Deepbooru, set `deepbooru_enabled` to `true` and `saucenao_enabled` to `false`. If you want to use SauceNAO and Deepbooru, set following options to `true`: `saucenao_enabled`, `deepbooru_enabled` and `deepbooru_forced`.
 
 __Usage__
 ```
-usage: auto-tagger [-h] [--sankaku_url SANKAKU_URL] [--add-tags ADD_TAGS] [--remove-tags REMOVE_TAGS] query
+usage: auto-tagger [-h] [--add-tags ADD_TAGS] [--remove-tags REMOVE_TAGS] query
 
 This script will automagically tag your szurubooru posts based on your input query.
 
 positional arguments:
   query                 Specify a single post id to tag or a szuru query. E.g. "date:today tag-count:0"
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
-  --sankaku_url SANKAKU_URL
-                        Fetch tags from specified Sankaku URL instead of searching SauceNAO.
-  --add-tags ADD_TAGS   Specify tags, separated by a comma, which will be added to all posts matching your query
+  --add-tags ADD_TAGS   Specify tags, separated by a comma, which will be added to all posts matching your query.
   --remove-tags REMOVE_TAGS
-                        Specify tags, separated by a comma, which will be removed from all posts matching your query
+                        Specify tags, separated by a comma, which will be removed from all posts matching your query.
 ```
 
 __Examples__
 * `auto-tagger "date:today tag-count:0"`
 * `auto-tagger "date:2021-04-07"`
 * `auto-tagger "tagme"`
 * `auto-tagger "id:100..111"`
@@ -281,49 +280,56 @@
 * max_similarity
 * convert_to_jpg
 * convert_threshold
 * shrink
 * shrink_threshold
 * shrink_dimensions
 
-:information_source:️ **Following Boorus are currently supported:**
+:information_source:️ **The source URL will be generated for following sites:**
 * Gelbooru
 * Danbooru
-* Sankaku
+* E-Hentai
 * Konachan
+* Kemono
+* Sankaku
 * Yandere
 
 Credentials in your `config.toml` file will be passed to the gallery-dl script if you use a single input URL to this script.
 
+However, it's recommended to use the `--cookie` flag for authentication, check https://github.com/mikf/gallery-dl#cookies for details.
+
 __Usage__
 ```
-usage: import-from-url [-h] [--range RANGE] [--input-file INPUT_FILE] [url ...]
+usage: import-from-url [-h] [--range RANGE] [--input-file INPUT_FILE] [--cookies COOKIES] [urls ...]
 
 This script downloads and tags posts from various Boorus based on your input query.
 
 positional arguments:
-  url                   The URL for the posts you want to download and tag
+  urls                  One or multiple URLs to the posts you want to download and tag
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --range RANGE         Index range(s) specifying which files to download. These can be either a constant value, range, or slice (e.g. '5', '8-20', or '1:24:3')
   --input-file INPUT_FILE
                         Download URLs found in FILE.
-
+  --cookies COOKIES     Path to a cookies file for gallery-dl to consume. Used for authentication.
 ```
 
 __Examples__
 * `import-from-url "https://danbooru.donmai.us/posts?tags=foo"`
 * `import-from-url "https://chan.sankakucomplex.com/?tags=foo"`
 * `import-from-url "https://beta.sankakucomplex.com/post/show/<id>"`
+* `import-from-url --cookies "~/cookies.txt" --range ":100" ""https://twitter.com/<USERNAME>/likes"`
 * `import-from-url --input-file urls.txt "https://danbooru.donmai.us/posts?tags=foo" "https://beta.sankakucomplex.com/post/show/<id>"`
 
-### :dove: import-from-twitter
+### :dove: import-from-twitter (Deprecated)
 This script fetches media files from your Twitter likes, uploads and optionally tags them.
 
+:warning: __This script is deprecated. Use `import-from-url` instead.__
+
 :warning: __OAuth 1.0a credentials are required to read the likes from a user. See https://developer.twitter.com/en/docs/authentication/oauth-1-0a on how to generate them.__
 
 The `user_id` can be converted on sites like https://tweeterid.com/. If you configured above credentials, you can also get your own ID from the `access_token`, which is in following format: `<user_id>-<random_string>`
 
 In the `config.toml` file, you can set if the post should be additionally tagged with SauceNAO or Deepbooru and if the progress bar should be shown.
 Since this script is using the `upload-media` script to upload the post, following settings apply from the `upload-media` section:
 * max_similarity
@@ -457,10 +463,32 @@
 The category has to be created beforehand manually (e.g. default, artist, series, character and meta).
 
 __Examples__
 * `create-tags`
 * `create-tags --query genshin* --overwrite`
 * `create-tags --tag-file tags.txt`
 
+### :label: create-relations
+__Usage__
+```
+usage: create-relations [-h] [--hide-progress HIDE_PROGRESS] query
+
+Create relations between character and parody tag categories
+
+positional arguments:
+  query                 Search for specific tags (default: "*").
+
+options:
+  -h, --help            show this help message and exit
+  --hide-progress HIDE_PROGRESS
+                        Hide the progress bar.
+```
+
+__Examples__
+* `create-relations hitori_bocchi`
+  * Will create the implication _bocchi_the_rock_ for tag _hitori_bocchi_ if other posts are found with query _hitori_bocchi_ containing _bocchi_the_rock_ as the parody (tag has to be of category _series_ or _parody_)
+  * Will also add _hitori_bocchi_ as a suggestion to the parody tag _bocchi_the_rock_
+  * These relations will only get generated if at least X posts are found containing the tags _bocchi_the_rock_ and _hitori_bocchi_. Control X with `threshold` under `[create-relations]` in `config.toml`.
+
 ## :information_source:	Image credit
 GitHub repo icon: <a href="https://www.flaticon.com/free-icons/code" title="code icons">Code icons created by Smashicons - Flaticon</a>
```

