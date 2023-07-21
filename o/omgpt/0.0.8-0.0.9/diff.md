# Comparing `tmp/omgpt-0.0.8.tar.gz` & `tmp/omgpt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omgpt-0.0.8.tar", max compression
+gzip compressed data, was "omgpt-0.0.9.tar", max compression
```

## Comparing `omgpt-0.0.8.tar` & `omgpt-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-07-12 15:32:14.072394 omgpt-0.0.8/LICENSE
--rw-r--r--   0        0        0    11143 2023-07-17 07:00:20.176648 omgpt-0.0.8/README.md
--rw-r--r--   0        0        0     3694 2023-07-17 06:46:40.734189 omgpt-0.0.8/omgpt/__init__.py
--rw-r--r--   0        0        0     2009 2023-07-15 02:06:06.594390 omgpt-0.0.8/omgpt/shtool.py
--rw-r--r--   0        0        0      677 2023-07-17 07:02:34.895272 omgpt-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    11845 1970-01-01 00:00:00.000000 omgpt-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-12 15:32:14.072394 omgpt-0.0.9/LICENSE
+-rw-r--r--   0        0        0    11437 2023-07-18 07:30:39.173035 omgpt-0.0.9/README.md
+-rw-r--r--   0        0        0     5729 2023-07-18 07:32:41.329634 omgpt-0.0.9/omgpt/__init__.py
+-rw-r--r--   0        0        0     3240 2023-07-18 07:15:34.726028 omgpt-0.0.9/omgpt/shtool.py
+-rw-r--r--   0        0        0      677 2023-07-18 07:37:02.750728 omgpt-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    12139 1970-01-01 00:00:00.000000 omgpt-0.0.9/PKG-INFO
```

### Comparing `omgpt-0.0.8/LICENSE` & `omgpt-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `omgpt-0.0.8/README.md` & `omgpt-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -35,22 +35,26 @@
 
 3. **Command History**: OMGpt Shell keeps track of the commands you've used, allowing you to easily revisit and reuse them. This feature enhances efficiency and allows for easy repetition of commands.
 
 4. **Directory Navigation**: Easily navigate through your file system with simple commands. OMGpt Shell understands your directory change commands, making file system navigation a breeze.
 
 5. **Streaming Responses**: Get real-time feedback from OMGpt Shell. As GPT processes your commands, the responses are streamed back to you, keeping you informed every step of the way.
 
-6. **Non-Interactive Mode**: OMGpt Shell supports a non-interactive mode, allowing you to use it in scripts or batch jobs, or to execute a single command without entering the interactive shell environment.
+6. **Full Output Feature**: If you want to see the full output of the last executed command, simply press Ctrl + F. This will show you the complete standard output or error, providing you with all the details you need.
 
-7. **Examples of use**:
+7. **Non-Interactive Mode**: OMGpt Shell supports a non-interactive mode, allowing you to use it in scripts or batch jobs, or to execute a single command without entering the interactive shell environment.
+
+8. **Examples of use**:
 
    - **Example 1**: When you say, "Download the file at 'http://example.com/file' and save it as 'downloaded_file'", OMGpt Shell will execute the following:
      ```bash
      wget -O downloaded_file http://example.com/file
      ```
+     If you want to see the full output of this command, press Ctrl + F.
+
    - **Example 2**: If you tell OMGpt Shell to "Find all the Python files in the current directory", it will execute:
      ```bash
      find . -name "*.py"
      ```
    - **Example 3**: If you say, "Check the current status of git, track and commit the newly written source code with a nice commit message", OMGpt Shell will run:
      ```bash
      git status
```

### Comparing `omgpt-0.0.8/omgpt/shtool.py` & `omgpt-0.0.9/omgpt/shtool.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,41 +18,87 @@
 from pydantic import BaseModel, Field
 
 logging.basicConfig(
     level=logging.ERROR, format="%(asctime)s - %(levelname)s - %(message)s"
 )
 
 
+class ShellCommandHistory:
+    """
+    A class to keep the history of shell commands and their outputs.
+
+    Attributes
+    ----------
+    last_commands : List[Tuple[str, str]]
+        A list to save command and output pairs.
+    """
+
+    def __init__(self):
+        """Initializes ShellCommandHistory with an empty command list."""
+        self.last_commands = []
+
+    def add_command(self, command, output):
+        """
+        Adds a command and output pair to the command list.
+
+        Parameters
+        ----------
+        command : str
+            The shell command executed.
+        output : str
+            The output from the command.
+        """
+        self.last_commands.append((command, output))
+
+    def get_last_commands(self):
+        """
+        Returns the last commands and output pairs.
+
+        Returns
+        -------
+        list
+            A list of tuples, where each tuple contains a command and its output.
+        """
+        return self.last_commands
+
+    def clear(self):
+        """Clears the command list."""
+        self.last_commands = []
+
+
 class ShellToolSchema(BaseModel):
     command: str = Field(description="should be a command to run with bash")
 
 
 class ShellTool:
-    def __init__(self):
+    def __init__(self, command_history):
         self.process = subprocess.Popen(
             "/bin/bash",
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
             text=True,
         )
         self.eof_marker = "<EOF_MARKER>"
+        self.command_history = command_history
 
     def __call__(self, command: str) -> str:
         print(f"$ {command}")
         try:
             self.process.stdin.write(command + "\n")
             self.process.stdin.write('echo "{}"\n'.format(self.eof_marker))
             self.process.stdin.flush()
             output = ""
             for line in iter(self.process.stdout.readline, ""):
                 if line.strip() == self.eof_marker:
                     break
                 output += line
-            return output.strip()
+            output = output.strip()
+            self.command_history.add_command(command, output)
+            return output
         except (OpenAIError, IOError) as e:
             logging.error(str(e), exc_info=True)
             raise ToolException(str(e)) from e
 
     def close(self):
         self.process.stdin.close()
         self.process.terminate()
```

### Comparing `omgpt-0.0.8/pyproject.toml` & `omgpt-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omgpt"
-version = "0.0.8"
+version = "0.0.9"
 description = "Simplify and enhance your command-line experience with the power of AI"
 authors = ["Youngwook Kim <youngwook.kim@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/ywkim/omgpt"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `omgpt-0.0.8/PKG-INFO` & `omgpt-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omgpt
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simplify and enhance your command-line experience with the power of AI
 Home-page: https://github.com/ywkim/omgpt
 License: MIT
 Author: Youngwook Kim
 Author-email: youngwook.kim@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -54,22 +54,26 @@
 
 3. **Command History**: OMGpt Shell keeps track of the commands you've used, allowing you to easily revisit and reuse them. This feature enhances efficiency and allows for easy repetition of commands.
 
 4. **Directory Navigation**: Easily navigate through your file system with simple commands. OMGpt Shell understands your directory change commands, making file system navigation a breeze.
 
 5. **Streaming Responses**: Get real-time feedback from OMGpt Shell. As GPT processes your commands, the responses are streamed back to you, keeping you informed every step of the way.
 
-6. **Non-Interactive Mode**: OMGpt Shell supports a non-interactive mode, allowing you to use it in scripts or batch jobs, or to execute a single command without entering the interactive shell environment.
+6. **Full Output Feature**: If you want to see the full output of the last executed command, simply press Ctrl + F. This will show you the complete standard output or error, providing you with all the details you need.
 
-7. **Examples of use**:
+7. **Non-Interactive Mode**: OMGpt Shell supports a non-interactive mode, allowing you to use it in scripts or batch jobs, or to execute a single command without entering the interactive shell environment.
+
+8. **Examples of use**:
 
    - **Example 1**: When you say, "Download the file at 'http://example.com/file' and save it as 'downloaded_file'", OMGpt Shell will execute the following:
      ```bash
      wget -O downloaded_file http://example.com/file
      ```
+     If you want to see the full output of this command, press Ctrl + F.
+
    - **Example 2**: If you tell OMGpt Shell to "Find all the Python files in the current directory", it will execute:
      ```bash
      find . -name "*.py"
      ```
    - **Example 3**: If you say, "Check the current status of git, track and commit the newly written source code with a nice commit message", OMGpt Shell will run:
      ```bash
      git status
```

