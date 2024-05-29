# Comparing `tmp/pyqtorch-1.1.1.tar.gz` & `tmp/pyqtorch-1.1.2.tar.gz`

## Comparing `pyqtorch-1.1.1.tar` & `pyqtorch-1.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/README.md
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/mkdocs.yml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/setup.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/.github/workflows/run-tests-and-mypy.yml
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0    14146 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/docs/index.md
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyqtorch/__init__.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyqtorch/adjoint.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyqtorch/analog.py
--rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyqtorch/apply.py
--rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyqtorch/circuit.py
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyqtorch/matrices.py
--rw-r--r--   0        0        0     8620 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyqtorch/parametric.py
--rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyqtorch/primitive.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyqtorch/py.typed
--rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyqtorch/utils.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/tests/conftest.py
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/tests/test_analog.py
--rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/tests/test_circuit.py
--rw-r--r--   0        0        0    13652 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/tests/test_digital.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/LICENSE
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pyqtorch-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/README.md
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/mkdocs.yml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/setup.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/.github/workflows/run-tests-and-mypy.yml
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/docs/index.md
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/pyqtorch/__init__.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/pyqtorch/adjoint.py
+-rw-r--r--   0        0        0     5532 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/pyqtorch/analog.py
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/pyqtorch/apply.py
+-rw-r--r--   0        0        0     6588 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/pyqtorch/circuit.py
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/pyqtorch/matrices.py
+-rw-r--r--   0        0        0     8604 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/pyqtorch/parametric.py
+-rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/pyqtorch/primitive.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/pyqtorch/py.typed
+-rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/pyqtorch/utils.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/tests/test_analog.py
+-rw-r--r--   0        0        0     7822 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/tests/test_circuit.py
+-rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/tests/test_digital.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/LICENSE
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pyqtorch-1.1.2/PKG-INFO
```

### Comparing `pyqtorch-1.1.1/.pre-commit-config.yaml` & `pyqtorch-1.1.2/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.5.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-added-large-files
 
 -   repo: https://github.com/ambv/black
-    rev: 23.3.0
+    rev: 24.4.2
     hooks:
       - id: black
 
 -   repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.274"
+    rev: "v0.4.4"
     hooks:
       - id: ruff
         args: [--fix]
 
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.4.0
+    rev: v1.10.0
     hooks:
       - id: mypy
         exclude: examples|docs
```

### Comparing `pyqtorch-1.1.1/README.md` & `pyqtorch-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-1.1.1/mkdocs.yml` & `pyqtorch-1.1.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-1.1.1/.github/workflows/run-tests-and-mypy.yml` & `pyqtorch-1.1.2/.github/workflows/run-tests-and-mypy.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-1.1.1/docs/CODE_OF_CONDUCT.md` & `pyqtorch-1.1.2/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-1.1.1/docs/CONTRIBUTING.md` & `pyqtorch-1.1.2/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-1.1.1/docs/index.md` & `pyqtorch-1.1.2/docs/index.md`

 * *Files 10% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 # Random hermitian hamiltonian
 matrix = torch.rand(2**n_qubits, 2**n_qubits, dtype=DEFAULT_MATRIX_DTYPE)
 hermitian_matrix = matrix + matrix.T.conj()
 
 # To be evolved for a batch of times
 t_list = torch.tensor([0.0, 0.5, 1.0, 2.0])
 
-hamiltonian_evolution = HamiltonianEvolution(qubit_support=[i for i in range(n_qubits)], n_qubits=n_qubits)
+hamiltonian_evolution = HamiltonianEvolution(qubit_support=[i for i in range(n_qubits)])
 
 # Starting from a uniform state
 psi_start = uniform_state(n_qubits)
 
 # Returns an evolved state at each time value
 psi_end = hamiltonian_evolution(
     hamiltonian=hermitian_matrix,
@@ -157,77 +157,65 @@
 ```python exec="on" source="material-block" html="1"
 from __future__ import annotations
 
 from operator import add
 from functools import reduce
 import torch
 import pyqtorch as pyq
+from pyqtorch.circuit import hea
 from pyqtorch.utils import DiffMode
 from pyqtorch.parametric import Parametric
 import matplotlib.pyplot as plt
 
 from torch.nn.functional import mse_loss
 
 # We can train on GPU if available
 DEVICE = torch.device('cuda') if torch.cuda.is_available() else torch.device('cpu')
 # We can also choose the precision we want to train on
 COMPLEX_DTYPE = torch.complex64
 REAL_DTYPE = torch.float32
+N_QUBITS = 4
+DEPTH = 2
+LR = .2
+DIFF_MODE = DiffMode.ADJOINT
+N_EPOCHS = 75
 
 # Target function and some training data
 fn = lambda x, degree: .05 * reduce(add, (torch.cos(i*x) + torch.sin(i*x) for i in range(degree)), 0)
 x = torch.linspace(0, 10, 100)
 y = fn(x, 5)
-
-
-def hea(n_qubits: int, n_layers: int, param_name: str) -> list:
-    ops = []
-    for l in range(n_layers):
-        ops += [pyq.RX(i, f'{param_name}_0_{l}_{i}') for i in range(n_qubits)]
-        ops += [pyq.RY(i, f'{param_name}_1_{l}_{i}') for i in range(n_qubits)]
-        ops += [pyq.RX(i, f'{param_name}_2_{l}_{i}') for i in range(n_qubits)]
-        ops += [pyq.CNOT(i % n_qubits, (i+1) % n_qubits) for i in range(n_qubits)]
-    return ops
-
-n_qubits = 5
-n_layers = 3
-diff_mode = DiffMode.ADJOINT
 # Lets define a feature map to encode our 'x' values
-feature_map = [pyq.RX(i, f'x') for i in range(n_qubits)]
+feature_map = [pyq.RX(i, f'x') for i in range(N_QUBITS)]
 # To fit the function, we define a hardware-efficient ansatz with tunable parameters
-ansatz = hea(n_qubits, n_layers, 'theta')
-observable = pyq.QuantumCircuit(n_qubits, [pyq.Z(0)])
-param_dict = torch.nn.ParameterDict({op.param_name: torch.rand(1, requires_grad=True) for op in ansatz if isinstance(op, Parametric)})
-circ = pyq.QuantumCircuit(n_qubits, feature_map + ansatz)
+ansatz, params = hea(N_QUBITS, DEPTH, 'theta')
 # Lets move all necessary components to the DEVICE
-circ = circ.to(device=DEVICE, dtype=COMPLEX_DTYPE)
-observable = observable.to(device=DEVICE, dtype=COMPLEX_DTYPE)
-param_dict = param_dict.to(device=DEVICE, dtype=REAL_DTYPE)
+circ = pyq.QuantumCircuit(N_QUBITS, feature_map + ansatz).to(device=DEVICE, dtype=COMPLEX_DTYPE)
+observable = pyq.Hamiltonian([pyq.Z(0)]).to(device=DEVICE, dtype=COMPLEX_DTYPE)
+params = params.to(device=DEVICE, dtype=REAL_DTYPE)
 x, y = x.to(device=DEVICE, dtype=REAL_DTYPE), y.to(device=DEVICE, dtype=REAL_DTYPE)
 state = circ.init_state()
 
-def exp_fn(param_dict: dict[str, torch.Tensor], inputs: dict[str, torch.Tensor]) -> torch.Tensor:
-    return pyq.expectation(circ, state, {**param_dict,**inputs}, observable, diff_mode)
+def exp_fn(params: dict[str, torch.Tensor], inputs: dict[str, torch.Tensor]) -> torch.Tensor:
+    return pyq.expectation(circ, state, {**params,**inputs}, observable, DIFF_MODE)
 
 with torch.no_grad():
-    y_init = exp_fn(param_dict, {'x': x})
+    y_init = exp_fn(params, {'x': x})
 
 # We need to set 'foreach' False since Adam doesnt support float64 on CUDA devices
-optimizer = torch.optim.Adam(param_dict.values(), lr=.01, foreach=False)
-epochs = 300
+optimizer = torch.optim.Adam(params.values(), lr=LR, foreach=False)
 
-for epoch in range(epochs):
+for _ in range(N_EPOCHS):
     optimizer.zero_grad()
-    y_pred = exp_fn(param_dict, {'x': x})
+    y_pred = exp_fn(params, {'x': x})
     loss = mse_loss(y, y_pred)
     loss.backward()
     optimizer.step()
 
 with torch.no_grad():
-    y_final = exp_fn(param_dict, {'x': x})
+    y_final = exp_fn(params, {'x': x})
 
 plt.plot(x.numpy(), y.numpy(), label="truth")
 plt.plot(x.numpy(), y_init.numpy(), label="initial")
 plt.plot(x.numpy(), y_final.numpy(), "--", label="final", linewidth=3)
 plt.legend()
 from io import StringIO  # markdown-exec: hide
 from matplotlib.figure import Figure  # markdown-exec: hide
@@ -251,66 +239,47 @@
 from typing import Callable
 
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
 from torch import Tensor, exp, linspace, ones_like, optim, rand, sin, tensor
 from torch.autograd import grad
-
-from pyqtorch import CNOT, RX, RY, QuantumCircuit, Z, expectation
+from pyqtorch.circuit import hea
+from pyqtorch import CNOT, RX, RY, QuantumCircuit, Z, expectation, Hamiltonian, Sequence, Merge
 from pyqtorch.parametric import Parametric
 from pyqtorch.utils import DiffMode
 
 DIFF_MODE = DiffMode.AD
 DEVICE = torch.device("cuda") if torch.cuda.is_available() else torch.device("cpu")
 # We can also choose the precision we want to train on
 COMPLEX_DTYPE = torch.complex64
 REAL_DTYPE = torch.float32
-PLOT = False
-LEARNING_RATE = 0.01
+LR = .15
 N_QUBITS = 4
 DEPTH = 3
 VARIABLES = ("x", "y")
-X_POS = 0
-Y_POS = 1
-N_POINTS = 150
-N_EPOCHS = 1000
-
-
-def hea(n_qubits: int, n_layers: int, param_name: str) -> list:
-    ops = []
-    for layer in range(n_layers):
-        ops += [RX(i, f"{param_name}_0_{layer}_{i}") for i in range(n_qubits)]
-        ops += [RY(i, f"{param_name}_1_{layer}_{i}") for i in range(n_qubits)]
-        ops += [RX(i, f"{param_name}_2_{layer}_{i}") for i in range(n_qubits)]
-        ops += [CNOT(i % n_qubits, (i + 1) % n_qubits) for i in range(n_qubits)]
-    return ops
-
-
-class TotalMagnetization(QuantumCircuit):
-    def __init__(self, n_qubits: int):
-        super().__init__(n_qubits, [Z(i) for i in range(n_qubits)])
-
-    def forward(self, state, values) -> Tensor:
-        return reduce(add, [op(state, values) for op in self.operations])
+N_VARIABLES = len(VARIABLES)
+X_POS, Y_POS = [i for i in range(N_VARIABLES)]
+BATCH_SIZE = 250
+N_EPOCHS = 750
 
 
 class DomainSampling(torch.nn.Module):
     def __init__(
-        self, exp_fn: Callable[[Tensor], Tensor], n_inputs: int, n_points: int, device: torch.device, dtype: torch.dtype
+        self, exp_fn: Callable[[Tensor], Tensor], n_inputs: int, batch_size: int, device: torch.device, dtype: torch.dtype
     ) -> None:
         super().__init__()
         self.exp_fn = exp_fn
         self.n_inputs = n_inputs
-        self.n_points = n_points
+        self.batch_size = batch_size
         self.device = device
         self.dtype = dtype
 
     def sample(self, requires_grad: bool = False) -> Tensor:
-        return rand((self.n_points, self.n_inputs), requires_grad=requires_grad, device=self.device, dtype=self.dtype)
+        return rand((self.batch_size, self.n_inputs), requires_grad=requires_grad, device=self.device, dtype=self.dtype)
 
     def left_boundary(self) -> Tensor:  # u(0,y)=0
         sample = self.sample()
         sample[:, X_POS] = 0.0
         return self.exp_fn(sample).pow(2).mean()
 
     def right_boundary(self) -> Tensor:  # u(L,y)=0
@@ -332,75 +301,66 @@
         sample = self.sample(requires_grad=True)
         f = self.exp_fn(sample)
         dfdxy = grad(
             f,
             sample,
             ones_like(f),
             create_graph=True,
-            retain_graph=True,
         )[0]
         dfdxxdyy = grad(
             dfdxy,
             sample,
             ones_like(dfdxy),
-            retain_graph=True,
         )[0]
 
         return (dfdxxdyy[:, X_POS] + dfdxxdyy[:, Y_POS]).pow(2).mean()
 
 
 feature_map = [RX(i, VARIABLES[X_POS]) for i in range(N_QUBITS // 2)] + [
     RX(i, VARIABLES[Y_POS]) for i in range(N_QUBITS // 2, N_QUBITS)
 ]
-ansatz = hea(N_QUBITS, DEPTH, "theta")
-param_dict = torch.nn.ParameterDict(
-    {
-        op.param_name: torch.rand(1, requires_grad=True)
-        for op in ansatz
-        if isinstance(op, Parametric)
-    }
-)
+ansatz, params = hea(N_QUBITS, DEPTH, "theta")
 circ = QuantumCircuit(N_QUBITS, feature_map + ansatz).to(device=DEVICE, dtype=COMPLEX_DTYPE)
-observable = TotalMagnetization(N_QUBITS).to(device=DEVICE, dtype=COMPLEX_DTYPE)
-param_dict = param_dict.to(device=DEVICE, dtype=REAL_DTYPE)
+total_magnetization = Hamiltonian([Z(i) for i in range(N_QUBITS)]).to(device=DEVICE, dtype=COMPLEX_DTYPE)
+params = params.to(device=DEVICE, dtype=REAL_DTYPE)
 state = circ.init_state()
 
 
 def exp_fn(inputs: Tensor) -> Tensor:
     return expectation(
         circ,
         state,
-        {**param_dict, **{VARIABLES[X_POS]: inputs[:, X_POS], VARIABLES[Y_POS]: inputs[:, Y_POS]}},
-        observable,
+        {**params, **{VARIABLES[X_POS]: inputs[:, X_POS], VARIABLES[Y_POS]: inputs[:, Y_POS]}},
+        total_magnetization,
         DIFF_MODE,
     )
 
 
-single_domain_torch = linspace(0, 1, steps=N_POINTS)
+single_domain_torch = linspace(0, 1, steps=BATCH_SIZE)
 domain_torch = tensor(list(product(single_domain_torch, single_domain_torch)))
 
-opt = optim.Adam(param_dict.values(), lr=LEARNING_RATE)
-sol = DomainSampling(exp_fn, len(VARIABLES), N_POINTS, DEVICE, REAL_DTYPE)
+opt = optim.Adam(params.values(), lr=LR)
+sol = DomainSampling(exp_fn, len(VARIABLES), BATCH_SIZE, DEVICE, REAL_DTYPE)
 
 for _ in range(N_EPOCHS):
     opt.zero_grad()
     loss = (
         sol.left_boundary()
         + sol.right_boundary()
         + sol.top_boundary()
         + sol.bottom_boundary()
         + sol.interior()
     )
     loss.backward()
     opt.step()
 
-dqc_sol = exp_fn(domain_torch.to(DEVICE)).reshape(N_POINTS, N_POINTS).detach().cpu().numpy()
+dqc_sol = exp_fn(domain_torch.to(DEVICE)).reshape(BATCH_SIZE, BATCH_SIZE).detach().cpu().numpy()
 analytic_sol = (
-    (exp(-np.pi * domain_torch[:, 0]) * sin(np.pi * domain_torch[:, 1]))
-    .reshape(N_POINTS, N_POINTS)
+    (exp(-np.pi * domain_torch[:, X_POS]) * sin(np.pi * domain_torch[:, Y_POS]))
+    .reshape(BATCH_SIZE, BATCH_SIZE)
     .T
 ).numpy()
 
 
 fig, ax = plt.subplots(1, 2, figsize=(7, 7))
 ax[0].imshow(analytic_sol, cmap="turbo")
 ax[0].set_xlabel("x")
@@ -414,7 +374,24 @@
 from matplotlib.figure import Figure  # markdown-exec: hide
 def fig_to_html(fig: Figure) -> str:  # markdown-exec: hide
     buffer = StringIO()  # markdown-exec: hide
     fig.savefig(buffer, format="svg")  # markdown-exec: hide
     return buffer.getvalue()  # markdown-exec: hide
 print(fig_to_html(plt.gcf())) # markdown-exec: hide
 ```
+
+## CUDA Profiling and debugging
+
+To debug your quantum programs on `CUDA` devices, `pyqtorch` offers a `DEBUG` mode, which can be activated via
+setting the `PYQ_LOG_LEVEL` environment variable.
+
+```bash
+export PYQ_LOG_LEVEL=DEBUG
+```
+
+Before running your script, make sure to install the following packages:
+
+```bash
+pip install nvidia-pyindex
+pip install nvidia-dlprof[pytorch]
+```
+For more information, check [the dlprof docs](https://docs.nvidia.com/deeplearning/frameworks/dlprof-user-guide/index.html).
```

### Comparing `pyqtorch-1.1.1/pyqtorch/apply.py` & `pyqtorch-1.1.2/pyqtorch/apply.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from string import ascii_letters as ABC
 
 import torch
 from numpy import array, log2
 from numpy.typing import NDArray
 from torch import Tensor, einsum
 
-from pyqtorch.utils import batch_first, batch_last, promote_operator
+from pyqtorch.utils import promote_operator
 
 ABC_ARRAY: NDArray = array(list(ABC))
 
 
 def apply_operator(
     state: Tensor,
     operator: Tensor,
@@ -81,8 +81,8 @@
     elif n_qubits_1 < n_qubits_2:
         op1 = promote_operator(op1, target, n_qubits_2)
     if batch_size_1 > batch_size_2:
         op2 = op2.repeat(1, 1, batch_size_1)[:, :, :batch_size_1]
     elif batch_size_2 > batch_size_1:
         op1 = op1.repeat(1, 1, batch_size_2)[:, :, :batch_size_2]
 
-    return batch_last(torch.bmm(batch_first(op1), batch_first(op2)))
+    return torch.einsum("ijb,jkb->ikb", op1, op2)
```

### Comparing `pyqtorch-1.1.1/pyqtorch/circuit.py` & `pyqtorch-1.1.2/pyqtorch/parametric.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,208 +1,262 @@
 from __future__ import annotations
 
-from functools import reduce
-from logging import getLogger
-from operator import add
-from typing import Any, Iterator
-
-from torch import Tensor, bmm, complex128, ones_like
-from torch import device as torch_device
-from torch import dtype as torch_dtype
-from torch.nn import Module, ModuleList, ParameterDict
-
-from pyqtorch.apply import apply_operator
-from pyqtorch.matrices import _dagger
-from pyqtorch.parametric import Parametric
+from typing import Any, Tuple
+
+import torch
+
+from pyqtorch.matrices import (
+    DEFAULT_MATRIX_DTYPE,
+    OPERATIONS_DICT,
+    _controlled,
+    _jacobian,
+    _unitary,
+)
 from pyqtorch.primitive import Primitive
-from pyqtorch.utils import DiffMode, State, batch_first, batch_last, inner_prod, zero_state
+from pyqtorch.utils import Operator
+
+
+class Parametric(Primitive):
+    n_params = 1
 
-logger = getLogger(__name__)
+    def __init__(
+        self,
+        generator_name: str,
+        target: int,
+        param_name: str = "",
+    ):
+        super().__init__(OPERATIONS_DICT[generator_name], target)
+        self.register_buffer("identity", OPERATIONS_DICT["I"])
+        self.param_name = param_name
 
+        def parse_values(values: dict[str, torch.Tensor] | torch.Tensor = {}) -> torch.Tensor:
+            return Parametric._expand_values(values[self.param_name])
 
-class Sequence(Module):
-    """A generic container for pyqtorch operations"""
+        def parse_tensor(values: dict[str, torch.Tensor] | torch.Tensor = {}) -> torch.Tensor:
+            return Parametric._expand_values(values)
 
-    def __init__(self, operations: list[Module]):
-        super().__init__()
-        self.operations = ModuleList(operations)
-        self._device = torch_device("cpu")
-        self._dtype = complex128
-        if len(self.operations) > 0:
-            try:
-                self._device = next(iter(set((op.device for op in self.operations))))
-            except StopIteration:
-                pass
+        self.parse_values = parse_tensor if param_name == "" else parse_values
 
-    def __iter__(self) -> Iterator:
-        return iter(self.operations)
+    def extra_repr(self) -> str:
+        return f"{self.qubit_support}, {self.param_name}"
 
     def __hash__(self) -> int:
-        return hash(reduce(add, (hash(op) for op in self.operations)))
+        return hash(self.qubit_support) + hash(self.param_name)
 
-    def forward(self, state: State, values: dict[str, Tensor] | ParameterDict = {}) -> State:
-        for op in self.operations:
-            state = op(state, values)
-        return state
-
-    @property
-    def device(self) -> torch_device:
-        return self._device
-
-    @property
-    def dtype(self) -> torch_dtype:
-        return self._dtype
-
-    def to(self, *args: Any, **kwargs: Any) -> QuantumCircuit:
-        self.operations = ModuleList([op.to(*args, **kwargs) for op in self.operations])
-        if len(self.operations) > 0:
-            self._device = self.operations[0].device
-            self._dtype = self.operations[0].dtype
-        return self
+    @staticmethod
+    def _expand_values(values: torch.Tensor) -> torch.Tensor:
+        return values.unsqueeze(0) if len(values.size()) == 0 else values
 
+    def unitary(self, values: dict[str, torch.Tensor] | torch.Tensor = {}) -> Operator:
+        thetas = self.parse_values(values)
+        batch_size = len(thetas)
+        return _unitary(thetas, self.pauli, self.identity, batch_size)
 
-class QuantumCircuit(Sequence):
-    """A QuantumCircuit defining a register / number of qubits of the full system."""
+    def jacobian(self, values: dict[str, torch.Tensor] | torch.Tensor = {}) -> Operator:
+        thetas = self.parse_values(values)
+        batch_size = len(thetas)
+        return _jacobian(thetas, self.pauli, self.identity, batch_size)
 
-    def __init__(self, n_qubits: int, operations: list[Module]):
-        super().__init__(operations)
-        self.n_qubits = n_qubits
-
-    def run(self, state: State = None, values: dict[str, Tensor] | ParameterDict = {}) -> State:
-        if state is None:
-            state = self.init_state()
-        return self.forward(state, values)
 
-    def __hash__(self) -> int:
-        return hash(reduce(add, (hash(op) for op in self.operations))) + hash(self.n_qubits)
+class RX(Parametric):
+    def __init__(
+        self,
+        target: int,
+        param_name: str = "",
+    ):
+        super().__init__("X", target, param_name)
 
-    def init_state(self, batch_size: int = 1) -> Tensor:
-        return zero_state(self.n_qubits, batch_size, device=self.device, dtype=self.dtype)
 
+class RY(Parametric):
+    def __init__(
+        self,
+        target: int,
+        param_name: str = "",
+    ):
+        super().__init__("Y", target, param_name)
 
-def expectation(
-    circuit: QuantumCircuit,
-    state: State,
-    values: dict[str, Tensor],
-    observable: QuantumCircuit,
-    diff_mode: DiffMode = DiffMode.AD,
-) -> Tensor:
-    """Compute the expectation value of the circuit given a state and observable.
-    Arguments:
-        circuit: QuantumCircuit instance
-        state: An input state
-        values: A dictionary of parameter values
-        observable: QuantumCircuit representing the observable
-        diff_mode: The differentiation mode
-    Returns:
-        A expectation value.
-    """
-    if observable is None:
-        raise ValueError("Please provide an observable to compute expectation.")
-    if state is None:
-        state = circuit.init_state(batch_size=1)
-    if diff_mode == DiffMode.AD:
-        state = circuit.run(state, values)
-        return inner_prod(state, observable.forward(state, values)).real
-    elif diff_mode == DiffMode.ADJOINT:
-        from pyqtorch.adjoint import AdjointExpectation
-
-        return AdjointExpectation.apply(circuit, observable, state, values.keys(), *values.values())
-    else:
-        raise ValueError(f"Requested diff_mode '{diff_mode}' not supported.")
-
-
-class Add(Sequence):
-    """The 'add' operation applies all 'operations' to 'state' and returns the sum of states."""
-
-    def __init__(self, operations: list[Module]):
-        super().__init__(operations=operations)
-
-    def forward(self, state: State, values: dict[str, Tensor] | ParameterDict = dict()) -> State:
-        return reduce(add, (op(state, values) for op in self.operations))
-
-
-class Merge(Sequence):
-    def __init__(
-        self,
-        operations: list[Module],
-    ):
-        """
-        Merge a sequence of single qubit operations acting on the same qubit into a single
-        einsum operation.
-
-        Arguments:
-            operations: A list of single qubit operations.
-            qubits: The target qubit.
-            n_qubits: The number of qubits in the full system.
-
-        """
-
-        if (
-            isinstance(operations, (list, ModuleList))
-            and all([isinstance(op, (Primitive, Parametric)) for op in operations])
-            and len(list(set([op.qubit_support[0] for op in operations]))) == 1
-        ):
-            # We want all operations to act on the same qubit
-
-            super().__init__(operations)
-            self.qubits = operations[0].qubit_support
-        else:
-            raise TypeError(f"Require all operations to act on a single qubit. Got: {operations}.")
-
-    def forward(self, state: Tensor, values: dict[str, Tensor] | None = None) -> Tensor:
-        batch_size = state.shape[-1]
-        if values and len(values) > 0:
-            batch_size = max(batch_size, max(list(map(len, values.values()))))
-        return apply_operator(
-            state,
-            self.unitary(values, batch_size),
-            self.qubits,
-        )
-
-    def unitary(self, values: dict[str, Tensor] | None, batch_size: int) -> Tensor:
-        def expand(operator: Tensor) -> Tensor:
-            """In case we have a sequence of batched parametric gates mixed with primitive gates,
-            we adjust the batch_dim of the primitive gates to match."""
-            return (
-                operator.repeat(1, 1, batch_size)
-                if operator.shape != (2, 2, batch_size)
-                else operator
-            )
 
-        # We reverse the list of tensors here since matmul is not commutative.
-        return batch_last(
-            reduce(
-                bmm,
-                (batch_first(expand(op.unitary(values))) for op in reversed(self.operations)),
-            )
+class RZ(Parametric):
+    def __init__(self, target: int, param_name: str = ""):
+        super().__init__("Z", target, param_name)
+
+
+class PHASE(Parametric):
+    def __init__(self, target: int, param_name: str = ""):
+        super().__init__("I", target, param_name)
+
+    def unitary(self, values: dict[str, torch.Tensor] = {}) -> Operator:
+        thetas = self.parse_values(values)
+        batch_size = len(thetas)
+        batch_mat = self.identity.unsqueeze(2).repeat(1, 1, batch_size)
+        batch_mat[1, 1, :] = torch.exp(1.0j * thetas).unsqueeze(0).unsqueeze(1)
+        return batch_mat
+
+    def jacobian(self, values: dict[str, torch.Tensor] = {}) -> Operator:
+        thetas = self.parse_values(values)
+        batch_mat = (
+            torch.zeros((2, 2), dtype=self.identity.dtype).unsqueeze(2).repeat(1, 1, len(thetas))
         )
+        batch_mat[1, 1, :] = 1j * torch.exp(1j * thetas).unsqueeze(0).unsqueeze(1)
+        return batch_mat
 
 
-class Scale(Sequence):
-    """Generic container for multiplying a 'Primitive' or 'Sequence' instance by a parameter."""
+class ControlledRotationGate(Parametric):
+    n_params = 1
 
-    def __init__(self, operations: Sequence | Primitive, param_name: str):
-        super().__init__(
-            operations.operations if isinstance(operations, Sequence) else [operations]
+    def __init__(
+        self,
+        gate: str,
+        control: int | Tuple[int, ...],
+        target: int,
+        param_name: str = "",
+    ):
+        self.control = control if isinstance(control, tuple) else (control,)
+        super().__init__(gate, target, param_name)
+        self.qubit_support = self.control + (self.target,)
+
+    def unitary(self, values: dict[str, torch.Tensor] = {}) -> Operator:
+        thetas = self.parse_values(values)
+        batch_size = len(thetas)
+        mat = _unitary(thetas, self.pauli, self.identity, batch_size)
+        return _controlled(mat, batch_size, len(self.control))
+
+    def jacobian(self, values: dict[str, torch.Tensor] = {}) -> Operator:
+        thetas = self.parse_values(values)
+        batch_size = len(thetas)
+        n_control = len(self.control)
+        jU = _jacobian(thetas, self.pauli, self.identity, batch_size)
+        n_dim = 2 ** (n_control + 1)
+        jC = (
+            torch.zeros((n_dim, n_dim), dtype=self.identity.dtype)
+            .unsqueeze(2)
+            .repeat(1, 1, batch_size)
         )
-        self.param_name = param_name
+        unitary_idx = 2 ** (n_control + 1) - 2
+        jC[unitary_idx:, unitary_idx:, :] = jU
+        return jC
 
-    def forward(self, state: Tensor, values: dict[str, Tensor] | ParameterDict = dict()) -> Tensor:
-        return (
-            values[self.param_name] * super().forward(state, values)
-            if isinstance(self.operations, Sequence)
-            else self._forward(state, values)
+
+class CRX(ControlledRotationGate):
+    def __init__(
+        self,
+        control: int | Tuple[int],
+        target: int,
+        param_name: str = "",
+    ):
+        super().__init__("X", control, target, param_name)
+
+
+class CRY(ControlledRotationGate):
+    def __init__(
+        self,
+        control: int | Tuple[int],
+        target: int,
+        param_name: str = "",
+    ):
+        super().__init__("Y", control, target, param_name)
+
+
+class CRZ(ControlledRotationGate):
+    def __init__(
+        self,
+        control: Tuple[int],
+        target: int,
+        param_name: str = "",
+    ):
+        super().__init__("Z", control, target, param_name)
+
+
+class CPHASE(ControlledRotationGate):
+    n_params = 1
+
+    def __init__(
+        self,
+        control: int | Tuple[int],
+        target: int,
+        param_name: str = "",
+    ):
+        super().__init__("I", control, target, param_name)
+
+    def unitary(self, values: dict[str, torch.Tensor] = {}) -> Operator:
+        thetas = self.parse_values(values)
+        batch_size = len(thetas)
+        mat = self.identity.unsqueeze(2).repeat(1, 1, batch_size)
+        mat[1, 1, :] = torch.exp(1.0j * thetas).unsqueeze(0).unsqueeze(1)
+        return _controlled(mat, batch_size, len(self.control))
+
+    def jacobian(self, values: dict[str, torch.Tensor] = {}) -> Operator:
+        thetas = self.parse_values(values)
+        batch_size = len(thetas)
+        n_control = len(self.control)
+        jU = torch.zeros((2, 2), dtype=self.identity.dtype).unsqueeze(2).repeat(1, 1, len(thetas))
+        jU[1, 1, :] = 1j * torch.exp(1j * thetas).unsqueeze(0).unsqueeze(1)
+        n_dim = 2 ** (n_control + 1)
+        jC = (
+            torch.zeros((n_dim, n_dim), dtype=self.identity.dtype)
+            .unsqueeze(2)
+            .repeat(1, 1, batch_size)
         )
+        unitary_idx = 2 ** (n_control + 1) - 2
+        jC[unitary_idx:, unitary_idx:, :] = jU
+        return jC
+
+    def to(self, *args: Any, **kwargs: Any) -> Primitive:
+        super().to(*args, **kwargs)
+        self._device = self.identity.device
+        return self
+
+
+class U(Parametric):
+    n_params = 3
 
-    def _forward(self, state: Tensor, values: dict[str, Tensor]) -> Tensor:
-        return apply_operator(state, self.unitary(values), self.operations[0].qubit_support)
+    def __init__(self, target: int, phi: str, theta: str, omega: str):
+        self.phi = phi
+        self.theta = theta
+        self.omega = omega
+        super().__init__("X", target, param_name="")
 
-    def unitary(self, values: dict[str, Tensor]) -> Tensor:
-        thetas = values[self.param_name]
-        return thetas * self.operations[0].unitary(values)
+        self.register_buffer(
+            "a", torch.tensor([[1, 0], [0, 0]], dtype=DEFAULT_MATRIX_DTYPE).unsqueeze(2)
+        )
+        self.register_buffer(
+            "b", torch.tensor([[0, 1], [0, 0]], dtype=DEFAULT_MATRIX_DTYPE).unsqueeze(2)
+        )
+        self.register_buffer(
+            "c", torch.tensor([[0, 0], [1, 0]], dtype=DEFAULT_MATRIX_DTYPE).unsqueeze(2)
+        )
+        self.register_buffer(
+            "d", torch.tensor([[0, 0], [0, 1]], dtype=DEFAULT_MATRIX_DTYPE).unsqueeze(2)
+        )
+
+    def unitary(self, values: dict[str, torch.Tensor] = {}) -> Operator:
+        phi, theta, omega = list(
+            map(
+                lambda t: t.unsqueeze(0) if len(t.size()) == 0 else t,
+                [values[self.phi], values[self.theta], values[self.omega]],
+            )
+        )
+        batch_size = len(theta)
 
-    def dagger(self, values: dict[str, Tensor]) -> Tensor:
-        return _dagger(self.unitary(values))
+        t_plus = torch.exp(-1j * (phi + omega) / 2)
+        t_minus = torch.exp(-1j * (phi - omega) / 2)
+        sin_t = torch.sin(theta / 2).unsqueeze(0).unsqueeze(1).repeat((2, 2, 1))
+        cos_t = torch.cos(theta / 2).unsqueeze(0).unsqueeze(1).repeat((2, 2, 1))
+
+        a = self.a.repeat(1, 1, batch_size) * cos_t * t_plus
+        b = self.b.repeat(1, 1, batch_size) * sin_t * torch.conj(t_minus)
+        c = self.c.repeat(1, 1, batch_size) * sin_t * t_minus
+        d = self.d.repeat(1, 1, batch_size) * cos_t * torch.conj(t_plus)
+        return a - b + c + d
+
+    def jacobian(self, values: dict[str, torch.Tensor] = {}) -> Operator:
+        raise NotImplementedError
+
+    def digital_decomposition(self) -> list[Parametric]:
+        return [
+            RZ(self.qubit_support[0], self.phi),
+            RY(self.qubit_support[0], self.theta),
+            RZ(self.qubit_support[0], self.omega),
+        ]
 
-    def jacobian(self, values: dict[str, Tensor]) -> Tensor:
-        return values[self.param_name] * ones_like(self.unitary(values))
+    def jacobian_decomposed(self, values: dict[str, torch.Tensor] = {}) -> list[Operator]:
+        return [op.jacobian(values) for op in self.digital_decomposition()]
```

### Comparing `pyqtorch-1.1.1/pyqtorch/matrices.py` & `pyqtorch-1.1.2/pyqtorch/matrices.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-1.1.1/pyqtorch/primitive.py` & `pyqtorch-1.1.2/pyqtorch/primitive.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 from __future__ import annotations
 
-from math import log2
+import logging
+from logging import getLogger
 from typing import Any
 
 import torch
 from torch import Tensor
 
 from pyqtorch.apply import apply_operator
 from pyqtorch.matrices import OPERATIONS_DICT, _controlled, _dagger
 from pyqtorch.utils import product_state
 
+logger = getLogger(__name__)
+
+
+def forward_hook(*args, **kwargs) -> None:  # type: ignore[no-untyped-def]
+    torch.cuda.nvtx.range_pop()
+
+
+def pre_forward_hook(*args, **kwargs) -> None:  # type: ignore[no-untyped-def]
+    torch.cuda.nvtx.range_push("Primitive.forward")
+
+
+def backward_hook(*args, **kwargs) -> None:  # type: ignore[no-untyped-def]
+    torch.cuda.nvtx.range_pop()
+
+
+def pre_backward_hook(*args, **kwargs) -> None:  # type: ignore[no-untyped-def]
+    torch.cuda.nvtx.range_push("Primitive.backward")
+
 
 class Primitive(torch.nn.Module):
     def __init__(self, pauli: Tensor, target: int) -> None:
         super().__init__()
         self.target: int = target
         self.qubit_support: tuple[int, ...] = (target,)
-        self.n_qubits: int = max(self.qubit_support)
         self.register_buffer("pauli", pauli)
-        self._param_type = None
         self._device = self.pauli.device
         self._dtype = self.pauli.dtype
 
-    def __key(self) -> tuple:
-        return self.qubit_support
-
-    def __eq__(self, other: object) -> bool:
-        if isinstance(other, type(self)):
-            return self.__key() == other.__key()
-        else:
-            return False
+        if logger.isEnabledFor(logging.DEBUG):
+            # When Debugging let's add logging and NVTX markers
+            # WARNING: incurs performance penalty
+            self.register_forward_hook(forward_hook, always_call=True)
+            self.register_full_backward_hook(backward_hook)
+            self.register_forward_pre_hook(pre_forward_hook)
+            self.register_full_backward_pre_hook(pre_backward_hook)
 
     def __hash__(self) -> int:
         return hash(self.qubit_support)
 
     def extra_repr(self) -> str:
-        return f"qubit_support={self.qubit_support}"
-
-    @property
-    def param_type(self) -> None:
-        return self._param_type
+        return f"{self.qubit_support}"
 
     def unitary(self, values: dict[str, Tensor] | Tensor = dict()) -> Tensor:
         return self.pauli.unsqueeze(2)
 
     def forward(self, state: Tensor, values: dict[str, Tensor] | Tensor = dict()) -> Tensor:
         return apply_operator(
             state, self.unitary(values), self.qubit_support, len(state.size()) - 1
@@ -128,38 +140,35 @@
 
 
 class SWAP(Primitive):
     def __init__(self, control: int, target: int):
         super().__init__(OPERATIONS_DICT["SWAP"], target)
         self.control = (control,) if isinstance(control, int) else control
         self.qubit_support = self.control + (target,)
-        self.n_qubits = max(self.qubit_support)
 
 
 class CSWAP(Primitive):
     def __init__(self, control: int | tuple[int, ...], target: int):
         super().__init__(OPERATIONS_DICT["CSWAP"], target)
         self.control = (control,) if isinstance(control, int) else control
         self.target = target
         self.qubit_support = self.control + (target,)
-        self.n_qubits = max(self.qubit_support)
 
 
 class ControlledOperationGate(Primitive):
     def __init__(self, gate: str, control: int | tuple[int, ...], target: int):
         self.control = (control,) if isinstance(control, int) else control
         mat = OPERATIONS_DICT[gate]
         mat = _controlled(
             unitary=mat.unsqueeze(2),
             batch_size=1,
-            n_control_qubits=len(self.control) - (int)(log2(mat.shape[0])) + 1,
+            n_control_qubits=len(self.control),
         ).squeeze(2)
         super().__init__(mat, target)
         self.qubit_support = self.control + (target,)
-        self.n_qubits = max(self.qubit_support)
 
 
 class CNOT(ControlledOperationGate):
     def __init__(self, control: int | tuple[int, ...], target: int):
         super().__init__("X", control, target)
```

### Comparing `pyqtorch-1.1.1/pyqtorch/utils.py` & `pyqtorch-1.1.2/pyqtorch/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,42 @@
 from __future__ import annotations
 
+import logging
 from enum import Enum
+from logging import getLogger
 from typing import Sequence
 
 import torch
 from torch import Tensor
 
 from pyqtorch.matrices import DEFAULT_MATRIX_DTYPE, DEFAULT_REAL_DTYPE
 
 State = Tensor
 Operator = Tensor
 
 ATOL = 1e-06
 RTOL = 0.0
 GRADCHECK_ATOL = 1e-06
 
+logger = getLogger(__name__)
+
 
 def inner_prod(bra: Tensor, ket: Tensor) -> Tensor:
+    if logger.isEnabledFor(logging.DEBUG):
+        logger.debug("Inner prod calculation")
+        torch.cuda.nvtx.range_push("inner_prod")
+
     n_qubits = len(bra.size()) - 1
     bra = bra.reshape((2**n_qubits, bra.size(-1)))
     ket = ket.reshape((2**n_qubits, ket.size(-1)))
-    return torch.einsum("ib,ib->b", bra.conj(), ket)
+    res = torch.einsum("ib,ib->b", bra.conj(), ket)
+    if logger.isEnabledFor(logging.DEBUG):
+        torch.cuda.nvtx.range_pop()
+        logger.debug("Inner prod complete")
+    return res
 
 
 def overlap(bra: Tensor, ket: Tensor) -> Tensor:
     return torch.pow(inner_prod(bra, ket).real, 2)
 
 
 class StrEnum(str, Enum):
@@ -121,14 +133,42 @@
     return state.reshape([2] * n_qubits + [batch_size]).to(device=device)
 
 
 def param_dict(keys: Sequence[str], values: Sequence[Tensor]) -> dict[str, Tensor]:
     return {key: val for key, val in zip(keys, values)}
 
 
+def batch_first(operator: Tensor) -> Tensor:
+    """
+    Permute the operator's batch dimension on first dimension.
+
+    Args:
+        operator (Tensor): Operator in size [2**n_qubits, 2**n_qubits,batch_size].
+
+    Returns:
+        Tensor: Operator in size [batch_size, 2**n_qubits, 2**n_qubits].
+    """
+    batch_first_perm = (2, 0, 1)
+    return torch.permute(operator, batch_first_perm)
+
+
+def batch_last(operator: Tensor) -> Tensor:
+    """
+    Permute the operator's batch dimension on last dimension.
+
+    Args:
+        operator (Tensor): Operator in size [batch_size,2**n_qubits, 2**n_qubits].
+
+    Returns:
+        Tensor: Operator in size [2**n_qubits, 2**n_qubits,batch_size].
+    """
+    undo_perm = (1, 2, 0)
+    return torch.permute(operator, undo_perm)
+
+
 def density_mat(state: Tensor) -> Tensor:
     """
     Computes the density matrix from a pure state vector.
 
     Args:
         state (Tensor): The pure state vector :math:`|\\psi\\rangle`.
 
@@ -136,16 +176,43 @@
         Tensor: The density matrix :math:`\\rho = |\psi \\rangle \\langle\\psi|`.
     """
     n_qubits = len(state.size()) - 1
     batch_dim = state.dim() - 1
     batch_size = state.shape[-1]
     batch_first_perm = [batch_dim] + list(range(batch_dim))
     state = torch.permute(state, batch_first_perm).reshape(batch_size, 2**n_qubits)
-    undo_perm = (1, 2, 0)
-    return torch.permute(torch.einsum("bi,bj->bij", (state, state.conj())), undo_perm)
+    return batch_last(torch.einsum("bi,bj->bij", (state, state.conj())))
+
+
+def operator_kron(op1: Tensor, op2: Tensor) -> Tensor:
+    """
+    Compute the Kronecker product of two operators.
+
+    Prevents errors related to the shape of the operators
+    [2**n_qubits, 2**n_qubits, batch_size] when simply using `torch.kron()`.
+    Use of `.contiguous()` to avoid errors related to the `torch.kron()` of a transposing tensor
+
+    Args:
+        op1 (Tensor): The first input tensor.
+        op2 (Tensor): The second input tensor.
+
+    Returns:
+        Tensor: The resulting tensor after applying the Kronecker product
+    """
+    batch_size_1, batch_size_2 = op1.size(2), op2.size(2)
+    if batch_size_1 > batch_size_2:
+        op2 = op2.repeat(1, 1, batch_size_1)[:, :, :batch_size_1]
+    elif batch_size_2 > batch_size_1:
+        op1 = op1.repeat(1, 1, batch_size_2)[:, :, :batch_size_2]
+    kron_product = torch.einsum(
+        "bik,bjl->bijkl", batch_first(op1).contiguous(), batch_first(op2).contiguous()
+    )
+    return batch_last(
+        kron_product.reshape(op1.size(2), op1.size(1) * op2.size(1), op1.size(0) * op2.size(0))
+    )
 
 
 def promote_operator(operator: Tensor, target: int, n_qubits: int) -> Tensor:
     from pyqtorch.primitive import I
 
     """
     Promotes `operator` to the size of the circuit (number of qubits and batch).
@@ -166,39 +233,17 @@
     if target > n_qubits - 1:
         raise ValueError("The target must be a valid qubit index within the circuit's range.")
     qubits = torch.arange(0, n_qubits)
     qubits = qubits[qubits != target]
     for qubit in qubits:
         operator = torch.where(
             target > qubit,
-            torch.kron(I(target).unitary(), operator.contiguous()),
-            torch.kron(operator.contiguous(), I(target).unitary()),
+            operator_kron(I(target).unitary(), operator),
+            operator_kron(operator, I(target).unitary()),
         )
     return operator
 
 
-def batch_first(operator: Tensor) -> Tensor:
-    """
-    Permute the operator's batch dimension on first dimension.
-
-    Args:
-        operator (Tensor): Operator in size [2**n_qubits, 2**n_qubits,batch_size].
-
-    Returns:
-        Tensor: Operator in size [batch_size, 2**n_qubits, 2**n_qubits].
-    """
-    batch_first_perm = (2, 0, 1)
-    return torch.permute(operator, batch_first_perm)
-
-
-def batch_last(operator: Tensor) -> Tensor:
-    """
-    Permute the operator's batch dimension on last dimension.
-
-    Args:
-        operator (Tensor): Operator in size [batch_size,2**n_qubits, 2**n_qubits].
-
-    Returns:
-        Tensor: Operator in size [2**n_qubits, 2**n_qubits,batch_size].
-    """
-    undo_perm = (1, 2, 0)
-    return torch.permute(operator, undo_perm)
+def add_batch_dim(operator: Tensor, batch_size: int = 1) -> Tensor:
+    """In case we have a sequence of batched parametric gates mixed with primitive gates,
+    we adjust the batch_dim of the primitive gates to match."""
+    return operator.repeat(1, 1, batch_size) if operator.shape != (2, 2, batch_size) else operator
```

### Comparing `pyqtorch-1.1.1/tests/test_analog.py` & `pyqtorch-1.1.2/tests/test_analog.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,39 +43,39 @@
 
 
 @pytest.mark.flaky(max_runs=5)
 @pytest.mark.parametrize("n_qubits, batch_size", [(2, 1), (4, 2)])
 def test_hamevo_general(n_qubits: int, batch_size: int) -> None:
     H = Hamiltonian_general(n_qubits, batch_size)
     t_evo = torch.rand(1, dtype=DEFAULT_REAL_DTYPE)
-    hamevo = pyq.HamiltonianEvolution(tuple([i for i in range(n_qubits)]), n_qubits)
+    hamevo = pyq.HamiltonianEvolution(tuple([i for i in range(n_qubits)]))
     psi = pyq.random_state(n_qubits, batch_size)
     psi_star = hamevo(H, t_evo, psi)
     assert is_normalized(psi_star, atol=ATOL)
 
 
 @pytest.mark.flaky(max_runs=5)
 def test_hamevo_single() -> None:
     n_qubits = 4
     H = Hamiltonian(1)
     t_evo = torch.tensor([torch.pi / 4], dtype=DEFAULT_MATRIX_DTYPE)
-    hamevo = pyq.HamiltonianEvolution(tuple([i for i in range(n_qubits)]), n_qubits)
+    hamevo = pyq.HamiltonianEvolution(tuple([i for i in range(n_qubits)]))
     psi = pyq.uniform_state(n_qubits)
     psi_star = hamevo(H, t_evo, psi)
     result = overlap(psi_star, psi)
     assert torch.isclose(result, torch.tensor([0.5], dtype=torch.float64), rtol=RTOL, atol=ATOL)
 
 
 @pytest.mark.flaky(max_runs=5)
 def test_hamevo_batch() -> None:
     n_qubits = 4
     batch_size = 2
     H = Hamiltonian(batch_size)
     t_evo = torch.tensor([torch.pi / 4], dtype=DEFAULT_MATRIX_DTYPE)
-    hamevo = pyq.HamiltonianEvolution(tuple([i for i in range(n_qubits)]), n_qubits)
+    hamevo = pyq.HamiltonianEvolution(tuple([i for i in range(n_qubits)]))
     psi = pyq.uniform_state(n_qubits, batch_size)
     psi_star = hamevo(H, t_evo, psi)
     result = overlap(psi_star, psi)
     assert torch.allclose(
         result, torch.tensor([0.5, 0.5], dtype=torch.float64), rtol=RTOL, atol=ATOL
     )
 
@@ -112,15 +112,15 @@
 def test_hamiltonianevolution_with_types(
     H: torch.Tensor,
     t_evo: torch.Tensor,
     target: torch.Tensor,
     batch_size: int,
 ) -> None:
     n_qubits = 4
-    hamevo = pyq.HamiltonianEvolution(tuple([i for i in range(n_qubits)]), n_qubits)
+    hamevo = pyq.HamiltonianEvolution(tuple([i for i in range(n_qubits)]))
     psi = pyq.uniform_state(n_qubits)
     psi_star = hamevo(H, t_evo, psi)
     result = overlap(psi_star, psi)
     assert result.size() == (batch_size,)
     assert torch.allclose(result, target, rtol=RTOL, atol=ATOL)
 
 
@@ -132,15 +132,15 @@
             [0.0000, 0.9701, 0.0000, 0.7078],
             [0.4594, 0.0000, 0.9207, 0.0000],
             [0.0000, 0.4594, 0.0000, 0.9207],
         ],
         dtype=torch.complex128,
     )
     iszero = torch.tensor([False, True, False, True])
-    op = pyq.HamiltonianEvolution(qubit_support=(0, 1), n_qubits=2)
+    op = pyq.HamiltonianEvolution(qubit_support=(0, 1))
     st = op(h, t, pyq.zero_state(2)).flatten()
     assert torch.allclose(
         st[iszero], torch.zeros(1, dtype=DEFAULT_MATRIX_DTYPE), rtol=RTOL, atol=ATOL
     )
 
     h = torch.tensor(
         [
@@ -148,12 +148,12 @@
             [0.4594, 0.9207, 0.0000, 0.0000],
             [0.0000, 0.0000, 0.9701, 0.7078],
             [0.0000, 0.0000, 0.4594, 0.9207],
         ],
         dtype=torch.complex128,
     )
     iszero = torch.tensor([False, False, True, True])
-    op = pyq.HamiltonianEvolution(qubit_support=(0, 1), n_qubits=2)
+    op = pyq.HamiltonianEvolution(qubit_support=(0, 1))
     st = op(h, t, pyq.zero_state(2)).flatten()
     assert torch.allclose(
         st[iszero], torch.zeros(1, dtype=DEFAULT_MATRIX_DTYPE), rtol=RTOL, atol=ATOL
     )
```

### Comparing `pyqtorch-1.1.1/tests/test_circuit.py` & `pyqtorch-1.1.2/tests/test_circuit.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import random
 
 import pytest
 import torch
 
 import pyqtorch as pyq
-from pyqtorch.circuit import DiffMode, expectation
+from pyqtorch import DiffMode, expectation
 from pyqtorch.matrices import COMPLEX_TO_REAL_DTYPES
 from pyqtorch.utils import GRADCHECK_ATOL
 
 
 def test_adjoint_diff() -> None:
     rx = pyq.RX(0, param_name="theta_0")
     cry = pyq.CPHASE(0, 1, param_name="theta_1")
@@ -151,26 +151,54 @@
     scaledwf_primitive = pyq.Scale(gate, "scale")(state, values)
     scaledwf_composite = pyq.Scale(pyq.Sequence([gate]), "scale")(state, values)
     assert torch.allclose(wf, scaledwf_primitive)
     assert torch.allclose(wf, scaledwf_composite)
 
 
 def test_add() -> None:
-    x = pyq.X(0)
-    z = pyq.Z(1)
-    state = pyq.zero_state(2)
-    assert torch.allclose(pyq.Add([x, z])(state), x(state) + z(state))
+    num_gates = 2
+    fns = [pyq.X, pyq.Y, pyq.Z, pyq.S, pyq.H, pyq.T]
+    ops = []
+    n_qubits = torch.randint(low=1, high=4, size=(1,)).item()
+    state = pyq.random_state(n_qubits)
+    chosen_gate_ids = torch.randint(0, len(fns) - 1, size=(num_gates,))
+    for id in chosen_gate_ids:
+        target = random.choice([i for i in range(n_qubits)])
+        ops.append(fns[id](target))
+
+    assert torch.allclose(pyq.Add(ops)(state), ops[0](state) + ops[1](state))
 
 
 def test_merge() -> None:
     ops = [pyq.RX(0, "theta_0"), pyq.RY(0, "theta_1"), pyq.RX(0, "theta_2")]
     circ = pyq.QuantumCircuit(2, ops)
     mergecirc = pyq.Merge(ops)
     state = pyq.random_state(2)
     values = {f"theta_{i}": torch.rand(1) for i in range(3)}
     assert torch.allclose(circ(state, values), mergecirc(state, values))
 
 
-@pytest.mark.xfail(reason="Can only merge gate acting on the same qubit support.")
-def test_merge_expect_fail() -> None:
+@pytest.mark.xfail(reason="Can only merge single qubit gates acting on the same qubit support.")
+def test_merge_different_sup_expect_fail() -> None:
     ops = [pyq.RX(0, "theta_0"), pyq.RY(1, "theta_1")]
     mergecirc = pyq.Merge(ops)
+
+
+@pytest.mark.xfail(reason="Can only merge single qubit gates acting on the same qubit support.")
+def test_merge_multiqubit_expect_fail() -> None:
+    ops = [pyq.CNOT(0, 1), pyq.RY(1, "theta_1")]
+    mergecirc = pyq.Merge(ops)
+
+
+@pytest.mark.parametrize("batch_size", [1, 2, 3])
+def test_merge_different_batchsize(batch_size: int) -> None:
+    ops = [pyq.X(0), pyq.RX(0, "theta_0")]
+    mergecirc = pyq.Merge(ops)
+    for bs in [1, batch_size]:
+        mergecirc(pyq.random_state(2, bs), {"theta_0": torch.rand(batch_size)})
+        mergecirc(pyq.random_state(2, batch_size), {"theta_0": torch.rand(bs)})
+
+
+@pytest.mark.xfail(reason="Hamiltonians can only be constructed from Scale, Add and Primitive.")
+def test_ham_expect_fail() -> None:
+    ops = [pyq.Z(0), pyq.RY(1, "theta_1")]
+    ham = pyq.Hamiltonian(ops)
```

### Comparing `pyqtorch-1.1.1/tests/test_digital.py` & `pyqtorch-1.1.2/tests/test_digital.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,18 +6,25 @@
 
 import pytest
 import torch
 from torch import Tensor
 
 import pyqtorch as pyq
 from pyqtorch.apply import apply_operator, operator_product
-from pyqtorch.matrices import DEFAULT_MATRIX_DTYPE, IMAT, ZMAT, _dagger
+from pyqtorch.matrices import DEFAULT_MATRIX_DTYPE, HMAT, IMAT, XMAT, YMAT, ZMAT, _dagger
 from pyqtorch.parametric import Parametric
-from pyqtorch.primitive import Primitive
-from pyqtorch.utils import ATOL, density_mat, product_state, promote_operator, random_state
+from pyqtorch.primitive import H, I, Primitive, X, Y, Z
+from pyqtorch.utils import (
+    ATOL,
+    density_mat,
+    operator_kron,
+    product_state,
+    promote_operator,
+    random_state,
+)
 
 state_000 = product_state("000")
 state_001 = product_state("001")
 state_100 = product_state("100")
 state_101 = product_state("101")
 state_110 = product_state("110")
 state_111 = product_state("111")
@@ -221,15 +228,15 @@
 def test_parametric_phase_hamevo(
     state_fn: Callable, batch_size: int = 1, n_qubits: int = 1
 ) -> None:
     target = 0
     state = state_fn(n_qubits, batch_size=batch_size)
     phi = torch.rand(1, dtype=DEFAULT_MATRIX_DTYPE)
     H = (ZMAT - IMAT) / 2
-    hamevo = pyq.HamiltonianEvolution(qubit_support=(target,), n_qubits=n_qubits)
+    hamevo = pyq.HamiltonianEvolution(qubit_support=(target,))
     phase = pyq.PHASE(target, "phi")
     assert torch.allclose(phase(state, {"phi": phi}), hamevo(H, phi, state))
 
 
 @pytest.mark.parametrize("state_fn", [pyq.random_state, pyq.zero_state, pyq.uniform_state])
 @pytest.mark.parametrize("batch_size", [1, 2, 4])
 @pytest.mark.parametrize("n_qubits", [1, 2, 4])
@@ -338,7 +345,49 @@
     op_mul = operator_product(
         gate(target).unitary().repeat(1, 1, batch_size_2), _dagger(op_prom), target
     )
     assert op_mul.size() == torch.Size([2**n_qubits, 2**n_qubits, max_batch])
     assert torch.allclose(
         op_mul, torch.eye(2**n_qubits, dtype=torch.cdouble).unsqueeze(2).repeat(1, 1, max_batch)
     )
+
+
+@pytest.mark.parametrize("operator,matrix", [(I, IMAT), (X, XMAT), (Z, ZMAT), (Y, YMAT), (H, HMAT)])
+def test_operator_kron(operator: Tensor, matrix: Tensor) -> None:
+    n_qubits = torch.randint(low=1, high=5, size=(1,)).item()
+    batch_size = torch.randint(low=1, high=5, size=(1,)).item()
+    states, krons = [], []
+    for batch in range(batch_size):
+        state = random_state(n_qubits)
+        states.append(state)
+        kron = torch.kron(density_mat(state).squeeze(), matrix).unsqueeze(2)
+        krons.append(kron)
+    input_state = torch.cat(states, dim=n_qubits)
+    kron_out = operator_kron(density_mat(input_state), operator(0).dagger())
+    assert kron_out.size() == torch.Size([2 ** (n_qubits + 1), 2 ** (n_qubits + 1), batch_size])
+    kron_expect = torch.cat(krons, dim=2)
+    assert torch.allclose(kron_out, kron_expect)
+    assert torch.allclose(
+        torch.kron(operator(0).dagger().contiguous(), I(0).unitary()),
+        operator_kron(operator(0).dagger(), I(0).unitary()),
+    )
+
+
+def test_kron_batch() -> None:
+    n_qubits = torch.randint(low=1, high=5, size=(1,)).item()
+    batch_size_1 = torch.randint(low=1, high=5, size=(1,)).item()
+    batch_size_2 = torch.randint(low=1, high=5, size=(1,)).item()
+    max_batch = max(batch_size_1, batch_size_2)
+    dm_1 = density_mat(random_state(n_qubits, batch_size_1))
+    dm_2 = density_mat(random_state(n_qubits, batch_size_2))
+    dm_out = operator_kron(dm_1, dm_2)
+    assert dm_out.size() == torch.Size([2 ** (2 * n_qubits), 2 ** (2 * n_qubits), max_batch])
+    if batch_size_1 > batch_size_2:
+        dm_2 = dm_2.repeat(1, 1, batch_size_1)[:, :, :batch_size_1]
+    elif batch_size_2 > batch_size_1:
+        dm_1 = dm_1.repeat(1, 1, batch_size_2)[:, :, :batch_size_2]
+    density_matrices = []
+    for batch in range(max_batch):
+        density_matrice = torch.kron(dm_1[:, :, batch], dm_2[:, :, batch]).unsqueeze(2)
+        density_matrices.append(density_matrice)
+    dm_expect = torch.cat(density_matrices, dim=2)
+    assert torch.allclose(dm_out, dm_expect)
```

### Comparing `pyqtorch-1.1.1/.gitignore` & `pyqtorch-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyqtorch-1.1.1/LICENSE` & `pyqtorch-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqtorch-1.1.1/pyproject.toml` & `pyqtorch-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     { name = "Dominik Seitz", email = "dominik.seitz@pasqal.com" },
     { name = "Niklas Heim", email = "niklas.heim@pasqal.com" },
     { name = "Roland Guichard", email = "roland.guichard@pasqal.com" },
     { name = "Joao P. Moutinho", email = "joao.moutinho@pasqal.com"},
 ]
 requires-python = ">=3.8,<3.13"
 license = {text = "Apache 2.0"}
-version = "1.1.1"
+version = "1.1.2"
 classifiers=[
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -59,28 +59,28 @@
 ]
 
 [tool.hatch.envs.docs.scripts]
 build = "mkdocs build --clean --strict"
 serve = "mkdocs serve --dev-addr localhost:8000"
 
 [tool.ruff]
-select = ["E", "F", "I", "Q"]
-extend-ignore = ["F841"]
+lint.select = ["E", "F", "I", "Q"]
+lint.extend-ignore = ["F841"]
 line-length = 100
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 required-imports = ["from __future__ import annotations"]
 
-[tool.ruff.per-file-ignores]
-"__init__.py" = ["F401"]
+[tool.ruff.lint.per-file-ignores]
+"__init__.py" = ["F401", "E402"]
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 15
 
-[tool.ruff.flake8-quotes]
+[tool.ruff.lint.flake8-quotes]
 docstring-quotes = "double"
 
 [tool.black]
 line-length = 100
 include = '\.pyi?$'
 exclude = '''
 /(
```

### Comparing `pyqtorch-1.1.1/PKG-INFO` & `pyqtorch-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyqtorch
-Version: 1.1.1
+Version: 1.1.2
 Summary: An efficient, large-scale emulator designed for quantum machine learning, seamlessly integrated with a PyTorch backend. Please refer to https://pyqtorch.readthedocs.io/en/latest/ for setup and usage info, along with the full documentation.
 Author-email: Slimane Thabet <slimane.thabet@pasqal.com>, Aleksander Wennersteen <aleksander.wennersteen@pasqal.com>, Mario Dagrada <mario.dagrada@pasqal.com>, Dominik Seitz <dominik.seitz@pasqal.com>, Niklas Heim <niklas.heim@pasqal.com>, Roland Guichard <roland.guichard@pasqal.com>, "Joao P. Moutinho" <joao.moutinho@pasqal.com>
 License: Apache 2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

