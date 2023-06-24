# Comparing `tmp/pysiml-0.2.9.dev202306221046-py3-none-any.whl.zip` & `tmp/pysiml-0.2.9.dev202306240932-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 170250 bytes, number of entries: 138
+Zip file size: 173272 bytes, number of entries: 142
 -rw-r--r--  2.0 unx     1520 b- defN 80-Jan-01 00:00 pyproject.toml
 -rw-r--r--  2.0 unx      638 b- defN 80-Jan-01 00:00 siml/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 siml/__main__/__init__.py
 -rw-r--r--  2.0 unx      900 b- defN 80-Jan-01 00:00 siml/__main__/convert_interim_data.py
 -rw-r--r--  2.0 unx     1400 b- defN 80-Jan-01 00:00 siml/__main__/convert_raw_data.py
 -rw-r--r--  2.0 unx     1742 b- defN 80-Jan-01 00:00 siml/__main__/optimize.py
 -rw-r--r--  2.0 unx     8663 b- defN 80-Jan-01 00:00 siml/__main__/plot_losses.py
@@ -109,32 +109,36 @@
 -rw-r--r--  2.0 unx     5603 b- defN 80-Jan-01 00:00 siml/services/inference/postprocessing/post_fem_data.py
 -rw-r--r--  2.0 unx     4979 b- defN 80-Jan-01 00:00 siml/services/inference/postprocessing/postprocessor.py
 -rw-r--r--  2.0 unx     7052 b- defN 80-Jan-01 00:00 siml/services/inference/postprocessing/save_processor.py
 -rw-r--r--  2.0 unx     1082 b- defN 80-Jan-01 00:00 siml/services/inference/record_object.py
 -rw-r--r--  2.0 unx     2574 b- defN 80-Jan-01 00:00 siml/services/model_builder.py
 -rw-r--r--  2.0 unx     4978 b- defN 80-Jan-01 00:00 siml/services/model_selector.py
 -rw-r--r--  2.0 unx     7124 b- defN 80-Jan-01 00:00 siml/services/path_rules.py
--rw-r--r--  2.0 unx       57 b- defN 80-Jan-01 00:00 siml/services/training/__init__.py
--rw-r--r--  2.0 unx     2383 b- defN 80-Jan-01 00:00 siml/services/training/inner_settings.py
+-rw-r--r--  2.0 unx      200 b- defN 80-Jan-01 00:00 siml/services/training/__init__.py
+-rw-r--r--  2.0 unx     2653 b- defN 80-Jan-01 00:00 siml/services/training/inner_settings.py
+-rw-r--r--  2.0 unx      775 b- defN 80-Jan-01 00:00 siml/services/training/logging_items/__init__.py
+-rw-r--r--  2.0 unx     4198 b- defN 80-Jan-01 00:00 siml/services/training/logging_items/logging_items.py
+-rw-r--r--  2.0 unx     5695 b- defN 80-Jan-01 00:00 siml/services/training/training_logger.py
 -rw-r--r--  2.0 unx    50394 b- defN 80-Jan-01 00:00 siml/setting.py
 -rw-r--r--  2.0 unx      163 b- defN 80-Jan-01 00:00 siml/siml_variables/__init__.py
 -rw-r--r--  2.0 unx      594 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/__init__.py
 -rw-r--r--  2.0 unx     1573 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/interface_wrapper.py
 -rw-r--r--  2.0 unx     1398 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/ndarray_wrapper.py
 -rw-r--r--  2.0 unx     1809 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/sparce_array_wrapper.py
 -rw-r--r--  2.0 unx     4156 b- defN 80-Jan-01 00:00 siml/siml_variables/tensor_variables/tensor_variables.py
--rw-r--r--  2.0 unx    13021 b- defN 80-Jan-01 00:00 siml/study.py
--rw-r--r--  2.0 unx    36269 b- defN 80-Jan-01 00:00 siml/trainer.py
+-rw-r--r--  2.0 unx    12967 b- defN 80-Jan-01 00:00 siml/study.py
+-rw-r--r--  2.0 unx    33627 b- defN 80-Jan-01 00:00 siml/trainer.py
 -rw-r--r--  2.0 unx      211 b- defN 80-Jan-01 00:00 siml/update_functions/__init__.py
 -rw-r--r--  2.0 unx     1774 b- defN 80-Jan-01 00:00 siml/update_functions/element_batch_update.py
 -rw-r--r--  2.0 unx     3623 b- defN 80-Jan-01 00:00 siml/update_functions/pseudo_batch_update.py
 -rw-r--r--  2.0 unx     2702 b- defN 80-Jan-01 00:00 siml/update_functions/standard_update.py
 -rw-r--r--  2.0 unx      429 b- defN 80-Jan-01 00:00 siml/update_functions/update_interface.py
 -rw-r--r--  2.0 unx    23027 b- defN 80-Jan-01 00:00 siml/util.py
 -rw-r--r--  2.0 unx       37 b- defN 80-Jan-01 00:00 siml/utils/__init__.py
 -rw-r--r--  2.0 unx     7682 b- defN 80-Jan-01 00:00 siml/utils/fem_data_utils.py
--rw-r--r--  2.0 unx    11431 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202306221046.dist-info/LICENSE
--rw-r--r--  2.0 unx     1638 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202306221046.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202306221046.dist-info/WHEEL
--rw-r--r--  2.0 unx      388 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202306221046.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    12580 b- defN 16-Jan-01 00:00 pysiml-0.2.9.dev202306221046.dist-info/RECORD
-138 files, 600479 bytes uncompressed, 150144 bytes compressed:  75.0%
+-rw-r--r--  2.0 unx     1247 b- defN 80-Jan-01 00:00 siml/utils/timer.py
+-rw-r--r--  2.0 unx    11431 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202306240932.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1638 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202306240932.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202306240932.dist-info/WHEEL
+-rw-r--r--  2.0 unx      388 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202306240932.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    12969 b- defN 16-Jan-01 00:00 pysiml-0.2.9.dev202306240932.dist-info/RECORD
+142 files, 610500 bytes uncompressed, 152540 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -342,14 +342,23 @@
 
 Filename: siml/services/training/__init__.py
 Comment: 
 
 Filename: siml/services/training/inner_settings.py
 Comment: 
 
+Filename: siml/services/training/logging_items/__init__.py
+Comment: 
+
+Filename: siml/services/training/logging_items/logging_items.py
+Comment: 
+
+Filename: siml/services/training/training_logger.py
+Comment: 
+
 Filename: siml/setting.py
 Comment: 
 
 Filename: siml/siml_variables/__init__.py
 Comment: 
 
 Filename: siml/siml_variables/array_variables/__init__.py
@@ -393,23 +402,26 @@
 
 Filename: siml/utils/__init__.py
 Comment: 
 
 Filename: siml/utils/fem_data_utils.py
 Comment: 
 
-Filename: pysiml-0.2.9.dev202306221046.dist-info/LICENSE
+Filename: siml/utils/timer.py
+Comment: 
+
+Filename: pysiml-0.2.9.dev202306240932.dist-info/LICENSE
 Comment: 
 
-Filename: pysiml-0.2.9.dev202306221046.dist-info/METADATA
+Filename: pysiml-0.2.9.dev202306240932.dist-info/METADATA
 Comment: 
 
-Filename: pysiml-0.2.9.dev202306221046.dist-info/WHEEL
+Filename: pysiml-0.2.9.dev202306240932.dist-info/WHEEL
 Comment: 
 
-Filename: pysiml-0.2.9.dev202306221046.dist-info/entry_points.txt
+Filename: pysiml-0.2.9.dev202306240932.dist-info/entry_points.txt
 Comment: 
 
-Filename: pysiml-0.2.9.dev202306221046.dist-info/RECORD
+Filename: pysiml-0.2.9.dev202306240932.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyproject.toml

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysiml"
-version = "0.2.9.dev202306221046"
+version = "0.2.9.dev202306240932"
 description = "SiML - a Simulation ML library"
 license = "Apache-2.0"
 authors = ["RICOS Co. Ltd."]
 readme = "README.md"
 repository = "https://github.com/ricosjp/pysiml"
 documentation = "https://ricosjp.github.io/pysiml/"
 packages = [
```

## siml/services/training/__init__.py

```diff
@@ -1 +1,5 @@
+# flake8: noqa
+
 from .inner_settings import InnerTrainingSetting  # NOQA
+from .training_logger import (LogRecordItems, SimlTrainingConsoleLogger,
+                              SimlTrainingFileLogger)
```

## siml/services/training/inner_settings.py

```diff
@@ -16,14 +16,23 @@
     class Config:
         arbitrary_types_allowed = True
 
     @property
     def trainer_setting(self) -> TrainerSetting:
         return self.main_settings.trainer
 
+    @property
+    def log_file_path(self):
+        return self.trainer_setting.output_directory / 'log.csv'
+
+    @property
+    def loss_figure_path(self):
+        return self.trainer_setting.output_directory \
+            / f"plot.{self.trainer_setting.figure_format}"
+
     def __post_init_post_parse__(self):
         self._check_restart_and_pretrain()
         if self.trainer_setting.restart_directory is not None:
             self._load_restart_settings()
 
     def _check_restart_and_pretrain(self):
         if self.trainer_setting.restart_directory is not None \
```

## siml/study.py

```diff
@@ -73,15 +73,14 @@
             'test_loss': nones,
             'status': statuses,
         })
         data_frame.to_csv(self.log_file_path, index=False, header=True)
 
     def initialize_study_setting(self):
         template_trainer = trainer.Trainer(self.original_setting)
-        template_trainer.prepare_training(draw=False)
         total_data_directories = np.unique(np.concatenate([
             template_trainer.train_loader.dataset.data_directories,
             template_trainer.validation_loader.dataset.data_directories]))
 
         update_dict = {
             'data': {
                 'train': total_data_directories,
```

## siml/trainer.py

```diff
@@ -1,36 +1,31 @@
 import enum
 import io
-import time
-from typing import Callable
 import random
+from typing import Callable
 
 import ignite
-import matplotlib.pyplot as plt
 import numpy as np
 import optuna
-import pandas as pd
 import torch
+import yaml
 from torch import Tensor
 from tqdm import tqdm
-import yaml
 
-from . import datasets
-from . import networks
-from . import setting
-from . import util
-
-from . import update_functions
-
-from siml.siml_variables import siml_tensor_variables
 from siml.loss_operations import LossCalculatorBuilder
-from siml.services.model_selector import ModelSelectorBuilder
-from siml.services.model_builder import ModelBuilder
 from siml.services.environment import ModelEnvironmentSetting
-from siml.services.training import InnerTrainingSetting
+from siml.services.model_builder import ModelBuilder
+from siml.services.model_selector import ModelSelectorBuilder
+from siml.services.training import (InnerTrainingSetting, LogRecordItems,
+                                    SimlTrainingConsoleLogger,
+                                    SimlTrainingFileLogger)
+from siml.siml_variables import siml_tensor_variables
+from siml.utils.timer import SimlStopWatch
+
+from . import datasets, setting, update_functions, util
 
 
 class Trainer:
 
     def __init__(self,
                  main_settings: setting.MainSetting,
                  *,
@@ -58,101 +53,85 @@
                 f"Unknown type for settings: {main_settings.__class__}")
         self.inference_mode = False
         self.user_loss_function_dic = user_loss_function_dic
 
         inner_setting = InnerTrainingSetting(main_settings=main_settings)
         # HACK: temporarly hack. Better to handle as a inner setting.
         self.setting = inner_setting.main_settings
+        overwrite_restart_mode = self._overwrite_restart_mode()
 
         self.optuna_trial = optuna_trial
         self._env_setting = self._create_model_env_setting()
-        return
+
+        self.prepare_training()
+        self._console_logger = SimlTrainingConsoleLogger(
+            display_margin=self.setting.trainer.display_mergin,
+            loss_keys=self.model.get_loss_keys()
+        )
+        self._file_logger = SimlTrainingFileLogger(
+            file_path=inner_setting.log_file_path,
+            loss_figure_path=inner_setting.loss_figure_path,
+            loss_keys=self.model.get_loss_keys(),
+            continue_mode=overwrite_restart_mode
+        )
+        time_offset = self._file_logger.read_offset_start_time()
+        self._stop_watch = SimlStopWatch(offset=time_offset)
 
     def _create_model_env_setting(self) -> ModelEnvironmentSetting:
         trainer_setting = self.setting.trainer
         _model_env = ModelEnvironmentSetting(
             gpu_id=trainer_setting.gpu_id,
             seed=trainer_setting.seed,
             data_parallel=trainer_setting.data_parallel,
             model_parallel=trainer_setting.model_parallel,
             time_series=trainer_setting.time_series
         )
         return _model_env
 
-    def train(self):
+    def train(self, draw_model: bool = True):
         """Perform training.
 
         Parameters
         ----------
         None
 
         Returns
         --------
         loss: float
             Loss value after training.
         """
 
         print(f"Output directory: {self.setting.trainer.output_directory}")
         overwrite_restart_mode = self._overwrite_restart_mode()
-        if not overwrite_restart_mode:
-            # When restart training, output directory already exists
-            self.setting.trainer.output_directory.mkdir(parents=True)
 
-        self.prepare_training()
+        self.setting.trainer.output_directory.mkdir(
+            parents=True, exist_ok=True
+        )
+        if self.setting.trainer.draw_network and draw_model:
+            self.model.draw(self.setting.trainer.output_directory)
 
         yaml_file_name = f"restart_settings_{util.date_string()}.yml" \
             if overwrite_restart_mode else "settings.yml"
         setting.write_yaml(
             self.setting,
             self.setting.trainer.output_directory / yaml_file_name,
             key=self.setting.trainer.model_key)
 
-        print(
-            self._display_mergin('epoch')
-            + self._display_mergin('train_loss')
-            + ''.join([
-                'train/' + self._display_mergin(k)
-                for k in self.model.get_loss_keys()])
-            + self._display_mergin('validation_loss')
-            + ''.join([
-                'validation/' + self._display_mergin(k)
-                for k in self.model.get_loss_keys()])
-            + self._display_mergin('elapsed_time'))
-        if not overwrite_restart_mode:
-            with open(self.log_file, 'w') as f:
-                f.write(
-                    'epoch, train_loss, '
-                    + ''.join([
-                        f"train/{k}, " for k in self.model.get_loss_keys()])
-                    + 'validation_loss, '
-                    + ''.join([
-                        f"validation/{k}, " for k in self.model.get_loss_keys()
-                    ])
-                    + 'elapsed_time\n')
-        self.start_time = time.time()
-        if not overwrite_restart_mode:
-            self.offset_start_time = 0
-        else:
-            df = pd.read_csv(
-                self.log_file,
-                header=0,
-                index_col=None,
-                skipinitialspace=True
-            )
-            self.offset_start_time = df.tail(1).loc[:, "elapsed_time"].item()
+        print(self._console_logger.output_header())
+        self._file_logger.write_header_if_needed()
+        self._stop_watch.start()
 
         self.pbar = self.create_pbar(
             len(self.train_loader) * self.setting.trainer.log_trigger_epoch)
 
         self.trainer.run(
             self.train_loader, max_epochs=self.setting.trainer.n_epoch)
         self.pbar.close()
 
-        df = pd.read_csv(
-            self.log_file, header=0, index_col=None, skipinitialspace=True)
+        df = self._file_logger.read_history()
         validation_loss = np.min(df['validation_loss'])
 
         return validation_loss
 
     def evaluate(self, evaluate_test=False, load_best_model=False):
         if load_best_model:
             self.setting.trainer.pretrain_directory \
@@ -176,32 +155,24 @@
 
         if self.setting.trainer.output_directory == \
                 self.setting.trainer.restart_directory:
             return True
 
         return False
 
-    def _display_mergin(self, input_string, reference_string=None):
-        if not reference_string:
-            reference_string = input_string
-        return input_string.ljust(
-            len(reference_string) + self.setting.trainer.display_mergin, ' ')
-
-    def prepare_training(self, draw=True):
+    def prepare_training(self):
         self._env_setting.set_seed()
 
         if len(self.setting.trainer.input_names) == 0:
             raise ValueError('No input_names fed')
         if len(self.setting.trainer.output_names) == 0:
             raise ValueError('No output_names fed')
 
         # Define model
         self.model = self._setup_model()
-        if self.setting.trainer.draw_network and draw:
-            self.model.draw(self.setting.trainer.output_directory)
 
         self.element_wise = self.setting.trainer.determine_element_wise()
         self.loss = LossCalculatorBuilder.create(
             trainer_setting=self.setting.trainer,
             user_loss_function_dic=self.user_loss_function_dic
         )
 
@@ -374,18 +345,14 @@
         @self.evaluator.on(
             ignite.engine.Events.ITERATION_COMPLETED(every=evaluator_tick))
         def log_evaluation(engine):
             self.evaluation_pbar.desc = self.evaluator_desc
             self.evaluation_pbar.update(evaluator_tick)
             return
 
-        self.log_file = self.setting.trainer.output_directory / 'log.csv'
-        self.plot_file = self.setting.trainer.output_directory \
-            / f"plot.{self.setting.trainer.figure_format}"
-
         @self.trainer.on(
             ignite.engine.Events.EPOCH_COMPLETED(
                 every=self.setting.trainer.log_trigger_epoch))
         def log_training_results(engine):
             self.pbar.close()
 
             self.evaluation_pbar = tqdm(
@@ -405,71 +372,39 @@
                     k: v for k, v in self.evaluator.state.metrics.items()
                     if k != 'loss'}
             else:
                 validation_loss = np.nan
                 validation_other_losses = {}
             self.evaluation_pbar.close()
 
-            elapsed_time = (time.time() - self.start_time) \
-                + self.offset_start_time
+            log_record = LogRecordItems(
+                epoch=engine.state.epoch,
+                train_loss=train_loss,
+                train_other_losses=train_other_losses,
+                validation_loss=validation_loss,
+                validation_other_losses=validation_other_losses,
+                elapsed_time=self._stop_watch.watch()
+            )
 
             # Print log
-            tqdm.write(
-                self._display_mergin(f"{engine.state.epoch}", 'epoch')
-                + self._display_mergin(f"{train_loss:.5e}", 'train_loss')
-                + ''.join([
-                    self._display_mergin(f"{v:.5e}", 'train/' + k)
-                    for k, v in train_other_losses.items()])
-                + self._display_mergin(
-                    f"{validation_loss:.5e}", 'validation_loss')
-                + ''.join([
-                    self._display_mergin(f"{v:.5e}", 'validation/' + k)
-                    for k, v in validation_other_losses.items()])
-                + self._display_mergin(f"{elapsed_time:.2f}", 'elapsed_time'))
+            tqdm.write(self._console_logger.output(log_record))
 
             self.pbar = self.create_pbar(
                 len(self.train_loader)
                 * self.setting.trainer.log_trigger_epoch)
             self.pbar.n = self.pbar.last_print_n = 0
 
             # Save checkpoint
             self.save_model(engine, validation_loss)
 
             # Write log
-            with open(self.log_file, 'a') as f:
-                f.write(
-                    f"{engine.state.epoch}, {train_loss:.5e}, "
-                    + ''.join([
-                        f"{v:.5e}, " for v in train_other_losses.values()])
-                    + f"{validation_loss:.5e}, "
-                    + ''.join([
-                        f"{v:.5e}, " for v
-                        in validation_other_losses.values()])
-                    + f"{elapsed_time:.2f}\n")
+            self._file_logger.write(log_record)
 
             # Plot
-            fig = plt.figure(figsize=(16 / 2, 9 / 2))
-            df = pd.read_csv(
-                self.log_file, header=0, index_col=None, skipinitialspace=True)
-            plt.plot(df['epoch'], df['train_loss'], label='train loss')
-            plt.plot(
-                df['epoch'], df['validation_loss'], label='validation loss')
-            for k in self.model.get_loss_keys():
-                plt.plot(df['epoch'], df[f"train/{k}"], label=f"train/{k}")
-            for k in self.model.get_loss_keys():
-                plt.plot(
-                    df['epoch'], df[f"validation/{k}"],
-                    label=f"validation/{k}")
-            plt.xlabel('epoch')
-            plt.ylabel('loss')
-            plt.yscale('log')
-            plt.legend()
-            plt.savefig(self.plot_file)
-            plt.close(fig)
-
+            self._file_logger.save_figure()
             return
 
         # Add early stopping
         class StopTriggerEvents(enum.Enum):
             EVALUATED = 'evaluated'
 
         @self.trainer.on(
```

## Comparing `pysiml-0.2.9.dev202306221046.dist-info/LICENSE` & `pysiml-0.2.9.dev202306240932.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pysiml-0.2.9.dev202306221046.dist-info/METADATA` & `pysiml-0.2.9.dev202306240932.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysiml
-Version: 0.2.9.dev202306221046
+Version: 0.2.9.dev202306240932
 Summary: SiML - a Simulation ML library
 Home-page: https://github.com/ricosjp/pysiml
 License: Apache-2.0
 Author: RICOS Co. Ltd.
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pysiml-0.2.9.dev202306221046.dist-info/RECORD` & `pysiml-0.2.9.dev202306240932.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pyproject.toml,sha256=aBmyKDRN80DodfitTBgxIwvI1QCZx8ptCROyiJvH9MU,1520
+pyproject.toml,sha256=xIHnGyltsgV3aHCUhX4PZAbMXfkLbAjcefVG_5eQhAg,1520
 siml/__init__.py,sha256=mC61oSLHO5F6zXHhOrzH51R-vkH0mL4MShhSBiRRe6s,638
 siml/__main__/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 siml/__main__/convert_interim_data.py,sha256=jA6GD7BlnsEjARcln3UBwXlFj64BeFALAmgD1ohBkqo,900
 siml/__main__/convert_raw_data.py,sha256=VNVOyx9lChopF2Q-9OXtN_-MtfBsyjS_JvFwCjdkv0c,1400
 siml/__main__/optimize.py,sha256=6HALn60Mxh4GUiPbSXjvrdpkoQ4NgYSzCHCBRbli4W0,1742
 siml/__main__/plot_losses.py,sha256=0uMsoPN-xR0JhPg0WzSQL5GbD80ovuFO12eVpc0x6Xc,8663
 siml/__main__/prepare_preprocess_converters.py,sha256=w_rzic--RUyISagQOJw_5-oEkOFEKXUN7G1TkTOxd8g,927
@@ -108,31 +108,35 @@
 siml/services/inference/postprocessing/post_fem_data.py,sha256=8apB2-cUyssum_6BOx9uVUhmNNvBjoXRnSWn4w4aJ-A,5603
 siml/services/inference/postprocessing/postprocessor.py,sha256=lnHod9-Wa87QLb4ZMq7cOOeRxFjKQYq4NeuPaTHD6Nk,4979
 siml/services/inference/postprocessing/save_processor.py,sha256=oJVxJJplyH8dLiYIpG1GJWD_Y58RwrnAwlqNt_dLuA0,7052
 siml/services/inference/record_object.py,sha256=9cSmtHyNuVwtQbAxkMoUOhCg7TQ6fgyFFwWqyBJ3Gw4,1082
 siml/services/model_builder.py,sha256=ybQorVluaFo-7gBFftUp4h5GaKCUhUDYfqG2PLl6o8M,2574
 siml/services/model_selector.py,sha256=q2oXdJcujaOa6Y_HFHZ1emxkNaRN00BAGi_kc0zXmvE,4978
 siml/services/path_rules.py,sha256=fPNdpXcf8GZtI6ZfMrEkKcdo0JkxxPNmnvohbY1evI8,7124
-siml/services/training/__init__.py,sha256=AbzAnWrtCsQ-ORTjrOP27OmTxsmXhWKEldP8CPCVwe0,57
-siml/services/training/inner_settings.py,sha256=pTkhRuZptV2sFw3jHnsIkJpm8hI1Hy9bp_tZDh6aTso,2383
+siml/services/training/__init__.py,sha256=nuxgfAYieJxucFOKJXwdICJuyvUhHdKjup0okMU8ULk,200
+siml/services/training/inner_settings.py,sha256=uSzxV3ftVhefUt1jjsKR_R5lkB5HzQ2VuOboakZZYuk,2653
+siml/services/training/logging_items/__init__.py,sha256=1Njqc0eCpuwo6mzxDv2iRhhvslHG3yfH3oHnCgc3FMc,775
+siml/services/training/logging_items/logging_items.py,sha256=hQMvAImDg2YpHFY8qIj72ICZRW6pgNZ4qdZi4hll2kE,4198
+siml/services/training/training_logger.py,sha256=SuSwfUy5klWCelKkWh39lTA2PNoAFGS0eJNTLNGiWQs,5695
 siml/setting.py,sha256=0DQ9_jJ7PCwgLwghIwrJwi0xtVfGr1YcxFQtw9Gt59U,50394
 siml/siml_variables/__init__.py,sha256=Nt8iJ0yLPBJpg1o6K_b5Qr-go5iurvC9FnHxI4lD6eg,163
 siml/siml_variables/array_variables/__init__.py,sha256=Y2syJXtd98L-Z3kRTCOlCEVZffc-xBbuMIS1uv3ekQU,594
 siml/siml_variables/array_variables/interface_wrapper.py,sha256=Wi0GcuEexwx6sqTqVcBCtWo2K7kw_LQN6LOdoXnNFYw,1573
 siml/siml_variables/array_variables/ndarray_wrapper.py,sha256=oNOfbQu_5twQZq9AM_NEWcbswnCzASAEGzCPpUXcujM,1398
 siml/siml_variables/array_variables/sparce_array_wrapper.py,sha256=yyWwfuKHn686-aQemDMIgcig4K9a6XC-HCTYETJS0O8,1809
 siml/siml_variables/tensor_variables/tensor_variables.py,sha256=Nh3W1ft6FbGID7cp88lw2VyVVxTkrx_1ovI_I2DFSX0,4156
-siml/study.py,sha256=VsiEuAiwcC0a1voORjic9RcZcnPVJiBowV-mobS6tAQ,13021
-siml/trainer.py,sha256=GuS6q7M1hNouTNx_ZzBPCfs_JbFfnwqa-4RmJN-mN0Y,36269
+siml/study.py,sha256=Sc8DBdT3ni3mcHICtURUmjDslCkSf7T6lCqADogoRs4,12967
+siml/trainer.py,sha256=DRORw3ji0m_XJWwuVtTuAfUtHfJ0TYW1kDgAkGtDlAI,33627
 siml/update_functions/__init__.py,sha256=fQY19xMEhZv7k6flZPBmhIgLl3uHuBWkay-YCFfaY64,211
 siml/update_functions/element_batch_update.py,sha256=93_L9jl4D9lFQXmEX1Lo8l4n3rDf1wdZljPJIQd9rUs,1774
 siml/update_functions/pseudo_batch_update.py,sha256=7PS6SEXOMB57uaJQhZ8VrtEiIkDF59JE1c6yyrKL3YY,3623
 siml/update_functions/standard_update.py,sha256=jIgeQ_c9R1dgcxDQWzx-w5TkJ7naDKmNi_WUFFchxc4,2702
 siml/update_functions/update_interface.py,sha256=O1fGrE21iXckz7NTOTDNlyQ4rll1SQDehdc_Kk5we0Q,429
 siml/util.py,sha256=AzvnYN1svE28ioHGPgMjkpiK35hCA5m5qwFEDb3agHA,23027
 siml/utils/__init__.py,sha256=DVdxWEBXfapWAWNM0jUouKJzru4RyK2ru2QheBmrm_s,37
 siml/utils/fem_data_utils.py,sha256=LDB_MxYPg_WELl6D_az9ikMZxAF5Ml5qKUXR2CnuxvE,7682
-pysiml-0.2.9.dev202306221046.dist-info/LICENSE,sha256=Ok4O8jxCIpLhGZjTNzgBW8V8xITF_SUVEp1juLijZpA,11431
-pysiml-0.2.9.dev202306221046.dist-info/METADATA,sha256=0g7_IM96ckM4t6bB-BqDBNih2nPQftu1893xsf5kX_I,1638
-pysiml-0.2.9.dev202306221046.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-pysiml-0.2.9.dev202306221046.dist-info/entry_points.txt,sha256=zXU0Gd56XeUfgaeG-CGXcYaTpORSU6kVeQ_vVvjIFPs,388
-pysiml-0.2.9.dev202306221046.dist-info/RECORD,,
+siml/utils/timer.py,sha256=DEDtrmFpFqiGRykErkLMnwZ3tWUsOsarubnN40kwb6I,1247
+pysiml-0.2.9.dev202306240932.dist-info/LICENSE,sha256=Ok4O8jxCIpLhGZjTNzgBW8V8xITF_SUVEp1juLijZpA,11431
+pysiml-0.2.9.dev202306240932.dist-info/METADATA,sha256=-JJIOYP5LQvNNxKgYHgfz9wEJFRpqU5o5snSd2C1WbE,1638
+pysiml-0.2.9.dev202306240932.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+pysiml-0.2.9.dev202306240932.dist-info/entry_points.txt,sha256=zXU0Gd56XeUfgaeG-CGXcYaTpORSU6kVeQ_vVvjIFPs,388
+pysiml-0.2.9.dev202306240932.dist-info/RECORD,,
```

