# Comparing `tmp/demogpt-1.1.1.2.tar.gz` & `tmp/demogpt-1.1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demogpt-1.1.1.2.tar", last modified: Sat Jul 22 20:25:43 2023, max compression
+gzip compressed data, was "demogpt-1.1.1.3.tar", last modified: Sat Jul 22 20:33:32 2023, max compression
```

## Comparing `demogpt-1.1.1.2.tar` & `demogpt-1.1.1.3.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:25:43.365633 demogpt-1.1.1.2/
--rw-rw-r--   0 melih     (1000) melih     (1000)     1069 2023-06-07 10:58:37.000000 demogpt-1.1.1.2/LICENSE
--rw-rw-r--   0 melih     (1000) melih     (1000)      409 2023-07-22 20:25:43.365633 demogpt-1.1.1.2/PKG-INFO
--rw-rw-r--   0 melih     (1000) melih     (1000)     6530 2023-07-19 15:30:18.000000 demogpt-1.1.1.2/README.md
--rw-rw-r--   0 melih     (1000) melih     (1000)       38 2023-07-22 20:25:43.365633 demogpt-1.1.1.2/setup.cfg
--rw-rw-r--   0 melih     (1000) melih     (1000)      770 2023-07-22 20:25:34.000000 demogpt-1.1.1.2/setup.py
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:25:43.357634 demogpt-1.1.1.2/src/
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:25:43.357634 demogpt-1.1.1.2/src/alpha/
--rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-21 17:19:00.000000 demogpt-1.1.1.2/src/alpha/__init__.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     4995 2023-07-21 17:19:00.000000 demogpt-1.1.1.2/src/alpha/agent_prompts.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     3868 2023-07-21 17:19:00.000000 demogpt-1.1.1.2/src/alpha/app.py
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:25:43.361633 demogpt-1.1.1.2/src/alpha/chains/
--rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-21 17:19:00.000000 demogpt-1.1.1.2/src/alpha/chains/__init__.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     2444 2023-07-21 17:19:00.000000 demogpt-1.1.1.2/src/alpha/chains/chains.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     7505 2023-07-21 17:19:00.000000 demogpt-1.1.1.2/src/alpha/chains/prompts.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     4277 2023-07-22 17:12:22.000000 demogpt-1.1.1.2/src/alpha/code.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     1820 2023-07-21 17:19:00.000000 demogpt-1.1.1.2/src/alpha/example_generation.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     8510 2023-07-21 17:19:00.000000 demogpt-1.1.1.2/src/alpha/langchain_agent.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     8899 2023-07-21 17:19:00.000000 demogpt-1.1.1.2/src/alpha/langchain_coder.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     4368 2023-07-21 17:19:00.000000 demogpt-1.1.1.2/src/alpha/langchain_expert.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     5537 2023-07-21 17:19:00.000000 demogpt-1.1.1.2/src/alpha/model.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     1963 2023-07-21 17:19:00.000000 demogpt-1.1.1.2/src/alpha/utils.py
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:25:43.361633 demogpt-1.1.1.2/src/beta/
--rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-21 08:30:31.000000 demogpt-1.1.1.2/src/beta/__init__.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     4995 2023-07-21 17:19:00.000000 demogpt-1.1.1.2/src/beta/agent_prompts.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     3868 2023-07-21 17:19:00.000000 demogpt-1.1.1.2/src/beta/app.py
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:25:43.361633 demogpt-1.1.1.2/src/beta/chains/
--rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-21 08:30:31.000000 demogpt-1.1.1.2/src/beta/chains/__init__.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     2444 2023-07-21 17:19:00.000000 demogpt-1.1.1.2/src/beta/chains/chains.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     7505 2023-07-21 08:30:31.000000 demogpt-1.1.1.2/src/beta/chains/prompts.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     1820 2023-07-21 08:30:31.000000 demogpt-1.1.1.2/src/beta/example_generation.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     8510 2023-07-21 17:19:00.000000 demogpt-1.1.1.2/src/beta/langchain_agent.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     8898 2023-07-21 17:19:00.000000 demogpt-1.1.1.2/src/beta/langchain_coder.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     4368 2023-07-21 17:19:00.000000 demogpt-1.1.1.2/src/beta/langchain_expert.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     5537 2023-07-21 17:19:00.000000 demogpt-1.1.1.2/src/beta/model.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     1963 2023-07-21 08:30:31.000000 demogpt-1.1.1.2/src/beta/utils.py
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:25:43.365633 demogpt-1.1.1.2/src/demogpt.egg-info/
--rw-rw-r--   0 melih     (1000) melih     (1000)      409 2023-07-22 20:25:43.000000 demogpt-1.1.1.2/src/demogpt.egg-info/PKG-INFO
--rw-rw-r--   0 melih     (1000) melih     (1000)      967 2023-07-22 20:25:43.000000 demogpt-1.1.1.2/src/demogpt.egg-info/SOURCES.txt
--rw-rw-r--   0 melih     (1000) melih     (1000)        1 2023-07-22 20:25:43.000000 demogpt-1.1.1.2/src/demogpt.egg-info/dependency_links.txt
--rw-rw-r--   0 melih     (1000) melih     (1000)       50 2023-07-22 20:25:43.000000 demogpt-1.1.1.2/src/demogpt.egg-info/entry_points.txt
--rw-rw-r--   0 melih     (1000) melih     (1000)       41 2023-07-22 20:25:43.000000 demogpt-1.1.1.2/src/demogpt.egg-info/requires.txt
--rw-rw-r--   0 melih     (1000) melih     (1000)       24 2023-07-22 20:25:43.000000 demogpt-1.1.1.2/src/demogpt.egg-info/top_level.txt
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:25:43.365633 demogpt-1.1.1.2/src/prompt_based/
--rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-22 20:22:29.000000 demogpt-1.1.1.2/src/prompt_based/__init__.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     4158 2023-07-22 20:22:27.000000 demogpt-1.1.1.2/src/prompt_based/app.py
--rw-rw-r--   0 melih     (1000) melih     (1000)    10574 2023-07-22 20:22:05.000000 demogpt-1.1.1.2/src/prompt_based/model.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     6115 2023-07-21 17:19:00.000000 demogpt-1.1.1.2/src/prompt_based/prompts.py
+drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:33:32.299214 demogpt-1.1.1.3/
+-rw-rw-r--   0 melih     (1000) melih     (1000)     1069 2023-06-07 10:58:37.000000 demogpt-1.1.1.3/LICENSE
+-rw-rw-r--   0 melih     (1000) melih     (1000)      409 2023-07-22 20:33:32.295212 demogpt-1.1.1.3/PKG-INFO
+-rw-rw-r--   0 melih     (1000) melih     (1000)     6530 2023-07-19 15:30:18.000000 demogpt-1.1.1.3/README.md
+-rw-rw-r--   0 melih     (1000) melih     (1000)       38 2023-07-22 20:33:32.299214 demogpt-1.1.1.3/setup.cfg
+-rw-rw-r--   0 melih     (1000) melih     (1000)      770 2023-07-22 20:33:27.000000 demogpt-1.1.1.3/setup.py
+drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:33:32.287210 demogpt-1.1.1.3/src/
+drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:33:32.291211 demogpt-1.1.1.3/src/alpha/
+-rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-21 17:19:00.000000 demogpt-1.1.1.3/src/alpha/__init__.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     4995 2023-07-21 17:19:00.000000 demogpt-1.1.1.3/src/alpha/agent_prompts.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     3868 2023-07-21 17:19:00.000000 demogpt-1.1.1.3/src/alpha/app.py
+drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:33:32.291211 demogpt-1.1.1.3/src/alpha/chains/
+-rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-21 17:19:00.000000 demogpt-1.1.1.3/src/alpha/chains/__init__.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     2444 2023-07-21 17:19:00.000000 demogpt-1.1.1.3/src/alpha/chains/chains.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     7505 2023-07-21 17:19:00.000000 demogpt-1.1.1.3/src/alpha/chains/prompts.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     4277 2023-07-22 17:12:22.000000 demogpt-1.1.1.3/src/alpha/code.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     1820 2023-07-21 17:19:00.000000 demogpt-1.1.1.3/src/alpha/example_generation.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     8510 2023-07-21 17:19:00.000000 demogpt-1.1.1.3/src/alpha/langchain_agent.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     8899 2023-07-21 17:19:00.000000 demogpt-1.1.1.3/src/alpha/langchain_coder.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     4368 2023-07-21 17:19:00.000000 demogpt-1.1.1.3/src/alpha/langchain_expert.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     5537 2023-07-21 17:19:00.000000 demogpt-1.1.1.3/src/alpha/model.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     1963 2023-07-21 17:19:00.000000 demogpt-1.1.1.3/src/alpha/utils.py
+drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:33:32.291211 demogpt-1.1.1.3/src/beta/
+-rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-21 08:30:31.000000 demogpt-1.1.1.3/src/beta/__init__.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     4995 2023-07-21 17:19:00.000000 demogpt-1.1.1.3/src/beta/agent_prompts.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     3868 2023-07-21 17:19:00.000000 demogpt-1.1.1.3/src/beta/app.py
+drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:33:32.295212 demogpt-1.1.1.3/src/beta/chains/
+-rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-21 08:30:31.000000 demogpt-1.1.1.3/src/beta/chains/__init__.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     2444 2023-07-21 17:19:00.000000 demogpt-1.1.1.3/src/beta/chains/chains.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     7505 2023-07-21 08:30:31.000000 demogpt-1.1.1.3/src/beta/chains/prompts.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     1820 2023-07-21 08:30:31.000000 demogpt-1.1.1.3/src/beta/example_generation.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     8510 2023-07-21 17:19:00.000000 demogpt-1.1.1.3/src/beta/langchain_agent.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     8898 2023-07-21 17:19:00.000000 demogpt-1.1.1.3/src/beta/langchain_coder.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     4368 2023-07-21 17:19:00.000000 demogpt-1.1.1.3/src/beta/langchain_expert.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     5537 2023-07-21 17:19:00.000000 demogpt-1.1.1.3/src/beta/model.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     1963 2023-07-21 08:30:31.000000 demogpt-1.1.1.3/src/beta/utils.py
+drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:33:32.295212 demogpt-1.1.1.3/src/demogpt.egg-info/
+-rw-rw-r--   0 melih     (1000) melih     (1000)      409 2023-07-22 20:33:32.000000 demogpt-1.1.1.3/src/demogpt.egg-info/PKG-INFO
+-rw-rw-r--   0 melih     (1000) melih     (1000)      991 2023-07-22 20:33:32.000000 demogpt-1.1.1.3/src/demogpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 melih     (1000) melih     (1000)        1 2023-07-22 20:33:32.000000 demogpt-1.1.1.3/src/demogpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 melih     (1000) melih     (1000)       50 2023-07-22 20:33:32.000000 demogpt-1.1.1.3/src/demogpt.egg-info/entry_points.txt
+-rw-rw-r--   0 melih     (1000) melih     (1000)       41 2023-07-22 20:33:32.000000 demogpt-1.1.1.3/src/demogpt.egg-info/requires.txt
+-rw-rw-r--   0 melih     (1000) melih     (1000)       24 2023-07-22 20:33:32.000000 demogpt-1.1.1.3/src/demogpt.egg-info/top_level.txt
+drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:33:32.295212 demogpt-1.1.1.3/src/prompt_based/
+-rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-22 20:22:29.000000 demogpt-1.1.1.3/src/prompt_based/__init__.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     4158 2023-07-22 20:22:27.000000 demogpt-1.1.1.3/src/prompt_based/app.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)      230 2023-07-22 20:32:48.000000 demogpt-1.1.1.3/src/prompt_based/cli.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)    10574 2023-07-22 20:22:05.000000 demogpt-1.1.1.3/src/prompt_based/model.py
+-rw-rw-r--   0 melih     (1000) melih     (1000)     6115 2023-07-21 17:19:00.000000 demogpt-1.1.1.3/src/prompt_based/prompts.py
```

### Comparing `demogpt-1.1.1.2/LICENSE` & `demogpt-1.1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/README.md` & `demogpt-1.1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/setup.py` & `demogpt-1.1.1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name="demogpt",
-    version="1.1.1.2",
+    version="1.1.1.3",
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
     entry_points={
         "console_scripts": [
-            "demogpt = prompt_based.app:main",
+            "demogpt = prompt_based.cli:main",
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `demogpt-1.1.1.2/src/alpha/agent_prompts.py` & `demogpt-1.1.1.3/src/alpha/agent_prompts.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/alpha/app.py` & `demogpt-1.1.1.3/src/alpha/app.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/alpha/chains/chains.py` & `demogpt-1.1.1.3/src/alpha/chains/chains.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/alpha/chains/prompts.py` & `demogpt-1.1.1.3/src/alpha/chains/prompts.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/alpha/code.py` & `demogpt-1.1.1.3/src/alpha/code.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/alpha/example_generation.py` & `demogpt-1.1.1.3/src/alpha/example_generation.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/alpha/langchain_agent.py` & `demogpt-1.1.1.3/src/alpha/langchain_agent.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/alpha/langchain_coder.py` & `demogpt-1.1.1.3/src/alpha/langchain_coder.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/alpha/langchain_expert.py` & `demogpt-1.1.1.3/src/alpha/langchain_expert.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/alpha/model.py` & `demogpt-1.1.1.3/src/alpha/model.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/alpha/utils.py` & `demogpt-1.1.1.3/src/alpha/utils.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/beta/agent_prompts.py` & `demogpt-1.1.1.3/src/beta/agent_prompts.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/beta/app.py` & `demogpt-1.1.1.3/src/beta/app.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/beta/chains/chains.py` & `demogpt-1.1.1.3/src/beta/chains/chains.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/beta/chains/prompts.py` & `demogpt-1.1.1.3/src/beta/chains/prompts.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/beta/example_generation.py` & `demogpt-1.1.1.3/src/beta/example_generation.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/beta/langchain_agent.py` & `demogpt-1.1.1.3/src/beta/langchain_agent.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/beta/langchain_coder.py` & `demogpt-1.1.1.3/src/beta/langchain_coder.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/beta/langchain_expert.py` & `demogpt-1.1.1.3/src/beta/langchain_expert.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/beta/model.py` & `demogpt-1.1.1.3/src/beta/model.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/beta/utils.py` & `demogpt-1.1.1.3/src/beta/utils.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/demogpt.egg-info/SOURCES.txt` & `demogpt-1.1.1.3/src/demogpt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -30,9 +30,10 @@
 src/demogpt.egg-info/SOURCES.txt
 src/demogpt.egg-info/dependency_links.txt
 src/demogpt.egg-info/entry_points.txt
 src/demogpt.egg-info/requires.txt
 src/demogpt.egg-info/top_level.txt
 src/prompt_based/__init__.py
 src/prompt_based/app.py
+src/prompt_based/cli.py
 src/prompt_based/model.py
 src/prompt_based/prompts.py
```

### Comparing `demogpt-1.1.1.2/src/prompt_based/app.py` & `demogpt-1.1.1.3/src/prompt_based/app.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/prompt_based/model.py` & `demogpt-1.1.1.3/src/prompt_based/model.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.2/src/prompt_based/prompts.py` & `demogpt-1.1.1.3/src/prompt_based/prompts.py`

 * *Files identical despite different names*

