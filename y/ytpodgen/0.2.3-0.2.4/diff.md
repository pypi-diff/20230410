# Comparing `tmp/ytpodgen-0.2.3.tar.gz` & `tmp/ytpodgen-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytpodgen-0.2.3.tar", max compression
+gzip compressed data, was "ytpodgen-0.2.4.tar", max compression
```

## Comparing `ytpodgen-0.2.3.tar` & `ytpodgen-0.2.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-03-20 04:23:49.450612 ytpodgen-0.2.3/LICENSE
--rw-r--r--   0        0        0     3762 2023-03-20 04:13:32.341825 ytpodgen-0.2.3/README.md
--rw-r--r--   0        0        0      541 2023-03-21 14:27:48.240807 ytpodgen-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-20 22:40:31.621239 ytpodgen-0.2.3/ytpodgen/__init__.py
--rw-r--r--   0        0        0     1377 2023-03-21 14:20:12.653307 ytpodgen-0.2.3/ytpodgen/downloader.py
--rw-r--r--   0        0        0      794 2023-03-16 00:54:56.672384 ytpodgen-0.2.3/ytpodgen/feedgenerator.py
--rw-r--r--   0        0        0     1455 2023-03-17 01:19:37.938064 ytpodgen-0.2.3/ytpodgen/uploader.py
--rw-r--r--   0        0        0     2649 2023-03-20 09:08:40.429288 ytpodgen-0.2.3/ytpodgen/ytpodgen.py
--rw-r--r--   0        0        0     4552 1970-01-01 00:00:00.000000 ytpodgen-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-03-27 04:22:24.231435 ytpodgen-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3019 2023-04-01 03:12:31.866761 ytpodgen-0.2.4/README.md
+-rw-r--r--   0        0        0      616 2023-04-10 03:48:04.648702 ytpodgen-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-27 04:22:24.232397 ytpodgen-0.2.4/ytpodgen/__init__.py
+-rw-r--r--   0        0        0     1527 2023-04-08 05:51:59.526544 ytpodgen-0.2.4/ytpodgen/downloader.py
+-rw-r--r--   0        0        0     1225 2023-04-10 03:41:14.385965 ytpodgen-0.2.4/ytpodgen/feedgenerator.py
+-rw-r--r--   0        0        0     1795 2023-04-08 05:56:06.207718 ytpodgen-0.2.4/ytpodgen/uploader.py
+-rw-r--r--   0        0        0     2870 2023-04-10 03:32:52.623757 ytpodgen-0.2.4/ytpodgen/ytpodgen.py
+-rw-r--r--   0        0        0     3809 1970-01-01 00:00:00.000000 ytpodgen-0.2.4/PKG-INFO
```

### Comparing `ytpodgen-0.2.3/LICENSE` & `ytpodgen-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ytpodgen-0.2.3/README.md` & `ytpodgen-0.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,31 @@
+Metadata-Version: 2.1
+Name: ytpodgen
+Version: 0.2.4
+Summary: turns YouTube live streams into podcasts
+Home-page: https://github.com/harupong/ytpodgen
+License: MIT
+Author: harupong
+Author-email: harupong@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: boto3 (>=1.26.89,<2.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: podgen (>=1.1.0,<2.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: yt-dlp (>=2023.3.4,<2024.0.0)
+Project-URL: Repository, https://github.com/harupong/ytpodgen
+Description-Content-Type: text/markdown
+
 # ytpodgen - turns YouTube live streams into podcasts
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## prerequisite
 - python3 and pip
 
 ## first time setup
 ```
 python3 -m pip install --user ytpodgen
@@ -59,17 +82,8 @@
 ## how I configured basic auth on Cloudflare R2 using Cloudflare Workers
 1. connected a custom domain to my R2 bucket, to make the bucket public. [docs](https://developers.cloudflare.com/r2/buckets/public-buckets/)
 2. configured a basic auth worker by following steps described [here](https://qiita.com/AnaKutsu/items/1c8bd0eb938edd3c0e0a).
 3. replaced the plaintext declaration of password with worker env var. [docs](https://developers.cloudflare.com/workers/platform/environment-variables/#environment-variables-via-the-dashboard)
 4. added a trigger(custom domain route) to the basic auth worker. [docs](https://developers.cloudflare.com/workers/platform/triggers/routes/)
 
 ## TODO/IDEAS
-- [ ] replace Click package with argparse (argparse is lightweight and suits ytpodgen well) ref: [1](https://stackoverflow.com/questions/10974491/how-to-combine-interactive-prompting-with-argparse-in-python)
-- [ ] simplify basic auth on R2 bucket e.g. [1](https://zenn.dev/yusukebe/articles/54649c85beef1b) [2](https://zenn.dev/morinokami/articles/url-shortener-with-hono-on-cloudflare-workers)
-- [ ] log when download has started
-- [x] add an option to specify output path
-- [x] use `boto3` for uploading files in order to remove `rclone`
-- [x] generate rss feed with python code in order to remove `dropcaster`
-- [x] embed `yt-dlp` into ytpodgen, instead of calling it via docker
-- [x] use `--live-from-start` option for yt-dlp if the stream has already started
-- [x] package this app using `poetry` so that I can install this using `pip`
-- [x] introduce [Click](https://click.palletsprojects.com/en/8.0.x/) for this project
+moved to [GitHub issues](https://github.com/harupong/ytpodgen/issues/)
```

#### html2text {}

```diff
@@ -1,15 +1,27 @@
-# ytpodgen - turns YouTube live streams into podcasts ## prerequisite - python3
-and pip ## first time setup ``` python3 -m pip install --user ytpodgen ``` Set
-environment variable `SLACK_WEBHOOK_URL`, if you want Slack notification. If
-you want to upload files to Cloudflare R2 as well, don't forget to set three
-environment variables for Cloudflare R2. - R2_ENDPOINT_URL - R2_ACCESS_KEY_ID -
-R2_SECRET_ACCESS_KEY For now, R2 bucket name must be `podcast`. ## examples ###
-wait for new livestream, and once on the air, record it and generate podcast
-RSS in background ``` TITLE=
+Metadata-Version: 2.1 Name: ytpodgen Version: 0.2.4 Summary: turns YouTube live
+streams into podcasts Home-page: https://github.com/harupong/ytpodgen License:
+MIT Author: harupong Author-email: harupong@gmail.com Requires-Python:
+>=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: boto3
+(>=1.26.89,<2.0.0) Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: loguru
+(>=0.6.0,<0.7.0) Requires-Dist: podgen (>=1.1.0,<2.0.0) Requires-Dist: requests
+(>=2.28.2,<3.0.0) Requires-Dist: yt-dlp (>=2023.3.4,<2024.0.0) Project-URL:
+Repository, https://github.com/harupong/ytpodgen Description-Content-Type:
+text/markdown # ytpodgen - turns YouTube live streams into podcasts [![Code
+style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
+(https://github.com/psf/black) ## prerequisite - python3 and pip ## first time
+setup ``` python3 -m pip install --user ytpodgen ``` Set environment variable
+`SLACK_WEBHOOK_URL`, if you want Slack notification. If you want to upload
+files to Cloudflare R2 as well, don't forget to set three environment variables
+for Cloudflare R2. - R2_ENDPOINT_URL - R2_ACCESS_KEY_ID - R2_SECRET_ACCESS_KEY
+For now, R2 bucket name must be `podcast`. ## examples ### wait for new
+livestream, and once on the air, record it and generate podcast RSS in
+background ``` TITLE=
  ; #YouTube live URL that ends with "/live" HOSTNAME= ; #hostname to serve
 files from screen -dmS ${TITLE} ytpodgen --liveurl ${LIVEURL} --title ${TITLE}
 --hostname ${HOSTNAME} ``` When completed, `ytpodgen` will wait for another
 livestream. Since all the waiting might take a while, I prefer running this in
 background using `screen`. ### Why not upload them as well!? You can pass `--
 upload-r2` argument to enable file uploadig to Cloudflare R2. By enabling it,
 mp3s/RSS are uploaded to Cloudflare R2. For example, by running the commands
@@ -30,20 +42,9 @@
 public. [docs](https://developers.cloudflare.com/r2/buckets/public-buckets/) 2.
 configured a basic auth worker by following steps described [here](https://
 qiita.com/AnaKutsu/items/1c8bd0eb938edd3c0e0a). 3. replaced the plaintext
 declaration of password with worker env var. [docs](https://
 developers.cloudflare.com/workers/platform/environment-variables/#environment-
 variables-via-the-dashboard) 4. added a trigger(custom domain route) to the
 basic auth worker. [docs](https://developers.cloudflare.com/workers/platform/
-triggers/routes/) ## TODO/IDEAS - [ ] replace Click package with argparse
-(argparse is lightweight and suits ytpodgen well) ref: [1](https://
-stackoverflow.com/questions/10974491/how-to-combine-interactive-prompting-with-
-argparse-in-python) - [ ] simplify basic auth on R2 bucket e.g. [1](https://
-zenn.dev/yusukebe/articles/54649c85beef1b) [2](https://zenn.dev/morinokami/
-articles/url-shortener-with-hono-on-cloudflare-workers) - [ ] log when download
-has started - [x] add an option to specify output path - [x] use `boto3` for
-uploading files in order to remove `rclone` - [x] generate rss feed with python
-code in order to remove `dropcaster` - [x] embed `yt-dlp` into ytpodgen,
-instead of calling it via docker - [x] use `--live-from-start` option for yt-
-dlp if the stream has already started - [x] package this app using `poetry` so
-that I can install this using `pip` - [x] introduce [Click](https://
-click.palletsprojects.com/en/8.0.x/) for this project
+triggers/routes/) ## TODO/IDEAS moved to [GitHub issues](https://github.com/
+harupong/ytpodgen/issues/)
```

### Comparing `ytpodgen-0.2.3/ytpodgen/downloader.py` & `ytpodgen-0.2.4/ytpodgen/downloader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 from yt_dlp import YoutubeDL
 
 
-from loguru import logger
+class Downloader:
+    def __init__(self):
+        pass
 
-def download(title, liveurl):
-    if _is_live(liveurl):
-        live_from_start = True
-    else:
-        live_from_start = False
-    
-    # See help(yt_dlp.YoutubeDL) for a list of available options and public functions
-    # https://github.com/yt-dlp/yt-dlp/blob/216bcb66d7dce0762767d751dad10650cb57da9d/yt_dlp/YoutubeDL.py#L184
-    ydl_opts = {
-        'format': 'bestaudio/best', # best audio-only format if available, if not, fall back to best format that contains both video and audio
-        'wait_for_video': (60, 60), 
-        'outtmpl': f'{title}_%(epoch>%Y%m%d%H%M%S)s_%(id)s',
-        'live_from_start': live_from_start,
-        'postprocessors': [{  # Extract audio using ffmpeg
-            'key': 'FFmpegExtractAudio',
-            'preferredcodec': 'mp3',
-            'preferredquality': '64'
-        }],
-        'postprocessor_args': [
-            '-ac', '1', # audio channel mono
-        ],
-    }
-
-    with YoutubeDL(ydl_opts) as ydl:
-        error_code = ydl.download(liveurl)
-
-def _is_live(liveurl):
-    ydl_opts = {}
-    with YoutubeDL(ydl_opts) as ydl:
-        try:
+    @staticmethod
+    def download(title, liveurl):
+        live_from_start = True if Downloader._is_live(liveurl) else False
+
+        # See help(yt_dlp.YoutubeDL) for a list of available options
+        # and public functions
+        # https://github.com/yt-dlp/yt-dlp/blob/216bcb66d7dce0762767d751dad10650cb57da9d/yt_dlp/YoutubeDL.py#L184
+        ydl_opts = {
+            # best audio-only format if available,
+            # and if not, fall back to best format that contains both video and audio
+            "format": "bestaudio/best",
+            "wait_for_video": (60, 60),
+            "outtmpl": f"{title}_%(epoch>%Y%m%d%H%M%S)s_%(id)s",
+            "live_from_start": live_from_start,
+            "postprocessors": [
+                {  # Extract audio using ffmpeg
+                    "key": "FFmpegExtractAudio",
+                    "preferredcodec": "mp3",
+                    "preferredquality": "64",
+                }
+            ],
+            "postprocessor_args": [
+                "-ac",
+                "1",  # audio channel mono
+            ],
+        }
+
+        with YoutubeDL(ydl_opts) as ydl:
+            ydl.download(liveurl)
+
+    @staticmethod
+    def _is_live(liveurl):
+        ydl_opts = {}
+        with YoutubeDL(ydl_opts) as ydl:
             info = ydl.extract_info(liveurl, download=False)
-            live_status = info['live_status'].rstrip('\n')
-            if live_status == 'is_live':
-                return True
-        except:
-                return False
+            live_status = info["live_status"].rstrip("\n")
+            return True if live_status == "is_live" else False
```

### Comparing `ytpodgen-0.2.3/ytpodgen/uploader.py` & `ytpodgen-0.2.4/ytpodgen/uploader.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,51 +4,58 @@
 
 
 from botocore.exceptions import ClientError
 import boto3
 from loguru import logger
 
 
-def upload_to_r2(title, bucket='podcast'):
-    s3 = boto3.resource(
-        's3',
-        endpoint_url = get_env_var('R2_ENDPOINT_URL'),
-        aws_access_key_id = get_env_var('R2_ACCESS_KEY_ID'),
-        aws_secret_access_key = get_env_var('R2_SECRET_ACCESS_KEY'),
-    )
-
-    filetypes = '(.+\.mp3|index.rss)' #regex pattern in string
-    files = collect_files(filetypes)
-    podcastbucket = get_or_create_bucket(bucket, s3)
-    upload(title, files, podcastbucket)
-
-def get_env_var(name):
-    try:
-        envvar = os.environ[name]
-        return envvar
-    except KeyError:
-        raise KeyError(f'{name} not set.')
-
-def get_or_create_bucket(bucket, s3):
-    podcastbucket = s3.Bucket(bucket)
-    if not bucket_exists(podcastbucket, s3):
-        podcastbucket.create()
-    return podcastbucket
-
-def collect_files(pattern):
-    files = [
-        p for p in Path('.').glob('*')
-        if re.search(pattern, str(p))
-    ]
-    if not len(files):
-        raise FileNotFoundError('required files not found.')
-    return files
+class Uploader:
+    def __init__(self):
+        pass
+
+    @staticmethod
+    def upload_to_r2(title, bucket="podcast"):
+        s3 = boto3.resource(
+            "s3",
+            endpoint_url=Uploader.get_env_var("R2_ENDPOINT_URL"),
+            aws_access_key_id=Uploader.get_env_var("R2_ACCESS_KEY_ID"),
+            aws_secret_access_key=Uploader.get_env_var("R2_SECRET_ACCESS_KEY"),
+        )
+
+        filetypes = r"(.+\.mp3|index.rss)"  # regex pattern in string
+        files = Uploader.collect_files(filetypes)
+        podcastbucket = Uploader.get_or_create_bucket(bucket, s3)
+        Uploader.upload(title, files, podcastbucket)
 
-def upload(title, upload_files, podcastbucket):
-    for file in upload_files:
+    @staticmethod
+    def get_env_var(name):
         try:
-            podcastbucket.upload_file(file, f'{title}/{file}')
-        except ClientError as e:
-            logger.error(e)
-
-def bucket_exists(s3bucket, s3) -> bool:
-    return s3bucket in s3.buckets.all()
+            envvar = os.environ[name]
+            return envvar
+        except KeyError:
+            raise KeyError(f"{name} not set.")
+
+    @staticmethod
+    def get_or_create_bucket(bucket, s3):
+        podcastbucket = s3.Bucket(bucket)
+        if not Uploader.bucket_exists(podcastbucket, s3):
+            podcastbucket.create()
+        return podcastbucket
+
+    @staticmethod
+    def collect_files(pattern):
+        files = [p for p in Path(".").glob("*") if re.search(pattern, str(p))]
+        if not len(files):
+            raise FileNotFoundError("required files not found.")
+        return files
+
+    @staticmethod
+    def upload(title, upload_files, podcastbucket):
+        for file in upload_files:
+            try:
+                podcastbucket.upload_file(file, f"{title}/{file}")
+            except ClientError as e:
+                logger.error(e)
+
+    @staticmethod
+    def bucket_exists(s3bucket, s3) -> bool:
+        return s3bucket in s3.buckets.all()
```

### Comparing `ytpodgen-0.2.3/ytpodgen/ytpodgen.py` & `ytpodgen-0.2.4/ytpodgen/ytpodgen.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,104 +1,121 @@
+import argparse
 import os
 from importlib.metadata import version
 from pathlib import Path
 from textwrap import dedent
 
 
-import click
 from loguru import logger
 import requests
 
 
-from ytpodgen import downloader, feedgenerator, uploader
+from ytpodgen.downloader import Downloader
+from ytpodgen.feedgenerator import FeedGenerator
+from ytpodgen.uploader import Uploader
+
 
 SLACK_WEBHOOK_URL = os.environ.get("SLACK_WEBHOOK_URL")
 
-def print_version(ctx, param, value):
-    if not value or ctx.resilient_parsing:
-        return
-    ytpodgen_version = version('ytpodgen')
-    click.echo(ytpodgen_version)
-    ctx.exit()
 
 def send_slack_notification(message):
     data = {"text": message}
     requests.post(SLACK_WEBHOOK_URL, json=data)
 
-@click.command()
-@click.option('--title', prompt='enter title', help='title for the podcast')
-@click.option(
-    '--hostname',
-    prompt='enter hostname',
-    help='hostname(custom or r2.dev) to serve files'
-)
-@click.option(
-    '--liveurl',
-    help='Watch for and download the specified YouTube Live URL.'
-)
-@click.option(
-    '--upload-r2',
-    is_flag=True,
-    help='If specified, upload mp3s/RSS to Cloudflare R2.'
-)
-@click.option(
-    '--output',
-    help='Output directory(default: current directory)'
-)
-@click.option(
-    '--version',
-    is_flag=True,
-    callback=print_version,
-    expose_value=False,
-    is_eager=True,
-    help='Show version and exit.'
-)
-
-def cli(title, hostname, liveurl, upload_r2, output):
-    change_work_dir(output, title)
-    create_logger(title)
+
+def get_version():
+    return version("ytpodgen")
+
+
+def parse_arguments():
+    parser = argparse.ArgumentParser(description="Podcast generator")
+    parser.add_argument(
+        "--title",
+        required=True,
+        help="title for the podcast"
+    )
+    parser.add_argument(
+        "--hostname",
+        required=True,
+        help="hostname(custom or r2.dev) to serve files"
+    )
+    parser.add_argument(
+        "--liveurl",
+        help="Watch for and download the specified YouTube Live URL."
+    )
+    parser.add_argument(
+        "--upload-r2",
+        action="store_true",
+        help="If specified, upload mp3s/RSS to Cloudflare R2.",
+    )
+    parser.add_argument(
+        "--output",
+        default=".",
+        help="Output directory(default: current directory)"
+    )
+    parser.add_argument(
+        "--version",
+        action="version",
+        version=get_version(),
+        help="Show version and exit.",
+    )
+
+    args = parser.parse_args()
+    return args
+
+
+def main():
+    args = parse_arguments()
+
+    change_work_dir(args.output, args.title)
+    create_logger(args.title)
 
     try:
         while True:
-            run(title, hostname, liveurl, upload_r2)
-            if liveurl is None:
+            run(args)
+            if args.liveurl is None:
                 break
     except Exception as e:
         logger.error(f"ytpodgen failed with following error messages: {e}")
 
+
 def create_logger(title):
     logger.add(f"{title}.log", level="INFO")
     if SLACK_WEBHOOK_URL:
         logger.add(send_slack_notification, level="SUCCESS")
 
+
 def change_work_dir(output, title):
     try:
         work_dir = Path.cwd()
         if output:
             work_dir = Path(output).absolute()
         os.chdir(work_dir)
     except FileNotFoundError:
         create_logger(title)
         logger.error(f"Invalid argument {output} for --output option.")
         exit()
 
-def run(title, hostname, liveurl, upload_r2):
-    if liveurl:
+
+def run(args):
+    if args.liveurl:
         logger.info("Running yt-dlp...")
-        downloader.download(title, liveurl)
+        Downloader.download(args.title, args.liveurl)
 
     logger.info("Generating feeds...")
-    feedgenerator.generate_rss(title, hostname)
+    FeedGenerator.generate_rss(args.title, args.hostname)
 
-    if upload_r2:
+    if args.upload_r2:
         logger.info("Uploading files...")
-        uploader.upload_to_r2(title)
-        logger.success(dedent(
-            f"""
+        Uploader.upload_to_r2(args.title)
+        logger.success(
+            dedent(
+                f"""
             Upload completed.  Podcast feed url:
-            https://{hostname}/{title}/index.rss
+            https://{args.hostname}/{args.title}/index.rss
             """
             ).strip("\n")
         )
 
-if __name__ == '__main__':
-    cli()
+
+if __name__ == "__main__":
+    main()
```

