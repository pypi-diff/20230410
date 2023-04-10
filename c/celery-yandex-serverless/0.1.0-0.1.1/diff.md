# Comparing `tmp/celery_yandex_serverless-0.1.0.tar.gz` & `tmp/celery_yandex_serverless-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery_yandex_serverless-0.1.0.tar", max compression
+gzip compressed data, was "celery_yandex_serverless-0.1.1.tar", max compression
```

## Comparing `celery_yandex_serverless-0.1.0.tar` & `celery_yandex_serverless-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     5289 2023-03-29 17:38:11.111003 celery_yandex_serverless-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-03-28 16:34:01.621354 celery_yandex_serverless-0.1.0/celery_yandex_serverless/__init__.py
--rw-r--r--   0        0        0     3571 2023-03-29 15:43:26.929194 celery_yandex_serverless-0.1.0/celery_yandex_serverless/django.py
--rw-r--r--   0        0        0      470 2023-03-30 17:25:33.323182 celery_yandex_serverless-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6173 1970-01-01 00:00:00.000000 celery_yandex_serverless-0.1.0/setup.py
--rw-r--r--   0        0        0     5958 1970-01-01 00:00:00.000000 celery_yandex_serverless-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5768 2023-04-10 11:45:26.941835 celery_yandex_serverless-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-03-28 16:34:01.621354 celery_yandex_serverless-0.1.1/celery_yandex_serverless/__init__.py
+-rw-r--r--   0        0        0     3381 2023-04-10 16:32:52.281683 celery_yandex_serverless-0.1.1/celery_yandex_serverless/django.py
+-rw-r--r--   0        0        0      471 2023-04-10 16:33:35.418769 celery_yandex_serverless-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6672 1970-01-01 00:00:00.000000 celery_yandex_serverless-0.1.1/setup.py
+-rw-r--r--   0        0        0     6438 1970-01-01 00:00:00.000000 celery_yandex_serverless-0.1.1/PKG-INFO
```

### Comparing `celery_yandex_serverless-0.1.0/README.md` & `celery_yandex_serverless-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -99,14 +99,33 @@
   --invoke-container-name SERVERLESS_CONTAINER_NAME \
   --invoke-container-service-account-name SERVICE_ACCOUNT_NAME \
   --invoke-container-path /worker/CELERY_YANDEX_SERVERLESS_KEY \
   --batch-size 1 \
   --batch-cutoff 10s 
 ```
 
+### Включение логирования
+
+Добавьте в `settings.py`:
+```python
+LOGGING = {
+    "version": 1,
+    "disable_existing_loggers": False,
+    "loggers": {
+        "celery_yandex_serverless.django": {
+            "level": "INFO",
+        },
+    },
+}
+```
+
+Уровни:
+- `INFO` - инфорация о начале и окончании обработки задачи
+- `DEBUG` - печать содержимого аргументов celery-таска
+
 ## Статьи в Яндекс.Облаке
 - [Подключение Celery](https://cloud.yandex.ru/docs/message-queue/instruments/celery)
 - [Документация по созданию триггеров через yc](https://cloud.yandex.ru/docs/cli/cli-ref/managed-services/serverless/trigger/create/message-queue).
 - [Подробнее про работу триггера](https://cloud.yandex.ru/docs/serverless-containers/concepts/trigger/ymq-trigger).
 
 ## Автор
 [Атнагулов Артур](https://atnartur.dev)
```

### Comparing `celery_yandex_serverless-0.1.0/celery_yandex_serverless/django.py` & `celery_yandex_serverless-0.1.1/celery_yandex_serverless/django.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,20 +65,18 @@
 
             try:
                 # start celery task
                 result = function.apply(
                     args=args,
                     kwargs=kwargs,
                     task_id=data['headers']['id'],
-                    headers=data['headers']['headers'],
                     **options
                 )
                 logger.info("task %s processed", function_name)
 
-                # возвращаем ответ в зависимости от успешности обработки задачи
                 if not result.successful():
                     logging.error(result.info)
                     return JsonResponse({"status": "task_error", "info": str(result.info)})
             except Exception:
                 raise
             finally:
                 # return settings to default state
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `celery_yandex_serverless-0.1.0/setup.py` & `celery_yandex_serverless-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 ['boto3>=1.26.101,<2.0.0',
  'celery>=5.2.7,<6.0.0',
  'django>=4,<5',
  'pycurl>=7.45.2,<8.0.0']
 
 setup_kwargs = {
     'name': 'celery-yandex-serverless',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Package for starting Celery worker inside Yandex Cloud Serverless Container',
-    'long_description': '# Celery Yandex Serverless\n\nМодуль, позволяющий запустить celery-worker внутри Yandex Cloud Serverless Container.\n\n**Классический подход с отдельно запущенным воркером**\n\n1. Бекенд отправляет задачу в очередь.\n2. Отдельный процесс воркера забирает задачу из очереди и выполняет ее.\n\n**Serverless-подход**\n\nВ Serverless подходе предполагается, что нет никаких запущенных постоянно процессов приложения. Эти процессы запускаются\nлибо по запросу пользователя, либо по различным тригерам облаком. \n\nМодуль `celery-yandex-serverless` помогает запустить воркер следующим образом:\n1. Бекенд отправляет задачу в очередь\n2. После попадания задачи в очередь срабатывает триггер, который делает http-запрос serverless-контейнеру.\n3. Serverless-контейнер запускает код задачи, который ранее выполнялся в воркере.\n\n## Использование\n\n### Подключение Celery к Yandex Message Queue\n\n1. Перейдите на страницу каталога в Яндекс.Облаке\n2. Зайдите в раздел **Сервисные аккаунты**\n3. Посмотрите название сервисного аккаунта в каталоге Яндекс.Облака\n4. Сгенерируйте `ACCESS_KEY` и `SECRET_KEY` с помощью команды \n(замените `SERVICE_ACCOUNT_NAME` на название сервисного аккаунта):\n\n```bash\nyc iam access-key create --service-account-name SERVICE_ACCOUNT_NAME\n```\n\nКоманда вернет следующую информацию. Сохраните ее, она пригодится в будущем.\n\n```yml{5,6}\naccess_key:\n  id: aje...\n  service_account_id: aje...\n  created_at: "2023-03-24T17:49:01.555836400Z"\n  key_id: YCAJ... # <- Это access key\nsecret: YCPM... # <- Это secret key\n```\n\n### Настройка\nУкажите переменные окружения с использованием только что полученных данных:\n\n```\nAWS_ACCESS_KEY_ID="access key, скопированный выше"\nAWS_SECRET_ACCESS_KEY="secret key, скопированный выше"\nAWS_DEFAULT_REGION="ru-central1"\nCELERY_BROKER_URL=sqs://message-queue.api.cloud.yandex.net:443\nCELERY_BROKER_IS_SECURE=True\n```\n\nВ файле `settings.py` укажите:\n\n```python\nCELERY_BROKER_URL = os.environ.get("CELERY_BROKER_URL")\nCELERY_BROKER_TRANSPORT_OPTIONS = {\n    \'is_secure\': os.environ.get("CELERY_BROKER_IS_SECURE", \'false\').lower() == \'true\'\n}\n```\n\nПосле этого отправьте celery-задачу, чтобы в Яндекс.Облаке появилась очередь.\n\n### Подключение модуля\n\n1. `pip install celery-yandex-serverless` - установите модуль\n2. В urls.py (`projectname` замените на название проекта):\n```python\nfrom django.urls import path\nfrom celery_yandex_serverless.django import worker_view_factory\n\nfrom projectname.celery import app\n\nurlpatterns = [\n    # другие адреса...\n    path("worker/<str:key>/", worker_view_factory(app)),\n]\n```\n\n3. Установите переменную окружения `CELERY_YANDEX_SERVERLESS_KEY` со случайным ключом. \nОн предотвратит нежелательные запуски воркеров по прямому обращению к URL.\n\n### Создание триггера в Яндекс.Облаке\n\nВ консольной команде ниже сделайте замены и выполните ее:\n- `YANDEX_MESSAGE_QUEUE_ARN` - ARN очереди\n- `SERVICE_ACCOUNT_NAME` - название сервисного аккаунта\n- `SERVERLESS_CONTAINER_NAME` - название serverless-контейнера\n- `CELERY_YANDEX_SERVERLESS_KEY` - ключ, созданный ранее\n\n```bash\nyc serverless trigger create message-queue \\\n  --name celery \\\n  --queue YANDEX_MESSAGE_QUEUE_ARN \\\n  --queue-service-account-name SERVICE_ACCOUNT_NAME \\\n  --invoke-container-name SERVERLESS_CONTAINER_NAME \\\n  --invoke-container-service-account-name SERVICE_ACCOUNT_NAME \\\n  --invoke-container-path /worker/CELERY_YANDEX_SERVERLESS_KEY \\\n  --batch-size 1 \\\n  --batch-cutoff 10s \n```\n\n## Статьи в Яндекс.Облаке\n- [Подключение Celery](https://cloud.yandex.ru/docs/message-queue/instruments/celery)\n- [Документация по созданию триггеров через yc](https://cloud.yandex.ru/docs/cli/cli-ref/managed-services/serverless/trigger/create/message-queue).\n- [Подробнее про работу триггера](https://cloud.yandex.ru/docs/serverless-containers/concepts/trigger/ymq-trigger).\n\n## Автор\n[Атнагулов Артур](https://atnartur.dev)\n\nЛицензия MIT.\n',
+    'long_description': '# Celery Yandex Serverless\n\nМодуль, позволяющий запустить celery-worker внутри Yandex Cloud Serverless Container.\n\n**Классический подход с отдельно запущенным воркером**\n\n1. Бекенд отправляет задачу в очередь.\n2. Отдельный процесс воркера забирает задачу из очереди и выполняет ее.\n\n**Serverless-подход**\n\nВ Serverless подходе предполагается, что нет никаких запущенных постоянно процессов приложения. Эти процессы запускаются\nлибо по запросу пользователя, либо по различным тригерам облаком. \n\nМодуль `celery-yandex-serverless` помогает запустить воркер следующим образом:\n1. Бекенд отправляет задачу в очередь\n2. После попадания задачи в очередь срабатывает триггер, который делает http-запрос serverless-контейнеру.\n3. Serverless-контейнер запускает код задачи, который ранее выполнялся в воркере.\n\n## Использование\n\n### Подключение Celery к Yandex Message Queue\n\n1. Перейдите на страницу каталога в Яндекс.Облаке\n2. Зайдите в раздел **Сервисные аккаунты**\n3. Посмотрите название сервисного аккаунта в каталоге Яндекс.Облака\n4. Сгенерируйте `ACCESS_KEY` и `SECRET_KEY` с помощью команды \n(замените `SERVICE_ACCOUNT_NAME` на название сервисного аккаунта):\n\n```bash\nyc iam access-key create --service-account-name SERVICE_ACCOUNT_NAME\n```\n\nКоманда вернет следующую информацию. Сохраните ее, она пригодится в будущем.\n\n```yml{5,6}\naccess_key:\n  id: aje...\n  service_account_id: aje...\n  created_at: "2023-03-24T17:49:01.555836400Z"\n  key_id: YCAJ... # <- Это access key\nsecret: YCPM... # <- Это secret key\n```\n\n### Настройка\nУкажите переменные окружения с использованием только что полученных данных:\n\n```\nAWS_ACCESS_KEY_ID="access key, скопированный выше"\nAWS_SECRET_ACCESS_KEY="secret key, скопированный выше"\nAWS_DEFAULT_REGION="ru-central1"\nCELERY_BROKER_URL=sqs://message-queue.api.cloud.yandex.net:443\nCELERY_BROKER_IS_SECURE=True\n```\n\nВ файле `settings.py` укажите:\n\n```python\nCELERY_BROKER_URL = os.environ.get("CELERY_BROKER_URL")\nCELERY_BROKER_TRANSPORT_OPTIONS = {\n    \'is_secure\': os.environ.get("CELERY_BROKER_IS_SECURE", \'false\').lower() == \'true\'\n}\n```\n\nПосле этого отправьте celery-задачу, чтобы в Яндекс.Облаке появилась очередь.\n\n### Подключение модуля\n\n1. `pip install celery-yandex-serverless` - установите модуль\n2. В urls.py (`projectname` замените на название проекта):\n```python\nfrom django.urls import path\nfrom celery_yandex_serverless.django import worker_view_factory\n\nfrom projectname.celery import app\n\nurlpatterns = [\n    # другие адреса...\n    path("worker/<str:key>/", worker_view_factory(app)),\n]\n```\n\n3. Установите переменную окружения `CELERY_YANDEX_SERVERLESS_KEY` со случайным ключом. \nОн предотвратит нежелательные запуски воркеров по прямому обращению к URL.\n\n### Создание триггера в Яндекс.Облаке\n\nВ консольной команде ниже сделайте замены и выполните ее:\n- `YANDEX_MESSAGE_QUEUE_ARN` - ARN очереди\n- `SERVICE_ACCOUNT_NAME` - название сервисного аккаунта\n- `SERVERLESS_CONTAINER_NAME` - название serverless-контейнера\n- `CELERY_YANDEX_SERVERLESS_KEY` - ключ, созданный ранее\n\n```bash\nyc serverless trigger create message-queue \\\n  --name celery \\\n  --queue YANDEX_MESSAGE_QUEUE_ARN \\\n  --queue-service-account-name SERVICE_ACCOUNT_NAME \\\n  --invoke-container-name SERVERLESS_CONTAINER_NAME \\\n  --invoke-container-service-account-name SERVICE_ACCOUNT_NAME \\\n  --invoke-container-path /worker/CELERY_YANDEX_SERVERLESS_KEY \\\n  --batch-size 1 \\\n  --batch-cutoff 10s \n```\n\n### Включение логирования\n\nДобавьте в `settings.py`:\n```python\nLOGGING = {\n    "version": 1,\n    "disable_existing_loggers": False,\n    "loggers": {\n        "celery_yandex_serverless.django": {\n            "level": "INFO",\n        },\n    },\n}\n```\n\nУровни:\n- `INFO` - инфорация о начале и окончании обработки задачи\n- `DEBUG` - печать содержимого аргументов celery-таска\n\n## Статьи в Яндекс.Облаке\n- [Подключение Celery](https://cloud.yandex.ru/docs/message-queue/instruments/celery)\n- [Документация по созданию триггеров через yc](https://cloud.yandex.ru/docs/cli/cli-ref/managed-services/serverless/trigger/create/message-queue).\n- [Подробнее про работу триггера](https://cloud.yandex.ru/docs/serverless-containers/concepts/trigger/ymq-trigger).\n\n## Автор\n[Атнагулов Артур](https://atnartur.dev)\n\nЛицензия MIT.\n',
     'author': 'atnartur',
-    'author_email': 'i@atnartur.ru',
+    'author_email': 'i@atnartur.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
```

### Comparing `celery_yandex_serverless-0.1.0/PKG-INFO` & `celery_yandex_serverless-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: celery-yandex-serverless
-Version: 0.1.0
+Version: 0.1.1
 Summary: Package for starting Celery worker inside Yandex Cloud Serverless Container
 Author: atnartur
-Author-email: i@atnartur.ru
+Author-email: i@atnartur.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.101,<2.0.0)
@@ -117,14 +117,33 @@
   --invoke-container-name SERVERLESS_CONTAINER_NAME \
   --invoke-container-service-account-name SERVICE_ACCOUNT_NAME \
   --invoke-container-path /worker/CELERY_YANDEX_SERVERLESS_KEY \
   --batch-size 1 \
   --batch-cutoff 10s 
 ```
 
+### Включение логирования
+
+Добавьте в `settings.py`:
+```python
+LOGGING = {
+    "version": 1,
+    "disable_existing_loggers": False,
+    "loggers": {
+        "celery_yandex_serverless.django": {
+            "level": "INFO",
+        },
+    },
+}
+```
+
+Уровни:
+- `INFO` - инфорация о начале и окончании обработки задачи
+- `DEBUG` - печать содержимого аргументов celery-таска
+
 ## Статьи в Яндекс.Облаке
 - [Подключение Celery](https://cloud.yandex.ru/docs/message-queue/instruments/celery)
 - [Документация по созданию триггеров через yc](https://cloud.yandex.ru/docs/cli/cli-ref/managed-services/serverless/trigger/create/message-queue).
 - [Подробнее про работу триггера](https://cloud.yandex.ru/docs/serverless-containers/concepts/trigger/ymq-trigger).
 
 ## Автор
 [Атнагулов Артур](https://atnartur.dev)
```

