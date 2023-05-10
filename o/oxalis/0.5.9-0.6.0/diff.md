# Comparing `tmp/oxalis-0.5.9.tar.gz` & `tmp/oxalis-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxalis-0.5.9.tar", max compression
+gzip compressed data, was "oxalis-0.6.0.tar", max compression
```

## Comparing `oxalis-0.5.9.tar` & `oxalis-0.6.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2022-06-07 12:05:40.532331 oxalis-0.5.9/LICENSE
--rw-r--r--   0        0        0     6896 2023-04-20 05:15:02.504528 oxalis-0.5.9/README.md
--rw-r--r--   0        0        0       22 2022-06-03 10:29:06.678568 oxalis-0.5.9/oxalis/__init__.py
--rw-r--r--   0        0        0    11094 2023-05-10 03:09:55.613429 oxalis-0.5.9/oxalis/amqp.py
--rw-r--r--   0        0        0     7490 2023-05-10 02:37:28.864230 oxalis-0.5.9/oxalis/base.py
--rw-r--r--   0        0        0     1978 2023-04-28 02:27:00.905636 oxalis-0.5.9/oxalis/beater.py
--rw-r--r--   0        0        0     4102 2023-04-28 02:24:48.816798 oxalis-0.5.9/oxalis/kafka.py
--rw-r--r--   0        0        0     3506 2023-04-20 05:15:02.508527 oxalis-0.5.9/oxalis/pool.py
--rw-r--r--   0        0        0     6536 2023-04-24 10:09:33.396921 oxalis-0.5.9/oxalis/redis.py
--rw-r--r--   0        0        0      972 2023-05-10 03:10:00.313316 oxalis-0.5.9/pyproject.toml
--rw-r--r--   0        0        0     7859 1970-01-01 00:00:00.000000 oxalis-0.5.9/setup.py
--rw-r--r--   0        0        0     8003 1970-01-01 00:00:00.000000 oxalis-0.5.9/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-06-07 12:05:40.532331 oxalis-0.6.0/LICENSE
+-rw-r--r--   0        0        0     6896 2023-04-20 05:15:02.504528 oxalis-0.6.0/README.md
+-rw-r--r--   0        0        0       22 2022-06-03 10:29:06.678568 oxalis-0.6.0/oxalis/__init__.py
+-rw-r--r--   0        0        0    11203 2023-05-10 09:38:10.724216 oxalis-0.6.0/oxalis/amqp.py
+-rw-r--r--   0        0        0     7842 2023-05-10 09:38:19.452007 oxalis-0.6.0/oxalis/base.py
+-rw-r--r--   0        0        0     1978 2023-04-28 02:27:00.905636 oxalis-0.6.0/oxalis/beater.py
+-rw-r--r--   0        0        0     4211 2023-05-10 09:28:43.097799 oxalis-0.6.0/oxalis/kafka.py
+-rw-r--r--   0        0        0     3506 2023-04-20 05:15:02.508527 oxalis-0.6.0/oxalis/pool.py
+-rw-r--r--   0        0        0     6645 2023-05-10 09:38:10.724216 oxalis-0.6.0/oxalis/redis.py
+-rw-r--r--   0        0        0      884 2023-05-10 09:40:41.272614 oxalis-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7860 1970-01-01 00:00:00.000000 oxalis-0.6.0/setup.py
+-rw-r--r--   0        0        0     7755 1970-01-01 00:00:00.000000 oxalis-0.6.0/PKG-INFO
```

### Comparing `oxalis-0.5.9/LICENSE` & `oxalis-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oxalis-0.5.9/README.md` & `oxalis-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `oxalis-0.5.9/oxalis/amqp.py` & `oxalis-0.6.0/oxalis/amqp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 import typing as tp
 
 import aio_pika
 
+from .base import PARAM, RT
 from .base import Oxalis as _Oxalis
 from .base import Task as _Task
 from .base import TaskCodec, logger
 from .pool import Pool
 
 ExchangeType = aio_pika.ExchangeType
 
@@ -68,15 +69,15 @@
         self.consumer_prefetch_size = consumer_prefetch_size
         self.global_ = global_
 
     def set_channel(self, channel: aio_pika.abc.AbstractChannel):
         self.channel = channel.channel
 
 
-class Task(_Task):
+class Task(_Task[PARAM, RT]):
     def __init__(
         self,
         oxalis: Oxalis,
         func: tp.Callable,
         exchange: Exchange,
         routing_key: str,
         name="",
@@ -99,15 +100,15 @@
             raise ValueError("'reject=True' must get alone with 'ack_later=True'")
         if self.ack_always and not self.ack_later:
             raise ValueError("'ack_always=True' must get alone with 'ack_later=True'")
         if self.reject_requeue and not self.reject:
             raise ValueError("'reject_queue=True' need 'reject=True'")
 
 
-class Oxalis(_Oxalis):
+class Oxalis(_Oxalis[Task]):
     def __init__(
         self,
         connection: aio_pika.Connection,
         task_cls: tp.Type[Task] = Task,
         task_codec: TaskCodec = TaskCodec(),
         pool: Pool = Pool(limit=-1),
         timeout: float = 5.0,
@@ -214,15 +215,17 @@
         exchange: tp.Optional[Exchange] = None,
         routing_key: str = "",
         ack_later: bool = True,
         ack_always: bool = False,
         reject: bool = True,
         reject_requeue: bool = False,
         **_,
-    ) -> tp.Callable[[tp.Callable], Task]:
+    ) -> tp.Callable[
+        [tp.Callable[PARAM, tp.Union[tp.Awaitable[RT], RT]]], Task[PARAM, RT]
+    ]:
         if not exchange:
             exchange = self.default_exchange
         if not routing_key:
             assert exchange
             routing_key = exchange.default_routing_key
 
         def wrapped(func):
```

### Comparing `oxalis-0.5.9/oxalis/base.py` & `oxalis-0.6.0/oxalis/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,46 +15,54 @@
 
 from .pool import Pool
 
 logger = logging.getLogger("oxalis")
 
 
 TASK_TV = tp.TypeVar("TASK_TV", bound="Task")
+PARAM = tp.ParamSpec("PARAM")
+RT = tp.TypeVar("RT")
 
 
-class Task:
+class Task(tp.Generic[PARAM, RT]):
     def __init__(
         self,
         oxalis: Oxalis,
-        func: tp.Callable,
+        func: tp.Callable[PARAM, RT],
         name="",
         timeout: float = -1,
         pool: tp.Optional[Pool] = None,
     ) -> None:
         self.oxalis = oxalis
         self.func = func
         self.name = name or self.get_name()
         self.timeout = timeout
         self.pool = pool or oxalis.pools[0]
+        self._delay: float = 0
+
+    def config(self: TASK_TV, *, delay: float) -> TASK_TV:
+        self._delay = delay
+        return self
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__}({self.name})>"
 
-    async def __call__(self, *args: tp.Any, **kwargs: tp.Any) -> tp.Any:
+    async def __call__(self, *args: PARAM.args, **kwargs: PARAM.kwargs) -> RT:
         ret = self.func(*args, **kwargs)
         if inspect.iscoroutine(ret):
             ret = await ret
 
         return ret
 
-    async def delay(self, *args, _delay: float = 0, **kwargs) -> tp.Any:
+    async def delay(self, *args: PARAM.args, **kwargs: PARAM.kwargs) -> None:
         if self.oxalis.test:
-            return await self(*args, **kwargs)
+            await self.__call__(*args, **kwargs)
         else:
-            await self.oxalis.send_task(self, *args, _delay=_delay, **kwargs)
+            await self.oxalis.send_task(self, *args, _delay=self._delay, **kwargs)
+        self._delay = 0
 
     def get_name(self) -> str:
         return ".".join((self.func.__module__, self.func.__name__))
 
 
 class TaskCodec:
     MESSAGE_TYPE = tp.Tuple[str, tp.Sequence[tp.Any], tp.Dict[str, tp.Any]]
@@ -188,16 +196,18 @@
     def register(
         self,
         *,
         task_name: str = "",
         timeout: float = -1,
         pool: tp.Optional[Pool] = None,
         **_,
-    ) -> tp.Callable[[tp.Callable], TASK_TV]:
-        def wrapped(func):
+    ) -> tp.Callable[
+        [tp.Callable[PARAM, tp.Union[tp.Awaitable[RT], RT]]], Task[PARAM, RT]
+    ]:
+        def wrapped(func: tp.Callable[PARAM, RT]):
             task = self.task_cls(self, func, name=task_name, timeout=timeout, pool=pool)
             self.register_task(task)
             return task
 
         return wrapped
 
     async def on_message_receive(
```

### Comparing `oxalis-0.5.9/oxalis/beater.py` & `oxalis-0.6.0/oxalis/beater.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.5.9/oxalis/kafka.py` & `oxalis-0.6.0/oxalis/kafka.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,35 +4,36 @@
 import contextlib
 import typing
 import typing as tp
 from collections import defaultdict
 
 import aiokafka
 
+from .base import PARAM, RT
 from .base import Oxalis as _Oxalis
 from .base import Task as _Task
 from .base import TaskCodec, logger
 from .pool import Pool
 
 
-class Task(_Task):
+class Task(_Task[PARAM, RT]):
     def __init__(
         self,
         oxalis: Oxalis,
         func: tp.Callable,
         topic: str,
         name="",
         timeout: float = -1,
         pool: tp.Optional[Pool] = None,
     ) -> None:
         super().__init__(oxalis, func, name, timeout, pool)
         self.topic = topic
 
 
-class Oxalis(_Oxalis):
+class Oxalis(_Oxalis[Task]):
     def __init__(
         self,
         kafka_url: str,
         task_cls: tp.Type[Task] = Task,
         task_codec: TaskCodec = TaskCodec(),
         pool: Pool = Pool(limit=-1),
         timeout: float = 5.0,
@@ -86,15 +87,17 @@
         self,
         *,
         task_name: str = "",
         timeout: float = -1,
         topic: str = "",
         pool: tp.Optional[Pool] = None,
         **_,
-    ) -> tp.Callable[[tp.Callable], Task]:
+    ) -> tp.Callable[
+        [tp.Callable[PARAM, tp.Union[tp.Awaitable[RT], RT]]], Task[PARAM, RT]
+    ]:
         if not topic:
             topic = self.default_topic
 
         def wrapped(func):
             task = self.task_cls(
                 self, func, name=task_name, timeout=timeout, topic=topic, pool=pool
             )
```

### Comparing `oxalis-0.5.9/oxalis/pool.py` & `oxalis-0.6.0/oxalis/pool.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.5.9/oxalis/redis.py` & `oxalis-0.6.0/oxalis/redis.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import time
 import typing as tp
 import uuid
 from collections import defaultdict
 
 from redis.asyncio.client import Redis
 
+from .base import PARAM, RT
 from .base import Oxalis as _Oxalis
 from .base import Task as _Task
 from .base import TaskCodec, logger
 from .pool import Pool
 
 
 class Queue:
@@ -21,29 +22,29 @@
         self.name = self.NAME_PREFIX + name
 
 
 class PubsubQueue(Queue):
     pass
 
 
-class Task(_Task):
+class Task(_Task[PARAM, RT]):
     def __init__(
         self,
         oxalis: Oxalis,
         func: tp.Callable,
         queue: Queue,
         name="",
         timeout: float = -1,
         pool: tp.Optional[Pool] = None,
     ) -> None:
         super().__init__(oxalis, func, name, timeout, pool)
         self.queue = queue
 
 
-class Oxalis(_Oxalis):
+class Oxalis(_Oxalis[Task]):
     def __init__(
         self,
         client: Redis,
         task_cls: tp.Type[Task] = Task,
         task_codec: TaskCodec = TaskCodec(),
         pool: Pool = Pool(),
         timeout: float = 2.0,
@@ -98,15 +99,17 @@
         self,
         *,
         task_name: str = "",
         timeout: float = -1,
         pool: tp.Optional[Pool] = None,
         queue: tp.Optional[Queue] = None,
         **_,
-    ) -> tp.Callable[[tp.Callable], Task]:
+    ) -> tp.Callable[
+        [tp.Callable[PARAM, tp.Union[tp.Awaitable[RT], RT]]], Task[PARAM, RT]
+    ]:
         def wrapped(func):
             task = self.task_cls(
                 self,
                 func,
                 queue or self.default_queue,
                 name=task_name,
                 timeout=timeout,
```

### Comparing `oxalis-0.5.9/pyproject.toml` & `oxalis-0.6.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 [tool.poetry]
 name = "oxalis"
-version = "0.5.9"
+version = "0.6.0"
 description = "Distributed async task/job queue"
 authors = ["strongbugman <strongbugman@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers=[
     "Environment :: Console",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 packages = [
     { include = "oxalis" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.10"
 aio-pika = ">=8.0.3"
 croniter = ">=1.3.5"
 redis = ">=4.5.1"
 aiokafka = ">=0.8.0"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=4.6"
```

### Comparing `oxalis-0.5.9/setup.py` & `oxalis-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['aio-pika>=8.0.3', 'aiokafka>=0.8.0', 'croniter>=1.3.5', 'redis>=4.5.1']
 
 setup_kwargs = {
     'name': 'oxalis',
-    'version': '0.5.9',
+    'version': '0.6.0',
     'description': 'Distributed async task/job queue',
     'long_description': '<p>\n<a href="https://pypi.org/project/oxalis/">\n    <img src="https://badge.fury.io/py/oxalis.svg" alt="Package version">\n</a>\n</p>\n\n# Oxalis  \n\nDistributed async task/job queue, like Celery for `asyncio` world\n\n## Feature\n\n* Redis and AMQP(RabbitMQ etc.) support\n* Task timeout and concurrency limit support\n* Delayed task(Both Redis and RabbitMQ) support\n* Cron task/job beater\n* Built-in coroutine pool with concurrency and time limit\n\n## Install\n\n```pip install oxalis```\n\n## Example with Redis backend\n\nDefine task:\n```python\nfrom redis.asyncio.client import Redis\nfrom oxalis.redis import Oxalis\n\n\noxalis = Oxalis(Redis(host=os.getenv("REDIS_HOST", "redis")))\n\n@oxalis.register()\nasync def hello_task():\n    print("Hello oxalis")\n```\n\nRun worker(consumer):\n```python\noxalis.run_worker_master()\n```\n\n```shell\npython ex.py\nINFO:oxalis:Registered Task: <Task(hello_task)>\nINFO:oxalis:Run worker: <Oxalis(pid-101547)>...\nINFO:oxalis:Run worker: <Oxalis(pid-101548)>...\nINFO:oxalis:Run worker: <Oxalis(pid-101549)>...\nINFO:oxalis:Run worker: <Oxalis(pid-101550)>...\nINFO:oxalis:Run worker: <Oxalis(pid-101551)>...\nINFO:oxalis:Run worker: <Oxalis(pid-101552)>...\nINFO:oxalis:Run worker: <Oxalis(pid-101554)>...\n```\n\nRun client(producer):\n```python\nimport asyncio\n\nasyncio.get_event_loop().run_until_complete(oxalis.connect())\nfor i in range(10):\n    asyncio.get_event_loop().run_until_complete(hello_task.delay())\n    asyncio.get_event_loop().run_until_complete(hello_task.delay(_delay=1))  # delay execution after 1s\n```\n\nRun cron beater:\n```python\nfrom oxalis.beater import Beater\n\nbeater = Beater(oxalis)\n\nbeater.register("*/1 * * * *", hello_task)\nbeater.run()\n```\n```shell\npython exb.py \nINFO:oxalis:Beat task: <Task(hello_task)> at <*/1 * * * *> ...\n```\n\n## TaskCodec\n\nThe `TaskCodec` will encode/decode task args, default codec will use `json`\n\nCustom task codec:\n```python\nfrom oxalis.base import TaskCodec\n\nclass MyTaskCodec(TaskCodec):\n    @classmethod\n    def encode(\n        cls,\n        task: Task,\n        task_args: tp.Sequence[tp.Any],\n        task_kwargs: tp.Dict[str, tp.Any],\n    ) -> bytes:\n        ...\n\n    @classmethod\n    def decode(cls, content: bytes) -> TaskCodec.MESSAGE_TYPE:\n        ...\n\n\n\noxalis = Oxalis(Redis(host=os.getenv("REDIS_HOST", "redis")), task_codec=MyTaskCodec())\n...\n```\n\n\n## Task pool\n\nOxalis use one coroutine pool with concurrency limit and timeout limit to run all task\n\nCustom pool:\n\n```python\nfrom redis.asyncio.client import Redis\nfrom oxalis.redis import Oxalis\nfrom oxalis.pool import Pool\n\noxalis = Oxalis(Redis(host=os.getenv("REDIS_HOST", "redis")), pool=Pool(concurrency=10, timeout=60))\n```\n\n* For Redis task, the `queue` will be blocked util `pool` is not fully loaded\n* For AMQP task, oxalis use AMQP\'s QOS to limit worker concurrency(`pool`\'s concurrency will be -1 which means the pool\'s concurrency will not be limited)\n* `asyncio.TimeoutError` will be raised if one task is timeout\n* Every worker process has owned limited pool\n\n\nSpecified one task timeout limit:\n```python\n@oxalis.register(queue=custom_queue, timeout=10)\ndef custom_task():\n    print("Hello oxalis")\n```\n\n## Custom hook\n\nOxalis defined some hook API for inherited subclass:\n```python\nclass MyOxalis(Oxalis):\n    def on_worker_init():\n        # will be called before worker started\n        pass\n\n    def on_worker_close():\n        # will be called after worker started\n        pass\n```\n\nSome API can be rewritten or inherited for custom usage, eg:\n```python\nimport sentry_sdk\n\nclass MyOxalis(Oxalis):\n    async def exec_task(self, task: Task, *task_args, **task_kwargs):\n        """\n        capture exception to sentry\n        """\n        try:\n            await super().exec_task(task, *task_args, **task_kwargs)\n        except Exception as e:\n            sentry_sdk.capture_exception(e)\n```\n\n\n## Redis Backend Detail\n\nOxalis use redis\'s `list` and `pubsub` structure as a message queue\n\n### Queue\n\nCustom queue:\n```python\nfrom oxalis.redis import Queue, PubsubQueue\n\ncustom_queue = Queue("custom")\nbus_queue = PubsubQueue("bus")\n```\n\nRegister task:\n```python\n@oxalis.register(queue=custom_queue)\ndef custom_task():\n    print("Hello oxalis")\n\n@oxalis.register(queue=bus_queue)\ndef bus_task():\n    print("Hello oxalis")\n```\n\n* For task producer, the task will send to specified queue when call `task.delay()`\n* For task consumer, oxalis will listen those queues and receive task from them\n\n### Concurrency limit\n\nOxalis using coroutine pool\'s concurrency limit way, we can set different concurrency limit with specified pool for one task:\n\n```python\n@oxalis.register(pool=Pool(concurrency=1))\ndef custom_task():\n    print("Hello oxalis")\n```\n\n### Delayed task\n\nSupport by redis [zset](https://redis.com/ebook/part-2-core-concepts/chapter-6-application-components-in-redis/6-4-task-queues/6-4-2-delayed-tasks/)\n\n##  AMQP Backend Detail\n\n\n### Custom Queue and Exchange\n\nOxalis using AMQP\'s way to define Exchange, Queue and their bindings\n\n```python\nimport asyncio\nimport logging\nimport time\n\nfrom aio_pika import RobustConnection\nfrom oxalis.amqp import Exchange, ExchangeType, Oxalis, Pool, Queue\n\ne = Exchange("test")\nq = Queue("test", durable=False)\ne2 = Exchange("testfanout", type=ExchangeType.FANOUT)\nq2 = Queue("testfanout", durable=False)\n\n\noxalis = Oxalis(RobustConnection("amqp://root:letmein@rabbitmq:5672/"))\noxalis.register_binding(q, e, "test")\noxalis.register_binding(q2, e2, "")\noxalis.register_queues([q, q2])\n\n\n@oxalis.register(exchange=e, routing_key="test")\nasync def task1():\n    await asyncio.sleep(1)\n    print("hello oxalis")\n\n\n@oxalis.register(exchange=e2)\nasync def task2():\n    await asyncio.sleep(10)\n    print("hello oxalis")\n\n```\n\n* For producer, task `oxalis.register`  defined one task message will send to which exchange(by routing key)\n* For consumer, `register_queues` defined which queues oxalis will listened\n* Task routing defined by bindings\n\n### Concurrency limit\n\nOxalis use AMQP\'s QOS to limit worker concurrency(Task\'s `ack_later` should be true), so coroutine pool\'s concurrency should not be limited.\n\nCustom queue QOS:\n```python\noxalis = Oxalis(RobustConnection("amqp://root:letmein@rabbitmq:5672/"), default_queue=Queue("custom",consumer_prefetch_count=10))\n...\nfanout_queue = Queue("testfanout", durable=False, consumer_prefetch_count=3)\noxalis.register_queues([fanout_queue])\n...\n```\n\n### Custom task behavior\n\nDefine task how to perform `ack` and `reject` \n\n```python\n# always ack even task failed(raise exception)\n@oxalis.register(ack_always=True, reject=False)\nasync def task2():\n    await asyncio.sleep(10)\n    print("hello oxalis")\n\n#  reject with requeue when task failed\n@oxalis.register(reject_requeue=True)\nasync def task2():\n    await asyncio.sleep(10)\n    print("hello oxalis")\n```\n\n### Delayed task\n\nSupport by RabbitMq\'s [plugin](https://blog.rabbitmq.com/posts/2015/04/scheduling-messages-with-rabbitmq)\n',
     'author': 'strongbugman',
     'author_email': 'strongbugman@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['oxalis']
 package_data = \ {'': ['*']} install_requires = \ ['aio-pika>=8.0.3',
 'aiokafka>=0.8.0', 'croniter>=1.3.5', 'redis>=4.5.1'] setup_kwargs = { 'name':
-'oxalis', 'version': '0.5.9', 'description': 'Distributed async task/job
+'oxalis', 'version': '0.6.0', 'description': 'Distributed async task/job
 queue', 'long_description': '
 \n\n_[Package_version]\n\n
 \n\n# Oxalis \n\nDistributed async task/job queue, like Celery for `asyncio`
 world\n\n## Feature\n\n* Redis and AMQP(RabbitMQ etc.) support\n* Task timeout
 and concurrency limit support\n* Delayed task(Both Redis and RabbitMQ)
 support\n* Cron task/job beater\n* Built-in coroutine pool with concurrency and
 time limit\n\n## Install\n\n```pip install oxalis```\n\n## Example with Redis
@@ -101,8 +101,8 @@
 when task failed\n@oxalis.register(reject_requeue=True)\nasync def task2():\n
 await asyncio.sleep(10)\n print("hello oxalis")\n```\n\n### Delayed
 task\n\nSupport by RabbitMq\'s [plugin](https://blog.rabbitmq.com/posts/2015/
 04/scheduling-messages-with-rabbitmq)\n', 'author': 'strongbugman',
 'author_email': 'strongbugman@gmail.com', 'maintainer': 'None',
 'maintainer_email': 'None', 'url': 'None', 'packages': packages,
 'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
+'python_requires': '>=3.10,<4.0', } setup(**setup_kwargs)
```

### Comparing `oxalis-0.5.9/PKG-INFO` & `oxalis-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 Metadata-Version: 2.1
 Name: oxalis
-Version: 0.5.9
+Version: 0.6.0
 Summary: Distributed async task/job queue
 License: MIT
 Author: strongbugman
 Author-email: strongbugman@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aio-pika (>=8.0.3)
 Requires-Dist: aiokafka (>=0.8.0)
 Requires-Dist: croniter (>=1.3.5)
 Requires-Dist: redis (>=4.5.1)
 Description-Content-Type: text/markdown
```

