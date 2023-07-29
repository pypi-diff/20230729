# Comparing `tmp/azure-quantum-0.28.277227.tar.gz` & `tmp/azure-quantum-0.28.291393b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-quantum-0.28.277227.tar", last modified: Mon Jun  5 22:16:43 2023, max compression
+gzip compressed data, was "azure-quantum-0.28.291393b1.tar", last modified: Fri Jul 28 04:52:22 2023, max compression
```

## Comparing `azure-quantum-0.28.277227.tar` & `azure-quantum-0.28.291393b1.tar`

### file list

```diff
@@ -1,168 +1,147 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.284259 azure-quantum-0.28.277227/
--rw-rw-rw-   0        0        0     5568 2023-06-05 22:16:43.284259 azure-quantum-0.28.277227/PKG-INFO
--rw-rw-rw-   0        0        0     5063 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.190509 azure-quantum-0.28.277227/azure/
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.206131 azure-quantum-0.28.277227/azure/quantum/
--rw-rw-rw-   0        0        0      414 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.206131 azure-quantum-0.28.277227/azure/quantum/_authentication/
--rw-rw-rw-   0        0        0      236 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_authentication/__init__.py
--rw-rw-rw-   0        0        0     5047 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_authentication/_chained.py
--rw-rw-rw-   0        0        0    10502 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_authentication/_default.py
--rw-rw-rw-   0        0        0     3570 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_authentication/_token.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.206131 azure-quantum-0.28.277227/azure/quantum/_client/
--rw-rw-rw-   0        0        0      896 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_client/__init__.py
--rw-rw-rw-   0        0        0     5854 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_client/_client.py
--rw-rw-rw-   0        0        0     4444 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_client/_configuration.py
--rw-rw-rw-   0        0        0      694 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_client/_patch.py
--rw-rw-rw-   0        0        0    80832 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_client/_serialization.py
--rw-rw-rw-   0        0        0      996 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_client/_vendor.py
--rw-rw-rw-   0        0        0      501 2023-06-05 22:16:42.000000 azure-quantum-0.28.277227/azure/quantum/_client/_version.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.206131 azure-quantum-0.28.277227/azure/quantum/_client/aio/
--rw-rw-rw-   0        0        0      840 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_client/aio/__init__.py
--rw-rw-rw-   0        0        0     6010 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_client/aio/_client.py
--rw-rw-rw-   0        0        0     4487 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_client/aio/_configuration.py
--rw-rw-rw-   0        0        0      694 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_client/aio/_patch.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.221759 azure-quantum-0.28.277227/azure/quantum/_client/aio/operations/
--rw-rw-rw-   0        0        0     1154 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_client/aio/operations/__init__.py
--rw-rw-rw-   0        0        0    54215 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_client/aio/operations/_operations.py
--rw-rw-rw-   0        0        0      694 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_client/aio/operations/_patch.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.221759 azure-quantum-0.28.277227/azure/quantum/_client/models/
--rw-rw-rw-   0        0        0     2100 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_client/models/__init__.py
--rw-rw-rw-   0        0        0     2977 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_client/models/_enums.py
--rw-rw-rw-   0        0        0    41802 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_client/models/_models.py
--rw-rw-rw-   0        0        0      694 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_client/models/_patch.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.221759 azure-quantum-0.28.277227/azure/quantum/_client/operations/
--rw-rw-rw-   0        0        0     1154 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_client/operations/__init__.py
--rw-rw-rw-   0        0        0    75919 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_client/operations/_operations.py
--rw-rw-rw-   0        0        0      694 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/_client/operations/_patch.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.221759 azure-quantum-0.28.277227/azure/quantum/aio/
--rw-rw-rw-   0        0        0      360 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.221759 azure-quantum-0.28.277227/azure/quantum/aio/_authentication/
--rw-rw-rw-   0        0        0      236 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/_authentication/__init__.py
--rw-rw-rw-   0        0        0     4647 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/_authentication/_chained.py
--rw-rw-rw-   0        0        0    10430 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/_authentication/_default.py
--rw-rw-rw-   0        0        0     3632 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/_authentication/_token.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.221759 azure-quantum-0.28.277227/azure/quantum/aio/job/
--rw-rw-rw-   0        0        0       43 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/job/__init__.py
--rw-rw-rw-   0        0        0    11565 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/job/base_job.py
--rw-rw-rw-   0        0        0     3728 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/job/job.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.221759 azure-quantum-0.28.277227/azure/quantum/aio/optimization/
--rw-rw-rw-   0        0        0      484 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/optimization/__init__.py
--rw-rw-rw-   0        0        0      560 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/optimization/online_problem.py
--rw-rw-rw-   0        0        0     3620 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/optimization/problem.py
--rw-rw-rw-   0        0        0    10536 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/optimization/streaming_problem.py
--rw-rw-rw-   0        0        0    12953 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/storage.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.237384 azure-quantum-0.28.277227/azure/quantum/aio/target/
--rw-rw-rw-   0        0        0      831 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/target/__init__.py
--rw-rw-rw-   0        0        0     1393 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/target/ionq.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.237384 azure-quantum-0.28.277227/azure/quantum/aio/target/microsoft/
--rw-rw-rw-   0        0        0      267 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/target/microsoft/__init__.py
--rw-rw-rw-   0        0        0     1113 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/target/microsoft/qio.py
--rw-rw-rw-   0        0        0      416 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/target/oneqbit.py
--rw-rw-rw-   0        0        0     1413 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/target/quantinuum.py
--rw-rw-rw-   0        0        0     3336 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/target/solvers.py
--rw-rw-rw-   0        0        0     2366 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/target/target.py
--rw-rw-rw-   0        0        0     2449 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/target/target_factory.py
--rw-rw-rw-   0        0        0      249 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/target/toshiba.py
--rw-rw-rw-   0        0        0    13507 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/aio/workspace.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.237384 azure-quantum-0.28.277227/azure/quantum/argument_types/
--rw-rw-rw-   0        0        0      213 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/argument_types/__init__.py
--rw-rw-rw-   0        0        0      721 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/argument_types/types.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.237384 azure-quantum-0.28.277227/azure/quantum/chemistry/
--rw-rw-rw-   0        0        0      351 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/chemistry/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.237384 azure-quantum-0.28.277227/azure/quantum/cirq/
--rw-rw-rw-   0        0        0      125 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/cirq/__init__.py
--rw-rw-rw-   0        0        0     2773 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/cirq/job.py
--rw-rw-rw-   0        0        0     8039 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/cirq/service.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.237384 azure-quantum-0.28.277227/azure/quantum/cirq/targets/
--rw-rw-rw-   0        0        0      502 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/cirq/targets/__init__.py
--rw-rw-rw-   0        0        0     6804 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/cirq/targets/ionq.py
--rw-rw-rw-   0        0        0     4541 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/cirq/targets/quantinuum.py
--rw-rw-rw-   0        0        0     2184 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/cirq/targets/target.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.237384 azure-quantum-0.28.277227/azure/quantum/job/
--rw-rw-rw-   0        0        0      372 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/job/__init__.py
--rw-rw-rw-   0        0        0    12056 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/job/base_job.py
--rw-rw-rw-   0        0        0     1683 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/job/filtered_job.py
--rw-rw-rw-   0        0        0     4505 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/job/job.py
--rw-rw-rw-   0        0        0    11936 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/job/session.py
--rw-rw-rw-   0        0        0     1198 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/job/workspace_item.py
--rw-rw-rw-   0        0        0     1200 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/job/workspace_item_factory.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.253009 azure-quantum-0.28.277227/azure/quantum/optimization/
--rw-rw-rw-   0        0        0      469 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/optimization/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.253009 azure-quantum-0.28.277227/azure/quantum/optimization/oneqbit/
--rw-rw-rw-   0        0        0      366 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/optimization/oneqbit/__init__.py
--rw-rw-rw-   0        0        0      402 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/optimization/oneqbit/solvers.py
--rw-rw-rw-   0        0        0      636 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/optimization/online_problem.py
--rw-rw-rw-   0        0        0    25096 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/optimization/problem.py
--rw-rw-rw-   0        0        0      512 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/optimization/solvers.py
--rw-rw-rw-   0        0        0    13733 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/optimization/streaming_problem.py
--rw-rw-rw-   0        0        0     9858 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/optimization/term.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.253009 azure-quantum-0.28.277227/azure/quantum/optimization/toshiba/
--rw-rw-rw-   0        0        0      302 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/optimization/toshiba/__init__.py
--rw-rw-rw-   0        0        0      374 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/optimization/toshiba/solvers.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.253009 azure-quantum-0.28.277227/azure/quantum/qiskit/
--rw-rw-rw-   0        0        0      273 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/qiskit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.253009 azure-quantum-0.28.277227/azure/quantum/qiskit/backends/
--rw-rw-rw-   0        0        0      965 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/qiskit/backends/__init__.py
--rw-rw-rw-   0        0        0    16467 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/qiskit/backends/backend.py
--rw-rw-rw-   0        0        0    12920 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/qiskit/backends/ionq.py
--rw-rw-rw-   0        0        0     3441 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/qiskit/backends/microsoft.py
--rw-rw-rw-   0        0        0     3884 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/qiskit/backends/qci.py
--rw-rw-rw-   0        0        0    13278 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/qiskit/backends/quantinuum.py
--rw-rw-rw-   0        0        0     4081 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/qiskit/backends/rigetti.py
--rw-rw-rw-   0        0        0    14829 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/qiskit/job.py
--rw-rw-rw-   0        0        0     9974 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/qiskit/provider.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.253009 azure-quantum-0.28.277227/azure/quantum/qiskit/results/
--rw-rw-rw-   0        0        0        0 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/qiskit/results/__init__.py
--rw-rw-rw-   0        0        0      814 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/qiskit/results/resource_estimator.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.268634 azure-quantum-0.28.277227/azure/quantum/serialization/
--rw-rw-rw-   0        0        0       58 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/serialization/__init__.py
--rw-rw-rw-   0        0        0    11227 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/serialization/problem_pb2.py
--rw-rw-rw-   0        0        0    12536 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/storage.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.268634 azure-quantum-0.28.277227/azure/quantum/target/
--rw-rw-rw-   0        0        0      817 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/__init__.py
--rw-rw-rw-   0        0        0     7212 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/ionq.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.268634 azure-quantum-0.28.277227/azure/quantum/target/microsoft/
--rw-rw-rw-   0        0        0      667 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/microsoft/__init__.py
--rw-rw-rw-   0        0        0     1005 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/microsoft/job.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.268634 azure-quantum-0.28.277227/azure/quantum/target/microsoft/qio/
--rw-rw-rw-   0        0        0      402 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/microsoft/qio/__init__.py
--rw-rw-rw-   0        0        0     3053 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/microsoft/qio/parallel_tempering.py
--rw-rw-rw-   0        0        0     3145 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/microsoft/qio/population_annealing.py
--rw-rw-rw-   0        0        0     2564 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/microsoft/qio/quantum_monte_carlo.py
--rw-rw-rw-   0        0        0     3971 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/microsoft/qio/simulated_annealing.py
--rw-rw-rw-   0        0        0     3712 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/microsoft/qio/substochastic_montecarlo.py
--rw-rw-rw-   0        0        0     2395 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/microsoft/qio/tabu.py
--rw-rw-rw-   0        0        0    14916 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/microsoft/result.py
--rw-rw-rw-   0        0        0     9169 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/microsoft/target.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.268634 azure-quantum-0.28.277227/azure/quantum/target/oneqbit/
--rw-rw-rw-   0        0        0      210 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/oneqbit/__init__.py
--rw-rw-rw-   0        0        0    13648 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/oneqbit/solvers.py
--rw-rw-rw-   0        0        0     8976 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/params.py
--rw-rw-rw-   0        0        0     7250 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/quantinuum.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.268634 azure-quantum-0.28.277227/azure/quantum/target/rigetti/
--rw-rw-rw-   0        0        0      378 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/rigetti/__init__.py
--rw-rw-rw-   0        0        0     2215 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/rigetti/result.py
--rw-rw-rw-   0        0        0     5916 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/rigetti/target.py
--rw-rw-rw-   0        0        0    17063 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/solvers.py
--rw-rw-rw-   0        0        0     9181 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/target.py
--rw-rw-rw-   0        0        0     5322 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/target_factory.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.268634 azure-quantum-0.28.277227/azure/quantum/target/toshiba/
--rw-rw-rw-   0        0        0      146 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/toshiba/__init__.py
--rw-rw-rw-   0        0        0     5722 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/target/toshiba/solvers.py
--rw-rw-rw-   0        0        0      241 2023-06-05 22:16:42.000000 azure-quantum-0.28.277227/azure/quantum/version.py
--rw-rw-rw-   0        0        0    19134 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/azure/quantum/workspace.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:16:43.284259 azure-quantum-0.28.277227/azure_quantum.egg-info/
--rw-rw-rw-   0        0        0     5568 2023-06-05 22:16:43.000000 azure-quantum-0.28.277227/azure_quantum.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5009 2023-06-05 22:16:43.000000 azure-quantum-0.28.277227/azure_quantum.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 22:16:43.000000 azure-quantum-0.28.277227/azure_quantum.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      866 2023-06-05 22:16:43.000000 azure-quantum-0.28.277227/azure_quantum.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-05 22:16:43.000000 azure-quantum-0.28.277227/azure_quantum.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       46 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/requirements-cirq.txt
--rw-rw-rw-   0        0        0      296 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/requirements-dev.txt
--rw-rw-rw-   0        0        0      130 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/requirements-qiskit.txt
--rw-rw-rw-   0        0        0       19 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/requirements-qsharp.txt
--rw-rw-rw-   0        0        0      275 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/requirements-quil.txt
--rw-rw-rw-   0        0        0      269 2023-06-05 22:16:37.000000 azure-quantum-0.28.277227/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 22:16:43.284259 azure-quantum-0.28.277227/setup.cfg
--rw-rw-rw-   0        0        0     3770 2023-06-05 21:54:39.000000 azure-quantum-0.28.277227/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.517689 azure-quantum-0.28.291393b1/
+-rw-rw-rw-   0        0        0     5398 2023-07-28 04:52:22.517689 azure-quantum-0.28.291393b1/PKG-INFO
+-rw-rw-rw-   0        0        0     4891 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.393275 azure-quantum-0.28.291393b1/azure/
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.423967 azure-quantum-0.28.291393b1/azure/quantum/
+-rw-rw-rw-   0        0        0      414 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.423967 azure-quantum-0.28.291393b1/azure/quantum/_authentication/
+-rw-rw-rw-   0        0        0      236 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_authentication/__init__.py
+-rw-rw-rw-   0        0        0     5047 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_authentication/_chained.py
+-rw-rw-rw-   0        0        0    10502 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_authentication/_default.py
+-rw-rw-rw-   0        0        0     3570 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_authentication/_token.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.439563 azure-quantum-0.28.291393b1/azure/quantum/_client/
+-rw-rw-rw-   0        0        0      896 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/__init__.py
+-rw-rw-rw-   0        0        0     5854 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/_client.py
+-rw-rw-rw-   0        0        0     4444 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/_configuration.py
+-rw-rw-rw-   0        0        0      694 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/_patch.py
+-rw-rw-rw-   0        0        0    80832 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/_serialization.py
+-rw-rw-rw-   0        0        0      996 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/_vendor.py
+-rw-rw-rw-   0        0        0      503 2023-07-28 04:52:21.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/_version.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.439563 azure-quantum-0.28.291393b1/azure/quantum/_client/aio/
+-rw-rw-rw-   0        0        0      840 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/aio/__init__.py
+-rw-rw-rw-   0        0        0     6010 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/aio/_client.py
+-rw-rw-rw-   0        0        0     4487 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/aio/_configuration.py
+-rw-rw-rw-   0        0        0      694 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/aio/_patch.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.439563 azure-quantum-0.28.291393b1/azure/quantum/_client/aio/operations/
+-rw-rw-rw-   0        0        0     1154 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/aio/operations/__init__.py
+-rw-rw-rw-   0        0        0    54215 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/aio/operations/_operations.py
+-rw-rw-rw-   0        0        0      694 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/aio/operations/_patch.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.439563 azure-quantum-0.28.291393b1/azure/quantum/_client/models/
+-rw-rw-rw-   0        0        0     2100 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/models/__init__.py
+-rw-rw-rw-   0        0        0     2977 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/models/_enums.py
+-rw-rw-rw-   0        0        0    41802 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/models/_models.py
+-rw-rw-rw-   0        0        0      694 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/models/_patch.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.455228 azure-quantum-0.28.291393b1/azure/quantum/_client/operations/
+-rw-rw-rw-   0        0        0     1154 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/operations/__init__.py
+-rw-rw-rw-   0        0        0    75919 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/operations/_operations.py
+-rw-rw-rw-   0        0        0      694 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/_client/operations/_patch.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.455228 azure-quantum-0.28.291393b1/azure/quantum/aio/
+-rw-rw-rw-   0        0        0      360 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.455228 azure-quantum-0.28.291393b1/azure/quantum/aio/_authentication/
+-rw-rw-rw-   0        0        0      236 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/_authentication/__init__.py
+-rw-rw-rw-   0        0        0     4647 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/_authentication/_chained.py
+-rw-rw-rw-   0        0        0    10430 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/_authentication/_default.py
+-rw-rw-rw-   0        0        0     3632 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/_authentication/_token.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.455228 azure-quantum-0.28.291393b1/azure/quantum/aio/job/
+-rw-rw-rw-   0        0        0       43 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/job/__init__.py
+-rw-rw-rw-   0        0        0    11565 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/job/base_job.py
+-rw-rw-rw-   0        0        0     3728 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/job/job.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.455228 azure-quantum-0.28.291393b1/azure/quantum/aio/optimization/
+-rw-rw-rw-   0        0        0      287 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/optimization/__init__.py
+-rw-rw-rw-   0        0        0      560 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/optimization/online_problem.py
+-rw-rw-rw-   0        0        0     3638 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/optimization/problem.py
+-rw-rw-rw-   0        0        0    10536 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/optimization/streaming_problem.py
+-rw-rw-rw-   0        0        0    12953 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/storage.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.470852 azure-quantum-0.28.291393b1/azure/quantum/aio/target/
+-rw-rw-rw-   0        0        0      521 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/target/__init__.py
+-rw-rw-rw-   0        0        0     1393 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/target/ionq.py
+-rw-rw-rw-   0        0        0     1413 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/target/quantinuum.py
+-rw-rw-rw-   0        0        0     3311 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/target/solvers.py
+-rw-rw-rw-   0        0        0     2366 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/target/target.py
+-rw-rw-rw-   0        0        0     2449 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/target/target_factory.py
+-rw-rw-rw-   0        0        0      249 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/target/toshiba.py
+-rw-rw-rw-   0        0        0    13507 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/aio/workspace.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.470852 azure-quantum-0.28.291393b1/azure/quantum/argument_types/
+-rw-rw-rw-   0        0        0      213 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/argument_types/__init__.py
+-rw-rw-rw-   0        0        0      721 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/argument_types/types.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.470852 azure-quantum-0.28.291393b1/azure/quantum/chemistry/
+-rw-rw-rw-   0        0        0      351 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/chemistry/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.470852 azure-quantum-0.28.291393b1/azure/quantum/cirq/
+-rw-rw-rw-   0        0        0      125 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/cirq/__init__.py
+-rw-rw-rw-   0        0        0     2773 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/cirq/job.py
+-rw-rw-rw-   0        0        0     8039 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/cirq/service.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.470852 azure-quantum-0.28.291393b1/azure/quantum/cirq/targets/
+-rw-rw-rw-   0        0        0      502 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/cirq/targets/__init__.py
+-rw-rw-rw-   0        0        0     6804 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/cirq/targets/ionq.py
+-rw-rw-rw-   0        0        0     4541 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/cirq/targets/quantinuum.py
+-rw-rw-rw-   0        0        0     2184 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/cirq/targets/target.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.486438 azure-quantum-0.28.291393b1/azure/quantum/job/
+-rw-rw-rw-   0        0        0      372 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/job/__init__.py
+-rw-rw-rw-   0        0        0    11987 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/job/base_job.py
+-rw-rw-rw-   0        0        0     1683 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/job/filtered_job.py
+-rw-rw-rw-   0        0        0     4505 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/job/job.py
+-rw-rw-rw-   0        0        0    11936 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/job/session.py
+-rw-rw-rw-   0        0        0     1198 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/job/workspace_item.py
+-rw-rw-rw-   0        0        0     1200 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/job/workspace_item_factory.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.486438 azure-quantum-0.28.291393b1/azure/quantum/optimization/
+-rw-rw-rw-   0        0        0      276 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/optimization/__init__.py
+-rw-rw-rw-   0        0        0      636 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/optimization/online_problem.py
+-rw-rw-rw-   0        0        0    13570 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/optimization/problem.py
+-rw-rw-rw-   0        0        0      319 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/optimization/solvers.py
+-rw-rw-rw-   0        0        0    13650 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/optimization/streaming_problem.py
+-rw-rw-rw-   0        0        0     5983 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/optimization/term.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.486438 azure-quantum-0.28.291393b1/azure/quantum/optimization/toshiba/
+-rw-rw-rw-   0        0        0      302 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/optimization/toshiba/__init__.py
+-rw-rw-rw-   0        0        0      374 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/optimization/toshiba/solvers.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.486438 azure-quantum-0.28.291393b1/azure/quantum/qiskit/
+-rw-rw-rw-   0        0        0      273 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.502097 azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/
+-rw-rw-rw-   0        0        0      965 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/__init__.py
+-rw-rw-rw-   0        0        0    16467 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/backend.py
+-rw-rw-rw-   0        0        0    12920 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/ionq.py
+-rw-rw-rw-   0        0        0     3441 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/microsoft.py
+-rw-rw-rw-   0        0        0     3884 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/qci.py
+-rw-rw-rw-   0        0        0    13278 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/quantinuum.py
+-rw-rw-rw-   0        0        0     4081 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/rigetti.py
+-rw-rw-rw-   0        0        0    14829 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/job.py
+-rw-rw-rw-   0        0        0     9974 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/provider.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.502097 azure-quantum-0.28.291393b1/azure/quantum/qiskit/results/
+-rw-rw-rw-   0        0        0        0 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/results/__init__.py
+-rw-rw-rw-   0        0        0      814 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/qiskit/results/resource_estimator.py
+-rw-rw-rw-   0        0        0    12536 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/storage.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.517689 azure-quantum-0.28.291393b1/azure/quantum/target/
+-rw-rw-rw-   0        0        0      507 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/__init__.py
+-rw-rw-rw-   0        0        0     7212 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/ionq.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.517689 azure-quantum-0.28.291393b1/azure/quantum/target/microsoft/
+-rw-rw-rw-   0        0        0      502 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/microsoft/__init__.py
+-rw-rw-rw-   0        0        0     1005 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/microsoft/job.py
+-rw-rw-rw-   0        0        0    13896 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/microsoft/result.py
+-rw-rw-rw-   0        0        0    15889 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/microsoft/target.py
+-rw-rw-rw-   0        0        0     8976 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/params.py
+-rw-rw-rw-   0        0        0     7250 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/quantinuum.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.517689 azure-quantum-0.28.291393b1/azure/quantum/target/rigetti/
+-rw-rw-rw-   0        0        0      378 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/rigetti/__init__.py
+-rw-rw-rw-   0        0        0     2215 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/rigetti/result.py
+-rw-rw-rw-   0        0        0     5916 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/rigetti/target.py
+-rw-rw-rw-   0        0        0    14807 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/solvers.py
+-rw-rw-rw-   0        0        0     8933 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/target.py
+-rw-rw-rw-   0        0        0     5322 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/target_factory.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.517689 azure-quantum-0.28.291393b1/azure/quantum/target/toshiba/
+-rw-rw-rw-   0        0        0      146 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/toshiba/__init__.py
+-rw-rw-rw-   0        0        0     5722 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/target/toshiba/solvers.py
+-rw-rw-rw-   0        0        0      243 2023-07-28 04:52:21.000000 azure-quantum-0.28.291393b1/azure/quantum/version.py
+-rw-rw-rw-   0        0        0    19134 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/azure/quantum/workspace.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:52:22.517689 azure-quantum-0.28.291393b1/azure_quantum.egg-info/
+-rw-rw-rw-   0        0        0     5398 2023-07-28 04:52:22.000000 azure-quantum-0.28.291393b1/azure_quantum.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4242 2023-07-28 04:52:22.000000 azure-quantum-0.28.291393b1/azure_quantum.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 04:52:22.000000 azure-quantum-0.28.291393b1/azure_quantum.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      782 2023-07-28 04:52:22.000000 azure-quantum-0.28.291393b1/azure_quantum.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-28 04:52:22.000000 azure-quantum-0.28.291393b1/azure_quantum.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       46 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/requirements-cirq.txt
+-rw-rw-rw-   0        0        0       94 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/requirements-dev.txt
+-rw-rw-rw-   0        0        0      248 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/requirements-qiskit.txt
+-rw-rw-rw-   0        0        0       19 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/requirements-qsharp.txt
+-rw-rw-rw-   0        0        0      275 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/requirements-quil.txt
+-rw-rw-rw-   0        0        0      246 2023-07-28 04:52:17.000000 azure-quantum-0.28.291393b1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 04:52:22.517689 azure-quantum-0.28.291393b1/setup.cfg
+-rw-rw-rw-   0        0        0     3770 2023-07-28 04:30:05.000000 azure-quantum-0.28.291393b1/setup.py
```

### Comparing `azure-quantum-0.28.277227/PKG-INFO` & `azure-quantum-0.28.291393b1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-quantum
-Version: 0.28.277227
+Version: 0.28.291393b1
 Summary: Python client for Azure Quantum
 Home-page: https://github.com/microsoft/qdk-python
 Author: Microsoft
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -51,15 +51,14 @@
 To work in Azure Quantum, you need an Azure subscription. If you don't have an Azure subscription, create a [free account](https://azure.microsoft.com/free/). Follow the [Create an Azure Quantum workspace](https://docs.microsoft.com/azure/quantum/how-to-create-workspace) how-to guide to set up your Workspace and enable your preferred providers.
 
 To get started, visit the following Quickstart guides:
 
 - [Quickstart: Submit a circuit with Qiskit](https://docs.microsoft.com/azure/quantum/quickstart-microsoft-qiskit)
 - [Quickstart: Submit a circuit with Cirq](https://docs.microsoft.com/azure/quantum/quickstart-microsoft-qiskit)
 - [Quickstart: Submit a circuit with a provider-specific format](https://docs.microsoft.com/azure/quantum/quickstart-microsoft-provider-format).
-- [Quickstart: Solve a simple optimization problem](https://docs.microsoft.com/azure/quantum/quickstart-microsoft-qio?pivots=platform-microsoft#express-a-simple-problem).
 
 ## General usage ##
 
 To connect to your Azure Quantum Workspace, go to the [Azure Portal](https://portal.azure.com), navigate to your Workspace and copy-paste the resource ID and location into the code snippet below.
 
 ```python
 from azure.quantum import Workspace
```

### Comparing `azure-quantum-0.28.277227/README.md` & `azure-quantum-0.28.291393b1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 To work in Azure Quantum, you need an Azure subscription. If you don't have an Azure subscription, create a [free account](https://azure.microsoft.com/free/). Follow the [Create an Azure Quantum workspace](https://docs.microsoft.com/azure/quantum/how-to-create-workspace) how-to guide to set up your Workspace and enable your preferred providers.
 
 To get started, visit the following Quickstart guides:
 
 - [Quickstart: Submit a circuit with Qiskit](https://docs.microsoft.com/azure/quantum/quickstart-microsoft-qiskit)
 - [Quickstart: Submit a circuit with Cirq](https://docs.microsoft.com/azure/quantum/quickstart-microsoft-qiskit)
 - [Quickstart: Submit a circuit with a provider-specific format](https://docs.microsoft.com/azure/quantum/quickstart-microsoft-provider-format).
-- [Quickstart: Solve a simple optimization problem](https://docs.microsoft.com/azure/quantum/quickstart-microsoft-qio?pivots=platform-microsoft#express-a-simple-problem).
 
 ## General usage ##
 
 To connect to your Azure Quantum Workspace, go to the [Azure Portal](https://portal.azure.com), navigate to your Workspace and copy-paste the resource ID and location into the code snippet below.
 
 ```python
 from azure.quantum import Workspace
```

### Comparing `azure-quantum-0.28.277227/azure/quantum/_authentication/_chained.py` & `azure-quantum-0.28.291393b1/azure/quantum/_authentication/_chained.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_authentication/_default.py` & `azure-quantum-0.28.291393b1/azure/quantum/_authentication/_default.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_authentication/_token.py` & `azure-quantum-0.28.291393b1/azure/quantum/_authentication/_token.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_client/__init__.py` & `azure-quantum-0.28.291393b1/azure/quantum/_client/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_client/_client.py` & `azure-quantum-0.28.291393b1/azure/quantum/_client/_client.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_client/_configuration.py` & `azure-quantum-0.28.291393b1/azure/quantum/_client/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_client/_patch.py` & `azure-quantum-0.28.291393b1/azure/quantum/_client/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_client/_serialization.py` & `azure-quantum-0.28.291393b1/azure/quantum/_client/_serialization.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_client/_vendor.py` & `azure-quantum-0.28.291393b1/azure/quantum/_client/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_client/aio/__init__.py` & `azure-quantum-0.28.291393b1/azure/quantum/_client/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_client/aio/_client.py` & `azure-quantum-0.28.291393b1/azure/quantum/_client/aio/_client.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_client/aio/_configuration.py` & `azure-quantum-0.28.291393b1/azure/quantum/_client/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_client/aio/_patch.py` & `azure-quantum-0.28.291393b1/azure/quantum/_client/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_client/aio/operations/__init__.py` & `azure-quantum-0.28.291393b1/azure/quantum/_client/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_client/aio/operations/_operations.py` & `azure-quantum-0.28.291393b1/azure/quantum/_client/aio/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_client/aio/operations/_patch.py` & `azure-quantum-0.28.291393b1/azure/quantum/_client/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_client/models/__init__.py` & `azure-quantum-0.28.291393b1/azure/quantum/_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_client/models/_enums.py` & `azure-quantum-0.28.291393b1/azure/quantum/_client/models/_enums.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_client/models/_models.py` & `azure-quantum-0.28.291393b1/azure/quantum/_client/models/_models.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_client/models/_patch.py` & `azure-quantum-0.28.291393b1/azure/quantum/_client/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_client/operations/__init__.py` & `azure-quantum-0.28.291393b1/azure/quantum/_client/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_client/operations/_operations.py` & `azure-quantum-0.28.291393b1/azure/quantum/_client/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/_client/operations/_patch.py` & `azure-quantum-0.28.291393b1/azure/quantum/_client/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/aio/_authentication/_chained.py` & `azure-quantum-0.28.291393b1/azure/quantum/aio/_authentication/_chained.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/aio/_authentication/_default.py` & `azure-quantum-0.28.291393b1/azure/quantum/aio/_authentication/_default.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/aio/_authentication/_token.py` & `azure-quantum-0.28.291393b1/azure/quantum/aio/_authentication/_token.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/aio/job/base_job.py` & `azure-quantum-0.28.291393b1/azure/quantum/aio/job/base_job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/aio/job/job.py` & `azure-quantum-0.28.291393b1/azure/quantum/aio/job/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/aio/optimization/online_problem.py` & `azure-quantum-0.28.291393b1/azure/quantum/aio/optimization/online_problem.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/aio/optimization/problem.py` & `azure-quantum-0.28.291393b1/azure/quantum/aio/optimization/problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,24 +38,24 @@
     :param problem_type: Problem type (ProblemType.pubo or
         ProblemType.ising), defaults to ProblemType.ising
     :type problem_type: ProblemType, optional
     """
     async def upload(
         self,
         workspace: "Workspace",
-        container_name: str = "qio-problems",
+        container_name: str = "optimization-problems",
         blob_name: str = "inputData",
         container_uri: str = None
     ):
         """Uploads an optimization problem instance to
         the cloud storage linked with the Workspace.
 
         :param workspace: interaction terms of the problem.
         :type workspace: Workspace
-        :param container_name: Container name, defaults to "qio-problems"
+        :param container_name: Container name, defaults to "optimization-problems"
         :type container_name: str, optional
         :param blob_name: Blob name, defaults to None
         :type blob_name: str, optional
         :param container_uri: Optional container URI
         :type container_uri: str
         :return: uri of the uploaded problem
         :rtype: str
```

### Comparing `azure-quantum-0.28.277227/azure/quantum/aio/optimization/streaming_problem.py` & `azure-quantum-0.28.291393b1/azure/quantum/aio/optimization/streaming_problem.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/aio/storage.py` & `azure-quantum-0.28.291393b1/azure/quantum/aio/storage.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/aio/target/ionq.py` & `azure-quantum-0.28.291393b1/azure/quantum/aio/target/ionq.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/aio/target/quantinuum.py` & `azure-quantum-0.28.291393b1/azure/quantum/aio/target/quantinuum.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/aio/target/solvers.py` & `azure-quantum-0.28.291393b1/azure/quantum/aio/target/solvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 if TYPE_CHECKING:
     from azure.quantum.aio.optimization.problem import Problem
 
 logger = logging.getLogger(__name__)
 
 __all__ = [
-    "HardwarePlatform",
     "RangeSchedule",
     "Solver",
 ]
 
 
 class Solver(Target, SyncSolver):
```

### Comparing `azure-quantum-0.28.277227/azure/quantum/aio/target/target.py` & `azure-quantum-0.28.291393b1/azure/quantum/aio/target/target.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/aio/target/target_factory.py` & `azure-quantum-0.28.291393b1/azure/quantum/aio/target/target_factory.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/aio/workspace.py` & `azure-quantum-0.28.291393b1/azure/quantum/aio/workspace.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/argument_types/types.py` & `azure-quantum-0.28.291393b1/azure/quantum/argument_types/types.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/cirq/job.py` & `azure-quantum-0.28.291393b1/azure/quantum/cirq/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/cirq/service.py` & `azure-quantum-0.28.291393b1/azure/quantum/cirq/service.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/cirq/targets/ionq.py` & `azure-quantum-0.28.291393b1/azure/quantum/cirq/targets/ionq.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/cirq/targets/quantinuum.py` & `azure-quantum-0.28.291393b1/azure/quantum/cirq/targets/quantinuum.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/cirq/targets/target.py` & `azure-quantum-0.28.291393b1/azure/quantum/cirq/targets/target.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/job/base_job.py` & `azure-quantum-0.28.291393b1/azure/quantum/job/base_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_TIMEOUT = 300  # Default timeout for waiting for job to complete
 
 class ContentType(str, Enum):
     json = "application/json"
-    protobuf = "application/x-protobuf"
 
 class BaseJob(WorkspaceItem):
     # Optionally override these to create a Provider-specific Job subclass
     """
     Base job class with methods to create a job from raw blob data,
     upload blob data and download results.
     """
@@ -233,15 +232,15 @@
     ) -> str:
         """Upload input data file
 
         :param container_uri: Container URI
         :type container_uri: str
         :param input_data: Input data in binary format
         :type input_data: bytes
-        :param content_type: Content type, e.g. "application/json" or "application/x-protobuf"
+        :param content_type: Content type, e.g. "application/json"
         :type content_type: Optional, ContentType
         :param blob_name: Blob name, defaults to "inputData"
         :type blob_name: str, optional
         :param encoding: Encoding, e.g. "gzip", defaults to ""
         :type encoding: str, optional
         :param return_sas_token: Flag to return SAS token as part of URI, defaults to False
         :type return_sas_token: bool, optional
```

### Comparing `azure-quantum-0.28.277227/azure/quantum/job/filtered_job.py` & `azure-quantum-0.28.291393b1/azure/quantum/job/filtered_job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/job/job.py` & `azure-quantum-0.28.291393b1/azure/quantum/job/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/job/session.py` & `azure-quantum-0.28.291393b1/azure/quantum/job/session.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/job/workspace_item.py` & `azure-quantum-0.28.291393b1/azure/quantum/job/workspace_item.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/job/workspace_item_factory.py` & `azure-quantum-0.28.291393b1/azure/quantum/job/workspace_item_factory.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/optimization/online_problem.py` & `azure-quantum-0.28.291393b1/azure/quantum/optimization/online_problem.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/optimization/streaming_problem.py` & `azure-quantum-0.28.291393b1/azure/quantum/optimization/streaming_problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,22 +119,20 @@
                 self.workspace.storage, self.id
             )
 
         return {"blob_name": blob_name, "container_client": container_client}
 
     def add_terms(
         self,
-        terms: List[Term],
-        c: Union[int, float] = 1
+        terms: List[Term]
     ):
         """Adds a list of terms to the `Problem`
          representation and queues them to be uploaded. Special terms are not supported.
 
         :param terms: The list of terms to add to the problem
-        :param c: Weight of grouped term, if applicable
         """
         if self.uploaded_uri is not None:
             raise Exception("Cannot add terms after problem has been uploaded")
 
         if terms is not None:
             if self.uploader is None:
                 upload_coords = self._get_upload_coords()
@@ -185,15 +183,15 @@
         blob = coords["container_client"].get_blob_client(coords["blob_name"])
         contents = download_blob(blob.url)
         return Problem.deserialize(contents, self.name)
 
     def upload(
         self,
         workspace,
-        container_name: str = "qio-problems",
+        container_name: str = "optimization-problems",
         blob_name: str = None,
     ):
         """Uploads an optimization problem instance
            to the cloud storage linked with the Workspace.
 
         :param workspace: interaction terms of the problem.
         :return: uri of the uploaded problem
```

### Comparing `azure-quantum-0.28.277227/azure/quantum/optimization/term.py` & `azure-quantum-0.28.291393b1/azure/quantum/optimization/term.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from __future__ import annotations
 import numpy as np
 from typing import List, Dict, Union, Optional
 from enum import Enum
 from abc import ABC
 
-__all__ = ["TermBase", "Term", "GroupType", "SlcTerm"]
+__all__ = ["TermBase", "Term"]
 
 try:
     import numpy.typing as npt
 
     WArray = Union[int, float, npt.ArrayLike]
 
     def _convert_if_numpy_type(param: WArray):
@@ -197,117 +197,7 @@
                 new_ids.append(i)
             else:
                 new_c *= fixed_variables[i]
                 if new_c == 0:
                     return None
 
         return Term(indices=new_ids, c=new_c)
-
-
-class GroupType(str, Enum):
-    combination = "na"
-    squared_linear_combination = "slc"
-
-class SlcTerm(TermBase):
-    """
-    Squared Linear Combination term class.
-    """
-    def __init__(
-        self,
-        terms: List[Term],
-        c: Optional[WArray] = 1.0,
-    ):
-        TermBase.__init__(self, c=c)
-        self.terms = terms
-        self.validate()
-    
-    def validate(self):
-        """
-        Check for and raise errors in Squared Linear Combination formulation.
-        """
-        # Check linearity of terms and that like terms are combined
-        seen = set()
-        for term in self.terms:
-            if len(term.ids) > 1:
-                # Nonlinear term
-                raise ValueError("Error - terms must be linear in type SlcTerm")
-            elif len(term.ids) == 1:
-                # Linear term
-                id = term.ids[0]
-            else:
-                # Constant term
-                id = -1
-            if id in seen:
-                raise ValueError("Error - like terms must be combined in type SlcTerm")
-            else:
-                seen.add(id)
-
-
-    def to_dict(self):
-        """
-        Return dictionary format of SlcTerm for solver input
-        """
-        return {
-            'c': self.c,
-            'terms': [monomial_term.to_dict() for monomial_term in self.terms],
-        }
-    
-    @classmethod
-    def from_dict(cls, obj: dict):
-        """
-        Create SlcTerm from dictionary with keys "terms" and "c"
-        """
-        try:
-            terms = [Term.from_dict(term_dict) for term_dict in obj["terms"]]
-        except:
-            print(
-                "Error - grouped list of terms missing or errant for squared linear combination type."
-            )
-            raise
-        return cls(terms=terms, c=obj["c"])
-    
-    def evaluate(self, configuration: Dict[int, int]) -> float:
-        """Given a variable configuration, evaluate the value of the slc term.
-        :param configuration:
-            Dictionary in which each key is a variable id;
-            each value is the variable assignment (usually -1, 0, or 1)
-        """
-        combination_eval = 0.0
-        for term in self.terms:
-            combination_eval += term.evaluate(configuration)
-        eval = self.c * combination_eval**2
-        
-        return eval
-    
-    def reduce_by_variable_state(
-        self,
-        fixed_variables: Dict[int, int]
-    ) -> Optional[TermBase]:
-        """Given some fixed variable states,
-            transform the existing grouped term into new term.
-        Returns None if the new term is effectively 0
-        :param fixed_variables:
-            The dictionary of variable ids and their fixed state
-        """
-        new_terms_dict = dict()
-        for monomial in self.terms:
-            new_monomial = monomial.reduce_by_variable_state(fixed_variables)
-            if new_monomial:
-                ids = tuple(sorted(new_monomial.ids))
-                try:
-                    new_terms_dict[ids] += new_monomial.c
-                except:
-                    new_terms_dict[ids] = new_monomial.c
-        new_terms = [Term(indices=list(ids), c=c) for ids,c in new_terms_dict.items()]
-        if len(new_terms) == 0:
-            return None
-
-        # Slc simplifications when new_terms has a single constant element
-        # such as simplifying an SLC term consisting of a single variable
-        if len(new_terms) == 1:
-            term = new_terms[0]
-            if len(term.ids) == 0:
-                # Simplify SLC term consisting of a single constant
-                # For example, C(k)^2 as a GroupedTerm to Ck^2 as a Term
-                return Term(indices=[], c=self.c * term.c**2)
-
-        return SlcTerm(terms=new_terms, c=self.c)
```

### Comparing `azure-quantum-0.28.277227/azure/quantum/qiskit/backends/__init__.py` & `azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/qiskit/backends/backend.py` & `azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/backend.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/qiskit/backends/ionq.py` & `azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/ionq.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/qiskit/backends/microsoft.py` & `azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/microsoft.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/qiskit/backends/qci.py` & `azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/qci.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/qiskit/backends/quantinuum.py` & `azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/quantinuum.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/qiskit/backends/rigetti.py` & `azure-quantum-0.28.291393b1/azure/quantum/qiskit/backends/rigetti.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/qiskit/job.py` & `azure-quantum-0.28.291393b1/azure/quantum/qiskit/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/qiskit/provider.py` & `azure-quantum-0.28.291393b1/azure/quantum/qiskit/provider.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/qiskit/results/resource_estimator.py` & `azure-quantum-0.28.291393b1/azure/quantum/qiskit/results/resource_estimator.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/storage.py` & `azure-quantum-0.28.291393b1/azure/quantum/storage.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/target/ionq.py` & `azure-quantum-0.28.291393b1/azure/quantum/target/ionq.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/target/microsoft/job.py` & `azure-quantum-0.28.291393b1/azure/quantum/target/microsoft/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/target/microsoft/result.py` & `azure-quantum-0.28.291393b1/azure/quantum/target/microsoft/result.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ##
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 ##
 from typing import Any, Dict, List, Optional, Union
 
+import json
 import markdown
 
 
 class HTMLWrapper:
     """
     Simple HTML wrapper to expose _repr_html_ for Jupyter clients.
     """
@@ -26,14 +27,16 @@
 
         if isinstance(data, dict):
             super().__init__(data)
 
             self._is_simple = True
             self._repr = self._item_result_table()
             self.summary = HTMLWrapper(self._item_result_summary_table())
+            self.diagram = EstimatorResultDiagram(self.data().copy())
+
         elif isinstance(data, list):
             super().__init__({idx: MicrosoftEstimatorResult(item_data)
                               for idx, item_data in enumerate(data)})
 
             self._data = data
             self._is_simple = False
             num_items = len(data)
@@ -163,64 +166,32 @@
         # get labels or use default value, then extend with missing elements,
         # and truncate extra elements
         labels = kwargs.pop("labels", [])
         labels.extend(range(len(labels), len(self)))
         labels = labels[:len(self)]
 
         def get_row(result):
-            physical_counts = result["physicalCounts"]
-            breakdown = physical_counts["breakdown"]
+            formatted = result["physicalCountsFormatted"]
 
-            # Extract raw data from result dictionary
-            logical_qubits = breakdown["algorithmicLogicalQubits"]
-            logical_depth = breakdown["logicalDepth"]
-            num_tstates = breakdown["numTstates"]
-            code_distance = result["logicalQubit"]["codeDistance"]
-            num_tfactories = breakdown["numTfactories"]
-            tfactory_fraction = (breakdown["physicalQubitsForTfactories"] /
-                                 physical_counts["physicalQubits"]) * 100
-            physical_qubits = physical_counts["physicalQubits"]
-            runtime = physical_counts["runtime"]
-
-            # Format some entries
-            logical_depth_formatted = f"{logical_depth:.1e}"
-            num_tstates_formatted = f"{num_tstates:.1e}"
-            tfactory_fraction_formatted = f"{tfactory_fraction:.1f}%"
-            physical_qubits_formatted = f"{physical_qubits / 1e6:.2f}M"
-
-            # Make runtime human readable; we find the largest units for which
-            # the runtime has a value that is larger than 1.0. For that unit we
-            # are rounding the value and append the unit suffix.
-            units = [("nanosecs", 1), ("microsecs", 1000), ("millisecs", 1000),
-                     ("secs", 1000), ("mins", 60), ("hours", 60), ("days", 24),
-                     ("years", 365)]
-            runtime_formatted = runtime
-            for idx in range(1, len(units)):
-                if runtime_formatted / units[idx][1] < 1.0:
-                    rounded_value = round(runtime_formatted) % units[idx][1]
-                    runtime_formatted = f"{rounded_value} {units[idx - 1][0]}"
-                    break
-                else:
-                    runtime_formatted = runtime_formatted / units[idx][1]
-
-            # special case for years
-            if isinstance(runtime_formatted, float):
-                runtime_formatted = \
-                    f"{round(runtime_formatted)} {units[-1][0]}"
-
-            # Append all extracted and formatted data to data array
-            return (logical_qubits, logical_depth_formatted,
-                    num_tstates_formatted, code_distance, num_tfactories,
-                    tfactory_fraction_formatted, physical_qubits_formatted,
-                    runtime_formatted)
+            return (
+                formatted["algorithmicLogicalQubits"],
+                formatted["logicalDepth"],
+                formatted["numTstates"],
+                result["logicalQubit"]["codeDistance"],
+                formatted["numTfactories"],
+                formatted["physicalQubitsForTfactoriesPercentage"],
+                formatted["physicalQubits"],
+                formatted["rqops"],
+                formatted["runtime"]
+            )
 
         data = [get_row(self.data(index)) for index in range(len(self))]
         columns = ["Logical qubits", "Logical depth", "T states",
                    "Code distance", "T factories", "T factory fraction",
-                   "Physical qubits", "Physical runtime"]
+                   "Physical qubits", "rQOPS", "Physical runtime"]
         return pd.DataFrame(data, columns=columns, index=labels)
 
     def _item_result_table(self):
         html = ""
 
         md = markdown.Markdown(extensions=['mdx_math'])
         for group in self['reportData']['groups']:
@@ -373,7 +344,28 @@
 
         html += f"<details><summary style=\"display:list-item\"><strong>Assumptions</strong></summary><ul>"
         for assumption in self[0]['reportData']['assumptions']:
             html += f"<li>{md.convert(assumption)}</li>"
         html += "</ul></details>"
 
         return html
+
+
+class EstimatorResultDiagram:
+    def __init__(self, data):
+        data.pop("reportData")
+        self.data_json = json.dumps(data).replace(" ", "")
+        self.vis_lib = "https://cdn-aquavisualization-prod.azureedge.net/resource-estimation/index.js"
+        self.space = HTMLWrapper(self._space_diagram())
+        self.time = HTMLWrapper(self._time_diagram())
+
+    def _space_diagram(self):
+        html = f"""
+            <script src={self.vis_lib}></script>
+            <re-space-diagram data={self.data_json}></re-space-diagram>"""
+        return html
+
+    def _time_diagram(self):
+        html = f"""
+            <script src={self.vis_lib}></script>
+            <re-time-diagram data={self.data_json}></re-time-diagram>"""
+        return html
```

### Comparing `azure-quantum-0.28.277227/azure/quantum/target/oneqbit/solvers.py` & `azure-quantum-0.28.291393b1/azure/quantum/target/solvers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,305 +1,376 @@
 ##
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 ##
-import logging
 import warnings
+import logging
+
+from typing import TYPE_CHECKING, Union, Any, Optional
+from enum import Enum
+from azure.quantum.job.base_job import ContentType
+from azure.quantum import Workspace, Job
+from azure.quantum.job.base_job import DEFAULT_TIMEOUT
+from azure.quantum.target.target import Target
 
-from typing import Optional, List
-from azure.quantum import Workspace
-from azure.quantum.target import Solver
+if TYPE_CHECKING:
+    from azure.quantum.optimization.problem import Problem
 
 logger = logging.getLogger(__name__)
 
-__all__ = ["TabuSearch", "PticmSolver", "PathRelinkingSolver"]
+__all__ = [
+    "RangeSchedule",
+    "Solver",
+]
 
 
-class TabuSearch(Solver):
-    target_names = ("1qbit.tabu",)
 
+class RangeSchedule:
+    def __init__(self, schedule_type: str, initial: float, final: float):
+        """Constructor of RangeSchedule for solvers.
+
+        :param schedule_type:
+            str, type of the RangeSchedule
+            currently only supports 'linear' and 'geometric'.
+        :param initial:
+            float, initial value of RangeSchedule
+        :param final:
+            float, final value of the RangeSchedule
+        """
+        self.schedule_type = schedule_type
+        self.initial = initial
+        self.final = final
+        if not (
+            self.schedule_type == "linear" or self.schedule_type == "geometric"
+        ):
+            raise ValueError(
+                '"schedule_type" must be "linear" or "geometric"!'
+            )
+
+class Solver(Target):
     def __init__(
         self,
         workspace: Workspace,
-        name: str = "1qbit.tabu",
-        improvement_cutoff: Optional[int] = None,
-        improvement_tolerance: Optional[float] = None,
-        seed: Optional[int] = None,
-        tabu_tenure: Optional[int] = None,
-        tabu_tenure_rand_max: Optional[int] = None,
-        timeout: Optional[int] = None,
+        name: str,
+        provider_id: str,
+        input_data_format="microsoft.qio.v2",
+        output_data_format="microsoft.qio-results.v2",
+        nested_params: bool = True,
+        force_str_params: bool = False,
+        params: dict = None,
+        content_type : Optional[ContentType] = ContentType.json,
         **kwargs
     ):
-        """The constructor of a Tabu Search solver.
+        self.provider_id = provider_id
+        self.nested_params = nested_params
+        self.force_str_params = force_str_params
+        self.params = {"params": {}} if nested_params else {}
+        params = params or {}
+        name = self._switch_name(name, **params)
 
-        An iterative heuristic algorithm that uses local search techniques
-        to solve a QUBO problem. It starts from a random solution and looks
-        for an improved solution in the solution's neighborhood which includes
-        all possible single flips.
-        The algorithm stops when it reaches a stopping
-        criterion, such as a specified number of consecutive iterations without
-        improvement.
-
-        For more information please visit:
-        https://portal.1qbit.com/docs/model/tabusolver
-
-        :param improvement_cutoff:
-            The number of iterations that
-            the solver attempts with no improvement
-            before stopping. Default: 0
-        :param improvement_tolerance:
-            The tolerance value that determines if a solution is an improvement
-            over the previous iteration. Default: 1e-9
-        :param seed:
-            The seed in the random number generator to control for deterministic
-            results. Default: a random integer
-        :param tabu_tenure:
-            The tenure prevents a flipped
-            variable from being flipped again during
-            the iterations. Default: 0
-        :param tabu_tenure_rand_max:
-            The upper limit of the exclusive range of random integers.
-            Valid value range: 1 to 200,000. Default: 0
-        :param timeout:
-            The duration in ms the solver
-            runs before exiting. If the value is set
-            to 0, it does not time out. Default: 0
-        """
         super().__init__(
             workspace=workspace,
-            provider_id="1qbit",
             name=name,
-            input_data_format="microsoft.qio.v2",
-            output_data_format="microsoft.qio-results.v1",
-            nested_params=False,
-            force_str_params=True,
+            input_data_format=input_data_format,
+            output_data_format=output_data_format,
+            provider_id=provider_id,
+            content_type = content_type,
+            encoding="gzip",
             **kwargs
         )
+ 
+        self._set_params(**params)
+        self._check_params(**params)
+
+
+    """Constants that define thresholds for submission warnings
+    """
+    SWEEPS_WARNING = 10000
+    TIMEOUT_WARNING = 600
+
+    def _switch_name(self, name, **params):
+        return name
+
+    def _check_params(self, **params):
+        pass
+
+    @staticmethod
+    def _encode_input_data(data: "Problem") -> bytes:
+        return data.to_blob()
+
+    def submit(
+        self, problem: Union[str, "Problem"]) -> Job:
+        """Submits a job to execution to the associated
+        Azure Quantum Workspace.
+
+        :param problem:
+            The Problem to solve. It can be an instance of a Problem,
+            or the URL of an Azure Storage Blob where the serialized version
+            of a Problem has been uploaded.
+        """
+        from azure.quantum.optimization import Problem
+        if isinstance(problem, Problem):
+            return super().submit(
+                input_data=problem,
+                name=problem.name,
+                input_params=self.params,
+                blob_name="inputData",
+                content_type = problem.content_type
+            )
+
+        else:
+            if hasattr(problem, "uploaded_blob_uri"):
+                name = problem.name
+                problem_uri = problem.uploaded_blob_uri
+
+            elif isinstance(problem, str):
+                name = "Optimization problem"
+                problem_uri = problem
+            
+            else:
+                raise ValueError("Cannot submit problem: should be of type str, Problem or have uploaded_blob_uri attribute.")
+
+            # Create job from storage URI
+            job = Job.from_storage_uri(
+                workspace=self.workspace,
+                name=name,
+                target=self.name,
+                input_data_uri=problem_uri,
+                provider_id=self.provider_id,
+                input_data_format=self.input_data_format,
+                output_data_format=self.output_data_format,
+                input_params=self.params,
+                session_id=self.get_latest_session_id()
+            )
+
+        return job
+
+    def optimize(self, problem: Union[str, "Problem"], timeout_secs: int=DEFAULT_TIMEOUT):
+        """[Submits the Problem to the associated
+            Azure Quantum Workspace and get the results.
+
+        :param problem:
+            The Problem to solve. It can be an instance of a Problem,
+            or the URL of an Azure Storage Blob where the serialized version
+            of a Problem has been uploaded.
+        :type problem: Union[str, Problem]
+        :param timeout_secs: Timeout in seconds, defaults to 300
+        :type timeout_secs: int
+        :return: Job results
+        :rtype: dict
+        """
+        if not isinstance(problem, str):
+            self.check_submission_warnings(problem)
 
-        self.set_one_param("improvement_cutoff", improvement_cutoff)
-        self.set_one_param("improvement_tolerance", improvement_tolerance)
-        self.set_one_param("seed", seed)
-        self.set_one_param("tabu_tenure", tabu_tenure)
-        self.set_one_param("tabu_tenure_rand_max", tabu_tenure_rand_max)
-        self.set_one_param("timeout", timeout)
+        job = self.submit(problem)
+        logger.info(f"Submitted job: '{job.id}'")
 
+        return job.get_results(timeout_secs=timeout_secs)
 
-class PticmSolver(Solver):
-    target_names = ("1qbit.pticm",)
+    def set_one_param(self, name: str, value: Any):
+        if value is not None:
+            params = (
+                self.params["params"] if self.nested_params else self.params
+            )
+            params[name] = str(value) if self.force_str_params else value
 
-    def __init__(
-        self,
-        workspace: Workspace,
-        name: str = "1qbit.pticm",
-        auto_set_temperatures: Optional[bool] = None,
-        elite_threshold: Optional[float] = None,
-        frac_icm_thermal_layers: Optional[float] = None,
-        frac_sweeps_fixing: Optional[float] = None,
-        frac_sweeps_idle: Optional[float] = None,
-        frac_sweeps_stagnation: Optional[float] = None,
-        goal: Optional[str] = None,
-        high_temp: Optional[float] = None,
-        low_temp: Optional[float] = None,
-        max_samples_per_layer: Optional[int] = None,
-        max_total_sweeps: Optional[int] = None,
-        manual_temperatures: Optional[List[float]] = None,
-        num_elite_temps: Optional[int] = None,
-        num_replicas: Optional[int] = None,
-        num_sweeps_per_run: Optional[int] = None,
-        num_temps: Optional[int] = None,
-        perform_icm: Optional[bool] = None,
-        scaling_type: Optional[str] = None,
-        seed: Optional[int] = None,
-        var_fixing_type: Optional[str] = None,
-        **kwargs
-    ):
-        """The constructor of a PTICM solver.
+    def _set_params(self, **params):
+        for param_name, param in params.items():
+            self.set_one_param(param_name, param)
+
+    def set_number_of_solutions(self, number_of_solutions: int):
+        """Sets the number of solutions to return.
 
-        The parallel tempering with isoenergetic
-        cluster moves (PTICM) solver is
-        a Monte Carlo approach to solving QUBO problems.
-        In this algorithm, multiple
-        replicas of the original system,
-        each with a different initial state, are
-        simulated at different temperatures simultaneously. The replicas at
-        neighboring temperatures are periodically swapped based on a Metropolis
-        criterion. These swaps allow
-        different replicas to do a random walk in the
-        temperature space, thereby, efficiently overcoming energy barriers.
-
-        For more information please visit:
-        https://portal.1qbit.com/docs/model/pticmsolver
-
-        :param auto_set_temperatures:
-            This defines whether the temperature parameters are auto-calculated
-            or not. Set it to True for
-            auto-calculating and False for customizing
-            the temperature parameters. Default: True
-        :param elite_threshold:
-            The fraction of the best solutions used for the var_fixing_type
-            parameter with value SPVAR. Default: 0.3
-        :param frac_icm_thermal_layers:
-            The fraction of temperatures for the iso-energetic cluster moves.
-            Default: 0.5
-        :param frac_sweeps_fixing:
-            The fraction of sweeps used for fixing the QUBO variables.
-            Default: 0.15
-        :param frac_sweeps_idle:
-            The fraction of sweeps to wait before fixing the QUBO variables.
-            Default: 1.0
-        :param frac_sweeps_stagnation:
-            The fraction of sweeps without improvement that triggers a restart.
-            Default: 1.0
-        :param goal:
-            This defines whether the solver is used for optimizing or sampling.
-            Valid values: "OPTIMIZE" or "SAMPLE". Default: "OPTIMIZE"
-        :param high_temp:
-            The highest temperature of a replica. Set the auto_set_temperatures
-            parameter to False to use this feature. Default: 2
-        :param low_temp:
-            The lowest temperature of a replica. Set the auto_set_temperatures
-            parameter to False to use this feature. Default: 0.2
-        :param max_samples_per_layer:
-            The maximum number of samples collected per replica. Default: 10
-        :param max_total_sweeps:
-            The total number of sweeps before termination.
-            Default: num_sweeps_per_run * 10
-        :param manual_temperatures:
-            An array of a custom temperature schedule which includes the high,
-            intermediate, and low temperature values for the replicas. Set the
-            auto_set_temperatures parameter to False to use this feature.
-        :param num_elite_temps:
-            The number of elite temperatures used for fixing the variables with
-            persistency. Default = 4
-        :param num_replicas:
-            The number of replicas at each temperature. Default: 2
-        :param num_sweeps_per_run:
-            The number of Monte Carlo sweeps. Default: 100
-        :param num_temps:
-            The number of temperatures including the highest and the lowest
-            temperatures. Set the auto_set_temperatures parameter to False to
-            use this feature. Default: 30
-        :param perform_icm:
-            This parameter is deprecated. Default: None
-        :param scaling_type:
-            This defines whether the QUBO problem
-            is automatically scaled or not.
-            "MEDIAN" means it's automatically
-            scaled, and "NO_SCALING" means it's
-            not. Valid values: "MEDIAN" or "NO_SCALING"
-        :param seed:
-            The seed in the random number generator to control for deterministic
-            results. Default: a random integer
-        :param var_fixing_type:
-            This decides whether the values of QUBO variables are fixed or not.
-            You can fix them with "PERSISTENCY" or
-            "SPVAR" types. "NO_FIXING" means the
-            variables are not fixed. If you
-            choose "PERSISTENCY" or "SPVAR", also
-            set the frac_sweeps_fixing and
-            frac_sweeps_idle parameters to a number
-            less than one. Valid values: "PERSISTENCY", "SPVAR" or "NO_FIXING".
-            Default: "NO_FIXING"
+        Applies to all solvers.
+        Default value is 1 if not supplied.
+
+        :param number_of_solutions:
+            Number of solutions to return. Must be a positive integer.
         """
-        if perform_icm is not None:
-            warnings.warn(DeprecationWarning("The perform_icm parameter has been deprecated and will be ignored."))
+        self.set_one_param("number_of_solutions", number_of_solutions)
 
-        super().__init__(
-            workspace=workspace,
-            provider_id="1qbit",
-            name=name,
-            input_data_format="microsoft.qio.v2",
-            output_data_format="microsoft.qio-results.v1",
-            nested_params=False,
-            force_str_params=True,
-            **kwargs
-        )
+    def check_submission_warnings(self, problem: "Problem"):
+        # print a warning if we suspect the job
+        # may take long based on its configured properties.
+        is_large_problem = problem.is_large()
+        if is_large_problem:
+            if self.nested_params and "sweeps" in self.params["params"]:
+                sweeps = int(self.params["params"]["sweeps"])
+                # if problem is large and sweeps is large, warn.
+                if sweeps >= Solver.SWEEPS_WARNING:
+                    logger.warning(
+                        f"There is a large problem submitted and \
+                        a large number of sweeps ({sweeps}) configured. \
+                        This submission could result in a long runtime."
+                    )
+
+        # do a timeout check if param-free, to warn
+        # new users who accidentally set high timeout values.
+        if self.nested_params and "timeout" in self.params["params"]:
+            timeout = int(self.params["params"]["timeout"])
+            if timeout >= Solver.TIMEOUT_WARNING:
+                logger.warning(
+                    f"A large timeout has been set for this submission \
+                        ({timeout}). \
+                        If this is intended, disregard this warning. \
+                        Otherwise, consider cancelling the job \
+                        and resubmitting with a lower timeout."
+                )
+    
+    class ScheduleEvolution(Enum):
+        INCREASING = 1
+        DECREASING = 2
 
-        self.set_one_param("auto_set_temperatures", auto_set_temperatures)
-        self.set_one_param("elite_threshold", elite_threshold)
-        self.set_one_param("frac_icm_thermal_layers", frac_icm_thermal_layers)
-        self.set_one_param("frac_sweeps_fixing", frac_sweeps_fixing)
-        self.set_one_param("frac_sweeps_idle", frac_sweeps_idle)
-        self.set_one_param("frac_sweeps_stagnation", frac_sweeps_stagnation)
-        self.set_one_param("goal", goal)
-        self.set_one_param("high_temp", high_temp)
-        self.set_one_param("low_temp", low_temp)
-        self.set_one_param("max_samples_per_layer", max_samples_per_layer)
-        self.set_one_param("max_total_sweeps", max_total_sweeps)
-        self.set_one_param("manual_temperatures", manual_temperatures)
-        self.set_one_param("num_elite_temps", num_elite_temps)
-        self.set_one_param("num_replicas", num_replicas)
-        self.set_one_param("num_sweeps_per_run", num_sweeps_per_run)
-        self.set_one_param("num_temps", num_temps)
-        self.set_one_param("scaling_type", scaling_type)
-        self.set_one_param("seed", seed)
-        self.set_one_param("var_fixing_type", var_fixing_type)
+    def check_set_schedule(
+        self,
+        schedule_name: str,
+        schedule_value: RangeSchedule,
+        evolution: Optional[ScheduleEvolution] = None,
+        lower_bound_exclusive: Optional[float] = None,
+        lower_bound_inclusive: Optional[float] = None,
+    ):
+        """Set the parameter `schedule_name` from the value `schedule_value`
+        and check that it is of type `RangeSchedule` and each end satisfies
+        the specified bound.
+
+        :param schedule_name:
+            Name of the schedule parameter.
+        :param schedule_value:
+            Schedule value to be assigned and checked.
+        :param evolution
+            Expected schedule evolution (INCREASING or DECREASING)
+        :lower_bound_exclusive:
+            Exclusive lower bound for both ends of the schedule, optional.
+        :lower_bound_inclusive:
+            Inclusive lower bound for both ends of the schedule, optional.
+        """
+        if not (schedule_value is None):
+            if not isinstance(schedule_value, RangeSchedule):
+                raise ValueError(
+                    f"{schedule_name} must be of type RangeSchedule; found"
+                    f" type({schedule_name})={type(schedule_value).__name__}."
+                )
+            schedule_param = {
+                "type": schedule_value.schedule_type,
+                "initial": schedule_value.initial,
+                "final": schedule_value.final,
+            }
+            if evolution is not None:
+                if (evolution == self.ScheduleEvolution.INCREASING and
+                        schedule_value.initial > schedule_value.final):
+                    raise ValueError(
+                            f"Schedule for {schedule_name} must be increasing;"
+                            f" found {schedule_name}.initial"
+                            f"={schedule_value.initial}"
+                            f" > {schedule_value.final}"
+                            f"={schedule_name}.final."
+                    )
+                if (evolution == self.ScheduleEvolution.DECREASING and
+                        schedule_value.initial < schedule_value.final):
+                    raise ValueError(
+                            f"Schedule for {schedule_name} must be decreasing;"
+                            f" found {schedule_name}.initial"
+                            f"={schedule_value.initial}"
+                            f" < {schedule_value.final}"
+                            f"={schedule_name}.final."
+                    )
+            self.check_limit(
+                    f"{schedule_name}.initial",
+                    schedule_value.initial,
+                    lower_bound_exclusive=lower_bound_exclusive,
+                    lower_bound_inclusive=lower_bound_inclusive)
+            self.check_limit(
+                    f"{schedule_name}.final",
+                    schedule_value.final,
+                    lower_bound_exclusive=lower_bound_exclusive,
+                    lower_bound_inclusive=lower_bound_inclusive)
+            self.set_one_param(schedule_name, schedule_param)
+
+    def check_set_positive_int(
+            self,
+            parameter_name: str,
+            parameter_value: int):
+        """Set the parameter `parameter_name` from the value `parameter_value`
+        and check that it is a positive integer.
+
+        :param parameter_name:
+            Name of the parameter.
+        :param parameter_value:
+            Value to be assigned and checked.
+        """
+        if not (parameter_value is None):
+            if not isinstance(parameter_value, int):
+                raise ValueError(
+                        f"{parameter_name} must be of type int; found"
+                        f"type({parameter_name})"
+                        f"={type(parameter_value).__name__}.")
+            if parameter_value <= 0:
+                raise ValueError(
+                        f"{parameter_name} must be positive; found "
+                        f"{parameter_name}={parameter_value}.")
+            self.set_one_param(parameter_name, parameter_value)
 
+    def check_set_float(
+        self,
+        parameter_name: str,
+        parameter_value: float,
+        lower_bound_exclusive: Optional[float] = None,
+        lower_bound_inclusive: Optional[float] = None,
+    ):
+        """Set the parameter `parameter_name` from the value `parameter_value`
+        and check that it has a float value satisfying bounds.
 
-class PathRelinkingSolver(Solver):
-    target_names = ("1qbit.pathrelinking",)
+        :param parameter_name:
+            Name of the parameter.
+        :param parameter_value:
+            Value to be assigned and checked.
+        :lower_bound_exclusive:
+            Exclusive lower bound to check parameter_value against, optional.
+        :lower_bound_inclusive:
+            Inclusive lower bound to check parameter_value against, optional.
+        """
+        if not (parameter_value is None):
+            if not (isinstance(parameter_value, float) or
+                    isinstance(parameter_value, int)):
+                raise ValueError(f"{parameter_name} must be a float!")
+            else:
+                self.check_limit(
+                        parameter_name=parameter_name,
+                        parameter_value=parameter_value,
+                        lower_bound_exclusive=lower_bound_exclusive,
+                        lower_bound_inclusive=lower_bound_inclusive)
+                self.set_one_param(parameter_name, parameter_value)
 
-    def __init__(
+    def check_limit(
         self,
-        workspace: Workspace,
-        name: str = "1qbit.pathrelinking",
-        distance_scale: Optional[float] = None,
-        greedy_path_relinking: Optional[bool] = None,
-        ref_set_count: Optional[int] = None,
-        seed: Optional[int] = None,
-        timeout: Optional[int] = None,
-        **kwargs
+        parameter_name: str,
+        parameter_value: Optional[float],
+        lower_bound_exclusive: Optional[float] = None,
+        lower_bound_inclusive: Optional[float] = None,
     ):
-        """The constructor of a Path-relinking Search solver.
+        """Check whether `parameter_value` satisfies a lower bound.
 
-        The path-relinking algorithm is a heuristic algorithm that uses the
-        tabu search as a subroutine to solve a QUBO problem. The algorithm
-        starts from a set of elite solutions found by the tabu search. It
-        then constructs a path between each pair of elite solutions, selects
-        one of the solutions along the path, and repeats the tabu search. If
-        the tabu search finds a distinct solution that is better than the
-        current worst elite solution, the elite solutions set is updated with
-        the new improved solution. This whole procedure is repeated until the
-        algorithm meets a stopping condition.
-
-        For more information please visit:
-        https://portal.1qbit.com/docs/model/pathrelinkingsolver
-
-        :param distance_scale:
-            The minimum distance from the initiating and guiding solutions for
-            constructing the candidate solution list. The highest quality
-            solution in the candidate solution list is then selected for
-            improvement. Valid values: 0.0 to 0.5. Default: 0.33
-        :param greedy_path_relinking:
-            When you use the path-relinking solver there are two ways you can
-            generate a path that leads to the solution:
-            one is the greedy function
-            and the other operates in a random matter. If you set the this
-            parameter to true, the solver will use the greedy function. If you
-            set it to false, it will use the random method. Default: False
-        :param ref_set_count:
-            The number of initial elite solutions to be generated by the tabu
-            search algorithm. Valid values: Greater than 1. Default: 10
-        :param seed:
-            The seed in the random number generator to control for deterministic
-            results. Default: a random integer
-        :param timeout:
-            The duration in ms the solver runs
-            before exiting. If the value is set
-            to 0, it does not time out. Default: 0
+        :param parameter_name:
+            Name of the parameter.
+        :param parameter_value:
+            Value to be checked.
+        :lower_bound_exclusive:
+            Exclusive lower bound to check parameter_value against, optional.
+        :lower_bound_inclusive:
+            Inclusive lower bound to check parameter_value against, optional.
         """
-        super().__init__(
-            workspace=workspace,
-            provider_id="1qbit",
-            name=name,
-            input_data_format="microsoft.qio.v2",
-            output_data_format="microsoft.qio-results.v1",
-            nested_params=False,
-            force_str_params=True,
-            **kwargs
-        )
+        if not (parameter_value is None):
+            if (lower_bound_exclusive is not None and
+                    parameter_value <= lower_bound_exclusive):
+                raise ValueError(
+                    f"{parameter_name} must be greater than "
+                    f"{lower_bound_exclusive}; "
+                    f"found {parameter_name}={parameter_value}."
+                )
+            if (lower_bound_inclusive is not None and
+                    parameter_value < lower_bound_inclusive):
+                raise ValueError(
+                    f"{parameter_name} must be greater equal "
+                    f"{lower_bound_inclusive}; found "
+                    f"{parameter_name}={parameter_value}."
+                )
 
-        self.set_one_param("distance_scale", distance_scale)
-        self.set_one_param("greedy_path_relinking", greedy_path_relinking)
-        self.set_one_param("ref_set_count", ref_set_count)
-        self.set_one_param("seed", seed)
-        self.set_one_param("timeout", timeout)
```

### Comparing `azure-quantum-0.28.277227/azure/quantum/target/params.py` & `azure-quantum-0.28.291393b1/azure/quantum/target/params.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/target/quantinuum.py` & `azure-quantum-0.28.291393b1/azure/quantum/target/quantinuum.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/target/rigetti/result.py` & `azure-quantum-0.28.291393b1/azure/quantum/target/rigetti/result.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/target/rigetti/target.py` & `azure-quantum-0.28.291393b1/azure/quantum/target/rigetti/target.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/target/target.py` & `azure-quantum-0.28.291393b1/azure/quantum/target/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,21 +222,14 @@
     def make_params(self):
         """
         Returns an input parameter object for convenient creation of input
         parameters.
         """
         return InputParams()
 
-    def supports_protobuf(self):
-        """
-        Return whether or not the Solver class supports protobuf serialization.
-        This should be overridden by Solver subclasses which do support protobuf.
-        """
-        return False
-
     def estimate_cost(
         self,
         input_data: Any,
         input_params: Union[Dict[str, Any], None] = None
     ):
         return NotImplementedError("Price estimation is not implemented yet for this target.")
```

### Comparing `azure-quantum-0.28.277227/azure/quantum/target/target_factory.py` & `azure-quantum-0.28.291393b1/azure/quantum/target/target_factory.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/target/toshiba/solvers.py` & `azure-quantum-0.28.291393b1/azure/quantum/target/toshiba/solvers.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure/quantum/workspace.py` & `azure-quantum-0.28.291393b1/azure/quantum/workspace.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-0.28.277227/azure_quantum.egg-info/PKG-INFO` & `azure-quantum-0.28.291393b1/azure_quantum.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-quantum
-Version: 0.28.277227
+Version: 0.28.291393b1
 Summary: Python client for Azure Quantum
 Home-page: https://github.com/microsoft/qdk-python
 Author: Microsoft
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -51,15 +51,14 @@
 To work in Azure Quantum, you need an Azure subscription. If you don't have an Azure subscription, create a [free account](https://azure.microsoft.com/free/). Follow the [Create an Azure Quantum workspace](https://docs.microsoft.com/azure/quantum/how-to-create-workspace) how-to guide to set up your Workspace and enable your preferred providers.
 
 To get started, visit the following Quickstart guides:
 
 - [Quickstart: Submit a circuit with Qiskit](https://docs.microsoft.com/azure/quantum/quickstart-microsoft-qiskit)
 - [Quickstart: Submit a circuit with Cirq](https://docs.microsoft.com/azure/quantum/quickstart-microsoft-qiskit)
 - [Quickstart: Submit a circuit with a provider-specific format](https://docs.microsoft.com/azure/quantum/quickstart-microsoft-provider-format).
-- [Quickstart: Solve a simple optimization problem](https://docs.microsoft.com/azure/quantum/quickstart-microsoft-qio?pivots=platform-microsoft#express-a-simple-problem).
 
 ## General usage ##
 
 To connect to your Azure Quantum Workspace, go to the [Azure Portal](https://portal.azure.com), navigate to your Workspace and copy-paste the resource ID and location into the code snippet below.
 
 ```python
 from azure.quantum import Workspace
```

### Comparing `azure-quantum-0.28.277227/azure_quantum.egg-info/SOURCES.txt` & `azure-quantum-0.28.291393b1/azure_quantum.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -47,22 +47,19 @@
 azure/quantum/aio/job/job.py
 azure/quantum/aio/optimization/__init__.py
 azure/quantum/aio/optimization/online_problem.py
 azure/quantum/aio/optimization/problem.py
 azure/quantum/aio/optimization/streaming_problem.py
 azure/quantum/aio/target/__init__.py
 azure/quantum/aio/target/ionq.py
-azure/quantum/aio/target/oneqbit.py
 azure/quantum/aio/target/quantinuum.py
 azure/quantum/aio/target/solvers.py
 azure/quantum/aio/target/target.py
 azure/quantum/aio/target/target_factory.py
 azure/quantum/aio/target/toshiba.py
-azure/quantum/aio/target/microsoft/__init__.py
-azure/quantum/aio/target/microsoft/qio.py
 azure/quantum/argument_types/__init__.py
 azure/quantum/argument_types/types.py
 azure/quantum/chemistry/__init__.py
 azure/quantum/cirq/__init__.py
 azure/quantum/cirq/job.py
 azure/quantum/cirq/service.py
 azure/quantum/cirq/targets/__init__.py
@@ -78,52 +75,39 @@
 azure/quantum/job/workspace_item_factory.py
 azure/quantum/optimization/__init__.py
 azure/quantum/optimization/online_problem.py
 azure/quantum/optimization/problem.py
 azure/quantum/optimization/solvers.py
 azure/quantum/optimization/streaming_problem.py
 azure/quantum/optimization/term.py
-azure/quantum/optimization/oneqbit/__init__.py
-azure/quantum/optimization/oneqbit/solvers.py
 azure/quantum/optimization/toshiba/__init__.py
 azure/quantum/optimization/toshiba/solvers.py
 azure/quantum/qiskit/__init__.py
 azure/quantum/qiskit/job.py
 azure/quantum/qiskit/provider.py
 azure/quantum/qiskit/backends/__init__.py
 azure/quantum/qiskit/backends/backend.py
 azure/quantum/qiskit/backends/ionq.py
 azure/quantum/qiskit/backends/microsoft.py
 azure/quantum/qiskit/backends/qci.py
 azure/quantum/qiskit/backends/quantinuum.py
 azure/quantum/qiskit/backends/rigetti.py
 azure/quantum/qiskit/results/__init__.py
 azure/quantum/qiskit/results/resource_estimator.py
-azure/quantum/serialization/__init__.py
-azure/quantum/serialization/problem_pb2.py
 azure/quantum/target/__init__.py
 azure/quantum/target/ionq.py
 azure/quantum/target/params.py
 azure/quantum/target/quantinuum.py
 azure/quantum/target/solvers.py
 azure/quantum/target/target.py
 azure/quantum/target/target_factory.py
 azure/quantum/target/microsoft/__init__.py
 azure/quantum/target/microsoft/job.py
 azure/quantum/target/microsoft/result.py
 azure/quantum/target/microsoft/target.py
-azure/quantum/target/microsoft/qio/__init__.py
-azure/quantum/target/microsoft/qio/parallel_tempering.py
-azure/quantum/target/microsoft/qio/population_annealing.py
-azure/quantum/target/microsoft/qio/quantum_monte_carlo.py
-azure/quantum/target/microsoft/qio/simulated_annealing.py
-azure/quantum/target/microsoft/qio/substochastic_montecarlo.py
-azure/quantum/target/microsoft/qio/tabu.py
-azure/quantum/target/oneqbit/__init__.py
-azure/quantum/target/oneqbit/solvers.py
 azure/quantum/target/rigetti/__init__.py
 azure/quantum/target/rigetti/result.py
 azure/quantum/target/rigetti/target.py
 azure/quantum/target/toshiba/__init__.py
 azure/quantum/target/toshiba/solvers.py
 azure_quantum.egg-info/PKG-INFO
 azure_quantum.egg-info/SOURCES.txt
```

### Comparing `azure-quantum-0.28.277227/azure_quantum.egg-info/requires.txt` & `azure-quantum-0.28.291393b1/azure_quantum.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,46 +2,41 @@
 azure-identity<2.0.0,>=1.12.0
 azure-storage-blob<13.0.0,>=12.14.1
 msrest<1.0,>=0.7.1
 numpy<2.0,>=1.21.0
 deprecated<2.0,>=1.2.12
 aiohttp<4.0,>=3.7.0
 aiofile<4.0,>=3.7.2
-protobuf<4.0,>=3.14.0
 Markdown>=3.4.1
 python-markdown-math>=0.8
 
 [all]
 cirq-core<2.0,>=1.1.0
 cirq-ionq<2.0,>=1.1.0
-urllib3==1.26.14
-vcrpy==4.2.1
-azure-devtools==1.2.0
-asyncmock<1.0,>=0.4.0
+vcrpy>=4.3.1
+azure-devtools<2.0,>=1.2.0
 qiskit-ionq<1.0,>=0.3.3
-qiskit-terra<1.0,>=0.19.1
+qiskit-terra<0.25.0,>=0.19.1
 qiskit-qir<0.4,>=0.3.1
 Markdown<4.0,>=3.4.1
 python-markdown-math<1.0,>=0.8.0
 qsharp>=0.28.263081
 pyquil>=3.3.2
 
 [cirq]
 cirq-core<2.0,>=1.1.0
 cirq-ionq<2.0,>=1.1.0
 
 [dev]
-urllib3==1.26.14
-vcrpy==4.2.1
-azure-devtools==1.2.0
-asyncmock<1.0,>=0.4.0
+vcrpy>=4.3.1
+azure-devtools<2.0,>=1.2.0
 
 [qiskit]
 qiskit-ionq<1.0,>=0.3.3
-qiskit-terra<1.0,>=0.19.1
+qiskit-terra<0.25.0,>=0.19.1
 qiskit-qir<0.4,>=0.3.1
 Markdown<4.0,>=3.4.1
 python-markdown-math<1.0,>=0.8.0
 
 [qsharp]
 qsharp>=0.28.263081
```

### Comparing `azure-quantum-0.28.277227/setup.py` & `azure-quantum-0.28.291393b1/setup.py`

 * *Files identical despite different names*

