# Comparing `tmp/intel_xai-0.3.1.dev20230608-py3-none-any.whl.zip` & `tmp/intel_xai-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,36 +1,111 @@
-Zip file size: 46081 bytes, number of entries: 34
--rw-r--r--  2.0 unx     3318 b- defN 23-Jun-09 23:26 explainer/README.md
--rw-r--r--  2.0 unx      709 b- defN 23-Jun-09 23:26 explainer/version.py
--rw-r--r--  2.0 unx     1057 b- defN 23-Jun-09 23:26 explainer/attributions/README.md
--rw-r--r--  2.0 unx      703 b- defN 23-Jun-09 23:26 explainer/attributions/__init__.py
--rw-r--r--  2.0 unx    14915 b- defN 23-Jun-09 23:26 explainer/attributions/attributions.py
--rw-r--r--  2.0 unx     2627 b- defN 23-Jun-09 17:45 explainer/attributions/attributions_info.py
--rw-r--r--  2.0 unx     5269 b- defN 23-Jun-09 23:25 explainer/attributions/plots.py
--rw-r--r--  2.0 unx    14839 b- defN 23-Jun-09 16:58 explainer/attributions/pt_attributions.py
--rw-r--r--  2.0 unx    14620 b- defN 23-Jun-09 18:02 explainer/attributions/widgets.py
--rw-r--r--  2.0 unx      876 b- defN 23-Jun-09 23:26 explainer/cam/README.md
--rw-r--r--  2.0 unx      694 b- defN 23-Jun-09 23:26 explainer/cam/__init__.py
--rw-r--r--  2.0 unx     6072 b- defN 23-Jun-09 23:26 explainer/cam/cam.py
--rw-r--r--  2.0 unx     9257 b- defN 23-Jun-09 16:58 explainer/cam/pt_cam.py
--rw-r--r--  2.0 unx     4813 b- defN 23-Jun-09 16:58 explainer/cam/tf_cam.py
--rw-r--r--  2.0 unx      995 b- defN 23-Jun-09 23:26 explainer/metrics/README.md
--rw-r--r--  2.0 unx      698 b- defN 23-Jun-09 16:58 explainer/metrics/__init__.py
--rw-r--r--  2.0 unx    11746 b- defN 23-Jun-09 23:26 explainer/metrics/metrics.py
--rw-r--r--  2.0 unx      674 b- defN 23-Jun-09 16:58 explainer/tests/__init__.py
--rw-r--r--  2.0 unx     2772 b- defN 23-Jun-09 23:26 explainer/tests/conftest.py
--rw-r--r--  2.0 unx      672 b- defN 23-Jun-09 16:58 explainer/tests/pytest.ini
--rw-r--r--  2.0 unx     2134 b- defN 23-Jun-09 23:26 explainer/tests/test_attributions.py
--rw-r--r--  2.0 unx     1367 b- defN 23-Jun-09 23:26 explainer/tests/test_cam.py
--rw-r--r--  2.0 unx     3196 b- defN 23-Jun-09 23:26 explainer/tests/test_metrics.py
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-09 16:58 explainer/tests/test_requirements.txt
--rw-r--r--  2.0 unx      768 b- defN 23-Jun-09 16:58 explainer/utils/types.py
--rw-r--r--  2.0 unx      673 b- defN 23-Jun-09 16:58 explainer/utils/graphics/__init__.py
--rw-r--r--  2.0 unx     2380 b- defN 23-Jun-09 16:58 explainer/utils/graphics/info.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 16:58 explainer/utils/model/__init__.py
--rw-r--r--  2.0 unx      938 b- defN 23-Jun-09 16:58 explainer/utils/model/model_framework.py
--rw-r--r--  2.0 unx    11347 b- defN 23-Jun-09 23:38 intel_xai-0.3.1.dev20230608.dist-info/LICENSE
--rw-r--r--  2.0 unx     7009 b- defN 23-Jun-09 23:38 intel_xai-0.3.1.dev20230608.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 23:38 intel_xai-0.3.1.dev20230608.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-09 23:38 intel_xai-0.3.1.dev20230608.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2963 b- defN 23-Jun-09 23:38 intel_xai-0.3.1.dev20230608.dist-info/RECORD
-34 files, 130219 bytes uncompressed, 41287 bytes compressed:  68.3%
+Zip file size: 378504 bytes, number of entries: 109
+-rw-r--r--  2.0 unx     3423 b- defN 23-Jun-23 22:32 explainer/README.md
+-rw-r--r--  2.0 unx      697 b- defN 23-Jun-23 22:32 explainer/version.py
+-rw-r--r--  2.0 unx      192 b- defN 23-Jun-23 22:33 explainer/__pycache__/version.cpython-39.pyc
+-rw-r--r--  2.0 unx     1045 b- defN 23-Jun-23 22:32 explainer/attributions/README.md
+-rw-r--r--  2.0 unx      734 b- defN 23-Jun-23 22:32 explainer/attributions/__init__.py
+-rw-r--r--  2.0 unx    18931 b- defN 23-Jun-23 22:32 explainer/attributions/attributions.py
+-rw-r--r--  2.0 unx     2627 b- defN 23-Jun-23 22:32 explainer/attributions/attributions_info.py
+-rw-r--r--  2.0 unx     5269 b- defN 23-Jun-23 22:32 explainer/attributions/plots.py
+-rw-r--r--  2.0 unx    14839 b- defN 23-Jun-23 22:32 explainer/attributions/pt_attributions.py
+-rw-r--r--  2.0 unx    14620 b- defN 23-Jun-23 22:32 explainer/attributions/widgets.py
+-rw-r--r--  2.0 unx      241 b- defN 23-Jun-23 22:33 explainer/attributions/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--  2.0 unx    18739 b- defN 23-Jun-23 22:33 explainer/attributions/__pycache__/attributions.cpython-39.pyc
+-rw-r--r--  2.0 unx     1842 b- defN 23-Jun-23 22:33 explainer/attributions/__pycache__/attributions_info.cpython-39.pyc
+-rw-r--r--  2.0 unx    14288 b- defN 23-Jun-23 22:33 explainer/attributions/__pycache__/pt_attributions.cpython-39.pyc
+-rw-r--r--  2.0 unx     1145 b- defN 23-Jun-23 22:32 explainer/cam/README.md
+-rw-r--r--  2.0 unx      803 b- defN 23-Jun-23 22:32 explainer/cam/__init__.py
+-rw-r--r--  2.0 unx     1302 b- defN 23-Jun-23 22:32 explainer/cam/cam.py
+-rw-r--r--  2.0 unx     9602 b- defN 23-Jun-23 22:32 explainer/cam/pt_cam.py
+-rw-r--r--  2.0 unx     4954 b- defN 23-Jun-23 22:32 explainer/cam/tf_cam.py
+-rw-r--r--  2.0 unx      369 b- defN 23-Jun-23 22:33 explainer/cam/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--  2.0 unx      973 b- defN 23-Jun-23 22:33 explainer/cam/__pycache__/cam.cpython-39.pyc
+-rw-r--r--  2.0 unx     7626 b- defN 23-Jun-23 22:33 explainer/cam/__pycache__/pt_cam.cpython-39.pyc
+-rw-r--r--  2.0 unx     3867 b- defN 23-Jun-23 22:33 explainer/cam/__pycache__/tf_cam.cpython-39.pyc
+-rw-r--r--  2.0 unx      983 b- defN 23-Jun-23 22:32 explainer/metrics/README.md
+-rw-r--r--  2.0 unx      698 b- defN 23-Jun-23 22:32 explainer/metrics/__init__.py
+-rw-r--r--  2.0 unx    13424 b- defN 23-Jun-23 22:32 explainer/metrics/metrics.py
+-rw-r--r--  2.0 unx      204 b- defN 23-Jun-23 22:33 explainer/metrics/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--  2.0 unx    13707 b- defN 23-Jun-23 22:33 explainer/metrics/__pycache__/metrics.cpython-39.pyc
+-rw-r--r--  2.0 unx      674 b- defN 23-Jun-23 22:32 explainer/tests/__init__.py
+-rw-r--r--  2.0 unx     6861 b- defN 23-Jun-23 22:32 explainer/tests/conftest.py
+-rw-r--r--  2.0 unx      672 b- defN 23-Jun-23 22:32 explainer/tests/pytest.ini
+-rw-r--r--  2.0 unx     7631 b- defN 23-Jun-23 22:32 explainer/tests/test_attributions.py
+-rw-r--r--  2.0 unx     2634 b- defN 23-Jun-23 22:32 explainer/tests/test_cam.py
+-rw-r--r--  2.0 unx     2875 b- defN 23-Jun-23 22:32 explainer/tests/test_metrics.py
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-23 22:32 explainer/tests/test_requirements.txt
+-rw-r--r--  2.0 unx      768 b- defN 23-Jun-23 22:32 explainer/utils/types.py
+-rw-r--r--  2.0 unx      286 b- defN 23-Jun-23 22:33 explainer/utils/__pycache__/types.cpython-39.pyc
+-rw-r--r--  2.0 unx      673 b- defN 23-Jun-23 22:32 explainer/utils/graphics/__init__.py
+-rw-r--r--  2.0 unx     2380 b- defN 23-Jun-23 22:32 explainer/utils/graphics/info.py
+-rw-r--r--  2.0 unx      187 b- defN 23-Jun-23 22:33 explainer/utils/graphics/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--  2.0 unx     2520 b- defN 23-Jun-23 22:33 explainer/utils/graphics/__pycache__/info.cpython-39.pyc
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-23 22:32 explainer/utils/model/__init__.py
+-rw-r--r--  2.0 unx      938 b- defN 23-Jun-23 22:32 explainer/utils/model/model_framework.py
+-rw-r--r--  2.0 unx      184 b- defN 23-Jun-23 22:33 explainer/utils/model/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--  2.0 unx     1285 b- defN 23-Jun-23 22:33 explainer/utils/model/__pycache__/model_framework.cpython-39.pyc
+-rw-r--r--  2.0 unx     9393 b- defN 23-Jun-23 22:32 model_card_gen/README.md
+-rw-r--r--  2.0 unx      674 b- defN 23-Jun-23 22:32 model_card_gen/__init__.py
+-rw-r--r--  2.0 unx     3423 b- defN 23-Jun-23 22:32 model_card_gen/base_model_card_field.py
+-rw-r--r--  2.0 unx    20799 b- defN 23-Jun-23 22:32 model_card_gen/model_card.py
+-rw-r--r--  2.0 unx    16503 b- defN 23-Jun-23 22:32 model_card_gen/model_card_gen.py
+-rw-r--r--  2.0 unx     3344 b- defN 23-Jun-23 22:32 model_card_gen/validation.py
+-rw-r--r--  2.0 unx      697 b- defN 23-Jun-23 22:32 model_card_gen/version.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Jun-23 22:33 model_card_gen/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--  2.0 unx     2867 b- defN 23-Jun-23 22:33 model_card_gen/__pycache__/base_model_card_field.cpython-39.pyc
+-rw-r--r--  2.0 unx    20176 b- defN 23-Jun-23 22:33 model_card_gen/__pycache__/model_card.cpython-39.pyc
+-rw-r--r--  2.0 unx    13742 b- defN 23-Jun-23 22:33 model_card_gen/__pycache__/model_card_gen.cpython-39.pyc
+-rw-r--r--  2.0 unx     2738 b- defN 23-Jun-23 22:33 model_card_gen/__pycache__/validation.cpython-39.pyc
+-rw-r--r--  2.0 unx      848 b- defN 23-Jun-23 22:32 model_card_gen/analyze/__init__.py
+-rw-r--r--  2.0 unx     2764 b- defN 23-Jun-23 22:32 model_card_gen/analyze/analyzer.py
+-rw-r--r--  2.0 unx     3610 b- defN 23-Jun-23 22:32 model_card_gen/analyze/analyzer_factory.py
+-rw-r--r--  2.0 unx     2633 b- defN 23-Jun-23 22:32 model_card_gen/analyze/pandas_analyzer.py
+-rw-r--r--  2.0 unx     3037 b- defN 23-Jun-23 22:32 model_card_gen/analyze/tf_analyzer.py
+-rw-r--r--  2.0 unx     4121 b- defN 23-Jun-23 22:32 model_card_gen/analyze/torch_analyzer.py
+-rw-r--r--  2.0 unx      407 b- defN 23-Jun-23 22:33 model_card_gen/analyze/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--  2.0 unx     2477 b- defN 23-Jun-23 22:33 model_card_gen/analyze/__pycache__/analyzer.cpython-39.pyc
+-rw-r--r--  2.0 unx     3604 b- defN 23-Jun-23 22:33 model_card_gen/analyze/__pycache__/analyzer_factory.cpython-39.pyc
+-rw-r--r--  2.0 unx     2377 b- defN 23-Jun-23 22:33 model_card_gen/analyze/__pycache__/pandas_analyzer.cpython-39.pyc
+-rw-r--r--  2.0 unx     2607 b- defN 23-Jun-23 22:33 model_card_gen/analyze/__pycache__/tf_analyzer.cpython-39.pyc
+-rw-r--r--  2.0 unx     3705 b- defN 23-Jun-23 22:33 model_card_gen/analyze/__pycache__/torch_analyzer.cpython-39.pyc
+-rw-r--r--  2.0 unx      795 b- defN 23-Jun-23 22:32 model_card_gen/datasets/__init__.py
+-rw-r--r--  2.0 unx     1320 b- defN 23-Jun-23 22:32 model_card_gen/datasets/datasets.py
+-rw-r--r--  2.0 unx     1092 b- defN 23-Jun-23 22:32 model_card_gen/datasets/tf_datasets.py
+-rw-r--r--  2.0 unx     4180 b- defN 23-Jun-23 22:32 model_card_gen/datasets/torch_datasets.py
+-rw-r--r--  2.0 unx      336 b- defN 23-Jun-23 22:33 model_card_gen/datasets/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--  2.0 unx     1178 b- defN 23-Jun-23 22:33 model_card_gen/datasets/__pycache__/datasets.cpython-39.pyc
+-rw-r--r--  2.0 unx      923 b- defN 23-Jun-23 22:33 model_card_gen/datasets/__pycache__/tf_datasets.cpython-39.pyc
+-rw-r--r--  2.0 unx     4580 b- defN 23-Jun-23 22:33 model_card_gen/datasets/__pycache__/torch_datasets.cpython-39.pyc
+-rw-r--r--  2.0 unx      674 b- defN 23-Jun-23 22:32 model_card_gen/docs/examples/__init__.py
+-rw-r--r--  2.0 unx   510942 b- defN 23-Jun-23 22:32 model_card_gen/docs/examples/html/compas_model_card.html
+-rw-r--r--  2.0 unx   520886 b- defN 23-Jun-23 22:32 model_card_gen/docs/examples/json/model_card_compas.json
+-rw-r--r--  2.0 unx     4964 b- defN 23-Jun-23 22:32 model_card_gen/docs/examples/json/model_card_example.json
+-rw-r--r--  2.0 unx      674 b- defN 23-Jun-23 22:32 model_card_gen/graphics/__init__.py
+-rw-r--r--  2.0 unx     5284 b- defN 23-Jun-23 22:32 model_card_gen/graphics/add_graphics.py
+-rw-r--r--  2.0 unx    11094 b- defN 23-Jun-23 22:32 model_card_gen/graphics/plotly_graphics.py
+-rw-r--r--  2.0 unx     3607 b- defN 23-Jun-23 22:32 model_card_gen/graphics/plotly_utils.py
+-rw-r--r--  2.0 unx      186 b- defN 23-Jun-23 22:33 model_card_gen/graphics/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--  2.0 unx     4940 b- defN 23-Jun-23 22:33 model_card_gen/graphics/__pycache__/add_graphics.cpython-39.pyc
+-rw-r--r--  2.0 unx     9770 b- defN 23-Jun-23 22:33 model_card_gen/graphics/__pycache__/plotly_graphics.cpython-39.pyc
+-rw-r--r--  2.0 unx     2837 b- defN 23-Jun-23 22:33 model_card_gen/graphics/__pycache__/plotly_utils.cpython-39.pyc
+-rw-r--r--  2.0 unx    10850 b- defN 23-Jun-23 22:32 model_card_gen/schema/v0.0.1/model_card.schema.json
+-rw-r--r--  2.0 unx     5966 b- defN 23-Jun-23 22:32 model_card_gen/template/html/default_template.html.jinja
+-rw-r--r--  2.0 unx      581 b- defN 23-Jun-23 22:32 model_card_gen/template/html/js/plotly_js_header.html.jinja
+-rw-r--r--  2.0 unx     3468 b- defN 23-Jun-23 22:32 model_card_gen/template/html/macros/default_macros.html.jinja
+-rw-r--r--  2.0 unx     1574 b- defN 23-Jun-23 22:32 model_card_gen/template/html/style/default_style.html.jinja
+-rw-r--r--  2.0 unx      674 b- defN 23-Jun-23 22:32 model_card_gen/tests/__init__.py
+-rw-r--r--  2.0 unx     2479 b- defN 23-Jun-23 22:32 model_card_gen/tests/test_end_to_end_tf.py
+-rw-r--r--  2.0 unx     2602 b- defN 23-Jun-23 22:32 model_card_gen/tests/test_end_to_end_torch.py
+-rw-r--r--  2.0 unx     2463 b- defN 23-Jun-23 22:32 model_card_gen/tests/test_model_card.py
+-rw-r--r--  2.0 unx     3996 b- defN 23-Jun-23 22:32 model_card_gen/tests/tf_model.py
+-rw-r--r--  2.0 unx     3294 b- defN 23-Jun-23 22:32 model_card_gen/tests/torch_model.py
+-rw-r--r--  2.0 unx      674 b- defN 23-Jun-23 22:32 model_card_gen/utils/__init__.py
+-rw-r--r--  2.0 unx      875 b- defN 23-Jun-23 22:32 model_card_gen/utils/types.py
+-rw-r--r--  2.0 unx      183 b- defN 23-Jun-23 22:33 model_card_gen/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--  2.0 unx      390 b- defN 23-Jun-23 22:33 model_card_gen/utils/__pycache__/types.cpython-39.pyc
+-rw-r--r--  2.0 unx    11347 b- defN 23-Jun-23 23:17 intel_xai-0.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7573 b- defN 23-Jun-23 23:17 intel_xai-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 23:17 intel_xai-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       25 b- defN 23-Jun-23 23:17 intel_xai-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    10805 b- defN 23-Jun-23 23:17 intel_xai-0.5.0.dist-info/RECORD
+109 files, 1474624 bytes uncompressed, 360854 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: explainer/README.md
 Comment: 
 
 Filename: explainer/version.py
 Comment: 
 
+Filename: explainer/__pycache__/version.cpython-39.pyc
+Comment: 
+
 Filename: explainer/attributions/README.md
 Comment: 
 
 Filename: explainer/attributions/__init__.py
 Comment: 
 
 Filename: explainer/attributions/attributions.py
@@ -21,14 +24,26 @@
 
 Filename: explainer/attributions/pt_attributions.py
 Comment: 
 
 Filename: explainer/attributions/widgets.py
 Comment: 
 
+Filename: explainer/attributions/__pycache__/__init__.cpython-39.pyc
+Comment: 
+
+Filename: explainer/attributions/__pycache__/attributions.cpython-39.pyc
+Comment: 
+
+Filename: explainer/attributions/__pycache__/attributions_info.cpython-39.pyc
+Comment: 
+
+Filename: explainer/attributions/__pycache__/pt_attributions.cpython-39.pyc
+Comment: 
+
 Filename: explainer/cam/README.md
 Comment: 
 
 Filename: explainer/cam/__init__.py
 Comment: 
 
 Filename: explainer/cam/cam.py
@@ -36,23 +51,41 @@
 
 Filename: explainer/cam/pt_cam.py
 Comment: 
 
 Filename: explainer/cam/tf_cam.py
 Comment: 
 
+Filename: explainer/cam/__pycache__/__init__.cpython-39.pyc
+Comment: 
+
+Filename: explainer/cam/__pycache__/cam.cpython-39.pyc
+Comment: 
+
+Filename: explainer/cam/__pycache__/pt_cam.cpython-39.pyc
+Comment: 
+
+Filename: explainer/cam/__pycache__/tf_cam.cpython-39.pyc
+Comment: 
+
 Filename: explainer/metrics/README.md
 Comment: 
 
 Filename: explainer/metrics/__init__.py
 Comment: 
 
 Filename: explainer/metrics/metrics.py
 Comment: 
 
+Filename: explainer/metrics/__pycache__/__init__.cpython-39.pyc
+Comment: 
+
+Filename: explainer/metrics/__pycache__/metrics.cpython-39.pyc
+Comment: 
+
 Filename: explainer/tests/__init__.py
 Comment: 
 
 Filename: explainer/tests/conftest.py
 Comment: 
 
 Filename: explainer/tests/pytest.ini
@@ -69,35 +102,227 @@
 
 Filename: explainer/tests/test_requirements.txt
 Comment: 
 
 Filename: explainer/utils/types.py
 Comment: 
 
+Filename: explainer/utils/__pycache__/types.cpython-39.pyc
+Comment: 
+
 Filename: explainer/utils/graphics/__init__.py
 Comment: 
 
 Filename: explainer/utils/graphics/info.py
 Comment: 
 
+Filename: explainer/utils/graphics/__pycache__/__init__.cpython-39.pyc
+Comment: 
+
+Filename: explainer/utils/graphics/__pycache__/info.cpython-39.pyc
+Comment: 
+
 Filename: explainer/utils/model/__init__.py
 Comment: 
 
 Filename: explainer/utils/model/model_framework.py
 Comment: 
 
-Filename: intel_xai-0.3.1.dev20230608.dist-info/LICENSE
+Filename: explainer/utils/model/__pycache__/__init__.cpython-39.pyc
+Comment: 
+
+Filename: explainer/utils/model/__pycache__/model_framework.cpython-39.pyc
+Comment: 
+
+Filename: model_card_gen/README.md
+Comment: 
+
+Filename: model_card_gen/__init__.py
+Comment: 
+
+Filename: model_card_gen/base_model_card_field.py
+Comment: 
+
+Filename: model_card_gen/model_card.py
+Comment: 
+
+Filename: model_card_gen/model_card_gen.py
+Comment: 
+
+Filename: model_card_gen/validation.py
+Comment: 
+
+Filename: model_card_gen/version.py
+Comment: 
+
+Filename: model_card_gen/__pycache__/__init__.cpython-39.pyc
+Comment: 
+
+Filename: model_card_gen/__pycache__/base_model_card_field.cpython-39.pyc
+Comment: 
+
+Filename: model_card_gen/__pycache__/model_card.cpython-39.pyc
+Comment: 
+
+Filename: model_card_gen/__pycache__/model_card_gen.cpython-39.pyc
+Comment: 
+
+Filename: model_card_gen/__pycache__/validation.cpython-39.pyc
+Comment: 
+
+Filename: model_card_gen/analyze/__init__.py
+Comment: 
+
+Filename: model_card_gen/analyze/analyzer.py
+Comment: 
+
+Filename: model_card_gen/analyze/analyzer_factory.py
+Comment: 
+
+Filename: model_card_gen/analyze/pandas_analyzer.py
+Comment: 
+
+Filename: model_card_gen/analyze/tf_analyzer.py
+Comment: 
+
+Filename: model_card_gen/analyze/torch_analyzer.py
+Comment: 
+
+Filename: model_card_gen/analyze/__pycache__/__init__.cpython-39.pyc
+Comment: 
+
+Filename: model_card_gen/analyze/__pycache__/analyzer.cpython-39.pyc
+Comment: 
+
+Filename: model_card_gen/analyze/__pycache__/analyzer_factory.cpython-39.pyc
+Comment: 
+
+Filename: model_card_gen/analyze/__pycache__/pandas_analyzer.cpython-39.pyc
+Comment: 
+
+Filename: model_card_gen/analyze/__pycache__/tf_analyzer.cpython-39.pyc
+Comment: 
+
+Filename: model_card_gen/analyze/__pycache__/torch_analyzer.cpython-39.pyc
+Comment: 
+
+Filename: model_card_gen/datasets/__init__.py
+Comment: 
+
+Filename: model_card_gen/datasets/datasets.py
+Comment: 
+
+Filename: model_card_gen/datasets/tf_datasets.py
+Comment: 
+
+Filename: model_card_gen/datasets/torch_datasets.py
+Comment: 
+
+Filename: model_card_gen/datasets/__pycache__/__init__.cpython-39.pyc
+Comment: 
+
+Filename: model_card_gen/datasets/__pycache__/datasets.cpython-39.pyc
+Comment: 
+
+Filename: model_card_gen/datasets/__pycache__/tf_datasets.cpython-39.pyc
+Comment: 
+
+Filename: model_card_gen/datasets/__pycache__/torch_datasets.cpython-39.pyc
+Comment: 
+
+Filename: model_card_gen/docs/examples/__init__.py
+Comment: 
+
+Filename: model_card_gen/docs/examples/html/compas_model_card.html
+Comment: 
+
+Filename: model_card_gen/docs/examples/json/model_card_compas.json
+Comment: 
+
+Filename: model_card_gen/docs/examples/json/model_card_example.json
+Comment: 
+
+Filename: model_card_gen/graphics/__init__.py
+Comment: 
+
+Filename: model_card_gen/graphics/add_graphics.py
+Comment: 
+
+Filename: model_card_gen/graphics/plotly_graphics.py
+Comment: 
+
+Filename: model_card_gen/graphics/plotly_utils.py
+Comment: 
+
+Filename: model_card_gen/graphics/__pycache__/__init__.cpython-39.pyc
+Comment: 
+
+Filename: model_card_gen/graphics/__pycache__/add_graphics.cpython-39.pyc
+Comment: 
+
+Filename: model_card_gen/graphics/__pycache__/plotly_graphics.cpython-39.pyc
+Comment: 
+
+Filename: model_card_gen/graphics/__pycache__/plotly_utils.cpython-39.pyc
+Comment: 
+
+Filename: model_card_gen/schema/v0.0.1/model_card.schema.json
+Comment: 
+
+Filename: model_card_gen/template/html/default_template.html.jinja
+Comment: 
+
+Filename: model_card_gen/template/html/js/plotly_js_header.html.jinja
+Comment: 
+
+Filename: model_card_gen/template/html/macros/default_macros.html.jinja
+Comment: 
+
+Filename: model_card_gen/template/html/style/default_style.html.jinja
+Comment: 
+
+Filename: model_card_gen/tests/__init__.py
+Comment: 
+
+Filename: model_card_gen/tests/test_end_to_end_tf.py
+Comment: 
+
+Filename: model_card_gen/tests/test_end_to_end_torch.py
+Comment: 
+
+Filename: model_card_gen/tests/test_model_card.py
+Comment: 
+
+Filename: model_card_gen/tests/tf_model.py
+Comment: 
+
+Filename: model_card_gen/tests/torch_model.py
+Comment: 
+
+Filename: model_card_gen/utils/__init__.py
+Comment: 
+
+Filename: model_card_gen/utils/types.py
+Comment: 
+
+Filename: model_card_gen/utils/__pycache__/__init__.cpython-39.pyc
+Comment: 
+
+Filename: model_card_gen/utils/__pycache__/types.cpython-39.pyc
+Comment: 
+
+Filename: intel_xai-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: intel_xai-0.3.1.dev20230608.dist-info/METADATA
+Filename: intel_xai-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: intel_xai-0.3.1.dev20230608.dist-info/WHEEL
+Filename: intel_xai-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: intel_xai-0.3.1.dev20230608.dist-info/top_level.txt
+Filename: intel_xai-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: intel_xai-0.3.1.dev20230608.dist-info/RECORD
+Filename: intel_xai-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## explainer/README.md

```diff
@@ -14,17 +14,18 @@
 | featureablation     | Explain predictions using Captum's feature ablation method                                  |
 | zero_shot           | ...                                                                                         |
 | sentiment_analyis   | Explain HuggingFace pipeline predictions the SHAP explainer methods                         |
 
 ### [CAM](cam)
 
 | Method   | Decription                                                                                                 |
-|----------|------------------------------------------------------------------------------------------------------------|
-| xgradcam | Explain predictions with axiom-based gradient-based class activation maps using pytorch-grad-cam methods   |
-| eigancam | Explain predictions with eigan-based class activation maps using pytorch-grad-cam methods                  |
+|------------|------------------------------------------------------------------------------------------------------------|
+| xgradcam   | Explain predictions with axiom-based gradient-based class activation maps using pytorch-grad-cam methods   |
+| eigancam   | Explain predictions with eigan-based class activation maps using pytorch-grad-cam methods                  |
+| tf_gradcam | Explain predictions with gradient-based class activation maps with the  TensorFlow|
 
 ### [Metrics](metrics)
 
 | Method | Decription                                                                                  |
 |--------|---------------------------------------------------------------------------------------------|
 | confusion_matrix | Visualize classifier performance  via  a contingency table visualization          |
 | plot   | Visualize classifier performance via ROC/PR values over a spread of probability threasholds |
```

## explainer/version.py

```diff
@@ -14,8 +14,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 
-__version__ = "0.3.1.dev20230608"
+__version__ = "0.5.0"
```

## explainer/attributions/README.md

```diff
@@ -1,10 +1,10 @@
 # Feature Attributions
 
-```{code-cell} python3
+```python3
 from explainer import attributions
 ```
 
 Feature Attributions are an approach to explaining a model's predictions based on how the model has weighted the features it's been trained on.
 This set of functions visualizes features by utilizing [SHAP](https://github.com/slundberg/shap) (SHapley Additive exPlanations): an approach to explain the output of ML/DL models. 
 
 ## Algorithm
```

## explainer/attributions/__init__.py

```diff
@@ -14,8 +14,9 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 
+from .pt_attributions import *
 from .attributions import *
```

## explainer/attributions/attributions.py

```diff
@@ -14,27 +14,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 
-import torch
 import pandas as pd
 import numpy as np
 from typing import Union, Optional, Callable, List
 from .attributions_info import force_plot_info_panel
 from explainer.utils.graphics.info import InfoPanel
 from explainer.utils.types import TorchTensor
 from explainer.utils.model.model_framework import (is_tf_model,
                                                    is_pt_model,
                                                    raise_unknown_model_error)
 
 
 class FeatureAttributions:
+    '''
+    Attributions base class. Holds the shap API.
+    '''
     def __init__(self):
         import shap
         shap.initjs()
         self.shap = shap
         self.datasets = shap.datasets
         self.plots = self.shap.plots
         self.bar_plot = self.plots.bar
@@ -52,95 +54,300 @@
 
     def get_info(self):
         """Display into panel in Jupyter Enviornment"""
         if self.info_panel:
             info = InfoPanel(**self.info_panel)
             info.show()
 
-
 class DeepExplainer(FeatureAttributions):
-    def __init__(self, model, background_images, target_images, labels):
+    '''
+    Approximate conditional expectations of shap values for deep learning models using a variation of the DeepLIFT algorithm
+     (Shrikumar, Greenside, and Kundaje, arXiv 2017)
+
+    Args:
+      model (tf.keras.functional or pytorch.nn.Module): CNN model to be interpreted
+      background_images (numpy.ndarray, pandas.DataFrame or torch.tensor): the selection of background images used to integrate output features
+        across each target image
+      targetImages (numpy.ndarray, pandas.DataFrame or torch.tensor): the images to be interpreted
+      labels (list of strings): list of label names for the given classification problem
+
+    Attributes:
+      target_images: images used to explain predictions
+      explainer: the shap DeepExplainer object
+      shap_values: the resulting shap value estimations on the target images
+      labels: the class labels of the given classification problem 
+    
+    Reference:
+      https://shap-lrjball.readthedocs.io/en/latest/generated/shap.DeepExplainer.html
+    '''
+    def __new__(cls, model, *args):    
+        if is_tf_model(model):
+            # do nothing 
+            return super().__new__(cls)
+        elif is_pt_model(model):
+            from .pt_attributions import PTDeepExplainer
+            return super().__new__(PTDeepExplainer)
+        else:
+            raise_unknown_model_error()
+
+    def __init__(self, 
+                 model, 
+                 background_images: Union[np.ndarray,  pd.DataFrame, TorchTensor], 
+                 target_images: Union[np.ndarray,  pd.DataFrame, TorchTensor], 
+                 labels: Union[List[str], np.ndarray]
+                 ) -> None:
         super().__init__()
         self.target_images = target_images
         self.explainer = self.shap.DeepExplainer(model, background_images)
         self.shap_values = self.explainer.shap_values(target_images)
         self.labels = labels
 
-    def visualize(self):
-        import numpy as np
-        import torch
-      
-        arr = np.full((len(self.labels)), " ")
-        if torch.is_tensor(self.target_images):
-            self.shap_values = [np.swapaxes(np.swapaxes(s, 1, -1), 1, 2) for s in self.shap_values]
-            self.target_images = -np.swapaxes(np.swapaxes(self.target_images.numpy(), 1, -1), 1, 2)
+    
+
+    def visualize(self) -> None:
+        '''
+        plot superposition of shap estimations on original image(s) across all labels predictions
+        '''
 
         self.shap.image_plot(
             self.shap_values,
             self.target_images,
             np.array([list(self.labels)]*len(self.target_images)),
         )
 
 
 class GradientExplainer(FeatureAttributions):
-    def __init__(self, model, background_images, target_images, ranked_outputs, labels ):
-        import numpy as np
+    '''
+    Approximate expected gradients of differentiable models using a variation of the integrated gradients algorithm
+     (Sundararajan et al. 2017)
+
+    Args:
+      model (tf.keras.functional or pytorch.nn.Module): CNN model to be interpreted
+      background_images (numpy.ndarray, pandas.DataFrame or torch.tensor): the selection of background images 
+        used to integrate output features across each target image
+      target_images (numpy.ndarray, pandas.DataFrame or torch.tensor): the images to be interpreted
+      labels (list of strings): list of label names for the given classification problem
+      ranked_outputs (int): the number of top label predictions to be analyzed. Defaults to 1.
+
+    Attributes:
+      target_images: images used to explain predictions
+      ranked_outputs: the number of top label predictions
+      explainer: the shap GradientExplainer object
+      shap_values: the resulting shap value estimations on the target images
+      indexes: indexes where for the corresponding rankings of the each target image ranking
+      labels: the class labels of the given classification problem 
+
+    Reference:
+      https://shap-lrjball.readthedocs.io/en/latest/generated/shap.GradientExplainer.html
+    '''
+
+    def __new__(cls, model, *args):    
+        if is_tf_model(model):
+            # do nothing
+            return super().__new__(cls)
+        elif is_pt_model(model):
+            from .pt_attributions import PTGradientExplainer
+            return super().__new__(PTGradientExplainer)
+        else:
+            raise_unknown_model_error()
+
+    def __init__(self, 
+                 model, 
+                 background_images: Union[np.ndarray, pd.DataFrame, TorchTensor], 
+                 target_images: Union[np.ndarray, pd.DataFrame, TorchTensor], 
+                 labels: Union[List[str], np.ndarray],
+                 ranked_outputs: Optional[int] = 1,
+                 ) -> None:
         super().__init__()
         self.target_images = target_images
         self.ranked_outputs = ranked_outputs
         self.labels = labels
         self.explainer = self.shap.GradientExplainer(model, background_images)
         self.shap_values, self.indexes = self.explainer.shap_values(self.target_images, ranked_outputs=ranked_outputs)
 
-    def visualize(self):
-        import numpy as np
-        import torch
-
-        if torch.is_tensor(self.target_images):
-            self.shap_values = [np.swapaxes(np.swapaxes(s, 1, -1), 1, 2) for s in self.shap_values]
-            self.target_images = -np.swapaxes(np.swapaxes(self.target_images.numpy(), 1, -1), 1, 2) 
-
-        # check if 
-        if self.ranked_outputs == 1 and len(self.labels[self.indexes]) == 1:
-            idxs_to_plot = np.expand_dims(np.expand_dims(self.labels[self.indexes], 0), 0)
+        if self.indexes.shape == (1,1):
+            self.idxs_to_plot = [self.labels[self.indexes[0][0]]]
         else:
-            idxs_to_plot = self.labels[self.indexes]
+            self.idxs_to_plot = np.array(self.labels)[self.indexes]
 
+    def visualize(self) -> None:
+        '''
+        plot superposition of shap estimations on original image(s) across top ranked_outputs 
+        '''
         self.shap.image_plot(
             self.shap_values, 
             self.target_images, 
-            idxs_to_plot
+            self.idxs_to_plot
         )
 
 
 class KernelExplainer(FeatureAttributions):
-    def __init__(self, model, background, targets, nsamples):
+    '''
+    Approximate shap values via a combination of local interpretable model-agnostic explanations (LIME) and
+    a weighted linear regression.
+
+    Args:
+      model (function): "black box" prediction function that takes an input array of shape (n samples, m features)
+      and outputs an array of n predictions.
+      background (numpy.ndarray or pandas.DataFrame): the selection of background examples used to integrate output features
+        across each target example
+      targets (numpy.ndarray or pandas.DataFrame): the target examples to be interpreted
+      nsamples (int): the number of times to re-evaluate the model per prediction. Defaults to 64.
+
+    Attributes:
+      bg: background examples
+      targets: target examples
+      explainer: shap KernelExplainer object
+      shap_values: the resulting shap value estimations on the target examples 
+
+    Reference:
+    https://shap-lrjball.readthedocs.io/en/latest/generated/shap.KernelExplainer.html
+    '''
+    def __init__(self, 
+                 model: Callable[[np.ndarray], np.ndarray], 
+                 background: Union[np.ndarray, pd.DataFrame],
+                 targets: Union[np.ndarray, pd.DataFrame], 
+                 nsamples: int = 64
+                 ) -> None:
         super().__init__()
         self.bg = background
         self.targets = targets
         self.explainer = self.shap.KernelExplainer(model, self.bg)
         self.shap_values = self.explainer.shap_values(self.targets, nsamples=nsamples)
         self.info_panel = force_plot_info_panel
 
     def visualize(self):
+        '''
+        Display the force plot of the of the target example(s)
+        '''
         return self.force_plot(self.explainer.expected_value, self.shap_values[0], self.targets)
 
 
 class PartitionExplainer(FeatureAttributions):
-    def __init__(self, model, tokenizer, categories):
-        super().__init__()
-        self.masker = self.shap.maskers.Text(tokenizer=tokenizer)
-        self.explainer = self.shap.Explainer(model, masker=self.masker, output_names=categories)
+    '''
+    Approximate an extension of shap values, known as Owen values, by recursively computing shap values 
+    through a hierarchy of features that define feature coalitions. This is the base partition explainer class
+    that generates partition explainer children objects for text or image classification.
 
-    def __call__(self, *args, **kwargs):
-        data = args[0]
-        self.shap_values = self.explainer(data)
-        return self
+    Args:
+      task_type (string): 'text' or 'image' to choose which classification domain to be explained
+      *args: the remaining arguments required for child class instantiation
+    '''
+    def __new__(cls, task_type: str, *args) -> None:
+        if task_type == 'text':
+            return super().__new__(PartitionTextExplainer)
+        elif task_type == 'image':
+            return super().__new__(PartitionImageExplainer)
+        else:
+            raise ValueError(f"Task type {type(task_type)} is unsupported: please use 'text' or 'image'")
+    
+
+
+class PartitionImageExplainer(PartitionExplainer, FeatureAttributions):
+    '''
+    Image classification-based partition explanation. 
+    
+    Args:
+      task_type (string): 'text' or 'image' used in PartitionExplainer generator class. It is not used in this 
+      child class.
+      model (function): "black box" prediction function that takes an input array of shape (n samples, m features)
+      and outputs an array of n predictions.
+      labels (list): list of label names (strings) for the given classification problem
+      shape (tuple): height (int) and width (int) of images to be analyzed
+
+    Attributes:
+      explainer: shap PartitionExplainer object
+      shap_values: the resulting shap value estimations on the target images 
+    '''
+    def __init__(self, 
+                 task_type: str, 
+                 model: Callable[[np.ndarray], np.ndarray], 
+                 labels: List[str], 
+                 shape: tuple[int, int] 
+                 ) -> None:
+        FeatureAttributions.__init__(self)
+        PartitionExplainer.__init__(self)
+        self.shap_values = None
+        self.explainer = self.shap.Explainer(model, self.shap.maskers.Image('inpaint_telea', shape), output_names=labels)      
+
+    def run_explainer(self, 
+                      target_images: np.ndarray, 
+                      top_n: int = 1, 
+                      max_evals: int = 64
+                      ) -> None:
+        '''
+        Execute the partition explanation on the target_images.
+
+        Args:
+          target_images (numpy.ndarray): n images in the shape (n, height, width, channels)
+          in a better the estimation. Defaults to 64. 
+          top_n (int): gather shap values for the top n most probable classes per image. Defaults to 1.
+          max_evals (int): number of evaluations used in the shap estimation. The higher the number result 
+
+        Returns:
+          None
+        '''
+        self.shap_values = self.explainer(target_images, max_evals=max_evals, outputs=self.shap.Explanation.argsort.flip[:top_n])
+    
+    def visualize(self) -> None:
+        '''
+        Plot superposition of shap estimations on original image(s) across top ranked_outputs 
+        '''
+        self.image_plot(self.shap_values)
+
+class PartitionTextExplainer(PartitionExplainer, FeatureAttributions):
+    '''
+    Text classification-based partition explanation (using HuggingFace Transformers API). 
+
+    Args:
+      task_type (string): 'text' or 'image' used in PartitionExplainer generator class. It is not used in this 
+      child class.
+      model (function): "black box" prediction function that takes an input array of shape (n samples, m features)
+      and outputs an array of n predictions.
+      labels (list): list of label names (strings) for the given classification problem
+      tokenizer (string or callable): tokenizer used to break apart strings during masking of the text
+
+    Attributes:
+      explainer: shap PartitionExplainer object
+      shap_values: the resulting shap value estimations on the target examples 
+
+    Reference:
+    https://shap-lrjball.readthedocs.io/en/latest/generated/shap.PartitionExplainer.html 
+    '''
+    def __init__(self, 
+                 task_type: str, 
+                 model: Callable[[np.ndarray], np.ndarray], 
+                 labels: List[str], 
+                 tokenizer: Union[Callable[[str], str], str]) -> None:
+
+        FeatureAttributions.__init__(self)
+        PartitionExplainer.__init__(self)
+        self.shap_values = None
+        self.explainer = self.shap.Explainer(model, masker=self.shap.maskers.Text(tokenizer=tokenizer), output_names=labels)
+
+    def run_explainer(self, 
+                      target_text: str, 
+                      max_evals: int = 64) -> None:
+        '''
+        Execute the partition explanation on the target_text.
+
+        Args:
+          target_text (numpy.ndarray): 1-d numpy array of strings holding the text examples
+          max_evals (int): number of evaluations used in the shap estimation. The higher the number result 
+          in a better the estimation. Defaults to 64. 
+
+        Returns:
+          None
+        '''
+        self.shap_values = self.explainer(target_text, max_evals=max_evals)
 
     def visualize(self):
+        '''
+        Display the force plot of the of the target example(s)
+        '''
         self.text_plot(self.shap_values)
 
 
 class PipelineExplainer(FeatureAttributions):
     def __init__(self, task, model):
         import transformers
 
@@ -157,157 +364,30 @@
         self.shap_values = self.explainer(data)
         return self
 
     def visualize(self, label):
         self.shap.plots.text(self.shap_values[:, :, label])
 
 
-class Captum_Saliency:
-    def __init__(self, model):
-        from captum.attr import Saliency
-
-        self.saliency = Saliency(model)
-
-    def visualize(self, input, labels, original_image, imageTitle):
-        import numpy as np
-        from captum.attr import visualization as viz
-
-        self.grads = self.saliency.attribute(input, target=labels.item())
-        self.grads = np.transpose(
-            self.grads.squeeze().cpu().detach().numpy(), (1, 2, 0)
-        )
-        viz.visualize_image_attr(
-            self.grads,
-            original_image,
-            method="blended_heat_map",
-            sign="absolute_value",
-            show_colorbar=True,
-            title=imageTitle,
-        )
-
-
-class Captum_IntegratedGradients:
-    def __init__(self, model):
-        from captum.attr import IntegratedGradients
-
-        self.ig = IntegratedGradients(model)
-
-    def visualize(self, input, labels, original_image, imageTitle):
-        import numpy as np
-        from captum.attr import visualization as viz
-
-        self.attr_ig = self.ig.attribute(input, target=labels, baselines=input * 0)
-        self.attr_ig = np.transpose(
-            self.attr_ig.squeeze().cpu().detach().numpy(), (1, 2, 0)
-        )
-        viz.visualize_image_attr(
-            self.attr_ig,
-            original_image,
-            method="blended_heat_map",
-            sign="all",
-            show_colorbar=True,
-            title=imageTitle,
-        )
-
-
-class Captum_DeepLift:
-    def __init__(self, model):
-        from captum.attr import DeepLift
-
-        self.dl = DeepLift(model)
-
-    def visualize(self, input, labels, original_image, imageTitle):
-        import numpy as np
-        from captum.attr import visualization as viz
-
-        self.attr_dl = self.dl.attribute(input, target=labels, baselines=input * 0)
-        self.attr_dl = np.transpose(
-            self.attr_dl.squeeze(0).cpu().detach().numpy(), (1, 2, 0)
-        )
-        viz.visualize_image_attr(
-            self.attr_dl,
-            original_image,
-            method="blended_heat_map",
-            sign="all",
-            show_colorbar=True,
-            title=imageTitle,
-        )
-
-
-class Captum_SmoothGrad:
-    def __init__(self, model):
-        from captum.attr import IntegratedGradients
-        from captum.attr import NoiseTunnel
-
-        self.ig = IntegratedGradients(model)
-        self.nt = NoiseTunnel(self.ig)
-
-    def visualize(self, input, labels, original_image, imageTitle):
-        import numpy as np
-        from captum.attr import visualization as viz
-
-        self.attr_ig_nt = self.nt.attribute(
-            input,
-            target=labels,
-            baselines=input * 0,
-            nt_type="smoothgrad_sq",
-            nt_samples=100,
-            stdevs=0.2,
-        )
-        self.attr_ig_nt = np.transpose(
-            self.attr_ig_nt.squeeze(0).cpu().detach().numpy(), (1, 2, 0)
-        )
-        viz.visualize_image_attr(
-            self.attr_ig_nt,
-            original_image,
-            method="blended_heat_map",
-            sign="absolute_value",
-            outlier_perc=10,
-            show_colorbar=True,
-            title=imageTitle,
-        )
-
-
-class Captum_FeatureAblation:
-    def __init__(self, model):
-        from captum.attr import FeatureAblation
-
-        self.ablator = FeatureAblation(model)
-
-    def visualize(self, input, labels, original_image, imageTitle):
-        import numpy as np
-        from captum.attr import visualization as viz
 
-        self.fa_attr = self.ablator.attribute(
-            input, target=labels, baselines=input * 0
-        )
-        self.fa_attr = np.transpose(
-            self.fa_attr.squeeze(0).cpu().detach().numpy(), (1, 2, 0)
-        )
-        viz.visualize_image_attr(
-            self.fa_attr,
-            original_image,
-            method="blended_heat_map",
-            sign="all",
-            show_colorbar=True,
-            title=imageTitle,
-        )
 
 def explainer():
     """
     Calls FeatureAttributions
     Returns FeatureAttributions which has native references as attributes
 
     Returns:
       FeatureAttributions
     
     Example:
-      >>> from explainer.explainers import feature_attributions_explainer
-      >>> explainer = feature_attributions_explainer.explainer
-      >>> ??explainer
+      >>> from explainer import attributions
+      >>> explainer = attributions.explainer()
+      <IPython.core.display.HTML object>
+      >>> explainer.shap.__version__
+      '0.41.0' 
     """
     return FeatureAttributions()
 
 
 def kernel_explainer(model, background, targets, nsamples=500):
     """
     Returns a SHAP KernelExplainer, using the Kernel SHAP method
@@ -322,15 +402,15 @@
 
     Reference:
       https://shap-lrjball.readthedocs.io/en/latest/generated/shap.KernelExplainer.html
     """
     return KernelExplainer(model, background, targets, nsamples=nsamples)
 
 
-def deep_explainer(model, backgroundImages, targetImages, labels):
+def deep_explainer(model, backgroundImages, targetImages, labels) -> DeepExplainer:
     """
     Returns a SHAP DeepExplainer that approximate SHAP values for deep learning models.
 
     Args:
       model: model
       backgroundImages: list
       targetImages: list
@@ -341,145 +421,77 @@
 
     Reference:
       https://shap-lrjball.readthedocs.io/en/latest/generated/shap.DeepExplainer.html
     """
     return DeepExplainer(model, backgroundImages, targetImages, labels)
 
 
-def gradient_explainer(model, backgroundImages, targetImages, rankedOutputs, labels):
+def gradient_explainer(model, 
+                       background_images: Union[np.ndarray,  pd.DataFrame, TorchTensor],
+                       target_images: Union[np.ndarray,  pd.DataFrame, TorchTensor], 
+                       labels: Union[List[str], np.ndarray],
+                       ranked_outputs: Optional[int] = 1,
+                 ) -> GradientExplainer:
     """
     Sets up a SHAP GradientExplainer, explains a model using expected gradients.
 
     Args:
       model: model
-      backgroundImages: list
-      targetImages: list
-      rankedOutputs: int
+      background_images: list
+      target_images: list
       labels: list
+      ranked_outputs: int (options and defaults to 1)
 
     Returns:
       GradientExplainer
 
     Reference:
       https://shap-lrjball.readthedocs.io/en/latest/generated/shap.GradientExplainer.html
     """
-    return GradientExplainer(model, backgroundImages, targetImages, rankedOutputs, labels)
+    return GradientExplainer(model, background_images, target_images, labels, ranked_outputs)
 
 
-def partition_explainer(model, tokenizer, categories):
+def partition_text_explainer(model, labels, target_text, tokenizer, max_evals=64):
     """
-    Calls PartitionExplainer with the model, masker and categories
-    Returns a SHAP PartitionExplainer that explain the output of any function.
+    Instantiates PartitionExplainer for text classification and executes run_explainer()
 
     Args:
       model (function): the model
-      tokenizer (str): the tokens you want to mask
+      tokenizer (string or callable): the tokens you want to mask
       categories (list): the category names
 
     Reference:
       https://shap-lrjball.readthedocs.io/en/latest/generated/shap.PartitionExplainer.html
 
     Returns:
       PartitionExplainer
-    
-    Example:
-      >>> def make_pred(X_batch_text):
-      >>>   X_batch = vectorizer.transform(X_batch_text).toarray()
-      >>>   preds = model.predict(X_batch)
-      >>>   return preds
-      >>>
-      >>> from explainer.explainers import feature_attributions_explainer
-      >>> partition_explainer = feature_attributions_explainer.partitionexplainer
-      >>> partition_explainer = partitione_explainer(make_pred, r"\W+",selected_categories)(X_batch_text)
-      >>> partition_explainer.visualize()
-    """
-    return PartitionExplainer(model, tokenizer, categories)
-
-
-def saliency(model):
-    """
-    Returns a Captum Saliency. This provides a baseline approach for computing
-    input attribution, returning the gradients with respect to inputs.
-
-    Args:
-      model: pytorch model
-
-    Returns:
-      captum.attr.Saliency
-
-    Reference:
-      https://captum.ai/api/saliency.html
-    """
-    return Captum_Saliency(model)
-
-
-def integratedgradients(model):
-    """
-    Returns a Captum IntegratedGradients
-
-    Args:
-      model: pytorch model
-
-    Returns:
-      captum.attr.IntegratedGradients
-
-    Reference:
-      https://captum.ai/api/integrated_gradients.html
-    """
-    return Captum_IntegratedGradients(model)
-
-
-def deeplift(model):
-    """
-    Returns a Captum DeepLift
-
-    Args:
-      model: pytorch model
-
-    Returns:
-      captum.attr.DeepLift
-
-    Reference:
-      https://captum.ai/api/deep_lift.html
     """
-    return Captum_DeepLift(model)
+    pe = PartitionExplainer('text', model, labels, tokenizer)
+    pe.run_explainer(target_text, max_evals=max_evals)
+    return pe
 
 
-def smoothgrad(model):
+def partition_image_explainer(model, labels, target_images, top_n=1, max_evals=64):
     """
-    Returns a Captum Integrated Gradients, Noise Tunnel SmoothGrad
+    Instantiates PartitionExplainer for image classification and executes run_explainer()
 
     Args:
-      model: pytorch model
-
-    Returns:
-      captum.attr.NoiseTunnel
+      model (function): the model
+      tokenizer (string or callable): the tokens you want to mask
+      categories (list): the category names
 
     Reference:
-      https://captum.ai/api/integrated_gradients.html
-      https://captum.ai/api/noise_tunnel.html
-    """
-    return Captum_SmoothGrad(model)
-
-
-def featureablation(model):
-    """
-    Returns a Captum FeatureAblation
-
-    Args:
-      model: pytorch model
+      https://shap-lrjball.readthedocs.io/en/latest/generated/shap.PartitionExplainer.html
 
     Returns:
-      captum.attr.FeatureAblation
-
-    Reference:
-      https://captum.ai/api/feature_ablation.html
+      PartitionImageExplainer
     """
-    return Captum_FeatureAblation(model)
-
+    pe = PartitionExplainer('image', model, labels, target_images[0].shape)
+    pe.run_explainer(target_images, top_n=top_n, max_evals=max_evals)
+    return pe
 
 def zero_shot(pipe, text):
     print(f"Shap version used: {shap.__version__}")
     explainer = shap.Explainer(pipe)
     shap_values = explainer(text)
     prediction = pipe(text)
     print(f"Model predictions are: {prediction}")
@@ -495,14 +507,9 @@
 
     Args:
       model: model
       data: examples used for sentiment-analysis
 
     Returns:
       PipelineExplainer
-
-    Example:
-      >>> from explainer.api import ExplainerContextManager as ec
-      >>> with ec('feature_attributions_explainer') as fe:
-      >>>   fe.sentiment_analysis(model.model, raw_text_input).visualize(1)
     """
     return PipelineExplainer('sentiment-analysis', model)(data)
```

## explainer/cam/README.md

```diff
@@ -1,27 +1,29 @@
 # CAM (Class Activation Mapping)
 
-```{code-cell} python3
+```python3
 from explainer import cam
 ```
 
 CAM is an approach which localizes regions in the image responsible for a class prediction. 
 Here, for object classification model, we support visualization of XGradCAM, which is the state-of-the art CAM method by
 utilizing [pytorch-grad-cam](https://github.com/jacobgil/pytorch-grad-cam) package. 
-We also support visualization of EigenCAM which is a fast method for object detection models. 
+We also support visualization of the base gradCAM method and EigenCAM which is a fast method for object detection models. 
 
 ## Algorithm
 CAM takes the input image and the trained model as input, and generates visualization by highlighting
 the region in the corresponding image that are responsible for the classification decision.
 
 ## Environment
 - Jupyter Notebooks
 
 ## XAI Methods
+- GradCAM
 - XGradCAM
 - EigenCAM
-
 ## Toolkits
 - pytorch-grad-cam
 
 ## References
-[pytorch-grad-cam](https://github.com/jacobgil/pytorch-grad-cam)
+[pytorch-grad-cam](https://github.com/jacobgil/pytorch-grad-cam)<br> 
+[TF GradCAM Implementation](https://github.com/ismailuddin/gradcam-tensorflow-2/blob/master/notebooks/GradCam.ipynb)<br>
+[Grad-CAM: Visual Explanations from Deep Networks via Gradient-based Localization](https://arxiv.org/abs/1610.02391)
```

## explainer/cam/__init__.py

```diff
@@ -14,8 +14,10 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 
-from .cam import *
+from .tf_cam import TFGradCAM,  tf_gradcam
+from .pt_cam import XGradCAM, EigenCAM, x_gradcam, eigencam
+from .cam import GradCAM
```

## explainer/cam/cam.py

```diff
@@ -1,154 +1,36 @@
-class XGradCAM:
-    def __init__(self, model, targetLayer, targetClass, image, dims, device):
-
-        # set any frozen layers to trainable
-        # gradcam cannot be calculated without it
-        for param in model.parameters():
-            if not param.requires_grad:
-                param.requires_grad = True
-
-        self.model = model
-        self.targetLayer = targetLayer
-        self.targetClass = targetClass
-        self.image = image
-        self.dims = dims
-        self.device = device
-
-    def visualize(self):
-        from pytorch_grad_cam import XGradCAM, GuidedBackpropReLUModel
-        from pytorch_grad_cam.utils.model_targets import ClassifierOutputTarget
-        from pytorch_grad_cam.utils.image import show_cam_on_image, deprocess_image, preprocess_image
-        import torch
-        import cv2
-        import numpy as np
-        import matplotlib.pyplot as plt
-
-        self.model.eval().to(self.device)
-
-        image = cv2.resize(self.image, self.dims)
-        # convert to rgb if image is grayscale
-        converted = False
-        if len(image.shape) == 2:
-            converted = True 
-            image = cv2.cvtColor(image, cv2.COLOR_GRAY2RGB)
-        
-        rgb_img = np.float32(image) / 255
-        input_tensor = preprocess_image(rgb_img,
-                                        mean=[0.485, 0.456, 0.406],
-                                        std=[0.229, 0.224, 0.225])
-        input_tensor = input_tensor.to(self.device)
-        
-        self.targetLayer = [self.targetLayer]
-        
-        if self.targetClass is None:
-            targets = None
-        else:
-            targets = [ClassifierOutputTarget(self.targetClass)]
-
-        cam = XGradCAM(self.model, self.targetLayer, use_cuda=torch.cuda.is_available())
-
-        # convert back to grayscale if that is the initial dim
-        if converted:
-            input_tensor = input_tensor[:, 0:1, :, :]
-
-        grayscale_cam = cam(input_tensor=input_tensor, targets=targets, aug_smooth=False,
-                            eigen_smooth=False)
-        grayscale_cam = grayscale_cam[0, :]
-        cam_image = show_cam_on_image(rgb_img, grayscale_cam, use_rgb=True)
-        cam_image = cv2.cvtColor(cam_image, cv2.COLOR_RGB2BGR)
-
-        gb_model = GuidedBackpropReLUModel(model=self.model, use_cuda=torch.cuda.is_available())
-        gb = gb_model(input_tensor, target_category=None)
-        cam_mask = cv2.merge([grayscale_cam, grayscale_cam, grayscale_cam])
-        cam_gb = deprocess_image(cam_mask * gb)
-        gb = deprocess_image(gb)
-
-        fig = plt.figure(figsize=(10, 7))
-        rows = 1
-        columns = 3
-
-        fig.add_subplot(rows, columns, 1)
-        plt.imshow(cv2.cvtColor(cam_image, cv2.COLOR_BGR2RGB))
-        plt.axis('off')
-        plt.title("XGradCAM")
-
-        fig.add_subplot(rows, columns, 2)
-        plt.imshow(cv2.cvtColor(gb, cv2.COLOR_BGR2RGB))
-        plt.axis('off')
-        plt.title("Guided backpropagation")
-
-        fig.add_subplot(rows, columns, 3)
-        plt.imshow(cv2.cvtColor(cam_gb, cv2.COLOR_BGR2RGB))
-        plt.axis('off')
-        plt.title("Guided XGradCAM")
-
-        print("XGradCAM, Guided backpropagation, and Guided XGradCAM are generated. ")
-
-def xgradcam(model, targetLayer, targetClass, image, dims, device):
-    return XGradCAM(model, targetLayer, targetClass, image, dims, device)
-
-class EigenCAM:
-    def __init__(self, model, targetLayer, boxes, classes, colors, reshape, image, device):
-        self.model = model
-        self.targetLayer = targetLayer
-        self.boxes = boxes
-        self.classes = classes
-        self.colors = colors
-        self.reshape = reshape
-        self.image = image
-        self.device = device
-
-    def visualize(self):
-        from pytorch_grad_cam import EigenCAM
-        from pytorch_grad_cam.utils.image import show_cam_on_image, preprocess_image, scale_cam_image
-        import torchvision
-        import torch
-        import cv2
-        import numpy as np
-        from PIL import Image
-        from IPython.display import display
-
-        self.model.eval().to(self.device)
-
-        rgb_img = np.float32(self.image) / 255
-        transform = torchvision.transforms.ToTensor()
-        input_tensor = transform(rgb_img)
-        input_tensor = input_tensor.unsqueeze(0)
-        input_tensor = input_tensor.to(self.device)
-
-        self.targetLayer = [self.targetLayer]
-
-        if self.reshape is None:
-            cam = EigenCAM(self.model, self.targetLayer, use_cuda=torch.cuda.is_available())
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+#
+# Copyright (c) 2023 Intel Corporation
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# SPDX-License-Identifier: Apache-2.0
+#
+
+from ..utils.model.model_framework import is_tf_model, is_pt_model, raise_unknown_model_error
+
+class GradCAM:
+    """GradCAM generator class. Depending on the model framework, GradCAM is a superclass to TFGradCAM or XGradCAM.
+    Note that EigenCAM (only supports PyTorch) is not included yet.
+    """
+    def __new__(cls, model, *args):    
+        from .tf_cam import TFGradCAM
+        from .pt_cam import XGradCAM
+
+        if is_tf_model(model):
+            return super().__new__(TFGradCAM)
+        elif is_pt_model(model):
+            return super().__new__(XGradCAM)
         else:
-            cam = EigenCAM(self.model, self.targetLayer, use_cuda=torch.cuda.is_available(),
-                           reshape_transform=self.reshape)
-        targets = []
-        grayscale_cam = cam(input_tensor=input_tensor, targets=targets, aug_smooth=False,
-                            eigen_smooth=False)
-        grayscale_cam = grayscale_cam[0, :]
-        cam_image = show_cam_on_image(rgb_img, grayscale_cam, use_rgb=True)
-
-        renormalized_cam = np.zeros(grayscale_cam.shape, dtype=np.float32)
-        for x1, y1, x2, y2 in self.boxes:
-            renormalized_cam[y1:y2, x1:x2] = scale_cam_image(grayscale_cam[y1:y2, x1:x2].copy())
-        renormalized_cam = scale_cam_image(renormalized_cam)
-        eigencam_image_renormalized = show_cam_on_image(rgb_img, renormalized_cam, use_rgb=True)
-        for i, box in enumerate(self.boxes):
-            color = self.colors[i]
-            cv2.rectangle(
-                eigencam_image_renormalized,
-                (box[0], box[1]),
-                (box[2], box[3]),
-                color, 2
-            )
-            cv2.putText(eigencam_image_renormalized, self.classes[i], (box[0], box[1] - 5),
-                        cv2.FONT_HERSHEY_SIMPLEX, 0.8, color, 2,
-                        lineType=cv2.LINE_AA)
-
-        display(Image.fromarray(np.hstack((cam_image, eigencam_image_renormalized))))
-
-        print("EigenCAM is generated. ")
-
-def eigencam(model, targetLayer, boxes, classes, colors, reshape, image, device):
-    return EigenCAM(model, targetLayer, boxes, classes, colors, reshape, image, device)
+            raise_unknown_model_error()
```

## explainer/cam/pt_cam.py

```diff
@@ -24,16 +24,14 @@
     '''
     Holds the calculations for the axiom-based gradient-weighted class activation mapping (XgradCAM) of a 
     given image and PyTorch CNN.
 
     Args:
       model (torch.nn.Module): the CNN used for classification 
       target_layer (torch.nn.modules.container.Sequential): the convolution layer that you want to analyze (usually the last) 
-      target_class (int): the index of the target class
-      image (numpy.ndarray): image to be analyzed with a shape (h,w,c)
       dims (tuple of ints): dimension of image (h, w)
       device (torch.device): torch.device('cpu') or torch.device('gpu') for PyTorch optimizations
 
         
     Attributes:
       model: the CNN being used
       target_layer: the target convolution being used 
@@ -44,94 +42,106 @@
 
     Methods:
       visualize: superimpose the gradCAM result on top of the original image
 
     Reference:
        https://github.com/jacobgil/pytorch-grad-cam
     '''
-    def __init__(self, model, targetLayer, targetClass, image, dims, device):
-
+    def __init__(self, model, target_layer, dims, device='cpu'):
         # set any frozen layers to trainable
         # gradcam cannot be calculated without it
         for param in model.parameters():
             if not param.requires_grad:
                 param.requires_grad = True
 
         self.model = model
-        self.targetLayer = targetLayer
-        self.targetClass = targetClass
-        self.image = image
+        self.target_layer = [target_layer]
         self.dims = dims
         self.device = device
 
-    def visualize(self):
+    def run_explainer(self, image, target_class):
+        '''
+        Execute the axiom-based gradient-based class activation mapping algorithm on the image.
+
+        Args: 
+            image (numpy.ndarray): image to be analyzed with a shape (h,w,c)
+            target_class (int): the index of the target class
+
+        Returns:
+            None
+        '''
         from pytorch_grad_cam import XGradCAM, GuidedBackpropReLUModel
         from pytorch_grad_cam.utils.model_targets import ClassifierOutputTarget
         from pytorch_grad_cam.utils.image import show_cam_on_image, deprocess_image, preprocess_image
-        import torch
         import cv2
         import numpy as np
-        import matplotlib.pyplot as plt
 
         self.model.eval().to(self.device)
 
-        image = cv2.resize(self.image, self.dims)
+        image = cv2.resize(image, self.dims)
         # convert to rgb if image is grayscale
         converted = False
         if len(image.shape) == 2:
             converted = True 
             image = cv2.cvtColor(image, cv2.COLOR_GRAY2RGB)
         
         rgb_img = np.float32(image) / 255
         input_tensor = preprocess_image(rgb_img,
                                         mean=[0.485, 0.456, 0.406],
                                         std=[0.229, 0.224, 0.225])
         input_tensor = input_tensor.to(self.device)
         
-        self.targetLayer = [self.targetLayer]
-        
-        if self.targetClass is None:
+        if target_class is None:
             targets = None
         else:
-            targets = [ClassifierOutputTarget(self.targetClass)]
+            targets = [ClassifierOutputTarget(target_class)]
 
-        cam = XGradCAM(self.model, self.targetLayer)
+        cam = XGradCAM(self.model, self.target_layer)
 
         # convert back to grayscale if that is the initial dim
         if converted:
             input_tensor = input_tensor[:, 0:1, :, :]
 
         grayscale_cam = cam(input_tensor=input_tensor, targets=targets, aug_smooth=False,
                             eigen_smooth=False)
         grayscale_cam = grayscale_cam[0, :]
         cam_image = show_cam_on_image(rgb_img, grayscale_cam, use_rgb=True)
-        cam_image = cv2.cvtColor(cam_image, cv2.COLOR_RGB2BGR)
+        self.cam_image = cv2.cvtColor(cam_image, cv2.COLOR_RGB2BGR)
 
         gb_model = GuidedBackpropReLUModel(model=self.model, use_cuda=False)
         gb = gb_model(input_tensor, target_category=None)
         cam_mask = cv2.merge([grayscale_cam, grayscale_cam, grayscale_cam])
-        cam_gb = deprocess_image(cam_mask * gb)
-        gb = deprocess_image(gb)
+        self.cam_gb = deprocess_image(cam_mask * gb)
+        self.gb = deprocess_image(gb)
+
+    def visualize(self):
+        '''
+        Plot the axiom gradCAM, guided back propagation and guided axiom gradCAM from left
+        to right, all superimposed on the target image.  
+        '''
 
+        import matplotlib.pyplot as plt
+        import cv2
+        
         fig = plt.figure(figsize=(10, 7))
         rows = 1
         columns = 3
 
         fig.add_subplot(rows, columns, 1)
-        plt.imshow(cv2.cvtColor(cam_image, cv2.COLOR_BGR2RGB))
+        plt.imshow(cv2.cvtColor(self.cam_image, cv2.COLOR_BGR2RGB))
         plt.axis('off')
         plt.title("XGradCAM")
 
         fig.add_subplot(rows, columns, 2)
-        plt.imshow(cv2.cvtColor(gb, cv2.COLOR_BGR2RGB))
+        plt.imshow(cv2.cvtColor(self.gb, cv2.COLOR_BGR2RGB))
         plt.axis('off')
         plt.title("Guided backpropagation")
 
         fig.add_subplot(rows, columns, 3)
-        plt.imshow(cv2.cvtColor(cam_gb, cv2.COLOR_BGR2RGB))
+        plt.imshow(cv2.cvtColor(self.cam_gb, cv2.COLOR_BGR2RGB))
         plt.axis('off')
         plt.title("Guided XGradCAM")
 
         print("XGradCAM, Guided backpropagation, and Guided XGradCAM are generated. ")
 
 
 
@@ -230,12 +240,14 @@
 
         display(Image.fromarray(np.hstack((cam_image, eigencam_image_renormalized))))
 
         print("EigenCAM is generated. ")
 
 
 
-def xgradcam(model, targetLayer, targetClass, image, dims, device):
-    return XGradCAM(model, targetLayer, targetClass, image, dims, device)
+def x_gradcam(model, target_layer, target_class, image, dims, device='cpu'):
+    gc = XGradCAM(model, target_layer, dims, device)
+    gc.run_explainer(image, target_class)
+    return gc
 
 def eigencam(model, targetLayer, boxes, classes, colors, reshape, image, device):
     return EigenCAM(model, targetLayer, boxes, classes, colors, reshape, image, device)
```

## explainer/cam/tf_cam.py

```diff
@@ -24,48 +24,48 @@
     '''
     Holds the calculations for the gradient-weighted class activation mapping (gradCAM) of a 
     given image and TensorFlow CNN.
 
     Args:
       model (tf.keras.functional): the CNN used for classification 
       target_layer (tf.keras.KerasLayer): the convolution layer that you want to analyze (usually the last) 
-      target_class (int): the index of the target class
-      image (numpy.ndarray): image to be analyzed with a shape (h,w,c)
+      dims (tuple of ints): dimension of image (h, w)
 
         
     Attributes:
       model: the CNN being used
       target_layer: the target convolution being used 
       target_class: the target class being used
       image: the image being used
-      dims: the dimensions of the image being used
       gradcam: the result of the gradCAM calculation from the model's target_layer on the image
 
-
-    Methods:
-      visualize: superimpose the gradCAM result on top of the original image
-
     Reference:
       https://github.com/ismailuddin/gradcam-tensorflow-2/blob/master/notebooks/GradCam.ipynb 
     '''
-    def __init__(self, model, target_layer, target_class, image):
+    def __init__(self, model, target_layer):
         
         self.model = model
         self.target_layer = target_layer
-        self.target_class = target_class
-        self.image = image
-        self.dims = (image.shape[0], image.shape[1])
         
-        self.gradcam = self._get_gradcam()
     
-    def _get_gradcam(self):
+    def run_explainer(self, image, target_class):
+        '''
+        Execute the gradient-based class activation mapping algorithm on target image.
+
+        Args:
+          image (numpy.ndarray): image to be analyzed with a shape (h,w,c)
+          target_class (int): the index of the target class
+        '''
+
         import numpy as np
         import tensorflow as tf
         import cv2
 
+        self.dims = (image.shape[0], image.shape[1]) 
+        self.image = image
         last_conv_layer_model = tf.keras.Model(self.model.inputs, self.target_layer.output)
         classifier_input = tf.keras.Input(shape=self.target_layer.output.shape[1:])
         x = classifier_input
         
         # get the last conv layer and all the proceeding layers  
         last_layers = []
         for layer in reversed(self.model.layers):
@@ -76,35 +76,38 @@
         # create the classifier model to get the gradient for the
         # target class
         for layer_name in reversed(last_layers):
             x = self.model.get_layer(layer_name)(x)
         classifier_model = tf.keras.Model(classifier_input, x)
         
         with tf.GradientTape() as tape:
-            inputs = self.image[np.newaxis, ...]
+            inputs = image[np.newaxis, ...]
             last_conv_layer_output = last_conv_layer_model(inputs)
             tape.watch(last_conv_layer_output)
             preds = classifier_model(last_conv_layer_output)
-            top_class_channel = preds[:, self.target_class]
+            top_class_channel = preds[:, target_class]
 
         grads = tape.gradient(top_class_channel, last_conv_layer_output)
         pooled_grads = tf.reduce_mean(grads, axis=(0, 1, 2)).numpy()
         
         last_conv_layer_output = last_conv_layer_output.numpy()[0]
         for i in range(pooled_grads.shape[-1]):
             last_conv_layer_output[:, :, i] *= pooled_grads[i]
         
         # Average over all the filters to get a single 2D array
         gradcam = np.mean(last_conv_layer_output, axis=-1)
         # Clip the values (equivalent to applying ReLU)
         # and then normalise the values
         gradcam = np.clip(gradcam, 0, np.max(gradcam)) / np.max(gradcam)
-        return cv2.resize(gradcam, self.dims)
+        self.gradcam = cv2.resize(gradcam, self.dims)
         
     def visualize(self):
+        '''
+        Plot the gradCAM superimposed on top of the original image.
+        '''
         import matplotlib.pyplot as plt
         
         plt.imshow(self.image)
         plt.imshow(self.gradcam, alpha=0.5)
         plt.axis('off')
 
 def tf_gradcam(model, target_layer, target_class, image):
@@ -113,15 +116,18 @@
     mapping of a given image and CNN.
 
     Args:
       model (tf.keras.Functional): the CNN used for classification 
       target_layer (tf.keras.KerasLayer): the convolution layer that you want to analyze (usually the last) 
       target_class (int): the index of the target class
       image (numpy.ndarray): image to be analyzed with a shape (h,w,c)
+      dims (tuple of ints): dimension of image (h, w)
 
     Returns:
       TFGradCAM
 
     Reference:
        https://github.com/ismailuddin/gradcam-tensorflow-2/blob/master/notebooks/GradCam.ipynb
     """
-    return TFGradCAM(model, target_layer, target_class, image)
+    gc = TFGradCAM(model, target_layer)
+    gc.run_explainer(image, target_class)
+    return gc
```

## explainer/metrics/README.md

```diff
@@ -1,10 +1,10 @@
 # Metrics
  
-```{code-cell} python3
+```python3
 from explainer import metrics
 ```
 
 Several base metrics are provided for ML/DL classification models. These metrics cover model execution and performance and orient the data scientist to where there is potential for classification bias. 
 
 ## Algorithms
 Provided with a classfication model's predictions and their corresponding ground truths, staple performance metrics can be calculated to determine prediction behaviors in the real world. These functions leverage scikit-learn and plotly (eventually) to calculate and visualize said metrics, respectively.
```

## explainer/metrics/metrics.py

```diff
@@ -26,16 +26,15 @@
     all class labels. Checking these accuracies on unseen test data (real-world data) is a 
     first step in identifying possible sample bias.
 
     This class supports both binary and multi-class classification. Currently, the accuracies
     are normalized across each ground truth (row).
 
     Args:
-      ground truth: 2-d array (n_samples, n_classes) of the ground truth, integer one-hot-encoded, 
-        correct target values that correspond to the examples used in testing
+      ground truth: 1-d or 2-d array (if one-hot-encoded) of the integer ground truth labels
       predictions: 2-d array (n_samples, n_classes) of the one-hot-encoded, predicted probabilities 
         that align with the ground truth array
       labels: 1-d array of strings that index the label names to the one-hot encodings
 
     Attributes:
       y_gt: 1-d array of integer ground truth labels
       y_pred: 1-d array of integer class prediction labels 
@@ -56,48 +55,56 @@
     import sklearn
     from sklearn.metrics import confusion_matrix as cmx
     from sklearn.metrics import classification_report
     import pandas as pd
     pd.options.plotting.backend = "plotly"
     import numpy as np
 
-    # ground truth
-    self.y_gt = np.argmax(groundtruth, axis=1)
+    # if gt is one-hot-encoded, flatten to original
+    if len(np.array(groundtruth).shape) == 2:
+      self.y_gt = np.argmax(groundtruth, axis=1)
+    else:
+      self.y_gt = np.array(groundtruth)
     # model predictions
     self.y_pred = np.argmax(predictions, axis=1)
     # label names
     self.labels = labels
     # array representation of the confusion matrix
     self.arr = cmx(self.y_gt, self.y_pred, normalize='true')
     # dataframe representation of the confusion matrix
     self.df = pd.DataFrame(self.arr, index = [i for i in self.labels],
                 columns = [i for i in self.labels]) 
     # str representation of metrics containing precision, recall, f1 and acc for each class
     self.report = classification_report(self.y_gt, self.y_pred, target_names=self.labels)
 
-
   def visualize(self):
     import matplotlib.pyplot as plt
     import seaborn as sn
-    plt.figure(figsize=(10,7))
-    sn.heatmap(self.df, annot=True)
-
+    plt.figure(figsize=(10,10))
+    s = sn.heatmap(self.df, 
+                   annot=True, 
+                   cmap=sn.color_palette("Blues", as_cmap=True),
+                   linewidths=2,
+                   cbar=False)
+    s.set_xlabel('Predict', fontsize=14)
+    s.set_ylabel('True', fontsize=14)
+    s.set_title('Confusion Matrix', fontsize=18)
+    s.tick_params(left=False, bottom=False)
 
 class Plotter:
   """
     Plotter object that calculates and holds the necessary values for various plots commonly used in 
     post-training analysis on test data. In particular, these plots utilize thesholding the predicted
     probabilities in order to quantify the skill of the model. They provide behavior of the classification
     rates dependent upon these probability thresholds and are useful in diagnosing dataset imbalance issues.
 
     This class accepts both binary and multi-class classification.
 
     Args:
-      ground truth: 2-d array (n_samples, n_classes) of the ground truth, integer one-hot-encoded, 
-        correct target values that correspond to the examples used in testing
+      ground truth: 1-d or 2-d array (if one-hot-encoded) of the integer ground truth labels
       predictions: 2-d array (n_samples, n_classes) of the one-hot-encoded, predicted probabilities 
         that align with the ground truth array
       labels: 1-d array of strings that index the label names to the one-hot encodings
 
     Attributes:
       y_gt: 2-d array of one-hot-encoded integer ground truth labels
       y_pred: 2-d array of class predicted probabilities 
@@ -122,78 +129,95 @@
   """  
   def __init__(self,groundtruth,predictions,labels):
     from sklearn.metrics import precision_recall_curve
     from sklearn.metrics import roc_curve as sk_roc_curve
     import pandas as pd
     import numpy as np
     pd.options.plotting.backend = "plotly"
-    
 
-    self.y_gt = np.array(groundtruth)
+    # one-hot encode gt if it is not already
+    if len(np.array(groundtruth).shape) == 1:
+      self.y_gt = np.eye(len(labels))[np.array(groundtruth).astype(int)]
+    else:
+      self.y_gt = np.array(groundtruth)
+      
     self.y_pred = np.array(predictions)
     self.labels = labels
     self.precision, self.recall = dict(), dict()
     self.tpr, self.fpr = dict(), dict()
 
 
     for i in range(len(self.labels)):
       self.precision[i], self.recall[i], _ = precision_recall_curve(self.y_gt[:, i], self.y_pred[:, i])
       self.fpr[i], self.tpr[i], _ = sk_roc_curve(self.y_gt[:, i], self.y_pred[:, i])
 
   def pr_curve(self):
+    '''
+    Plot the Precision-Recall Curve
+    '''
     import plotly.express as px
     fig = px.line(title='PR Curve').update_layout(yaxis_title='Precision', xaxis_title='Recall')
     for i in range(len(self.labels)):
       fig.add_scatter(x=self.recall[i], y=self.precision[i], name=self.labels[i])
 
     return fig
 
   def roc_curve(self):
+    '''
+    Plot the receiver operating charactersitic curve
+    '''
     import plotly.express as px
     fig = px.line(title="ROC Curve").update_layout(yaxis_title='TPR', xaxis_title='FPR')
     for i in range(len(self.labels)):
       fig.add_scatter(x=self.fpr[i], y=self.tpr[i], name=self.labels[i])
 
     return fig
 
 
 class PStats:
+  """
+    Executes cProfile.run and saves the results in the PStats class as panda DataFrames. 
+    Two DataFrames are stored - A summary and a report which call PStats.summary and PStats.report respectively.
+
+    Args:
+      command (string): the command to be analyzed  
+
+    Attributes:
+      profile: tokenized results of cProfile.run() on the command in a list of strings
+
+    Reference:
+      https://docs.python.org/3/library/profile.html
+  """ 
   def __init__(self, command):
     import cProfile
     import io
     from contextlib import redirect_stdout
     f = io.StringIO()
     with redirect_stdout(f):
       cProfile.run(command, sort='tottime')
     self.profile = f.getvalue().split('\n')
 
   @property
   def summary(self):
+    '''Pandas DataFrame summarizing duration of each function'''
     import pstats
     import pandas as pd
     import numpy as np
     cols = ['function calls', 'time']
     summary_data = self.profile[:4]
-#    return summary_data[0].strip()
     data = np.array(summary_data[0].split())[[0,-2]].reshape(1,2)
-#    data = data.astype(float)
     data_ = pd.DataFrame(data)
     data_.columns=cols
     data_['function calls'].astype(int)
     data_['time'].astype(float)
-#    def swap_columns(df, col1, col2):
-#      col_list = list(df.columns)
-#      x, y = col_list.index(col1), col_list.index(col2)
-#      col_list[y], col_list[x] = col_list[x], col_list[y]
-#      df = df[col_list]
-#      return df
     return data_
 
   @property
   def report(self):
+    '''Pandas DataFrame in-depth report of the duration of each call '''
     import pstats
     import pandas as pd
     core_profile = self.profile[4:]
     cols = core_profile[0].split()
     n = len(cols[:-1])
     data = [_.split() for _ in core_profile[1:]]
     data = [_ if len(_)==n+1 else _[:n]+[" ".join(_[n+1:])] for _ in data]
@@ -219,21 +243,21 @@
     Reference:
       https://scikit-learn.org/stable/modules/generated/sklearn.metrics.confusion_matrix.html
 
     Example:
       >>> y_true = [[0, 0, 1], [1, 0, 0], [0, 1, 0], [1, 0, 0], [0, 1, 0]]
       >>> y_pred = [[0, 0, 1], [0, 1, 0], [0, 1, 0], [1, 0, 0], [0, 1, 0]]
       >>> label_names = ['cat', 'dog', 'horse']
-      >>> from explainer.explainers import metrics_explainer
-      >>> cm = metrics_explainer['confusionmatrix'](y_true, y_pred, label_names)
+      >>> from explainer import metrics
+      >>> cm = metrics.confusion_matrix(y_true, y_pred, label_names)
       >>> print(cm.df)
-                 cat  dog  horse
-      cat        0.5  0.5        0.0
-      dog        0.0  1.0        0.0
-      horse  0.0  0.0        1.0
+             cat  dog  horse
+      cat    0.5  0.5    0.0
+      dog    0.0  1.0    0.0
+      horse  0.0  0.0    1.0
 
   """
   cm = ConfusionMatrix(groundtruth, predictions, labels) 
   return cm
 
 
 def plot(groundtruth,predictions,labels):
@@ -254,32 +278,47 @@
     Reference:
       https://scikit-learn.org/stable/modules/generated/sklearn.metrics.precision_recall_curve.html 
 
     Example:
       >>> y_true = [[0, 0, 1], [1, 0, 0], [0, 1, 0], [1, 0, 0], [0, 1, 0]]
       >>> y_pred = [[.002, .09, .89], [.01, .7, .29], [.3, .67, .03], [.55, .4, .05], [.03, .86, .11]]
       >>> label_names = ['cat', 'dog', 'horse']
-      >>> from explainer.explainers import metrics_explainer
-      >>> plotter = metrics_explainer['plot'](y_true, y_pred, label_names)
+      >>> from explainer import metrics
+      >>> plotter = metrics.plot(y_true, y_pred, label_names)
       >>> plotter.recall
       {0: array([1. , 1. , 0.5, 0.5, 0.5, 0. ]), 1: array([1. , 1. , 1. , 0.5, 0.5, 0. ]), 2: array([1., 1., 1., 1., 1., 0.])}
 
   """
   plotter = Plotter(groundtruth,predictions,labels)
   return plotter
 
 
 def pstats(command):
   """
-     Executes cProfile.run and saves the results in the PStats class as panda DataFrames. 
-     Two DataFrames are stored - A summary and a report which call PStats.summary and PStats.report respectively.
+    Executes cProfile.run and saves the results in the PStats class as panda DataFrames. 
+    Two DataFrames are stored - A summary and a report which call PStats.summary and PStats.report respectively.
+
+    Args:
+      command: command to run
 
-     Args:
-       command: command to run
+    Returns:
+      PStats: this class provides summary and report methods to display the DataFrames
+
+    Reference:
+      https://docs.python.org/3/library/profile.html
 
-     Returns:
-       PStats: this class provides summary and report methods to display the DataFrames
 
-     Reference:
-       https://docs.python.org/3/library/profile.html
+    Example:
+      >>> import random
+      >>> from explainer import metrics
+      >>> stats = metrics.pstats('[i**2 for i in range(100000)]')
+      >>> stats.report #doctest:+SKIP
+            ncalls tottime percall cumtime percall                 filename:lineno(function)
+      0      1   0.025   0.025   0.025   0.025                    <string>:1(<listcomp>)
+      1      1   0.001   0.001   0.026   0.026                      <string>:1(<module>)
+      2      1   0.000   0.000   0.027   0.027                     method builtins.exec}
+      3      1   0.000   0.000   0.000   0.000  'disable' of '_lsprof.Profiler' objects}
+      4           None    None    None    None                                      None
+      5           None    None    None    None                                      None
+      6           None    None    None    None                                      None 
   """
   return PStats(command)
```

## explainer/tests/conftest.py

```diff
@@ -1,10 +1,10 @@
 import pytest
 import numpy as np
-import torch, torchvision
+import torch
 from torchvision import datasets, transforms
 from torch import nn, optim
 from torch.nn import functional as F
 torch.manual_seed(0)
 
 @pytest.fixture(scope='session')
 def custom_pyt_CNN():
@@ -75,9 +75,119 @@
     model = Net().to(device)
     optimizer = optim.SGD(model.parameters(), lr=0.01, momentum=0.5)
 
     for epoch in range(1, num_epochs + 1):
         train(model, device, train_loader, optimizer, epoch)
 
     class_names = np.array(['0', '1', '2', '3', '4', '5', '6', '7', '8', '9'])
+    y_true = next(iter(test_loader))[1].to(device)
+    X_test = next(iter(test_loader))[0].to(device)
 
-    return model, test_loader, class_names
+    return model, X_test, class_names, y_true
+
+@pytest.fixture(scope='session')
+def custom_tf_CNN():
+    '''
+    Creates and trains a simple TF CNN on the mnist dataset.
+    Returns the model, a subset of the test dataset and the class names.
+
+    Taken from https://shap-lrjball.readthedocs.io/en/latest/example_notebooks/deep_explainer/Front%20Page%20DeepExplainer%20MNIST%20Example.html
+    '''
+    import tensorflow as tf
+    from tensorflow.keras.datasets import mnist
+    from tensorflow.keras.models import Sequential
+    from tensorflow.keras.layers import (Dense, 
+                                        Dropout,
+                                        Flatten,
+                                        Conv2D,
+                                        MaxPooling2D)
+    from tensorflow.keras import backend as K
+
+    batch_size = 128
+    num_classes = 10
+    epochs = 3 
+
+    # input image dimensions
+    img_rows, img_cols = 28, 28
+
+    # the data, split between train and test sets
+    (X_train, y_train), (X_test, y_test) = mnist.load_data()
+
+    if K.image_data_format() == 'channels_first':
+        X_train = X_train.reshape(X_train.shape[0], 1, img_rows, img_cols)
+        X_test = X_test.reshape(X_test.shape[0], 1, img_rows, img_cols)
+        input_shape = (1, img_rows, img_cols)
+    else:
+        X_train = X_train.reshape(X_train.shape[0], img_rows, img_cols, 1)
+        X_test = X_test.reshape(X_test.shape[0], img_rows, img_cols, 1)
+        input_shape = (img_rows, img_cols, 1)
+
+    X_train = X_train.astype('float32')[:500]
+    X_test = X_test.astype('float32')[:100]
+    X_train /= 255
+    X_test /= 255
+    y_train = y_train[:500]
+    y_test = y_test[:100]
+    print('x_train shape:', X_train.shape)
+    print(X_train.shape[0], 'train samples')
+    print(X_test.shape[0], 'test samples')
+
+    # convert class vectors to binary class matrices
+    y_train = tf.keras.utils.to_categorical(y_train, num_classes)
+    y_test = tf.keras.utils.to_categorical(y_test, num_classes)
+
+    model = Sequential()
+    model.add(Conv2D(32, kernel_size=(3, 3),
+                    activation='relu',
+                    input_shape=input_shape))
+    model.add(Conv2D(64, (3, 3), activation='relu'))
+    model.add(MaxPooling2D(pool_size=(2, 2)))
+    model.add(Dropout(0.25))
+    model.add(Flatten())
+    model.add(Dense(128, activation='relu'))
+    model.add(Dropout(0.5))
+    model.add(Dense(num_classes, activation='softmax'))
+
+    model.compile(loss=tf.keras.losses.categorical_crossentropy,
+                optimizer=tf.keras.optimizers.Adadelta(),
+                metrics=['accuracy'])
+
+    model.fit(X_train, y_train,
+            batch_size=batch_size,
+            epochs=epochs,
+            verbose=1,
+            validation_data=(X_test, y_test))
+
+    return model, X_test[:10], [str(i) for i in range(10)], y_test[:10]
+
+@pytest.fixture(scope='session')
+def dog_cat_image():
+    '''Loads the cat-dog image exampe from imagenet.'''
+    from PIL import Image
+    import requests
+    from io import BytesIO
+    response = requests.get("https://raw.githubusercontent.com/jacobgil/pytorch-grad-cam/master/examples/both.png")
+    return np.array(Image.open(BytesIO(response.content)))
+
+@pytest.fixture(scope='session')
+def tf_VGG():
+    '''Loads the keras.applications VGG16 pretrained on imagenet'''
+    from tensorflow.keras.applications import VGG16
+
+    return VGG16(weights='imagenet')
+
+@pytest.fixture(scope='session')
+def tf_resnet50():
+    '''Loads the keras.applications ResNet50 pretrained on imagenet'''
+    from tensorflow.keras.applications.resnet50 import ResNet50
+
+    return ResNet50(weights='imagenet') 
+
+@pytest.fixture(scope='session')
+def imagenet_class_names():
+    # load the ImageNet class names as a vectorized mapping function from ids to names
+    import shap
+    import json
+    url = "https://s3.amazonaws.com/deep-learning-models/image-models/imagenet_class_index.json"
+    with open(shap.datasets.cache(url)) as file:
+        class_names = [v[1] for v in json.load(file).values()]
+    return class_names
```

## explainer/tests/test_attributions.py

```diff
@@ -13,38 +13,148 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 #
+
 ### libraries to support tests ###
 import pytest
-from deepdiff import DeepDiff
 import numpy as np
 import pandas as pd
+import torch
 import scipy as sp
 import transformers
-import torch
 torch.manual_seed(0)
 ### library to be tested ###
 from explainer import attributions
 from attributions.plots import shap_waterwall_plot
 from attributions.widgets import ShapUI
 ###################################
 
-device = torch.device('cpu')
+@pytest.mark.parametrize("custom_CNN", ['custom_pyt_CNN', 'custom_tf_CNN'])
+def test_DeepExplainer(custom_CNN, request):
+    '''
+    Test every way to instantiate DeepExplainer and PTDeepExplainer objects
+    '''
+    model, X_test, class_names, y_test = request.getfixturevalue(custom_CNN)
+    if isinstance(X_test, torch.Tensor) == True:
+        deViz = attributions.DeepExplainer(model, X_test[:2], X_test[2:4], class_names)
+        assert isinstance(deViz, attributions.PTDeepExplainer) 
+        deViz = attributions.PTDeepExplainer(model, X_test[:2], X_test[2:4], class_names)
+        assert isinstance(deViz, attributions.PTDeepExplainer) 
+        deViz = attributions.deep_explainer(model, X_test[:2], X_test[2:4], class_names)
+        assert isinstance(deViz, attributions.PTDeepExplainer) 
+    else:
+        deViz = attributions.DeepExplainer(model, X_test[:2], X_test[2:4], class_names)
+        assert isinstance(deViz, attributions.DeepExplainer) 
+        deViz = attributions.deep_explainer(model, X_test[:2], X_test[2:4], class_names)
+        assert isinstance(deViz, attributions.DeepExplainer) 
+    deViz.visualize()
 
-def test_deep_explainer(custom_pyt_CNN):
-    model, test_loader, class_names = custom_pyt_CNN 
-    X_test = next(iter(test_loader))[0].to(device)
-    deViz = attributions.deep_explainer(model, X_test[:2], X_test[2:4], class_names)
-    assert isinstance(deViz, attributions.attributions.DeepExplainer) 
+@pytest.mark.parametrize("custom_CNN", ['custom_pyt_CNN', 'custom_tf_CNN'])
+def test_DeepExplainer_one_image(custom_CNN, request):
+    '''
+    Test edge case of one image input (with 1 and 2 background images)
+    '''
+    model, X_test, class_names, y_test = request.getfixturevalue(custom_CNN)
+    deViz = attributions.deep_explainer(model, X_test[:1], X_test[2:3], class_names)
+    deViz = attributions.deep_explainer(model, X_test[:1], X_test[2:4], class_names)
     deViz.visualize()
 
+@pytest.mark.parametrize("custom_CNN", ['custom_pyt_CNN', 'custom_tf_CNN'])
+def test_GradientExplainer(custom_CNN, request):
+    '''
+    Test every way to instantiate GradientExplainer and PTGradientExplainer objects
+    '''
+    model, X_test, class_names, y_test = request.getfixturevalue(custom_CNN)
+    if isinstance(X_test, torch.Tensor) == True:
+        geViz = attributions.GradientExplainer(model, X_test[:2], X_test[2:4], class_names)
+        assert isinstance(geViz, attributions.PTGradientExplainer) 
+        geViz = attributions.PTGradientExplainer(model, X_test[:2], X_test[2:4], class_names)
+        assert isinstance(geViz, attributions.PTGradientExplainer) 
+        geViz = attributions.gradient_explainer(model, X_test[:2], X_test[2:4], class_names)
+        assert isinstance(geViz, attributions.PTGradientExplainer) 
+    else:
+        geViz = attributions.GradientExplainer(model, X_test[:2], X_test[2:4], class_names)
+        assert isinstance(geViz, attributions.GradientExplainer) 
+        geViz = attributions.gradient_explainer(model, X_test[:2], X_test[2:4], class_names)
+        assert isinstance(geViz, attributions.GradientExplainer) 
+    geViz.visualize()
+
+@pytest.mark.parametrize("custom_CNN", ['custom_pyt_CNN', 'custom_tf_CNN'])
+def test_GradientExplainer_one_image(custom_CNN, request):
+    '''
+    Test edge case of one image input (with 1 and 2 background images and 1 and 2 ranked outputs)
+    '''
+    model, X_test, class_names, y_test = request.getfixturevalue(custom_CNN)
+    geViz = attributions.gradient_explainer(model, X_test[:1], X_test[2:3], class_names, 1)
+    geViz = attributions.gradient_explainer(model, X_test[:1], X_test[2:3], class_names, 2)
+    geViz = attributions.gradient_explainer(model, X_test[:1], X_test[2:4], class_names, 1)
+    geViz = attributions.gradient_explainer(model, X_test[:1], X_test[2:4], class_names, 2)
+    geViz.visualize()
+
+def test_partition_image(tf_resnet50, dog_cat_image, imagenet_class_names):
+    from tensorflow.keras.applications.resnet50 import preprocess_input
+    def f(X):
+        tmp = X.copy()
+        preprocess_input(tmp)
+        return tf_resnet50(tmp)
+
+    image = np.expand_dims(dog_cat_image, axis=0) 
+
+    # test generator class manually
+    pe = attributions.PartitionExplainer('image', f, imagenet_class_names, image[0].shape)
+    pe.run_explainer(image)
+    assert isinstance(pe, attributions.PartitionImageExplainer)
+    pe.visualize()
+
+    # test explicit class
+    pe = attributions.PartitionImageExplainer('image', f, imagenet_class_names,image[0].shape)
+    pe.run_explainer(image)
+    assert isinstance(pe, attributions.PartitionImageExplainer)
+    pe.visualize()
+
+    # test module function
+    pe = attributions.partition_image_explainer(f, imagenet_class_names, image)
+    assert isinstance(pe, attributions.PartitionImageExplainer)
+    pe.visualize()
+
+def test_partition_text():
+    labels = ['sadness', 'joy', 'love', 'anger', 'fear', 'surprise']
+    tokenizer = transformers.AutoTokenizer.from_pretrained("nateraw/bert-base-uncased-emotion", use_fast=True)
+    model = transformers.AutoModelForSequenceClassification.from_pretrained("nateraw/bert-base-uncased-emotion")
+
+    def f(x):
+        tv = torch.tensor([tokenizer.encode(v, padding='max_length', max_length=128, truncation=True) for v in x])
+        attention_mask = (tv!=0).type(torch.int64)
+        outputs = model(tv,attention_mask=attention_mask)[0].detach().cpu().numpy()
+        scores = (np.exp(outputs).T / np.exp(outputs).sum(-1)).T
+        val = sp.special.logit(scores)
+        return val
+    
+    # test generator class manually
+    pe = attributions.PartitionExplainer('text', f, labels, tokenizer)
+    pe.run_explainer(['i didnt feel humiliated'])
+    assert isinstance(pe, attributions.PartitionTextExplainer)
+    pe.visualize()
+
+    # test explicit class 
+    pe = attributions.PartitionTextExplainer('text', f, labels, tokenizer)
+    pe.run_explainer(['i didnt feel humiliated'])
+    assert isinstance(pe, attributions.PartitionTextExplainer)
+    pe.visualize()
+
+    # test module function
+    pe = attributions.partition_text_explainer(f, labels, ['i didnt feel humiliated'], tokenizer)
+    assert isinstance(pe, attributions.PartitionTextExplainer)
+    pe.visualize()
+
+
 def test_shap_waterwall_plot():
     kwargs = dict(expected_value=.5,
                   shap_values=np.random.normal(0, 1, 10),
                   feature_values=np.random.rand(10),
                   columns=list(range(10)),
                   y_true=0)
```

## explainer/tests/test_cam.py

```diff
@@ -18,23 +18,56 @@
 # SPDX-License-Identifier: Apache-2.0
 #
 ### libraries to support tests ###
 import pytest
 import torch 
 torch.manual_seed(0)
 ### library to be tested ###
-from explainer import cam 
+from explainer import cam
 ###################################
 
 device = torch.device('cpu')
 
-def test_grad_cam(custom_pyt_CNN):
-    model, test_loader, class_names = custom_pyt_CNN 
-    X_test = next(iter(test_loader))[0].to(device)[0]
-    image = torch.movedim(X_test, 0, 2).numpy()
+def test_x_gradcam(custom_pyt_CNN):
+    model, X_test, class_names, y_test = custom_pyt_CNN 
+    image = torch.movedim(X_test[0], 0, 2).numpy()
     target_layer = model.conv_layers
     # use the highest-scoring category as the target class
     target_class = None
     image_dims = (28, 28)
-    gcam = cam.xgradcam(model, target_layer, target_class, image, image_dims, device)
+    gcam = cam.x_gradcam(model, target_layer, target_class, image, image_dims)
     assert isinstance(gcam, cam.XGradCAM)
     gcam.visualize()
+
+def test_tf_gradcam_vgg(tf_VGG, dog_cat_image):
+    target_class = 281
+    target_layer = tf_VGG.get_layer('block5_conv3')
+    gcam = cam.tf_gradcam(tf_VGG, target_layer, target_class, dog_cat_image)
+    assert isinstance(gcam, cam.TFGradCAM)
+    gcam.visualize()
+
+def test_tf_gradcam_resnet50(tf_resnet50, dog_cat_image):
+    target_class = 281
+    target_layer = tf_resnet50.get_layer('conv5_block3_out')
+    gcam = cam.tf_gradcam(tf_resnet50, target_layer, target_class, dog_cat_image)
+    assert isinstance(gcam, cam.TFGradCAM)
+    gcam.visualize()
+
+def test_gradcam_tf_resnet50(tf_resnet50, dog_cat_image):
+    target_class = 281
+    target_layer = tf_resnet50.get_layer('conv5_block3_out')
+    gcam = cam.GradCAM(tf_resnet50, target_layer)
+    gcam.run_explainer(dog_cat_image, target_class)
+    assert isinstance(gcam, cam.TFGradCAM)
+    gcam.visualize()
+
+def test_gradcam_pytorch(custom_pyt_CNN):
+    model, X_test, class_names, y_test = custom_pyt_CNN 
+    image = torch.movedim(X_test[0], 0, 2).numpy()
+    target_layer = model.conv_layers
+    # use the highest-scoring category as the target class
+    target_class = None
+    image_dims = (28, 28)
+    gcam = cam.GradCAM(model, target_layer, image_dims)
+    gcam.run_explainer(image, target_class)
+    assert isinstance(gcam, cam.XGradCAM)
+    gcam.visualize()
```

## explainer/tests/test_metrics.py

```diff
@@ -25,23 +25,24 @@
 import pandas as pd
 import torch
 ### library to be tested ###
 from explainer import metrics
 ###################################
 
 # Namedtuple that holds necessary input and outputs to the cm and curve plots.
-Data = namedtuple('Data', ['y_true', 'y_pred', 'label_names', 'recall', 'cm'])
+Data = namedtuple('Data', ['y_true', 'oh_y_true', 'y_pred', 'label_names', 'recall', 'cm'])
 
 @pytest.fixture(scope='session')
 def simple_data():
     '''
     A simple 3-class use case with only 5 examples.
 
     '''
-    y_true = [[0, 0, 1], [1, 0, 0], [0, 1, 0], [1, 0, 0], [0, 1, 0]]
+    y_true = [2, 0, 1, 0, 1]
+    oh_y_true = [[0, 0, 1], [1, 0, 0], [0, 1, 0], [1, 0, 0], [0, 1, 0]]
     y_pred = [
         [.002, .09, .89],
         [.01, .7, .29],
         [.3, .67, .03],
         [.55, .4, .05],
         [.03, .86, .11]]
     label_names = ['cat', 'dog', 'horse']
@@ -53,45 +54,35 @@
         }
     cm = pd.DataFrame(
         {label_names[0]: [0.5, 0.0, 0.0],
          label_names[1]: [0.5, 1.0, 0.0],
          label_names[2]: [0.0, 0.0, 1.0]},
          index=label_names)
 
-    return Data(y_true, y_pred, label_names, recall, cm)
+    return Data(y_true, oh_y_true, y_pred, label_names, recall, cm)
 
 @pytest.mark.simple
 def test_plot(simple_data):
     data = simple_data
     plotter = metrics.plot(data.y_true, data.y_pred, data.label_names)
     assert DeepDiff(plotter.recall, data.recall) == {}
 
 @pytest.mark.simple
 def test_confusion_matrix(simple_data):
     data = simple_data
+    # test without one-hot-encoding
     cm = metrics.confusion_matrix(data.y_true, data.y_pred, data.label_names)
     assert cm.df.equals(data.cm)
+    # test with one-hot-encoding
+    cm = metrics.confusion_matrix(data.oh_y_true, data.y_pred, data.label_names)
+    assert cm.df.equals(data.cm)
 
 def test_confusion_matrix_pyt(custom_pyt_CNN):
-    device = torch.device('cpu')
-    model, test_loader, class_names = custom_pyt_CNN 
+    model, X_test, class_names, y_true = custom_pyt_CNN 
 
     # test the model
     model.eval()
-    test_loss = 0
-    correct = 0
-    y_true = torch.empty(0)
-    y_pred = torch.empty((0, 10))
-    X_test = torch.empty((0, 1, 28, 28))
-
     with torch.no_grad():
-        for data, target in test_loader:
-            data, target = data.to(device), target.to(device)
-            output = model(data)
-            X_test = torch.cat((X_test, data))
-            y_true, y_pred = torch.cat((y_true, target)), torch.cat((y_pred, output))
-    
-    # one-hot-encode for metrics explanation
-    oh_y_true = torch.from_numpy(np.eye(int(torch.max(y_true)+1))[list(y_true.numpy().astype(int))])
-    cm = metrics.confusion_matrix(oh_y_true, y_pred, class_names)
+        output = model(X_test)
+    cm = metrics.confusion_matrix(y_true, output, class_names)
     assert isinstance(cm, metrics.metrics.ConfusionMatrix)
     cm.visualize()
```

## Comparing `intel_xai-0.3.1.dev20230608.dist-info/LICENSE` & `intel_xai-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `intel_xai-0.3.1.dev20230608.dist-info/METADATA` & `intel_xai-0.5.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intel-xai
-Version: 0.3.1.dev20230608
+Version: 0.5.0
 Summary: Intel® Explainable AI Tools
 Home-page: https://github.com/IntelAI/intel-xai-tools
 Author: IntelAI
 Author-email: IntelAI@intel.com
 License: Apache 2.0
 Keywords: XAI,explainer
 Platform: any
@@ -18,41 +18,52 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.9,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: captum
-Requires-Dist: intel-tensorflow (==2.11.0)
-Requires-Dist: ipywidgets
-Requires-Dist: numpy (<1.23.0,>=1.14.3)
-Requires-Dist: opencv-python
-Requires-Dist: scikit-plot
-Requires-Dist: scipy
-Requires-Dist: shap
+Requires-Dist: captum (~=0.6.0)
+Requires-Dist: intel-tensorflow (==2.12.0)
+Requires-Dist: ipywidgets (~=7.7.5)
+Requires-Dist: numpy (~=1.22.4)
+Requires-Dist: opencv-python (~=4.7.0.72)
+Requires-Dist: plotly (~=5.15.0)
+Requires-Dist: scikit-plot (~=0.3.7)
+Requires-Dist: scipy (~=1.10.1)
+Requires-Dist: shap (~=0.41.0)
 Requires-Dist: torch (==1.13.1)
-Requires-Dist: transformers
-Requires-Dist: plotly (==5.14.1)
-Requires-Dist: grad-cam
-Requires-Dist: matplotlib
-Requires-Dist: pandas
-Requires-Dist: plotly
-Requires-Dist: scikit-learn
-Requires-Dist: seaborn
+Requires-Dist: transformers (~=4.30.0)
+Requires-Dist: grad-cam (==1.4.6)
+Requires-Dist: matplotlib (~=3.7.1)
+Requires-Dist: pandas (~=1.5.3)
+Requires-Dist: scikit-learn (~=1.2.2)
+Requires-Dist: seaborn (~=0.12.2)
+Requires-Dist: Jinja2 (~=3.1.2)
+Requires-Dist: absl-py (~=1.4.0)
+Requires-Dist: attrs (~=21.4.0)
+Requires-Dist: grpcio-status (~=1.48.2)
+Requires-Dist: joblib (~=1.2.0)
+Requires-Dist: jsonschema[format-nongpl] (~=4.17.3)
+Requires-Dist: protobuf (~=3.20.3)
+Requires-Dist: semantic-version (~=2.10.0)
+Requires-Dist: tensorflow-data-validation (~=1.13.0)
+Requires-Dist: tensorflow-model-analysis (~=0.44.0)
+Requires-Dist: dataclasses (~=2.10.1) ; python_version < "3.7"
 Provides-Extra: pytorch
 Requires-Dist: torch (==1.13.1) ; extra == 'pytorch'
 Requires-Dist: torchvision (==0.14.1) ; extra == 'pytorch'
 Provides-Extra: test
-Requires-Dist: deepdiff ; extra == 'test'
-Requires-Dist: pytest ; extra == 'test'
-Requires-Dist: tensorflow-hub ; extra == 'test'
+Requires-Dist: datasets (~=2.10.1) ; extra == 'test'
+Requires-Dist: deepdiff (~=6.3.0) ; extra == 'test'
+Requires-Dist: pytest (~=7.3.2) ; extra == 'test'
+Requires-Dist: tensorflow-hub (~=0.13.0) ; extra == 'test'
 Requires-Dist: torch (==1.13.1) ; extra == 'test'
 Requires-Dist: torchvision (==0.14.1) ; extra == 'test'
 
 # Intel® Explainable AI Tools
 
 This repository provides tools for data scientists and MLOps engineers that have requirements specific to AI model interpretability.
 
@@ -65,39 +76,33 @@
   * Creates interactive HTML reports containing model performance and fairness metrics
 * [Explainer](explainer)
   * Runs post-hoc model distillation and visualization methods to examine predictive behavior for both TensorFlow* and PyTorch* models via a simple Python API including the following modules:
     * [Attributions](explainer/attributions/): Visualize negative and positive attributions of tabular features, pixels, and word tokens for predictions
     * [CAM (Class Activation Mapping)](explainer/cam/): Create heatmaps for CNN image classifications using gradient-weight class activation CAM mapping
     * [Metrics](explainer/metrics/): Gain insight into models with the measurements and visualizations needed during the machine learning workflow
 
-
-  * [ShapUI](explainer/attributions/widgets.py#L254): A user interface to explore and compare impact scores of model predictions for each record of a tabular data set and discover insights of a model's behavior:
-    * **Error Analysis** allows the user to filter data points based on their error type.
-    * **Impact Analysis** allows users to filter data points based on their associated SHAP impact score for top important features.
-    * **Feature Analysis** allows users to filter data points by feature values for top important features.
-
 ## Get Started
 
 ### Requirements
 * Linux system or WSL2 on Windows (validated on Ubuntu* 20.04/22.04 LTS)
-* Python 3.9 or 3.10
+* Python 3.9
 * Install required OS packages with `apt-get install build-essential python3-dev`
 * git (only required for the "Developer Installation")
 
 ### Create and activate a Python3 virtual environment
 We encourage you to use a python virtual environment (virtualenv or conda) for consistent package management.
 There are two ways to do this:
 
 a. Using `virtualenv`:
    ```
    python3.9 -m virtualenv xai_env
    source xai_env/bin/activate
    ```
 
-   Or `conda`:
+b. Or `conda`:
    ```
    conda create --name xai_env python=3.9
    conda activate xai_env
    ```
 
 ### Basic Installation
 ```
@@ -115,33 +120,44 @@
    cd intel-xai-tools
    ```
 2. Install the Intel Explainable AI Tools using the following command:
    ```
    make install
    ```
 
+### Additional Feature-Specific Steps
+Notebooks may require additional dependencies listed in their associated documentation.
+
+### Verify Installation
+
+Verify that your installation was successful by using the following commands, which display the Explainer and Model Card Generator versions:
+```
+python -c "from explainer import version; print(version.__version__)"
+python -c "from model_card_gen import version; print(version.__version__)"
+```
+
 ## Running Notebooks
 
 The following links have Jupyter* notebooks showing how to use the Explainer and Model Card Generator APIs in various ML domains and use cases:
-* [Model Card Generator Notebooks](/model_card_gen/notebooks)
-* [Explainer Notebooks](notebooks/)
+* [Model Card Generator Notebooks](notebooks#model-card-generator-tutorial-notebooks)
+* [Explainer Notebooks](notebooks#explainer-tutorial-notebooks)
 
 ## Support
 
 The Intel Explainable AI Tools team tracks bugs and enhancement requests using
 [GitHub issues](https://github.com/intelai/intel-xai-tools/issues). Before submitting a
 suggestion or bug report, search the existing GitHub issues to see if your issue has already been reported.
 
 *Other names and brands may be claimed as the property of others. [Trademarks](http://www.intel.com/content/www/us/en/legal/trademarks.html)
 
-#### DISCLAIMER: ####
+#### DISCLAIMER
 These scripts are not intended for benchmarking Intel platforms. For any performance and/or benchmarking information on specific Intel platforms, visit https://www.intel.ai/blog.
  
 Intel is committed to the respect of human rights and avoiding complicity in human rights abuses, a policy reflected in the Intel Global Human Rights Principles. Accordingly, by accessing the Intel material on this platform you agree that you will not use the material in a product or application that causes or contributes to a violation of an internationally recognized human right.
  
-#### License: ####
+#### License
 Intel® Explainable AI Tools is licensed under Apache License Version 2.0.
  
-#### Datasets: ####
+#### Datasets
 To the extent that any public datasets are referenced by Intel or accessed using tools or code on this site those datasets are provided by the third party indicated as the data source. Intel does not create the data, or datasets, and does not warrant their accuracy or quality. By accessing the public dataset(s) you agree to the terms associated with those datasets and that your use complies with the applicable license. [DATASETS](DATASETS.md)
  
 Intel expressly disclaims the accuracy, adequacy, or completeness of any public datasets, and is not liable for any errors, omissions, or defects in the data, or for any reliance on the data.  Intel is not liable for any liability or damages relating to your use of public datasets.
```

