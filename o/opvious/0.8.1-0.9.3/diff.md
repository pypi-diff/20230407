# Comparing `tmp/opvious-0.8.1.tar.gz` & `tmp/opvious-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opvious-0.8.1.tar", max compression
+gzip compressed data, was "opvious-0.9.3.tar", max compression
```

## Comparing `opvious-0.8.1.tar` & `opvious-0.9.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    10756 2023-03-22 01:10:25.353147 opvious-0.8.1/LICENSE
--rw-r--r--   0        0        0     3174 2023-03-22 01:10:25.353147 opvious-0.8.1/README.md
--rw-r--r--   0        0        0     1878 2023-03-22 01:10:25.353147 opvious-0.8.1/opvious/__init__.py
--rw-r--r--   0        0        0    21613 2023-03-22 01:10:25.353147 opvious-0.8.1/opvious/client.py
--rw-r--r--   0        0        0      969 2023-03-22 01:10:25.353147 opvious-0.8.1/opvious/common.py
--rw-r--r--   0        0        0    13133 2023-03-22 01:10:25.353147 opvious-0.8.1/opvious/data.py
--rw-r--r--   0        0        0     1745 2023-03-22 01:10:25.353147 opvious-0.8.1/opvious/executors/__init__.py
--rw-r--r--   0        0        0     1800 2023-03-22 01:11:07.545611 opvious-0.8.1/opvious/executors/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4124 2023-03-22 01:11:07.557611 opvious-0.8.1/opvious/executors/__pycache__/aiohttp.cpython-310.pyc
--rw-r--r--   0        0        0     5862 2023-03-22 01:11:07.549611 opvious-0.8.1/opvious/executors/__pycache__/common.cpython-310.pyc
--rw-r--r--   0        0        0     3503 2023-03-22 01:11:07.669612 opvious-0.8.1/opvious/executors/__pycache__/urllib.cpython-310.pyc
--rw-r--r--   0        0        0     4501 2023-03-22 01:10:25.353147 opvious-0.8.1/opvious/executors/aiohttp.py
--rw-r--r--   0        0        0     4621 2023-03-22 01:10:25.353147 opvious-0.8.1/opvious/executors/common.py
--rw-r--r--   0        0        0     3046 2023-03-22 01:10:25.353147 opvious-0.8.1/opvious/executors/pyodide.py
--rw-r--r--   0        0        0     3522 2023-03-22 01:10:25.353147 opvious-0.8.1/opvious/executors/urllib.py
--rw-r--r--   0        0        0      734 2023-03-22 01:10:25.353147 opvious-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     4117 1970-01-01 00:00:00.000000 opvious-0.8.1/setup.py
--rw-r--r--   0        0        0     3973 1970-01-01 00:00:00.000000 opvious-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    10756 2023-04-07 18:18:57.258050 opvious-0.9.3/LICENSE
+-rw-r--r--   0        0        0     3181 2023-04-07 18:18:57.258050 opvious-0.9.3/README.md
+-rw-r--r--   0        0        0     1982 2023-04-07 18:18:57.258050 opvious-0.9.3/opvious/__init__.py
+-rw-r--r--   0        0        0    23218 2023-04-07 18:18:57.258050 opvious-0.9.3/opvious/client.py
+-rw-r--r--   0        0        0     1062 2023-04-07 18:18:57.258050 opvious-0.9.3/opvious/common.py
+-rw-r--r--   0        0        0    15835 2023-04-07 18:18:57.258050 opvious-0.9.3/opvious/data.py
+-rw-r--r--   0        0        0     1966 2023-04-07 18:18:57.258050 opvious-0.9.3/opvious/executors/__init__.py
+-rw-r--r--   0        0        0     1880 2023-04-07 18:19:47.474284 opvious-0.9.3/opvious/executors/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3521 2023-04-07 18:19:47.486284 opvious-0.9.3/opvious/executors/__pycache__/aiohttp.cpython-310.pyc
+-rw-r--r--   0        0        0     9497 2023-04-07 18:19:47.478284 opvious-0.9.3/opvious/executors/__pycache__/common.cpython-310.pyc
+-rw-r--r--   0        0        0     2762 2023-04-07 18:19:47.566285 opvious-0.9.3/opvious/executors/__pycache__/urllib.cpython-310.pyc
+-rw-r--r--   0        0        0     4068 2023-04-07 18:18:57.258050 opvious-0.9.3/opvious/executors/aiohttp.py
+-rw-r--r--   0        0        0     8799 2023-04-07 18:18:57.262050 opvious-0.9.3/opvious/executors/common.py
+-rw-r--r--   0        0        0     2412 2023-04-07 18:18:57.262050 opvious-0.9.3/opvious/executors/pyodide.py
+-rw-r--r--   0        0        0     2685 2023-04-07 18:18:57.262050 opvious-0.9.3/opvious/executors/urllib.py
+-rw-r--r--   0        0        0      788 2023-04-07 18:18:57.262050 opvious-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     4125 1970-01-01 00:00:00.000000 opvious-0.9.3/setup.py
+-rw-r--r--   0        0        0     3981 1970-01-01 00:00:00.000000 opvious-0.9.3/PKG-INFO
```

### Comparing `opvious-0.8.1/LICENSE` & `opvious-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opvious-0.8.1/README.md` & `opvious-0.9.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ```python
 import opvious
 
 # Instantiate an API client from an API token
 client = opvious.Client.from_token(TOKEN)
 
 # Solve a simple portfolio selection optimization model
-outputs = await client.solve(
+response = await client.solve(
     sources=[
       r"""
           We find an allocation of assets which minimizes risk while satisfying
           a minimum expected return:
 
           + A collection of assets: $\S^d_{asset}: A$
           + Covariances: $\S^p_{covariance}: c \in \mathbb{R}^{A \times A}$
@@ -58,18 +58,18 @@
             # ..
         },
         "desiredReturn": 0.05,
     },
 )
 
 # Print the optimal allocation, if any
-if isinstance(outputs.outcome, opvious.FeasibleOutcome):
-  print(outputs.data.variable("allocation"))
+if isinstance(response.outcome, opvious.FeasibleOutcome):
+  print(response.outputs.variable("allocation"))
 else:
-  print(f"Problem was {outputs.status}.") # INFEASIBLE, UNBOUNDED
+  print(f"Problem was {response.status}.") # INFEASIBLE, UNBOUNDED
 ```
 
 
 ## Environments
 
 Clients are compatible with Pyodide environments, for example [JupyterLite][]
 kernels. Simply install the package as usual in a notebook, omitting the `aio`
```

### Comparing `opvious-0.8.1/opvious/__init__.py` & `opvious-0.9.3/opvious/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,66 +16,69 @@
   specific language governing permissions and limitations
   under the License.
 """
 
 import logging
 
 from .client import Client
+from .common import __version__
 from .executors import ApiError, Executor
 from .data import (
     Attempt,
+    AttemptRequest,
     CancelledOutcome,
     ConstraintRelaxation,
     DimensionArgument,
     FailedOutcome,
     FeasibleOutcome,
     InfeasibleOutcome,
-    InputData,
-    Inputs,
     Key,
     KeyItem,
     Label,
     Notification,
     Outcome,
-    OutputData,
-    Outputs,
     Penalty,
     Relaxation,
+    SolveInputs,
+    SolveOptions,
+    SolveOutputs,
+    SolveResponse,
     SparseTensorArgument,
     Summary,
     Tensor,
     TensorArgument,
     UnboundedOutcome,
     Value,
 )
 
 
 __all__ = [
+    "__version__",
     "ApiError",
     "Attempt",
+    "AttemptRequest",
     "CancelledOutcome",
     "Client",
     "ConstraintRelaxation",
     "DimensionArgument",
     "Executor",
     "FailedOutcome",
     "FeasibleOutcome",
     "InfeasibleOutcome",
-    "InputData",
-    "Inputs",
-    "InputsBuilder",
     "Key",
     "KeyItem",
     "Label",
     "Notification",
     "Outcome",
-    "OutputData",
-    "Outputs",
     "Penalty",
     "Relaxation",
+    "SolveInputs",
+    "SolveOptions",
+    "SolveOutputs",
+    "SolveResponse",
     "SparseTensorArgument",
     "Summary",
     "Tensor",
     "TensorArgument",
     "UnboundedOutcome",
     "Value",
 ]
```

### Comparing `opvious-0.8.1/opvious/client.py` & `opvious-0.9.3/opvious/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,39 +19,55 @@
 
 import backoff
 from datetime import datetime, timezone
 import json
 import humanize
 import logging
 import os
-from typing import Any, Dict, List, Mapping, Optional, Tuple, Union
+from typing import (
+    Any,
+    cast,
+    Dict,
+    Mapping,
+    Optional,
+    Tuple,
+    Union,
+)
 
 from .common import format_percent, strip_nones
 from .data import (
     Attempt,
+    AttemptRequest,
     CancelledOutcome,
     DimensionArgument,
     FailedOutcome,
     FeasibleOutcome,
     InfeasibleOutcome,
-    InputData,
-    Inputs,
     Label,
     Notification,
     Outcome,
     Outline,
-    OutputData,
-    Outputs,
     Relaxation,
+    SolveInputs,
+    SolveOptions,
+    SolveOutputs,
+    SolveResponse,
+    solve_options_to_json,
     Summary,
     Tensor,
     TensorArgument,
     UnboundedOutcome,
 )
-from .executors import default_executor, Executor, execute_graphql_query
+from .executors import (
+    default_executor,
+    Executor,
+    JsonExecutorResult,
+    JsonSeqExecutorResult,
+    PlainTextExecutorResult,
+)
 
 
 _logger = logging.getLogger(__name__)
 
 
 _DEFAULT_DOMAIN = "beta.opvious.io"
 
@@ -96,91 +112,77 @@
         contain a valid API token. OPVIOUS_DOMAIN can optionally be set to use
         a custom domain.
         """
         return Client.from_token(
             token=env[_TOKEN_EVAR], domain=env.get(_DOMAIN_EVAR)
         )
 
+    async def inspect(
+        self,
+        sources: Optional[list[str]] = None,
+        formulation_name: Optional[str] = None,
+        tag_name: Optional[str] = None,
+        parameters: Optional[Mapping[Label, TensorArgument]] = None,
+        dimensions: Optional[Mapping[Label, DimensionArgument]] = None,
+    ) -> str:
+        """Inspects an optimization problem, returning its underlying solver
+        instructions.
+        """
+        body, _outline = await self._assemble_solve_request(
+            sources=sources,
+            formulation_name=formulation_name,
+            tag_name=tag_name,
+            parameters=parameters,
+            dimensions=dimensions,
+        )
+        async with self._executor.execute(
+            result_type=PlainTextExecutorResult,
+            path="/solves/inspect/instructions",
+            method="POST",
+            json_data={
+                "runRequest": body,
+            },
+        ) as res:
+            lines = []
+            async for line in res.lines():
+                if line.startswith("\\"):
+                    _logger.debug(line[2:].strip())
+                else:
+                    lines.append(line)
+            return "".join(lines)
+
     async def solve(
         self,
         sources: Optional[list[str]] = None,
         formulation_name: Optional[str] = None,
         tag_name: Optional[str] = None,
         parameters: Optional[Mapping[Label, TensorArgument]] = None,
         dimensions: Optional[Mapping[Label, DimensionArgument]] = None,
-        relative_gap_threshold: Optional[float] = None,
-        absolute_gap_threshold: Optional[float] = None,
-        primal_value_epsilon: Optional[float] = None,
-        timeout_millis: Optional[float] = None,
-    ) -> Outputs:
+        relaxation: Optional[Relaxation] = None,
+        options: Optional[SolveOptions] = None,
+    ) -> SolveResponse:
         """Solves an optimization problem. See also `start_attempt` for an
         alternative for long-running solves.
         """
-        # First we fetch the outline to validate/coerce inputs later on
-        if formulation_name:
-            if sources:
-                raise Exception(
-                    "Sources and formulation name are mutually exclusive"
-                )
-            outline, _tag = await self._fetch_formulation_outline(
-                formulation_name, tag_name
-            )
-            formulation = strip_nones(
-                {
-                    "name": formulation_name,
-                    "specificationTagName": tag_name,
-                }
-            )
-        else:
-            if not sources:
-                raise Exception("Sources or formulation name must be set")
-            outline = await self._fetch_sources_outline(sources)
-            formulation = {"sources": sources}
-
-        # Then we assemble the inputs
-        builder = _InputDataBuilder(outline=outline)
-        if dimensions:
-            for label, dim in dimensions.items():
-                builder.set_dimension(label, dim)
-        if parameters:
-            for label, param in parameters.items():
-                builder.set_parameter(label, param)
-        inputs = builder.build()
-        _logger.info(
-            "Validated inputs. [parameters=%s]",
-            builder.parameter_entry_count,
+        body, outline = await self._assemble_solve_request(
+            sources=sources,
+            formulation_name=formulation_name,
+            tag_name=tag_name,
+            parameters=parameters,
+            dimensions=dimensions,
+            relaxation=relaxation,
+            options=options,
         )
-
-        # After that we parse the streamed response data
         solved_data = None
         async with self._executor.execute(
+            result_type=JsonSeqExecutorResult,
             path="/solves/run",
             method="POST",
-            headers={
-                "accept": "application/json-seq, text/*",
-            },
-            json_body={
-                "formulation": formulation,
-                "inputs": strip_nones(
-                    {
-                        "dimensions": inputs.raw_dimensions,
-                        "parameters": inputs.raw_parameters,
-                    }
-                ),
-                "options": strip_nones(
-                    {
-                        "absoluteGapThreshold": absolute_gap_threshold,
-                        "relativeGapThreshold": relative_gap_threshold,
-                        "timeoutMillis": timeout_millis,
-                        "primalValueEpsilon": primal_value_epsilon,
-                    }
-                ),
-            },
+            json_data=body,
         ) as res:
-            _logger.debug("Uploaded inputs.")
             async for data in res.json_seq_data():
                 kind = data["kind"]
                 if kind == "reifying":
                     progress = data["progress"]
                     if progress["kind"] == "constraint":
                         summary = progress["summary"]
                         _logger.debug(
@@ -209,167 +211,216 @@
                     if iter_count is not None:
                         _logger.info(
                             "Solve in progress... [iters=%s, cuts=%s, gap=%s]",
                             iter_count,
                             progress.get("cutCount"),
                             "n/a" if gap is None else format_percent(gap),
                         )
-                else:
+                elif kind == "solved":
                     _logger.debug("Downloaded outputs.")
                     reached_at = datetime.now(timezone.utc)
                     solved_data = data
+                elif kind == "error":
+                    message = data["error"]["message"]
+                    raise Exception(f"Solve failed: {message}")
+                else:
+                    raise Exception(f"Unexpected response: {json.dumps(data)}")
+        if not solved_data:
+            raise Exception("Solve terminated without any data")
 
         # Finally we gather the outputs
         outcome_data = solved_data["outcome"]
         status = outcome_data["status"]
         if status == "INFEASIBLE":
-            outcome = InfeasibleOutcome(reached_at)
+            outcome = cast(Outcome, InfeasibleOutcome(reached_at))
         elif status == "UNBOUNDED":
             outcome = UnboundedOutcome(reached_at)
         else:
             outcome = FeasibleOutcome(
                 reached_at=reached_at,
                 is_optimal=status == "OPTIMAL",
                 objective_value=outcome_data.get("objectiveValue"),
                 relative_gap=outcome_data.get("relativeGap"),
             )
-        outputs_data = None
+        outputs = None
         if isinstance(outcome, FeasibleOutcome):
-            outputs_data = OutputData.from_json(
+            outputs = SolveOutputs.from_json(
                 data=solved_data["outputs"],
                 outline=outline,
             )
-        return Outputs(
+        return SolveResponse(
             status=status,
             outcome=outcome,
             summary=summary,
-            data=outputs_data,
+            outputs=outputs,
         )
 
+    async def _assemble_solve_request(
+        self,
+        sources: Optional[list[str]] = None,
+        formulation_name: Optional[str] = None,
+        tag_name: Optional[str] = None,
+        parameters: Optional[Mapping[Label, TensorArgument]] = None,
+        dimensions: Optional[Mapping[Label, DimensionArgument]] = None,
+        options: Optional[SolveOptions] = None,
+        relaxation: Union[None, Relaxation] = None,
+    ) -> Tuple[Any, Outline]:
+        # First we fetch the outline to validate/coerce inputs later on
+        if formulation_name:
+            if sources:
+                raise Exception(
+                    "Sources and formulation name are mutually exclusive"
+                )
+            outline, _tag = await self._fetch_formulation_outline(
+                formulation_name, tag_name
+            )
+            formulation = strip_nones(
+                {
+                    "name": formulation_name,
+                    "specificationTagName": tag_name,
+                }
+            )
+        else:
+            if not sources:
+                raise Exception("Sources or formulation name must be set")
+            outline = await self._fetch_sources_outline(sources)
+            formulation = {"sources": sources}
+
+        # Then we assemble the inputs
+        builder = _SolveInputsBuilder(outline=outline)
+        if dimensions:
+            for label, dim in dimensions.items():
+                builder.set_dimension(label, dim)
+        if parameters:
+            for label, param in parameters.items():
+                builder.set_parameter(label, param)
+        inputs = builder.build()
+        _logger.info(
+            "Validated inputs. [parameters=%s]",
+            builder.parameter_entry_count,
+        )
+
+        # Finally we put everything together
+        body = {
+            "formulation": formulation,
+            "inputs": strip_nones(
+                {
+                    "dimensions": inputs.raw_dimensions,
+                    "parameters": inputs.raw_parameters,
+                }
+            ),
+            "options": solve_options_to_json(options, relaxation),
+        }
+        return (body, outline)
+
     async def _fetch_sources_outline(self, sources: list[str]) -> Outline:
         async with self._executor.execute(
+            result_type=JsonExecutorResult,
             path="/sources/parse",
             method="POST",
-            json_body={"sources": sources, "outline": True},
+            json_data={"sources": sources, "outline": True},
         ) as res:
             outline_data = res.json_data()
         errors = outline_data.get("errors")
         if errors:
             raise Exception(f"Invalid sources: {json.dumps(errors)}")
         return Outline.from_json(outline_data["outline"])
 
     async def _fetch_formulation_outline(
         self, name: str, tag_name: Optional[str] = None
     ) -> Tuple[Outline, str]:
-        data = await execute_graphql_query(
-            executor=self._executor,
+        data = await self._executor.execute_graphql_query(
             query="@FetchOutline",
             variables={"formulationName": name, "tagName": tag_name},
         )
         formulation = data.get("formulation")
         if not formulation:
             raise Exception("No matching formulation found")
         tag = formulation.get("tag")
         if not tag:
             raise Exception("No matching specification found")
         spec = tag["specification"]
         outline = Outline.from_json(spec["outline"])
-        return [outline, tag["name"]]
+        return (outline, tag["name"])
 
-    async def assemble_inputs(
+    async def prepare_attempt_request(
         self,
         formulation_name: str,
         tag_name: Optional[str] = None,
         parameters: Optional[Mapping[Label, TensorArgument]] = None,
         dimensions: Optional[Mapping[Label, DimensionArgument]] = None,
-    ) -> Inputs:
+    ) -> AttemptRequest:
         """Assembles and validates inputs for a given formulation. The returned
         object can be used to start an asynchronous solve via `start_attempt`.
         """
         outline, tag = await self._fetch_formulation_outline(
             formulation_name, tag_name
         )
-        builder = _InputDataBuilder(outline)
+        builder = _SolveInputsBuilder(outline)
         if dimensions:
             for label, dim in dimensions.items():
                 builder.set_dimension(label, dim)
         if parameters:
             for label, param in parameters.items():
                 builder.set_parameter(label, param)
-        return Inputs(
+        return AttemptRequest(
             formulation_name=formulation_name,
             tag_name=tag,
-            data=builder.build(),
+            inputs=builder.build(),
         )
 
     async def start_attempt(
         self,
-        inputs: Inputs,
-        relative_gap_threshold: Optional[float] = None,
-        absolute_gap_threshold: Optional[float] = None,
-        primal_value_epsilon: Optional[float] = None,
-        timeout_millis: Optional[float] = None,
-        relaxed_constraints: Union[None, List[Label], Relaxation] = None,
+        request: AttemptRequest,
+        options: Optional[SolveOptions] = None,
+        relaxation: Union[None, Relaxation] = None,
         pinned_variables: Optional[Mapping[Label, TensorArgument]] = None,
     ) -> Attempt:
         """Starts a new asynchronous solve attempt."""
-        if relaxed_constraints:
-            if isinstance(relaxed_constraints, list):
-                data = Relaxation.from_constraint_labels(relaxed_constraints)
-            else:
-                data = relaxed_constraints
-            relaxation = data.to_json()
-        else:
-            relaxation = None
         pins = []
         if pinned_variables:
             for label, arg in pinned_variables.items():
-                var_outline = inputs.data.outline.variables.get(label)
+                var_outline = request.inputs.outline.variables.get(label)
                 if not var_outline:
                     raise Exception(f"Unknown variable {label}")
-                tensor = Tensor.from_argument(arg, var_outline.is_indicator())
+                tensor = Tensor.from_argument(
+                    arg, len(var_outline.bindings), var_outline.is_indicator()
+                )
                 if tensor.default_value:
                     raise Exception("Pinned variables may not have defaults")
                 pins.append({"label": label, "entries": tensor.entries})
+
         async with self._executor.execute(
+            result_type=JsonExecutorResult,
             path="/attempts/start",
             method="POST",
-            json_body={
-                "formulationName": inputs.formulation_name,
-                "specificationTagName": inputs.tag_name,
+            json_data={
+                "formulationName": request.formulation_name,
+                "specificationTagName": request.tag_name,
                 "inputs": strip_nones(
                     {
-                        "dimensions": inputs.data.raw_dimensions,
-                        "parameters": inputs.data.raw_parameters,
+                        "dimensions": request.inputs.raw_dimensions,
+                        "parameters": request.inputs.raw_parameters,
                         "pinnedVariables": pins,
                     }
                 ),
-                "options": strip_nones(
-                    {
-                        "absoluteGapThreshold": absolute_gap_threshold,
-                        "relativeGapThreshold": relative_gap_threshold,
-                        "timeoutMillis": timeout_millis,
-                        "primalValueEpsilon": primal_value_epsilon,
-                        "relaxation": relaxation,
-                    }
-                ),
+                "options": solve_options_to_json(options, relaxation),
             },
         ) as res:
             uuid = res.json_data()["uuid"]
         return Attempt(
             uuid=uuid,
             started_at=datetime.now(timezone.utc),
-            outline=inputs.data.outline,
+            outline=request.inputs.outline,
             url=self._attempt_url(uuid),
         )
 
     async def load_attempt(self, uuid: str) -> Optional[Attempt]:
         """Loads an existing attempt from its UUID."""
-        data = await execute_graphql_query(
-            executor=self._executor,
+        data = await self._executor.execute_graphql_query(
             query="@FetchAttempt",
             variables={"uuid": uuid},
         )
         attempt = data["attempt"]
         if not attempt:
             return None
         return Attempt.from_graphql(
@@ -379,41 +430,39 @@
         )
 
     def _attempt_url(self, uuid) -> str:
         return self._hub_url + "/attempts/" + uuid
 
     async def cancel_attempt(self, uuid: str) -> bool:
         """Cancels a running attempt."""
-        data = await execute_graphql_query(
-            executor=self._executor,
+        data = await self._executor.execute_graphql_query(
             query="@CancelAttempt",
             variables={"uuid": uuid},
         )
         return bool(data["cancelAttempt"])
 
     async def poll_attempt(
         self, attempt: Attempt
     ) -> Union[Notification, Outcome]:
         """Polls an attempt for its outcome or latest progress notification."""
-        data = await execute_graphql_query(
-            executor=self._executor,
+        data = await self._executor.execute_graphql_query(
             query="@PollAttempt",
             variables={"uuid": attempt.uuid},
         )
         attempt_data = data["attempt"]
         status = attempt_data["status"]
         if status == "PENDING":
             edges = attempt_data["notifications"]["edges"]
             return Notification.from_graphql(
                 dequeued=bool(attempt_data["dequeuedAt"]),
                 data=edges[0]["node"] if edges else None,
             )
         reached_at = datetime.fromisoformat(attempt_data["endedAt"])
         if status == "CANCELLED":
-            return CancelledOutcome(reached_at)
+            return cast(Outcome, CancelledOutcome(reached_at))
         if status == "INFEASIBLE":
             return InfeasibleOutcome(reached_at)
         if status == "UNBOUNDED":
             return UnboundedOutcome(reached_at)
         outcome = attempt_data["outcome"]
         if status == "ERRORED":
             return FailedOutcome.from_graphql(reached_at, outcome)
@@ -487,36 +536,40 @@
         """Waits for the attempt to complete and returns its outcome."""
         print(f"Tracking attempt... [url={attempt.url}]")
         outcome = await self._track_attempt(attempt, silent=silent)
         if assert_feasible and not isinstance(outcome, FeasibleOutcome):
             raise Exception(f"Unexpected outcome: {outcome}")
         return outcome
 
-    async def fetch_input_data(self, attempt: Attempt) -> InputData:
-        url = f"/attempts/{attempt.uuid}/inputs"
-        async with self._executor.execute(url) as res:
+    async def fetch_attempt_inputs(self, attempt: Attempt) -> SolveInputs:
+        async with self._executor.execute(
+            result_type=JsonExecutorResult,
+            path=f"/attempts/{attempt.uuid}/inputs",
+        ) as res:
             data = res.json_data()
-        return InputData(
+        return SolveInputs(
             outline=attempt.outline,
             raw_parameters=data["parameters"],
             raw_dimensions=data["dimensions"],
         )
 
-    async def fetch_output_data(self, attempt: Attempt) -> OutputData:
-        url = f"/attempts/{attempt.uuid}/outputs"
-        async with self._executor.execute(url) as res:
+    async def fetch_attempt_outputs(self, attempt: Attempt) -> SolveOutputs:
+        async with self._executor.execute(
+            result_type=JsonExecutorResult,
+            path=f"/attempts/{attempt.uuid}/outputs",
+        ) as res:
             data = res.json_data()
-        return OutputData(
+        return SolveOutputs(
             outline=attempt.outline,
             raw_variables=data["variables"],
             raw_constraints=data["constraints"],
         )
 
 
-class _InputDataBuilder:
+class _SolveInputsBuilder:
     def __init__(self, outline: Outline):
         self._outline = outline
         self._dimensions: Dict[Label, Any] = {}
         self._parameters: Dict[Label, Any] = {}
         self.parameter_entry_count = 0
 
     def set_dimension(self, label: Label, arg: DimensionArgument) -> None:
@@ -528,37 +581,42 @@
         items = list(arg)
         self._dimensions[label] = {"label": label, "items": items}
 
     def set_parameter(self, label: Label, arg: Any) -> None:
         outline = self._outline.parameters.get(label)
         if not outline:
             raise Exception(f"Unknown parameter: {label}")
-        tensor = Tensor.from_argument(arg, outline.is_indicator())
         if label in self._parameters:
             raise Exception(f"Duplicate parameter: {label}")
+        try:
+            tensor = Tensor.from_argument(
+                arg, len(outline.bindings), outline.is_indicator()
+            )
+        except Exception as exc:
+            raise ValueError(f"Invalid  parameter: {label}") from exc
         self._parameters[label] = {
             "label": label,
             "entries": tensor.entries,
             "defaultValue": tensor.default_value,
         }
         self.parameter_entry_count += len(tensor.entries)
 
-    def build(self) -> Inputs:
+    def build(self) -> SolveInputs:
         missing_labels = set()
 
         for label in self._outline.parameters:
             if label not in self._parameters:
                 missing_labels.add(label)
 
         if self._dimensions:
             for label in self._outline.dimensions:
                 if label not in self._dimensions:
                     missing_labels.add(label)
 
         if missing_labels:
             raise Exception(f"Missing label(s): {missing_labels}")
 
-        return InputData(
+        return SolveInputs(
             outline=self._outline,
             raw_parameters=list(self._parameters.values()),
             raw_dimensions=list(self._dimensions.values()) or None,
         )
```

### Comparing `opvious-0.8.1/opvious/common.py` & `opvious-0.9.3/opvious/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,14 +13,22 @@
   software distributed under the License is distributed on an
   "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
   KIND, either express or implied.  See the License for the
   specific language governing permissions and limitations
   under the License.
 """
 
+from importlib import metadata
+
+
+__version__ = metadata.version(__package__)
+
+
+del metadata
+
 
 def format_percent(val):
     if val == "Infinity":
         return "inf"
     return f"{int(val * 10_000) / 100}%"
```

### Comparing `opvious-0.8.1/opvious/data.py` & `opvious-0.9.3/opvious/data.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,16 +17,17 @@
   under the License.
 """
 
 from __future__ import annotations
 
 import dataclasses
 from datetime import datetime
+import math
 import pandas as pd
-from typing import Any, Iterable, List, Mapping, Optional, Tuple, Union
+from typing import Any, Iterable, Mapping, Optional, Tuple, Union
 
 from .common import strip_nones
 
 
 KeyItem = Union[float, int, str]
 
 
@@ -58,98 +59,135 @@
 
 
 TensorArgument = Union[
     Value, SparseTensorArgument, Tuple[SparseTensorArgument, Value]
 ]
 
 
+ExtendedFloat = Union[float, str]
+
+
+def encode_extended_float(val: float):
+    if val == math.inf:
+        return "Infinity"
+    elif val == -math.inf:
+        return "-Infinity"
+    return val
+
+
+def decode_extended_float(val: ExtendedFloat):
+    if val == "Infinity":
+        return math.inf
+    elif val == "-Infinity":
+        return -math.inf
+    return val
+
+
 @dataclasses.dataclass
 class Tensor:
-    entries: List[Any]
-    default_value: float = 0
+    entries: list[Any]
+    default_value: ExtendedFloat = 0
 
     @classmethod
-    def from_argument(cls, arg: TensorArgument, is_indicator: bool = False):
+    def from_argument(
+        cls, arg: TensorArgument, rank: int, is_indicator: bool = False
+    ):
         if isinstance(arg, tuple):
             data, default_value = arg
+        elif rank > 0 and is_value(arg) and not is_indicator:
+            data = {}
+            default_value = arg
         else:
             data = arg
             default_value = 0
         if (
             is_indicator
             and isinstance(data, pd.Series)
             and not pd.api.types.is_numeric_dtype(data)
         ):
             data = data.reset_index()
+        keyifier = _Keyifier(rank)
         if is_indicator and isinstance(data, pd.DataFrame):
             entries = [
-                {"key": key, "value": 1}
+                {"key": keyifier.keyify(key), "value": 1}
                 for key in data.itertuples(index=False, name=None)
             ]
         elif is_indicator and not hasattr(data, "items"):
-            entries = [{"key": key, "value": 1} for key in data]
+            entries = [
+                {"key": keyifier.keyify(key), "value": 1} for key in data
+            ]
         else:
             if is_value(data):
-                entries = [{"key": (), "value": data}]
+                entries = [{"key": (), "value": encode_extended_float(data)}]
             else:
                 entries = [
-                    {"key": _keyify(key), "value": value}
+                    {
+                        "key": keyifier.keyify(key),
+                        "value": encode_extended_float(value),
+                    }
                     for key, value in data.items()
                 ]
-        return Tensor(entries, default_value)
+        return Tensor(entries, encode_extended_float(default_value))
 
 
-def _keyify(key):
-    return tuple(key) if isinstance(key, (list, tuple)) else (key,)
+class _Keyifier:
+    def __init__(self, rank: int):
+        self.rank = rank
+
+    def keyify(self, key):
+        tup = tuple(key) if isinstance(key, (list, tuple)) else (key,)
+        if len(tup) != self.rank:
+            raise Exception(f"Invalid key rank: {len(tup)} != {self.rank}")
+        return tup
 
 
 # Outlines
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class SourceBinding:
     dimension_label: Optional[Label]
     qualifier: Optional[Label]
 
     @classmethod
     def from_json(cls, data: Any) -> SourceBinding:
         return SourceBinding(
             dimension_label=data.get("dimensionLabel"),
             qualifier=data.get("qualifier"),
         )
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class ObjectiveOutline:
     is_maximization: bool
 
     @classmethod
     def from_json(cls, data: Any) -> ObjectiveOutline:
         return ObjectiveOutline(is_maximization=data["isMaximization"])
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class DimensionOutline:
     label: Label
     is_numeric: bool
 
     @classmethod
     def from_json(cls, data: Any) -> DimensionOutline:
         return DimensionOutline(
             label=data["label"], is_numeric=data["isNumeric"]
         )
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class TensorOutline:
     label: Label
     lower_bound: Optional[Value]
     upper_bound: Optional[Value]
     is_integral: bool
-    bindings: List[SourceBinding]
+    bindings: list[SourceBinding]
 
     def is_indicator(self) -> bool:
         return (
             self.is_integral
             and self.lower_bound == 0
             and self.upper_bound == 1
         )
@@ -163,28 +201,28 @@
             lower_bound=lb if is_value(lb) else None,
             upper_bound=ub if is_value(ub) else None,
             is_integral=data["isIntegral"],
             bindings=[SourceBinding.from_json(b) for b in data["bindings"]],
         )
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class ConstraintOutline:
     label: Label
-    bindings: List[SourceBinding]
+    bindings: list[SourceBinding]
 
     @classmethod
     def from_json(cls, data: Any) -> ConstraintOutline:
         return ConstraintOutline(
             label=data["label"],
             bindings=[SourceBinding.from_json(b) for b in data["bindings"]],
         )
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class Outline:
     objective: Optional[ObjectiveOutline]
     dimensions: Mapping[Label, DimensionOutline]
     parameters: Mapping[Label, TensorOutline]
     variables: Mapping[Label, TensorOutline]
     constraints: Mapping[Label, ConstraintOutline]
 
@@ -203,20 +241,20 @@
 def _map_outlines(cls, data):
     return {o["label"]: cls.from_json(o) for o in data}
 
 
 # Outcomes
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class CancelledOutcome:
     reached_at: datetime
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class FailedOutcome:
     reached_at: datetime
     status: str
     message: str
     code: Optional[str]
     tags: Any
 
@@ -228,15 +266,15 @@
             status=failure["status"],
             message=failure["message"],
             code=failure.get("code"),
             tags=failure.get("tags"),
         )
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class FeasibleOutcome:
     reached_at: datetime
     is_optimal: bool
     objective_value: Optional[Value]
     relative_gap: Optional[Value]
 
     @classmethod
@@ -245,20 +283,20 @@
             reached_at=reached_at,
             is_optimal=data["isOptimal"],
             objective_value=data.get("objectiveValue"),
             relative_gap=data.get("relativeGap"),
         )
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class InfeasibleOutcome:
     reached_at: datetime
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class UnboundedOutcome:
     reached_at: datetime
 
 
 Outcome = Union[
     FailedOutcome,
     FeasibleOutcome,
@@ -266,15 +304,15 @@
     UnboundedOutcome,
 ]
 
 
 # Summaries
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class Summary:
     column_count: int
     row_count: int
     weight_count: int
 
     def density(self) -> float:
         denom = self.column_count * self.row_count
@@ -297,132 +335,150 @@
         )
 
 
 # Solve data
 
 
 @dataclasses.dataclass
-class InputData:
+class SolveInputs:
     outline: Outline
-    raw_parameters: List[Any]
-    raw_dimensions: Optional[List[Any]]
+    raw_parameters: list[Any]
+    raw_dimensions: Optional[list[Any]]
 
     def parameter(self, label: Label) -> pd.Series:
         for param in self.raw_parameters:
             if param["label"] == label:
                 entries = param["entries"]
                 outline = self.outline.parameters[label]
                 return pd.Series(
-                    data=(e["value"] for e in entries),
+                    data=(decode_extended_float(e["value"]) for e in entries),
                     index=_entry_index(entries, outline.bindings),
                 )
         raise Exception(f"Unknown parameter: {label}")
 
-    def dimension(self, label: Label) -> pd.Series:
+    def dimension(self, label: Label) -> pd.Index:
         for dim in self.raw_dimensions or []:
             if dim["label"] == label:
                 return pd.Index(dim["items"])
         raise Exception(f"Unknown dimension: {label}")
 
 
-@dataclasses.dataclass
-class OutputData:
+@dataclasses.dataclass(frozen=True)
+class SolveOutputs:
     outline: Outline
-    raw_variables: List[Any]
-    raw_constraints: List[Any]
+    raw_variables: list[Any]
+    raw_constraints: list[Any]
 
     @classmethod
     def from_json(cls, data, outline):
-        return OutputData(
+        return SolveOutputs(
             outline=outline,
             raw_variables=data["variables"],
             raw_constraints=data["constraints"],
         )
 
     def variable(self, label: Label) -> pd.DataFrame:
         for res in self.raw_variables:
             if res["label"] == label:
                 entries = res["entries"]
                 outline = self.outline.variables[label]
                 df = pd.DataFrame(
                     data=(
-                        {"value": e["value"], "dual_value": e.get("dualValue")}
+                        {
+                            "value": decode_extended_float(e["value"]),
+                            "dual_value": e.get("dualValue"),
+                        }
                         for e in entries
                     ),
                     index=_entry_index(entries, outline.bindings),
                 )
                 return df.dropna(axis=1, how="all").fillna(0)
         raise Exception(f"Unknown variable {label}")
 
     def constraint(self, label: Label) -> pd.DataFrame:
         for res in self.raw_constraints:
             if res["label"] == label:
                 entries = res["entries"]
                 outline = self.outline.constraints[label]
                 df = pd.DataFrame(
                     data=(
-                        {"slack": e["value"], "dual_value": e.get("dualValue")}
+                        {
+                            "slack": e["value"],
+                            "dual_value": e.get("dualValue"),
+                        }
                         for e in entries
                     ),
                     index=_entry_index(entries, outline.bindings),
                 )
                 return df.dropna(axis=1, how="all").fillna(0)
         raise Exception(f"Unknown constraint {label}")
 
 
+@dataclasses.dataclass(frozen=True)
+class SolveResponse:
+    status: str
+    outcome: Outcome
+    summary: Summary
+    outputs: Optional[SolveOutputs] = dataclasses.field(
+        default=None, repr=False
+    )
+
+
+# Attempt data
+
+
 def _entry_index(entries, bindings):
+    if not bindings:
+        return None
     if len(bindings) == 1:
         binding = bindings[0]
         return pd.Index(
             data=[e["key"][0] for e in entries],
             name=binding.qualifier or binding.dimension_label,
         )
     return pd.MultiIndex.from_tuples(
         tuples=[tuple(e["key"]) for e in entries],
         names=[b.qualifier or b.dimension_label for b in bindings],
     )
 
 
 @dataclasses.dataclass
-class Inputs:
-    """Solve inputs"""
+class AttemptRequest:
+    """Attempt inputs"""
 
     formulation_name: str
     tag_name: str
-    data: InputData = dataclasses.field(repr=False)
-
-
-@dataclasses.dataclass
-class Outputs:
-    """Solve outputs"""
-
-    status: str
-    outcome: Outcome
-    summary: Summary
-    data: Optional[OutputData] = dataclasses.field(default=None, repr=False)
+    inputs: SolveInputs = dataclasses.field(repr=False)
 
 
 # Attempt options
 
 Penalty = str
 
 
 _DEFAULT_PENALTY = "TOTAL_DEVIATION"
 
 
 @dataclasses.dataclass
 class Relaxation:
-    penalty: Penalty
+    penalty: Penalty = _DEFAULT_PENALTY
     objective_weight: Optional[float] = None
-    constraints: Optional[List[ConstraintRelaxation]] = None
+    constraints: Optional[list[ConstraintRelaxation]] = None
 
     @classmethod
-    def from_constraint_labels(cls, labels: List[Label]) -> Relaxation:
+    def from_constraint_labels(
+        cls,
+        labels: list[Label],
+        penalty: Penalty = _DEFAULT_PENALTY,
+        objective_weight: Optional[float] = None,
+    ) -> Relaxation:
+        """Relaxes all input constraints using a common penalty."""
         return Relaxation(
-            penalty=_DEFAULT_PENALTY,
+            penalty=penalty,
+            objective_weight=objective_weight,
             constraints=[ConstraintRelaxation(label=n) for n in labels],
         )
 
     def to_json(self):
         return strip_nones(
             {
                 "penalty": self.penalty,
@@ -451,31 +507,58 @@
                 "deficitBound": None if self.bound is None else -self.bound,
                 "surplusBound": self.bound,
             }
         )
 
 
 @dataclasses.dataclass
+class SolveOptions:
+    relative_gap_threshold: Optional[float] = None
+    absolute_gap_threshold: Optional[float] = None
+    zero_value_threshold: Optional[float] = None
+    infinity_value_threshold: Optional[float] = None
+    timeout_millis: Optional[float] = None
+
+
+def solve_options_to_json(
+    options: Optional[SolveOptions] = None,
+    relaxation: Optional[Relaxation] = None,
+):
+    if not options:
+        options = SolveOptions()
+    return strip_nones(
+        {
+            "absoluteGapThreshold": options.absolute_gap_threshold,
+            "relativeGapThreshold": options.relative_gap_threshold,
+            "timeoutMillis": options.timeout_millis,
+            "zeroValueThreshold": options.zero_value_threshold,
+            "infinityValueThreshold": options.infinity_value_threshold,
+            "relaxation": relaxation.to_json() if relaxation else None,
+        }
+    )
+
+
+@dataclasses.dataclass(frozen=True)
 class Attempt:
     uuid: str
     started_at: datetime
-    outline: Outline
-    url: str
+    url: str = dataclasses.field(repr=False)
+    outline: Outline = dataclasses.field(repr=False)
 
     @classmethod
     def from_graphql(cls, data: Any, outline: Outline, url: str):
         return Attempt(
             uuid=data["uuid"],
             started_at=datetime.fromisoformat(data["startedAt"]),
             outline=outline,
             url=url,
         )
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class Notification:
     dequeued: bool
     relative_gap: Optional[Value]
     lp_iteration_count: Optional[int]
     cut_count: Optional[int]
 
     @classmethod
```

### Comparing `opvious-0.8.1/opvious/executors/__init__.py` & `opvious-0.9.3/opvious/executors/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,23 +16,32 @@
   specific language governing permissions and limitations
   under the License.
 """
 
 import sys
 from typing import Optional
 
-from .common import ApiError, Executor, ExecutorResult, execute_graphql_query
+from .common import (
+    ApiError,
+    Executor,
+    ExecutorResult,
+    JsonExecutorResult,
+    JsonSeqExecutorResult,
+    PlainTextExecutorResult,
+)
 
 
 __all__ = [
     "default_executor",
     "ApiError",
     "Executor",
     "ExecutorResult",
-    "execute_graphql_query",
+    "JsonExecutorResult",
+    "JsonSeqExecutorResult",
+    "PlainTextExecutorResult",
 ]
 
 
 def _is_using_pyodide():
     # https://pyodide.org/en/stable/usage/faq.html#how-to-detect-that-code-is-run-with-pyodide
     return "pyodide" in sys.modules
 
@@ -40,18 +49,19 @@
 def default_executor(
     api_url: str, authorization: Optional[str] = None
 ) -> Executor:
     """Infers the best executor for the current environment"""
     if _is_using_pyodide():
         from .pyodide import PyodideExecutor
 
-        Executor = PyodideExecutor
+        return PyodideExecutor(api_url=api_url, authorization=authorization)
     else:
         try:
             from .aiohttp import AiohttpExecutor
         except ImportError:
             from .urllib import UrllibExecutor
 
-            Executor = UrllibExecutor
+            return UrllibExecutor(api_url=api_url, authorization=authorization)
         else:
-            Executor = AiohttpExecutor
-    return Executor(api_url=api_url, authorization=authorization)
+            return AiohttpExecutor(
+                api_url=api_url, authorization=authorization
+            )
```

### Comparing `opvious-0.8.1/opvious/executors/__pycache__/__init__.cpython-310.pyc` & `opvious-0.9.3/opvious/executors/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Mar 22 01:10:25 2023 UTC, .py size: 1745 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,113 +1,118 @@
-00000000: 6f0d 0d0a 0000 0000 8155 1a64 d106 0000  o........U.d....
+00000000: 6f0d 0d0a 0000 0000 915e 3064 ae07 0000  o........^0d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
+00000020: 0007 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6404 6405 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6700  m.Z.m.Z.m.Z...g.
-00000060: 6406 a201 5a09 6407 6408 8400 5a0a 0902  d...Z.d.d...Z...
-00000070: 640e 6409 650b 640a 6503 650b 1900 640b  d.d.e.d.e.e...d.
-00000080: 6506 6606 640c 640d 8405 5a0c 6402 5300  e.f.d.d...Z.d.S.
-00000090: 290f 6100 0300 000a 4c69 6365 6e73 6564  ).a.....Licensed
-000000a0: 2074 6f20 7468 6520 4170 6163 6865 2053   to the Apache S
-000000b0: 6f66 7477 6172 6520 466f 756e 6461 7469  oftware Foundati
-000000c0: 6f6e 2028 4153 4629 2075 6e64 6572 206f  on (ASF) under o
-000000d0: 6e65 0a6f 7220 6d6f 7265 2063 6f6e 7472  ne.or more contr
-000000e0: 6962 7574 6f72 206c 6963 656e 7365 2061  ibutor license a
-000000f0: 6772 6565 6d65 6e74 732e 2020 5365 6520  greements.  See 
-00000100: 7468 6520 4e4f 5449 4345 2066 696c 650a  the NOTICE file.
-00000110: 6469 7374 7269 6275 7465 6420 7769 7468  distributed with
-00000120: 2074 6869 7320 776f 726b 2066 6f72 2061   this work for a
-00000130: 6464 6974 696f 6e61 6c20 696e 666f 726d  dditional inform
-00000140: 6174 696f 6e0a 7265 6761 7264 696e 6720  ation.regarding 
-00000150: 636f 7079 7269 6768 7420 6f77 6e65 7273  copyright owners
-00000160: 6869 702e 2020 5468 6520 4153 4620 6c69  hip.  The ASF li
-00000170: 6365 6e73 6573 2074 6869 7320 6669 6c65  censes this file
-00000180: 0a74 6f20 796f 7520 756e 6465 7220 7468  .to you under th
-00000190: 6520 4170 6163 6865 204c 6963 656e 7365  e Apache License
-000001a0: 2c20 5665 7273 696f 6e20 322e 3020 2874  , Version 2.0 (t
-000001b0: 6865 0a22 4c69 6365 6e73 6522 293b 2079  he."License"); y
-000001c0: 6f75 206d 6179 206e 6f74 2075 7365 2074  ou may not use t
-000001d0: 6869 7320 6669 6c65 2065 7863 6570 7420  his file except 
-000001e0: 696e 2063 6f6d 706c 6961 6e63 650a 7769  in compliance.wi
-000001f0: 7468 2074 6865 204c 6963 656e 7365 2e20  th the License. 
-00000200: 2059 6f75 206d 6179 206f 6274 6169 6e20   You may obtain 
-00000210: 6120 636f 7079 206f 6620 7468 6520 4c69  a copy of the Li
-00000220: 6365 6e73 6520 6174 0a0a 2020 6874 7470  cense at..  http
-00000230: 3a2f 2f77 7777 2e61 7061 6368 652e 6f72  ://www.apache.or
-00000240: 672f 6c69 6365 6e73 6573 2f4c 4943 454e  g/licenses/LICEN
-00000250: 5345 2d32 2e30 0a0a 2020 556e 6c65 7373  SE-2.0..  Unless
-00000260: 2072 6571 7569 7265 6420 6279 2061 7070   required by app
-00000270: 6c69 6361 626c 6520 6c61 7720 6f72 2061  licable law or a
-00000280: 6772 6565 6420 746f 2069 6e20 7772 6974  greed to in writ
-00000290: 696e 672c 0a20 2073 6f66 7477 6172 6520  ing,.  software 
-000002a0: 6469 7374 7269 6275 7465 6420 756e 6465  distributed unde
-000002b0: 7220 7468 6520 4c69 6365 6e73 6520 6973  r the License is
-000002c0: 2064 6973 7472 6962 7574 6564 206f 6e20   distributed on 
-000002d0: 616e 0a20 2022 4153 2049 5322 2042 4153  an.  "AS IS" BAS
-000002e0: 4953 2c20 5749 5448 4f55 5420 5741 5252  IS, WITHOUT WARR
-000002f0: 414e 5449 4553 204f 5220 434f 4e44 4954  ANTIES OR CONDIT
-00000300: 494f 4e53 204f 4620 414e 590a 2020 4b49  IONS OF ANY.  KI
-00000310: 4e44 2c20 6569 7468 6572 2065 7870 7265  ND, either expre
-00000320: 7373 206f 7220 696d 706c 6965 642e 2020  ss or implied.  
-00000330: 5365 6520 7468 6520 4c69 6365 6e73 6520  See the License 
-00000340: 666f 7220 7468 650a 2020 7370 6563 6966  for the.  specif
-00000350: 6963 206c 616e 6775 6167 6520 676f 7665  ic language gove
-00000360: 726e 696e 6720 7065 726d 6973 7369 6f6e  rning permission
-00000370: 7320 616e 6420 6c69 6d69 7461 7469 6f6e  s and limitation
-00000380: 730a 2020 756e 6465 7220 7468 6520 4c69  s.  under the Li
-00000390: 6365 6e73 652e 0ae9 0000 0000 4e29 01da  cense.......N)..
-000003a0: 084f 7074 696f 6e61 6ce9 0100 0000 2904  .Optional.....).
-000003b0: da08 4170 6945 7272 6f72 da08 4578 6563  ..ApiError..Exec
-000003c0: 7574 6f72 da0e 4578 6563 7574 6f72 5265  utor..ExecutorRe
-000003d0: 7375 6c74 da15 6578 6563 7574 655f 6772  sult..execute_gr
-000003e0: 6170 6871 6c5f 7175 6572 7929 05da 1064  aphql_query)...d
-000003f0: 6566 6175 6c74 5f65 7865 6375 746f 7272  efault_executorr
-00000400: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
-00000410: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000420: 0000 0000 0200 0000 4300 0000 730a 0000  ........C...s...
-00000430: 0064 0174 006a 0176 0053 0029 024e da07  .d.t.j.v.S.).N..
-00000440: 7079 6f64 6964 6529 02da 0373 7973 da07  pyodide)...sys..
-00000450: 6d6f 6475 6c65 73a9 0072 0c00 0000 720c  modules..r....r.
-00000460: 0000 00fa 3d2f 686f 6d65 2f72 756e 6e65  ....=/home/runne
-00000470: 722f 776f 726b 2f73 646b 2e70 792f 7364  r/work/sdk.py/sd
-00000480: 6b2e 7079 2f6f 7076 696f 7573 2f65 7865  k.py/opvious/exe
-00000490: 6375 746f 7273 2f5f 5f69 6e69 745f 5f2e  cutors/__init__.
-000004a0: 7079 da11 5f69 735f 7573 696e 675f 7079  py.._is_using_py
-000004b0: 6f64 6964 6523 0000 0073 0200 0000 0a02  odide#...s......
-000004c0: 720e 0000 00da 0761 7069 5f75 726c da0d  r......api_url..
-000004d0: 6175 7468 6f72 697a 6174 696f 6eda 0672  authorization..r
-000004e0: 6574 7572 6e63 0200 0000 0000 0000 0000  eturnc..........
-000004f0: 0000 0600 0000 0800 0000 4300 0000 735c  ..........C...s\
-00000500: 0000 0074 0083 0072 0c64 0164 026c 016d  ...t...r.d.d.l.m
-00000510: 027d 0201 007c 027d 036e 1c7a 0864 0164  .}...|.}.n.z.d.d
-00000520: 036c 036d 047d 0401 0057 006e 1104 0074  .l.m.}...W.n...t
-00000530: 0579 2501 0001 0001 0064 0164 046c 066d  .y%......d.d.l.m
-00000540: 077d 0501 007c 057d 0359 006e 0377 007c  .}...|.}.Y.n.w.|
-00000550: 047d 037c 037c 007c 0164 058d 0253 0029  .}.|.|.|.d...S.)
-00000560: 067a 3449 6e66 6572 7320 7468 6520 6265  .z4Infers the be
-00000570: 7374 2065 7865 6375 746f 7220 666f 7220  st executor for 
-00000580: 7468 6520 6375 7272 656e 7420 656e 7669  the current envi
-00000590: 726f 6e6d 656e 7472 0300 0000 2901 da0f  ronmentr....)...
-000005a0: 5079 6f64 6964 6545 7865 6375 746f 7229  PyodideExecutor)
-000005b0: 01da 0f41 696f 6874 7470 4578 6563 7574  ...AiohttpExecut
-000005c0: 6f72 2901 da0e 5572 6c6c 6962 4578 6563  or)...UrllibExec
-000005d0: 7574 6f72 2902 720f 0000 0072 1000 0000  utor).r....r....
-000005e0: 2908 720e 0000 0072 0900 0000 7212 0000  ).r....r....r...
-000005f0: 005a 0761 696f 6874 7470 7213 0000 00da  .Z.aiohttpr.....
-00000600: 0b49 6d70 6f72 7445 7272 6f72 da06 7572  .ImportError..ur
-00000610: 6c6c 6962 7214 0000 0029 0672 0f00 0000  llibr....).r....
-00000620: 7210 0000 0072 1200 0000 7205 0000 0072  r....r....r....r
-00000630: 1300 0000 7214 0000 0072 0c00 0000 720c  ....r....r....r.
-00000640: 0000 0072 0d00 0000 7208 0000 0028 0000  ...r....r....(..
-00000650: 0073 1600 0000 0604 0c01 0602 0202 1001  .s..............
-00000660: 0c01 0c01 0802 02fd 0405 0c01 7208 0000  ............r...
-00000670: 0029 014e 290d da07 5f5f 646f 635f 5f72  .).N)...__doc__r
-00000680: 0a00 0000 da06 7479 7069 6e67 7202 0000  ......typingr...
-00000690: 00da 0663 6f6d 6d6f 6e72 0400 0000 7205  ...commonr....r.
-000006a0: 0000 0072 0600 0000 7207 0000 00da 075f  ...r....r......_
-000006b0: 5f61 6c6c 5f5f 720e 0000 00da 0373 7472  _all__r......str
-000006c0: 7208 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
-000006d0: 0c00 0000 720d 0000 00da 083c 6d6f 6475  ....r......<modu
-000006e0: 6c65 3e01 0000 0073 1c00 0000 0400 0813  le>....s........
-000006f0: 0c01 1802 0803 0809 0206 04ff 0201 02ff  ................
-00000700: 0601 02ff 0202 0efe                      ........
+00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
+00000060: 6d0a 5a0a 0100 6700 6406 a201 5a0b 6407  m.Z...g.d...Z.d.
+00000070: 6408 8400 5a0c 0902 640e 6409 650d 640a  d...Z...d.d.e.d.
+00000080: 6503 650d 1900 640b 6506 6606 640c 640d  e.e...d.e.f.d.d.
+00000090: 8405 5a0e 6402 5300 290f 6100 0300 000a  ..Z.d.S.).a.....
+000000a0: 4c69 6365 6e73 6564 2074 6f20 7468 6520  Licensed to the 
+000000b0: 4170 6163 6865 2053 6f66 7477 6172 6520  Apache Software 
+000000c0: 466f 756e 6461 7469 6f6e 2028 4153 4629  Foundation (ASF)
+000000d0: 2075 6e64 6572 206f 6e65 0a6f 7220 6d6f   under one.or mo
+000000e0: 7265 2063 6f6e 7472 6962 7574 6f72 206c  re contributor l
+000000f0: 6963 656e 7365 2061 6772 6565 6d65 6e74  icense agreement
+00000100: 732e 2020 5365 6520 7468 6520 4e4f 5449  s.  See the NOTI
+00000110: 4345 2066 696c 650a 6469 7374 7269 6275  CE file.distribu
+00000120: 7465 6420 7769 7468 2074 6869 7320 776f  ted with this wo
+00000130: 726b 2066 6f72 2061 6464 6974 696f 6e61  rk for additiona
+00000140: 6c20 696e 666f 726d 6174 696f 6e0a 7265  l information.re
+00000150: 6761 7264 696e 6720 636f 7079 7269 6768  garding copyrigh
+00000160: 7420 6f77 6e65 7273 6869 702e 2020 5468  t ownership.  Th
+00000170: 6520 4153 4620 6c69 6365 6e73 6573 2074  e ASF licenses t
+00000180: 6869 7320 6669 6c65 0a74 6f20 796f 7520  his file.to you 
+00000190: 756e 6465 7220 7468 6520 4170 6163 6865  under the Apache
+000001a0: 204c 6963 656e 7365 2c20 5665 7273 696f   License, Versio
+000001b0: 6e20 322e 3020 2874 6865 0a22 4c69 6365  n 2.0 (the."Lice
+000001c0: 6e73 6522 293b 2079 6f75 206d 6179 206e  nse"); you may n
+000001d0: 6f74 2075 7365 2074 6869 7320 6669 6c65  ot use this file
+000001e0: 2065 7863 6570 7420 696e 2063 6f6d 706c   except in compl
+000001f0: 6961 6e63 650a 7769 7468 2074 6865 204c  iance.with the L
+00000200: 6963 656e 7365 2e20 2059 6f75 206d 6179  icense.  You may
+00000210: 206f 6274 6169 6e20 6120 636f 7079 206f   obtain a copy o
+00000220: 6620 7468 6520 4c69 6365 6e73 6520 6174  f the License at
+00000230: 0a0a 2020 6874 7470 3a2f 2f77 7777 2e61  ..  http://www.a
+00000240: 7061 6368 652e 6f72 672f 6c69 6365 6e73  pache.org/licens
+00000250: 6573 2f4c 4943 454e 5345 2d32 2e30 0a0a  es/LICENSE-2.0..
+00000260: 2020 556e 6c65 7373 2072 6571 7569 7265    Unless require
+00000270: 6420 6279 2061 7070 6c69 6361 626c 6520  d by applicable 
+00000280: 6c61 7720 6f72 2061 6772 6565 6420 746f  law or agreed to
+00000290: 2069 6e20 7772 6974 696e 672c 0a20 2073   in writing,.  s
+000002a0: 6f66 7477 6172 6520 6469 7374 7269 6275  oftware distribu
+000002b0: 7465 6420 756e 6465 7220 7468 6520 4c69  ted under the Li
+000002c0: 6365 6e73 6520 6973 2064 6973 7472 6962  cense is distrib
+000002d0: 7574 6564 206f 6e20 616e 0a20 2022 4153  uted on an.  "AS
+000002e0: 2049 5322 2042 4153 4953 2c20 5749 5448   IS" BASIS, WITH
+000002f0: 4f55 5420 5741 5252 414e 5449 4553 204f  OUT WARRANTIES O
+00000300: 5220 434f 4e44 4954 494f 4e53 204f 4620  R CONDITIONS OF 
+00000310: 414e 590a 2020 4b49 4e44 2c20 6569 7468  ANY.  KIND, eith
+00000320: 6572 2065 7870 7265 7373 206f 7220 696d  er express or im
+00000330: 706c 6965 642e 2020 5365 6520 7468 6520  plied.  See the 
+00000340: 4c69 6365 6e73 6520 666f 7220 7468 650a  License for the.
+00000350: 2020 7370 6563 6966 6963 206c 616e 6775    specific langu
+00000360: 6167 6520 676f 7665 726e 696e 6720 7065  age governing pe
+00000370: 726d 6973 7369 6f6e 7320 616e 6420 6c69  rmissions and li
+00000380: 6d69 7461 7469 6f6e 730a 2020 756e 6465  mitations.  unde
+00000390: 7220 7468 6520 4c69 6365 6e73 652e 0ae9  r the License...
+000003a0: 0000 0000 4e29 01da 084f 7074 696f 6e61  ....N)...Optiona
+000003b0: 6ce9 0100 0000 2906 da08 4170 6945 7272  l.....)...ApiErr
+000003c0: 6f72 da08 4578 6563 7574 6f72 da0e 4578  or..Executor..Ex
+000003d0: 6563 7574 6f72 5265 7375 6c74 da12 4a73  ecutorResult..Js
+000003e0: 6f6e 4578 6563 7574 6f72 5265 7375 6c74  onExecutorResult
+000003f0: da15 4a73 6f6e 5365 7145 7865 6375 746f  ..JsonSeqExecuto
+00000400: 7252 6573 756c 74da 1750 6c61 696e 5465  rResult..PlainTe
+00000410: 7874 4578 6563 7574 6f72 5265 7375 6c74  xtExecutorResult
+00000420: 2907 da10 6465 6661 756c 745f 6578 6563  )...default_exec
+00000430: 7574 6f72 7204 0000 0072 0500 0000 7206  utorr....r....r.
+00000440: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
+00000450: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000460: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
+00000470: 6401 7400 6a01 7600 5300 2902 4eda 0770  d.t.j.v.S.).N..p
+00000480: 796f 6469 6465 2902 da03 7379 73da 076d  yodide)...sys..m
+00000490: 6f64 756c 6573 a900 720e 0000 0072 0e00  odules..r....r..
+000004a0: 0000 fa3d 2f68 6f6d 652f 7275 6e6e 6572  ...=/home/runner
+000004b0: 2f77 6f72 6b2f 7364 6b2e 7079 2f73 646b  /work/sdk.py/sdk
+000004c0: 2e70 792f 6f70 7669 6f75 732f 6578 6563  .py/opvious/exec
+000004d0: 7574 6f72 732f 5f5f 696e 6974 5f5f 2e70  utors/__init__.p
+000004e0: 79da 115f 6973 5f75 7369 6e67 5f70 796f  y.._is_using_pyo
+000004f0: 6469 6465 2c00 0000 7302 0000 000a 0272  dide,...s......r
+00000500: 1000 0000 da07 6170 695f 7572 6cda 0d61  ......api_url..a
+00000510: 7574 686f 7269 7a61 7469 6f6e da06 7265  uthorization..re
+00000520: 7475 726e 6302 0000 0000 0000 0000 0000  turnc...........
+00000530: 0005 0000 0008 0000 0043 0000 0073 6600  .........C...sf.
+00000540: 0000 7400 8300 720f 6401 6402 6c01 6d02  ..t...r.d.d.l.m.
+00000550: 7d02 0100 7c02 7c00 7c01 6403 8d02 5300  }...|.|.|.d...S.
+00000560: 7a08 6401 6404 6c03 6d04 7d03 0100 5700  z.d.d.l.m.}...W.
+00000570: 6e15 0400 7405 792c 0100 0100 0100 6401  n...t.y,......d.
+00000580: 6405 6c06 6d07 7d04 0100 7c04 7c00 7c01  d.l.m.}...|.|.|.
+00000590: 6403 8d02 0600 5900 5300 7700 7c03 7c00  d.....Y.S.w.|.|.
+000005a0: 7c01 6403 8d02 5300 2906 7a34 496e 6665  |.d...S.).z4Infe
+000005b0: 7273 2074 6865 2062 6573 7420 6578 6563  rs the best exec
+000005c0: 7574 6f72 2066 6f72 2074 6865 2063 7572  utor for the cur
+000005d0: 7265 6e74 2065 6e76 6972 6f6e 6d65 6e74  rent environment
+000005e0: 7203 0000 0029 01da 0f50 796f 6469 6465  r....)...Pyodide
+000005f0: 4578 6563 7574 6f72 2902 7211 0000 0072  Executor).r....r
+00000600: 1200 0000 2901 da0f 4169 6f68 7474 7045  ....)...AiohttpE
+00000610: 7865 6375 746f 7229 01da 0e55 726c 6c69  xecutor)...Urlli
+00000620: 6245 7865 6375 746f 7229 0872 1000 0000  bExecutor).r....
+00000630: 720b 0000 0072 1400 0000 5a07 6169 6f68  r....r....Z.aioh
+00000640: 7474 7072 1500 0000 da0b 496d 706f 7274  ttpr......Import
+00000650: 4572 726f 72da 0675 726c 6c69 6272 1600  Error..urllibr..
+00000660: 0000 2905 7211 0000 0072 1200 0000 7214  ..).r....r....r.
+00000670: 0000 0072 1500 0000 7216 0000 0072 0e00  ...r....r....r..
+00000680: 0000 720e 0000 0072 0f00 0000 720a 0000  ..r....r....r...
+00000690: 0031 0000 0073 1800 0000 0604 0c01 0c02  .1...s..........
+000006a0: 0202 1001 0c01 0c01 1002 02fd 0205 0401  ................
+000006b0: 06ff 720a 0000 0029 014e 290f da07 5f5f  ..r....).N)...__
+000006c0: 646f 635f 5f72 0c00 0000 da06 7479 7069  doc__r......typi
+000006d0: 6e67 7202 0000 00da 0663 6f6d 6d6f 6e72  ngr......commonr
+000006e0: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
+000006f0: 0000 0072 0800 0000 7209 0000 00da 075f  ...r....r......_
+00000700: 5f61 6c6c 5f5f 7210 0000 00da 0373 7472  _all__r......str
+00000710: 720a 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+00000720: 0e00 0000 720f 0000 00da 083c 6d6f 6475  ....r......<modu
+00000730: 6c65 3e01 0000 0073 1c00 0000 0400 0813  le>....s........
+00000740: 0c01 2002 080a 080b 0206 04ff 0201 02ff  .. .............
+00000750: 0601 02ff 0202 0efe                      ........
```

### Comparing `opvious-0.8.1/opvious/executors/__pycache__/urllib.cpython-310.pyc` & `opvious-0.9.3/opvious/executors/__pycache__/urllib.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Mar 22 01:10:25 2023 UTC, .py size: 3522 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,219 +1,173 @@
-00000000: 6f0d 0d0a 0000 0000 8155 1a64 c20d 0000  o........U.d....
+00000000: 6f0d 0d0a 0000 0000 915e 3064 7d0a 0000  o........^0d}...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000b 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
-00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
-00000050: 5a05 6401 6402 6c06 5a05 6401 6402 6c07  Z.d.d.l.Z.d.d.l.
-00000060: 5a05 6401 6403 6c08 6d09 5a09 6d0a 5a0a  Z.d.d.l.m.Z.m.Z.
-00000070: 0100 6404 6405 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
-00000080: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
-00000090: 6d12 5a12 6d13 5a13 6d14 5a14 0100 6503  m.Z.m.Z.m.Z...e.
-000000a0: a015 6516 a101 5a17 4700 6406 6407 8400  ..e...Z.G.d.d...
-000000b0: 6407 8302 5a18 6501 6a19 6408 651a 6409  d...Z.e.j.d.e.d.
-000000c0: 651a 640a 650e 640b 6509 640c 650f 660a  e.d.e.d.e.d.e.f.
-000000d0: 640d 640e 8404 8301 5a1b 6402 5300 290f  d.d.....Z.d.S.).
-000000e0: 6100 0300 000a 4c69 6365 6e73 6564 2074  a.....Licensed t
-000000f0: 6f20 7468 6520 4170 6163 6865 2053 6f66  o the Apache Sof
-00000100: 7477 6172 6520 466f 756e 6461 7469 6f6e  tware Foundation
-00000110: 2028 4153 4629 2075 6e64 6572 206f 6e65   (ASF) under one
-00000120: 0a6f 7220 6d6f 7265 2063 6f6e 7472 6962  .or more contrib
-00000130: 7574 6f72 206c 6963 656e 7365 2061 6772  utor license agr
-00000140: 6565 6d65 6e74 732e 2020 5365 6520 7468  eements.  See th
-00000150: 6520 4e4f 5449 4345 2066 696c 650a 6469  e NOTICE file.di
-00000160: 7374 7269 6275 7465 6420 7769 7468 2074  stributed with t
-00000170: 6869 7320 776f 726b 2066 6f72 2061 6464  his work for add
-00000180: 6974 696f 6e61 6c20 696e 666f 726d 6174  itional informat
-00000190: 696f 6e0a 7265 6761 7264 696e 6720 636f  ion.regarding co
-000001a0: 7079 7269 6768 7420 6f77 6e65 7273 6869  pyright ownershi
-000001b0: 702e 2020 5468 6520 4153 4620 6c69 6365  p.  The ASF lice
-000001c0: 6e73 6573 2074 6869 7320 6669 6c65 0a74  nses this file.t
-000001d0: 6f20 796f 7520 756e 6465 7220 7468 6520  o you under the 
-000001e0: 4170 6163 6865 204c 6963 656e 7365 2c20  Apache License, 
-000001f0: 5665 7273 696f 6e20 322e 3020 2874 6865  Version 2.0 (the
-00000200: 0a22 4c69 6365 6e73 6522 293b 2079 6f75  ."License"); you
-00000210: 206d 6179 206e 6f74 2075 7365 2074 6869   may not use thi
-00000220: 7320 6669 6c65 2065 7863 6570 7420 696e  s file except in
-00000230: 2063 6f6d 706c 6961 6e63 650a 7769 7468   compliance.with
-00000240: 2074 6865 204c 6963 656e 7365 2e20 2059   the License.  Y
-00000250: 6f75 206d 6179 206f 6274 6169 6e20 6120  ou may obtain a 
-00000260: 636f 7079 206f 6620 7468 6520 4c69 6365  copy of the Lice
-00000270: 6e73 6520 6174 0a0a 2020 6874 7470 3a2f  nse at..  http:/
-00000280: 2f77 7777 2e61 7061 6368 652e 6f72 672f  /www.apache.org/
-00000290: 6c69 6365 6e73 6573 2f4c 4943 454e 5345  licenses/LICENSE
-000002a0: 2d32 2e30 0a0a 2020 556e 6c65 7373 2072  -2.0..  Unless r
-000002b0: 6571 7569 7265 6420 6279 2061 7070 6c69  equired by appli
-000002c0: 6361 626c 6520 6c61 7720 6f72 2061 6772  cable law or agr
-000002d0: 6565 6420 746f 2069 6e20 7772 6974 696e  eed to in writin
-000002e0: 672c 0a20 2073 6f66 7477 6172 6520 6469  g,.  software di
-000002f0: 7374 7269 6275 7465 6420 756e 6465 7220  stributed under 
-00000300: 7468 6520 4c69 6365 6e73 6520 6973 2064  the License is d
-00000310: 6973 7472 6962 7574 6564 206f 6e20 616e  istributed on an
-00000320: 0a20 2022 4153 2049 5322 2042 4153 4953  .  "AS IS" BASIS
-00000330: 2c20 5749 5448 4f55 5420 5741 5252 414e  , WITHOUT WARRAN
-00000340: 5449 4553 204f 5220 434f 4e44 4954 494f  TIES OR CONDITIO
-00000350: 4e53 204f 4620 414e 590a 2020 4b49 4e44  NS OF ANY.  KIND
-00000360: 2c20 6569 7468 6572 2065 7870 7265 7373  , either express
-00000370: 206f 7220 696d 706c 6965 642e 2020 5365   or implied.  Se
-00000380: 6520 7468 6520 4c69 6365 6e73 6520 666f  e the License fo
-00000390: 7220 7468 650a 2020 7370 6563 6966 6963  r the.  specific
-000003a0: 206c 616e 6775 6167 6520 676f 7665 726e   language govern
-000003b0: 696e 6720 7065 726d 6973 7369 6f6e 7320  ing permissions 
-000003c0: 616e 6420 6c69 6d69 7461 7469 6f6e 730a  and limitations.
-000003d0: 2020 756e 6465 7220 7468 6520 4c69 6365    under the Lice
-000003e0: 6e73 652e 0ae9 0000 0000 4e29 02da 0341  nse.......N)...A
-000003f0: 6e79 da08 4f70 7469 6f6e 616c e901 0000  ny..Optional....
-00000400: 0029 09da 1343 4f4e 5445 4e54 5f54 5950  .)...CONTENT_TYP
-00000410: 455f 4845 4144 4552 da0f 6465 6661 756c  E_HEADER..defaul
-00000420: 745f 6865 6164 6572 73da 0748 6561 6465  t_headers..Heade
-00000430: 7273 da09 4578 6563 7574 696f 6eda 124a  rs..Execution..J
-00000440: 736f 6e45 7865 6375 746f 7252 6573 756c  sonExecutorResul
-00000450: 74da 154a 736f 6e53 6571 4578 6563 7574  t..JsonSeqExecut
-00000460: 6f72 5265 7375 6c74 da0c 5452 4143 455f  orResult..TRACE_
-00000470: 4845 4144 4552 da19 756e 6578 7065 6374  HEADER..unexpect
-00000480: 6564 5f72 6573 706f 6e73 655f 6572 726f  ed_response_erro
-00000490: 72da 1e75 6e73 7570 706f 7274 6564 5f63  r..unsupported_c
-000004a0: 6f6e 7465 6e74 5f74 7970 655f 6572 726f  ontent_type_erro
-000004b0: 7263 0000 0000 0000 0000 0000 0000 0000  rc..............
-000004c0: 0000 0b00 0000 4000 0000 7356 0000 0065  ......@...sV...e
-000004d0: 005a 0164 005a 0264 015a 0364 0f64 0365  .Z.d.Z.d.Z.d.d.e
-000004e0: 0464 0465 0565 0419 0066 0464 0564 0684  .d.e.e...f.d.d..
-000004f0: 055a 0609 0709 0209 0264 1064 0865 0464  .Z.......d.d.e.d
-00000500: 0965 0464 0a65 0565 0719 0064 0b65 0565  .e.d.e.e...d.e.e
-00000510: 0819 0064 0c65 0966 0a64 0d64 0e84 055a  ...d.e.f.d.d...Z
-00000520: 0a64 0253 0029 11da 0e55 726c 6c69 6245  .d.S.)...UrllibE
-00000530: 7865 6375 746f 727a 780a 2020 2020 6075  xecutorzx.    `u
-00000540: 726c 6c69 6260 2d70 6f77 6572 6564 2047  rllib`-powered G
-00000550: 7261 7068 514c 2065 7865 6375 746f 722c  raphQL executor,
-00000560: 2075 7365 6420 6173 2066 616c 6c62 6163   used as fallbac
-00000570: 6b2e 2057 6865 6e20 706f 7373 6962 6c65  k. When possible
-00000580: 2c20 7072 6566 6572 0a20 2020 2075 7369  , prefer.    usi
-00000590: 6e67 2074 6865 2060 6169 6f68 7474 7060  ng the `aiohttp`
-000005a0: 2065 7175 6976 616c 656e 742e 0a20 2020   equivalent..   
-000005b0: 204e da07 6170 695f 7572 6cda 0d61 7574   N..api_url..aut
-000005c0: 686f 7269 7a61 7469 6f6e 6303 0000 0000  horizationc.....
-000005d0: 0000 0000 0000 0003 0000 0005 0000 0043  ...............C
-000005e0: 0000 0073 3400 0000 7c01 7c00 5f00 7401  ...s4...|.|._.t.
-000005f0: 6401 8301 7c00 5f02 7c02 720f 7c02 7c00  d...|._.|.r.|.|.
-00000600: 6a02 6402 3c00 7403 a004 6403 7c00 6a05  j.d.<.t...d.|.j.
-00000610: 6a06 7c01 a103 0100 6400 5300 2904 4eda  j.|.....d.S.).N.
-00000620: 0675 726c 6c69 6272 1000 0000 7a28 496e  .urllibr....z(In
-00000630: 7374 616e 7469 6174 6564 2065 7865 6375  stantiated execu
-00000640: 746f 722e 205b 6e61 6d65 3d25 732c 2075  tor. [name=%s, u
-00000650: 726c 3d25 735d 2907 da08 5f61 7069 5f75  rl=%s])..._api_u
-00000660: 726c 7206 0000 00da 085f 6865 6164 6572  rlr......_header
-00000670: 73da 075f 6c6f 6767 6572 da05 6465 6275  s.._logger..debu
-00000680: 67da 095f 5f63 6c61 7373 5f5f da08 5f5f  g..__class__..__
-00000690: 6e61 6d65 5f5f 2903 da04 7365 6c66 720f  name__)...selfr.
-000006a0: 0000 0072 1000 0000 a900 7219 0000 00fa  ...r......r.....
-000006b0: 3b2f 686f 6d65 2f72 756e 6e65 722f 776f  ;/home/runner/wo
-000006c0: 726b 2f73 646b 2e70 792f 7364 6b2e 7079  rk/sdk.py/sdk.py
-000006d0: 2f6f 7076 696f 7573 2f65 7865 6375 746f  /opvious/executo
-000006e0: 7273 2f75 726c 6c69 622e 7079 da08 5f5f  rs/urllib.py..__
-000006f0: 696e 6974 5f5f 3200 0000 7312 0000 0006  init__2...s.....
-00000700: 010a 0104 010a 0104 0102 0106 0102 0108  ................
-00000710: fd7a 1755 726c 6c69 6245 7865 6375 746f  .z.UrllibExecuto
-00000720: 722e 5f5f 696e 6974 5f5f da03 4745 54da  r.__init__..GET.
-00000730: 0470 6174 68da 066d 6574 686f 64da 0768  .path..method..h
-00000740: 6561 6465 7273 da09 6a73 6f6e 5f62 6f64  eaders..json_bod
-00000750: 79da 0672 6574 7572 6e63 0500 0000 0000  y..returnc......
-00000760: 0000 0000 0000 0700 0000 0600 0000 4300  ..............C.
-00000770: 0000 7356 0000 007c 006a 00a0 01a1 007d  ..sV...|.j.....}
-00000780: 057c 0372 0c7c 05a0 027c 03a1 0101 007c  .|.r.|...|.....|
-00000790: 0472 1b64 017c 0564 023c 0074 03a0 047c  .r.d.|.d.<.t...|
-000007a0: 04a1 01a0 0564 03a1 017d 066e 0264 007d  .....d...}.n.d.}
-000007b0: 0674 0674 076a 08a0 097c 006a 0a7c 01a1  .t.t.j...|.j.|..
-000007c0: 027c 057c 027c 0664 048d 0453 0029 054e  .|.|.|.d...S.).N
-000007d0: 7a10 6170 706c 6963 6174 696f 6e2f 6a73  z.application/js
-000007e0: 6f6e 7a0c 636f 6e74 656e 742d 7479 7065  onz.content-type
-000007f0: da04 7574 6638 a904 da03 7572 6c72 1f00  ..utf8....urlr..
-00000800: 0000 721e 0000 00da 0464 6174 6129 0b72  ..r......data).r
-00000810: 1300 0000 da04 636f 7079 da06 7570 6461  ......copy..upda
-00000820: 7465 da04 6a73 6f6e da05 6475 6d70 73da  te..json..dumps.
-00000830: 0665 6e63 6f64 65da 0a5f 6578 6563 7574  .encode.._execut
-00000840: 696f 6e72 1100 0000 da05 7061 7273 65da  ionr......parse.
-00000850: 0775 726c 6a6f 696e 7212 0000 0029 0772  .urljoinr....).r
-00000860: 1800 0000 721d 0000 0072 1e00 0000 721f  ....r....r....r.
-00000870: 0000 0072 2000 0000 da0b 616c 6c5f 6865  ...r .....all_he
-00000880: 6164 6572 7372 2500 0000 7219 0000 0072  adersr%...r....r
-00000890: 1900 0000 721a 0000 00da 0765 7865 6375  ....r......execu
-000008a0: 7465 3d00 0000 731a 0000 000a 0704 010a  te=...s.........
-000008b0: 0104 0108 0112 0104 0202 010e 0102 0102  ................
-000008c0: 0102 0106 fc7a 1655 726c 6c69 6245 7865  .....z.UrllibExe
-000008d0: 6375 746f 722e 6578 6563 7574 6529 014e  cutor.execute).N
-000008e0: 2903 721c 0000 004e 4e29 0b72 1700 0000  ).r....NN).r....
-000008f0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000900: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
-00000910: 635f 5fda 0373 7472 7203 0000 0072 1b00  c__..strr....r..
-00000920: 0000 7207 0000 0072 0200 0000 7208 0000  ..r....r....r...
-00000930: 0072 2f00 0000 7219 0000 0072 1900 0000  .r/...r....r....
-00000940: 7219 0000 0072 1a00 0000 720e 0000 002c  r....r....r....,
-00000950: 0000 0073 2200 0000 0800 0401 1805 020e  ...s"...........
-00000960: 0201 0201 04fb 0202 02fe 0203 02fd 0604  ................
-00000970: 02fc 0605 02fb 0206 0efa 720e 0000 0072  ..........r....r
-00000980: 2400 0000 721e 0000 0072 1f00 0000 7225  $...r....r....r%
-00000990: 0000 0072 2100 0000 6304 0000 0000 0000  ...r!...c.......
-000009a0: 0000 0000 000b 0000 000a 0000 0043 0200  .............C..
-000009b0: 0073 0c01 0000 8102 7400 a001 6401 7c03  .s......t...d.|.
-000009c0: 720a 7402 7c03 8301 6e01 6402 a102 0100  r.t.|...n.d.....
-000009d0: 7403 6a04 6a05 7c00 7c02 7c01 7c03 6403  t.j.j.|.|.|.|.d.
-000009e0: 8d04 7d04 7a08 7403 6a04 a006 7c04 a101  ..}.z.t.j...|...
-000009f0: 7d05 5700 6e2e 0400 7403 6a07 6a08 7935  }.W.n...t.j.j.y5
-00000a00: 0100 7d06 0100 7a08 7c06 7d05 5700 5900  ..}...z.|.}.W.Y.
-00000a10: 6400 7d06 7e06 6e1d 6400 7d06 7e06 7701  d.}.~.n.d.}.~.w.
-00000a20: 0400 7409 794d 0100 7d06 0100 7a0d 7c06  ..t.yM..}...z.|.
-00000a30: 6a0a a00b 740c a101 7d07 740d 7c06 6a0e  j...t...}.t.|.j.
-00000a40: 7c07 6404 8d02 8201 6400 7d06 7e06 7701  |.d.....d.}.~.w.
-00000a50: 7700 7c05 6a0f 7d08 7c05 a010 740c a101  w.|.j.}.|...t...
-00000a60: 7d07 7c05 a010 7411 a101 7d09 7412 a013  }.|...t...}.t...
-00000a70: 7c09 a101 7271 7c05 a014 a100 a015 6405  |...rq|.......d.
-00000a80: a101 7d0a 7412 7c08 7c07 7c0a 6406 8d03  ..}.t.|.|.|.d...
-00000a90: 5600 0100 6400 5300 7416 a013 7c09 a101  V...d.S.t...|...
-00000aa0: 7280 7416 7c08 7c07 7c05 6407 8d03 5600  r.t.|.|.|.d...V.
-00000ab0: 0100 6400 5300 7417 7c09 7c07 6408 8d02  ..d.S.t.|.|.d...
-00000ac0: 8201 2909 4e7a 2053 656e 6469 6e67 2041  ..).Nz Sending A
-00000ad0: 5049 2072 6571 7565 7374 2e2e 2e20 5b73  PI request... [s
-00000ae0: 697a 653d 2573 5d72 0100 0000 7223 0000  ize=%s]r....r#..
-00000af0: 0029 02da 076d 6573 7361 6765 da05 7472  .)...message..tr
-00000b00: 6163 6572 2200 0000 2903 da06 7374 6174  acer"...)...stat
-00000b10: 7573 7235 0000 00da 0474 6578 7429 0372  usr5.....text).r
-00000b20: 3600 0000 7235 0000 00da 0672 6561 6465  6...r5.....reade
-00000b30: 7229 02da 0c63 6f6e 7465 6e74 5f74 7970  r)...content_typ
-00000b40: 6572 3500 0000 2918 7214 0000 0072 1500  er5...).r....r..
-00000b50: 0000 da03 6c65 6e72 1100 0000 da07 7265  ....lenr......re
-00000b60: 7175 6573 74da 0752 6571 7565 7374 da07  quest..Request..
-00000b70: 7572 6c6f 7065 6eda 0565 7272 6f72 da09  urlopen..error..
-00000b80: 4854 5450 4572 726f 72da 0945 7863 6570  HTTPError..Excep
-00000b90: 7469 6f6e 721f 0000 00da 0367 6574 720b  tionr......getr.
-00000ba0: 0000 0072 0c00 0000 da06 7265 6173 6f6e  ...r......reason
-00000bb0: 7236 0000 00da 0967 6574 6865 6164 6572  r6.....getheader
-00000bc0: 7205 0000 0072 0900 0000 da0b 6973 5f65  r....r......is_e
-00000bd0: 6c69 6769 626c 65da 0472 6561 64da 0664  ligible..read..d
-00000be0: 6563 6f64 6572 0a00 0000 720d 0000 0029  ecoder....r....)
-00000bf0: 0b72 2400 0000 721e 0000 0072 1f00 0000  .r$...r....r....
-00000c00: 7225 0000 00da 0372 6571 da03 7265 73da  r%.....req..res.
-00000c10: 0365 7272 7235 0000 0072 3600 0000 da05  .errr5...r6.....
-00000c20: 6374 7970 6572 3700 0000 7219 0000 0072  ctyper7...r....r
-00000c30: 1900 0000 721a 0000 0072 2b00 0000 5400  ....r....r+...T.
-00000c40: 0000 733c 0000 0002 8018 0406 0102 0102  ..s<............
-00000c50: 0102 0102 0106 fc02 0610 0112 0110 0108  ................
-00000c60: 800e 010c 010e 0108 8002 fe06 030a 010a  ................
-00000c70: 010a 010e 0114 010a 0114 0202 0202 0102  ................
-00000c80: 0106 fe72 2b00 0000 291c 7232 0000 00da  ...r+...).r2....
-00000c90: 0a63 6f6e 7465 7874 6c69 6272 2800 0000  .contextlibr(...
-00000ca0: da07 6c6f 6767 696e 67da 0c75 726c 6c69  ..logging..urlli
-00000cb0: 622e 6572 726f 7272 1100 0000 da0c 7572  b.errorr......ur
-00000cc0: 6c6c 6962 2e70 6172 7365 da0e 7572 6c6c  llib.parse..urll
-00000cd0: 6962 2e72 6571 7565 7374 da06 7479 7069  ib.request..typi
-00000ce0: 6e67 7202 0000 0072 0300 0000 da06 636f  ngr....r......co
-00000cf0: 6d6d 6f6e 7205 0000 0072 0600 0000 7207  mmonr....r....r.
-00000d00: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
-00000d10: 0000 720b 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-00000d20: 00da 0967 6574 4c6f 6767 6572 7217 0000  ...getLoggerr...
-00000d30: 0072 1400 0000 720e 0000 00da 1361 7379  .r....r......asy
-00000d40: 6e63 636f 6e74 6578 746d 616e 6167 6572  nccontextmanager
-00000d50: 7233 0000 0072 2b00 0000 7219 0000 0072  r3...r+...r....r
-00000d60: 1900 0000 7219 0000 0072 1a00 0000 da08  ....r....r......
-00000d70: 3c6d 6f64 756c 653e 0100 0000 732e 0000  <module>....s...
-00000d80: 0004 0008 1308 0108 0108 0108 0108 0110  ................
-00000d90: 012c 020a 0d0e 0304 2802 0102 0102 ff02  .,......(.......
-00000da0: 0102 ff02 0102 ff02 0102 ff02 0210 fe    ...............
+00000040: 5a02 6401 6402 6c03 5a04 6401 6402 6c05  Z.d.d.l.Z.d.d.l.
+00000050: 5a04 6401 6403 6c06 6d07 5a07 6d08 5a08  Z.d.d.l.m.Z.m.Z.
+00000060: 0100 6404 6405 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
+00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
+00000080: 6d10 5a10 6d11 5a11 6d12 5a12 0100 6502  m.Z.m.Z.m.Z...e.
+00000090: a013 6514 a101 5a15 4700 6406 6407 8400  ..e...Z.G.d.d...
+000000a0: 6407 650c 8303 5a16 6402 5300 2908 6100  d.e...Z.d.S.).a.
+000000b0: 0300 000a 4c69 6365 6e73 6564 2074 6f20  ....Licensed to 
+000000c0: 7468 6520 4170 6163 6865 2053 6f66 7477  the Apache Softw
+000000d0: 6172 6520 466f 756e 6461 7469 6f6e 2028  are Foundation (
+000000e0: 4153 4629 2075 6e64 6572 206f 6e65 0a6f  ASF) under one.o
+000000f0: 7220 6d6f 7265 2063 6f6e 7472 6962 7574  r more contribut
+00000100: 6f72 206c 6963 656e 7365 2061 6772 6565  or license agree
+00000110: 6d65 6e74 732e 2020 5365 6520 7468 6520  ments.  See the 
+00000120: 4e4f 5449 4345 2066 696c 650a 6469 7374  NOTICE file.dist
+00000130: 7269 6275 7465 6420 7769 7468 2074 6869  ributed with thi
+00000140: 7320 776f 726b 2066 6f72 2061 6464 6974  s work for addit
+00000150: 696f 6e61 6c20 696e 666f 726d 6174 696f  ional informatio
+00000160: 6e0a 7265 6761 7264 696e 6720 636f 7079  n.regarding copy
+00000170: 7269 6768 7420 6f77 6e65 7273 6869 702e  right ownership.
+00000180: 2020 5468 6520 4153 4620 6c69 6365 6e73    The ASF licens
+00000190: 6573 2074 6869 7320 6669 6c65 0a74 6f20  es this file.to 
+000001a0: 796f 7520 756e 6465 7220 7468 6520 4170  you under the Ap
+000001b0: 6163 6865 204c 6963 656e 7365 2c20 5665  ache License, Ve
+000001c0: 7273 696f 6e20 322e 3020 2874 6865 0a22  rsion 2.0 (the."
+000001d0: 4c69 6365 6e73 6522 293b 2079 6f75 206d  License"); you m
+000001e0: 6179 206e 6f74 2075 7365 2074 6869 7320  ay not use this 
+000001f0: 6669 6c65 2065 7863 6570 7420 696e 2063  file except in c
+00000200: 6f6d 706c 6961 6e63 650a 7769 7468 2074  ompliance.with t
+00000210: 6865 204c 6963 656e 7365 2e20 2059 6f75  he License.  You
+00000220: 206d 6179 206f 6274 6169 6e20 6120 636f   may obtain a co
+00000230: 7079 206f 6620 7468 6520 4c69 6365 6e73  py of the Licens
+00000240: 6520 6174 0a0a 2020 6874 7470 3a2f 2f77  e at..  http://w
+00000250: 7777 2e61 7061 6368 652e 6f72 672f 6c69  ww.apache.org/li
+00000260: 6365 6e73 6573 2f4c 4943 454e 5345 2d32  censes/LICENSE-2
+00000270: 2e30 0a0a 2020 556e 6c65 7373 2072 6571  .0..  Unless req
+00000280: 7569 7265 6420 6279 2061 7070 6c69 6361  uired by applica
+00000290: 626c 6520 6c61 7720 6f72 2061 6772 6565  ble law or agree
+000002a0: 6420 746f 2069 6e20 7772 6974 696e 672c  d to in writing,
+000002b0: 0a20 2073 6f66 7477 6172 6520 6469 7374  .  software dist
+000002c0: 7269 6275 7465 6420 756e 6465 7220 7468  ributed under th
+000002d0: 6520 4c69 6365 6e73 6520 6973 2064 6973  e License is dis
+000002e0: 7472 6962 7574 6564 206f 6e20 616e 0a20  tributed on an. 
+000002f0: 2022 4153 2049 5322 2042 4153 4953 2c20   "AS IS" BASIS, 
+00000300: 5749 5448 4f55 5420 5741 5252 414e 5449  WITHOUT WARRANTI
+00000310: 4553 204f 5220 434f 4e44 4954 494f 4e53  ES OR CONDITIONS
+00000320: 204f 4620 414e 590a 2020 4b49 4e44 2c20   OF ANY.  KIND, 
+00000330: 6569 7468 6572 2065 7870 7265 7373 206f  either express o
+00000340: 7220 696d 706c 6965 642e 2020 5365 6520  r implied.  See 
+00000350: 7468 6520 4c69 6365 6e73 6520 666f 7220  the License for 
+00000360: 7468 650a 2020 7370 6563 6966 6963 206c  the.  specific l
+00000370: 616e 6775 6167 6520 676f 7665 726e 696e  anguage governin
+00000380: 6720 7065 726d 6973 7369 6f6e 7320 616e  g permissions an
+00000390: 6420 6c69 6d69 7461 7469 6f6e 730a 2020  d limitations.  
+000003a0: 756e 6465 7220 7468 6520 4c69 6365 6e73  under the Licens
+000003b0: 652e 0ae9 0000 0000 4e29 02da 0d41 7379  e.......N)...Asy
+000003c0: 6e63 4974 6572 6174 6f72 da08 4f70 7469  ncIterator..Opti
+000003d0: 6f6e 616c e901 0000 0029 09da 1343 4f4e  onal.....)...CON
+000003e0: 5445 4e54 5f54 5950 455f 4845 4144 4552  TENT_TYPE_HEADER
+000003f0: da07 4865 6164 6572 73da 0845 7865 6375  ..Headers..Execu
+00000400: 746f 72da 0e45 7865 6375 746f 7252 6573  tor..ExecutorRes
+00000410: 756c 74da 124a 736f 6e45 7865 6375 746f  ult..JsonExecuto
+00000420: 7252 6573 756c 74da 154a 736f 6e53 6571  rResult..JsonSeq
+00000430: 4578 6563 7574 6f72 5265 7375 6c74 da17  ExecutorResult..
+00000440: 506c 6169 6e54 6578 7445 7865 6375 746f  PlainTextExecuto
+00000450: 7252 6573 756c 74da 0c54 5241 4345 5f48  rResult..TRACE_H
+00000460: 4541 4445 52da 1e75 6e73 7570 706f 7274  EADER..unsupport
+00000470: 6564 5f63 6f6e 7465 6e74 5f74 7970 655f  ed_content_type_
+00000480: 6572 726f 7263 0000 0000 0000 0000 0000  errorc..........
+00000490: 0000 0000 0000 0c00 0000 0000 0000 735c  ..............s\
+000004a0: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+000004b0: 0e64 0365 0464 0465 0565 0419 0066 0487  .d.e.d.e.e...f..
+000004c0: 0066 0164 0564 0684 0d5a 0665 076a 0864  .f.d.d...Z.e.j.d
+000004d0: 0765 0464 0865 0464 0965 0964 0a65 0565  .e.d.e.d.e.d.e.e
+000004e0: 0a19 0064 0b65 0b65 0c19 0066 0a64 0c64  ...d.e.e...f.d.d
+000004f0: 0d84 0483 015a 0d87 0004 005a 0e53 0029  .....Z.....Z.S.)
+00000500: 0fda 0e55 726c 6c69 6245 7865 6375 746f  ...UrllibExecuto
+00000510: 727a 700a 2020 2020 6075 726c 6c69 6260  rzp.    `urllib`
+00000520: 2d70 6f77 6572 6564 2065 7865 6375 746f  -powered executo
+00000530: 722c 2075 7365 6420 6173 2066 616c 6c62  r, used as fallb
+00000540: 6163 6b2e 2057 6865 6e20 706f 7373 6962  ack. When possib
+00000550: 6c65 2c20 7072 6566 6572 2075 7369 6e67  le, prefer using
+00000560: 0a20 2020 2074 6865 2060 6169 6f68 7474  .    the `aiohtt
+00000570: 7060 2065 7175 6976 616c 656e 742e 0a20  p` equivalent.. 
+00000580: 2020 204e da07 6170 695f 7572 6cda 0d61     N..api_url..a
+00000590: 7574 686f 7269 7a61 7469 6f6e 6303 0000  uthorizationc...
+000005a0: 0000 0000 0000 0000 0003 0000 0005 0000  ................
+000005b0: 0003 0000 0073 1400 0000 7400 8300 a001  .....s....t.....
+000005c0: 6401 7c01 7c02 a103 0100 6400 5300 2902  d.|.|.....d.S.).
+000005d0: 4eda 0675 726c 6c69 6229 02da 0573 7570  N..urllib)...sup
+000005e0: 6572 da08 5f5f 696e 6974 5f5f 2903 da04  er..__init__)...
+000005f0: 7365 6c66 720f 0000 0072 1000 0000 a901  selfr....r......
+00000600: da09 5f5f 636c 6173 735f 5fa9 00fa 3b2f  ..__class__...;/
+00000610: 686f 6d65 2f72 756e 6e65 722f 776f 726b  home/runner/work
+00000620: 2f73 646b 2e70 792f 7364 6b2e 7079 2f6f  /sdk.py/sdk.py/o
+00000630: 7076 696f 7573 2f65 7865 6375 746f 7273  pvious/executors
+00000640: 2f75 726c 6c69 622e 7079 7213 0000 0030  /urllib.pyr....0
+00000650: 0000 0073 0200 0000 1401 7a17 5572 6c6c  ...s......z.Urll
+00000660: 6962 4578 6563 7574 6f72 2e5f 5f69 6e69  ibExecutor.__ini
+00000670: 745f 5fda 0375 726c da06 6d65 7468 6f64  t__..url..method
+00000680: da07 6865 6164 6572 73da 0462 6f64 79da  ..headers..body.
+00000690: 0672 6574 7572 6e63 0500 0000 0000 0000  .returnc........
+000006a0: 0000 0000 0c00 0000 0a00 0000 4302 0000  ............C...
+000006b0: 73e2 0000 0081 0274 006a 016a 027c 017c  s......t.j.j.|.|
+000006c0: 037c 027c 0464 018d 047d 057a 0874 006a  .|.|.d...}.z.t.j
+000006d0: 01a0 037c 05a1 017d 0657 006e 1604 0074  ...|...}.W.n...t
+000006e0: 006a 046a 0579 2901 007d 0701 007a 087c  .j.j.y)..}...z.|
+000006f0: 077d 0657 0059 0064 007d 077e 076e 0564  .}.W.Y.d.}.~.n.d
+00000700: 007d 077e 0777 0177 007c 066a 067d 087c  .}.~.w.w.|.j.}.|
+00000710: 06a0 0774 08a1 017d 097c 06a0 0774 09a1  ...t...}.|...t..
+00000720: 017d 0a74 0aa0 0b7c 0aa1 0172 4d7c 06a0  .}.t...|...rM|..
+00000730: 0ca1 00a0 0d64 02a1 017d 0b74 0a7c 087c  .....d...}.t.|.|
+00000740: 097c 0b64 038d 0356 0001 0064 0053 0074  .|.d...V...d.S.t
+00000750: 0ea0 0b7c 0aa1 0172 5c74 0e7c 087c 097c  ...|...r\t.|.|.|
+00000760: 0664 048d 0356 0001 0064 0053 0074 0fa0  .d...V...d.S.t..
+00000770: 0b7c 0aa1 0172 6b74 0f7c 087c 097c 0664  .|...rkt.|.|.|.d
+00000780: 048d 0356 0001 0064 0053 0074 107c 0a7c  ...V...d.S.t.|.|
+00000790: 0964 058d 0282 0129 064e 2904 7219 0000  .d.....).N).r...
+000007a0: 0072 1b00 0000 721a 0000 00da 0464 6174  .r....r......dat
+000007b0: 61da 0475 7466 3829 03da 0673 7461 7475  a..utf8)...statu
+000007c0: 73da 0574 7261 6365 da04 7465 7874 2903  s..trace..text).
+000007d0: 7220 0000 0072 2100 0000 da06 7265 6164  r ...r!.....read
+000007e0: 6572 2902 da0c 636f 6e74 656e 745f 7479  er)...content_ty
+000007f0: 7065 7221 0000 0029 1172 1100 0000 da07  per!...).r......
+00000800: 7265 7175 6573 74da 0752 6571 7565 7374  request..Request
+00000810: da07 7572 6c6f 7065 6eda 0565 7272 6f72  ..urlopen..error
+00000820: da09 4854 5450 4572 726f 7272 2000 0000  ..HTTPErrorr ...
+00000830: da09 6765 7468 6561 6465 7272 0c00 0000  ..getheaderr....
+00000840: 7205 0000 0072 0900 0000 da0b 6973 5f65  r....r......is_e
+00000850: 6c69 6769 626c 65da 0472 6561 64da 0664  ligible..read..d
+00000860: 6563 6f64 6572 0b00 0000 720a 0000 0072  ecoder....r....r
+00000870: 0d00 0000 290c 7214 0000 0072 1900 0000  ....).r....r....
+00000880: 721a 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
+00000890: 0372 6571 da03 7265 73da 0365 7272 7220  .req..res..errr 
+000008a0: 0000 0072 2100 0000 da05 6374 7970 6572  ...r!.....ctyper
+000008b0: 2200 0000 7217 0000 0072 1700 0000 7218  "...r....r....r.
+000008c0: 0000 00da 055f 7365 6e64 3300 0000 733a  ....._send3...s:
+000008d0: 0000 0002 8006 0402 0102 0102 0102 0106  ................
+000008e0: fc02 0610 0112 0110 0108 8002 ff06 020a  ................
+000008f0: 010a 010a 010e 0114 010a 0102 0106 010c  ................
+00000900: ff0a 0314 0202 0202 0102 0106 fe7a 1455  .............z.U
+00000910: 726c 6c69 6245 7865 6375 746f 722e 5f73  rllibExecutor._s
+00000920: 656e 6429 014e 290f da08 5f5f 6e61 6d65  end).N)...__name
+00000930: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000940: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
+00000950: 646f 635f 5fda 0373 7472 7203 0000 0072  doc__..strr....r
+00000960: 1300 0000 da0a 636f 6e74 6578 746c 6962  ......contextlib
+00000970: da13 6173 796e 6363 6f6e 7465 7874 6d61  ..asynccontextma
+00000980: 6e61 6765 7272 0600 0000 da05 6279 7465  nagerr......byte
+00000990: 7372 0200 0000 7208 0000 0072 3200 0000  sr....r....r2...
+000009a0: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
+000009b0: 1700 0000 7217 0000 0072 1500 0000 7218  ....r....r....r.
+000009c0: 0000 0072 0e00 0000 2a00 0000 731e 0000  ...r....*...s...
+000009d0: 0008 0004 011c 0504 0302 0102 0102 ff02  ................
+000009e0: 0102 ff02 0102 ff06 0102 ff06 0214 fe72  ...............r
+000009f0: 0e00 0000 2917 7236 0000 0072 3800 0000  ....).r6...r8...
+00000a00: da07 6c6f 6767 696e 67da 0c75 726c 6c69  ..logging..urlli
+00000a10: 622e 6572 726f 7272 1100 0000 da0e 7572  b.errorr......ur
+00000a20: 6c6c 6962 2e72 6571 7565 7374 da06 7479  llib.request..ty
+00000a30: 7069 6e67 7202 0000 0072 0300 0000 da06  pingr....r......
+00000a40: 636f 6d6d 6f6e 7205 0000 0072 0600 0000  commonr....r....
+00000a50: 7207 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
+00000a60: 0a00 0000 720b 0000 0072 0c00 0000 720d  ....r....r....r.
+00000a70: 0000 00da 0967 6574 4c6f 6767 6572 7233  .....getLoggerr3
+00000a80: 0000 00da 075f 6c6f 6767 6572 720e 0000  ....._loggerr...
+00000a90: 0072 1700 0000 7217 0000 0072 1700 0000  .r....r....r....
+00000aa0: 7218 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000ab0: 0000 0073 1200 0000 0400 0813 0801 0801  ...s............
+00000ac0: 0801 1001 2c02 0a0d 1403                 ....,.....
```

### Comparing `opvious-0.8.1/opvious/executors/aiohttp.py` & `opvious-0.9.3/opvious/executors/aiohttp.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,27 +14,26 @@
   "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
   KIND, either express or implied.  See the License for the
   specific language governing permissions and limitations
   under the License.
 """
 
 import aiohttp
-import brotli
+import brotli  # type: ignore
 import contextlib
-import json
 import logging
-import urllib.parse
-from typing import Any, Optional
+from typing import AsyncIterator, Optional
 
 from .common import (
     CONTENT_TYPE_HEADER,
-    default_headers,
-    Execution,
+    Executor,
+    ExecutorResult,
     JsonExecutorResult,
     JsonSeqExecutorResult,
+    PlainTextExecutorResult,
     Headers,
     TRACE_HEADER,
     unexpected_response_error,
     unsupported_content_type_error,
 )
 
 
@@ -49,93 +48,71 @@
 
 _READ_BUFFER_SIZE = 2**26  # 512MiB
 
 
 _REQUEST_TIMEOUT_SECONDS = 900  # 15 minutes
 
 
-class AiohttpExecutor:
-    """`aiohttp`-powered GraphQL executor"""
+class AiohttpExecutor(Executor):
+    """`aiohttp`-powered executor"""
 
     def __init__(self, api_url: str, authorization: Optional[str] = None):
-        self._api_url = api_url
-        self._headers = default_headers("aiohttp")
-        self._headers["accept-encoding"] = "br;q=1.0, gzip;q=0.5, *;q=0.1"
-        if authorization:
-            self._headers["authorization"] = authorization
-        _logger.debug(
-            "Instantiated executor. [name=%s, url=%s]",
-            self.__class__.__name__,
-            api_url,
-        )
-
-    def execute(
-        self,
-        path: str,
-        method: str = "GET",
-        headers: Optional[Headers] = None,
-        json_body: Optional[Any] = None,
-    ) -> Execution:
-        all_headers = self._headers.copy()
-        if headers:
-            all_headers.update(headers)
-        if json_body:
-            all_headers["content-type"] = "application/json"
-            data = json.dumps(json_body)
-            if len(data) > _COMPRESSION_THRESHOLD:
-                _logger.debug(
-                    "Compressing API request... [size=%s]", len(data)
-                )
-                all_headers["content-encoding"] = "br"
-                data = brotli.compress(
-                    data.encode("utf8"),
-                    mode=brotli.MODE_TEXT,
-                    quality=_BROTLI_QUALITY,
+        super().__init__("aiohttp", api_url, authorization)
+
+    @contextlib.asynccontextmanager
+    async def _send(
+        self, url: str, method: str, headers: Headers, body: Optional[bytes]
+    ) -> AsyncIterator[ExecutorResult]:
+        if body and len(body) > _COMPRESSION_THRESHOLD:
+            headers["content-encoding"] = "br"
+            compressed_body = brotli.compress(
+                body,
+                mode=brotli.MODE_TEXT,
+                quality=_BROTLI_QUALITY,
+            )
+            _logger.debug(
+                "Compressed request body. [size=%s]", len(compressed_body)
+            )
+            body = compressed_body
+        try:
+            async with aiohttp.ClientSession(
+                headers=headers,
+                read_bufsize=_READ_BUFFER_SIZE,
+                timeout=aiohttp.ClientTimeout(total=_REQUEST_TIMEOUT_SECONDS),
+            ) as session:
+                async with session.request(
+                    url=url, method=method, data=body
+                ) as res:
+                    status = res.status
+                    trace = res.headers.get(TRACE_HEADER)
+                    ctype = res.headers.get(CONTENT_TYPE_HEADER)
+                    if JsonExecutorResult.is_eligible(ctype):
+                        text = await res.text()
+                        yield JsonExecutorResult(
+                            status=status,
+                            trace=trace,
+                            text=text,
+                        )
+                    elif JsonSeqExecutorResult.is_eligible(ctype):
+                        yield JsonSeqExecutorResult(
+                            status=status,
+                            trace=trace,
+                            reader=res.content,
+                        )
+                    elif PlainTextExecutorResult.is_eligible(ctype):
+                        yield PlainTextExecutorResult(
+                            status=status,
+                            trace=trace,
+                            reader=res.content,
+                        )
+                    else:
+                        raise unsupported_content_type_error(
+                            content_type=ctype,
+                            trace=trace,
+                        )
+        except aiohttp.ClientResponseError as err:
+            trace = None
+            if isinstance(err.headers, list):
+                trace = next(
+                    (v for (k, v) in err.headers if k == TRACE_HEADER), None
                 )
-        else:
-            data = None
-        return _execution(
-            url=urllib.parse.urljoin(self._api_url, path),
-            method=method,
-            headers=all_headers,
-            data=data,
-        )
-
-
-@contextlib.asynccontextmanager
-async def _execution(
-    url: str, method: str, headers: Headers, data: Any
-) -> Execution:
-    _logger.debug("Sending API request... [size=%s]", len(data) if data else 0)
-    try:
-        async with aiohttp.ClientSession(
-            headers=headers,
-            read_bufsize=_READ_BUFFER_SIZE,
-            timeout=aiohttp.ClientTimeout(total=_REQUEST_TIMEOUT_SECONDS),
-        ) as session:
-            async with session.request(
-                method=method, url=url, data=data
-            ) as res:
-                status = res.status
-                trace = res.headers.get(TRACE_HEADER)
-                ctype = res.headers.get(CONTENT_TYPE_HEADER)
-                if JsonExecutorResult.is_eligible(ctype):
-                    text = await res.text()
-                    yield JsonExecutorResult(
-                        status=status,
-                        trace=trace,
-                        text=text,
-                    )
-                elif JsonSeqExecutorResult.is_eligible(ctype):
-                    yield JsonSeqExecutorResult(
-                        status=status,
-                        trace=trace,
-                        reader=res.content,
-                    )
-                else:
-                    raise unsupported_content_type_error(
-                        content_type=ctype,
-                        trace=trace,
-                    )
-    except aiohttp.ClientResponseError as err:
-        trace = next((v for k, v in err.headers if k == TRACE_HEADER), None)
-        raise unexpected_response_error(message=err.message, trace=trace)
+            raise unexpected_response_error(message=err.message, trace=trace)
```

### Comparing `opvious-0.8.1/opvious/executors/pyodide.py` & `opvious-0.9.3/opvious/executors/urllib.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,89 +14,69 @@
   "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
   KIND, either express or implied.  See the License for the
   specific language governing permissions and limitations
   under the License.
 """
 
 import contextlib
-import json
 import logging
-from pyodide.http import pyfetch
-from typing import Any, Optional
-import urllib.parse
+import urllib.error
+import urllib.request
+from typing import AsyncIterator, Optional
 
 from .common import (
     CONTENT_TYPE_HEADER,
-    default_headers,
-    Execution,
-    JsonExecutorResult,
     Headers,
+    Executor,
+    ExecutorResult,
+    JsonExecutorResult,
+    JsonSeqExecutorResult,
+    PlainTextExecutorResult,
     TRACE_HEADER,
     unsupported_content_type_error,
 )
 
 
 _logger = logging.getLogger(__name__)
 
 
-class PyodideExecutor:
-    """`pyodide`-powered executor"""
+class UrllibExecutor(Executor):
+    """
+    `urllib`-powered executor, used as fallback. When possible, prefer using
+    the `aiohttp` equivalent.
+    """
 
     def __init__(self, api_url: str, authorization: Optional[str] = None):
-        self._api_url = api_url
-        self._headers = default_headers("pyodide")
-        if authorization:
-            self._headers["authorization"] = authorization
-        _logger.debug(
-            "Instantiated executor. [name=%s, url=%s]",
-            self.__class__.__name__,
-            api_url,
-        )
+        super().__init__("urllib", api_url, authorization)
 
-    def execute(
-        self,
-        path: str,
-        method: str = "GET",
-        headers: Optional[Headers] = None,
-        json_body: Optional[Any] = None,
-    ) -> Execution:
-        all_headers = self._headers.copy()
-        if headers:
-            all_headers.update(headers)
-        if json_body:
-            all_headers["content-type"] = "application/json"
-            data = json.dumps(json_body)
-        else:
-            data = None
-        return _execution(
-            url=urllib.parse.urljoin(self._api_url, path),
+    @contextlib.asynccontextmanager
+    async def _send(
+        self, url: str, method: str, headers: Headers, body: Optional[bytes]
+    ) -> AsyncIterator[ExecutorResult]:
+        req = urllib.request.Request(
+            url=url,
+            headers=headers,
             method=method,
-            headers=all_headers,
-            data=data,
-        )
-
-
-@contextlib.asynccontextmanager
-async def _execution(
-    url: str, method: str, headers: Headers, data: Any
-) -> Execution:
-    _logger.debug("Sending API request... [size=%s]", len(data) if data else 0)
-    # TODO: Raise any errors as ApiError
-    res = await pyfetch(
-        url=url,
-        method=method,
-        headers=headers,
-        body=data,
-    )
-    status = res.status
-    headers = res.js_response.headers
-    trace = (headers.get(TRACE_HEADER),)
-    ctype = headers.get(CONTENT_TYPE_HEADER)
-    if JsonExecutorResult.is_eligible(ctype):
-        text = await res.js_response.text()
-        yield JsonExecutorResult(status=status, trace=trace, text=text)
-    else:
-        # TODO: Support streaming responses.
-        raise unsupported_content_type_error(
-            content_type=ctype,
-            trace=trace,
+            data=body,
         )
+        try:
+            res = urllib.request.urlopen(req)
+        except urllib.error.HTTPError as err:
+            res = err
+        status = res.status
+        trace = res.getheader(TRACE_HEADER)
+        ctype = res.getheader(CONTENT_TYPE_HEADER)
+        if JsonExecutorResult.is_eligible(ctype):
+            text = res.read().decode("utf8")
+            yield JsonExecutorResult(status=status, trace=trace, text=text)
+        elif PlainTextExecutorResult.is_eligible(ctype):
+            yield PlainTextExecutorResult(
+                status=status, trace=trace, reader=res
+            )
+        elif JsonSeqExecutorResult.is_eligible(ctype):
+            # TODO: Check compatible
+            yield JsonSeqExecutorResult(status=status, trace=trace, reader=res)
+        else:
+            raise unsupported_content_type_error(
+                content_type=ctype,
+                trace=trace,
+            )
```

### Comparing `opvious-0.8.1/pyproject.toml` & `opvious-0.9.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "opvious"
-version = "0.8.1"
+version = "0.9.3"
 description = "Opvious Python SDK"
 authors = ["Opvious Engineering <oss@opvious.io>"]
 readme = "README.md"
 repository = "https://github.com/opvious/sdk.py"
 packages = [{include = "opvious"}]
 
 [tool.poetry.dependencies]
 aiohttp = {version = "^3.8", optional = true}
 backoff = "^2.2"
 Brotli = {version = "^1.0.9", optional = true}
 humanize = "^4.4.0"
 pandas = "^1.4"
-python = "^3.8"
+python = ">=3.8,<3.12"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
 flake8 = "^4.0.1"
+mypy = "^1.2.0"
 pytest = "~7.1.2"
 pytest-asyncio = "^0.20.2"
+pandas-stubs = "^1.5.3.230321"
 
 [tool.poetry.extras]
 aio = ["aiohttp", "Brotli"]
 
 [tool.black]
 line-length = 79
 include = '\.py$'
```

### Comparing `opvious-0.8.1/setup.py` & `opvious-0.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 ['backoff>=2.2,<3.0', 'humanize>=4.4.0,<5.0.0', 'pandas>=1.4,<2.0']
 
 extras_require = \
 {'aio': ['aiohttp>=3.8,<4.0', 'Brotli>=1.0.9,<2.0.0']}
 
 setup_kwargs = {
     'name': 'opvious',
-    'version': '0.8.1',
+    'version': '0.9.3',
     'description': 'Opvious Python SDK',
-    'long_description': '# Opvious Python SDK  [![CI](https://github.com/opvious/sdk.py/actions/workflows/ci.yml/badge.svg)](https://github.com/opvious/sdk.py/actions/workflows/ci.yml) [![Pypi badge](https://badge.fury.io/py/opvious.svg)](https://pypi.python.org/pypi/opvious/)\n\nThis package provides a lightweight SDK for solving optimization models with the\n[Opvious API][api]. Its main features are:\n\n+ Seamless data import/export via native support for [`pandas`][pandas]\n+ Powerful built-in debugging capabilities: automatic infeasibility relaxation,\n  variable pinning, and more\n+ Non-blocking APIs for performant parallel calls\n\n\n## Quickstart\n\nFirst, install this package and have an API access token handy (these can be\ngenerated [here][token]).\n\n```sh\npip install opvious[aio] # aio is recommended for improved performance\n```\n\nWith these steps out of the way, you are ready to optimize!\n\n```python\nimport opvious\n\n# Instantiate an API client from an API token\nclient = opvious.Client.from_token(TOKEN)\n\n# Solve a simple portfolio selection optimization model\noutputs = await client.solve(\n    sources=[\n      r"""\n          We find an allocation of assets which minimizes risk while satisfying\n          a minimum expected return:\n\n          + A collection of assets: $\\S^d_{asset}: A$\n          + Covariances: $\\S^p_{covariance}: c \\in \\mathbb{R}^{A \\times A}$\n          + Expected return: $\\S^p_{expectedReturn}: m \\in \\mathbb{R}^A$\n          + Minimum desired return: $\\S^p_{desiredReturn}: r \\in \\mathbb{R}$\n\n          The only output is the allocation per asset\n          $\\S^v_{allocation}: \\alpha \\in [0,1]^A$ chosen to minimize risk:\n          $\\S^o_{risk}: \\min \\sum_{a, b \\in A} c_{a,b} \\alpha_a \\alpha_b$.\n\n          Subject to the following constraints:\n\n          + $\\S^c_{atLeastMinimumReturn}: \\sum_{a \\in A} m_a \\alpha_a \\geq r$\n          + $\\S^c_{totalAllocation}: \\sum_{a \\in A} \\alpha_a = 1$\n      """\n    ],\n    parameters={\n        "covariance": {\n            ("AAPL", "AAPL"): 0.08,\n            # ...\n        },\n        "expectedReturn": {\n            "AAPL": 0.07,\n            # ..\n        },\n        "desiredReturn": 0.05,\n    },\n)\n\n# Print the optimal allocation, if any\nif isinstance(outputs.outcome, opvious.FeasibleOutcome):\n  print(outputs.data.variable("allocation"))\nelse:\n  print(f"Problem was {outputs.status}.") # INFEASIBLE, UNBOUNDED\n```\n\n\n## Environments\n\nClients are compatible with Pyodide environments, for example [JupyterLite][]\nkernels. Simply install the package as usual in a notebook, omitting the `aio`\noptional dependencies:\n\n```python\nimport piplite\nawait piplite.install(\'opvious\')\n```\n\nIn other environments, prefer using the `aiohttp`-powered clients as they are\nmore performant (this is the default if the `aio` dependencies were specified).\n\n\n## Next steps\n\nThis SDK is focused on solving optimization models. For convenient access to the\nrest of Opvious API\'s functionality, consider using the [TypeScript SDK and\nCLI][cli].\n\n\n[api]: https://www.opvious.io\n[cli]: https://www.opvious.io/sdk.ts\n[JupyterLite]: https://jupyterlite.readthedocs.io/\n[token]: https://hub.beta.opvious.io/authorizations\n[pandas]: https://pandas.pydata.org\n',
+    'long_description': '# Opvious Python SDK  [![CI](https://github.com/opvious/sdk.py/actions/workflows/ci.yml/badge.svg)](https://github.com/opvious/sdk.py/actions/workflows/ci.yml) [![Pypi badge](https://badge.fury.io/py/opvious.svg)](https://pypi.python.org/pypi/opvious/)\n\nThis package provides a lightweight SDK for solving optimization models with the\n[Opvious API][api]. Its main features are:\n\n+ Seamless data import/export via native support for [`pandas`][pandas]\n+ Powerful built-in debugging capabilities: automatic infeasibility relaxation,\n  variable pinning, and more\n+ Non-blocking APIs for performant parallel calls\n\n\n## Quickstart\n\nFirst, install this package and have an API access token handy (these can be\ngenerated [here][token]).\n\n```sh\npip install opvious[aio] # aio is recommended for improved performance\n```\n\nWith these steps out of the way, you are ready to optimize!\n\n```python\nimport opvious\n\n# Instantiate an API client from an API token\nclient = opvious.Client.from_token(TOKEN)\n\n# Solve a simple portfolio selection optimization model\nresponse = await client.solve(\n    sources=[\n      r"""\n          We find an allocation of assets which minimizes risk while satisfying\n          a minimum expected return:\n\n          + A collection of assets: $\\S^d_{asset}: A$\n          + Covariances: $\\S^p_{covariance}: c \\in \\mathbb{R}^{A \\times A}$\n          + Expected return: $\\S^p_{expectedReturn}: m \\in \\mathbb{R}^A$\n          + Minimum desired return: $\\S^p_{desiredReturn}: r \\in \\mathbb{R}$\n\n          The only output is the allocation per asset\n          $\\S^v_{allocation}: \\alpha \\in [0,1]^A$ chosen to minimize risk:\n          $\\S^o_{risk}: \\min \\sum_{a, b \\in A} c_{a,b} \\alpha_a \\alpha_b$.\n\n          Subject to the following constraints:\n\n          + $\\S^c_{atLeastMinimumReturn}: \\sum_{a \\in A} m_a \\alpha_a \\geq r$\n          + $\\S^c_{totalAllocation}: \\sum_{a \\in A} \\alpha_a = 1$\n      """\n    ],\n    parameters={\n        "covariance": {\n            ("AAPL", "AAPL"): 0.08,\n            # ...\n        },\n        "expectedReturn": {\n            "AAPL": 0.07,\n            # ..\n        },\n        "desiredReturn": 0.05,\n    },\n)\n\n# Print the optimal allocation, if any\nif isinstance(response.outcome, opvious.FeasibleOutcome):\n  print(response.outputs.variable("allocation"))\nelse:\n  print(f"Problem was {response.status}.") # INFEASIBLE, UNBOUNDED\n```\n\n\n## Environments\n\nClients are compatible with Pyodide environments, for example [JupyterLite][]\nkernels. Simply install the package as usual in a notebook, omitting the `aio`\noptional dependencies:\n\n```python\nimport piplite\nawait piplite.install(\'opvious\')\n```\n\nIn other environments, prefer using the `aiohttp`-powered clients as they are\nmore performant (this is the default if the `aio` dependencies were specified).\n\n\n## Next steps\n\nThis SDK is focused on solving optimization models. For convenient access to the\nrest of Opvious API\'s functionality, consider using the [TypeScript SDK and\nCLI][cli].\n\n\n[api]: https://www.opvious.io\n[cli]: https://www.opvious.io/sdk.ts\n[JupyterLite]: https://jupyterlite.readthedocs.io/\n[token]: https://hub.beta.opvious.io/authorizations\n[pandas]: https://pandas.pydata.org\n',
     'author': 'Opvious Engineering',
     'author_email': 'oss@opvious.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/opvious/sdk.py',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.8,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `opvious-0.8.1/PKG-INFO` & `opvious-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: opvious
-Version: 0.8.1
+Version: 0.9.3
 Summary: Opvious Python SDK
 Home-page: https://github.com/opvious/sdk.py
 Author: Opvious Engineering
 Author-email: oss@opvious.io
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: aio
 Requires-Dist: Brotli (>=1.0.9,<2.0.0); extra == "aio"
@@ -45,15 +45,15 @@
 ```python
 import opvious
 
 # Instantiate an API client from an API token
 client = opvious.Client.from_token(TOKEN)
 
 # Solve a simple portfolio selection optimization model
-outputs = await client.solve(
+response = await client.solve(
     sources=[
       r"""
           We find an allocation of assets which minimizes risk while satisfying
           a minimum expected return:
 
           + A collection of assets: $\S^d_{asset}: A$
           + Covariances: $\S^p_{covariance}: c \in \mathbb{R}^{A \times A}$
@@ -80,18 +80,18 @@
             # ..
         },
         "desiredReturn": 0.05,
     },
 )
 
 # Print the optimal allocation, if any
-if isinstance(outputs.outcome, opvious.FeasibleOutcome):
-  print(outputs.data.variable("allocation"))
+if isinstance(response.outcome, opvious.FeasibleOutcome):
+  print(response.outputs.variable("allocation"))
 else:
-  print(f"Problem was {outputs.status}.") # INFEASIBLE, UNBOUNDED
+  print(f"Problem was {response.status}.") # INFEASIBLE, UNBOUNDED
 ```
 
 
 ## Environments
 
 Clients are compatible with Pyodide environments, for example [JupyterLite][]
 kernels. Simply install the package as usual in a notebook, omitting the `aio`
```

