# Comparing `tmp/leetcode-cli-0.0.7.tar.gz` & `tmp/leetcode-cli-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leetcode-cli-0.0.7.tar", last modified: Tue Nov  8 12:02:52 2022, max compression
+gzip compressed data, was "leetcode-cli-0.1.0.tar", last modified: Mon Apr 10 08:22:57 2023, max compression
```

## Comparing `leetcode-cli-0.0.7.tar` & `leetcode-cli-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pengchengchen   (501) staff       (20)        0 2022-11-08 12:02:52.837015 leetcode-cli-0.0.7/
--rw-r--r--   0 pengchengchen   (501) staff       (20)     1074 2022-11-08 06:05:26.000000 leetcode-cli-0.0.7/LICENSE
--rw-r--r--   0 pengchengchen   (501) staff       (20)       32 2022-11-08 06:05:26.000000 leetcode-cli-0.0.7/MANIFEST.in
--rw-r--r--   0 pengchengchen   (501) staff       (20)     8214 2022-11-08 12:02:52.837114 leetcode-cli-0.0.7/PKG-INFO
--rw-r--r--   0 pengchengchen   (501) staff       (20)     7798 2022-11-08 11:49:53.000000 leetcode-cli-0.0.7/README.md
-drwxr-xr-x   0 pengchengchen   (501) staff       (20)        0 2022-11-08 12:02:52.836556 leetcode-cli-0.0.7/leetcode_cli.egg-info/
--rw-r--r--   0 pengchengchen   (501) staff       (20)     8214 2022-11-08 12:02:52.000000 leetcode-cli-0.0.7/leetcode_cli.egg-info/PKG-INFO
--rw-r--r--   0 pengchengchen   (501) staff       (20)      333 2022-11-08 12:02:52.000000 leetcode-cli-0.0.7/leetcode_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pengchengchen   (501) staff       (20)        1 2022-11-08 12:02:52.000000 leetcode-cli-0.0.7/leetcode_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pengchengchen   (501) staff       (20)       54 2022-11-08 12:02:52.000000 leetcode-cli-0.0.7/leetcode_cli.egg-info/entry_points.txt
--rw-r--r--   0 pengchengchen   (501) staff       (20)       61 2022-11-08 12:02:52.000000 leetcode-cli-0.0.7/leetcode_cli.egg-info/requires.txt
--rw-r--r--   0 pengchengchen   (501) staff       (20)       12 2022-11-08 12:02:52.000000 leetcode-cli-0.0.7/leetcode_cli.egg-info/top_level.txt
-drwxr-xr-x   0 pengchengchen   (501) staff       (20)        0 2022-11-08 12:02:52.836923 leetcode-cli-0.0.7/leetcodecli/
--rw-r--r--   0 pengchengchen   (501) staff       (20)       21 2022-11-08 06:05:26.000000 leetcode-cli-0.0.7/leetcodecli/__init__.py
--rwxr-xr-x   0 pengchengchen   (501) staff       (20)    30698 2022-11-08 11:58:25.000000 leetcode-cli-0.0.7/leetcodecli/cli.py
--rw-r--r--   0 pengchengchen   (501) staff       (20)      525 2022-11-08 06:05:26.000000 leetcode-cli-0.0.7/leetcodecli/header.html
--rw-r--r--   0 pengchengchen   (501) staff       (20)       67 2022-11-08 12:02:52.837412 leetcode-cli-0.0.7/setup.cfg
--rwxr-xr-x   0 pengchengchen   (501) staff       (20)      947 2022-11-08 10:57:43.000000 leetcode-cli-0.0.7/setup.py
+drwxr-xr-x   0 pengchengchen   (501) staff       (20)        0 2023-04-10 08:22:57.244134 leetcode-cli-0.1.0/
+-rw-r--r--   0 pengchengchen   (501) staff       (20)     1074 2023-04-05 08:49:14.000000 leetcode-cli-0.1.0/LICENSE
+-rw-r--r--   0 pengchengchen   (501) staff       (20)       32 2023-04-05 08:49:14.000000 leetcode-cli-0.1.0/MANIFEST.in
+-rw-r--r--   0 pengchengchen   (501) staff       (20)     8214 2023-04-10 08:22:57.244184 leetcode-cli-0.1.0/PKG-INFO
+-rw-r--r--   0 pengchengchen   (501) staff       (20)     7798 2023-04-05 08:49:14.000000 leetcode-cli-0.1.0/README.md
+drwxr-xr-x   0 pengchengchen   (501) staff       (20)        0 2023-04-10 08:22:57.243710 leetcode-cli-0.1.0/leetcode_cli.egg-info/
+-rw-r--r--   0 pengchengchen   (501) staff       (20)     8214 2023-04-10 08:22:57.000000 leetcode-cli-0.1.0/leetcode_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pengchengchen   (501) staff       (20)      333 2023-04-10 08:22:57.000000 leetcode-cli-0.1.0/leetcode_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pengchengchen   (501) staff       (20)        1 2023-04-10 08:22:57.000000 leetcode-cli-0.1.0/leetcode_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pengchengchen   (501) staff       (20)       54 2023-04-10 08:22:57.000000 leetcode-cli-0.1.0/leetcode_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pengchengchen   (501) staff       (20)       61 2023-04-10 08:22:57.000000 leetcode-cli-0.1.0/leetcode_cli.egg-info/requires.txt
+-rw-r--r--   0 pengchengchen   (501) staff       (20)       12 2023-04-10 08:22:57.000000 leetcode-cli-0.1.0/leetcode_cli.egg-info/top_level.txt
+drwxr-xr-x   0 pengchengchen   (501) staff       (20)        0 2023-04-10 08:22:57.244028 leetcode-cli-0.1.0/leetcodecli/
+-rw-r--r--   0 pengchengchen   (501) staff       (20)       21 2023-04-05 08:49:14.000000 leetcode-cli-0.1.0/leetcodecli/__init__.py
+-rwxr-xr-x   0 pengchengchen   (501) staff       (20)    31680 2023-04-10 08:04:47.000000 leetcode-cli-0.1.0/leetcodecli/cli.py
+-rw-r--r--   0 pengchengchen   (501) staff       (20)     1059 2023-04-05 08:49:14.000000 leetcode-cli-0.1.0/leetcodecli/header.html
+-rw-r--r--   0 pengchengchen   (501) staff       (20)       67 2023-04-10 08:22:57.244367 leetcode-cli-0.1.0/setup.cfg
+-rwxr-xr-x   0 pengchengchen   (501) staff       (20)      947 2023-04-10 08:22:35.000000 leetcode-cli-0.1.0/setup.py
```

### Comparing `leetcode-cli-0.0.7/LICENSE` & `leetcode-cli-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `leetcode-cli-0.0.7/PKG-INFO` & `leetcode-cli-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leetcode-cli
-Version: 0.0.7
+Version: 0.1.0
 Summary: LeetCode CLI
 Home-page: https://github.com/chenpengcheng/cli
 Author: Pengcheng Chen
 Author-email: pengcheng.chen@gmail.com
 Keywords: leetcode
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `leetcode-cli-0.0.7/README.md` & `leetcode-cli-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `leetcode-cli-0.0.7/leetcode_cli.egg-info/PKG-INFO` & `leetcode-cli-0.1.0/leetcode_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leetcode-cli
-Version: 0.0.7
+Version: 0.1.0
 Summary: LeetCode CLI
 Home-page: https://github.com/chenpengcheng/cli
 Author: Pengcheng Chen
 Author-email: pengcheng.chen@gmail.com
 Keywords: leetcode
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `leetcode-cli-0.0.7/leetcodecli/cli.py` & `leetcode-cli-0.1.0/leetcodecli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 #!/usr/bin/env python
 
 import cmd
 import contextlib
 import difflib
 import functools
-import getpass
 import inspect
 import json
 import os
 import random
 import re
 import sys
 import time
 from datetime import datetime
 
 import browser_cookie3
 import bs4
 import execjs
 import requests
+import webbrowser
 
 
 class Magic(object):
     bunnies = [
         """
-  (\(\\
+  (\\(\\
  (='.')
 o(__")")""",
 
         """
-(\__/)
+(\\__/)
 (='.'=)
 (")_(")""",
 
         """
- (\_/)
+ (\\_/)
 =(^.^)=
 (")_(")""",
 
         """
-(\__/)
+(\\__/)
 (>'.'<)
 (")_(")""",
     ]
 
     def __init__(self):
         self.motd = random.choice(self.bunnies)[1:]
 
@@ -251,14 +251,16 @@
         self.session.cookies.update(browser_cookie3.load(domain_name=self.domain))
 
         if self.session.cookies.get('LEETCODE_SESSION'):
             self.loggedIn = True
             print('Welcome to %s!' % self.domain)
         else:
             self.loggedIn = False
+            print('Please login into %s!' % self.domain)
+            webbrowser.open_new_tab(self.url)
 
     def parse_sessions(self, resp):
         sd = {}
         for s in json.loads(resp.text).get('sessions', []):
             sid, name, active = s['id'], s['name'] or '#', s['is_active']
             sd[name] = Session(sid, name, active)
         return sd
@@ -315,16 +317,16 @@
             c = e.get('slug')
             ql = e.get('questions')
             companies[c] = set(ql)
 
         return (topics, companies)
 
     def get_problems(self):
-        ps = 'algorithms/'
-#       ps = 'favorite_lists/top-interview-questions/'
+        # ps = 'algorithms/'
+        ps = 'favorite_lists/top-interview-questions/'
         url = self.url + '/api/problems/' + ps
 
         resp = self.session.get(url)
 
         problems = {}
         for e in json.loads(resp.text).get('stat_status_pairs'):
             i = e.get('stat').get('question_id')
@@ -363,15 +365,14 @@
                 }
             """,
             'variables': {
                 'titleSlug': p.slug
             },
             'operationName': 'getQuestionDetail',
         }
-
         resp = self.session.post(url, json=data, headers=headers)
 
         q = json.loads(resp.text)['data']['question']
         soup = bs4.BeautifulSoup(q.get('content'), 'html.parser')
         p.html = self.strip(soup.prettify())
         p.desc = self.wrap(self.strip(soup.get_text()))
 
@@ -510,57 +511,82 @@
                 break
         else:
             data = {'error': '< network timeout >'}
 
         return Result(sid, data)
 
     def get_history(self, p):
-        url = self.url + '/api/submissions/%s/' % p.slug
-
-        resp = self.session.get(url)
+        url = self.url + '/graphql/'
+        referer = self.url + '/problems/%s/submissions/' % p.slug
+        headers = {
+            'referer': referer,
+            'content-type': 'application/json',
+            'x-csrftoken': self.session.cookies['csrftoken'],
+        }
+        data = {
+            'query': """
+                query Submissions( $offset: Int!  $limit: Int!  $lastKey: String $questionSlug: String!) {
+                    submissionList( offset: $offset limit: $limit lastKey: $lastKey questionSlug: $questionSlug) {
+                        submissions {
+                            id
+                            statusDisplay
+                            lang
+                            timestamp
+                            url
+                        }
+                    }
+                }
+            """,
+            'variables': {
+                'offset': 0,
+                'limit': 10,
+                'questionSlug': p.slug
+            },
+            'operationName': 'Submissions',
+        }
+        resp = self.session.post(url, json=data, headers=headers)
 
         r = History(p.slug)
         try:
-            for e in json.loads(resp.text).get('submissions_dump'):
+            for e in json.loads(resp.text)['data']['submissionList']['submissions']:
                 sid = e.get('url').split('/')[3]
                 lang = e.get('lang')
-                s = e.get('status_display')
-                t = e.get('time')
+                s = e.get('statusDisplay')
+                t = e.get('timestamp')
                 r.add(sid=sid, lang=lang, status=s, timestamp=t)
         except TypeError:
             pass
 
         return r
 
 
 class Html(object):
     def __init__(self, p):
         self.p = p
 
     @staticmethod
     def header():
-        with open('header.html', 'r') as f:
+        with open('leetcodecli/header.html', 'r') as f:
             s = f.read()
         return s + '<body><div class="container">'
 
     @staticmethod
     def tail():
         return '</div></body>'
 
     @property
     def title(self):
         p = self.p
-        s = '<h4>' + str(p.pid) + ' ' + p.slug.replace('-',
-                                                       ' ').title() + '</h4>'
+        s = '<h4>' + str(p.pid) + ' ' + p.slug.replace('-', ' ').title() + '</h4>'
         if p.todo:
-            s = '<div class="bg-primary text-white">' + s + '</div>'
+            s = '<div class="bg-light text-primary">' + s + '</div>'
         elif p.failed or p.rate < 0.34:
-            s = '<div class="bg-danger text-white">' + s + '</div>'
+            s = '<div class="bg-light text-danger">' + s + '</div>'
         else:
-            s = '<div>' + s + '</div>'
+            s = '<div class="bg-light text-dark">' + s + '</div>'
         return s
 
     @property
     def tags(self):
         p = self.p
         return '<div><mark>' + p.tags + '</mark></div>' if p.tags else ''
 
@@ -706,36 +732,32 @@
                 print('   ', p)
 
     def top(self):
         with self.count(self.problems.values()):
             pass
 
     def limit(self, limit):
-        def order(i, j):
-            p, q = self.problems[i], self.problems[j]
-            return -int(p.freq - q.freq)
-
         def update(pd):
-            for k in pd.keys():
+            for k in list(pd):
                 pl = list(filter(lambda i: i not in ps, pd[k]))
                 if pl:
                     pd[k] = pl
                 else:
                     del pd[k]
 
         self.xlimit = limit
         if self.xlimit:
-            ps = set(sorted(self.problems, order)[limit:])
+            ps = set(sorted(self.problems, key=lambda i: -int(self.problems[i].freq))[limit:])
             for pid in ps:
                 del self.problems[pid]
             for pd in [self.topics, self.companies]:
                 update(pd)
 
     def do_help(self, arg):
-        methods = inspect.getmembers(CodeShell, predicate=inspect.ismethod)
+        methods = inspect.getmembers(CodeShell, predicate=inspect.isfunction)
         for key, method in methods:
             if key.startswith('do_'):
                 name = key.split('_')[1]
                 doc = method.__doc__
                 if (not arg or arg == name) and doc:
                     print(name, '\t', doc)
         print("""
@@ -944,33 +966,29 @@
                                 f.write('\n' + result.input)
                         status = 'Wrong Answer'
                     p.record.add(sid=result.sid, lang=self.lang, status=status)
                     print(result)
 
     @login_required
     def do_cheat(self, limit):
-        """<number>\t- C.H.E.A.T."""
+        """<number>\t- Find the best solution."""
         p = self.problems.get(self.pid)
         if p:
             sid = p.record.sid
             cs = self.cheatsheet.get(p.pid, [])
             if not cs and sid:
                 cs = self.get_solutions(p.pid, sid)
                 self.cheatsheet[p.pid] = cs
 
             limit = 1 if not limit else int(limit)
             for c in cs[: limit]:
                 print(c)
 
     def do_print(self, key):
         """[keyword]\t- Print problems by keyword in HTML."""
-        def order(p, q):
-            a = (p.rate, p.pid)
-            b = (q.rate, q.pid)
-            return 1 if a > b else -1 if a < b else 0
 
         def find(key):
             if key in self.topics:
                 topics = {key: self.topics[key]}
             elif key in self.companies:
                 topics = {key: self.companies[key]}
             else:
@@ -996,19 +1014,20 @@
 
         topics, printed = find(key), set()
 
         with open(self.ws + '/%s.html' % fname(key), 'w') as f:
             f.write(Html.header())
             for t, pids in sorted(topics.items()):
                 pl = load(pids, len(printed))
-                for p in sorted(pl, order):
+                for p in sorted(pl, key=lambda p: (p.rate, p.pid)):
                     if p.pid not in printed:
                         f.write(str(Html(p)))
                         printed.add(p.pid)
             f.write(Html.tail())
+        print()
 
     def do_clear(self, unused):
         """\t\t- Clear screen."""
         os.system('clear')
 
     def do_limit(self, limit):
         """<number>\t- Limit the number of problems."""
@@ -1024,7 +1043,11 @@
         return True
 
 
 def main():
     shell = CodeShell()
     shell.do_login()
     shell.cmdloop()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `leetcode-cli-0.0.7/setup.py` & `leetcode-cli-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="leetcode-cli",
-    version="0.0.7",
+    version="0.1.0",
     author="Pengcheng Chen",
     author_email="pengcheng.chen@gmail.com",
     description="LeetCode CLI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/chenpengcheng/cli",
     packages=setuptools.find_packages(),
```

