# Comparing `tmp/wwt_api_client-0.3.0.tar.gz` & `tmp/wwt_api_client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwt_api_client-0.3.0.tar", last modified: Fri Mar 31 02:38:44 2023, max compression
+gzip compressed data, was "wwt_api_client-0.4.0.tar", last modified: Fri Jul 21 22:08:14 2023, max compression
```

## Comparing `wwt_api_client-0.3.0.tar` & `wwt_api_client-0.4.0.tar`

### file list

```diff
@@ -1,107 +1,138 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-31 02:38:44.947285 wwt_api_client-0.3.0/
--rw-r--r--   0 vsts      (1001) docker     (123)      175 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/.coveragerc
--rw-r--r--   0 vsts      (1001) docker     (123)      364 2023-03-31 02:38:01.000000 wwt_api_client-0.3.0/CHANGELOG.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1040 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      208 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     1334 2023-03-31 02:38:44.947285 wwt_api_client-0.3.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     3794 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-31 02:38:44.939285 wwt_api_client-0.3.0/docs/
--rw-r--r--   0 vsts      (1001) docker     (123)        9 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (123)      618 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/Makefile
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-31 02:38:44.939285 wwt_api_client-0.3.0/docs/_static/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/_static/.gitignore
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-31 02:38:44.943285 wwt_api_client-0.3.0/docs/api/
--rw-r--r--   0 vsts      (1001) docker     (123)      486 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.APIRequest.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      106 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.APIResponseError.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      493 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.Client.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      115 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.InvalidRequestError.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      670 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.LoginRequest.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     1290 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.ShowImageRequest.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     1140 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.TileImageRequest.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      151 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.communities.CommunitiesAPIRequest.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      798 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.communities.CommunitiesClient.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      574 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.communities.CreateCommunityRequest.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      564 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.communities.DeleteCommunityRequest.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      570 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.communities.GetCommunityInfoRequest.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      422 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.communities.GetLatestCommunityRequest.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      392 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.communities.GetMyProfileRequest.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      756 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.communities.GetProfileEntitiesRequest.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      412 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.communities.IsUserRegisteredRequest.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      156 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.communities.interactive_communities_login.rst
--rw-r--r--   0 vsts      (1001) docker     (123)       97 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.communities.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      338 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.ClientConfig.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      289 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.CxClient.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      490 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.data.HandleInfo.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      538 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.data.ImageDisplayInfo.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      506 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.data.ImageStorage.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      506 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.data.ImageSummary.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      474 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.data.ImageWwt.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      506 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.data.SceneContent.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      570 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.data.SceneContentHydrated.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      530 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.data.SceneImageLayer.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      594 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.data.SceneImageLayerHydrated.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      490 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.data.ScenePlace.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      105 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.data.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.handles.AddImageRequest.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.handles.AddSceneRequest.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      504 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.handles.HandleClient.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.handles.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      438 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.images.ImageClient.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      107 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.images.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      100 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      540 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.scenes.GetSceneResponse.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      466 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.scenes.SceneClient.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      107 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.scenes.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     1713 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.enums.CategoryType.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      446 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.enums.CommunityType.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      781 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.enums.ContentType.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      479 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.enums.EntityType.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      584 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.enums.HighlightType.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.enums.PermissionsTab.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      667 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.enums.UserRole.rst
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.enums.rst
--rw-r--r--   0 vsts      (1001) docker     (123)       85 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/api/wwt_api_client.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     1582 2023-03-31 02:38:01.000000 wwt_api_client-0.3.0/docs/conf.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-31 02:38:44.935284 wwt_api_client-0.3.0/docs/endpoints/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-31 02:38:44.943285 wwt_api_client-0.3.0/docs/endpoints/constellations/
--rw-r--r--   0 vsts      (1001) docker     (123)      523 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/endpoints/constellations/get-handle-_handle.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      670 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/endpoints/constellations/get-image-_id-img_wtml.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      775 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/endpoints/constellations/get-scene-_id-place_wtml.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     2569 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/endpoints/constellations/get-scene-_id.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     1549 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/endpoints/constellations/post-handle-_handle-image.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     1792 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/endpoints/constellations/post-handle-_handle-scene.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     1277 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/endpoints/constellations/post-images-find-by-legacy-url.rst
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-31 02:38:44.947285 wwt_api_client-0.3.0/docs/endpoints/legacy/
--rw-r--r--   0 vsts      (1001) docker     (123)     3872 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/endpoints/legacy/login.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     6076 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/endpoints/legacy/show-image.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     8750 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/endpoints/legacy/tile-image.rst
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-31 02:38:44.947285 wwt_api_client-0.3.0/docs/images/
--rw-r--r--   0 vsts      (1001) docker     (123)   272620 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/images/logo.png
--rw-r--r--   0 vsts      (1001) docker     (123)     3049 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/index.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      732 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/installation.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      787 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/docs/make.bat
--rw-r--r--   0 vsts      (1001) docker     (123)       54 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (123)       31 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/pytest.ini
--rw-r--r--   0 vsts      (1001) docker     (123)      109 2023-03-31 02:38:44.947285 wwt_api_client-0.3.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     2501 2023-03-31 02:38:01.000000 wwt_api_client-0.3.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-31 02:38:44.947285 wwt_api_client-0.3.0/wwt_api_client/
--rw-r--r--   0 vsts      (1001) docker     (123)    26359 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/wwt_api_client/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    23020 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/wwt_api_client/communities.py
--rw-r--r--   0 vsts      (1001) docker     (123)      113 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/wwt_api_client/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-31 02:38:44.947285 wwt_api_client-0.3.0/wwt_api_client/constellations/
--rw-r--r--   0 vsts      (1001) docker     (123)     9628 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/wwt_api_client/constellations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2635 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/wwt_api_client/constellations/data.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6525 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/wwt_api_client/constellations/handles.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1888 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/wwt_api_client/constellations/images.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3258 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/wwt_api_client/constellations/scenes.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2171 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/wwt_api_client/enums.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-31 02:38:44.947285 wwt_api_client-0.3.0/wwt_api_client/tests/
--rw-r--r--   0 vsts      (1001) docker     (123)      178 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/wwt_api_client/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9654 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/wwt_api_client/tests/test_communities.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10749 2023-03-31 02:37:59.000000 wwt_api_client-0.3.0/wwt_api_client/tests/test_core.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-31 02:38:44.947285 wwt_api_client-0.3.0/wwt_api_client.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     1334 2023-03-31 02:38:44.000000 wwt_api_client-0.3.0/wwt_api_client.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4081 2023-03-31 02:38:44.000000 wwt_api_client-0.3.0/wwt_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-03-31 02:38:44.000000 wwt_api_client-0.3.0/wwt_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      196 2023-03-31 02:38:44.000000 wwt_api_client-0.3.0/wwt_api_client.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       15 2023-03-31 02:38:44.000000 wwt_api_client-0.3.0/wwt_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-21 22:08:14.049127 wwt_api_client-0.4.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)      175 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/.coveragerc
+-rw-r--r--   0 vsts      (1001) docker     (123)      466 2023-07-21 22:07:37.000000 wwt_api_client-0.4.0/CHANGELOG.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1040 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)      208 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     1334 2023-07-21 22:08:14.049127 wwt_api_client-0.4.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     3794 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-21 22:08:14.025127 wwt_api_client-0.4.0/docs/
+-rw-r--r--   0 vsts      (1001) docker     (123)        9 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (123)      618 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/Makefile
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-21 22:08:14.025127 wwt_api_client-0.4.0/docs/_static/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/_static/.gitignore
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-21 22:08:14.037127 wwt_api_client-0.4.0/docs/api/
+-rw-r--r--   0 vsts      (1001) docker     (123)      486 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.APIRequest.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      106 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.APIResponseError.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      493 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.Client.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      115 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.InvalidRequestError.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      670 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.LoginRequest.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     1290 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.ShowImageRequest.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     1140 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.TileImageRequest.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      151 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.communities.CommunitiesAPIRequest.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      798 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.communities.CommunitiesClient.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      574 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.communities.CreateCommunityRequest.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      564 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.communities.DeleteCommunityRequest.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      570 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.communities.GetCommunityInfoRequest.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      422 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.communities.GetLatestCommunityRequest.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      392 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.communities.GetMyProfileRequest.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      756 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.communities.GetProfileEntitiesRequest.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      412 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.communities.IsUserRegisteredRequest.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      156 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.communities.interactive_communities_login.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)       97 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.communities.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      338 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.ClientConfig.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      628 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.CxClient.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      538 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.HandleImageStats.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      490 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.HandleInfo.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      546 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.HandlePermissions.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      538 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.HandleSceneStats.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      498 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.HandleStats.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      506 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.HandleUpdate.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      562 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.ImageApiPermissions.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      594 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.ImageContentPermissions.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      538 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.ImageDisplayInfo.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      482 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.ImageInfo.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      506 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.ImageStorage.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      506 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.ImageSummary.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      498 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.ImageUpdate.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      474 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.ImageWwt.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      506 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.SceneContent.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      570 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.SceneContentHydrated.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      514 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.SceneHydrated.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      530 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.SceneImageLayer.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      594 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.SceneImageLayerHydrated.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      482 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.SceneInfo.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      538 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.ScenePermissions.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      490 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.ScenePlace.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      514 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.ScenePreviews.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      498 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.SceneUpdate.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      105 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.handles.AddImageRequest.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.handles.AddSceneRequest.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      905 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.handles.HandleClient.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.handles.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      598 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.images.ImageClient.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      107 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.images.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      100 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      580 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.scenes.SceneClient.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      107 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.scenes.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     1713 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.enums.CategoryType.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      446 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.enums.CommunityType.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      781 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.enums.ContentType.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      479 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.enums.EntityType.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      584 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.enums.HighlightType.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.enums.PermissionsTab.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      667 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.enums.UserRole.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.enums.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)       85 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/api/wwt_api_client.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     1582 2023-07-21 22:07:37.000000 wwt_api_client-0.4.0/docs/conf.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-21 22:08:14.021127 wwt_api_client-0.4.0/docs/endpoints/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-21 22:08:14.045127 wwt_api_client-0.4.0/docs/endpoints/constellations/
+-rw-r--r--   0 vsts      (1001) docker     (123)      755 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/delete-scene-_id-likes.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     1576 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/get-handle-_handle-imageinfo.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     1237 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/get-handle-_handle-permissions.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     1499 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/get-handle-_handle-sceneinfo.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     1001 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/get-handle-_handle-stats.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      936 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/get-handle-_handle-timeline.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      523 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/get-handle-_handle.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      670 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/get-image-_id-img_wtml.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     1195 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/get-image-_id-permissions.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     1954 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/get-image-_id.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     1057 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/get-images-builtin-backgrounds.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     1195 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/get-scene-_id-permissions.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      775 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/get-scene-_id-place_wtml.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     2284 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/get-scene-_id.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      848 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/get-scenes-home-timeline.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      788 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/patch-handle-_handle.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      998 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/patch-image-_id.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      981 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/patch-scene-_id.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     3357 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/post-handle-_handle-image.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     1885 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/post-handle-_handle-scene.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     1277 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/post-images-find-by-legacy-url.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      759 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/post-scene-_id-impressions.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      748 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/post-scene-_id-likes.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/constellations/post-session-init.rst
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-21 22:08:14.045127 wwt_api_client-0.4.0/docs/endpoints/legacy/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3872 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/legacy/login.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     6076 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/legacy/show-image.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     8750 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/endpoints/legacy/tile-image.rst
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-21 22:08:14.045127 wwt_api_client-0.4.0/docs/images/
+-rw-r--r--   0 vsts      (1001) docker     (123)   272620 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/images/logo.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     3931 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      732 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/installation.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      787 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/docs/make.bat
+-rw-r--r--   0 vsts      (1001) docker     (123)       54 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)       31 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/pytest.ini
+-rw-r--r--   0 vsts      (1001) docker     (123)      109 2023-07-21 22:08:14.049127 wwt_api_client-0.4.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2564 2023-07-21 22:07:37.000000 wwt_api_client-0.4.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-21 22:08:14.045127 wwt_api_client-0.4.0/wwt_api_client/
+-rw-r--r--   0 vsts      (1001) docker     (123)    26359 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/wwt_api_client/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    23020 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/wwt_api_client/communities.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      113 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/wwt_api_client/conftest.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-21 22:08:14.045127 wwt_api_client-0.4.0/wwt_api_client/constellations/
+-rw-r--r--   0 vsts      (1001) docker     (123)    11558 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/wwt_api_client/constellations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6631 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/wwt_api_client/constellations/data.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17994 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/wwt_api_client/constellations/handles.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3580 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/wwt_api_client/constellations/images.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4199 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/wwt_api_client/constellations/scenes.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2171 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/wwt_api_client/enums.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-21 22:08:14.049127 wwt_api_client-0.4.0/wwt_api_client/tests/
+-rw-r--r--   0 vsts      (1001) docker     (123)      178 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/wwt_api_client/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9654 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/wwt_api_client/tests/test_communities.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1388 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/wwt_api_client/tests/test_constellations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10749 2023-07-21 22:07:36.000000 wwt_api_client-0.4.0/wwt_api_client/tests/test_core.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-21 22:08:14.045127 wwt_api_client-0.4.0/wwt_api_client.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1334 2023-07-21 22:08:14.000000 wwt_api_client-0.4.0/wwt_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     5924 2023-07-21 22:08:14.000000 wwt_api_client-0.4.0/wwt_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-21 22:08:14.000000 wwt_api_client-0.4.0/wwt_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      236 2023-07-21 22:08:14.000000 wwt_api_client-0.4.0/wwt_api_client.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       15 2023-07-21 22:08:14.000000 wwt_api_client-0.4.0/wwt_api_client.egg-info/top_level.txt
```

### Comparing `wwt_api_client-0.3.0/LICENSE` & `wwt_api_client-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/PKG-INFO` & `wwt_api_client-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwt_api_client
-Version: 0.3.0
+Version: 0.4.0
 Summary: An API client for the AAS WorldWide Telescope web services
 Home-page: https://github.com/WorldWideTelescope/wwt_api_client
 Author: AAS WorldWide Telescope Team
 Author-email: wwt@aas.org
 License: MIT
 Keywords: Science
 Platform: Linux
```

### Comparing `wwt_api_client-0.3.0/README.md` & `wwt_api_client-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/Makefile` & `wwt_api_client-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/api/wwt_api_client.LoginRequest.rst` & `wwt_api_client-0.4.0/docs/api/wwt_api_client.LoginRequest.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/api/wwt_api_client.ShowImageRequest.rst` & `wwt_api_client-0.4.0/docs/api/wwt_api_client.ShowImageRequest.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/api/wwt_api_client.TileImageRequest.rst` & `wwt_api_client-0.4.0/docs/api/wwt_api_client.TileImageRequest.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/api/wwt_api_client.communities.CommunitiesClient.rst` & `wwt_api_client-0.4.0/docs/api/wwt_api_client.communities.CommunitiesClient.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/api/wwt_api_client.communities.CreateCommunityRequest.rst` & `wwt_api_client-0.4.0/docs/api/wwt_api_client.communities.CreateCommunityRequest.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/api/wwt_api_client.communities.DeleteCommunityRequest.rst` & `wwt_api_client-0.4.0/docs/api/wwt_api_client.communities.DeleteCommunityRequest.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/api/wwt_api_client.communities.GetCommunityInfoRequest.rst` & `wwt_api_client-0.4.0/docs/api/wwt_api_client.communities.GetCommunityInfoRequest.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/api/wwt_api_client.communities.GetProfileEntitiesRequest.rst` & `wwt_api_client-0.4.0/docs/api/wwt_api_client.communities.GetProfileEntitiesRequest.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.data.ImageDisplayInfo.rst` & `wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.ImageDisplayInfo.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.data.SceneContentHydrated.rst` & `wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.SceneContentHydrated.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.data.SceneImageLayer.rst` & `wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.SceneImageLayer.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.data.SceneImageLayerHydrated.rst` & `wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.SceneImageLayerHydrated.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.handles.AddImageRequest.rst` & `wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.handles.AddImageRequest.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.handles.AddSceneRequest.rst` & `wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.handles.AddSceneRequest.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/api/wwt_api_client.constellations.scenes.GetSceneResponse.rst` & `wwt_api_client-0.4.0/docs/api/wwt_api_client.constellations.data.ScenePreviews.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-GetSceneResponse
-================
+ScenePreviews
+=============
 
-.. currentmodule:: wwt_api_client.constellations.scenes
+.. currentmodule:: wwt_api_client.constellations.data
 
-.. autoclass:: GetSceneResponse
+.. autoclass:: ScenePreviews
    :show-inheritance:
 
    .. rubric:: Methods Summary
 
    .. autosummary::
 
-      ~GetSceneResponse.from_dict
-      ~GetSceneResponse.from_json
-      ~GetSceneResponse.schema
-      ~GetSceneResponse.to_dict
-      ~GetSceneResponse.to_json
+      ~ScenePreviews.from_dict
+      ~ScenePreviews.from_json
+      ~ScenePreviews.schema
+      ~ScenePreviews.to_dict
+      ~ScenePreviews.to_json
 
    .. rubric:: Methods Documentation
 
    .. automethod:: from_dict
    .. automethod:: from_json
    .. automethod:: schema
    .. automethod:: to_dict
```

### Comparing `wwt_api_client-0.3.0/docs/api/wwt_api_client.enums.CategoryType.rst` & `wwt_api_client-0.4.0/docs/api/wwt_api_client.enums.CategoryType.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/api/wwt_api_client.enums.ContentType.rst` & `wwt_api_client-0.4.0/docs/api/wwt_api_client.enums.ContentType.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/api/wwt_api_client.enums.HighlightType.rst` & `wwt_api_client-0.4.0/docs/api/wwt_api_client.enums.HighlightType.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/api/wwt_api_client.enums.UserRole.rst` & `wwt_api_client-0.4.0/docs/api/wwt_api_client.enums.UserRole.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/conf.py` & `wwt_api_client-0.4.0/docs/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 project = "wwt_api_client"
 author = "WorldWide Telescope project"
 copyright = "2019-2023 " + author
 
-release = "0.3.0"  # cranko project-version
+release = "0.4.0"  # cranko project-version
 version = ".".join(release.split(".")[:2])
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.doctest",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
```

### Comparing `wwt_api_client-0.3.0/docs/endpoints/constellations/get-handle-_handle.rst` & `wwt_api_client-0.4.0/docs/endpoints/constellations/get-handle-_handle.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/endpoints/constellations/get-image-_id-img_wtml.rst` & `wwt_api_client-0.4.0/docs/endpoints/constellations/get-image-_id-img_wtml.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/endpoints/constellations/get-scene-_id-place_wtml.rst` & `wwt_api_client-0.4.0/docs/endpoints/constellations/get-scene-_id-place_wtml.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/endpoints/constellations/get-scene-_id.rst` & `wwt_api_client-0.4.0/docs/endpoints/constellations/post-handle-_handle-image.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,77 +1,93 @@
-.. _endpoint-GET-scene-_id:
+.. _endpoint-POST-handle-_handle-image:
 
-==============
-GET /scene/:id
-==============
+==========================
+POST /handle/:handle/image
+==========================
 
-This API gets basic information about a specific WWT scene.
+This API creates a new Constellations image owned by the specified handle.
+
+
+Authorization
+=============
+
+The request must be made by an account that has permissions to add new images
+to the associated handle.
 
 
 Request Structure
 =================
 
-The request takes no content. The ``:id`` URL parameter gives the ID of the
-scene to query.
+The URL parameter ``:handle`` is the handle that will own the image.
+
+The structure of the request is:
+
+.. code-block:: javascript
+
+  {
+    "wwt": {
+      // See the `wwt_data_formats` documentation for definitions of these fields
+      "base_degrees_per_tile": $number,
+      "bottoms_up": $boolean,
+      "center_x": $number,
+      "center_y": $number,
+      "file_type": $string,
+      "offset_x": $number,
+      "offset_y": $number,
+      "projection": $string,
+      "quad_tree_map": $string,
+      "rotation": $number,
+      "thumbnail_url": $string,
+      "tile_levels": $number(int),
+      "width_factor": $number(int),
+    },
+    "permissions": {
+      // Free plain text giving the copyright statement for this image. Preferred form is
+      // along the lines of "Copyright 2020 Henrietta Swan Leavitt" or "Public
+      // domain". *Please* provide support in higher-level applications to allow
+      // users to input valid information here — the correct information for this
+      // field cannot be determined algorithmically. Note that under the world's
+      // current regime of intellectual property law, virtually every single image
+      // in WWT can be presumed to be copyrighted, with the major exception of
+      // images produced by employees of the US Federal government in the course of
+      // their duties.
+      "copyright": $string,
+
+      // HTML content giving credits to be shown when displaying this image. This is
+      // different information than the copyright statement, which specifies who
+      // "owns" the image. The credits have no legal significance, except that
+      // some images are licensed in a way that requires that specific credit texts
+      // are shown alongside them.
+      //
+      // Only a subset of HTML is allowed here. Allowed tags are `<a>`, `<b>`, `<br>`,
+      // `<em>`, `<i>`, and `<strong>`.
+      "credits": $string?,
+
+      // The SPDX License Identifier (https://spdx.org/licenses/) of the license
+      // under which this image is made available through WWT. Use `CC-PDDC` for
+      // images in the public domain. For images with known licenses that are not
+      // in the SPDX list, use `LicenseRef-$TEXT` for some value of `$TEXT`; see
+      // the "Other licensing information detected" section of the SPDX
+      // specification
+      // (https://spdx.github.io/spdx-spec/v2-draft/other-licensing-information-detected/).
+      "license": $string,
+    },
+    "storage": {
+      // For now, this is the only valid storage type:
+      "legacy_url_template": $string // This image's legacy URL
+    },
+    "note": $string, // Freeform text describing the image; not generally exposed
+  }
 
 
 Response Structure
 ==================
 
 The structure of the response is:
 
 .. code-block:: javascript
 
   {
     "error": $bool // Whether an error occurred
-    "id": $string(objectID), // the ID of this scene
-    "handle_id": $string(objectID), // the ID of this scenes's owner
-    "handle": { // Information about the owning handle
-      "handle": $string, // the unique handle name
-      "display_name": $string, // the handle's display name
-    },
-    "creation_date": $string(iso8601), // the date this scene was created
-    "likes": $number, // the number of likes this scene has received
-    "place": { // WWT camera information associated with this scene
-      // See "POST /handle/:handle/scene" docs for descriptions:
-      "ra_rad": $number,
-      "dec_rad": $number,
-      "zoom_deg": $number,
-      "roll_rad": $number,
-    },
-    "content": { // The contents of this scene
-      // Eventually, multiple content forms will likely be supported.
-      // For now, the only one is:
-      "image_layers": [
-        // List of "hydrated" image layer records:
-        {
-          "image": {
-            "wwt": {
-              // Astrometric/data fields used by WWT, as in `POST /handle/:handle/image`;
-              // see the `wwt_data_formats` documentation for definitions of these fields
-              "base_degrees_per_tile": $number,
-              "bottoms_up": $boolean,
-              "center_x": $number,
-              "center_y": $number,
-              "file_type": $string,
-              "offset_x": $number,
-              "offset_y": $number,
-              "projection": $string,
-              "quad_tree_map": $string,
-              "rotation": $number,
-              "thumbnail_url": $string,
-              "tile_levels": $number(int),
-              "width_factor": $number(int),
-            }
-            "storage": {
-              // Data storage information as in `POST /handle/:handle/image`
-              // For now, this is the only valid storage type:
-              "legacy_url_template": $string // This image's legacy URL
-            }
-          },
-          "opacity": $number, // between 0 and 1
-        }
-      ],
-    },
-    "text": $string, // The text associated with this scene
-    "outgoing_url": $string(URL)?, // optional outgoing URL associated with this scene
+    "id": $string(objectID), // the ID of the newly-created image
+    "rel_url": $string, // the API-relative URL used to access this image; `/image/:id`
   }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wwt_api_client-0.3.0/docs/endpoints/constellations/post-handle-_handle-image.rst` & `wwt_api_client-0.4.0/docs/endpoints/constellations/get-image-_id.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,65 @@
-.. _endpoint-POST-handle-_handle-image:
+.. _endpoint-GET-image-_id:
 
-==========================
-POST /handle/:handle/image
-==========================
+==============
+GET /image/:id
+==============
 
-This API creates a new Constellations image owned by the specified handle.
-
-
-Authorization
-=============
-
-The request must be made by an account that has permissions to add new images
-to the associated handle.
+This API gets basic information about a specific WWT image.
 
 
 Request Structure
 =================
 
-The URL parameter ``:handle`` is the handle that will own the image.
+The request takes no content. The ``:id`` URL parameter gives the ID of the
+image to query.
+
+
+Response Structure
+==================
 
-The structure of the request is:
+The structure of the response is:
 
 .. code-block:: javascript
 
   {
+    "error": $bool // Whether an error occurred
+    "id": $string(objectID), // the ID of this image
+    "handle_id": $string(objectID), // the ID of this images's owner
+    "handle": { // Information about the owning handle
+      "handle": $string, // the unique handle name
+      "display_name": $string, // the handle's display name
+    },
+    "creation_date": $string(iso8601), // the date this image was created
     "wwt": {
-      // See the `wwt_data_formats` documentation for definitions of these fields
+      // Astrometric/data fields used by WWT, as in `POST /handle/:handle/image`;
+      // see the `wwt_data_formats` documentation for definitions of these fields
       "base_degrees_per_tile": $number,
       "bottoms_up": $boolean,
       "center_x": $number,
       "center_y": $number,
       "file_type": $string,
       "offset_x": $number,
       "offset_y": $number,
       "projection": $string,
       "quad_tree_map": $string,
       "rotation": $number,
       "thumbnail_url": $string,
       "tile_levels": $number(int),
       "width_factor": $number(int),
     },
+    "permissions": {
+      // Permissions information; see `POST /handle/:handle/image` for specification.
+      "copyright": $string,
+      "credits": $string?,
+      "license": $string,
+    },
     "storage": {
+      // Data storage information as in `POST /handle/:handle/image`
       // For now, this is the only valid storage type:
       "legacy_url_template": $string // This image's legacy URL
-    }
-    "note": $string, // Freeform text describing the image; not generally exposed
+    },
+    "note": $string, // A textual note associated with this image
   }
 
-
-Response Structure
-==================
-
-The structure of the response is:
-
-.. code-block:: javascript
-
-  {
-    "error": $bool // Whether an error occurred
-    "id": $string(objectID), // the ID of the newly-created image
-    "rel_url": $string, // the API-relative URL used to access this image; `/image/:id`
-  }
+See :ref:`endpoint-post-handle-_handle-image` for definitions of the contents of the inner
+image fields.
```

### Comparing `wwt_api_client-0.3.0/docs/endpoints/constellations/post-handle-_handle-scene.rst` & `wwt_api_client-0.4.0/docs/endpoints/constellations/post-handle-_handle-scene.rst`

 * *Files 16% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 
 .. code-block:: javascript
 
   {
     "place": {
       "ra_rad": $number, // The RA of the final camera position for this scene, in radians
       "dec_rad": $number, // The dec. of the final camera position for this scene, in radians
-      "zoom_deg": $number, // The WWT zoom level of the final camera position, in degrees
       "roll_rad": $number, // The roll of the final camera position, in radians
+      "roi_height_deg": $number, // The height of the region of interest, in degrees
+      "roi_aspect_ratio": $number, // The aspect ratio (width / height) of the region of interest
     },
     "content": {
       "image_layers": [
         // An optional list of image layers that comprise this scene.
         // Right now this field is not optional because it is the only supported scene
         // type, but that might change.
         {
```

### Comparing `wwt_api_client-0.3.0/docs/endpoints/constellations/post-images-find-by-legacy-url.rst` & `wwt_api_client-0.4.0/docs/endpoints/constellations/post-images-find-by-legacy-url.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/endpoints/legacy/login.rst` & `wwt_api_client-0.4.0/docs/endpoints/legacy/login.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/endpoints/legacy/show-image.rst` & `wwt_api_client-0.4.0/docs/endpoints/legacy/show-image.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/endpoints/legacy/tile-image.rst` & `wwt_api_client-0.4.0/docs/endpoints/legacy/tile-image.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/images/logo.png` & `wwt_api_client-0.4.0/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/installation.rst` & `wwt_api_client-0.4.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/docs/make.bat` & `wwt_api_client-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/setup.py` & `wwt_api_client-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 """
     )
     return "".join(lines)
 
 
 setup_args = dict(
     name="wwt_api_client",  # cranko project-name
-    version="0.3.0",  # cranko project-version
+    version="0.4.0",  # cranko project-version
     description="An API client for the AAS WorldWide Telescope web services",
     long_description=get_long_desc(),
     long_description_content_type="text/markdown",
     author="AAS WorldWide Telescope Team",
     author_email="wwt@aas.org",
     url="https://github.com/WorldWideTelescope/wwt_api_client",
     packages=[
@@ -60,14 +60,16 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     include_package_data=True,
     install_requires=[
         "dataclasses-json >=0.5",
+        "html-sanitizer",
+        "license-expression >=21.6",
         "openidc_client >=0.6",
         "requests >=2.10",
         "wwt_data_formats >=0.16",
     ],
     extras_require={
         "test": [
             "httpretty",
```

### Comparing `wwt_api_client-0.3.0/wwt_api_client/__init__.py` & `wwt_api_client-0.4.0/wwt_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/wwt_api_client/communities.py` & `wwt_api_client-0.4.0/wwt_api_client/communities.py`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/wwt_api_client/constellations/__init__.py` & `wwt_api_client-0.4.0/wwt_api_client/constellations/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from dataclasses_json import dataclass_json
 import os
 from requests import RequestException, Response
 from typing import List, Optional
 
 from openidc_client import OpenIDCClient
 
-from .data import ImageSummary, _strip_nulls_in_place
+from .data import ImageSummary, SceneHydrated, _strip_nulls_in_place
 
 __all__ = """
 ClientConfig
 CxClient
 """.split()
 
 
@@ -140,27 +140,35 @@
         return cls(
             id_provider_url="https://wwtelescope.dev/auth/realms/constellations",
             client_id="cli-tool",
             api_url="https://api.wwtelescope.dev/",
         )
 
 
-@dataclass_json
+@dataclass_json(undefined="EXCLUDE")
 @dataclass
 class FindImagesByLegacyRequest:
     wwt_legacy_url: str
 
 
-@dataclass_json
+@dataclass_json(undefined="EXCLUDE")
 @dataclass
 class FindImagesByLegacyResponse:
-    error: bool
     results: List[ImageSummary]
 
 
+@dataclass_json(undefined="EXCLUDE")
+@dataclass
+class TimelineResponse:
+    results: List[SceneHydrated]
+
+
+BuiltinBackgroundsResponse = FindImagesByLegacyResponse
+
+
 # I think this is unlikely to ever need to be configurable?
 _ID_PROVIDER_MAPPING = {
     "Authorization": "/protocol/openid-connect/auth",
     "Token": "/protocol/openid-connect/token",
 }
 
 
@@ -262,15 +270,15 @@
         Parameters
         ----------
         id : :class:`str`
             The ID of the scene of interest.
 
         Returns
         -------
-        :class:`handles.SceneClient`
+        :class:`scenes.SceneClient`
         """
         from .scenes import SceneClient
 
         return SceneClient(self, id)
 
     def find_images_by_wwt_url(self, wwt_url: str) -> List[ImageSummary]:
         """
@@ -281,9 +289,61 @@
         :ref:`endpoint-POST-images-find-by-legacy-url` API endpoint.
         """
         req = FindImagesByLegacyRequest(wwt_legacy_url=wwt_url)
         resp = self._send_and_check(
             "/images/find-by-legacy-url",
             json=_strip_nulls_in_place(req.to_dict()),
         )
-        resp = FindImagesByLegacyResponse.schema().load(resp.json())
+        resp = resp.json()
+        resp.pop("error")
+        resp = FindImagesByLegacyResponse.schema().load(resp)
+        return resp.results
+
+    def get_home_timeline(self, page_num: int) -> List[SceneHydrated]:
+        """
+        Get information about a group of scenes on the home timeline.
+
+        Parameters
+        ----------
+        page_num : int
+            Which page to retrieve. Page zero gives the top items on the
+            timeline, page one gives the next set, etc.
+
+        Returns
+        -------
+        A list of :class:`~wwt_api_client.constellations.data.SceneHydrated`
+        items.
+
+        Notes
+        -----
+        The page size is not specified externally, nor is it guaranteed to be
+        stable from one page to the next. If you care, look at the length of the
+        list that you get back from an API.
+        """
+        try:
+            use_page_num = int(page_num)
+            assert use_page_num >= 0
+        except Exception:
+            raise ValueError(f"invalid page_num argument {page_num!r}")
+
+        resp = self._send_and_check(
+            "/scenes/home-timeline",
+            http_method="GET",
+            params={"page": use_page_num},
+        )
+        resp = resp.json()
+        resp.pop("error")
+        resp = TimelineResponse.schema().load(resp)
+        return resp.results
+
+    def get_builtin_backgrounds(self) -> List[ImageSummary]:
+        """
+        Get the list of builtin background imagery options.
+
+        This method corresponds to the
+        :ref:`endpoint-GET-images-builtin-backgrounds` API endpoint.
+        """
+        resp = self._send_and_check("/images/builtin-backgrounds", http_method="GET")
+        resp = resp.json()
+        resp.pop("error")
+        resp = BuiltinBackgroundsResponse.schema().load(resp)
         return resp.results
```

### Comparing `wwt_api_client-0.3.0/wwt_api_client/enums.py` & `wwt_api_client-0.4.0/wwt_api_client/enums.py`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/wwt_api_client/tests/test_communities.py` & `wwt_api_client-0.4.0/wwt_api_client/tests/test_communities.py`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/wwt_api_client/tests/test_core.py` & `wwt_api_client-0.4.0/wwt_api_client/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `wwt_api_client-0.3.0/wwt_api_client.egg-info/PKG-INFO` & `wwt_api_client-0.4.0/wwt_api_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwt-api-client
-Version: 0.3.0
+Version: 0.4.0
 Summary: An API client for the AAS WorldWide Telescope web services
 Home-page: https://github.com/WorldWideTelescope/wwt_api_client
 Author: AAS WorldWide Telescope Team
 Author-email: wwt@aas.org
 License: MIT
 Keywords: Science
 Platform: Linux
```

