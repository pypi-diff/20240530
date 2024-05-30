# Comparing `tmp/pr_pilot_cli-1.3.0.tar.gz` & `tmp/pr_pilot_cli-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr_pilot_cli-1.3.0.tar", last modified: Tue May 28 01:41:31 2024, max compression
+gzip compressed data, was "pr_pilot_cli-1.3.1.tar", last modified: Thu May 30 17:51:15 2024, max compression
```

## Comparing `pr_pilot_cli-1.3.0.tar` & `pr_pilot_cli-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:41:31.785709 pr_pilot_cli-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 01:41:26.000000 pr_pilot_cli-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 01:41:26.000000 pr_pilot_cli-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-28 01:41:31.785709 pr_pilot_cli-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-28 01:41:26.000000 pr_pilot_cli-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:41:31.781710 pr_pilot_cli-1.3.0/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 01:41:26.000000 pr_pilot_cli-1.3.0/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-28 01:41:26.000000 pr_pilot_cli-1.3.0/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-28 01:41:26.000000 pr_pilot_cli-1.3.0/cli/detect_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:41:31.785709 pr_pilot_cli-1.3.0/pr_pilot_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-28 01:41:31.000000 pr_pilot_cli-1.3.0/pr_pilot_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-28 01:41:31.000000 pr_pilot_cli-1.3.0/pr_pilot_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:41:31.000000 pr_pilot_cli-1.3.0/pr_pilot_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 01:41:31.000000 pr_pilot_cli-1.3.0/pr_pilot_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 01:41:31.000000 pr_pilot_cli-1.3.0/pr_pilot_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-28 01:41:31.000000 pr_pilot_cli-1.3.0/pr_pilot_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 01:41:26.000000 pr_pilot_cli-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 01:41:31.785709 pr_pilot_cli-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-28 01:41:26.000000 pr_pilot_cli-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:51:15.216295 pr_pilot_cli-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 17:51:11.000000 pr_pilot_cli-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 17:51:11.000000 pr_pilot_cli-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-30 17:51:15.216295 pr_pilot_cli-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-30 17:51:11.000000 pr_pilot_cli-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:51:15.212295 pr_pilot_cli-1.3.1/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:51:11.000000 pr_pilot_cli-1.3.1/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-30 17:51:11.000000 pr_pilot_cli-1.3.1/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-30 17:51:11.000000 pr_pilot_cli-1.3.1/cli/detect_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-30 17:51:11.000000 pr_pilot_cli-1.3.1/cli/task_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-30 17:51:11.000000 pr_pilot_cli-1.3.1/cli/templating.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:51:15.216295 pr_pilot_cli-1.3.1/pr_pilot_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-30 17:51:15.000000 pr_pilot_cli-1.3.1/pr_pilot_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-30 17:51:15.000000 pr_pilot_cli-1.3.1/pr_pilot_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 17:51:15.000000 pr_pilot_cli-1.3.1/pr_pilot_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 17:51:15.000000 pr_pilot_cli-1.3.1/pr_pilot_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-30 17:51:15.000000 pr_pilot_cli-1.3.1/pr_pilot_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-30 17:51:15.000000 pr_pilot_cli-1.3.1/pr_pilot_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-30 17:51:11.000000 pr_pilot_cli-1.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 17:51:15.216295 pr_pilot_cli-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-30 17:51:11.000000 pr_pilot_cli-1.3.1/setup.py
```

### Comparing `pr_pilot_cli-1.3.0/LICENSE` & `pr_pilot_cli-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.3.0/PKG-INFO` & `pr_pilot_cli-1.3.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: pr-pilot-cli
-Version: 1.3.0
-Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
-Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
-Author: Marco Lamina
-Author-email: marco@pr-pilot.ai
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: click==8.1.7
-Requires-Dist: pr-pilot==1.4.0
-Requires-Dist: pyyaml==6.0.1
-Requires-Dist: yaspin==3.0.2
-Requires-Dist: rich==13.7.1
-
 <div align="center">
 <img src="https://avatars.githubusercontent.com/ml/17635?s=140&v=" width="100" alt="PR Pilot Logo">
 </div>
 
 <p align="center">
   <a href="https://github.com/apps/pr-pilot-ai/installations/new"><b>Install</b></a> |
   <a href="https://docs.pr-pilot.ai">Documentation</a> | 
@@ -25,15 +9,38 @@
   <a href="https://www.pr-pilot.ai">Website</a>
 </p>
 
 # PR Pilot CLI
 
 PR Pilot gives you a natural language interface for your Github projects.
 Given a prompt, it uses LLMs (Large Language Models) to autonomously fulfill tasks by interacting with your code base
-and Github issues, enabling a wide variety of ground-breaking AI-assisted automation use cases.
+and Github issues.
+
+Using templates, you can create powerful, reusable commands that can be executed by PR Pilot. Here is how it works:
+
+Write a template file:
+
+```markdown
+Take a look at our test results:
+
+---
+{{ sh('pytest') }}
+---
+
+Understand why the tests are failing by reading the relevant code files. 
+Give a short, concise, structured analysis of the test results.
+```
+
+Execute the file:
+
+`pilot -f analyze_test_results.md.jinja2`
+
+For more examples, check out the [prompts](./prompts) directory in this repository.
+
+### 
 
 ## Installation
 
  > Make sure you have PR Pilot [installed in your repository](https://github.com/apps/pr-pilot-ai/installations/new)
 
 To install the CLI, run the following command:
 
@@ -77,14 +84,19 @@
 Usage: pilot [OPTIONS] [PROMPT]...
 
 Options:
   --wait / --no-wait  Wait for the result.
   --repo TEXT         Github repository in the format owner/repo.
   --chatty            Print more information.
   --raw               For piping. No pretty-print, no status indicator.
+  --code              Disable formatting, enable RAW mode, use GPT-4 model.
+  -f, --file PATH     Load prompt from a template file.
+  --direct            Do not use the rendered template as a prompt for PR
+                      Pilot, but render it directly as output.
+  -o, --output PATH   Output file for the result.
   --model TEXT        GPT model to use.
   --debug             Display debug information.
   --help              Show this message and exit.
 ```
 
 
 ## Features
```

#### html2text {}

```diff
@@ -1,43 +1,44 @@
-Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.3.0 Summary: CLI for PR
-Pilot, a text-to-task automation platform for Github. Home-page: https://
-github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
-marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
-pilot==1.4.0 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
-Requires-Dist: rich==13.7.1
                                 [PR Pilot Logo]
                    _II_nn_ss_tt_aa_ll_ll | _D_o_c_u_m_e_n_t_a_t_i_o_n | _B_l_o_g | _W_e_b_s_i_t_e
 # PR Pilot CLI PR Pilot gives you a natural language interface for your Github
 projects. Given a prompt, it uses LLMs (Large Language Models) to autonomously
-fulfill tasks by interacting with your code base and Github issues, enabling a
-wide variety of ground-breaking AI-assisted automation use cases. ##
-Installation > Make sure you have PR Pilot [installed in your repository]
-(https://github.com/apps/pr-pilot-ai/installations/new) To install the CLI, run
-the following command: ```bash pip install --upgrade pr-pilot-cli ``` By
-default, the CLI will prompt you to input your API key if it is not already
-configured. ## Usage After installation, open a terminal and `ls` into a
-repository you have installed PR Pilot in and talk to PR Pilot: ### Examples
-Translate a file: ```bash pilot --raw "translate the README into German" >
-README_German.md ``` Let it write some unit tests: ```bash pilot "Write some
-unit tests for the utils.py file." ``` Find some information in your Github
-issues: ```bash pilot "Do we have any open Github issues regarding the
-AuthenticationView class?" ``` For more information, check out our [User Guide]
-(https://docs.pr-pilot.ai/user_guide.html). ### Options and Parameters You can
-change the default settings with parameters and options: ```bash Usage: pilot
-[OPTIONS] [PROMPT]... Options: --wait / --no-wait Wait for the result. --repo
-TEXT Github repository in the format owner/repo. --chatty Print more
-information. --raw For piping. No pretty-print, no status indicator. --model
-TEXT GPT model to use. --debug Display debug information. --help Show this
-message and exit. ``` ## Features - **Configuration Management**: Automatically
-manages API key configuration by prompting the user to input their API key if
-not already configured. - **Task Creation**: Users can create tasks by
-specifying a repository and a prompt. The CLI handles task creation and
-optionally waits for the result. - **Result Retrieval**: If the `--wait` option
-is used, the CLI waits for the task to complete and displays the result
-directly in the terminal. - **Dashboard Link**: For tasks that are not awaited,
-the CLI provides a link to the task's dashboard for further monitoring. ##
-Configuration The configuration file is located at `~/.pr-pilot.yaml`. ##
-Contributing Contributors are welcome to improve the CLI by submitting pull
-requests or reporting issues. For more details, check the project's GitHub
-repository. ## License The PR Pilot CLI is open-source software licensed under
-the GPL-3 license.
+fulfill tasks by interacting with your code base and Github issues. Using
+templates, you can create powerful, reusable commands that can be executed by
+PR Pilot. Here is how it works: Write a template file: ```markdown Take a look
+at our test results: --- {{ sh('pytest') }} --- Understand why the tests are
+failing by reading the relevant code files. Give a short, concise, structured
+analysis of the test results. ``` Execute the file: `pilot -
+f analyze_test_results.md.jinja2` For more examples, check out the [prompts](./
+prompts) directory in this repository. ### ## Installation > Make sure you have
+PR Pilot [installed in your repository](https://github.com/apps/pr-pilot-ai/
+installations/new) To install the CLI, run the following command: ```bash pip
+install --upgrade pr-pilot-cli ``` By default, the CLI will prompt you to input
+your API key if it is not already configured. ## Usage After installation, open
+a terminal and `ls` into a repository you have installed PR Pilot in and talk
+to PR Pilot: ### Examples Translate a file: ```bash pilot --raw "translate the
+README into German" > README_German.md ``` Let it write some unit tests:
+```bash pilot "Write some unit tests for the utils.py file." ``` Find some
+information in your Github issues: ```bash pilot "Do we have any open Github
+issues regarding the AuthenticationView class?" ``` For more information, check
+out our [User Guide](https://docs.pr-pilot.ai/user_guide.html). ### Options and
+Parameters You can change the default settings with parameters and options:
+```bash Usage: pilot [OPTIONS] [PROMPT]... Options: --wait / --no-wait Wait for
+the result. --repo TEXT Github repository in the format owner/repo. --chatty
+Print more information. --raw For piping. No pretty-print, no status indicator.
+--code Disable formatting, enable RAW mode, use GPT-4 model. -f, --file PATH
+Load prompt from a template file. --direct Do not use the rendered template as
+a prompt for PR Pilot, but render it directly as output. -o, --output PATH
+Output file for the result. --model TEXT GPT model to use. --debug Display
+debug information. --help Show this message and exit. ``` ## Features -
+**Configuration Management**: Automatically manages API key configuration by
+prompting the user to input their API key if not already configured. - **Task
+Creation**: Users can create tasks by specifying a repository and a prompt. The
+CLI handles task creation and optionally waits for the result. - **Result
+Retrieval**: If the `--wait` option is used, the CLI waits for the task to
+complete and displays the result directly in the terminal. - **Dashboard
+Link**: For tasks that are not awaited, the CLI provides a link to the task's
+dashboard for further monitoring. ## Configuration The configuration file is
+located at `~/.pr-pilot.yaml`. ## Contributing Contributors are welcome to
+improve the CLI by submitting pull requests or reporting issues. For more
+details, check the project's GitHub repository. ## License The PR Pilot CLI is
+open-source software licensed under the GPL-3 license.
```

### Comparing `pr_pilot_cli-1.3.0/cli/cli.py` & `pr_pilot_cli-1.3.1/cli/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,92 +4,95 @@
 import yaml
 from pr_pilot.util import create_task, wait_for_result, get_task
 from rich.console import Console
 from rich.markdown import Markdown
 from yaspin import yaspin
 
 from cli.detect_repository import detect_repository
+from cli.task_handler import TaskHandler
+from cli.templating import render_prompt_template
 
 CONFIG_LOCATION = os.path.expanduser('~/.pr-pilot.yaml')
 CONFIG_API_KEY = "api_key"
+CODE_MODEL = "gpt-4"
+POLL_INTERVAL = 2
 
 
 def load_config():
     """Load the configuration from the default location. If it doesn't exist,
     ask user to enter API key and save config."""
     if not os.path.exists(CONFIG_LOCATION):
         api_key_url = "https://app.pr-pilot.ai/dashboard/api-keys/"
-        click.echo(f"Configuration file not found. Please create an API key at {api_key_url}.")
+        console.print(f"Configuration file not found. Please create an API key at {api_key_url}.")
         api_key = click.prompt("PR Pilot API key")
         with open(CONFIG_LOCATION, "w") as f:
             f.write(f"{CONFIG_API_KEY}: {api_key}")
-        click.echo(f"Configuration saved in {CONFIG_LOCATION}")
+        console.print(f"Configuration saved in {CONFIG_LOCATION}")
     with open(CONFIG_LOCATION) as f:
         config = yaml.safe_load(f)
     return config
 
 
 @click.command()
 @click.option('--wait/--no-wait', is_flag=True, default=True, help='Wait for the result.')
 @click.option('--repo', help='Github repository in the format owner/repo.', required=False)
 @click.option('--chatty', is_flag=True, default=False, help='Print more information.')
 @click.option('--raw', is_flag=True, default=False, help='For piping. No pretty-print, no status indicator.')
+@click.option('--code', is_flag=True, default=False, help='Disable formatting, enable RAW mode, use GPT-4 model.')
+@click.option('--file', '-f', type=click.Path(exists=True), help='Load prompt from a template file.')
+@click.option('--direct', is_flag=True, default=False,
+              help='Do not use the rendered template as a prompt for PR Pilot, but render it directly as output.')
+@click.option('--output', '-o', type=click.Path(exists=False), help='Output file for the result.')
 @click.option('--model', help='GPT model to use.', default='gpt-4-turbo')
 @click.option('--debug', is_flag=True, default=False, help='Display debug information.')
 @click.argument('prompt', nargs=-1)
-def main(wait, repo, chatty, raw, model, debug, prompt):
+def main(wait, repo, chatty, raw, code, file, direct, output, model, debug, prompt):
     prompt = ' '.join(prompt)
     config = load_config()
+    console = Console()
+
     if debug:
         chatty = True
     if not os.getenv("PR_PILOT_API_KEY"):
         os.environ["PR_PILOT_API_KEY"] = config[CONFIG_API_KEY]
     if not repo:
         # No repository provided, try to detect it
         repo = detect_repository()
     if not repo:
         # Current directory is not a git repository, see if there is a default repo in the config
         repo = config.get("default_repo")
     if not repo:
-        click.echo(f"No Github repository provided. Use --repo or set 'default_repo' in {CONFIG_LOCATION}.")
+        console.print(f"No Github repository provided. Use --repo or set 'default_repo' in {CONFIG_LOCATION}.")
         return
+    if file:
+        prompt = render_prompt_template(file, repo, model)
     if not prompt:
-        click.echo("Please provide a prompt.")
-        return
+        prompt = click.edit("", extension=".md")
+        if not prompt:
+            console.print("No prompt provided.")
+            return
+    if code:
+        raw = True
+        prompt += "\n\nONLY respond with the code, no other text. Do not wrap it in triple backticks."
+        model = CODE_MODEL
+
+    if direct:
+        # Do not send the prompt, just return it as the result
+        if output:
+            with open(output, "w") as f:
+                f.write(prompt)
+            console.print(Markdown(f"Rendered template `{file}` into `{output}`"))
+            return
 
-    if raw:
-        task = create_task(repo, prompt, log=False, gpt_model=model)
-        result = wait_for_result(task, log=False)
-        print(result)
-        return
+    task = create_task(repo, prompt, log=False, gpt_model=model)
 
-    console = Console()
-    with yaspin(text=f"Creating new task for repository {repo}", color="cyan") as sp:
-        task = create_task(repo, prompt, gpt_model=model)
-        dashboard_url = f"https://app.pr-pilot.ai/dashboard/tasks/{task.id}/"
+    if not wait:
         if chatty:
-            sp.write(f"✅ Task created: {dashboard_url}")
-            if debug:
-                console.print(task)
-        if wait:
-            sp.text = f"I'm working on it :) Track my progress in the dashboard: {dashboard_url}"
-            try:
-                result = wait_for_result(task)
-                if chatty:
-                    sp.ok("✅")
-                else:
-                    sp.hide()
-
-                console.line()
-                if debug:
-                    console.print(get_task(task.id))
-                    console.line()
-                if raw:
-                    console.print(result)
-                else:
-                    console.print(Markdown(result))
-            except Exception as e:
-                sp.fail("💥")
-                click.echo(f"Error: {e}")
+            console.print(f"✅ Task created: https://app.pr-pilot.ai/dashboard/tasks/{task.id}")
+        return
+
+    task_handler = TaskHandler(task, show_spinner=not raw)
+    task_handler.wait_for_result(output, raw)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `pr_pilot_cli-1.3.0/cli/detect_repository.py` & `pr_pilot_cli-1.3.1/cli/detect_repository.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.3.0/pr_pilot_cli.egg-info/PKG-INFO` & `pr_pilot_cli-1.3.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pr-pilot-cli
-Version: 1.3.0
+Version: 1.3.1
 Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
-Requires-Dist: pr-pilot==1.4.0
+Requires-Dist: pr-pilot==1.4.1
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: yaspin==3.0.2
 Requires-Dist: rich==13.7.1
+Requires-Dist: jinja2==3.1.4
 
 <div align="center">
 <img src="https://avatars.githubusercontent.com/ml/17635?s=140&v=" width="100" alt="PR Pilot Logo">
 </div>
 
 <p align="center">
   <a href="https://github.com/apps/pr-pilot-ai/installations/new"><b>Install</b></a> |
@@ -25,15 +26,38 @@
   <a href="https://www.pr-pilot.ai">Website</a>
 </p>
 
 # PR Pilot CLI
 
 PR Pilot gives you a natural language interface for your Github projects.
 Given a prompt, it uses LLMs (Large Language Models) to autonomously fulfill tasks by interacting with your code base
-and Github issues, enabling a wide variety of ground-breaking AI-assisted automation use cases.
+and Github issues.
+
+Using templates, you can create powerful, reusable commands that can be executed by PR Pilot. Here is how it works:
+
+Write a template file:
+
+```markdown
+Take a look at our test results:
+
+---
+{{ sh('pytest') }}
+---
+
+Understand why the tests are failing by reading the relevant code files. 
+Give a short, concise, structured analysis of the test results.
+```
+
+Execute the file:
+
+`pilot -f analyze_test_results.md.jinja2`
+
+For more examples, check out the [prompts](./prompts) directory in this repository.
+
+### 
 
 ## Installation
 
  > Make sure you have PR Pilot [installed in your repository](https://github.com/apps/pr-pilot-ai/installations/new)
 
 To install the CLI, run the following command:
 
@@ -77,14 +101,19 @@
 Usage: pilot [OPTIONS] [PROMPT]...
 
 Options:
   --wait / --no-wait  Wait for the result.
   --repo TEXT         Github repository in the format owner/repo.
   --chatty            Print more information.
   --raw               For piping. No pretty-print, no status indicator.
+  --code              Disable formatting, enable RAW mode, use GPT-4 model.
+  -f, --file PATH     Load prompt from a template file.
+  --direct            Do not use the rendered template as a prompt for PR
+                      Pilot, but render it directly as output.
+  -o, --output PATH   Output file for the result.
   --model TEXT        GPT model to use.
   --debug             Display debug information.
   --help              Show this message and exit.
 ```
 
 
 ## Features
```

#### html2text {}

```diff
@@ -1,43 +1,51 @@
-Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.3.0 Summary: CLI for PR
+Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.3.1 Summary: CLI for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
 marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
-pilot==1.4.0 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
-Requires-Dist: rich==13.7.1
+pilot==1.4.1 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
+Requires-Dist: rich==13.7.1 Requires-Dist: jinja2==3.1.4
                                 [PR Pilot Logo]
                    _II_nn_ss_tt_aa_ll_ll | _D_o_c_u_m_e_n_t_a_t_i_o_n | _B_l_o_g | _W_e_b_s_i_t_e
 # PR Pilot CLI PR Pilot gives you a natural language interface for your Github
 projects. Given a prompt, it uses LLMs (Large Language Models) to autonomously
-fulfill tasks by interacting with your code base and Github issues, enabling a
-wide variety of ground-breaking AI-assisted automation use cases. ##
-Installation > Make sure you have PR Pilot [installed in your repository]
-(https://github.com/apps/pr-pilot-ai/installations/new) To install the CLI, run
-the following command: ```bash pip install --upgrade pr-pilot-cli ``` By
-default, the CLI will prompt you to input your API key if it is not already
-configured. ## Usage After installation, open a terminal and `ls` into a
-repository you have installed PR Pilot in and talk to PR Pilot: ### Examples
-Translate a file: ```bash pilot --raw "translate the README into German" >
-README_German.md ``` Let it write some unit tests: ```bash pilot "Write some
-unit tests for the utils.py file." ``` Find some information in your Github
-issues: ```bash pilot "Do we have any open Github issues regarding the
-AuthenticationView class?" ``` For more information, check out our [User Guide]
-(https://docs.pr-pilot.ai/user_guide.html). ### Options and Parameters You can
-change the default settings with parameters and options: ```bash Usage: pilot
-[OPTIONS] [PROMPT]... Options: --wait / --no-wait Wait for the result. --repo
-TEXT Github repository in the format owner/repo. --chatty Print more
-information. --raw For piping. No pretty-print, no status indicator. --model
-TEXT GPT model to use. --debug Display debug information. --help Show this
-message and exit. ``` ## Features - **Configuration Management**: Automatically
-manages API key configuration by prompting the user to input their API key if
-not already configured. - **Task Creation**: Users can create tasks by
-specifying a repository and a prompt. The CLI handles task creation and
-optionally waits for the result. - **Result Retrieval**: If the `--wait` option
-is used, the CLI waits for the task to complete and displays the result
-directly in the terminal. - **Dashboard Link**: For tasks that are not awaited,
-the CLI provides a link to the task's dashboard for further monitoring. ##
-Configuration The configuration file is located at `~/.pr-pilot.yaml`. ##
-Contributing Contributors are welcome to improve the CLI by submitting pull
-requests or reporting issues. For more details, check the project's GitHub
-repository. ## License The PR Pilot CLI is open-source software licensed under
-the GPL-3 license.
+fulfill tasks by interacting with your code base and Github issues. Using
+templates, you can create powerful, reusable commands that can be executed by
+PR Pilot. Here is how it works: Write a template file: ```markdown Take a look
+at our test results: --- {{ sh('pytest') }} --- Understand why the tests are
+failing by reading the relevant code files. Give a short, concise, structured
+analysis of the test results. ``` Execute the file: `pilot -
+f analyze_test_results.md.jinja2` For more examples, check out the [prompts](./
+prompts) directory in this repository. ### ## Installation > Make sure you have
+PR Pilot [installed in your repository](https://github.com/apps/pr-pilot-ai/
+installations/new) To install the CLI, run the following command: ```bash pip
+install --upgrade pr-pilot-cli ``` By default, the CLI will prompt you to input
+your API key if it is not already configured. ## Usage After installation, open
+a terminal and `ls` into a repository you have installed PR Pilot in and talk
+to PR Pilot: ### Examples Translate a file: ```bash pilot --raw "translate the
+README into German" > README_German.md ``` Let it write some unit tests:
+```bash pilot "Write some unit tests for the utils.py file." ``` Find some
+information in your Github issues: ```bash pilot "Do we have any open Github
+issues regarding the AuthenticationView class?" ``` For more information, check
+out our [User Guide](https://docs.pr-pilot.ai/user_guide.html). ### Options and
+Parameters You can change the default settings with parameters and options:
+```bash Usage: pilot [OPTIONS] [PROMPT]... Options: --wait / --no-wait Wait for
+the result. --repo TEXT Github repository in the format owner/repo. --chatty
+Print more information. --raw For piping. No pretty-print, no status indicator.
+--code Disable formatting, enable RAW mode, use GPT-4 model. -f, --file PATH
+Load prompt from a template file. --direct Do not use the rendered template as
+a prompt for PR Pilot, but render it directly as output. -o, --output PATH
+Output file for the result. --model TEXT GPT model to use. --debug Display
+debug information. --help Show this message and exit. ``` ## Features -
+**Configuration Management**: Automatically manages API key configuration by
+prompting the user to input their API key if not already configured. - **Task
+Creation**: Users can create tasks by specifying a repository and a prompt. The
+CLI handles task creation and optionally waits for the result. - **Result
+Retrieval**: If the `--wait` option is used, the CLI waits for the task to
+complete and displays the result directly in the terminal. - **Dashboard
+Link**: For tasks that are not awaited, the CLI provides a link to the task's
+dashboard for further monitoring. ## Configuration The configuration file is
+located at `~/.pr-pilot.yaml`. ## Contributing Contributors are welcome to
+improve the CLI by submitting pull requests or reporting issues. For more
+details, check the project's GitHub repository. ## License The PR Pilot CLI is
+open-source software licensed under the GPL-3 license.
```

### Comparing `pr_pilot_cli-1.3.0/setup.py` & `pr_pilot_cli-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pr-pilot-cli',
-    version='1.3.0',
+    version='1.3.1',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         line.strip() for line in open('requirements.txt').readlines()
     ],
     python_requires='>=3.6',
     author='Marco Lamina',
```

