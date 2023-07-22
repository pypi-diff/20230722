# Comparing `tmp/nextflowpy-0.6.2-py3-none-any.whl.zip` & `tmp/nextflowpy-0.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 29110 bytes, number of entries: 14
--rw-r--r--  2.0 unx      312 b- defN 23-Jul-21 10:13 nextflow/__init__.py
--rw-r--r--  2.0 unx     8731 b- defN 23-Jul-07 18:57 nextflow/command.py
+Zip file size: 29427 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      312 b- defN 23-Jul-22 10:14 nextflow/__init__.py
+-rw-r--r--  2.0 unx    10057 b- defN 23-Jul-22 13:05 nextflow/command.py
 -rw-r--r--  2.0 unx      148 b- defN 23-Feb-09 15:42 nextflow/exceptions.py
 -rw-r--r--  2.0 unx     9133 b- defN 22-Oct-31 17:04 nextflow/execution.py
 -rw-r--r--  2.0 unx     1155 b- defN 23-May-24 20:50 nextflow/io.py
 -rw-r--r--  2.0 unx     3862 b- defN 23-Apr-07 01:28 nextflow/log.py
 -rw-r--r--  2.0 unx     3228 b- defN 23-Jul-21 10:15 nextflow/models.py
 -rw-r--r--  2.0 unx     7652 b- defN 22-Oct-31 17:06 nextflow/pipeline.py
 -rw-r--r--  2.0 unx     6989 b- defN 22-Oct-31 17:04 nextflow/utils.py
--rw-r--r--  2.0 unx    35148 b- defN 23-Jul-21 10:35 nextflowpy-0.6.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    11967 b- defN 23-Jul-21 10:35 nextflowpy-0.6.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 10:35 nextflowpy-0.6.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-21 10:35 nextflowpy-0.6.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1079 b- defN 23-Jul-21 10:35 nextflowpy-0.6.2.dist-info/RECORD
-14 files, 89505 bytes uncompressed, 27344 bytes compressed:  69.4%
+-rw-r--r--  2.0 unx    35148 b- defN 23-Jul-22 15:22 nextflowpy-0.7.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12707 b- defN 23-Jul-22 15:22 nextflowpy-0.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-22 15:22 nextflowpy-0.7.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-22 15:22 nextflowpy-0.7.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1080 b- defN 23-Jul-22 15:22 nextflowpy-0.7.0.dist-info/RECORD
+14 files, 91572 bytes uncompressed, 27661 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: nextflow/pipeline.py
 Comment: 
 
 Filename: nextflow/utils.py
 Comment: 
 
-Filename: nextflowpy-0.6.2.dist-info/LICENSE
+Filename: nextflowpy-0.7.0.dist-info/LICENSE
 Comment: 
 
-Filename: nextflowpy-0.6.2.dist-info/METADATA
+Filename: nextflowpy-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: nextflowpy-0.6.2.dist-info/WHEEL
+Filename: nextflowpy-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: nextflowpy-0.6.2.dist-info/top_level.txt
+Filename: nextflowpy-0.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: nextflowpy-0.6.2.dist-info/RECORD
+Filename: nextflowpy-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nextflow/__init__.py

```diff
@@ -1,11 +1,11 @@
 from shutil import which
 from .exceptions import NextflowNotInstalledError
 from .command import run, run_and_poll
 
 __author__ = "Sam Ireland"
-__version__ = "0.6.2"
+__version__ = "0.7.0"
 
 if not which("nextflow"):
     raise NextflowNotInstalledError(
         "Nextflow is either not installed, not in PATH, or is not executable."
     )
```

## nextflow/command.py

```diff
@@ -20,14 +20,17 @@
     :param str run_path: the location to run the pipeline in.
     :param function runner: a function to run the pipeline command.
     :param str version: the nextflow version to use.
     :param list configs: any config files to be applied.
     :param dict params: the parameters to pass.
     :param list profiles: any profiles to be applied.
     :param str timezone: the timezone to use for the log.
+    :param str report: the filename to use for the execution report.
+    :param str timeline: the filename to use for the timeline report.
+    :param str dag: the filename to use for the DAG report.
     :rtype: ``nextflow.models.Execution``"""
 
     return list(_run(*args, poll=False, **kwargs))[0]
 
 
 def run_and_poll(*args, **kwargs):
     """Runs a pipeline and polls it for updates. Yields the execution after each
@@ -37,28 +40,33 @@
     :param str run_path: the location to run the pipeline in.
     :param function runner: a function to run the pipeline command.
     :param str version: the nextflow version to use.
     :param list configs: any config files to be applied.
     :param dict params: the parameters to pass.
     :param list profiles: any profiles to be applied.
     :param str timezone: the timezone to use for the log.
+    :param str report: the filename to use for the execution report.
+    :param str timeline: the filename to use for the timeline report.
+    :param str dag: the filename to use for the DAG report.
     :param int sleep: the number of seconds to wait between polls.
     :rtype: ``nextflow.models.Execution``"""
 
     for execution in _run(*args, poll=True, **kwargs):
         yield execution
 
 
 def _run(
         pipeline_path, poll=False, run_path=None, runner=None, version=None,
-        configs=None, params=None, profiles=None, timezone=None, sleep=1
+        configs=None, params=None, profiles=None, timezone=None, report=None,
+        timeline=None, dag=None, sleep=1
 ):
     if not run_path: run_path = os.path.abspath(".")
     nextflow_command = make_nextflow_command(
-        run_path, pipeline_path, version, configs, params, profiles, timezone
+        run_path, pipeline_path, version, configs, params, profiles, timezone,
+        report, timeline, dag
     )
     if runner:
         process = None
         runner(nextflow_command)
     else:
         process = subprocess.Popen(
             nextflow_command, universal_newlines=True, shell=True        
@@ -70,34 +78,38 @@
         if execution and poll: yield execution
         process_finished = not process or process.poll() is not None
         if execution and execution.return_code and process_finished:
             if not poll: yield execution
             break
 
 
-def make_nextflow_command(run_path, pipeline_path, version, configs, params, profiles, timezone):
+def make_nextflow_command(run_path, pipeline_path, version, configs, params, profiles, timezone, report, timeline, dag):
     """Generates the `nextflow run` commmand.
     
     :param str run_path: the location to run the pipeline in.
     :param str pipeline_path: the absolute path to the pipeline .nf file.
     :param str version: the nextflow version to use.
     :param list configs: any config files to be applied.
     :param dict params: the parameters to pass.
     :param list profiles: any profiles to be applied.
     :param str timezone: the timezone to use.
+    :param str report: the filename to use for the execution report.
+    :param str timeline: the filename to use for the timeline report.
+    :param str dag: the filename to use for the DAG report.
     :rtype: ``str``"""
 
     env = make_nextflow_command_env_string(version, timezone)
     if env: env += " "
     nf = "nextflow -Duser.country=US"
     configs = make_nextflow_command_config_string(configs)
     if configs: configs += " "
     params = make_nextflow_command_params_string(params)
     profiles = make_nextflow_command_profiles_string(profiles)
-    command = f"{env}{nf} {configs}run {pipeline_path} {params} {profiles}"
+    reports = make_reports_string(report, timeline, dag)
+    command = f"{env}{nf} {configs}run {pipeline_path} {params} {profiles} {reports}"
     if run_path: command = f"cd {run_path}; {command}"
     command = command.rstrip() + " >stdout.txt 2>stderr.txt; echo $? >rc.txt"
     return command
 
 
 def make_nextflow_command_env_string(version, timezone):
     """Creates the environment variable setting portion of the nextflow run
@@ -143,14 +155,29 @@
     :param list profiles: any profiles to be applied.
     :rtype: ``str``"""
 
     if not profiles: return ""
     return ("-profile " + ",".join(profiles))
 
 
+def make_reports_string(report, timeline, dag):
+    """Creates the report setting portion of the nextflow run command string.
+    
+    :param str report: the filename to use for the execution report.
+    :param str timeline: the filename to use for the timeline report.
+    :param str dag: the filename to use for the DAG report.
+    :rtype: ``str``"""
+
+    params = []
+    if report: params.append(f"-with-report {report}")
+    if timeline: params.append(f"-with-timeline {timeline}")
+    if dag: params.append(f"-with-dag {dag}")
+    return " ".join(params)
+
+
 def get_execution(execution_path, nextflow_command):
     """Creates an execution object from a location.
     
     :param str execution_path: the location of the execution.
     :param str nextflow_command: the command used to run the pipeline.
     :rtype: ``nextflow.models.Execution``"""
```

## Comparing `nextflowpy-0.6.2.dist-info/LICENSE` & `nextflowpy-0.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nextflowpy-0.6.2.dist-info/METADATA` & `nextflowpy-0.7.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextflowpy
-Version: 0.6.2
+Version: 0.7.0
 Summary: A Python wrapper around Nextflow.
 Home-page: https://github.com/goodwright/nextflow.py
 Author: Sam Ireland
 Author-email: sam@goodwright.com
 License: GPLv3+
 Keywords: nextflow bioinformatics pipeline
 Platform: UNKNOWN
@@ -32,18 +32,18 @@
 
 .. |version| image:: https://img.shields.io/pypi/v/nextflowpy.svg
   :target: https://pypi.org/project/nextflowpy/
 
 .. |pypi| image:: https://img.shields.io/pypi/pyversions/nextflowpy.svg
   :target: https://pypi.org/project/nextflowpy/
 
-.. |nextfow| image:: https://img.shields.io/badge/Nextflow-22.04%20%7C%2021.10%20%7C%2020.10-orange
+.. |nextfow| image:: https://img.shields.io/badge/Nextflow-23.04%20%7C%2022.04%20%7C%2021.10-orange
   :target: https://www.nextflow.io/
 
-.. |license| image:: https://img.shields.io/pypi/l/nextflowpy.svg?color=blue)
+.. |license| image:: https://img.shields.io/pypi/l/nextflowpy.svg?color=blue
   :target: https://github.com/goodwright/nextflow.py/blob/master/LICENSE
 
 nextflow.py is a Python wrapper around the Nextflow pipeline framework. It lets
 you run Nextflow pipelines from Python code.
 
 Example
 -------
@@ -111,28 +111,34 @@
 
     >>> pipeline = nextflow.run("pipelines/my-pipeline.nf")
 
 This will return an ``Execution`` object, which represents the pipeline
 execution that just took place (see below for details on this object). You can
 customise the execution with various options:
 
-    >>> execution = pipeline.run("my-pipeline.nf", run_path="./rundir", params={"param1": "123"}, profiles=["docker", "test"], version="22.0.1", configs=["env.config"])
+    >>> execution = pipeline.run("my-pipeline.nf", run_path="./rundir", params={"param1": "123"}, profiles=["docker", "test"], version="22.0.1", configs=["env.config"], timezone="UTC", report="report.html", timeline="timeline.html", dag="dag.html")
 
 * ``run_path`` - The location to run the pipeline from, which by default is just the current working directory.
 
 * ``params`` - A dictionary of parameters to pass to the pipeline as command. In the above example, this would run the pipeline with ``--param1=123``.
 
 * ``profiles`` - A list of Nextflow profiles to use when running the pipeline. These are defined in the ``nextflow.config`` file, and can be used to configure things like the executor to use, or the container engine to use. In the above example, this would run the pipeline with ``-profile docker,test``.
 
 * ``version`` - The version of Nextflow to use when running the pipeline. By default, the version of Nextflow installed on the system is used, but this can be overridden with this parameter.
 
 * ``configs`` - A list of config files to use when running the pipeline. These are merged with the config files specified in the pipeline itself, and can be used to override any of the settings in the pipeline config.
 
 * ``timezone`` - A timezone to pass to Nextflow - this determines the timestamps used in the log file.
 
+* ``report`` - A filename for a report file to generate. This will be an HTML file containing information about the pipeline execution.
+
+* ``timeline`` - A filename for a timeline file to generate. This will be an HTML file containing a timeline of the pipeline execution.
+
+* ``dag`` - A filename for a DAG file to generate. This will be an HTML file containing a DAG diagram of the pipeline execution.
+
 
 Custom Runners
 ~~~~~~~~~~~~~~
 
 When you run a pipeline with nextflow.py, it will generate the command string
 that you would use at the command line if you were running the pipeline
 manually. This will be some variant of ``nextflow run some-pipeline.nf``, and
@@ -244,14 +250,25 @@
    'published' via some channel, and those which weren't. It is not possible to
    distinguish these once execution is complete, so nextflow.py reports all
    output files, not just those which are 'published'.
 
 Changelog
 ---------
 
+Release 0.7.0
+~~~~~~~~~~~~~
+
+`22nd July, 2023`
+
+* An execution report can now be published with the `report` parameter.
+* A timeline report can now be published with the `timeline` parameter.
+* A DAG report can now be published with the `dag` parameter.
+
+
+
 Release 0.6.2
 ~~~~~~~~~~~~~
 
 `21st July, 2023`
 
 * Fixed issue in handling no path for process execution input data.
```

## Comparing `nextflowpy-0.6.2.dist-info/RECORD` & `nextflowpy-0.7.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-nextflow/__init__.py,sha256=vCuuDX0NgDbWo0-DPycL5t-sawl2kNPAJTWqph-eVnA,312
-nextflow/command.py,sha256=bHJ382e43utvSwJUnJhzeEGUcN0Ahx7Fy7HPpTLXrTs,8731
+nextflow/__init__.py,sha256=_r1T_P2CkKMU5_OX-bFTXGjKKLcenYVroRa8mrfz2bU,312
+nextflow/command.py,sha256=acOnGStAXtJ0PXGHtPUWKm2N76JaVHC2bzk7ryTm4zA,10057
 nextflow/exceptions.py,sha256=ktaEfdLca9Bk52CtJoKYMkGaXLrQ9dZVfYh0QtSC9lk,148
 nextflow/execution.py,sha256=j_wsEuqyZafY3BapmhQBkxAmEJsnq9X-a8ADW3Bs0LA,9133
 nextflow/io.py,sha256=8BuYCRGfsI8_oGRkeY3hjTcT4CC_8eFk21Db-Zo5UIk,1155
 nextflow/log.py,sha256=uuL2bMUmuh2iplkfnX6Ch-LgDiWEcZLNxPvEO761yyU,3862
 nextflow/models.py,sha256=Q57ZRefj1EsNwdILanWpg_KriNgIvq6za4xLoxqAUfI,3228
 nextflow/pipeline.py,sha256=XUCsUtcGW3Ou6resfZJIWGkc5rfAq4gAY-jmZ4md9xo,7652
 nextflow/utils.py,sha256=7jSVHEc57_dZb8ZUNVrpUxIQTs3cp7wLQU9R-r-K6OE,6989
-nextflowpy-0.6.2.dist-info/LICENSE,sha256=ixuiBLtpoK3iv89l7ylKkg9rs2GzF9ukPH7ynZYzK5s,35148
-nextflowpy-0.6.2.dist-info/METADATA,sha256=kSBtb34x7dT2hTcS06-4lCWoX3h5B6JRoeS4V-k7Ztg,11967
-nextflowpy-0.6.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-nextflowpy-0.6.2.dist-info/top_level.txt,sha256=uD97_QD0Jwq__urXtKK-PQMFxiAjWT-y63C2Oi_lad0,9
-nextflowpy-0.6.2.dist-info/RECORD,,
+nextflowpy-0.7.0.dist-info/LICENSE,sha256=ixuiBLtpoK3iv89l7ylKkg9rs2GzF9ukPH7ynZYzK5s,35148
+nextflowpy-0.7.0.dist-info/METADATA,sha256=eyLZZSTgaxHDiYHSzHlQXqqPFbA_NsKmI7C_-OR3cPw,12707
+nextflowpy-0.7.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+nextflowpy-0.7.0.dist-info/top_level.txt,sha256=uD97_QD0Jwq__urXtKK-PQMFxiAjWT-y63C2Oi_lad0,9
+nextflowpy-0.7.0.dist-info/RECORD,,
```

