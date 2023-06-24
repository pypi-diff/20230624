# Comparing `tmp/funboost-23.4-py3-none-any.whl.zip` & `tmp/funboost-23.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1683837 bytes, number of entries: 220
+Zip file size: 1684056 bytes, number of entries: 220
 -rw-rw-rw-  2.0 fat     2402 b- defN 23-Jun-23 09:05 funboost/__init__.py
 -rw-rw-rw-  2.0 fat    20378 b- defN 23-Jun-03 06:12 funboost/__init__old.py
 -rw-rw-rw-  2.0 fat     6489 b- defN 23-Jun-21 13:54 funboost/constant.py
 -rw-rw-rw-  2.0 fat     7399 b- defN 23-Jun-23 09:05 funboost/funboost_config_deafult.py
 -rw-rw-rw-  2.0 fat     9149 b- defN 23-Apr-27 12:40 funboost/set_frame_config.py
 -rw-rw-rw-  2.0 fat     4186 b- defN 23-Jun-17 05:37 funboost/assist/celery_helper.py
 -rw-rw-rw-  2.0 fat     2089 b- defN 23-May-22 13:41 funboost/assist/dramatiq_helper.py
@@ -23,15 +23,15 @@
 -rw-rw-rw-  2.0 fat     9317 b- defN 22-Jul-15 16:25 funboost/concurrent_pool/custom_threadpool_executor000.py
 -rw-rw-rw-  2.0 fat      373 b- defN 22-Jul-15 16:25 funboost/concurrent_pool/single_thread_executor.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-27 12:40 funboost/concurrent_pool/backup/__init__.py
 -rw-rw-rw-  2.0 fat     9548 b- defN 23-Apr-27 12:40 funboost/concurrent_pool/backup/async_pool_executor0223.py
 -rw-rw-rw-  2.0 fat     9568 b- defN 23-Apr-27 12:40 funboost/concurrent_pool/backup/async_pool_executor_back.py
 -rw-rw-rw-  2.0 fat     5728 b- defN 23-Apr-27 12:40 funboost/concurrent_pool/backup/async_pool_executor_janus.py
 -rw-rw-rw-  2.0 fat      126 b- defN 23-Apr-27 12:40 funboost/consumers/__init__.py
--rw-rw-rw-  2.0 fat    85359 b- defN 23-Jun-23 09:34 funboost/consumers/base_consumer.py
+-rw-rw-rw-  2.0 fat    85044 b- defN 23-Jun-24 02:53 funboost/consumers/base_consumer.py
 -rw-rw-rw-  2.0 fat     7574 b- defN 23-Jun-05 13:53 funboost/consumers/celery_consumer.py
 -rw-rw-rw-  2.0 fat     4574 b- defN 23-Apr-27 12:40 funboost/consumers/celery_consumer000.py
 -rw-rw-rw-  2.0 fat     6033 b- defN 23-Jun-20 13:31 funboost/consumers/confirm_mixin.py
 -rw-rw-rw-  2.0 fat     2144 b- defN 23-May-26 03:56 funboost/consumers/dramatiq_consumer.py
 -rw-rw-rw-  2.0 fat     2025 b- defN 23-May-13 11:56 funboost/consumers/http_consumer.py
 -rw-rw-rw-  2.0 fat     4463 b- defN 23-Apr-27 12:40 funboost/consumers/http_consumer000.py
 -rw-rw-rw-  2.0 fat     1080 b- defN 23-May-13 08:23 funboost/consumers/httpsqs_consumer.py
@@ -76,15 +76,15 @@
 -rw-rw-rw-  2.0 fat      576 b- defN 23-Jun-10 06:27 funboost/core/exit_signal.py
 -rw-rw-rw-  2.0 fat     8875 b- defN 23-Jun-04 14:54 funboost/core/fabric_deploy_helper.py
 -rw-rw-rw-  2.0 fat     1570 b- defN 23-Jun-03 06:43 funboost/core/function_result_status_config.py
 -rw-rw-rw-  2.0 fat     8886 b- defN 23-Jun-23 09:05 funboost/core/function_result_status_saver.py
 -rw-rw-rw-  2.0 fat     1169 b- defN 23-Jun-08 14:00 funboost/core/get_booster.py
 -rw-rw-rw-  2.0 fat      340 b- defN 23-Jun-08 14:00 funboost/core/global_boosters.py
 -rw-rw-rw-  2.0 fat     1192 b- defN 23-Jun-23 09:05 funboost/core/helper_funs.py
--rw-rw-rw-  2.0 fat     5388 b- defN 23-Jun-23 09:24 funboost/core/kill_remote_task.py
+-rw-rw-rw-  2.0 fat     8159 b- defN 23-Jun-24 06:54 funboost/core/kill_remote_task.py
 -rw-rw-rw-  2.0 fat     7782 b- defN 23-Apr-27 12:40 funboost/core/msg_result_getter.py
 -rw-rw-rw-  2.0 fat     3814 b- defN 23-Jun-08 14:00 funboost/core/muliti_process_enhance.py
 -rw-rw-rw-  2.0 fat      178 b- defN 23-Apr-27 12:40 funboost/factories/__init__.py
 -rw-rw-rw-  2.0 fat     8976 b- defN 23-Jun-21 13:54 funboost/factories/broker_kind__publsiher_consumer_type_map.py
 -rw-rw-rw-  2.0 fat      946 b- defN 23-Jun-03 04:51 funboost/factories/consumer_factory.py
 -rw-rw-rw-  2.0 fat     2281 b- defN 23-Jun-03 04:51 funboost/factories/publisher_factotry.py
 -rw-rw-rw-  2.0 fat     4841 b- defN 23-Apr-27 12:40 funboost/function_result_web/app.py
@@ -210,13 +210,13 @@
 -rw-rw-rw-  2.0 fat      909 b- defN 22-Jul-15 16:25 funboost/utils/pysnooper_ydf/__init__.py
 -rw-rw-rw-  2.0 fat     2243 b- defN 22-Jul-15 16:25 funboost/utils/pysnooper_ydf/pycompat.py
 -rw-rw-rw-  2.0 fat    19131 b- defN 23-Apr-27 12:40 funboost/utils/pysnooper_ydf/tracer.py
 -rw-rw-rw-  2.0 fat     2753 b- defN 23-Apr-27 12:40 funboost/utils/pysnooper_ydf/utils.py
 -rw-rw-rw-  2.0 fat     3693 b- defN 23-Apr-27 12:40 funboost/utils/pysnooper_ydf/variables.py
 -rw-rw-rw-  2.0 fat     2332 b- defN 23-Jun-08 14:07 funboost/utils/times/__init__.py
 -rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-08 14:07 funboost/utils/times/version.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-23 09:41 funboost-23.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    26615 b- defN 23-Jun-23 09:41 funboost-23.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-23 09:41 funboost-23.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-23 09:41 funboost-23.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    22651 b- defN 23-Jun-23 09:41 funboost-23.4.dist-info/RECORD
-220 files, 2710526 bytes uncompressed, 1646687 bytes compressed:  39.3%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-24 06:55 funboost-23.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    26615 b- defN 23-Jun-24 06:55 funboost-23.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-24 06:55 funboost-23.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-24 06:55 funboost-23.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    22651 b- defN 23-Jun-24 06:55 funboost-23.5.dist-info/RECORD
+220 files, 2712982 bytes uncompressed, 1646906 bytes compressed:  39.3%
```

## zipnote {}

```diff
@@ -639,23 +639,23 @@
 
 Filename: funboost/utils/times/__init__.py
 Comment: 
 
 Filename: funboost/utils/times/version.py
 Comment: 
 
-Filename: funboost-23.4.dist-info/LICENSE
+Filename: funboost-23.5.dist-info/LICENSE
 Comment: 
 
-Filename: funboost-23.4.dist-info/METADATA
+Filename: funboost-23.5.dist-info/METADATA
 Comment: 
 
-Filename: funboost-23.4.dist-info/WHEEL
+Filename: funboost-23.5.dist-info/WHEEL
 Comment: 
 
-Filename: funboost-23.4.dist-info/top_level.txt
+Filename: funboost-23.5.dist-info/top_level.txt
 Comment: 
 
-Filename: funboost-23.4.dist-info/RECORD
+Filename: funboost-23.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## funboost/consumers/base_consumer.py

```diff
@@ -33,17 +33,17 @@
 
 import nb_log
 from funboost.concurrent_pool.single_thread_executor import SoloExecutor
 from funboost.core.function_result_status_saver import FunctionResultStatusPersistanceConfig, ResultPersistenceHelper, FunctionResultStatus
 
 # noinspection PyUnresolvedReferences
 from funboost.core.helper_funs import delete_keys_and_return_new_dict, get_publish_time
-from nb_log import get_logger, LoggerLevelSetterMixin, nb_print, LoggerMixin, \
-    LoggerMixinDefaultWithFileHandler, stdout_write, is_main_process, \
-    nb_log_config_default
+from nb_log import (get_logger, LoggerLevelSetterMixin, nb_print, LoggerMixin,
+                    LoggerMixinDefaultWithFileHandler, stdout_write, is_main_process,
+                    nb_log_config_default)
 # noinspection PyUnresolvedReferences
 from funboost.concurrent_pool.async_helper import simple_run_in_executor
 from funboost.concurrent_pool.async_pool_executor import AsyncPoolExecutor
 # noinspection PyUnresolvedReferences
 from funboost.concurrent_pool.bounded_threadpoolexcutor import \
     BoundedThreadPoolExecutor
 from func_timeout import func_set_timeout  # noqa
@@ -55,15 +55,14 @@
     CustomThreadPoolExecutor, check_not_monkey
 # from funboost.concurrent_pool.concurrent_pool_with_multi_process import ConcurrentPoolWithProcess
 from funboost.consumers.redis_filter import RedisFilter, RedisImpermanencyFilter
 from funboost.factories.publisher_factotry import get_publisher
 from funboost.utils import decorators, time_util, RedisMixin, un_strict_json_dumps
 # noinspection PyUnresolvedReferences
 from funboost.utils.bulk_operation import MongoBulkWriteHelper, InsertOne
-from funboost.utils.mongo_util import MongoMixin
 from funboost import funboost_config_deafult
 # noinspection PyUnresolvedReferences
 from funboost.constant import ConcurrentModeEnum, BrokerEnum
 from funboost.core import kill_remote_task
 
 
 # patch_apscheduler_run_job()
@@ -118,15 +117,15 @@
     @classmethod
     def show_all_consumer_info(cls):
         # nb_print(f'当前解释器内，所有消费者的信息是：\n  {cls.consumers_queue__info_map}')
         # if only_print_on_main_process(f'当前解释器内，所有消费者的信息是：\n  {json.dumps(cls.consumers_queue__info_map, indent=4, ensure_ascii=False)}'):
         if not cls._has_show_conusmers_info:
             for _, consumer_info in cls.consumers_queue__info_map.items():
                 stdout_write(f'{time.strftime("%H:%M:%S")} "{consumer_info["where_to_instantiate"]}" '
-                             f' \033[0;30;44m{consumer_info["queue_name"]} 的消费者\033[0m\n')
+                             f' \033[0;37;44m{consumer_info["queue_name"]} 的消费者。 \033[0m\n')
         cls._has_show_conusmers_info = True
 
     @staticmethod
     def get_concurrent_name_by_concurrent_mode(concurrent_mode):
         if concurrent_mode == ConcurrentModeEnum.THREADING:
             return 'thread'
         elif concurrent_mode == ConcurrentModeEnum.GEVENT:
@@ -383,15 +382,15 @@
         self._schedule_tasks_on_main_thread = schedule_tasks_on_main_thread
 
         self._function_result_status_persistance_conf = function_result_status_persistance_conf
         self._result_persistence_helper: ResultPersistenceHelper
         self._user_custom_record_process_info_func = user_custom_record_process_info_func
 
         self._is_using_rpc_mode = is_using_rpc_mode  # 是否使用rpc模式 需要安装和配置好redis
-        self._is_support_remote_kill_task = is_support_remote_kill_task # 是否支持远程杀死函数task，需要安装和配置好redis
+        self._is_support_remote_kill_task = is_support_remote_kill_task  # 是否支持远程杀死函数task，需要安装和配置好redis
 
         if broker_exclusive_config is None:
             broker_exclusive_config = {}
         self.broker_exclusive_config = copy.deepcopy(self.BROKER_EXCLUSIVE_CONFIG_DEFAULT)
         self.broker_exclusive_config.update(broker_exclusive_config)
 
         self._stop_flag = None
@@ -831,15 +830,15 @@
                 self.publisher_of_dlx_queue.publish(kw['body'])  # 发布到死信队列，不重回当前队列
                 function_result_status._has_to_dlx_queue = True
             if isinstance(e, kill_remote_task.TaskHasKilledError):
                 log_msg = f'task_id 为 {task_id} , 函数 [{self.consuming_function.__name__}] 运行入参 {function_only_params}   ，已被远程指令杀死 {type(e)}  {e}'
                 self.logger.critical(msg=f'{log_msg} ')
                 self.error_file_logger.critical(msg=f'{log_msg} ')
                 function_result_status._has_kill_task = True
-            if isinstance(e, (ExceptionForRequeue, ExceptionForPushToDlxqueue,kill_remote_task.TaskHasKilledError)):
+            if isinstance(e, (ExceptionForRequeue, ExceptionForPushToDlxqueue, kill_remote_task.TaskHasKilledError)):
                 return function_result_status
             log_msg = f'''函数 {self.consuming_function.__name__}  第{current_retry_times + 1}次运行发生错误，
                               函数运行时间是 {round(time.time() - t_start, 4)} 秒,\n  入参是  {function_only_params}    \n 原因是 {type(e)} {e} '''
             self.logger.error(msg=f'{log_msg} \n', exc_info=self._get_priority_conf(kw, 'is_print_detail_exception'))
             self.error_file_logger.error(msg=f'{log_msg} \n', exc_info=self._get_priority_conf(kw, 'is_print_detail_exception'))
             # traceback.print_exc()
             function_result_status.exception = f'{e.__class__.__name__}    {str(e)}'
@@ -984,21 +983,14 @@
             if self._msg_num_in_broker != -1:
                 self.logger.info(f'队列 [{self._queue_name}] 中还有 [{self._msg_num_in_broker}] 个任务')
             self._last_timestamp_print_msg_num = time.time()
         if self._msg_num_in_broker != 0:
             self._last_timestamp_when_has_task_in_queue = time.time()
         return self._msg_num_in_broker
 
-    @staticmethod
-    def _thread_kill_task_by_task_id():
-        task_id_tuple = RedisMixin().redis_db_frame_version3.brpop(kill_remote_task.REDIS_LIST_KEY_KILL_TASK, timeout=60)
-        if task_id_tuple:
-            task_id = task_id_tuple[1]
-            kill_remote_task.kill_task(task_id)
-
     @abc.abstractmethod
     def _requeue(self, kw):
         """重新入队"""
         raise NotImplementedError
 
     def _apscheduler_job_miss(self, event):
         """
```

## funboost/core/kill_remote_task.py

```diff
@@ -58,57 +58,117 @@
                 t.event_kill.set()
                 kill_thread(t.ident)
 
 
 kill_task = kill_thread_by_task_id
 
 
-class RemoteTaskKiller(RedisMixin, nb_log.LoggerMixin):
+class RemoteTaskKillerZset(RedisMixin, nb_log.LoggerMixin):
+    """
+    zset实现的，需要zrank 多次。
+    """
 
     def __init__(self, queue_name, task_id):
         self.queue_name = queue_name
         self.task_id = task_id
-        self.redis_zset_key = f'funboost_kill_task:{queue_name}'
+        self._redis_zset_key = f'funboost_kill_task:{queue_name}'
         self._lsat_kill_task_ts = time.time()
 
     def send_remote_task_comd(self):
-        self.redis_db_frame_version3.zadd(self.redis_zset_key, {self.task_id: time.time()})
+        self.redis_db_frame_version3.zadd(self._redis_zset_key, {self.task_id: time.time()})
 
     def judge_need_revoke_run(self):
-        if self.redis_db_frame_version3.zrank(self.redis_zset_key, self.task_id) is not None:
-            self.redis_db_frame_version3.zrem(self.redis_zset_key, self.task_id)
+        if self.redis_db_frame_version3.zrank(self._redis_zset_key, self.task_id) is not None:
+            self.redis_db_frame_version3.zrem(self._redis_zset_key, self.task_id)
             return True
         return False
 
     def kill_local_task(self):
         kill_task(self.task_id)
 
     def start_cycle_kill_task(self):
-        def f():
+        def _start_cycle_kill_task():
             while 1:
                 for t in threading.enumerate():
                     if isinstance(t, ThreadKillAble):
                         thread_task_id = getattr(t, 'task_id', None)
-                        if self.redis_db_frame_version3.zrank(self.redis_zset_key, thread_task_id) is not None:
-                            self.redis_db_frame_version3.zrem(self.redis_zset_key, thread_task_id)
+                        if self.redis_db_frame_version3.zrank(self._redis_zset_key, thread_task_id) is not None:
+                            self.redis_db_frame_version3.zrem(self._redis_zset_key, thread_task_id)
                             t.killed = True
                             t.event_kill.set()
                             kill_thread(t.ident)
                             self._lsat_kill_task_ts = time.time()
-                            self.logger.warning(f'队列的 {self.queue_name} ,  任务 {thread_task_id} 被杀死')
+                            self.logger.warning(f'队列 {self.queue_name} 的 任务 {thread_task_id} 被杀死')
                 if time.time() - self._lsat_kill_task_ts < 2:
+                    time.sleep(0.001)
+                else:
+                    time.sleep(5)
+
+        threading.Thread(target=_start_cycle_kill_task).start()
+
+
+class RemoteTaskKiller(RedisMixin, nb_log.LoggerMixin):
+    """
+    hash实现的，只需要 hmget 一次
+    """
+
+    def __init__(self, queue_name, task_id):
+        self.queue_name = queue_name
+        self.task_id = task_id
+        # self.redis_zset_key = f'funboost_kill_task:{queue_name}'
+        self._redis_hash_key = f'funboost_kill_task_hash:{queue_name}'
+        # self._lsat_kill_task_ts = 0  # time.time()
+        self._recent_scan_need_kill_task = False
+
+    def send_kill_remote_task_comd(self):
+        # self.redis_db_frame_version3.zadd(self.redis_zset_key, {self.task_id: time.time()})
+        self.redis_db_frame_version3.hset(self._redis_hash_key, key=self.task_id, value=time.time())
+
+    def judge_need_revoke_run(self):
+        if self.redis_db_frame_version3.hexists(self._redis_hash_key, self.task_id):
+            self.redis_db_frame_version3.hdel(self._redis_hash_key, self.task_id)
+            return True
+        return False
+
+    def kill_local_task(self):
+        kill_task(self.task_id)
+
+    def start_cycle_kill_task(self):
+        def _start_cycle_kill_task():
+            while 1:
+                if self._recent_scan_need_kill_task:
+                    # print(0.0001)
                     time.sleep(0.01)
                 else:
+                    # print(555)
                     time.sleep(5)
+                self._recent_scan_need_kill_task = False
+                thread_task_id_list = []
+                task_id__thread_map = {}
+                for t in threading.enumerate():
+                    if isinstance(t, ThreadKillAble):
+                        thread_task_id = getattr(t, 'task_id', None)
+                        thread_task_id_list.append(thread_task_id)
+                        task_id__thread_map[thread_task_id] = t
+                if thread_task_id_list:
+                    values = self.redis_db_frame_version3.hmget(self._redis_hash_key, keys=thread_task_id_list)
+                    for idx, thread_task_id in enumerate(thread_task_id_list):
+                        if values[idx] is not None:
+                            self.redis_db_frame_version3.hdel(self._redis_hash_key, thread_task_id)
+                            t = task_id__thread_map[thread_task_id]
+                            t.killed = True
+                            t.event_kill.set()
+                            kill_thread(t.ident)
+                            self._recent_scan_need_kill_task = True
+                            self.logger.warning(f'队列 {self.queue_name} 的 任务 {thread_task_id} 被杀死')
 
-        threading.Thread(target=f).start()
+        threading.Thread(target=_start_cycle_kill_task).start()
 
 
 if __name__ == '__main__':
-    import nb_log
 
     test_lock = threading.Lock()
 
 
     def my_fun(x):
         """
         使用lock.acquire(),强行杀死会一直无法释放锁
@@ -141,15 +201,15 @@
     threading.Thread(target=kill_fun_deco(task_id='task1234')(my_fun2), args=(777,)).start()
     threading.Thread(target=kill_fun_deco(task_id='task5678')(my_fun2), args=(888,)).start()
     time.sleep(5)
     # kill_thread_by_task_id('task1234')
 
     k = RemoteTaskKiller('test_kill_queue', 'task1234')
     k.start_cycle_kill_task()
-    k.send_remote_task_comd()
+    k.send_kill_remote_task_comd()
 
     """
     第一种代码：
     test_lock.acquire()
     执行io耗时代码
     test_lock.release()
     如果使用lock.acquire()获得锁以后，执行耗时代码时候，还没有执行lock.release() 强行杀死线程，会导致锁一直不能释放
```

## Comparing `funboost-23.4.dist-info/LICENSE` & `funboost-23.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `funboost-23.4.dist-info/METADATA` & `funboost-23.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funboost
-Version: 23.4
+Version: 23.5
 Summary: pip install funboost，python全功能分布式函数调度框架,。支持python所有类型的并发模式和一切知名消息队列中间件，python函数加速器，框架包罗万象，一统编程思维，兼容50% python业务场景，适用范围广。只需要一行代码即可分布式执行python一切函数，99%用过funboost的pythoner 感受是 方便 快速 强大，相见恨晚 
 Home-page: https://github.com/ydf0509/funboost
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

## Comparing `funboost-23.4.dist-info/RECORD` & `funboost-23.5.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 funboost/concurrent_pool/custom_threadpool_executor000.py,sha256=jJLXy3h-bELap6nZA6yLtdozzTWcvCtZ7IY6MTqLEAM,9317
 funboost/concurrent_pool/single_thread_executor.py,sha256=NDWOegh8Nxpb-Bp-lUlj-DONWvepSmA9qepL1yNgdQI,373
 funboost/concurrent_pool/backup/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funboost/concurrent_pool/backup/async_pool_executor0223.py,sha256=iTxxJFk2lu1P9ZAIkBip3euq3oEQ4_qTODy3xUaOecY,9548
 funboost/concurrent_pool/backup/async_pool_executor_back.py,sha256=vIgUUyF4Zb0jIRPWgNPqyO09YEkQP32kkpGBldqm4qA,9568
 funboost/concurrent_pool/backup/async_pool_executor_janus.py,sha256=OHMWJ9l3EYTpPpcrPrGGKd4K0tmQ2PN8HiX0Dta0EOo,5728
 funboost/consumers/__init__.py,sha256=ZXY_6Kut1VYNQiF5aWEgIWobsW1ht9YUP0TdRZRWFqI,126
-funboost/consumers/base_consumer.py,sha256=oIA1IiXL8SADzxpxCeoGIq1QJg7FB0LVfkYbzBX1CDM,85359
+funboost/consumers/base_consumer.py,sha256=2wZW7m4i63xf9zfXvsGIp26khTAjMod9-K9828LvbC8,85044
 funboost/consumers/celery_consumer.py,sha256=6CqorZH5pbxIjVwn5gNzcxSbos5YWT8eYqxYyYjgUcY,7574
 funboost/consumers/celery_consumer000.py,sha256=8SF8ppHIMH-BIAHO0NyJYnSQxe_PcT6hv05e7DySG54,4574
 funboost/consumers/confirm_mixin.py,sha256=oVBQ1RayIBFOzGNTJ69HdBR_kLd46xd0VfCOKfqDpLA,6033
 funboost/consumers/dramatiq_consumer.py,sha256=kiHM1wpSZykYDomtSGZ2PlMInCDn_8GOGEHqHUD9m0o,2144
 funboost/consumers/http_consumer.py,sha256=3HF8tsH90fUPX3iOmVid_nqW_7hZCFaL7feOkuAM36U,2025
 funboost/consumers/http_consumer000.py,sha256=NXOSiN1qpLAJfJkuF6SjFpWQ28YxMDULzWCBTNMwYe8,4463
 funboost/consumers/httpsqs_consumer.py,sha256=LICZzovaMVrZsJY4GgLrk3EaHz8f9ZZBLKZtWl3frMc,1080
@@ -75,15 +75,15 @@
 funboost/core/exit_signal.py,sha256=GDP3si_hNm7-iNZeeRaON62He47j_jX5weOOsDYW68Y,576
 funboost/core/fabric_deploy_helper.py,sha256=yIdWhlJAR1rCpzvcSme-KrU7RwKH8B7tdwHG-q6QH0U,8875
 funboost/core/function_result_status_config.py,sha256=CE7xaGoL7vT2VsLTHvv-EnJE7K83XVWivBimHVmVfnQ,1570
 funboost/core/function_result_status_saver.py,sha256=tNYRvUfb2T59mda9fLWDftbPbLvyKQg7Sph6BTBy_J4,8886
 funboost/core/get_booster.py,sha256=YlImXa5yjvuON_9JOa2yAlPw0tHj7RET5jBjmbj1gcM,1169
 funboost/core/global_boosters.py,sha256=CDrnKhxEEb-GxTL7JhrDTD1tyhLj7ciAtO1Cy2iyi1Q,340
 funboost/core/helper_funs.py,sha256=SKSMKytJTOFQJsuMKWJ-_mQg6e_Bgpq1ANDzjjBAcio,1192
-funboost/core/kill_remote_task.py,sha256=jLvwcEDEQ0n0MBVB8oV8nki1yuCMg5bM2yAV-udUFFE,5388
+funboost/core/kill_remote_task.py,sha256=Rj4nrz13CKka8he1T8-k6CYN_yjvcaYZaZ7yurKcKzo,8159
 funboost/core/msg_result_getter.py,sha256=a2ffSE8Rvz1t1KVEt4UxIPsWgcriaHE_Armkac-JrJY,7782
 funboost/core/muliti_process_enhance.py,sha256=zNodv3Ww5yCmwO6xCh7k8HntFHjIYYJ9EPaGinvPV9Q,3814
 funboost/factories/__init__.py,sha256=s7kKKjR1HU5eMjPD6r5b-SXTVMo1zBp2JjOAtkyt5Yo,178
 funboost/factories/broker_kind__publsiher_consumer_type_map.py,sha256=Ig1Kze8keS04_vXMNenZSDxibBSjxVrcMkDHviPsxnQ,8976
 funboost/factories/consumer_factory.py,sha256=KFvYkx1a7egtSiTLuVsoRMKLUAotx-QJX1jAI8Xzo3s,946
 funboost/factories/publisher_factotry.py,sha256=Vz66GrCxMt7GV5iqyIXSzZcC_eHF8fj-2kYduzbTTpg,2281
 funboost/function_result_web/app.py,sha256=xUSDBwwDA5wQVWFdFBXj9Y1s7BOh2itUw5pCZl0URMw,4841
@@ -209,12 +209,12 @@
 funboost/utils/pysnooper_ydf/__init__.py,sha256=ctbQdJpLVZ5g_PPstj7Xaqcl0sMIgvUGwZXtcogYyHA,909
 funboost/utils/pysnooper_ydf/pycompat.py,sha256=ehsCfjsLdwoK0_o5fwYWDo3WeqCVfHW5lxekrEZxq4Y,2243
 funboost/utils/pysnooper_ydf/tracer.py,sha256=DYxYeRFSH1jXy4OTB5KIAgQm2EHRWEOwq3EXJig7Yrk,19131
 funboost/utils/pysnooper_ydf/utils.py,sha256=evSmGi_Oul7vSP47AJ0DLjFwoCYCfunJZ1mWxAkwPZw,2753
 funboost/utils/pysnooper_ydf/variables.py,sha256=QejRDESBA06KG9OH4sBT4J1M55eaU29EIHg8K_igaXo,3693
 funboost/utils/times/__init__.py,sha256=z-KQTxXapfu2ScJxISGe7QGffASuyJYL6JGsLXxD6O0,2332
 funboost/utils/times/version.py,sha256=JiZLGTB-HYyBOV4xS0rnx2K2OqVMTebUj30sZRbrleE,16
-funboost-23.4.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-funboost-23.4.dist-info/METADATA,sha256=7U8JVYTqu-PoU-TkMwN82y2eHK0fkqUni7YWcEmmnO8,26615
-funboost-23.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-funboost-23.4.dist-info/top_level.txt,sha256=K8WuKnS6MRcEWxP1NvbmCeujJq6TEfbsB150YROlRw0,9
-funboost-23.4.dist-info/RECORD,,
+funboost-23.5.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+funboost-23.5.dist-info/METADATA,sha256=vP7DG7GGXW7ktzISGDk4Vsgo-GkvlLpCatSrtc9z9uE,26615
+funboost-23.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+funboost-23.5.dist-info/top_level.txt,sha256=K8WuKnS6MRcEWxP1NvbmCeujJq6TEfbsB150YROlRw0,9
+funboost-23.5.dist-info/RECORD,,
```

