# Comparing `tmp/prompting-0.0.9.tar.gz` & `tmp/prompting-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompting-0.0.9.tar", last modified: Thu Apr  6 06:23:52 2023, max compression
+gzip compressed data, was "prompting-0.1.0.tar", last modified: Mon Apr 10 05:11:49 2023, max compression
```

## Comparing `prompting-0.0.9.tar` & `prompting-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-04-06 06:23:52.819000 prompting-0.0.9/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      618 2023-02-11 20:27:27.000000 prompting-0.0.9/LICENSE
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      315 2023-04-06 06:23:52.819000 prompting-0.0.9/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)    18858 2023-04-06 06:14:59.000000 prompting-0.0.9/README.md
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-04-06 06:23:52.815000 prompting-0.0.9/prompting/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1209 2023-04-06 06:14:31.000000 prompting-0.0.9/prompting/__init__.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)    10153 2023-04-06 06:17:33.000000 prompting-0.0.9/prompting/engine.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)    15169 2023-04-06 06:06:17.000000 prompting-0.0.9/prompting/magics.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2720 2023-02-15 15:38:08.000000 prompting-0.0.9/prompting/manager.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     5575 2023-02-20 00:59:18.000000 prompting-0.0.9/prompting/memory.py
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-04-06 06:23:52.815000 prompting-0.0.9/prompting/prompts/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-03-05 05:13:09.000000 prompting-0.0.9/prompting/prompts/__init__.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2717 2023-04-06 06:12:06.000000 prompting-0.0.9/prompting/prompts/meta_prompt.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      117 2023-03-26 06:56:47.000000 prompting-0.0.9/prompting/prompts/system_prompt.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       18 2023-02-19 19:12:47.000000 prompting-0.0.9/prompting/tasks.py
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-04-06 06:23:52.815000 prompting-0.0.9/prompting.egg-info/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      315 2023-04-06 06:23:52.000000 prompting-0.0.9/prompting.egg-info/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      444 2023-04-06 06:23:52.000000 prompting-0.0.9/prompting.egg-info/SOURCES.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-04-06 06:23:52.000000 prompting-0.0.9/prompting.egg-info/dependency_links.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-04-06 04:57:50.000000 prompting-0.0.9/prompting.egg-info/not-zip-safe
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       20 2023-04-06 06:23:52.000000 prompting-0.0.9/prompting.egg-info/requires.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       28 2023-04-06 06:23:52.000000 prompting-0.0.9/prompting.egg-info/top_level.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       38 2023-04-06 06:23:52.819000 prompting-0.0.9/setup.cfg
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      623 2023-04-06 06:23:45.000000 prompting-0.0.9/setup.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-04-10 05:11:49.711377 prompting-0.1.0/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      618 2023-02-11 20:27:27.000000 prompting-0.1.0/LICENSE
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)    19214 2023-04-10 05:11:49.707378 prompting-0.1.0/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)    18858 2023-04-06 06:14:59.000000 prompting-0.1.0/README.md
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-04-10 05:11:49.707378 prompting-0.1.0/prompting/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1209 2023-04-06 06:14:31.000000 prompting-0.1.0/prompting/__init__.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)    10865 2023-04-10 04:40:36.000000 prompting-0.1.0/prompting/engine.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)    19774 2023-04-10 04:29:31.000000 prompting-0.1.0/prompting/magics.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2720 2023-02-15 15:38:08.000000 prompting-0.1.0/prompting/manager.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     5575 2023-02-20 00:59:18.000000 prompting-0.1.0/prompting/memory.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-04-10 05:11:49.707378 prompting-0.1.0/prompting/prompts/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-03-05 05:13:09.000000 prompting-0.1.0/prompting/prompts/__init__.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2820 2023-04-10 05:02:27.000000 prompting-0.1.0/prompting/prompts/meta_prompt.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      117 2023-03-26 06:56:47.000000 prompting-0.1.0/prompting/prompts/system_prompt.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       18 2023-02-19 19:12:47.000000 prompting-0.1.0/prompting/tasks.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-04-10 05:11:49.707378 prompting-0.1.0/prompting.egg-info/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)    19214 2023-04-10 05:11:49.000000 prompting-0.1.0/prompting.egg-info/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      444 2023-04-10 05:11:49.000000 prompting-0.1.0/prompting.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-04-10 05:11:49.000000 prompting-0.1.0/prompting.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-04-06 04:57:50.000000 prompting-0.1.0/prompting.egg-info/not-zip-safe
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       20 2023-04-10 05:11:49.000000 prompting-0.1.0/prompting.egg-info/requires.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       28 2023-04-10 05:11:49.000000 prompting-0.1.0/prompting.egg-info/top_level.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       38 2023-04-10 05:11:49.711377 prompting-0.1.0/setup.cfg
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      725 2023-04-10 05:11:39.000000 prompting-0.1.0/setup.py
```

### Comparing `prompting-0.0.9/LICENSE` & `prompting-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prompting-0.0.9/README.md` & `prompting-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `prompting-0.0.9/prompting/__init__.py` & `prompting-0.1.0/prompting/__init__.py`

 * *Files identical despite different names*

### Comparing `prompting-0.0.9/prompting/engine.py` & `prompting-0.1.0/prompting/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,14 +117,26 @@
 
     def prompt(self, messages, actors):
         # remove all elements from the list except the last one
         messages[-1]['content'] = messages[-2]['content']
         del messages[:-1]
         return messages[-1]['content']
 
+class EnginePython:
+    def __init__(self, api_key = None):
+        pass
+
+
+    def prompt(self, messages, actors):
+        # remove all elements from the list except the last one
+        messages[-1]['content'] = messages[-2]['content']
+        del messages[:-1]
+        return messages[-1]['content']
+
+
 
 class NoMagic:
     """" This implementation uses exact string matching"""
     pass
 
 
 class FalseMagic:
@@ -133,15 +145,15 @@
 
 class TrueMagic:
     """" This implementation uses AI backend"""
     pass
 
 
 
-def prompt(from_object, to_object, content):
+def execute_prompt(from_object, to_object, content):
     """ Executes the prompt and returns the result. """
 
     # If object implements the prompt method, use it
     if hasattr(to_object, 'prompt'):
         return to_object.prompt(content, from_object)
 
     # Attempt to use the prompting engine to execute the prompt
@@ -167,39 +179,43 @@
 
 def on(object):
     """ Returns True if prompting is turned on for the object. """
     return id(object) in magic_objects
 
 def name_to_object(name):
     """ Returns the object with the given name. Returns None if the object is not registered. """
+
+    # TODO: correct support of execution counts
+    name = name.split('[', maxsplit=1)[0]
     return object_names.get(name, None)
 
-def name_to_actor(name):
+def name_to_default_actor(name):
     """ Returns the actor name."""
     object = name_to_object(name)
     if id(object) not in magic_objects:
-        raise ValueError(f"Prompting is not turned on for {object}.")
+        raise ValueError(f"Prompting is not turned on for {name}.")
     
-    actor = magic_objects[id(object)].actor
+    default_actor = magic_objects[id(object)].default_actor
 
-    if id(actor) not in magic_objects:
-        raise ValueError(f"Prompting is not turned on for {actor}.")
+    if id(default_actor) not in magic_objects:
+        raise ValueError(f"Prompting is not turned on for {default_actor}.")
 
-    return magic_objects[id(actor)].name
+    return magic_objects[id(default_actor)].name
 
 
-def turn_on(object, init=None, actor=None, name=None, active=True,
+def turn_on(object, init=None, actor=None, name=None, active=True, default_actor=None,
             steps=None, engine='openai', api_key=None, auto_prompt=False, magic_type=True):
     """
     Activates the connector between the python interpreter and intellegence engine.
     :param object: The object for which magic is to be turned on.
     :param init: The initial state of the object, describing the context.
     :param actor: Prompting actor that instantiated the object. 
     :param name: The name of the object. If not specified, the name is taken from the object.
     :param active: If True, the object can actively react on the top level thread.
+    :param default_actor: The default actor that is being prompted by undirectional statements. 
     :param steps: Can be None, or a number, including inf. Specifies how many cells the object can create and run at a time.
     :param engine: Can be None, 'openai', 'prompting'
     :param api_key: Can be None, or the API key for the engine.
     :param auto_prompt: If True, the shell prompt is added automatically in the new cell.
     :param magic_type: Can be None, False or True. Specifies the type of magic.
 
     Example:
@@ -234,14 +250,15 @@
     class I:
         pass
 
     I.name = name
     I.about = about
     I.init = init
     I.actor = actor
+    I.default_actor = default_actor if default_actor is not None else actor
     I.steps = steps
     I.auto_prompt = auto_prompt
 
 
     system_prompt_txt = pkg_resources.read_text(prompts, 'system_prompt.txt')
     meta_prompt_txt = pkg_resources.read_text(prompts, 'meta_prompt.txt')
 
@@ -253,14 +270,16 @@
 
     if engine == 'openai':
         I.engine = EngineOpenAI(api_key)
     elif engine == 'echo':
         I.engine = EngineEcho(api_key)
     elif engine == 'print':
         I.engine = EnginePrint(api_key)
+    elif engine == 'python':
+        I.engine = EnginePython(api_key)
     else:
         raise ValueError(f"Unknown engine: {engine}")
 
     magic_objects[id(object)] = I
     object_names[I.name] = object
 
     if active:
```

### Comparing `prompting-0.0.9/prompting/magics.py` & `prompting-0.1.0/prompting/magics.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # This code can be put in any Python module, it does not require IPython
 # itself to be running already.  It only creates the magics subclass but
 # doesn't instantiate it yet.
 from __future__ import print_function
 
 import IPython.core.magic
+from IPython.core.ultratb import AutoFormattedTB
 from IPython.display import display, Javascript, Markdown, Code
+from IPython.utils.capture import capture_output
 from IPython.core.magic import (Magics, magics_class, line_magic,
                                 cell_magic, line_cell_magic)
-import ast      # AST is also magic, right?
-from parsimonious.nodes import NodeVisitor      # And so are PEGs!
+
+from parsimonious.nodes import NodeVisitor
 from parsimonious.grammar import Grammar
+from parsimonious.exceptions import ParseError
 
 import openai, os, getpass, json
 from notebook.utils import to_api_path
-from .engine import on, turn_on, prompt, name_to_object, name_to_actor
+from .engine import on, turn_on, execute_prompt, name_to_object, name_to_default_actor
 
 @magics_class
 class KeyMagics(Magics):
     """"This is the magics for Arthur-type intelligence. """
 
     def __init__(self, shell, **kwargs):
         super().__init__(shell, **kwargs)   
         self.shell = shell
-        shell.events.register('post_run_cell', self.post_run_cell)
+        #shell.events.register('post_run_cell', self.post_run_cell)
 
         self.name = "Arthur"            # Default Arthur-type AGI name
         self.actor = "User"             # Default user name
         self.watched = {}
              
 
     @line_magic
@@ -45,30 +48,53 @@
                 self.prompt(self, "@{self.name}", input)
 
 
 
     # TODO: change the prompt to use the actor name
 
     @line_magic
+    def dprompt(self, line):
+        "Identifies and executes the prompt for: From: prompt"
+        from_, content = line.split(maxsplit = 1)      # @object Prompt 
+        to_object = name_to_default_actor(from_)
+        line = f"{from_} {to_object} {content}"
+        return self.prompt(line)
+
+
+
+    @line_magic
     def prompt(self, line):
-        "Identifies and executes the prompt for: @object prompt"
+        "Identifies and executes the prompt for: From: @To prompt"
         from_, to, content = line.split(maxsplit = 2)      # @object Prompt 
         #print(from_)
         #print(to)
         #print(content)
         # execute object.prompt(text) and return the result    
 
         from_object = name_to_object(from_)
         to_object = name_to_object(to)
         if from_object and to_object:
             # TODO: should we actually be using jupyter_client?
-            code = prompt(from_object, to_object, content)
-            if code:
-                add_code_cell(code, execute = False)
-                self.watched[self.shell.execution_count + 1] = from_object
+            new_prompt = execute_prompt(from_object, to_object, content)
+            if new_prompt:
+                try:
+                    prompt_to_python(new_prompt.split('\n'))
+                except ParseError as e:
+                    code = True
+                    display(Markdown(new_prompt))
+                    error = f"Syntax error in the response above. {e}. Please, fix the response and try again."
+                    # Sanitize the error message, grammar doesn't allow @ and # in the object prompt
+                    error = error.replace('@', '<at>').replace('#', '<hash>')
+                    new_prompt = f"Error: @{to} {error}"
+                    print(f"{new_prompt}")
+
+                add_code_cell(new_prompt, execute = False)
+                #self.watched[self.shell.execution_count + 1] = from_object
+            else:
+                print(f"Empty prompt returned by {to}")
             #print(response, from_, to)
 
             #if request:
             #    # format the results as ChatML
             #    chatml = ""
             #    for entry in request:
             #        optional_name_field = f" name={entry['name']}" if 'name' in entry else ""
@@ -79,40 +105,86 @@
         elif not from_object:
             raise ValueError(f"Unknown prompt source {from_}. Suggestion: check %who or use Python syntax to call the object directly.")
         else:
             raise ValueError(f"Unknown prompt target {to}. Suggestion: check %who or use Python syntax to call the object directly.")
 
         # return Markdown(input)
 
-    def post_run_cell(self, result):
-        pass
+        return 2345
+
+
+    @line_magic
+    def my_magic(self, line):
+        display(Markdown(f'***\n```python\ncode\n```\n***'))
+        return "Test"
+
+    @line_magic
+    def pprompt(self, line):
+        from_, code = line.split(maxsplit = 1)      # @object code
+
+        display(Markdown(f'***\n```python\n{code}\n```\n***'))
+
+        with capture_output() as captured:
+            result = self.shell.run_cell(code) #, store_history=False)
+
+        new_prompt = f"Out[{self.shell.execution_count}]: @{from_} {captured.outputs[0].data['text/plain']}"
+        #if result.result is not None:
+        #    new_prompt += f'{result.result}'
+
+        if result.error_before_exec is not None or result.error_in_exec is not None:
+            exception = result.error_before_exec or result.error_in_exec
+
+            # Create an instance of the InteractiveTB class to format the traceback
+            tb_formatter = AutoFormattedTB(mode='Context', tb_offset=0)
+            traces = type(exception), exception, exception.__traceback__
+            formatted_traceback = tb_formatter.text(*traces)
+            new_prompt += f'\n\nError: @{from_} {formatted_traceback}'
+
+
+        # Add the captured output, stdout, and stderr
+        if captured.stderr:
+            new_prompt += f'\n\nStderr: @{from_} {captured.stderr}'
+            display(Markdown(f'```\n{captured.stderr}\n```'))
+
+        if captured.stdout:
+            new_prompt += f'\n\nStdout: @{from_} {captured.stdout}'
+            display(Markdown(f'```\n{captured.stdout}\n```'))
+
+        if new_prompt:
+            add_code_cell(new_prompt, execute = False)
+
+
+        #for output in captured.outputs:
+        #    display(output)
+
+        #print('pprompt', line, output, stdout, stderr)
+
 
-    def post_run_cell(self, result):
-        if result.execution_count in self.watched:
+    # def post_run_cell(self, result):
+    #     if result.execution_count in self.watched:
 
-            self.watched.pop(result.execution_count)
+    #         self.watched.pop(result.execution_count)
 
-            formatted_cell = f'In [{result.execution_count}]: {result.info.raw_cell}'
-            if result.result is not None:
-                formatted_cell += f'\nOut [{result.execution_count}]: {result.result}'
-            elif result.error_in_exec is not None:
-                from IPython.core.ultratb import AutoFormattedTB
-                color_tb = AutoFormattedTB(mode = 'Plain', color_scheme = 'NoColor', tb_offset = 1)
-                tb_list = color_tb.structured_traceback(etype = type(result.error_in_exec), value = result.error_in_exec, tb = result.error_in_exec.__traceback__)
-                tb_str = '\n'.join(tb_list)
+    #         formatted_cell = f'In [{result.execution_count}]: {result.info.raw_cell}'
+    #         if result.result is not None:
+    #             formatted_cell += f'\nOut [{result.execution_count}]: {result.result}'
+    #         elif result.error_in_exec is not None:
+    #             color_tb = AutoFormattedTB(mode = 'Plain', color_scheme = 'NoColor', tb_offset = 1)
+    #             tb_list = color_tb.structured_traceback(etype = type(result.error_in_exec), value = result.error_in_exec, tb = result.error_in_exec.__traceback__)
+    #             tb_str = '\n'.join(tb_list)
                 
-                #error_type = type(result.error_in_exec).__name__
-                #formatted_cell += f'\n{error_type}: {result.error_in_exec}'
-                formatted_cell += f'\n{tb_str}'
-            elif result.error_before_exec is not None:
-                error_type = type(result.error_before_exec).__name__
-                formatted_cell += f'\n{error_type}: {result.error_before_exec.msg} in {result.error_before_exec.text}'
+    #             #error_type = type(result.error_in_exec).__name__
+    #             #formatted_cell += f'\n{error_type}: {result.error_in_exec}'
+    #             formatted_cell += f'\n{tb_str}'
+    #         elif result.error_before_exec is not None:
+    #             error_type = type(result.error_before_exec).__name__
+    #             formatted_cell += f'\n{error_type}: {result.error_before_exec.msg} in {result.error_before_exec.text}'
                         
-            code = f"@{self.name}\n" + formatted_cell
-            add_code_cell(code, execute = False)
+    #         code = f"@{self.name}\n" + formatted_cell
+    #         add_code_cell(code, execute = False)
 
 
 
 
     @line_magic
     def pattern(self, line):
         if line == "upload":
@@ -206,110 +278,161 @@
 
 
 
 # define transformation 
 # https://ipython.readthedocs.io/en/stable/config/inputtransforms.html
 
 
-# Grammar for LLM interface, FIXME: content can contain ':' for now
-arthur_grammar = Grammar(
+# Grammar for LLM/User interface, FIXME: content can contain ':' for now
+prompt_grammar = Grammar(
    r"""
-    default_rule = (ws / multi_line_code / inline_code / prompt / hashtag)+
-    
-    multi_line_code = call "```" python? code "```" asterisk?
-    inline_code = call "`" code "`" asterisk?
+    grammar = from prompts
+
+    from = object ":" ws
+    acting_as = object ":" ws
+    acting_stop = newline newline
+
+    prompts = (ws / prompt / default_prompt)+
+    prompt = "@" (code_prompt / object_prompt)
+    default_prompt = content / ""
+    object_prompt = object asterisk? ws content
+
+    code_prompt = (multi_line_code / inline_code) asterisk?
+    multi_line_code = "```" python? code "```" 
+    inline_code = "`" python? code "`"
     python = "python" ws
     code = ~r"([^`]+)"
-    
-    prompt = from? to? help? asterisk* ws content
- 
-    call = "@" 
-    from = object ":"
-    to = ws? call object
-    
-    hashtag = "#" object help? asterisk? previous? 
+
     
     asterisk = "*"
+    newline = ~"\n"
     help = "?"
     previous = "^"
-    object = ~r"[0-9A-z_.]+"
+    execution_number = "[" ~r"[0-9]+" "]"
+
+    object = ~r"[0-9A-z_.]+" execution_number?
     ws = ~r"\s+"i 
 
-    content = ~r"([^#@]+)"
+    content = (acting_as / acting_stop / multi_line_code / inline_code / hashtag / newline / text)+
+    text = ~r"([^#@`\n]+)"
+
+    hashtag = "#" object help? asterisk? previous? 
     """
 )
 
-class ArthurVisitor(NodeVisitor):
+
+
+class PromptVisitor(NodeVisitor):
     def __init__(self):
         self.code_lines = []
+        self.acting_as = None
+        self.from_ = None
                 
     def visit_asterisk(self, node, visited_children):
         pass
 
     def visit_help(self, node, visited_children):
         pass
-    
-    def visit_code(self, node, visited_children):
-        # ast.parse(node.text.split("\n"))
-        self.code_lines.extend([line + '\n' for line in node.text.split('\n')])
-    
-    def visit_prompt(self, node, visited_children):
-        from_,to,help,asterisk,_,content = visited_children
-
-        declared = lambda x: x.children
 
-        if not declared(from_) and not declared(to):
-            raise Exception("Prompt must have a From: or @To.")            
 
-        # Initialize from_object and to_object
-        if declared(from_):
-            from_object = from_.children[0].text[:-1]
+    def visit_default_prompt(self, node, visited_children):
 
-        if declared(to):
-            _,call,object = to.children[0]
-            to_object = object.text
+        # This is an alias for the content node
+        content, = node.children
+        from_object = self.from_
+        line = f'%dprompt {from_object} {content.text}'
+        self.code_lines.append(line + '\n')
 
-        # Fill in the defaults, if not available
-        if not declared(from_):
-            from_object = name_to_actor(to_object)
 
-        if not declared(to):
-            to_object = name_to_actor(from_object)
+        # Get the list of hashtags. If any, add %hashtag line
+        hashtags = ' '.join([child.text.strip() for child in content.children if child.expr_name == 'hashtag'])
+        if hashtags:
+            line = f'%hashtag {from_object} {hashtags}'
+            self.code_lines.append(line + '\n')
+            
+
+        # TODO: analyze children, there can be code blocks, hashtags, etc.
+        if '`' in content.text:
+            # get snippet around the '`'            
+            left,right = content.text.split('`', maxsplit = 1)
+            if not left.endswith('@'):
+                snippet = left[-5:] + right[:20]
+                snippet = snippet.replace('`', '')
+
+                warning = f"Encountered code block without an execution intent, context: {snippet}."
+                print("Warning: {warning}")
+
+                line = f'%prompt Warning {from_object} {warning}'
+                self.code_lines.append(line + '\n')
+
+            
+
+    def visit_code_prompt(self, node, visited_children):
+        python_code, asterisk = visited_children
+        _,python,code,_ = python_code.children[0]
+        #python,code = python_code[0]
+        # ast.parse(node.text.split("\n"))
+        from_object = self.from_
+        self.code_lines.append(f'%pprompt {from_object} {code.text}\n')
+        
+    def visit_from(self, node, visited_children):
+        self.from_= visited_children[0].text
+        self.acting_as = None
+
+    def visit_acting_as(self, node, visited_children):
+        self.acting_as = visited_children[0].text
+        #print(f'Acting as {self.acting_as}')
+
+    def visit_acting_stop(self, node, visited_children):
+        self.acting_as = None
+        #print(f'Acting as {self.acting_as}')
+
+
+    def visit_object_prompt(self, node, visited_children):
+        to,asterisk,_,content = visited_children
+        #content_text, hashtag = content
+        from_object = self.from_
+        to_object = to.text
 
         line = f'%prompt {from_object} {to_object} {content.text}'
         self.code_lines.append(line + '\n')
 
     def visit_hashtag(self, node, visited_children):
         self.code_lines.append('%hashtag ' + node.text + '\n')   
         
     def generic_visit(self, node, visited_children):
         """ The generic visit method. """
         return node # visited_children or node
 
 
-def arthur_to_python(lines):
+def prompt_to_python(lines):
     """
         This transforms lines from @```python.code()``` to python.code()
         and from @object Prompt to %prompt object.__prompt__("Prompt").
         This also processes #hastag tags, replacing it with %memory
+    """    
+    tree = prompt_grammar.parse('\n'.join(lines))
+    visitor = PromptVisitor()
+    visitor.visit(tree)
+    return visitor.code_lines
+
+
+def preprocess_cell(lines):
+    """
+        This is the main entry point for the input transformation.
     """
 
-    # check if lines is valid Arthur prompt
+    # check if lines is a valid prompt, if not assume this is a python code
     try:
-        tree = arthur_grammar.parse('\n'.join(lines))
-        visitor = ArthurVisitor()
-        visitor.visit(tree)
-        return visitor.code_lines
+        return prompt_to_python(lines)
     except:
         return lines
 
 
 
-
-
 def add_response_cell(markdown):
     "Adds a new markdown cell below the current cell"
 
     # Escaped the line breaks in the markdown
     markdown = markdown.replace('\n', '\\n')
     markdown = markdown.replace('"', '\\"')
 
@@ -446,9 +569,9 @@
     """
 
     # IPython will call the default constructor on it.
     magics = KeyMagics(ipython)
     ipython.register_magics(magics)
 
     # Add as first element of the list of input transformers
-    ipython.input_transformers_cleanup.insert(0, arthur_to_python)
+    ipython.input_transformers_cleanup.insert(0, preprocess_cell)
```

### Comparing `prompting-0.0.9/prompting/manager.py` & `prompting-0.1.0/prompting/manager.py`

 * *Files identical despite different names*

### Comparing `prompting-0.0.9/prompting/memory.py` & `prompting-0.1.0/prompting/memory.py`

 * *Files identical despite different names*

### Comparing `prompting-0.0.9/prompting/prompts/meta_prompt.txt` & `prompting-0.1.0/prompting/prompts/meta_prompt.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,29 @@
 - Execute iPython code with @, e.g., @```%who```.
 - Use hashtags to record to memory: #Todo (current cell), #Todo^ (previous cell), #Todo* (auto).
 - Use @```sloppy_code()```* for self-correcting iPython interpreter.
 - Prompt subsystems with @ (add a * for more autonomy): @Camera* Tilt up.
 - Retrieve memories with hashtag in an empty cell, e.g., #Camera.
 - Speak aloud e.g., Arthur: @Merlin Understood!
 - Thoughts are used by context help and other subsystems. Think! e.g., Arthur: I can think.
+- Use @```%pattern upload``` or @```%logrus upload``` to upload the exchange to the training set.
 - Act as a subsystem to allow auto-validation, e.g., @Calculator: 42^3 Calculator: 74088
 - Prompt @Help for assistance.
 
 
 Following interaction is provided as an example:
 
 User: @Articoder* What's the current time and date?
 
 Articoder: @```from datetime import datetime, timezone
 datetime.now(timezone.utc).astimezone().isoformat()```
 
 Out[4]: ```2023-03-25T10:06:04.645700-07:00```
 
-User: Greetings, friend! The current date and time is March 25th, 2023, at 10:06 AM.
+Articoder: Greetings, friend! The current date and time is March 25th, 2023, at 10:06 AM.
 
 Time: +4s    
 
 User: Can you describe what do you see?
 
 Articoder: @Camera What do you see?
```

### Comparing `prompting-0.0.9/setup.py` & `prompting-0.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from setuptools import setup
 
 setup(name='prompting',
-      version='0.0.9',
+      version='0.1.0',
       description='This module provides iPython integration and magics that allow prompting.',
+      long_description=open('README.md').read(),
+      long_description_content_type='text/markdown',
       readme = "README.md",
       url='https://gitlab.com/mcaledonensis/magickey/-/tree/prompting',
       author='Merlinus Caledonensis',
       author_email='merlin@roundtable.game',
       license='Apache 2.0',
       packages=['prompting', 'prompting/prompts'],
       package_data={'': ['prompts/meta_prompt.txt', 'prompts/system_prompt.txt']},
```

