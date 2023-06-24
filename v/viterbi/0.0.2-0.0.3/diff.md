# Comparing `tmp/viterbi-0.0.2.tar.gz` & `tmp/viterbi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viterbi-0.0.2.tar", last modified: Wed Jun 21 08:21:34 2023, max compression
+gzip compressed data, was "viterbi-0.0.3.tar", last modified: Sat Jun 24 09:22:07 2023, max compression
```

## Comparing `viterbi-0.0.2.tar` & `viterbi-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:21:34.003274 viterbi-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 08:21:25.000000 viterbi-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 08:21:25.000000 viterbi-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16586 2023-06-21 08:21:34.003274 viterbi-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-21 08:21:25.000000 viterbi-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-21 08:21:25.000000 viterbi-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 08:21:34.003274 viterbi-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-21 08:21:25.000000 viterbi-0.0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-21 08:21:25.000000 viterbi-0.0.2/viterbi.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:21:34.003274 viterbi-0.0.2/viterbi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16586 2023-06-21 08:21:33.000000 viterbi-0.0.2/viterbi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-21 08:21:33.000000 viterbi-0.0.2/viterbi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:21:33.000000 viterbi-0.0.2/viterbi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 08:21:33.000000 viterbi-0.0.2/viterbi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-06-21 08:21:25.000000 viterbi-0.0.2/viterbi.h
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-21 08:21:25.000000 viterbi-0.0.2/viterbi.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-21 08:21:25.000000 viterbi-0.0.2/viterbi_python.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:22:07.248939 viterbi-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-24 09:21:57.000000 viterbi-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-24 09:21:57.000000 viterbi-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14540 2023-06-24 09:22:07.248939 viterbi-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-24 09:21:57.000000 viterbi-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-24 09:21:57.000000 viterbi-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 09:22:07.248939 viterbi-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-24 09:21:57.000000 viterbi-0.0.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-06-24 09:21:57.000000 viterbi-0.0.3/viterbi.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:22:07.244939 viterbi-0.0.3/viterbi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14540 2023-06-24 09:22:07.000000 viterbi-0.0.3/viterbi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-24 09:22:07.000000 viterbi-0.0.3/viterbi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 09:22:07.000000 viterbi-0.0.3/viterbi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-24 09:22:07.000000 viterbi-0.0.3/viterbi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-24 09:21:57.000000 viterbi-0.0.3/viterbi.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-24 09:21:57.000000 viterbi-0.0.3/viterbi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-24 09:21:57.000000 viterbi-0.0.3/viterbi_python.cpp
```

### Comparing `viterbi-0.0.2/LICENSE` & `viterbi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `viterbi-0.0.2/PKG-INFO` & `viterbi-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viterbi
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Convolutional Encoder and Viterbi Decoder in Python/C++.
 Author-email: Yachen Mao <maoyachen55@gmail.com>, Min Xu <xukmin@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -206,154 +206,46 @@
            limitations under the License.
         
 Keywords: viterbi
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Convolutional Encoder and Viterbi Decoder
-=========================================
+# Convolutional Encoder and Viterbi Decoder
 
-Author: Min Xu &lt;xukmin@gmail.com&gt;
+> This project is a fork of <https://github.com/xukmin/viterbi> that introduces Python support, enabling effortless utilization of the Viterbi module within the Python environment.
 
-This program implements both a Convolutional Encoder and a Viterbi Decoder in C++.
+## Install
 
-Running ViterbiCodec
---------------------
-
-Compile:
-
-```bash
-make
-```
-
-Run:
-
-```bash
-./viterbi_main <constraint> <polynomial>... <bits>
-```
-
-Example use:
-
-Decoding:
-
-```bash
-./viterbi_main 3 7 5 0011100001100111111000101100111011
-010111001010001
-```
-
-Encoding:
-
-```bash
-$ ./viterbi_main 3 7 5 --encode 010111001010001
-0011100001100111111000101100111011
+```sh
+pip install viterbi
 ```
 
-Please note there are `(constraint - 1)` "0" bits padded in front of the original message.
-
-More Features
--------------
-
-- It supports reading input from stdin or from commandline arguments. When
-  reading from stdin, it ignores blank lines or comment lines (which start with
-  `#`).
+## Usage
 
-- It supports any number of generator polynomials.
+The following is a convolutional encoder with a constraint length of 7. The diagram indicates the binary values and polynomial form, indicating the left-most bit is the most-significant-bit (MSB). The generating polynomials are 1011011 and 1111001 can be alternatively expressed in octal as 133 and 171, respectively.
 
-- It can perform convolutional encoding by providing `--encode` commandline
-  flag.
+![convolutional encoder](docs/convolutional%20encoder.svg)
 
-- It supports a different notation of generator polynomials by providing
-  `--reverse_polynomials` commandline flag.
+Expressed in code as:
 
-Here are more options to run the program.
-
-Show help message:
-
-```bash
-./viterbi_main --help
+```python
+from viterbi import Viterbi
+dot11a_codec = Viterbi(7, [0o133, 0o171])
 ```
 
-Read input from stdin:
-
-```bash
-./viterbi_main [--reverse_polynomials] [--encode]
-```
-
-Input format is:
-
-```
-<constraint> <polynomial>... <bits>
-```
+You can use the viterbi decoder like this:
 
-Read input from commandline arguments:
+```python
+from viterbi import Viterbi
 
-```bash
-./viterbi_main [--reverse_polynomials] [--encode] <constraint> <polynomial>... <bits>
+dot11a_codec = Viterbi(7, [0o133, 0o171])
+bits = [0, 1, 0, 1, 0, 0, 0, 0, 1, 1, 1, 0]
+output = dot11a_codec.encode(bits)
+# [0, 0, 1, 1, 0, 1, 0, 0, 1, 0, 1, 1, 0, 1, 1, 1, 0, 1, 0, 1, 0, 1, 0, 1]
+dot11a_codec.decode(output)
+# [0, 1, 0, 1, 0, 0, 0, 0, 1, 1, 1, 0]
 ```
 
-Flags:
-
-```bash
---reverse_polynomials
-    Reverse polynomials. E.g. 6 (=0b110) becomes 3 (=0b011).
-
---encode
-    Do encoding instead of decoding.
-```
-
-Example usage:
-
-```bash
-./viterbi_main 3 7 5 0011100001100111111000101100111011
-./viterbi_main 3 6 5 111011011100101011
-./viterbi_main 7 91 121 1010110100001101001000011101
-./viterbi_main 7 91 117 121 111100101110001011110101111111001011100111
-./viterbi_main --reverse_polynomials 3 3 5 111011011100101011
-./viterbi_main --encode 3 7 5 010111001010001
-./viterbi_main --encode 3 6 5 1001101
-./viterbi_main --encode --reverse_polynomials 3 3 5 1001101
-```
-
-Error Handling
---------------
-
-All inputs are validated, and proper error messages will be output.
-
-- The `constraint` should be greater than `0`.
-- A generator polynomial should be greater than `0` and less than
-  `1 << constraint`.
-- The received bit sequence should be consisted with only `0` and `1`.
-- The received bit sequence should be of length `N * <num-of-polynomials>` where
-  `N` is an integer. Otherwise some bits must be missing during transmission.
-  We will fill in appropriate number of trailing zeros.
-
-Running Unit Test
------------------
-
-Run unit test:
-
-```bash
-make test
-```
-
-Or
-
-```bash
-make viterbi_test && ./viterbi_test
-```
-
-If the test passes, it will output `PASSED` and the end of the output;
-otherwise, the test program aborts with assertion error.
-
-There are a few sample cases in the unit test, some are with manually injected
-bit errors.
-
-It also generates random messages of length `8`, `16` and `32` for several different
-convolutional codes and test if they can be properly encoded and decoded.
-
-Dependencies
-------------
-
-The code is self-contained, meaning it depends on nothing but the C++ standard
-library. The purpose is to make it easy to be integrated in any project.
+## Using in C++
 
+You can find the way to use the Viterbi decoder in C++ in the [README](https://github.com/xukmin/viterbi) of the original project.
```

### Comparing `viterbi-0.0.2/pyproject.toml` & `viterbi-0.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "pybind11"]
 build-backend = "setuptools.build_meta"
 
 [project]
-version = "0.0.2"
+version = "0.0.3"
 name = "viterbi"
 authors = [
     {name = "Yachen Mao", email = "maoyachen55@gmail.com"},
     {name = "Min Xu", email = "xukmin@gmail.com"},
 ]
 description = "A Convolutional Encoder and Viterbi Decoder in Python/C++."
 readme = "README.md"
```

### Comparing `viterbi-0.0.2/viterbi.cpp` & `viterbi-0.0.3/viterbi.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -15,22 +15,25 @@
 
 namespace {
 
 int HammingDistance(const std::string& x, const std::string& y) {
   assert(x.size() == y.size());
   int distance = 0;
   for (int i = 0; i < x.size(); i++) {
+    if (x.at(i) == '-' || y.at(i) == '-') {
+      continue;
+    }
     distance += x[i] != y[i];
   }
   return distance;
 }
 
 }  // namespace
 
-std::ostream& operator <<(std::ostream& os, const ViterbiCodec& codec) {
+std::ostream& operator<<(std::ostream& os, const ViterbiCodec& codec) {
   os << "ViterbiCodec(" << codec.constraint() << ", {";
   const std::vector<int>& polynomials = codec.polynomials();
   assert(!polynomials.empty());
   os << polynomials.front();
   for (int i = 1; i < polynomials.size(); i++) {
     os << ", " << polynomials[i];
   }
@@ -43,27 +46,28 @@
   while (num_bits-- > 0) {
     output = (output << 1) + (input & 1);
     input >>= 1;
   }
   return output;
 }
 
-ViterbiCodec::ViterbiCodec(int constraint, const std::vector<int>& polynomials)
-    : constraint_(constraint), polynomials_(polynomials) {
+ViterbiCodec::ViterbiCodec(int constraint, const std::vector<int>& polynomials, const std::string& puncpat)
+    : constraint_(constraint), polynomials_(polynomials), puncpat_(puncpat) {
   assert(!polynomials_.empty());
   for (int i = 0; i < polynomials_.size(); i++) {
     assert(polynomials_[i] > 0);
     assert(polynomials_[i] < (1 << constraint_));
   }
   InitializeOutputs();
 }
 
-int ViterbiCodec::num_parity_bits() const {
-  return polynomials_.size();
-}
+ViterbiCodec::ViterbiCodec(int constraint, const std::vector<int>& polynomials)
+    : ViterbiCodec(constraint, polynomials, "") {}
+
+int ViterbiCodec::num_parity_bits() const { return polynomials_.size(); }
 
 int ViterbiCodec::NextState(int current_state, int input) const {
   return (current_state >> 1) | (input << (constraint_ - 2));
 }
 
 std::string ViterbiCodec::Output(int current_state, int input) const {
   return outputs_.at(current_state | (input << (constraint_ - 1)));
@@ -79,17 +83,21 @@
     assert(c == '0' || c == '1');
     int input = c - '0';
     encoded += Output(state, input);
     state = NextState(state, input);
   }
 
   // Encode (constaint_ - 1) flushing bits.
-  for (int i = 0; i < constraint_ - 1; i++) {
-    encoded += Output(state, 0);
-    state = NextState(state, 0);
+  // for (int i = 0; i < constraint_ - 1; i++) {
+  //   encoded += Output(state, 0);
+  //   state = NextState(state, 0);
+  // }
+
+  if (puncpat_.size() > 0) {
+    return Puncturing(encoded);
   }
 
   return encoded;
 }
 
 void ViterbiCodec::InitializeOutputs() {
   outputs_.resize(1 << constraint_);
@@ -105,29 +113,24 @@
         input >>= 1;
       }
       outputs_[i] += output ? "1" : "0";
     }
   }
 }
 
-int ViterbiCodec::BranchMetric(const std::string& bits,
-                               int source_state,
-                               int target_state) const {
+int ViterbiCodec::BranchMetric(const std::string& bits, int source_state, int target_state) const {
   assert(bits.size() == num_parity_bits());
   assert((target_state & ((1 << (constraint_ - 2)) - 1)) == source_state >> 1);
-  const std::string output =
-      Output(source_state, target_state >> (constraint_ - 2));
+  const std::string output = Output(source_state, target_state >> (constraint_ - 2));
 
   return HammingDistance(bits, output);
 }
 
-std::pair<int, int> ViterbiCodec::PathMetric(
-    const std::string& bits,
-    const std::vector<int>& prev_path_metrics,
-    int state) const {
+std::pair<int, int> ViterbiCodec::PathMetric(const std::string& bits, const std::vector<int>& prev_path_metrics,
+                                             int state) const {
   int s = (state & ((1 << (constraint_ - 2)) - 1)) << 1;
   int source_state1 = s | 0;
   int source_state2 = s | 1;
 
   int pm1 = prev_path_metrics[source_state1];
   if (pm1 < std::numeric_limits<int>::max()) {
     pm1 += BranchMetric(bits, source_state1, state);
@@ -140,53 +143,84 @@
   if (pm1 <= pm2) {
     return std::make_pair(pm1, source_state1);
   } else {
     return std::make_pair(pm2, source_state2);
   }
 }
 
-void ViterbiCodec::UpdatePathMetrics(const std::string& bits,
-                                     std::vector<int>* path_metrics,
-                                     Trellis* trellis) const {
+void ViterbiCodec::UpdatePathMetrics(const std::string& bits, std::vector<int>* path_metrics, Trellis* trellis) const {
   std::vector<int> new_path_metrics(path_metrics->size());
   std::vector<int> new_trellis_column(1 << (constraint_ - 1));
   for (int i = 0; i < path_metrics->size(); i++) {
     std::pair<int, int> p = PathMetric(bits, *path_metrics, i);
     new_path_metrics[i] = p.first;
     new_trellis_column[i] = p.second;
   }
 
   *path_metrics = new_path_metrics;
   trellis->push_back(new_trellis_column);
 }
 
 std::string ViterbiCodec::Decode(const std::string& bits) const {
+  std::string depunctured;
+  if (puncpat_.size() > 0) {
+    depunctured = Depuncturing(bits) + std::string(num_parity_bits() * (constraint_ - 1), '0');
+  } else {
+    depunctured = bits + std::string(num_parity_bits() * (constraint_ - 1), '0');
+  }
   // Compute path metrics and generate trellis.
   Trellis trellis;
-  std::vector<int> path_metrics(1 << (constraint_ - 1),
-                                std::numeric_limits<int>::max());
+  std::vector<int> path_metrics(1 << (constraint_ - 1), std::numeric_limits<int>::max());
   path_metrics.front() = 0;
-  for (int i = 0; i < bits.size(); i += num_parity_bits()) {
-    std::string current_bits(bits, i, num_parity_bits());
+  for (int i = 0; i < depunctured.size(); i += num_parity_bits()) {
+    std::string current_bits(depunctured, i, num_parity_bits());
     // If some bits are missing, fill with trailing zeros.
     // This is not ideal but it is the best we can do.
     if (current_bits.size() < num_parity_bits()) {
-      current_bits.append(
-          std::string(num_parity_bits() - current_bits.size(), '0'));
+      current_bits.append(std::string(num_parity_bits() - current_bits.size(), '0'));
     }
     UpdatePathMetrics(current_bits, &path_metrics, &trellis);
   }
 
   // Traceback.
   std::string decoded;
-  int state = std::min_element(path_metrics.begin(), path_metrics.end()) -
-              path_metrics.begin();
+  int state = std::min_element(path_metrics.begin(), path_metrics.end()) - path_metrics.begin();
   for (int i = trellis.size() - 1; i >= 0; i--) {
     decoded += state >> (constraint_ - 2) ? "1" : "0";
     state = trellis[i][state];
   }
   std::reverse(decoded.begin(), decoded.end());
 
   // Remove (constraint_ - 1) flushing bits.
   return decoded.substr(0, decoded.size() - constraint_ + 1);
 }
 
+std::string ViterbiCodec::Puncturing(const std::string bits) const {
+  std::string punctured;
+  int index = 0;
+  for (int i = 0; i < bits.size(); i++) {
+    if (puncpat_.at(index) == '1') punctured += bits[i];
+    index = (index + 1) % puncpat_.size();
+  }
+  return punctured;
+}
+
+std::string ViterbiCodec::Depuncturing(const std::string bits) const {
+  std::string depunctured;
+  int index = 0;
+  int i = 0;
+  while (index < bits.size()) {
+    for (int j = 0; j < puncpat_.size(); j++) {
+      if (puncpat_.at(j) == '1') {
+        if (index >= bits.size()) {
+          depunctured += "0";
+        } else {
+          depunctured += bits[index++];
+        }
+      } else {
+        depunctured += "-";
+      }
+    }
+    i += puncpat_.size();
+  }
+  return depunctured;
+}
```

### Comparing `viterbi-0.0.2/viterbi.egg-info/PKG-INFO` & `viterbi-0.0.3/viterbi.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viterbi
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Convolutional Encoder and Viterbi Decoder in Python/C++.
 Author-email: Yachen Mao <maoyachen55@gmail.com>, Min Xu <xukmin@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -206,154 +206,46 @@
            limitations under the License.
         
 Keywords: viterbi
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Convolutional Encoder and Viterbi Decoder
-=========================================
+# Convolutional Encoder and Viterbi Decoder
 
-Author: Min Xu &lt;xukmin@gmail.com&gt;
+> This project is a fork of <https://github.com/xukmin/viterbi> that introduces Python support, enabling effortless utilization of the Viterbi module within the Python environment.
 
-This program implements both a Convolutional Encoder and a Viterbi Decoder in C++.
+## Install
 
-Running ViterbiCodec
---------------------
-
-Compile:
-
-```bash
-make
-```
-
-Run:
-
-```bash
-./viterbi_main <constraint> <polynomial>... <bits>
-```
-
-Example use:
-
-Decoding:
-
-```bash
-./viterbi_main 3 7 5 0011100001100111111000101100111011
-010111001010001
-```
-
-Encoding:
-
-```bash
-$ ./viterbi_main 3 7 5 --encode 010111001010001
-0011100001100111111000101100111011
+```sh
+pip install viterbi
 ```
 
-Please note there are `(constraint - 1)` "0" bits padded in front of the original message.
-
-More Features
--------------
-
-- It supports reading input from stdin or from commandline arguments. When
-  reading from stdin, it ignores blank lines or comment lines (which start with
-  `#`).
+## Usage
 
-- It supports any number of generator polynomials.
+The following is a convolutional encoder with a constraint length of 7. The diagram indicates the binary values and polynomial form, indicating the left-most bit is the most-significant-bit (MSB). The generating polynomials are 1011011 and 1111001 can be alternatively expressed in octal as 133 and 171, respectively.
 
-- It can perform convolutional encoding by providing `--encode` commandline
-  flag.
+![convolutional encoder](docs/convolutional%20encoder.svg)
 
-- It supports a different notation of generator polynomials by providing
-  `--reverse_polynomials` commandline flag.
+Expressed in code as:
 
-Here are more options to run the program.
-
-Show help message:
-
-```bash
-./viterbi_main --help
+```python
+from viterbi import Viterbi
+dot11a_codec = Viterbi(7, [0o133, 0o171])
 ```
 
-Read input from stdin:
-
-```bash
-./viterbi_main [--reverse_polynomials] [--encode]
-```
-
-Input format is:
-
-```
-<constraint> <polynomial>... <bits>
-```
+You can use the viterbi decoder like this:
 
-Read input from commandline arguments:
+```python
+from viterbi import Viterbi
 
-```bash
-./viterbi_main [--reverse_polynomials] [--encode] <constraint> <polynomial>... <bits>
+dot11a_codec = Viterbi(7, [0o133, 0o171])
+bits = [0, 1, 0, 1, 0, 0, 0, 0, 1, 1, 1, 0]
+output = dot11a_codec.encode(bits)
+# [0, 0, 1, 1, 0, 1, 0, 0, 1, 0, 1, 1, 0, 1, 1, 1, 0, 1, 0, 1, 0, 1, 0, 1]
+dot11a_codec.decode(output)
+# [0, 1, 0, 1, 0, 0, 0, 0, 1, 1, 1, 0]
 ```
 
-Flags:
-
-```bash
---reverse_polynomials
-    Reverse polynomials. E.g. 6 (=0b110) becomes 3 (=0b011).
-
---encode
-    Do encoding instead of decoding.
-```
-
-Example usage:
-
-```bash
-./viterbi_main 3 7 5 0011100001100111111000101100111011
-./viterbi_main 3 6 5 111011011100101011
-./viterbi_main 7 91 121 1010110100001101001000011101
-./viterbi_main 7 91 117 121 111100101110001011110101111111001011100111
-./viterbi_main --reverse_polynomials 3 3 5 111011011100101011
-./viterbi_main --encode 3 7 5 010111001010001
-./viterbi_main --encode 3 6 5 1001101
-./viterbi_main --encode --reverse_polynomials 3 3 5 1001101
-```
-
-Error Handling
---------------
-
-All inputs are validated, and proper error messages will be output.
-
-- The `constraint` should be greater than `0`.
-- A generator polynomial should be greater than `0` and less than
-  `1 << constraint`.
-- The received bit sequence should be consisted with only `0` and `1`.
-- The received bit sequence should be of length `N * <num-of-polynomials>` where
-  `N` is an integer. Otherwise some bits must be missing during transmission.
-  We will fill in appropriate number of trailing zeros.
-
-Running Unit Test
------------------
-
-Run unit test:
-
-```bash
-make test
-```
-
-Or
-
-```bash
-make viterbi_test && ./viterbi_test
-```
-
-If the test passes, it will output `PASSED` and the end of the output;
-otherwise, the test program aborts with assertion error.
-
-There are a few sample cases in the unit test, some are with manually injected
-bit errors.
-
-It also generates random messages of length `8`, `16` and `32` for several different
-convolutional codes and test if they can be properly encoded and decoded.
-
-Dependencies
-------------
-
-The code is self-contained, meaning it depends on nothing but the C++ standard
-library. The purpose is to make it easy to be integrated in any project.
+## Using in C++
 
+You can find the way to use the Viterbi decoder in C++ in the [README](https://github.com/xukmin/viterbi) of the original project.
```

### Comparing `viterbi-0.0.2/viterbi.h` & `viterbi-0.0.3/viterbi.h`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,16 @@
   //    MSB corresponds to the oldest input that still remains in the shift
   //    register.
   //    This representation is used by the Spiral Viterbi Decoder Software
   //    Generator. See http://www.spiral.net/software/viterbi.html
   // We use 2.
   ViterbiCodec(int constraint, const std::vector<int>& polynomials);
 
+  ViterbiCodec(int constraint, const std::vector<int>& polynomials, const std::string& puncpat);
+
   std::string Encode(const std::string& bits) const;
 
   std::string Decode(const std::string& bits) const;
 
   int constraint() const { return constraint_; }
 
   const std::vector<int>& polynomials() const { return polynomials_; }
@@ -56,40 +58,39 @@
 
   void InitializeOutputs();
 
   int NextState(int current_state, int input) const;
 
   std::string Output(int current_state, int input) const;
 
-  int BranchMetric(const std::string& bits,
-                   int source_state,
-                   int target_state) const;
+  int BranchMetric(const std::string& bits, int source_state, int target_state) const;
 
   // Given num_parity_bits() received bits, compute and returns path
   // metric and its corresponding previous state.
-  std::pair<int, int> PathMetric(const std::string& bits,
-                                 const std::vector<int>& prev_path_metrics,
-                                 int state) const;
+  std::pair<int, int> PathMetric(const std::string& bits, const std::vector<int>& prev_path_metrics, int state) const;
 
   // Given num_parity_bits() received bits, update path metrics of all states
   // in the current iteration, and append new traceback vector to trellis.
-  void UpdatePathMetrics(const std::string& bits,
-                         std::vector<int>* path_metrics,
-                         Trellis* trellis) const;
+  void UpdatePathMetrics(const std::string& bits, std::vector<int>* path_metrics, Trellis* trellis) const;
+
+  std::string Puncturing(const std::string bits) const;
+
+  std::string Depuncturing(const std::string bits) const;
 
   const int constraint_;
   const std::vector<int> polynomials_;
+  const std::string puncpat_;
 
   // The output table.
   // The index is current input bit combined with previous inputs in the shift
   // register. The value is the output parity bits in string format for
   // convenience, e.g. "10". For example, suppose the shift register contains
   // 0b10 (= 2), and the current input is 0b1 (= 1), then the index is 0b110 (=
   // 6).
   std::vector<std::string> outputs_;
 };
 
-std::ostream& operator <<(std::ostream& os, const ViterbiCodec& codec);
+std::ostream& operator<<(std::ostream& os, const ViterbiCodec& codec);
 
 int ReverseBits(int num_bits, int input);
 
 #endif  // VITERBI_H_
```

