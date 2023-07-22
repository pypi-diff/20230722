# Comparing `tmp/demogpt-1.1.1.6.tar.gz` & `tmp/demogpt-1.1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demogpt-1.1.1.6.tar", last modified: Sat Jul 22 20:45:14 2023, max compression
+gzip compressed data, was "demogpt-1.1.1.7.tar", last modified: Sat Jul 22 20:49:08 2023, max compression
```

## Comparing `demogpt-1.1.1.6.tar` & `demogpt-1.1.1.7.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:45:14.016217 demogpt-1.1.1.6/
--rw-rw-r--   0 melih     (1000) melih     (1000)     1069 2023-06-07 10:58:37.000000 demogpt-1.1.1.6/LICENSE
--rw-rw-r--   0 melih     (1000) melih     (1000)      409 2023-07-22 20:45:14.016217 demogpt-1.1.1.6/PKG-INFO
--rw-rw-r--   0 melih     (1000) melih     (1000)     6530 2023-07-19 15:30:18.000000 demogpt-1.1.1.6/README.md
--rw-rw-r--   0 melih     (1000) melih     (1000)       38 2023-07-22 20:45:14.016217 demogpt-1.1.1.6/setup.cfg
--rw-rw-r--   0 melih     (1000) melih     (1000)      845 2023-07-22 20:45:00.000000 demogpt-1.1.1.6/setup.py
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:45:14.008216 demogpt-1.1.1.6/src/
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:45:14.012217 demogpt-1.1.1.6/src/alpha/
--rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-21 17:19:00.000000 demogpt-1.1.1.6/src/alpha/__init__.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     4995 2023-07-21 17:19:00.000000 demogpt-1.1.1.6/src/alpha/agent_prompts.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     3868 2023-07-21 17:19:00.000000 demogpt-1.1.1.6/src/alpha/app.py
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:45:14.012217 demogpt-1.1.1.6/src/alpha/chains/
--rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-21 17:19:00.000000 demogpt-1.1.1.6/src/alpha/chains/__init__.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     2444 2023-07-21 17:19:00.000000 demogpt-1.1.1.6/src/alpha/chains/chains.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     7505 2023-07-21 17:19:00.000000 demogpt-1.1.1.6/src/alpha/chains/prompts.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     4277 2023-07-22 17:12:22.000000 demogpt-1.1.1.6/src/alpha/code.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     1820 2023-07-21 17:19:00.000000 demogpt-1.1.1.6/src/alpha/example_generation.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     8510 2023-07-21 17:19:00.000000 demogpt-1.1.1.6/src/alpha/langchain_agent.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     8899 2023-07-21 17:19:00.000000 demogpt-1.1.1.6/src/alpha/langchain_coder.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     4368 2023-07-21 17:19:00.000000 demogpt-1.1.1.6/src/alpha/langchain_expert.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     5537 2023-07-21 17:19:00.000000 demogpt-1.1.1.6/src/alpha/model.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     1963 2023-07-21 17:19:00.000000 demogpt-1.1.1.6/src/alpha/utils.py
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:45:14.012217 demogpt-1.1.1.6/src/beta/
--rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-21 08:30:31.000000 demogpt-1.1.1.6/src/beta/__init__.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     4995 2023-07-21 17:19:00.000000 demogpt-1.1.1.6/src/beta/agent_prompts.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     3868 2023-07-21 17:19:00.000000 demogpt-1.1.1.6/src/beta/app.py
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:45:14.012217 demogpt-1.1.1.6/src/beta/chains/
--rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-21 08:30:31.000000 demogpt-1.1.1.6/src/beta/chains/__init__.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     2444 2023-07-21 17:19:00.000000 demogpt-1.1.1.6/src/beta/chains/chains.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     7505 2023-07-21 08:30:31.000000 demogpt-1.1.1.6/src/beta/chains/prompts.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     1820 2023-07-21 08:30:31.000000 demogpt-1.1.1.6/src/beta/example_generation.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     8510 2023-07-21 17:19:00.000000 demogpt-1.1.1.6/src/beta/langchain_agent.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     8898 2023-07-21 17:19:00.000000 demogpt-1.1.1.6/src/beta/langchain_coder.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     4368 2023-07-21 17:19:00.000000 demogpt-1.1.1.6/src/beta/langchain_expert.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     5537 2023-07-21 17:19:00.000000 demogpt-1.1.1.6/src/beta/model.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     1963 2023-07-21 08:30:31.000000 demogpt-1.1.1.6/src/beta/utils.py
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:45:14.016217 demogpt-1.1.1.6/src/demogpt.egg-info/
--rw-rw-r--   0 melih     (1000) melih     (1000)      409 2023-07-22 20:45:13.000000 demogpt-1.1.1.6/src/demogpt.egg-info/PKG-INFO
--rw-rw-r--   0 melih     (1000) melih     (1000)      991 2023-07-22 20:45:13.000000 demogpt-1.1.1.6/src/demogpt.egg-info/SOURCES.txt
--rw-rw-r--   0 melih     (1000) melih     (1000)        1 2023-07-22 20:45:13.000000 demogpt-1.1.1.6/src/demogpt.egg-info/dependency_links.txt
--rw-rw-r--   0 melih     (1000) melih     (1000)       50 2023-07-22 20:45:13.000000 demogpt-1.1.1.6/src/demogpt.egg-info/entry_points.txt
--rw-rw-r--   0 melih     (1000) melih     (1000)       41 2023-07-22 20:45:13.000000 demogpt-1.1.1.6/src/demogpt.egg-info/requires.txt
--rw-rw-r--   0 melih     (1000) melih     (1000)       24 2023-07-22 20:45:13.000000 demogpt-1.1.1.6/src/demogpt.egg-info/top_level.txt
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:45:14.016217 demogpt-1.1.1.6/src/prompt_based/
--rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-22 20:22:29.000000 demogpt-1.1.1.6/src/prompt_based/__init__.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     4158 2023-07-22 20:22:27.000000 demogpt-1.1.1.6/src/prompt_based/app.py
--rw-rw-r--   0 melih     (1000) melih     (1000)      230 2023-07-22 20:32:48.000000 demogpt-1.1.1.6/src/prompt_based/cli.py
--rw-rw-r--   0 melih     (1000) melih     (1000)    10650 2023-07-22 20:44:51.000000 demogpt-1.1.1.6/src/prompt_based/model.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     6115 2023-07-21 17:19:00.000000 demogpt-1.1.1.6/src/prompt_based/prompts.py
+drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:49:08.000589 demogpt-1.1.1.7/
+-rw-rw-r--   0 melih     (1000) melih     (1000)     1069 2023-06-07 10:58:37.000000 demogpt-1.1.1.7/LICENSE
+-rw-rw-r--   0 melih     (1000) melih     (1000)      409 2023-07-22 20:49:08.000589 demogpt-1.1.1.7/PKG-INFO
+-rw-rw-r--   0 melih     (1000) melih     (1000)     6530 2023-07-19 15:30:18.000000 demogpt-1.1.1.7/README.md
+-rw-rw-r--   0 melih     (1000) melih     (1000)       38 2023-07-22 20:49:08.000589 demogpt-1.1.1.7/setup.cfg
+-rw-rw-r--   0 melih     (1000) melih     (1000)      832 2023-07-22 20:49:01.000000 demogpt-1.1.1.7/setup.py
+drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:49:07.992589 demogpt-1.1.1.7/src/
+drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:49:07.996589 demogpt-1.1.1.7/src/alpha/
+-rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/__init__.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     4995 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/agent_prompts.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     3868 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/app.py
+drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:49:07.996589 demogpt-1.1.1.7/src/alpha/chains/
+-rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/chains/__init__.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     2444 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/chains/chains.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     7505 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/chains/prompts.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     4277 2023-07-22 17:12:22.000000 demogpt-1.1.1.7/src/alpha/code.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     1820 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/example_generation.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     8510 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/langchain_agent.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     8899 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/langchain_coder.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     4368 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/langchain_expert.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     5537 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/model.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     1963 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/utils.py
+drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:49:07.996589 demogpt-1.1.1.7/src/beta/
+-rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-21 08:30:31.000000 demogpt-1.1.1.7/src/beta/__init__.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     4995 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/beta/agent_prompts.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     3868 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/beta/app.py
+drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:49:07.996589 demogpt-1.1.1.7/src/beta/chains/
+-rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-21 08:30:31.000000 demogpt-1.1.1.7/src/beta/chains/__init__.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     2444 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/beta/chains/chains.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     7505 2023-07-21 08:30:31.000000 demogpt-1.1.1.7/src/beta/chains/prompts.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     1820 2023-07-21 08:30:31.000000 demogpt-1.1.1.7/src/beta/example_generation.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     8510 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/beta/langchain_agent.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     8898 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/beta/langchain_coder.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     4368 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/beta/langchain_expert.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     5537 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/beta/model.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     1963 2023-07-21 08:30:31.000000 demogpt-1.1.1.7/src/beta/utils.py
+drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:49:08.000589 demogpt-1.1.1.7/src/demogpt.egg-info/
+-rw-rw-r--   0 melih     (1000) melih     (1000)      409 2023-07-22 20:49:07.000000 demogpt-1.1.1.7/src/demogpt.egg-info/PKG-INFO
+-rw-rw-r--   0 melih     (1000) melih     (1000)     1020 2023-07-22 20:49:07.000000 demogpt-1.1.1.7/src/demogpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 melih     (1000) melih     (1000)        1 2023-07-22 20:49:07.000000 demogpt-1.1.1.7/src/demogpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 melih     (1000) melih     (1000)       50 2023-07-22 20:49:07.000000 demogpt-1.1.1.7/src/demogpt.egg-info/entry_points.txt
+-rw-rw-r--   0 melih     (1000) melih     (1000)       41 2023-07-22 20:49:07.000000 demogpt-1.1.1.7/src/demogpt.egg-info/requires.txt
+-rw-rw-r--   0 melih     (1000) melih     (1000)       24 2023-07-22 20:49:07.000000 demogpt-1.1.1.7/src/demogpt.egg-info/top_level.txt
+drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:49:08.000589 demogpt-1.1.1.7/src/prompt_based/
+-rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-22 20:22:29.000000 demogpt-1.1.1.7/src/prompt_based/__init__.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     4158 2023-07-22 20:22:27.000000 demogpt-1.1.1.7/src/prompt_based/app.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)      230 2023-07-22 20:32:48.000000 demogpt-1.1.1.7/src/prompt_based/cli.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)    10642 2023-07-22 20:48:24.000000 demogpt-1.1.1.7/src/prompt_based/model.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     6115 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/prompt_based/prompts.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     6169 2023-07-09 11:27:25.000000 demogpt-1.1.1.7/src/prompt_based/prompts.txt
```

### Comparing `demogpt-1.1.1.6/LICENSE` & `demogpt-1.1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/README.md` & `demogpt-1.1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/setup.py` & `demogpt-1.1.1.7/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name="demogpt",
-    version="1.1.1.6",
+    version="1.1.1.7",
     url="https://github.com/melih-unsal/DemoGPT",
     author="Melih Unsal",
     author_email="melih@demogpt.io",
     description="Description of my package",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
         "streamlit",
         "langchain",
         "openai",
         "python-dotenv"
     ],
     package_data={
-        "demogpt": ["prompt_based/prompts.txt"],
+    "prompt_based": ["prompts.txt"]
     },
     entry_points={
         "console_scripts": [
             "demogpt = prompt_based.cli:main",
         ]
     },
     classifiers=[
```

### Comparing `demogpt-1.1.1.6/src/alpha/agent_prompts.py` & `demogpt-1.1.1.7/src/alpha/agent_prompts.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/alpha/app.py` & `demogpt-1.1.1.7/src/alpha/app.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/alpha/chains/chains.py` & `demogpt-1.1.1.7/src/alpha/chains/chains.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/alpha/chains/prompts.py` & `demogpt-1.1.1.7/src/alpha/chains/prompts.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/alpha/code.py` & `demogpt-1.1.1.7/src/alpha/code.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/alpha/example_generation.py` & `demogpt-1.1.1.7/src/alpha/example_generation.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/alpha/langchain_agent.py` & `demogpt-1.1.1.7/src/alpha/langchain_agent.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/alpha/langchain_coder.py` & `demogpt-1.1.1.7/src/alpha/langchain_coder.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/alpha/langchain_expert.py` & `demogpt-1.1.1.7/src/alpha/langchain_expert.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/alpha/model.py` & `demogpt-1.1.1.7/src/alpha/model.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/alpha/utils.py` & `demogpt-1.1.1.7/src/alpha/utils.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/beta/agent_prompts.py` & `demogpt-1.1.1.7/src/beta/agent_prompts.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/beta/app.py` & `demogpt-1.1.1.7/src/beta/app.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/beta/chains/chains.py` & `demogpt-1.1.1.7/src/beta/chains/chains.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/beta/chains/prompts.py` & `demogpt-1.1.1.7/src/beta/chains/prompts.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/beta/example_generation.py` & `demogpt-1.1.1.7/src/beta/example_generation.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/beta/langchain_agent.py` & `demogpt-1.1.1.7/src/beta/langchain_agent.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/beta/langchain_coder.py` & `demogpt-1.1.1.7/src/beta/langchain_coder.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/beta/langchain_expert.py` & `demogpt-1.1.1.7/src/beta/langchain_expert.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/beta/model.py` & `demogpt-1.1.1.7/src/beta/model.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/beta/utils.py` & `demogpt-1.1.1.7/src/beta/utils.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/demogpt.egg-info/SOURCES.txt` & `demogpt-1.1.1.7/src/demogpt.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -32,8 +32,9 @@
 src/demogpt.egg-info/entry_points.txt
 src/demogpt.egg-info/requires.txt
 src/demogpt.egg-info/top_level.txt
 src/prompt_based/__init__.py
 src/prompt_based/app.py
 src/prompt_based/cli.py
 src/prompt_based/model.py
-src/prompt_based/prompts.py
+src/prompt_based/prompts.py
+src/prompt_based/prompts.txt
```

### Comparing `demogpt-1.1.1.6/src/prompt_based/app.py` & `demogpt-1.1.1.7/src/prompt_based/app.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.6/src/prompt_based/model.py` & `demogpt-1.1.1.7/src/prompt_based/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,16 +92,16 @@
         self.addDocuments()
 
     def addDocuments(self):
         """
         Adds documents to the logic model for generating Python code.
         """
         self.document = ""
-        for path in ["prompt_based/prompts.txt"]:
-            with resource_stream('demogpt', path) as f:
+        for path in ["prompts.txt"]:
+            with resource_stream('prompt_based', path) as f:
                 self.document += f.read().decode('utf-8')
 
     def decode_results(self, results):
         """
         Decodes the results returned by the executed python code
 
         Args:
```

### Comparing `demogpt-1.1.1.6/src/prompt_based/prompts.py` & `demogpt-1.1.1.7/src/prompt_based/prompts.py`

 * *Files identical despite different names*

