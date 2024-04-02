# Comparing `tmp/PyQvd-1.0.1.tar.gz` & `tmp/PyQvd-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQvd-1.0.1.tar", last modified: Thu Mar 14 11:01:57 2024, max compression
+gzip compressed data, was "PyQvd-1.0.2.tar", last modified: Tue Apr  2 11:18:02 2024, max compression
```

## Comparing `PyQvd-1.0.1.tar` & `PyQvd-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 11:01:57.338444 PyQvd-1.0.1/
--rw-rw-rw-   0        0        0     1075 2024-02-15 12:35:45.000000 PyQvd-1.0.1/LICENSE.md
--rw-rw-rw-   0        0        0    11944 2024-03-14 11:01:57.334396 PyQvd-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-14 11:01:57.330400 PyQvd-1.0.1/PyQvd.egg-info/
--rw-rw-rw-   0        0        0    11944 2024-03-14 11:01:57.000000 PyQvd-1.0.1/PyQvd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-03-14 11:01:57.000000 PyQvd-1.0.1/PyQvd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 11:01:57.000000 PyQvd-1.0.1/PyQvd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-03-14 11:01:57.000000 PyQvd-1.0.1/PyQvd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-14 11:01:57.000000 PyQvd-1.0.1/PyQvd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9734 2024-03-14 10:01:11.000000 PyQvd-1.0.1/README.md
--rw-rw-rw-   0        0        0     1288 2024-03-14 10:57:16.000000 PyQvd-1.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-03-14 11:01:57.325490 PyQvd-1.0.1/pyqvd/
--rw-rw-rw-   0        0        0       83 2024-02-19 16:50:50.000000 PyQvd-1.0.1/pyqvd/__init__.py
--rw-rw-rw-   0        0        0    35483 2024-03-14 10:53:03.000000 PyQvd-1.0.1/pyqvd/qvd.py
--rw-rw-rw-   0        0        0       42 2024-03-14 11:01:57.339457 PyQvd-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 11:18:02.803867 PyQvd-1.0.2/
+-rw-rw-rw-   0        0        0     1096 2024-03-27 12:50:40.000000 PyQvd-1.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0    11944 2024-04-02 11:18:02.803867 PyQvd-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 11:18:02.803867 PyQvd-1.0.2/PyQvd.egg-info/
+-rw-rw-rw-   0        0        0    11944 2024-04-02 11:18:02.000000 PyQvd-1.0.2/PyQvd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-04-02 11:18:02.000000 PyQvd-1.0.2/PyQvd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 11:18:02.000000 PyQvd-1.0.2/PyQvd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-02 11:18:02.000000 PyQvd-1.0.2/PyQvd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-02 11:18:02.000000 PyQvd-1.0.2/PyQvd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9734 2024-03-27 12:50:40.000000 PyQvd-1.0.2/README.md
+-rw-rw-rw-   0        0        0     1288 2024-04-02 11:12:07.000000 PyQvd-1.0.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-02 11:18:02.801249 PyQvd-1.0.2/pyqvd/
+-rw-rw-rw-   0        0        0       88 2024-04-02 10:45:55.000000 PyQvd-1.0.2/pyqvd/__init__.py
+-rw-rw-rw-   0        0        0    36067 2024-04-02 11:00:04.000000 PyQvd-1.0.2/pyqvd/qvd.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 11:18:02.803867 PyQvd-1.0.2/setup.cfg
```

### Comparing `PyQvd-1.0.1/LICENSE.md` & `PyQvd-1.0.2/LICENSE.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Constantin Müller
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Constantin Müller
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `PyQvd-1.0.1/PKG-INFO` & `PyQvd-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQvd
-Version: 1.0.1
+Version: 1.0.2
 Summary: Utility library for reading/writing Qlik View Data (QVD) files in Python.
 Author-email: Constantin Müller <info@mueller-constantin.de>
 License: MIT License
         
         Copyright (c) 2024 Constantin Müller
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `PyQvd-1.0.1/PyQvd.egg-info/PKG-INFO` & `PyQvd-1.0.2/PyQvd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQvd
-Version: 1.0.1
+Version: 1.0.2
 Summary: Utility library for reading/writing Qlik View Data (QVD) files in Python.
 Author-email: Constantin Müller <info@mueller-constantin.de>
 License: MIT License
         
         Copyright (c) 2024 Constantin Müller
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `PyQvd-1.0.1/README.md` & `PyQvd-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `PyQvd-1.0.1/pyproject.toml` & `PyQvd-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyQvd"
-version = "1.0.1"
+version = "1.0.2"
 description = "Utility library for reading/writing Qlik View Data (QVD) files in Python."
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE.md"}
 authors = [
     {name = "Constantin Müller", email = "info@mueller-constantin.de"},
 ]
 keywords = ["qlik", "qvd", "qlik sense", "qlik view", "pandas"]
```

### Comparing `PyQvd-1.0.1/pyqvd/qvd.py` & `PyQvd-1.0.2/pyqvd/qvd.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,26 +361,29 @@
             raise ValueError('The XML header section does not exist or is not properly delimited from the binary data.')
 
         header_end_index = header_delimiter_index + len(HEADER_DELIMITER)
         header_buffer = self._buffer[header_begin_index:header_end_index].decode()
 
         self._header = ET.fromstring(header_buffer[:-1])
 
-        if not self._header:
+        if self._header is None:
             raise ValueError('The XML header could not be parsed.')
 
         self._header_offset = header_begin_index
         self._symbol_table_offset = header_end_index
         self._index_table_offset = self._symbol_table_offset + int(self._header.find('./Offset').text, 10)
 
     def _parse_symbol_table(self):
         """
         Parses the symbol table of the QVD file.
         """
-        if not all([self._buffer, self._header, self._symbol_table_offset, self._index_table_offset]):
+        if (self._buffer is None or
+            self._header is None or
+            self._symbol_table_offset is None or
+            self._index_table_offset is None):
             raise ValueError('The QVD file has not been loaded in the proper order or has not been loaded at all.')
 
         fields = self._header.find('./Fields').findall('./QvdFieldHeader')
         symbol_buffer = self._buffer[self._symbol_table_offset:self._index_table_offset]
 
         self._symbol_table = [None] * len(fields)
 
@@ -443,15 +446,15 @@
 
             self._symbol_table[index] = symbols
 
     def _parse_index_table(self):
         """
         Parses the index table of the QVD file.
         """
-        if not (self._buffer and self._header and self._index_table_offset):
+        if self._buffer is None or self._header is None or self._index_table_offset is None:
             raise ValueError('The QVD file has not been loaded in the proper order or has not been loaded at all.')
 
         fields = self._header.find('./Fields').findall('./QvdFieldHeader')
         record_size = int(self._header.find('RecordByteSize').text, 10)
         length = int(self._header.find('Length').text, 10)
 
         index_buffer = self._buffer[self._index_table_offset:self._index_table_offset + length + 1]
@@ -749,15 +752,15 @@
         """
 
         self._symbol_table = [None] * len(self._df.columns)
         self._symbol_table_metadata = [None] * len(self._df.columns)
         self._symbol_buffer = b''
 
         for column_index, _ in enumerate(self._df.columns):
-            unique_values = set([row[column_index] for row in self._df.data])
+            unique_values = QvdFileWriter._get_unique_values([row[column_index] for row in self._df.data])
 
             symbols = []
 
             for value in unique_values:
                 symbols.append(self._convert_raw_to_symbol(value))
 
             current_symbol_buffer = b''.join([symbol.to_byte_representation() for symbol in symbols])
@@ -851,35 +854,38 @@
 
             # Pad the bit representation of the indices with zeros to match the bit width
             for bit_indices in self._index_table:
                 bit_indices[column_index] = bit_indices[column_index].rjust(bit_width, '0')
 
         # Concatenate the bit representation of the indices of each row to a single binary string per row
         for bit_indices in self._index_table:
+            bit_indices = bit_indices[::-1]
             bits = ''.join(bit_indices)
-            padded_bits = '0' * (8 - len(bits) % 8) + bits
+            padding_width = (8 - len(bits) % 8) % 8
+            padded_bits = '0' * padding_width + bits
             byte_values = [int(padded_bits[index:index + 8], 2) for index in range(0, len(padded_bits), 8)]
             byte_representation = struct.pack('<' + 'B' * len(byte_values), *byte_values)
+            byte_representation = byte_representation[::-1]
 
             self._index_buffer += byte_representation
 
         self._record_byte_size = len(self._index_buffer) // len(self._df.data)
 
     def _convert_raw_to_symbol(self, raw: any) -> QvdSymbol:
         """
         Converts a raw value to a QVD symbol.
 
         :param raw: The raw value.
         :return: The QVD symbol.
         """
         if isinstance(raw, int):
-            return QvdSymbol.from_dual_int_value(raw, str(raw))
+            return QvdSymbol.from_int_value(raw)
 
         if isinstance(raw, float):
-            return QvdSymbol.from_dual_double_value(raw, str(raw))
+            return QvdSymbol.from_double_value(raw)
 
         if isinstance(raw, str):
             return QvdSymbol.from_string_value(raw)
 
         return QvdSymbol.from_string_value(str(raw))
 
     @staticmethod
@@ -889,14 +895,27 @@
 
         :param value: The integer value.
         :param width: The width of the bits.
         :return: The list of bits.
         """
         return [int(bit) for bit in format(value, '0' + str(width) + 'b')]
 
+    @staticmethod
+    def _get_unique_values(values: List[any]) -> List[any]:
+        """
+        Determines the unique values of a given list.
+        """
+        unique_values = []
+
+        for value in values:
+            if value not in unique_values:
+                unique_values.append(value)
+
+        return unique_values
+
     def save(self):
         """
         Persists the data frame to a QVD file.
         """
 
         self._build_symbol_table()
         self._build_index_table()
```

