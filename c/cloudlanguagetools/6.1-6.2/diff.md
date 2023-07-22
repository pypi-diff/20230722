# Comparing `tmp/cloudlanguagetools-6.1.tar.gz` & `tmp/cloudlanguagetools-6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudlanguagetools-6.1.tar", last modified: Mon Jul 17 06:18:13 2023, max compression
+gzip compressed data, was "cloudlanguagetools-6.2.tar", last modified: Sat Jul 22 00:24:48 2023, max compression
```

## Comparing `cloudlanguagetools-6.1.tar` & `cloudlanguagetools-6.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-17 06:18:13.669045 cloudlanguagetools-6.1/
--rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/LICENSE
--rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-07-17 06:18:13.669045 cloudlanguagetools-6.1/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)      169 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/README.rst
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-17 06:18:13.669045 cloudlanguagetools-6.1/cloudlanguagetools/
--rw-r--r--   0 luc       (1000) luc       (1000)        0 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/__init__.py
--rw-r--r--   0 luc       (1000) luc       (1000)    13412 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/amazon.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2667 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/argostranslate.py
--rw-r--r--   0 luc       (1000) luc       (1000)    23928 2023-07-14 14:25:16.000000 cloudlanguagetools-6.1/cloudlanguagetools/azure.py
--rw-r--r--   0 luc       (1000) luc       (1000)     4388 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/cereproc.py
--rw-r--r--   0 luc       (1000) luc       (1000)    17939 2023-07-16 13:29:35.000000 cloudlanguagetools-6.1/cloudlanguagetools/chatapi.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2165 2023-07-14 14:25:16.000000 cloudlanguagetools-6.1/cloudlanguagetools/constants.py
--rw-r--r--   0 luc       (1000) luc       (1000)     4023 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/deepl.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1232 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/dictionarylookup.py
--rw-r--r--   0 luc       (1000) luc       (1000)     9171 2023-07-05 00:37:32.000000 cloudlanguagetools-6.1/cloudlanguagetools/easypronunciation.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6883 2023-07-14 14:25:16.000000 cloudlanguagetools-6.1/cloudlanguagetools/elevenlabs.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1052 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/encryption.py
--rw-r--r--   0 luc       (1000) luc       (1000)     7015 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/epitran.py
--rw-r--r--   0 luc       (1000) luc       (1000)      218 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/errors.py
--rw-r--r--   0 luc       (1000) luc       (1000)    13308 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/forvo.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6310 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/fptai.py
--rw-r--r--   0 luc       (1000) luc       (1000)     8801 2023-07-14 14:25:16.000000 cloudlanguagetools-6.1/cloudlanguagetools/google.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6355 2023-07-14 14:25:16.000000 cloudlanguagetools-6.1/cloudlanguagetools/keys.py
--rw-r--r--   0 luc       (1000) luc       (1000)    14056 2023-07-14 14:25:16.000000 cloudlanguagetools-6.1/cloudlanguagetools/languages.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2806 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/libretranslate.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3980 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/mandarincantonese.py
--rw-r--r--   0 luc       (1000) luc       (1000)    18680 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/naver.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2511 2023-07-14 14:25:16.000000 cloudlanguagetools-6.1/cloudlanguagetools/openai.py
--rw-r--r--   0 luc       (1000) luc       (1000)      339 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/options.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3310 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/pythainlp.py
--rw-r--r--   0 luc       (1000) luc       (1000)      432 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/service.py
--rw-r--r--   0 luc       (1000) luc       (1000)    18797 2023-07-14 14:25:16.000000 cloudlanguagetools-6.1/cloudlanguagetools/servicemanager.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3006 2023-07-14 14:25:16.000000 cloudlanguagetools-6.1/cloudlanguagetools/spacy.py
--rw-r--r--   0 luc       (1000) luc       (1000)     5539 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/test_services.py
--rw-r--r--   0 luc       (1000) luc       (1000)      528 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/tokenization.py
--rw-r--r--   0 luc       (1000) luc       (1000)      515 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/translationlanguage.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1187 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/transliterationlanguage.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1239 2023-07-14 14:25:16.000000 cloudlanguagetools-6.1/cloudlanguagetools/ttsvoice.py
--rw-r--r--   0 luc       (1000) luc       (1000)    30649 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/vocalware.py
--rw-r--r--   0 luc       (1000) luc       (1000)     5479 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/voicen.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6491 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/watson.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6384 2023-05-24 03:51:37.000000 cloudlanguagetools-6.1/cloudlanguagetools/wenlin.py
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-17 06:18:13.669045 cloudlanguagetools-6.1/cloudlanguagetools.egg-info/
--rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-07-17 06:18:13.000000 cloudlanguagetools-6.1/cloudlanguagetools.egg-info/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)     1430 2023-07-17 06:18:13.000000 cloudlanguagetools-6.1/cloudlanguagetools.egg-info/SOURCES.txt
--rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-07-17 06:18:13.000000 cloudlanguagetools-6.1/cloudlanguagetools.egg-info/dependency_links.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       59 2023-07-17 06:18:13.000000 cloudlanguagetools-6.1/cloudlanguagetools.egg-info/requires.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       19 2023-07-17 06:18:13.000000 cloudlanguagetools-6.1/cloudlanguagetools.egg-info/top_level.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-07-17 06:18:13.669045 cloudlanguagetools-6.1/setup.cfg
--rwxr-xr-x   0 luc       (1000) luc       (1000)      931 2023-07-17 06:18:10.000000 cloudlanguagetools-6.1/setup.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-22 00:24:48.979308 cloudlanguagetools-6.2/
+-rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/LICENSE
+-rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-07-22 00:24:48.979308 cloudlanguagetools-6.2/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)      169 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/README.rst
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-22 00:24:48.979308 cloudlanguagetools-6.2/cloudlanguagetools/
+-rw-r--r--   0 luc       (1000) luc       (1000)        0 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/__init__.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    13412 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/amazon.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2667 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/argostranslate.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    23928 2023-07-14 14:25:16.000000 cloudlanguagetools-6.2/cloudlanguagetools/azure.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     4388 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/cereproc.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    17838 2023-07-22 00:24:24.000000 cloudlanguagetools-6.2/cloudlanguagetools/chatapi.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2165 2023-07-14 14:25:16.000000 cloudlanguagetools-6.2/cloudlanguagetools/constants.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     4023 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/deepl.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1232 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/dictionarylookup.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     9171 2023-07-05 00:37:32.000000 cloudlanguagetools-6.2/cloudlanguagetools/easypronunciation.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6883 2023-07-14 14:25:16.000000 cloudlanguagetools-6.2/cloudlanguagetools/elevenlabs.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1052 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/encryption.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     7015 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/epitran.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      218 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/errors.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    13308 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/forvo.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6310 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/fptai.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     8801 2023-07-14 14:25:16.000000 cloudlanguagetools-6.2/cloudlanguagetools/google.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6355 2023-07-14 14:25:16.000000 cloudlanguagetools-6.2/cloudlanguagetools/keys.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    14056 2023-07-14 14:25:16.000000 cloudlanguagetools-6.2/cloudlanguagetools/languages.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2806 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/libretranslate.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3980 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/mandarincantonese.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    18680 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/naver.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2511 2023-07-14 14:25:16.000000 cloudlanguagetools-6.2/cloudlanguagetools/openai.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      339 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/options.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3310 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/pythainlp.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      432 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/service.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    18797 2023-07-14 14:25:16.000000 cloudlanguagetools-6.2/cloudlanguagetools/servicemanager.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3006 2023-07-14 14:25:16.000000 cloudlanguagetools-6.2/cloudlanguagetools/spacy.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     5539 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/test_services.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      528 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/tokenization.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      515 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/translationlanguage.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1187 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/transliterationlanguage.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1239 2023-07-14 14:25:16.000000 cloudlanguagetools-6.2/cloudlanguagetools/ttsvoice.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    30649 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/vocalware.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     5479 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/voicen.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6491 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/watson.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6384 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/wenlin.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-22 00:24:48.979308 cloudlanguagetools-6.2/cloudlanguagetools.egg-info/
+-rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-07-22 00:24:48.000000 cloudlanguagetools-6.2/cloudlanguagetools.egg-info/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)     1430 2023-07-22 00:24:48.000000 cloudlanguagetools-6.2/cloudlanguagetools.egg-info/SOURCES.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-07-22 00:24:48.000000 cloudlanguagetools-6.2/cloudlanguagetools.egg-info/dependency_links.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       59 2023-07-22 00:24:48.000000 cloudlanguagetools-6.2/cloudlanguagetools.egg-info/requires.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       19 2023-07-22 00:24:48.000000 cloudlanguagetools-6.2/cloudlanguagetools.egg-info/top_level.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-07-22 00:24:48.979308 cloudlanguagetools-6.2/setup.cfg
+-rwxr-xr-x   0 luc       (1000) luc       (1000)      931 2023-07-22 00:24:45.000000 cloudlanguagetools-6.2/setup.py
```

### Comparing `cloudlanguagetools-6.1/LICENSE` & `cloudlanguagetools-6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/PKG-INFO` & `cloudlanguagetools-6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudlanguagetools
-Version: 6.1
+Version: 6.2
 Summary: Interface with various cloud APIs for language processing such as translation, text to speech
 Home-page: https://github.com/Language-Tools/cloud-language-tools-core
 Author: Luc
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/amazon.py` & `cloudlanguagetools-6.2/cloudlanguagetools/amazon.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/argostranslate.py` & `cloudlanguagetools-6.2/cloudlanguagetools/argostranslate.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/azure.py` & `cloudlanguagetools-6.2/cloudlanguagetools/azure.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/cereproc.py` & `cloudlanguagetools-6.2/cloudlanguagetools/cereproc.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/chatapi.py` & `cloudlanguagetools-6.2/cloudlanguagetools/chatapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,32 +18,25 @@
 it will try to find the ideal service and parameters for the given request, 
 but sometimes parameters will be overriden to ensure an output is produced.
 """
 
 class NoDataFoundException(Exception):
     pass
 
-
-class TranslateQuery(pydantic.BaseModel):
-    input_text: str = Field(description="text to translate")
-    source_language: cloudlanguagetools.languages.CommonLanguage = Field(description="language to translate from")
-    target_language: cloudlanguagetools.languages.CommonLanguage = Field(description="language to translate to")
+class TranslateLookupQuery(pydantic.BaseModel):
+    input_text: str = Field(description="text to translate or lookup in the dictionary")
+    source_language: cloudlanguagetools.languages.CommonLanguage = Field(description="language of the text to translate or lookup in dictionary")
+    target_language: cloudlanguagetools.languages.CommonLanguage = Field(description="language to translate to, or language of dictionary definition")
     service: Optional[cloudlanguagetools.constants.Service] = Field(default=None, description='service to use for translation')
 
 class TransliterateQuery(pydantic.BaseModel):
     input_text: str = Field(description="text to transliterate")
     language: cloudlanguagetools.languages.CommonLanguage = Field(description="language the text is in")
     service: Optional[cloudlanguagetools.constants.Service] = Field(default=None, description='service to use for transliteration')
 
-class DictionaryLookup(pydantic.BaseModel):
-    input_text: str = Field(description="text to lookup in the dictionary")
-    source_language: cloudlanguagetools.languages.CommonLanguage = Field(description="language of the text to look up")
-    target_language: cloudlanguagetools.languages.CommonLanguage = Field(description="language for the dictionary definition")
-    service: Optional[cloudlanguagetools.constants.Service] = Field(default=None, description='service to use for dictionary lookup')
-
 class AudioQuery(pydantic.BaseModel):
     input_text: str = Field(description="text to pronounce / generate audio")
     language: cloudlanguagetools.languages.CommonLanguage = Field(description="language the text is in")
     service: Optional[cloudlanguagetools.constants.Service] = Field(default=None, description='service to use audio pronunciation')
     gender: Optional[cloudlanguagetools.constants.Gender] = Field(default=None, description='gender of the voice to pronounce the text in')
 
 class BreakdownQuery(pydantic.BaseModel):
@@ -130,15 +123,15 @@
             final_candidates = [x for x in candidates if 
                                 x.service == service and x.get_transliteration_key()['tone_numbers'] == False and
                                 x.service == service and x.get_transliteration_key()['spaces'] == False]
         transliteration_option = final_candidates[0]
 
         return transliteration_option
 
-    def translate(self, query: TranslateQuery):
+    def translate(self, query: TranslateLookupQuery):
         logger.info(f'translating {query.input_text} from {query.source_language} to {query.target_language}')
 
         source_language = cloudlanguagetools.languages.Language[query.source_language.name]
         target_language = cloudlanguagetools.languages.Language[query.target_language.name]
         translation_option = self.select_translation_option(query.service, source_language, target_language)
 
         # get the translation
@@ -147,25 +140,37 @@
             translation_option['service'],
             translation_option['source_language_id'],
             translation_option['target_language_id'],
         )
         return translated_text
 
 
-    def transliterate(self, query: TranslateQuery):
+    def transliterate(self, query: TransliterateQuery):
         language = cloudlanguagetools.languages.Language[query.language.name]
         transliteration_option = self.select_transliteration_option(query.service, language)
         transliterated_text = self.manager.get_transliteration(
             query.input_text,
             transliteration_option.service,
             transliteration_option.get_transliteration_key()
         )
         return transliterated_text
 
-    def dictionary_lookup(self, query: DictionaryLookup):
+    def translate_or_lookup(self, query: TranslateLookupQuery):
+        logger.info(f'translation or dictionary lookup: {query}')
+
+        try:
+            # try dictionary lookup as a first attempt
+            result = self.dictionary_lookup(query)
+            return result
+        except cloudlanguagetools.errors.NotFoundError as e:
+            # if dictionary lookup fails, try translation
+            result = self.translate(query)
+            return result
+
+    def dictionary_lookup(self, query: TranslateLookupQuery):
         logger.info(f'dictionary lookup {query}')
         source_language = cloudlanguagetools.languages.Language[query.source_language.name]
         target_language = cloudlanguagetools.languages.Language[query.target_language.name]
         dictionary_option_list = self.manager.get_dictionary_lookup_options()
         candidates = [x for x in dictionary_option_list if x.language == source_language and x.target_language == target_language]
         if len(candidates) == 0:
             raise NoDataFoundException(f'No dictionary service found for source language {query.source_language.lang_name} / target language: {query.target_language.lang_name}')
@@ -194,23 +199,20 @@
             
         service = service_preference[0]
         final_candidates = [x for x in candidates if x.service == service]
 
         dictionary_option = final_candidates[0]
         logger.debug(f'Using dictionary option {pprint.pformat(dictionary_option.json_obj())}')
 
-        try:
-            dictionary_result = self.manager.get_dictionary_lookup(
-                query.input_text,
-                service,
-                dictionary_option.get_lookup_key()
-            )
-            result = ' / '.join(dictionary_result)
-        except cloudlanguagetools.errors.NotFoundError as e:
-            result = f'No dictionary lookup results found for {query.input_text}'
+        dictionary_result = self.manager.get_dictionary_lookup(
+            query.input_text,
+            service,
+            dictionary_option.get_lookup_key()
+        )
+        result = ' / '.join(dictionary_result)
         return result
         
 
     def audio(self, query: AudioQuery, format: cloudlanguagetools.options.AudioFormat) -> tempfile.NamedTemporaryFile:
         logger.info(f'processing audio query: {query}')
         language = cloudlanguagetools.languages.Language[query.language.name]
         # get full voice list, filter down to correct language
```

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/constants.py` & `cloudlanguagetools-6.2/cloudlanguagetools/constants.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/deepl.py` & `cloudlanguagetools-6.2/cloudlanguagetools/deepl.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/dictionarylookup.py` & `cloudlanguagetools-6.2/cloudlanguagetools/dictionarylookup.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/easypronunciation.py` & `cloudlanguagetools-6.2/cloudlanguagetools/easypronunciation.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/elevenlabs.py` & `cloudlanguagetools-6.2/cloudlanguagetools/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/encryption.py` & `cloudlanguagetools-6.2/cloudlanguagetools/encryption.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/epitran.py` & `cloudlanguagetools-6.2/cloudlanguagetools/epitran.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/forvo.py` & `cloudlanguagetools-6.2/cloudlanguagetools/forvo.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/fptai.py` & `cloudlanguagetools-6.2/cloudlanguagetools/fptai.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/google.py` & `cloudlanguagetools-6.2/cloudlanguagetools/google.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/keys.py` & `cloudlanguagetools-6.2/cloudlanguagetools/keys.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/languages.py` & `cloudlanguagetools-6.2/cloudlanguagetools/languages.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/libretranslate.py` & `cloudlanguagetools-6.2/cloudlanguagetools/libretranslate.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/mandarincantonese.py` & `cloudlanguagetools-6.2/cloudlanguagetools/mandarincantonese.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/naver.py` & `cloudlanguagetools-6.2/cloudlanguagetools/naver.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/openai.py` & `cloudlanguagetools-6.2/cloudlanguagetools/openai.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/pythainlp.py` & `cloudlanguagetools-6.2/cloudlanguagetools/pythainlp.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/servicemanager.py` & `cloudlanguagetools-6.2/cloudlanguagetools/servicemanager.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/spacy.py` & `cloudlanguagetools-6.2/cloudlanguagetools/spacy.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/test_services.py` & `cloudlanguagetools-6.2/cloudlanguagetools/test_services.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/tokenization.py` & `cloudlanguagetools-6.2/cloudlanguagetools/tokenization.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/translationlanguage.py` & `cloudlanguagetools-6.2/cloudlanguagetools/translationlanguage.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/transliterationlanguage.py` & `cloudlanguagetools-6.2/cloudlanguagetools/transliterationlanguage.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/ttsvoice.py` & `cloudlanguagetools-6.2/cloudlanguagetools/ttsvoice.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/vocalware.py` & `cloudlanguagetools-6.2/cloudlanguagetools/vocalware.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/voicen.py` & `cloudlanguagetools-6.2/cloudlanguagetools/voicen.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/watson.py` & `cloudlanguagetools-6.2/cloudlanguagetools/watson.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools/wenlin.py` & `cloudlanguagetools-6.2/cloudlanguagetools/wenlin.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools.egg-info/PKG-INFO` & `cloudlanguagetools-6.2/cloudlanguagetools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudlanguagetools
-Version: 6.1
+Version: 6.2
 Summary: Interface with various cloud APIs for language processing such as translation, text to speech
 Home-page: https://github.com/Language-Tools/cloud-language-tools-core
 Author: Luc
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudlanguagetools-6.1/cloudlanguagetools.egg-info/SOURCES.txt` & `cloudlanguagetools-6.2/cloudlanguagetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.1/setup.py` & `cloudlanguagetools-6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools.command.install import install
 
 # build instructions
 # python setup.py sdist
 # twine upload dist/*
 
 setup(name='cloudlanguagetools',
-      version='6.1',
+      version='6.2',
       description='Interface with various cloud APIs for language processing such as translation, text to speech',
       long_description=open('README.rst', encoding='utf-8').read(),
       url='https://github.com/Language-Tools/cloud-language-tools-core',
       author='Luc',
       author_email='languagetools@mailc.net',
       classifiers=[
         'Programming Language :: Python :: 3.7',
```

