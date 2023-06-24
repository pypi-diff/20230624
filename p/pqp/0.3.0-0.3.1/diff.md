# Comparing `tmp/pqp-0.3.0.tar.gz` & `tmp/pqp-0.3.1.tar.gz`

## Comparing `pqp-0.3.0.tar` & `pqp-0.3.1.tar`

### file list

```diff
@@ -1,193 +1,205 @@
--rw-r--r--   0        0        0      273 1970-01-01 00:00:00.000000 pqp-0.3.0/Cargo.toml
--rw-r--r--   0      501       20    53248 2023-03-17 07:12:19.000000 pqp-0.3.0/.coverage
--rw-r--r--   0      501       20      105 2023-02-01 03:34:57.000000 pqp-0.3.0/.gitignore
--rw-r--r--   0      501       20      579 2023-02-25 01:53:51.000000 pqp-0.3.0/CHANGELOG.md
--rw-r--r--   0      501       20     1145 2023-02-01 03:55:07.000000 pqp-0.3.0/CONTRIBUTING.md
--rw-r--r--   0      501       20     1047 2023-02-01 03:34:57.000000 pqp-0.3.0/LICENSE.txt
--rw-r--r--   0      501       20     1273 2023-02-01 03:56:12.000000 pqp-0.3.0/README.md
--rw-r--r--   0      501       20      333 2023-02-01 03:34:57.000000 pqp-0.3.0/publish_docs.sh
--rw-r--r--   0      501       20      812 2023-04-01 13:18:05.000000 pqp-0.3.0/pyproject.toml
--rw-r--r--   0      501       20       38 2023-03-01 09:39:53.000000 pqp-0.3.0/python/.gitignore
--rw-r--r--   0      501       20        0 2023-02-01 03:34:57.000000 pqp-0.3.0/python/conftest.py
--rw-r--r--   0      501       20       12 2023-02-01 03:34:57.000000 pqp-0.3.0/python/docs/.gitignore
--rw-r--r--   0      501       20      850 2023-03-31 02:19:59.000000 pqp-0.3.0/python/docs/Makefile
--rw-r--r--   0      501       20      804 2023-02-01 03:34:57.000000 pqp-0.3.0/python/docs/make.bat
--rw-r--r--   0      501       20      280 2023-03-31 02:41:09.000000 pqp-0.3.0/python/docs/source/api/pqp.data.BinaryDomain.rst
--rw-r--r--   0      501       20      442 2023-03-31 02:41:09.000000 pqp-0.3.0/python/docs/source/api/pqp.data.CategoricalDomain.rst
--rw-r--r--   0      501       20      286 2023-03-31 02:41:09.000000 pqp-0.3.0/python/docs/source/api/pqp.data.ContinuousDomain.rst
--rw-r--r--   0      501       20      412 2023-03-31 02:41:09.000000 pqp-0.3.0/python/docs/source/api/pqp.data.Data.rst
--rw-r--r--   0      501       20      268 2023-03-31 02:41:09.000000 pqp-0.3.0/python/docs/source/api/pqp.data.DiscreteDomain.rst
--rw-r--r--   0      501       20      441 2023-03-31 02:41:09.000000 pqp-0.3.0/python/docs/source/api/pqp.data.Domain.rst
--rw-r--r--   0      501       20      478 2023-03-31 02:41:09.000000 pqp-0.3.0/python/docs/source/api/pqp.data.IntegerDomain.rst
--rw-r--r--   0      501       20      272 2023-03-31 02:41:09.000000 pqp-0.3.0/python/docs/source/api/pqp.data.RealDomain.rst
--rw-r--r--   0      501       20      102 2023-03-31 02:41:09.000000 pqp-0.3.0/python/docs/source/api/pqp.data.infer_domain_type.rst
--rw-r--r--   0      501       20       84 2023-03-31 02:41:09.000000 pqp-0.3.0/python/docs/source/api/pqp.data.make_domain.rst
--rw-r--r--   0      501       20      279 2023-03-31 03:04:18.000000 pqp-0.3.0/python/docs/source/api/pqp.estimation.EstimationResult.rst
--rw-r--r--   0      501       20      764 2023-03-31 02:27:29.000000 pqp-0.3.0/python/docs/source/api/pqp.estimation.Estimator.rst
--rw-r--r--   0      501       20      973 2023-03-31 02:27:29.000000 pqp-0.3.0/python/docs/source/api/pqp.estimation.MultinomialEstimator.rst
--rw-r--r--   0      501       20      307 2023-02-01 03:34:57.000000 pqp-0.3.0/python/docs/source/api/pqp.expression.Expression.rst
--rw-r--r--   0      501       20      234 2023-02-01 03:34:57.000000 pqp-0.3.0/python/docs/source/api/pqp.expression.Hedge.rst
--rw-r--r--   0      501       20      246 2023-02-01 03:34:57.000000 pqp-0.3.0/python/docs/source/api/pqp.expression.Marginal.rst
--rw-r--r--   0      501       20      218 2023-02-01 03:34:57.000000 pqp-0.3.0/python/docs/source/api/pqp.expression.P.rst
--rw-r--r--   0      501       20      242 2023-02-01 03:34:57.000000 pqp-0.3.0/python/docs/source/api/pqp.expression.Product.rst
--rw-r--r--   0      501       20      246 2023-02-01 03:34:57.000000 pqp-0.3.0/python/docs/source/api/pqp.expression.Quotient.rst
--rw-r--r--   0      501       20       87 2023-02-01 03:34:57.000000 pqp-0.3.0/python/docs/source/api/pqp.expression.parse_json.rst
--rw-r--r--   0      501       20      113 2023-02-01 03:34:57.000000 pqp-0.3.0/python/docs/source/api/pqp.graph.BidirectedEdge.rst
--rw-r--r--   0      501       20      107 2023-02-01 03:34:57.000000 pqp-0.3.0/python/docs/source/api/pqp.graph.DirectedEdge.rst
--rw-r--r--   0      501       20      435 2023-02-01 03:34:57.000000 pqp-0.3.0/python/docs/source/api/pqp.graph.Graph.rst
--rw-r--r--   0      501       20      294 2023-03-31 04:09:43.000000 pqp-0.3.0/python/docs/source/api/pqp.identification.ATE.rst
--rw-r--r--   0      501       20      310 2023-03-31 04:09:43.000000 pqp-0.3.0/python/docs/source/api/pqp.identification.AbstractCausalEstimand.rst
--rw-r--r--   0      501       20      122 2023-03-31 04:09:43.000000 pqp-0.3.0/python/docs/source/api/pqp.identification.BidirectedEdge.rst
--rw-r--r--   0      501       20      295 2023-03-31 04:09:43.000000 pqp-0.3.0/python/docs/source/api/pqp.identification.CATE.rst
--rw-r--r--   0      501       20      278 2023-03-31 04:09:43.000000 pqp-0.3.0/python/docs/source/api/pqp.identification.CausalEstimand.rst
--rw-r--r--   0      501       20      116 2023-03-31 04:09:43.000000 pqp-0.3.0/python/docs/source/api/pqp.identification.DirectedEdge.rst
--rw-r--r--   0      501       20      624 2023-03-31 04:09:43.000000 pqp-0.3.0/python/docs/source/api/pqp.identification.Graph.rst
--rw-r--r--   0      501       20      140 2023-03-31 04:09:43.000000 pqp-0.3.0/python/docs/source/api/pqp.identification.IdentificationResult.rst
--rw-r--r--   0      501       20      103 2023-03-31 02:27:29.000000 pqp-0.3.0/python/docs/source/api/pqp.refutation.Operation.rst
--rw-r--r--   0      501       20      586 2023-03-31 02:27:29.000000 pqp-0.3.0/python/docs/source/api/pqp.refutation.Result.rst
--rw-r--r--   0      501       20      408 2023-03-31 02:27:29.000000 pqp-0.3.0/python/docs/source/api/pqp.refutation.Step.rst
--rw-r--r--   0      501       20       87 2023-03-31 02:27:29.000000 pqp-0.3.0/python/docs/source/api/pqp.refutation.entrypoint.rst
--rw-r--r--   0      501       20      730 2023-03-31 02:27:29.000000 pqp-0.3.0/python/docs/source/api/pqp.symbols.AbstractExpression.rst
--rw-r--r--   0      501       20      314 2023-03-31 02:27:29.000000 pqp-0.3.0/python/docs/source/api/pqp.symbols.AbstractMath.rst
--rw-r--r--   0      501       20      522 2023-03-31 02:27:30.000000 pqp-0.3.0/python/docs/source/api/pqp.symbols.Difference.rst
--rw-r--r--   0      501       20      319 2023-03-31 02:27:30.000000 pqp-0.3.0/python/docs/source/api/pqp.symbols.EqualityEvent.rst
--rw-r--r--   0      501       20      238 2023-03-31 02:27:30.000000 pqp-0.3.0/python/docs/source/api/pqp.symbols.Event.rst
--rw-r--r--   0      501       20      531 2023-03-31 02:27:30.000000 pqp-0.3.0/python/docs/source/api/pqp.symbols.Expectation.rst
--rw-r--r--   0      501       20      435 2023-03-31 02:27:30.000000 pqp-0.3.0/python/docs/source/api/pqp.symbols.Hedge.rst
--rw-r--r--   0      501       20      397 2023-03-31 02:27:30.000000 pqp-0.3.0/python/docs/source/api/pqp.symbols.InterventionEvent.rst
--rw-r--r--   0      501       20      504 2023-03-31 02:27:30.000000 pqp-0.3.0/python/docs/source/api/pqp.symbols.Marginal.rst
--rw-r--r--   0      501       20      777 2023-03-31 02:27:30.000000 pqp-0.3.0/python/docs/source/api/pqp.symbols.P.rst
--rw-r--r--   0      501       20      495 2023-03-31 02:27:30.000000 pqp-0.3.0/python/docs/source/api/pqp.symbols.Product.rst
--rw-r--r--   0      501       20      504 2023-03-31 02:27:30.000000 pqp-0.3.0/python/docs/source/api/pqp.symbols.Quotient.rst
--rw-r--r--   0      501       20      121 2023-03-31 02:27:30.000000 pqp-0.3.0/python/docs/source/api/pqp.symbols.StatisticalEvent.rst
--rw-r--r--   0      501       20      477 2023-03-31 02:27:30.000000 pqp-0.3.0/python/docs/source/api/pqp.symbols.Value.rst
--rw-r--r--   0      501       20      243 2023-03-31 02:27:30.000000 pqp-0.3.0/python/docs/source/api/pqp.symbols.Variable.rst
--rw-r--r--   0      501       20       60 2023-03-31 02:27:30.000000 pqp-0.3.0/python/docs/source/api/pqp.symbols.do.rst
--rw-r--r--   0      501       20       81 2023-03-31 02:27:30.000000 pqp-0.3.0/python/docs/source/api/pqp.symbols.make_vars.rst
--rw-r--r--   0      501       20       84 2023-03-31 02:27:30.000000 pqp-0.3.0/python/docs/source/api/pqp.symbols.parse_json.rst
--rw-r--r--   0      501       20       95 2023-03-31 02:27:29.000000 pqp-0.3.0/python/docs/source/api/pqp.utils.attrdict.rst
--rw-r--r--   0      501       20      127 2023-03-31 02:27:29.000000 pqp-0.3.0/python/docs/source/api/pqp.utils.exceptions.DomainValidationError.rst
--rw-r--r--   0      501       20      127 2023-03-31 02:27:29.000000 pqp-0.3.0/python/docs/source/api/pqp.utils.exceptions.InferredDomainWarning.rst
--rw-r--r--   0      501       20      106 2023-03-31 02:27:29.000000 pqp-0.3.0/python/docs/source/api/pqp.utils.exceptions.NumericalError.rst
--rw-r--r--   0      501       20      121 2023-03-31 02:27:29.000000 pqp-0.3.0/python/docs/source/api/pqp.utils.exceptions.PositivityException.rst
--rw-r--r--   0      501       20      115 2023-03-31 02:27:29.000000 pqp-0.3.0/python/docs/source/api/pqp.utils.exceptions.UnitDomainWarning.rst
--rw-r--r--   0      501       20       85 2023-03-31 02:27:29.000000 pqp-0.3.0/python/docs/source/api/pqp.utils.order_graph.rst
--rw-r--r--   0      501       20       94 2023-03-31 02:27:29.000000 pqp-0.3.0/python/docs/source/api/pqp.utils.recursive_sort.rst
--rw-r--r--   0      501       20      113 2023-03-31 02:27:29.000000 pqp-0.3.0/python/docs/source/api/pqp.utils.staticproperty.rst
--rw-r--r--   0      501       20      244 2023-02-01 03:34:57.000000 pqp-0.3.0/python/docs/source/api/pqp.variable.Variable.rst
--rw-r--r--   0      501       20       82 2023-02-01 03:34:57.000000 pqp-0.3.0/python/docs/source/api/pqp.variable.make_vars.rst
--rw-r--r--   0      501       20     1483 2023-02-01 04:08:19.000000 pqp-0.3.0/python/docs/source/conf.py
--rw-r--r--   0      501       20       42 2023-02-01 03:34:57.000000 pqp-0.3.0/python/docs/source/example_notebooks.rst
--rw-r--r--   0      501       20   238718 2023-02-01 03:34:57.000000 pqp-0.3.0/python/docs/source/favicon.ico
--rw-r--r--   0      501       20    19314 2023-02-01 03:34:57.000000 pqp-0.3.0/python/docs/source/imgs/frontdoor_estimator.png
--rw-r--r--   0      501       20    18477 2023-02-01 03:34:57.000000 pqp-0.3.0/python/docs/source/imgs/frontdoor_new.png
--rw-r--r--   0      501       20    97789 2023-02-01 03:34:57.000000 pqp-0.3.0/python/docs/source/imgs/frontdoor_viz.png
--rw-r--r--   0      501       20    37703 2023-03-31 05:48:21.000000 pqp-0.3.0/python/docs/source/imgs/qs_causal_estimand.png
--rw-r--r--   0      501       20    75030 2023-03-31 05:55:41.000000 pqp-0.3.0/python/docs/source/imgs/qs_stat_estimand.png
--rw-r--r--   0      501       20      809 2023-03-31 06:13:18.000000 pqp-0.3.0/python/docs/source/index.rst
--rw-r--r--   0      501       20       24 2023-03-31 02:39:47.000000 pqp-0.3.0/python/docs/source/module_maps/data.rst
--rw-r--r--   0      501       20       30 2023-03-31 02:21:59.000000 pqp-0.3.0/python/docs/source/module_maps/estimation.rst
--rw-r--r--   0      501       20       36 2023-03-31 02:28:16.000000 pqp-0.3.0/python/docs/source/module_maps/exceptions.rst
--rw-r--r--   0      501       20       34 2023-03-31 02:22:26.000000 pqp-0.3.0/python/docs/source/module_maps/identification.rst
--rw-r--r--   0      501       20       30 2023-03-31 02:23:26.000000 pqp-0.3.0/python/docs/source/module_maps/refutation.rst
--rw-r--r--   0      501       20       27 2023-03-31 02:22:32.000000 pqp-0.3.0/python/docs/source/module_maps/symbols.rst
--rw-r--r--   0      501       20       46 2023-02-01 03:34:57.000000 pqp-0.3.0/python/docs/source/modules.rst
--rw-r--r--   0      501       20      432 2023-03-31 02:20:15.000000 pqp-0.3.0/python/docs/source/pqp.data.rst
--rw-r--r--   0      501       20      548 2023-03-31 02:20:15.000000 pqp-0.3.0/python/docs/source/pqp.estimation.rst
--rw-r--r--   0      501       20      534 2023-03-31 02:20:15.000000 pqp-0.3.0/python/docs/source/pqp.identification.rst
--rw-r--r--   0      501       20      340 2023-03-31 02:20:15.000000 pqp-0.3.0/python/docs/source/pqp.refutation.rst
--rw-r--r--   0      501       20      419 2023-03-31 02:20:15.000000 pqp-0.3.0/python/docs/source/pqp.rst
--rw-r--r--   0      501       20     1051 2023-03-31 02:20:16.000000 pqp-0.3.0/python/docs/source/pqp.symbols.rst
--rw-r--r--   0      501       20      456 2023-03-31 02:20:16.000000 pqp-0.3.0/python/docs/source/pqp.utils.rst
--rw-r--r--   0      501       20     6082 2023-04-01 02:03:49.000000 pqp-0.3.0/python/docs/source/quickstart.rst
--rw-r--r--   0      501       20       16 2023-02-01 03:34:57.000000 pqp-0.3.0/python/pqp/.gitignore
--rw-r--r--   0      501       20      276 2023-03-18 05:47:28.000000 pqp-0.3.0/python/pqp/__init__.py
--rw-r--r--   0      501       20       60 2023-03-31 02:50:56.000000 pqp-0.3.0/python/pqp/data/__init__.py
--rw-r--r--   0      501       20     7569 2023-04-01 11:23:18.000000 pqp-0.3.0/python/pqp/data/data.py
--rw-r--r--   0      501       20     8507 2023-04-01 07:52:26.000000 pqp-0.3.0/python/pqp/data/domain.py
--rw-r--r--   0      501       20      135 2023-03-31 03:00:34.000000 pqp-0.3.0/python/pqp/estimation/__init__.py
--rw-r--r--   0      501       20     4072 2023-04-01 08:03:10.000000 pqp-0.3.0/python/pqp/estimation/estimator.py
--rw-r--r--   0      501       20     8925 2023-04-01 07:57:47.000000 pqp-0.3.0/python/pqp/estimation/multinomial_estimator.py
--rw-r--r--   0      501       20      186 2023-03-31 04:17:25.000000 pqp-0.3.0/python/pqp/identification/__init__.py
--rw-r--r--   0      501       20     7711 2023-04-01 08:00:58.000000 pqp-0.3.0/python/pqp/identification/estimands.py
--rw-r--r--   0      501       20    10785 2023-04-01 08:48:35.000000 pqp-0.3.0/python/pqp/identification/graph.py
--rw-r--r--   0      501       20     2388 2023-03-31 01:56:15.000000 pqp-0.3.0/python/pqp/refutation/__init__.py
--rw-r--r--   0      501       20     4929 2023-03-31 05:24:06.000000 pqp-0.3.0/python/pqp/refutation/result.py
--rw-r--r--   0      501       20      241 2023-03-31 04:12:37.000000 pqp-0.3.0/python/pqp/symbols/__init__.py
--rw-r--r--   0      501       20      396 2023-03-18 07:10:53.000000 pqp-0.3.0/python/pqp/symbols/abstract_math.py
--rw-r--r--   0      501       20     3018 2023-03-31 04:16:19.000000 pqp-0.3.0/python/pqp/symbols/event.py
--rw-r--r--   0      501       20     7580 2023-03-25 09:26:26.000000 pqp-0.3.0/python/pqp/symbols/p.py
--rw-r--r--   0      501       20     1126 2023-03-23 04:31:01.000000 pqp-0.3.0/python/pqp/symbols/parse.py
--rw-r--r--   0      501       20    16468 2023-04-01 12:02:01.000000 pqp-0.3.0/python/pqp/symbols/relation.py
--rw-r--r--   0      501       20     3409 2023-04-01 08:04:42.000000 pqp-0.3.0/python/pqp/symbols/variable.py
--rw-r--r--   0      501       20       29 2023-03-23 02:58:35.000000 pqp-0.3.0/python/pqp/utils/__init__.py
--rw-r--r--   0      501       20      683 2023-03-25 06:45:09.000000 pqp-0.3.0/python/pqp/utils/exceptions.py
--rw-r--r--   0      501       20     1473 2023-03-28 09:15:44.000000 pqp-0.3.0/python/pqp/utils/utils.py
--rw-r--r--   0      501       20       11 2023-02-01 03:34:57.000000 pqp-0.3.0/python/tests/.gitignore
--rw-r--r--   0      501       20      552 2023-03-26 06:08:17.000000 pqp-0.3.0/python/tests/test_abstract_step.py
--rw-r--r--   0      501       20      594 2023-03-26 04:07:53.000000 pqp-0.3.0/python/tests/test_causal_estimand.py
--rw-r--r--   0      501       20     3021 2023-03-28 07:26:00.000000 pqp-0.3.0/python/tests/test_data.py
--rw-r--r--   0      501       20     1690 2023-03-25 03:20:40.000000 pqp-0.3.0/python/tests/test_domain.py
--rw-r--r--   0      501       20      228 2023-03-23 04:38:36.000000 pqp-0.3.0/python/tests/test_event.py
--rw-r--r--   0      501       20     6346 2023-04-01 08:45:57.000000 pqp-0.3.0/python/tests/test_examples.py
--rw-r--r--   0      501       20     1112 2023-04-01 08:17:19.000000 pqp-0.3.0/python/tests/test_graph.py
--rw-r--r--   0      501       20     1538 2023-03-28 06:40:11.000000 pqp-0.3.0/python/tests/test_id.py
--rw-r--r--   0      501       20     7724 2023-04-01 04:27:39.000000 pqp-0.3.0/python/tests/test_multinomial_estimator.py
--rw-r--r--   0      501       20     2413 2023-03-25 05:57:51.000000 pqp-0.3.0/python/tests/test_p.py
--rw-r--r--   0      501       20      832 2023-03-31 01:59:17.000000 pqp-0.3.0/python/tests/test_refutation.py
--rw-r--r--   0      501       20     2544 2023-03-25 09:31:23.000000 pqp-0.3.0/python/tests/test_relation.py
--rw-r--r--   0      501       20      550 2023-03-28 09:16:20.000000 pqp-0.3.0/python/tests/test_utils.py
--rw-r--r--   0      501       20      794 2023-03-26 04:05:53.000000 pqp-0.3.0/python/tests/test_variable.py
--rw-r--r--   0      501       20       74 2023-04-01 08:30:11.000000 pqp-0.3.0/requirements.txt
--rw-r--r--   0      501       20      574 2023-02-01 03:34:57.000000 pqp-0.3.0/src/api/functions.rs
--rw-r--r--   0      501       20       58 2023-02-25 00:17:24.000000 pqp-0.3.0/src/api/mod.rs
--rw-r--r--   0      501       20      651 2023-02-01 03:34:57.000000 pqp-0.3.0/src/api/python.rs
--rw-r--r--   0      501       20     1364 2023-02-01 03:34:57.000000 pqp-0.3.0/src/api/test.rs
--rw-r--r--   0      501       20     5453 2023-04-01 08:49:23.000000 pqp-0.3.0/src/api/wrapper.rs
--rw-r--r--   0      501       20     7806 2023-02-25 14:57:20.000000 pqp-0.3.0/src/form/form.rs
--rw-r--r--   0      501       20      129 2023-02-01 03:34:57.000000 pqp-0.3.0/src/form/mod.rs
--rw-r--r--   0      501       20     5218 2023-02-01 03:34:57.000000 pqp-0.3.0/src/form/simplify.rs
--rw-r--r--   0      501       20     3991 2023-02-25 00:21:49.000000 pqp-0.3.0/src/form/test_form.rs
--rw-r--r--   0      501       20     6687 2023-02-01 03:34:57.000000 pqp-0.3.0/src/form/test_simplify.rs
--rw-r--r--   0      501       20     3459 2023-02-01 03:34:57.000000 pqp-0.3.0/src/form/tikka.rs
--rw-r--r--   0      501       20     2552 2023-02-24 11:35:34.000000 pqp-0.3.0/src/graph/bigraph.rs
--rw-r--r--   0      501       20     4865 2023-02-24 11:35:34.000000 pqp-0.3.0/src/graph/digraph.rs
--rw-r--r--   0      501       20      303 2023-02-24 11:35:34.000000 pqp-0.3.0/src/graph/graph.rs
--rw-r--r--   0      501       20     2075 2023-02-24 11:35:34.000000 pqp-0.3.0/src/graph/graph_builder.rs
--rw-r--r--   0      501       20      296 2023-02-24 11:35:34.000000 pqp-0.3.0/src/graph/mod.rs
--rw-r--r--   0      501       20      242 2023-02-24 11:35:34.000000 pqp-0.3.0/src/graph/node.rs
--rw-r--r--   0      501       20     5763 2023-02-01 03:34:57.000000 pqp-0.3.0/src/graph/tests.rs
--rw-r--r--   0      501       20       64 2023-02-25 00:14:14.000000 pqp-0.3.0/src/identification/mod.rs
--rw-r--r--   0      501       20     3689 2023-02-25 00:13:29.000000 pqp-0.3.0/src/identification/shpitser.rs
--rw-r--r--   0      501       20     6678 2023-02-01 03:34:57.000000 pqp-0.3.0/src/identification/tests.rs
--rw-r--r--   0      501       20      154 2023-02-24 11:35:34.000000 pqp-0.3.0/src/lib.rs
--rw-r--r--   0      501       20      368 2023-02-01 03:34:57.000000 pqp-0.3.0/src/model/examples.rs
--rw-r--r--   0      501       20       93 2023-02-24 11:35:34.000000 pqp-0.3.0/src/model/mod.rs
--rw-r--r--   0      501       20     6166 2023-02-24 11:35:34.000000 pqp-0.3.0/src/model/model.rs
--rw-r--r--   0      501       20     2565 2023-02-01 03:34:57.000000 pqp-0.3.0/src/model/order.rs
--rw-r--r--   0      501       20     4246 2023-02-24 11:35:34.000000 pqp-0.3.0/src/model/tests.rs
--rw-r--r--   0      501       20      901 2023-02-25 00:10:46.000000 pqp-0.3.0/src/test.rs
--rw-r--r--   0      501       20      304 2023-02-01 03:34:57.000000 pqp-0.3.0/src/utils/defaults.rs
--rw-r--r--   0      501       20       99 2023-02-24 11:35:34.000000 pqp-0.3.0/src/utils/mod.rs
--rw-r--r--   0      501       20     2185 2023-02-01 03:34:57.000000 pqp-0.3.0/src/utils/set_utils.rs
--rw-r--r--   0      501       20      987 2023-02-01 03:34:57.000000 pqp-0.3.0/src/utils/tests.rs
--rw-r--r--   0      501       20      612 2023-02-24 11:35:34.000000 pqp-0.3.0/src/utils/utils.rs
--rw-r--r--   0      501       20       49 2023-02-01 03:34:57.000000 pqp-0.3.0/test.sh
--rw-r--r--   0      501       20   150084 2023-02-01 03:34:57.000000 pqp-0.3.0/writeup/2023-01-14-13-06-10.png
--rw-r--r--   0      501       20    51282 2023-02-01 03:34:57.000000 pqp-0.3.0/writeup/2023-01-14-13-52-24.png
--rw-r--r--   0      501       20    53166 2023-02-01 03:34:57.000000 pqp-0.3.0/writeup/2023-01-14-14-22-06.png
--rw-r--r--   0      501       20   118082 2023-02-01 03:34:57.000000 pqp-0.3.0/writeup/2023-01-14-15-01-52.png
--rw-r--r--   0      501       20    45879 2023-02-25 02:07:37.000000 pqp-0.3.0/writeup/2023-02-25-09-07-36.png
--rw-r--r--   0      501       20    50872 2023-02-25 02:22:50.000000 pqp-0.3.0/writeup/2023-02-25-09-22-50.png
--rw-r--r--   0      501       20   112197 2023-04-01 13:06:23.000000 pqp-0.3.0/writeup/Correct and Performant Causal Identification with pqp.ipynb
--rw-r--r--   0      501       20   197652 2023-04-01 03:17:51.000000 pqp-0.3.0/writeup/PQP.ipynb
--rw-r--r--   0      501       20   117397 2023-04-01 03:17:56.000000 pqp-0.3.0/writeup/agg.ipynb
--rw-r--r--   0      501       20      882 2023-02-25 16:01:13.000000 pqp-0.3.0/writeup/build.py
--rw-r--r--   0      501       20    16499 2023-03-11 07:28:34.000000 pqp-0.3.0/writeup/demo.ipynb
--rw-r--r--   0      501       20     8008 2023-04-01 12:33:43.000000 pqp-0.3.0/writeup/demo1.csv
--rw-r--r--   0      501       20    27322 2023-04-01 12:35:30.000000 pqp-0.3.0/writeup/doctordemo.csv
--rw-r--r--   0      501       20    16826 2023-03-16 15:16:30.000000 pqp-0.3.0/writeup/examples.ipynb
--rw-r--r--   0      501       20     1756 2023-02-25 15:09:55.000000 pqp-0.3.0/writeup/grab_code.py
--rw-r--r--   0      501       20      678 2023-04-01 03:08:56.000000 pqp-0.3.0/writeup/supplement.py
--rw-r--r--   0      501       20     9185 2023-02-24 11:35:34.000000 pqp-0.3.0/Cargo.lock
--rw-r--r--   0        0        0     2156 1970-01-01 00:00:00.000000 pqp-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      273 1970-01-01 00:00:00.000000 pqp-0.3.1/Cargo.toml
+-rw-r--r--   0      501       20    53248 2023-03-17 07:12:19.000000 pqp-0.3.1/.coverage
+-rw-r--r--   0      501       20      105 2023-02-01 03:34:57.000000 pqp-0.3.1/.gitignore
+-rw-r--r--   0      501       20      579 2023-02-25 01:53:51.000000 pqp-0.3.1/CHANGELOG.md
+-rw-r--r--   0      501       20     1145 2023-02-01 03:55:07.000000 pqp-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0      501       20     1047 2023-02-01 03:34:57.000000 pqp-0.3.1/LICENSE.txt
+-rw-r--r--   0      501       20     1273 2023-02-01 03:56:12.000000 pqp-0.3.1/README.md
+-rw-r--r--   0      501       20      333 2023-02-01 03:34:57.000000 pqp-0.3.1/publish_docs.sh
+-rw-r--r--   0      501       20      827 2023-06-24 05:53:03.000000 pqp-0.3.1/pyproject.toml
+-rw-r--r--   0      501       20       38 2023-03-01 09:39:53.000000 pqp-0.3.1/python/.gitignore
+-rw-r--r--   0      501       20        0 2023-02-01 03:34:57.000000 pqp-0.3.1/python/conftest.py
+-rw-r--r--   0      501       20       12 2023-02-01 03:34:57.000000 pqp-0.3.1/python/docs/.gitignore
+-rw-r--r--   0      501       20      850 2023-03-31 02:19:59.000000 pqp-0.3.1/python/docs/Makefile
+-rw-r--r--   0      501       20      804 2023-02-01 03:34:57.000000 pqp-0.3.1/python/docs/make.bat
+-rw-r--r--   0      501       20      280 2023-03-31 02:41:09.000000 pqp-0.3.1/python/docs/source/api/pqp.data.BinaryDomain.rst
+-rw-r--r--   0      501       20      442 2023-03-31 02:41:09.000000 pqp-0.3.1/python/docs/source/api/pqp.data.CategoricalDomain.rst
+-rw-r--r--   0      501       20      286 2023-03-31 02:41:09.000000 pqp-0.3.1/python/docs/source/api/pqp.data.ContinuousDomain.rst
+-rw-r--r--   0      501       20      412 2023-03-31 02:41:09.000000 pqp-0.3.1/python/docs/source/api/pqp.data.Data.rst
+-rw-r--r--   0      501       20      268 2023-03-31 02:41:09.000000 pqp-0.3.1/python/docs/source/api/pqp.data.DiscreteDomain.rst
+-rw-r--r--   0      501       20      441 2023-03-31 02:41:09.000000 pqp-0.3.1/python/docs/source/api/pqp.data.Domain.rst
+-rw-r--r--   0      501       20      478 2023-03-31 02:41:09.000000 pqp-0.3.1/python/docs/source/api/pqp.data.IntegerDomain.rst
+-rw-r--r--   0      501       20      272 2023-03-31 02:41:09.000000 pqp-0.3.1/python/docs/source/api/pqp.data.RealDomain.rst
+-rw-r--r--   0      501       20      102 2023-03-31 02:41:09.000000 pqp-0.3.1/python/docs/source/api/pqp.data.infer_domain_type.rst
+-rw-r--r--   0      501       20       84 2023-03-31 02:41:09.000000 pqp-0.3.1/python/docs/source/api/pqp.data.make_domain.rst
+-rw-r--r--   0      501       20      279 2023-03-31 03:04:18.000000 pqp-0.3.1/python/docs/source/api/pqp.estimation.EstimationResult.rst
+-rw-r--r--   0      501       20      764 2023-03-31 02:27:29.000000 pqp-0.3.1/python/docs/source/api/pqp.estimation.Estimator.rst
+-rw-r--r--   0      501       20      973 2023-03-31 02:27:29.000000 pqp-0.3.1/python/docs/source/api/pqp.estimation.MultinomialEstimator.rst
+-rw-r--r--   0      501       20      307 2023-02-01 03:34:57.000000 pqp-0.3.1/python/docs/source/api/pqp.expression.Expression.rst
+-rw-r--r--   0      501       20      234 2023-02-01 03:34:57.000000 pqp-0.3.1/python/docs/source/api/pqp.expression.Hedge.rst
+-rw-r--r--   0      501       20      246 2023-02-01 03:34:57.000000 pqp-0.3.1/python/docs/source/api/pqp.expression.Marginal.rst
+-rw-r--r--   0      501       20      218 2023-02-01 03:34:57.000000 pqp-0.3.1/python/docs/source/api/pqp.expression.P.rst
+-rw-r--r--   0      501       20      242 2023-02-01 03:34:57.000000 pqp-0.3.1/python/docs/source/api/pqp.expression.Product.rst
+-rw-r--r--   0      501       20      246 2023-02-01 03:34:57.000000 pqp-0.3.1/python/docs/source/api/pqp.expression.Quotient.rst
+-rw-r--r--   0      501       20       87 2023-02-01 03:34:57.000000 pqp-0.3.1/python/docs/source/api/pqp.expression.parse_json.rst
+-rw-r--r--   0      501       20      113 2023-02-01 03:34:57.000000 pqp-0.3.1/python/docs/source/api/pqp.graph.BidirectedEdge.rst
+-rw-r--r--   0      501       20      107 2023-02-01 03:34:57.000000 pqp-0.3.1/python/docs/source/api/pqp.graph.DirectedEdge.rst
+-rw-r--r--   0      501       20      435 2023-02-01 03:34:57.000000 pqp-0.3.1/python/docs/source/api/pqp.graph.Graph.rst
+-rw-r--r--   0      501       20      294 2023-03-31 04:09:43.000000 pqp-0.3.1/python/docs/source/api/pqp.identification.ATE.rst
+-rw-r--r--   0      501       20      310 2023-03-31 04:09:43.000000 pqp-0.3.1/python/docs/source/api/pqp.identification.AbstractCausalEstimand.rst
+-rw-r--r--   0      501       20      122 2023-03-31 04:09:43.000000 pqp-0.3.1/python/docs/source/api/pqp.identification.BidirectedEdge.rst
+-rw-r--r--   0      501       20      295 2023-03-31 04:09:43.000000 pqp-0.3.1/python/docs/source/api/pqp.identification.CATE.rst
+-rw-r--r--   0      501       20      278 2023-03-31 04:09:43.000000 pqp-0.3.1/python/docs/source/api/pqp.identification.CausalEstimand.rst
+-rw-r--r--   0      501       20      116 2023-03-31 04:09:43.000000 pqp-0.3.1/python/docs/source/api/pqp.identification.DirectedEdge.rst
+-rw-r--r--   0      501       20      624 2023-03-31 04:09:43.000000 pqp-0.3.1/python/docs/source/api/pqp.identification.Graph.rst
+-rw-r--r--   0      501       20      140 2023-03-31 04:09:43.000000 pqp-0.3.1/python/docs/source/api/pqp.identification.IdentificationResult.rst
+-rw-r--r--   0      501       20      103 2023-03-31 02:27:29.000000 pqp-0.3.1/python/docs/source/api/pqp.refutation.Operation.rst
+-rw-r--r--   0      501       20      586 2023-03-31 02:27:29.000000 pqp-0.3.1/python/docs/source/api/pqp.refutation.Result.rst
+-rw-r--r--   0      501       20      408 2023-03-31 02:27:29.000000 pqp-0.3.1/python/docs/source/api/pqp.refutation.Step.rst
+-rw-r--r--   0      501       20       87 2023-03-31 02:27:29.000000 pqp-0.3.1/python/docs/source/api/pqp.refutation.entrypoint.rst
+-rw-r--r--   0      501       20      730 2023-03-31 02:27:29.000000 pqp-0.3.1/python/docs/source/api/pqp.symbols.AbstractExpression.rst
+-rw-r--r--   0      501       20      314 2023-03-31 02:27:29.000000 pqp-0.3.1/python/docs/source/api/pqp.symbols.AbstractMath.rst
+-rw-r--r--   0      501       20      522 2023-03-31 02:27:30.000000 pqp-0.3.1/python/docs/source/api/pqp.symbols.Difference.rst
+-rw-r--r--   0      501       20      319 2023-03-31 02:27:30.000000 pqp-0.3.1/python/docs/source/api/pqp.symbols.EqualityEvent.rst
+-rw-r--r--   0      501       20      238 2023-03-31 02:27:30.000000 pqp-0.3.1/python/docs/source/api/pqp.symbols.Event.rst
+-rw-r--r--   0      501       20      531 2023-03-31 02:27:30.000000 pqp-0.3.1/python/docs/source/api/pqp.symbols.Expectation.rst
+-rw-r--r--   0      501       20      435 2023-03-31 02:27:30.000000 pqp-0.3.1/python/docs/source/api/pqp.symbols.Hedge.rst
+-rw-r--r--   0      501       20      397 2023-03-31 02:27:30.000000 pqp-0.3.1/python/docs/source/api/pqp.symbols.InterventionEvent.rst
+-rw-r--r--   0      501       20      504 2023-03-31 02:27:30.000000 pqp-0.3.1/python/docs/source/api/pqp.symbols.Marginal.rst
+-rw-r--r--   0      501       20      777 2023-03-31 02:27:30.000000 pqp-0.3.1/python/docs/source/api/pqp.symbols.P.rst
+-rw-r--r--   0      501       20      495 2023-03-31 02:27:30.000000 pqp-0.3.1/python/docs/source/api/pqp.symbols.Product.rst
+-rw-r--r--   0      501       20      504 2023-03-31 02:27:30.000000 pqp-0.3.1/python/docs/source/api/pqp.symbols.Quotient.rst
+-rw-r--r--   0      501       20      121 2023-03-31 02:27:30.000000 pqp-0.3.1/python/docs/source/api/pqp.symbols.StatisticalEvent.rst
+-rw-r--r--   0      501       20      477 2023-03-31 02:27:30.000000 pqp-0.3.1/python/docs/source/api/pqp.symbols.Value.rst
+-rw-r--r--   0      501       20      243 2023-03-31 02:27:30.000000 pqp-0.3.1/python/docs/source/api/pqp.symbols.Variable.rst
+-rw-r--r--   0      501       20       60 2023-03-31 02:27:30.000000 pqp-0.3.1/python/docs/source/api/pqp.symbols.do.rst
+-rw-r--r--   0      501       20       81 2023-03-31 02:27:30.000000 pqp-0.3.1/python/docs/source/api/pqp.symbols.make_vars.rst
+-rw-r--r--   0      501       20       84 2023-03-31 02:27:30.000000 pqp-0.3.1/python/docs/source/api/pqp.symbols.parse_json.rst
+-rw-r--r--   0      501       20       95 2023-03-31 02:27:29.000000 pqp-0.3.1/python/docs/source/api/pqp.utils.attrdict.rst
+-rw-r--r--   0      501       20      127 2023-03-31 02:27:29.000000 pqp-0.3.1/python/docs/source/api/pqp.utils.exceptions.DomainValidationError.rst
+-rw-r--r--   0      501       20      127 2023-03-31 02:27:29.000000 pqp-0.3.1/python/docs/source/api/pqp.utils.exceptions.InferredDomainWarning.rst
+-rw-r--r--   0      501       20      106 2023-03-31 02:27:29.000000 pqp-0.3.1/python/docs/source/api/pqp.utils.exceptions.NumericalError.rst
+-rw-r--r--   0      501       20      121 2023-03-31 02:27:29.000000 pqp-0.3.1/python/docs/source/api/pqp.utils.exceptions.PositivityException.rst
+-rw-r--r--   0      501       20      115 2023-03-31 02:27:29.000000 pqp-0.3.1/python/docs/source/api/pqp.utils.exceptions.UnitDomainWarning.rst
+-rw-r--r--   0      501       20       85 2023-03-31 02:27:29.000000 pqp-0.3.1/python/docs/source/api/pqp.utils.order_graph.rst
+-rw-r--r--   0      501       20       94 2023-03-31 02:27:29.000000 pqp-0.3.1/python/docs/source/api/pqp.utils.recursive_sort.rst
+-rw-r--r--   0      501       20      113 2023-03-31 02:27:29.000000 pqp-0.3.1/python/docs/source/api/pqp.utils.staticproperty.rst
+-rw-r--r--   0      501       20      244 2023-02-01 03:34:57.000000 pqp-0.3.1/python/docs/source/api/pqp.variable.Variable.rst
+-rw-r--r--   0      501       20       82 2023-02-01 03:34:57.000000 pqp-0.3.1/python/docs/source/api/pqp.variable.make_vars.rst
+-rw-r--r--   0      501       20     1483 2023-02-01 04:08:19.000000 pqp-0.3.1/python/docs/source/conf.py
+-rw-r--r--   0      501       20       42 2023-02-01 03:34:57.000000 pqp-0.3.1/python/docs/source/example_notebooks.rst
+-rw-r--r--   0      501       20   238718 2023-02-01 03:34:57.000000 pqp-0.3.1/python/docs/source/favicon.ico
+-rw-r--r--   0      501       20    19314 2023-02-01 03:34:57.000000 pqp-0.3.1/python/docs/source/imgs/frontdoor_estimator.png
+-rw-r--r--   0      501       20    18477 2023-02-01 03:34:57.000000 pqp-0.3.1/python/docs/source/imgs/frontdoor_new.png
+-rw-r--r--   0      501       20    97789 2023-02-01 03:34:57.000000 pqp-0.3.1/python/docs/source/imgs/frontdoor_viz.png
+-rw-r--r--   0      501       20    37703 2023-03-31 05:48:21.000000 pqp-0.3.1/python/docs/source/imgs/qs_causal_estimand.png
+-rw-r--r--   0      501       20    75030 2023-03-31 05:55:41.000000 pqp-0.3.1/python/docs/source/imgs/qs_stat_estimand.png
+-rw-r--r--   0      501       20      809 2023-03-31 06:13:18.000000 pqp-0.3.1/python/docs/source/index.rst
+-rw-r--r--   0      501       20       24 2023-03-31 02:39:47.000000 pqp-0.3.1/python/docs/source/module_maps/data.rst
+-rw-r--r--   0      501       20       30 2023-03-31 02:21:59.000000 pqp-0.3.1/python/docs/source/module_maps/estimation.rst
+-rw-r--r--   0      501       20       36 2023-03-31 02:28:16.000000 pqp-0.3.1/python/docs/source/module_maps/exceptions.rst
+-rw-r--r--   0      501       20       34 2023-03-31 02:22:26.000000 pqp-0.3.1/python/docs/source/module_maps/identification.rst
+-rw-r--r--   0      501       20       30 2023-03-31 02:23:26.000000 pqp-0.3.1/python/docs/source/module_maps/refutation.rst
+-rw-r--r--   0      501       20       27 2023-03-31 02:22:32.000000 pqp-0.3.1/python/docs/source/module_maps/symbols.rst
+-rw-r--r--   0      501       20       46 2023-02-01 03:34:57.000000 pqp-0.3.1/python/docs/source/modules.rst
+-rw-r--r--   0      501       20      432 2023-03-31 02:20:15.000000 pqp-0.3.1/python/docs/source/pqp.data.rst
+-rw-r--r--   0      501       20      548 2023-03-31 02:20:15.000000 pqp-0.3.1/python/docs/source/pqp.estimation.rst
+-rw-r--r--   0      501       20      534 2023-03-31 02:20:15.000000 pqp-0.3.1/python/docs/source/pqp.identification.rst
+-rw-r--r--   0      501       20      340 2023-03-31 02:20:15.000000 pqp-0.3.1/python/docs/source/pqp.refutation.rst
+-rw-r--r--   0      501       20      419 2023-03-31 02:20:15.000000 pqp-0.3.1/python/docs/source/pqp.rst
+-rw-r--r--   0      501       20     1051 2023-03-31 02:20:16.000000 pqp-0.3.1/python/docs/source/pqp.symbols.rst
+-rw-r--r--   0      501       20      456 2023-03-31 02:20:16.000000 pqp-0.3.1/python/docs/source/pqp.utils.rst
+-rw-r--r--   0      501       20     6082 2023-04-01 02:03:49.000000 pqp-0.3.1/python/docs/source/quickstart.rst
+-rw-r--r--   0      501       20   116713 2023-06-23 21:55:04.000000 pqp-0.3.1/python/fd_case_study.ipynb
+-rw-r--r--   0      501       20       16 2023-02-01 03:34:57.000000 pqp-0.3.1/python/pqp/.gitignore
+-rw-r--r--   0      501       20      269 2023-06-22 21:46:02.000000 pqp-0.3.1/python/pqp/__init__.py
+-rw-r--r--   0      501       20       60 2023-03-31 02:50:56.000000 pqp-0.3.1/python/pqp/data/__init__.py
+-rw-r--r--   0      501       20     7569 2023-04-01 11:23:18.000000 pqp-0.3.1/python/pqp/data/data.py
+-rw-r--r--   0      501       20     8507 2023-04-01 07:52:26.000000 pqp-0.3.1/python/pqp/data/domain.py
+-rw-r--r--   0      501       20      135 2023-03-31 03:00:34.000000 pqp-0.3.1/python/pqp/estimation/__init__.py
+-rw-r--r--   0      501       20     4072 2023-04-01 08:03:10.000000 pqp-0.3.1/python/pqp/estimation/estimator.py
+-rw-r--r--   0      501       20     8925 2023-04-01 07:57:47.000000 pqp-0.3.1/python/pqp/estimation/multinomial_estimator.py
+-rw-r--r--   0      501       20      589 2023-06-22 22:02:47.000000 pqp-0.3.1/python/pqp/fd_demo.py
+-rw-r--r--   0      501       20      186 2023-03-31 04:17:25.000000 pqp-0.3.1/python/pqp/identification/__init__.py
+-rw-r--r--   0      501       20     8977 2023-06-23 20:53:27.000000 pqp-0.3.1/python/pqp/identification/estimands.py
+-rw-r--r--   0      501       20    13147 2023-06-23 16:55:29.000000 pqp-0.3.1/python/pqp/identification/graph.py
+-rw-r--r--   0      501       20     2388 2023-03-31 01:56:15.000000 pqp-0.3.1/python/pqp/refutation/__init__.py
+-rw-r--r--   0      501       20     6271 2023-06-23 16:52:32.000000 pqp-0.3.1/python/pqp/refutation/result.py
+-rw-r--r--   0      501       20      241 2023-03-31 04:12:37.000000 pqp-0.3.1/python/pqp/symbols/__init__.py
+-rw-r--r--   0      501       20      396 2023-03-18 07:10:53.000000 pqp-0.3.1/python/pqp/symbols/abstract_math.py
+-rw-r--r--   0      501       20     3018 2023-03-31 04:16:19.000000 pqp-0.3.1/python/pqp/symbols/event.py
+-rw-r--r--   0      501       20     7580 2023-03-25 09:26:26.000000 pqp-0.3.1/python/pqp/symbols/p.py
+-rw-r--r--   0      501       20     1126 2023-03-23 04:31:01.000000 pqp-0.3.1/python/pqp/symbols/parse.py
+-rw-r--r--   0      501       20    20412 2023-06-23 21:46:53.000000 pqp-0.3.1/python/pqp/symbols/relation.py
+-rw-r--r--   0      501       20     4317 2023-06-23 20:46:28.000000 pqp-0.3.1/python/pqp/symbols/variable.py
+-rw-r--r--   0      501       20       29 2023-03-23 02:58:35.000000 pqp-0.3.1/python/pqp/utils/__init__.py
+-rw-r--r--   0      501       20      683 2023-03-25 06:45:09.000000 pqp-0.3.1/python/pqp/utils/exceptions.py
+-rw-r--r--   0      501       20     1473 2023-03-28 09:15:44.000000 pqp-0.3.1/python/pqp/utils/utils.py
+-rw-r--r--   0      501       20       11 2023-02-01 03:34:57.000000 pqp-0.3.1/python/tests/.gitignore
+-rw-r--r--   0      501       20      552 2023-03-26 06:08:17.000000 pqp-0.3.1/python/tests/test_abstract_step.py
+-rw-r--r--   0      501       20      966 2023-06-23 20:52:53.000000 pqp-0.3.1/python/tests/test_causal_estimand.py
+-rw-r--r--   0      501       20     3021 2023-03-28 07:26:00.000000 pqp-0.3.1/python/tests/test_data.py
+-rw-r--r--   0      501       20     1690 2023-03-25 03:20:40.000000 pqp-0.3.1/python/tests/test_domain.py
+-rw-r--r--   0      501       20      228 2023-03-23 04:38:36.000000 pqp-0.3.1/python/tests/test_event.py
+-rw-r--r--   0      501       20     6346 2023-04-01 08:45:57.000000 pqp-0.3.1/python/tests/test_examples.py
+-rw-r--r--   0      501       20     2280 2023-06-23 16:10:10.000000 pqp-0.3.1/python/tests/test_graph.py
+-rw-r--r--   0      501       20     1538 2023-03-28 06:40:11.000000 pqp-0.3.1/python/tests/test_id.py
+-rw-r--r--   0      501       20     7724 2023-04-01 04:27:39.000000 pqp-0.3.1/python/tests/test_multinomial_estimator.py
+-rw-r--r--   0      501       20     2413 2023-03-25 05:57:51.000000 pqp-0.3.1/python/tests/test_p.py
+-rw-r--r--   0      501       20      832 2023-03-31 01:59:17.000000 pqp-0.3.1/python/tests/test_refutation.py
+-rw-r--r--   0      501       20     3032 2023-06-23 19:24:57.000000 pqp-0.3.1/python/tests/test_relation.py
+-rw-r--r--   0      501       20      550 2023-03-28 09:16:20.000000 pqp-0.3.1/python/tests/test_utils.py
+-rw-r--r--   0      501       20     1040 2023-06-23 20:00:53.000000 pqp-0.3.1/python/tests/test_variable.py
+-rw-r--r--   0      501       20       74 2023-04-01 08:30:11.000000 pqp-0.3.1/requirements.txt
+-rw-r--r--   0      501       20      574 2023-02-01 03:34:57.000000 pqp-0.3.1/src/api/functions.rs
+-rw-r--r--   0      501       20       58 2023-02-25 00:17:24.000000 pqp-0.3.1/src/api/mod.rs
+-rw-r--r--   0      501       20      651 2023-02-01 03:34:57.000000 pqp-0.3.1/src/api/python.rs
+-rw-r--r--   0      501       20     1364 2023-02-01 03:34:57.000000 pqp-0.3.1/src/api/test.rs
+-rw-r--r--   0      501       20     5453 2023-04-01 08:49:23.000000 pqp-0.3.1/src/api/wrapper.rs
+-rw-r--r--   0      501       20     9318 2023-06-22 18:22:01.000000 pqp-0.3.1/src/form/form.rs
+-rw-r--r--   0      501       20      129 2023-02-01 03:34:57.000000 pqp-0.3.1/src/form/mod.rs
+-rw-r--r--   0      501       20     5218 2023-02-01 03:34:57.000000 pqp-0.3.1/src/form/simplify.rs
+-rw-r--r--   0      501       20     4151 2023-06-22 18:25:20.000000 pqp-0.3.1/src/form/test_form.rs
+-rw-r--r--   0      501       20     6687 2023-02-01 03:34:57.000000 pqp-0.3.1/src/form/test_simplify.rs
+-rw-r--r--   0      501       20     3459 2023-02-01 03:34:57.000000 pqp-0.3.1/src/form/tikka.rs
+-rw-r--r--   0      501       20     2552 2023-02-24 11:35:34.000000 pqp-0.3.1/src/graph/bigraph.rs
+-rw-r--r--   0      501       20     4865 2023-02-24 11:35:34.000000 pqp-0.3.1/src/graph/digraph.rs
+-rw-r--r--   0      501       20      303 2023-02-24 11:35:34.000000 pqp-0.3.1/src/graph/graph.rs
+-rw-r--r--   0      501       20     2075 2023-02-24 11:35:34.000000 pqp-0.3.1/src/graph/graph_builder.rs
+-rw-r--r--   0      501       20      296 2023-06-22 19:37:08.000000 pqp-0.3.1/src/graph/mod.rs
+-rw-r--r--   0      501       20      373 2023-06-22 21:00:19.000000 pqp-0.3.1/src/graph/node.rs
+-rw-r--r--   0      501       20     5763 2023-02-01 03:34:57.000000 pqp-0.3.1/src/graph/tests.rs
+-rw-r--r--   0      501       20       64 2023-02-25 00:14:14.000000 pqp-0.3.1/src/identification/mod.rs
+-rw-r--r--   0      501       20     3689 2023-02-25 00:13:29.000000 pqp-0.3.1/src/identification/shpitser.rs
+-rw-r--r--   0      501       20     6682 2023-06-22 18:22:08.000000 pqp-0.3.1/src/identification/tests.rs
+-rw-r--r--   0      501       20      154 2023-02-24 11:35:34.000000 pqp-0.3.1/src/lib.rs
+-rw-r--r--   0      501       20      368 2023-02-01 03:34:57.000000 pqp-0.3.1/src/model/examples.rs
+-rw-r--r--   0      501       20       93 2023-06-22 21:01:19.000000 pqp-0.3.1/src/model/mod.rs
+-rw-r--r--   0      501       20     6195 2023-06-22 18:44:17.000000 pqp-0.3.1/src/model/model.rs
+-rw-r--r--   0      501       20     2565 2023-02-01 03:34:57.000000 pqp-0.3.1/src/model/order.rs
+-rw-r--r--   0      501       20     4253 2023-06-22 21:01:26.000000 pqp-0.3.1/src/model/tests.rs
+-rw-r--r--   0      501       20      795 2023-06-22 21:01:57.000000 pqp-0.3.1/src/test.rs
+-rw-r--r--   0      501       20      304 2023-02-01 03:34:57.000000 pqp-0.3.1/src/utils/defaults.rs
+-rw-r--r--   0      501       20       99 2023-02-24 11:35:34.000000 pqp-0.3.1/src/utils/mod.rs
+-rw-r--r--   0      501       20     2185 2023-02-01 03:34:57.000000 pqp-0.3.1/src/utils/set_utils.rs
+-rw-r--r--   0      501       20      987 2023-02-01 03:34:57.000000 pqp-0.3.1/src/utils/tests.rs
+-rw-r--r--   0      501       20      612 2023-02-24 11:35:34.000000 pqp-0.3.1/src/utils/utils.rs
+-rw-r--r--   0      501       20       49 2023-02-01 03:34:57.000000 pqp-0.3.1/test.sh
+-rw-r--r--   0      501       20   150084 2023-02-01 03:34:57.000000 pqp-0.3.1/writeup/2023-01-14-13-06-10.png
+-rw-r--r--   0      501       20    51282 2023-02-01 03:34:57.000000 pqp-0.3.1/writeup/2023-01-14-13-52-24.png
+-rw-r--r--   0      501       20    53166 2023-02-01 03:34:57.000000 pqp-0.3.1/writeup/2023-01-14-14-22-06.png
+-rw-r--r--   0      501       20   118082 2023-02-01 03:34:57.000000 pqp-0.3.1/writeup/2023-01-14-15-01-52.png
+-rw-r--r--   0      501       20    45879 2023-02-25 02:07:37.000000 pqp-0.3.1/writeup/2023-02-25-09-07-36.png
+-rw-r--r--   0      501       20    50872 2023-02-25 02:22:50.000000 pqp-0.3.1/writeup/2023-02-25-09-22-50.png
+-rw-r--r--   0      501       20   367476 2023-04-02 04:33:16.000000 pqp-0.3.1/writeup/2023-04-02-14-33-14.png
+-rw-r--r--   0      501       20   325115 2023-04-02 04:33:45.000000 pqp-0.3.1/writeup/2023-04-02-14-33-44.png
+-rw-r--r--   0      501       20   213508 2023-04-02 04:34:20.000000 pqp-0.3.1/writeup/2023-04-02-14-34-19.png
+-rw-r--r--   0      501       20   336724 2023-04-02 04:34:31.000000 pqp-0.3.1/writeup/2023-04-02-14-34-30.png
+-rw-r--r--   0      501       20   349974 2023-04-02 04:34:45.000000 pqp-0.3.1/writeup/2023-04-02-14-34-44.png
+-rw-r--r--   0      501       20   407521 2023-04-02 04:35:40.000000 pqp-0.3.1/writeup/2023-04-02-14-35-39.png
+-rw-r--r--   0      501       20   115292 2023-04-02 04:36:00.000000 pqp-0.3.1/writeup/2023-04-02-14-36-00.png
+-rw-r--r--   0      501       20   476032 2023-04-02 04:36:59.000000 pqp-0.3.1/writeup/2023-04-02-14-36-57.png
+-rw-r--r--   0      501       20   345389 2023-04-02 04:37:11.000000 pqp-0.3.1/writeup/2023-04-02-14-37-10.png
+-rw-r--r--   0      501       20   108822 2023-04-02 04:47:11.000000 pqp-0.3.1/writeup/PQP a Library for End-to-End Causal Inference.ipynb
+-rw-r--r--   0      501       20   197652 2023-04-01 03:17:51.000000 pqp-0.3.1/writeup/PQP.ipynb
+-rw-r--r--   0      501       20   117397 2023-04-01 03:17:56.000000 pqp-0.3.1/writeup/agg.ipynb
+-rw-r--r--   0      501       20      882 2023-02-25 16:01:13.000000 pqp-0.3.1/writeup/build.py
+-rw-r--r--   0      501       20    16499 2023-03-11 07:28:34.000000 pqp-0.3.1/writeup/demo.ipynb
+-rw-r--r--   0      501       20     8008 2023-04-02 04:40:20.000000 pqp-0.3.1/writeup/demo1.csv
+-rw-r--r--   0      501       20    27322 2023-04-01 12:35:30.000000 pqp-0.3.1/writeup/doctordemo.csv
+-rw-r--r--   0      501       20    14520 2023-06-22 21:23:55.000000 pqp-0.3.1/writeup/examples.ipynb
+-rw-r--r--   0      501       20     1756 2023-02-25 15:09:55.000000 pqp-0.3.1/writeup/grab_code.py
+-rw-r--r--   0      501       20     6485 2023-04-03 04:52:12.000000 pqp-0.3.1/writeup/speed.ipynb
+-rw-r--r--   0      501       20      678 2023-04-01 03:08:56.000000 pqp-0.3.1/writeup/supplement.py
+-rw-r--r--   0      501       20     9185 2023-02-24 11:35:34.000000 pqp-0.3.1/Cargo.lock
+-rw-r--r--   0        0        0     2136 1970-01-01 00:00:00.000000 pqp-0.3.1/PKG-INFO
```

### Comparing `pqp-0.3.0/.coverage` & `pqp-0.3.1/.coverage`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/CHANGELOG.md` & `pqp-0.3.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/CONTRIBUTING.md` & `pqp-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/LICENSE.txt` & `pqp-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/README.md` & `pqp-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/pyproject.toml` & `pqp-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 [project]
 name = "pqp"
-version = "0.3.0"
+version = "0.3.1"
 description = "Subroutines for structural causal modeling"
 license = {file = "LICENSE.txt"}
 authors = [{name = "Leo Ware"}]
-dependencies = []
+dependencies = [
+    "pandas",
+    "numpy",
+    "tomli",
+    "matplotlib"
+]
 requires-python = ">=3.10"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["causal inference", "causal identification"]
 
 [project.optional-dependencies]
 dev = [
     "sphinx",
     "maturin",
     "sphinx-autobuild",
-    "toml",
     "pytest",
-    "matplotlib",
-    "numpy",
     "networkx",
 ]
 
 [project.urls]
 Homepage = "https://leo-ware.github.io/capstone/"
 Source = "https://github.com/leo-ware/capstone"
```

### Comparing `pqp-0.3.0/python/docs/Makefile` & `pqp-0.3.1/python/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/docs/make.bat` & `pqp-0.3.1/python/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/docs/source/api/pqp.estimation.Estimator.rst` & `pqp-0.3.1/python/docs/source/api/pqp.estimation.Estimator.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/docs/source/api/pqp.estimation.MultinomialEstimator.rst` & `pqp-0.3.1/python/docs/source/api/pqp.estimation.MultinomialEstimator.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/docs/source/api/pqp.identification.Graph.rst` & `pqp-0.3.1/python/docs/source/api/pqp.identification.Graph.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/docs/source/api/pqp.refutation.Result.rst` & `pqp-0.3.1/python/docs/source/api/pqp.refutation.Result.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/docs/source/api/pqp.symbols.AbstractExpression.rst` & `pqp-0.3.1/python/docs/source/api/pqp.symbols.AbstractExpression.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/docs/source/api/pqp.symbols.Difference.rst` & `pqp-0.3.1/python/docs/source/api/pqp.symbols.Difference.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/docs/source/api/pqp.symbols.Expectation.rst` & `pqp-0.3.1/python/docs/source/api/pqp.symbols.Expectation.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/docs/source/api/pqp.symbols.P.rst` & `pqp-0.3.1/python/docs/source/api/pqp.symbols.P.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/docs/source/conf.py` & `pqp-0.3.1/python/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/docs/source/favicon.ico` & `pqp-0.3.1/python/docs/source/favicon.ico`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/docs/source/imgs/frontdoor_estimator.png` & `pqp-0.3.1/python/docs/source/imgs/frontdoor_estimator.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/docs/source/imgs/frontdoor_new.png` & `pqp-0.3.1/python/docs/source/imgs/frontdoor_new.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/docs/source/imgs/frontdoor_viz.png` & `pqp-0.3.1/python/docs/source/imgs/frontdoor_viz.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/docs/source/imgs/qs_causal_estimand.png` & `pqp-0.3.1/python/docs/source/imgs/qs_causal_estimand.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/docs/source/imgs/qs_stat_estimand.png` & `pqp-0.3.1/python/docs/source/imgs/qs_stat_estimand.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/docs/source/index.rst` & `pqp-0.3.1/python/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/docs/source/pqp.estimation.rst` & `pqp-0.3.1/python/docs/source/pqp.estimation.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/docs/source/pqp.identification.rst` & `pqp-0.3.1/python/docs/source/pqp.identification.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/docs/source/pqp.symbols.rst` & `pqp-0.3.1/python/docs/source/pqp.symbols.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/docs/source/quickstart.rst` & `pqp-0.3.1/python/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/pqp/data/data.py` & `pqp-0.3.1/python/pqp/data/data.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/pqp/data/domain.py` & `pqp-0.3.1/python/pqp/data/domain.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/pqp/estimation/estimator.py` & `pqp-0.3.1/python/pqp/estimation/estimator.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/pqp/estimation/multinomial_estimator.py` & `pqp-0.3.1/python/pqp/estimation/multinomial_estimator.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/pqp/identification/estimands.py` & `pqp-0.3.1/python/pqp/identification/estimands.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,26 +15,46 @@
     def expression(self):
         """Derive the expression for the causal estimand
         
         Returns:
             AbstractExpression: the expression for the causal estimand
         """
         raise NotImplementedError()
+    
+    @abstractmethod
+    def literal(self):
+        """The estimand represented as a function call, as an Expression
+        
+        Returns:
+            AbstractExpression: the literal for the causal estimand
+        """
+        raise NotImplementedError()
+    
+    def display(self):
+        """Display the causal estimand"""
+        from IPython.display import display, Math
+        tex = self.literal().to_latex() + " = " + self.expression().to_latex()
+        return display(Math(tex))
 
 class CausalEstimand(AbstractCausalEstimand):
     """Subclass of AbstractCausalEstimand which carries its expression as a literal"""
+    LITERAL_CLASS = create_literal("CausalEstimand")
+
     def __init__(self, exp):
         super().__init__()
         self.exp = exp
     
     def __repr__(self):
         return f"CausalEstimand({repr(self.exp)[:12]})"
     
     def expression(self):
         return self.exp
+    
+    def literal(self):
+        return self.__class__.LITERAL_CLASS(self.exp)
 
 class ATE(AbstractCausalEstimand):
     """Causal estimand for the average treatment effect
 
     To define the average treatment effect, it's necessary to specify what is meant
     by "treatment" and "control" in this context. You can do this by passing either
     a dict or a list of StatisticalEvent objects to each of the treatment_condition
@@ -52,14 +72,16 @@
         
     
     Args:
         outcome (Variable): the outcome variable
         treatment_condition (dict or list): the treatment condition
         control_condition (dict or list): the control condition
     """
+    LITERAL_CLASS = create_literal("ATE", arity=2, sep=" | ", name_tex="\\text{ATE}", sep_tex=" \\mid ")
+
     def __init__(self, outcome, treatment_condition, control_condition=None):
         super().__init__()
         self.name = "average treatment effect"
 
         if not isinstance(outcome, Variable):
             raise TypeError(f"outcome must be a Variable, not {type(outcome)}")
 
@@ -108,14 +130,18 @@
     
     def __repr__(self):
         return f"ATE(outcome={repr(self.outcome)}, treatment={self._treatment_vars()})"
     
     def expression(self):
         return Expectation(self.outcome, P(self.outcome, given=[do(c) for c in self.treatment_condition])) -\
             Expectation(self.outcome, P(self.outcome, given=[do(c) for c in self.control_condition]))
+    
+    def literal(self):
+        vset = VarSet(self._treatment_vars(), left="", right="")
+        return self.__class__.LITERAL_CLASS(self.outcome, vset)
 
 class CATE(ATE):
     """Causal estimand for the conditional average treatment effect
 
     To define the conditional average treatment effect, it's necessary to specify 
     what is meant by treatment and control in this context, and you need to specify the
     subpopulation in which to measure the effect. You can 
@@ -148,14 +174,15 @@
     
     Args:
         outcome (Variable): the outcome variable
         treatment_condition (dict or list): the treatment condition
         control_condition (dict or list): the control condition
         subpopulation (dict or list): the subpopulation in which to measure the effect
     """
+    LITERAL_CLASS = create_literal("CATE", arity=3, sep=" | ", name_tex="\\text{CATE}", sep_tex=" \\mid ")
     def __init__(self, outcome, treatment_condition, control_condition, subpopulation):
         super().__init__(outcome, treatment_condition, control_condition)
         self.name = "conditional average treatment effect"
         self.subpopulation = self._validate_condition(subpopulation, "subpopulation")
     
     def _control_vars(self):
         return [v.get_var() for v in self.subpopulation]
@@ -164,7 +191,12 @@
         return f"<CATE treatment_vars={self._treatment_vars()}, outcome={self.outcome}, control_vars={self._control_vars()}>"
 
     def expression(self):
         tc = [do(c) for c in self.treatment_condition]
         oc = [do(c) for c in self.control_condition]
         return Expectation(self.outcome, P(self.outcome, given=tc + self.subpopulation)) -\
             Expectation(self.outcome, P(self.outcome, given=oc + self.subpopulation))
+    
+    def literal(self):
+        intervention_set = VarSet(self._treatment_vars(), left="", right="")
+        control_set = VarSet(self._control_vars(), left="", right="")
+        return self.__class__.LITERAL_CLASS(self.outcome, intervention_set, control_set)
```

### Comparing `pqp-0.3.0/python/pqp/identification/graph.py` & `pqp-0.3.1/python/pqp/identification/graph.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,43 @@
 from pqp.symbols import Variable, Expectation, parse_json, P, EqualityEvent, InterventionEvent, do
 from pqp.identification.estimands import ATE, CATE, AbstractCausalEstimand, CausalEstimand
 from pqp.refutation import entrypoint, Result
 from pqp.pqp import id as rust_id
+
+from collections import defaultdict
+from dataclasses import dataclass
+from typing import Optional, Any
 import json
 from itertools import chain
 
 class IdentificationResult(Result):
     """Stores the result of identification
 
     Attributes:
         identified_estimand (AbstractExpression): the identified causal estimand
     """
     _keys = ["identified_estimand"]
 
 
+@dataclass(frozen=True)
+class SearchNode:
+    prev: Optional["SearchNode"]
+    graph_node: Any
+
+    def unpack(self, _path=None):
+        if _path is None:
+            p = []
+            self.unpack(_path=p)
+            return list(reversed(p))
+        
+        _path.append(self.graph_node)
+        if self.prev is not None:
+            self.prev.unpack(_path=_path)
+
+
 class Graph:
     """A causal graph
 
     The best way to create a `Graph` is using the `<=` and `&` infix operators. When you use
     these operators between `Variable`s, they create a `DirectedEdge` or `BidirectedEdge` respectively.
 
     Example: The Front-Door Model
@@ -50,16 +70,33 @@
     
     Args:
         edges (list of DirectedEdge or BidirectedEdge): the edges in the graph
     """
     def __init__(self, edges=[]):
         self.bi_edges = []
         self.directed_edges = []
+        self.nodes = set()
         self.add_edges(edges)
     
+    def add_node(self, node):
+        """Adds a node to the graph
+        
+        Args:
+            node (Variable): the node to add
+        """
+        self.nodes.add(node)
+    
+    def add_nodes(self, nodes):
+        """Adds multiple nodes to the graph
+        
+        Args:
+            nodes (list of Variable): the nodes to add
+        """
+        self.nodes.update(nodes)
+    
     def add_edges(self, edges):
         """Add multiple edges to the graph
         
         Args:
             edges (list of DirectedEdge or BidirectedEdge): the edges to add
         """
         while edges:
@@ -75,16 +112,18 @@
         """Adds an edge to the graph
         
         Args:
             edge (DirectedEdge or BidirectedEdge): the edge to add
         """
         if isinstance(edge, BidirectedEdge):
             self.bi_edges.append(edge)
+            self.add_nodes([edge.a, edge.b])
         elif isinstance(edge, DirectedEdge):
             self.directed_edges.append(edge)
+            self.add_nodes([edge.start, edge.end])
         else:
             raise TypeError(f"Cannot add edge of type {type(edge)}")
     
     def _bi_edge_tuples(self):
         return [(str(edge.a), str(edge.b)) for edge in self.bi_edges]
     
     def _di_edge_tuples(self):
@@ -237,15 +276,52 @@
         nx.draw_networkx_labels(layout_graph, layout)
     
     def __repr__(self):
         return f"Graph({self.bi_edges + self.directed_edges})"
     
     def __str__(self):
         return f"<Graph n_edges={len(self.bi_edges + self.directed_edges)}>"
-
+    
+    def dir_edge_dict(self):
+        """Returns a dict mapping each node to its children in the graph"""
+        edges = defaultdict(list)
+        for edge in self.directed_edges:
+            edges[edge.start].append(edge.end)
+        return dict(edges)
+    
+    def _dfs(self, start, end):
+        if start == end:
+            yield [start]
+        else:
+            edges = self.dir_edge_dict()
+            stack = [SearchNode(None, start)]
+            while stack:
+                node = stack.pop()
+                for nxt in edges.get(node.graph_node, []):
+                    nxt_node = SearchNode(node, nxt)
+                    if nxt == end:
+                        yield nxt_node.unpack()
+                    else:
+                        stack.append(nxt_node)
+    
+    def dfs(self, start, end):
+        """Performs a depth-first search over directed edges in the graph, returning a generator over paths
+        
+        Args:
+            start (Variable): the start of the search
+            end (Variable): the end of the search
+        
+        Returns:
+            Generator[List[DirectedEdge]]: the path from start to end
+        """
+        if start not in self.nodes:
+            raise ValueError(f"{start} is not in the graph")
+        if end not in self.nodes:
+            raise ValueError(f"{end} is not in the graph")
+        return self._dfs(start, end)
 
 class DirectedEdge:
     """A directed edge between two variables, represents a causal relationship
     
     Args:
         start (Variable): the start of the edge
         end (Variable): the end of the edge
```

### Comparing `pqp-0.3.0/python/pqp/refutation/__init__.py` & `pqp-0.3.1/python/pqp/refutation/__init__.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/pqp/refutation/result.py` & `pqp-0.3.1/python/pqp/refutation/result.py`

 * *Files 20% similar despite different names*

```diff
@@ -135,14 +135,35 @@
     
     def explain_all(self):
         """Prints a human-readable explanation of the result to the console, including all prior steps.
         Equivalent to calling self.explain(nested=True)"""
         self.explain(nested=True)
 
 def entrypoint(step_name, result_class=Result):
+    """Wrapper for logical steps in the assumption management system
+
+    Args:
+        step_name (str): the name of the step (human readable)
+        result_class (class): used to store results of the step, must be a subclass of `Result`
+    Returns:
+        decorator: wrapper for functions implementing logical steps in an analysis
+    
+    This function returns a a decorator which can be used to wrap a method implementing a step, a 
+    `Step` instance is passed as a keyword argument ("step") to the method and should 
+    be used to record substeps, assumptions, and results. The method should not return a value.
+
+    The three core constructs of the assumption management system are `Assumption`a, `Step`s, and 
+    `Result`s. A step is a logical unit of work encapsulated in a single method, which may be 
+    composed of multiple substeps. During the process of calculation, the method can report 
+    logical substeps, assumptions it is making, results as they are computed, and notes for 
+    the user. This information is consolidated into the `Step` object, which stores references
+    to previous steps in the analysis in a graph representing the entire computation. This way,
+    metadata about the computation is available at all times and can be used by both the user and
+    automated sensitivity analysis tools.
+    """
     def decorator(func):
         def wrapper(*args, **kwargs):
             step = Step(step_name)
             op = Operation(func, args, kwargs)
             func_return = func(*args, **kwargs, step=step)
             assert func_return is None, "entrypoint functions must not return a value"
```

### Comparing `pqp-0.3.0/python/pqp/symbols/event.py` & `pqp-0.3.1/python/pqp/symbols/event.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/pqp/symbols/p.py` & `pqp-0.3.1/python/pqp/symbols/p.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/pqp/symbols/parse.py` & `pqp-0.3.1/python/pqp/symbols/parse.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/pqp/symbols/relation.py` & `pqp-0.3.1/python/pqp/symbols/relation.py`

 * *Files 11% similar despite different names*

```diff
@@ -59,14 +59,16 @@
         """Recursively maps a function over the expression tree"""
         raise NotImplementedError()
     
     @abstractmethod
     def r_adapt_map(self, func):
         """Recursive map where the func decides callables used to transform children
 
+        DO NOT USE! This is a powerful and necessary method but it results in almost unreadable code.
+
         So, `func` takes an `AbstractExpression` and needs to return a `tuple` of two things. First, 
         a function `A` which maps from `AbstractExpression` to `AbstractExpression`. Second, a function `B` 
         of the same time as `func`.
 
         At each level of recursion, `func` will be called on an expression `E` to get `A` and `B`.
         This method, `r_adapt_map` will then be called on the children of `E`
         with `B` as input (if `B` is `None`, recursion terminates). An expression of the same 
@@ -513,7 +515,120 @@
     
     def r_map(self, func):
         return func(self)
     
     def r_adapt_map(self, func):
         A, B = func(self)
         return A(self)
+    
+    def copy(self):
+        return Hedge()
+    
+    def __repr__(self):
+        return "FAIL"
+
+def create_literal(name, arity=1, sep=", ", name_tex=None, sep_tex=None):
+    """Class factory for creating expression literals
+
+    Suppose you have a function `f` that takes a single expression as an argument and you 
+    want to use this function in a symbolic expression.
+
+    >>> F = create_literal("f")
+    >>> x = Variable("x")
+    >>> F(x)
+    f(x)
+    >>> F(x).to_latex()
+    $f(x)$
+
+    Args:
+        name (str): The name of the new class
+        arity (int, optional): The arity of the new class. Defaults to 1. Zero is allowed.
+        sep (str, optional): The separator to use when printing the expression. Defaults to ", ".
+        name_tex (str, optional): The name of the new class in LaTeX. Defaults to name.
+        sep_tex (str, optional): The separator to use when printing the expression in LaTeX. Defaults to sep.
+    Returns:
+        A new subclass of `AbstractExpression`
+
+    """
+
+    # I ❤️ closures
+    if name_tex is None:
+        name_tex = name
+    if sep_tex is None:
+        sep_tex = sep
+
+    class NewLiteral(AbstractExpression):
+        def __init__(self, *args):
+            if len(args) != arity:
+                raise ValueError(f"Expected {arity} arguments, got {len(args)}")
+            
+            for arg in list(args):
+                if not isinstance(arg, AbstractMath):
+                    raise TypeError(f"Expected {AbstractMath.__name__}, got {type(arg)}")
+            
+            self.args = args
+        
+        def __repr__(self):
+            if arity == 0:
+                return name
+            return f"{name}({sep.join(a.__repr__() for a in self.args)})"
+        
+        def copy(self):
+            new_args = tuple(a.copy() for a in self.args)
+            return self.__class__(new_args)
+        
+        def sorted(self):
+            def arg_sorter(arg):
+                if hasattr(arg, "sorted"):
+                    return arg.sorted()
+                elif isinstance(arg, Variable):
+                    return arg
+                else:
+                    raise TypeError(f"Cannot sort {arg}")
+
+            new_args = tuple(arg_sorter(a) for a in self.args)
+            return self.__class__(*new_args)
+        
+        def syntactic_eq(self, other):
+            def arg_eq(a, b):
+                if hasattr(a, "syntactic_eq"):
+                    return a.syntactic_eq(b)
+                else:
+                    return a == b
+            
+            return (
+                (isinstance(other, self.__class__)) and
+                (len(self.args) == len(other.args)) and
+                all(arg_eq(a, b) for a, b in zip(self.args, other.args))
+            )
+        
+        def r_map(self, func):
+            new_args = tuple(args.r_map(func) for args in self.args)
+            return func(self.__class__(*new_args))
+        
+        def r_adapt_map(self, func):
+            A, B = func(self)
+            if B is not None:
+                new_args = [
+                    arg.r_adapt_map(B) if hasattr(arg, "r_adapt_map")
+                    else arg
+                    for arg in self.args
+                ]
+                return A(self.__class__(*new_args))
+            else:
+                return A(self.copy())
+        
+        def free_variables(self):
+            def free(obj):
+                if hasattr(obj, "free_variables"):
+                    return obj.free_variables()
+                elif isinstance(obj, Variable):
+                    return {obj}
+                else:
+                    return set()
+            return set().union(*(free(arg) for arg in self.args))
+        
+        def to_latex(self):
+            return f"{name_tex}({sep_tex.join(a.to_latex() for a in self.args)})"
+    
+    NewLiteral.__name__ = name
+    return NewLiteral
```

### Comparing `pqp-0.3.0/python/pqp/symbols/variable.py` & `pqp-0.3.1/python/pqp/symbols/variable.py`

 * *Files 26% similar despite different names*

```diff
@@ -92,14 +92,38 @@
     def to_latex(self):
         return self.name
     
     # def r_adapt_map(self, func):
     #     A, B = func(self)
     #     return A(self)
 
+class VarSet(AbstractMath):
+    def __init__(self, variables, left="(", right=")"):
+        if not isinstance(variables, (list, tuple)):
+            raise TypeError(f"variables must be a list or tuple of Variables, not {type(variables)}")
+
+        for v in variables:
+            if not isinstance(v, Variable):
+                raise TypeError(f"variables must be a list or tuple of Variables, not {type(v)}")
+        
+        if type(left) != str:
+            raise TypeError(f"left must be a string, not {type(left)}")
+        if type(right) != str:
+            raise TypeError(f"right must be a string, not {type(right)}")
+        
+        self.vars = list(variables)
+        self.left = left
+        self.right = right
+    
+    def __repr__(self):
+        return f"VarSet({self.vars})"
+    
+    def to_latex(self):
+        return f"{self.left}{', '.join([v.to_latex() for v in self.vars])}{self.right}"
+
 
 def make_vars(names):
     """Creates a list of variables from a list of names
     
     Example:
         >>> make_vars(["x", "y", "z"])
         [Variable("x"), Variable("y"), Variable("z")]
```

### Comparing `pqp-0.3.0/python/pqp/utils/exceptions.py` & `pqp-0.3.1/python/pqp/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/pqp/utils/utils.py` & `pqp-0.3.1/python/pqp/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/tests/test_abstract_step.py` & `pqp-0.3.1/python/tests/test_abstract_step.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/tests/test_causal_estimand.py` & `pqp-0.3.1/python/tests/test_causal_estimand.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,8 +5,15 @@
     x, y, z = make_vars("xyz")
     assert ATE(y, treatment_condition={x: 1}, control_condition={x: 0}).expression() == \
         (Expectation(y, P(y, given=do(x.val == 1))) - Expectation(y, P(y, given=[do(x.val == 0)])))
     assert CATE(y, control_condition={x: 0}, treatment_condition={x: 1}, subpopulation={z: 1}).expression() == \
         (
             Expectation(y, P(y, given=[do(x.val == 1), z.val == 1])) -
             Expectation(y, P(y, given=[do(x.val == 0), z.val == 1]))
-        )
+        )
+
+def test_literal():
+    x, y, z = make_vars("xyz")
+    ate_lit = ATE(y, treatment_condition={x: 1}, control_condition={x: 0}).literal()
+    assert ate_lit.to_latex() == "\\text{ATE}(y \\mid x)"
+    cate_lit = CATE(y, control_condition={x: 0}, treatment_condition={x: 1}, subpopulation={z: 1}).literal()
+    assert cate_lit.to_latex() == "\\text{CATE}(y \\mid x \\mid z)"
```

### Comparing `pqp-0.3.0/python/tests/test_data.py` & `pqp-0.3.1/python/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/tests/test_domain.py` & `pqp-0.3.1/python/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/tests/test_examples.py` & `pqp-0.3.1/python/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/tests/test_id.py` & `pqp-0.3.1/python/tests/test_id.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/tests/test_multinomial_estimator.py` & `pqp-0.3.1/python/tests/test_multinomial_estimator.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/tests/test_p.py` & `pqp-0.3.1/python/tests/test_p.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/tests/test_refutation.py` & `pqp-0.3.1/python/tests/test_refutation.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/tests/test_relation.py` & `pqp-0.3.1/python/tests/test_relation.py`

 * *Files 15% similar despite different names*

```diff
@@ -51,7 +51,24 @@
     x, y, z, m = make_vars(["x", "y", "z", "m"])
     assert P(x).free_variables() == {x}
     assert P([x], given=[y]).free_variables() == {x, y}
     assert (P(x) * P(y)).free_variables() == {x, y}
     assert (P(x) * P(y)).assign(x, 3).free_variables() == {y}
     assert (P(x) * Marginal(y, P(x) * P(y))).free_variables() == {x}
     assert (P(x) * Marginal(y, P(x) * P(y))).assign(x, 3).free_variables() == set()
+
+def test_create_literal():
+    F = create_literal("f")
+    x = Variable("x")
+    y = Variable("y")
+
+    F(x)
+
+    assert F(x) == F(x)
+    # assert F(x) != F(y)
+    assert F(x).__repr__() == "f(Variable(x))"
+    assert F(x).free_variables() == {x}
+
+    G = create_literal("g", arity=2, sep="|", name_tex="\\mathcal{G}", sep_tex="\\mid ")
+    assert G(x, y) != G(y, x)
+    assert G(x, y).__repr__() == "g(Variable(x)|Variable(y))"
+    assert G(x, y).to_latex() == "\\mathcal{G}(x\\mid y)"
```

### Comparing `pqp-0.3.0/python/tests/test_utils.py` & `pqp-0.3.1/python/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/python/tests/test_variable.py` & `pqp-0.3.1/python/tests/test_variable.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,8 +16,19 @@
 
 def test_event_infix():
     x, y = make_vars("xy")
     assert (x.val == 1) == EqualityEvent(x, 1)
     with pytest.raises(ValueError):
         x.val == y
     with pytest.raises(ValueError):
-        x.val == y.val
+        x.val == y.val
+
+def test_var_set():
+    x, y, z = make_vars("xyz")
+
+    v = VarSet([x, y, z])
+    assert v.vars == [x, y, z]
+    assert v.to_latex() == "(x, y, z)"
+
+    v = VarSet([x], left="", right="")
+    assert v.vars == [x]
+    assert v.to_latex() == "x"
```

### Comparing `pqp-0.3.0/src/api/functions.rs` & `pqp-0.3.1/src/api/functions.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/src/api/python.rs` & `pqp-0.3.1/src/api/python.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/src/api/test.rs` & `pqp-0.3.1/src/api/test.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/src/api/wrapper.rs` & `pqp-0.3.1/src/api/wrapper.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/src/form/simplify.rs` & `pqp-0.3.1/src/form/simplify.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/src/form/test_form.rs` & `pqp-0.3.1/src/form/test_form.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-use super::{
-    form::Form,
+use super::form::{Form, one};
+use crate::{
+    P,
+    api::wrapper::ModelWrapper,
+    identification::id_no_simplify,
+    model::examples::frontdoor_model,
+    utils::defaults::{set, Set},
+    graph::make_nodes,
 };
 
-use crate::{utils::defaults::{set, Set}, model::examples::frontdoor_model, identification::id_no_simplify, api::wrapper::ModelWrapper};
-
 #[test]
-fn test_sort () {
+fn test_sort() {
     let f = Form::prob(vec![1, 2, 0]).sorted();
     let s = Form::prob(vec![0, 1, 2]);
     assert_eq!(f, Form::prob(vec![0, 1, 2]), "{:?} should equal {:?}", f, s);
 }
 
 #[test]
-fn test_structural_eq () {
+fn test_structural_eq() {
     let f1 = Form::product(vec![
         Form::prob(vec![0, 3]),
         Form::prob(vec![4]),
         Form::prob(vec![6, 7]),
     ]);
     let f2 = Form::product(vec![
         Form::prob(vec![6, 7]),
@@ -62,80 +66,78 @@
     ]);
     assert!(f1.structural_eq(&f2), "{:?} should equal {:?}", f1, f2);
 
     // test involving quotients of marginals
     let f1 = Form::quotient(
         Form::marginal(
             set![0, 1],
-            Form::product(vec![
-                Form::prob(vec![0, 1, 2]),
-                Form::prob(vec![3, 4, 5]),
-                ])),
+            Form::product(vec![Form::prob(vec![0, 1, 2]), Form::prob(vec![3, 4, 5])]),
+        ),
         Form::prob(vec![0, 1, 2]),
     );
     let f2 = Form::quotient(
         Form::marginal(
             set![1, 0],
-            Form::product(vec![
-                Form::prob(vec![3, 4, 5]),
-                Form::prob(vec![0, 1, 2]),
-                ])),
+            Form::product(vec![Form::prob(vec![3, 4, 5]), Form::prob(vec![0, 1, 2])]),
+        ),
         Form::prob(vec![0, 1, 2]),
     );
-    assert!(f1.structural_eq(&f2), "{:?} should equal {:?}", f1, f2);  
+    assert!(f1.structural_eq(&f2), "{:?} should equal {:?}", f1, f2);
 
     // test involving quotients of marginals
     let f1 = Form::quotient(
         Form::marginal(
             set![0, 1],
-            Form::product(vec![
-                Form::prob(vec![0, 1, 2]),
-                Form::prob(vec![3, 4, 5]),
-                ])),
+            Form::product(vec![Form::prob(vec![0, 1, 2]), Form::prob(vec![3, 4, 5])]),
+        ),
         Form::prob(vec![0, 1, 2]),
     );
     let f2 = Form::quotient(
         Form::marginal(
             set![1, 0],
-            Form::product(vec![
-                Form::prob(vec![4, 5, 3]),
-                Form::prob(vec![0, 1, 2]),
-                ])),
+            Form::product(vec![Form::prob(vec![4, 5, 3]), Form::prob(vec![0, 1, 2])]),
+        ),
         Form::prob(vec![0, 1, 2]),
     );
-    assert!(f1.structural_eq(&f2), "{:?} should equal {:?}", f1, f2);   
-
+    assert!(f1.structural_eq(&f2), "{:?} should equal {:?}", f1, f2);
 }
 
 #[test]
 fn test_factorize_subset() {
     let model = frontdoor_model();
     let order = model.order_vec();
     let p = model.p();
 
     let f = Form::factorize_subset(order, p, &set![0, 2]);
     let ans = Form::quotient(
-        Form::product(vec![Form::prob(vec![0]), Form::cond_prob(vec![0, 1, 2], vec![])]),
-        Form::prob(vec![0, 1])
+        Form::product(vec![
+            Form::prob(vec![0]),
+            Form::cond_prob(vec![0, 1, 2], vec![]),
+        ]),
+        Form::prob(vec![0, 1]),
     );
 
     assert_eq!(f.simplify(), ans.simplify());
 }
 
 #[test]
-fn demonstrate_simplify() {
-    let m = frontdoor_model();
-    let f_raw = id_no_simplify(&m, &set![2], &set![0]);
-    let f = m.id(&set![2], &set![0]);
-
-    let mut foo = ModelWrapper::new();
-    foo.add_effect("X", "Z");
-    foo.add_effect("Z", "Y");
-    foo.add_confounding("X", "Y");
-
-    let f_json = ModelWrapper::form_sub(&foo, f).to_json();
-    let f_raw_json = ModelWrapper::form_sub(&foo, f_raw).to_json();
-
-    println!("f_raw = {:?}", f_raw_json);
-    println!("f = {:?}", f_json);
-    assert!(false);
+fn test_p_macro () {
+    if let [a, b, c] = make_nodes(3)[..] {
+        assert_eq!(P!(a, b), Form::prob(vec![a, b]));
+        assert_eq!(P!(a, b | c), Form::cond_prob(vec![a, b], vec![c]));
+        assert_eq!(P!(), one());
+    } else {
+        panic!("make_nodes(3) should return 3 nodes");
+    }
+}
+
+#[test]
+fn test_infix() {
+    if let [a, b, c] = make_nodes(3)[..] {
+        assert_eq!(P!(a) * P!(b), Form::product(vec![P!(a), P!(b)]));
+        assert_eq!(P!(a) / P!(b), Form::quotient(P!(a), P!(b)));
+        assert_eq!(P!(a) * P!(b) * P!(c), Form::product(vec![P!(a), P!(b), P!(c)]));
+        assert_eq!(P!(a) * P!(b) / P!(c), Form::quotient(Form::product(vec![P!(a), P!(b)]), P!(c)));
+    } else {
+        panic!("make_nodes(3) should return 3 nodes");
+    }
 }
```

### Comparing `pqp-0.3.0/src/form/test_simplify.rs` & `pqp-0.3.1/src/form/test_simplify.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/src/form/tikka.rs` & `pqp-0.3.1/src/form/tikka.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/src/graph/bigraph.rs` & `pqp-0.3.1/src/graph/bigraph.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/src/graph/digraph.rs` & `pqp-0.3.1/src/graph/digraph.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/src/graph/graph_builder.rs` & `pqp-0.3.1/src/graph/graph_builder.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/src/graph/tests.rs` & `pqp-0.3.1/src/graph/tests.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/src/identification/shpitser.rs` & `pqp-0.3.1/src/identification/shpitser.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/src/identification/tests.rs` & `pqp-0.3.1/src/identification/tests.rs`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 use super::id;
 use crate::{
     model::{
         Model,
         examples::frontdoor_model
     },
-    utils::defaults::{set, Set}, form::{Form, HEDGE},
+    utils::defaults::{set, Set},
+    form::{Form, HEDGE},
 };
 
 #[test]
 fn test_backdoor() {
     let model = Model::from_elems(
         vec![
             (2, vec![0, 1]),
```

### Comparing `pqp-0.3.0/src/model/model.rs` & `pqp-0.3.1/src/model/model.rs`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
             dag: self.dag.to_owned(),
             confounded: self.confounded.to_owned(),
             vars: self.vars.to_owned(),
             cond_vars: union(&self.cond_vars, &cond)
         }
     }
 
-    /// Sets variables as not observed in the model. Inverse of `cond`.
+    /// Sets variables as not observed in the model. Inverse of `cond`. (Todo: what does this mean?)
     pub fn hide(&self, observed: &Set<Node>) -> Model {
         Model {
             dag: self.dag.to_owned(),
             confounded: self.confounded.to_owned(),
             vars: self.vars.to_owned(),
             cond_vars: difference(&self.cond_vars, &observed)
         }
```

### Comparing `pqp-0.3.0/src/model/order.rs` & `pqp-0.3.1/src/model/order.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/src/model/tests.rs` & `pqp-0.3.1/src/model/tests.rs`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,16 @@
     graph::{
         Graph,
         make_nodes,
     },
     utils::{
         defaults::{Set, Map},
         set_utils::make_set,
-    }, set
+    },
+    set, P
 };
 
 use super::{order::Order, examples::frontdoor_model};
 
 #[test]
 fn subgraphing() {
     let (a, b, c, d) = (1, 2, 3, 4);
```

### Comparing `pqp-0.3.0/src/test.rs` & `pqp-0.3.1/src/test.rs`

 * *Files 26% similar despite different names*

```diff
@@ -3,21 +3,14 @@
 use crate::{
     model::examples::frontdoor_model,
     identification::id,
     utils::defaults::{set, Set},
 };
 
 #[test]
-fn foo() {
-    let a = String::from("a");
-    let b = String::from("a");
-    assert_eq!(a, b);
-}
-
-#[test]
 fn do_stuff() {
     let fd = frontdoor_model();
     println!("{:?}", fd);
     println!("{:?}", id(&fd, &set!(2), &set!(0)));
 }
 
 // "Marginal({1}, Product([Marginal({}, Product([Quotient(Marginal({}, Marginal({2}, P([2, 0, 1], []))), Marginal({1}, Marginal({2}, P([2, 0, 1], [])))), Quotient(Marginal({1}, Marginal({2}, P([2, 0, 1], []))), Marginal({1, 0}, Marginal({2}, P([2, 0, 1], []))))])), Marginal({}, Product([Quotient(Marginal({}, P([2, 0, 1], [])), Marginal({2}, P([2, 0, 1], []))), Quotient(Marginal({2}, P([2, 0, 1], [])), Marginal({1, 2}, P([2, 0, 1], []))), Quotient(Marginal({1, 2}, P([2, 0, 1], [])), Marginal({1, 0, 2}, P([2, 0, 1], [])))]))]))"
```

### Comparing `pqp-0.3.0/src/utils/set_utils.rs` & `pqp-0.3.1/src/utils/set_utils.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/src/utils/tests.rs` & `pqp-0.3.1/src/utils/tests.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/src/utils/utils.rs` & `pqp-0.3.1/src/utils/utils.rs`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/writeup/2023-01-14-13-06-10.png` & `pqp-0.3.1/writeup/2023-01-14-13-06-10.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/writeup/2023-01-14-13-52-24.png` & `pqp-0.3.1/writeup/2023-01-14-13-52-24.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/writeup/2023-01-14-14-22-06.png` & `pqp-0.3.1/writeup/2023-01-14-14-22-06.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/writeup/2023-01-14-15-01-52.png` & `pqp-0.3.1/writeup/2023-01-14-15-01-52.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/writeup/2023-02-25-09-07-36.png` & `pqp-0.3.1/writeup/2023-02-25-09-07-36.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/writeup/2023-02-25-09-22-50.png` & `pqp-0.3.1/writeup/2023-02-25-09-22-50.png`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/writeup/Correct and Performant Causal Identification with pqp.ipynb` & `pqp-0.3.1/writeup/PQP a Library for End-to-End Causal Inference.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9832792186318973%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(1, 'Causal inference under Pearl’s framework of structural "*

 * *            'causal models has been the subject of intense theoretical study, but performant '*

 * *            'open-source implementations of many of the key algorithms are still lacking or, where '*

 * *            'they exist, are not widely adopted or maintained. I present `pqp` (short for '*

 * *            '*Pourquoi-pas?*), a end-to-end library for structural causal inference that includes '*

 * *            'an implemen […]*

```diff
@@ -2,15 +2,15 @@
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Abstract\n",
-                "Causal inference under Pearl\u2019s framework of structural causal models has been the subject of intense theoretical study, but performant open-source implementations of many of the key algorithms are still lacking or, where they exist, are not widely adopted or maintained. I present `pqp` (short for *Pourquoi-pas?*), a performant implementation of Shpitser\u2019s IDC algorithm for identification of conditional causal effects in semi-Markovian causal models. The library includes sophisticated memory-sharing graph data structures, a symbolic simplification routine, and it comes wrapped in an elegant Python interface."
+                "Causal inference under Pearl\u2019s framework of structural causal models has been the subject of intense theoretical study, but performant open-source implementations of many of the key algorithms are still lacking or, where they exist, are not widely adopted or maintained. I present `pqp` (short for *Pourquoi-pas?*), a end-to-end library for structural causal inference that includes an implementation of Shpitser\u2019s IDC algorithm for identification of conditional causal effects in semi-Markovian causal models as well as tools for estimation. The library includes sophisticated memory-sharing graph data structures, a symbolic simplification routine, and it comes wrapped in an elegant Python interface. FInally, I have created a number of educational resources to help users get started with the library."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -18,59 +18,70 @@
                 "\n",
                 "Causal inference is a fundamental task in many fields, including epidemiology, economics, and data science. One popular framework for causal inference is Pearl's structural causal modeling framework, which utilizes directed acyclic graphs (DAGs) and the do-calculus to explicitly model potential causal relationships. (Pearl, 2000) This approach allows for a clear and intuitive representation of causal assumptions, while also helping to avoid common biases that can arise with other methodologies. However, a crucial step in this framework is identification: translating a causal question into an abstract statistical estimator that can be estimated using a combination of a model and parametric assumptions.\n",
                 "\n",
                 "One important algorithm for identification in the structural causal modeling framework is Shpitser's algorithm for conditional interventional effects. (Shpitser, 2008) This algorithm is polynomial time and guarantees a result when one is possible. However, existing open-source implementations of this algorithm are often incorrect, slow, or unmaintained. In this paper, I present a novel implementation of Shpitser's algorithm, written in Rust for efficient cross-functional use. Our implementation is production-quality code and includes extensive testing routines to ensure performance and correctness.\n",
                 "\n",
                 "To bridge the gap between theoretical algorithm and practical tool, I developed two techniques as subroutines to the algorithm. I developed and implemented a heuristic symbolic simplification algorithm. To protect the speed and memory efficiency of the program, I designed a memory-sharing graph datastructure which allows similar graphs to share memory via a system of references and immutable data. Further, I am close to finishing an implementation of a estimation technique which will extend the work in Brule (2018).\n",
                 "\n",
-                "To aid in adoption of this algorithm, I designed and implemented a user-friendly Python wrapper. This wrapper allows for the specification and visualization of causal graphs using a concise and elegant API, as well as giving the user full access to the underlying algorithms. This is available as a Python package on PyPi, and I created a website with documentation."
+                "To aid in adoption of this algorithm, I designed and implemented a user-friendly Python wrapper. This wrapper allows for the specification and visualization of causal graphs using a concise and elegant API, as well as giving the user full access to the underlying algorithms. In addition, this wrapper tracks steps in a user's analysis, constructing a computational graph of intermediate results. This graph tracks assumptions made by the various subroutines of the algorithm, allowing the user to access a list of the assumptions made during an analysis so they can understand potential limitations. The wrapper is available as a Python package on PyPi, and I created a website with documentation.\n",
+                "\n",
+                "I created a number of educational resources to share my work: a Medium article detailed some of the theoretical background and two explainer videos covering practical use of the library."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Overview\n",
                 "\n",
                 "The paper is organized as follows: in the first section, I provide an overview of much of the literature on structural causal modeling. I review the literature on available implementations of the algorithm and justify the need for this implementation.\n",
                 "\n",
-                "In the Implementation section, I describe technical insights I employed and analysis I performed on my implementation. I detail techniques I developed for simplication and memory-sharing, and I describe the extensive testing procedures I used to ensure correctness. I describe the Python wrapper I developed to make the algorithm accessible to a wider audience. I evaluate my implementation on correctness, performance, and ease of use.\n",
+                "In the Implementation section, I describe technical insights I employed and analysis I performed on my implementation. I detail techniques I developed for simplication and memory-sharing, and I describe the extensive testing procedures I used to ensure correctness. I describe the Python wrapper I developed to make the algorithm accessible to a wider audience. I outline my technique for tracking assumptions made during analysis. I evaluate my implementation on correctness, performance, and ease of use.\n",
+                "\n",
+                "Following the implementation, I provide an end-to-end example of using the library to estimate an effect. Then, I overview the educational resources I created as part of the project.\n",
                 "\n",
                 "Appendices include HC/LO footnotes, documentation, and code."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Contributions\n",
                 "\n",
-                "In this work, I present a novel implementation of Shpitser's ID algorithm, including a comprehensive set of graph routines and a heuristic-based simplification algorithm. The implementation is written in Rust and the code is provided in the appendix. Additionally, I have developed Python bindings to facilitate usage of the algorithm. It is important to note that while this implementation and techniques for simplification and memory-sharing are novel, the underlying algorithm and all the material covered in the Background section is not a contribution of this paper and is instead a summary of the current state of the field."
+                "In this work, I present a novel implementation of Shpitser's ID algorithm, including a comprehensive set of graph routines and a heuristic-based simplification algorithm. The implementation is written in Rust and the code is provided in the appendix. Additionally, I have developed Python bindings to facilitate usage of the algorithm. These bindings track assumptions made during the analysis in a computational graph that allows users to track the dependencies between various intermediate results and the assumptions they rely on.\n",
+                "\n",
+                "In order to share my work with the broader community, I developed a high quality project website with detailed documentation. I wrote a Medium article which overviews some of the theory and introduces the library. I also created two explainer videos which provide a practical intro to using the library.\n",
+                "\n",
+                "It is important to note that while this implementation and techniques for simplification and memory-sharing are novel, the underlying algorithm and all the material covered in the Background section is not a contribution of this paper and is instead a summary of the current state of the field."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Links\n",
                 "\n",
                 "- Documentation: [https://leo-ware.github.io/pqp/index.html](https://leo-ware.github.io/pqp/index.html)\n",
                 "- Source code: [https://github.com/leo-ware/pqp](https://github.com/leo-ware/pqp)\n",
-                "- PyPI Distribution: [https://pypi.org/project/pqp/](https://pypi.org/project/pqp/)"
+                "- PyPI Distribution: [https://pypi.org/project/pqp/](https://pypi.org/project/pqp/)\n",
+                "- Medium Article: [https://medium.com/@leoware/causal-inference-a-four-stage-framework-7fc2f8deafe2](https://medium.com/@leoware/causal-inference-a-four-stage-framework-7fc2f8deafe2)\n",
+                "- Video 1: [https://www.loom.com/share/91dc669b931d487a84c8030c80d2391c](https://www.loom.com/share/91dc669b931d487a84c8030c80d2391c)\n",
+                "- Video 2: [https://www.loom.com/share/7d8feab2b4f54a7caa59c495a9ce9858](https://www.loom.com/share/7d8feab2b4f54a7caa59c495a9ce9858)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Note on this text\n",
+                "## Note\n",
                 "\n",
                 "AI text generation algorithms were used in the production of this text. Specifically, the OpenAI model ChatPGT was used extensively to edit for tone and concision."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -496,55 +507,25 @@
                 "\n",
                 "This is often okay in the context of predictive inference, as the goal is usually to simply make accurate predictions, and this can be checked against ground truth using a holdout set. But, in the context of causal inference, the goal is to make causal claims, and so there is no easily accessible ground truth against which to check the results. Additionally, many of the assumptions made in causal inference are often numerous and complex, and so users cannot be expected to know (or necessarily understand) them.\n",
                 "\n",
                 "To approach these problem, I decided that it was important that users of `pqp` be able to access a summary of the intermediate steps, transformations, and underlying assumptions performed by the algorithms. As such, I implemented the Python wrapper to automatically construct a computational graph to track the dependencies between different intermediate results derived during an analysis. This allows the user to inspect the steps actually performed by the library during an analysis and understand the assumptions that are being made.\n",
                 "\n",
                 "To achieve this technically, I implemented a `Result` class which stores the outputs of key computations, such as data preprocessing, model fitting, identification, and estimation. A higher order function (called `entrypoint` in the code) wraps the key subroutines which perform these calculations. When they are called, it dynamically captures inputs to these functions, saving them for reproducability or sensitivity analysis. It then searches the inputs for any instances of `Result` and, if found, adds these as dependencies of the current calculation. Then, it wraps the output of these functions in a `Result` which can access information about its logical dependencies. In addition, the subroutines report any transformations or assumptions they make, and these are captured by `entrypoint` and included in the metadata inside `Result`. As such, any `Result` object can be used to reconstruct the entire analysis up to that point, and it knows all the assumptions underlying it.\n",
                 "\n",
-                "To use these in the code, you can call the `.explain()` and `.explain_all()` methods in the code to get an overall summary. Here is an example output of `.explain_all()`, called at the end of an analysis."
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "```\n",
-                "Data Processing\n",
-                "\tAssume: x is on BinaryDomain()\n",
-                "\tAssume: z is on BinaryDomain()\n",
-                "\tAssume: y is on BinaryDomain()\n",
-                "Identification\n",
-                "\tWe will identify the average treatment effect using IDC.\n",
-                "\tAssume: Noncontradictory evidence\n",
-                "\tAssume: Acyclicity\n",
-                "\tAssume: Positivty\n",
-                "\tIDC\n",
-                "\t\tInput:\n",
-                "\t\tP(y| do(x))\n",
-                "\t\tOutput:\n",
-                "\t\t\u03a3_(z) [ [\u03a3_(x) [ [P(x) * P(x, z, y) / P(x, z)] ] * P(x, z) / P(x)] ]\n",
-                "\tDerived: identified_estimand = E_(y) [ \u03a3_(z) [ [\u03a3_(x) [ [P(x) * P(x, z, y) / P(x, z)] ] * P(x = 1, z) / P(x = 1)] ] ] - E_(y) [ \u03a3_(z) [ [\u03a3_(x) [ [P(x) * P(x, z, y) / P(x, z)] ] * P(x = 0, z) / P(x = 0)] ] ]\n",
-                "Fit MultinomialEstimator\n",
-                "\tAssume: Multinomial likelihood\n",
-                "\tAssume: Dirichlet prior\n",
-                "Estimation\n",
-                "\tPerforming brute force estimation using a multinomial likelihood and dirichlet prior.\n",
-                "\tDerived: value = 0.4433808167141502\n",
-                "```"
+                "To use these in the code, you can call the `.explain()` and `.explain_all()` methods in the code to get an overall summary. A demonstration of this method is shown in the example below."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Analysis\n",
                 "\n",
-                "The primary goals for this implementation were correctness, performance, and ease of use. In this section, I examine the library in light of each of these goals in turn."
+                "The primary goals for this implementation were correctness and ease of use. In this section, I examine the library in light of each of these goals."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -649,15 +630,15 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/latex": [
-                            "$\\displaystyle \\textbf{Model g: } P(y | do(x)) = \\sum_{z3, z1, z2} \\big({\\sum_{z1, x} \\big({P(z3, y, z1, z2, x) P(z3, z2, x) \\over P(z3, z1, z2, x)}\\big) \\sum_{x, z3, y, z1} \\big({P(z3, y, z1, z2, x) P(z3, z2, x) \\over P(z3, z1, z2, x)}\\big) P(z3, z2) P(z1, z2, x) \\over \\sum_{y, x, z1} \\big({P(z3, y, z1, z2, x) P(z3, z2, x) \\over P(z3, z1, z2, x)}\\big) \\sum_{z3, x, y, z2, z1} \\big({P(z3, y, z1, z2, x) P(z3, z2, x) \\over P(z3, z1, z2, x)}\\big) P(z2) P(z2, x)}\\big)$"
+                            "$\\displaystyle \\textbf{Model g: } P(y | do(x)) = \\sum_{z2, z3, z1} \\big({\\sum_{z1, x} \\big({P(z3, y, z1, z2, x) P(z3, z2, x) \\over P(z3, z1, z2, x)}\\big) \\sum_{z1, z3, y, x} \\big({P(z3, y, z1, z2, x) P(z3, z2, x) \\over P(z3, z1, z2, x)}\\big) P(z3, z2) P(z1, z2, x) \\over \\sum_{z1, y, x} \\big({P(z3, y, z1, z2, x) P(z3, z2, x) \\over P(z3, z1, z2, x)}\\big) \\sum_{z3, x, z1, y, z2} \\big({P(z3, y, z1, z2, x) P(z3, z2, x) \\over P(z3, z1, z2, x)}\\big) P(z2) P(z2, x)}\\big)$"
                         ],
                         "text/plain": [
                             "<IPython.core.display.Math object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -698,24 +679,14 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Performance\n",
-                "\n",
-                "To test to performance of the implementation, I am designing a set of benchmarks to compare it to other existing implementations. For these benchmanrks, I will randomly generated a large number of graphs with different properties. Then, I will time my algorithm at identifying these graphs."
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
                 "### Ease of Use\n",
                 "The Rust code underlying the library is extremely fast, but Rust is a language used by few in the causal inference community. To make the library more accessible, I created a Python library that wraps the Rust code. Although Python is definitely second to R in terms of adoption in the community, it is much more common among industrial practicioners.\n",
                 "\n",
                 "While the focus of the Rust implementation is correctness and performance, the focus of the Python bindings is on elegance and usability. I used Python's magic methods to create an API for specifying and querying causal models that is extremely simple and readable. I created a website with documentation for the python library, and I have published the library on PyPI.\n",
                 "\n",
                 "By utilizing Python's infix operators, I was able to create an API in which graphs can be created via an intuitive embedded syntax. It is possible to create a new causal model using the library in just a few lines. The `<=` operator creates a directed edge in the graph, while the `&` operator creates a bidirected edge. See the following example, which implements the front-door model."
             ]
@@ -785,15 +756,16 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "# identification of ATE\n",
-                "ate = Expectation(y, P(y, given=do(x.val == 1)) - P(y, given=do(x.val == 0)))\n",
+                "ate = Expectation(y, P(y, given=do(x.val == 1)) -\n",
+                "    P(y, given=do(x.val == 0)))\n",
                 "g.identify(ate).identified_estimand.display()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
@@ -818,15 +790,20 @@
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "from pqp.identification import CATE\n",
                 "\n",
-                "cate = CATE(outcome=y, treatment_condition={x: 1}, control_condition={x: 0}, subpopulation={z: 1})\n",
+                "cate = CATE(\n",
+                "    outcome=y,\n",
+                "    treatment_condition={x: 1},\n",
+                "    control_condition={x: 0},\n",
+                "    subpopulation={z: 1}\n",
+                ")\n",
                 "g.identify(cate).identified_estimand.display()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
@@ -848,20 +825,20 @@
             "metadata": {},
             "source": [
                 "In this section, I show how my code can be used to estimate an average treatment effect using the front door model on a simulated dataset. The dataset has four variables: $x$, $z$, $y$, and $m$. The variable $x$ represents a treatment which influences an outcome $y$ via a mediator $m$. The variable $z$ is a confounder which influences both $x$ and $y$. The following graph shows the causal structure of the model. All are binary except for $y$, which is on ${1, 2, 3}$."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -882,30 +859,34 @@
             "metadata": {},
             "source": [
                 "In the dataset, $x$ has the effect of raising the value of $y$ by $-0.5$ by virtue of the process which simulated the data. We can quickly recover this quantity using the graph above."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "EstimationResult(value=-0.4732071277264369)"
                         ]
                     },
-                    "execution_count": 23,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "model = MultinomialEstimator(pd.read_csv(\"demo1.csv\"))\n",
+                "from pqp.estimation import MultinomialEstimator\n",
+                "from pqp.identification import ATE\n",
+                "\n",
+                "df = pd.read_csv(\"demo1.csv\")\n",
+                "model = MultinomialEstimator(df)\n",
                 "effect = ATE(y, x)\n",
                 "\n",
                 "estimand = g.identify(effect)\n",
                 "model.estimate(estimand)"
             ]
         },
         {
@@ -914,24 +895,24 @@
             "metadata": {},
             "source": [
                 "However, what if $z$ were unobserved, would we still be able to recover the result? We first attempt this without reference to our knowledge of the data generating process. This is equivalent to directly regressing $y$ on $x$ without any controls."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "EstimationResult(value=0.00768827677796402)"
                         ]
                     },
-                    "execution_count": 24,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "naive_graph = Graph([\n",
                 "    y <= x\n",
@@ -946,15 +927,15 @@
             "metadata": {},
             "source": [
                 "It turns out that in this dataset, the effect of $z$ is to exactly cancel out the effect of $x$ on $y$. So, we won't be able to estimate the effect directly. In addition, there is no sufficient adjustment set to recover the effect of $x$ on $y$. However, we can use ID to identify the estimand. Since we are taking $z$ as unobserved, we represent $x$ and $y$ as confounded in this model."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/latex": [
                             "$\\displaystyle E_{y} \\big[\\sum_{m} \\big({\\sum_{x} \\big({P(m, y, x) P(x) \\over P(m, x)}\\big) P(m, x = 1) \\over P(x = 1)}\\big)\\big] - E_{y} \\big[\\sum_{m} \\big({\\sum_{x} \\big({P(m, y, x) P(x) \\over P(m, x)}\\big) P(m, x = 0) \\over P(x = 0)}\\big)\\big]$"
                         ],
@@ -975,24 +956,24 @@
                 "effect = ATE(y, x)\n",
                 "estimand = g.identify(effect)\n",
                 "estimand.identified_estimand.display()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "EstimationResult(value=-0.4747611636992284)"
                         ]
                     },
-                    "execution_count": 28,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "model = MultinomialEstimator(df)\n",
                 "result = model.estimate(estimand)\n",
@@ -1005,15 +986,15 @@
             "metadata": {},
             "source": [
                 "We have successfully recovered the true effect. We can now use the inspection features of `pqp` to show the process which led to this result. This conventiently lists all the assumptions made during the analysis."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Data Processing\n",
@@ -1046,14 +1027,28 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "# Educational Materials\n",
+                "\n",
+                "I created a Medium article and two explainer videos to introduce the library to the causal inference community. The Medium article is available covered more of the theoretical background for SCM inference, while the videos are more practical and focus on how to use the library.\n",
+                "\n",
+                "- [Medium Article](https://medium.com/@leoware/causal-inference-a-four-stage-framework-7fc2f8deafe2)\n",
+                "- [First Video](https://www.loom.com/share/91dc669b931d487a84c8030c80d2391c)\n",
+                "- [Second Video](https://www.loom.com/share/7d8feab2b4f54a7caa59c495a9ce9858)"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "# References\n",
                 "\n",
                 "Bhattacharya, R., Nabi, R., & Shpitser, I. (2021). Semiparametric Inference For Causal Effects In Graphical Models With Hidden Variables (arXiv:2003.12659). arXiv. http://arxiv.org/abs/2003.12659\n",
                 "\n",
                 "\n",
                 "Breitling, L. P. (2010). dagR: A suite of R functions for directed acyclic graphs. Epidemiology (Cambridge, Mass.), 21(4), 586\u2013587. https://doi.org/10.1097/EDE.0b013e3181e09112\n",
                 "\n",
@@ -1136,154 +1131,154 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#induction\n",
+                "induction\n",
                 "\n",
                 "Structural causal modeling is all about principled approaches to induction, and the four-steps model of causal inference in Pearl's framework is a paradigm for inductive reasoning. I carefully explain how inference is conceptualized within this framework, and I draw connections between the framework and predictions that result on actual datasets. I show a deep understanding of the nuances of inductive reasoning."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#algorithms\n",
+                "algorithms\n",
                 "\n",
                 "I explain the tradeoffs between a number of approaches to identification. I carefully explain how each alternative works, and I provide a high-level overview of Shpitser\u2019s identification algorithm. I use asymptotic complexity to characterize tradeoffs. I implement Shpitser\u2019s identification algorithm.\n",
                 "\n",
                 "In the Technical Challenges section, I explain three algorithmic subroutines I developed for this project: the heuristic simplification algorith, the memory-sharing graph data structure, and my approach to estimation. In each case, I review the literature to characterize existing approaches, and drawing from this synthesis, I develop a novel approach. For the memory sharing graph data structure, I provide a sophisticated argument about computational complexity constraints to justify my approach."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#variables\n",
+                "variables\n",
                 "\n",
                 "I carefully handle distinctions between treatment, outcome, and control variables. I provide a subtle discussion of the relationships between treatment and outcome variables in the structural causal modeling framework. I explain how treatment variables in a causal estimand may be converted to control variables or excluded via identification.\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#probability\n",
+                "probability\n",
                 "\n",
                 "I show a deep understanding of probabilistic expressions and how they can be manipulated via the two rules of probability. I show how an extension to the basic logic of probability (do-expressions) can be incorporated into probabilistic reasoning. I draw on deep understanding of the logic of probability to criticise Brule's (2018) approach to estimation on the basis of its failure to guarantee positivity, and a I suggest a way to fix this problem using Bayesian statistics."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#deduction\n",
+                "deduction\n",
                 "\n",
                 "The do-calculus is a framework for using formal mathematics to reason about the very hairy and complex inductive problem of causal inference. I present the key intuitions behind the do-calculus, and then leverage an algorithm based on the do-calculus to perform identification. In addition, I make use of mathematical reasoning to prove a number of small supporting points."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#organization\n",
+                "organization\n",
                 "\n",
                 "\n",
                 "Structural causal modeling is a complex framework for reasoning about inductive reasoning. I break down this highly complex and interconnected topic into a series of short digestible insights, each of which I present in a subsection. I present the idea in an order which allows the reader to build an intuition for the field.\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#professionalism\n",
+                "professionalism\n",
                 "\n",
                 "I present a professional report using latex. The formatting and visual presentation of the report add to its credibility. I carefully follow citation standards."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#composition\n",
+                "composition\n",
                 "\n",
                 "I explain a complex, technically rigorous topic in a way that is accessible to someone educated in mathematics or computer science. I carefully handle jargon\u2014using it only when necessary and being careful to define my terms. I condense most of the information I have learned over the course of a year-long literature review into a few pages of background information. I balance concision with clarity in a highly difficult explanation."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#regression\n",
+                "regression\n",
                 "\n",
                 "I explain how regression modeling (under the name estimation) fits into the framework of structural causal modeling. I show a deep understanding of the role of regression in larger causal inference through my explanation of the role of abstract statistical estimators. Misapplication of principles of causal reasoning are one of the top reasons for poor use of regression models, and I present a report detailing how to avoid many of these.\n",
                 "\n",
                 "I demonstrate powerful understanding of regression through my development of an estimation technique relying on Bayesian priors."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#correlation\n",
+                "correlation\n",
                 "\n",
                 "\n",
                 "Rather than referring to correlation directly, I discuss the more general notion of statistical estimation. I explain how association in the joint distribution of a dataset relates to d-separation and live paths in the causal model. I explain how statistical association can change as a result of conditioning, and I present a complete account (based on Pearl\u2019s work) of when this occurs.\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#sampling\n",
+                "sampling\n",
                 "\n",
                 "\n",
                 "All of the difficulties of observational research fundamentally result from biased samples. In the final deliverable, I will explain how sampling bias in a real dataset can be controlled for using structural causal models."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#observationalstudy\n",
+                "observationalstudy\n",
                 "\n",
                 "\n",
                 "I implement a complex software library aimed to help researchers working with observational data. I show a deep understanding of the pitfalls of observational research through my explanation of confounding and collider bias. I explain how identification can be used to remove biases from estimation of causal effects. I present a tool whose primary purpose is to aid in conducting better observational studies."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#modeling\n",
+                "modeling\n",
                 "\n",
                 "\n",
                 "I show a deeply researched and incredibly rigorous understanding of the structural causal modeling approach to causal inference. I explain how the \u201cmoving parts\u201d of the model relate to changes in its predictions for the data. I implement a tool to aid in using structural causal modeling on real data.\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#comparisongroups\n",
+                "comparisongroups\n",
                 "\n",
                 "\n",
                 "In observational research, proper control groups are rarely available. The marginalization and control operations called for in the abstract estimator returned from identification can be interpreted as reweighting and excluding existing data in a way that synthetically generates a proper control group from available data. I will develop this analogy further in the final deliverable.\n"
             ]
         },
         {
             "attachments": {},
@@ -1294,87 +1289,87 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#CS110-ComputationalCritique\n",
+                "CS110-ComputationalCritique\n",
                 "\n",
                 "Throughout the technical challenges section, I weigh the relative merits of various approaches from the literature and present sophisticated technical arguments. I explain the tradeoffs between multiple approaches to estimation and explain why I chose this one. I demonstrate similar skill in discussion of simplification."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#CS110-ComputationalSolutions\n",
+                "CS110-ComputationalSolutions\n",
                 "\n",
                 "I best demonstrate this skill in my development of the memory-sharing graph data structure. I characterize the problem as requiring the ability to efficiently handle sequential calls to perform ancestor lookups, c-component lookups, and modifications to the graph. Given this characterization, I develop a novel approach to the problem which is both efficient and elegant. I provide a sophisticated argument about computational complexity constraints to justify my approach."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#CS110-DataStructures\n",
+                "CS110-DataStructures\n",
                 "\n",
                 "I best demonstrate this skill in my development of the memory-sharing graph data structure. I characterize the problem as requiring the ability to efficiently handle sequential calls to perform ancestor lookups, c-component lookups, and modifications to the graph. Given this characterization, I develop a novel approach to the problem which is both efficient and elegant. I provide a sophisticated argument about computational complexity constraints to justify my approach."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#CS110-CodeRedability\n",
+                "CS110-CodeRedability\n",
                 "\n",
                 "I present code at a very high level of readablility because of my aspiration to turn this project into an open-source library. I follow standards for commenting in both Python and Rust, and I generate documentation to aid use."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#CS146-GraphicalModels\n",
+                "CS146-GraphicalModels\n",
                 "\n",
                 "Structural causal models are a form of graphical model. I show a high level of understanding in the Background section, where I condense the literature on these models. I discuss how specific aspects of the graphical model (flow, connectedness) relate to conditional independence properties of the graph. I explain how modifications to the model (surgery) correspond to causal reasoning. I give clear explanations of how complex structures such as c-components and hedges affect our ability to make causal inferences.\n",
                 "\n",
                 "I also demonstrate this skill in my approach to the estimation problem, where I discuss the problem of marginalization and various approaches to solving it."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#CS146-ProbabilityTheory\n",
+                "CS146-ProbabilityTheory\n",
                 "\n",
                 "I present a software library designed for the symbolic manipulation of probability expressions and corresponding causal graphs. My literature review demonstrates deep understanding, and my simplification routine is a simple but powerful tool for programmatic symbolic manipulation of probability expressions."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#CS146-QuantProfessionalism\n",
+                "CS146-QuantProfessionalism\n",
                 "\n",
                 "I do everything I can to make my work useful to others, and I follow best practices for quantitative academic work and open source code. I present my work using Latex. I follow citaion practices. My code is available on GitHub and as an open-source distribution via PyPi. My code is well documented, commented, readable, and intended for reuse.\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#CS154-NumImplementation\n",
+                "CS154-NumImplementation\n",
                 "\n",
                 "I write performant, low-level code in a systems programming language to create a fast and correct interpretation of an algorithm. Although I will cover this more thoroughly in the final deliverable, I implement a marginalization and estimation algorithm for real data. Issues of converge are pressing."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -1394,146 +1389,68 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#qualitydeliverables\n",
+                "qualitydeliverables\n",
                 "\n",
                 "I present a concise but informative literature review, a strong characterization of the problem, a professional and appealing documentation website, a production-quality piece of software and a number of algorithmic insights."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#curation\n",
+                "curation\n",
                 "\n",
                 "For each section, I write in a concise but not terse manner, effectively characterizing each problem, summmarizing current work in the area, and presenting my own solution along with justification. I carefully select elements from my library to demo, focusing on aspects which are most likely to engage the reader and help them understand my work."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#navigation\n",
+                "navigation\n",
                 "\n",
                 "I am well on track to complete my capstone on time. I have completed my original goal (published implementation of ID, handling of conditional effects, python bindings, extensive testing, documentation), and I have extensive work towards a number of stretch goals (estimation, medium articles, ATE and CATE routines, randomized testing and benchmarking). I am on track to finish at least a couple of these if nothing goes terribly. I present a prioritization of the next steps along with a time estimate for each."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#outcomeanalysis\n",
+                "outcomeanalysis\n",
                 "\n",
                 "My two top goals for the implementation were correctness and performance, and my top goal for the python wrapper was usability. I have characterized the correctness by using hand-derived examples from the literature. I have done some work to characterize performance using computational complexity, and I am working towards performance benchmarks. I hope to better understand the usability of my interface by interacting with it in the next few weeks."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Appendix 2: Documentation\n",
-                "\n",
-                "This appendix contains documentation which can be found on the project website. I present it here as work compelted towards the project"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Landing Page\n",
-                "\n",
-                "![](2023-02-26-04-04-18.png)"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Quickstart Guide\n",
-                "\n",
-                "![](2023-02-26-04-04-52.png)\n",
-                "![](2023-02-26-04-05-15.png)\n",
-                "![](2023-02-26-04-05-29.png)"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Expression Module Documentation\n",
-                "\n",
-                "![](2023-02-26-04-06-16.png)"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Graph Module Documentation\n",
-                "\n",
-                "![](2023-02-26-04-06-43.png)"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Variable Module Documentation\n",
-                "\n",
-                "![](2023-02-26-04-07-22.png)"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Submodule Documentation\n",
-                "\n",
-                "![](2023-02-26-04-07-57.png)\n",
-                "![](2023-02-26-04-08-12.png)\n",
-                "![](2023-02-26-04-08-27.png)\n",
-                "![](2023-02-26-04-08-47.png)\n",
-                "![](2023-02-26-04-09-02.png)\n",
-                "![](2023-02-26-04-09-16.png)\n",
-                "![](2023-02-26-04-09-29.png)"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Appendix 3: Code"
+                "## Appendix 2: Code"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Code Relating to Examples in the Text"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -1604,15 +1521,15 @@
                             "0  0  0  0  2\n",
                             "1  1  1  0  3\n",
                             "2  0  1  1  1\n",
                             "3  0  0  0  2\n",
                             "4  0  1  1  1"
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import pandas as pd\n",
                 "import numpy as np\n",
@@ -1624,21 +1541,14 @@
                 "df[\"x\"] = (0.5*df.z + np.random.random(size=1000) > 0.75).astype(int)\n",
                 "df[\"m\"] = (0.5*df.x + np.random.random(size=1000) > 0.75).astype(int)\n",
                 "df[\"y\"] = df.z - df.m + 2\n",
                 "\n",
                 "df.to_csv(\"demo1.csv\", index=False)\n",
                 "df.head()"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "venv",
             "language": "python",
             "name": "python3"
```

### Comparing `pqp-0.3.0/writeup/PQP.ipynb` & `pqp-0.3.1/writeup/PQP.ipynb`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/writeup/agg.ipynb` & `pqp-0.3.1/writeup/agg.ipynb`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/writeup/build.py` & `pqp-0.3.1/writeup/build.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/writeup/demo.ipynb` & `pqp-0.3.1/writeup/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/writeup/demo1.csv` & `pqp-0.3.1/writeup/demo1.csv`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/writeup/doctordemo.csv` & `pqp-0.3.1/writeup/doctordemo.csv`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/writeup/grab_code.py` & `pqp-0.3.1/writeup/grab_code.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/writeup/supplement.py` & `pqp-0.3.1/writeup/supplement.py`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/Cargo.lock` & `pqp-0.3.1/Cargo.lock`

 * *Files identical despite different names*

### Comparing `pqp-0.3.0/PKG-INFO` & `pqp-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pqp
-Version: 0.3.0
+Version: 0.3.1
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: sphinx; extra == 'dev'
-Requires-Dist: maturin; extra == 'dev'
-Requires-Dist: sphinx-autobuild; extra == 'dev'
-Requires-Dist: toml; extra == 'dev'
-Requires-Dist: pytest; extra == 'dev'
-Requires-Dist: matplotlib; extra == 'dev'
-Requires-Dist: numpy; extra == 'dev'
-Requires-Dist: networkx; extra == 'dev'
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: tomli
+Requires-Dist: matplotlib
+Requires-Dist: sphinx ; extra == 'dev'
+Requires-Dist: maturin ; extra == 'dev'
+Requires-Dist: sphinx-autobuild ; extra == 'dev'
+Requires-Dist: pytest ; extra == 'dev'
+Requires-Dist: networkx ; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE.txt
 Summary: Subroutines for structural causal modeling
 Keywords: causal inference,causal identification
 Author: Leo Ware
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

