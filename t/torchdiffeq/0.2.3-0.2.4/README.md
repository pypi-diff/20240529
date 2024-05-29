# Comparing `tmp/torchdiffeq-0.2.3.tar.gz` & `tmp/torchdiffeq-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchdiffeq-0.2.3.tar", last modified: Fri Apr 22 15:21:15 2022, max compression
+gzip compressed data, was "torchdiffeq-0.2.4.tar", last modified: Wed May 29 14:57:41 2024, max compression
```

## Comparing `torchdiffeq-0.2.3.tar` & `torchdiffeq-0.2.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 rtqichen (1185200601) rtqichen (1185200601)        0 2022-04-22 15:21:15.929434 torchdiffeq-0.2.3/
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)     1075 2022-01-17 18:00:02.000000 torchdiffeq-0.2.3/LICENSE
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)      426 2022-04-22 15:21:15.928149 torchdiffeq-0.2.3/PKG-INFO
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)     6839 2022-01-17 18:00:02.000000 torchdiffeq-0.2.3/README.md
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)       38 2022-04-22 15:21:15.930455 torchdiffeq-0.2.3/setup.cfg
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)      979 2022-01-17 18:00:03.000000 torchdiffeq-0.2.3/setup.py
-drwxrwxr-x   0 rtqichen (1185200601) rtqichen (1185200601)        0 2022-04-22 15:21:15.831189 torchdiffeq-0.2.3/torchdiffeq/
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)      114 2022-04-22 15:20:25.000000 torchdiffeq-0.2.3/torchdiffeq/__init__.py
-drwxrwxr-x   0 rtqichen (1185200601) rtqichen (1185200601)        0 2022-04-22 15:21:15.923668 torchdiffeq-0.2.3/torchdiffeq/_impl/
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)       77 2022-01-17 18:00:03.000000 torchdiffeq-0.2.3/torchdiffeq/_impl/__init__.py
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)      577 2022-01-17 18:00:03.000000 torchdiffeq-0.2.3/torchdiffeq/_impl/adaptive_heun.py
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)    13067 2022-01-17 18:00:03.000000 torchdiffeq-0.2.3/torchdiffeq/_impl/adjoint.py
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)      751 2022-01-17 18:00:03.000000 torchdiffeq-0.2.3/torchdiffeq/_impl/bosh3.py
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)     1477 2022-01-17 18:00:03.000000 torchdiffeq-0.2.3/torchdiffeq/_impl/dopri5.py
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)     4806 2022-01-17 18:00:03.000000 torchdiffeq-0.2.3/torchdiffeq/_impl/dopri8.py
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)     1051 2022-01-17 18:00:03.000000 torchdiffeq-0.2.3/torchdiffeq/_impl/event_handling.py
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)      678 2022-01-17 18:00:03.000000 torchdiffeq-0.2.3/torchdiffeq/_impl/fehlberg2.py
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)    12047 2022-01-17 18:00:03.000000 torchdiffeq-0.2.3/torchdiffeq/_impl/fixed_adams.py
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)      874 2022-01-17 18:00:03.000000 torchdiffeq-0.2.3/torchdiffeq/_impl/fixed_grid.py
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)     1808 2022-01-17 18:00:03.000000 torchdiffeq-0.2.3/torchdiffeq/_impl/interp.py
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)    11534 2022-01-17 18:00:03.000000 torchdiffeq-0.2.3/torchdiffeq/_impl/misc.py
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)     6181 2022-01-17 18:00:03.000000 torchdiffeq-0.2.3/torchdiffeq/_impl/odeint.py
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)    13745 2022-01-17 20:14:49.000000 torchdiffeq-0.2.3/torchdiffeq/_impl/rk_common.py
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)     1601 2022-01-17 18:00:03.000000 torchdiffeq-0.2.3/torchdiffeq/_impl/scipy_wrapper.py
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)     5884 2022-01-17 18:00:03.000000 torchdiffeq-0.2.3/torchdiffeq/_impl/solvers.py
-drwxrwxr-x   0 rtqichen (1185200601) rtqichen (1185200601)        0 2022-04-22 15:21:15.854611 torchdiffeq-0.2.3/torchdiffeq.egg-info/
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)      426 2022-04-22 15:21:15.000000 torchdiffeq-0.2.3/torchdiffeq.egg-info/PKG-INFO
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)      710 2022-04-22 15:21:15.000000 torchdiffeq-0.2.3/torchdiffeq.egg-info/SOURCES.txt
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)        1 2022-04-22 15:21:15.000000 torchdiffeq-0.2.3/torchdiffeq.egg-info/dependency_links.txt
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)       26 2022-04-22 15:21:15.000000 torchdiffeq-0.2.3/torchdiffeq.egg-info/requires.txt
--rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)       12 2022-04-22 15:21:15.000000 torchdiffeq-0.2.3/torchdiffeq.egg-info/top_level.txt
+drwxrwxr-x   0 rtqichen (1185200601) rtqichen (1185200601)        0 2024-05-29 14:57:41.482805 torchdiffeq-0.2.4/
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)     1075 2022-01-17 18:00:02.000000 torchdiffeq-0.2.4/LICENSE
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)      381 2024-05-29 14:57:41.481571 torchdiffeq-0.2.4/PKG-INFO
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)     7712 2022-12-27 16:45:12.000000 torchdiffeq-0.2.4/README.md
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)       38 2024-05-29 14:57:41.483611 torchdiffeq-0.2.4/setup.cfg
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)      979 2022-11-16 16:15:35.000000 torchdiffeq-0.2.4/setup.py
+drwxrwxr-x   0 rtqichen (1185200601) rtqichen (1185200601)        0 2024-05-29 14:57:41.405169 torchdiffeq-0.2.4/torchdiffeq/
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)      146 2023-10-19 19:23:02.000000 torchdiffeq-0.2.4/torchdiffeq/__init__.py
+drwxrwxr-x   0 rtqichen (1185200601) rtqichen (1185200601)        0 2024-05-29 14:57:41.477744 torchdiffeq-0.2.4/torchdiffeq/_impl/
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)       91 2023-10-19 19:23:16.000000 torchdiffeq-0.2.4/torchdiffeq/_impl/__init__.py
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)      577 2022-01-17 18:00:03.000000 torchdiffeq-0.2.4/torchdiffeq/_impl/adaptive_heun.py
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)    13496 2023-02-18 18:20:17.000000 torchdiffeq-0.2.4/torchdiffeq/_impl/adjoint.py
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)      751 2022-01-17 18:00:03.000000 torchdiffeq-0.2.4/torchdiffeq/_impl/bosh3.py
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)     1477 2022-01-17 18:00:03.000000 torchdiffeq-0.2.4/torchdiffeq/_impl/dopri5.py
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)     4806 2022-01-17 18:00:03.000000 torchdiffeq-0.2.4/torchdiffeq/_impl/dopri8.py
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)     1051 2023-02-18 17:57:31.000000 torchdiffeq-0.2.4/torchdiffeq/_impl/event_handling.py
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)      678 2022-01-17 18:00:03.000000 torchdiffeq-0.2.4/torchdiffeq/_impl/fehlberg2.py
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)    12047 2022-01-17 18:00:03.000000 torchdiffeq-0.2.4/torchdiffeq/_impl/fixed_adams.py
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)     1359 2023-08-30 12:58:17.000000 torchdiffeq-0.2.4/torchdiffeq/_impl/fixed_grid.py
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)     1808 2022-01-17 18:00:03.000000 torchdiffeq-0.2.4/torchdiffeq/_impl/interp.py
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)    13364 2023-04-06 15:41:30.000000 torchdiffeq-0.2.4/torchdiffeq/_impl/misc.py
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)     7899 2023-10-19 19:22:09.000000 torchdiffeq-0.2.4/torchdiffeq/_impl/odeint.py
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)    15609 2023-08-30 13:02:48.000000 torchdiffeq-0.2.4/torchdiffeq/_impl/rk_common.py
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)     1850 2022-07-30 02:25:18.000000 torchdiffeq-0.2.4/torchdiffeq/_impl/scipy_wrapper.py
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)     6088 2023-02-19 02:35:56.000000 torchdiffeq-0.2.4/torchdiffeq/_impl/solvers.py
+drwxrwxr-x   0 rtqichen (1185200601) rtqichen (1185200601)        0 2024-05-29 14:57:41.421406 torchdiffeq-0.2.4/torchdiffeq.egg-info/
+-rw-r--r--   0 rtqichen (1185200601) rtqichen (1185200601)      381 2024-05-29 14:57:41.000000 torchdiffeq-0.2.4/torchdiffeq.egg-info/PKG-INFO
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)      710 2024-05-29 14:57:41.000000 torchdiffeq-0.2.4/torchdiffeq.egg-info/SOURCES.txt
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)        1 2024-05-29 14:57:41.000000 torchdiffeq-0.2.4/torchdiffeq.egg-info/dependency_links.txt
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)       26 2024-05-29 14:57:41.000000 torchdiffeq-0.2.4/torchdiffeq.egg-info/requires.txt
+-rw-rw-r--   0 rtqichen (1185200601) rtqichen (1185200601)       12 2024-05-29 14:57:41.000000 torchdiffeq-0.2.4/torchdiffeq.egg-info/top_level.txt
```

### Comparing `torchdiffeq-0.2.3/LICENSE` & `torchdiffeq-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `torchdiffeq-0.2.3/README.md` & `torchdiffeq-0.2.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -66,19 +66,19 @@
  - `event_fn(t, y)` returns a tensor, and is a required keyword argument.
  - `reverse_time` is a boolean specifying whether we should solve in reverse time. Default is `False`.
  - `odeint_interface` is one of `odeint` or `odeint_adjoint`, specifying whether adjoint mode should be used for differentiating through the ODE solution. Default is `odeint`.
  - `**kwargs`: any remaining keyword arguments are passed to `odeint_interface`.
 
 The solve is terminated at an event time `t` and state `y` when an element of `event_fn(t, y)` is equal to zero. Multiple outputs from `event_fn` can be used to specify multiple event functions, of which the first to trigger will terminate the solve.
 
-Both the event time and final state are returned from `odeint_event`, and can be differentiated. Gradients will be backpropagated through the event function.
+Both the event time and final state are returned from `odeint_event`, and can be differentiated. Gradients will be backpropagated through the event function. **NOTE**: parameters for the event function must be in the state itself to obtain gradients. 
 
 The numerical precision for the event time is determined by the `atol` argument.
 
-See example of simulating and differentiating through a bouncing ball in [`examples/bouncing_ball.py`](./examples/bouncing_ball.py).
+See example of simulating and differentiating through a bouncing ball in [`examples/bouncing_ball.py`](./examples/bouncing_ball.py). See example code for learning a simple event function in [`examples/learn_physics.py`](./examples/learn_physics.py).
 
 <p align="center">
 <img align="middle" src="./assets/bouncing_ball.png" alt="Bouncing Ball" width="500" height="250" />
 </p>
 
 ## Keyword arguments for odeint(_adjoint)
 
@@ -114,29 +114,53 @@
 ## Further documentation
 For details of the adjoint-specific and solver-specific options, check out the [further documentation](FURTHER_DOCUMENTATION.md).
 
 ## References
 
 Applications of differentiable ODE solvers and event handling are discussed in these two papers:
 
-[1] Ricky T. Q. Chen, Yulia Rubanova, Jesse Bettencourt, David Duvenaud. "Neural Ordinary Differential Equations." *Advances in Neural Information Processing Systems.* 2018. [[arxiv]](https://arxiv.org/abs/1806.07366)
+Ricky T. Q. Chen, Yulia Rubanova, Jesse Bettencourt, David Duvenaud. "Neural Ordinary Differential Equations." *Advances in Neural Information Processing Systems.* 2018. [[arxiv]](https://arxiv.org/abs/1806.07366)
 
-[2] Ricky T. Q. Chen, Brandon Amos, Maximilian Nickel. "Learning Neural Event Functions for Ordinary Differential Equations." *International Conference on Learning Representations.* 2021. [[arxiv]](https://arxiv.org/abs/2011.03902)
-
----
-
-If you found this library useful in your research, please consider citing.
 ```
 @article{chen2018neuralode,
   title={Neural Ordinary Differential Equations},
   author={Chen, Ricky T. Q. and Rubanova, Yulia and Bettencourt, Jesse and Duvenaud, David},
   journal={Advances in Neural Information Processing Systems},
   year={2018}
 }
+```
 
+Ricky T. Q. Chen, Brandon Amos, Maximilian Nickel. "Learning Neural Event Functions for Ordinary Differential Equations." *International Conference on Learning Representations.* 2021. [[arxiv]](https://arxiv.org/abs/2011.03902)
+
+```
 @article{chen2021eventfn,
   title={Learning Neural Event Functions for Ordinary Differential Equations},
   author={Chen, Ricky T. Q. and Amos, Brandon and Nickel, Maximilian},
   journal={International Conference on Learning Representations},
   year={2021}
 }
 ```
+
+The seminorm option for computing adjoints is discussed in
+
+Patrick Kidger, Ricky T. Q. Chen, Terry Lyons. "'Hey, that’s not an ODE': Faster ODE Adjoints via Seminorms." *International Conference on Machine
+Learning.* 2021. [[arxiv]](https://arxiv.org/abs/2009.09457)
+```
+@article{kidger2021hey,
+  title={"Hey, that's not an ODE": Faster ODE Adjoints via Seminorms.},
+  author={Kidger, Patrick and Chen, Ricky T. Q. and Lyons, Terry J.},
+  journal={International Conference on Machine Learning},
+  year={2021}
+}
+```
+
+---
+
+If you found this library useful in your research, please consider citing.
+```
+@misc{torchdiffeq,
+	author={Chen, Ricky T. Q.},
+	title={torchdiffeq},
+	year={2018},
+	url={https://github.com/rtqichen/torchdiffeq},
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torchdiffeq-0.2.3/setup.py` & `torchdiffeq-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,14 @@
     name="torchdiffeq",
     version=version,
     author="Ricky Tian Qi Chen",
     author_email="rtqichen@cs.toronto.edu",
     description="ODE solvers and adjoint sensitivity analysis in PyTorch.",
     url="https://github.com/rtqichen/torchdiffeq",
     packages=setuptools.find_packages(),
-    install_requires=['torch>=1.3.0', 'scipy>=1.4.0'],
+    install_requires=['torch>=1.5.0', 'scipy>=1.4.0'],
     python_requires='~=3.6',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
 )
```

### Comparing `torchdiffeq-0.2.3/torchdiffeq/_impl/adaptive_heun.py` & `torchdiffeq-0.2.4/torchdiffeq/_impl/adaptive_heun.py`

 * *Files identical despite different names*

### Comparing `torchdiffeq-0.2.3/torchdiffeq/_impl/adjoint.py` & `torchdiffeq-0.2.4/torchdiffeq/_impl/adjoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import warnings
 import torch
 import torch.nn as nn
 from .odeint import SOLVERS, odeint
-from .misc import _check_inputs, _flat_to_shape
-from .misc import _mixed_norm
+from .misc import _check_inputs, _flat_to_shape, _mixed_norm, _all_callback_names, _all_adjoint_callback_names
 
 
 class OdeintAdjointMethod(torch.autograd.Function):
 
     @staticmethod
     def forward(ctx, shapes, func, y0, t, rtol, atol, method, options, event_fn, adjoint_rtol, adjoint_atol, adjoint_method,
                 adjoint_options, t_requires_grad, *adjoint_params):
@@ -101,14 +100,23 @@
                 vjp_t = torch.zeros_like(t) if vjp_t is None else vjp_t
                 vjp_y = torch.zeros_like(y) if vjp_y is None else vjp_y
                 vjp_params = [torch.zeros_like(param) if vjp_param is None else vjp_param
                               for param, vjp_param in zip(adjoint_params, vjp_params)]
 
                 return (vjp_t, func_eval, vjp_y, *vjp_params)
 
+            # Add adjoint callbacks
+            for callback_name, adjoint_callback_name in zip(_all_callback_names, _all_adjoint_callback_names):
+                try:
+                    callback = getattr(func, adjoint_callback_name)
+                except AttributeError:
+                    pass
+                else:
+                    setattr(augmented_dynamics, callback_name, callback)
+
             ##################################
             #       Solve adjoint ODE        #
             ##################################
 
             if t_requires_grad:
                 time_vjps = torch.empty(len(t), dtype=t.dtype, device=t.device)
             else:
```

### Comparing `torchdiffeq-0.2.3/torchdiffeq/_impl/bosh3.py` & `torchdiffeq-0.2.4/torchdiffeq/_impl/bosh3.py`

 * *Files identical despite different names*

### Comparing `torchdiffeq-0.2.3/torchdiffeq/_impl/dopri5.py` & `torchdiffeq-0.2.4/torchdiffeq/_impl/dopri5.py`

 * *Files identical despite different names*

### Comparing `torchdiffeq-0.2.3/torchdiffeq/_impl/dopri8.py` & `torchdiffeq-0.2.4/torchdiffeq/_impl/dopri8.py`

 * *Files identical despite different names*

### Comparing `torchdiffeq-0.2.3/torchdiffeq/_impl/event_handling.py` & `torchdiffeq-0.2.4/torchdiffeq/_impl/event_handling.py`

 * *Files identical despite different names*

### Comparing `torchdiffeq-0.2.3/torchdiffeq/_impl/fehlberg2.py` & `torchdiffeq-0.2.4/torchdiffeq/_impl/fehlberg2.py`

 * *Files identical despite different names*

### Comparing `torchdiffeq-0.2.3/torchdiffeq/_impl/fixed_adams.py` & `torchdiffeq-0.2.4/torchdiffeq/_impl/fixed_adams.py`

 * *Files identical despite different names*

### Comparing `torchdiffeq-0.2.3/torchdiffeq/_impl/fixed_grid.py` & `torchdiffeq-0.2.4/torchdiffeq/_impl/fixed_grid.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .solvers import FixedGridODESolver
-from .rk_common import rk4_alt_step_func
+from .rk_common import rk4_alt_step_func, rk3_step_func
 from .misc import Perturb
 
 
 class Euler(FixedGridODESolver):
     order = 1
 
     def _step_func(self, func, t0, dt, t1, y0):
@@ -23,7 +23,23 @@
 
 class RK4(FixedGridODESolver):
     order = 4
 
     def _step_func(self, func, t0, dt, t1, y0):
         f0 = func(t0, y0, perturb=Perturb.NEXT if self.perturb else Perturb.NONE)
         return rk4_alt_step_func(func, t0, dt, t1, y0, f0=f0, perturb=self.perturb), f0
+
+
+class Heun3(FixedGridODESolver):
+    order = 3
+
+    def _step_func(self, func, t0, dt, t1, y0):
+        f0 = func(t0, y0, perturb=Perturb.NEXT if self.perturb else Perturb.NONE)
+
+        butcher_tableu = [
+            [0.0, 0.0, 0.0, 0.0],
+            [1/3, 1/3, 0.0, 0.0],
+            [2/3, 0.0, 2/3, 0.0],
+            [0.0, 1/4, 0.0, 3/4],
+        ]
+
+        return rk3_step_func(func, t0, dt, t1, y0, butcher_tableu=butcher_tableu, f0=f0, perturb=self.perturb), f0
```

### Comparing `torchdiffeq-0.2.3/torchdiffeq/_impl/interp.py` & `torchdiffeq-0.2.4/torchdiffeq/_impl/interp.py`

 * *Files identical despite different names*

### Comparing `torchdiffeq-0.2.3/torchdiffeq/_impl/misc.py` & `torchdiffeq-0.2.4/torchdiffeq/_impl/misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,25 +2,29 @@
 import math
 import numpy as np
 import torch
 import warnings
 from .event_handling import combine_event_functions
 
 
+_all_callback_names = ['callback_step', 'callback_accept_step', 'callback_reject_step']
+_all_adjoint_callback_names = [name + '_adjoint' for name in _all_callback_names]
+_null_callback = lambda *args, **kwargs: None
+
 def _handle_unused_kwargs(solver, unused_kwargs):
     if len(unused_kwargs) > 0:
         warnings.warn('{}: Unexpected arguments {}'.format(solver.__class__.__name__, unused_kwargs))
 
 
 def _linf_norm(tensor):
-    return tensor.max()
+    return tensor.abs().max()
 
 
 def _rms_norm(tensor):
-    return tensor.pow(2).mean().sqrt()
+    return tensor.abs().pow(2).mean().sqrt()
 
 
 def _zero_norm(tensor):
     return 0.
 
 
 def _mixed_norm(tensor_tuple):
@@ -39,45 +43,47 @@
     .. [1] E. Hairer, S. P. Norsett G. Wanner, "Solving Ordinary Differential
            Equations I: Nonstiff Problems", Sec. II.4, 2nd edition.
     """
 
     dtype = y0.dtype
     device = y0.device
     t_dtype = t0.dtype
-    t0 = t0.to(dtype)
+    t0 = t0.to(t_dtype)
 
     if f0 is None:
         f0 = func(t0, y0)
 
     scale = atol + torch.abs(y0) * rtol
 
-    d0 = norm(y0 / scale)
-    d1 = norm(f0 / scale)
+    d0 = norm(y0 / scale).abs()
+    d1 = norm(f0 / scale).abs()
 
     if d0 < 1e-5 or d1 < 1e-5:
         h0 = torch.tensor(1e-6, dtype=dtype, device=device)
     else:
         h0 = 0.01 * d0 / d1
+    h0 = h0.abs()
 
     y1 = y0 + h0 * f0
     f1 = func(t0 + h0, y1)
 
-    d2 = norm((f1 - f0) / scale) / h0
+    d2 = torch.abs(norm((f1 - f0) / scale) / h0)
 
     if d1 <= 1e-15 and d2 <= 1e-15:
         h1 = torch.max(torch.tensor(1e-6, dtype=dtype, device=device), h0 * 1e-3)
     else:
         h1 = (0.01 / max(d1, d2)) ** (1. / float(order + 1))
+    h1 = h1.abs()
 
     return torch.min(100 * h0, h1).to(t_dtype)
 
 
 def _compute_error_ratio(error_estimate, rtol, atol, y0, y1, norm):
     error_tol = atol + rtol * torch.max(y0.abs(), y1.abs())
-    return norm(error_estimate / error_tol)
+    return norm(error_estimate / error_tol).abs()
 
 
 @torch.no_grad()
 def _optimal_step_size(last_step, error_ratio, safety, ifactor, dfactor, order):
     """Calculate the optimal size for the next step."""
     if error_ratio == 0:
         return last_step * ifactor
@@ -172,15 +178,17 @@
         self.base_func = base_func
 
     def forward(self, t, y, *, perturb=Perturb.NONE):
         assert isinstance(perturb, Perturb), "perturb argument must be of type Perturb enum"
         # This dtype change here might be buggy.
         # The exact time value should be determined inside the solver,
         # but this can slightly change it due to numerical differences during casting.
-        t = t.to(y.dtype)
+        if torch.is_complex(t):
+            t = t.real
+        t = t.to(y.abs().dtype)
         if perturb is Perturb.NEXT:
             # Replace with next smallest representable value.
             t = _nextafter(t, t + 1)
         elif perturb is Perturb.PREV:
             # Replace with prev largest representable value.
             t = _nextafter(t, t - 1)
         else:
@@ -194,27 +202,29 @@
     if event_fn is not None:
         if len(t) != 2:
             raise ValueError(f"We require len(t) == 2 when in event handling mode, but got len(t)={len(t)}.")
 
         # Combine event functions if the output is multivariate.
         event_fn = combine_event_functions(event_fn, t[0], y0)
 
+    # Keep reference to original func as passed in
+    original_func = func
+
     # Normalise to tensor (non-tupled) input
     shapes = None
     is_tuple = not isinstance(y0, torch.Tensor)
     if is_tuple:
         assert isinstance(y0, tuple), 'y0 must be either a torch.Tensor or a tuple'
         shapes = [y0_.shape for y0_ in y0]
         rtol = _tuple_tol('rtol', rtol, shapes)
         atol = _tuple_tol('atol', atol, shapes)
         y0 = torch.cat([y0_.reshape(-1) for y0_ in y0])
         func = _TupleFunc(func, shapes)
         if event_fn is not None:
             event_fn = _TupleInputOnlyFunc(event_fn, shapes)
-    _assert_floating('y0', y0)
 
     # Normalise method and options
     if options is None:
         options = {}
     else:
         options = options.copy()
     if method is None:
@@ -296,14 +306,46 @@
         warnings.warn("t is not on the same device as y0. Coercing to y0.device.")
         t = t.to(y0.device)
     # ~Backward compatibility
 
     # Add perturb argument to func.
     func = _PerturbFunc(func)
 
+    # Add callbacks to wrapped_func
+    callback_names = set()
+    for callback_name in _all_callback_names:
+        try:
+            callback = getattr(original_func, callback_name)
+        except AttributeError:
+            setattr(func, callback_name, _null_callback)
+        else:
+            if callback is not _null_callback:
+                callback_names.add(callback_name)
+                # At the moment all callbacks have the arguments (t0, y0, dt).
+                # These will need adjusting on a per-callback basis if that changes in the future.
+                if is_tuple:
+                    def callback(t0, y0, dt, _callback=callback):
+                        y0 = _flat_to_shape(y0, (), shapes)
+                        return _callback(t0, y0, dt)
+                if t_is_reversed:
+                    def callback(t0, y0, dt, _callback=callback):
+                        return _callback(-t0, y0, dt)
+            setattr(func, callback_name, callback)
+    for callback_name in _all_adjoint_callback_names:
+        try:
+            callback = getattr(original_func, callback_name)
+        except AttributeError:
+            pass
+        else:
+            setattr(func, callback_name, callback)
+
+    invalid_callbacks = callback_names - SOLVERS[method].valid_callbacks()
+    if len(invalid_callbacks) > 0:
+        warnings.warn("Solver '{}' does not support callbacks {}".format(method, invalid_callbacks))
+
     return shapes, func, y0, t, rtol, atol, method, options, event_fn, t_is_reversed
 
 
 class _StitchGradient(torch.autograd.Function):
     @staticmethod
     def forward(ctx, x1, out):
         return out
```

### Comparing `torchdiffeq-0.2.3/torchdiffeq/_impl/odeint.py` & `torchdiffeq-0.2.4/torchdiffeq/_impl/odeint.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import torch
 from torch.autograd.functional import vjp
 from .dopri5 import Dopri5Solver
 from .bosh3 import Bosh3Solver
 from .adaptive_heun import AdaptiveHeunSolver
 from .fehlberg2 import Fehlberg2
-from .fixed_grid import Euler, Midpoint, RK4
+from .fixed_grid import Euler, Midpoint, Heun3, RK4
 from .fixed_adams import AdamsBashforth, AdamsBashforthMoulton
 from .dopri8 import Dopri8Solver
 from .scipy_wrapper import ScipyWrapperODESolver
 from .misc import _check_inputs, _flat_to_shape
+from .interp import _interp_evaluate
 
 SOLVERS = {
     'dopri8': Dopri8Solver,
     'dopri5': Dopri5Solver,
     'bosh3': Bosh3Solver,
     'fehlberg2': Fehlberg2,
     'adaptive_heun': AdaptiveHeunSolver,
     'euler': Euler,
     'midpoint': Midpoint,
+    'heun3': Heun3,
     'rk4': RK4,
     'explicit_adams': AdamsBashforth,
     'implicit_adams': AdamsBashforthMoulton,
     # Backward compatibility: use the same name as before
     'fixed_adams': AdamsBashforthMoulton,
     # ~Backwards compatibility
     'scipy_solver': ScipyWrapperODESolver,
@@ -86,14 +88,63 @@
 
     if event_fn is None:
         return solution
     else:
         return event_t, solution
 
 
+def odeint_dense(func, y0, t0, t1, *, rtol=1e-7, atol=1e-9, method=None, options=None):
+
+    assert torch.is_tensor(y0)  # TODO: handle tuple of tensors
+
+    t = torch.tensor([t0, t1]).to(t0)
+
+    shapes, func, y0, t, rtol, atol, method, options, _, _ = _check_inputs(func, y0, t, rtol, atol, method, options, None, SOLVERS)
+
+    assert method == "dopri5"
+
+    solver = Dopri5Solver(func=func, y0=y0, rtol=rtol, atol=atol, **options)    
+    
+    # The integration loop
+    solution = torch.empty(len(t), *solver.y0.shape, dtype=solver.y0.dtype, device=solver.y0.device)
+    solution[0] = solver.y0
+    t = t.to(solver.dtype)
+    solver._before_integrate(t)
+    t0 = solver.rk_state.t0
+
+    times = [t0]
+    interp_coeffs = []
+
+    for i in range(1, len(t)):
+        next_t = t[i]
+        while next_t > solver.rk_state.t1:
+            solver.rk_state = solver._adaptive_step(solver.rk_state)
+            t1 = solver.rk_state.t1
+
+            if t1 != t0:
+                # Step accepted.
+                t0 = t1
+                times.append(t1)
+                interp_coeffs.append(torch.stack(solver.rk_state.interp_coeff))
+
+        solution[i] = _interp_evaluate(solver.rk_state.interp_coeff, solver.rk_state.t0, solver.rk_state.t1, next_t)
+
+    times = torch.stack(times).reshape(-1).cpu()
+    interp_coeffs = torch.stack(interp_coeffs)
+
+    def dense_output_fn(t_eval):
+        idx = torch.searchsorted(times, t_eval, side="right")
+        t0 = times[idx - 1]
+        t1 = times[idx]
+        coef = [interp_coeffs[idx - 1][i] for i in range(interp_coeffs.shape[1])]
+        return _interp_evaluate(coef, t0, t1, t_eval)
+
+    return dense_output_fn
+
+
 def odeint_event(func, y0, t0, *, event_fn, reverse_time=False, odeint_interface=odeint, **kwargs):
     """Automatically links up the gradient from the event time."""
 
     if reverse_time:
         t = torch.cat([t0.reshape(-1), t0.reshape(-1).detach() - 1.0])
     else:
         t = torch.cat([t0.reshape(-1), t0.reshape(-1).detach() + 1.0])
```

### Comparing `torchdiffeq-0.2.3/torchdiffeq/_impl/rk_common.py` & `torchdiffeq-0.2.4/torchdiffeq/_impl/rk_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,17 +52,19 @@
     Returns:
         Tuple `(y1, f1, y1_error, k)` giving the estimated function value after
         the Runge-Kutta step at `t1 = t0 + dt`, the derivative of the state at `t1`,
         estimated error at `t1`, and a list of Runge-Kutta coefficients `k` used for
         calculating these terms.
     """
 
-    t0 = t0.to(y0.dtype)
-    dt = dt.to(y0.dtype)
-    t1 = t1.to(y0.dtype)
+    t_dtype = y0.abs().dtype
+
+    t0 = t0.to(t_dtype)
+    dt = dt.to(t_dtype)
+    t1 = t1.to(t_dtype)
 
     # We use an unchecked assign to put data into k without incrementing its _version counter, so that the backward
     # doesn't throw an (overzealous) error about in-place correctness. We know that it's actually correct.
     k = torch.empty(*f0.shape, len(tableau.alpha) + 1, dtype=y0.dtype, device=y0.device)
     k = _UncheckedAssign.apply(k, f0, (..., 0))
     for i, (alpha_i, beta_i) in enumerate(zip(tableau.alpha, tableau.beta)):
         if alpha_i == 1.:
@@ -110,39 +112,64 @@
         k1 = func(t0, y0, perturb=Perturb.NEXT if perturb else Perturb.NONE)
     k2 = func(t0 + dt * _one_third, y0 + dt * k1 * _one_third)
     k3 = func(t0 + dt * _two_thirds, y0 + dt * (k2 - k1 * _one_third))
     k4 = func(t1, y0 + dt * (k1 - k2 + k3), perturb=Perturb.PREV if perturb else Perturb.NONE)
     return (k1 + 3 * (k2 + k3) + k4) * dt * 0.125
 
 
+def rk3_step_func(func, t0, dt, t1, y0, butcher_tableu=None, f0=None, perturb=False):
+    """butcher_tableu should be of the form
+    
+    [
+        [0  , 0     , 0     ,   0],
+        [c_2, a_{21}, 0     ,   0],
+        [c_3, a_{31}, a_{32},   0],
+        [0  , b_1   , b_2   , b_3],
+    ]
+
+    https://en.wikipedia.org/wiki/List_of_Runge-Kutta_methods
+    """
+    k1 = f0
+    if k1 is None:
+        k1 = func(t0, y0, perturb=Perturb.NEXT if perturb else Perturb.NONE)
+
+    k2 = func(t0 + dt * butcher_tableu[1][0], y0 + dt * k1 * butcher_tableu[1][1])
+    k3 = func(t0 + dt * butcher_tableu[2][0], y0 + dt * (k1 * butcher_tableu[2][1] + k2 * butcher_tableu[2][2]))
+    return dt * (k1 * butcher_tableu[3][1] + k2 * butcher_tableu[3][2] + k3 * butcher_tableu[3][3])
+
+
 class RKAdaptiveStepsizeODESolver(AdaptiveStepsizeEventODESolver):
     order: int
     tableau: _ButcherTableau
     mid: torch.Tensor
 
     def __init__(self, func, y0, rtol, atol,
+                 min_step=0,
+                 max_step=float('inf'),
                  first_step=None,
                  step_t=None,
                  jump_t=None,
                  safety=0.9,
                  ifactor=10.0,
                  dfactor=0.2,
                  max_num_steps=2 ** 31 - 1,
                  dtype=torch.float64,
                  **kwargs):
         super(RKAdaptiveStepsizeODESolver, self).__init__(dtype=dtype, y0=y0, **kwargs)
 
         # We use mixed precision. y has its original dtype (probably float32), whilst all 'time'-like objects use
         # `dtype` (defaulting to float64).
-        dtype = torch.promote_types(dtype, y0.dtype)
+        dtype = torch.promote_types(dtype, y0.abs().dtype)
         device = y0.device
 
         self.func = func
         self.rtol = torch.as_tensor(rtol, dtype=dtype, device=device)
         self.atol = torch.as_tensor(atol, dtype=dtype, device=device)
+        self.min_step = torch.as_tensor(min_step, dtype=dtype, device=device)
+        self.max_step = torch.as_tensor(max_step, dtype=dtype, device=device)
         self.first_step = None if first_step is None else torch.as_tensor(first_step, dtype=dtype, device=device)
         self.safety = torch.as_tensor(safety, dtype=dtype, device=device)
         self.ifactor = torch.as_tensor(ifactor, dtype=dtype, device=device)
         self.dfactor = torch.as_tensor(dfactor, dtype=dtype, device=device)
         self.max_num_steps = torch.as_tensor(max_num_steps, dtype=torch.int32, device=device)
         self.dtype = dtype
 
@@ -152,14 +179,20 @@
         # Copy from class to instance to set device
         self.tableau = _ButcherTableau(alpha=self.tableau.alpha.to(device=device, dtype=y0.dtype),
                                        beta=[b.to(device=device, dtype=y0.dtype) for b in self.tableau.beta],
                                        c_sol=self.tableau.c_sol.to(device=device, dtype=y0.dtype),
                                        c_error=self.tableau.c_error.to(device=device, dtype=y0.dtype))
         self.mid = self.mid.to(device=device, dtype=y0.dtype)
 
+    @classmethod
+    def valid_callbacks(cls):
+        return super(RKAdaptiveStepsizeODESolver, cls).valid_callbacks() | {'callback_step',
+                                                                            'callback_accept_step',
+                                                                            'callback_reject_step'}
+
     def _before_integrate(self, t):
         t0 = t[0]
         f0 = self.func(t[0], self.y0)
         if self.first_step is None:
             first_step = _select_initial_step(self.func, t[0], self.y0, self.order - 1, self.rtol, self.atol,
                                               self.norm, f0=f0)
         else:
@@ -208,14 +241,18 @@
             n_steps += 1
         interp_fn = lambda t: _interp_evaluate(self.rk_state.interp_coeff, self.rk_state.t0, self.rk_state.t1, t)
         return find_event(interp_fn, sign0, self.rk_state.t0, self.rk_state.t1, event_fn, self.atol)
 
     def _adaptive_step(self, rk_state):
         """Take an adaptive Runge-Kutta step to integrate the ODE."""
         y0, f0, _, t0, dt, interp_coeff = rk_state
+        if not torch.isfinite(dt):
+            dt = self.min_step
+        dt = dt.clamp(self.min_step, self.max_step)
+        self.func.callback_step(t0, y0, dt)
         t1 = t0 + dt
         # dtypes: self.y0.dtype (probably float32); self.dtype (probably float64)
         # used for state and timelike objects respectively.
         # Then:
         # y0.dtype == self.y0.dtype
         # f0.dtype == self.y0.dtype
         # t0.dtype == self.dtype
@@ -260,39 +297,49 @@
         # k.dtype == self.y0.dtype
 
         ########################################################
         #                     Error Ratio                      #
         ########################################################
         error_ratio = _compute_error_ratio(y1_error, self.rtol, self.atol, y0, y1, self.norm)
         accept_step = error_ratio <= 1
+
+        # Handle min max stepping
+        if dt > self.max_step:
+            accept_step = False
+        if dt <= self.min_step:
+            accept_step = True
+
         # dtypes:
         # error_ratio.dtype == self.dtype
 
         ########################################################
         #                   Update RK State                    #
         ########################################################
         if accept_step:
+            self.func.callback_accept_step(t0, y0, dt)
             t_next = t1
             y_next = y1
             interp_coeff = self._interp_fit(y0, y_next, k, dt)
             if on_step_t:
                 if self.next_step_index != len(self.step_t) - 1:
                     self.next_step_index += 1
             if on_jump_t:
                 if self.next_jump_index != len(self.jump_t) - 1:
                     self.next_jump_index += 1
                 # We've just passed a discontinuity in f; we should update f to match the side of the discontinuity
                 # we're now on.
                 f1 = self.func(t_next, y_next, perturb=Perturb.NEXT)
             f_next = f1
         else:
+            self.func.callback_reject_step(t0, y0, dt)
             t_next = t0
             y_next = y0
             f_next = f0
         dt_next = _optimal_step_size(dt, error_ratio, self.safety, self.ifactor, self.dfactor, self.order)
+        dt_next = dt_next.clamp(self.min_step, self.max_step)
         rk_state = _RungeKuttaState(y_next, f_next, t0, t_next, dt_next, interp_coeff)
         return rk_state
 
     def _interp_fit(self, y0, y1, k, dt):
         """Fit an interpolating polynomial to the results of a Runge-Kutta step."""
         dt = dt.type_as(y0)
         y_mid = y0 + torch.sum(k * (dt * self.mid), dim=-1).view_as(y0)
```

### Comparing `torchdiffeq-0.2.3/torchdiffeq/_impl/scipy_wrapper.py` & `torchdiffeq-0.2.4/torchdiffeq/_impl/scipy_wrapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 import torch
 from scipy.integrate import solve_ivp
 from .misc import _handle_unused_kwargs
 
 
 class ScipyWrapperODESolver(metaclass=abc.ABCMeta):
 
-    def __init__(self, func, y0, rtol, atol, solver="LSODA", **unused_kwargs):
+    def __init__(self, func, y0, rtol, atol, min_step=0, max_step=float('inf'), solver="LSODA", **unused_kwargs):
         unused_kwargs.pop('norm', None)
         unused_kwargs.pop('grid_points', None)
         unused_kwargs.pop('eps', None)
         _handle_unused_kwargs(self, unused_kwargs)
         del unused_kwargs
 
         self.dtype = y0.dtype
         self.device = y0.device
         self.shape = y0.shape
         self.y0 = y0.detach().cpu().numpy().reshape(-1)
         self.rtol = rtol
         self.atol = atol
+        self.min_step = min_step
+        self.max_step = max_step
         self.solver = solver
         self.func = convert_func_to_numpy(func, self.shape, self.device, self.dtype)
 
     def integrate(self, t):
         if t.numel() == 1:
             return torch.tensor(self.y0)[None].to(self.device, self.dtype)
         t = t.detach().cpu().numpy()
@@ -30,18 +32,24 @@
             self.func,
             t_span=[t.min(), t.max()],
             y0=self.y0,
             t_eval=t,
             method=self.solver,
             rtol=self.rtol,
             atol=self.atol,
+            min_step=self.min_step,
+            max_step=self.max_step
         )
         sol = torch.tensor(sol.y).T.to(self.device, self.dtype)
         sol = sol.reshape(-1, *self.shape)
         return sol
+        
+    @classmethod
+    def valid_callbacks(cls):
+        return set()
 
 
 def convert_func_to_numpy(func, shape, device, dtype):
 
     def np_func(t, y):
         t = torch.tensor(t).to(device, dtype)
         y = torch.reshape(torch.tensor(y).to(device, dtype), shape)
```

### Comparing `torchdiffeq-0.2.3/torchdiffeq/_impl/solvers.py` & `torchdiffeq-0.2.4/torchdiffeq/_impl/solvers.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,18 @@
     def _before_integrate(self, t):
         pass
 
     @abc.abstractmethod
     def _advance(self, next_t):
         raise NotImplementedError
 
+    @classmethod
+    def valid_callbacks(cls):
+        return set()
+
     def integrate(self, t):
         solution = torch.empty(len(t), *self.y0.shape, dtype=self.y0.dtype, device=self.y0.device)
         solution[0] = self.y0
         t = t.to(self.dtype)
         self._before_integrate(t)
         for i in range(1, len(t)):
             solution[i] = self._advance(t[i])
@@ -70,14 +74,18 @@
                 self.grid_constructor = grid_constructor
         else:
             if grid_constructor is None:
                 self.grid_constructor = self._grid_constructor_from_step_size(step_size)
             else:
                 raise ValueError("step_size and grid_constructor are mutually exclusive arguments.")
 
+    @classmethod
+    def valid_callbacks(cls):
+        return {'callback_step'}
+
     @staticmethod
     def _grid_constructor_from_step_size(step_size):
         def _grid_constructor(func, y0, t):
             start_time = t[0]
             end_time = t[-1]
 
             niters = torch.ceil((end_time - start_time) / step_size + 1).item()
@@ -98,14 +106,15 @@
         solution = torch.empty(len(t), *self.y0.shape, dtype=self.y0.dtype, device=self.y0.device)
         solution[0] = self.y0
 
         j = 1
         y0 = self.y0
         for t0, t1 in zip(time_grid[:-1], time_grid[1:]):
             dt = t1 - t0
+            self.func.callback_step(t0, y0, dt)
             dy, f0 = self._step_func(self.func, t0, dt, t1, y0)
             y1 = y0 + dy
 
             while j < len(t) and t1 >= t[j]:
                 if self.interp == "linear":
                     solution[j] = self._linear_interp(t0, t1, y0, y1, t[j])
                 elif self.interp == "cubic":
@@ -117,15 +126,15 @@
             y0 = y1
 
         return solution
 
     def integrate_until_event(self, t0, event_fn):
         assert self.step_size is not None, "Event handling for fixed step solvers currently requires `step_size` to be provided in options."
 
-        t0 = t0.type_as(self.y0)
+        t0 = t0.type_as(self.y0.abs())
         y0 = self.y0
         dt = self.step_size
 
         sign0 = torch.sign(event_fn(t0, y0))
         max_itrs = 20000
         itr = 0
         while True:
```

### Comparing `torchdiffeq-0.2.3/torchdiffeq.egg-info/SOURCES.txt` & `torchdiffeq-0.2.4/torchdiffeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

