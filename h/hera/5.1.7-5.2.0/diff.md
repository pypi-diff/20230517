# Comparing `tmp/hera-5.1.7.tar.gz` & `tmp/hera-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hera-5.1.7.tar", max compression
+gzip compressed data, was "hera-5.2.0.tar", max compression
```

## Comparing `hera-5.1.7.tar` & `hera-5.2.0.tar`

### file list

```diff
@@ -1,132 +1,133 @@
--rw-r--r--   0        0        0     1066 2023-04-29 15:25:11.644935 hera-5.1.7/LICENSE
--rw-r--r--   0        0        0    11696 2023-04-29 15:25:11.644935 hera-5.1.7/README.md
--rw-r--r--   0        0        0     3530 2023-04-29 15:25:26.389086 hera-5.1.7/pyproject.toml
--rw-r--r--   0        0        0      522 2023-04-29 15:25:11.656935 hera-5.1.7/src/hera/__init__.py
--rw-r--r--   0        0        0      300 2023-04-29 15:25:11.656935 hera-5.1.7/src/hera/_version.py
--rw-r--r--   0        0        0        0 2023-04-29 15:25:11.656935 hera-5.1.7/src/hera/events/__init__.py
--rw-r--r--   0        0        0     3267 2023-04-29 15:25:11.656935 hera-5.1.7/src/hera/events/models/__init__.py
--rw-r--r--   0        0        0     1418 2023-04-29 15:25:11.656935 hera-5.1.7/src/hera/events/models/eventsource.py
--rw-r--r--   0        0        0      861 2023-04-29 15:25:11.656935 hera-5.1.7/src/hera/events/models/eventsource.pyi
--rw-r--r--   0        0        0      144 2023-04-29 15:25:11.656935 hera-5.1.7/src/hera/events/models/google/__init__.py
--rw-r--r--   0        0        0      347 2023-04-29 15:25:11.656935 hera-5.1.7/src/hera/events/models/google/protobuf.py
--rw-r--r--   0        0        0      164 2023-04-29 15:25:11.656935 hera-5.1.7/src/hera/events/models/google/protobuf.pyi
--rw-r--r--   0        0        0        0 2023-04-29 15:25:11.656935 hera-5.1.7/src/hera/events/models/grpc/__init__.py
--rw-r--r--   0        0        0      144 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/grpc/gateway/__init__.py
--rw-r--r--   0        0        0      691 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/grpc/gateway/runtime.py
--rw-r--r--   0        0        0      470 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/grpc/gateway/runtime.pyi
--rw-r--r--   0        0        0        0 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/__init__.py
--rw-r--r--   0        0        0        0 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/argoproj/__init__.py
--rw-r--r--   0        0        0      144 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/argoproj/events/__init__.py
--rw-r--r--   0        0        0   102993 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/argoproj/events/v1alpha1.py
--rw-r--r--   0        0        0    25271 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/argoproj/events/v1alpha1.pyi
--rw-r--r--   0        0        0      144 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/argoproj/workflow/__init__.py
--rw-r--r--   0        0        0   144549 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/argoproj/workflow/v1alpha1.py
--rw-r--r--   0        0        0    31958 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi
--rw-r--r--   0        0        0        0 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/k8s/__init__.py
--rw-r--r--   0        0        0        0 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/k8s/api/__init__.py
--rw-r--r--   0        0        0      144 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/k8s/api/core/__init__.py
--rw-r--r--   0        0        0   127883 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/k8s/api/core/v1.py
--rw-r--r--   0        0        0    18004 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/k8s/api/core/v1.pyi
--rw-r--r--   0        0        0      144 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/k8s/api/policy/__init__.py
--rw-r--r--   0        0        0     1751 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/k8s/api/policy/v1beta1.py
--rw-r--r--   0        0        0      376 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/k8s/api/policy/v1beta1.pyi
--rw-r--r--   0        0        0        0 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/k8s/apimachinery/__init__.py
--rw-r--r--   0        0        0        0 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/__init__.py
--rw-r--r--   0        0        0      144 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/api/__init__.py
--rw-r--r--   0        0        0     3161 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py
--rw-r--r--   0        0        0      105 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.pyi
--rw-r--r--   0        0        0        0 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/apis/__init__.py
--rw-r--r--   0        0        0      144 2023-04-29 15:25:11.660935 hera-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
--rw-r--r--   0        0        0    22218 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
--rw-r--r--   0        0        0     2064 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
--rw-r--r--   0        0        0      144 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/util/__init__.py
--rw-r--r--   0        0        0      277 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.py
--rw-r--r--   0        0        0      108 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.pyi
--rw-r--r--   0        0        0     1453 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/events/models/sensor.py
--rw-r--r--   0        0        0      887 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/events/models/sensor.pyi
--rw-r--r--   0        0        0    26811 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/events/service.py
--rw-r--r--   0        0        0      282 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/expr/__init__.py
--rw-r--r--   0        0        0    12021 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/expr/_node.py
--rw-r--r--   0        0        0      647 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/expr/_sprig.py
--rw-r--r--   0        0        0        0 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/py.typed
--rw-r--r--   0        0        0      188 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/shared/__init__.py
--rw-r--r--   0        0        0      269 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/shared/_base_model.py
--rw-r--r--   0        0        0     4927 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/shared/_global_config.py
--rw-r--r--   0        0        0      513 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/shared/serialization.py
--rw-r--r--   0        0        0     4413 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/__init__.py
--rw-r--r--   0        0        0     2912 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/_context.py
--rw-r--r--   0        0        0    23864 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/_mixins.py
--rw-r--r--   0        0        0    32815 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/_unparse.py
--rw-r--r--   0        0        0       25 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/action.py
--rw-r--r--   0        0        0     1115 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/archive.py
--rw-r--r--   0        0        0     7697 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/artifact.py
--rw-r--r--   0        0        0     3446 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/container.py
--rw-r--r--   0        0        0     3988 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/container_set.py
--rw-r--r--   0        0        0     3763 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/cron_workflow.py
--rw-r--r--   0        0        0     2771 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/dag.py
--rw-r--r--   0        0        0     2186 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/data.py
--rw-r--r--   0        0        0     4855 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/env.py
--rw-r--r--   0        0        0     1329 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/env_from.py
--rw-r--r--   0        0        0      208 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/exceptions.py
--rw-r--r--   0        0        0     2291 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/http_template.py
--rw-r--r--   0        0        0       30 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/memoize.py
--rw-r--r--   0        0        0     6913 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/__init__.py
--rw-r--r--   0        0        0     1418 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/eventsource.py
--rw-r--r--   0        0        0      861 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/eventsource.pyi
--rw-r--r--   0        0        0      144 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/google/__init__.py
--rw-r--r--   0        0        0      347 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/google/protobuf.py
--rw-r--r--   0        0        0      164 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/google/protobuf.pyi
--rw-r--r--   0        0        0        0 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/grpc/__init__.py
--rw-r--r--   0        0        0      144 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/grpc/gateway/__init__.py
--rw-r--r--   0        0        0      691 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/grpc/gateway/runtime.py
--rw-r--r--   0        0        0      470 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/grpc/gateway/runtime.pyi
--rw-r--r--   0        0        0        0 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/__init__.py
--rw-r--r--   0        0        0        0 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/argoproj/__init__.py
--rw-r--r--   0        0        0      144 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/argoproj/events/__init__.py
--rw-r--r--   0        0        0   102993 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/argoproj/events/v1alpha1.py
--rw-r--r--   0        0        0    25271 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi
--rw-r--r--   0        0        0      144 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/argoproj/workflow/__init__.py
--rw-r--r--   0        0        0   144549 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py
--rw-r--r--   0        0        0    31958 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi
--rw-r--r--   0        0        0        0 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/k8s/__init__.py
--rw-r--r--   0        0        0        0 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/k8s/api/__init__.py
--rw-r--r--   0        0        0      144 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/k8s/api/core/__init__.py
--rw-r--r--   0        0        0   127883 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/k8s/api/core/v1.py
--rw-r--r--   0        0        0    18004 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/k8s/api/core/v1.pyi
--rw-r--r--   0        0        0      144 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/k8s/api/policy/__init__.py
--rw-r--r--   0        0        0     1751 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py
--rw-r--r--   0        0        0      376 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/k8s/api/policy/v1beta1.pyi
--rw-r--r--   0        0        0        0 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/__init__.py
--rw-r--r--   0        0        0        0 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/__init__.py
--rw-r--r--   0        0        0      144 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/__init__.py
--rw-r--r--   0        0        0     3161 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py
--rw-r--r--   0        0        0      105 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.pyi
--rw-r--r--   0        0        0        0 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/__init__.py
--rw-r--r--   0        0        0      144 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
--rw-r--r--   0        0        0    22218 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
--rw-r--r--   0        0        0     2064 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
--rw-r--r--   0        0        0      144 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/__init__.py
--rw-r--r--   0        0        0      277 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.py
--rw-r--r--   0        0        0      108 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.pyi
--rw-r--r--   0        0        0     1453 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/sensor.py
--rw-r--r--   0        0        0      887 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/models/sensor.pyi
--rw-r--r--   0        0        0      722 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/operator.py
--rw-r--r--   0        0        0     4084 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/parameter.py
--rw-r--r--   0        0        0     1018 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/protocol.py
--rw-r--r--   0        0        0     2554 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/resource.py
--rw-r--r--   0        0        0     5262 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/resources.py
--rw-r--r--   0        0        0     1856 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/retry_strategy.py
--rw-r--r--   0        0        0     3707 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/runner.py
--rw-r--r--   0        0        0    14818 2023-04-29 15:25:11.664935 hera-5.1.7/src/hera/workflows/script.py
--rw-r--r--   0        0        0    49251 2023-04-29 15:25:11.668935 hera-5.1.7/src/hera/workflows/service.py
--rw-r--r--   0        0        0     9297 2023-04-29 15:25:11.668935 hera-5.1.7/src/hera/workflows/steps.py
--rw-r--r--   0        0        0     3323 2023-04-29 15:25:11.668935 hera-5.1.7/src/hera/workflows/suspend.py
--rw-r--r--   0        0        0    10501 2023-04-29 15:25:11.668935 hera-5.1.7/src/hera/workflows/task.py
--rw-r--r--   0        0        0       27 2023-04-29 15:25:11.668935 hera-5.1.7/src/hera/workflows/toleration.py
--rw-r--r--   0        0        0     2007 2023-04-29 15:25:11.668935 hera-5.1.7/src/hera/workflows/user_container.py
--rw-r--r--   0        0        0     2610 2023-04-29 15:25:11.668935 hera-5.1.7/src/hera/workflows/validators.py
--rw-r--r--   0        0        0    18656 2023-04-29 15:25:11.668935 hera-5.1.7/src/hera/workflows/volume.py
--rw-r--r--   0        0        0    15572 2023-04-29 15:25:11.668935 hera-5.1.7/src/hera/workflows/workflow.py
--rw-r--r--   0        0        0      911 2023-04-29 15:25:11.668935 hera-5.1.7/src/hera/workflows/workflow_status.py
--rw-r--r--   0        0        0     5925 2023-04-29 15:25:11.668935 hera-5.1.7/src/hera/workflows/workflow_template.py
--rw-r--r--   0        0        0    13270 1970-01-01 00:00:00.000000 hera-5.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-17 14:27:07.480466 hera-5.2.0/LICENSE
+-rw-r--r--   0        0        0    11980 2023-05-17 14:27:07.480466 hera-5.2.0/README.md
+-rw-r--r--   0        0        0     3530 2023-05-17 14:27:29.296856 hera-5.2.0/pyproject.toml
+-rw-r--r--   0        0        0      522 2023-05-17 14:27:07.492467 hera-5.2.0/src/hera/__init__.py
+-rw-r--r--   0        0        0      300 2023-05-17 14:27:07.492467 hera-5.2.0/src/hera/_version.py
+-rw-r--r--   0        0        0        0 2023-05-17 14:27:07.492467 hera-5.2.0/src/hera/events/__init__.py
+-rw-r--r--   0        0        0     3267 2023-05-17 14:27:07.492467 hera-5.2.0/src/hera/events/models/__init__.py
+-rw-r--r--   0        0        0     1418 2023-05-17 14:27:07.492467 hera-5.2.0/src/hera/events/models/eventsource.py
+-rw-r--r--   0        0        0      861 2023-05-17 14:27:07.492467 hera-5.2.0/src/hera/events/models/eventsource.pyi
+-rw-r--r--   0        0        0      144 2023-05-17 14:27:07.492467 hera-5.2.0/src/hera/events/models/google/__init__.py
+-rw-r--r--   0        0        0      347 2023-05-17 14:27:07.492467 hera-5.2.0/src/hera/events/models/google/protobuf.py
+-rw-r--r--   0        0        0      164 2023-05-17 14:27:07.492467 hera-5.2.0/src/hera/events/models/google/protobuf.pyi
+-rw-r--r--   0        0        0        0 2023-05-17 14:27:07.492467 hera-5.2.0/src/hera/events/models/grpc/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-17 14:27:07.492467 hera-5.2.0/src/hera/events/models/grpc/gateway/__init__.py
+-rw-r--r--   0        0        0      691 2023-05-17 14:27:07.492467 hera-5.2.0/src/hera/events/models/grpc/gateway/runtime.py
+-rw-r--r--   0        0        0      470 2023-05-17 14:27:07.492467 hera-5.2.0/src/hera/events/models/grpc/gateway/runtime.pyi
+-rw-r--r--   0        0        0        0 2023-05-17 14:27:07.492467 hera-5.2.0/src/hera/events/models/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 14:27:07.492467 hera-5.2.0/src/hera/events/models/io/argoproj/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-17 14:27:07.492467 hera-5.2.0/src/hera/events/models/io/argoproj/events/__init__.py
+-rw-r--r--   0        0        0   102993 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/argoproj/events/v1alpha1.py
+-rw-r--r--   0        0        0    25271 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/argoproj/events/v1alpha1.pyi
+-rw-r--r--   0        0        0      144 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/argoproj/workflow/__init__.py
+-rw-r--r--   0        0        0   144549 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.py
+-rw-r--r--   0        0        0    31958 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi
+-rw-r--r--   0        0        0        0 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/k8s/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/k8s/api/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/k8s/api/core/__init__.py
+-rw-r--r--   0        0        0   127883 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/k8s/api/core/v1.py
+-rw-r--r--   0        0        0    18004 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/k8s/api/core/v1.pyi
+-rw-r--r--   0        0        0      144 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/k8s/api/policy/__init__.py
+-rw-r--r--   0        0        0     1751 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/k8s/api/policy/v1beta1.py
+-rw-r--r--   0        0        0      376 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/k8s/api/policy/v1beta1.pyi
+-rw-r--r--   0        0        0        0 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/k8s/apimachinery/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/k8s/apimachinery/pkg/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0        0        0     3161 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py
+-rw-r--r--   0        0        0      105 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.pyi
+-rw-r--r--   0        0        0        0 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
+-rw-r--r--   0        0        0    22218 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
+-rw-r--r--   0        0        0     2064 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
+-rw-r--r--   0        0        0      144 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/k8s/apimachinery/pkg/util/__init__.py
+-rw-r--r--   0        0        0      277 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.py
+-rw-r--r--   0        0        0      108 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.pyi
+-rw-r--r--   0        0        0     1453 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/sensor.py
+-rw-r--r--   0        0        0      887 2023-05-17 14:27:07.496467 hera-5.2.0/src/hera/events/models/sensor.pyi
+-rw-r--r--   0        0        0    26811 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/events/service.py
+-rw-r--r--   0        0        0      282 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/expr/__init__.py
+-rw-r--r--   0        0        0    12021 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/expr/_node.py
+-rw-r--r--   0        0        0      647 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/expr/_sprig.py
+-rw-r--r--   0        0        0        0 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/py.typed
+-rw-r--r--   0        0        0      188 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/shared/__init__.py
+-rw-r--r--   0        0        0      269 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/shared/_base_model.py
+-rw-r--r--   0        0        0     4927 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/shared/_global_config.py
+-rw-r--r--   0        0        0      513 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/shared/serialization.py
+-rw-r--r--   0        0        0     4585 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/__init__.py
+-rw-r--r--   0        0        0     2912 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/_context.py
+-rw-r--r--   0        0        0    27731 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/_mixins.py
+-rw-r--r--   0        0        0    32815 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/_unparse.py
+-rw-r--r--   0        0        0       25 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/action.py
+-rw-r--r--   0        0        0     1115 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/archive.py
+-rw-r--r--   0        0        0     7697 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/artifact.py
+-rw-r--r--   0        0        0     3464 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/container.py
+-rw-r--r--   0        0        0     4060 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/container_set.py
+-rw-r--r--   0        0        0     3763 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/cron_workflow.py
+-rw-r--r--   0        0        0     2877 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/dag.py
+-rw-r--r--   0        0        0     2241 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/data.py
+-rw-r--r--   0        0        0     4855 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/env.py
+-rw-r--r--   0        0        0     1329 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/env_from.py
+-rw-r--r--   0        0        0      208 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/exceptions.py
+-rw-r--r--   0        0        0     2346 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/http_template.py
+-rw-r--r--   0        0        0       30 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/memoize.py
+-rw-r--r--   0        0        0     4418 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/metrics.py
+-rw-r--r--   0        0        0     6913 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/__init__.py
+-rw-r--r--   0        0        0     1418 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/eventsource.py
+-rw-r--r--   0        0        0      861 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/eventsource.pyi
+-rw-r--r--   0        0        0      144 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/google/__init__.py
+-rw-r--r--   0        0        0      347 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/google/protobuf.py
+-rw-r--r--   0        0        0      164 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/google/protobuf.pyi
+-rw-r--r--   0        0        0        0 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/grpc/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/grpc/gateway/__init__.py
+-rw-r--r--   0        0        0      691 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/grpc/gateway/runtime.py
+-rw-r--r--   0        0        0      470 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/grpc/gateway/runtime.pyi
+-rw-r--r--   0        0        0        0 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/argoproj/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/argoproj/events/__init__.py
+-rw-r--r--   0        0        0   102993 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.py
+-rw-r--r--   0        0        0    25271 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi
+-rw-r--r--   0        0        0      144 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/argoproj/workflow/__init__.py
+-rw-r--r--   0        0        0   144549 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py
+-rw-r--r--   0        0        0    31958 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi
+-rw-r--r--   0        0        0        0 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/k8s/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/k8s/api/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/k8s/api/core/__init__.py
+-rw-r--r--   0        0        0   127883 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/k8s/api/core/v1.py
+-rw-r--r--   0        0        0    18004 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/k8s/api/core/v1.pyi
+-rw-r--r--   0        0        0      144 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/k8s/api/policy/__init__.py
+-rw-r--r--   0        0        0     1751 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py
+-rw-r--r--   0        0        0      376 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/k8s/api/policy/v1beta1.pyi
+-rw-r--r--   0        0        0        0 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/k8s/apimachinery/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0        0        0     3161 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py
+-rw-r--r--   0        0        0      105 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.pyi
+-rw-r--r--   0        0        0        0 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
+-rw-r--r--   0        0        0    22218 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
+-rw-r--r--   0        0        0     2064 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
+-rw-r--r--   0        0        0      144 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/__init__.py
+-rw-r--r--   0        0        0      277 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.py
+-rw-r--r--   0        0        0      108 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.pyi
+-rw-r--r--   0        0        0     1453 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/sensor.py
+-rw-r--r--   0        0        0      887 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/models/sensor.pyi
+-rw-r--r--   0        0        0      722 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/operator.py
+-rw-r--r--   0        0        0     4084 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/parameter.py
+-rw-r--r--   0        0        0     1018 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/protocol.py
+-rw-r--r--   0        0        0     3146 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/resource.py
+-rw-r--r--   0        0        0     5262 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/resources.py
+-rw-r--r--   0        0        0     1856 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/retry_strategy.py
+-rw-r--r--   0        0        0     3707 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/runner.py
+-rw-r--r--   0        0        0    14836 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/script.py
+-rw-r--r--   0        0        0    49251 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/service.py
+-rw-r--r--   0        0        0     9148 2023-05-17 14:27:07.500467 hera-5.2.0/src/hera/workflows/steps.py
+-rw-r--r--   0        0        0     3332 2023-05-17 14:27:07.504467 hera-5.2.0/src/hera/workflows/suspend.py
+-rw-r--r--   0        0        0    10501 2023-05-17 14:27:07.504467 hera-5.2.0/src/hera/workflows/task.py
+-rw-r--r--   0        0        0       27 2023-05-17 14:27:07.504467 hera-5.2.0/src/hera/workflows/toleration.py
+-rw-r--r--   0        0        0     2007 2023-05-17 14:27:07.504467 hera-5.2.0/src/hera/workflows/user_container.py
+-rw-r--r--   0        0        0     2610 2023-05-17 14:27:07.504467 hera-5.2.0/src/hera/workflows/validators.py
+-rw-r--r--   0        0        0    18656 2023-05-17 14:27:07.504467 hera-5.2.0/src/hera/workflows/volume.py
+-rw-r--r--   0        0        0    15738 2023-05-17 14:27:07.504467 hera-5.2.0/src/hera/workflows/workflow.py
+-rw-r--r--   0        0        0      911 2023-05-17 14:27:07.504467 hera-5.2.0/src/hera/workflows/workflow_status.py
+-rw-r--r--   0        0        0     5509 2023-05-17 14:27:07.504467 hera-5.2.0/src/hera/workflows/workflow_template.py
+-rw-r--r--   0        0        0    13554 1970-01-01 00:00:00.000000 hera-5.2.0/PKG-INFO
```

### Comparing `hera-5.1.7/LICENSE` & `hera-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/README.md` & `hera-5.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 [![Pypi](https://img.shields.io/pypi/v/hera.svg)](https://pypi.python.org/pypi/hera)
 [![CondaForge](https://anaconda.org/conda-forge/hera-workflows/badges/version.svg)](https://anaconda.org/conda-forge/hera-workflows)
 [![Versions](https://img.shields.io/pypi/pyversions/hera.svg)](https://github.com/argoproj-labs/hera)
 
 ### Stats after the [rename to Hera](https://github.com/argoproj-labs/hera/discussions/532)
+
 [![Downloads](https://pepy.tech/badge/hera)](https://pepy.tech/project/hera)
 [![Downloads/month](https://pepy.tech/badge/hera/month)](https://pepy.tech/project/hera)
 [![Downloads/week](https://pepy.tech/badge/hera/week)](https://pepy.tech/project/hera)
 
 ### Stats before the [rename to Hera](https://github.com/argoproj-labs/hera/discussions/532)
+
 [![Downloads](https://pepy.tech/badge/hera-workflows)](https://pepy.tech/project/hera-workflows)
 [![Downloads/month](https://pepy.tech/badge/hera-workflows/month)](https://pepy.tech/project/hera-workflows)
 [![Downloads/week](https://pepy.tech/badge/hera-workflows/week)](https://pepy.tech/project/hera-workflows)
 
 Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make the Argo
 ecosystem accessible by simplifying workflow construction and submission.
 
@@ -72,14 +74,22 @@
 | Source                                                   | Command                                                                                              |
 |----------------------------------------------------------|------------------------------------------------------------------------------------------------------|
 | [PyPi](https://pypi.org/project/hera/)                   | `pip install hera`                                                                                   |
 | [PyPi](https://pypi.org/project/hera-workflows/)         | `pip install hera-workflows`                                                                         |
 | [Conda](https://anaconda.org/conda-forge/hera-workflows) | `conda install -c conda-forge hera-workflows`                                                        |
 | [GitHub repo](https://github.com/argoproj-labs/hera)     | `python -m pip install git+https://github.com/argoproj-labs/hera --ignore-installed`/`pip install .` |
 
+## Optional dependencies
+
+### yaml
+
+- Install via `hera[yaml]`
+- [PyYAML](https://pypi.org/project/PyYAML/) is required for the `yaml` output format, which is accessible via  
+  `hera.workflows.Workflow.to_yaml(*args, **kwargs)`. This enables GitOps practices and easier debugging
+
 # Examples
 
 ### Single step script
 
 ```python
 from hera.workflows import Steps, Workflow, script
```

### Comparing `hera-5.1.7/pyproject.toml` & `hera-5.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "hera"  # project-name
 # The version is automatically substituted by the CI
-version = "5.1.7"
+version = "5.2.0"
 description = "Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make Argo Workflows more accessible by abstracting away some setup that is typically necessary for constructing Argo workflows."
 authors = ["Flaviu Vadan <flaviu.vadan@dynotx.com>", "Sambhav Kothari <sambhavs.email@gmail.com>", "Elliot Gunton <elliotgunton@gmail.com>"]
 maintainers = ["Flaviu Vadan <flaviu.vadan@dynotx.com>", "Sambhav Kothari <sambhavs.email@gmail.com>", "Elliot Gunton <elliotgunton@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/argoproj-labs/hera"
 repository = "https://github.com/argoproj-labs/hera"
```

### Comparing `hera-5.1.7/src/hera/__init__.py` & `hera-5.2.0/src/hera/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/events/models/__init__.py` & `hera-5.2.0/src/hera/events/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/events/models/eventsource.py` & `hera-5.2.0/src/hera/events/models/eventsource.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/events/models/eventsource.pyi` & `hera-5.2.0/src/hera/events/models/eventsource.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/events/models/grpc/gateway/runtime.py` & `hera-5.2.0/src/hera/events/models/grpc/gateway/runtime.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/events/models/io/argoproj/events/v1alpha1.py` & `hera-5.2.0/src/hera/events/models/io/argoproj/events/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/events/models/io/argoproj/events/v1alpha1.pyi` & `hera-5.2.0/src/hera/events/models/io/argoproj/events/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/events/models/io/argoproj/workflow/v1alpha1.py` & `hera-5.2.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi` & `hera-5.2.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/events/models/io/k8s/api/core/v1.py` & `hera-5.2.0/src/hera/events/models/io/k8s/api/core/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/events/models/io/k8s/api/core/v1.pyi` & `hera-5.2.0/src/hera/events/models/io/k8s/api/core/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/events/models/io/k8s/api/policy/v1beta1.py` & `hera-5.2.0/src/hera/events/models/io/k8s/api/policy/v1beta1.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py` & `hera-5.2.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py` & `hera-5.2.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi` & `hera-5.2.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/events/models/sensor.py` & `hera-5.2.0/src/hera/events/models/sensor.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/events/models/sensor.pyi` & `hera-5.2.0/src/hera/events/models/sensor.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/events/service.py` & `hera-5.2.0/src/hera/events/service.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/expr/_node.py` & `hera-5.2.0/src/hera/expr/_node.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/expr/_sprig.py` & `hera-5.2.0/src/hera/expr/_sprig.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/shared/_global_config.py` & `hera-5.2.0/src/hera/shared/_global_config.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/shared/serialization.py` & `hera-5.2.0/src/hera/shared/serialization.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/__init__.py` & `hera-5.2.0/src/hera/workflows/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from hera.workflows.cron_workflow import CronWorkflow
 from hera.workflows.dag import DAG
 from hera.workflows.data import Data
 from hera.workflows.env import ConfigMapEnv, Env, FieldEnv, ResourceEnv, SecretEnv
 from hera.workflows.env_from import ConfigMapEnvFrom, SecretEnvFrom
 from hera.workflows.exceptions import InvalidDispatchType, InvalidTemplateCall, InvalidType
 from hera.workflows.http_template import HTTP
+from hera.workflows.metrics import Counter, Gauge, Histogram, Label, Metric, Metrics
 from hera.workflows.operator import Operator
 from hera.workflows.parameter import Parameter
 from hera.workflows.resource import Resource
 from hera.workflows.resources import Resources
 from hera.workflows.retry_strategy import RetryPolicy, RetryStrategy
 from hera.workflows.script import InlineScriptConstructor, RunnerScriptConstructor, Script, ScriptConstructor, script
 from hera.workflows.service import WorkflowsService
@@ -91,40 +92,46 @@
     "CinderVolume",
     "ConfigMapEnv",
     "ConfigMapEnvFrom",
     "ConfigMapVolume",
     "Container",
     "ContainerNode",
     "ContainerSet",
+    "Counter",
     "CronWorkflow",
     "DAG",
     "Data",
     "DownwardAPIVolume",
     "EmptyDirVolume",
     "Env",
     "EphemeralVolume",
     "ExistingVolume",
     "FCVolume",
     "FieldEnv",
     "FlexVolume",
     "FlockerVolume",
     "GCEPersistentDiskVolume",
     "GCSArtifact",
+    "Gauge",
     "GitArtifact",
     "GitRepoVolume",
     "GlusterfsVolume",
     "HDFSArtifact",
     "HTTP",
     "HTTPArtifact",
+    "Histogram",
     "HostPathVolume",
     "ISCSIVolume",
     "InlineScriptConstructor",
     "InvalidDispatchType",
     "InvalidTemplateCall",
     "InvalidType",
+    "Label",
+    "Metric",
+    "Metrics",
     "NFSVolume",
     "NoneArchiveStrategy",
     "OSSArtifact",
     "Operator",
     "Parallel",
     "Parameter",
     "PhotonPersistentDiskVolume",
```

### Comparing `hera-5.1.7/src/hera/workflows/_context.py` & `hera-5.2.0/src/hera/workflows/_context.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/_mixins.py` & `hera-5.2.0/src/hera/workflows/_mixins.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
 import inspect
-from typing import Any, Callable, Dict, List, Optional, TypeVar, Union, cast
+from typing import Any, Callable, Dict, List, Optional, Set, TypeVar, Union, cast
 
 from pydantic import root_validator, validator
 
 from hera.shared import BaseMixin, global_config
 from hera.shared.serialization import serialize
 from hera.workflows._context import SubNodeMixin, _context
 from hera.workflows.artifact import Artifact
 from hera.workflows.env import Env, _BaseEnv
 from hera.workflows.env_from import _BaseEnvFrom
 from hera.workflows.exceptions import InvalidTemplateCall, InvalidType
+from hera.workflows.metrics import Metrics, _BaseMetric
 from hera.workflows.models import (
     HTTP,
     Affinity,
     Arguments as ModelArguments,
     Artifact as ModelArtifact,
     ArtifactLocation,
     ContainerPort,
@@ -27,21 +28,22 @@
     ImagePullPolicy,
     Inputs as ModelInputs,
     IntOrString,
     Item,
     LifecycleHook,
     Memoize,
     Metadata,
-    Metrics,
+    Metrics as ModelMetrics,
     Outputs as ModelOutputs,
     Parameter as ModelParameter,
     PersistentVolumeClaim,
     Plugin,
     PodSecurityContext,
     Probe,
+    Prometheus as ModelPrometheus,
     ResourceRequirements,
     RetryStrategy,
     Sequence,
     Synchronization,
     Template,
     TemplateRef,
     TerminationMessagePolicy,
@@ -265,45 +267,84 @@
                     if params is None
                     else params + [Parameter(name=spec.param_name, value=value)]
                 )
 
         return params
 
 
-class TemplateMixin(SubNodeMixin, HookMixin):
+class MetricsMixin(BaseMixin):
+    metrics: Optional[
+        Union[
+            _BaseMetric,
+            List[_BaseMetric],
+            Metrics,
+            ModelPrometheus,
+            List[ModelPrometheus],
+            ModelMetrics,
+        ]
+    ] = None
+
+    def _build_metrics(self) -> Optional[ModelMetrics]:
+        if self.metrics is None or isinstance(self.metrics, ModelMetrics):
+            return self.metrics
+        elif isinstance(self.metrics, ModelPrometheus):
+            return ModelMetrics(prometheus=[self.metrics])
+        elif isinstance(self.metrics, Metrics):
+            return ModelMetrics(prometheus=self.metrics._build_metrics())
+        elif isinstance(self.metrics, _BaseMetric):
+            return ModelMetrics(prometheus=[self.metrics._build_metric()])
+
+        metrics = []
+        for m in self.metrics:
+            if isinstance(m, _BaseMetric):
+                metrics.append(m._build_metric())
+            else:
+                metrics.append(m)
+        return ModelMetrics(prometheus=metrics)
+
+
+class TemplateMixin(SubNodeMixin, HookMixin, MetricsMixin):
     active_deadline_seconds: Optional[Union[int, str, IntOrString]] = None
     affinity: Optional[Affinity] = None
     archive_location: Optional[ArtifactLocation] = None
     automount_service_account_token: Optional[bool] = None
     daemon: Optional[bool] = None
     executor: Optional[ExecutorConfig] = None
     fail_fast: Optional[bool] = None
     host_aliases: Optional[List[HostAlias]] = None
     init_containers: Optional[List[Union[UserContainer, ModelUserContainer]]] = None
     memoize: Optional[Memoize] = None
     annotations: Optional[Dict[str, str]] = None
     labels: Optional[Dict[str, str]] = None
-    metrics: Optional[Metrics] = None
     name: Optional[str] = None
     node_selector: Optional[Dict[str, str]] = None
     parallelism: Optional[int] = None
     http: Optional[HTTP] = None
     plugin: Optional[Plugin] = None
     pod_spec_patch: Optional[str] = None
     priority: Optional[int] = None
     priority_class_name: Optional[str] = None
     retry_strategy: Optional[RetryStrategy] = None
     scheduler_name: Optional[str] = None
     pod_security_context: Optional[PodSecurityContext] = None
     service_account_name: Optional[str] = None
-    sidecars: Optional[List[UserContainer]] = None
+    sidecars: Optional[Union[UserContainer, List[UserContainer]]] = None
     synchronization: Optional[Synchronization] = None
     timeout: Optional[str] = None
     tolerations: Optional[List[Toleration]] = None
 
+    def _build_sidecars(self) -> Optional[List[UserContainer]]:
+        if self.sidecars is None:
+            return None
+
+        if isinstance(self.sidecars, UserContainer):
+            return [self.sidecars]
+
+        return self.sidecars
+
     def _build_active_deadline_seconds(self) -> Optional[IntOrString]:
         if self.active_deadline_seconds is None:
             return None
 
         return IntOrString(__root__=str(self.active_deadline_seconds))
 
     def _build_metadata(self) -> Optional[Metadata]:
@@ -420,61 +461,131 @@
 
 
 class CallableTemplateMixin(ArgumentsMixin):
     def __call__(self, *args, **kwargs) -> Optional[SubNodeMixin]:
         if "name" not in kwargs:
             kwargs["name"] = self.name  # type: ignore
 
+        # when the `source` is set via an `@script` decorator, it does not come in with the `kwargs` so we need to
+        # set it here in order for the following logic to capture it
+        if "source" not in kwargs and hasattr(self, "source"):
+            kwargs["source"] = self.source  # type: ignore
+
         try:
             from hera.workflows.steps import Step
 
             return Step(*args, template=self, **kwargs)
         except InvalidType:
             pass
 
         try:
             from hera.workflows.task import Task
 
-            # these are the already set parameters. If a users has already set a parameter argument, then Hera
-            # uses the user-provided value rather than the inferred value
-            arguments = self.arguments if isinstance(self.arguments, list) else [self.arguments]  # type: ignore
-            arguments = list(filter(lambda x: x is not None, arguments))
-            parameters = [arg for arg in arguments if isinstance(arg, ModelParameter) or isinstance(arg, Parameter)]
-            parameter_names = {p.name for p in parameters}
-            artifacts = [arg for arg in arguments if isinstance(arg, ModelArtifact) or isinstance(arg, Artifact)]
-            artifact_names = {a.name for a in artifacts}
+            arguments = self._get_arguments(**kwargs)
+            parameter_names = self._get_parameter_names(arguments)
+            artifact_names = self._get_artifact_names(arguments)
             if "source" in kwargs and "with_param" in kwargs:
-                # Argo uses the `inputs` field to indicate the expected parameters of a specific template whereas the
-                # `arguments` are used to indicate exactly what _values_ are assigned to the set inputs. Here,
-                # we infer the arguments when `with_param` is used. If a source is passed along with `with_param`, we
-                # infer the arguments to set from the given source. It is assumed that `with_param` will return the
-                # expected result for Argo to fan out the task on
-                new_parameters = _get_params_from_source(kwargs["source"])
-                if new_parameters is not None:
-                    for p in new_parameters:
-                        if p.name not in parameter_names and p.name not in artifact_names:
-                            arguments.append(p)
+                arguments += self._get_deduped_params_from_source(parameter_names, artifact_names, kwargs["source"])
             elif "source" in kwargs and "with_items" in kwargs:
-                # similarly to the above, we can infer the arguments to create based on the content of `with_items`.
-                # The main difference between `with_items` and `with_param` is that param is a serialized version of
-                # `with_items`. Hence, `with_items` comes in the form of a list of objects, whereas `with_param` comes
-                # in as a single serialized object. Here, we can infer the parameters to create based on the content
-                # of `with_items`
-                new_parameters = _get_params_from_items(kwargs["with_items"])
-                if new_parameters is not None:
-                    for p in new_parameters:
-                        if p.name not in parameter_names:
-                            arguments.append(p)
+                arguments += self._get_deduped_params_from_items(parameter_names, kwargs["with_items"])
+
+            # it is possible for the user to pass `arguments` via `kwargs` along with `with_param`. The `with_param`
+            # additional parameters are inferred and have to be added to the `kwargs['arguments']` for otherwise
+            # the task will miss adding them when building the final arguments
+            kwargs["arguments"] = arguments
 
             return Task(*args, template=self, **kwargs)
         except InvalidType:
             pass
 
         raise InvalidTemplateCall("Container is not under a Steps, Parallel, or DAG context")
 
+    def _get_arguments(self, **kwargs) -> List:
+        """Returns a list of arguments from the kwargs given to the template call"""
+
+        # these are the already set parameters. If a user has already set a parameter argument, then Hera
+        # uses the user-provided value rather than the inferred value
+        kwargs_arguments = kwargs.get("arguments", [])
+        kwargs_arguments = (
+            kwargs_arguments if isinstance(kwargs_arguments, List) else [kwargs_arguments]
+        )  # type: ignore
+        arguments = (
+            self.arguments if isinstance(self.arguments, List) else [self.arguments] + kwargs_arguments
+        )  # type: ignore
+        return list(filter(lambda x: x is not None, arguments))
+
+    def _get_parameter_names(self, arguments: List) -> Set[str]:
+        parameters = [arg for arg in arguments if isinstance(arg, ModelParameter) or isinstance(arg, Parameter)]
+        return {p.name for p in parameters}
+
+    def _get_artifact_names(self, arguments: List) -> Set[str]:
+        artifacts = [arg for arg in arguments if isinstance(arg, ModelArtifact) or isinstance(arg, Artifact)]
+        return {a.name for a in artifacts}
+
+    def _get_deduped_params_from_source(
+        self, parameter_names: Set[str], artifact_names: Set[str], source: Callable
+    ) -> List[Parameter]:
+        """Infer arguments from the given source and deduplicates based on the given params and artifacts.
+
+        Argo uses the `inputs` field to indicate the expected parameters of a specific template whereas the
+        `arguments` are used to indicate exactly what _values_ are assigned to the set inputs. Here,
+        we infer the arguments when `with_param` is used. If a source is passed along with `with_param`, we
+        infer the arguments to set from the given source. It is assumed that `with_param` will return the
+        expected result for Argo to fan out the task on.
+
+        Parameters
+        ----------
+        parameter_names: Set[str]
+            Set of already constructed parameter names.
+        artifact_names: Set[str]
+            Set of already constructed artifact names.
+        source: Callable
+            The source function to infer the arguments from.
+
+        Returns
+        -------
+        List[Parameter]
+            The list of inferred arguments to set.
+        """
+        new_arguments = []
+        new_parameters = _get_params_from_source(source)
+        if new_parameters is not None:
+            for p in new_parameters:
+                if p.name not in parameter_names and p.name not in artifact_names:
+                    new_arguments.append(p)
+        return new_arguments
+
+    def _get_deduped_params_from_items(self, parameter_names: Set[str], items: List[Any]) -> List[Parameter]:
+        """Infer arguments from the given items.
+
+        The main difference between `with_items` and `with_param` is that param is a serialized version of
+        `with_items`. Hence, `with_items` comes in the form of a list of objects, whereas `with_param` comes
+        in as a single serialized object. Here, we can infer the parameters to create based on the content
+        of `with_items`.
+
+        Parameters
+        ----------
+        parameter_names: Set[str]
+            Set of already constructed parameter names.
+        items: List[Any]
+            The items to infer the arguments from.
+
+        Returns
+        -------
+        List[Parameter]
+            The list of inferred arguments to set.
+        """
+        item_params = _get_params_from_items(items)
+        new_params = []
+        if item_params is not None:
+            for p in item_params:
+                if p.name not in parameter_names:
+                    new_params.append(p)
+        return new_params
+
 
 class ParameterMixin(BaseMixin):
     with_param: Optional[Any] = None  # this must be a serializable object, or `hera.workflows.parameter.Parameter`
 
     def _build_with_param(self) -> Optional[str]:
         if self.with_param is None:
             return None
```

### Comparing `hera-5.1.7/src/hera/workflows/_unparse.py` & `hera-5.2.0/src/hera/workflows/_unparse.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/archive.py` & `hera-5.2.0/src/hera/workflows/archive.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/artifact.py` & `hera-5.2.0/src/hera/workflows/artifact.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/container.py` & `hera-5.2.0/src/hera/workflows/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,27 +75,27 @@
             executor=self.executor,
             fail_fast=self.fail_fast,
             host_aliases=self.host_aliases,
             init_containers=self.init_containers,
             inputs=self._build_inputs(),
             memoize=self.memoize,
             metadata=self._build_metadata(),
-            metrics=self.metrics,
+            metrics=self._build_metrics(),
             name=self.name,
             node_selector=self.node_selector,
             outputs=self._build_outputs(),
             plugin=self.plugin,
             pod_spec_patch=self.pod_spec_patch,
             priority=self.priority,
             priority_class_name=self.priority_class_name,
             retry_strategy=self.retry_strategy,
             scheduler_name=self.scheduler_name,
             security_context=self.pod_security_context,
             service_account_name=self.service_account_name,
-            sidecars=self.sidecars,
+            sidecars=self._build_sidecars(),
             synchronization=self.synchronization,
             timeout=self.timeout,
             tolerations=self.tolerations,
             volumes=self._build_volumes(),
         )
```

### Comparing `hera-5.1.7/src/hera/workflows/container_set.py` & `hera-5.2.0/src/hera/workflows/container_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from typing import Any, List, Optional, Union
 
 from hera.workflows._mixins import (
+    CallableTemplateMixin,
     ContainerMixin,
     ContextMixin,
     EnvIOMixin,
     ResourceMixin,
     SubNodeMixin,
     TemplateMixin,
     VolumeMountMixin,
@@ -51,14 +52,15 @@
         raise ValueError(f"Unknown type {type(other)} provided to `__rshift__`")
 
 
 class ContainerSet(
     EnvIOMixin,
     ContainerMixin,
     TemplateMixin,
+    CallableTemplateMixin,
     ResourceMixin,
     VolumeMountMixin,
     ContextMixin,
 ):
     containers: List[ContainerNode] = []
     container_set_retry_strategy: Optional[ContainerSetRetryStrategy] = None
 
@@ -86,28 +88,28 @@
             executor=self.executor,
             fail_fast=self.fail_fast,
             host_aliases=self.host_aliases,
             init_containers=self.init_containers,
             inputs=self._build_inputs(),
             memoize=self.memoize,
             metadata=self._build_metadata(),
-            metrics=self.metrics,
+            metrics=self._build_metrics(),
             name=self.name,
             node_selector=self.node_selector,
             outputs=self._build_outputs(),
             plugin=self.plugin,
             pod_spec_patch=self.pod_spec_patch,
             priority=self.priority,
             priority_class_name=self.priority_class_name,
             resource=self._build_resources(),
             retry_strategy=self.retry_strategy,
             scheduler_name=self.scheduler_name,
             security_context=self.pod_security_context,
             service_account_name=self.service_account_name,
-            sidecars=self.sidecars,
+            sidecars=self._build_sidecars(),
             synchronization=self.synchronization,
             timeout=self.timeout,
             tolerations=self.tolerations,
             volumes=self._build_volumes(),
         )
```

### Comparing `hera-5.1.7/src/hera/workflows/cron_workflow.py` & `hera-5.2.0/src/hera/workflows/cron_workflow.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/dag.py` & `hera-5.2.0/src/hera/workflows/dag.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 See https://argoproj.github.io/argo-workflows/walk-through/dag/
 for more on DAGs (Directed Acyclic Graphs).
 """
 from __future__ import annotations
 
 from typing import Any, List, Optional, Union
 
-from hera.workflows._mixins import ContextMixin, IOMixin, TemplateMixin
+from hera.workflows._mixins import CallableTemplateMixin, ContextMixin, IOMixin, TemplateMixin
 from hera.workflows.exceptions import InvalidType
 from hera.workflows.models import (
     DAGTask,
     DAGTemplate as _ModelDAGTemplate,
     Template as _ModelTemplate,
 )
 from hera.workflows.task import Task
 
 
-class DAG(IOMixin, TemplateMixin, ContextMixin):
+class DAG(IOMixin, TemplateMixin, CallableTemplateMixin, ContextMixin):
     """A DAG template invocator is used to define Task dependencies as an acyclic graph.
 
     DAG implements the contextmanager interface so allows usage of `with`, under which any
     `hera.workflows.task.Task` objects instantiated will be added to the DAG's list of Tasks.
     """
 
     fail_fast: Optional[bool] = None
@@ -50,27 +50,28 @@
             executor=self.executor,
             fail_fast=self.fail_fast,
             host_aliases=self.host_aliases,
             init_containers=self.init_containers,
             inputs=self._build_inputs(),
             memoize=self.memoize,
             metadata=self._build_metadata(),
-            metrics=self.metrics,
+            metrics=self._build_metrics(),
             name=self.name,
             node_selector=self.node_selector,
             outputs=self._build_outputs(),
+            parallelism=self.parallelism,
             plugin=self.plugin,
             pod_spec_patch=self.pod_spec_patch,
             priority=self.priority,
             priority_class_name=self.priority_class_name,
             retry_strategy=self.retry_strategy,
             scheduler_name=self.scheduler_name,
             security_context=self.pod_security_context,
             service_account_name=self.service_account_name,
-            sidecars=self.sidecars,
+            sidecars=self._build_sidecars(),
             synchronization=self.synchronization,
             timeout=self.timeout,
             tolerations=self.tolerations,
         )
 
 
 __all__ = ["DAG"]
```

### Comparing `hera-5.1.7/src/hera/workflows/data.py` & `hera-5.2.0/src/hera/workflows/data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import List, Union
 
 from hera.expr._node import Node
 from hera.workflows import models as m
-from hera.workflows._mixins import IOMixin, TemplateMixin
+from hera.workflows._mixins import CallableTemplateMixin, IOMixin, TemplateMixin
 from hera.workflows.artifact import Artifact
 
 
-class Data(TemplateMixin, IOMixin):
+class Data(TemplateMixin, IOMixin, CallableTemplateMixin):
     source: Union[m.DataSource, m.ArtifactPaths, Artifact]
     transformations: List[Union[str, Node]] = []
 
     def _build_source(self) -> m.DataSource:
         if isinstance(self.source, m.DataSource):
             return self.source
         elif isinstance(self.source, m.ArtifactPaths):
@@ -43,15 +43,15 @@
             plugin=self.plugin,
             priority=self.priority,
             priority_class_name=self.priority_class_name,
             retry_strategy=self.retry_strategy,
             scheduler_name=self.scheduler_name,
             security_context=self.pod_security_context,
             service_account_name=self.service_account_name,
-            sidecars=self.sidecars,
+            sidecars=self._build_sidecars(),
             synchronization=self.synchronization,
             timeout=self.timeout,
             tolerations=self.tolerations,
         )
 
 
 __all__ = ["Data"]
```

### Comparing `hera-5.1.7/src/hera/workflows/env.py` & `hera-5.2.0/src/hera/workflows/env.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/env_from.py` & `hera-5.2.0/src/hera/workflows/env_from.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/http_template.py` & `hera-5.2.0/src/hera/workflows/http_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import List, Optional
 
-from hera.workflows._mixins import IOMixin, TemplateMixin
+from hera.workflows._mixins import CallableTemplateMixin, IOMixin, TemplateMixin
 from hera.workflows.models import (
     HTTP as _ModelHTTP,
     HTTPBodySource,
     Template as _ModelTemplate,
     V1HTTPHeader as HTTPHeader,
 )
 
 
-class HTTP(TemplateMixin, IOMixin):
+class HTTP(TemplateMixin, IOMixin, CallableTemplateMixin):
     url: str
     body: Optional[str] = None
     body_from: Optional[HTTPBodySource] = None
     headers: Optional[List[HTTPHeader]] = None
     insecure_skip_verify: Optional[bool] = None
     method: Optional[str] = None
     success_condition: Optional[str] = None
@@ -51,15 +51,15 @@
             plugin=self.plugin,
             priority=self.priority,
             priority_class_name=self.priority_class_name,
             retry_strategy=self.retry_strategy,
             scheduler_name=self.scheduler_name,
             security_context=self.pod_security_context,
             service_account_name=self.service_account_name,
-            sidecars=self.sidecars,
+            sidecars=self._build_sidecars(),
             synchronization=self.synchronization,
             timeout=self.timeout,
             tolerations=self.tolerations,
         )
 
 
 __all__ = ["HTTP"]
```

### Comparing `hera-5.1.7/src/hera/workflows/models/__init__.py` & `hera-5.2.0/src/hera/workflows/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/models/eventsource.py` & `hera-5.2.0/src/hera/workflows/models/eventsource.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/models/eventsource.pyi` & `hera-5.2.0/src/hera/workflows/models/eventsource.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/models/grpc/gateway/runtime.py` & `hera-5.2.0/src/hera/workflows/models/grpc/gateway/runtime.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/models/io/argoproj/events/v1alpha1.py` & `hera-5.2.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi` & `hera-5.2.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py` & `hera-5.2.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi` & `hera-5.2.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/models/io/k8s/api/core/v1.py` & `hera-5.2.0/src/hera/workflows/models/io/k8s/api/core/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/models/io/k8s/api/core/v1.pyi` & `hera-5.2.0/src/hera/workflows/models/io/k8s/api/core/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py` & `hera-5.2.0/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py` & `hera-5.2.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py` & `hera-5.2.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi` & `hera-5.2.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/models/sensor.py` & `hera-5.2.0/src/hera/workflows/models/sensor.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/models/sensor.pyi` & `hera-5.2.0/src/hera/workflows/models/sensor.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/operator.py` & `hera-5.2.0/src/hera/workflows/operator.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/parameter.py` & `hera-5.2.0/src/hera/workflows/parameter.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/protocol.py` & `hera-5.2.0/src/hera/workflows/protocol.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/resource.py` & `hera-5.2.0/src/hera/workflows/resource.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,42 @@
-from typing import List, Optional
+from typing import List, Optional, Union
 
-from hera.workflows._mixins import IOMixin, SubNodeMixin, TemplateMixin
+from hera.workflows._mixins import CallableTemplateMixin, IOMixin, SubNodeMixin, TemplateMixin
+from hera.workflows.cron_workflow import CronWorkflow
 from hera.workflows.models import (
     ManifestFrom,
     ResourceTemplate as _ModelResourceTemplate,
     Template as _ModelTemplate,
 )
+from hera.workflows.workflow import Workflow
+from hera.workflows.workflow_template import WorkflowTemplate
 
 
-class Resource(TemplateMixin, SubNodeMixin, IOMixin):
+class Resource(CallableTemplateMixin, TemplateMixin, SubNodeMixin, IOMixin):
     action: str
     failure_condition: Optional[str] = None
     flags: Optional[List[str]] = None
-    manifest: Optional[str] = None
+    manifest: Optional[Union[str, Workflow, CronWorkflow, WorkflowTemplate]] = None
     manifest_from: Optional[ManifestFrom] = None
     merge_strategy: Optional[str] = None
     set_owner_reference: Optional[bool] = None
     success_condition: Optional[str] = None
 
+    def _build_manifest(self) -> Optional[str]:
+        if isinstance(self.manifest, (Workflow, CronWorkflow, WorkflowTemplate)):
+            # hack to appease raw yaml string comparison
+            return self.manifest.to_yaml().replace("'{{", "{{").replace("}}'", "}}")
+        return self.manifest
+
     def _build_resource_template(self) -> _ModelResourceTemplate:
         return _ModelResourceTemplate(
             action=self.action,
             failure_condition=self.failure_condition,
             flags=self.flags,
-            manifest=self.manifest,
+            manifest=self._build_manifest(),
             manifest_from=self.manifest_from,
             merge_strategy=self.merge_strategy,
             set_owner_reference=self.set_owner_reference,
             success_condition=self.success_condition,
         )
 
     def _build_template(self) -> _ModelTemplate:
@@ -40,29 +49,29 @@
             executor=self.executor,
             fail_fast=self.fail_fast,
             host_aliases=self.host_aliases,
             init_containers=self.init_containers,
             inputs=self._build_inputs(),
             memoize=self.memoize,
             metadata=self._build_metadata(),
-            metrics=self.metrics,
+            metrics=self._build_metrics(),
             name=self.name,
             node_selector=self.node_selector,
             outputs=self._build_outputs(),
             parallelism=self.parallelism,
             plugin=self.plugin,
             pod_spec_patch=self.pod_spec_patch,
             priority=self.priority,
             priority_class_name=self.priority_class_name,
             resource=self._build_resource_template(),
             retry_strategy=self.retry_strategy,
             scheduler_name=self.scheduler_name,
             security_context=self.pod_security_context,
             service_account_name=self.service_account_name,
-            sidecars=self.sidecars,
+            sidecars=self._build_sidecars(),
             synchronization=self.synchronization,
             timeout=self.timeout,
             tolerations=self.tolerations,
         )
 
 
 __all__ = ["Resource"]
```

### Comparing `hera-5.1.7/src/hera/workflows/resources.py` & `hera-5.2.0/src/hera/workflows/resources.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/retry_strategy.py` & `hera-5.2.0/src/hera/workflows/retry_strategy.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/runner.py` & `hera-5.2.0/src/hera/workflows/runner.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/script.py` & `hera-5.2.0/src/hera/workflows/script.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,29 +155,29 @@
                 executor=self.executor,
                 fail_fast=self.fail_fast,
                 host_aliases=self.host_aliases,
                 init_containers=self.init_containers,
                 inputs=self._build_inputs(),
                 memoize=self.memoize,
                 metadata=self._build_metadata(),
-                metrics=self.metrics,
+                metrics=self._build_metrics(),
                 name=self.name,
                 node_selector=self.node_selector,
                 outputs=self._build_outputs(),
                 parallelism=self.parallelism,
                 plugin=self.plugin,
                 pod_spec_patch=self.pod_spec_patch,
                 priority=self.priority,
                 priority_class_name=self.priority_class_name,
                 retry_strategy=self.retry_strategy,
                 scheduler_name=self.scheduler_name,
                 script=self._build_script(),
                 security_context=self.pod_security_context,
                 service_account_name=self.service_account_name,
-                sidecars=self.sidecars,
+                sidecars=self._build_sidecars(),
                 synchronization=self.synchronization,
                 timeout=self.timeout,
                 tolerations=self.tolerations,
                 volumes=self._build_volumes(),
             ),
         )
```

### Comparing `hera-5.1.7/src/hera/workflows/service.py` & `hera-5.2.0/src/hera/workflows/service.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/steps.py` & `hera-5.2.0/src/hera/workflows/steps.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,21 +94,17 @@
             raise ValueError(f"Cannot get output parameters when the template has no outputs: {template}")
         if template.outputs.parameters is None:  # type: ignore
             raise ValueError(f"Cannot get output parameters when the template has no output parameters: {template}")
         parameters = template.outputs.parameters  # type: ignore
 
         obj = next((output for output in parameters if output.name == name), None)
         if obj is not None:
-            obj.value = f"{{{{steps.{self.name}.outputs.parameters.{name}}}}}"
             return Parameter(
                 name=obj.name,
-                value=obj.value,
-                value_from=obj.value_from,
-                global_name=obj.global_name,
-                description=obj.description,
+                value=f"{{{{steps.{self.name}.outputs.parameters.{name}}}}}",
             )
         raise KeyError(f"No output parameter named `{name}` found")
 
     def _build_as_workflow_step(self) -> _ModelWorkflowStep:
         _template = None
         if isinstance(self.template, str):
             _template = self.template
@@ -244,30 +240,30 @@
             fail_fast=self.fail_fast,
             http=None,
             host_aliases=self.host_aliases,
             init_containers=self.init_containers,
             inputs=self._build_inputs(),
             memoize=self.memoize,
             metadata=self._build_metadata(),
-            metrics=self.metrics,
+            metrics=self._build_metrics(),
             name=self.name,
             node_selector=self.node_selector,
             outputs=self._build_outputs(),
             parallelism=self.parallelism,
             plugin=self.plugin,
             pod_spec_patch=self.pod_spec_patch,
             priority=self.priority,
             priority_class_name=self.priority_class_name,
             resource=None,
             retry_strategy=self.retry_strategy,
             scheduler_name=self.scheduler_name,
             script=None,
             security_context=self.pod_security_context,
             service_account_name=self.service_account_name,
-            sidecars=self.sidecars,
+            sidecars=self._build_sidecars(),
             steps=self._build_steps(),
             suspend=None,
             synchronization=self.synchronization,
             timeout=self.timeout,
             tolerations=self.tolerations,
         )
```

### Comparing `hera-5.1.7/src/hera/workflows/suspend.py` & `hera-5.2.0/src/hera/workflows/suspend.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             plugin=self.plugin,
             priority_class_name=self.priority_class_name,
             priority=self.priority,
             retry_strategy=self.retry_strategy,
             scheduler_name=self.scheduler_name,
             security_context=self.pod_security_context,
             service_account_name=self.service_account_name,
-            sidecars=self.sidecars,
+            sidecars=self._build_sidecars(),
             suspend=self._build_suspend_template(),
             synchronization=self.synchronization,
             timeout=self.timeout,
             tolerations=self.tolerations,
         )
```

### Comparing `hera-5.1.7/src/hera/workflows/task.py` & `hera-5.2.0/src/hera/workflows/task.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/user_container.py` & `hera-5.2.0/src/hera/workflows/user_container.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/validators.py` & `hera-5.2.0/src/hera/workflows/validators.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/volume.py` & `hera-5.2.0/src/hera/workflows/volume.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/workflow.py` & `hera-5.2.0/src/hera/workflows/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,26 @@
 from types import ModuleType
 from typing import Any, Dict, List, Optional, Union
 
 from pydantic import validator
 from typing_extensions import get_args
 
 from hera.shared import global_config
-from hera.workflows._mixins import ArgumentsMixin, ContextMixin, HookMixin, VolumeMixin
+from hera.workflows._mixins import ArgumentsMixin, ContextMixin, HookMixin, MetricsMixin, VolumeMixin
 from hera.workflows.exceptions import InvalidType
 from hera.workflows.models import (
     Affinity,
     ArtifactGC,
     ArtifactRepositoryRef,
     ExecutorConfig,
     HostAlias,
     LifecycleHook,
     LocalObjectReference,
     ManagedFieldsEntry,
     Metadata,
-    Metrics,
     ObjectMeta,
     OwnerReference,
     PersistentVolumeClaim,
     PodDisruptionBudgetSpec,
     PodDNSConfig,
     PodGC,
     PodSecurityContext,
@@ -63,14 +62,15 @@
 
 
 class Workflow(
     ArgumentsMixin,
     ContextMixin,
     HookMixin,
     VolumeMixin,
+    MetricsMixin,
 ):
     """The base Workflow class for Hera.
 
     Workflow implements the contextmanager interface so allows usage of `with`, under which
     any `hera.workflows.protocol.Templatable` object instantiated under the context will be
     added to the Workflow's list of templates.
 
@@ -113,15 +113,14 @@
     dns_policy: Optional[str] = None
     entrypoint: Optional[str] = None
     executor: Optional[ExecutorConfig] = None
     hooks: Optional[Dict[str, LifecycleHook]] = None
     host_aliases: Optional[List[HostAlias]] = None
     host_network: Optional[bool] = None
     image_pull_secrets: ImagePullSecrets = None
-    metrics: Optional[Metrics] = None
     node_selector: Optional[Dict[str, str]] = None
     on_exit: Optional[str] = None
     parallelism: Optional[int] = None
     pod_disruption_budget: Optional[PodDisruptionBudgetSpec] = None
     pod_gc: Optional[PodGC] = None
     pod_metadata: Optional[Metadata] = None
     pod_priority: Optional[int] = None
@@ -195,18 +194,16 @@
         for secret in v:
             if isinstance(secret, str):
                 result.append(LocalObjectReference(name=secret))
             elif isinstance(secret, LocalObjectReference):
                 result.append(secret)
         return result
 
-    def build(self) -> TWorkflow:
-        """Builds the Workflow and its components into an Argo schema Workflow object."""
-        self = self._dispatch_hooks()
-
+    def _build_templates(self) -> List[TTemplate]:
+        """Builds the templates into an Argo schema."""
         templates = []
         for template in self.templates:
             if isinstance(template, HookMixin):
                 template = template._dispatch_hooks()
 
             if isinstance(template, Templatable):
                 templates.append(template._build_template())
@@ -239,15 +236,21 @@
                         assert claim.metadata is not None, "expected a volume claim with metadata"
                         assert claim.metadata.name is not None, "expected a named volume claim"
                         new_volume_claims_map[claim.metadata.name] = claim
 
                     for claim_name, claim in new_volume_claims_map.items():
                         if claim_name not in current_volume_claims_map:
                             self.volume_claim_templates.append(claim)
+        return templates
+
+    def build(self) -> TWorkflow:
+        """Builds the Workflow and its components into an Argo schema Workflow object."""
+        self = self._dispatch_hooks()
 
+        templates = self._build_templates()
         workflow_claims = self._build_persistent_volume_claims()
         volume_claim_templates = (self.volume_claim_templates or []) + (workflow_claims or [])
         return _ModelWorkflow(
             api_version=self.api_version,
             kind=self.kind,
             metadata=ObjectMeta(
                 annotations=self.annotations,
@@ -279,15 +282,15 @@
                 dns_policy=self.dns_policy,
                 entrypoint=self.entrypoint,
                 executor=self.executor,
                 hooks=self.hooks,
                 host_aliases=self.host_aliases,
                 host_network=self.host_network,
                 image_pull_secrets=self.image_pull_secrets,
-                metrics=self.metrics,
+                metrics=self._build_metrics(),
                 node_selector=self.node_selector,
                 on_exit=self.on_exit,
                 parallelism=self.parallelism,
                 pod_disruption_budget=self.pod_disruption_budget,
                 pod_gc=self.pod_gc,
                 pod_metadata=self.pod_metadata,
                 pod_priority=self.pod_priority,
```

### Comparing `hera-5.1.7/src/hera/workflows/workflow_status.py` & `hera-5.2.0/src/hera/workflows/workflow_status.py`

 * *Files identical despite different names*

### Comparing `hera-5.1.7/src/hera/workflows/workflow_template.py` & `hera-5.2.0/src/hera/workflows/workflow_template.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 """The workflow_template module provides the WorkflowTemplate class
 
 See https://argoproj.github.io/argo-workflows/workflow-templates/
 for more on WorkflowTemplates.
 """
 from pydantic import validator
-from typing_extensions import get_args
 
-from hera.workflows._mixins import HookMixin
-from hera.workflows.exceptions import InvalidType
 from hera.workflows.models import (
     ObjectMeta,
     WorkflowSpec as _ModelWorkflowSpec,
     WorkflowTemplate as _ModelWorkflowTemplate,
     WorkflowTemplateCreateRequest,
     WorkflowTemplateLintRequest,
 )
-from hera.workflows.protocol import Templatable, TTemplate, TWorkflow
+from hera.workflows.protocol import TWorkflow
 from hera.workflows.workflow import Workflow
 
 
 class WorkflowTemplate(Workflow):
     """WorkflowTemplates are definitions of Workflows that live in your cluster. This allows you
     to create a library of frequently-used templates and reuse them by referencing them from your
     Workflows.
@@ -48,26 +45,17 @@
             WorkflowTemplateLintRequest(template=self.build()), namespace=self.namespace
         )
 
     def build(self) -> TWorkflow:
         """Builds the WorkflowTemplate and its components into an Argo schema WorkflowTemplate object."""
         self = self._dispatch_hooks()
 
-        templates = []
-        for template in self.templates:
-            if isinstance(template, HookMixin):
-                template = template._dispatch_hooks()
-
-            if isinstance(template, Templatable):
-                templates.append(template._build_template())
-            elif isinstance(template, get_args(TTemplate)):
-                templates.append(template)
-            else:
-                raise InvalidType(f"{type(template)} is not a valid template type")
-
+        templates = self._build_templates()
+        workflow_claims = self._build_persistent_volume_claims()
+        volume_claim_templates = (self.volume_claim_templates or []) + (workflow_claims or [])
         return _ModelWorkflowTemplate(
             api_version=self.api_version,
             kind=self.kind,
             metadata=ObjectMeta(
                 annotations=self.annotations,
                 cluster_name=self.cluster_name,
                 creation_timestamp=self.creation_timestamp,
@@ -97,15 +85,15 @@
                 dns_policy=self.dns_policy,
                 entrypoint=self.entrypoint,
                 executor=self.executor,
                 hooks=self.hooks,
                 host_aliases=self.host_aliases,
                 host_network=self.host_network,
                 image_pull_secrets=self.image_pull_secrets,
-                metrics=self.metrics,
+                metrics=self._build_metrics(),
                 node_selector=self.node_selector,
                 on_exit=self.on_exit,
                 parallelism=self.parallelism,
                 pod_disruption_budget=self.pod_disruption_budget,
                 pod_gc=self.pod_gc,
                 pod_metadata=self.pod_metadata,
                 pod_priority=self.pod_priority,
@@ -120,16 +108,16 @@
                 suspend=self.suspend,
                 synchronization=self.synchronization,
                 template_defaults=self.template_defaults,
                 templates=templates or None,
                 tolerations=self.tolerations,
                 ttl_strategy=self.ttl_strategy,
                 volume_claim_gc=self.volume_claim_gc,
-                volume_claim_templates=self.volume_claim_templates,
-                volumes=self.volumes,
+                volume_claim_templates=volume_claim_templates or None,
+                volumes=self._build_volumes(),
                 workflow_metadata=self.workflow_metadata,
                 workflow_template_ref=self.workflow_template_ref,
             ),
         )
 
 
 __all__ = ["WorkflowTemplate"]
```

### Comparing `hera-5.1.7/PKG-INFO` & `hera-5.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hera
-Version: 5.1.7
+Version: 5.2.0
 Summary: Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make Argo Workflows more accessible by abstracting away some setup that is typically necessary for constructing Argo workflows.
 Home-page: https://github.com/argoproj-labs/hera
 License: MIT
 Author: Flaviu Vadan
 Author-email: flaviu.vadan@dynotx.com
 Maintainer: Flaviu Vadan
 Maintainer-email: flaviu.vadan@dynotx.com
@@ -47,19 +47,21 @@
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 [![Pypi](https://img.shields.io/pypi/v/hera.svg)](https://pypi.python.org/pypi/hera)
 [![CondaForge](https://anaconda.org/conda-forge/hera-workflows/badges/version.svg)](https://anaconda.org/conda-forge/hera-workflows)
 [![Versions](https://img.shields.io/pypi/pyversions/hera.svg)](https://github.com/argoproj-labs/hera)
 
 ### Stats after the [rename to Hera](https://github.com/argoproj-labs/hera/discussions/532)
+
 [![Downloads](https://pepy.tech/badge/hera)](https://pepy.tech/project/hera)
 [![Downloads/month](https://pepy.tech/badge/hera/month)](https://pepy.tech/project/hera)
 [![Downloads/week](https://pepy.tech/badge/hera/week)](https://pepy.tech/project/hera)
 
 ### Stats before the [rename to Hera](https://github.com/argoproj-labs/hera/discussions/532)
+
 [![Downloads](https://pepy.tech/badge/hera-workflows)](https://pepy.tech/project/hera-workflows)
 [![Downloads/month](https://pepy.tech/badge/hera-workflows/month)](https://pepy.tech/project/hera-workflows)
 [![Downloads/week](https://pepy.tech/badge/hera-workflows/week)](https://pepy.tech/project/hera-workflows)
 
 Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make the Argo
 ecosystem accessible by simplifying workflow construction and submission.
 
@@ -106,14 +108,22 @@
 | Source                                                   | Command                                                                                              |
 |----------------------------------------------------------|------------------------------------------------------------------------------------------------------|
 | [PyPi](https://pypi.org/project/hera/)                   | `pip install hera`                                                                                   |
 | [PyPi](https://pypi.org/project/hera-workflows/)         | `pip install hera-workflows`                                                                         |
 | [Conda](https://anaconda.org/conda-forge/hera-workflows) | `conda install -c conda-forge hera-workflows`                                                        |
 | [GitHub repo](https://github.com/argoproj-labs/hera)     | `python -m pip install git+https://github.com/argoproj-labs/hera --ignore-installed`/`pip install .` |
 
+## Optional dependencies
+
+### yaml
+
+- Install via `hera[yaml]`
+- [PyYAML](https://pypi.org/project/PyYAML/) is required for the `yaml` output format, which is accessible via  
+  `hera.workflows.Workflow.to_yaml(*args, **kwargs)`. This enables GitOps practices and easier debugging
+
 # Examples
 
 ### Single step script
 
 ```python
 from hera.workflows import Steps, Workflow, script
```

