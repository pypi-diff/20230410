# Comparing `tmp/qq_chat_history-1.1.3.tar.gz` & `tmp/qq_chat_history-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qq_chat_history-1.1.3.tar", max compression
+gzip compressed data, was "qq_chat_history-1.1.4.tar", max compression
```

## Comparing `qq_chat_history-1.1.3.tar` & `qq_chat_history-1.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1084 2023-01-22 09:17:50.147457 qq_chat_history-1.1.3/LICENSE
--rw-r--r--   0        0        0      744 2023-04-09 14:58:02.590517 qq_chat_history-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      168 2023-03-18 07:36:17.870473 qq_chat_history-1.1.3/qq_chat_history/__init__.py
--rw-r--r--   0        0        0     5484 2023-04-09 14:55:58.142430 qq_chat_history-1.1.3/qq_chat_history/body.py
--rw-r--r--   0        0        0     1011 2023-04-09 14:56:07.727793 qq_chat_history-1.1.3/qq_chat_history/cli.py
--rw-r--r--   0        0        0      450 2023-04-09 14:56:46.627991 qq_chat_history-1.1.3/qq_chat_history/message.py
--rw-r--r--   0        0        0        0 2023-01-22 12:44:48.720506 qq_chat_history-1.1.3/qq_chat_history/py.typed
--rw-r--r--   0        0        0     2669 2023-03-19 03:17:24.426596 qq_chat_history-1.1.3/README.md
--rw-r--r--   0        0        0     3497 1970-01-01 00:00:00.000000 qq_chat_history-1.1.3/setup.py
--rw-r--r--   0        0        0     3295 1970-01-01 00:00:00.000000 qq_chat_history-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-01-22 09:17:50.147457 qq_chat_history-1.1.4/LICENSE
+-rw-r--r--   0        0        0      744 2023-04-10 05:05:06.287372 qq_chat_history-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-03-18 07:36:17.870473 qq_chat_history-1.1.4/qq_chat_history/__init__.py
+-rw-r--r--   0        0        0     5531 2023-04-10 05:00:53.363865 qq_chat_history-1.1.4/qq_chat_history/body.py
+-rw-r--r--   0        0        0     1012 2023-04-10 04:57:06.745714 qq_chat_history-1.1.4/qq_chat_history/cli.py
+-rw-r--r--   0        0        0      429 2023-04-10 04:57:01.654118 qq_chat_history-1.1.4/qq_chat_history/message.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:44:48.720506 qq_chat_history-1.1.4/qq_chat_history/py.typed
+-rw-r--r--   0        0        0     2405 2023-04-10 05:04:51.495080 qq_chat_history-1.1.4/README.md
+-rw-r--r--   0        0        0     3233 1970-01-01 00:00:00.000000 qq_chat_history-1.1.4/setup.py
+-rw-r--r--   0        0        0     3048 1970-01-01 00:00:00.000000 qq_chat_history-1.1.4/PKG-INFO
```

### Comparing `qq_chat_history-1.1.3/LICENSE` & `qq_chat_history-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qq_chat_history-1.1.3/pyproject.toml` & `qq_chat_history-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qq-chat-history"
-version = "1.1.3"
+version = "1.1.4"
 description = "A tool to extract QQ chat history."
 authors = ["kifuan <kifuan@foxmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "qq_chat_history"}]
 repository = "https://github.com/kifuan/qq-chat-history"
```

### Comparing `qq_chat_history-1.1.3/qq_chat_history/body.py` & `qq_chat_history-1.1.4/qq_chat_history/body.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class Body:
     """Chat history file body containing messages."""
 
     def __init__(self, messages: list[Message]) -> None:
         """Initializes the body with messages.
 
-        Not recommended to construct a body directly.
+        Constructing a body directly by this method is not recommended.
         Instead, using class methods `from_xxx` is recommended.
         """
         self._messages = messages
 
     @staticmethod
     def _make_builder_from_head(line: str) -> Optional[MessageBuilder]:
         """Parses a message head. Returns None if the given line is invalid."""
@@ -70,15 +70,15 @@
                 content_lines.append(line)
 
         messages.extend(cls._gen_from_builder(builder, content_lines))
         return cls(messages)
 
     @classmethod
     def from_path(cls, path: Union[str, Path]) -> 'Body':
-        """Builds a body from path to certain file."""
+        """Builds a body from the path to a certain file."""
         if isinstance(path, str):
             path = Path(path)
         return cls.from_lines(path.read_text('utf8').splitlines())
 
     def save(self, fp: TextIO, fmt: str, indent: int) -> None:
         """Saves to a file, supporting `yaml` and `json` formats."""
         data = [m.__dict__ for m in self._messages]
@@ -141,15 +141,15 @@
         for msg in self._messages:
             if msg.name == name:
                 return msg
         return None
 
 
 def parse(data: Union[Iterable[str], TextIOBase, str, Path]) -> Body:
-    """Builds a message body by given data."""
+    """Builds a message body by the data in an iterable or a file."""
     if isinstance(data, (str, Path)):
         return Body.from_path(data)
 
     if isinstance(data, TextIOBase):
         data = data.read().splitlines()
 
     return Body.from_lines(data)
```

### Comparing `qq_chat_history-1.1.3/qq_chat_history/cli.py` & `qq_chat_history-1.1.4/qq_chat_history/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 )
 @click.option(
     '--output-format', '-f', help='Output file format.',
     type=click.Choice(['json', 'yaml']), default='json', show_default=True,
 )
 @click.option('--indent', '-d', help='Output file indent.', type=int, default=2, show_default=True)
 def run(input_file: Path, output_file: Path, output_format: str, indent: int) -> None:
-    """Parse a chat history file in the CLI."""
+    """Parses a chat history file in the CLI."""
     if output_file.suffix[1:] != output_format:
         output_file = output_file.with_suffix(f'.{output_format}')
 
     with output_file.open('w', encoding='utf8') as fp:
         parse(input_file).save(fp, output_format, indent)
```

### Comparing `qq_chat_history-1.1.3/README.md` & `qq_chat_history-1.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 启动时输入 `--help` 参数查看更多配置项。
 
 ```bash
 > qq-chat-history --help
 ```
 
-或者，可以在代码中使用，如下：
+或者，可以作为一个第三方库使用，如下：
 
 ```python
 import qq_chat_history
 
 lines = '''
 =========
 假装我是 QQ 自动生成的文件头
@@ -47,44 +47,27 @@
 1883-03-07 13:24:36 C(456456)
 TCG
 
 1883-03-07 22:00:51 A<someone@example.com>
 塔菲怎么你了
 '''.strip().splitlines()
 
+# 这里的 lines 也可以是文件对象或者以字符串或者 Path 对象表示的文件路径。
 for msg in qq_chat_history.parse(lines):
     print(msg.date, msg.id, msg.name, msg.content)
 ```
 
-注意 `parse` 方法返回的是一个 `Body` 对象，一般以 `Iterable[Message]` 的形式使用。除外，`Body` 也提供了几个函数，~虽然一般也没什么用~。
+注意 `parse` 方法返回的是一个 `Body` 对象，一般以 `Iterable[Message]` 的形式使用。当然 `Body` 也提供了几个函数，~虽然一般也没什么用~。
 
 ## Tips
 
-+ 在 `0.3.0+` 版本中，对于 `parse` 方法的实现进行了大调整，它将返回一个 `Body` 类，原先是 `Iterable[Message]`。但这并**不会导致兼容性问题**，因为 `Body` 也是一个 `Iterable[Message]`。
++ 在 `0.3.0+` 版本中，对于 `parse` 方法的实现进行了较大调整，它将返回一个 `Body` 类，原先是 `Iterable[Message]`。但这并**不会导致兼容性问题**，因为 `Body` 也是一个 `Iterable[Message]`。
 
   不同的是，`Body` 类相对于原先单纯的生成器**提供更多功能**，例如`find_xxx` 方法，可以从数据中查找指定 `id` 或 `name` 的消息；`save` 方法可以将数据以 `yaml` 或 `json` 格式保存到文件中，虽然这个工作一般都直接以 `CLI` 模式启动来完成。
 
-+ 在 `0.3.0+` 版本中，你可以向 `parse` 中传入多种多样的类型。
++ 在 `0.3.0+` 版本中，你可以向 `parse` 中传入多样的类型。
 
   + `Iterable[str]`：迭代每行的可迭代对象，如 `list` 或 `tuple` 等。
   + `TextIOBase`：文本文件对象，如用 `open` 打开的文本文件，或者 `io.StringIO` 都属于文本文件对象。
   + `str`, `Path`：文件路径，如 `./data.txt`。
 
-  这些参数都将被调用合适的工厂方法来构造 `Body` 对象。
-
-+ 由于 `parse` 这个名字的含义比较不清晰，推荐与不推荐的使用方式如下：
-
-  ```python
-  # Not recommended 👎
-  from qq_chat_history import parse
-  parse(...)
-  
-  
-  # Recommended 👍
-  import qq_chat_history
-  qq_chat_history.parse(...)
-  
-  
-  from qq_chat_history import parse as parse_qq
-  parse_qq(...)
-  ```
-
+  这些参数都将以对应的方法来构造 `Body` 对象。
```

### Comparing `qq_chat_history-1.1.3/setup.py` & `qq_chat_history-1.1.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['click>=8.1.3,<9.0.0', 'pyyaml>=6.0,<7.0', 'ujson>=5.7.0,<6.0.0']
 
 entry_points = \
 {'console_scripts': ['qq-chat-history = qq_chat_history.cli:run']}
 
 setup_kwargs = {
     'name': 'qq-chat-history',
-    'version': '1.1.3',
+    'version': '1.1.4',
     'description': 'A tool to extract QQ chat history.',
-    'long_description': "# QQ 聊天记录提取器\n\n## 简介\n\n从 QQ 聊天记录文件中提取聊天信息，仅支持 `txt` 格式的聊天记录。\n\n\n## 安装\n\n使用 `pip` 安装，要求 `Python 3.9` 或以上版本。\n\n```bash\n> pip install -U qq-chat-history\n```\n\n## 使用\n\n最简单的启动方式如下，它会自动在当前目录下创建 `output.json` 进行输出（如果安装到虚拟环境请确保已激活）。\n\n```bash\n> qq-chat-history /path/to/file.txt\n```\n\n启动时输入 `--help` 参数查看更多配置项。\n\n```bash\n> qq-chat-history --help\n```\n\n或者，可以在代码中使用，如下：\n\n```python\nimport qq_chat_history\n\nlines = '''\n=========\n假装我是 QQ 自动生成的文件头\n=========\n\n1883-03-07 11:22:33 A<someone@example.com>\n关注永雏塔菲喵\n关注永雏塔菲谢谢喵\n\n1883-03-07 12:34:56 B(123123)\nTCG\n\n1883-03-07 13:24:36 C(456456)\nTCG\n\n1883-03-07 22:00:51 A<someone@example.com>\n塔菲怎么你了\n'''.strip().splitlines()\n\nfor msg in qq_chat_history.parse(lines):\n    print(msg.date, msg.id, msg.name, msg.content)\n```\n\n注意 `parse` 方法返回的是一个 `Body` 对象，一般以 `Iterable[Message]` 的形式使用。除外，`Body` 也提供了几个函数，~虽然一般也没什么用~。\n\n## Tips\n\n+ 在 `0.3.0+` 版本中，对于 `parse` 方法的实现进行了大调整，它将返回一个 `Body` 类，原先是 `Iterable[Message]`。但这并**不会导致兼容性问题**，因为 `Body` 也是一个 `Iterable[Message]`。\n\n  不同的是，`Body` 类相对于原先单纯的生成器**提供更多功能**，例如`find_xxx` 方法，可以从数据中查找指定 `id` 或 `name` 的消息；`save` 方法可以将数据以 `yaml` 或 `json` 格式保存到文件中，虽然这个工作一般都直接以 `CLI` 模式启动来完成。\n\n+ 在 `0.3.0+` 版本中，你可以向 `parse` 中传入多种多样的类型。\n\n  + `Iterable[str]`：迭代每行的可迭代对象，如 `list` 或 `tuple` 等。\n  + `TextIOBase`：文本文件对象，如用 `open` 打开的文本文件，或者 `io.StringIO` 都属于文本文件对象。\n  + `str`, `Path`：文件路径，如 `./data.txt`。\n\n  这些参数都将被调用合适的工厂方法来构造 `Body` 对象。\n\n+ 由于 `parse` 这个名字的含义比较不清晰，推荐与不推荐的使用方式如下：\n\n  ```python\n  # Not recommended 👎\n  from qq_chat_history import parse\n  parse(...)\n  \n  \n  # Recommended 👍\n  import qq_chat_history\n  qq_chat_history.parse(...)\n  \n  \n  from qq_chat_history import parse as parse_qq\n  parse_qq(...)\n  ```\n\n",
+    'long_description': "# QQ 聊天记录提取器\n\n## 简介\n\n从 QQ 聊天记录文件中提取聊天信息，仅支持 `txt` 格式的聊天记录。\n\n\n## 安装\n\n使用 `pip` 安装，要求 `Python 3.9` 或以上版本。\n\n```bash\n> pip install -U qq-chat-history\n```\n\n## 使用\n\n最简单的启动方式如下，它会自动在当前目录下创建 `output.json` 进行输出（如果安装到虚拟环境请确保已激活）。\n\n```bash\n> qq-chat-history /path/to/file.txt\n```\n\n启动时输入 `--help` 参数查看更多配置项。\n\n```bash\n> qq-chat-history --help\n```\n\n或者，可以作为一个第三方库使用，如下：\n\n```python\nimport qq_chat_history\n\nlines = '''\n=========\n假装我是 QQ 自动生成的文件头\n=========\n\n1883-03-07 11:22:33 A<someone@example.com>\n关注永雏塔菲喵\n关注永雏塔菲谢谢喵\n\n1883-03-07 12:34:56 B(123123)\nTCG\n\n1883-03-07 13:24:36 C(456456)\nTCG\n\n1883-03-07 22:00:51 A<someone@example.com>\n塔菲怎么你了\n'''.strip().splitlines()\n\n# 这里的 lines 也可以是文件对象或者以字符串或者 Path 对象表示的文件路径。\nfor msg in qq_chat_history.parse(lines):\n    print(msg.date, msg.id, msg.name, msg.content)\n```\n\n注意 `parse` 方法返回的是一个 `Body` 对象，一般以 `Iterable[Message]` 的形式使用。当然 `Body` 也提供了几个函数，~虽然一般也没什么用~。\n\n## Tips\n\n+ 在 `0.3.0+` 版本中，对于 `parse` 方法的实现进行了较大调整，它将返回一个 `Body` 类，原先是 `Iterable[Message]`。但这并**不会导致兼容性问题**，因为 `Body` 也是一个 `Iterable[Message]`。\n\n  不同的是，`Body` 类相对于原先单纯的生成器**提供更多功能**，例如`find_xxx` 方法，可以从数据中查找指定 `id` 或 `name` 的消息；`save` 方法可以将数据以 `yaml` 或 `json` 格式保存到文件中，虽然这个工作一般都直接以 `CLI` 模式启动来完成。\n\n+ 在 `0.3.0+` 版本中，你可以向 `parse` 中传入多样的类型。\n\n  + `Iterable[str]`：迭代每行的可迭代对象，如 `list` 或 `tuple` 等。\n  + `TextIOBase`：文本文件对象，如用 `open` 打开的文本文件，或者 `io.StringIO` 都属于文本文件对象。\n  + `str`, `Path`：文件路径，如 `./data.txt`。\n\n  这些参数都将以对应的方法来构造 `Body` 对象。\n",
     'author': 'kifuan',
     'author_email': 'kifuan@foxmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kifuan/qq-chat-history',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `qq_chat_history-1.1.3/PKG-INFO` & `qq_chat_history-1.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qq-chat-history
-Version: 1.1.3
+Version: 1.1.4
 Summary: A tool to extract QQ chat history.
 Home-page: https://github.com/kifuan/qq-chat-history
 License: MIT
 Author: kifuan
 Author-email: kifuan@foxmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -43,15 +43,15 @@
 
 启动时输入 `--help` 参数查看更多配置项。
 
 ```bash
 > qq-chat-history --help
 ```
 
-或者，可以在代码中使用，如下：
+或者，可以作为一个第三方库使用，如下：
 
 ```python
 import qq_chat_history
 
 lines = '''
 =========
 假装我是 QQ 自动生成的文件头
@@ -67,45 +67,28 @@
 1883-03-07 13:24:36 C(456456)
 TCG
 
 1883-03-07 22:00:51 A<someone@example.com>
 塔菲怎么你了
 '''.strip().splitlines()
 
+# 这里的 lines 也可以是文件对象或者以字符串或者 Path 对象表示的文件路径。
 for msg in qq_chat_history.parse(lines):
     print(msg.date, msg.id, msg.name, msg.content)
 ```
 
-注意 `parse` 方法返回的是一个 `Body` 对象，一般以 `Iterable[Message]` 的形式使用。除外，`Body` 也提供了几个函数，~虽然一般也没什么用~。
+注意 `parse` 方法返回的是一个 `Body` 对象，一般以 `Iterable[Message]` 的形式使用。当然 `Body` 也提供了几个函数，~虽然一般也没什么用~。
 
 ## Tips
 
-+ 在 `0.3.0+` 版本中，对于 `parse` 方法的实现进行了大调整，它将返回一个 `Body` 类，原先是 `Iterable[Message]`。但这并**不会导致兼容性问题**，因为 `Body` 也是一个 `Iterable[Message]`。
++ 在 `0.3.0+` 版本中，对于 `parse` 方法的实现进行了较大调整，它将返回一个 `Body` 类，原先是 `Iterable[Message]`。但这并**不会导致兼容性问题**，因为 `Body` 也是一个 `Iterable[Message]`。
 
   不同的是，`Body` 类相对于原先单纯的生成器**提供更多功能**，例如`find_xxx` 方法，可以从数据中查找指定 `id` 或 `name` 的消息；`save` 方法可以将数据以 `yaml` 或 `json` 格式保存到文件中，虽然这个工作一般都直接以 `CLI` 模式启动来完成。
 
-+ 在 `0.3.0+` 版本中，你可以向 `parse` 中传入多种多样的类型。
++ 在 `0.3.0+` 版本中，你可以向 `parse` 中传入多样的类型。
 
   + `Iterable[str]`：迭代每行的可迭代对象，如 `list` 或 `tuple` 等。
   + `TextIOBase`：文本文件对象，如用 `open` 打开的文本文件，或者 `io.StringIO` 都属于文本文件对象。
   + `str`, `Path`：文件路径，如 `./data.txt`。
 
-  这些参数都将被调用合适的工厂方法来构造 `Body` 对象。
-
-+ 由于 `parse` 这个名字的含义比较不清晰，推荐与不推荐的使用方式如下：
-
-  ```python
-  # Not recommended 👎
-  from qq_chat_history import parse
-  parse(...)
-  
-  
-  # Recommended 👍
-  import qq_chat_history
-  qq_chat_history.parse(...)
-  
-  
-  from qq_chat_history import parse as parse_qq
-  parse_qq(...)
-  ```
-
+  这些参数都将以对应的方法来构造 `Body` 对象。
```

