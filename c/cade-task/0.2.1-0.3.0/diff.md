# Comparing `tmp/cade_task-0.2.1.tar.gz` & `tmp/cade_task-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cade_task-0.2.1.tar", max compression
+gzip compressed data, was "cade_task-0.3.0.tar", max compression
```

## Comparing `cade_task-0.2.1.tar` & `cade_task-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-06-22 21:56:01.797435 cade_task-0.2.1/LICENSE
--rw-r--r--   0        0        0     3129 2023-07-18 17:48:03.192515 cade_task-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-07-18 17:17:25.645802 cade_task-0.2.1/cade_task/__init__.py
--rw-r--r--   0        0        0       61 2023-07-18 17:17:25.646114 cade_task-0.2.1/cade_task/__main__.py
--rw-r--r--   0        0        0     3889 2023-07-18 17:17:25.646439 cade_task-0.2.1/cade_task/cli.py
--rw-r--r--   0        0        0     2772 2023-07-18 17:17:25.646697 cade_task-0.2.1/cade_task/lib.py
--rw-r--r--   0        0        0      535 2023-07-19 02:12:15.658884 cade_task-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 cade_task-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-22 21:56:01.797435 cade_task-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2828 2023-07-22 17:27:22.754257 cade_task-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-18 17:17:25.645802 cade_task-0.3.0/cade_task/__init__.py
+-rw-r--r--   0        0        0       59 2023-07-22 17:27:22.754596 cade_task-0.3.0/cade_task/__main__.py
+-rw-r--r--   0        0        0     3788 2023-07-22 17:27:22.754812 cade_task-0.3.0/cade_task/cli.py
+-rw-r--r--   0        0        0     4230 2023-07-22 17:27:22.755112 cade_task-0.3.0/cade_task/lib.py
+-rw-r--r--   0        0        0      732 2023-07-22 18:02:20.189358 cade_task-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3252 1970-01-01 00:00:00.000000 cade_task-0.3.0/PKG-INFO
```

### Comparing `cade_task-0.2.1/LICENSE` & `cade_task-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cade_task-0.2.1/README.md` & `cade_task-0.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 # Task (cade-task)
+
 Task is a light CLI wrapper around Reminders.app ([reminders-cli](https://github.com/keith/reminders-cli)) that unifies use with dead-simple, sane defaults to remove friction from GTD.
 
 ## Install
 
-Installation is easiest via [brew](https://brew.sh/):
+[pipx](https://pypa.github.io/pipx/):
+
+```
+pipx install cade-task
+```
+
+[brew](https://brew.sh/):
+
+*Building bottles of python modules is flaky, not currently maintained*
 
 ```
-brew install cadeef/homebrew-tap/cade-task
+brew install cadeef/tap/cade-task
 ```
 
 ## Usage
 
 Commands are aware of project context where available. Task assumes you store all of your projects in the same directory (defined with `—-project-dir`), shell aliases are your friend.
 
 Short flags exist for all options, but the long version is used here for clarity.
@@ -25,16 +34,14 @@
 
 Not in your project directory? No problem, specify the list you’d like to interact with:
 
 ```
 task list —-list <yourgloriouslist>
 ```
 
-Don’t feel like passing a list? Specify `—-list` without an argument to select at the prompt.
-
 The list selection convention is consistent throughout the app.
 
 ### Add a Task
 
 ```
 task add A glorious task that should be completed
 ```
@@ -47,30 +54,29 @@
 
 ```
 task complete 6 1 3
 ```
 
 Tasks are completed in reverse numerical order (10...1) to avoid re-parsing the task list after each task is completed.
 
-
 ### Open Reminders.app
 
 Conveniently open (or bring to the foreground) Reminders.app:
 
 ```
 task open
 ```
 
-- - - -
+______________________________________________________________________
 
 Additional usage information is available via `—-help` on the command line.
 
 ### Shell Aliases
 
-I’m not keen on managing additional configuration files for simple applications so there is no external config to set, but the defaults may not work for you. Shell aliases let us accomplish similar without another file to manage. Define a different project directory from bash:
+The defaults may not work for you. Shell aliases are cheap and easy. Define a different project directory from bash:
 
 ```bash
 TASK_PROJECT_DIR=“${HOME}/myprettyneatprojectdir”
 # List tasks in current project
 alias t=“task -d ${TASK_PROJECT_DIR} list”
 # Add task in current project
 alias ta=“task -d ${TASK_PROJECT_DIR} add”
@@ -84,15 +90,14 @@
 alias to=“task open”
 ```
 
 Tweak until your heart is content without monkeying yet another config file.
 
 ## Caveats
 
-* Apple doesn’t expose the ability to create lists via the EventKit API or AppleScript. 😔 In scenarios where a project task list doesn’t exist, you’ll be prompted to create the list in Reminders.app.
-* Task wraps [Keith Smiley’s reminders-cli](https://github.com/keith/reminders-cli). Task is intended as a backend-agnostic wrapper that standardizes use without being tied to a specific implementation— I don’t want to retrain muscle memory if a new killer app comes along.
+- Task wraps [Keith Smiley’s reminders-cli](https://github.com/keith/reminders-cli). Task is intended as a backend-agnostic wrapper that standardizes use without being tied to a specific implementation— I don’t want to retrain muscle memory if a new killer app comes along.
 
 ## License
 
 This project is distributed under an MIT license, see [LICENSE](https://github.com/cadeef/cade-task/blob/main/LICENSE) for more information.
 
 Made it this far? **You deserve a hug.**
```

### Comparing `cade_task-0.2.1/cade_task/cli.py` & `cade_task-0.3.0/cade_task/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,150 +1,157 @@
 from pathlib import Path
-from typing import List, Sequence
+from typing import Optional
 
-import click
-from tablib import Dataset
+import typer
 
-from .lib import (  # isort:skip
+# from devtools import debug  # noqa: F401
+from rich import print
+from rich.console import Console
+from rich.table import Table
+from typing_extensions import Annotated
+
+from .lib import (
     ListNotFoundException,
     TaskCommandException,
+    TaskItem,
+    TaskList,
     get_lists,
-    get_tasks,
-    list_resolve,
+    list_name_from_path,
     run_and_return,
 )
 
 # Default
 PROJECT_DIR = Path.home() / "code"
 
+app = typer.Typer()
 
-@click.group()
-@click.option(
-    "-d",
-    "--project-dir",
-    "project_dir",
-    type=click.Path(exists=True),
-    required=False,
-    help="Base path for automatic directory-based list resolution",
-)
-@click.pass_context
-def main(ctx, project_dir: str | None) -> None:
-    if ctx.obj is None:
-        ctx.obj = dict()
-
-    project_dir = project_dir or str(PROJECT_DIR)
-    ctx.obj["project"] = list_resolve(project_dir)
 
+@app.callback()
+def main(
+    ctx: typer.Context,
+    project_dir: str = typer.Option(
+        default=str(PROJECT_DIR), envvar="TASK_PROJECT_DIR"
+    ),
+) -> None:
+    ctx.ensure_object(dict)
+
+    project = list_name_from_path(project_dir)
+
+    # Create list if it is a project in project_dir and doesn't exist
+    if project is not None:
+        task_list = TaskList(project)
+        if not task_list.exists():
+            task_list.create()
+            print(f":information_desk_person: Created list '{project}'.")
 
-@main.command()
-@click.pass_context
-@click.option("-l", "--list", "project", required=False)
-def list(ctx, project: str | None = None) -> None:
+    ctx.obj["project"] = project
+
+
+@app.command("list")
+def list_(
+    ctx: typer.Context, project: Annotated[Optional[str], typer.Option("--list")] = None
+) -> None:
     """
     List tasks for a given project
     """
-    project = project or ctx.obj["project"]
+    project = project_set(project, ctx.obj["project"])
 
-    if not project:
-        raise click.ClickException("Unable to determine list")
-
-    display_title(project)
     try:
-        tasks = [t["title"] for t in get_tasks(project)]  # type: ignore
-        display_table(tasks, ["Task"], number_lines=True)
+        task_list = TaskList(project)
+        tasks = [t.title for t in task_list.tasks()]  # type: ignore
     except ListNotFoundException:
-        raise click.ClickException(f"List '{project}' not found")
+        print(f":x: List '{project}' not found")
+        raise typer.Exit(code=1)
+
+    if not tasks:
+        print(":yawning_face: List empty.")
+    else:
+        table = Table(title="Tasks", show_header=False)
+
+        for index, task in enumerate(tasks):
+            table.add_row(str(index), task)
 
+        Console().print(table)
 
-@main.command()
-def lists() -> None:
+
+@app.command()
+def lists(create: Optional[str] = None) -> None:
     """
     List all Reminders.app lists
     """
-    try:
-        display_table(get_lists(), ["List"], number_lines=False)
-    except TaskCommandException as e:
-        raise click.ClickException(e)
+    if create:
+        task_list = TaskList(create)
+        task_list.create()
+        print(f"List '{create}' created.")
+    else:
+        lists = get_lists()
+        table = Table(title="Lists", show_header=False)
 
+        for list in lists:
+            table.add_row(list)
 
-@main.command()
-@click.pass_context
-@click.argument("task", nargs=-1)
-@click.option("-l", "--list", "project", required=False)
-def add(ctx, task: Sequence[str], project: str | None = None) -> None:
+        Console().print(table)
+
+
+@app.command()
+def add(
+    ctx: typer.Context,
+    title: list[str],
+    project: Annotated[Optional[str], typer.Option("--list")] = None,
+) -> None:
     """
     Add a task to a given project
     """
-    project = project or ctx.obj["project"]
-
-    if not project:
-        raise click.ClickException("Unable to determine list")
-
-    t = " ".join(str(i) for i in task)
-    if not t:
-        raise click.ClickException("No task specified, arborting")
-
-    try:
-        click.echo(run_and_return(["add", project, t])[0])
-    except TaskCommandException as e:
-        raise click.ClickException(e)
+    project = project_set(project, ctx.obj["project"])
+    title_str = " ".join(title)
+    task = TaskItem(title_str, project)
+    task.add()
+    print(f"Task '{title_str}' added to {project}.")
 
 
-@main.command()
-@click.pass_context
-@click.argument("tasks", nargs=-1)
-@click.option("-l", "--list", "project", required=False)
-def complete(ctx, tasks: Sequence[str], project: str | None = None) -> None:
+@app.command()
+def complete(
+    ctx: typer.Context,
+    tasks: list[str],
+    project: Annotated[Optional[str], typer.Option("--list")] = None,
+) -> None:
     """
     Complete task(s) for a given project
     """
-    if not project and not ctx.obj["project"]:
-        raise click.ClickException("Unable to determine list")
-
-    project = project or ctx.obj["project"]
+    project = project_set(project, ctx.obj["project"])
 
     for t in sorted(tasks, reverse=True):
-        try:
-            click.echo(run_and_return(["complete", project, t])[0])
-        except TaskCommandException as e:
-            raise click.ClickException(e)
+        # FIXME: setting a dummy title is inelegant
+        task = TaskItem(title="complete_task", parent=project, index=int(t))
+        task.complete()
+
+    print("Task(s) completed.")
 
 
-@main.command()
+@app.command()
 def open() -> None:
     """
     Open Reminders.app or move it to the foreground
     """
     try:
         run_and_return(
             ["/usr/bin/open", "/System/Applications/Reminders.app/"],
             inject_reminder=False,
         )
     except TaskCommandException as e:
-        raise click.ClickException(f"Command '{e.cmd}' failed with '{e.stderr}'")
+        print(f":x: Failed to open Reminders.app\n{e}")
+        raise typer.Exit(code=1)
 
 
-def display_table(
-    array: Sequence[str],
-    # FIXME: Having a function called list wasn't a great idea, figure out re-naming so list[str]
-    # can be used for consistency
-    headers: List[str],
-    number_lines=False,
-    tablefmt: str = "fancy_grid",
-) -> None:
-    if len(array) == 0:
-        raise click.ClickException("No results found")
-    else:
-        data = Dataset()
-        data.headers = headers
-        for t in array:
-            data.append([t])
-
-        click.echo(data.export("cli", showindex=number_lines, tablefmt=tablefmt))
+def project_set(first: str | None, second: str) -> str:
+    # This is dumb, but I wanted it out of the way without thinking more than function
+    project = first or second
 
+    if not project:
+        print(":exclamation: Unable to determine list")
+        raise typer.Exit(code=1)
 
-def display_title(title: str) -> None:
-    click.secho(f"{title}", fg="green", bold=True)
+    return project
 
 
 if __name__ == "__main__":
-    main()
+    app()
```

### Comparing `cade_task-0.2.1/pyproject.toml` & `cade_task-0.3.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 [tool.poetry]
 name = "cade-task"
-version = "0.2.1"
+version = "0.3.0"
 description = "A loose wrapper around reminders-cli"
 readme = "README.md"
 authors = ["Cade Ekblad-Frank <cade@e-f.me>"]
 
 [tool.poetry.urls]
 "Homepage" = "https://github.com/cadeef/cade-task"
 
 [tool.poetry.scripts]
-task = 'cade_task.cli:main'
+task = 'cade_task.cli:app'
 
 [tool.poetry.dependencies]
 python = "^3.11"
-click = "^8.1.5"
-tablib = {extras = ["cli"], version = "^3.5.0"}
+typer = {extras = ["all"], version = "^0.9.0"}
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+pytest-cov = "^4.1.0"
 pytest = "^7.4.0"
+black = "^23.7.0"
+ruff = "^0.0.278"
+mypy = "^1.4.1"
+devtools = "^0.11.0"
+pygments = "^2.15.1"
+coveralls = "^3.3.1"
 
 [build-system]
 requires = ["poetry>=1.5.1"]
 build-backend = "poetry.masonry.api"
+
+[tool.ruff]
+# https://beta.ruff.rs/docs/rules/
+select = ["E", "F", "I"]
```

### Comparing `cade_task-0.2.1/PKG-INFO` & `cade_task-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 Metadata-Version: 2.1
 Name: cade-task
-Version: 0.2.1
+Version: 0.3.0
 Summary: A loose wrapper around reminders-cli
 Author: Cade Ekblad-Frank
 Author-email: cade@e-f.me
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.1.5,<9.0.0)
-Requires-Dist: tablib[cli] (>=3.5.0,<4.0.0)
+Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Project-URL: Homepage, https://github.com/cadeef/cade-task
 Description-Content-Type: text/markdown
 
 # Task (cade-task)
+
 Task is a light CLI wrapper around Reminders.app ([reminders-cli](https://github.com/keith/reminders-cli)) that unifies use with dead-simple, sane defaults to remove friction from GTD.
 
 ## Install
 
-Installation is easiest via [brew](https://brew.sh/):
+[pipx](https://pypa.github.io/pipx/):
+
+```
+pipx install cade-task
+```
+
+[brew](https://brew.sh/):
+
+*Building bottles of python modules is flaky, not currently maintained*
 
 ```
-brew install cadeef/homebrew-tap/cade-task
+brew install cadeef/tap/cade-task
 ```
 
 ## Usage
 
 Commands are aware of project context where available. Task assumes you store all of your projects in the same directory (defined with `—-project-dir`), shell aliases are your friend.
 
 Short flags exist for all options, but the long version is used here for clarity.
@@ -39,16 +47,14 @@
 
 Not in your project directory? No problem, specify the list you’d like to interact with:
 
 ```
 task list —-list <yourgloriouslist>
 ```
 
-Don’t feel like passing a list? Specify `—-list` without an argument to select at the prompt.
-
 The list selection convention is consistent throughout the app.
 
 ### Add a Task
 
 ```
 task add A glorious task that should be completed
 ```
@@ -61,30 +67,29 @@
 
 ```
 task complete 6 1 3
 ```
 
 Tasks are completed in reverse numerical order (10...1) to avoid re-parsing the task list after each task is completed.
 
-
 ### Open Reminders.app
 
 Conveniently open (or bring to the foreground) Reminders.app:
 
 ```
 task open
 ```
 
-- - - -
+______________________________________________________________________
 
 Additional usage information is available via `—-help` on the command line.
 
 ### Shell Aliases
 
-I’m not keen on managing additional configuration files for simple applications so there is no external config to set, but the defaults may not work for you. Shell aliases let us accomplish similar without another file to manage. Define a different project directory from bash:
+The defaults may not work for you. Shell aliases are cheap and easy. Define a different project directory from bash:
 
 ```bash
 TASK_PROJECT_DIR=“${HOME}/myprettyneatprojectdir”
 # List tasks in current project
 alias t=“task -d ${TASK_PROJECT_DIR} list”
 # Add task in current project
 alias ta=“task -d ${TASK_PROJECT_DIR} add”
@@ -98,16 +103,15 @@
 alias to=“task open”
 ```
 
 Tweak until your heart is content without monkeying yet another config file.
 
 ## Caveats
 
-* Apple doesn’t expose the ability to create lists via the EventKit API or AppleScript. 😔 In scenarios where a project task list doesn’t exist, you’ll be prompted to create the list in Reminders.app.
-* Task wraps [Keith Smiley’s reminders-cli](https://github.com/keith/reminders-cli). Task is intended as a backend-agnostic wrapper that standardizes use without being tied to a specific implementation— I don’t want to retrain muscle memory if a new killer app comes along.
+- Task wraps [Keith Smiley’s reminders-cli](https://github.com/keith/reminders-cli). Task is intended as a backend-agnostic wrapper that standardizes use without being tied to a specific implementation— I don’t want to retrain muscle memory if a new killer app comes along.
 
 ## License
 
 This project is distributed under an MIT license, see [LICENSE](https://github.com/cadeef/cade-task/blob/main/LICENSE) for more information.
 
 Made it this far? **You deserve a hug.**
```

