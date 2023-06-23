# Comparing `tmp/neoaccess-4.2.0.tar.gz` & `tmp/neoaccess-4.3.1.tar.gz`

## Comparing `neoaccess-4.2.0.tar` & `neoaccess-4.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1092 2020-02-02 00:00:00.000000 neoaccess-4.2.0/LICENSE.txt
--rwxr-xr-x   0        0        0      242 2020-02-02 00:00:00.000000 neoaccess-4.2.0/README.md
--rwxr-xr-x   0        0        0      975 2020-02-02 00:00:00.000000 neoaccess-4.2.0/pyproject.toml
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 neoaccess-4.2.0/src/neoaccess/__init__.py
--rwxr-xr-x   0        0        0    24237 2020-02-02 00:00:00.000000 neoaccess-4.2.0/src/neoaccess/cypher_utils.py
--rwxr-xr-x   0        0        0   160376 2020-02-02 00:00:00.000000 neoaccess-4.2.0/src/neoaccess/neoaccess.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 neoaccess-4.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1092 2020-02-02 00:00:00.000000 neoaccess-4.3.1/LICENSE.txt
+-rwxr-xr-x   0        0        0      421 2020-02-02 00:00:00.000000 neoaccess-4.3.1/README.md
+-rwxr-xr-x   0        0        0      975 2020-02-02 00:00:00.000000 neoaccess-4.3.1/pyproject.toml
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 neoaccess-4.3.1/src/neoaccess/__init__.py
+-rwxr-xr-x   0        0        0    28230 2020-02-02 00:00:00.000000 neoaccess-4.3.1/src/neoaccess/cypher_utils.py
+-rwxr-xr-x   0        0        0   158618 2020-02-02 00:00:00.000000 neoaccess-4.3.1/src/neoaccess/neoaccess.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 neoaccess-4.3.1/PKG-INFO
```

### Comparing `neoaccess-4.2.0/LICENSE.txt` & `neoaccess-4.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neoaccess-4.2.0/pyproject.toml` & `neoaccess-4.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "neoaccess"
-version = "4.2.0"
+version = "4.3.1"
 authors = [
   { name = "Julian West BrainAnnex.org" },
 ]
 maintainers = [
   { email = "julian@brainannex.org" },
 ]
 description = "High-level interface to the Neo4j graph database"
```

### Comparing `neoaccess-4.2.0/src/neoaccess/cypher_utils.py` & `neoaccess-4.3.1/src/neoaccess/cypher_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,105 +1,223 @@
+# This file contains 3 helper classes for the NeoAccess library:
+#       - NodeSpecs         To store the specs to identify one or more nodes (the "RAW match structure")
+#       - CypherMatch       To store Cypher fragments & data-binding dict, to identify one or more nodes (the "PROCESSED match structure")
+#       - CypherUtils       Static class to pre-process node specs, plus misc. Cypher-related utilities
+
 from typing import Union
 
 
-class CypherUtils:
+
+class NodeSpecs:
     """
     Helper class for the class "NeoAccess".
-
-    Most of it, is used for node-matching utilizing the "processed match structure", defined below.
-
     Meant as a PRIVATE class for NeoAccess; not indicated for the end user.
-
-    A "processed match structure" (a dict) is used to facilitate for a user to specify a node in a wide variety of way - and
-    save those specifications, in a "pre-digested" way, to use as needed in Cypher queries.
-    It is a Python dictionary with UP TO the following 4 keys (not all are necessarily present):
-
-            1) "node": a string, defining a node in a Cypher query, *excluding* the "MATCH" keyword
-            2) "where": a string, defining the "WHERE" part of the subquery (*excluding* the "WHERE"), if applicable;
-                        otherwise, a blank
-            3) "data_binding": a (possibly empty) data-binding dictionary
-            4) "dummy_node_name": a string used for the node name inside the Cypher query (by default, "n");
-                                  potentially relevant to the "node" and "where" values
-
-
-        EXAMPLES:
-            *   {"node": "(n  )" , "where": "" , "data_binding": {}, "dummy_node_name": "n"}
-            *   {"node": "(p :`person` )" , "where": "" , "data_binding": {}, "dummy_node_name": "p"}
-            *   {"node": "(n  )" , "where": "id(n) = 123" , "data_binding": {}, "dummy_node_name": "n"}
-            *   {"node": "(n :`car`:`surplus inventory` )" ,
-                 "where": "" ,
-                 "data_binding": {},
-                 "dummy_node_name": "n"}
-            *   {"node": "(n :`person` {`gender`: $n_par_1, `age`: $n_par_2})",
-                 "where": "",
-                 "data_binding": {"n_par_1": "F", "n_par_2": 22},
-                 "dummy_node_name": "n"}
-            *   {"node": "(n :`person` {`gender`: $n_par_1, `age`: $n_par_2})",
-                 "where": "n.income > 90000 OR n.state = 'CA'",
-                 "data_binding": {"n_par_1": "F", "n_par_2": 22},
-                 "dummy_node_name": "n"}
-            *   {"node": "(n :`person` {`gender`: $n_par_1, `age`: $n_par_2})",
-                 "where": "n.income > $min_income",
-                 "data_binding": {"n_par_1": "F", "n_par_2": 22, "min_income": 90000},
-                 "dummy_node_name": "n"}
+    
+    Validates and stores all the passed specifications (the "RAW match structure"),
+    that are used to identify a node or group of nodes.
+
+    Note:   NO database operation is actually performed
+
+    IMPORTANT:  By our convention -
+                    if internal_id is provided, all other conditions are DISREGARDED;
+                    if it's missing, an implicit AND operation applies to all the specified conditions
+                (Regardless, all the passed data is stored in this object)
     """
 
-
-    @classmethod
-    def define_match(cls, labels=None, internal_id=None, key_name=None, key_value=None, properties=None, subquery=None,
-                     dummy_node_name="n") -> dict:
+    def __init__(self, internal_id=None,
+                 labels=None, key_name=None, key_value=None,
+                 properties=None,
+                 clause=None, clause_dummy_name="n"):
         """
-        Turn the set of specification into the MATCH part, and (if applicable) the WHERE part,
-        of a Cypher query (using the specified dummy variable name),
-        together with its data-binding dictionary.
+        ALL THE ARGUMENTS ARE OPTIONAL (no arguments at all means "match everything in the database")
 
-        The keywords "MATCH" and "WHERE" are *not* returned, to facilitate the assembly of larger Cypher queries
-        that involve multiple matches.
+        :param internal_id: An integer with the node's internal database ID.
+                                If specified, it will lead to all the remaining arguments being DISREGARDED (though saved)
 
-        ALL THE ARGUMENTS ARE OPTIONAL (no arguments at all means "match everything in the database")
         :param labels:      A string (or list/tuple of strings) specifying one or more Neo4j labels.
                                 (Note: blank spaces ARE allowed in the strings)
                                 EXAMPLES:  "cars"
-                                            ("cars", "vehicles")
-
-        :param internal_id:      An integer with the node's internal ID.
-                                If specified, it OVER-RIDES all the remaining arguments, except for the labels
+                                            ("cars", "powered vehicles")
+                            Note that if multiple labels are given, then only nodes possessing ALL of them will be matched;
+                            at present, there's no way to request an "OR" operation on labels
 
         :param key_name:    A string with the name of a node attribute; if provided, key_value must be present, too
         :param key_value:   The required value for the above key; if provided, key_name must be present, too
                                 Note: no requirement for the key to be primary
 
         :param properties:  A (possibly-empty) dictionary of property key/values pairs, indicating a condition to match.
                                 EXAMPLE: {"gender": "F", "age": 22}
 
-        :param subquery:    Either None, or a (possibly empty) string containing a Cypher subquery,
-                            or a pair/list (string, dict) containing a Cypher subquery and the data-binding dictionary for it.
+        :param clause:      Either None, OR a (possibly empty) string containing a Cypher subquery,
+                            OR a pair/list (string, dict) containing a Cypher subquery and the data-binding dictionary for it.
                             The Cypher subquery should refer to the node using the assigned dummy_node_name (by default, "n")
                                 IMPORTANT:  in the dictionary, don't use keys of the form "n_par_i",
                                             where n is the dummy node name and i is an integer,
                                             or an Exception will be raised - those names are for internal use only
                                 EXAMPLES:   "n.age < 25 AND n.income > 100000"
                                             ("n.weight < $max_weight", {"max_weight": 100})
 
-        :param dummy_node_name: A string with a name by which to refer to the node (by default, "n")
+        :param clause_dummy_name: A string with a name by which to refer to the nodes (by default, "n") in the clause;
+                                only used if a `clause` argument is passed (in the absence of a clause, it's stored as None)
+        """
+        # Validate all the passed arguments
+        if internal_id is not None:
+            assert CypherUtils.valid_internal_id(internal_id), \
+                f"NodeSpecs(): the argument `internal_id` ({internal_id}) is not a valid internal database ID value"
+
+        if labels is not None:
+            assert (type(labels) == str) or (type(labels) == list) or (type(labels) == tuple), \
+                f"NodeSpecs(): the argument `labels`, if provided, must be a string, or a list/tuple of strings"
 
-        :return:            A dictionary of data storing the parameters of the match.
-                            For details, see the info stored in the comments for this Class
+        if key_name is not None:
+            assert type(key_name) == str, \
+                f"NodeSpecs(): the argument `key_name`, if provided, must be a string"
+            assert key_value is not None, \
+                f"NodeSpecs(): if the argument `key_name` is provided, there must also be a `key_value` argument"
+
+        if properties is not None:
+            assert type(properties) == dict, \
+                f"NodeSpecs(): the argument `properties`, if provided, must be a python dictionary"
+
+        if clause is not None:
+            assert (type(clause) == str) or (type(clause) == list) or (type(clause) == tuple), \
+                f"NodeSpecs(): the argument `clause`, if provided, must be a string or a pair.  EXAMPLE: 'n.age > 21'"
+            if type(clause) != str:
+                assert len(clause) == 2, \
+                    f"NodeSpecs(): the argument `clause`, if provided as tuple or list, must have exactly 2 elements.  " \
+                    f"EXAMPLE: ('n.weight < $max_weight', {'max_weight': 100})"
+                    
+
+
+        if clause is None:
+            clause_dummy_name = None      # In this scenario, the dummy name isn't yet used, and any name could be used
+
+
+        # The following group of object variables can be thought of as
+        #   the "RAW match structure".  Any of the variables could be None
+        self.internal_id = internal_id
+        self.labels = labels
+        self.key_name = key_name
+        self.key_value = key_value
+        self.properties = properties
+        self.clause = clause
+        self.clause_dummy_name = clause_dummy_name
+
+
+
+    def __str__(self):
+        return f"RAW match structure:\n" \
+                f"    internal_id: {self.internal_id}" \
+                f"    labels: {self.labels}" \
+                f"    key_name: {self.key_name}" \
+                f"    key_value: {self.key_value}" \
+                f"    properties: {self.properties}" \
+                f"    clause: {self.clause}" \
+                f"    clause_dummy_name: {self.clause_dummy_name}"
+
+
+
+
+######################################################################################################################
+
+class CypherMatch:
+    """
+    Helper class for the class "NeoAccess".
+    Meant as a PRIVATE class for NeoAccess; not indicated for the end user.
+    
+    Objects of this class (sometimes referred to as a "PROCESSED match structures")
+    are used to facilitate for a user to specify a node in a wide variety of way - and
+    save those specifications, in a "pre-digested" way, to use as needed in Cypher queries.
+    
+    They store the following 4 properties:
+
+        1) "node":  a string, defining a node in a Cypher query, *excluding* the "MATCH" keyword
+        2) "where": a string, defining the "WHERE" part of the subquery (*excluding* the "WHERE"), if applicable;
+                    otherwise, a blank
+        3) "data_binding":      a (possibly empty) data-binding dictionary
+        4) "dummy_node_name":   a string used for the node name inside the Cypher query (by default, "n");
+                                potentially relevant to the "node" and "where" values
+
+        EXAMPLES:
+            *   node: "(n)"
+                    where: ""
+                    data_binding: {}
+                    dummy_node_name: "n"
+            *   node: "(p :`person` )"
+                    where: ""
+                    data_binding: {}
+                    dummy_node_name: "p"
+            *   node: "(n  )"
+                    where: "id(n) = 123"
+                    data_binding: {}
+                    dummy_node_name: "n"
+            *   node: "(n :`car`:`surplus inventory` )"
+                    where: ""
+                    data_binding: {}
+                    dummy_node_name: "n"
+            *    node: "(n :`person` {`gender`: $n_par_1, `age`: $n_par_2})"
+                    where: ""
+                    data_binding: {"n_par_1": "F", "n_par_2": 22}
+                    dummy_node_name: "n"
+            *   node: "(n :`person` {`gender`: $n_par_1, `age`: $n_par_2})"
+                    where: "n.income > 90000 OR n.state = 'CA'"
+                    data_binding: {"n_par_1": "F", "n_par_2": 22}
+                    dummy_node_name: "n"
+            *   node: "(n :`person` {`gender`: $n_par_1, `age`: $n_par_2})"
+                    where: "n.income > $min_income"
+                    data_binding: {"n_par_1": "F", "n_par_2": 22, "min_income": 90000}
+                    dummy_node_name: "n"
+    """
+    
+    def __init__(self, node_specs, dummy_node_name_if_missing=None):
         """
-        # Turn labels (string or list/tuple of strings) into a string suitable for inclusion into Cypher
-        cypher_labels = cls.prepare_labels(labels)     # EXAMPLES:     ":`patient`"
-        #               ":`CAR`:`INVENTORY`"
 
-        if internal_id is not None:      # If an internal node ID is specified, it over-rides all the other conditions
-            # CAUTION: internal_id might be 0 ; that's a valid Neo4j node ID
+
+        :param node_specs:                  Object of type "NodeSpecs"
+        :param dummy_node_name_if_missing:  String that will be used ONLY if the object passed to in node_specs
+                                                lacks that attribute
+        """
+        # If a value is already present in the raw match structure,
+        # it takes priority
+        if node_specs.clause_dummy_name is None:
+            dummy_node_name = dummy_node_name_if_missing
+        else:
+            dummy_node_name = node_specs.clause_dummy_name
+
+        assert dummy_node_name is not None, \
+                "The class `CypherMatch` cannot be instantiated with a missing dummy none name"
+
+
+        """
+        IMPORTANT:  By our convention -
+                if internal_id is provided, all other conditions are DISREGARDED;
+                if it's missing, an implicit AND operation applies to all the specified conditions
+        """
+        if node_specs.internal_id is not None:     # If an internal node ID is specified, it over-rides all the other conditions
+                                        # CAUTION: internal_id might be 0 ; that's a valid Neo4j node ID
             cypher_match = f"({dummy_node_name})"
-            cypher_where = f"id({dummy_node_name}) = {internal_id}"
-            return {"node": cypher_match, "where": cypher_where, "data_binding": {}, "dummy_node_name": dummy_node_name}
+            cypher_where = f"id({dummy_node_name}) = {node_specs.internal_id}"
+            self.node = cypher_match
+            self.where = cypher_where
+            self.data_binding = {}
+            self.dummy_node_name = dummy_node_name
+            return
+
 
 
+        # Turn labels (string or list/tuple of strings) into a string suitable for inclusion into Cypher
+        cypher_labels = CypherUtils.prepare_labels(node_specs.labels)       # EXAMPLES:     ":`patient`"
+                                                                            #               ":`CAR`:`INVENTORY`"
+
+        # Extract all the data from the "NodeSpecs" object
+        key_name=node_specs.key_name
+        key_value=node_specs.key_value
+        properties=node_specs.properties
+        subquery=node_specs.clause
+
         if key_name and key_value is None:  # CAUTION: key_value might legitimately be 0 or "" (hence the "is None")
             raise Exception("If key_name is specified, so must be key_value")
 
         if key_value and not key_name:
             raise Exception("If key_value is specified, so must be key_name")
 
 
@@ -138,15 +256,15 @@
             #
             #       EXAMPLE:
             #               properties: {"gender": "F", "year first met": 2003}
             #           will lead to:
             #               clause_from_properties = "{`gender`: $n_par_1, `year first met`: $n_par_2}"
             #               props_data_binding = {'n_par_1': "F", 'n_par_2': 2003}
 
-            (clause_from_properties, props_data_binding) = cls.dict_to_cypher(properties, prefix=dummy_node_name + "_par_")
+            (clause_from_properties, props_data_binding) = CypherUtils.dict_to_cypher(properties, prefix=dummy_node_name + "_par_")
 
             if not cypher_dict:
                 cypher_dict = props_data_binding        # The properties dictionary is to be used as the only Cypher-binding dictionary
             else:
                 # Merge the properties dictionary into the existing cypher_dict, PROVIDED that there's no conflict
                 overlap = cypher_dict.keys() & props_data_binding.keys()    # Take the set intersection
                 if overlap != set():                                        # If not equal to the empty set
@@ -158,186 +276,209 @@
 
         # Start constructing the Cypher string
         cypher_match = f"({dummy_node_name} {cypher_labels} {clause_from_properties})"
 
         if cypher_clause:
             cypher_clause = cypher_clause.strip()           # Zap any leading/trailing blanks
 
-        match_structure = {"node": cypher_match, "where": cypher_clause, "data_binding": cypher_dict, "dummy_node_name": dummy_node_name}
+        # Save all the processed data to be used for query parts to identify the node or nodes
+        self.node = cypher_match
+        self.where = cypher_clause
+        self.data_binding = cypher_dict
+        self.dummy_node_name = dummy_node_name
 
-        return match_structure
 
 
+    def __str__(self):
+        return f"CYPHER-PROCESSED match structure:\n" \
+               f"    node: {self.node}" \
+               f"    where: {self.where}" \
+               f"    data_binding: {self.data_binding}" \
+               f"    dummy_node_name: {self.dummy_node_name}"
 
-    @classmethod
-    def assert_valid_match_structure(cls, match: dict) -> None:
+
+
+    def extract_node(self) -> str:
         """
-        Verify that an alleged "match" dictionary is a valid one; if not, raise an Exception
-        TODO: tighten up the checks
+        Return the node information to be used in composing Cypher queries
 
-        :param match:   A dictionary of data to identify a node, or set of nodes, as returned by match()
-        :return:        None
+        :return:        A string with the node information, as needed by Cypher queries.  EXAMPLES:
+                            "(n  )"
+                            "(p :`person` )"
+                            "(n :`car`:`surplus inventory` )"
+                            "(n :`person` {`gender`: $n_par_1, `age`: $n_par_2})"
         """
-        assert type(match) == dict, f"`match` argument is not a dictionary as expected; instead, it is a {type(match)}"
+        return self.node
 
-        assert len(match) == 4, f"the `match` dictionary does not contain the expected 4 entries; instead, it has {len(match)}"
 
-        assert "node" in match, "the `match` dictionary does not contain the expected 'node' key"
-        assert "where" in match, "the `match` dictionary does not contain the expected 'where' key"
-        assert "data_binding" in match, "the `match` dictionary does not contain the expected 'data_binding' key"
-        assert "dummy_node_name" in match, "the `match` dictionary does not contain the expected 'dummy_node_name' key"
-
-        assert type(match["node"]) == str, "the `node` entry in the `match` dictionary is not a string, as expected"
-        assert type(match["where"]) == str, f"the `where` entry in the `match` dictionary is not a string, as expected; instead, it is {match['where']}"
-        assert type(match["data_binding"]) == dict, "the `data_binding` entry in the `match` dictionary is not a dictionary, as expected"
-        assert type(match["dummy_node_name"]) == str, "the `dummy_node_name` entry in the `match` dictionary is not a string, as expected"
+    def extract_dummy_name(self) -> str:
+        """
+        Return the dummy node _name to be used in composing Cypher queries
 
+        :return:        A string with the dummy node name (often "n" , or "to" , or "from")
+        """
+        return self.dummy_node_name
 
-    @classmethod
-    def assert_valid_internal_id(cls, internal_id: int) -> None:
+
+    def unpack_match(self) -> list:
         """
-        Raise an Exception if the argument is not a valid Neo4j internal database ID
+        Return a list containing:
+        [node, where, data_binding, dummy_node_name] ,
+        for use in composing Cypher queries
 
-        :param internal_id: Alleged Neo4j internal database ID
-        :return:            None
+        :return:                A list containing [node, where, data_binding, dummy_node_name]
         """
-        assert type(internal_id) == int, \
-            f"assert_valid_internal_id(): Neo4j internal ID's MUST be integers; the value passed ({internal_id}) was {type(internal_id)}"
+        match_as_list = [self.node, self.where , self.data_binding, self.dummy_node_name]
 
-        # Note that 0 is a valid Neo4j ID (apparently inconsistently assigned, on occasion, by the database)
-        assert internal_id >= 0, \
-            f"assert_valid_internal_id(): Neo4j internal ID's cannot be negative; the value passed was {internal_id}"
+        return match_as_list
 
 
 
-    @classmethod
-    def validate_internal_id(cls, internal_id: int) -> bool:    # TODO: maybe phase out in favor of assert_valid_internal_id()
+    def assert_valid_structure(self) -> None:
         """
-        Return True if internal_id is a valid ID as used internally by the database
-        (aka "Neo4j ID")
+        Verify that the object is a valid one (i.e., correctly initialized); if not, raise an Exception
+        TODO: NOT IN CURRENT USE.  Perhaps to phase out, or keep it but tighten its tests
 
-        :param internal_id:
-        :return:
+        :return:        None
         """
-        return (type(internal_id) == int) and (internal_id >= 0)
+        assert type(self.node) == str, "the `node` attribute is not a string, as expected"
+        assert type(self.where) == str, f"the `where` attribute is not a string, as expected; instead, it is {self.where}"
+        assert type(self.data_binding) == dict, "the `data_binding` attribute is not a dictionary, as expected"
+        assert type(self.dummy_node_name) == str, "the `dummy_node_name` attribute is not a string, as expected"
+
 
 
 
-    @classmethod
-    def process_match_structure(cls, handle: Union[int, dict], dummy_node_name="n") -> dict:
-        if cls.validate_internal_id(handle):
-            return cls.define_match(internal_id=handle, dummy_node_name=dummy_node_name)
-
-        if handle.get("dummy_node_name") is not None:
-            dummy_node_name = handle.get("dummy_node_name") # If a value is already present in the raw match structure,
-                                                            # it takes priority
-
-        return cls.define_match(internal_id=handle.get("internal_id"),
-                                labels=handle.get("labels"),
-                                key_name=handle.get("key_name"), key_value=handle.get("key_value"),
-                                properties=handle.get("properties"),
-                                subquery=handle.get("clause"),
-                                dummy_node_name=dummy_node_name)
 
+######################################################################################################################
+
+class CypherUtils:
+    """
+    Helper STATIC class for the class "NeoAccess".
+    Meant as a PRIVATE class for NeoAccess; not indicated for the end user.
+    """
 
     @classmethod
-    def validate_and_standardize(cls, match, dummy_node_name="n") -> dict:
+    def process_match_structure(cls, handle: Union[int, NodeSpecs], dummy_node_name="n") -> CypherMatch:
         """
-        If match is a non-negative integer, it's assumed to be a Neo4j ID, and a match dictionary is created and returned.
-        Otherwise, verify that an alleged "match" dictionary is a valid one:
-        if yes, return it back; if not, raise an Exception
+        Accept either a valid internal database node ID, or a "NodeSpecs" object (a "raw match"),
+        and turn it into a "CypherMatch" object (a "processed match")
+
+        :param handle:
+        :param dummy_node_name:
+        :return:                A "CypherMatch" object (a "processed match"), used to identify a node,
+                                    or group of nodes
+        """
+        if cls.valid_internal_id(handle):    # If the argument "handle" is a valid internal database ID
+            node_specs = NodeSpecs(internal_id=handle)
+            return CypherMatch(node_specs, dummy_node_name_if_missing=dummy_node_name)
 
-        TIP:
-              Calling methods that accept "match" arguments can have a line such as:
-                    match = CypherUtils.validate_and_standardize(match)
-              and, at that point, they will be automatically also accepting Neo4j IDs as "matches"
 
-        TODO: also, accept as argument a list/tuple - and, in addition to the above ops, carry out checks for compatibilities
+        return CypherMatch(handle, dummy_node_name_if_missing=dummy_node_name)
 
-        :param match:           Either a valid Neo4j internal ID, or a "match" dictionary (TODO: or a list/tuple of those)
-        :param dummy_node_name: A string with a name by which to refer to the node (by default, "n");
-                                    note: this is only used if the `match` argument is a valid Neo4j internal ID
 
-        :return:                A valid "match" structure, i.e. a dictionary of data to identify a node, or set of nodes
+
+    @classmethod
+    def check_match_compatibility(cls, match1: CypherMatch, match2: CypherMatch) -> None:
         """
-        if type(match) == int and match >= 0:       # If the argument "match" is a valid Neo4j ID
-            return cls.define_match(internal_id=match, dummy_node_name=dummy_node_name)
+        If the two given "CypherMatch" objects (i.e. PROCESSED match structures)
+        are incompatible - in terms of collision in their dummy node names -
+        raise an Exception.
 
-        cls.assert_valid_match_structure(match)
-        return match
+        :param match1:  A CypherMatch" object to be used to identify a node, or group of nodes
+        :param match2:  A CypherMatch" object to be used to identify a node, or group of nodes
+        :return:        None
+        """
+        assert match1.dummy_node_name != match2.dummy_node_name, \
+            f"check_match_compatibility(): conflict between 2 matches " \
+            f"using the same dummy node name ({match1.dummy_node_name}). " \
+            f"Make sure to pass different dummy names"
 
 
 
     @classmethod
-    def extract_node(cls, match: dict) -> str:
+    def combined_where(cls, match1: CypherMatch, match2: CypherMatch, check_compatibility=True) -> str:
         """
-        Return the node information from the given "match" data structure
+        Given the two "CypherMatch" objects (i.e. PROCESSED match structures),
+        return the combined version of all their WHERE statements.
+        For details, see prepare_where()
 
-        :param match:   A dictionary, as created by define_match()
-        :return:        A string with the node information.  EXAMPLES:
-                            "(n  )"
-                            "(p :`person` )"
-                            "(n :`car`:`surplus inventory` )"
-                            "(n :`person` {`gender`: $n_par_1, `age`: $n_par_2})"
+        :param match1:  A CypherMatch" object to be used to identify a node, or group of nodes
+        :param match2:  A CypherMatch" object to be used to identify a node, or group of nodes
+        :param check_compatibility: Use True if the individual matches are meant to refer to different nodes,
+                                        and need to make sure there's no conflict in the dummy node names
+        :return:        A string with the combined WHERE statement,
+                            suitable for inclusion into a Cypher query (empty if there were no subclauses)
         """
-        return match.get("node")
+        if check_compatibility:
+            cls.check_match_compatibility(match1, match2)
+
+        where_list = [match1.where, match2.where]
+        return cls.prepare_where(where_list)
 
 
     @classmethod
-    def extract_dummy_name(cls, match: dict) -> str:
+    def combined_data_binding(cls, match1: CypherMatch, match2: CypherMatch) -> dict:
         """
-        Return the dummy_node_name from the given "match" data structure
+        Given the two "CypherMatch" objects (i.e. PROCESSED match structures),
+        return the combined version of all their data binding dictionaries.
+        NOTE:  if the individual matches are meant to refer to different nodes,
+                    need to first make sure there's no conflict in the dummy node names -
+                    use check_match_compatibility() as needed.
+                    In practice, combined_where() is typically run whenever combined_data_binding() is -
+                    and the former can take care of checking for compatibility
+
+        :param match1:  A CypherMatch" object to be used to identify a node, or group of nodes
+        :param match2:  A CypherMatch" object to be used to identify a node, or group of nodes
+        :return:        A (possibly empty) dict with the combined data binding dictionaries,
+                            suitable for inclusion into a Cypher query
+        """
+        combined_data_binding = match1.data_binding     # Our 1st dict
+        new_data_binding = match2.data_binding          # Our 2nd dict
+        combined_data_binding.update(new_data_binding)  # Merge the second dict into the first one
+
+        return combined_data_binding
 
-        :param match:   A dictionary, as created by define_match()
-        :return:        A string with the dummy node name (often "n", or "to, or "from")
-        """
-        return match.get("dummy_node_name")
 
 
 
+    ############ The following methods make no reference to any "match" object (neither NodeSpecs nor CypherMatch objects)
+
     @classmethod
-    def unpack_match(cls, match: dict, include_dummy=True) -> list:
+    def assert_valid_internal_id(cls, internal_id: int) -> None:
         """
-        Turn the passed "match" dictionary structure into a list containing:
-        [node, where, data_binding, dummy_node_name]
-        or
-        [node, where, data_binding]
-        depending on the include_dummy flag
-
-        TODO:   gradually phase out, as more advanced util methods
-                make the unpacking of all the "match" internal structure unnecessary
-                Maybe switch default value for include_dummy to False...
-
-        :param match:           A dictionary, as created by define_match()
-        :param include_dummy:   Flag indicating whether to also include the "dummy_node_name" value, as a 4th element in the returned list
-        :return:
+        Raise an Exception if the argument is not a valid Neo4j internal database ID
+
+        :param internal_id: Alleged Neo4j internal database ID
+        :return:            None
         """
-        if include_dummy:
-            match_as_list = [match.get(key) for key in ["node", "where", "data_binding", "dummy_node_name"]]
-        else:
-            match_as_list = [match.get(key) for key in ["node", "where", "data_binding"]]
+        assert type(internal_id) == int, \
+            f"assert_valid_internal_id(): Neo4j internal ID's MUST be integers; " \
+            f"the value passed ({internal_id}) was of type {type(internal_id)}"
 
-        return match_as_list
+        # Note that 0 is a valid Neo4j ID (apparently inconsistently assigned, on occasion, by the database)
+        assert internal_id >= 0, \
+            f"assert_valid_internal_id(): Neo4j internal ID's cannot be negative; the value passed was {internal_id}"
 
 
 
     @classmethod
-    def check_match_compatibility(cls, match1, match2) -> None:
+    def valid_internal_id(cls, internal_id: int) -> bool:
         """
-        If the two given match structures are incompatible (in terms of collision in their dummy node name),
-        raise an Exception.
+        Return True if internal_id is a valid ID as used internally by the database
+        (aka "Neo4j ID")
 
-        :param match1:
-        :param match2:
-        :return:        None
+        :param internal_id: An alleged internal database ID
+        :return:            True if internal_id is a valid internal database ID, or False otherwise
         """
-        assert match1.get("dummy_node_name") != match2.get("dummy_node_name"), \
-            f"check_match_compatibility(): conflict between 2 matches " \
-            f"using the same dummy node name ({match1.get('dummy_node_name')}). " \
-            f"Make sure to pass different dummy names to match()"
+        try:
+            cls.assert_valid_internal_id(internal_id)
+            return True
+        except Exception:
+            return False
 
 
 
     @classmethod
     def prepare_labels(cls, labels) -> str:
         """
         Turn the given string, or list/tuple of strings - representing Neo4j labels - into a string
@@ -345,15 +486,16 @@
         Blanks ARE allowed in the names.
         EXAMPLES:
             "" or None          give rise to    ""
             "client"            gives rise to   ":`client`"
             "my label"          gives rise to   ":`my label`"
             ["car", "vehicle"]  gives rise to   ":`car`:`vehicle`"
 
-        :param labels:  A string, or list/tuple of strings, representing one or multiple Neo4j labels
+        :param labels:  A string, or list/tuple of strings, representing one or multiple Neo4j labels;
+                            it's acceptable to be None
         :return:        A string suitable for inclusion in the node part of a Cypher query
         """
         if not labels:
             return ""   # No labels
 
         if type(labels) == str:
             labels = [labels]
@@ -364,83 +506,47 @@
             # Note: the back ticks allow the inclusion of blank spaces in the labels
 
         return cypher_labels
 
 
 
     @classmethod
-    def combined_where(cls, match_list: list) -> str:
-        """
-        Given a list of "match" structures, return the combined version of all their WHERE statements.
-        For details, see prepare_where()
-        TODO: Make sure there's no conflict in the dummy node names
-
-        :param match_list:  A list of "match" structures
-        :return:            A string with the combined WHERE statement,
-                            suitable for inclusion into a Cypher query (empty if there were no subclauses)
-        """
-        where_list = [match.get("where", "") for match in match_list]
-        return cls.prepare_where(where_list)
-
-
-
-    @classmethod
     def prepare_where(cls, where_list: Union[str, list]) -> str:
         """
-        Given a WHERE clauses, or list/tuple of them, combined them all into one -
-        and also prefix to the result (if appropriate) the WHERE keyword.
-        The combined clauses of the WHERE statement are parentheses-enclosed, to protect against code injection
+        Given a WHERE clause, or list/tuple of them, combined them all into one -
+        and also prefix the WHERE keyword to the result (if appropriate).
+        The *combined* clauses of the WHERE statement are parentheses-enclosed, to protect against code injection
 
         EXAMPLES:   "" or "      " or [] or ("  ", "") all result in  ""
                     "n.name = 'Julian'" returns "WHERE (n.name = 'Julian')"
                         Likewise for ["n.name = 'Julian'"]
                     ("p.key1 = 123", "   ",  "p.key2 = 456") returns "WHERE (p.key1 = 123 AND p.key2 = 456)"
 
         :param where_list:  A string with a subclause, or list or tuple of subclauses,
                             suitable for insertion in a WHERE statement
 
         :return:            A string with the combined WHERE statement,
                             suitable for inclusion into a Cypher query (empty if there were no subclauses)
         """
         if type(where_list) == str:
             where_list = [where_list]
-
-        assert type(where_list) == list or type(where_list) == tuple, \
-            f"prepare_where(): the argument must be a string, list or tuple; instead, it was {type(where_list)}"
+        else:
+            assert type(where_list) == list or type(where_list) == tuple, \
+                f"prepare_where(): the argument must be a string, list or tuple; instead, it was of type {type(where_list)}"
 
         purged_where_list = [w for w in where_list if w.strip() != ""]      # Drop all the blank terms in the list
 
         if len(purged_where_list) == 0:
             return ""
 
         return "WHERE (" + " AND ".join(purged_where_list) + ")"    # The outer parentheses are to protect against code injection
 
 
 
     @classmethod
-    def combined_data_binding(cls, match_list: list) -> dict:
-        """
-        Given a list of "match" structures, returned the combined version of all their data binding dictionaries.
-        TODO: Make sure there's no conflicts
-        TODO: Since this also works with a 1-element list, it can be use to simply unpack the data binding from the match structure
-              (i.e. ought to drop the "combined" from the name)
-        """
-        first_match = match_list[0]
-        combined_data_binding = first_match.get("data_binding", {})
-
-        for i, match in enumerate(match_list):
-            if i != 0:      # Skip the first one, which we already processed above
-                new_data_binding = match.get("data_binding", {})
-                combined_data_binding.update(new_data_binding)
-
-        return combined_data_binding
-
-
-
-    @classmethod
     def dict_to_cypher(cls, data_dict: {}, prefix="par_") -> (str, {}):
         """
         Turn a Python dictionary (meant for specifying node or relationship attributes)
         into a string suitable for Cypher queries,
         plus its corresponding data-binding dictionary.
 
         EXAMPLE :
```

### Comparing `neoaccess-4.2.0/src/neoaccess/neoaccess.py` & `neoaccess-4.3.1/src/neoaccess/neoaccess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,77 +1,45 @@
 from neo4j import GraphDatabase                         # The Neo4j python connectivity library "Neo4j Python Driver"
 from neo4j import __version__ as neo4j_driver_version   # The version of the Neo4j driver being used
 import neo4j.graph                                      # To check returned data types
-from .cypher_utils import CypherUtils                   # Helper class for NeoAccess
+from .cypher_utils import CypherUtils, NodeSpecs        # Helper classes for NeoAccess
 import numpy as np
 import pandas as pd
 import os
 import sys
 import json
 from typing import Union, List
 
 
-class NeoAccess:
-    """
-    IMPORTANT : for versions 4.x of the Neo4j database
-
-    High-level class to interface with the Neo4j graph database from Python.
-
-    Mostly tested on versions 4.3 and 4.4 of Neo4j Community version, but should work with other 4.x versions, too.
-    NOT tested on any other major version of Neo4j; in particular, NOT tested with version 5
-
-    Conceptually, there are two parts to NeoAccess:
-        1) A thin wrapper around the Neo4j python connectivity library "Neo4j Python Driver"
-          that is documented at: https://neo4j.com/docs/api/python-driver/current/api.html
-
-        2) A layer above, providing higher-level functionality for common database operations,
-           such as lookup, creation, deletion, modification, import, indices, etc.
-
-    SECTIONS IN THIS CLASS:
-        * INIT
-        * RUNNING GENERIC QUERIES
-        * RETRIEVE DATA
-        * FOLLOW LINKS
-        * CREATE NODES
-        * DELETE NODES
-        * MODIFY FIELDS
-        * RELATIONSHIPS
-        * LABELS
-        * INDEXES
-        * CONSTRAINTS
-        * READ IN DATA from PANDAS
-        * JSON IMPORT/EXPORT
-        * DEBUGGING SUPPORT
-
-    Plus separate class "CypherUtils"
-
+'''
     ----------------------------------------------------------------------------------
     HISTORY and AUTHORS:
         - NeoAccess (this library) is a fork of NeoInterface;
                 NeoAccess was created, and is being maintained, by Julian West,
                 primarily in the context of the BrainAnnex.org open-source project.
-                It started out in late 2021; for change log thru 2022,
+                It started out in late 2021; for change log thru 2023,
                 see the "LIBRARIES" entries in https://brainannex.org/viewer.php?ac=2&cat=14
 
         - NeoInterface (the parent library)
                 was co-authored by Alexey Kuznetsov and Julian West in 2021,
                 and is maintained by GSK pharmaceuticals
                 with an Apache License 2.0 (https://github.com/GSK-Biostatistics/neointerface).
                 NeoInterface is in part based on the earlier library Neo4jLiaison,
                 as well as a library developed by Alexey Kuznetsov.
 
-        - Neo4jLiaison, now deprecated, was authored by Julian West in 2020
+        - Neo4jLiaison, an ancestor library now obsoleted, was authored by Julian West in 2020
                 (https://github.com/BrainAnnex/neo4j-liaison)
 
     ----------------------------------------------------------------------------------
 	MIT License
 
         Copyright (c) 2021-2023 Julian A. West
 
-        This file is part of the "Brain Annex" project (https://BrainAnnex.org).
+        This file is part of the "Brain Annex" project (https://BrainAnnex.org),
+        though it's released independently.
         See "AUTHORS", above, for full credits.
 
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
@@ -84,19 +52,35 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 	----------------------------------------------------------------------------------
+'''
+
+
+class NeoAccessCore:
+    """
+    IMPORTANT : for versions 4.x of the Neo4j database
+
+    A thin wrapper around the Neo4j python connectivity library "Neo4j Python Driver"
+    that is documented at: https://neo4j.com/docs/api/python-driver/current/api.html
+
+    This "CORE" library may be used independently,
+    or as the foundation of the higher-level child class, "NeoAccess"
+
+    SECTIONS IN THIS CLASS:
+        * INIT (constructor) and DATABASE CONNECTION
+        * RUNNING GENERIC CYPHER QUERIES
     """
 
     def __init__(self,
-                 host=os.environ.get("NEO4J_HOST"),
-                 credentials=(os.environ.get("NEO4J_USER"), os.environ.get("NEO4J_PASSWORD")),
+                 host=os.getenv("NEO4J_HOST"),
+                 credentials=(os.getenv("NEO4J_USER"), os.getenv("NEO4J_PASSWORD")),
                  apoc=False,
                  debug=False,
                  autoconnect=True):
         """
         If unable to create a Neo4j driver object, raise an Exception
         reminding the user to check whether the Neo4j database is running
 
@@ -106,16 +90,14 @@
         :param credentials: Pair of strings (tuple or list) containing, respectively, the database username and password
                                 DEFAULT: read from NEO4J_USER and NEO4J_PASSWORD environmental variables
         :param apoc:        Flag indicating whether apoc library is used on Neo4j database to connect to
                                 Notes: APOC, if used, must also be enabled on the database.
                                 The only method currently requiring APOC is export_dbase_json()
         :param debug:       Flag indicating whether a debug mode is to be used by all methods of this class
         :param autoconnect  Flag indicating whether the class should establish connection to database at initialization
-
-        TODO: try os.getenv() in lieu of os.environ.get()
         """
         self.debug = debug
 
         self.host = host
         self.credentials = credentials
 
         self.apoc = apoc
@@ -137,34 +119,39 @@
         In the process, create and save a driver object.
         """
         assert self.host, "Host name must be specified in order to connect to the Neo4j database"
         assert self.credentials, "Neo4j database credentials (username and password) must be specified in order to connect to it"
 
         try:
             user, password = self.credentials  # This unpacking will work whether the credentials were passed as a tuple or list
-            print(f"Attempting to connect to Neo4j host '{self.host}', with username '{user}'")
+            if self.debug:
+                print(f"Attempting to connect to Neo4j host '{self.host}', with username '{user}'")
+            else:
+                print(f"Attempting to connect to Neo4j database")
+
             self.driver = GraphDatabase.driver(self.host,
                                                auth=(user, password))   # Object to connect to Neo4j's Bolt driver for Python
-                                                                        # https://neo4j.com/docs/api/python-driver/4.3/api.html#driver
+            # https://neo4j.com/docs/api/python-driver/4.3/api.html#driver
         except Exception as ex:
             error_msg = f"CHECK WHETHER NEO4J IS RUNNING! While instantiating the NeoAccess object, it failed to create the driver: {ex}"
             # In case of sluggish server connection, a ConnectionResetError seems to be generated;
             # TODO: maybe try to detect that, and give a more informative message
             raise Exception(error_msg)
 
-        self.debug_print(f"Connection to host '{self.host}' established")
+        if self.debug:
+            print(f"Connection to host '{self.host}' established")
 
         # If we get thus far, the connection to the host was successfully established,
         # BUT this doesn't prove that we can actually connect to the database;
         # for example, with bad credentials, the connection to the host can still be established
         try:
             self.test_dbase_connection()
         except Exception as ex:
             (exc_type, _, _) = sys.exc_info()   # This is for the purpose of giving more informative error messages;
-                                                # for example, a bad database passwd will show "<class 'neo4j.exceptions.AuthError'>"
+            # for example, a bad database passwd will show "<class 'neo4j.exceptions.AuthError'>"
             error_msg = f"Unable to access the Neo4j database; " \
                         f"CHECK THE DATABASE USERNAME/PASSWORD in the credentials your provided: {str(exc_type)} - {ex}"
             raise Exception(error_msg)
 
 
 
     def test_dbase_connection(self) -> None:
@@ -189,38 +176,28 @@
         return neo4j_driver_version
 
 
 
     def close(self) -> None:
         """
         Terminate the database connection.
-        Note: this method is automatically invoked after the last operation of a "with" statement
+        Note: this method is automatically invoked
+              after the last operation included in "with" statements
 
         :return:    None
         """
         if self.driver is not None:
             self.driver.close()
 
 
 
-    def assert_valid_internal_id(self, internal_id: int) -> None:
-        """
-        Raise an Exception if the argument is not a valid database internal ID
-
-        :param internal_id: Alleged Neo4j internal database ID
-        :return:            None
-        """
-        CypherUtils.assert_valid_internal_id(internal_id)
-
-
-
 
     #####################################################################################################
 
-    '''                                 ~   RUN GENERIC QUERIES   ~                                   '''
+    '''                          ~   RUN GENERIC CYPHER QUERIES   ~                                   '''
 
     def ________RUN__GENERIC_QUERIES________(DIVIDER):
         pass        # Used to get a better structure view in IDEs
     #####################################################################################################
 
 
     def query(self, q: str, data_binding=None, single_row=False, single_cell="", single_column=""):
@@ -283,16 +260,16 @@
 
             # Note: A neo4j.Result object (printing it, shows an object of type "neo4j.work.result.Result")
             #       See https://neo4j.com/docs/api/python-driver/current/api.html#neo4j.Result
             if result is None:
                 return []
 
             data_as_list = result.data()        # Return the result as a list of dictionaries.
-                                                #       This must be done inside the "with" block,
-                                                #       while the session is still open
+            #       This must be done inside the "with" block,
+            #       while the session is still open
 
         # Deal with empty result lists
         if len(data_as_list) == 0:  # If no results were produced
             if single_row:
                 return {}           # representing an empty record
             if single_cell:
                 return None
@@ -401,15 +378,15 @@
                         neo4j_properties["internal_id"] = item.id               # Example: 227
                         neo4j_properties["neo4j_labels"] = list(item.labels)    # Example: ['person', 'client']
 
                     elif isinstance(item, neo4j.graph.Relationship):
                         neo4j_properties["internal_id"] = item.id               # Example: 227
                         neo4j_properties["neo4j_start_node"] = item.start_node  # A neo4j.graph.Node object with "id", "labels" and "properties"
                         neo4j_properties["neo4j_end_node"] = item.end_node      # A neo4j.graph.Node object with "id", "labels" and "properties"
-                                                                                #   Example: <Node id=118 labels=frozenset({'car'}) properties={'color': 'white'}>
+                        #   Example: <Node id=118 labels=frozenset({'car'}) properties={'color': 'white'}>
                         neo4j_properties["neo4j_type"] = item.type              # The name of the relationship
 
                     elif isinstance(item, neo4j.graph.Path):
                         neo4j_properties["neo4j_nodes"] = item.nodes            # The sequence of Node objects in this path
 
                     # Exclude any unwanted (ordinary or special) field
                     if fields_to_exclude:
@@ -425,31 +402,32 @@
                 if not flatten:
                     data_as_list.append(data)
 
             return data_as_list
 
 
 
-    def update_query(self, cypher: str, data_binding=None) -> dict:
+    def update_query(self, q: str, data_binding=None) -> dict:
         """
         Run a Cypher query and return statistics about its actions (such number of nodes created, etc.)
         Typical use is for queries that update the database.
         If the query returns any values, a list of them is also made available, as the value of the key 'returned_data'.
 
         Note: if the query creates nodes and one wishes to obtain their Neo4j internal ID's,
               one can include Cypher code such as "RETURN id(n) AS internal_id" (where n is the dummy name of the newly-created node)
 
         EXAMPLE:  result = update_query("CREATE(n :CITY {name: 'San Francisco'}) RETURN id(n) AS internal_id")
 
                   result will be {'nodes_created': 1, 'properties_set': 1, 'labels_added': 1,
                                   'returned_data': [{'internal_id': 123}]
                                  } , assuming 123 is the Neo4j internal ID of the newly-created node
 
-        :param cypher:      Any Cypher query, but typically one that doesn't return anything
+        :param q:           Any Cypher query, but typically one that doesn't return anything
         :param data_binding: Data-binding dictionary for the Cypher query
+
         :return:            A dictionary of statistics (counters) about the query just run
                             EXAMPLES -
                                 {}      The query had no effect
                                 {'nodes_deleted': 3}    The query resulted in the deletion of 3 nodes
                                 {'properties_set': 2}   The query had the effect of setting 2 properties
                                 {'relationships_created': 1}    One new relationship got created
                                 {'returned_data': [{'internal_id': 123}]}  'returned_data' contains the results of the query,
@@ -461,26 +439,26 @@
                                 properties_set, labels_added, labels_removed,
                                 indexes_added, indexes_removed, constraints_added, constraints_removed
                                 More info:  https://neo4j.com/docs/api/python-driver/current/api.html#neo4j.SummaryCounters
         """
 
         # Start a new session, use it, and then immediately close it
         with self.driver.session() as new_session:
-            result = new_session.run(cypher, data_binding)
+            result = new_session.run(q, data_binding)
             if self.profiling:
-                print("-- update_query() PROFILING ----------\n", cypher, "\n", data_binding)
+                print("-- update_query() PROFILING ----------\n", q, "\n", data_binding)
 
             # Note: result is a neo4j.Result iterable object
             #       See https://neo4j.com/docs/api/python-driver/current/api.html#neo4j.Result
 
             data_as_list = result.data()    # Fetch any data returned by the query, as a (possibly-empty) list of dictionaries
 
             info = result.consume() # Get the stats of the query just executed
-                                    # This is a neo4j.ResultSummary object
-                                    # See https://neo4j.com/docs/api/python-driver/current/api.html#neo4j.ResultSummary
+            # This is a neo4j.ResultSummary object
+            # See https://neo4j.com/docs/api/python-driver/current/api.html#neo4j.ResultSummary
 
             if self.debug:
                 print("In update_query(). Attributes of ResultSummary object:")
                 # Show as dictionary, which is available in info.__dict__
                 for k, v in info.__dict__.items():
                     print(f"    {k} -> {v}")
                 '''
@@ -502,24 +480,72 @@
                     'counters': {'nodes_deleted': 1}, 
                     'result_available_after': 0, 
                     'result_consumed_after': 0
                 }
                 '''
 
             stats = info.counters   # A neo4j.SummaryCounters object
-                                    # See https://neo4j.com/docs/api/python-driver/current/api.html#neo4j.SummaryCounters
+            # See https://neo4j.com/docs/api/python-driver/current/api.html#neo4j.SummaryCounters
             stats_dict = stats.__dict__   # Convert object to dictionary
 
             stats_dict['returned_data'] = data_as_list  # Add an extra entry to the dictionary, with the data returned by the query
 
             return stats_dict
 
 
 
 
+
+
+###################################################################################################
+###################################################################################################
+
+class NeoAccess(NeoAccessCore):
+    """
+    IMPORTANT : for versions 4.x of the Neo4j database
+
+    High-level class to interface with the Neo4j graph database from Python.
+
+    Mostly tested on versions 4.3 and 4.4 of Neo4j Community version, but should work with other 4.x versions, too.
+    NOT tested on any other major version of Neo4j; in particular, NOT tested with version 5
+
+    This class is a layer above its parent class "NeoAccessCore",
+        and it provides a higher-level functionality for common database operations,
+        such as lookup, creation, deletion, modification, import, indices, etc.
+
+    SECTIONS IN THIS CLASS:
+        * INTERNAL DATABASE ID
+        * RETRIEVE DATA
+        * FOLLOW LINKS
+        * CREATE NODES
+        * DELETE NODES
+        * MODIFY FIELDS
+        * RELATIONSHIPS
+        * LABELS
+        * INDEXES
+        * CONSTRAINTS
+        * READ IN DATA from PANDAS
+        * JSON IMPORT/EXPORT
+        * DEBUGGING SUPPORT
+
+    It makes use of separate classes (NOT meant for the end user) in the file cypher_utils.py
+    """
+
+
+    def assert_valid_internal_id(self, internal_id: int) -> None:
+        """
+        Raise an Exception if the argument is not a valid database internal ID
+
+        :param internal_id: Alleged Neo4j internal database ID
+        :return:            None
+        """
+        CypherUtils.assert_valid_internal_id(internal_id)
+
+
+
     #####################################################################################################
 
     '''                                      ~   RETRIEVE DATA   ~                                            '''
 
     def ________RETRIEVE_DATA________(DIVIDER):
         pass        # Used to get a better structure view in IDEs
     #####################################################################################################
@@ -559,17 +585,17 @@
 
 
 
     def exists_by_key(self, labels: str, key_name: str, key_value) -> bool:
         """
         Return True if a node with the given labels and key_name/key_value exists, or False otherwise
         TODO: test for multiple labels
-        :param labels:
-        :param key_name:
-        :param key_value:
+        :param labels:      A string or list/tuple of strings
+        :param key_name:    A string with the name of a node attribute
+        :param key_value:   The desired value of the key_name attribute
         :return:            True if a node with the given labels and key_name/key_value exists,
                                 or False otherwise
         """
         record = self.get_record_by_primary_key(labels, key_name, key_value)
 
         if record is None:
             return False
@@ -595,22 +621,22 @@
 
         number_of_nodes = result[0]["number_of_nodes"]
 
         return number_of_nodes > 0
 
 
 
-    def get_single_field(self, match: Union[int, dict], field_name: str, order_by=None, limit=None) -> list:
+    def get_single_field(self, match: Union[int, NodeSpecs], field_name: str, order_by=None, limit=None) -> list:
         """
         For situations where one is fetching just 1 field,
         and one desires a list of the values of that field, rather than a dictionary of records.
         In other respects, similar to the more general get_nodes()
 
-        :param match:       EITHER an integer with a Neo4j node id,
-                                OR a dictionary of data to identify a node, or set of nodes, as returned by match()
+        :param match:       EITHER an integer with an internal database node id,
+                                OR a "NodeSpecs" object, as returned by match(), with data to identify a node or set of nodes
         :param field_name:  A string with the name of the desired field (attribute)
         :param order_by:    see get_nodes()
         :param limit:       see get_nodes()
 
         :return:  A list of the values of the field_name attribute in the nodes that match the specified conditions
         """
 
@@ -618,23 +644,23 @@
 
         single_field_list = [record.get(field_name) for record in record_list]
 
         return single_field_list
 
 
 
-    def get_nodes(self, match: Union[int, dict],
+    def get_nodes(self, match: Union[int, NodeSpecs],
                   return_internal_id=False, return_labels=False, order_by=None, limit=None,
                   single_row=False, single_cell=""):
         """
         RETURN a list of the records (as dictionaries of ALL the key/value node properties)
         corresponding to all the Neo4j nodes specified by the given match data.
 
-        :param match:           EITHER an integer with a Neo4j node id,
-                                OR a dictionary of data to identify a node, or set of nodes, as returned by match()
+        :param match:           EITHER an integer with an internal database node id,
+                                    OR a "NodeSpecs" object, as returned by match(), with data to identify a node or set of nodes
 
         :param return_internal_id:  Flag indicating whether to also include the Neo4j internal node ID in the returned data
                                     (using "internal_id" as its key in the returned dictionary)
         :param return_labels:   Flag indicating whether to also include the Neo4j label names in the returned data
                                     (using "neo4j_labels" as its key in the returned dictionary)
 
         :param order_by:        Optional string with the key (field) name to order by, in ascending order
@@ -671,15 +697,15 @@
         match_structure = CypherUtils.process_match_structure(match)
 
         if self.debug:
             print("In get_nodes()")
             print("    match_structure:", match_structure)
 
         # Unpack needed values from the match dictionary
-        (node, where, data_binding, dummy_node_name) = CypherUtils.unpack_match(match_structure)
+        (node, where, data_binding, dummy_node_name) = match_structure.unpack_match()
 
         cypher = f"MATCH {node} {CypherUtils.prepare_where(where)} RETURN {dummy_node_name}"
 
         if order_by:
             cypher += f" ORDER BY n.{order_by}"
 
         if limit:
@@ -714,38 +740,39 @@
         if single_cell:
             return result_list[0].get(single_cell)
 
         return result_list
 
 
 
-    def get_df(self, match: Union[int, dict], order_by=None, limit=None) -> pd.DataFrame:
+    def get_df(self, match: Union[int, NodeSpecs], order_by=None, limit=None) -> pd.DataFrame:
         """
         Similar to get_nodes(), but with fewer arguments - and the result is returned as a Pandas dataframe
 
         [See get_nodes() for more information about the arguments]
-        :param match:       EITHER an integer with a Neo4j node id,
-                                OR a dictionary of data to identify a node, or set of nodes, as returned by match()
+        :param match:       EITHER an integer with an internal database node id,
+                                OR a "NodeSpecs" object, as returned by match(), with data to identify a node or set of nodes
         :param order_by:    Optional string with the key (field) name to order by, in ascending order
                                 Note: lower and uppercase names are treated differently in the sort order
         :param limit:       Optional integer to specify the maximum number of nodes returned
 
         :return:            A Pandas dataframe
         """
 
         result_list = self.get_nodes(match=match, order_by=order_by, limit=limit)
         return pd.DataFrame(result_list)
 
 
 
     def match(self, labels=None, internal_id=None,
-              key_name=None, key_value=None, properties=None, clause=None, dummy_node_name="n") -> dict:
+              key_name=None, key_value=None, properties=None, clause=None, dummy_node_name="n") -> NodeSpecs:
         """
-        Return a dictionary storing all the passed specifications (the "RAW match structure"),
-        as expected as argument in various other functions in this library, in order to identify a node or group of nodes.
+        Return a "NodeSpecs" object storing all the passed specifications (the "RAW match structure"),
+        as expected as argument in various other functions in this library,
+        in order to identify a node or group of nodes.
 
         IMPORTANT:  if internal_id is provided, all other conditions are DISREGARDED;
                     otherwise, an implicit AND applies to all the specified conditions.
 
         Note:   NO database operation is actually performed by this function.
 
         [Other names explored: identify(), preserve(), define_match(), locate(), choose() or identify()]
@@ -778,68 +805,40 @@
                                             ("n.weight < $max_weight", {"max_weight": 100})
 
         :param dummy_node_name: A string with a name by which to refer to the node (by default, "n");
                                 only used if a `clause` argument is passed
 
         :return:            A python data dictionary, to preserve together all the passed arguments
         """
-        if labels is not None:
-            assert (type(labels) == str) or (type(labels) == list) or (type(labels) == tuple), \
-                f"match(): the argument `labels`, if provided, must be a string, or a list/tuple of strings"
-
-        if internal_id is not None:
-            assert CypherUtils.validate_internal_id(internal_id), \
-                f"match(): the argument `internal_id` ({internal_id}) is not a valid internal database ID value"
-
-        if key_name is not None:
-            assert type(key_name) == str, \
-                f"match(): the argument `key_name`, if provided, must be a string"
-            assert key_value is not None, \
-                f"match(): if the argument `key_name` is provided, there must also be a `key_value` argument"
-
-        if properties is not None:
-            assert type(properties) == dict, \
-                f"match(): the argument `properties`, if provided, must be a python dictionary"
-
-        if clause is not None:
-            assert (type(clause) == str) or (type(clause) == list) or (type(clause) == tuple), \
-                f"match(): the argument `clause`, if provided, must be a string or a pair.  EXAMPLE: 'n.age > 21'"
-
-
-        if clause is None:
-            dummy_node_name = None      # In this scenario, the dummy name isn't yet used, and any name could be used
-
-        raw_match_structure = {"internal_id": internal_id, "labels": labels,
-                           "key_name": key_name, "key_value": key_value,
-                           "properties": properties, "clause": clause,
-                           "dummy_node_name": dummy_node_name}
+        return NodeSpecs(internal_id=internal_id,
+                         labels=labels, key_name=key_name, key_value=key_value,
+                         properties=properties, clause=clause, clause_dummy_name=dummy_node_name)
 
-        return raw_match_structure
 
 
-
-    def get_node_internal_id(self, match: dict) -> int:
+    def get_node_internal_id(self, match: Union[int, NodeSpecs]) -> int:
         """
         Return the internal database ID of a SINGLE node identified by the "match" data
         created by a call to match().
 
         If not found, or if more than 1 found, an Exception is raised
 
-        :param match:   A dictionary of data to identify a single node, as returned by match()
+        :param match:   EITHER an integer with an internal database node id,
+                            OR a "NodeSpecs" object, as returned by match(), with data to identify a node or set of nodes
         :return:        An integer with the internal database ID of the located node,
                         if exactly 1 node is found; otherwise, raise an Exception
         """
         match_structure = CypherUtils.process_match_structure(match)
 
         if self.debug:
             print("In get_node_internal_id()")
             print("    match_structure:", match_structure)
 
         # Unpack needed values from the match dictionary
-        (node, where, data_binding) = CypherUtils.unpack_match(match_structure, include_dummy=False)
+        (node, where, data_binding, _) = match_structure.unpack_match()
 
         q = f"MATCH {node} {CypherUtils.prepare_where(where)} RETURN id(n) AS INTERNAL_ID"
         self.debug_query_print(q, data_binding, "get_node_internal_id")
 
         result = self.query(q, data_binding, single_column="INTERNAL_ID")
 
         assert len(result) != 0, "get_node_internal_id(): node NOT found"
@@ -879,19 +878,20 @@
 
     def create_node(self, labels, properties=None) -> int:
         """
         Create a new node with the given label(s),
         and with the attributes/values specified in the properties dictionary.
         Return the Neo4j internal ID of the node just created.
 
-        :param labels:      A string, or list/tuple of strings, specifying Neo4j labels (ok to have blank spaces)
+        :param labels:      A string, or list/tuple of strings, specifying Neo4j labels (ok to have blank spaces);
+                                it's acceptable to be None
         :param properties:  OPTIONAL (possibly empty or None) dictionary of properties to set for the new node.
                                 EXAMPLE: {'age': 22, 'gender': 'F'}
 
-        :return:            An integer with the Neo4j internal ID of the node just created
+        :return:            An integer with the internal database ID of the node just created
         """
 
         if properties is None:
             properties = {}
 
         # From the dictionary of attribute names/values,
         #       create a part of a Cypher query, with its accompanying data dictionary
@@ -1058,15 +1058,15 @@
                                 a string or list/tuple of strings; blanks allowed inside strings
         :param properties:  A dictionary of optional properties to assign to the newly-created node
         :param links:       Optional list of dicts identifying existing nodes,
                                 and specifying the name, direction and optional properties
                                 to give to the links connecting to them;
                                 use None, or an empty list, to indicate if there aren't any
                                 Each dict contains the following keys:
-                                    "internal_id"        REQUIRED - to identify an existing node
+                                    "internal_id"   REQUIRED - to identify an existing node
                                     "rel_name"      REQUIRED - the name to give to the link
                                     "rel_dir"       OPTIONAL (default "OUT") - either "IN" or "OUT" from the new node
                                     "rel_attrs"     OPTIONAL - A dictionary of relationship attributes
         :param merge:       (OPTIONAL; default False) If True, a new node gets created only if there's no existing node
                                 with the same properties and labels     TODO: test more
 
         :return:            An integer with the Neo4j ID of the newly-created node
@@ -1434,32 +1434,32 @@
     '''                                      ~   DELETE NODES   ~                                     '''
 
     def ________DELETE_NODES________(DIVIDER):
         pass        # Used to get a better structure view in IDEs
     #####################################################################################################
 
 
-    def delete_nodes(self, match: Union[int, dict]) -> int:
+    def delete_nodes(self, match: Union[int, NodeSpecs]) -> int:
         """
         Delete the node or nodes specified by the match argument.
         Return the number of nodes deleted.
 
         :param match:   EITHER an integer with an internal database node id,
-                            OR a dictionary of data to identify a node, or set of nodes, as returned by match()
+                            OR a "NodeSpecs" object, as returned by match(), with data to identify a node or set of nodes
         :return:        The number of nodes deleted (possibly zero)
         """
         # Create the "processed-match dictionaries"
         match_structure = CypherUtils.process_match_structure(match)
 
         if self.debug:
             print("In delete_nodes()")
             print("    match_structure:", match_structure)
 
         # Unpack needed values from the match dictionary
-        (node, where, data_binding) = CypherUtils.unpack_match(match_structure, include_dummy=False)
+        (node, where, data_binding, _) = match_structure.unpack_match()
 
         q = f"MATCH {node} {CypherUtils.prepare_where(where)} DETACH DELETE n"
         self.debug_query_print(q, data_binding, "delete_nodes")
 
         stats = self.update_query(q, data_binding)
         number_nodes_deleted = stats.get("nodes_deleted", 0)
         return number_nodes_deleted
@@ -1484,15 +1484,15 @@
 
             q = "MATCH (n) DETACH DELETE(n)"
             self.query(q)       # TODO: switch to update_query() and return the number of nodes deleted
             return
 
         if not delete_labels:
             delete_labels = self.get_labels()   # If no specific labels to delete were given,
-                                                # then consider all labels for possible deletion (unless marked as "keep", below)
+            # then consider all labels for possible deletion (unless marked as "keep", below)
         else:
             if type(delete_labels) == str:
                 delete_labels = [delete_labels] # If a string was passed, turn it into a list
 
         if not keep_labels:
             keep_labels = []    # Initialize list of labels to keep, if not provided
         else:
@@ -1507,15 +1507,15 @@
                 self.debug_query_print(q, method="delete_nodes_by_label")
                 self.query(q)       # TODO: switch to update_query() and return the number of nodes deleted
 
 
 
     def bulk_delete_by_label(self, label: str):    # TODO: test.  CAUTION: only tested interactively
         """
-        IMPORTANT: APOC required (starting from v 4.4 of Neo4j, will be able to do this without APOC)
+        IMPORTANT: APOC required (starting from v 4.4 of Neo4j, will be able to do this without APOC; TODO: not yet tested)
 
         Meant for large databases, where the straightforward deletion operations may result
         in very large number of nodes, and take a long time (or possibly fail)
 
         "If you need to delete some large number of objects from the graph,
         one needs to be mindful of the not building up such a large single transaction
         such that a Java OUT OF HEAP Error will be encountered."
@@ -1563,29 +1563,29 @@
     '''                                      ~   MODIFY FIELDS   ~                                          '''
 
     def ________MODIFY_FIELDS________(DIVIDER):
         pass        # Used to get a better structure view in IDEs
     #####################################################################################################
 
 
-    def set_fields(self, match: Union[int, dict], set_dict: dict ) -> int:
+    def set_fields(self, match: Union[int, NodeSpecs], set_dict: dict ) -> int:
         """
         EXAMPLE - locate the "car" with vehicle id 123 and set its color to white and price to 7000
             match_structure = match(labels = "car", properties = {"vehicle id": 123})
             set_fields(match=match_structure, set_dict = {"color": "white", "price": 7000})
 
         NOTE: other fields are left un-disturbed
 
         Return the number of properties set.
 
         TODO: if any field is blank, offer the option drop it altogether from the node,
               with a "REMOVE n.field" statement in Cypher; doing SET n.field = "" doesn't drop it
 
-        :param match:       EITHER an integer with a Neo4j node id,
-                                OR a dictionary of data to identify a node, or set of nodes, as returned by match()
+        :param match:       EITHER an integer with an internal database node id,
+                                OR a "NodeSpecs" object, as returned by match(), with data to identify a node or set of nodes
         :param set_dict:    A dictionary of field name/values to create/update the node's attributes
                             (note: blanks ARE allowed in the keys)
 
         :return:            The number of properties set
         """
 
         if set_dict == {}:
@@ -1594,15 +1594,15 @@
         match_structure = CypherUtils.process_match_structure(match)
 
         if self.debug:
             print("In set_fields()")
             print("    match_structure:", match_structure)
 
         # Unpack needed values from the match dictionary
-        (node, where, data_binding, dummy_node_name) = CypherUtils.unpack_match(match_structure)
+        (node, where, data_binding, dummy_node_name) = match_structure.unpack_match()
 
         cypher_match = f"MATCH {node} {CypherUtils.prepare_where(where)} "
 
         set_list = []
         for field_name, field_value in set_dict.items():        # field_name, field_value are key/values in set_dict
             field_name_safe = field_name.replace(" ", "_")      # To protect against blanks in name.  E.g., "end date" becomes "end_date"
             set_list.append(f"{dummy_node_name}.`{field_name}` = ${field_name_safe}")    # Example:  "n.`field1` = $field1"
@@ -1649,74 +1649,71 @@
         :return:    A list of strings
         """
         results = self.query("call db.relationshipTypes() yield relationshipType return relationshipType")
         return [x['relationshipType'] for x in results]
 
 
 
-    def add_links(self, match_from: Union[int, dict], match_to: Union[int, dict], rel_name:str) -> int:
+    def add_links(self, match_from: Union[int, NodeSpecs], match_to: Union[int, NodeSpecs], rel_name:str) -> int:
         """
         Add one or more links (aka graph edges/relationships), with the specified rel_name,
-        originating in any of the nodes specified by the match_from specifications,
-        and terminating in any of the nodes specified by the match_to specifications
+        originating in each of the nodes specified by the match_from specifications,
+        and terminating in each of the nodes specified by the match_to specifications
 
         Return the number of links added; if none were added, or in case of error, raise an Exception.
 
         Notes:  - if a relationship with the same name already exists, nothing gets created (and an Exception is raised)
                 - more than 1 node could be present in either of the matches
 
         TODO: add a `rel_props` argument
               (Unclear what multiple calls would do in this case: update the props or create a new relationship??)
 
         :param match_from:  EITHER an integer with an internal database node id,
-                                OR a dictionary of data to identify a node, or set of nodes, as returned by match()
+                                OR a "NodeSpecs" object, as returned by match(), with data to identify a node or set of nodes
         :param match_to:    EITHER an integer with an internal database node id,
-                                OR a dictionary of data to identify a node, or set of nodes, as returned by match()
+                                OR a "NodeSpecs" object, as returned by match(), with data to identify a node or set of nodes
                             Note: match_from and match_to, if created by calls to match(),
-                                  in scenarios where a dummy name is used,
-                                  MUST use different node dummy names;
-                                  e.g., make sure that for match_from, match() used the option: dummy_node_name="from"
-                                                     and for match_to, match() used the option: dummy_node_name="to"
+                                  in scenarios where a clause dummy name is actually used,
+                                  MUST use different clause dummy names.
 
         :param rel_name:    The name to give to all the new relationships between the 2 specified nodes, or sets or nodes.
                                 Blanks allowed.
 
         :return:            The number of edges added.  If none got added, or in case of error, an Exception is raised
         """
-        # Create the "processed-match dictionaries"
-        match_from = CypherUtils.process_match_structure(match_from, dummy_node_name="from")
-        match_to   = CypherUtils.process_match_structure(match_to, dummy_node_name="to")
+        # Create the corresponding "CypherMatch" objects
+        cypher_match_from = CypherUtils.process_match_structure(match_from, dummy_node_name="from")
+        cypher_match_to   = CypherUtils.process_match_structure(match_to, dummy_node_name="to")
 
         if self.debug:
             print("In add_links()")
-            print("    match_from:", match_from)
-            print("    match_to:", match_to)
+            print("    cypher_match_from:", cypher_match_from)
+            print("    cypher_match_to:", cypher_match_to)
 
-        # Make sure there's no conflict in node dummy names
-        CypherUtils.check_match_compatibility(match_from, match_to)
+        # Unpack needed values from the cypher_match_from and cypher_match_to structures
+        nodes_from = cypher_match_from.extract_node()
+        nodes_to   = cypher_match_to.extract_node()
 
-        # Unpack needed values from the match_from and match_to structures
-        nodes_from = CypherUtils.extract_node(match_from)
-        nodes_to   = CypherUtils.extract_node(match_to)
+        # Combine the two WHERE clauses from each of the matches,
+        # and also prefix (if appropriate) the WHERE keyword
+        where_clause = CypherUtils.combined_where(cypher_match_from, cypher_match_to, check_compatibility=True)
 
-        where_clause = CypherUtils.combined_where([match_from, match_to])   # Combine the two WHERE clauses from each of the matches,
-                                                                            # and also prefix (if appropriate) the WHERE keyword
 
-        from_dummy_name = CypherUtils.extract_dummy_name(match_from)
-        to_dummy_name = CypherUtils.extract_dummy_name(match_to)
+        from_dummy_name = cypher_match_from.extract_dummy_name()
+        to_dummy_name = cypher_match_to.extract_dummy_name()
 
         # Prepare the query to add the requested links between the given nodes (possibly, sets of nodes)
         q = f'''
             MATCH {nodes_from}, {nodes_to}
             {where_clause}
             MERGE ({from_dummy_name}) -[:`{rel_name}`]-> ({to_dummy_name})           
             '''
 
         # Merge the data-binding dict's
-        combined_data_binding = CypherUtils.combined_data_binding([match_from, match_to])
+        combined_data_binding = CypherUtils.combined_data_binding(cypher_match_from, cypher_match_to)
 
         self.debug_query_print(q, combined_data_binding, "add_links")
 
         result = self.update_query(q, combined_data_binding)
         if self.debug:
             print("    RESULT of update_query in add_links(): ", result)
 
@@ -1755,38 +1752,36 @@
         if number_relationships_added == 0:       # This could be more than 1: see notes above
             raise Exception(f"add_links_fast(): the requested relationship ({rel_name}) was NOT added")
 
         return number_relationships_added
 
 
 
-    def remove_links(self, match_from: Union[int, dict], match_to: Union[int, dict], rel_name) -> int:
+    def remove_links(self, match_from: Union[int, NodeSpecs], match_to: Union[int, NodeSpecs], rel_name) -> int:
         """
         Remove one or more links (relationships, aka edges)
         originating in any of the nodes specified by the match_from specifications,
         and terminating in any of the nodes specified by the match_to specifications,
         optionally matching the given relationship name (will remove all edges if the name is blank or None)
 
         Return the number of edges removed; if none found, or in case of error, raise an Exception.
 
         Notes: - the nodes themselves are left untouched
                - more than 1 node could be present in either of the matches
                - the number of relationships deleted could be more than 1 even with a single "from" node and a single "to" node;
                         Neo4j allows multiple relationships with the same name between the same two nodes,
                         as long as the relationships differ in their properties
 
-        :param match_from:  EITHER an integer with a Neo4j node id,
-                                OR a dictionary of data to identify a node, or set of nodes, as returned by match()
-        :param match_to:    EITHER an integer with a Neo4j node id,
-                                OR a dictionary of data to identify a node, or set of nodes, as returned by match()
+        :param match_from:  EITHER an integer with an internal database node id,
+                                OR a "NodeSpecs" object, as returned by match(), with data to identify a node or set of nodes
+        :param match_to:    EITHER an integer with an internal database node id,
+                                OR a "NodeSpecs" object, as returned by match(), with data to identify a node or set of nodes
                             Note: match_from and match_to, if created by calls to match(),
-                                  in scenarios where a dummy name is used,
-                                  MUST use different node dummy names;
-                                  e.g., make sure that for match_from, match() used the option: dummy_node_name="from"
-                                                     and for match_to, match() used the option: dummy_node_name="to"
+                                  in scenarios where a clause dummy name is actually used,
+                                  MUST use different clause dummy names.
 
         :param rel_name:    (OPTIONAL) The name of the relationship to delete between the 2 specified nodes;
                                 if None or a blank string, all relationships between those 2 nodes will get deleted.
                                 Blanks allowed.
 
         :return:            The number of edges removed.  If none got deleted, or in case of error, an Exception is raised
         """
@@ -1795,23 +1790,22 @@
         match_to   = CypherUtils.process_match_structure(match_to, dummy_node_name="to")
 
         if self.debug:
             print("In remove_links()")
             print("    match_from:", match_from)
             print("    match_to:", match_to)
 
-        # Make sure there's no conflict in node dummy names
-        CypherUtils.check_match_compatibility(match_from, match_to)
-
         # Unpack needed values from the match_from and match_to structures
-        nodes_from = CypherUtils.extract_node(match_from)
-        nodes_to   = CypherUtils.extract_node(match_to)
+        nodes_from = match_from.extract_node()
+        nodes_to   = match_to.extract_node()
+
+        # Combine the two WHERE clauses from each of the matches,
+        # and also prefix (if appropriate) the WHERE keyword
+        where_clause = CypherUtils.combined_where(match_from, match_to, check_compatibility=True)
 
-        where_clause = CypherUtils.combined_where([match_from, match_to])   # Combine the two WHERE clauses from each of the matches,
-                                                                            # and also prefix (if appropriate) the WHERE keyword
         # Prepare the query
         if rel_name is None or rel_name == "":  # Delete ALL relationships
             q = f'''
                 MATCH {nodes_from} -[r]-> {nodes_to}
                 {where_clause}
                 DELETE r           
                 '''
@@ -1819,15 +1813,15 @@
             q = f'''
                 MATCH {nodes_from} -[r :`{rel_name}`]-> {nodes_to}
                 {where_clause}
                 DELETE r           
                 '''
 
         # Merge the data-binding dict's
-        combined_data_binding = CypherUtils.combined_data_binding([match_from, match_to])
+        combined_data_binding = CypherUtils.combined_data_binding(match_from, match_to)
 
         self.debug_query_print(q, combined_data_binding, "remove_links")
 
         result = self.update_query(q, combined_data_binding)
         if self.debug:
             print("    result of update_query in remove_links: ", result)
 
@@ -1835,85 +1829,80 @@
         if number_relationships_deleted == 0:       # This could be more than 1: see notes above
             raise Exception("remove_links(): no relationship was deleted")
 
         return number_relationships_deleted
 
 
 
-    def links_exist(self, match_from: Union[int, dict], match_to: Union[int, dict], rel_name: str) -> bool:
+    def links_exist(self, match_from: Union[int, NodeSpecs], match_to: Union[int, NodeSpecs], rel_name: str) -> bool:
         """
         Return True if one or more edges (relationships) with the specified name exist in the direction
         from and to the nodes (individual nodes or set of nodes) specified in the first two arguments.
         Typically used to find whether 2 given nodes have a direct link between them.
 
-        :param match_from:  EITHER an integer with a Neo4j node id,
-                                OR a dictionary of data to identify a node, or set of nodes, as returned by match()
-        :param match_to:    EITHER an integer with a Neo4j node id,
-                                OR a dictionary of data to identify a node, or set of nodes, as returned by match()
+        :param match_from:  EITHER an integer with an internal database node id,
+                                OR a "NodeSpecs" object, as returned by match(), with data to identify a node or set of nodes
+        :param match_to:    EITHER an integer with an internal database node id,
+                                OR a "NodeSpecs" object, as returned by match(), with data to identify a node or set of nodes
                             Note: match_from and match_to, if created by calls to match(),
-                                  in scenarios where a dummy name is used,
-                                  MUST use different node dummy names;
-                                  e.g., make sure that for match_from, match() used the option: dummy_node_name="from"
-                                                     and for match_to, match() used the option: dummy_node_name="to"
+                                  in scenarios where a clause dummy name is actually used,
+                                  MUST use different clause dummy names.
 
         :param rel_name:    The name of the relationship to look for between the 2 specified nodes.
                                 Blanks are allowed
 
         :return:            True if one or more relationships were found, or False if not
         """
         return self.number_of_links(match_from=match_from, match_to=match_to, rel_name=rel_name) >= 1   # True if at least 1
 
 
 
-    def number_of_links(self, match_from: Union[int, dict], match_to: Union[int, dict], rel_name: str) -> int:
+    def number_of_links(self, match_from: Union[int, NodeSpecs], match_to: Union[int, NodeSpecs], rel_name: str) -> int:
         """
         Return the number of links (aka edges, relationships) with the specified name exist in the direction
         from and to the nodes (individual nodes or set of nodes) specified in the first two arguments.
 
-        :param match_from:  EITHER an integer with a Neo4j node id,
-                                OR a dictionary of data to identify a node, or set of nodes, as returned by match()
-        :param match_to:    EITHER an integer with a Neo4j node id,
-                                OR a dictionary of data to identify a node, or set of nodes, as returned by match()
+        :param match_from:  EITHER an integer with an internal database node id,
+                                OR a "NodeSpecs" object, as returned by match(), with data to identify a node or set of nodes
+        :param match_to:    EITHER an integer with an internal database node id,
+                                OR a "NodeSpecs" object, as returned by match(), with data to identify a node or set of nodes
                             Note: match_from and match_to, if created by calls to match(),
-                                  in scenarios where a dummy name is used,
-                                  MUST use different node dummy names;
-                                  e.g., make sure that for match_from, match() used the option: dummy_node_name="from"
-                                                     and for match_to, match() used the option: dummy_node_name="to"
+                                  in scenarios where a clause dummy name is actually used,
+                                  MUST use different clause dummy names.
 
         :param rel_name:    The name of the relationship to look for between the 2 specified nodes or groups of nodes.
                                 Blanks are allowed
 
         :return:            The number of links (relationships) that were found
         """
         match_from = CypherUtils.process_match_structure(match_from, dummy_node_name="from")
         match_to   = CypherUtils.process_match_structure(match_to, dummy_node_name="to")
 
         if self.debug:
             print("In number_of_links()")
             print("    match_from:", match_from)
             print("    match_to:", match_to)
 
-        # Make sure there's no conflict in the dummy node names
-        CypherUtils.check_match_compatibility(match_from, match_to)
-
         # Unpack needed values from the match_from and match_to structures
-        nodes_from = CypherUtils.extract_node(match_from)
-        nodes_to   = CypherUtils.extract_node(match_to)
+        nodes_from = match_from.extract_node()
+        nodes_to   = match_to.extract_node()
+
+        # Combine the two WHERE clauses from each of the matches,
+        # and also prefix (if appropriate) the WHERE keyword
+        where_clause = CypherUtils.combined_where(match_from, match_to, check_compatibility=True)
 
-        where_clause = CypherUtils.combined_where([match_from, match_to])   # Combine the two WHERE clauses from each of the matches,
-                                                                            # and also prefix (if appropriate) the WHERE keyword
         # Prepare the query
         q = f'''
             MATCH {nodes_from} -[r :`{rel_name}`]-> {nodes_to}
             {where_clause} 
             RETURN r          
             '''
 
         # Merge the data-binding dict's
-        combined_data_binding = CypherUtils.combined_data_binding([match_from, match_to])
+        combined_data_binding = CypherUtils.combined_data_binding(match_from, match_to)
 
         self.debug_query_print(q, combined_data_binding, "number_of_links")
 
         result = self.query(q, combined_data_binding)
         if self.debug:
             print("    result of query in number_of_links(): ", result)
 
@@ -1932,19 +1921,19 @@
         :param old_attachment:  An integer with the internal database ID of the other node currently connected to
         :param new_attachment:  An integer with the internal database ID of the new node to connect to
         :param rel_name:        Name of the old relationship name
         :param rel_name_new:    (OPTIONAL) Name of the new relationship name (by default the same as the old one)
 
         :return:                None.  If unsuccessful, an Exception is raised
         """
-        assert CypherUtils.validate_internal_id(node), \
+        assert CypherUtils.valid_internal_id(node), \
             f"reattach_node(): not a valid internal database ID ({node})"
-        assert CypherUtils.validate_internal_id(old_attachment), \
+        assert CypherUtils.valid_internal_id(old_attachment), \
             f"reattach_node(): not a valid internal database ID ({old_attachment})"
-        assert CypherUtils.validate_internal_id(new_attachment), \
+        assert CypherUtils.valid_internal_id(new_attachment), \
             f"reattach_node(): not a valid internal database ID ({new_attachment})"
 
         if rel_name_new is None:
             rel_name_new = rel_name     # Use the default value, if not provided
 
         q = f'''
             MATCH (node_start) -[rel :{rel_name}]-> (node_old), (node_new)
@@ -2043,37 +2032,37 @@
     '''                                    ~   FOLLOW LINKS   ~                                        '''
 
     def ________FOLLOW_LINKS________(DIVIDER):
         pass        # Used to get a better structure view in IDEs
     #####################################################################################################
 
 
-    def follow_links(self, match: Union[int, dict], rel_name: str, rel_dir ="OUT", neighbor_labels = None) -> [dict]:
+    def follow_links(self, match: Union[int, NodeSpecs], rel_name: str, rel_dir ="OUT", neighbor_labels = None) -> [dict]:
         """
         From the given starting node(s), follow all the relationships of the given name to and/or from it,
         into/from neighbor nodes (optionally having the given labels),
         and return all the properties of those neighbor nodes.
 
-        :param match:           EITHER an integer with a Neo4j node id,
-                                    OR a dictionary of data to identify a node, or set of nodes, as returned by match()
+        :param match:           EITHER an integer with an internal database node id,
+                                    OR a "NodeSpecs" object, as returned by match(), with data to identify a node or set of nodes
         :param rel_name:        A string with the name of relationship to follow.  (Note: any other relationships are ignored)
         :param rel_dir:         Either "OUT"(default), "IN" or "BOTH".  Direction(s) of the relationship to follow
         :param neighbor_labels: Optional label(s) required on the neighbors.  If present, either a string or list of strings
 
         :return:                A list of dictionaries with all the properties of the neighbor nodes
                                 TODO: maybe add the option to just return a subset of fields
         """
         match_structure = CypherUtils.process_match_structure(match)
 
         if self.debug:
             print("In follow_links()")
             print("    match_structure:", match_structure)
 
         # Unpack needed values from the match dictionary
-        (node, where, data_binding) = CypherUtils.unpack_match(match_structure, include_dummy=False)
+        (node, where, data_binding, _) = match_structure.unpack_match()
 
         neighbor_labels_str = CypherUtils.prepare_labels(neighbor_labels)     # EXAMPLE:  ":`CAR`:`INVENTORY`"
 
         if rel_dir == "OUT":    # Follow outbound links
             q =  f"MATCH {node} - [:{rel_name}] -> (neighbor {neighbor_labels_str})"
         elif rel_dir == "IN":   # Follow inbound links
             q =  f"MATCH {node} <- [:{rel_name}] - (neighbor {neighbor_labels_str})"
@@ -2087,35 +2076,35 @@
 
         result = self.query(q, data_binding, single_column='neighbor')
 
         return result
 
 
 
-    def count_links(self, match: Union[int, dict], rel_name: str, rel_dir="OUT", neighbor_labels = None) -> int:
+    def count_links(self, match: Union[int, NodeSpecs], rel_name: str, rel_dir="OUT", neighbor_labels = None) -> int:
         """
         From the given starting node(s), count all the relationships OF THE GIVEN NAME to and/or from it,
         into/from neighbor nodes (optionally having the given labels)
 
-        :param match:           EITHER an integer with a Neo4j node id,
-                                    OR a dictionary of data to identify a node, or set of nodes, as returned by match()
+        :param match:           EITHER an integer with an internal database node id,
+                                    OR a "NodeSpecs" object, as returned by match(), with data to identify a node or set of nodes
         :param rel_name:        A string with the name of relationship to follow.  (Note: any other relationships are ignored)
         :param rel_dir:         Either "OUT"(default), "IN" or "BOTH".  Direction(s) of the relationship to follow
         :param neighbor_labels: Optional label(s) required on the neighbors.  If present, either a string or list of strings
 
         :return:                The total number of inbound and/or outbound relationships to the given node(s)
         """
         match_structure = CypherUtils.process_match_structure(match)
 
         if self.debug:
             print("In count_links()")
             print("    match_structure:", match_structure)
 
         # Unpack needed values from the match dictionary
-        (node, where, data_binding) = CypherUtils.unpack_match(match_structure, include_dummy=False)
+        (node, where, data_binding, _) = match_structure.unpack_match()
 
         neighbor_labels_str = CypherUtils.prepare_labels(neighbor_labels)     # EXAMPLE:  ":`CAR`:`INVENTORY`"
 
         if rel_dir == "OUT":            # Follow outbound links
             q =  f"MATCH {node} - [:{rel_name}] -> (neighbor {neighbor_labels_str})"
         elif rel_dir == "IN":           # Follow inbound links
             q =  f"MATCH {node} <- [:{rel_name}] - (neighbor {neighbor_labels_str})"
@@ -2314,20 +2303,20 @@
         then the given pair (label, key) is checked against ("l1_l2", "p1_p2"), to decide whether it already exists.
 
         :param label:   A string with the node label to which the index is to be applied
         :param key:     A string with the key (property) name to which the index is to be applied
         :return:        True if a new index was created, or False otherwise
         """
         existing_indexes = self.get_indexes()   # A Pandas dataframe with info about indexes;
-                                                #       in particular 2 columns named "labelsOrTypes" and "properties"
+        #       in particular 2 columns named "labelsOrTypes" and "properties"
 
         # Index is created if not already exists.
         # a standard name for the index is assigned: `{label}.{key}`
         existing_standard_name_pairs = list(existing_indexes.apply(
-                lambda x: ("_".join(x['labelsOrTypes']), "_".join(x['properties'])), axis=1))   # Proceed by row
+            lambda x: ("_".join(x['labelsOrTypes']), "_".join(x['properties'])), axis=1))   # Proceed by row
         """
         For example, if the Pandas dataframe existing_indexes contains the following columns: 
                             labelsOrTypes     properties
                 0                   [car]  [color, make]
                 1                [person]          [sex]
                 
         then existing_standard_names will be:  [('car', 'color_make'), ('person', 'sex')]
@@ -2530,15 +2519,15 @@
         pass        # Used to get a better structure view in IDEs
     #####################################################################################################
 
 
     def export_dbase_json(self) -> {}:
         """
         Export the entire Neo4j database as a JSON string.
-        TODO: offer an option to automatically include today's date in name of exported file
+        TODO: offer an option to automatically include today's date in the name of exported file
 
         IMPORTANT: APOC must be activated in the database, to use this function.
                    Otherwise it'll raise an Exception
 
         EXAMPLE:
         { 'nodes': 2,
           'relationships': 1,
@@ -2581,15 +2570,15 @@
             YIELD nodes, relationships, properties, data
             RETURN nodes, relationships, properties, data
             '''
         # TODO: unclear if the part "useTypes: true" is needed
 
         result = self.query(cypher)     # It returns a list with a single element
         export_dict = result[0]         # This will be a dictionary with 4 keys: "nodes", "relationships", "properties", "data"
-                                        #   "nodes", "relationships" and "properties" contain their respective counts
+        #   "nodes", "relationships" and "properties" contain their respective counts
 
         json_lines = export_dict["data"]
         # Tweak the "JSON_LINES" format to make it a valid JSON string, and more readable.
         # See https://neo4j.com/labs/apoc/4.3/export/json/#export-nodes-relationships-json
         json_str = "[" + json_lines.replace("\n", ",\n ") + "\n]"   # The newlines \n make the JSON much more human-readable
         export_dict["data"] = json_str                              # Replace the "data" value
 
@@ -2652,15 +2641,15 @@
         '''
 
         #self.debug_print(cypher, method="export_nodes_rels_json", force_output=True)
         result = self.query(cypher)     # It returns a list with a single element
         #print("In export_nodes_rels_json(): result = ", result)
 
         export_dict = result[0]     # This will be a dictionary with 4 keys: "nodes", "relationships", "properties", "data"
-                                    #   "nodes", "relationships" and "properties" contain their respective counts
+        #   "nodes", "relationships" and "properties" contain their respective counts
 
         json_lines = export_dict["data"]
         # Tweak the "JSON_LINES" format to make it a valid JSON string, and more readable.
         # See https://neo4j.com/labs/apoc/4.3/export/json/#export-nodes-relationships-json
         json_str = "[" + json_lines.replace("\n", ",\n ") + "\n]"       # The newlines \n make the JSON much more human-readable
         export_dict["data"] = json_str                                  # Replace the "data" value
 
@@ -2701,15 +2690,15 @@
                                 (only used if the top-level JSON structure is an object, i.e. if there's a single root node)
 
         :return:            List of integer ID's (possibly empty), of the root node(s) created
         """
         # Try to obtain Python data (which ought to be a dict or list) that corresponds to the passed JSON string
         try:
             json_data = json.loads(json_str)    # Turn the string (representing JSON data) into its Python counterpart;
-                                                # at the top level, it should be a dict or list
+            # at the top level, it should be a dict or list
         except Exception as ex:
             raise Exception(f"Incorrectly-formatted JSON string. {ex}")
 
         #print("Python version of the JSON file:\n"
         #self.debug_trim_print(json_data, max_len = 250)
 
         if parse_only:
@@ -2754,15 +2743,15 @@
 
         # If the data is a literal, first turn it into a dictionary using a key named "value"
         if self.is_literal(python_data):
             # The data is a literal
             original_data = python_data             # Only used for debug-printing, below
             python_data = {"value": python_data}    # Turn the literal data into a dictionary
             self.debug_print(f"{indent_str}Turning literal ({self.debug_trim(original_data, max_len=200)}) into dict, "
-                  f"using `value` as key, as follows: {self.debug_trim(python_data)}")
+                             f"using `value` as key, as follows: {self.debug_trim(python_data)}")
 
         if type(python_data) == dict:
             self.debug_print(f"{indent_str}Input is a dict with {len(python_data)} key(s): {list(python_data.keys())}")
             new_root_id = self.dict_importer(d=python_data, labels=root_labels, level=level)
             self.debug_print(f"{indent_str}dict_importer returned new_root_id: {new_root_id}")
             return [new_root_id]
 
@@ -2898,15 +2887,15 @@
             print("json_list: ", json_list)
 
         assert type(json_list) == list, \
             "import_json_dump(): the JSON string does not represent a list"
 
 
         id_shifting = {}    # To map the Neo4j internal ID's specified in the JSON data dump
-                            #       into the ID's of newly-created nodes
+        #       into the ID's of newly-created nodes
 
         if extended_validation:
             # Do an initial pass for correctness, to help avoid partial imports.
             # TODO: maybe also check the validity of the start and end nodes of relationships
             for i, item in enumerate(json_list):
                 assert type(item) == dict, \
                     f"import_json_dump(): Item in list index {i} should be a dict, but instead it's of type {type(item)}.  Nothing imported.  Item: {item}"
@@ -2941,15 +2930,16 @@
         num_nodes_imported = 0
         try:
             for item in json_list:
                 if item["type"] == "node":
                     #print("ADDING NODE: ", item)
                     #print(f'     Creating node with labels `{item["labels"]}` and properties {item["properties"]}')
                     old_id = int(item["id"])
-                    new_id = self.create_node(item["labels"], item["properties"])  # Note: any number of labels can be imported
+                    new_id = self.create_node(labels=item.get("labels"), properties=item.get("properties")) # Note: any number of labels can be imported
+                                                                                                            #       if item has no labels/properties, None will be passed
                     id_shifting[old_id] = new_id
                     num_nodes_imported += 1
         except Exception as ex:
             raise Exception(f"import_json_dump(): the import process was INTERRUPTED "
                             f"after importing {num_nodes_imported} node(s) and 0 relationship(s). Reason: " + str(ex))
 
 
@@ -3093,7 +3083,8 @@
     def _debug_local(self) -> str:
         """
         Use to test the switch from a local to remote repository, for debugging
 
         :return:
         """
         return "local"
+
```

### Comparing `neoaccess-4.2.0/PKG-INFO` & `neoaccess-4.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neoaccess
-Version: 4.2.0
+Version: 4.3.1
 Summary: High-level interface to the Neo4j graph database
 Project-URL: Bug Tracker, https://github.com/BrainAnnex/brain-annex/issues
 Project-URL: Documentation, https://brainannex.org/guide.php
 Project-URL: Home-page, https://brainannex.org/guide.php
 Project-URL: Homepage, https://brainannex.org/guide.php
 Project-URL: Source, https://github.com/BrainAnnex/neoaccess
 Author: Julian West BrainAnnex.org
@@ -15,14 +15,19 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: neo4j==4.4.11
 Requires-Dist: numpy~=1.22.4
 Requires-Dist: pandas~=1.4.3
 Description-Content-Type: text/markdown
 
-# High-level interface to the Neo4j graph database    
+# High-level python interface to the Neo4j graph database
 
 https://brainannex.org/guide.php
 
 
-This library used to be distributed together with the web app "Brain Annex";
-but, starting with version 4.0.3, it's being independently released.
+This library used to be distributed as part of the full technology stack "Brain Annex";
+but, starting with version 4.0.3, it's being independently released.
+
+To use it, just `pip install neoaccess`
+
+
+[Intro and tutorial](https://julianspolymathexplorations.blogspot.com/2023/06/neo4j-python-neoaccess-library.html)
```

