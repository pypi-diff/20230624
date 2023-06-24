# Comparing `tmp/xsdata-23.5.tar.gz` & `tmp/xsdata-23.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsdata-23.5.tar", last modified: Sun May 21 10:07:07 2023, max compression
+gzip compressed data, was "xsdata-23.6.tar", last modified: Sat Jun 24 15:31:04 2023, max compression
```

## Comparing `xsdata-23.5.tar` & `xsdata-23.6.tar`

### file list

```diff
@@ -1,498 +1,498 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.395054 xsdata-23.5/
--rw-r--r--   0 runner    (1001) docker     (123)    32061 2023-05-21 10:06:58.000000 xsdata-23.5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-21 10:06:58.000000 xsdata-23.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-21 10:06:58.000000 xsdata-23.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-05-21 10:07:07.395054 xsdata-23.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-05-21 10:06:58.000000 xsdata-23.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.311052 xsdata-23.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-21 10:06:58.000000 xsdata-23.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.311052 xsdata-23.5/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-21 10:06:58.000000 xsdata-23.5/docs/_ext/xsdatadocs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.311052 xsdata-23.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-21 10:06:58.000000 xsdata-23.5/docs/_static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-21 10:06:58.000000 xsdata-23.5/docs/_static/logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-21 10:06:58.000000 xsdata-23.5/docs/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.311052 xsdata-23.5/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-21 10:06:58.000000 xsdata-23.5/docs/_templates/dataclass.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.315052 xsdata-23.5/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/codegen.rst
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/generics.rst
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/parsing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/serializing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/xml-context.rst
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/xml-datatypes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/xml-handlers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/xml-nodes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/xml-writers.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-21 10:06:58.000000 xsdata-23.5/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-21 10:06:58.000000 xsdata-23.5/docs/codegen.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-21 10:06:58.000000 xsdata-23.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-21 10:06:58.000000 xsdata-23.5/docs/data-types-table.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-05-21 10:06:58.000000 xsdata-23.5/docs/data-types.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.319052 xsdata-23.5/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/compound-fields.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/custom-class-factory.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/custom-property-names.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/custom-type-mapping.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/dataclasses-features.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/docstrings.rst
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/dtd-modeling.rst
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/json-modeling.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/pycode-serializer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/samples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/w3c-suite.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/working-with-wildcards.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/wrapped-list.rst
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/xml-modeling.rst
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.319052 xsdata-23.5/docs/faq/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-21 10:06:58.000000 xsdata-23.5/docs/faq/error-parsing-dtd.rst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-21 10:06:58.000000 xsdata-23.5/docs/faq/how-can-i-compare-output-results-between-versions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-21 10:06:58.000000 xsdata-23.5/docs/faq/why-are-elements-out-of-order.rst
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-21 10:06:58.000000 xsdata-23.5/docs/faq/why-i-get-a-typeerror-requires-a-single-type.rst
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-21 10:06:58.000000 xsdata-23.5/docs/faq/why-non-nullable-fields-are-marked-as-optional.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-21 10:06:58.000000 xsdata-23.5/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-21 10:06:58.000000 xsdata-23.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-21 10:06:58.000000 xsdata-23.5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-05-21 10:06:58.000000 xsdata-23.5/docs/json.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-21 10:06:58.000000 xsdata-23.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-21 10:06:58.000000 xsdata-23.5/docs/models.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-21 10:06:58.000000 xsdata-23.5/docs/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.319052 xsdata-23.5/docs/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/docs/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-21 10:06:58.000000 xsdata-23.5/docs/scripts/generate_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-21 10:06:58.000000 xsdata-23.5/docs/wsdl.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-05-21 10:06:58.000000 xsdata-23.5/docs/xml.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-21 10:07:07.395054 xsdata-23.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 10:06:58.000000 xsdata-23.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.323052 xsdata-23.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-21 10:06:58.000000 xsdata-23.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.323052 xsdata-23.5/tests/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.331052 xsdata-23.5/tests/codegen/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_add_attribute_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_calculate_attribute_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_create_compound_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_designate_class_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_filter_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_flatten_attribute_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    20197 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_flatten_class_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_merge_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    18994 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_process_attributes_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_process_mixed_content_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_rename_duplicate_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_rename_duplicate_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_reset_attribute_sequence_numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_reset_attribute_sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_sanitize_attributes_default_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_sanitize_enumeration_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_unnest_inner_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_update_attributes_effective_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_vacuum_inner_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_validate_attributes_overrides.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.331052 xsdata-23.5/tests/codegen/mappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29551 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/mappers/test_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/mappers/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/mappers/test_dtd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/mappers/test_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    17815 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/mappers/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.331052 xsdata-23.5/tests/codegen/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/models/test_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/models/test_attr_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/models/test_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/models/test_restrictions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.335052 xsdata-23.5/tests/codegen/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/parsers/test_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/parsers/test_dtd.py
--rw-r--r--   0 runner    (1001) docker     (123)    16367 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/parsers/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/test_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/test_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    19370 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14142 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/test_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-21 10:06:58.000000 xsdata-23.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.335052 xsdata-23.5/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.335052 xsdata-23.5/tests/fixtures/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/annotations/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/annotations/model.xsd
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/annotations/sample.xml
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/annotations/units.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/annotations/units.xsd
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/annotations/xsdata.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.339053 xsdata-23.5/tests/fixtures/artists/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/artists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/artists/art001.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/artists/art002.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/artists/art003.xml
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/artists/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.339053 xsdata-23.5/tests/fixtures/books/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/bk001.xml
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/bk002.xml
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/books-xinclude.xml
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/books.json
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/books.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/books.xml
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/books_auto_ns.xml
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/books_default_ns.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/schema.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.343053 xsdata-23.5/tests/fixtures/calculator/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/calculator/AddRQ.xml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/calculator/AddRS.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/calculator/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/calculator/services.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.343053 xsdata-23.5/tests/fixtures/compound/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/compound/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/compound/sample.json
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/compound/sample.xml
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/compound/sample.xsdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/compound/schema.xsd
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.343053 xsdata-23.5/tests/fixtures/docstrings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.343053 xsdata-23.5/tests/fixtures/docstrings/accessible/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/accessible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/accessible/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.343053 xsdata-23.5/tests/fixtures/docstrings/blank/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/blank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/blank/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/docstrings/google/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/google/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/docstrings/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/numpy/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/docstrings/rst/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/rst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/rst/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/schema.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/dtd/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/dtd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/dtd/complete_example.dtd
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/dtd/default_namespace.dtd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/dtd/models/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/dtd/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/dtd/models/complete_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/dtd/prefix_namespace.dtd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/hello/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/hello/HelloRQ.xml
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/hello/HelloRS.xml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/hello/HelloRS_SoapFault.xml
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/hello/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/hello/hello.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/hello/hello.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/hello/hello.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/primer/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/primer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/primer/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/primer/order.xsd
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/primer/sample.json
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/primer/sample.xml
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/primer/sample.xsdata.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/series/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/series/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/series/samples/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/series/samples/show1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/series/samples/show2.json
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/series/series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/stripe/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/stripe/.xsdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/stripe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/stripe/models/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/stripe/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/stripe/models/balance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/stripe/samples/
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/stripe/samples/balance.json
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/submodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.351053 xsdata-23.5/tests/formats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.351053 xsdata-23.5/tests/formats/dataclass/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.351053 xsdata-23.5/tests/formats/dataclass/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18738 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/models/test_builders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.351053 xsdata-23.5/tests/formats/dataclass/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.351053 xsdata-23.5/tests/formats/dataclass/parsers/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/handlers/test_lxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/handlers/test_native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.351053 xsdata-23.5/tests/formats/dataclass/parsers/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_primitive.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_skip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_union.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_wildcard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/test_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.355053 xsdata-23.5/tests/formats/dataclass/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/serializers/test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/serializers/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/serializers/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    24101 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/serializers/test_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.355053 xsdata-23.5/tests/formats/dataclass/serializers/writers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/serializers/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/serializers/writers/test_lxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/serializers/writers/test_native.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/test_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    33895 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/test_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/test_mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.355053 xsdata-23.5/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.355053 xsdata-23.5/tests/integration/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/benchmarks/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/benchmarks/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/benchmarks/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_artists.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_books.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_compound.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_dtd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_hello_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_primer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.355053 xsdata-23.5/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.355053 xsdata-23.5/tests/models/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/enums/test_datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    21919 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/test_datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/test_type_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.355053 xsdata-23.5/tests/models/typemapping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/typemapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/typemapping/city.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/typemapping/house.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/typemapping/street.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.359053 xsdata-23.5/tests/models/wsdl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/wsdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/wsdl/test_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/wsdl/test_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/wsdl/test_port_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.359053 xsdata-23.5/tests/models/xsd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_alternative.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_annotation_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_any.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_any_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_attribute_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_complex_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_complex_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_element.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_enumeration.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_restriction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_simple_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_union.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-05-21 10:06:58.000000 xsdata-23.5/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.359053 xsdata-23.5/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-21 10:06:58.000000 xsdata-23.5/tests/utils/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-21 10:06:58.000000 xsdata-23.5/tests/utils/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-21 10:06:58.000000 xsdata-23.5/tests/utils/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-21 10:06:58.000000 xsdata-23.5/tests/utils/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-05-21 10:06:58.000000 xsdata-23.5/tests/utils/test_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-21 10:06:58.000000 xsdata-23.5/tests/utils/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-21 10:06:58.000000 xsdata-23.5/tests/utils/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-05-21 10:06:58.000000 xsdata-23.5/tests/utils/test_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-21 10:06:58.000000 xsdata-23.5/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.363053 xsdata-23.5/xsdata/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.363053 xsdata-23.5/xsdata/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.367053 xsdata-23.5/xsdata/codegen/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/add_attribute_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/calculate_attribute_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/create_compound_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/designate_class_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/filter_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/flatten_attribute_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/flatten_class_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/merge_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/process_attributes_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/process_mixed_content_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/rename_duplicate_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/rename_duplicate_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/reset_attribute_sequence_numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/reset_attribute_sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/sanitize_attributes_default_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/sanitize_enumeration_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/unnest_inner_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/update_attributes_effective_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/vacuum_inner_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/validate_attributes_overrides.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.371053 xsdata-23.5/xsdata/codegen/mappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/mappers/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/mappers/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/mappers/dtd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/mappers/element.py
--rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/mappers/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    20155 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.371053 xsdata-23.5/xsdata/codegen/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/parsers/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/parsers/dtd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/parsers/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.371053 xsdata-23.5/xsdata/formats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16134 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.375053 xsdata-23.5/xsdata/formats/dataclass/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    26070 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.375053 xsdata-23.5/xsdata/formats/dataclass/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17777 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/models/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/models/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/models/generics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.379053 xsdata-23.5/xsdata/formats/dataclass/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/bases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.379053 xsdata-23.5/xsdata/formats/dataclass/parsers/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/handlers/lxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/handlers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.383054 xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14972 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/primitive.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/skip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/union.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/wildcard.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.383054 xsdata-23.5/xsdata/formats/dataclass/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/serializers/code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/serializers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/serializers/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.383054 xsdata-23.5/xsdata/formats/dataclass/serializers/writers/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/serializers/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/serializers/writers/lxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/serializers/writers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)    16180 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/serializers/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.387054 xsdata-23.5/xsdata/formats/dataclass/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/class.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/docstrings.accessible.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/docstrings.blank.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/docstrings.google.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/docstrings.numpy.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/docstrings.rst.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/enum.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/imports.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/module.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/package.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/service.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/transports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.391054 xsdata-23.5/xsdata/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17796 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/models/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20264 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/models/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/models/dtd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/models/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/models/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/models/wsdl.py
--rw-r--r--   0 runner    (1001) docker     (123)    36929 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/models/xsd.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.391054 xsdata-23.5/xsdata/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/schemas/mathml3-common.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    28457 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/schemas/mathml3-content.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    84129 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/schemas/mathml3-presentation.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/schemas/mathml3-strict-content.xsd
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/schemas/mathml3.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/schemas/xlink.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/schemas/xml.xsd
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/schemas/xsi.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.395054 xsdata-23.5/xsdata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    17285 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.363053 xsdata-23.5/xsdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-05-21 10:07:07.000000 xsdata-23.5/xsdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-05-21 10:07:07.000000 xsdata-23.5/xsdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 10:07:07.000000 xsdata-23.5/xsdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-21 10:07:07.000000 xsdata-23.5/xsdata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-21 10:07:07.000000 xsdata-23.5/xsdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-21 10:07:07.000000 xsdata-23.5/xsdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.954966 xsdata-23.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    33027 2023-06-24 15:30:56.000000 xsdata-23.6/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-24 15:30:56.000000 xsdata-23.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-24 15:30:56.000000 xsdata-23.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-24 15:31:04.954966 xsdata-23.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-24 15:30:56.000000 xsdata-23.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.890965 xsdata-23.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-24 15:30:56.000000 xsdata-23.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.890965 xsdata-23.6/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-24 15:30:56.000000 xsdata-23.6/docs/_ext/xsdatadocs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.890965 xsdata-23.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-24 15:30:56.000000 xsdata-23.6/docs/_static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-24 15:30:56.000000 xsdata-23.6/docs/_static/logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-24 15:30:56.000000 xsdata-23.6/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.890965 xsdata-23.6/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-24 15:30:56.000000 xsdata-23.6/docs/_templates/dataclass.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.890965 xsdata-23.6/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-24 15:30:56.000000 xsdata-23.6/docs/api/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-24 15:30:56.000000 xsdata-23.6/docs/api/codegen.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-24 15:30:56.000000 xsdata-23.6/docs/api/generics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-24 15:30:56.000000 xsdata-23.6/docs/api/parsing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-24 15:30:56.000000 xsdata-23.6/docs/api/serializing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-24 15:30:56.000000 xsdata-23.6/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-24 15:30:56.000000 xsdata-23.6/docs/api/xml-context.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-24 15:30:56.000000 xsdata-23.6/docs/api/xml-datatypes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-24 15:30:56.000000 xsdata-23.6/docs/api/xml-handlers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-24 15:30:56.000000 xsdata-23.6/docs/api/xml-nodes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-24 15:30:56.000000 xsdata-23.6/docs/api/xml-writers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-24 15:30:56.000000 xsdata-23.6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-24 15:30:56.000000 xsdata-23.6/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-24 15:30:56.000000 xsdata-23.6/docs/codegen.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-24 15:30:56.000000 xsdata-23.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-24 15:30:56.000000 xsdata-23.6/docs/data-types-table.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-06-24 15:30:56.000000 xsdata-23.6/docs/data-types.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.894965 xsdata-23.6/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-24 15:30:56.000000 xsdata-23.6/docs/examples/compound-fields.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-24 15:30:56.000000 xsdata-23.6/docs/examples/custom-class-factory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-24 15:30:56.000000 xsdata-23.6/docs/examples/custom-property-names.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-24 15:30:56.000000 xsdata-23.6/docs/examples/custom-type-mapping.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-24 15:30:56.000000 xsdata-23.6/docs/examples/dataclasses-features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-24 15:30:56.000000 xsdata-23.6/docs/examples/docstrings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-24 15:30:56.000000 xsdata-23.6/docs/examples/dtd-modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-24 15:30:56.000000 xsdata-23.6/docs/examples/extending-models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-24 15:30:56.000000 xsdata-23.6/docs/examples/json-modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-24 15:30:56.000000 xsdata-23.6/docs/examples/pycode-serializer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-24 15:30:56.000000 xsdata-23.6/docs/examples/samples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-24 15:30:56.000000 xsdata-23.6/docs/examples/w3c-suite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-24 15:30:56.000000 xsdata-23.6/docs/examples/working-with-wildcards.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-24 15:30:56.000000 xsdata-23.6/docs/examples/wrapped-list.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-24 15:30:56.000000 xsdata-23.6/docs/examples/xml-modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-24 15:30:56.000000 xsdata-23.6/docs/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.894965 xsdata-23.6/docs/faq/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-24 15:30:56.000000 xsdata-23.6/docs/faq/error-parsing-dtd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-24 15:30:56.000000 xsdata-23.6/docs/faq/how-can-i-compare-output-results-between-versions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-24 15:30:56.000000 xsdata-23.6/docs/faq/why-are-elements-out-of-order.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-24 15:30:56.000000 xsdata-23.6/docs/faq/why-i-get-a-typeerror-requires-a-single-type.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-24 15:30:56.000000 xsdata-23.6/docs/faq/why-non-nullable-fields-are-marked-as-optional.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-24 15:30:56.000000 xsdata-23.6/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-24 15:30:56.000000 xsdata-23.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-24 15:30:56.000000 xsdata-23.6/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-06-24 15:30:56.000000 xsdata-23.6/docs/json.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-24 15:30:56.000000 xsdata-23.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-06-24 15:30:56.000000 xsdata-23.6/docs/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-24 15:30:56.000000 xsdata-23.6/docs/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.894965 xsdata-23.6/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/docs/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-24 15:30:56.000000 xsdata-23.6/docs/scripts/generate_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-06-24 15:30:56.000000 xsdata-23.6/docs/wsdl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12791 2023-06-24 15:30:56.000000 xsdata-23.6/docs/xml.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-24 15:30:56.000000 xsdata-23.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 15:31:04.954966 xsdata-23.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.894965 xsdata-23.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-24 15:30:56.000000 xsdata-23.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.898965 xsdata-23.6/tests/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.902965 xsdata-23.6/tests/codegen/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/handlers/test_add_attribute_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/handlers/test_calculate_attribute_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/handlers/test_create_compound_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/handlers/test_designate_class_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/handlers/test_filter_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/handlers/test_flatten_attribute_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20197 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/handlers/test_flatten_class_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/handlers/test_merge_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18994 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/handlers/test_process_attributes_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/handlers/test_process_mixed_content_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/handlers/test_rename_duplicate_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/handlers/test_rename_duplicate_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/handlers/test_reset_attribute_sequence_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/handlers/test_reset_attribute_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/handlers/test_sanitize_attributes_default_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/handlers/test_sanitize_enumeration_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/handlers/test_unnest_inner_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/handlers/test_update_attributes_effective_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/handlers/test_vacuum_inner_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/handlers/test_validate_attributes_overrides.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.902965 xsdata-23.6/tests/codegen/mappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29551 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/mappers/test_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/mappers/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/mappers/test_dtd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/mappers/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17815 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/mappers/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.902965 xsdata-23.6/tests/codegen/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/models/test_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/models/test_attr_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/models/test_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/models/test_restrictions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.902965 xsdata-23.6/tests/codegen/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/parsers/test_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/parsers/test_dtd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16367 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/parsers/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/test_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/test_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19370 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14142 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-24 15:30:56.000000 xsdata-23.6/tests/codegen/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-24 15:30:56.000000 xsdata-23.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.902965 xsdata-23.6/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.906965 xsdata-23.6/tests/fixtures/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/annotations/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/annotations/model.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/annotations/sample.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/annotations/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/annotations/units.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/annotations/xsdata.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.906965 xsdata-23.6/tests/fixtures/artists/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/artists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/artists/art001.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/artists/art002.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/artists/art003.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     9186 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/artists/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.906965 xsdata-23.6/tests/fixtures/books/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/books/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/books/bk001.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/books/bk002.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/books/books-xinclude.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/books/books.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/books/books.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/books/books.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/books/books_auto_ns.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/books/books_default_ns.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/books/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/books/schema.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.910965 xsdata-23.6/tests/fixtures/calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/calculator/AddRQ.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/calculator/AddRS.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/calculator/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/calculator/services.wsdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.910965 xsdata-23.6/tests/fixtures/compound/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/compound/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/compound/sample.json
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/compound/sample.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/compound/sample.xsdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/compound/schema.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.910965 xsdata-23.6/tests/fixtures/docstrings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/docstrings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.910965 xsdata-23.6/tests/fixtures/docstrings/accessible/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/docstrings/accessible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/docstrings/accessible/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.910965 xsdata-23.6/tests/fixtures/docstrings/blank/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/docstrings/blank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/docstrings/blank/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.910965 xsdata-23.6/tests/fixtures/docstrings/google/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/docstrings/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/docstrings/google/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.910965 xsdata-23.6/tests/fixtures/docstrings/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/docstrings/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/docstrings/numpy/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.910965 xsdata-23.6/tests/fixtures/docstrings/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/docstrings/rst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/docstrings/rst/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/docstrings/schema.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.910965 xsdata-23.6/tests/fixtures/dtd/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/dtd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/dtd/complete_example.dtd
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/dtd/default_namespace.dtd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.914965 xsdata-23.6/tests/fixtures/dtd/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/dtd/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/dtd/models/complete_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/dtd/prefix_namespace.dtd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.914965 xsdata-23.6/tests/fixtures/hello/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/hello/HelloRQ.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/hello/HelloRS.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/hello/HelloRS_SoapFault.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/hello/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/hello/hello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/hello/hello.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/hello/hello.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.914965 xsdata-23.6/tests/fixtures/primer/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/primer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/primer/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/primer/order.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/primer/sample.json
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/primer/sample.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/primer/sample.xsdata.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.914965 xsdata-23.6/tests/fixtures/series/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/series/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.914965 xsdata-23.6/tests/fixtures/series/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/series/samples/show1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/series/samples/show2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/series/series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.914965 xsdata-23.6/tests/fixtures/stripe/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/stripe/.xsdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/stripe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.914965 xsdata-23.6/tests/fixtures/stripe/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/stripe/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/stripe/models/balance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.914965 xsdata-23.6/tests/fixtures/stripe/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/stripe/samples/balance.json
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-24 15:30:56.000000 xsdata-23.6/tests/fixtures/submodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.918965 xsdata-23.6/tests/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.918965 xsdata-23.6/tests/formats/dataclass/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.918965 xsdata-23.6/tests/formats/dataclass/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18738 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/models/test_builders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.918965 xsdata-23.6/tests/formats/dataclass/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.918965 xsdata-23.6/tests/formats/dataclass/parsers/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/parsers/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/parsers/handlers/test_lxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/parsers/handlers/test_native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.922966 xsdata-23.6/tests/formats/dataclass/parsers/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/parsers/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/parsers/nodes/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/parsers/nodes/test_primitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/parsers/nodes/test_skip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/parsers/nodes/test_standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/parsers/nodes/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/parsers/nodes/test_wildcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/parsers/nodes/test_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/parsers/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/parsers/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/parsers/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/parsers/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/parsers/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/parsers/test_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.922966 xsdata-23.6/tests/formats/dataclass/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/serializers/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/serializers/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/serializers/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24101 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/serializers/test_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.922966 xsdata-23.6/tests/formats/dataclass/serializers/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/serializers/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/serializers/writers/test_lxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/serializers/writers/test_native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/test_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40645 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/test_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/dataclass/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-24 15:30:56.000000 xsdata-23.6/tests/formats/test_mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.926966 xsdata-23.6/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.926966 xsdata-23.6/tests/integration/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/integration/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-24 15:30:56.000000 xsdata-23.6/tests/integration/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-24 15:30:56.000000 xsdata-23.6/tests/integration/benchmarks/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-24 15:30:56.000000 xsdata-23.6/tests/integration/benchmarks/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-24 15:30:56.000000 xsdata-23.6/tests/integration/benchmarks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-24 15:30:56.000000 xsdata-23.6/tests/integration/test_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-24 15:30:56.000000 xsdata-23.6/tests/integration/test_artists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-24 15:30:56.000000 xsdata-23.6/tests/integration/test_books.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-24 15:30:56.000000 xsdata-23.6/tests/integration/test_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-24 15:30:56.000000 xsdata-23.6/tests/integration/test_compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-24 15:30:56.000000 xsdata-23.6/tests/integration/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-24 15:30:56.000000 xsdata-23.6/tests/integration/test_dtd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-24 15:30:56.000000 xsdata-23.6/tests/integration/test_hello_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-24 15:30:56.000000 xsdata-23.6/tests/integration/test_primer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-24 15:30:56.000000 xsdata-23.6/tests/integration/test_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-24 15:30:56.000000 xsdata-23.6/tests/integration/test_stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.926966 xsdata-23.6/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.926966 xsdata-23.6/tests/models/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/enums/test_datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21919 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/test_datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/test_type_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.926966 xsdata-23.6/tests/models/typemapping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/typemapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/typemapping/city.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/typemapping/house.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/typemapping/street.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.926966 xsdata-23.6/tests/models/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/wsdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/wsdl/test_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/wsdl/test_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/wsdl/test_port_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.930966 xsdata-23.6/tests/models/xsd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/xsd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/xsd/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/xsd/test_alternative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/xsd/test_annotation_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/xsd/test_any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/xsd/test_any_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/xsd/test_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/xsd/test_attribute_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/xsd/test_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/xsd/test_complex_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/xsd/test_complex_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/xsd/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/xsd/test_enumeration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/xsd/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/xsd/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/xsd/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/xsd/test_restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/xsd/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/xsd/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/xsd/test_simple_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-24 15:30:56.000000 xsdata-23.6/tests/models/xsd/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-06-24 15:30:56.000000 xsdata-23.6/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.930966 xsdata-23.6/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-24 15:30:56.000000 xsdata-23.6/tests/utils/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-24 15:30:56.000000 xsdata-23.6/tests/utils/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-06-24 15:30:56.000000 xsdata-23.6/tests/utils/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-24 15:30:56.000000 xsdata-23.6/tests/utils/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-06-24 15:30:56.000000 xsdata-23.6/tests/utils/test_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-24 15:30:56.000000 xsdata-23.6/tests/utils/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-24 15:30:56.000000 xsdata-23.6/tests/utils/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-06-24 15:30:56.000000 xsdata-23.6/tests/utils/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.934966 xsdata-23.6/xsdata/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.934966 xsdata-23.6/xsdata/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.938966 xsdata-23.6/xsdata/codegen/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/handlers/add_attribute_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/handlers/calculate_attribute_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/handlers/create_compound_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/handlers/designate_class_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/handlers/filter_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/handlers/flatten_attribute_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/handlers/flatten_class_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/handlers/merge_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/handlers/process_attributes_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/handlers/process_mixed_content_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/handlers/rename_duplicate_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/handlers/rename_duplicate_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/handlers/reset_attribute_sequence_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/handlers/reset_attribute_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/handlers/sanitize_attributes_default_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/handlers/sanitize_enumeration_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/handlers/unnest_inner_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/handlers/update_attributes_effective_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/handlers/vacuum_inner_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/handlers/validate_attributes_overrides.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.938966 xsdata-23.6/xsdata/codegen/mappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/mappers/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/mappers/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/mappers/dtd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/mappers/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/mappers/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20155 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.942966 xsdata-23.6/xsdata/codegen/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/parsers/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/parsers/dtd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/parsers/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/codegen/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.942966 xsdata-23.6/xsdata/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.942966 xsdata-23.6/xsdata/formats/dataclass/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29441 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.942966 xsdata-23.6/xsdata/formats/dataclass/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/models/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/models/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/models/generics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.942966 xsdata-23.6/xsdata/formats/dataclass/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/parsers/bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/parsers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.946966 xsdata-23.6/xsdata/formats/dataclass/parsers/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/parsers/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/parsers/handlers/lxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/parsers/handlers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11828 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/parsers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/parsers/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.946966 xsdata-23.6/xsdata/formats/dataclass/parsers/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/parsers/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14972 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/parsers/nodes/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/parsers/nodes/primitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/parsers/nodes/skip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/parsers/nodes/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/parsers/nodes/union.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/parsers/nodes/wildcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/parsers/nodes/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/parsers/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/parsers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/parsers/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.946966 xsdata-23.6/xsdata/formats/dataclass/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/serializers/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/serializers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/serializers/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.946966 xsdata-23.6/xsdata/formats/dataclass/serializers/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/serializers/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/serializers/writers/lxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/serializers/writers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/serializers/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.950966 xsdata-23.6/xsdata/formats/dataclass/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/templates/class.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/templates/docstrings.accessible.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/templates/docstrings.blank.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/templates/docstrings.google.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/templates/docstrings.numpy.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/templates/docstrings.rst.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/templates/enum.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/templates/imports.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/templates/module.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/templates/package.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/templates/service.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/transports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/dataclass/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/formats/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.950966 xsdata-23.6/xsdata/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21294 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20286 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/models/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/models/dtd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/models/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/models/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/models/wsdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36973 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/models/xsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.950966 xsdata-23.6/xsdata/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/schemas/mathml3-common.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    28457 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/schemas/mathml3-content.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    84129 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/schemas/mathml3-presentation.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/schemas/mathml3-strict-content.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/schemas/mathml3.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/schemas/xlink.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/schemas/xml.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/schemas/xsi.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.954966 xsdata-23.6/xsdata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/utils/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/utils/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/utils/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/utils/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/utils/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/utils/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17285 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-06-24 15:30:56.000000 xsdata-23.6/xsdata/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:31:04.934966 xsdata-23.6/xsdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-24 15:31:04.000000 xsdata-23.6/xsdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-06-24 15:31:04.000000 xsdata-23.6/xsdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 15:31:04.000000 xsdata-23.6/xsdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-24 15:31:04.000000 xsdata-23.6/xsdata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-24 15:31:04.000000 xsdata-23.6/xsdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-24 15:31:04.000000 xsdata-23.6/xsdata.egg-info/top_level.txt
```

### Comparing `xsdata-23.5/CHANGES.rst` & `xsdata-23.6/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+23.6 (2023-06-24)
+-----------------
+- Fixed conflicting enum values leading to wrong default values (`#806 <https://github.com/tefra/xsdata/pull/806>`_)
+- Added support for custom decorators and base classes (`#793 <https://github.com/tefra/xsdata/pull/793>`_)
+- Added parser config to load external dtd to resolve entities (`#797 <https://github.com/tefra/xsdata/pull/797>`_)
+- Added requests sessions on the wsdl client transport (`#798 <https://github.com/tefra/xsdata/pull/798>`_)
+- Added support subscriptable types and UnionType (`#801 <https://github.com/tefra/xsdata/pull/801>`_)
+- Added option to restrict models package for auto-locator (`#809 <https://github.com/tefra/xsdata/pull/809>`_)
+- Updated context to only cache supported classes (`#796 <https://github.com/tefra/xsdata/pull/796>`_)
+- Removed tox requirement (`#800 <https://github.com/tefra/xsdata/pull/800>`_)
+- Converted to pyproject.toml (`#802 <https://github.com/tefra/xsdata/pull/802>`_)
+
 23.5 (2023-05-21)
 ------------------
 - Fixed XML meta var index conflicts.
 - Fixed mixed content handling for DTD elements. (`#749 <https://github.com/tefra/xsdata/pull/749>`_, `#762 <https://github.com/tefra/xsdata/pull/762>`_)
 - Fixed an issue with required attributes turning into optional ones.
 - Fixed calculation of min/max occurs when parsing XML/JSON documents. (`#756 <https://github.com/tefra/xsdata/pull/756>`_)
 - Fixed calculation of min/max occurs when parsing DTD choice content types. (`#760 <https://github.com/tefra/xsdata/pull/760>`_)
```

### Comparing `xsdata-23.5/LICENSE` & `xsdata-23.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/PKG-INFO` & `xsdata-23.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: xsdata
-Version: 23.5
+Version: 23.6
 Summary: Python XML Binding
-Home-page: https://github.com/tefra/xsdata
-Author: Christodoulos Tsoulloftas
-Author-email: "chris@komposta.net",
+Author-email: Christodoulos Tsoulloftas <chris@komposta.net>
 License: MIT
+Project-URL: Homepage, https://github.com/tefra/xsdata
 Project-URL: Source, https://github.com/tefra/xsdata
 Project-URL: Documentation, https://xsdata.readthedocs.io/
 Project-URL: Changelog, https://xsdata.readthedocs.io/en/latest/changelog.html
 Keywords: xsd,wsdl,schema,dtd,binding,xml,json,dataclasses,generator,cli
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Text Processing :: Markup :: XML
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: cli
@@ -131,43 +131,18 @@
   - Handlers and Writers based on lxml and native xml python
   - Support wildcard elements and attributes
   - Support xinclude statements and unknown properties
   - Customize behaviour through config
 
 
 
-Changelog: 23.5 (2023-05-21)
+Changelog: 23.6 (2023-06-24)
 ----------------------------
-- Fixed XML meta var index conflicts.
-- Fixed mixed content handling for DTD elements. (`#749 <https://github.com/tefra/xsdata/pull/749>`_, `#762 <https://github.com/tefra/xsdata/pull/762>`_)
-- Fixed an issue with required attributes turning into optional ones.
-- Fixed calculation of min/max occurs when parsing XML/JSON documents. (`#756 <https://github.com/tefra/xsdata/pull/756>`_)
-- Fixed calculation of min/max occurs when parsing DTD choice content types. (`#760 <https://github.com/tefra/xsdata/pull/760>`_)
-- Fixed an issue when parsing tail content for compound wildcard elements.
-- Fixed an issue with the code analyzer not fully processing some classes.
-- Fixed an issue with the code analyzer taking forever to process very large enumerations. (`#776 <https://github.com/tefra/xsdata/issue/776>`_)
-- Fixed an issue in the JSON parser with optional choice elements.
-- Updated the transformer to silently ignore malformed JSON files. (`#750 <https://github.com/tefra/xsdata/pull/750>`_)
-- Updated the override attribute handler to fix naming conflicts.
-- Updated the override attribute handler to allow wildcard overrides.
-- Updated conditions on extensions flattening (over-flattening). (`#754 <https://github.com/tefra/xsdata/pull/754>`_)
-- Updated Group, AttributeGroup handling, skipping a few cases.
-- Updated how min/max occurs are calculated with nested containers.
-- Updated handling of element substitutions to treat them as choices. (`#786 <https://github.com/tefra/xsdata/pull/786>`_)
-- Updated Pycodeserializer to skip default field values.
-- Updated flattening restriction base classes when sequence elements are out of order.
-- Updated docformatter to v1.6.5.
-- Added support to override compound fields.
-- Added support for multiple sequential groups in a class.
-- Added support for non-list compound fields.
-- Added support to mix list and non-list fields with sequence groups.
-- Added an option to include headers in generated files. (`#746 <https://github.com/tefra/xsdata/pull/746>`_)
-- Added an option to cache the initial load and mapping of resources.
-- Added support for regular expressions in config substitutions. (`#755 <https://github.com/tefra/xsdata/pull/755>`_)
-- Added a pretty print indentation option in the serializer config. (`#780 <https://github.com/tefra/xsdata/pull/780>`_)
-- Added an option to set the encoding in the SOAP Client. (`#773 <https://github.com/tefra/xsdata/pull/773>`_)
-- Added a CLI flag to show debug messages.
-- Added a debug message for possible circular references during code generation.
-- Added support to generate prohibited fields when they restrict parent fields. (`#781 <https://github.com/tefra/xsdata/pull/781>`_)
-
-This release is bigger than intended and includes many major changes,
-that's why it took so long.
+- Fixed conflicting enum values leading to wrong default values (`#806 <https://github.com/tefra/xsdata/pull/806>`_)
+- Added support for custom decorators and base classes (`#793 <https://github.com/tefra/xsdata/pull/793>`_)
+- Added parser config to load external dtd to resolve entities (`#797 <https://github.com/tefra/xsdata/pull/797>`_)
+- Added requests sessions on the wsdl client transport (`#798 <https://github.com/tefra/xsdata/pull/798>`_)
+- Added support subscriptable types and UnionType (`#801 <https://github.com/tefra/xsdata/pull/801>`_)
+- Added option to restrict models package for auto-locator (`#809 <https://github.com/tefra/xsdata/pull/809>`_)
+- Updated context to only cache supported classes (`#796 <https://github.com/tefra/xsdata/pull/796>`_)
+- Removed tox requirement (`#800 <https://github.com/tefra/xsdata/pull/800>`_)
+- Converted to pyproject.toml (`#802 <https://github.com/tefra/xsdata/pull/802>`_)
```

### Comparing `xsdata-23.5/README.rst` & `xsdata-23.6/xsdata.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,43 @@
+Metadata-Version: 2.1
+Name: xsdata
+Version: 23.6
+Summary: Python XML Binding
+Author-email: Christodoulos Tsoulloftas <chris@komposta.net>
+License: MIT
+Project-URL: Homepage, https://github.com/tefra/xsdata
+Project-URL: Source, https://github.com/tefra/xsdata
+Project-URL: Documentation, https://xsdata.readthedocs.io/
+Project-URL: Changelog, https://xsdata.readthedocs.io/en/latest/changelog.html
+Keywords: xsd,wsdl,schema,dtd,binding,xml,json,dataclasses,generator,cli
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Text Processing :: Markup :: XML
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: cli
+Provides-Extra: docs
+Provides-Extra: lxml
+Provides-Extra: soap
+Provides-Extra: test
+License-File: LICENSE
+
 .. image:: https://github.com/tefra/xsdata/raw/master/docs/_static/logo.svg
     :target: https://xsdata.readthedocs.io/
 
 Naive XML Bindings for python
 =============================
 
 .. image:: https://github.com/tefra/xsdata/workflows/tests/badge.svg
@@ -95,43 +131,18 @@
   - Handlers and Writers based on lxml and native xml python
   - Support wildcard elements and attributes
   - Support xinclude statements and unknown properties
   - Customize behaviour through config
 
 
 
-Changelog: 23.5 (2023-05-21)
+Changelog: 23.6 (2023-06-24)
 ----------------------------
-- Fixed XML meta var index conflicts.
-- Fixed mixed content handling for DTD elements. (`#749 <https://github.com/tefra/xsdata/pull/749>`_, `#762 <https://github.com/tefra/xsdata/pull/762>`_)
-- Fixed an issue with required attributes turning into optional ones.
-- Fixed calculation of min/max occurs when parsing XML/JSON documents. (`#756 <https://github.com/tefra/xsdata/pull/756>`_)
-- Fixed calculation of min/max occurs when parsing DTD choice content types. (`#760 <https://github.com/tefra/xsdata/pull/760>`_)
-- Fixed an issue when parsing tail content for compound wildcard elements.
-- Fixed an issue with the code analyzer not fully processing some classes.
-- Fixed an issue with the code analyzer taking forever to process very large enumerations. (`#776 <https://github.com/tefra/xsdata/issue/776>`_)
-- Fixed an issue in the JSON parser with optional choice elements.
-- Updated the transformer to silently ignore malformed JSON files. (`#750 <https://github.com/tefra/xsdata/pull/750>`_)
-- Updated the override attribute handler to fix naming conflicts.
-- Updated the override attribute handler to allow wildcard overrides.
-- Updated conditions on extensions flattening (over-flattening). (`#754 <https://github.com/tefra/xsdata/pull/754>`_)
-- Updated Group, AttributeGroup handling, skipping a few cases.
-- Updated how min/max occurs are calculated with nested containers.
-- Updated handling of element substitutions to treat them as choices. (`#786 <https://github.com/tefra/xsdata/pull/786>`_)
-- Updated Pycodeserializer to skip default field values.
-- Updated flattening restriction base classes when sequence elements are out of order.
-- Updated docformatter to v1.6.5.
-- Added support to override compound fields.
-- Added support for multiple sequential groups in a class.
-- Added support for non-list compound fields.
-- Added support to mix list and non-list fields with sequence groups.
-- Added an option to include headers in generated files. (`#746 <https://github.com/tefra/xsdata/pull/746>`_)
-- Added an option to cache the initial load and mapping of resources.
-- Added support for regular expressions in config substitutions. (`#755 <https://github.com/tefra/xsdata/pull/755>`_)
-- Added a pretty print indentation option in the serializer config. (`#780 <https://github.com/tefra/xsdata/pull/780>`_)
-- Added an option to set the encoding in the SOAP Client. (`#773 <https://github.com/tefra/xsdata/pull/773>`_)
-- Added a CLI flag to show debug messages.
-- Added a debug message for possible circular references during code generation.
-- Added support to generate prohibited fields when they restrict parent fields. (`#781 <https://github.com/tefra/xsdata/pull/781>`_)
-
-This release is bigger than intended and includes many major changes,
-that's why it took so long.
+- Fixed conflicting enum values leading to wrong default values (`#806 <https://github.com/tefra/xsdata/pull/806>`_)
+- Added support for custom decorators and base classes (`#793 <https://github.com/tefra/xsdata/pull/793>`_)
+- Added parser config to load external dtd to resolve entities (`#797 <https://github.com/tefra/xsdata/pull/797>`_)
+- Added requests sessions on the wsdl client transport (`#798 <https://github.com/tefra/xsdata/pull/798>`_)
+- Added support subscriptable types and UnionType (`#801 <https://github.com/tefra/xsdata/pull/801>`_)
+- Added option to restrict models package for auto-locator (`#809 <https://github.com/tefra/xsdata/pull/809>`_)
+- Updated context to only cache supported classes (`#796 <https://github.com/tefra/xsdata/pull/796>`_)
+- Removed tox requirement (`#800 <https://github.com/tefra/xsdata/pull/800>`_)
+- Converted to pyproject.toml (`#802 <https://github.com/tefra/xsdata/pull/802>`_)
```

### Comparing `xsdata-23.5/docs/Makefile` & `xsdata-23.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/_ext/xsdatadocs.py` & `xsdata-23.6/docs/_ext/xsdatadocs.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/_static/logo-dark.svg` & `xsdata-23.6/docs/_static/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/_static/logo.svg` & `xsdata-23.6/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/api/codegen.rst` & `xsdata-23.6/docs/api/codegen.rst`

 * *Files 18% similar despite different names*

```diff
@@ -28,15 +28,18 @@
 
     GeneratorConfig
     GeneratorOutput
 
     OutputFormat
     GeneratorConventions
     GeneratorSubstitutions
+    GeneratorExtensions
     StructureStyle
     DocstringStyle
     ClassFilterStrategy
     CompoundFields
     ObjectType
+    ExtensionType
     GeneratorSubstitution
+    GeneratorExtension
     NameConvention
     NameCase
```

### Comparing `xsdata-23.5/docs/api/xml-handlers.rst` & `xsdata-23.6/docs/api/xml-handlers.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/api/xml-writers.rst` & `xsdata-23.6/docs/api/xml-writers.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/codegen.rst` & `xsdata-23.6/docs/codegen.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/conf.py` & `xsdata-23.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/data-types-table.rst` & `xsdata-23.6/docs/data-types-table.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/data-types.rst` & `xsdata-23.6/docs/data-types.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/examples/compound-fields.rst` & `xsdata-23.6/docs/examples/compound-fields.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/examples/custom-class-factory.rst` & `xsdata-23.6/docs/examples/custom-class-factory.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/examples/custom-property-names.rst` & `xsdata-23.6/docs/examples/custom-property-names.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/examples/custom-type-mapping.rst` & `xsdata-23.6/docs/examples/custom-type-mapping.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/examples/dataclasses-features.rst` & `xsdata-23.6/docs/examples/dataclasses-features.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/examples/docstrings.rst` & `xsdata-23.6/docs/examples/docstrings.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/examples/json-modeling.rst` & `xsdata-23.6/docs/examples/json-modeling.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/examples/pycode-serializer.rst` & `xsdata-23.6/docs/examples/pycode-serializer.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/examples/w3c-suite.rst` & `xsdata-23.6/docs/examples/w3c-suite.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/examples/working-with-wildcards.rst` & `xsdata-23.6/docs/examples/working-with-wildcards.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/examples/wrapped-list.rst` & `xsdata-23.6/docs/examples/wrapped-list.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/examples/xml-modeling.rst` & `xsdata-23.6/docs/examples/xml-modeling.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/examples.rst` & `xsdata-23.6/docs/examples.rst`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
     examples/docstrings
     examples/xml-modeling
     examples/json-modeling
     examples/dtd-modeling
     examples/compound-fields
     examples/dataclasses-features
+    examples/extending-models
 
 
 Data Binding
 ============
 
 .. toctree::
     :maxdepth: 1
```

### Comparing `xsdata-23.5/docs/faq/why-are-elements-out-of-order.rst` & `xsdata-23.6/docs/faq/why-are-elements-out-of-order.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/faq/why-i-get-a-typeerror-requires-a-single-type.rst` & `xsdata-23.6/docs/faq/why-i-get-a-typeerror-requires-a-single-type.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/faq/why-non-nullable-fields-are-marked-as-optional.rst` & `xsdata-23.6/docs/faq/why-non-nullable-fields-are-marked-as-optional.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/index.rst` & `xsdata-23.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/installation.rst` & `xsdata-23.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/json.rst` & `xsdata-23.6/docs/json.rst`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/make.bat` & `xsdata-23.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/models.rst` & `xsdata-23.6/docs/models.rst`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,30 @@
 
 .. warning::
 
     Currently only List, Tuple, Dict and Union annotations are supported.
     Everything else will raise an exception as unsupported.
 
 
+
+Support for generics in standard collections and the new union type was added
+in v23.6
+
+
+.. warning::
+
+    You will get false positive errors from mypy if you are using compound fields.
+
+    Mypy `issue <https://github.com/python/mypy/issues/13026>`_
+
+    .. code-block::
+
+        Value of type "Type[type]" is not indexable  [index]
+
+
 Field Metadata
 ==============
 
 Through the metadata properties you can control the field's behaviour during data
 binding procedures.
 
 .. list-table::
```

### Comparing `xsdata-23.5/docs/scripts/generate_data_types.py` & `xsdata-23.6/docs/scripts/generate_data_types.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/docs/wsdl.rst` & `xsdata-23.6/docs/wsdl.rst`

 * *Files 6% similar despite different names*

```diff
@@ -91,14 +91,24 @@
         soap_action="",
         input=None,
         output=None,
     )
     client = Client(config=config)
 
 
+Initialize a transport with a custom requests session instance.
+
+.. code-block::
+
+    from requests import Session
+
+    transport = DefaultTransport(session=Session())
+    client = Client(config=config, transport=transport)
+
+
 Performing Requests
 -------------------
 
 The send method requires either an object that matches the config input type or a
 dictionary with raw values that matches the input dataclass field names and structure.
 
 .. code-block::
```

### Comparing `xsdata-23.5/docs/xml.rst` & `xsdata-23.6/docs/xml.rst`

 * *Files 2% similar despite different names*

```diff
@@ -163,17 +163,19 @@
 
 .. doctest::
 
     >>> from xsdata.formats.dataclass.parsers.config import ParserConfig
     ...
     >>> config = ParserConfig(
     ...     base_url=None,
+    ...     load_dtd=False,
     ...     process_xinclude=False,
     ...     fail_on_unknown_properties=False,
     ...     fail_on_unknown_attributes=False,
+    ...     fail_on_converter_warnings=False,
     ... )
     >>> parser = XmlParser(config=config)
     >>> order = parser.from_bytes(xml_path.read_bytes())
     >>> order.bill_to.street
     '8 Oak Avenue'
 
 API :ref:`Reference <ParserConfig>`.
```

### Comparing `xsdata-23.5/tests/codegen/handlers/test_add_attribute_substitutions.py` & `xsdata-23.6/tests/codegen/handlers/test_add_attribute_substitutions.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/handlers/test_calculate_attribute_paths.py` & `xsdata-23.6/tests/codegen/handlers/test_calculate_attribute_paths.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/handlers/test_create_compound_fields.py` & `xsdata-23.6/tests/codegen/handlers/test_create_compound_fields.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/handlers/test_designate_class_packages.py` & `xsdata-23.6/tests/codegen/handlers/test_designate_class_packages.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/handlers/test_filter_classes.py` & `xsdata-23.6/tests/codegen/handlers/test_filter_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/handlers/test_flatten_attribute_groups.py` & `xsdata-23.6/tests/codegen/handlers/test_flatten_attribute_groups.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/handlers/test_flatten_class_extensions.py` & `xsdata-23.6/tests/codegen/handlers/test_flatten_class_extensions.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/handlers/test_merge_attributes.py` & `xsdata-23.6/tests/codegen/handlers/test_merge_attributes.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/handlers/test_process_attributes_types.py` & `xsdata-23.6/tests/codegen/handlers/test_process_attributes_types.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/handlers/test_process_mixed_content_class.py` & `xsdata-23.6/tests/codegen/handlers/test_process_mixed_content_class.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/handlers/test_rename_duplicate_attributes.py` & `xsdata-23.6/tests/codegen/handlers/test_rename_duplicate_attributes.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/handlers/test_rename_duplicate_classes.py` & `xsdata-23.6/tests/codegen/handlers/test_rename_duplicate_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/handlers/test_reset_attribute_sequence_numbers.py` & `xsdata-23.6/tests/codegen/handlers/test_reset_attribute_sequence_numbers.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/handlers/test_reset_attribute_sequences.py` & `xsdata-23.6/tests/codegen/handlers/test_reset_attribute_sequences.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/handlers/test_sanitize_attributes_default_value.py` & `xsdata-23.6/tests/codegen/handlers/test_sanitize_attributes_default_value.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/handlers/test_sanitize_enumeration_class.py` & `xsdata-23.6/tests/codegen/handlers/test_sanitize_enumeration_class.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/handlers/test_unnest_inner_classes.py` & `xsdata-23.6/tests/codegen/handlers/test_unnest_inner_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/handlers/test_update_attributes_effective_choice.py` & `xsdata-23.6/tests/codegen/handlers/test_update_attributes_effective_choice.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/handlers/test_vacuum_inner_classes.py` & `xsdata-23.6/tests/codegen/handlers/test_vacuum_inner_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/handlers/test_validate_attributes_overrides.py` & `xsdata-23.6/tests/codegen/handlers/test_validate_attributes_overrides.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/mappers/test_definitions.py` & `xsdata-23.6/tests/codegen/mappers/test_definitions.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/mappers/test_dict.py` & `xsdata-23.6/tests/codegen/mappers/test_dict.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/mappers/test_dtd.py` & `xsdata-23.6/tests/codegen/mappers/test_dtd.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/mappers/test_element.py` & `xsdata-23.6/tests/codegen/mappers/test_element.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/mappers/test_schema.py` & `xsdata-23.6/tests/codegen/mappers/test_schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/models/test_attr.py` & `xsdata-23.6/tests/codegen/models/test_attr.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/models/test_attr_type.py` & `xsdata-23.6/tests/codegen/models/test_attr_type.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/models/test_class.py` & `xsdata-23.6/tests/codegen/models/test_class.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/models/test_restrictions.py` & `xsdata-23.6/tests/codegen/models/test_restrictions.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/parsers/test_definitions.py` & `xsdata-23.6/tests/codegen/parsers/test_definitions.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/parsers/test_dtd.py` & `xsdata-23.6/tests/codegen/parsers/test_dtd.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/parsers/test_schema.py` & `xsdata-23.6/tests/codegen/parsers/test_schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/test_analyzer.py` & `xsdata-23.6/tests/codegen/test_analyzer.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/test_container.py` & `xsdata-23.6/tests/codegen/test_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,20 @@
                 "UpdateAttributesEffectiveChoice",
                 "UnnestInnerClasses",
                 "AddAttributeSubstitutions",
                 "ProcessAttributeTypes",
                 "MergeAttributes",
                 "ProcessMixedContentClass",
             ],
-            30: ["ResetAttributeSequences", "SanitizeAttributesDefaultValue"],
-            40: ["ValidateAttributesOverrides", "RenameDuplicateAttributes"],
+            30: [
+                "ResetAttributeSequences",
+                "RenameDuplicateAttributes",
+                "SanitizeAttributesDefaultValue",
+            ],
+            40: ["ValidateAttributesOverrides"],
             50: [
                 "VacuumInnerClasses",
                 "CreateCompoundFields",
                 "ResetAttributeSequenceNumbers",
             ],
         }
```

### Comparing `xsdata-23.5/tests/codegen/test_resolver.py` & `xsdata-23.6/tests/codegen/test_resolver.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/test_transformer.py` & `xsdata-23.6/tests/codegen/test_transformer.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/test_utils.py` & `xsdata-23.6/tests/codegen/test_utils.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/test_validator.py` & `xsdata-23.6/tests/codegen/test_validator.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/codegen/test_writer.py` & `xsdata-23.6/tests/codegen/test_writer.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/conftest.py` & `xsdata-23.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/annotations/model.py` & `xsdata-23.6/tests/fixtures/annotations/model.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/annotations/model.xsd` & `xsdata-23.6/tests/fixtures/annotations/model.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/annotations/units.xsd` & `xsdata-23.6/tests/fixtures/annotations/units.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/annotations/xsdata.xml` & `xsdata-23.6/tests/fixtures/annotations/xsdata.xml`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/artists/art001.xml` & `xsdata-23.6/tests/fixtures/artists/art001.xml`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/artists/art002.xml` & `xsdata-23.6/tests/fixtures/artists/art002.xml`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/artists/art003.xml` & `xsdata-23.6/tests/fixtures/artists/art003.xml`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/artists/metadata.py` & `xsdata-23.6/tests/fixtures/artists/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,18 @@
         default=None,
         metadata={
             "name": "sort-name",
             "type": "Attribute",
             "required": True,
         }
     )
-    type: Optional[str] = field(
+    type_value: Optional[str] = field(
         default=None,
         metadata={
+            "name": "type",
             "type": "Attribute",
         }
     )
     type_id: Optional[str] = field(
         default=None,
         metadata={
             "name": "type-id",
@@ -299,17 +300,18 @@
     id: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "required": True,
         }
     )
-    type: Optional[str] = field(
+    type_value: Optional[str] = field(
         default=None,
         metadata={
+            "name": "type",
             "type": "Attribute",
             "required": True,
         }
     )
     type_id: Optional[str] = field(
         default=None,
         metadata={
```

### Comparing `xsdata-23.5/tests/fixtures/books/books.py` & `xsdata-23.6/tests/fixtures/books/books.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/books/books.xml` & `xsdata-23.6/tests/fixtures/books/books.xml`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/books/books_auto_ns.xml` & `xsdata-23.6/tests/fixtures/books/books_auto_ns.xml`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/books/books_default_ns.xml` & `xsdata-23.6/tests/fixtures/books/books_default_ns.xml`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/books/fixtures.py` & `xsdata-23.6/tests/fixtures/books/fixtures.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/books/schema.xsd` & `xsdata-23.6/tests/fixtures/books/schema.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/calculator/__init__.py` & `xsdata-23.6/tests/fixtures/calculator/__init__.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/calculator/services.py` & `xsdata-23.6/tests/fixtures/calculator/services.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/calculator/services.wsdl` & `xsdata-23.6/tests/fixtures/calculator/services.wsdl`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/compound/models.py` & `xsdata-23.6/tests/fixtures/compound/models.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/compound/schema.xsd` & `xsdata-23.6/tests/fixtures/compound/schema.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/datatypes.py` & `xsdata-23.6/tests/fixtures/datatypes.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/docstrings/accessible/schema.py` & `xsdata-23.6/tests/fixtures/docstrings/accessible/schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/docstrings/blank/schema.py` & `xsdata-23.6/tests/fixtures/docstrings/blank/schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/docstrings/google/schema.py` & `xsdata-23.6/tests/fixtures/docstrings/google/schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/docstrings/numpy/schema.py` & `xsdata-23.6/tests/fixtures/docstrings/numpy/schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/docstrings/rst/schema.py` & `xsdata-23.6/tests/fixtures/docstrings/rst/schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/docstrings/schema.xsd` & `xsdata-23.6/tests/fixtures/docstrings/schema.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/dtd/models/complete_example.py` & `xsdata-23.6/tests/fixtures/dtd/models/complete_example.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/hello/hello.py` & `xsdata-23.6/tests/fixtures/hello/hello.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/hello/hello.wsdl` & `xsdata-23.6/tests/fixtures/hello/hello.wsdl`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/hello/hello.xsd` & `xsdata-23.6/tests/fixtures/hello/hello.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/models.py` & `xsdata-23.6/tests/fixtures/models.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/primer/order.py` & `xsdata-23.6/tests/fixtures/primer/order.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/primer/order.xsd` & `xsdata-23.6/tests/fixtures/primer/order.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/primer/sample.json` & `xsdata-23.6/tests/fixtures/primer/sample.json`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/primer/sample.xml` & `xsdata-23.6/tests/fixtures/primer/sample.xml`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/primer/sample.xsdata.xml` & `xsdata-23.6/tests/fixtures/primer/sample.xsdata.xml`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/series/samples/show1.json` & `xsdata-23.6/tests/fixtures/series/samples/show1.json`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/series/samples/show2.json` & `xsdata-23.6/tests/fixtures/series/samples/show2.json`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/series/series.py` & `xsdata-23.6/tests/fixtures/series/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,17 +211,18 @@
     name: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
             "required": True,
         }
     )
-    type: Optional[str] = field(
+    type_value: Optional[str] = field(
         default=None,
         metadata={
+            "name": "type",
             "type": "Element",
             "required": True,
         }
     )
     language: Optional[str] = field(
         default=None,
         metadata={
```

### Comparing `xsdata-23.5/tests/fixtures/stripe/.xsdata.xml` & `xsdata-23.6/tests/fixtures/stripe/.xsdata.xml`

 * *Files 14% similar despite different names*

#### Comparing `xsdata-23.5/tests/fixtures/stripe/.xsdata.xml` & `xsdata-23.6/tests/fixtures/stripe/.xsdata.xml`

```diff
@@ -13,8 +13,9 @@
     <FieldName case="snakeCase" safePrefix="value"/>
     <ConstantName case="screamingSnakeCase" safePrefix="value"/>
     <ModuleName case="snakeCase" safePrefix="mod"/>
     <PackageName case="snakeCase" safePrefix="pkg"/>
   </Conventions>
   <Aliases/>
   <Substitutions/>
+  <Extensions/>
 </Config>
```

### Comparing `xsdata-23.5/tests/fixtures/stripe/models/balance.py` & `xsdata-23.6/tests/fixtures/stripe/models/balance.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/fixtures/stripe/samples/balance.json` & `xsdata-23.6/tests/fixtures/stripe/samples/balance.json`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/models/test_builders.py` & `xsdata-23.6/tests/formats/dataclass/models/test_builders.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/parsers/handlers/test_lxml.py` & `xsdata-23.6/tests/formats/dataclass/parsers/handlers/test_lxml.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/parsers/handlers/test_native.py` & `xsdata-23.6/tests/formats/dataclass/parsers/handlers/test_native.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_element.py` & `xsdata-23.6/tests/formats/dataclass/parsers/nodes/test_element.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_primitive.py` & `xsdata-23.6/tests/formats/dataclass/parsers/nodes/test_primitive.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_standard.py` & `xsdata-23.6/tests/formats/dataclass/parsers/nodes/test_standard.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_union.py` & `xsdata-23.6/tests/formats/dataclass/parsers/nodes/test_union.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_wildcard.py` & `xsdata-23.6/tests/formats/dataclass/parsers/nodes/test_wildcard.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_wrapper.py` & `xsdata-23.6/tests/formats/dataclass/parsers/nodes/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/parsers/test_json.py` & `xsdata-23.6/tests/formats/dataclass/parsers/test_json.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/parsers/test_mixins.py` & `xsdata-23.6/tests/formats/dataclass/parsers/test_mixins.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/parsers/test_node.py` & `xsdata-23.6/tests/formats/dataclass/parsers/test_node.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/parsers/test_tree.py` & `xsdata-23.6/tests/formats/dataclass/parsers/test_tree.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/parsers/test_utils.py` & `xsdata-23.6/tests/formats/dataclass/parsers/test_utils.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/parsers/test_xml.py` & `xsdata-23.6/tests/formats/dataclass/parsers/test_xml.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/serializers/test_code.py` & `xsdata-23.6/tests/formats/dataclass/serializers/test_code.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/serializers/test_json.py` & `xsdata-23.6/tests/formats/dataclass/serializers/test_json.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/serializers/test_mixins.py` & `xsdata-23.6/tests/formats/dataclass/serializers/test_mixins.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/serializers/test_xml.py` & `xsdata-23.6/tests/formats/dataclass/serializers/test_xml.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/serializers/writers/test_lxml.py` & `xsdata-23.6/tests/formats/dataclass/serializers/writers/test_lxml.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/serializers/writers/test_native.py` & `xsdata-23.6/tests/formats/dataclass/serializers/writers/test_native.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/test_client.py` & `xsdata-23.6/tests/formats/dataclass/test_client.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/test_compat.py` & `xsdata-23.6/tests/formats/dataclass/test_compat.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/test_context.py` & `xsdata-23.6/tests/formats/dataclass/test_context.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 from dataclasses import make_dataclass
+from pathlib import Path
 from unittest import mock
 
 from tests.fixtures.artists import Artist
 from tests.fixtures.artists import BeginArea
 from tests.fixtures.books import BookForm
 from tests.fixtures.books import BooksForm
 from tests.fixtures.models import BaseType
@@ -74,27 +75,50 @@
     def test_find_type_by_fields(self):
         field_names = {"id", "name", "sort-name"}
         self.assertEqual(BeginArea, self.ctx.find_type_by_fields(field_names))
 
         field_names.update({"please", "dont", "exist"})  # Test matching with more
         self.assertIsNone(self.ctx.find_type_by_fields(field_names))
 
+    def test_local_names_match_remove_clazz_from_cache_on_error(self):
+        undefined = make_dataclass("UndefinedType", [("content", "Literal['yes']")])
+        unsupported = make_dataclass("UndefinedType", [("content", Path)])
+        uncached = make_dataclass("Uncached", [("content", Path)])
+
+        builder = self.ctx.get_builder()
+        for clazz in (undefined, unsupported):
+            meta = builder.build_class_meta(clazz)
+            self.ctx.xsi_cache[meta.target_qname].append(clazz)
+
+        self.assertFalse(self.ctx.local_names_match({"content"}, undefined))
+        self.assertFalse(self.ctx.local_names_match({"content"}, unsupported))
+        self.assertFalse(self.ctx.local_names_match({"content"}, uncached))
+
+        total = [x for types in self.ctx.cache.values() for x in types]
+        self.assertEqual(0, len(total))
+
     def test_find_subclass(self):
         a = make_dataclass("A", fields=[])
         b = make_dataclass("B", fields=[], bases=(a,))
         c = make_dataclass("C", fields=[], bases=(a,))
         other = make_dataclass("Other", fields=[])  # Included in the locals
 
         self.assertEqual(b, self.ctx.find_subclass(a, "B"))
         self.assertEqual(b, self.ctx.find_subclass(c, "B"))
         self.assertIsNone(self.ctx.find_subclass(b, "A"))
         self.assertIsNone(self.ctx.find_subclass(c, "A"))
         self.assertIsNone(self.ctx.find_subclass(c, "Unknown"))
         self.assertIsNone(self.ctx.find_subclass(c, "Other"))
 
+    def is_binding_model(self):
+        self.assertTrue(self.ctx.is_binding_model(ChoiceType))
+
+        self.ctx.models_package = "xsdata.models"
+        self.assertFalse(self.ctx.is_binding_model(ChoiceType))
+
     def test_is_derived(self):
         a = make_dataclass("A", fields=[])
         b = make_dataclass("B", fields=[], bases=(a,))
         c = make_dataclass("C", fields=[], bases=(a,))
         d = make_dataclass("D", fields=[])
 
         self.assertTrue(self.ctx.is_derived(c(), b))
```

### Comparing `xsdata-23.5/tests/formats/dataclass/test_elements.py` & `xsdata-23.6/tests/formats/dataclass/test_elements.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/test_filters.py` & `xsdata-23.6/tests/formats/dataclass/test_filters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from collections import namedtuple
 from unittest import mock
 
 from tests.fixtures.datatypes import Telephone
 from xsdata.codegen.models import Restrictions
 from xsdata.formats.dataclass.filters import Filters
 from xsdata.models.config import DocstringStyle
+from xsdata.models.config import ExtensionType
 from xsdata.models.config import GeneratorConfig
+from xsdata.models.config import GeneratorExtension
 from xsdata.models.config import GeneratorSubstitution
 from xsdata.models.config import NameCase
 from xsdata.models.config import ObjectType
 from xsdata.models.enums import DataType
 from xsdata.models.enums import Namespace
 from xsdata.models.enums import Tag
 from xsdata.utils.testing import AttrFactory
 from xsdata.utils.testing import AttrTypeFactory
+from xsdata.utils.testing import ClassFactory
+from xsdata.utils.testing import ExtensionFactory
 from xsdata.utils.testing import FactoryTestCase
 
 type_str = AttrTypeFactory.native(DataType.STRING)
 type_int = AttrTypeFactory.native(DataType.INT)
 type_float = AttrTypeFactory.native(DataType.FLOAT)
 type_decimal = AttrTypeFactory.native(DataType.DECIMAL)
 type_bool = AttrTypeFactory.native(DataType.BOOLEAN)
@@ -38,14 +42,110 @@
 
         self.assertEqual("XsString", self.filters.class_name("xs:string"))
         self.assertEqual("FooBarBam", self.filters.class_name("foo:bar_bam"))
         self.assertEqual("ListType", self.filters.class_name("List"))
         self.assertEqual("TypeType", self.filters.class_name(".*"))
         self.assertEqual("Cbad", self.filters.class_name("abcd"))
 
+    def test_class_bases(self):
+        etp = ExtensionType.CLASS
+        self.filters.extensions[etp] = [
+            GeneratorExtension(
+                type=etp,
+                class_name=".*Bar",
+                import_string="a.b",
+                apply_if_derived=True,
+                prepend=False,
+            ),
+            GeneratorExtension(
+                type=etp,
+                class_name="Foo.*",
+                import_string="a.b",
+                apply_if_derived=True,
+                prepend=True,
+            ),
+            GeneratorExtension(
+                type=etp,
+                class_name="Foo.*",
+                import_string="a.c",
+                apply_if_derived=True,
+                prepend=True,
+            ),
+            GeneratorExtension(
+                type=etp,
+                class_name="Foo.*",
+                import_string="a.d",
+                apply_if_derived=False,
+                prepend=True,
+            ),
+            GeneratorExtension(
+                type=etp,
+                class_name="Nope.*",
+                import_string="a.e",
+                apply_if_derived=True,
+                prepend=False,
+            ),
+        ]
+        target = ClassFactory.create(extensions=ExtensionFactory.list(1))
+
+        expected = self.filters.class_bases(target, "FooBar")
+        self.assertEqual(["c", "b", "AttrB"], expected)
+
+        target.extensions.clear()
+        expected = self.filters.class_bases(target, "FooBar")
+        self.assertEqual(["d", "c", "b"], expected)
+
+    def test_class_annotations(self):
+        etp = ExtensionType.DECORATOR
+        self.filters.extensions[etp] = [
+            GeneratorExtension(
+                type=etp,
+                class_name=".*Bar",
+                import_string="a.b",
+                apply_if_derived=True,
+                prepend=False,
+            ),
+            GeneratorExtension(
+                type=etp,
+                class_name="Foo.*",
+                import_string="a.b",
+                apply_if_derived=True,
+                prepend=True,
+            ),
+            GeneratorExtension(
+                type=etp,
+                class_name="Foo.*",
+                import_string="a.c",
+                apply_if_derived=True,
+                prepend=True,
+            ),
+            GeneratorExtension(
+                type=etp,
+                class_name="Foo.*",
+                import_string="a.d",
+                apply_if_derived=False,
+                prepend=False,
+            ),
+            GeneratorExtension(
+                type=etp,
+                class_name="Nope.*",
+                import_string="a.e",
+                apply_if_derived=True,
+                prepend=False,
+            ),
+        ]
+        target = ClassFactory.create(extensions=ExtensionFactory.list(1))
+
+        expected = self.filters.class_annotations(target, "FooBar")
+        self.assertEqual(["@c", "@b", "@dataclass"], expected)
+
+        target.extensions.clear()
+        expected = self.filters.class_annotations(target, "FooBar")
+        self.assertEqual(["@c", "@b", "@dataclass", "@d"], expected)
+
     def test_field_name(self):
         self.filters.substitutions[ObjectType.FIELD]["abc"] = "cba"
 
         self.assertEqual("value", self.filters.field_name("", "cls"))
         self.assertEqual("foo", self.filters.field_name("foo", "cls"))
         self.assertEqual("foo_bar", self.filters.field_name("foo:bar", "cls"))
         self.assertEqual("foo_bar", self.filters.field_name("FooBar", "cls"))
@@ -436,25 +536,31 @@
         )
 
         self.assertEqual("FooBar", self.filters.field_type(attr, []))
 
         attr.restrictions.nillable = True
         self.assertEqual("Optional[FooBar]", self.filters.field_type(attr, []))
 
+        self.filters.union_type = True
+        self.assertEqual("None | FooBar", self.filters.field_type(attr, []))
+
     def test_field_type_with_optional_value(self):
         attr = AttrFactory.create(types=AttrTypeFactory.list(1, qname="foo_bar"))
 
         self.assertEqual("Optional[FooBar]", self.filters.field_type(attr, []))
 
         self.filters.format.kw_only = True
         self.assertEqual("FooBar", self.filters.field_type(attr, []))
 
         attr.restrictions.min_occurs = 0
         self.assertEqual("Optional[FooBar]", self.filters.field_type(attr, []))
 
+        self.filters.union_type = True
+        self.assertEqual("None | FooBar", self.filters.field_type(attr, []))
+
     def test_field_type_with_circular_reference(self):
         attr = AttrFactory.create(
             types=AttrTypeFactory.list(1, qname="foo_bar", circular=True)
         )
 
         self.assertEqual(
             'Optional["FooBar"]', self.filters.field_type(attr, ["Parent"])
@@ -465,14 +571,21 @@
             types=AttrTypeFactory.list(1, qname="foo_bar", forward=True)
         )
         self.assertEqual(
             'Optional["Parent.Inner.FooBar"]',
             self.filters.field_type(attr, ["Parent", "Inner"]),
         )
 
+        self.filters.postponed_annotations = True
+        self.filters.union_type = True
+        self.assertEqual(
+            "None | Parent.Inner.FooBar",
+            self.filters.field_type(attr, ["Parent", "Inner"]),
+        )
+
     def test_field_type_with_forward_and_circular_reference(self):
         attr = AttrFactory.create(
             types=AttrTypeFactory.list(1, qname="foo_bar", forward=True, circular=True)
         )
 
         self.assertEqual(
             'Optional["Parent.Inner"]',
@@ -491,14 +604,26 @@
 
         self.filters.format.frozen = True
         self.assertEqual(
             'Tuple["A.Parent.FooBar", ...]',
             self.filters.field_type(attr, ["A", "Parent"]),
         )
 
+        self.filters.subscriptable_types = True
+        self.assertEqual(
+            'tuple["A.Parent.FooBar", ...]',
+            self.filters.field_type(attr, ["A", "Parent"]),
+        )
+
+        self.filters.format.frozen = False
+        self.assertEqual(
+            'list["A.Parent.FooBar"]',
+            self.filters.field_type(attr, ["A", "Parent"]),
+        )
+
     def test_field_type_with_token_attr(self):
         attr = AttrFactory.create(
             types=AttrTypeFactory.list(1, qname="foo_bar"),
             restrictions=Restrictions(tokens=True),
         )
         self.assertEqual("List[FooBar]", self.filters.field_type(attr, []))
 
@@ -510,14 +635,19 @@
         self.assertEqual("Tuple[FooBar, ...]", self.filters.field_type(attr, []))
 
         attr.restrictions.max_occurs = 2
         self.assertEqual(
             "Tuple[Tuple[FooBar, ...], ...]", self.filters.field_type(attr, [])
         )
 
+        self.filters.subscriptable_types = True
+        self.assertEqual(
+            "tuple[tuple[FooBar, ...], ...]", self.filters.field_type(attr, [])
+        )
+
     def test_field_type_with_alias(self):
         attr = AttrFactory.create(
             types=AttrTypeFactory.list(
                 1, qname="foo_bar", forward=True, alias="Boss:Life"
             )
         )
         attr.restrictions.max_occurs = 2
@@ -536,57 +666,93 @@
         attr.restrictions.max_occurs = 2
 
         self.assertEqual(
             'List[Union["A.Parent.BossLife", int]]',
             self.filters.field_type(attr, ["A", "Parent"]),
         )
 
+        self.filters.union_type = True
+        self.assertEqual(
+            'List["A.Parent.BossLife" | int]',
+            self.filters.field_type(attr, ["A", "Parent"]),
+        )
+        self.filters.subscriptable_types = True
+        self.assertEqual(
+            'list["A.Parent.BossLife" | int]',
+            self.filters.field_type(attr, ["A", "Parent"]),
+        )
+
     def test_field_type_with_any_attribute(self):
         attr = AttrFactory.any_attribute()
 
         self.assertEqual("Dict[str, str]", self.filters.field_type(attr, ["a", "b"]))
 
+        self.filters.subscriptable_types = True
+        self.assertEqual("dict[str, str]", self.filters.field_type(attr, ["a", "b"]))
+
     def test_field_type_with_native_type(self):
         attr = AttrFactory.create(
             types=[
                 AttrTypeFactory.native(DataType.INT),
                 AttrTypeFactory.native(DataType.POSITIVE_INTEGER),
+                AttrTypeFactory.native(DataType.STRING),
             ]
         )
-        self.assertEqual("Optional[int]", self.filters.field_type(attr, ["a", "b"]))
+        self.assertEqual(
+            "Optional[Union[int, str]]", self.filters.field_type(attr, ["a", "b"])
+        )
+
+        self.filters.union_type = True
+        self.assertEqual("None | int | str", self.filters.field_type(attr, ["a", "b"]))
 
     def test_field_type_with_prohibited_attr(self):
         attr = AttrFactory.create(restrictions=Restrictions(max_occurs=0))
 
         self.assertEqual("Any", self.filters.field_type(attr, ["a", "b"]))
 
     def test_choice_type(self):
         choice = AttrFactory.create(types=[AttrTypeFactory.create("foobar")])
         actual = self.filters.choice_type(choice, ["a", "b"])
         self.assertEqual("Type[Foobar]", actual)
 
+        self.filters.subscriptable_types = True
+        actual = self.filters.choice_type(choice, ["a", "b"])
+        self.assertEqual("type[Foobar]", actual)
+
     def test_choice_type_with_forward_reference(self):
         choice = AttrFactory.create(
             types=[AttrTypeFactory.create("foobar", forward=True)]
         )
         actual = self.filters.choice_type(choice, ["a", "b"])
         self.assertEqual('Type["A.B.Foobar"]', actual)
 
     def test_choice_type_with_circular_reference(self):
         choice = AttrFactory.create(
             types=[AttrTypeFactory.create("foobar", circular=True)]
         )
         actual = self.filters.choice_type(choice, ["a", "b"])
         self.assertEqual('Type["Foobar"]', actual)
 
+        self.filters.postponed_annotations = True
+        actual = self.filters.choice_type(choice, ["a", "b"])
+        self.assertEqual("Type[Foobar]", actual)
+
     def test_choice_type_with_multiple_types(self):
         choice = AttrFactory.create(types=[type_str, type_bool])
         actual = self.filters.choice_type(choice, ["a", "b"])
         self.assertEqual("Type[Union[str, bool]]", actual)
 
+        self.filters.subscriptable_types = True
+        actual = self.filters.choice_type(choice, ["a", "b"])
+        self.assertEqual("type[Union[str, bool]]", actual)
+
+        self.filters.union_type = True
+        actual = self.filters.choice_type(choice, ["a", "b"])
+        self.assertEqual("type[str | bool]", actual)
+
     def test_choice_type_with_list_types_are_ignored(self):
         choice = AttrFactory.create(types=[type_str, type_bool])
         choice.restrictions.max_occurs = 200
         actual = self.filters.choice_type(choice, ["a", "b"])
         self.assertEqual("Type[Union[str, bool]]", actual)
 
     def test_choice_type_with_restrictions_tokens_true(self):
@@ -595,14 +761,19 @@
         actual = self.filters.choice_type(choice, ["a", "b"])
         self.assertEqual("Type[List[Union[str, bool]]]", actual)
 
         self.filters.format.frozen = True
         actual = self.filters.choice_type(choice, ["a", "b"])
         self.assertEqual("Type[Tuple[Union[str, bool], ...]]", actual)
 
+        self.filters.union_type = True
+        self.filters.subscriptable_types = True
+        actual = self.filters.choice_type(choice, ["a", "b"])
+        self.assertEqual("type[tuple[str | bool, ...]]", actual)
+
     def test_default_imports_with_decimal(self):
         expected = "from decimal import Decimal"
 
         self.assertIn(expected, self.filters.default_imports("Optional[Decimal]"))
         self.assertIn(expected, self.filters.default_imports("Union[str, Decimal]"))
         self.assertIn(expected, self.filters.default_imports("Union[Decimal, "))
         self.assertIn(expected, self.filters.default_imports("Union[str, Decimal, int"))
@@ -813,14 +984,22 @@
         config.conventions.module_name.case = NameCase.SNAKE
         config.substitutions.substitution.append(
             GeneratorSubstitution(ObjectType.FIELD, "k", "l")
         )
         config.substitutions.substitution.append(
             GeneratorSubstitution(ObjectType.PACKAGE, "m", "n")
         )
+        config.extensions.extension.extend(
+            [
+                GeneratorExtension(ExtensionType.DECORATOR, "a", "a.b"),
+                GeneratorExtension(ExtensionType.DECORATOR, "b", "a.c"),
+                GeneratorExtension(ExtensionType.CLASS, "c", "a.d"),
+                GeneratorExtension(ExtensionType.CLASS, "d", "a.e"),
+            ]
+        )
 
         filters = Filters(config)
 
         self.assertFalse(filters.relative_imports)
 
         self.assertEqual("safe_class", filters.class_safe_prefix)
         self.assertEqual("safe_field", filters.field_safe_prefix)
@@ -835,7 +1014,21 @@
         expected_substitutions = {
             ObjectType.CLASS: {},
             ObjectType.FIELD: {"k": "l"},
             ObjectType.MODULE: {},
             ObjectType.PACKAGE: {"m": "n"},
         }
         self.assertEqual(expected_substitutions, filters.substitutions)
+
+        expected_extensions = {
+            ExtensionType.DECORATOR: config.extensions.extension[0:2],
+            ExtensionType.CLASS: config.extensions.extension[2:4],
+        }
+        self.assertEqual(expected_extensions, filters.extensions)
+
+        expected_imports = {
+            "b": {"@b"},
+            "c": {"@c"},
+            "d": {"(d", " d)"},
+            "e": {"(e", " e)"},
+        }
+        self.assertEqual(expected_imports, filters.import_patterns["a"])
```

### Comparing `xsdata-23.5/tests/formats/dataclass/test_generator.py` & `xsdata-23.6/tests/formats/dataclass/test_generator.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/dataclass/test_transport.py` & `xsdata-23.6/tests/formats/dataclass/test_transport.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from unittest import mock
 from unittest import TestCase
 
 from requests import HTTPError
 from requests import Response
+from requests import Session
 
 from xsdata.formats.dataclass.transports import DefaultTransport
 
 
 class DefaultTransportTest(TestCase):
     @mock.patch.object(Response, "content", new_callable=mock.PropertyMock)
     @mock.patch.object(Response, "raise_for_status")
-    @mock.patch("xsdata.formats.dataclass.transports.requests.get")
+    @mock.patch.object(Session, "get")
     def test_get(self, mock_get, mock_raise_for_status, mock_content):
         transport = DefaultTransport()
         params = {"a": "b"}
         url = "http://endpoint.stub/action"
         headers = {"content-type": "text/xml"}
 
         response = Response()
@@ -27,15 +28,15 @@
         self.assertEqual(0, mock_raise_for_status.call_count)
         mock_get.assert_called_once_with(
             url, params=params, headers=headers, timeout=transport.timeout
         )
 
     @mock.patch.object(Response, "content", new_callable=mock.PropertyMock)
     @mock.patch.object(Response, "raise_for_status")
-    @mock.patch("xsdata.formats.dataclass.transports.requests.post")
+    @mock.patch.object(Session, "post")
     def test_post(self, mock_post, mock_raise_for_status, mock_content):
         transport = DefaultTransport(timeout=1.0)
         data = {"a": "b"}
         url = "http://endpoint.stub/action"
         headers = {"content-type": "text/xml"}
 
         response = Response()
```

### Comparing `xsdata-23.5/tests/formats/test_converter.py` & `xsdata-23.6/tests/formats/test_converter.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/formats/test_mixins.py` & `xsdata-23.6/tests/formats/test_mixins.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/integration/benchmarks/test_converters.py` & `xsdata-23.6/tests/integration/benchmarks/test_converters.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/integration/benchmarks/test_handlers.py` & `xsdata-23.6/tests/integration/benchmarks/test_handlers.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/integration/benchmarks/utils.py` & `xsdata-23.6/tests/integration/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/integration/test_annotations.py` & `xsdata-23.6/tests/integration/test_annotations.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/integration/test_artists.py` & `xsdata-23.6/tests/integration/test_artists.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/integration/test_books.py` & `xsdata-23.6/tests/integration/test_books.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/integration/test_calculator.py` & `xsdata-23.6/tests/integration/test_calculator.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/integration/test_compound.py` & `xsdata-23.6/tests/integration/test_compound.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/integration/test_docstrings.py` & `xsdata-23.6/tests/integration/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/integration/test_dtd.py` & `xsdata-23.6/tests/integration/test_dtd.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/integration/test_hello_rpc.py` & `xsdata-23.6/tests/integration/test_hello_rpc.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/integration/test_primer.py` & `xsdata-23.6/tests/integration/test_primer.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/integration/test_series.py` & `xsdata-23.6/tests/integration/test_series.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/integration/test_stripe.py` & `xsdata-23.6/tests/integration/test_stripe.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/models/enums/test_datatype.py` & `xsdata-23.6/tests/models/enums/test_datatype.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/models/test_config.py` & `xsdata-23.6/tests/models/test_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 import warnings
 from pathlib import Path
 from unittest import TestCase
 
 from xsdata import __version__
 from xsdata.exceptions import GeneratorConfigError
 from xsdata.exceptions import ParserError
+from xsdata.models.config import ExtensionType
 from xsdata.models.config import GeneratorAlias
 from xsdata.models.config import GeneratorAliases
 from xsdata.models.config import GeneratorConfig
+from xsdata.models.config import GeneratorExtension
 from xsdata.models.config import GeneratorOutput
 from xsdata.models.config import ObjectType
 from xsdata.models.config import OutputFormat
 
 
 class GeneratorConfigTests(TestCase):
     def setUp(self) -> None:
@@ -24,15 +26,15 @@
         obj = GeneratorConfig.create()
         with file_path.open("w") as fp:
             obj.write(fp, obj)
 
         expected = (
             '<?xml version="1.0" encoding="UTF-8"?>\n'
             f'<Config xmlns="http://pypi.org/project/xsdata" version="{__version__}">\n'
-            '  <Output maxLineLength="79">\n'
+            '  <Output maxLineLength="79" subscriptableTypes="false" unionType="false">\n'
             "    <Package>generated</Package>\n"
             '    <Format repr="true" eq="true" order="false" unsafeHash="false" frozen="false" slots="false" kwOnly="false">dataclasses</Format>\n'
             "    <Structure>filenames</Structure>\n"
             "    <DocstringStyle>reStructuredText</DocstringStyle>\n"
             "    <FilterStrategy>allGlobals</FilterStrategy>\n"
             "    <RelativeImports>false</RelativeImports>\n"
             '    <CompoundFields defaultName="choice" forceDefaultName="false">false</CompoundFields>\n'
@@ -56,24 +58,25 @@
             '    <Substitution type="package" search="http://www.w3.org/1999/xlink" replace="xlink"/>\n'
             '    <Substitution type="package" search="http://www.w3.org/1999/xhtml" replace="xhtml"/>\n'
             '    <Substitution type="package" search="http://schemas.xmlsoap.org/wsdl/soap/" replace="soap"/>\n'
             '    <Substitution type="package" search="http://schemas.xmlsoap.org/wsdl/soap12/" replace="soap12"/>\n'
             '    <Substitution type="package" search="http://schemas.xmlsoap.org/soap/envelope/" replace="soapenv"/>\n'
             '    <Substitution type="class" search="(.*)Class$" replace="\\1Type"/>\n'
             "  </Substitutions>\n"
+            "  <Extensions/>\n"
             "</Config>\n"
         )
         self.assertEqual(expected, file_path.read_text())
         file_path.unlink()
 
     def test_read(self):
         existing = (
             '<?xml version="1.0" encoding="UTF-8"?>\n'
             '<Config xmlns="http://pypi.org/project/xsdata" version="20.8">\n'
-            '  <Output maxLineLength="79">\n'
+            '  <Output maxLineLength="79" subscriptableTypes="false" unionType="false">\n'
             "    <Package>foo.bar</Package>\n"
             "  </Output>\n"
             "  <Conventions>\n"
             '    <ClassName case="pascalCase" safePrefix="type"/>\n'
             "  </Conventions>\n"
             "  <Aliases/>\n"
             "  <Substitutions/>\n"
@@ -84,15 +87,15 @@
         config = GeneratorConfig.read(file_path)
         with file_path.open("w") as fp:
             GeneratorConfig.write(fp, config)
 
         expected = (
             '<?xml version="1.0" encoding="UTF-8"?>\n'
             f'<Config xmlns="http://pypi.org/project/xsdata" version="{__version__}">\n'
-            '  <Output maxLineLength="79">\n'
+            '  <Output maxLineLength="79" subscriptableTypes="false" unionType="false">\n'
             "    <Package>foo.bar</Package>\n"
             '    <Format repr="true" eq="true" order="false" unsafeHash="false"'
             ' frozen="false" slots="false" kwOnly="false">dataclasses</Format>\n'
             "    <Structure>filenames</Structure>\n"
             "    <DocstringStyle>reStructuredText</DocstringStyle>\n"
             "    <FilterStrategy>allGlobals</FilterStrategy>\n"
             "    <RelativeImports>false</RelativeImports>\n"
@@ -107,14 +110,15 @@
             '    <FieldName case="snakeCase" safePrefix="value"/>\n'
             '    <ConstantName case="screamingSnakeCase" safePrefix="value"/>\n'
             '    <ModuleName case="snakeCase" safePrefix="mod"/>\n'
             '    <PackageName case="snakeCase" safePrefix="pkg"/>\n'
             "  </Conventions>\n"
             "  <Aliases/>\n"
             "  <Substitutions/>\n"
+            "  <Extensions/>\n"
             "</Config>\n"
         )
         self.assertEqual(expected, file_path.read_text())
 
     def test_read_with_wrong_value(self):
         existing = (
             '<?xml version="1.0" encoding="UTF-8"?>\n'
@@ -131,14 +135,44 @@
 
     def test_format_with_invalid_state(self):
         with self.assertRaises(GeneratorConfigError) as cm:
             OutputFormat(eq=False, order=True)
 
         self.assertEqual("eq must be true if order is true", str(cm.exception))
 
+    def test_subscriptable_types_requires_390(self):
+        if sys.version_info < (3, 9):
+            with warnings.catch_warnings(record=True) as w:
+                self.assertFalse(
+                    GeneratorOutput(subscriptable_types=True).subscriptable_types
+                )
+
+            self.assertEqual(
+                "Generics PEP 585 requires python >= 3.9, reverting...",
+                str(w[-1].message),
+            )
+
+        else:
+            self.assertTrue(
+                GeneratorOutput(subscriptable_types=True).subscriptable_types
+            )
+
+    def test_use_union_type_requires_310(self):
+        if sys.version_info < (3, 10):
+            with warnings.catch_warnings(record=True) as w:
+                self.assertFalse(GeneratorOutput(union_type=True).union_type)
+
+            self.assertEqual(
+                "UnionType PEP 604 requires python >= 3.10, reverting...",
+                str(w[-1].message),
+            )
+
+        else:
+            self.assertTrue(GeneratorOutput(union_type=True).union_type)
+
     def test_format_slots_requires_310(self):
         if sys.version_info < (3, 10):
             self.assertTrue(OutputFormat(slots=True, value="attrs").slots)
 
             with warnings.catch_warnings(record=True) as w:
                 self.assertFalse(OutputFormat(slots=True).slots)
 
@@ -205,7 +239,23 @@
         config.substitutions = None
         with output_path.open("w") as fp:
             config.write(fp, config)
 
         config = GeneratorConfig.read(output_path)
         self.assertIsNone(config.aliases)
         self.assertEqual(4, len(config.substitutions.substitution))
+
+    def test_extension_with_invalid_import_string(self):
+        cases = [None, "", "bar"]
+        for case in cases:
+            with self.assertRaises(GeneratorConfigError) as cm:
+                GeneratorExtension(type=ExtensionType.DECORATOR, import_string=case)
+
+            self.assertEqual(f"Invalid extension import '{case}'", str(cm.exception))
+
+    def test_extension_with_invalid_class_name_pattern(self):
+        with self.assertRaises(GeneratorConfigError) as cm:
+            GeneratorExtension(
+                type=ExtensionType.DECORATOR, import_string="a.b", class_name="*Foo"
+            )
+
+        self.assertEqual(f"Failed to compile pattern '*Foo'", str(cm.exception))
```

### Comparing `xsdata-23.5/tests/models/test_datatype.py` & `xsdata-23.6/tests/models/test_datatype.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/models/test_mixins.py` & `xsdata-23.6/tests/models/test_mixins.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/models/test_type_mapping.py` & `xsdata-23.6/tests/models/test_type_mapping.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/models/wsdl/test_binding.py` & `xsdata-23.6/tests/models/wsdl/test_binding.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/models/wsdl/test_definitions.py` & `xsdata-23.6/tests/models/wsdl/test_definitions.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/models/wsdl/test_port_type.py` & `xsdata-23.6/tests/models/wsdl/test_port_type.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/models/xsd/test_alternative.py` & `xsdata-23.6/tests/models/xsd/test_alternative.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/models/xsd/test_annotation_base.py` & `xsdata-23.6/tests/models/xsd/test_annotation_base.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/models/xsd/test_any.py` & `xsdata-23.6/tests/models/xsd/test_any.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/models/xsd/test_any_attribute.py` & `xsdata-23.6/tests/models/xsd/test_any_attribute.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/models/xsd/test_attribute.py` & `xsdata-23.6/tests/models/xsd/test_attribute.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/models/xsd/test_complex_type.py` & `xsdata-23.6/tests/models/xsd/test_complex_type.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/models/xsd/test_element.py` & `xsdata-23.6/tests/models/xsd/test_element.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/models/xsd/test_enumeration.py` & `xsdata-23.6/tests/models/xsd/test_enumeration.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/models/xsd/test_group.py` & `xsdata-23.6/tests/models/xsd/test_group.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/models/xsd/test_list.py` & `xsdata-23.6/tests/models/xsd/test_list.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/models/xsd/test_restriction.py` & `xsdata-23.6/tests/models/xsd/test_restriction.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/models/xsd/test_schema.py` & `xsdata-23.6/tests/models/xsd/test_schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/models/xsd/test_simple_type.py` & `xsdata-23.6/tests/models/xsd/test_simple_type.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/models/xsd/test_union.py` & `xsdata-23.6/tests/models/xsd/test_union.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/test_cli.py` & `xsdata-23.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/utils/test_collections.py` & `xsdata-23.6/tests/utils/test_collections.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/utils/test_dates.py` & `xsdata-23.6/tests/utils/test_dates.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/utils/test_downloader.py` & `xsdata-23.6/tests/utils/test_downloader.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/utils/test_hooks.py` & `xsdata-23.6/tests/utils/test_hooks.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/utils/test_namespaces.py` & `xsdata-23.6/tests/utils/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/tests/utils/test_text.py` & `xsdata-23.6/tests/utils/test_text.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/cli.py` & `xsdata-23.6/xsdata/cli.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/analyzer.py` & `xsdata-23.6/xsdata/codegen/analyzer.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/container.py` & `xsdata-23.6/xsdata/codegen/container.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -65,19 +65,19 @@
                 AddAttributeSubstitutions(self),
                 ProcessAttributeTypes(self),
                 MergeAttributes(),
                 ProcessMixedContentClass(),
             ],
             Steps.SANITIZE: [
                 ResetAttributeSequences(),
+                RenameDuplicateAttributes(),
                 SanitizeAttributesDefaultValue(self),
             ],
             Steps.RESOLVE: [
                 ValidateAttributesOverrides(self),
-                RenameDuplicateAttributes(),
             ],
             Steps.FINALIZE: [
                 VacuumInnerClasses(),
                 CreateCompoundFields(self),
                 # Prettify things!!!
                 ResetAttributeSequenceNumbers(self),
             ],
```

### Comparing `xsdata-23.5/xsdata/codegen/handlers/__init__.py` & `xsdata-23.6/xsdata/codegen/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/handlers/add_attribute_substitutions.py` & `xsdata-23.6/xsdata/codegen/handlers/add_attribute_substitutions.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/handlers/calculate_attribute_paths.py` & `xsdata-23.6/xsdata/codegen/handlers/calculate_attribute_paths.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/handlers/create_compound_fields.py` & `xsdata-23.6/xsdata/codegen/handlers/create_compound_fields.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/handlers/designate_class_packages.py` & `xsdata-23.6/xsdata/codegen/handlers/designate_class_packages.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/handlers/filter_classes.py` & `xsdata-23.6/xsdata/codegen/handlers/filter_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/handlers/flatten_attribute_groups.py` & `xsdata-23.6/xsdata/codegen/handlers/flatten_attribute_groups.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/handlers/flatten_class_extensions.py` & `xsdata-23.6/xsdata/codegen/handlers/flatten_class_extensions.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/handlers/merge_attributes.py` & `xsdata-23.6/xsdata/codegen/handlers/merge_attributes.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/handlers/process_attributes_types.py` & `xsdata-23.6/xsdata/codegen/handlers/process_attributes_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,17 +157,19 @@
     def copy_attribute_properties(
         cls, source: Class, target: Class, attr: Attr, attr_type: AttrType
     ):
         """
         Replace the given attribute type with the types of the single field
         source class.
 
-        Ignore enumerations and gracefully handle dump types with no attributes.
+        Ignore enumerations and gracefully handle dump types with no
+        attributes.
 
-        :raises: AnalyzerValueError if the source class has more than one attributes
+        :raises: AnalyzerValueError if the source class has more than
+            one attributes
         """
         source_attr = source.attrs[0]
         index = attr.types.index(attr_type)
         attr.types.pop(index)
 
         for source_attr_type in source_attr.types:
             clone_type = source_attr_type.clone()
```

### Comparing `xsdata-23.5/xsdata/codegen/handlers/process_mixed_content_class.py` & `xsdata-23.6/xsdata/codegen/handlers/process_mixed_content_class.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/handlers/rename_duplicate_attributes.py` & `xsdata-23.6/xsdata/codegen/handlers/rename_duplicate_attributes.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/handlers/rename_duplicate_classes.py` & `xsdata-23.6/xsdata/codegen/handlers/rename_duplicate_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/handlers/reset_attribute_sequence_numbers.py` & `xsdata-23.6/xsdata/codegen/handlers/reset_attribute_sequence_numbers.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/handlers/reset_attribute_sequences.py` & `xsdata-23.6/xsdata/codegen/handlers/reset_attribute_sequences.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/handlers/sanitize_attributes_default_value.py` & `xsdata-23.6/xsdata/codegen/handlers/sanitize_attributes_default_value.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/handlers/sanitize_enumeration_class.py` & `xsdata-23.6/xsdata/codegen/handlers/sanitize_enumeration_class.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/handlers/unnest_inner_classes.py` & `xsdata-23.6/xsdata/codegen/handlers/unnest_inner_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/handlers/update_attributes_effective_choice.py` & `xsdata-23.6/xsdata/codegen/handlers/update_attributes_effective_choice.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/handlers/vacuum_inner_classes.py` & `xsdata-23.6/xsdata/codegen/handlers/vacuum_inner_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/handlers/validate_attributes_overrides.py` & `xsdata-23.6/xsdata/codegen/handlers/validate_attributes_overrides.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/mappers/definitions.py` & `xsdata-23.6/xsdata/codegen/mappers/definitions.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/mappers/dict.py` & `xsdata-23.6/xsdata/codegen/mappers/dict.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/mappers/dtd.py` & `xsdata-23.6/xsdata/codegen/mappers/dtd.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/mappers/element.py` & `xsdata-23.6/xsdata/codegen/mappers/element.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/mappers/schema.py` & `xsdata-23.6/xsdata/codegen/mappers/schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/mixins.py` & `xsdata-23.6/xsdata/codegen/mixins.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/models.py` & `xsdata-23.6/xsdata/codegen/models.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/parsers/definitions.py` & `xsdata-23.6/xsdata/codegen/parsers/definitions.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/parsers/dtd.py` & `xsdata-23.6/xsdata/codegen/parsers/dtd.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/parsers/schema.py` & `xsdata-23.6/xsdata/codegen/parsers/schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/resolver.py` & `xsdata-23.6/xsdata/codegen/resolver.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/transformer.py` & `xsdata-23.6/xsdata/codegen/transformer.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/utils.py` & `xsdata-23.6/xsdata/codegen/utils.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/validator.py` & `xsdata-23.6/xsdata/codegen/validator.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/codegen/writer.py` & `xsdata-23.6/xsdata/codegen/writer.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/exceptions.py` & `xsdata-23.6/xsdata/exceptions.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/formats/bindings.py` & `xsdata-23.6/xsdata/formats/bindings.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/formats/converter.py` & `xsdata-23.6/xsdata/formats/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,16 @@
     """Abstract converter class."""
 
     @abc.abstractmethod
     def deserialize(self, value: Any, **kwargs: Any) -> Any:
         """
         Convert any type to the converter dedicated type.
 
-        :raises ConverterError: if converter fails with and expected ValueError
+        :raises ConverterError: if converter fails with and expected
+            ValueError
         """
 
     @abc.abstractmethod
     def serialize(self, value: Any, **kwargs: Any) -> str:
         """Convert value to string."""
 
     @classmethod
@@ -65,15 +66,16 @@
     def __init__(self):
         self.registry: Dict[Type, Converter] = {}
 
     def deserialize(self, value: Any, types: Sequence[Type], **kwargs: Any) -> Any:
         """
         Attempt to convert a any value to one of the given types.
 
-        If all attempts fail return the value input value and issue a warning.
+        If all attempts fail return the value input value and issue a
+        warning.
 
         :return: The first successful converted value.
         """
         for data_type in types:
             try:
                 instance = self.type_converter(data_type)
                 return instance.deserialize(value, data_type=data_type, **kwargs)
```

### Comparing `xsdata-23.5/xsdata/formats/dataclass/client.py` & `xsdata-23.6/xsdata/formats/dataclass/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,16 @@
 
     def prepare_headers(self, headers: Dict) -> Dict:
         """
         Prepare request headers according to the service configuration.
 
         Don't mutate input headers dictionary.
 
-        :raises ClientValueError: If the service transport type is unsupported.
+        :raises ClientValueError: If the service transport type is
+            unsupported.
         """
         result = headers.copy()
         if self.config.transport == TransportTypes.SOAP:
             result["content-type"] = "text/xml"
             if self.config.soap_action:
                 result["SOAPAction"] = self.config.soap_action
         else:
@@ -113,16 +114,16 @@
 
         return result
 
     def prepare_payload(self, obj: Any) -> Any:
         """
         Prepare and serialize payload to be sent.
 
-        :raises ClientValueError: If the config input type doesn't match the given
-            input.
+        :raises ClientValueError: If the config input type doesn't match
+            the given input.
         """
         if isinstance(obj, Dict):
             obj = self.dict_converter.convert(obj, self.config.input)
 
         if not isinstance(obj, self.config.input):
             raise ClientValueError(
                 f"Invalid input service type, "
```

### Comparing `xsdata-23.5/xsdata/formats/dataclass/compat.py` & `xsdata-23.6/xsdata/formats/dataclass/compat.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/formats/dataclass/context.py` & `xsdata-23.6/xsdata/formats/dataclass/context.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,96 +15,112 @@
 from xsdata.formats.dataclass.models.elements import XmlMeta
 from xsdata.models.enums import DataType
 from xsdata.utils.constants import return_input
 
 
 class XmlContext:
     """
-    The service provider for binding operations metadata.
+    The service provider for binding operations' metadata.
 
     :param element_name_generator: Default element name generator
     :param attribute_name_generator: Default attribute name generator
     :param class_type: Default class type `dataclasses`
+    :param models_package: Restrict auto locate to a specific package
     """
 
     __slots__ = (
         "element_name_generator",
         "attribute_name_generator",
         "class_type",
         "cache",
         "xsi_cache",
         "sys_modules",
+        "models_package",
     )
 
     def __init__(
         self,
         element_name_generator: Callable = return_input,
         attribute_name_generator: Callable = return_input,
         class_type: str = "dataclasses",
+        models_package: Optional[str] = None,
     ):
         self.element_name_generator = element_name_generator
         self.attribute_name_generator = attribute_name_generator
         self.class_type = class_types.get_type(class_type)
 
         self.cache: Dict[Type, XmlMeta] = {}
         self.xsi_cache: Dict[str, List[Type]] = defaultdict(list)
+        self.models_package = models_package
         self.sys_modules = 0
 
     def reset(self):
         self.cache.clear()
         self.xsi_cache.clear()
         self.sys_modules = 0
 
+    def get_builder(
+        self, globalns: Optional[Dict[str, Callable]] = None
+    ) -> XmlMetaBuilder:
+        return XmlMetaBuilder(
+            class_type=self.class_type,
+            element_name_generator=self.element_name_generator,
+            attribute_name_generator=self.attribute_name_generator,
+            globalns=globalns,
+        )
+
     def fetch(
         self,
         clazz: Type,
         parent_ns: Optional[str] = None,
         xsi_type: Optional[str] = None,
     ) -> XmlMeta:
         """
         Fetch the model metadata of the given dataclass type, namespace and xsi
         type.
 
         :param clazz: The requested dataclass type
         :param parent_ns: The inherited parent namespace
-        :param xsi_type: if present it means that the given clazz is derived and the
-            lookup procedure needs to check and match a dataclass model to the qualified
-            name instead
+        :param xsi_type: if present it means that the given clazz is
+            derived and the lookup procedure needs to check and match a
+            dataclass model to the qualified name instead
         """
         meta = self.build(clazz, parent_ns)
         subclass = None
         if xsi_type and meta.target_qname != xsi_type:
             subclass = self.find_subclass(clazz, xsi_type)
 
         return self.build(subclass, parent_ns) if subclass else meta
 
     def build_xsi_cache(self):
         """Index all imported dataclasses by their xsi:type qualified name."""
         if len(sys.modules) == self.sys_modules:
             return
 
         self.xsi_cache.clear()
-        builder = XmlMetaBuilder(
-            class_type=self.class_type,
-            element_name_generator=self.element_name_generator,
-            attribute_name_generator=self.attribute_name_generator,
-        )
+        builder = self.get_builder()
         for clazz in self.get_subclasses(object):
-            # This is new!
-            if clazz.__module__.startswith("_pytest"):
-                continue
-
-            if self.class_type.is_model(clazz):
-                meta = builder.build_class_meta(clazz, None)
+            if self.is_binding_model(clazz):
+                meta = builder.build_class_meta(clazz)
 
                 if meta.target_qname:
                     self.xsi_cache[meta.target_qname].append(clazz)
 
         self.sys_modules = len(sys.modules)
 
+    def is_binding_model(self, clazz: Type[T]) -> bool:
+        if not self.class_type.is_model(clazz):
+            return False
+
+        return not self.models_package or (
+            hasattr(clazz, "__module__")
+            and isinstance(clazz.__module__, str)
+            and clazz.__module__.startswith(self.models_package)
+        )
+
     def find_types(self, qname: str) -> List[Type[T]]:
         """
         Find all classes that match the given xsi:type qname.
 
         - Ignores native schema types, xs:string, xs:float, xs:int, ...
         - Rebuild cache if new modules were imported since last run
 
@@ -183,22 +199,16 @@
         """
         Fetch from cache or build the binding metadata for the given class and
         parent namespace.
 
         :param clazz: A dataclass type
         :param parent_ns: The inherited parent namespace
         """
-
         if clazz not in self.cache:
-            builder = XmlMetaBuilder(
-                class_type=self.class_type,
-                element_name_generator=self.element_name_generator,
-                attribute_name_generator=self.attribute_name_generator,
-                globalns=globalns,
-            )
+            builder = self.get_builder(globalns)
             self.cache[clazz] = builder.build(clazz, parent_ns)
         return self.cache[clazz]
 
     def build_recursive(self, clazz: Type, parent_ns: Optional[str] = None):
         """Build the binding metadata for the given class and all of its
         dependencies."""
         if clazz not in self.cache:
@@ -210,15 +220,22 @@
                         self.build_recursive(tp, meta.namespace)
 
     def local_names_match(self, names: Set[str], clazz: Type) -> bool:
         try:
             meta = self.build(clazz)
             local_names = {var.local_name for var in meta.get_all_vars()}
             return not names.difference(local_names)
-        except XmlContextError:
+        except (XmlContextError, NameError):
+            # The dataclass includes unsupported typing annotations
+            # Let's remove it from xsi_cache
+            builder = self.get_builder()
+            target_qname = builder.build_class_meta(clazz).target_qname
+            if target_qname and target_qname in self.xsi_cache:
+                self.xsi_cache[target_qname].remove(clazz)
+
             return False
 
     @classmethod
     def is_derived(cls, obj: Any, clazz: Type) -> bool:
         """
         Return whether the given obj is derived from the given dataclass type.
```

### Comparing `xsdata-23.5/xsdata/formats/dataclass/filters.py` & `xsdata-23.6/xsdata/formats/dataclass/filters.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,28 +4,31 @@
 from collections import defaultdict
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
+from typing import Set
 from typing import Tuple
 from typing import Type
 
 from docformatter import configuration
 from docformatter import format
 from jinja2 import Environment
 
 from xsdata.codegen.models import Attr
 from xsdata.codegen.models import AttrType
 from xsdata.codegen.models import Class
 from xsdata.formats.converter import converter
 from xsdata.formats.dataclass.models.elements import XmlType
 from xsdata.models.config import DocstringStyle
+from xsdata.models.config import ExtensionType
 from xsdata.models.config import GeneratorConfig
+from xsdata.models.config import GeneratorExtension
 from xsdata.models.config import ObjectType
 from xsdata.models.config import OutputFormat
 from xsdata.utils import collections
 from xsdata.utils import namespaces
 from xsdata.utils import text
 from xsdata.utils.objects import literal_value
 
@@ -33,71 +36,104 @@
 class Filters:
     DEFAULT_KEY = "default"
     FACTORY_KEY = "default_factory"
     UNESCAPED_DBL_QUOTE_REGEX = re.compile(r"([^\\])\"")
 
     __slots__ = (
         "substitutions",
+        "extensions",
         "class_case",
         "field_case",
         "constant_case",
         "package_case",
         "module_case",
         "class_safe_prefix",
         "field_safe_prefix",
         "constant_safe_prefix",
         "package_safe_prefix",
         "module_safe_prefix",
         "docstring_style",
         "max_line_length",
+        "union_type",
+        "subscriptable_types",
         "relative_imports",
         "postponed_annotations",
         "format",
         "import_patterns",
+        "default_class_annotation",
     )
 
     def __init__(self, config: GeneratorConfig):
         self.substitutions: Dict[ObjectType, Dict[str, str]] = defaultdict(dict)
         for sub in config.substitutions.substitution:
             self.substitutions[sub.type][sub.search] = sub.replace
 
+        self.import_patterns: Dict[str, Dict[str, Set[str]]] = defaultdict(
+            lambda: defaultdict(set)
+        )
+        self.extensions: Dict[ExtensionType, List[GeneratorExtension]] = defaultdict(
+            list
+        )
+        for ext in config.extensions.extension:
+            self.extensions[ext.type].append(ext)
+
+            is_annotation = ext.type is ExtensionType.DECORATOR
+            patterns = self.import_patterns[ext.module_path][ext.func_name]
+
+            if is_annotation:
+                patterns.add(f"@{ext.func_name}")
+            else:
+                patterns.update(
+                    [
+                        f"({ext.func_name}",
+                        f" {ext.func_name})",
+                    ]
+                )
+
         self.class_case: Callable = config.conventions.class_name.case
         self.field_case: Callable = config.conventions.field_name.case
         self.constant_case: Callable = config.conventions.constant_name.case
         self.package_case: Callable = config.conventions.package_name.case
         self.module_case: Callable = config.conventions.module_name.case
         self.class_safe_prefix: str = config.conventions.class_name.safe_prefix
         self.field_safe_prefix: str = config.conventions.field_name.safe_prefix
         self.constant_safe_prefix: str = config.conventions.constant_name.safe_prefix
         self.package_safe_prefix: str = config.conventions.package_name.safe_prefix
         self.module_safe_prefix: str = config.conventions.module_name.safe_prefix
         self.docstring_style: DocstringStyle = config.output.docstring_style
         self.max_line_length: int = config.output.max_line_length
+        self.union_type: bool = config.output.union_type
+        self.subscriptable_types: bool = config.output.subscriptable_types
         self.relative_imports: bool = config.output.relative_imports
         self.postponed_annotations: bool = config.output.postponed_annotations
         self.format = config.output.format
 
         # Build things
-        self.import_patterns = self.build_import_patterns()
+        for module, imports in self.build_import_patterns().items():
+            for imp, patterns in imports.items():
+                self.import_patterns[module][imp].update(patterns)
+
+        self.default_class_annotation = self.build_class_annotation(self.format)
 
     def register(self, env: Environment):
         env.globals.update(
             {
                 "docstring_name": self.docstring_style.name.lower(),
-                "class_annotation": self.build_class_annotation(self.format),
             }
         )
         env.filters.update(
             {
                 "field_name": self.field_name,
                 "field_type": self.field_type,
                 "field_default": self.field_default_value,
                 "field_metadata": self.field_metadata,
                 "field_definition": self.field_definition,
                 "class_name": self.class_name,
+                "class_bases": self.class_bases,
+                "class_annotations": self.class_annotations,
                 "class_params": self.class_params,
                 "format_string": self.format_string,
                 "format_docstring": self.format_docstring,
                 "constant_name": self.constant_name,
                 "constant_value": self.constant_value,
                 "default_imports": self.default_imports,
                 "format_metadata": self.format_metadata,
@@ -106,29 +142,29 @@
                 "clean_docstring": self.clean_docstring,
                 "import_module": self.import_module,
                 "import_class": self.import_class,
             }
         )
 
     @classmethod
-    def build_class_annotation(cls, format: OutputFormat) -> str:
+    def build_class_annotation(cls, fmt: OutputFormat) -> str:
         args = []
-        if not format.repr:
+        if not fmt.repr:
             args.append("repr=False")
-        if not format.eq:
+        if not fmt.eq:
             args.append("eq=False")
-        if format.order:
+        if fmt.order:
             args.append("order=True")
-        if format.unsafe_hash:
+        if fmt.unsafe_hash:
             args.append("unsafe_hash=True")
-        if format.frozen:
+        if fmt.frozen:
             args.append("frozen=True")
-        if format.slots:
+        if fmt.slots:
             args.append("slots=True")
-        if format.kw_only:
+        if fmt.kw_only:
             args.append("kw_only=True")
 
         return f"@dataclass({', '.join(args)})" if args else "@dataclass"
 
     def class_params(self, obj: Class):
         is_enum = obj.is_enumeration
         for attr in obj.attrs:
@@ -142,14 +178,46 @@
     def class_name(self, name: str) -> str:
         """Convert the given string to a class name according to the selected
         conventions or use an existing alias."""
         name = self.apply_substitutions(name, ObjectType.CLASS)
         name = self.safe_name(name, self.class_safe_prefix, self.class_case)
         return self.apply_substitutions(name, ObjectType.CLASS)
 
+    def class_bases(self, obj: Class, class_name: str) -> List[str]:
+        """Return a list of base class names."""
+        bases = []
+        for obj_ext in obj.extensions:
+            bases.append(self.type_name(obj_ext.type))
+
+        derived = len(obj.extensions) > 0
+        for ext in self.extensions[ExtensionType.CLASS]:
+            is_valid = not derived or ext.apply_if_derived
+            if is_valid and ext.pattern.match(class_name):
+                if ext.prepend:
+                    bases.insert(0, ext.func_name)
+                else:
+                    bases.append(ext.func_name)
+
+        return collections.unique_sequence(bases)
+
+    def class_annotations(self, obj: Class, class_name: str) -> List[str]:
+        """Return a list of decorator names."""
+        annotations = [self.default_class_annotation]
+
+        derived = len(obj.extensions) > 0
+        for ext in self.extensions[ExtensionType.DECORATOR]:
+            is_valid = not derived or ext.apply_if_derived
+            if is_valid and ext.pattern.match(class_name):
+                if ext.prepend:
+                    annotations.insert(0, f"@{ext.func_name}")
+                else:
+                    annotations.append(f"@{ext.func_name}")
+
+        return collections.unique_sequence(annotations)
+
     def apply_substitutions(self, name: str, obj_type: ObjectType) -> str:
         for search, replace in self.substitutions[obj_type].items():
             name = re.sub(rf"{search}", rf"{replace}", name)
 
         return name
 
     def field_definition(
@@ -596,36 +664,41 @@
         if attr.is_prohibited:
             return "Any"
 
         type_names = collections.unique_sequence(
             self.field_type_name(x, parents) for x in attr.types
         )
 
-        result = ", ".join(type_names)
-        if len(type_names) > 1:
-            result = f"Union[{result}]"
+        if self.union_type:
+            result = " | ".join(type_names)
+        else:
+            result = ", ".join(type_names)
+            if len(type_names) > 1:
+                result = f"Union[{result}]"
 
         iterable = "Tuple[{}, ...]" if self.format.frozen else "List[{}]"
+        if self.subscriptable_types:
+            iterable = iterable.lower()
 
         if attr.is_tokens:
             result = iterable.format(result)
 
         if attr.is_list:
             return iterable.format(result)
 
         if attr.is_tokens:
             return result
 
         if attr.is_dict:
-            return "Dict[str, str]"
+            return "dict[str, str]" if self.subscriptable_types else "Dict[str, str]"
 
         if attr.is_nillable or (
             attr.default is None and (attr.is_optional or not self.format.kw_only)
         ):
-            return f"Optional[{result}]"
+            return f"None | {result}" if self.union_type else f"Optional[{result}]"
 
         return result
 
     def choice_type(self, choice: Attr, parents: List[str]) -> str:
         """
         Generate type hints for the given choice.
 
@@ -636,22 +709,30 @@
         compound field that might be a list, that's why list restriction
         is also ignored.
         """
         type_names = collections.unique_sequence(
             self.field_type_name(x, parents) for x in choice.types
         )
 
-        result = ", ".join(type_names)
-        if len(type_names) > 1:
-            result = f"Union[{result}]"
+        if self.union_type:
+            result = " | ".join(type_names)
+        else:
+            result = ", ".join(type_names)
+            if len(type_names) > 1:
+                result = f"Union[{result}]"
 
         if choice.is_tokens:
-            result = (
-                f"Tuple[{result}, ...]" if self.format.frozen else f"List[{result}]"
-            )
+            iterable = "Tuple[{}, ...]" if self.format.frozen else "List[{}]"
+            if self.subscriptable_types:
+                iterable = iterable.lower()
+
+            result = iterable.format(result)
+
+        if self.subscriptable_types:
+            return f"type[{result}]"
 
         return f"Type[{result}]"
 
     def field_type_name(self, attr_type: AttrType, parents: List[str]) -> str:
         name = self.type_name(attr_type)
 
         if attr_type.forward and attr_type.circular:
@@ -659,14 +740,17 @@
             name = f'"{outer_str}"'
         elif attr_type.forward:
             outer_str = ".".join(map(self.class_name, parents))
             name = f'"{outer_str}.{name}"'
         elif attr_type.circular:
             name = f'"{name}"'
 
+        if self.postponed_annotations:
+            name = name.strip('"')
+
         return name
 
     def constant_value(self, attr: Attr) -> str:
         """Return the attr default value or type as constant value."""
         attr_type = attr.types[0]
         if attr_type.native:
             return f'"{attr.default}"'
@@ -691,15 +775,15 @@
             ]
 
             if len(names) == 1 and names[0] == "__module__":
                 result.append(f"import {library}")
             elif names:
                 result.append(f"from {library} import {', '.join(names)}")
 
-        return "\n".join(result)
+        return "\n".join(sorted(result))
 
     @classmethod
     def build_import_patterns(cls) -> Dict[str, Dict]:
         type_patterns = cls.build_type_patterns
         return {
             "dataclasses": {"dataclass": ["@dataclass"], "field": [" = field("]},
             "decimal": {"Decimal": type_patterns("Decimal")},
@@ -721,8 +805,17 @@
                 "XmlPeriod": type_patterns("XmlPeriod"),
                 "XmlTime": type_patterns("XmlTime"),
             },
         }
 
     @classmethod
     def build_type_patterns(cls, x: str) -> Tuple:
-        return f": {x} =", f"[{x}]", f"[{x},", f" {x},", f" {x}]", f" {x}("
+        return (
+            f": {x} =",
+            f"[{x}]",
+            f"[{x},",
+            f" {x},",
+            f" {x}]",
+            f" {x}(",
+            f" | {x}",
+            f"{x} |",
+        )
```

### Comparing `xsdata-23.5/xsdata/formats/dataclass/generator.py` & `xsdata-23.6/xsdata/formats/dataclass/generator.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/formats/dataclass/models/builders.py` & `xsdata-23.6/xsdata/formats/dataclass/models/builders.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,15 @@
                 self.class_type.default_value(field),
                 globalns,
             )
             if var is not None:
                 yield var
 
     def build_class_meta(
-        self, clazz: Type, parent_namespace: Optional[str]
+        self, clazz: Type, parent_namespace: Optional[str] = None
     ) -> ClassMeta:
         """
         Fetch the class meta options and merge defaults.
 
         Metaclass is not inheritable
         """
         meta = clazz.Meta if "Meta" in clazz.__dict__ else None
@@ -410,21 +410,22 @@
         namespace: Optional[str],
         parent_namespace: Optional[str],
     ) -> Tuple[str, ...]:
         """
         Resolve the namespace(s) for the given xml type and the parent
         namespace.
 
-        Only elements and wildcards are allowed to inherit the parent namespace if
-        the given namespace is empty.
+        Only elements and wildcards are allowed to inherit the parent
+        namespace if the given namespace is empty.
 
-        In case of wildcard try to decode the ##any, ##other, ##local, ##target.
+        In case of wildcard try to decode the ##any, ##other, ##local,
+        ##target.
 
-
-        :param xml_type: The xml type (Text|Element(s)|Attribute(s)|Wildcard)
+        :param xml_type: The xml type
+            (Text|Element(s)|Attribute(s)|Wildcard)
         :param namespace: The field namespace
         :param parent_namespace: The parent namespace
         """
         if xml_type in (XmlType.ELEMENT, XmlType.WILDCARD) and namespace is None:
             namespace = parent_namespace
 
         if not namespace:
@@ -444,16 +445,16 @@
         return tuple(result)
 
     @classmethod
     def default_namespace(cls, namespaces: Sequence[str]) -> Optional[str]:
         """
         Return the first valid namespace uri or None.
 
-        :param namespaces: A list of namespace options which may
-            include valid uri(s) or one of the ##any, ##other,
+        :param namespaces: A list of namespace options which may include
+            valid uri(s) or one of the ##any, ##other,
             ##targetNamespace, ##local
         """
         for namespace in namespaces:
             if namespace and not namespace.startswith("#"):
                 return namespace
 
         return None
@@ -470,18 +471,19 @@
     def analyze_types(
         cls, type_hint: Any, globalns: Any
     ) -> Tuple[Any, Any, Tuple[Type, ...]]:
         """
         Analyze a type hint and return the origin, sub origin and the type
         args.
 
-        The only case we support a sub origin is for fields derived from xs:NMTOKENS!
-
+        The only case we support a sub origin is for fields derived from
+        xs:NMTOKENS!
 
-        :raises XmlContextError: if the typing is not supported for binding
+        :raises XmlContextError: if the typing is not supported for
+            binding
         """
         try:
             types = evaluate(type_hint, globalns)
             origin = None
             sub_origin = None
 
             while types[0] in (tuple, list, dict):
```

### Comparing `xsdata-23.5/xsdata/formats/dataclass/models/elements.py` & `xsdata-23.6/xsdata/formats/dataclass/models/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,16 @@
     """
     Class field binding metadata.
 
     :param index: Field ordering
     :param name: Field name
     :param qname: Qualified name
     :param types: List of all the supported data types
-    :param init:  Include field in the constructor
-    :param mixed:  Field supports mixed content type values
+    :param init: Include field in the constructor
+    :param mixed: Field supports mixed content type values
     :param tokens: Field is derived from xs:list
     :param format: Value format information
     :param derived: Wrap parsed values with a generic type
     :param any_type: Field supports dynamic value types
     :param required: Field is mandatory
     :param nillable: Field supports nillable content
     :param sequence: Render values in sequential mode
@@ -294,15 +294,16 @@
 class XmlMeta(MetaMixin):
     """
     Class binding metadata.
 
     :param clazz: The dataclass type
     :param qname: The namespace qualified name.
     :param target_qname: The target namespace qualified name.
-    :param nillable: Specifies whether an explicit empty value can be assigned.
+    :param nillable: Specifies whether an explicit empty value can be
+        assigned.
     :param mixed_content: Has a wildcard with mixed flag enabled
     :param text: Text var
     :param choices: List of compound vars
     :param elements: Mapping of qname-element vars
     :param wildcards: List of wildcard vars
     :param attributes: Mapping of qname-attribute vars
     :param any_attributes: List of wildcard attributes vars
```

### Comparing `xsdata-23.5/xsdata/formats/dataclass/models/generics.py` & `xsdata-23.6/xsdata/formats/dataclass/models/generics.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/formats/dataclass/parsers/bases.py` & `xsdata-23.6/xsdata/formats/dataclass/parsers/bases.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,16 +136,15 @@
         text: Optional[str],
         tail: Optional[str],
     ) -> bool:
         """
         End element notification receiver.
 
         Pop the last XmlNode from the queue and use it to build and
-        return the resulting object tree with its text and tail
-        content.
+        return the resulting object tree with its text and tail content.
 
         :param queue: Xml nodes queue
         :param objects: List of parsed objects
         :param qname: Qualified name
         :param text: Text content
         :param tail: Tail content
         """
@@ -171,16 +170,16 @@
         qname: str,
         attrs: Dict,
         ns_map: Dict,
     ):
         """
         Start element notification receiver.
 
-        Build and queue the XmlNode for the starting element, append
-        the event with the attributes and ns map to the events list.
+        Build and queue the XmlNode for the starting element, append the
+        event with the attributes and ns map to the events list.
 
         :param clazz: Root class type, if it's missing look for any
             suitable models from the current context.
         :param queue: The active XmlNode queue
         :param objects: The list of all intermediate parsed objects
         :param qname: Qualified name
         :param attrs: Attributes key-value map
@@ -197,17 +196,17 @@
         text: Optional[str],
         tail: Optional[str],
     ) -> Any:
         """
         End element notification receiver.
 
         Pop the last XmlNode from the queue and use it to build and
-        return the resulting object tree with its text and tail
-        content. Append the end event with the text,tail content to
-        the events list.
+        return the resulting object tree with its text and tail content.
+        Append the end event with the text,tail content to the events
+        list.
 
         :param queue: Xml nodes queue
         :param objects: List of parsed objects
         :param qname: Qualified name
         :param text: Text content
         :param tail: Tail content
         """
```

### Comparing `xsdata-23.5/xsdata/formats/dataclass/parsers/config.py` & `xsdata-23.6/xsdata/formats/dataclass/parsers/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,43 +10,47 @@
     return cls(**params)  # type: ignore
 
 
 class ParserConfig:
     """
     Parsing configuration options.
 
-    :param base_url: Specify a base URL when parsing from memory and
-        you need support for relative links eg xinclude
+    :param base_url: Specify a base URL when parsing from memory, and
+        you need support for relative links e.g. xinclude
+    :param load_dtd: Enable loading external dtd (lxml only)
     :param process_xinclude: Enable xinclude statements processing
     :param class_factory: Override default object instantiation
-    :param fail_on_unknown_properties: Skip unknown properties or
+    :param fail_on_unknown_properties: Skip unknown properties or fail
+        with exception
+    :param fail_on_unknown_attributes: Skip unknown XML attributes or
         fail with exception
-    :param fail_on_unknown_attributes: Skip unknown XML attributes
-        or fail with exception
     :param fail_on_converter_warnings: Turn converter warnings to
         exceptions
     """
 
     __slots__ = (
         "base_url",
+        "load_dtd",
         "process_xinclude",
         "class_factory",
         "fail_on_unknown_properties",
         "fail_on_unknown_attributes",
         "fail_on_converter_warnings",
     )
 
     def __init__(
         self,
         base_url: Optional[str] = None,
+        load_dtd: bool = False,
         process_xinclude: bool = False,
         class_factory: Callable[[Type[T], Dict], T] = default_class_factory,
         fail_on_unknown_properties: bool = True,
         fail_on_unknown_attributes: bool = False,
         fail_on_converter_warnings: bool = False,
     ):
         self.base_url = base_url
+        self.load_dtd = load_dtd
         self.process_xinclude = process_xinclude
         self.class_factory = class_factory
         self.fail_on_unknown_properties = fail_on_unknown_properties
         self.fail_on_unknown_attributes = fail_on_unknown_attributes
         self.fail_on_converter_warnings = fail_on_converter_warnings
```

### Comparing `xsdata-23.5/xsdata/formats/dataclass/parsers/handlers/__init__.py` & `xsdata-23.6/xsdata/formats/dataclass/parsers/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/formats/dataclass/parsers/handlers/lxml.py` & `xsdata-23.6/xsdata/formats/dataclass/parsers/handlers/lxml.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,33 +19,39 @@
     """
 
     __slots__ = ()
 
     def parse(self, source: Any) -> Any:
         """
         Parse an XML document from a system identifier or an InputSource or
-        directly from an lxml Element or Tree.
+        directly from a lxml Element or Tree.
 
-        When Source is an lxml Element or Tree the handler will switch
-        to the :class:`lxml.etree.iterwalk` api.
+        When Source is a lxml Element or Tree the handler will switch to
+        the :class:`lxml.etree.iterwalk` api.
 
         When source is a system identifier or an InputSource the parser
         will ignore comments and recover from errors.
 
         When config process_xinclude is enabled the handler will parse
         the whole document and then walk down the element tree.
         """
         if isinstance(source, (etree._ElementTree, etree._Element)):
             ctx = etree.iterwalk(source, EVENTS)
         elif self.parser.config.process_xinclude:
             tree = etree.parse(source, base_url=self.parser.config.base_url)  # nosec
             tree.xinclude()
             ctx = etree.iterwalk(tree, EVENTS)
         else:
-            ctx = etree.iterparse(source, EVENTS, recover=True, remove_comments=True)
+            ctx = etree.iterparse(
+                source,
+                EVENTS,
+                recover=True,
+                remove_comments=True,
+                load_dtd=self.parser.config.load_dtd,
+            )
 
         return self.process_context(ctx)
 
     def process_context(self, context: Iterable) -> Any:
         """Iterate context and push the events to main parser."""
         for event, element in context:
             if event == EventType.START:
```

### Comparing `xsdata-23.5/xsdata/formats/dataclass/parsers/handlers/native.py` & `xsdata-23.6/xsdata/formats/dataclass/parsers/handlers/native.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/formats/dataclass/parsers/json.py` & `xsdata-23.6/xsdata/formats/dataclass/parsers/json.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 @dataclass
 class JsonParser(AbstractParser):
     """
     Json parser for dataclasses.
 
     :param config: Parser configuration
     :param context: Model context provider
-    :param load_factory: Replace the default json.load call with another implementation
+    :param load_factory: Replace the default json.load call with another
+        implementation
     """
 
     config: ParserConfig = field(default_factory=ParserConfig)
     context: XmlContext = field(default_factory=XmlContext)
     load_factory: Callable = field(default=json.load)
 
     def parse(self, source: Any, clazz: Optional[Type[T]] = None) -> T:
@@ -70,15 +71,15 @@
     def verify_type(self, clazz: Optional[Type[T]], data: Union[Dict, List]) -> Type[T]:
         if clazz is None:
             return self.detect_type(data)
 
         try:
             origin = get_origin(clazz)
             list_type = False
-            if origin is List:
+            if origin is list:
                 list_type = True
                 args = get_args(clazz)
 
                 if len(args) != 1 or not self.context.class_type.is_model(args[0]):
                     raise TypeError()
 
                 clazz = args[0]
```

### Comparing `xsdata-23.5/xsdata/formats/dataclass/parsers/mixins.py` & `xsdata-23.6/xsdata/formats/dataclass/parsers/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,17 @@
 
     @abc.abstractmethod
     def child(self, qname: str, attrs: Dict, ns_map: Dict, position: int) -> "XmlNode":
         """
         Initialize the next child node to be queued, when a new xml element
         starts.
 
-        This entry point is responsible to create the next node
-        type with all the necessary information on how to bind
-        the incoming input data.
+        This entry point is responsible to create the next node type
+        with all the necessary information on how to bind the incoming
+        input data.
 
         :param qname: Qualified name
         :param attrs: Attribute key-value map
         :param ns_map: Namespace prefix-URI map
         :param position: The current objects position, to mark future
             objects as children
         """
@@ -92,22 +92,22 @@
     @abc.abstractmethod
     def bind(self, qname: str, text: NoneStr, tail: NoneStr, objects: List) -> bool:
         """
         Build the object tree for the ending element and return whether the
         result was successful or not.
 
         This entry point is called when an xml element ends and is
-        responsible to parse the current element attributes/text,
-        bind any children objects and initialize  new object.
+        responsible to parse the current element attributes/text, bind
+        any children objects and initialize  new object.
 
         :param qname: Qualified name
         :param text: Text content
         :param tail: Tail content
-        :param objects: The list of intermediate parsed objects,
-            eg [(qname, object)]
+        :param objects: The list of intermediate parsed objects, eg
+            [(qname, object)]
         """
 
 
 class XmlHandler:
     """
     Abstract content handler.
```

### Comparing `xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/__init__.py` & `xsdata-23.6/xsdata/formats/dataclass/parsers/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/element.py` & `xsdata-23.6/xsdata/formats/dataclass/parsers/nodes/element.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,17 +179,17 @@
         return False
 
     @classmethod
     def bind_var(cls, params: Dict, var: XmlVar, value: Any) -> bool:
         """
         Add the given value to the params dictionary with the var name as key.
 
-        Wrap the value to a list if var is a list. If the var name already exists it
-        means we have a name conflict and the parser needs to lookup for any available
-        wildcard fields.
+        Wrap the value to a list if var is a list. If the var name
+        already exists it means we have a name conflict and the parser
+        needs to lookup for any available wildcard fields.
 
         :return: Whether the binding process was successful or not.
         """
         if var.init:
             if var.list_element:
                 items = params.get(var.name)
                 if items is None:
```

### Comparing `xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/primitive.py` & `xsdata-23.6/xsdata/formats/dataclass/parsers/nodes/primitive.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/skip.py` & `xsdata-23.6/xsdata/formats/dataclass/parsers/nodes/skip.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/standard.py` & `xsdata-23.6/xsdata/formats/dataclass/parsers/nodes/standard.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/union.py` & `xsdata-23.6/xsdata/formats/dataclass/parsers/nodes/union.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/wildcard.py` & `xsdata-23.6/xsdata/formats/dataclass/parsers/nodes/wildcard.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/wrapper.py` & `xsdata-23.6/xsdata/formats/dataclass/parsers/nodes/wrapper.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/formats/dataclass/parsers/tree.py` & `xsdata-23.6/xsdata/formats/dataclass/parsers/tree.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/formats/dataclass/parsers/utils.py` & `xsdata-23.6/xsdata/formats/dataclass/parsers/utils.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/formats/dataclass/parsers/xml.py` & `xsdata-23.6/xsdata/formats/dataclass/parsers/xml.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/formats/dataclass/serializers/code.py` & `xsdata-23.6/xsdata/formats/dataclass/serializers/code.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 
 
 @dataclass
 class PycodeSerializer(AbstractSerializer):
     """
     Pycode serializer for dataclasses.
 
-    Return a python representation code of
-    a model instance.
+    Return a python representation code of a model instance.
 
     :param config: Serializer configuration
     :param context: Model context provider
     """
 
     config: SerializerConfig = field(default_factory=SerializerConfig)
     context: XmlContext = field(default_factory=XmlContext)
```

### Comparing `xsdata-23.5/xsdata/formats/dataclass/serializers/config.py` & `xsdata-23.6/xsdata/formats/dataclass/serializers/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     :param pretty_print: Enable pretty output
     :param pretty_print_indent: Indentation string for each indent level
     :param ignore_default_attributes: Ignore optional attributes with
         default values
     :param schema_location: xsi:schemaLocation attribute value
     :param no_namespace_schema_location: xsi:noNamespaceSchemaLocation
         attribute value
-    :param globalns: Dictionary containing global variables to extend
-        or overwrite for typing
+    :param globalns: Dictionary containing global variables to extend or
+        overwrite for typing
     """
 
     __slots__ = (
         "encoding",
         "xml_version",
         "xml_declaration",
         "pretty_print",
```

### Comparing `xsdata-23.5/xsdata/formats/dataclass/serializers/json.py` & `xsdata-23.6/xsdata/formats/dataclass/serializers/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,18 @@
 @dataclass
 class JsonSerializer(AbstractSerializer):
     """
     Json serializer for dataclasses.
 
     :param config: Serializer configuration
     :param context: Model context provider
-    :param dict_factory: Override default dict factory to add further logic
-    :param dump_factory: Override default json.dump call with another implementation
+    :param dict_factory: Override default dict factory to add further
+        logic
+    :param dump_factory: Override default json.dump call with another
+        implementation
     :param indent: Output indentation level
     """
 
     config: SerializerConfig = field(default_factory=SerializerConfig)
     context: XmlContext = field(default_factory=XmlContext)
     dict_factory: Callable = field(default=dict)
     dump_factory: Callable = field(default=json.dump)
```

### Comparing `xsdata-23.5/xsdata/formats/dataclass/serializers/mixins.py` & `xsdata-23.6/xsdata/formats/dataclass/serializers/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,17 +126,16 @@
             self.output.write(f'<?xml version="{self.config.xml_version}"')
             self.output.write(f' encoding="{self.config.encoding}"?>\n')
 
     def start_tag(self, qname: str):
         """
         Start tag notification receiver.
 
-        The receiver will flush the start of any pending element,
-        create new namespaces context and queue the current tag
-        for generation.
+        The receiver will flush the start of any pending element, create
+        new namespaces context and queue the current tag for generation.
 
         :param qname: Tag qualified name
         """
         self.flush_start(False)
 
         self.ns_context.append(self.ns_map.copy())
         self.ns_map = self.ns_context[-1]
@@ -144,17 +143,17 @@
         self.pending_tag = split_qname(qname)
         self.add_namespace(self.pending_tag[0])
 
     def add_attribute(self, key: str, value: Any, check_pending: bool = True):
         """
         Add attribute notification receiver.
 
-        The receiver will convert the key to a namespace, name tuple
-        and convert the value to string. Internally the converter will
-        also generate any missing namespace prefixes.
+        The receiver will convert the key to a namespace, name tuple and
+        convert the value to string. Internally the converter will also
+        generate any missing namespace prefixes.
 
         :param key: Attribute name
         :param value: Attribute value
         :param check_pending: Raise exception if not no element is
             pending start
         """
         if not self.pending_tag and check_pending:
@@ -179,20 +178,20 @@
         if uri and not prefix_exists(uri, self.ns_map):
             generate_prefix(uri, self.ns_map)
 
     def set_data(self, data: Any):
         """
         Set data notification receiver.
 
-        The receiver will convert the data to string, flush any previous pending
-        start element and send it to the handler for generation.
+        The receiver will convert the data to string, flush any previous
+        pending start element and send it to the handler for generation.
 
-        If the text content of the tag has already been generated then treat the
-        current data as element tail content and queue it to be generated when the
-        tag ends.
+        If the text content of the tag has already been generated then
+        treat the current data as element tail content and queue it to
+        be generated when the tag ends.
 
         :param data: Element text or tail content
         """
         value = self.encode_data(data)
         self.flush_start(is_nil=value is None)
 
         if value:
```

### Comparing `xsdata-23.5/xsdata/formats/dataclass/serializers/writers/__init__.py` & `xsdata-23.6/xsdata/formats/dataclass/serializers/writers/__init__.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/formats/dataclass/serializers/writers/lxml.py` & `xsdata-23.6/xsdata/formats/dataclass/serializers/writers/lxml.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/formats/dataclass/serializers/writers/native.py` & `xsdata-23.6/xsdata/formats/dataclass/serializers/writers/native.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/formats/dataclass/serializers/xml.py` & `xsdata-23.6/xsdata/formats/dataclass/serializers/xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,15 +377,16 @@
         Return the attribute variables with their object values if set and not
         empty iterables.
 
         :param obj: Input object
         :param meta: Object metadata
         :param nillable: Is model nillable
         :param xsi_type: The true xsi:type of the object
-        :param ignore_optionals: Skip optional attributes with default value
+        :param ignore_optionals: Skip optional attributes with default
+            value
         :return:
         """
         for var in meta.get_attribute_vars():
             if var.is_attribute:
                 value = getattr(obj, var.name)
                 if (
                     value is None
```

### Comparing `xsdata-23.5/xsdata/formats/dataclass/templates/class.jinja2` & `xsdata-23.6/xsdata/formats/dataclass/templates/class.jinja2`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 {% set level = level|default(0) -%}
 {% set help | format_docstring(level + 1) %}
     {%- include "docstrings." + docstring_name + ".jinja2" -%}
 {% endset -%}
 {% set parent_namespace = obj.namespace if obj.namespace is not none else parent_namespace|default(None) -%}
 {% set parents = parents|default([obj.name]) -%}
 {% set class_name =  obj.name|class_name -%}
+{% set class_annotations =  obj | class_annotations(class_name) -%}
 {% set global_type = level == 0 and not obj.local_type -%}
 {% set local_name =  obj.meta_name or obj.name -%}
 {% set local_name = None if class_name == local_name or not global_type else local_name -%}
-{% set base_classes = obj.extensions|map(attribute='type')|map('type_name')|join(', ') -%}
+{% set base_classes = obj | class_bases(class_name) | join(', ')-%}
 {% set target_namespace = obj.target_namespace if global_type and module_namespace != obj.target_namespace else None %}
 
-{{ class_annotation }}
+{{ class_annotations | join('\n') }}
 class {{ class_name }}{{"({})".format(base_classes) if base_classes }}:
 {%- if help %}
 {{ help|indent(4, first=True) }}
 {%- endif -%}
 {%- if local_name or obj.is_nillable or obj.namespace is not none or target_namespace or obj.local_type %}
     class Meta:
         {%- if obj.local_type %}
```

### Comparing `xsdata-23.5/xsdata/formats/dataclass/templates/enum.jinja2` & `xsdata-23.6/xsdata/formats/dataclass/templates/enum.jinja2`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/formats/dataclass/transports.py` & `xsdata-23.6/xsdata/formats/dataclass/transports.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import abc
 from typing import Any
 from typing import Dict
+from typing import Optional
 
-import requests
+from requests import Response
+from requests import Session
 
 
 class Transport(abc.ABC):
     __slots__ = ()
 
     @abc.abstractmethod
     def get(self, url: str, params: Dict, headers: Dict) -> bytes:
@@ -20,35 +22,38 @@
 class DefaultTransport(Transport):
     """
     Default transport based on the requests library.
 
     :param timeout: Read timeout
     """
 
-    __slots__ = "timeout"
+    __slots__ = "timeout", "session"
 
-    def __init__(self, timeout: float = 2.0):
+    def __init__(self, timeout: float = 2.0, session: Optional[Session] = None):
         self.timeout = timeout
+        self.session = session or Session()
 
     def get(self, url: str, params: Dict, headers: Dict) -> bytes:
         """
         :raises HTTPError: if status code is not valid for content unmarshalling.
         """
-        res = requests.get(url, params=params, headers=headers, timeout=self.timeout)
+        res = self.session.get(
+            url, params=params, headers=headers, timeout=self.timeout
+        )
         return self.handle_response(res)
 
     def post(self, url: str, data: Any, headers: Dict) -> Any:
         """
         :raises HTTPError: if status code is not valid for content unmarshalling.
         """
-        res = requests.post(url, data=data, headers=headers, timeout=self.timeout)
+        res = self.session.post(url, data=data, headers=headers, timeout=self.timeout)
         return self.handle_response(res)
 
     @classmethod
-    def handle_response(cls, response: requests.Response) -> bytes:
+    def handle_response(cls, response: Response) -> bytes:
         """
         Status codes 200 or 500 means that we can unmarshall the response.
 
         :raises HTTPError: If the response status code is not 200 or 500
         """
         if response.status_code not in (200, 500):
             response.raise_for_status()
```

### Comparing `xsdata-23.5/xsdata/formats/dataclass/typing.py` & `xsdata-23.6/xsdata/formats/dataclass/typing.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,78 @@
-from typing import _eval_type  # type: ignore
+import sys
 from typing import Any
-from typing import Dict
 from typing import Iterator
-from typing import List
-from typing import Optional
 from typing import Tuple
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
-NONE_TYPE = type(None)
-EMPTY_ARGS = ()
+from typing_extensions import get_args
+from typing_extensions import get_origin
 
+NONE_TYPE = type(None)
 
-def get_origin(tp: Any) -> Any:
-    if tp is Dict:
-        return Dict
 
-    if tp in (Tuple, List, Union):
-        raise TypeError()
+try:
+    from types import UnionType  # type: ignore
+except ImportError:
+    UnionType = ()  # type: ignore
 
-    if isinstance(tp, TypeVar):
-        return TypeVar
 
-    origin = getattr(tp, "__origin__", None)
-    if origin:
-        if origin in (list, List):
-            return List
+if (3, 9) <= sys.version_info[:2] <= (3, 10):
+    # Backport this fix for python 3.9 and 3.10
+    # https://github.com/python/cpython/pull/30900
 
-        if origin in (tuple, Tuple):
-            return Tuple
+    from types import GenericAlias
+    from typing import ForwardRef
+    from typing import _eval_type as __eval_type  # type: ignore
 
-        if origin in (dict, Dict):
-            return Dict
+    def _eval_type(tp: Any, globalns: Any, localns: Any) -> Any:
+        if isinstance(tp, GenericAlias):
+            args = tuple(
+                ForwardRef(arg) if isinstance(arg, str) else arg for arg in tp.__args__
+            )
+            tp = tp.__origin__[args]  # type: ignore
 
-        if origin is Union:
-            return Union
+        return __eval_type(tp, globalns, localns)
 
-        if origin in (type, Type):
-            return Type
+else:
+    from typing import _eval_type  # type: ignore
 
-    if origin or str(tp).startswith("typing."):
-        raise TypeError()
 
-    return None
+intern_typing = sys.intern("typing.")
 
 
-def get_args(tp: Any) -> Tuple:
-    return getattr(tp, "__args__", EMPTY_ARGS) or EMPTY_ARGS
+def is_from_typing(tp: Any) -> bool:
+    return str(tp).startswith(intern_typing)
 
 
 def evaluate(
-    tp: Any, globalns: Optional[Any] = None, localns: Optional[Any] = None
+    tp: Any,
+    globalns: Any = None,
+    localns: Any = None,
 ) -> Tuple[Type, ...]:
     return tuple(_evaluate(_eval_type(tp, globalns, localns)))
 
 
 def _evaluate(tp: Any) -> Iterator[Type]:
-    origin = get_origin(tp)
+    if tp in (dict, list, tuple):
+        origin = tp
+    elif isinstance(tp, TypeVar):
+        origin = TypeVar
+    else:
+        origin = get_origin(tp)
 
-    func = __evaluations__.get(origin)
-    if func:
-        yield from func(tp)
+    if origin:
+        try:
+            yield from __evaluations__[origin](tp)
+        except KeyError:
+            raise TypeError()
+    elif is_from_typing(tp):
+        raise TypeError()
     else:
         yield tp
 
 
 def _evaluate_type(tp: Any) -> Iterator[Type]:
     args = get_args(tp)
     if not args or isinstance(args[0], TypeVar):
@@ -78,87 +85,97 @@
     args = get_args(tp)
 
     if not args:
         yield str
         yield str
 
     for arg in args:
-        origin = get_origin(arg)
-        if origin is TypeVar:
+        if isinstance(arg, TypeVar):
             try:
                 next(_evaluate_typevar(arg))
             except TypeError:
                 yield str
             else:
                 raise TypeError()
-        elif origin is not None:
+        elif is_from_typing(arg) or get_origin(arg) is not None:
             raise TypeError()
         else:
             yield arg
 
 
 def _evaluate_list(tp: Any) -> Iterator[Type]:
     yield list
 
     args = get_args(tp)
+    if not args:
+        yield str
+
     for arg in args:
+        yield from _evaluate_array_arg(arg)
+
+
+def _evaluate_array_arg(arg: Any) -> Iterator[Type]:
+    if isinstance(arg, TypeVar):
+        yield from _evaluate_typevar(arg)
+    else:
         origin = get_origin(arg)
 
-        if origin is None:
+        if origin is None and not is_from_typing(arg):
             yield arg
-        elif origin in (Union, List, Tuple, TypeVar):
+        elif origin in (Union, UnionType, list, tuple):
             yield from __evaluations__[origin](arg)
         else:
             raise TypeError()
 
 
 def _evaluate_tuple(tp: Any) -> Iterator[Type]:
     yield tuple
 
     args = get_args(tp)
+    if not args:
+        yield str
+
     for arg in args:
         if arg is Ellipsis:
             continue
 
-        origin = get_origin(arg)
-        if origin is None:
-            yield arg
-        elif origin in (Union, List, Tuple, TypeVar):
-            yield from __evaluations__[origin](arg)
-        else:
-            raise TypeError()
+        yield from _evaluate_array_arg(arg)
 
 
 def _evaluate_union(tp: Any) -> Iterator[Type]:
     origin_locked = False
     for arg in get_args(tp):
         if arg is NONE_TYPE:
             continue
 
-        origin = get_origin(arg)
-        if origin is None:
-            yield arg
-        elif origin is List and not origin_locked:
-            yield from _evaluate_list(arg)
-            origin_locked = True
+        if isinstance(arg, TypeVar):
+            yield from _evaluate_typevar(arg)
         else:
-            raise TypeError()
+            origin = get_origin(arg)
+            if origin is list and not origin_locked:
+                yield from _evaluate_list(arg)
+                origin_locked = True
+            elif origin is None and not is_from_typing(arg):
+                yield arg
+            else:
+                raise TypeError()
 
 
 def _evaluate_typevar(tp: TypeVar):
     if tp.__bound__:
         yield from _evaluate(tp.__bound__)
     elif tp.__constraints__:
         for arg in tp.__constraints__:
             yield from _evaluate(arg)
     else:
         raise TypeError()
 
 
 __evaluations__ = {
-    Tuple: _evaluate_tuple,
-    List: _evaluate_list,
-    Dict: _evaluate_mapping,
+    tuple: _evaluate_tuple,
+    list: _evaluate_list,
+    dict: _evaluate_mapping,
     Union: _evaluate_union,
-    Type: _evaluate_type,
+    UnionType: _evaluate_union,
+    type: _evaluate_type,
     TypeVar: _evaluate_typevar,
 }
```

### Comparing `xsdata-23.5/xsdata/formats/mixins.py` & `xsdata-23.6/xsdata/formats/mixins.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/models/config.py` & `xsdata-23.6/xsdata/models/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+import re
 import sys
 import warnings
 from dataclasses import dataclass
+from dataclasses import field
 from enum import Enum
 from pathlib import Path
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import Pattern
 from typing import TextIO
 
 from xsdata import __version__
 from xsdata.exceptions import CodeGenerationWarning
 from xsdata.exceptions import GeneratorConfigError
 from xsdata.formats.dataclass.context import XmlContext
 from xsdata.formats.dataclass.parsers import XmlParser
@@ -161,27 +164,42 @@
 
     CLASS = "class"
     FIELD = "field"
     MODULE = "module"
     PACKAGE = "package"
 
 
+class ExtensionType(Enum):
+    """
+    Extension type enumeration.
+
+    :cvar CLASS: class
+    :cvar DECORATOR: decorator
+    """
+
+    CLASS = "class"
+    DECORATOR = "decorator"
+
+
 @dataclass
 class OutputFormat:
     """
     Output format options.
 
     :param value: Output format name, default: dataclasses
     :param repr: Generate __repr__ method, default: true
     :param eq: Generate __eq__ method, default: true
-    :param order: Generate  __lt__, __le__, __gt__, and __ge__ methods, default: false
-    :param unsafe_hash: Generate __hash__ method if not frozen, default: false
+    :param order: Generate __lt__, __le__, __gt__, and __ge__ methods,
+        default: false
+    :param unsafe_hash: Generate __hash__ method if not frozen, default:
+        false
     :param frozen: Enable read only properties, default false
     :param slots: Enable __slots__, default: false, python>=3.10 Only
-    :param kw_only: Enable keyword only arguments, default: false, python>=3.10 Only
+    :param kw_only: Enable keyword only arguments, default: false,
+        python>=3.10 Only
     """
 
     value: str = text_node(default="dataclasses", cli="output")
     repr: bool = attribute(default=True)
     eq: bool = attribute(default=True)
     order: bool = attribute(default=False)
     unsafe_hash: bool = attribute(default=False)
@@ -213,19 +231,21 @@
 
 
 @dataclass
 class CompoundFields:
     """
     Compound fields options.
 
-    :param enabled: Use compound fields for repeatable elements, default: false
+    :param enabled: Use compound fields for repeatable elements,
+        default: false
     :param default_name: Default compound field name, default: choice
-    :param force_default_name: Always use the default compound field, otherwise
-        if the number of elements is less than 4 the generator will try to dynamically
-        create the field name eg. hat_or_dress_or_something.
+    :param force_default_name: Always use the default compound field,
+        otherwise if the number of elements is less than 4 the generator
+        will try to dynamically create the field name eg.
+        hat_or_dress_or_something.
     """
 
     enabled: bool = text_node(default=False, cli="compound-fields")
     default_name: str = attribute(default="choice", cli=False)
     force_default_name: bool = attribute(default=False, cli=False)
 
 
@@ -236,16 +256,20 @@
 
     :param package: Target package, default: generated
     :param format: Output format
     :param structure_style: Output structure style, default: filenames
     :param docstring_style: Docstring style, default: reStructuredText
     :param filter_strategy: Class filter strategy, default: globals
     :param relative_imports: Use relative imports, default: false
-    :param compound_fields: Use compound fields for repeatable elements, default: false
+    :param compound_fields: Use compound fields for repeatable elements,
+        default: false
     :param max_line_length: Adjust the maximum line length, default: 79
+    :param subscriptable_types: Use PEP-585 generics for standard collections,
+        default: false, python>=3.9 Only
+    :param union_type: Use PEP-604 union type, default: false, python>=3.10 Only
     :param postponed_annotations: Enable postponed evaluation of annotations,
         default: false, python>=3.7 Only
     :param unnest_classes: Move inner classes to upper level, default: false
     :param ignore_patterns: Ignore pattern restrictions, default: false
     :param include_header: Include a header with codegen information in the output,
         default: false
     """
@@ -258,19 +282,46 @@
     docstring_style: DocstringStyle = element(default=DocstringStyle.RST)
     filter_strategy: ClassFilterStrategy = element(
         default=ClassFilterStrategy.ALL_GLOBALS
     )
     relative_imports: bool = element(default=False)
     compound_fields: CompoundFields = element(default_factory=CompoundFields)
     max_line_length: int = attribute(default=79)
+    subscriptable_types: bool = attribute(default=False)
+    union_type: bool = attribute(default=False)
     postponed_annotations: bool = element(default=False)
     unnest_classes: bool = element(default=False)
     ignore_patterns: bool = element(default=False)
     include_header: bool = element(default=False)
 
+    def __post_init__(self):
+        self.validate()
+
+    def validate(self):
+        if self.subscriptable_types and sys.version_info < (3, 9):
+            self.subscriptable_types = False
+            warnings.warn(
+                "Generics PEP 585 requires python >= 3.9, reverting...",
+                CodeGenerationWarning,
+            )
+
+        if self.union_type and sys.version_info < (3, 10):
+            self.union_type = False
+            warnings.warn(
+                "UnionType PEP 604 requires python >= 3.10, reverting...",
+                CodeGenerationWarning,
+            )
+
+        if self.union_type and not self.postponed_annotations:
+            self.postponed_annotations = True
+            warnings.warn(
+                "Enabling postponed annotations, because `union_type==True`",
+                CodeGenerationWarning,
+            )
+
     def update(self, **kwargs: Any):
         objects.update(self, **kwargs)
         self.format.validate()
 
 
 @dataclass
 class NameConvention:
@@ -372,14 +423,62 @@
 
     type: ObjectType = attribute(required=True)
     search: str = attribute(required=True)
     replace: str = attribute(required=True)
 
 
 @dataclass
+class GeneratorExtension:
+    """
+    Add decorators or base classes on the generated classes that match the
+    class name pattern.
+
+    :param type: The extension type
+    :param class_name: The class name or a pattern to apply the
+        extension
+    :param import_string: The import string of the extension type
+    :param prepend: Prepend or append decorator or base class
+    :param apply_if_derived: Apply or skip if the class is already a
+        subclass
+    """
+
+    type: ExtensionType = attribute(required=True)
+    class_name: str = attribute(required=True, name="class")
+    import_string: str = attribute(required=True, name="import")
+    prepend: bool = attribute(default=False)
+    apply_if_derived: bool = attribute(default=False, name="applyIfDerived")
+
+    module_path: str = field(
+        init=False,
+        metadata={"type": "Ignore"},
+    )
+    func_name: str = field(
+        init=False,
+        metadata={"type": "Ignore"},
+    )
+    pattern: Pattern = field(
+        init=False,
+        metadata={"type": "Ignore"},
+    )
+
+    def __post_init__(self):
+        try:
+            self.module_path, self.func_name = self.import_string.rsplit(".", 1)
+        except (ValueError, AttributeError):
+            raise GeneratorConfigError(
+                f"Invalid extension import '{self.import_string}'"
+            )
+
+        try:
+            self.pattern = re.compile(self.class_name)
+        except re.error:
+            raise GeneratorConfigError(f"Failed to compile pattern '{self.class_name}'")
+
+
+@dataclass
 class GeneratorSubstitutions:
     """
     Generator search and replace substitutions for classes, fields, packages
     and modules names. The process runs before and after the default naming
     conventions.
 
     .. warning:: The generator doesn't validate substitutions.
@@ -387,37 +486,55 @@
     :param substitution: The list of substitutions
     """
 
     substitution: List[GeneratorSubstitution] = array_element()
 
 
 @dataclass
+class GeneratorExtensions:
+    """
+    Generator extensions for classes. The process runs after the default naming
+    conventions.
+
+    .. warning:: The generator doesn't validate imports!
+
+    :param extension: The list of extensions
+    """
+
+    extension: List[GeneratorExtension] = array_element()
+
+
+@dataclass
 class GeneratorConfig:
     """
     Generator configuration binding model.
 
     :cvar version: xsdata version number the config was created/updated
     :param output: Output options
     :param conventions: Generator conventions
-    :param aliases: Generator aliases, Deprecated since v21.12, use substitutions
-    :param substitutions: Generator search and replace substitutions for classes,
-        fields, packages and modules names.
+    :param aliases: Generator aliases, Deprecated since v21.12, use
+        substitutions
+    :param substitutions: Generator search and replace substitutions for
+        classes, fields, packages and modules names.
+    :param extensions: Generator custom base classes and decorators for
+        classes.
     """
 
     class Meta:
         name = "Config"
         namespace = "http://pypi.org/project/xsdata"
 
     version: str = attribute(init=False, default=__version__)
     output: GeneratorOutput = element(default_factory=GeneratorOutput)
     conventions: GeneratorConventions = element(default_factory=GeneratorConventions)
     aliases: Optional[GeneratorAliases] = element(default=None)
     substitutions: GeneratorSubstitutions = element(
         default_factory=GeneratorSubstitutions
     )
+    extensions: GeneratorExtensions = element(default_factory=GeneratorExtensions)
 
     def __post_init__(self):
         if self.aliases:
             alias_map = {
                 ObjectType.CLASS: self.aliases.class_name,
                 ObjectType.FIELD: self.aliases.field_name,
                 ObjectType.PACKAGE: self.aliases.package_name,
```

### Comparing `xsdata-23.5/xsdata/models/datatype.py` & `xsdata-23.6/xsdata/models/datatype.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,16 @@
 
     Represents iso 8601 date format [-]CCYY-MM-DD[Z|(+|-)hh:mm] with
     rich comparisons and hashing.
 
     :param year: Any signed integer, eg (0, -535, 2020)
     :param month: Unsigned integer between 1-12
     :param day: Unsigned integer between 1-31
-    :param offset: Signed integer representing timezone offset in minutes
+    :param offset: Signed integer representing timezone offset in
+        minutes
     """
 
     year: int
     month: int
     day: int
     offset: Optional[int] = None
 
@@ -91,15 +92,15 @@
     @classmethod
     def from_date(cls, obj: datetime.date) -> "XmlDate":
         """
         Initialize from :class:`datetime.date` instance.
 
         .. warning::
 
-        date instances don't have timezone information!
+            date instances don't have timezone information!
         """
         return cls(obj.year, obj.month, obj.day)
 
     @classmethod
     def from_datetime(cls, obj: datetime.datetime) -> "XmlDate":
         """Initialize from :class:`datetime.datetime` instance."""
         return cls(obj.year, obj.month, obj.day, calculate_offset(obj))
@@ -137,17 +138,16 @@
         return f"{self.__class__.__qualname__}({', '.join(map(str, args))})"
 
 
 class XmlDateTime(NamedTuple):
     """
     Concrete xs:dateTime builtin type.
 
-    Represents iso 8601 date time format [-]CCYY-MM-DDThh:mm:ss[Z|(+|-)hh:mm]
-    with rich comparisons and hashing.
-
+    Represents iso 8601 date time format [-]CCYY-MM-DDThh
+    :mm: ss[Z|(+|-)hh:mm] with rich comparisons and hashing.
     :param year: Any signed integer, eg (0, -535, 2020)
     :param month: Unsigned integer between 1-12
     :param day: Unsigned integer between 1-31
     :param hour: Unsigned integer between 0-24
     :param minute: Unsigned integer between 0-59
     :param second: Unsigned integer between 0-59
     :param fractional_second: Unsigned integer between 0-999999999
@@ -326,22 +326,22 @@
         return cmp(self, other, operator.ge)
 
 
 class XmlTime(NamedTuple):
     """
     Concrete xs:time builtin type.
 
-    Represents iso 8601 time format hh:mm:ss[Z|(+|-)hh:mm]
-    with rich comparisons and hashing.
-
+    Represents iso 8601 time format hh
+    :mm: ss[Z|(+|-)hh:mm] with rich comparisons and hashing.
     :param hour: Unsigned integer between 0-24
     :param minute: Unsigned integer between 0-59
     :param second: Unsigned integer between 0-59
     :param fractional_second: Unsigned integer between 0-999999999
-    :param offset: Signed integer representing timezone offset in minutes
+    :param offset: Signed integer representing timezone offset in
+        minutes
     """
 
     hour: int
     minute: int
     second: int
     fractional_second: int = 0
     offset: Optional[int] = None
```

### Comparing `xsdata-23.5/xsdata/models/dtd.py` & `xsdata-23.6/xsdata/models/dtd.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/models/enums.py` & `xsdata-23.6/xsdata/models/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,17 +67,19 @@
 
 
 class NamespaceType:
     """
     Wildcard elements/attributes namespace types.
 
     :cvar ANY_NS: elements from any namespace is allowed
-    :cvar OTHER_NS: elements from any namespace except the parent element's namespace
+    :cvar OTHER_NS: elements from any namespace except the parent
+        element's namespace
     :cvar LOCAL_NS: elements must come from no namespace
-    :cvar TARGET_NS: elements from the namespace of the parent element can be present
+    :cvar TARGET_NS: elements from the namespace of the parent element
+        can be present
     """
 
     ANY_NS = "##any"
     OTHER_NS = "##other"
     LOCAL_NS = "##local"
     TARGET_NS = "##targetNamespace"
```

### Comparing `xsdata-23.5/xsdata/models/mixins.py` & `xsdata-23.6/xsdata/models/mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,16 @@
 
     @property
     def real_name(self) -> str:
         """
         Return the real name for this element by looking by looking either to
         the name or ref attribute value.
 
-        :raises SchemaValueError: when instance has no name/ref attribute.
+        :raises SchemaValueError: when instance has no name/ref
+            attribute.
         """
         name = getattr(self, "name", None) or getattr(self, "ref", None)
         if name:
             return text.suffix(name)
 
         raise SchemaValueError(f"Schema class `{self.class_name}` unknown real name.")
```

### Comparing `xsdata-23.5/xsdata/models/wsdl.py` & `xsdata-23.6/xsdata/models/wsdl.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/models/xsd.py` & `xsdata-23.6/xsdata/models/xsd.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,16 @@
 
 
 @dataclass
 class AnyAttribute(AnnotationBase):
     """
     Model representation of a schema xs:anyAttribute element.
 
-    :param namespace: ##any | ##other) | List of anyURI | (##targetNamespace | ##local)
+    :param namespace: ##any | ##other) | List of anyURI |
+        (##targetNamespace | ##local)
     :param process_contents: (lax | skip | strict) : strict
     """
 
     namespace: str = attribute(default="##any")
     process_contents: Optional[ProcessType] = attribute(name="processContents")
 
     def __post_init__(self):
@@ -1058,15 +1059,16 @@
     :param name: NCName
     :param ref: QName
     :param type: QName
     :param substitution_group: List of QName
     :param default:
     :param fixed:
     :param form: qualified | unqualified
-    :param block: (#all | List of (extension | restriction | substitution))
+    :param block: (#all | List of (extension | restriction |
+        substitution))
     :param final: (#all | List of (extension | restriction))
     :param target_namespace: anyURI
     :param simple_type:
     :param complex_type:
     :param alternatives:
     :param uniques:
     :param keys:
@@ -1167,15 +1169,16 @@
 
 @dataclass
 class SchemaLocation(AnnotationBase):
     """
     Model representation of a schema xs:schemaLocation element. Base schema
     location.
 
-    :param location: any url with a urllib supported scheme file: http:
+    :param location: any url with a urllib supported scheme file
+    : http:
     """
 
     location: Optional[str] = field(default=None)
 
 
 @dataclass
 class Import(SchemaLocation):
@@ -1247,22 +1250,25 @@
 
 @dataclass
 class Schema(SchemaLocation):
     """
     Model representation of a schema xs:schema element.
 
     :param target:
-    :param block_default: (#all | List of (extension | restriction | substitution))
+    :param block_default: (#all | List of (extension | restriction |
+        substitution))
     :param default_attributes: QName
-    :param final_default: (#all | List of extension | restriction | list | union) : ''
+    :param final_default: (#all | List of extension | restriction | list
+        | union) : ''
     :param target_namespace: anyURI
     :param version: token
     :param xmlns:
     :param element_form_default: (qualified | unqualified) : unqualified
-    :param attribute_form_default:  (qualified | unqualified) : unqualified
+    :param attribute_form_default: (qualified | unqualified) :
+        unqualified
     :param default_open_content:
     :param imports:
     :param redefines:
     :param overrides:
     :param annotations:
     :param simple_types:
     :param complex_types:
```

### Comparing `xsdata-23.5/xsdata/schemas/mathml3-common.xsd` & `xsdata-23.6/xsdata/schemas/mathml3-common.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/schemas/mathml3-content.xsd` & `xsdata-23.6/xsdata/schemas/mathml3-content.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/schemas/mathml3-presentation.xsd` & `xsdata-23.6/xsdata/schemas/mathml3-presentation.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/schemas/mathml3-strict-content.xsd` & `xsdata-23.6/xsdata/schemas/mathml3-strict-content.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/schemas/xlink.xsd` & `xsdata-23.6/xsdata/schemas/xlink.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/schemas/xml.xsd` & `xsdata-23.6/xsdata/schemas/xml.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/utils/click.py` & `xsdata-23.6/xsdata/utils/click.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/utils/collections.py` & `xsdata-23.6/xsdata/utils/collections.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/utils/dates.py` & `xsdata-23.6/xsdata/utils/dates.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/utils/debug.py` & `xsdata-23.6/xsdata/utils/debug.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/utils/downloader.py` & `xsdata-23.6/xsdata/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/utils/graphs.py` & `xsdata-23.6/xsdata/utils/graphs.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from typing import Set
 
 
 def strongly_connected_components(edges: Dict[str, List[str]]) -> Iterator[Set[str]]:
     """
     Compute Strongly Connected Components of a directed graph.
 
-    From https://code.activestate.com/recipes/578507/
-    From https://github.com/python/mypy/blob/master/mypy/build.py
+    From https://code.activestate.com/recipes/578507/ From
+    https://github.com/python/mypy/blob/master/mypy/build.py
 
     :param edges: Mapping of vertex-edges values
     """
     identified: Set[str] = set()
     stack: List[str] = []
     index: Dict[str, int] = {}
     boundaries: List[int] = []
```

### Comparing `xsdata-23.5/xsdata/utils/namespaces.py` & `xsdata-23.6/xsdata/utils/namespaces.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/utils/objects.py` & `xsdata-23.6/xsdata/utils/objects.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/utils/package.py` & `xsdata-23.6/xsdata/utils/package.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/utils/testing.py` & `xsdata-23.6/xsdata/utils/testing.py`

 * *Files identical despite different names*

### Comparing `xsdata-23.5/xsdata/utils/text.py` & `xsdata-23.6/xsdata/utils/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     "or",
     "pass",
     "raise",
     "return",
     "self",
     "str",
     "try",
+    "type",
     "while",
     "with",
     "yield",
 }
 
 is_reserved = stop_words.__contains__
```

### Comparing `xsdata-23.5/xsdata.egg-info/SOURCES.txt` & `xsdata-23.6/xsdata.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 CHANGES.rst
 LICENSE
 MANIFEST.in
 README.rst
-setup.cfg
-setup.py
-tox.ini
+pyproject.toml
 docs/Makefile
 docs/__init__.py
 docs/api.rst
 docs/changelog.rst
 docs/codegen.rst
 docs/conf.py
 docs/data-types-table.rst
@@ -42,14 +40,15 @@
 docs/examples/compound-fields.rst
 docs/examples/custom-class-factory.rst
 docs/examples/custom-property-names.rst
 docs/examples/custom-type-mapping.rst
 docs/examples/dataclasses-features.rst
 docs/examples/docstrings.rst
 docs/examples/dtd-modeling.rst
+docs/examples/extending-models.rst
 docs/examples/json-modeling.rst
 docs/examples/pycode-serializer.rst
 docs/examples/samples.rst
 docs/examples/w3c-suite.rst
 docs/examples/working-with-wildcards.rst
 docs/examples/wrapped-list.rst
 docs/examples/xml-modeling.rst
```

