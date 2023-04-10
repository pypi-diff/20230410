# Comparing `tmp/convtools-1.1.2.tar.gz` & `tmp/convtools-1.2.0.tar.gz`

## Comparing `convtools-1.1.2.tar` & `convtools-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 convtools-1.1.2/convtools/__init__.py
--rw-r--r--   0        0        0    47910 2020-02-02 00:00:00.000000 convtools-1.1.2/convtools/_aggregations.py
--rw-r--r--   0        0        0   105674 2020-02-02 00:00:00.000000 convtools-1.1.2/convtools/_base.py
--rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 convtools-1.1.2/convtools/_chunks.py
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 convtools-1.1.2/convtools/_columns.py
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 convtools-1.1.2/convtools/_conversion.py
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 convtools-1.1.2/convtools/_cumulative.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 convtools-1.1.2/convtools/_debug.py
--rw-r--r--   0        0        0    20223 2020-02-02 00:00:00.000000 convtools-1.1.2/convtools/_dt.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 convtools-1.1.2/convtools/_heuristics.py
--rw-r--r--   0        0        0    17783 2020-02-02 00:00:00.000000 convtools-1.1.2/convtools/_joins.py
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 convtools-1.1.2/convtools/_mutations.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 convtools-1.1.2/convtools/_unique.py
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 convtools-1.1.2/convtools/_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 convtools-1.1.2/convtools/contrib/__init__.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 convtools-1.1.2/convtools/contrib/fs.py
--rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 convtools-1.1.2/convtools/contrib/tables.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 convtools-1.1.2/.gitignore
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 convtools-1.1.2/LICENSE.txt
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 convtools-1.1.2/README.md
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 convtools-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 convtools-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/__init__.py
+-rw-r--r--   0        0        0    51224 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_aggregations.py
+-rw-r--r--   0        0        0   107382 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_base.py
+-rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_chunks.py
+-rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_columns.py
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_conversion.py
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_cumulative.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_debug.py
+-rw-r--r--   0        0        0    20223 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_dt.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_heuristics.py
+-rw-r--r--   0        0        0    17783 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_joins.py
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_mutations.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_unique.py
+-rw-r--r--   0        0        0     8584 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/contrib/__init__.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/contrib/fs.py
+-rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 convtools-1.2.0/convtools/contrib/tables.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 convtools-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 convtools-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 convtools-1.2.0/README.md
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 convtools-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 convtools-1.2.0/PKG-INFO
```

### Comparing `convtools-1.1.2/convtools/_aggregations.py` & `convtools-1.2.0/convtools/_aggregations.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """This module brings aggregations with various reduce functions"""
 import typing as t
+import warnings
 from collections import defaultdict
 from decimal import Decimal
+from itertools import chain
 from math import ceil
 
 from ._base import (
     BaseConversion,
     CallFunc,
     ConversionException,
     ConverterOptionsCtx,
@@ -19,407 +21,314 @@
     ListComp,
     NaiveConversion,
     Namespace,
     NamespaceCtx,
     This,
     Tuple,
     _None,
-    ensure_conversion,
+    _none,
 )
 from ._heuristics import Weights
 from ._utils import Code
 
 
-_none = BaseConversion._none
-RBT = t.TypeVar("RBT", bound="ReduceBlock")
+class ReduceCode:
+    """Merges and stores code of reducers"""
 
+    def __init__(self):
+        self.value_to_name: "t.Dict[str, str]" = {}
+        self.condition_to_child: "t.Dict[str, ReduceCode]" = {}
+        self.key_to_reduce_lines = {}
+
+    def add_assignment(self, value):
+        if value in self.value_to_name:
+            return self.value_to_name[value]
+
+        new_name = self.value_to_name[value] = f"_r{len(self.value_to_name)}_"
+        return new_name
+
+    def use_expression(self, value):
+        if value in self.value_to_name:
+            return self.value_to_name[value]
+        return value
+
+    def add_condition(self, condition):
+        if condition in self.condition_to_child:
+            return self.condition_to_child[condition]
+        reduce_code = self.condition_to_child[condition] = ReduceCode()
+        return reduce_code
+
+    def add_reduce_lines(
+        self, var_agg_data_value, prepare_first_lines, reduce_lines
+    ) -> str:
+        key = "".join(
+            line.replace(var_agg_data_value, "")
+            for line in chain(prepare_first_lines, reduce_lines)
+        )
+        if key in self.key_to_reduce_lines:
+            return self.key_to_reduce_lines[key][0]
+
+        self.key_to_reduce_lines[key] = (
+            var_agg_data_value,
+            prepare_first_lines,
+            reduce_lines,
+        )
+        return var_agg_data_value
+
+
+class ReduceManager:
+    """Builds group by / aggregate code"""
+
+    __slots__ = [
+        "var_row",
+        "var_agg_data",
+        "aggregate_mode",
+        "number",
+        "reduce_code",
+        "used_indexes",
+    ]
 
-class ReduceBlock:
-    """Represents a section of code of a single reducer"""
-
-    var_checksum = "checksum_"
-
-    def __init__(
-        self,
-        reduce_initial: t.Iterable[str],
-        reduce_two: t.Iterable[str],
-        reducer_code_input: str,
-        var_agg_data_value: str,
-        checksum_flag: int,
-        unconditional_init: bool,
-    ):
-        self.reduce_initial = {var_agg_data_value: reduce_initial}
-        self.reduce_two = {var_agg_data_value: reduce_two}
-        self.reducer_code_input = reducer_code_input
-        self.condition_code = None
-        self.unconditional_init = unconditional_init
-        self.checksum_flag = checksum_flag
-
-    def consume(self: RBT, reduce_block: RBT) -> RBT:
-        if (
-            self.condition_code != reduce_block.condition_code
-            or not self.unconditional_init
-            or not reduce_block.unconditional_init
-        ):
-            raise AssertionError
-
-        for k, v in reduce_block.reduce_initial.items():
-            if k in self.reduce_initial:
-                raise AssertionError
-            self.reduce_initial[k] = v
-
-        for k, v in reduce_block.reduce_two.items():
-            if k in self.reduce_two:
-                raise AssertionError
-            self.reduce_two[k] = v
-
-        self.checksum_flag += reduce_block.checksum_flag
-        return self
-
-    def iter_reduce_lines(self, lines_info_dict) -> t.Iterable[str]:
-        for var_agg_data_value, lines in lines_info_dict.items():
-            template_kwargs = {
-                "result": var_agg_data_value,
-                "input": self.reducer_code_input,
-            }
-            yield from (line % template_kwargs for line in lines)
-
-    def iter_reduce_initial_lines(self) -> t.Iterable[str]:
-        yield from self.iter_reduce_lines(self.reduce_initial)
-
-    def iter_reduce_two_lines(self) -> t.Iterable[str]:
-        yield from self.iter_reduce_lines(self.reduce_two)
-
-    def as_key(self):
-        return (
-            self.condition_code,
-            self.unconditional_init,
-            self.reducer_code_input,
-            tuple(
-                line
-                for lines in self.reduce_initial.values()
-                for line in lines
-            ),
-            tuple(
-                line for lines in self.reduce_two.values() for line in lines
-            ),
-        )
-
-
-class ReduceConditionalBlock(ReduceBlock):
-    """Represents a section of code of a single reducer with an incoming
-    condition"""
-
-    def __init__(self, *args, **kwargs):
-        condition_code = kwargs.pop("condition_code")
-        super().__init__(*args, **kwargs)
-        self.condition_code = condition_code
-
-
-ReduceBlockType = t.Union[ReduceBlock, ReduceConditionalBlock]
-
-
-class ReduceBlocks:
-    """Represents a set of reduce blocks"""
-
-    def __init__(self, var_agg_data, aggregate_mode):
+    def __init__(self, var_row, var_agg_data, aggregate_mode):
+        self.var_row = var_row
         self.var_agg_data = var_agg_data
         self.aggregate_mode = aggregate_mode
-
-        self.block_key_to_index = {}
-        self.agg_data_values = []
-
-        self.condition_to_blocks = {}
-        self.other_blocks = []
         self.number = 0
+        self.reduce_code = ReduceCode()
+        self.used_indexes = []
 
-    def exchange_reducer_code_input(self, reducer, reducer_code_input, ctx):
-        checksum_flag = 1 if self.aggregate_mode else 0
-        agg_data_value = self._gen_agg_data_value(self.number)
-        reduce_block = reducer.gen_reduce_code_block(
-            agg_data_value,
-            reducer_code_input,
-            checksum_flag,
-            ctx,
+    def gen_group_by_code(self, var_signature_to_agg_data, code_signature):
+        code = Code()
+        code.add_line(f"for {self.var_row} in data_:", 1)
+        code.add_line(
+            f"{self.var_agg_data} = {var_signature_to_agg_data}[{code_signature}]",
+            0,
         )
-        key = reduce_block.as_key()
-        index = self.block_key_to_index.get(key)
+        self.add_group_by_code(code, self.reduce_code)
+        return code
 
-        if index is not None:
-            return self._gen_agg_data_value(index)
+    def gen_aggregate_code(self):
+        var_init_checksum = "checksum_"
+        code = Code()
+        code.add_line(f"{var_init_checksum} = 0", 0)
+        code.add_line("it_ = iter(data_)", 0)
+        code.add_line(f"for {self.var_row} in it_:", 1)
+        checksum = self.add_group_by_code(
+            code, self.reduce_code, var_init_checksum=var_init_checksum
+        )
+        code.add_line(f"if {var_init_checksum} == {checksum}:", 1)
+        if ConverterOptionsCtx.get_option_value("debug"):
+            code.add_line(
+                "globals()['__BROKEN_EARLY__'] = True  # DEBUG ONLY",
+                0,
+            )
+        code.add_line("break", -2)
 
-        self.block_key_to_index[key] = self.number
-        self._add_block(reduce_block)
-        self.agg_data_values.append(agg_data_value)
-        return agg_data_value
+        ref = code.get_ref()
+        code.add_line(f"for {self.var_row} in it_:", 1)
+        if self.add_aggregate_stage2_code(code, self.reduce_code) == 0:
+            code.cut_to_ref(ref)
+        return code
 
-    def _gen_agg_data_value(self, index):
+    def fmt_agg_data_value(self, index):
         return (
             f"{self.var_agg_data}_v{index}"
             if self.aggregate_mode
             else f"{self.var_agg_data}.v{index}"
         )
 
-    def _add_block(self, reduce_block: ReduceBlockType):
+    def gen_agg_data_value(self):
+        index = self.number
         self.number += 1
+        return index, self.fmt_agg_data_value(index)
 
-        if reduce_block.unconditional_init:
-            condition = (
-                reduce_block.condition_code
-                if isinstance(reduce_block, ReduceConditionalBlock)
-                else None
-            )
-
-            if condition in self.condition_to_blocks:
-                self.condition_to_blocks[condition].consume(reduce_block)
-            else:
-                self.condition_to_blocks[condition] = reduce_block
+    def gen_group_by_data_container(self, grouper, container_name, ctx):
+        attrs = [f"v{i}" for i in self.used_indexes]
 
+        code = Code()
+        code.add_line(f"class {container_name}:", 1)
+        _ = ",".join(f"'{attr}'" for attr in attrs)
+        code.add_line(f"__slots__ = [{_}]", 0)
+        code.add_line("def __init__(self, _none=__none__):", 1)
+        if attrs:
+            for attr in attrs:
+                code.add_line(f"self.{attr} = _none", 0)
         else:
-            return self.other_blocks.append(reduce_block)
-
-    def iter_blocks(self) -> t.Generator[ReduceBlockType, None, None]:
-        yield from self.condition_to_blocks.values()
-        yield from self.other_blocks
+            code.add_line("pass", 0)
+        return ctx[
+            grouper.compile_converter(container_name, code.to_string(0), ctx)
+        ]
 
-    def gen_group_by_code(
-        self,
-        var_row,
-        var_agg_data,
-        var_signature_to_agg_data,
-        code_signature,
-    ) -> Code:
-        code = Code()
-        code.add_line(f"for {var_row} in data_:", 1)
-        code.add_line(
-            f"{var_agg_data} = {var_signature_to_agg_data}[{code_signature}]",
-            0,
+    def gen_init_aggregate_vars(self):
+        vars_code = " = ".join(
+            [self.fmt_agg_data_value(index) for index in self.used_indexes]
         )
+        return f"{vars_code} = _none"
 
-        for block in self.iter_blocks():
-            reduce_initial_lines = list(block.iter_reduce_initial_lines())
-            reduce_two_lines = list(block.iter_reduce_two_lines())
-            any_var_agg_data_value = next(iter(block.reduce_initial))
-
-            if block.condition_code:
-                code.add_line(f"if {block.condition_code}:", 1)
-
-            code.add_line(f"if {any_var_agg_data_value} is _none:", 1)
-            for line in reduce_initial_lines:
-                code.add_line(line, 0)
-            code.incr_indent_level(-1)
-
-            if reduce_two_lines:
-                code.add_line("else:", 1)
-                for line in reduce_two_lines:
-                    code.add_line(line, 0)
-                code.incr_indent_level(-1)
-
-            if block.condition_code:
-                code.incr_indent_level(-1)
-        return code
-
-    def gen_aggregate_code(
+    def add_group_by_code(
         self,
-        var_row,
-        expected_checksum,
-    ) -> Code:
-        is_debug = ConverterOptionsCtx.get_option_value("debug")
-        var_checksum = ReduceBlock.var_checksum
-        first_phase_code = Code()
-        second_phase_code = Code()
-
-        needs_sum_checking = False
-
-        reduce_blocks = list(self.iter_blocks())
-        is_single_block = len(reduce_blocks) == 1
-        for block in reduce_blocks:
-            reduce_initial_lines = list(block.iter_reduce_initial_lines())
-            reduce_two_lines = list(block.iter_reduce_two_lines())
-            any_var_agg_data_value = next(iter(block.reduce_initial))
-
-            init_phase_needs_else = not (
-                is_single_block and block.unconditional_init
-            )
-
-            if block.condition_code:
-                first_phase_code.add_line(f"if {block.condition_code}:", 1)
+        code: Code,
+        reduce_code: ReduceCode,
+        delegated_conditions=(),
+        var_init_checksum=None,
+    ):
+        checksum = 0
+        initial_indent_level = code.indent_level
 
-            first_phase_code.add_line(
-                f"if {any_var_agg_data_value} is _none:", 1
-            )
-            for line in reduce_initial_lines:
-                first_phase_code.add_line(line, 0)
+        if delegated_conditions and (
+            reduce_code.value_to_name
+            or reduce_code.key_to_reduce_lines
+            or len(reduce_code.condition_to_child) > 1
+        ):
+            code.add_line(f"if {' and '.join(delegated_conditions)}:", 1)
+            delegated_conditions = ()
 
-            if is_single_block:
-                if block.unconditional_init:
-                    if is_debug:
-                        first_phase_code.add_line(
-                            "globals()['__BROKEN_EARLY__'] = True  # DEBUG ONLY",
-                            0,
-                        )
-                    first_phase_code.add_line("break", 0)
-                else:
-                    first_phase_code.add_line(
-                        f"if {any_var_agg_data_value} is not _none:", 1
-                    )
-                    if is_debug:
-                        first_phase_code.add_line(
-                            "globals()['__BROKEN_EARLY__'] = True  # DEBUG ONLY",
-                            0,
-                        )
-                    first_phase_code.add_line("break", -1)
+        for value, name in reduce_code.value_to_name.items():
+            code.add_line(f"{name} = {value}", 0)
 
-            else:
-                if block.unconditional_init:
-                    first_phase_code.add_line(
-                        f"{var_checksum} += {block.checksum_flag}", 0
-                    )
-                else:
-                    first_phase_code.add_line(
-                        f"if {any_var_agg_data_value} is not _none:", 1
-                    )
-                    first_phase_code.add_line(
-                        f"{var_checksum} += {block.checksum_flag}", -1
-                    )
-                needs_sum_checking = True
+        if reduce_code.key_to_reduce_lines:
+            var_agg_data_value = next(
+                iter(reduce_code.key_to_reduce_lines.values())
+            )[0]
+            code.add_line(f"if {var_agg_data_value} is _none:", 1)
 
-            first_phase_code.incr_indent_level(-1)
+            if var_init_checksum:
+                code.add_line(f"{var_init_checksum} += 1", 0)
+            checksum += 1
 
-            if init_phase_needs_else and reduce_two_lines:
-                first_phase_code.add_line("else:", 1)
-                for line in reduce_two_lines:
-                    first_phase_code.add_line(line, 0)
-                first_phase_code.incr_indent_level(-1)
-
-            if block.condition_code:
-                first_phase_code.incr_indent_level(-1)
-
-            if reduce_two_lines:
-                if block.condition_code:
-                    second_phase_code.add_line(
-                        f"if {block.condition_code}:", 1
-                    )
-
-                for line in reduce_two_lines:
-                    second_phase_code.add_line(line, 0)
+            for item in reduce_code.key_to_reduce_lines.values():
+                for line in item[1]:  # prepare_first_lines
+                    code.add_line(line, 0)
 
-                if block.condition_code:
-                    second_phase_code.incr_indent_level(-1)
+            code.incr_indent_level(-1)
+            code.add_line("else:", 1)
 
-        resulting_code = Code()
+            lines_before = len(code.lines_info)
+            for item in reduce_code.key_to_reduce_lines.values():
+                for line in item[2]:  # reduce_lines
+                    code.add_line(line, 0)
+            if lines_before == len(code.lines_info):
+                code.add_line("pass", 0)
 
-        resulting_code.add_line("it_ = iter(data_)", 0)
-        resulting_code.add_line(f"for {var_row} in it_:", 1)
+            code.incr_indent_level(-1)
 
-        resulting_code.add_code(first_phase_code)
-        if needs_sum_checking:
-            resulting_code.add_line(
-                f"if {var_checksum} == {expected_checksum}:", 1
+        for condition, child in reduce_code.condition_to_child.items():
+            checksum += self.add_group_by_code(
+                code,
+                child,
+                delegated_conditions=delegated_conditions + (condition,),
+                var_init_checksum=var_init_checksum,
             )
-            if is_debug:
-                resulting_code.add_line(
-                    "globals()['__BROKEN_EARLY__'] = True  # DEBUG ONLY", 0
-                )
-            resulting_code.add_line("break", -1)
-        resulting_code.incr_indent_level(-1)
-
-        if second_phase_code.has_lines():
-            resulting_code.add_line("", 0)
-            resulting_code.add_line(f"for {var_row} in it_:", 1)
-
-            resulting_code.add_code(second_phase_code)
-            resulting_code.incr_indent_level(-1)
-        return resulting_code
-
-
-GROUPER_TEMPLATE = """
-def {converter_name}({code_args}):
-    {var_signature_to_agg_data} = defaultdict({var_agg_data_cls})
 
-{code_group_by}
-
-{code_result}
-"""
-AGGREGATE_TEMPLATE = """
-def {converter_name}({code_args}):
-    {code_init_agg_vars}
-    {var_checksum} = 0
+        code.indent_level = initial_indent_level
+        return checksum
 
-{code_aggregate}
+    def add_aggregate_stage2_code(
+        self, code: Code, reduce_code: ReduceCode, delegated_conditions=()
+    ):
+        initial_indent_level = code.indent_level
+        checksum = 0
+        add_pass_if_line_number = -1
+
+        if delegated_conditions and (
+            reduce_code.value_to_name
+            or reduce_code.key_to_reduce_lines
+            or len(reduce_code.condition_to_child) > 1
+        ):
+            code.add_line(f"if {' and '.join(delegated_conditions)}:", 1)
+            add_pass_if_line_number = len(code.lines_info)
+            delegated_conditions = ()
+
+        for value, name in reduce_code.value_to_name.items():
+            code.add_line(f"{name} = {value}", 0)
+
+        if reduce_code.key_to_reduce_lines:
+            for item in reduce_code.key_to_reduce_lines.values():
+                if item[2]:
+                    checksum += 1
+                for line in item[2]:  # reduce_lines
+                    code.add_line(line, 0)
 
-{code_result}
-"""
+        for condition, child in reduce_code.condition_to_child.items():
+            checksum += self.add_aggregate_stage2_code(
+                code,
+                child,
+                delegated_conditions=delegated_conditions + (condition,),
+            )
 
+        if add_pass_if_line_number == len(code.lines_info):
+            code.add_line("pass", -1)
 
-RT = t.TypeVar("RT", bound="BaseReducer")
+        code.indent_level = initial_indent_level
+        return checksum
 
 
 class BaseReducer(BaseConversion):
     """Base of a reduce operation to be used during the aggregation"""
 
-    expressions: t.Tuple[t.Any, ...]
-    post_conversion: t.Optional[BaseConversion] = None
-    default: t.Any
-    where: t.Any = _none
-    unconditional_init: bool = False
+    _expressions: t.Sequence[BaseConversion]
+
+    default: t.Union[_None, BaseConversion] = _none
+    initial: t.Union[_None, BaseConversion] = _none
+    internals_are_public: bool
+    values_use_times: t.Tuple[int, ...]
+    works_with_not_none_only: t.Tuple[int, ...]
+    prepare_first_lines: t.Union[
+        t.Tuple[str, ...], t.Callable[[], t.Tuple[str, ...]]
+    ]
+    reduce_lines: t.Union[t.Tuple[str, ...], t.Callable[[], t.Tuple[str, ...]]]
+    where: t.Union[_None, BaseConversion]
 
     self_content_type = (
         (
             BaseConversion.self_content_type
             & ~BaseConversion.ContentTypes.FUNCTION_OF_INPUT
         )
         | BaseConversion.ContentTypes.REDUCER
         | BaseConversion.ContentTypes.NONE_USAGE
     )
 
-    def __init__(self, default, initial):
+    def __init__(self, *expressions, initial=_none, default=_none, where=None):
         super().__init__()
-
+        self.expressions = tuple(
+            self.ensure_conversion(expression) for expression in expressions
+        )
         self.default, self.initial = self.prepare_default_n_initial(
             default, initial
         )
+        self.check_expressions()
+        self.where = (
+            _none
+            if (where is None or where is _none)
+            else self.ensure_conversion(where)
+        )
+        post_conversion = self.get_option("post_conversion", None, None)
         self.conversion = self.ensure_conversion(
             If(
-                This().is_(EscapedString("_none")),
+                This.is_(EscapedString("_none")),
                 self.default,
-                (
-                    self.post_conversion
-                    if self.post_conversion is not None
-                    else This()
-                ),
+                (post_conversion if post_conversion is not None else This),
             )
         )
 
-    def gen_reduce_code_block(
-        self,
-        var_agg_data_value: str,
-        reducer_code_input: str,
-        checksum_flag: int,
-        ctx: dict,
-    ) -> ReduceBlockType:
-        raise NotImplementedError
-
-    def _gen_code_and_update_ctx(self, code_input, ctx) -> str:
-        code_input = ctx["exchange_reducer_code_input_methods"][-1](
-            reducer=self,
-            reducer_code_input=code_input,
-            ctx=ctx,
-        )
-        return self.conversion.gen_code_and_update_ctx(code_input, ctx)
+    def check_expressions(self):
+        if not self.internals_are_public and not isinstance(
+            self.initial, _None
+        ):
+            warnings.warn(
+                "2.0 will raise ValueError if initial is "
+                f"passed to {self.__class__.__name__}",
+                DeprecationWarning,
+            )
 
     def prepare_default_n_initial(self, default, initial):
         if default is _none:
-            try:
-                default = self.default
-            except AttributeError:
-                pass
-
-        if initial is _none and hasattr(self, "initial"):
+            default = self.default
+        if initial is _none:
             initial = self.initial
+
         if initial is not _none:
             initial = self.ensure_conversion(initial)
             if initial.is_itself_callable_like():
                 initial = initial.call_like()
 
             if default is _none and initial.ignores_input():
                 default = initial
@@ -429,586 +338,317 @@
 
         default = self.ensure_conversion(default)
         if default.is_itself_callable_like():
             default = default.call_like()
 
         return default, initial
 
+    def get_option(self, name, ctx, default=_none):
+        if default is _none:
+            option_value = getattr(self, name)
+        else:
+            option_value = getattr(self, name, default)
+        if callable(option_value):
+            return option_value(ctx)
+        return option_value
 
-class MultiStatementReducer(BaseReducer):
-    """Defines the reduce operation, which is based on multiple python
-    statements, to be used during the aggregation"""
-
-    base_condition_code: "t.Optional[str]" = None
-    prepare_first: t.Tuple[str, ...]
-    reduce: t.Tuple[str, ...]
-
-    def __init__(self, *expressions, initial=_none, default=_none, where=None):
-        super().__init__(default, initial)
-        self.where = (
-            _none
-            if (where is None or where is _none)
-            else self.ensure_conversion(where)
+    def _gen_code_and_update_ctx(self, code_input, ctx) -> str:
+        reduce_manager: ReduceManager = ctx["current_reduce_manager"][-1]
+        index, proposed_code_input = reduce_manager.gen_agg_data_value()
+        new_code_input = self.update_reduce_code(
+            reduce_manager.reduce_code,
+            proposed_code_input,
+            reduce_manager.var_row,
+            code_input,
+            ctx,
         )
+        if proposed_code_input == new_code_input:
+            reduce_manager.used_indexes.append(index)
 
-        self.expressions = tuple(
-            self.ensure_conversion(expr)
-            for expr in (
-                self.expressions
-                if hasattr(self, "expressions") and not expressions
-                else expressions
-            )
-        )
+        return self.conversion.gen_code_and_update_ctx(new_code_input, ctx)
 
-    def _format_statements(
+    def update_reduce_code(
         self,
-        statements,
-        args,
+        reduce_code: ReduceCode,
+        var_agg_data_value,
+        var_row,
         reducer_code_input,
         ctx,
-        prev_result="%(result)s",
     ):
-        code_args = tuple(
-            arg.gen_code_and_update_ctx(reducer_code_input, ctx)
-            for arg in args
-        )
-        return [
-            statement.format(*code_args, prev_result=prev_result)
-            for statement in statements
-        ]
-
-    def gen_reduce_code_block(
-        self,
-        var_agg_data_value: str,
-        reducer_code_input: str,
-        checksum_flag: int,
-        ctx: dict,
-    ) -> ReduceBlockType:
-        if self.initial is _none:
-            reduce_initial = self._format_statements(
-                (
-                    self.prepare_first(ctx)
-                    if callable(self.prepare_first)
-                    else self.prepare_first
-                ),
-                self.expressions,
-                reducer_code_input,
-                ctx,
-            )
-        else:
-            reduce_initial = self._format_statements(
-                (self.reduce(ctx) if callable(self.reduce) else self.reduce),
-                self.expressions,
-                reducer_code_input,
-                ctx,
-                prev_result=self.initial.gen_code_and_update_ctx(
-                    reducer_code_input, ctx
-                ),
+        if not isinstance(self.where, _None):
+            reduce_code = reduce_code.add_condition(
+                self.where.gen_code_and_update_ctx(var_row, ctx)
             )
 
-        reduce_two = self._format_statements(
-            (self.reduce(ctx) if callable(self.reduce) else self.reduce),
-            self.expressions,
-            reducer_code_input,
-            ctx,
-        )
-
         kwargs = {
-            "reduce_initial": reduce_initial,
-            "reduce_two": reduce_two,
-            "reducer_code_input": reducer_code_input,
-            "var_agg_data_value": var_agg_data_value,
-            "checksum_flag": checksum_flag,
-            "unconditional_init": self.unconditional_init,
+            "result": var_agg_data_value,
+            "row": var_row,
+            # "value0", "value1", etc.
         }
-        if self.where is not _none:
-            condition_code = self.where.gen_code_and_update_ctx(
-                reducer_code_input, ctx
-            )
-            if condition_code != "True":
-                kwargs["condition_code"] = condition_code
-
-        if self.base_condition_code:
-            base_condition_code = self._format_statements(
-                [self.base_condition_code],
-                self.expressions,
-                reducer_code_input,
-                ctx,
-            )[0]
-            if "condition_code" in kwargs:
-                kwargs[
-                    "condition_code"
-                ] = f"{base_condition_code} and {kwargs['condition_code']}"
-            else:
-                kwargs["condition_code"] = base_condition_code
-
-        block_cls = (
-            ReduceConditionalBlock
-            if "condition_code" in kwargs
-            else ReduceBlock
+        works_with_not_none_only = self.get_option(
+            "works_with_not_none_only", ctx
         )
-        return block_cls(**kwargs)
-
-
-class Reduce(BaseReducer):
-    """Defines the reduce operation, which is based on a callable / expression
-    to be used during the aggregation"""
-
-    initial: t.Any
-
-    def __init__(
-        self,
-        to_call_with_2_args: t.Union[t.Callable, InlineExpr],
-        *expressions: t.Tuple[t.Any, ...],
-        initial: t.Union[_None, t.Callable, InlineExpr, t.Any],
-        default: t.Union[_None, t.Callable, t.Any] = _none,
-        unconditional_init: bool = False,
-        where=None,
-    ):
-        """
-        Args:
-          to_call_with_2_args: defines the reduce function/expression
-          expressions: args to be passed to `to_call_with_2_args` after the
-            aggregation value
-          initial: defines the very first item to be passed to
-            `to_call_with_2_args` item. If callable, then the result of a call
-            is used. If a conversion is passed, it is resolved on the first
-            row met.
-          default: defines the value to be returned when there was nothing to
-            reduce in a group (e.g. the current reduce operation has filtered
-            out some rows, while an adjacent reduce operation has got
-            something to reduce, forming a group). If callable, then the result
-            of a call is used.  When default is not passed, initial is used if
-            it doesn't depend on input data.
-          unconditional_init: tells whether the first call initializes the
-            aggregation value OR there is a condition for that
-        """
-        super().__init__(default, initial)
-        self.where = (
-            _none
-            if (where is None or where is _none)
-            else self.ensure_conversion(where)
-        )
-        self.to_call_with_2_args = self.ensure_conversion(to_call_with_2_args)
-        self.expressions = tuple(
-            self.ensure_conversion(expr) for expr in expressions
-        )
-        self.unconditional_init = unconditional_init
-
-    def gen_reduce_code_block(
-        self,
-        var_agg_data_value: str,
-        reducer_code_input: str,
-        checksum_flag: int,
-        ctx: dict,
-    ) -> ReduceBlockType:
-        _ = self.to_call_with_2_args.call_like(
-            self.initial,
-            *self.expressions,
-        ).gen_code_and_update_ctx(reducer_code_input, ctx)
-        reduce_initial = [f"%(result)s = {_}"]
-        _ = self.to_call_with_2_args.call_like(
-            EscapedString("%(result)s"),
-            *self.expressions,
-        ).gen_code_and_update_ctx(reducer_code_input, ctx)
-        reduce_two = [f"%(result)s = {_}"]
+        values_use_times = self.get_option("values_use_times", ctx)
 
-        kwargs = {
-            "reduce_initial": reduce_initial,
-            "reduce_two": reduce_two,
-            "reducer_code_input": reducer_code_input,
-            "var_agg_data_value": var_agg_data_value,
-            "checksum_flag": checksum_flag,
-            "unconditional_init": self.unconditional_init,
-        }
-        if self.where is not _none:
-            condition_code = self.where.gen_code_and_update_ctx(
+        prev_reduce_code = reduce_code
+        for index, expression in enumerate(self.expressions):
+            expression_code = expression.gen_code_and_update_ctx(
                 reducer_code_input, ctx
             )
-            if condition_code != "True":
-                kwargs["condition_code"] = condition_code
-
-        block_cls = (
-            ReduceConditionalBlock
-            if "condition_code" in kwargs
-            else ReduceBlock
-        )
-
-        return block_cls(**kwargs)
-
-
-class GroupBy:
-    """Generates the function which aggregates the data, grouping by
-    conversions, specified in `__init__` method and returns list of items in a
-    format defined by the parameter passed to ``aggregate`` method.
-
-    If no group keys are passed, then it returns just a single value, defined
-    by the parameter passed to ``aggregate`` method.
-
-    Current optimizations:
-     * piping like ``c.group_by(...).aggregate().pipe(...)`` won't run
-       the aggregation twice, this is handled as 2 statements
-     * using the same reduce clause twice (e.g. one used as an argument
-       for some function calls) won't result in calculating this reduce twice
-    """
-
-    def __init__(self, *by):
-        """Takes any number of conversions to group by
-
-        Args:
-          by (tuple): each item is to be wrapped with
-            :py:obj:`ensure_conversion`.  Each is to resolve to a hashable
-            object to allow using such tuples as keys. If nothing is passed,
-            aggregate the input into a single object.
-        """
-        self.by = by
-
-    def aggregate(
-        self, reducer: t.Union[dict, list, set, tuple, BaseConversion]
-    ) -> "Grouper":
-        return Grouper(self.by, reducer)
-
-
-def delegate_input_switching_method(name, force_iter_first=False):
-    def method(self, *args, **kwargs):
-        conversion = self.conversion
-        if force_iter_first:
-            conversion = conversion.to_iter()
-        return Grouper(
-            by=self.by,
-            reducer=self.reducer,
-            conversion=getattr(conversion, name)(*args, **kwargs),
-        )
-
-    return method
-
-
-class Grouper(BaseConversion):
-    """Fully initialized GroupBy conversion, which delegates some of methods
-    like iter to its internals"""
-
-    self_content_type = (
-        BaseConversion.self_content_type
-        | BaseConversion.ContentTypes.AGGREGATION
-        | BaseConversion.ContentTypes.NONE_USAGE
-    )
-
-    SIGNATURE_NAME = "signature"
-    AGG_DATA_NAME = "agg_data"
-    AGG_RESULT_ITEM_NAME = "agg_result_item"
-    SIGNATURE = Namespace(
-        LazyEscapedString(SIGNATURE_NAME), {SIGNATURE_NAME: None}
-    )
-    AGG_DATA = Namespace(
-        LazyEscapedString(AGG_DATA_NAME), {AGG_DATA_NAME: None}
-    )
-    AGG_RESULT_ITEM = Namespace(
-        LazyEscapedString(AGG_RESULT_ITEM_NAME), {AGG_RESULT_ITEM_NAME: None}
-    )
-    AGG_RESULT_ITEM.weight = Weights.UNPREDICTABLE
+            none_check_needed = works_with_not_none_only[
+                index
+            ] and not expression.has_hint(BaseConversion.OutputHints.NOT_NONE)
+            if (
+                none_check_needed + values_use_times[index] > 1
+                and expression is not This
+            ):
+                prev_reduce_code.add_assignment(expression_code)
 
-    def __init__(self, by, reducer, conversion=None):
-        super().__init__()
-        self.by = [self.ensure_conversion(by_) for by_ in by]
-        self.reducer = self.ensure_conversion(reducer)
-        self.contents = self.contents & ~self.ContentTypes.REDUCER
-        self.number_of_input_uses = 1
-        self.aggregate_mode = len(self.by) == 0
+            expression_code = prev_reduce_code.use_expression(expression_code)
 
-        if conversion:
-            self.conversion = self.ensure_conversion(conversion)
-        else:
-            self.conversion = self.ensure_conversion(
-                ListComp(
-                    GeneratorItem(
-                        self.AGG_RESULT_ITEM,
-                        self.SIGNATURE,
-                        self.AGG_DATA,
-                    ),
-                    _none,
-                    _none,
+            if none_check_needed:
+                reduce_code = reduce_code.add_condition(
+                    f"{expression_code} is not None"
                 )
-                if len(self.by)
-                else self.AGG_RESULT_ITEM
-            )
 
-    to_iter = delegate_input_switching_method("to_iter")
-    iter = delegate_input_switching_method("iter", True)
-    iter_mut = delegate_input_switching_method("iter_mut", True)
-    iter_windows = delegate_input_switching_method("iter_windows", True)
-    filter = delegate_input_switching_method("filter")
-    flatten = delegate_input_switching_method("flatten", True)
-    take_while = delegate_input_switching_method("take_while", True)
-    drop_while = delegate_input_switching_method("drop_while", True)
-    as_type = delegate_input_switching_method("as_type", True)
-    sort = delegate_input_switching_method("sort", True)
-    tap = delegate_input_switching_method("tap", True)
+            kwargs[f"value{index}"] = expression_code
 
-    def _gen_agg_data_container(self, container_name, number_of_reducers, ctx):
-        attrs = [f"v{i}" for i in range(number_of_reducers)]
+        reduce_lines = self.get_option("reduce_lines", ctx)
 
-        code = Code()
-        code.add_line(f"class {container_name}:", 1)
-        _ = ",".join(f"'{attr}'" for attr in attrs)
-        code.add_line(f"__slots__ = [{_}]", 0)
-        code.add_line("def __init__(self, _none=__none__):", 1)
-        if attrs:
-            for attr in attrs:
-                code.add_line(f"self.{attr} = _none", 0)
+        if not isinstance(self.initial, _None) and self.internals_are_public:
+            prepare_first_lines = (
+                f"%(result)s = {self.initial.gen_code_and_update_ctx(var_row, ctx)}",
+            ) + reduce_lines
         else:
-            code.add_line("pass", 0)
-        return ctx[
-            self.compile_converter(container_name, code.to_string(0), ctx)
-        ]
-
-    def _gen_code_and_update_ctx(self, code_input, ctx) -> str:
-        ctx["defaultdict"] = defaultdict
-        ctx["ListSortedOnceWrapper"] = ListSortedOnceWrapper
-
-        suffix = self.gen_random_name("_", ctx)
-        var_row = f"row{suffix}"
-        var_signature = f"signature{suffix}"
-        var_signature_to_agg_data = f"signature_to_agg_data{suffix}"
-        var_agg_data = f"agg_data{suffix}"
-        var_agg_data_cls = f"AggData{suffix}"
-
-        function_ctx = self.as_function_ctx(ctx, optimize_naive=True)
-        function_ctx.add_arg("data_", This())
-
-        with function_ctx:
-            reduce_blocks = ReduceBlocks(var_agg_data, self.aggregate_mode)
-            if "exchange_reducer_code_input_methods" not in ctx:
-                ctx["exchange_reducer_code_input_methods"] = []
+            prepare_first_lines = self.get_option("prepare_first_lines", ctx)
 
-            ctx["exchange_reducer_code_input_methods"].append(
-                reduce_blocks.exchange_reducer_code_input
+        new_agg_data_value = reduce_code.add_reduce_lines(
+            var_agg_data_value,
+            tuple(line % kwargs for line in prepare_first_lines),
+            tuple(line % kwargs for line in reduce_lines),
+        )
+        return new_agg_data_value
+
+
+class OptionalExpressionReducer(BaseReducer):
+    def check_expressions(self):
+        super().check_expressions()
+        if len(self.expressions) > 1:
+            warnings.warn(
+                "2.0 will raise TypeError if more than 1 expression is "
+                f"passed to {self.__class__.__name__}",
+                DeprecationWarning,
             )
-            try:
-                code_agg_result = self.reducer.gen_code_and_update_ctx(
-                    var_row, ctx
-                )
-            finally:
-                ctx["exchange_reducer_code_input_methods"].pop()
-                if not ctx["exchange_reducer_code_input_methods"]:
-                    del ctx["exchange_reducer_code_input_methods"]
 
-            by_is_single = len(self.by) == 1
-            code_signature = []
-            for index, by_ in enumerate(self.by):
-                code_by = by_.gen_code_and_update_ctx(var_row, ctx)
-                code_signature.append(code_by)
-                code_agg_result = self.replace_word(
-                    code_agg_result,
-                    code_by,
-                    (
-                        var_signature
-                        if by_is_single
-                        else f"{var_signature}[{index}]"
-                    ),
-                )
 
-            code_signature = (
-                code_signature[0]
-                if by_is_single
-                else f"({', '.join(code_signature)})"
+class SingleExpressionReducer(BaseReducer):
+    def check_expressions(self):
+        super().check_expressions()
+        expressions_len = len(self.expressions)
+        if expressions_len < 1:
+            raise ValueError("expected one expression")
+
+        if expressions_len > 1:
+            warnings.warn(
+                "2.0 will raise TypeError if more than 1 expression is "
+                f"passed to {self.__class__.__name__}",
+                DeprecationWarning,
             )
 
-            if var_row in code_agg_result:
-                raise ConversionException(
-                    "something other than group_by keys and reducers have been used",
-                    code_agg_result,
-                )
 
-            with NamespaceCtx(
-                {
-                    self.SIGNATURE_NAME: var_signature,
-                    self.AGG_DATA_NAME: var_agg_data,
-                    self.AGG_RESULT_ITEM_NAME: code_agg_result,
-                },
-                ctx,
-            ):
-                code_final_result = (
-                    self.conversion.gen_code_and_update_ctx(None, ctx)
-                    if self.aggregate_mode
-                    else self.conversion.gen_code_and_update_ctx(
-                        f"{var_signature_to_agg_data}.items()", ctx
-                    )
-                )
-
-            agg_template_kwargs = {
-                "code_args": function_ctx.get_def_all_args_code(),
-                "code_result": f"    return {code_final_result}",
-                "var_row": var_row,
-            }
-
-            if self.aggregate_mode:
-                converter_name = f"aggregate{suffix}"
-                grouper_code = AGGREGATE_TEMPLATE.format(
-                    converter_name=converter_name,
-                    code_init_agg_vars=f"{' = '.join(reduce_blocks.agg_data_values)} = _none",
-                    var_checksum=ReduceBlock.var_checksum,
-                    code_aggregate=reduce_blocks.gen_aggregate_code(
-                        var_row=var_row,
-                        expected_checksum=reduce_blocks.number,
-                    ).to_string(
-                        base_indent_level=1,
-                    ),
-                    **agg_template_kwargs,
-                )
-            else:
-                converter_name = f"group_by{suffix}"
-                ctx[var_agg_data_cls] = self._gen_agg_data_container(
-                    var_agg_data_cls, reduce_blocks.number, ctx
-                )
-                grouper_code = GROUPER_TEMPLATE.format(
-                    converter_name=converter_name,
-                    var_signature_to_agg_data=var_signature_to_agg_data,
-                    var_agg_data_cls=var_agg_data_cls,
-                    var_agg_data=var_agg_data,
-                    code_signature=code_signature,
-                    code_group_by=reduce_blocks.gen_group_by_code(
-                        var_row=var_row,
-                        var_agg_data=var_agg_data,
-                        var_signature_to_agg_data=var_signature_to_agg_data,
-                        code_signature=code_signature,
-                    ).to_string(base_indent_level=1),
-                    **agg_template_kwargs,
-                )
+class BaseDictReducer(BaseReducer):
+    """This reducer accepts 2 expressions:
 
-            conversion = function_ctx.gen_conversion(
-                converter_name, grouper_code
-            )
-        return function_ctx.call_with_all_args(
-            conversion
-        ).gen_code_and_update_ctx(code_input, ctx)
+    - the first one is used to calculate keys of the resulting dict
+    - the second one is used to calculate values to be reduced and put as the
+      final value, under the certain key.
 
+    Effectively dict reducers allow for double grouping: the first one on the
+    top level, the second one on DictReducer level.
+    """
 
-def Aggregate(  # pylint:disable=invalid-name
-    *args, **kwargs
-) -> BaseConversion:
-    """Shortcut for ``GroupBy().aggregate(*args, **kwargs)``"""
-    return GroupBy().aggregate(*args, **kwargs)
+    def check_expressions(self):
+        super().check_expressions()
+        expressions_len = len(self.expressions)
+        if expressions_len == 2:
+            return
 
+        if expressions_len == 1:
+            expr = self.expressions[0]
+            if (
+                isinstance(expr, (Tuple, List))
+                and expr.conversions is not None
+                and len(expr.conversions) == 2
+            ):
+                self.expressions = tuple(expr.conversions)
+                return
+        raise ValueError("invalid dict reducer input: two values expected")
 
-class ReducerDispatcher:
-    pass
 
+class SumReducer(SingleExpressionReducer):
+    """Takes a sum, None is considered as 0"""
 
-class SumReducer(MultiStatementReducer):
-    prepare_first = ("%(result)s = ({0} or 0)",)
-    reduce = ("%(result)s = {prev_result} + ({0} or 0)",)
     default = NaiveConversion(0)
-    unconditional_init = True
+    internals_are_public = True
+    values_use_times = (1,)  # TODO set to 1 once debugged
+    works_with_not_none_only = (False,)
+
+    def prepare_first_lines(self, ctx):  # pylint: disable=unused-argument
+        if self.expressions[0].has_hint(BaseConversion.OutputHints.NOT_NONE):
+            return ("%(result)s = %(value0)s",)
+        return ("%(result)s = %(value0)s or 0",)
+
+    def reduce_lines(self, ctx):  # pylint: disable=unused-argument
+        if self.expressions[0].has_hint(BaseConversion.OutputHints.NOT_NONE):
+            return ("%(result)s += %(value0)s",)
+        return ("%(result)s += %(value0)s or 0",)
 
 
-class FastSumReducer(MultiStatementReducer):
-    prepare_first = ("%(result)s = ({0} or 0)",)
-    reduce = ("%(result)s = {prev_result} + {0}",)
-    default = NaiveConversion(0)
-    unconditional_init = True
-
+class SumOrNoneReducer(SingleExpressionReducer):
+    """Takes a sum, if at least one None is met, the result is None"""
 
-class SumReducerDispatcher(ReducerDispatcher):
-    def __call__(self, expression, *args, **kwargs):
-        expression = ensure_conversion(expression)
-        if expression.output_hints & expression.OutputHints.NOT_NONE:
-            return FastSumReducer(expression, *args, **kwargs)
-        return SumReducer(expression, *args, **kwargs)
-
-
-class SumOrNoneReducer(MultiStatementReducer):
-    prepare_first = ("%(result)s = {0}",)
-    reduce = (
-        "if {0} is None:",
-        "    %(result)s = None",
-        "elif %(result)s is not None:",
-        "    %(result)s = {prev_result} + {0}",
-    )
     default = NaiveConversion(None)
-    unconditional_init = True
+    internals_are_public = True
+    works_with_not_none_only = (False,)
+    prepare_first_lines = ("%(result)s = %(value0)s",)
+
+    def values_use_times(self, ctx):  # pylint: disable=unused-argument
+        if self.expressions[0].has_hint(BaseConversion.OutputHints.NOT_NONE):
+            return (1,)
+        return (2,)
+
+    def reduce_lines(self, ctx):  # pylint: disable=unused-argument
+        if self.expressions[0].has_hint(BaseConversion.OutputHints.NOT_NONE):
+            return ("%(result)s += %(value0)s",)
+        return (
+            "if %(value0)s is None:",
+            "    %(result)s = None",
+            "elif %(result)s is not None:",
+            "    %(result)s += %(value0)s",
+        )
 
 
-class MaxReducer(MultiStatementReducer):
-    base_condition_code = "{0} is not None"
-    prepare_first = ("%(result)s = {0}",)
-    reduce = (
-        "if {0} > %(result)s:",
-        "    %(result)s = {0}",
-    )
+class MaxReducer(SingleExpressionReducer):
     default = NaiveConversion(None)
-    unconditional_init = True
+    internals_are_public = True
+    values_use_times = (2,)
+    works_with_not_none_only = (True,)
+    prepare_first_lines = ("%(result)s = %(value0)s",)
+    reduce_lines = (
+        "if %(result)s < %(value0)s:",
+        "    %(result)s = %(value0)s",
+    )
 
 
-class MinReducer(MultiStatementReducer):
-    base_condition_code = "{0} is not None"
-    prepare_first = ("%(result)s = {0}",)
-    reduce = (
-        "if {0} < %(result)s:",
-        "    %(result)s = {0}",
-    )
+class MinReducer(SingleExpressionReducer):
     default = NaiveConversion(None)
-    unconditional_init = True
+    internals_are_public = True
+    values_use_times = (2,)
+    works_with_not_none_only = (True,)
+    prepare_first_lines = ("%(result)s = %(value0)s",)
+    reduce_lines = (
+        "if %(result)s > %(value0)s:",
+        "    %(result)s = %(value0)s",
+    )
 
 
-class CountReducer(MultiStatementReducer):
-    prepare_first = ("%(result)s = 1",)
-    reduce = ("%(result)s = {prev_result} + 1",)
+class CountReducer(OptionalExpressionReducer):
+    """Counts objects. It accepts either zero or one expression as an argument and:
+    - if zero expressions passed: counts number of rows
+    - one expression: counts not None values of the evaluated expression
+    """
+
     default = NaiveConversion(0)
-    unconditional_init = True
+    internals_are_public = True
+    values_use_times = (0,)
+    prepare_first_lines = ("%(result)s = 1",)
+    reduce_lines = ("%(result)s += 1",)
+
+    def works_with_not_none_only(self, ctx):  # pylint: disable=unused-argument
+        if len(self.expressions) == 1 and not self.expressions[0].has_hint(
+            BaseConversion.OutputHints.NOT_NONE
+        ):
+            return (True,)
+        return (False,)
 
 
-class CountDistinctReducer(MultiStatementReducer):
-    prepare_first = ("%(result)s = {{ {0} }}",)
-    reduce = ("%(result)s.add({0})",)
+class CountDistinctReducer(SingleExpressionReducer):
     default = NaiveConversion(0)
-    unconditional_init = True
-    post_conversion = CallFunc(len, This())
+    internals_are_public = False
+    values_use_times = (1,)
+    works_with_not_none_only = (False,)
+    prepare_first_lines = ("%(result)s = {%(value0)s}",)
+    reduce_lines = ("%(result)s.add(%(value0)s)",)
+    post_conversion = CallFunc(len, This)
 
 
-class FirstReducer(MultiStatementReducer):
-    prepare_first = ("%(result)s = {0}",)
-    reduce = ()
+class FirstReducer(SingleExpressionReducer):
     default = NaiveConversion(None)
-    unconditional_init = True
+    internals_are_public = False
+    values_use_times = (1,)
+    works_with_not_none_only = (False,)
+    prepare_first_lines = ("%(result)s = %(value0)s",)
+    reduce_lines = ()
 
 
-class LastReducer(MultiStatementReducer):
-    prepare_first = ("%(result)s = {0}",)
-    reduce = ("%(result)s = {0}",)
+class LastReducer(SingleExpressionReducer):
     default = NaiveConversion(None)
-    unconditional_init = True
+    internals_are_public = False
+    values_use_times = (1,)
+    works_with_not_none_only = (False,)
+    prepare_first_lines = ("%(result)s = %(value0)s",)
+    reduce_lines = ("%(result)s = %(value0)s",)
 
 
-class MaxRowReducer(MultiStatementReducer):
-    """Reducer which finds an item with max value of the expression and returns
-    this item"""
+class MaxRowReducer(SingleExpressionReducer):
+    """Returns a row with a max value of object, defined by the argument"""
 
-    base_condition_code = "{0} is not None"
-    prepare_first = ("%(result)s = ({0}, %(input)s)",)
-    reduce = (
-        "if %(result)s[0] < {0}:",
-        "    %(result)s = ({0}, %(input)s)",
-    )
     default = NaiveConversion(None)
+    internals_are_public = False
+    values_use_times = (2,)
+    works_with_not_none_only = (True,)
+    prepare_first_lines = ("%(result)s = (%(value0)s, %(row)s)",)
+    reduce_lines = (
+        "if %(result)s[0] < %(value0)s:",
+        "    %(result)s = (%(value0)s, %(row)s)",
+    )
     post_conversion = GetItem(1)
-    unconditional_init = True
 
 
-class MinRowReducer(MaxRowReducer):
-    reduce = (
-        "if %(result)s[0] > {0}:",
-        "    %(result)s = ({0}, %(input)s)",
+class MinRowReducer(SingleExpressionReducer):
+    """Returns a row with a min value of object, defined by the argument"""
+
+    default = NaiveConversion(None)
+    internals_are_public = False
+    values_use_times = (2,)
+    works_with_not_none_only = (True,)
+    prepare_first_lines = ("%(result)s = (%(value0)s, %(row)s)",)
+    reduce_lines = (
+        "if %(result)s[0] > %(value0)s:",
+        "    %(result)s = (%(value0)s, %(row)s)",
     )
+    post_conversion = GetItem(1)
+
+    def check_expressions(self):
+        super().check_expressions()
+        if not isinstance(self.initial, _None):
+            warnings.warn(
+                "2.0 will raise ValueError if initial is "
+                f"passed to {self.__class__.__name__}",
+                DeprecationWarning,
+            )
 
 
-class ArrayReducer(MultiStatementReducer):
-    prepare_first = ("%(result)s = [{0}]",)
-    reduce = ("%(result)s.append({0})",)
+class ArrayReducer(SingleExpressionReducer):
     default = NaiveConversion(None)
-    unconditional_init = True
+    internals_are_public = True
+    values_use_times = (1,)
+    works_with_not_none_only = (False,)
+    prepare_first_lines = ("%(result)s = [%(value0)s]",)
+    reduce_lines = ("%(result)s.append(%(value0)s)",)
 
 
 class ListSortedOnceWrapper:
     """Wraps a list, exposes append method only. Once the list is filled up, it
     is sorted (only once) in-place and is returned when get method called."""
 
     __slots__ = ["list_", "append", "sorted", "key", "reverse"]
@@ -1024,224 +664,314 @@
         if not self.sorted:
             self.list_.sort(key=self.key, reverse=self.reverse)
             self.sorted = True
             del self.append
         return self.list_
 
 
-class SortedArrayReducer(MultiStatementReducer):
+class SortedArrayReducer(SingleExpressionReducer):
     """Array reducer which sorts the list just once in the end"""
 
-    reduce = ("%(result)s.append({0})",)
     default = NaiveConversion(None)
-    unconditional_init = True
+    internals_are_public = False
+    values_use_times = (1,)
+    works_with_not_none_only = (False,)
+    reduce_lines = ("%(result)s.append(%(value0)s)",)
+    post_conversion = This.call_method("get")
 
     def __init__(self, *args, key=None, reverse=False, **kwargs):
         super().__init__(*args, **kwargs)
         self.key = self.ensure_conversion(key)
         self.reverse = self.ensure_conversion(reverse)
 
-    def prepare_first(self, ctx):
-        key_code = self.key.gen_code_and_update_ctx("{0}", ctx)
-        reverse_code = self.reverse.gen_code_and_update_ctx("{0}", ctx)
+    def prepare_first_lines(self, ctx):
+        key_code = self.key.gen_code_and_update_ctx("%(value0)s", ctx)
+        reverse_code = self.reverse.gen_code_and_update_ctx("%(value0)s", ctx)
         return (
             "%(result)s = ListSortedOnceWrapper("
-            f"[{{0}}], {key_code}, {reverse_code})",
+            f"[%(value0)s], {key_code}, {reverse_code})",
         )
 
-    @property
-    def post_conversion(self):
-        return This().call_method("get")
 
-
-class ArrayDistinctReducer(MultiStatementReducer):
-    prepare_first = ("%(result)s = {{ {0}: None }}",)
-    reduce = ("%(result)s[{0}] = None",)
-    post_conversion = InlineExpr("list({0})").pass_args(This())
+class ArrayDistinctReducer(SingleExpressionReducer):
     default = NaiveConversion(None)
-    unconditional_init = True
-
-
-class BaseDictReducer(MultiStatementReducer):
-    """This reducer accepts 2 expressions:
-
-    - the first one is used to calculate keys of the resulting dict
-    - the second one is used to calculate values to be reduced and put as the
-      final value, under the certain key.
-
-    Effectively dict reducers allow for double grouping: the first one on the
-    top level, the second one on DictReducer level.
-    """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        # for backward compatibility with versions <= 0.8
-        if len(self.expressions) == 1:
-            expr = self.expressions[0]
-            if isinstance(expr, (Tuple, List)) and len(expr.items) == 2:
-                self.expressions = tuple(expr.items)
-        if len(self.expressions) != 2:
-            raise ValueError("invalid dict reducer input: two values expected")
+    internals_are_public = False
+    values_use_times = (1,)
+    works_with_not_none_only = (False,)
+    prepare_first_lines = ("%(result)s = { %(value0)s: None }",)
+    reduce_lines = ("%(result)s[%(value0)s] = None",)
+    post_conversion = This.as_type(list)
 
 
 class DictReducer(BaseDictReducer):
-    prepare_first = ("%(result)s = {{ {0}: {1} }}",)
-    reduce = ("%(result)s[{0}] = {1}",)
+    """Aggregates values to a dict:
+    - keys: defined by the first argument
+    - values: defined by the second argument, reduced with Last."""
+
     default = NaiveConversion(None)
-    unconditional_init = True
+    internals_are_public = False
+    values_use_times = (1, 1)
+    works_with_not_none_only = (False, False)
+    prepare_first_lines = ("%(result)s = { %(value0)s: %(value1)s }",)
+    reduce_lines = ("%(result)s[%(value0)s] = %(value1)s",)
 
 
 lock_default_dict_conversion = InlineExpr(
     'setattr({this_}, "default_factory", None) or {this_}'
-).pass_args(this_=This())
+).pass_args(this_=This)
 
 
 class DictArrayReducer(BaseDictReducer):
-    prepare_first = (
-        "%(result)s = _d = defaultdict(list)",
-        "_d[{0}].append({1})",
+    """Aggregates values to a dict:
+    - keys: defined by the first argument
+    - values: defined by the second argument, reduced with Array."""
+
+    default = NaiveConversion(None)
+    internals_are_public = False
+    values_use_times = (1, 1)
+    works_with_not_none_only = (False, False)
+    prepare_first_lines = (
+        "%(result)s = defaultdict(list)",
+        "%(result)s[%(value0)s].append(%(value1)s)",
     )
-    reduce = ("%(result)s[{0}].append({1})",)
+    reduce_lines = ("%(result)s[%(value0)s].append(%(value1)s)",)
     post_conversion = lock_default_dict_conversion
-    default = NaiveConversion(None)
-    unconditional_init = True
 
 
 class DictArrayDistinctReducer(BaseDictReducer):
-    """Dict reducer where dict values are lists of distinct values"""
+    """Aggregates values to a dict:
+    - keys: defined by the first argument
+    - values: defined by the second argument, reduced with ArrayDistinct."""
 
-    prepare_first = (
-        "%(result)s = _d = defaultdict(dict)",
-        "_d[{0}][{1}] = None",
+    default = NaiveConversion(None)
+    internals_are_public = False
+    values_use_times = (1, 1)
+    works_with_not_none_only = (False, False)
+    prepare_first_lines = (
+        "%(result)s = defaultdict(dict)",
+        "%(result)s[%(value0)s][%(value1)s] = None",
     )
-    reduce = ("%(result)s[{0}][{1}] = None",)
+    reduce_lines = ("%(result)s[%(value0)s][%(value1)s] = None",)
     post_conversion = InlineExpr(
         "{{k_: list(v_) for k_, v_ in {}.items()}}"
-    ).pass_args(This())
-    default = NaiveConversion(None)
-    unconditional_init = True
+    ).pass_args(This)
 
 
 class DictSumReducer(BaseDictReducer):
-    prepare_first = (
-        "%(result)s = _d = defaultdict(int)",
-        "_d[{0}] = {1} or 0",
+    """Aggregates values to a dict:
+    - keys: defined by the first argument
+    - values: defined by the second argument, reduced with Sum
+       * None is considered 0"""
+
+    default = NaiveConversion(None)
+    internals_are_public = False
+    values_use_times = (1, 1)
+    works_with_not_none_only = (False, False)
+    prepare_first_lines = (
+        "%(result)s = defaultdict(int)",
+        "%(result)s[%(value0)s] = %(value1)s or 0",
     )
-    reduce = ("%(result)s[{0}] = {prev_result}[{0}] + ({1} or 0)",)
     post_conversion = lock_default_dict_conversion
-    default = NaiveConversion(None)
-    unconditional_init = True
+
+    def reduce_lines(self, ctx):  # pylint: disable=unused-argument
+        if self.expressions[1].has_hint(BaseConversion.OutputHints.NOT_NONE):
+            return ("%(result)s[%(value0)s] += %(value1)s",)
+        return ("%(result)s[%(value0)s] += (%(value1)s or 0)",)
 
 
 class DictSumOrNoneReducer(BaseDictReducer):
-    """Dict reducer where dict values are either numbers or None if there's
-    been at least one None value within the group"""
+    """Aggregates values to a dict:
+    - keys: defined by the first argument
+    - values: defined by the second argument, reduced with SumOrNone
+       * if at least one None is met, the result is None"""
 
-    prepare_first = ("%(result)s = _d = defaultdict(int)", "_d[{0}] = {1}")
-    reduce = (
-        "if {1} is None:",
-        "    %(result)s[{0}] = None",
-        "elif %(result)s[{0}] is not None:",
-        "    %(result)s[{0}] = {prev_result}[{0}] + {1}",
+    default = NaiveConversion(None)
+    internals_are_public = False
+    works_with_not_none_only = (False, False)
+    prepare_first_lines = (
+        "%(result)s = defaultdict(int)",
+        "%(result)s[%(value0)s] = %(value1)s",
     )
     post_conversion = lock_default_dict_conversion
-    default = NaiveConversion(None)
-    unconditional_init = True
+
+    def values_use_times(self, ctx):  # pylint: disable=unused-argument
+        if self.expressions[1].has_hint(BaseConversion.OutputHints.NOT_NONE):
+            return (1, 1)
+        return (2, 2)
+
+    def reduce_lines(self, ctx):  # pylint: disable=unused-argument
+        if self.expressions[1].has_hint(BaseConversion.OutputHints.NOT_NONE):
+            return ("%(result)s[%(value0)s] += %(value1)s",)
+        return (
+            "if %(value1)s is None:",
+            "    %(result)s[%(value0)s] = None",
+            "elif %(result)s[%(value0)s] is not None:",
+            "    %(result)s[%(value0)s] += %(value1)s",
+        )
 
 
 class DictMaxReducer(BaseDictReducer):
-    """DictMax reducer which takes first positional item as keys and
-    accumulates max value of second positional item"""
+    """Aggregates values to a dict:
+    - keys: defined by the first argument
+    - values: defined by the second argument, reduced with Max."""
 
-    base_condition_code = "{1} is not None"
-    prepare_first = ("%(result)s = {{ {0}: {1} }}",)
-    reduce = (
-        "if {0} not in %(result)s or {1} > %(result)s[{0}]:",
-        "    %(result)s[{0}] = {1}",
-    )
     default = NaiveConversion(None)
-    unconditional_init = True
+    internals_are_public = False
+    values_use_times = (1, 1)
+    prepare_first_lines = ("%(result)s = { %(value0)s: %(value1)s }",)
+
+    def works_with_not_none_only(self, ctx):  # pylint: disable=unused-argument
+        if self.expressions[1].has_hint(BaseConversion.OutputHints.NOT_NONE):
+            return (False, False)
+        return (False, True)
+
+    def reduce_lines(self, ctx):  # pylint: disable=unused-argument
+        return (
+            "if %(value0)s not in %(result)s or %(value1)s > %(result)s[%(value0)s]:",
+            "    %(result)s[%(value0)s] = %(value1)s",
+        )
 
 
-class DictMinReducer(DictMaxReducer):
-    reduce = (
-        "if {0} not in %(result)s or {1} < %(result)s[{0}]:",
-        "    %(result)s[{0}] = {1}",
-    )
+class DictMinReducer(BaseDictReducer):
+    """Aggregates values to a dict:
+    - keys: defined by the first argument
+    - values: defined by the second argument, reduced with Min."""
+
+    default = NaiveConversion(None)
+    internals_are_public = False
+    values_use_times = (1, 1)
+    prepare_first_lines = ("%(result)s = { %(value0)s: %(value1)s }",)
+
+    def works_with_not_none_only(self, ctx):  # pylint: disable=unused-argument
+        if self.expressions[1].has_hint(BaseConversion.OutputHints.NOT_NONE):
+            return (False, False)
+        return (False, True)
+
+    def reduce_lines(self, ctx):  # pylint: disable=unused-argument
+        return (
+            "if %(value0)s not in %(result)s or %(value1)s < %(result)s[%(value0)s]:",
+            "    %(result)s[%(value0)s] = %(value1)s",
+        )
 
 
 class DictCountReducer(BaseDictReducer):
-    prepare_first = ("%(result)s = {{ {0}: 1 }}",)
-    reduce = (
-        "if {0} not in %(result)s:",
-        "    %(result)s[{0}] = 1",
+    """Aggregates values to a dict:
+    - keys: defined by the first argument
+    - values: defined by the second argument (optional), reduced with Count.
+       * counts rows if no 2nd arg is passed
+       * counts non None values if 2nd arg is passed"""
+
+    default = NaiveConversion(None)
+    internals_are_public = False
+    values_use_times = (2, 0)
+    prepare_first_lines = ("%(result)s = { %(value0)s: 1 }",)
+    reduce_lines = (
+        "if %(value0)s not in %(result)s:",
+        "    %(result)s[%(value0)s] = 1",
         "else:",
-        "    %(result)s[{0}] = {prev_result}[{0}] + 1",
+        "    %(result)s[%(value0)s] += 1",
     )
-    default = NaiveConversion(None)
-    unconditional_init = True
+
+    def check_expressions(self):
+        BaseReducer.check_expressions(self)
+        expressions_len = len(self.expressions)
+        if expressions_len == 2:
+            return
+
+        if expressions_len == 1:
+            expr = self.expressions[0]
+            if (
+                isinstance(expr, (Tuple, List))
+                and expr.conversions is not None
+                and len(expr.conversions) == 2
+            ):
+                self.expressions = tuple(expr.conversions)
+        else:
+            raise ValueError("invalid dict reducer input: two values expected")
+
+    def works_with_not_none_only(self, ctx):  # pylint: disable=unused-argument
+        if len(self.expressions) == 2 and not self.expressions[1].has_hint(
+            BaseConversion.OutputHints.NOT_NONE
+        ):
+            return (False, True)
+        return (False, False)
 
 
 class DictCountDistinctReducer(BaseDictReducer):
-    """Dict reducer where dict values are numbers of distinct values per
-    group"""
+    """Aggregates values to a dict:
+    - keys: defined by the first argument
+    - values: defined by the second argument, reduced with CountDistinct."""
 
-    prepare_first = ("%(result)s = {{ {0}: {{ {1} }} }}",)
-    reduce = (
-        "if {0} not in %(result)s:",
-        "    %(result)s[{0}] = {{ {1} }}",
+    default = NaiveConversion(None)
+    internals_are_public = False
+    values_use_times = (2, 1)
+    works_with_not_none_only = (False, False)
+    prepare_first_lines = ("%(result)s = { %(value0)s: { %(value1)s } }",)
+    reduce_lines = (
+        "if %(value0)s not in %(result)s:",
+        "    %(result)s[%(value0)s] = { %(value1)s }",
         "else:",
-        "    %(result)s[{0}].add({1})",
+        "    %(result)s[%(value0)s].add(%(value1)s)",
     )
     post_conversion = InlineExpr(
         "{{ k_: len(v_) for k_, v_ in {}.items() }}"
-    ).pass_args(This())
-    default = NaiveConversion(None)
-    unconditional_init = True
+    ).pass_args(This)
 
 
 class DictFirstReducer(BaseDictReducer):
-    prepare_first = ("%(result)s = {{ {0}: {1} }}",)
-    reduce = ("if {0} not in %(result)s:", "    %(result)s[{0}] = {1}")
+    """Aggregates values to a dict:
+    - keys: defined by the first argument
+    - values: defined by the second argument, reduced with First."""
+
     default = NaiveConversion(None)
-    unconditional_init = True
+    internals_are_public = False
+    values_use_times = (2, 1)
+    works_with_not_none_only = (False, False)
+    prepare_first_lines = ("%(result)s = { %(value0)s: %(value1)s }",)
+    reduce_lines = (
+        "if %(value0)s not in %(result)s:",
+        "    %(result)s[%(value0)s] = %(value1)s",
+    )
 
 
 class DictLastReducer(BaseDictReducer):
-    prepare_first = ("%(result)s = {{ {0}: {1} }}",)
-    reduce = ("%(result)s[{0}] = {1}",)
+    """Aggregates values to a dict:
+    - keys: defined by the first argument
+    - values: defined by the second argument, reduced with Last."""
+
     default = NaiveConversion(None)
-    unconditional_init = True
+    internals_are_public = False
+    values_use_times = (1, 1)
+    works_with_not_none_only = (False, False)
+    prepare_first_lines = ("%(result)s = { %(value0)s: %(value1)s }",)
+    reduce_lines = ("%(result)s[%(value0)s] = %(value1)s",)
 
 
-class AverageReducerDispatcher(ReducerDispatcher):
-    """Dispatcher which chooses between weighted and simple averages"""
+class ReducerDispatcher:
+    def __call__(self, *args, **kwargs) -> "BaseConversion":
+        raise NotImplementedError
+
 
-    sum_reducer_dispatcher = SumReducerDispatcher()
+class AverageReducerDispatcher(ReducerDispatcher):
+    """Calculates weighted average (default weight is 0)"""
 
     def __call__(
         self, value, weight=1, default=None, where=None
     ) -> "BaseConversion":
-        """
-        Calculates the arithmetic mean or weighted mean.
-        """
         if isinstance(weight, (int, float, Decimal)) and weight == 1:
             return If(
                 CountReducer(where=where),
-                (
-                    self.sum_reducer_dispatcher(value, where=where)
-                    / CountReducer(where=where)
-                ),
+                (SumReducer(value, where=where) / CountReducer(where=where)),
                 default,
             )
         return If(
-            self.sum_reducer_dispatcher(weight, where=where),
+            SumReducer(weight, where=where),
             (
-                self.sum_reducer_dispatcher(value * weight, where=where)
-                / self.sum_reducer_dispatcher(weight, where=where)
+                SumReducer(value * weight, where=where)
+                / SumReducer(weight, where=where)
             ),
             default,
         )
 
 
 class TopReducer(DictCountReducer):
     """
@@ -1253,30 +983,30 @@
         if not isinstance(k, int):
             raise TypeError("K must be an integer.")
 
         if k < 1:
             raise ValueError("K must be a positive integer greater than 0.")
 
         self.k = k
-        super().__init__(key_conv, 1, *args, **kwargs)
+        super().__init__(key_conv, *args, **kwargs)
 
-    @property
-    def post_conversion(self):
+    def post_conversion(self, ctx):  # pylint: disable=unused-argument
         return InlineExpr(
-            "[k for k,v in sorted((v,k) for k,v in {data}.items())[:-{k}:-1]]"
-        ).pass_args(data=This(), k=self.k + 1)
+            "[key for key, value in sorted((v, k) for k, v in {data}.items())[:-{k}:-1]]"
+        ).pass_args(data=This, k=self.k + 1)
 
 
 class ModeReducer(DictCountReducer):
     def __init__(self, conv, *args, **kwargs):
         super().__init__(conv, conv, *args, **kwargs)
 
+    # TODO: check how MaxRow performs here
     post_conversion = InlineExpr(
-        "sorted(((v,k) for k,v in {data}.items()))[-1][1]"
-    ).pass_args(data=This())
+        "sorted({data}.items(), key=lambda x: x[1])[-1][0]"
+    ).pass_args(data=This)
 
 
 class PercentileReducer(SortedArrayReducer):
     """Calculates percentile (floats from 0 to 100 inclusive)
 
     >>> c.ReduceFuncs.Percentile(95, c.item("amount"))
     >>> c.ReduceFuncs.Percentile(95, c.item("amount"), interpolation="lower")
@@ -1353,18 +1083,19 @@
         index = (len(data) - 1) * quantile
         left_index = int(index)
         if index - left_index > 0.5:
             return data[left_index + 1]
         else:
             return data[left_index]
 
-    @property
-    def post_conversion(self):
+    def post_conversion(self, ctx):  # pylint: disable=unused-argument
         return CallFunc(
-            self.method, super().post_conversion, self.percentile * 0.01
+            self.method,
+            This.call_method("get"),
+            self.percentile * 0.01,
         )
 
 
 PercentileReducer.interpolation_to_method = {
     "linear": PercentileReducer.percentile_linear,
     "lower": PercentileReducer.percentile_lower,
     "higher": PercentileReducer.percentile_higher,
@@ -1381,15 +1112,15 @@
 
 class ReduceFuncs:
     """Exposes the list of reduce functions"""
 
     # pylint: disable=invalid-name
 
     #: Calculates the sum, skips false values
-    Sum = SumReducerDispatcher()
+    Sum = SumReducer
     #: Calculates the sum, any ``None`` makes the total sum ``None``
     SumOrNone = SumOrNoneReducer
 
     #: Finds max value, skips ``None``
     Max = MaxReducer
     #: Finds a row with max value, skips ``None``
     MaxRow = MaxRowReducer
@@ -1451,7 +1182,314 @@
     #: Aggregates values into dict; dict values are numbers of unique values
     #: in groups
     DictCountDistinct = DictCountDistinctReducer
     #: Aggregates values into dict; dict values are first values per group
     DictFirst = DictFirstReducer
     #: Aggregates values into dict; dict values are last values per group
     DictLast = DictLastReducer
+
+
+class GroupBy:
+    """Generates the function which aggregates the data, grouping by
+    conversions, specified in `__init__` method and returns list of items in a
+    format defined by the parameter passed to ``aggregate`` method.
+
+    If no group keys are passed, then it returns just a single value, defined
+    by the parameter passed to ``aggregate`` method.
+
+    Current optimizations:
+     * piping like ``c.group_by(...).aggregate().pipe(...)`` won't run
+       the aggregation twice, this is handled as 2 statements
+     * using the same reduce clause twice (e.g. one used as an argument
+       for some function calls) won't result in calculating this reduce twice
+    """
+
+    def __init__(self, *by):
+        """Takes any number of conversions to group by
+
+        Args:
+          by (tuple): each item is to be wrapped with
+            :py:obj:`ensure_conversion`.  Each is to resolve to a hashable
+            object to allow using such tuples as keys. If nothing is passed,
+            aggregate the input into a single object.
+        """
+        self.by = by
+
+    def aggregate(
+        self, reducer: t.Union[dict, list, set, tuple, BaseConversion]
+    ) -> "Grouper":
+        return Grouper(self.by, reducer)
+
+
+def delegate_input_switching_method(name, force_iter_first=False):
+    def method(self, *args, **kwargs):
+        conversion = self.conversion
+        if force_iter_first:
+            conversion = conversion.to_iter()
+        return Grouper(
+            by=self.by,
+            reducer=self.reducer,
+            conversion=getattr(conversion, name)(*args, **kwargs),
+        )
+
+    return method
+
+
+GROUPER_TEMPLATE = """
+def {converter_name}({code_args}):
+    {var_signature_to_agg_data} = defaultdict({var_agg_data_cls})
+
+{code_group_by}
+
+{code_result}
+"""
+AGGREGATE_TEMPLATE = """
+def {converter_name}({code_args}):
+    {code_init_agg_vars}
+
+{code_aggregate}
+
+{code_result}
+"""
+
+
+class Grouper(BaseConversion):
+    """Fully initialized GroupBy conversion, which delegates some of methods
+    like iter to its internals"""
+
+    self_content_type = (
+        BaseConversion.self_content_type
+        | BaseConversion.ContentTypes.AGGREGATION
+        | BaseConversion.ContentTypes.NONE_USAGE
+    )
+
+    SIGNATURE_NAME = "signature"
+    AGG_DATA_NAME = "agg_data"
+    AGG_RESULT_ITEM_NAME = "agg_result_item"
+    SIGNATURE = Namespace(
+        LazyEscapedString(SIGNATURE_NAME), {SIGNATURE_NAME: None}
+    )
+    AGG_DATA = Namespace(
+        LazyEscapedString(AGG_DATA_NAME), {AGG_DATA_NAME: None}
+    )
+    AGG_RESULT_ITEM = Namespace(
+        LazyEscapedString(AGG_RESULT_ITEM_NAME), {AGG_RESULT_ITEM_NAME: None}
+    )
+    AGG_RESULT_ITEM.weight = Weights.UNPREDICTABLE
+
+    def __init__(self, by, reducer, conversion=None):
+        super().__init__()
+        self.by = [self.ensure_conversion(by_) for by_ in by]
+        self.reducer = self.ensure_conversion(reducer)
+        self.contents = self.contents & ~self.ContentTypes.REDUCER
+        self.number_of_input_uses = 1
+        self.aggregate_mode = len(self.by) == 0
+
+        if conversion:
+            self.conversion = self.ensure_conversion(conversion)
+        else:
+            self.conversion = self.ensure_conversion(
+                ListComp(
+                    GeneratorItem(
+                        self.AGG_RESULT_ITEM,
+                        self.SIGNATURE,
+                        self.AGG_DATA,
+                    ),
+                    _none,
+                    _none,
+                )
+                if len(self.by)
+                else self.AGG_RESULT_ITEM
+            )
+
+    to_iter = delegate_input_switching_method("to_iter")
+    iter = delegate_input_switching_method("iter", True)
+    iter_mut = delegate_input_switching_method("iter_mut", True)
+    iter_windows = delegate_input_switching_method("iter_windows", True)
+    filter = delegate_input_switching_method("filter")
+    flatten = delegate_input_switching_method("flatten", True)
+    take_while = delegate_input_switching_method("take_while", True)
+    drop_while = delegate_input_switching_method("drop_while", True)
+    as_type = delegate_input_switching_method("as_type", True)
+    sort = delegate_input_switching_method("sort", True)
+    tap = delegate_input_switching_method("tap", True)
+
+    def _gen_code_and_update_ctx(self, code_input, ctx) -> str:
+        ctx["defaultdict"] = defaultdict
+        ctx["ListSortedOnceWrapper"] = ListSortedOnceWrapper
+
+        suffix = self.gen_random_name("_", ctx)
+        var_row = f"row{suffix}"
+        var_signature = f"signature{suffix}"
+        var_signature_to_agg_data = f"signature_to_agg_data{suffix}"
+        var_agg_data = f"agg_data{suffix}"
+        var_agg_data_cls = f"AggData{suffix}"
+
+        function_ctx = self.as_function_ctx(ctx, optimize_naive=True)
+        function_ctx.add_arg("data_", This())
+
+        reduce_manager = ReduceManager(
+            var_row, var_agg_data, self.aggregate_mode
+        )
+        with function_ctx:
+            if "current_reduce_manager" not in ctx:
+                ctx["current_reduce_manager"] = [reduce_manager]
+            else:
+                ctx["current_reduce_manager"].append(reduce_manager)
+
+            try:
+                code_agg_result = self.reducer.gen_code_and_update_ctx(
+                    var_row, ctx
+                )
+            finally:
+                ctx["current_reduce_manager"].pop()
+                if not ctx["current_reduce_manager"]:
+                    del ctx["current_reduce_manager"]
+
+            by_is_single = len(self.by) == 1
+            code_signatures = []
+            for index, by_ in enumerate(self.by):
+                code_by = by_.gen_code_and_update_ctx(var_row, ctx)
+                code_signatures.append(code_by)
+                code_agg_result = self.replace_word(
+                    code_agg_result,
+                    code_by,
+                    (
+                        var_signature
+                        if by_is_single
+                        else f"{var_signature}[{index}]"
+                    ),
+                )
+
+            code_signature = (
+                code_signatures[0]
+                if by_is_single
+                else f"({', '.join(code_signatures)})"
+            )
+
+            if var_row in code_agg_result:
+                raise ConversionException(
+                    "something other than group_by keys and reducers have been used",
+                    code_agg_result,
+                )
+
+            with NamespaceCtx(
+                {
+                    self.SIGNATURE_NAME: var_signature,
+                    self.AGG_DATA_NAME: var_agg_data,
+                    self.AGG_RESULT_ITEM_NAME: code_agg_result,
+                },
+                ctx,
+            ):
+                code_final_result = (
+                    self.conversion.gen_code_and_update_ctx(None, ctx)
+                    if self.aggregate_mode
+                    else self.conversion.gen_code_and_update_ctx(
+                        f"{var_signature_to_agg_data}.items()", ctx
+                    )
+                )
+            agg_template_kwargs = {
+                "code_args": function_ctx.get_def_all_args_code(),
+                "code_result": f"    return {code_final_result}",
+                "var_row": var_row,
+            }
+
+            if self.aggregate_mode:
+                converter_name = f"aggregate{suffix}"
+                grouper_code = AGGREGATE_TEMPLATE.format(
+                    converter_name=converter_name,
+                    code_init_agg_vars=reduce_manager.gen_init_aggregate_vars(),
+                    code_aggregate=reduce_manager.gen_aggregate_code().to_string(
+                        base_indent_level=1,
+                    ),
+                    **agg_template_kwargs,
+                )
+            else:
+                converter_name = f"group_by{suffix}"
+                ctx[
+                    var_agg_data_cls
+                ] = reduce_manager.gen_group_by_data_container(
+                    self, var_agg_data_cls, ctx
+                )
+                grouper_code = GROUPER_TEMPLATE.format(
+                    converter_name=converter_name,
+                    var_signature_to_agg_data=var_signature_to_agg_data,
+                    var_agg_data_cls=var_agg_data_cls,
+                    var_agg_data=var_agg_data,
+                    code_signature=code_signature,
+                    code_group_by=reduce_manager.gen_group_by_code(
+                        var_signature_to_agg_data=var_signature_to_agg_data,
+                        code_signature=code_signature,
+                    ).to_string(base_indent_level=1),
+                    **agg_template_kwargs,
+                )
+
+            conversion = function_ctx.gen_conversion(
+                converter_name, grouper_code
+            )
+        return function_ctx.call_with_all_args(
+            conversion
+        ).gen_code_and_update_ctx(code_input, ctx)
+
+
+def Aggregate(  # pylint:disable=invalid-name
+    *args, **kwargs
+) -> BaseConversion:
+    """Shortcut for ``GroupBy().aggregate(*args, **kwargs)``"""
+    return GroupBy().aggregate(*args, **kwargs)
+
+
+class Reduce(BaseReducer):
+    """Defines the reduce operation, which is based on a callable / expression
+    to be used during the aggregation"""
+
+    internals_are_public = True
+
+    def __init__(
+        self,
+        to_call_with_2_args: t.Union[t.Callable, InlineExpr],
+        *expressions: t.Tuple[t.Any, ...],
+        initial: t.Union[_None, t.Callable, InlineExpr, t.Any],
+        default: t.Union[_None, t.Callable, t.Any] = _none,
+        unconditional_init: bool = False,
+        where=None,
+    ):
+        """
+        Args:
+          to_call_with_2_args: defines the reduce function/expression
+          expressions: args to be passed to `to_call_with_2_args` after the
+            aggregation value
+          initial: defines the very first item to be passed to
+            `to_call_with_2_args` item. If callable, then the result of a call
+            is used. If a conversion is passed, it is resolved on the first
+            row met.
+          default: defines the value to be returned when there was nothing to
+            reduce in a group (e.g. the current reduce operation has filtered
+            out some rows, while an adjacent reduce operation has got
+            something to reduce, forming a group). If callable, then the result
+            of a call is used.  When default is not passed, initial is used if
+            it doesn't depend on input data.
+          unconditional_init: tells whether the first call initializes the
+            aggregation value OR there is a condition for that
+        """
+        super().__init__(
+            *expressions, initial=initial, default=default, where=where
+        )
+
+        self.to_call_with_2_args = self.ensure_conversion(to_call_with_2_args)
+        if unconditional_init:
+            warnings.warn(
+                "unconditional_init is no longer needed", DeprecationWarning
+            )
+
+    def values_use_times(self, ctx):  # pylint: disable=unused-argument
+        return (1,) * len(self.expressions)
+
+    def works_with_not_none_only(self, ctx):  # pylint: disable=unused-argument
+        return (False,) * len(self.expressions)
+
+    def reduce_lines(self, ctx):
+        _ = self.to_call_with_2_args.call_like(
+            EscapedString("%(result)s"),
+            *self.expressions,
+        ).gen_code_and_update_ctx("%(row)s", ctx)
+        return (f"%(result)s = {_}",)
```

### Comparing `convtools-1.1.2/convtools/_base.py` & `convtools-1.2.0/convtools/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 import re
 import string
 import sys
 import typing as t
 from collections import deque
 from datetime import datetime
+from decimal import Decimal
 from itertools import chain
 from keyword import iskeyword
 from random import Random
 
 from ._dt import (
     DayOfWeekStep,
     MonthStep,
@@ -191,14 +192,15 @@
     self_content_type = ContentTypes.FUNCTION_OF_INPUT
 
     class OutputHints:
         NOT_NONE = 1
 
     output_hints = 0
     weight = Weights.UNPREDICTABLE
+    function_call_threshold = Weights.FUNCTION_CALL * 1.33
 
     base_type_to_cast: "t.Union[_None, t.Type]" = _none
 
     def __init__(self):
         self._depends_on = {}
         self.contents = self.self_content_type
         self.total_weight = self.weight
@@ -207,14 +209,20 @@
     def __hash__(self):
         return id(self)
 
     def add_hint(self, hint: int):
         self.output_hints |= hint
         return self
 
+    def has_hint(self, hint: int) -> int:
+        return self.output_hints & hint
+
+    def is_simple_for_n_uses(self, n):
+        return self.total_weight * (n - 1) < self.function_call_threshold
+
     def check_dependency(self, b):
         if (
             b.contents & 1 and self.self_content_type & 1
         ):  # self.ContentTypes.REDUCER
             raise ValueError("nested aggregation", self.__dict__)
 
     def is_dependency_trackable(self, dependency: "BaseConversion"):
@@ -230,16 +238,15 @@
 
             self.number_of_input_uses += arg.number_of_input_uses
             self.total_weight += arg.total_weight
             self.contents |= arg.contents
         return self
 
     def get_dependencies(self, types=None):
-        deps = self._depends_on.values()
-        deps = chain(deps, (self,))
+        deps: "t.Iterator[t.Any]" = chain(self._depends_on.values(), (self,))
         if types:
             deps = (dep for dep in deps if isinstance(dep, types))
         return deps
 
     def ensure_conversion(self, conversion, **kwargs) -> "BaseConversion":
         """Runs ensure_conversion on the input object and adds the resulting
         conversion to the list of dependencies"""
@@ -342,15 +349,15 @@
                 raise ValueError(
                     "non-resolved lazy escaped strings", non_resolved_lazy
                 )
 
         if len({dep_name for dep_name, _ in args}) != len(args):
             raise ValueError("duplicate args found", args)
 
-        name_to_code = {}
+        name_to_code: "t.Dict[str, str]" = {}
 
         positional_args_as_def_names = []
         positional_args_as_conversions = []
         keyword_args_as_def_names = []
         keyword_args_as_conversions = {}
 
         if "_none" not in args_to_skip and (
@@ -974,15 +981,15 @@
         `other_formats`, otherwise:
           - returns `default if provided
           - or raises ValueError
         """
         if other_formats or default is not _none:
             default = ensure_conversion(default)
             default_is_complex = not isinstance(default, NaiveConversion)
-            conversion = CallFunc(
+            conversion: "BaseConversion" = CallFunc(
                 date_parse,
                 self,
                 main_format,
                 NaiveConversion(other_formats),
                 None if default_is_complex else default,
             )
             if default_is_complex:
@@ -998,15 +1005,15 @@
         `other_formats`, otherwise:
           - returns `default if provided
           - or raises ValueError
         """
         if other_formats or default is not _none:
             default = ensure_conversion(default)
             default_is_complex = not isinstance(default, NaiveConversion)
-            conversion = CallFunc(
+            conversion: "BaseConversion" = CallFunc(
                 datetime_parse,
                 self,
                 main_format,
                 NaiveConversion(other_formats),
                 None if default_is_complex else default,
             )
             if default_is_complex:
@@ -1214,14 +1221,17 @@
     # Remove invalid characters
     s = _pattern_illegal_chars.sub("", s)
     # Remove leading characters until we find a letter or underscore
     s = _pattern_illegal_leading_chars.sub("", s)
     return s
 
 
+NOT_NONE_FUNCS = {sum, min, max, len, int, float, Decimal}
+
+
 class NaiveConversion(BaseConversion):
     """Naive conversion gets compiled into the code, which just returns the
     `value` it's been initialized with.  Allows to make any object available
     inside other conversions.
     """
 
     _builtin_dict = get_builtins_dict()
@@ -1289,14 +1299,23 @@
 
     def is_itself_callable_like(self) -> t.Optional[bool]:
         return callable(self.value)
 
     def is_itself_callable(self) -> t.Optional[bool]:
         return callable(self.value)
 
+    def call(self, *args, **kwargs) -> "Call":
+        conv = super().call(*args, **kwargs)
+        try:
+            if self.value in NOT_NONE_FUNCS:
+                conv.add_hint(BaseConversion.OutputHints.NOT_NONE)
+        except TypeError:
+            pass
+        return conv
+
     @staticmethod
     def get_value(conversion) -> bool:
         return (
             conversion.value
             if isinstance(conversion, NaiveConversion)
             else conversion
         )
@@ -1401,15 +1420,15 @@
         BaseConversion.self_content_type
         & ~BaseConversion.ContentTypes.FUNCTION_OF_INPUT
     )
 
     def __init__(
         self,
         conversion: "t.Any",
-        name_to_code: "t.Dict[str, t.Optional[t.Union[bool, str]]]",
+        name_to_code: "t.Dict[str, t.Union[bool, str, None]]",
     ):
         super().__init__()
         self.name_to_code = name_to_code
         self.conversion = self.ensure_conversion(conversion)
 
     def _gen_code_and_update_ctx(self, code_input, ctx):
         with NamespaceCtx(self.name_to_code, ctx):
@@ -1532,38 +1551,40 @@
 
     _name_to_code = None
     ctx = None
     active = False
 
     NAMESPACES = BaseConversion.NAMESPACES
 
-    def __init__(self, name_to_code: "t.Dict[str, str]", ctx):
+    def __init__(
+        self, name_to_code: "t.Mapping[str, t.Union[bool, str, None]]", ctx
+    ):
         name_to_code = {
             name: code for name, code in name_to_code.items() if code
         }
         if name_to_code:
             self._name_to_code = name_to_code
             self._ctx = ctx
 
     def __enter__(self):
         if self._name_to_code:
-            new_value: "t.Dict[str, str]" = {}
+            new_value: "t.MutableMapping[str, t.Union[bool, str, None]]" = {}
             new_value.update(self.name_to_code(self._ctx))
             new_value.update(self._name_to_code)
             self._ctx[self.NAMESPACES].append(new_value)
         self.active = True
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         if self._name_to_code:
             self._ctx[self.NAMESPACES].pop()
         self.active = False
 
     @classmethod
-    def name_to_code(cls, ctx) -> "t.Dict[str, str]":
+    def name_to_code(cls, ctx) -> "t.Mapping[str, str]":
         return ctx[cls.NAMESPACES][-1]
 
     def prevent_rendering_while_active(self, conversion):
         return NamespaceControlledUnit(self, conversion)
 
 
 class NamespaceControlledUnit(BaseConversion):
@@ -2275,15 +2296,15 @@
 
         self.generator_item = GeneratorItem.ensure_type(generator_item)
         self.depends_on(self.generator_item.item)
 
         for param in self.generator_item.custom_for_params:
             self.depends_on(param)
 
-        self.where = (
+        self.where: "t.Union[_None, BaseConversion]" = (
             _none
             if (where is None or where is _none)
             else self.ensure_conversion(where)
         )
         self.number_of_input_uses = 1
 
     def get_item_n_param_codes(self, ctx):
@@ -2310,15 +2331,15 @@
 class GeneratorComp(BaseComp):
     """Generates python generator comprehension code."""
 
     def _gen_code_and_update_ctx(self, code_input, ctx):
         item_code, param_code = self.get_item_n_param_codes(ctx)
         code_iterable = self.get_iterable_code(code_input, ctx)
 
-        if self.where is _none:
+        if isinstance(self.where, _None):
             return f"({item_code} for {param_code} in {code_iterable})"
 
         condition_code = self.where.gen_code_and_update_ctx(param_code, ctx)
         return f"({item_code} for {param_code} in {code_iterable} if {condition_code})"
 
     def to_iter(self):
         return self
@@ -2373,15 +2394,15 @@
 
     base_type_to_cast = set
 
     def _gen_code_and_update_ctx(self, code_input, ctx):
         item_code, param_code = self.get_item_n_param_codes(ctx)
         code_iterable = self.get_iterable_code(code_input, ctx)
 
-        if self.where is _none:
+        if isinstance(self.where, _None):
             return f"{{{item_code} for {param_code} in {code_iterable}}}"
 
         condition_code = self.where.gen_code_and_update_ctx(param_code, ctx)
         return f"{{{item_code} for {param_code} in {code_iterable} if {condition_code}}}"
 
     def as_type(self, callable_):
         if NaiveConversion.get_value(callable_) is set:
@@ -2394,15 +2415,15 @@
 
     base_type_to_cast = list
 
     def _gen_code_and_update_ctx(self, code_input, ctx):
         item_code, param_code = self.get_item_n_param_codes(ctx)
         code_iterable = self.get_iterable_code(code_input, ctx)
 
-        if self.where is _none:
+        if isinstance(self.where, _None):
             return f"[{item_code} for {param_code} in {code_iterable}]"
 
         condition_code = self.where.gen_code_and_update_ctx(param_code, ctx)
         return f"[{item_code} for {param_code} in {code_iterable} if {condition_code}]"
 
     def to_iter(self):
         return GeneratorComp(self.generator_item, self.where, self.self_conv)
@@ -2424,15 +2445,15 @@
 
     base_type_to_cast = tuple
 
     def _gen_code_and_update_ctx(self, code_input, ctx):
         item_code, param_code = self.get_item_n_param_codes(ctx)
         code_iterable = self.get_iterable_code(code_input, ctx)
 
-        if self.where is _none:
+        if isinstance(self.where, _None):
             return f"tuple({item_code} for {param_code} in {code_iterable})"
 
         condition_code = self.where.gen_code_and_update_ctx(param_code, ctx)
         return f"tuple({item_code} for {param_code} in {code_iterable} if {condition_code})"
 
     def to_iter(self):
         return GeneratorComp(self.generator_item, self.where, self.self_conv)
@@ -2459,27 +2480,31 @@
             used on each item of a collection to form keys
           value (object): to be wrapped with :py:obj:`ensure_conversion` and
             used on each item of a collection to form values
         """
         super().__init__(self_conv)
         self.key = self.ensure_conversion(key)
         self.value = self.ensure_conversion(value)
-        self.where = (
+        self.where: "t.Union[_None, BaseConversion]" = (
             _none
             if (where is None or where is _none)
             else self.ensure_conversion(where)
         )
         self.number_of_input_uses = 1
 
+    def get_iterable_code(self, code_input, ctx):
+        code_self, _ = self.get_self_and_input_code(code_input, ctx)
+        return code_self
+
     def _gen_code_and_update_ctx(self, code_input, ctx):
         param_code = self.gen_random_name("i", ctx)
         key_code = self.key.gen_code_and_update_ctx(param_code, ctx)
         value_code = self.value.gen_code_and_update_ctx(param_code, ctx)
-        code_iterable = BaseComp.get_iterable_code(self, code_input, ctx)
-        if self.where is _none:
+        code_iterable = self.get_iterable_code(code_input, ctx)
+        if isinstance(self.where, _None):
             return f"{{{key_code}: {value_code} for {param_code} in {code_iterable}}}"
 
         condition_code = self.where.gen_code_and_update_ctx(param_code, ctx)
         return f"{{{key_code}: {value_code} for {param_code} in {code_iterable} if {condition_code}}}"
 
     def filter(self, condition_conv, cast=BaseConversion._none):
         if cast is self._none:
@@ -2493,96 +2518,128 @@
 class BaseCollectionConversion(BaseConversion):
     """This is a base conversion of every collection"""
 
     self_content_type = (
         BaseConversion.self_content_type
         & ~BaseConversion.ContentTypes.FUNCTION_OF_INPUT
     )
+    conversions: t.Optional[t.List[BaseConversion]] = None
+    pairs: t.Optional[t.List[t.Tuple[BaseConversion, BaseConversion]]] = None
+    conditions: t.Optional[t.Mapping[int, BaseConversion]] = None
 
     def __init__(self, *items):
         """
         Args:
           items (objects): items to form a collection from.
             every item gets wrapped with :py:obj:`ensure_conversion`
         """
         super().__init__()
-        resulting_items = []
-        condition_to_item_pairs = None
+        self._init_from_items(items)
+
+    def _init_from_items(self, items):
+        conversions: "t.List[BaseConversion]" = []
+        conditions = None
+
         for item in items:
-            item = self.ensure_conversion(item)
-            if condition_to_item_pairs is None:
-                if isinstance(item, OptionalCollectionItem):
-                    condition_to_item_pairs = [
-                        (None, item_) for item_ in resulting_items
-                    ]
-                    condition_to_item_pairs.append(
-                        (item.condition, item.conversion)
-                    )
-                    resulting_items = None
-                else:
-                    resulting_items.append(item)
+            conv = self.ensure_conversion(item)
+            if isinstance(conv, OptionalCollectionItem):
+                if conditions is None:
+                    conditions = {}
+
+                conditions[len(conversions)] = conv.condition
+                conversions.append(conv.conversion)
             else:
-                condition_to_item_pairs.append(
-                    (item.condition, item.conversion)
-                    if isinstance(item, OptionalCollectionItem)
-                    else (None, item)
-                )
-        self.items = resulting_items
-        self.condition_to_item_pairs = condition_to_item_pairs
+                conversions.append(conv)
+
+        self.conversions = conversions
+        self.conditions = conditions
 
     def gen_optional_items_generator_code(self, code_input, ctx):
         inner_code_input = "data_"
         code = Code()
         converter_name = self.gen_random_name("optional_items_generator", ctx)
         function_ctx = self.as_function_ctx(ctx, optimize_naive=True)
         function_ctx.add_arg("data_", This())
         with function_ctx:
             code.add_line("def placeholder", 1)
 
-            for condition, item in self.condition_to_item_pairs:
-                value_code = ensure_conversion(item).gen_code_and_update_ctx(
-                    inner_code_input, ctx
-                )
-                if condition is not None:
-                    condition_code = condition.gen_code_and_update_ctx(
-                        inner_code_input, ctx
+            if self.conversions is not None:
+                conv_code_to_condition_code = [
+                    (
+                        conv.gen_code_and_update_ctx(inner_code_input, ctx),
+                        (
+                            self.conditions[index].gen_code_and_update_ctx(
+                                inner_code_input, ctx
+                            )
+                            if self.conditions and index in self.conditions
+                            else None
+                        ),
+                    )
+                    for index, conv in enumerate(self.conversions)
+                ]
+            elif self.pairs is not None:
+                conv_code_to_condition_code = [
+                    (
+                        (
+                            f"({key.gen_code_and_update_ctx(inner_code_input, ctx)}, "
+                            f"{value.gen_code_and_update_ctx(inner_code_input, ctx)})"
+                        ),
+                        (
+                            self.conditions[index].gen_code_and_update_ctx(
+                                inner_code_input, ctx
+                            )
+                            if self.conditions and index in self.conditions
+                            else None
+                        ),
                     )
+                    for index, (key, value) in enumerate(self.pairs)
+                ]
+
+            else:
+                raise AssertionError
+
+            for conv_code, condition_code in conv_code_to_condition_code:
+                if condition_code:
                     code.add_line(f"if {condition_code}:", 1)
-                    code.add_line(f"yield {value_code}", -1)
+                    code.add_line(f"yield {conv_code}", -1)
+
                 else:
-                    code.add_line(f"yield {value_code}", 0)
+                    code.add_line(f"yield {conv_code}", 0)
 
             code.lines_info[0] = (
                 0,
                 f"def {converter_name}({function_ctx.get_def_all_args_code()}):",
             )
 
             conversion = function_ctx.gen_conversion(
                 converter_name, code.to_string(base_indent_level=0)
             )
         return function_ctx.call_with_all_args(
             conversion
         ).gen_code_and_update_ctx(code_input, ctx)
 
     def gen_joined_items_code(self, code_input, ctx):
-        return ("," if len(self.items) < 3 else ",\n").join(
+        if self.conversions is None:
+            raise AssertionError
+
+        return ("," if len(self.conversions) < 3 else ",\n").join(
             item.gen_code_and_update_ctx(code_input, ctx)
-            for item in self.items
+            for item in self.conversions
         )
 
     def gen_collection_from_items_code(
         self, joined_items_code, code_input, ctx
     ):
         raise NotImplementedError
 
     def gen_collection_from_generator(self, generator_code, code_input, ctx):
         raise NotImplementedError
 
     def _gen_code_and_update_ctx(self, code_input, ctx):
-        if self.condition_to_item_pairs is not None:
+        if self.conditions is not None:
             return self.gen_collection_from_generator(
                 self.gen_optional_items_generator_code(code_input, ctx),
                 code_input,
                 ctx,
             )
 
         joined_items_code = self.gen_joined_items_code(code_input, ctx)
@@ -2593,14 +2650,17 @@
 
 class OptionalCollectionItem(BaseConversion):
     """Wrapping conversion which makes key/value/item of a collection
     optional."""
 
     valid_pipe_output = False
 
+    condition: BaseConversion
+    conversion: BaseConversion
+
     def __init__(
         self,
         conversion,
         skip_value=None,
         skip_if=BaseConversion._none,
         keep_if=BaseConversion._none,
     ):
@@ -2685,60 +2745,51 @@
 
 
 class Dict(BaseCollectionConversion):
     """Gets compiled into the code which generates a dict"""
 
     weight = Weights.DICT_INIT
 
-    def __init__(self, *key_value_pairs):
-        """
-        Args:
-          key_value_pairs (:obj:`list` of :obj:`tuple`): each tuple is a
-            key-value pair to form a dict from.
-            Every key and value gets wrapped with ``ensure_conversion``
-        """
-        super().__init__()
-        pairs = []
-        condition_to_item_pairs = None
-        for pair in key_value_pairs:
-            pair = tuple(self.ensure_conversion(item_) for item_ in pair)
-            conditions = [
-                item_.condition
-                for item_ in pair
-                if isinstance(item_, OptionalCollectionItem)
-            ]
-            condition = And(*conditions) if conditions else None
+    def _init_from_items(self, items):
+        pairs: "t.List[t.Tuple[BaseConversion, BaseConversion]]" = []
+        conditions = None
+
+        for key, value in items:
+            key = self.ensure_conversion(key)
+            value = self.ensure_conversion(value)
+            condition = None
+
+            if isinstance(key, OptionalCollectionItem):
+                condition = key.condition
+                key = key.conversion
+
+            if isinstance(value, OptionalCollectionItem):
+                if condition is None:
+                    condition = value.condition
+                else:
+                    condition = condition.and_(value.condition)
+                value = value.conversion
+
             if condition is not None:
-                pair = tuple(
-                    item_.conversion
-                    if isinstance(item_, OptionalCollectionItem)
-                    else item_
-                    for item_ in pair
-                )
+                if conditions is None:
+                    conditions = {}
+                conditions[len(pairs)] = condition
 
-            if condition_to_item_pairs is None:
-                if condition:
-                    condition_to_item_pairs = [
-                        (None, pair_) for pair_ in pairs
-                    ]
-                    pairs = None
-                    condition_to_item_pairs.append((condition, pair))
-                else:
-                    pairs.append(pair)
-            else:
-                condition_to_item_pairs.append((condition, pair))
+            pairs.append((key, value))
 
-        self.key_value_pairs = pairs
-        self.condition_to_item_pairs = condition_to_item_pairs
+        self.pairs = pairs
+        self.conditions = conditions
 
     def gen_joined_items_code(self, code_input, ctx):
-        return ("," if len(self.key_value_pairs) < 3 else ",\n").join(
+        if self.pairs is None:
+            raise AssertionError
+        return ("," if len(self.pairs) < 3 else ",\n").join(
             f"{key.gen_code_and_update_ctx(code_input, ctx)}:"
             f"{value.gen_code_and_update_ctx(code_input, ctx)}"
-            for key, value in self.key_value_pairs
+            for key, value in self.pairs
         )
 
     def gen_collection_from_generator(self, generator_code, code_input, ctx):
         return f"dict({generator_code})"
 
     def gen_collection_from_items_code(
         self, joined_items_code, code_input, ctx
@@ -2895,15 +2946,14 @@
     Supports predicate/sorting/type casting push down (each is directly applied
     to the ``where`` conversion.
 
     Supports labeling both pipe input and output data (allows to apply
     conversions before labeling)."""
 
     weight = 0
-    function_call_threshold = Weights.FUNCTION_CALL * 1.33
     self_content_type = (
         BaseConversion.self_content_type
     ) & ~BaseConversion.ContentTypes.FUNCTION_OF_INPUT
 
     def __init__(
         self,
         what,
@@ -2969,24 +3019,24 @@
             if label_output is None
             else self._prepare_labels(self.input_args_container, label_output)
         )
         input_has_no_side_effects = (
             what.contents & 4 == 0  # self.ContentTypes.NEW_LABEL
             and self.label_input is None
         )
+
         self.to_be_inlined = (
             # can be inlined
             (
                 (
                     # if "where" uses an input multiple times, we should weigh
                     # wrapping it into a function and so the input is calculated
                     # only once (of course taking into account function call
                     # overhead)
-                    what.total_weight * (where.number_of_input_uses - 1)
-                    < self.function_call_threshold
+                    what.is_simple_for_n_uses(where.number_of_input_uses)
                 )
                 and self.label_output is None
                 and input_has_no_side_effects
             )
             # must be inlined - self.ContentTypes.REDUCER
             or where.contents & 1
         )
@@ -3018,14 +3068,19 @@
             label_input=self.label_input,
             label_output=self.label_output,
         )
 
     def __hash__(self):
         return id(self)
 
+    def has_hint(self, hint: int) -> int:
+        if self.where is This:
+            return self.what.has_hint(hint)
+        return self.where.has_hint(hint)
+
     __add__ = delegate_simple_1_arg("__add__")
     add = delegate_simple_1_arg("add")
     __and__ = delegate_simple_1_arg("__and__")
     __eq__ = delegate_simple_1_arg("__eq__")
     __floordiv__ = delegate_simple_1_arg("__floordiv__")
     floor_div = delegate_simple_1_arg("floor_div")
     __ge__ = delegate_simple_1_arg("__ge__")
```

### Comparing `convtools-1.1.2/convtools/_chunks.py` & `convtools-1.2.0/convtools/_chunks.py`

 * *Files identical despite different names*

### Comparing `convtools-1.1.2/convtools/_columns.py` & `convtools-1.2.0/convtools/_columns.py`

 * *Files identical despite different names*

### Comparing `convtools-1.1.2/convtools/_conversion.py` & `convtools-1.2.0/convtools/_conversion.py`

 * *Files identical despite different names*

### Comparing `convtools-1.1.2/convtools/_cumulative.py` & `convtools-1.2.0/convtools/_cumulative.py`

 * *Files identical despite different names*

### Comparing `convtools-1.1.2/convtools/_debug.py` & `convtools-1.2.0/convtools/_debug.py`

 * *Files identical despite different names*

### Comparing `convtools-1.1.2/convtools/_dt.py` & `convtools-1.2.0/convtools/_dt.py`

 * *Files identical despite different names*

### Comparing `convtools-1.1.2/convtools/_heuristics.py` & `convtools-1.2.0/convtools/_heuristics.py`

 * *Files identical despite different names*

### Comparing `convtools-1.1.2/convtools/_joins.py` & `convtools-1.2.0/convtools/_joins.py`

 * *Files identical despite different names*

### Comparing `convtools-1.1.2/convtools/_mutations.py` & `convtools-1.2.0/convtools/_mutations.py`

 * *Files identical despite different names*

### Comparing `convtools-1.1.2/convtools/_unique.py` & `convtools-1.2.0/convtools/_unique.py`

 * *Files identical despite different names*

### Comparing `convtools-1.1.2/convtools/_utils.py` & `convtools-1.2.0/convtools/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
             if not k.startswith("_") and k not in {"clone", "to_defaults"}
         }
 
 
 class BaseOptions(object, metaclass=BaseOptionsMeta):
     """Container object, which carries current options"""
 
+    _option_attrs: dict
+
     def clone(self):
         clone = self.__class__()
         for option_attr in self._option_attrs.keys():
             setattr(clone, option_attr, getattr(self, option_attr))
         return clone
 
     def to_defaults(self, option_name=None):
@@ -121,16 +123,20 @@
     def add_code(self, code: "Code"):
         for indent_level, line in code.lines_info:
             self.lines_info.append((indent_level + self.indent_level, line))
 
     def incr_indent_level(self, incr: int):
         self.indent_level += incr
 
-    def has_lines(self):
-        return bool(self.lines_info)
+    def get_ref(self):
+        return len(self.lines_info), self.indent_level
+
+    def cut_to_ref(self, ref):
+        new_len, self.indent_level = ref
+        self.lines_info[new_len:] = ()
 
     def to_string(self, base_indent_level: int, single_indent: str = "    "):
         return "\n".join(
             f"{single_indent * (base_indent_level + indent_level)}{line}"
             for indent_level, line in self.lines_info
         )
 
@@ -139,24 +145,24 @@
     """Lazy instance to hold and initialize debug directory for generated code
     sources"""
 
     def __init__(self):
         self.debug_dir = None
         self.dir_initialized = False
 
-    def get(self):
+    def get(self) -> str:
         if self.debug_dir is None:
             self.debug_dir = os.environ.get(
                 "PY_CONVTOOLS_DEBUG_DIR", None
             ) or os.path.join(tempfile.gettempdir(), "py_convtools_debug")
         return self.debug_dir
 
     def ensure_initialized(self):
         if not self.dir_initialized:
-            os.makedirs(self.debug_dir, exist_ok=True)
+            os.makedirs(self.get(), exist_ok=True)
             self.dir_initialized = True
 
 
 debug_dir = LazyDebugDir()
 
 
 class CodePiece:
@@ -177,15 +183,15 @@
 
 
 class CodeStorage:
     """Container which stores generated code pieces. It allows to dump code
     sources on disk into a debug directory."""
 
     def __init__(self):
-        self.key_to_code_piece = {}
+        self.key_to_code_piece: "t.Dict[str, CodePiece]" = {}
         self.converter_names = set()
         finalize(self, drop_dumped_code, self.key_to_code_piece)
 
     def add_sources(self, converter_name, code_str):
         def_name = f"def {converter_name}("
         code_parts = (def_name, code_str.replace(def_name, ""))
 
@@ -222,16 +228,21 @@
         if code_piece.is_dumped:
             try:
                 os.remove(code_piece.abs_path)
             except FileNotFoundError:  # pragma: no cover
                 pass
 
 
-def iter_windows(collection, width, step):
-    window = deque(maxlen=width)
+T = t.TypeVar("T")
+
+
+def iter_windows(
+    collection: t.Iterator[T], width, step
+) -> t.Generator[t.Tuple[T, ...], None, None]:
+    window: "deque[T]" = deque(maxlen=width)
     window_append = window.append
 
     index = 0
     for index, obj in enumerate(collection):
         window_append(obj)
         if index % step == 0:
             yield tuple(window)
```

### Comparing `convtools-1.1.2/convtools/contrib/fs.py` & `convtools-1.2.0/convtools/contrib/fs.py`

 * *Files identical despite different names*

### Comparing `convtools-1.1.2/convtools/contrib/tables.py` & `convtools-1.2.0/convtools/contrib/tables.py`

 * *Files identical despite different names*

### Comparing `convtools-1.1.2/.gitignore` & `convtools-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `convtools-1.1.2/LICENSE.txt` & `convtools-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `convtools-1.1.2/README.md` & `convtools-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `convtools-1.1.2/pyproject.toml` & `convtools-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.hatch.build.targets.sdist]
 include = ["/src"]
 
 
 [project]
 name = "convtools"
-version = "1.1.2"
+version = "1.2.0"
 description = "dynamic, declarative data transformations with automatic code generation"
 
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE.txt"}
 keywords = ["etl", "converters", "codegen", "convtools"]
 authors = [
```

### Comparing `convtools-1.1.2/PKG-INFO` & `convtools-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convtools
-Version: 1.1.2
+Version: 1.2.0
 Summary: dynamic, declarative data transformations with automatic code generation
 Project-URL: homepage, https://github.com/westandskif/convtools
 Project-URL: documentation, https://convtools.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/westandskif/convtools
 Project-URL: changelog, https://github.com/westandskif/convtools/blob/master/docs/CHANGELOG.md
 Author-email: Nikita Almakov <nikita.almakov@gmail.com>
 Maintainer-email: Nikita Almakov <nikita.almakov@gmail.com>
```

