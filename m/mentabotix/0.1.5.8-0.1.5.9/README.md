# Comparing `tmp/mentabotix-0.1.5.8.tar.gz` & `tmp/mentabotix-0.1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentabotix-0.1.5.8.tar", last modified: Mon May 27 12:07:42 2024, max compression
+gzip compressed data, was "mentabotix-0.1.5.9.tar", last modified: Tue May 28 09:12:02 2024, max compression
```

## Comparing `mentabotix-0.1.5.8.tar` & `mentabotix-0.1.5.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1066 2024-05-27 12:07:18.378980 mentabotix-0.1.5.8/LICENSE
--rw-r--r--   0        0        0    23799 2024-05-27 12:07:18.378980 mentabotix-0.1.5.8/README.md
--rw-r--r--   0        0        0      613 2024-05-27 12:07:42.530809 mentabotix-0.1.5.8/pyproject.toml
--rw-r--r--   0        0        0     1301 2024-05-27 12:07:18.378980 mentabotix-0.1.5.8/src/mentabotix/__init__.py
--rw-r--r--   0        0        0    79930 2024-05-27 12:07:18.378980 mentabotix-0.1.5.8/src/mentabotix/modules/botix.py
--rw-r--r--   0        0        0      225 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/src/mentabotix/modules/exceptions.py
--rw-r--r--   0        0        0      580 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/src/mentabotix/modules/logger.py
--rw-r--r--   0        0        0    21088 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/src/mentabotix/modules/menta.py
--rw-r--r--   0        0        0    20857 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/src/mentabotix/tools/composers.py
--rw-r--r--   0        0        0     2292 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/src/mentabotix/tools/generators.py
--rw-r--r--   0        0        0      867 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/src/mentabotix/tools/selectors.py
--rw-r--r--   0        0        0        0 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/tests/__init__.py
--rw-r--r--   0        0        0      682 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/tests/find_tests.py
--rw-r--r--   0        0        0    15660 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/tests/test_botix.py
--rw-r--r--   0        0        0     2521 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/tests/test_case_registry.py
--rw-r--r--   0        0        0    11493 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/tests/test_composer.py
--rw-r--r--   0        0        0     8998 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/tests/test_menta.py
--rw-r--r--   0        0        0    11921 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/tests/test_moving_state.py
--rw-r--r--   0        0        0     7475 2024-05-27 12:07:18.382979 mentabotix-0.1.5.8/tests/test_moving_transition.py
--rw-r--r--   0        0        0    24152 1970-01-01 00:00:00.000000 mentabotix-0.1.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-28 09:11:38.894070 mentabotix-0.1.5.9/LICENSE
+-rw-r--r--   0        0        0    23799 2024-05-28 09:11:38.894070 mentabotix-0.1.5.9/README.md
+-rw-r--r--   0        0        0      638 2024-05-28 09:12:02.486110 mentabotix-0.1.5.9/pyproject.toml
+-rw-r--r--   0        0        0     1353 2024-05-28 09:11:38.894070 mentabotix-0.1.5.9/src/mentabotix/__init__.py
+-rw-r--r--   0        0        0    82858 2024-05-28 09:11:38.894070 mentabotix-0.1.5.9/src/mentabotix/modules/botix.py
+-rw-r--r--   0        0        0      225 2024-05-28 09:11:38.894070 mentabotix-0.1.5.9/src/mentabotix/modules/exceptions.py
+-rw-r--r--   0        0        0      580 2024-05-28 09:11:38.894070 mentabotix-0.1.5.9/src/mentabotix/modules/logger.py
+-rw-r--r--   0        0        0    21088 2024-05-28 09:11:38.894070 mentabotix-0.1.5.9/src/mentabotix/modules/menta.py
+-rw-r--r--   0        0        0    21433 2024-05-28 09:11:38.898070 mentabotix-0.1.5.9/src/mentabotix/tools/composers.py
+-rw-r--r--   0        0        0     2292 2024-05-28 09:11:38.898070 mentabotix-0.1.5.9/src/mentabotix/tools/generators.py
+-rw-r--r--   0        0        0      867 2024-05-28 09:11:38.898070 mentabotix-0.1.5.9/src/mentabotix/tools/selectors.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:11:38.898070 mentabotix-0.1.5.9/tests/__init__.py
+-rw-r--r--   0        0        0      682 2024-05-28 09:11:38.898070 mentabotix-0.1.5.9/tests/find_tests.py
+-rw-r--r--   0        0        0    19137 2024-05-28 09:11:38.898070 mentabotix-0.1.5.9/tests/test_botix.py
+-rw-r--r--   0        0        0     2521 2024-05-28 09:11:38.898070 mentabotix-0.1.5.9/tests/test_case_registry.py
+-rw-r--r--   0        0        0    13392 2024-05-28 09:11:38.898070 mentabotix-0.1.5.9/tests/test_composer.py
+-rw-r--r--   0        0        0     8998 2024-05-28 09:11:38.898070 mentabotix-0.1.5.9/tests/test_menta.py
+-rw-r--r--   0        0        0    11921 2024-05-28 09:11:38.898070 mentabotix-0.1.5.9/tests/test_moving_state.py
+-rw-r--r--   0        0        0     7475 2024-05-28 09:11:38.898070 mentabotix-0.1.5.9/tests/test_moving_transition.py
+-rw-r--r--   0        0        0    24185 1970-01-01 00:00:00.000000 mentabotix-0.1.5.9/PKG-INFO
```

### Comparing `mentabotix-0.1.5.8/LICENSE` & `mentabotix-0.1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.8/README.md` & `mentabotix-0.1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.8/pyproject.toml` & `mentabotix-0.1.5.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [project]
 name = "mentabotix"
-version = "0.1.5.8"
+version = "0.1.5.9"
 description = "A Bot control lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "numpy>=1.26.4",
     "terminaltables>=3.1.10",
     "bdmc>=0.1.5.10",
+    "pyuptech>=0.1.6.4",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `mentabotix-0.1.5.8/src/mentabotix/__init__.py` & `mentabotix-0.1.5.9/src/mentabotix/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-from .modules.botix import MovingState, MovingTransition, Botix
+from .modules.botix import MovingState, MovingTransition, Botix, ArrowStyle
 from .modules.exceptions import BadSignatureError, RequirementError, SamplerTypeError, TokenizeError, StructuralError
 from .modules.logger import set_log_level
 from .modules.menta import Menta, SequenceSampler, IndexedSampler, DirectSampler, SamplerUsage, SamplerType, Sampler
 
 from .tools.composers import (
     MovingChainComposer,
     CaseRegistry,
     straight_chain,
     snaking_chain,
     scanning_chain,
     random_lr_turn_branch,
+    copy,
 )
 from .tools.generators import NameGenerator, Multipliers, make_multiplier_generator
 from .tools.selectors import make_weighted_selector
 
 __all__ = [
     "set_log_level",
     # botix
     "MovingState",
     "MovingTransition",
     "Botix",
+    "ArrowStyle",
     # menta
     "Menta",
     "SequenceSampler",
     "IndexedSampler",
     "DirectSampler",
     "SamplerUsage",
     "SamplerType",
@@ -37,13 +39,14 @@
     # tools/composers
     "MovingChainComposer",
     "CaseRegistry",
     "straight_chain",
     "snaking_chain",
     "scanning_chain",
     "random_lr_turn_branch",
+    "copy",
     # tools/generators
     "NameGenerator",
     "Multipliers",
     # tools/selectors
     "make_weighted_selector",
 ]
```

### Comparing `mentabotix-0.1.5.8/src/mentabotix/modules/botix.py` & `mentabotix-0.1.5.9/src/mentabotix/modules/botix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 from collections import Counter
 from dataclasses import dataclass
-from enum import Enum
-from itertools import zip_longest
+from enum import Enum, StrEnum
+from itertools import zip_longest, chain
 from queue import Queue
 from random import random
 from typing import (
     Tuple,
     TypeAlias,
     Self,
     Unpack,
@@ -57,14 +57,29 @@
     """
 
     Full = 1
     LR = 2
     Individual = 4
 
 
+class ArrowStyle(StrEnum):
+    """
+    Attributes:
+        DOWN: "-->"
+        LEFT: "-left->"
+        RIGHT: "-right->"
+        UP: "-up->"
+    """
+
+    DOWN = "-->"
+    LEFT = "-left->"
+    RIGHT = "-right->"
+    UP = "-up->"
+
+
 def get_function_annotations(func: Callable) -> str:
     """
     Get the function annotations of a given function.
 
     Args:
         func (callable): The function to get the annotations for.
 
@@ -97,36 +112,49 @@
             param_types.append("Any")
 
     # Handle the return type
     return_type = convert_type_str(type_hints.get("return", Any))
 
     # Concatenate the parameter type strings and return type to form the annotation string
     params_str = ", ".join(param_types)
-    return f"{func.__name__}({params_str}) -> {return_type}"
+    return f"def {func.__name__}({params_str}) -> {return_type}"
 
 
 def convert_type_str(hint) -> str:
     """
     Convert a type hint to a string representation, handling complex types and generics.
 
     Args:
         hint: The type hint to convert.
 
     Returns:
         str: The string representation of the type hint.
     """
-    if hint is None:
+    if hint == type(None):
         return "None"
     elif hint in {int, float, bool, str, list, tuple, set, dict}:
         return hint.__name__
     else:
         # For other types, convert directly to string
         return str(hint).replace("typing.", "")
 
 
+def bold(string: str) -> str:
+    """
+    Takes a string as input and returns the same string surrounded by double asterisks.
+
+    Parameters:
+        string (str): The string to be formatted.
+
+    Returns:
+        str: The input string surrounded by double asterisks.
+    """
+    return f"**{string}**"
+
+
 class MovingState:
     """
     Describes the movement state of the bot.
     Include:
     - halt: make a stop state,all wheels stop moving
     - straight: make a straight moving state,all wheels move in the same direction,same speed
     - turn: make a turning state,left and right wheels turn in different direction,same speed
@@ -1590,83 +1618,140 @@
                 return lines
             case _:
                 compiled_lines.append(line)
                 # If no forward transition is present, return the compiled lines
                 return compiled_lines
 
     @classmethod
-    def export_structure(cls, save_path: str, transitions: TokenPool) -> Self:
+    def export_structure(
+        cls,
+        save_path: str,
+        transitions: TokenPool,
+        arrow_style: ArrowStyle | Literal["up", "down", "left", "right"] | str = "down",
+    ) -> Self:
         """
         Export the structure to a UML file based on the provided transitions.
 
         Args:
             save_path (str): The path to save the UML file.
             transitions (Optional[List[MovingTransition]]): The list of transitions to represent in the UML.
-
+            arrow_style (Optional[ArrowStyle]): The style of the arrows to use in the UML. Defaults to "down".
         Returns:
             Self: The current instance.
         """
+        undefined_to_state = "UNDEFINED_TO_STATE"
+        undefined_from_state = "UNDEFINED_FROM_STATE"
+        if isinstance(arrow_style, ArrowStyle):
+            arrow = arrow_style
+        else:
+            upper = arrow_style.upper()
+            matched = list(filter(lambda x: x.name == upper, ArrowStyle))
+            if matched:
+                arrow = matched[0]
+            else:
+                raise ValueError(f"Must be one of {list(ArrowStyle)}, but got unknown arrow style: {arrow_style}")
+
         start_string = "@startuml\n"
         end_string = "@enduml\n"
 
-        used_state: Dict[MovingState, str] = {}
-
+        states_alias_mapping: Dict[MovingState, str] = {}  # type: ignore
+        state_name_gen: NameGenerator = NameGenerator(basename="state_")
+        all_states: Set[MovingState] = set(
+            chain(*[transition.from_states + list(transition.to_states.values()) for transition in transitions])
+        )
         lines: List[str] = []
-        name_gen: NameGenerator = NameGenerator(basename="state_")
+        if no_from := list(filter(lambda x: not x.from_states, transitions)):
+
+            states_alias_mapping[undefined_from_state] = undefined_from_state  # type: ignore
+            for t in no_from:
+                t: MovingTransition
+                t.from_states.append(undefined_from_state)  # type: ignore
+        for state in all_states:
+            cls._inject_state_meta_info(lines, state, state_name_gen, states_alias_mapping)
+
         break_gen: NameGenerator = NameGenerator(basename="break_")
         for transition in transitions:
+
             for from_state in transition.from_states:
 
-                if from_state in used_state:
-                    from_state_alias = used_state.get(from_state)
-                else:
-                    from_state_alias: str = name_gen()
-                    used_state[from_state] = from_state_alias
-                    lines.insert(0, f'state "{from_state}" as {from_state_alias}\n')
-
-                if len(transition.to_states) == 1:
-                    to_state = list(transition.to_states.values())[0]
-                    if to_state not in used_state:
-                        to_state_alias: str = name_gen()
-                        used_state[to_state] = to_state_alias
-                        lines.insert(0, f'state "{to_state}" as {to_state_alias}\n')
-                    else:
-                        to_state_alias = used_state.get(to_state)
-                    lines.append(f"{from_state_alias} --> {to_state_alias}\n")
-                else:
-                    if not callable(transition.breaker):
-                        raise ValueError("The break function must be callable. Since branch must need a valid breaker.")
-                    break_node_name: str = break_gen()
-                    lines.insert(0, f"state {break_node_name} <<choice>>\n")
-                    lines.insert(
-                        1, f"note right of {break_node_name}: {get_function_annotations(transition.breaker)}\n"
-                    )
-                    lines.append(f"{from_state_alias} --> {break_node_name}\n")
-                    for case_name, to_state in transition.to_states.items():
+                match len(transition.to_states):
+                    case 0:
+                        lines.append(f"{states_alias_mapping.get(from_state)} {arrow} {undefined_to_state}\n")
+                        lines.append(f"note on link\nThis transition does not define a to_states\nend note\n")
+                    case 1:
+                        to_state = list(transition.to_states.values())[0]
 
-                        if to_state not in used_state:
-                            to_state_alias: str = name_gen()
-                            used_state[to_state] = to_state_alias
-                            lines.insert(0, f'state "{to_state}" as {to_state_alias}\n')
-                        else:
-                            to_state_alias = used_state.get(to_state)
+                        lines.append(
+                            f"{states_alias_mapping.get(from_state)} {arrow} {states_alias_mapping.get(to_state)}\n"
+                        )
+                    case _:
+                        if not callable(transition.breaker):
+                            raise ValueError(
+                                "The break function must be callable. Since branch must need a valid breaker."
+                            )
+                        break_node_name: str = break_gen()
 
-                        lines.append(f"{break_node_name} --> {to_state_alias}: {case_name}\n")
+                        lines.insert(0, f"state {break_node_name} <<choice>>\n")
+                        lines.insert(
+                            1, f"note right of {break_node_name}: {get_function_annotations(transition.breaker)}\n"
+                        )
+                        lines.append(f"{states_alias_mapping.get(from_state)} {arrow} {break_node_name}\n")
+                        for case_name, to_state in transition.to_states.items():
 
+                            lines.append(
+                                f"{break_node_name} {arrow} {states_alias_mapping.get(to_state)}: {case_name}\n"
+                            )
+
+        if no_from:
+            for t in no_from:
+                t: MovingTransition
+                t.from_states.remove(undefined_from_state)  # type: ignore
         start_states: Set[MovingState] = Botix.acquire_start_states(token_pool=transitions)
         end_states: Set[MovingState] = Botix.acquire_end_states(token_pool=transitions)
 
-        start_heads: List[str] = [f"[*] --> {used_state.get(sta)}\n" for sta in start_states]
-        end_heads: List[str] = [f"{used_state.get(sta)} --> [*]\n" for sta in end_states]
+        start_heads: List[str] = [f"[*] {arrow} {states_alias_mapping.get(sta)}\n" for sta in start_states]
+        end_heads: List[str] = [f"{states_alias_mapping.get(sta)} {arrow} [*]\n" for sta in end_states]
 
         with open(save_path, "w") as f:
 
             f.writelines([start_string, *lines, "\n", *start_heads, "\n", *end_heads, "\n", end_string])
         return cls
 
+    @classmethod
+    def _inject_state_meta_info(
+        cls,
+        lines: List[str],
+        state: MovingState,
+        state_name_gen: NameGenerator,
+        states_alias_mapping: Dict[MovingState, str],
+    ):
+        states_alias_mapping[state] = (state_alias := state_name_gen())
+        state_name = f"{state.state_id}-MovingState"
+        lines.insert(0, f'state "{state_name}" as {state_alias}\n')
+        state_cmds_expr = bold((string := str(state))[string.index("(") :])
+        before_entering_desc = (
+            f"{bold('Before:')}\\n"
+            + "\\n".join(f"##{get_function_annotations(fun)}" for fun in state.before_entering)
+            + "\\n"
+            if state.before_entering
+            else ""
+        )
+        after_entering_desc = (
+            f"{bold('After:')}\\n"
+            + "\\n".join(f"##{get_function_annotations(fun)}" for fun in state.after_exiting)
+            + "\\n"
+            if state.after_exiting
+            else ""
+        )
+        if before_entering_desc or after_entering_desc:
+            description = f"{state_cmds_expr}\\n====\\n{before_entering_desc}{after_entering_desc}"
+        else:
+            description = state_cmds_expr
+        lines.insert(1, f"{state_alias}: {description}\n")
+
     def compile(self, return_median: bool = False) -> Callable[[], None] | Tuple[List[str], Context]:
         """
         Compiles the bot's code and returns a callable function or a tuple of compiled lines and context.
 
         Args:
             return_median (bool, optional): Whether to return the compiled lines and context instead of a callable function. Defaults to False.
```

### Comparing `mentabotix-0.1.5.8/src/mentabotix/modules/logger.py` & `mentabotix-0.1.5.9/src/mentabotix/modules/logger.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.8/src/mentabotix/modules/menta.py` & `mentabotix-0.1.5.9/src/mentabotix/modules/menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.8/src/mentabotix/tools/composers.py` & `mentabotix-0.1.5.9/src/mentabotix/tools/composers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from enum import Enum
-from typing import List, Tuple, Callable, Optional, Self, Type, TypeVar, Dict, Hashable
+from itertools import zip_longest
+from typing import List, Tuple, Callable, Optional, Self, Type, TypeVar, Dict, Hashable, Iterable
 
 from numpy.random import random
 
 from ..modules.botix import MovingState, MovingTransition, __PLACE_HOLDER__
 
 StateTransitionPack = Tuple[List[MovingState], List[MovingTransition]]
 
 UnitType = TypeVar("UnitType", Type[MovingState], Type[MovingTransition])
+SupportClone = TypeVar("SupportClone", MovingState, MovingTransition)
 from terminaltables import SingleTable
 
 
 class MovingChainComposer:
     """
     A class that manages the composition of moving states and transitions.
 
@@ -99,132 +101,143 @@
 
         Raises:
             ValueError: If the type of the unit does not match the next need.
             RuntimeError: If the type of the unit is neither `MovingState` nor `MovingTransition`.
         """
         unit_type = type(unit)
         if unit_type != self.next_need:
-            raise ValueError(f"Need {self.next_need}, got {unit}!")
+            raise ValueError(f"Need {self.next_need}, got {type(unit)}, which is {repr(unit)}!")
         elif unit_type == MovingState:
             self._chain_container[MovingState].append(unit)
-            if self.last_transition:
+            if self.last_transition and unit not in self.last_transition.to_states.values():
                 self.last_transition.to_states[register_case] = unit
         elif unit_type == MovingTransition:
             unit.from_states.append(self.last_state) if self.last_state not in unit.from_states else None
             self._chain_container[MovingTransition].append(unit)
         else:
             raise RuntimeError("Should never reach here!")
         self._flip()
         return self
 
-    def concat(self, states: List[MovingState], transitions: List[MovingTransition]) -> Self:
+    def concat(
+        self,
+        states: List[MovingState],
+        transitions: List[MovingTransition],
+        register_case: Optional[Hashable] = __PLACE_HOLDER__,
+    ) -> Self:
         """
         Concatenates the given list of states and transitions into the current data structure.
 
         Args:
             states: A list of MovingState objects representing the states to concatenate.
             transitions: A list of MovingTransition objects representing the transitions to concatenate.
-
+            register_case (Optional[Hashable]): The case to register the state or transition with.
         Returns:
             Returns the concatenated data structure itself.
 
         Raises:
             ValueError if no states or transitions are provided.
             ValueError if the initial condition of the transition's starting state doesn't match the expectation.
             ValueError if the number of states and transitions don't match by no more than 1.
 
         This function checks the validity of the input and connects the states and transitions accordingly.
         It handles different scenarios based on whether there's an initial state and the difference between the lengths of states and transitions.
-        """
-
+        """  # FIXME
+        state_len, trans_len = len(states), len(transitions)
         # Check if at least one state and one transition are provided
         if not (states or transitions):
             raise ValueError("Need at least one state and one transition!")
+        elif not abs(state_len - trans_len) <= 1:
+            raise ValueError(
+                f"The number of states and transitions don't match by no more than 1! "
+                f"Got {state_len} states and {trans_len} transitions!"
+            )
 
         # Initialize the head transition and check if it has a starting state
         head_transition = transitions[0]
-        has_start_state = len(head_transition.from_states) == 1
+        has_start_state = bool(head_transition.from_states)
         head_state = states[0]
 
         # Validate the expected next element type (state or transition) based on the initial condition
         if self.next_need == MovingTransition and has_start_state:
-            raise ValueError(f"Need {self.next_need}, got {head_transition.from_states[0]}!")
+            raise ValueError(f"Need {MovingTransition}, but got {head_state}!")
         elif self.next_need == MovingState and not has_start_state:
-            raise ValueError(f"Need {self.next_need}, got {head_transition.to_states}!")
-        elif self.next_need == MovingState and head_transition.from_states[0] != head_state:
-            raise ValueError(f"The transition {head_transition} should only start from {head_state}!")
+            raise ValueError(f"Need {MovingState}, but the head of the seq is {repr(head_transition)}!")
+        elif self.next_need == MovingState and head_state not in head_transition.from_states:
+            raise ValueError(f"The transition {repr(head_transition)} should only start from {head_state}!")
 
         # Reset the states and transitions lists for concatenation
-        states: List[MovingState]
-        transitions: List[MovingTransition]
+        states: List[MovingState] = list(states)
+        transitions: List[MovingTransition] = list(transitions)
+
+        if has_start_state:
 
-        # Connect the states and transitions based on the presence of an initial state and their lengths
-        match has_start_state, len(states), len(transitions):
-            case True, sta_len, tran_len if sta_len == tran_len:
-                # If there's an initial state and the lengths match, connect them normally
-                if self.last_transition:
-                    self.last_transition.to_states[__PLACE_HOLDER__] = head_state
-
-                for sta, tran in zip(states, transitions):
-                    # Ensure each state is in the corresponding transition's from_states
-                    if sta not in tran.from_states:
-                        raise ValueError(f"The state {sta} should be in the from_states of the transition {tran}!")
-                    self._chain_container[MovingState].append(sta)
-                    self._chain_container[MovingTransition].append(tran)
-
-            case False, sta_len, tran_len if sta_len == tran_len:
-                # If there's no initial state and the lengths match, connect them differently
-                if self.last_state:
-                    head_transition.from_states.append(self.last_state)
-
-                for sta, tran in zip(states, transitions):
-                    # Ensure each state is in the corresponding transition's to_states
-                    if sta not in tran.to_states.values():
-                        raise ValueError(f"The state {sta} should be in the to_states of the transition {tran}!")
-                    self._chain_container[MovingState].append(sta)
-                    self._chain_container[MovingTransition].append(tran)
-
-            case True, sta_len, tran_len if sta_len - tran_len == 1:
-                # If there's an extra state
-                excessive_state = states.pop(0)
-                if self.last_transition:
-                    self.last_transition.to_states[__PLACE_HOLDER__] = excessive_state
-
-                self._chain_container[MovingState].append(excessive_state)
-                for sta, tran in zip(states, transitions):
-                    # Ensure each state is in the corresponding transition's to_states
-                    if sta not in tran.to_states.values():
-                        raise ValueError(f"The state {sta} should be in the to_states of the transition {tran}!")
-
-                    self._chain_container[MovingState].append(sta)
-                    self._chain_container[MovingTransition].append(tran)
-                self._flip()  # Flip the internal representation to accommodate the new connection
-
-            case False, sta_len, tran_len if sta_len - tran_len == -1:
-                # If there's an extra transition
-                excessive_transition = transitions.pop(0)
-                excessive_transition.from_states.append(self.last_state)
-                self._chain_container[MovingTransition].append(excessive_transition)
-                for sta, tran in zip(states, transitions):
-                    # Ensure each state is in the corresponding transition's from_states
-                    if sta not in tran.from_states:
-                        raise ValueError(f"The state {sta} should be in the from_states of the transition {tran}!")
-                    self._chain_container[MovingState].append(sta)
-                    self._chain_container[MovingTransition].append(tran)
-                self._flip()  # Flip the internal representation to accommodate the new connection
+            start_state = states.pop(0)
+            self.add(start_state, register_case)
+
+        for sta, trans in zip_longest(states, transitions):
+            self._add_with_connection_check(trans) if trans else None
+            self._add_with_connection_check(sta) if sta else None
+        return self
+
+    def _add_with_connection_check(self, unit: MovingState | MovingTransition) -> Self:
+        """
+        Adds a `MovingState` or `MovingTransition` object to the chain container.
 
-            case _, _, _:
-                # If the lengths differ by more than 1, the data pack is invalid
+        Args:
+            unit (MovingState | MovingTransition): The unit to be added to the chain container.
+
+        Returns:
+            Self: The current instance of the class.
+
+        Raises:
+            ValueError: If the type of the unit does not match the next need.
+            RuntimeError: If the type of the unit is neither `MovingState` nor `MovingTransition`.
+        """
+        unit_type = type(unit)
+        if unit_type != self.next_need:
+            raise ValueError(f"Need {self.next_need}, got {type(unit)}, which is {repr(unit)}!")
+        elif unit_type == MovingState:
+            self._chain_container[MovingState].append(unit)
+            if self.last_transition and unit not in self.last_transition.to_states.values():
+                raise ValueError(
+                    f"Connection break! The state {unit} should be in the to_states of the transition {self.last_transition}!"
+                )
+        elif unit_type == MovingTransition:
+            if self.last_state not in unit.from_states:
                 raise ValueError(
-                    f"The data pack {states} {transitions} is not valid! "
-                    f"A DataPack should have a length difference no more than 1!"
+                    f"Connection break! The state {self.last_state} should be in the from_states of the transition {repr(unit)}!"
                 )
 
+            self._chain_container[MovingTransition].append(unit)
+        else:
+            raise RuntimeError("Should never reach here!")
+        self._flip()
         return self
 
+    def _mid_transition_inject(self, states, transitions):
+        for sta, tran in zip(states, transitions):
+            # Ensure each state is in the corresponding transition's to_states
+            if sta not in tran.to_states.values():
+                raise ValueError(f"The state {sta} should be in the to_states of the transition {tran}!")
+            if self.last_state and self.last_state not in tran.from_states:
+                raise ValueError(f"The state {self.last_state} should be in the from_states of the transition {tran}!")
+            self._chain_container[MovingState].append(sta)
+            self._chain_container[MovingTransition].append(tran)
+
+    def _mid_state_inject(self, states, transitions):
+        for sta, tran in zip(states, transitions):
+            # Ensure each state is in the corresponding transition's from_states
+            if sta not in tran.from_states:
+                raise ValueError(f"The state {sta} should be in the from_states of the transition {tran}!")
+            if sta not in self.last_transition.to_states.values():
+                raise ValueError(f"The state {sta} should be in the to_states of the transition {tran}!")
+            self._chain_container[MovingState].append(sta)
+            self._chain_container[MovingTransition].append(tran)
+
 
 KT = TypeVar("KT", bound=Hashable)
 
 
 class CaseRegistry:
     """
     Initializes a new instance of the CaseRegistry class.
@@ -519,7 +532,20 @@
     )
     turn_transition = MovingTransition(
         from_states=[left_turn_state, right_turn_state],
         to_states={__PLACE_HOLDER__: end_state},
         duration=turn_duration,
     )
     return start_transition, turn_transition
+
+
+def copy(iters: Iterable[SupportClone]) -> List[SupportClone]:
+    """
+    Returns a new list containing clones of the elements in the input iterable.
+
+    Args:
+        iters (Iterable[SupportClone]): An iterable of objects that support the `clone()` method.
+
+    Returns:
+        List[SupportClone]: A new list containing clones of the input objects.
+    """
+    return [i.clone() for i in iters]
```

### Comparing `mentabotix-0.1.5.8/src/mentabotix/tools/generators.py` & `mentabotix-0.1.5.9/src/mentabotix/tools/generators.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.8/src/mentabotix/tools/selectors.py` & `mentabotix-0.1.5.9/src/mentabotix/tools/selectors.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.8/tests/find_tests.py` & `mentabotix-0.1.5.9/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.8/tests/test_botix.py` & `mentabotix-0.1.5.9/tests/test_botix.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import random
 import unittest
 from typing import List
 
 from bdmc.modules.controller import CloseLoopController
 
-from mentabotix import Botix, MovingState, MovingTransition
+from mentabotix import Botix, MovingState, MovingTransition, ArrowStyle
 from mentabotix.modules.exceptions import StructuralError
 
 
 class TestBotix(unittest.TestCase):
 
     def setUp(self):
         # 创建一些假的MovingState对象用于测试
@@ -346,10 +346,109 @@
         std_out = ""
         for state in states:
             std_out += str(state.tokenize(self.botix_instance.controller)[0][0])
 
         correct = ".set_motors_speed((state0_val_tmp1:=(state0_context_getter_1()),state0_val_tmp1,state0_val_tmp1,state0_val_tmp1)).set_motors_speed((state1_val_tmp1:=(state1_context_getter_1()),state1_val_tmp1,state1_val_tmp2:=(state1_context_getter_2()),state1_val_tmp2)).set_motors_speed((state2_context_getter_1(), state2_context_getter_2(), state2_context_getter_3(), state2_context_getter_4())).set_motors_speed((state3_val_tmp1:=(state3_context_getter_1()),state3_val_tmp1,100,100)).set_motors_speed((state4_context_getter_1(), state4_context_getter_2(), state4_context_getter_3(), 666)).set_motors_speed((500,500,state5_val_tmp2:=(state5_context_getter_1()),state5_val_tmp2)).set_motors_speed((state6_val_tmp1:=((state6_context_getter_temp_1:=state6_context_getter_1())),state6_val_tmp1,state6_val_tmp2:=(state6_context_getter_2()*state6_context_getter_temp_1),state6_val_tmp2))"
         self.assertEqual(correct, std_out)
 
+    def test_before_after_rendering(self):
+        MovingState.__state_id_counter__ = 0
+        MovingTransition.__transition_id_counter__ = 0
+
+        def tes_1() -> None: ...
+        def tes_2(): ...
+
+        def tes_3(): ...
+
+        state_a = MovingState(100, before_entering=[tes_1, tes_2], after_exiting=[tes_3])
+        state_b = MovingState(200, before_entering=[tes_3])
+        state_c = MovingState(300, after_exiting=[tes_3])
+        state_d = MovingState(400)
+        state_e = MovingState(500)
+        state_f = MovingState(600)
+
+        def transition_breaker_fac(lst: List[int]):
+            def _inner() -> int:
+                return random.choice(lst)
+
+            return _inner
+
+        transition_a_bcd = MovingTransition(
+            duration=1,
+            from_states=state_a,
+            to_states={1: state_b, 2: state_c, 3: state_d},
+            breaker=transition_breaker_fac([1, 2, 3]),
+        )
+        transition_d_ef = MovingTransition(
+            duration=1,
+            from_states=state_d,
+            to_states={1: state_e, 2: state_f},
+            breaker=transition_breaker_fac([1, 2]),
+        )
+        self.botix_instance.token_pool = [transition_a_bcd, transition_d_ef]
+        self.botix_instance.export_structure("test_entering_exiting.puml", self.botix_instance.token_pool)
+
+    def test_display_direction(self):
+        MovingState.__state_id_counter__ = 0
+        MovingTransition.__transition_id_counter__ = 0
+
+        def tes_1() -> None: ...
+        def tes_2(): ...
+
+        def tes_3(): ...
+
+        state_a = MovingState(100, before_entering=[tes_1, tes_2], after_exiting=[tes_3])
+        state_b = MovingState(200, before_entering=[tes_3])
+        state_c = MovingState(300, after_exiting=[tes_3])
+        state_d = MovingState(400)
+        state_e = MovingState(500)
+        state_f = MovingState(600)
+
+        def transition_breaker_fac(lst: List[int]):
+            def _inner() -> int:
+                return random.choice(lst)
+
+            return _inner
+
+        transition_a_bcd = MovingTransition(
+            duration=1,
+            from_states=state_a,
+            to_states={1: state_b, 2: state_c, 3: state_d},
+            breaker=transition_breaker_fac([1, 2, 3]),
+        )
+        transition_d_ef = MovingTransition(
+            duration=1,
+            from_states=state_d,
+            to_states={1: state_e, 2: state_f},
+            breaker=transition_breaker_fac([1, 2]),
+        )
+        self.botix_instance.token_pool = [transition_a_bcd, transition_d_ef]
+        self.botix_instance.export_structure("test_left.puml", self.botix_instance.token_pool, ArrowStyle.UP)
+
+    def test_empty_isolated_trans(self):
+        state_a = MovingState(100)
+
+        state_e = MovingState(500)
+        state_f = MovingState(600)
+
+        def transition_breaker_fac(lst: List[int]):
+            def _inner() -> int:
+                return random.choice(lst)
+
+            return _inner
+
+        transition_a_bcd = MovingTransition(
+            duration=1,
+            from_states=state_a,
+            breaker=transition_breaker_fac([1, 2, 3]),
+        )
+        transition_d_ef = MovingTransition(
+            duration=1,
+            to_states={1: state_e, 2: state_f},
+            breaker=transition_breaker_fac([1, 2]),
+        )
+        self.botix_instance.token_pool = [transition_a_bcd, transition_d_ef]
+        self.botix_instance.export_structure("test_isolated.puml", self.botix_instance.token_pool)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mentabotix-0.1.5.8/tests/test_case_registry.py` & `mentabotix-0.1.5.9/tests/test_case_registry.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.8/tests/test_composer.py` & `mentabotix-0.1.5.9/tests/test_composer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 import random
 import unittest
 
 from bdmc import CloseLoopController, MotorInfo
 
-from mentabotix import MovingChainComposer, MovingState, MovingTransition, straight_chain, Botix, random_lr_turn_branch
+from mentabotix import (
+    MovingChainComposer,
+    MovingState,
+    MovingTransition,
+    straight_chain,
+    Botix,
+    random_lr_turn_branch,
+    copy,
+)
 from mentabotix.tools.composers import __PLACE_HOLDER__
 
 
 # Assuming MovingState, MovingTransition, UnitType, StateTransitionPack are defined elsewhere
 # You'll need to replace these with the actual classes and types
 
 
@@ -306,10 +314,59 @@
             breaker=_a,
         )
         self.moving_chain_composer.init_container().add(state).add(transition).concat(*chain_pack)
         pack = self.moving_chain_composer.export_structure()[1]
         self.assertAlmostEqual(pre_val + dur - lead_time, sum(t.duration for t in pack))
         Botix.export_structure("seq_add_breaker.puml", pack)
 
+        # ----------------
+
+        state_1 = MovingState(100)
+        state_2 = MovingState(200)
+        state_3 = MovingState(300)
+        state_4 = MovingState(400)
+        state_123 = [state_1, state_2, state_3]
+        with self.assertRaises(ValueError):
+            sta, tran = (
+                self.moving_chain_composer.init_container()
+                # .add(MovingState.halt())
+                .concat(
+                    cloned := copy(state_123),
+                    [
+                        MovingTransition(1, to_states=cloned[1], from_states=cloned[0]),
+                        MovingTransition(2, to_states=cloned[2], from_states=[]),
+                        MovingTransition(3, from_states=cloned[2]),
+                    ],
+                ).export_structure()
+            )
+
+        sta, tran = (
+            self.moving_chain_composer.init_container()
+            # .add(MovingState.halt())
+            .concat(
+                cloned := copy(state_123),
+                [
+                    MovingTransition(1, to_states=cloned[1], from_states=cloned[0]),
+                    MovingTransition(2, to_states=cloned[2], from_states=cloned[1]),
+                ],
+            ).export_structure()
+        )
+        Botix.export_structure("test_seq_concat_mode1.puml", tran)
+
+        sta, tran = (
+            self.moving_chain_composer.init_container()
+            # .add(MovingState.halt())
+            .concat(
+                cloned := copy(state_123),
+                [
+                    MovingTransition(1, to_states=cloned[1], from_states=cloned[0]),
+                    MovingTransition(2, to_states=cloned[2], from_states=cloned[1]),
+                    MovingTransition(3, from_states=cloned[2]),
+                ],
+            ).export_structure()
+        )
+
+        Botix.export_structure("test_seq_concat_mode2.puml", tran)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mentabotix-0.1.5.8/tests/test_menta.py` & `mentabotix-0.1.5.9/tests/test_menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.8/tests/test_moving_state.py` & `mentabotix-0.1.5.9/tests/test_moving_state.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.8/tests/test_moving_transition.py` & `mentabotix-0.1.5.9/tests/test_moving_transition.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.8/PKG-INFO` & `mentabotix-0.1.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: mentabotix
-Version: 0.1.5.8
+Version: 0.1.5.9
 Summary: A Bot control lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: terminaltables>=3.1.10
 Requires-Dist: bdmc>=0.1.5.10
+Requires-Dist: pyuptech>=0.1.6.4
 Description-Content-Type: text/markdown
 
 # mentabotix
 
 > A dedicated lib to control 4-fixed-wheels robot
 ---
```

