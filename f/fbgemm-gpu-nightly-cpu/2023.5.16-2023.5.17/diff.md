# Comparing `tmp/fbgemm_gpu_nightly_cpu-2023.5.16-cp39-cp39-manylinux1_x86_64.whl.zip` & `tmp/fbgemm_gpu_nightly_cpu-2023.5.17-cp39-cp39-manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,39 +1,39 @@
-Zip file size: 3812212 bytes, number of entries: 37
--rw-r--r--  2.0 unx      567 b- defN 23-May-16 13:02 fbgemm_gpu/__init__.py
--rw-r--r--  2.0 unx    14800 b- defN 23-May-16 13:02 fbgemm_gpu/_fbgemm_gpu_docs.py
--rw-r--r--  2.0 unx     2747 b- defN 23-May-16 13:02 fbgemm_gpu/batched_unary_embeddings_ops.py
--rw-r--r--  2.0 unx      818 b- defN 23-May-16 13:02 fbgemm_gpu/enums.py
--rwxr-xr-x  2.0 unx 13704384 b- defN 23-May-16 13:02 fbgemm_gpu/fbgemm_gpu_py.so
--rw-r--r--  2.0 unx     5648 b- defN 23-May-16 13:02 fbgemm_gpu/metrics.py
--rw-r--r--  2.0 unx     2339 b- defN 23-May-16 13:02 fbgemm_gpu/permute_pooled_embedding_modules.py
--rw-r--r--  2.0 unx     2477 b- defN 23-May-16 13:02 fbgemm_gpu/permute_pooled_embedding_modules_split.py
--rw-r--r--  2.0 unx     7682 b- defN 23-May-16 13:02 fbgemm_gpu/quantize_comm.py
--rw-r--r--  2.0 unx     4005 b- defN 23-May-16 13:02 fbgemm_gpu/quantize_utils.py
--rw-r--r--  2.0 unx     5727 b- defN 23-May-16 13:02 fbgemm_gpu/split_embedding_configs.py
--rw-r--r--  2.0 unx     8738 b- defN 23-May-16 13:02 fbgemm_gpu/split_embedding_inference_converter.py
--rw-r--r--  2.0 unx    20503 b- defN 23-May-16 13:02 fbgemm_gpu/split_embedding_utils.py
--rw-r--r--  2.0 unx   133833 b- defN 23-May-16 13:02 fbgemm_gpu/split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx    39018 b- defN 23-May-16 13:02 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx      910 b- defN 23-May-16 13:02 fbgemm_gpu/uvm.py
--rw-r--r--  2.0 unx     1912 b- defN 23-May-16 13:00 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
--rw-r--r--  2.0 unx     4163 b- defN 23-May-16 13:00 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
--rw-r--r--  2.0 unx     4932 b- defN 23-May-16 13:00 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
--rw-r--r--  2.0 unx     4465 b- defN 23-May-16 13:00 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad.py
--rw-r--r--  2.0 unx     6474 b- defN 23-May-16 13:00 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     4501 b- defN 23-May-16 13:00 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_weight_decay.py
--rw-r--r--  2.0 unx     3710 b- defN 23-May-16 13:00 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_sgd.py
--rw-r--r--  2.0 unx     1533 b- defN 23-May-16 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
--rw-r--r--  2.0 unx     4932 b- defN 23-May-16 13:00 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
--rw-r--r--  2.0 unx     4401 b- defN 23-May-16 13:00 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
--rw-r--r--  2.0 unx     4964 b- defN 23-May-16 13:00 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
--rw-r--r--  2.0 unx     4964 b- defN 23-May-16 13:00 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
--rw-r--r--  2.0 unx     4451 b- defN 23-May-16 13:00 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
--rw-r--r--  2.0 unx     6460 b- defN 23-May-16 13:00 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     4487 b- defN 23-May-16 13:00 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py
--rw-r--r--  2.0 unx     4407 b- defN 23-May-16 13:00 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
--rw-r--r--  2.0 unx     3696 b- defN 23-May-16 13:00 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
--rw-r--r--  2.0 unx     2934 b- defN 23-May-16 13:02 fbgemm_gpu_nightly_cpu-2023.5.16.dist-info/METADATA
--rw-r--r--  2.0 unx      102 b- defN 23-May-16 13:02 fbgemm_gpu_nightly_cpu-2023.5.16.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-16 13:02 fbgemm_gpu_nightly_cpu-2023.5.16.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4129 b- defN 23-May-16 13:02 fbgemm_gpu_nightly_cpu-2023.5.16.dist-info/RECORD
-37 files, 14035824 bytes uncompressed, 3805236 bytes compressed:  72.9%
+Zip file size: 3812209 bytes, number of entries: 37
+-rw-r--r--  2.0 unx      567 b- defN 23-May-17 13:00 fbgemm_gpu/__init__.py
+-rw-r--r--  2.0 unx    14800 b- defN 23-May-17 13:00 fbgemm_gpu/_fbgemm_gpu_docs.py
+-rw-r--r--  2.0 unx     2747 b- defN 23-May-17 13:00 fbgemm_gpu/batched_unary_embeddings_ops.py
+-rw-r--r--  2.0 unx      818 b- defN 23-May-17 13:00 fbgemm_gpu/enums.py
+-rwxr-xr-x  2.0 unx 13704384 b- defN 23-May-17 13:00 fbgemm_gpu/fbgemm_gpu_py.so
+-rw-r--r--  2.0 unx     5648 b- defN 23-May-17 13:00 fbgemm_gpu/metrics.py
+-rw-r--r--  2.0 unx     2339 b- defN 23-May-17 13:00 fbgemm_gpu/permute_pooled_embedding_modules.py
+-rw-r--r--  2.0 unx     2477 b- defN 23-May-17 13:00 fbgemm_gpu/permute_pooled_embedding_modules_split.py
+-rw-r--r--  2.0 unx     7682 b- defN 23-May-17 13:00 fbgemm_gpu/quantize_comm.py
+-rw-r--r--  2.0 unx     4005 b- defN 23-May-17 13:00 fbgemm_gpu/quantize_utils.py
+-rw-r--r--  2.0 unx     5727 b- defN 23-May-17 13:00 fbgemm_gpu/split_embedding_configs.py
+-rw-r--r--  2.0 unx     8738 b- defN 23-May-17 13:00 fbgemm_gpu/split_embedding_inference_converter.py
+-rw-r--r--  2.0 unx    20503 b- defN 23-May-17 13:00 fbgemm_gpu/split_embedding_utils.py
+-rw-r--r--  2.0 unx   133833 b- defN 23-May-17 13:00 fbgemm_gpu/split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx    39018 b- defN 23-May-17 13:00 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx      910 b- defN 23-May-17 13:00 fbgemm_gpu/uvm.py
+-rw-r--r--  2.0 unx     1912 b- defN 23-May-17 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
+-rw-r--r--  2.0 unx     4163 b- defN 23-May-17 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
+-rw-r--r--  2.0 unx     4932 b- defN 23-May-17 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
+-rw-r--r--  2.0 unx     4465 b- defN 23-May-17 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     6474 b- defN 23-May-17 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     4501 b- defN 23-May-17 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_weight_decay.py
+-rw-r--r--  2.0 unx     3710 b- defN 23-May-17 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_sgd.py
+-rw-r--r--  2.0 unx     1533 b- defN 23-May-17 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
+-rw-r--r--  2.0 unx     4932 b- defN 23-May-17 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
+-rw-r--r--  2.0 unx     4401 b- defN 23-May-17 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
+-rw-r--r--  2.0 unx     4964 b- defN 23-May-17 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
+-rw-r--r--  2.0 unx     4964 b- defN 23-May-17 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
+-rw-r--r--  2.0 unx     4451 b- defN 23-May-17 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     6460 b- defN 23-May-17 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     4487 b- defN 23-May-17 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py
+-rw-r--r--  2.0 unx     4407 b- defN 23-May-17 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
+-rw-r--r--  2.0 unx     3696 b- defN 23-May-17 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
+-rw-r--r--  2.0 unx     2934 b- defN 23-May-17 13:00 fbgemm_gpu_nightly_cpu-2023.5.17.dist-info/METADATA
+-rw-r--r--  2.0 unx      102 b- defN 23-May-17 13:00 fbgemm_gpu_nightly_cpu-2023.5.17.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-17 13:00 fbgemm_gpu_nightly_cpu-2023.5.17.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4129 b- defN 23-May-17 13:00 fbgemm_gpu_nightly_cpu-2023.5.17.dist-info/RECORD
+37 files, 14035824 bytes uncompressed, 3805233 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -93,20 +93,20 @@
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
 Comment: 
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.5.16.dist-info/METADATA
+Filename: fbgemm_gpu_nightly_cpu-2023.5.17.dist-info/METADATA
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.5.16.dist-info/WHEEL
+Filename: fbgemm_gpu_nightly_cpu-2023.5.17.dist-info/WHEEL
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.5.16.dist-info/top_level.txt
+Filename: fbgemm_gpu_nightly_cpu-2023.5.17.dist-info/top_level.txt
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.5.16.dist-info/RECORD
+Filename: fbgemm_gpu_nightly_cpu-2023.5.17.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fbgemm_gpu/fbgemm_gpu_py.so

### strings --all --bytes=8 {}

```diff
@@ -15423,15 +15423,15 @@
 output_lengths is currently on 
 grad must be on the same device as output_lengths! grad is currently on 
 Tensor 'values' must have 1 dimension(s). Found 
 values must be on the same device as lengths! values is currently on 
 start should be always be positive
  which doesn't have a schema registered yet
 Tried to access the schema for 
-schema_.has_value() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/dispatch/OperatorEntry.h":80, please report a bug to PyTorch. 
+schema_.has_value() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/dispatch/OperatorEntry.h":81, please report a bug to PyTorch. 
 /github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/dispatch/OperatorEntry.h
 Expected TensorList but got 
 toTensorList
 isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2028, please report a bug to PyTorch. 
 isDouble() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":540, please report a bug to PyTorch. 
 isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1952, please report a bug to PyTorch. 
 isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2024, please report a bug to PyTorch.
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -962879,15 +962879,15 @@
 	lea    0x4fce99(%rip),%rcx        # a59c78 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedSliceOp>*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>+0x1d8>
 	mov    $0x3c,%edx
 	lea    0x4fcd4d(%rip),%rsi        # a59b38 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedSliceOp>*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>+0x98>
 	lea    0x4ff0b4(%rip),%rdi        # a5bea6 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<std::tuple<at::Tensor, at::Tensor> (at::Tensor const&, at::Tensor const&, at::Tensor const&, long), &fbgemm_gpu::jagged_slice>, std::tuple<at::Tensor, at::Tensor>, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, at::Tensor const&, long> >+0x506>
 	call   145b90 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, char const*)@plt>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x5d3989(%rip),%rax        # b30790 <fbgemm_gpu::(anonymous namespace)::JaggedToPaddedDenseOp::backward(torch::autograd::AutogradContext*, std::vector<at::Tensor, std::allocator<at::Tensor> >)::op>
-	cmpb   $0x0,0xfa0(%rax)
+	cmpb   $0x0,0xfa8(%rax)
 	je     55c6dc <torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedToPaddedDenseOp>::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)+0x25c>
 	push   -0x190(%rbp)
 	mov    %rbx,%r9
 	mov    %r12,%rcx
 	lea    -0x150(%rbp),%r14
 	push   -0x170(%rbp)
 	lea    -0x98(%rbp),%rdx
@@ -963313,15 +963313,15 @@
 	jmp    55d1b9 <fbgemm_gpu::(anonymous namespace)::JaggedToPaddedDenseOp::forward(torch::autograd::AutogradContext*, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<long, std::allocator<long> > const&, double)+0x99>
 	nopl   0x0(%rax)
 	lea    -0xa9(%rbp),%rsi
 	call   556ac0 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>
 	jmp    55d249 <fbgemm_gpu::(anonymous namespace)::JaggedToPaddedDenseOp::forward(torch::autograd::AutogradContext*, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<long, std::allocator<long> > const&, double)+0x129>
 	nopl   0x0(%rax)
 	mov    0x5d3199(%rip),%rdx        # b307b0 <fbgemm_gpu::(anonymous namespace)::JaggedToPaddedDenseOp::forward(torch::autograd::AutogradContext*, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<long, std::allocator<long> > const&, double)::op>
-	cmpb   $0x0,0xfa0(%rdx)
+	cmpb   $0x0,0xfa8(%rdx)
 	je     55d35d <fbgemm_gpu::(anonymous namespace)::JaggedToPaddedDenseOp::forward(torch::autograd::AutogradContext*, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<long, std::allocator<long> > const&, double)+0x23d>
 	push   -0xc8(%rbp)
 	mov    %r14,%r9
 	mov    %rax,%r8
 	mov    %r15,%rcx
 	push   %rbx
 	lea    -0x98(%rbp),%rdx
@@ -965385,15 +965385,15 @@
 	mov    %rbx,%rsi
 	mov    %rax,-0x1c0(%rbp)
 	call   145db0 <c10::impl::BoxedKernelWrapper<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<long, std::allocator<long> > const&, double), void>::call(c10::BoxedKernel const&, c10::OperatorHandle const&, c10::DispatchKeySet, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<long, std::allocator<long> > const&, double)@plt>
 	pop    %rax
 	pop    %rdx
 	jmp    55f61f <torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp>::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)+0x3cf>
 	mov    0x5d0925(%rip),%rax        # b30750 <fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp::backward(torch::autograd::AutogradContext*, std::vector<at::Tensor, std::allocator<at::Tensor> >)::op>
-	cmpb   $0x0,0xfa0(%rax)
+	cmpb   $0x0,0xfa8(%rax)
 	je     55f5e0 <torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp>::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)+0x390>
 	lea    -0xe0(%rbp),%rax
 	vxorpd %xmm0,%xmm0,%xmm0
 	mov    %rbx,%r8
 	mov    -0x1b8(%rbp),%r9
 	push   %rax
 	mov    -0x198(%rbp),%rdi
@@ -966209,15 +966209,15 @@
 	lea    0x5cf8d6(%rip),%rdx        # b30690 <fbgemm_gpu::(anonymous namespace)::DenseToJaggedOp::backward(torch::autograd::AutogradContext*, std::vector<at::Tensor, std::allocator<at::Tensor> >)::op>
 	mov    %rax,-0x1c0(%rbp)
 	call   145db0 <c10::impl::BoxedKernelWrapper<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<long, std::allocator<long> > const&, double), void>::call(c10::BoxedKernel const&, c10::OperatorHandle const&, c10::DispatchKeySet, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<long, std::allocator<long> > const&, double)@plt>
 	pop    %rax
 	pop    %rdx
 	jmp    560538 <torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::DenseToJaggedOp>::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)+0x3d8>
 	mov    0x5cf8bc(%rip),%rax        # b30690 <fbgemm_gpu::(anonymous namespace)::DenseToJaggedOp::backward(torch::autograd::AutogradContext*, std::vector<at::Tensor, std::allocator<at::Tensor> >)::op>
-	cmpb   $0x0,0xfa0(%rax)
+	cmpb   $0x0,0xfa8(%rax)
 	je     5604fd <torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::DenseToJaggedOp>::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)+0x39d>
 	lea    -0xe0(%rbp),%rax
 	mov    %r13,%r9
 	mov    %rbx,%r8
 	mov    %r12,%rcx
 	push   %rax
 	mov    -0x1a0(%rbp),%rdi
@@ -967190,15 +967190,15 @@
 	nopl   0x0(%rax)
 	cmpb   $0x0,-0x1c9(%rbp)
 	je     561d43 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp, fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<std::vector<at::Tensor, std::allocator<at::Tensor> > const&>)(), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&>(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)+0xc03>
 	jmp    561df8 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp, fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<std::vector<at::Tensor, std::allocator<at::Tensor> > const&>)(), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&>(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)+0xcb8>
 	mov    0x50(%rdi),%rbx
 	jmp    561780 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp, fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<std::vector<at::Tensor, std::allocator<at::Tensor> > const&>)(), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&>(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)+0x640>
 	mov    0x5ce5ae(%rip),%rax        # b30770 <fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp::forward(torch::autograd::AutogradContext*, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)::op>
-	cmpb   $0x0,0xfa0(%rax)
+	cmpb   $0x0,0xfa8(%rax)
 	je     561a40 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp, fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<std::vector<at::Tensor, std::allocator<at::Tensor> > const&>)(), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedDenseDenseAddJaggedOutputOp, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&>(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)+0x900>
 	sub    $0x8,%rsp
 	push   -0x1b8(%rbp)
 	mov    -0x1b0(%rbp),%r9
 	lea    -0x98(%rbp),%rdx
 	push   -0x1a8(%rbp)
 	mov    %rbx,%rcx
@@ -968030,15 +968030,15 @@
 	mov    %rax,-0x1a0(%rbp)
 	lea    -0x180(%rbp),%rax
 	push   %rax
 	mov    %rax,-0x1d8(%rbp)
 	call   144040 <c10::impl::BoxedKernelWrapper<std::tuple<at::Tensor, at::Tensor> (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&), void>::call(c10::BoxedKernel const&, c10::OperatorHandle const&, c10::DispatchKeySet, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@plt>
 	jmp    562a4a <torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp>::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)+0x55a>
 	mov    0x5cd5bd(%rip),%rax        # b30710 <fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp::backward(torch::autograd::AutogradContext*, std::vector<at::Tensor, std::allocator<at::Tensor> >)::op>
-	cmpb   $0x0,0xfa0(%rax)
+	cmpb   $0x0,0xfa8(%rax)
 	je     5629f5 <torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp>::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)+0x505>
 	sub    $0x8,%rsp
 	lea    -0x188(%rbp),%rax
 	lea    -0x170(%rbp),%r12
 	mov    -0x1e0(%rbp),%r8
 	push   %rax
 	mov    -0x198(%rbp),%rcx
@@ -969074,15 +969074,15 @@
 	jmp    564208 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp, fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<std::vector<at::Tensor, std::allocator<at::Tensor> > const&>)(), (declval<at::Tensor const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&>(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)+0xd88>
 	nopl   0x0(%rax)
 	cmpb   $0x0,-0x1c1(%rbp)
 	jne    564010 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp, fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<std::vector<at::Tensor, std::allocator<at::Tensor> > const&>)(), (declval<at::Tensor const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&>(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)+0xb90>
 	jmp    563f5c <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp, fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<std::vector<at::Tensor, std::allocator<at::Tensor> > const&>)(), (declval<at::Tensor const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&>(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)+0xadc>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x5cc131(%rip),%rax        # b30730 <fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp::forward(torch::autograd::AutogradContext*, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)::op>
-	cmpb   $0x0,0xfa0(%rax)
+	cmpb   $0x0,0xfa8(%rax)
 	je     563c45 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp, fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<std::vector<at::Tensor, std::allocator<at::Tensor> > const&>)(), (declval<at::Tensor const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedDenseMulOp, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&>(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)+0x7c5>
 	push   -0x1b0(%rbp)
 	lea    -0x120(%rbp),%rbx
 	mov    -0x1a8(%rbp),%r9
 	lea    -0x98(%rbp),%rdx
 	push   -0x1d0(%rbp)
 	mov    %r12,%rcx
@@ -969807,15 +969807,15 @@
 	lea    0x4f4861(%rip),%rcx        # a59bd8 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedSliceOp>*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>+0x138>
 	mov    $0xe1,%edx
 	lea    0x4f47b5(%rip),%rsi        # a59b38 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedSliceOp>*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>+0x98>
 	lea    0x4f6b1c(%rip),%rdi        # a5bea6 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<std::tuple<at::Tensor, at::Tensor> (at::Tensor const&, at::Tensor const&, at::Tensor const&, long), &fbgemm_gpu::jagged_slice>, std::tuple<at::Tensor, at::Tensor>, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, at::Tensor const&, long> >+0x506>
 	call   145b90 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, char const*)@plt>
 	nop
 	mov    0x5cb339(%rip),%rax        # b306d0 <fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp::backward(torch::autograd::AutogradContext*, std::vector<at::Tensor, std::allocator<at::Tensor> >)::op>
-	cmpb   $0x0,0xfa0(%rax)
+	cmpb   $0x0,0xfa8(%rax)
 	je     564c3e <torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp>::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)+0x27e>
 	sub    $0x8,%rsp
 	lea    -0x160(%rbp),%rax
 	lea    -0x170(%rbp),%r14
 	mov    -0x180(%rbp),%r8
 	push   %rax
 	lea    -0x150(%rbp),%rdi
@@ -970675,15 +970675,15 @@
 	jmp    565ade <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp, fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp>::apply<fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp, at::Tensor const&, at::Tensor const&, at::Tensor const&>(at::Tensor const&, at::Tensor const&, at::Tensor const&)+0x3ce>
 	nopl   0x0(%rax)
 	cmpb   $0x0,-0x1c9(%rbp)
 	je     566214 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp, fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp>::apply<fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp, at::Tensor const&, at::Tensor const&, at::Tensor const&>(at::Tensor const&, at::Tensor const&, at::Tensor const&)+0xb04>
 	jmp    566380 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp, fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp>::apply<fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp, at::Tensor const&, at::Tensor const&, at::Tensor const&>(at::Tensor const&, at::Tensor const&, at::Tensor const&)+0xc70>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x5ca179(%rip),%rax        
-	cmpb   $0x0,0xfa0(%rax)
+	cmpb   $0x0,0xfa8(%rax)
 	je     565f14 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp, fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp>::apply<fbgemm_gpu::(anonymous namespace)::BatchedDenseVecJagged2DMulOp, at::Tensor const&, at::Tensor const&, at::Tensor const&>(at::Tensor const&, at::Tensor const&, at::Tensor const&)+0x804>
 	push   -0x1b8(%rbp)
 	lea    -0xe0(%rbp),%r13
 	mov    -0x1a8(%rbp),%r9
 	lea    -0x98(%rbp),%rdx
 	push   -0x1b0(%rbp)
 	mov    %r14,%rcx
@@ -971229,15 +971229,15 @@
 	lea    0x4ebdff(%rip),%rcx        
 	mov    $0x7a4,%edx
 	lea    0x4eb5fb(%rip),%rsi        
 	lea    0x4eaa45(%rip),%rdi        
 	call   1485f0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	nopl   0x0(%rax)
 	mov    0x5c9739(%rip),%rax        # b306b0 <fbgemm_gpu::(anonymous namespace)::DenseToJaggedOp::forward(torch::autograd::AutogradContext*, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::optional<long> const&)::op>
-	cmpb   $0x0,0xfa0(%rax)
+	cmpb   $0x0,0xfa8(%rax)
 	je     566c18 <fbgemm_gpu::(anonymous namespace)::DenseToJaggedOp::forward(torch::autograd::AutogradContext*, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::optional<long> const&)+0x328>
 	push   -0xe0(%rbp)
 	mov    %r15,%r9
 	mov    %rbx,%r8
 	mov    %r14,%rcx
 	push   -0xd8(%rbp)
 	lea    -0x98(%rbp),%rdx
@@ -973005,15 +973005,15 @@
 	call   145b90 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, char const*)@plt>
 	nop
 	lea    -0x148(%rbp),%rsi
 	call   556ac0 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>
 	jmp    568a17 <torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp>::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)+0x177>
 	nopl   0x0(%rax)
 	mov    0x5c7381(%rip),%rax        # b30650 <fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp::backward(torch::autograd::AutogradContext*, std::vector<at::Tensor, std::allocator<at::Tensor> >)::op>
-	cmpb   $0x0,0xfa0(%rax)
+	cmpb   $0x0,0xfa8(%rax)
 	je     568b5b <torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp>::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)+0x2bb>
 	sub    $0x8,%rsp
 	push   -0x1a0(%rbp)
 	lea    -0x158(%rbp),%rax
 	lea    -0x150(%rbp),%r15
 	push   %rax
 	lea    -0x98(%rbp),%rdx
@@ -973733,15 +973733,15 @@
 	call   145b90 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, char const*)@plt>
 	nop
 	lea    -0x148(%rbp),%rsi
 	call   556ac0 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>
 	jmp    5697cf <torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp>::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)+0x19f>
 	nopl   0x0(%rax)
 	mov    0x5c6581(%rip),%rax        # b30610 <fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp::backward(torch::autograd::AutogradContext*, std::vector<at::Tensor, std::allocator<at::Tensor> >)::op>
-	cmpb   $0x0,0xfa0(%rax)
+	cmpb   $0x0,0xfa8(%rax)
 	je     569889 <torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp>::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)+0x259>
 	sub    $0x8,%rsp
 	push   -0x198(%rbp)
 	lea    -0x158(%rbp),%rax
 	mov    -0x1a0(%rbp),%r9
 	push   -0x178(%rbp)
 	lea    -0x98(%rbp),%rdx
@@ -973752,15 +973752,15 @@
 	lea    0x5c6539(%rip),%rsi        # b30610 <fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp::backward(torch::autograd::AutogradContext*, std::vector<at::Tensor, std::allocator<at::Tensor> >)::op>
 	mov    %rax,-0x1d0(%rbp)
 	call   146370 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, at::Tensor const&, at::Tensor const&, long>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, long)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@plt>
 	add    $0x20,%rsp
 	jmp    5698d3 <torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp>::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)+0x2a3>
 	nopl   0x0(%rax)
 	mov    0x5c6519(%rip),%rax        # b30610 <fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp::backward(torch::autograd::AutogradContext*, std::vector<at::Tensor, std::allocator<at::Tensor> >)::op>
-	cmpb   $0x0,0xfa0(%rax)
+	cmpb   $0x0,0xfa8(%rax)
 	je     56995e <torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp>::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)+0x32e>
 	sub    $0x8,%rsp
 	push   -0x198(%rbp)
 	lea    -0x150(%rbp),%rax
 	mov    -0x1c8(%rbp),%r8
 	push   -0x1a8(%rbp)
 	mov    %r13,%r9
@@ -974674,15 +974674,15 @@
 	jmp    56a87d <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp, fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<long const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp, at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&>(at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&)+0x3dd>
 	nopl   0x0(%rax)
 	cmpb   $0x0,-0x1c9(%rbp)
 	jne    56b1d0 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp, fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<long const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp, at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&>(at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&)+0xd30>
 	jmp    56b066 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp, fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<long const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp, at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&>(at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&)+0xbc6>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x5c5259(%rip),%rax        
-	cmpb   $0x0,0xfa0(%rax)
+	cmpb   $0x0,0xfa8(%rax)
 	je     56ad61 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp, fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<long const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedJaggedBmmOp, at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&>(at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&)+0x8c1>
 	sub    $0x8,%rsp
 	push   -0x1e8(%rbp)
 	mov    -0x1a8(%rbp),%r9
 	lea    -0x98(%rbp),%rdx
 	push   -0x1b8(%rbp)
 	mov    %r13,%rcx
@@ -975428,15 +975428,15 @@
 	call   145b90 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, char const*)@plt>
 	nopl   (%rax)
 	lea    -0x148(%rbp),%rsi
 	call   556ac0 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>
 	jmp    56b836 <torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp>::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)+0x1a6>
 	nopl   0x0(%rax)
 	mov    0x5c43c1(%rip),%rax        # b305b0 <fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp::backward(torch::autograd::AutogradContext*, std::vector<at::Tensor, std::allocator<at::Tensor> >)::op2>
-	cmpb   $0x0,0xfa0(%rax)
+	cmpb   $0x0,0xfa8(%rax)
 	je     56b9f3 <torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp>::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)+0x363>
 	sub    $0x8,%rsp
 	push   -0x188(%rbp)
 	lea    -0x158(%rbp),%rax
 	mov    -0x1d0(%rbp),%r8
 	push   %r12
 	lea    -0x98(%rbp),%rdx
@@ -975447,15 +975447,15 @@
 	lea    0x5c4379(%rip),%rsi        # b305b0 <fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp::backward(torch::autograd::AutogradContext*, std::vector<at::Tensor, std::allocator<at::Tensor> >)::op2>
 	mov    %rax,-0x1e0(%rbp)
 	call   146370 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, at::Tensor const&, at::Tensor const&, long>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, long)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@plt>
 	add    $0x20,%rsp
 	jmp    56ba3d <torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp>::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)+0x3ad>
 	nopl   0x0(%rax)
 	mov    0x5c4379(%rip),%rax        # b305d0 <fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp::backward(torch::autograd::AutogradContext*, std::vector<at::Tensor, std::allocator<at::Tensor> >)::op>
-	cmpb   $0x0,0xfa0(%rax)
+	cmpb   $0x0,0xfa8(%rax)
 	je     56b8fc <torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp>::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)+0x26c>
 	sub    $0x8,%rsp
 	push   -0x188(%rbp)
 	lea    -0x160(%rbp),%rax
 	mov    -0x1b0(%rbp),%r9
 	push   %r14
 	lea    -0x98(%rbp),%rdx
@@ -976387,15 +976387,15 @@
 	jmp    56ca3d <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp, fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<long const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp, at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&>(at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&)+0x3dd>
 	nopl   0x0(%rax)
 	cmpb   $0x0,-0x1c9(%rbp)
 	jne    56d390 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp, fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<long const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp, at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&>(at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&)+0xd30>
 	jmp    56d226 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp, fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<long const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp, at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&>(at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&)+0xbc6>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x5c3059(%rip),%rax        
-	cmpb   $0x0,0xfa0(%rax)
+	cmpb   $0x0,0xfa8(%rax)
 	je     56cf21 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp, fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<long const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedDenseBmmOp, at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&>(at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&)+0x8c1>
 	sub    $0x8,%rsp
 	push   -0x1e8(%rbp)
 	mov    -0x1a8(%rbp),%r9
 	lea    -0x98(%rbp),%rdx
 	push   -0x1b8(%rbp)
 	mov    %r13,%rcx
@@ -977246,15 +977246,15 @@
 	jmp    56dc0f <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp, fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<long const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp, at::Tensor const&, at::Tensor const&, long const&>(at::Tensor const&, at::Tensor const&, long const&)+0x3bf>
 	nopl   0x0(%rax)
 	cmpb   $0x0,-0x1c1(%rbp)
 	jne    56e520 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp, fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<long const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp, at::Tensor const&, at::Tensor const&, long const&>(at::Tensor const&, at::Tensor const&, long const&)+0xcd0>
 	jmp    56e3a5 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp, fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<long const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp, at::Tensor const&, at::Tensor const&, long const&>(at::Tensor const&, at::Tensor const&, long const&)+0xb55>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x5c1f69(%rip),%rax        
-	cmpb   $0x0,0xfa0(%rax)
+	cmpb   $0x0,0xfa8(%rax)
 	je     56df22 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp, fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<long const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedSoftmaxOp, at::Tensor const&, at::Tensor const&, long const&>(at::Tensor const&, at::Tensor const&, long const&)+0x6d2>
 	push   -0x1d8(%rbp)
 	lea    -0x100(%rbp),%rbx
 	mov    -0x1b0(%rbp),%r9
 	lea    -0x98(%rbp),%rdx
 	push   -0x1a8(%rbp)
 	mov    %r14,%rcx
@@ -978122,15 +978122,15 @@
 	lea    0x4e36d1(%rip),%rcx        
 	mov    $0x285,%edx
 	lea    0x4e3775(%rip),%rsi        
 	lea    0x4e2211(%rip),%rdi        
 	call   145b90 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, char const*)@plt>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x5c0db9(%rip),%rax        # b30570 <fbgemm_gpu::(anonymous namespace)::JaggedIndexSelect2dOp::backward(torch::autograd::AutogradContext*, std::vector<at::Tensor, std::allocator<at::Tensor> >)::op>
-	cmpb   $0x0,0xfa0(%rax)
+	cmpb   $0x0,0xfa8(%rax)
 	je     56eed9 <torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedIndexSelect2dOp>::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)+0x3e9>
 	sub    $0x8,%rsp
 	push   -0x1e0(%rbp)
 	lea    -0x168(%rbp),%rax
 	lea    -0x160(%rbp),%r15
 	push   -0x1c8(%rbp)
 	mov    %r15,%r9
@@ -979293,15 +979293,15 @@
 	jmp    570a41 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedIndexSelect2dOp, fbgemm_gpu::(anonymous namespace)::JaggedIndexSelect2dOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedIndexSelect2dOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedIndexSelect2dOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedIndexSelect2dOp, at::Tensor const&, at::Tensor const&, at::Tensor const&>(at::Tensor const&, at::Tensor const&, at::Tensor const&)+0xeb1>
 	lea    0x4dff5d(%rip),%rcx        
 	mov    $0x4e5,%edx
 	lea    0x4dff85(%rip),%rsi        
 	lea    0x4dff68(%rip),%rdi        
 	call   145b90 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, char const*)@plt>
 	mov    0x5bf58a(%rip),%rax        
-	cmpb   $0x0,0xfa0(%rax)
+	cmpb   $0x0,0xfa8(%rax)
 	je     570708 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedIndexSelect2dOp, fbgemm_gpu::(anonymous namespace)::JaggedIndexSelect2dOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedIndexSelect2dOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedIndexSelect2dOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedIndexSelect2dOp, at::Tensor const&, at::Tensor const&, at::Tensor const&>(at::Tensor const&, at::Tensor const&, at::Tensor const&)+0xb78>
 	push   -0x210(%rbp)
 	mov    %r14,%r8
 	mov    %r13,%rcx
 	mov    -0x1b8(%rbp),%r9
 	push   -0x1e0(%rbp)
 	lea    -0x98(%rbp),%rdx
@@ -980094,15 +980094,15 @@
 	lea    0x4e0f11(%rip),%rcx        
 	mov    $0x285,%edx
 	lea    0x4e0fb5(%rip),%rsi        
 	lea    0x4dfa51(%rip),%rdi        
 	call   145b90 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, char const*)@plt>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x5be5b9(%rip),%rax        # b30530 <fbgemm_gpu::(anonymous namespace)::JaggedSliceOp::backward(torch::autograd::AutogradContext*, std::vector<at::Tensor, std::allocator<at::Tensor> >)::op>
-	cmpb   $0x0,0xfa0(%rax)
+	cmpb   $0x0,0xfa8(%rax)
 	je     5716a3 <torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedSliceOp>::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)+0x403>
 	sub    $0x8,%rsp
 	lea    -0x170(%rbp),%rax
 	lea    -0x180(%rbp),%r14
 	mov    -0x1d0(%rbp),%r8
 	push   $0x1
 	lea    -0x160(%rbp),%r9
@@ -981304,15 +981304,15 @@
 	lea    -0x280(%rbp),%rsi
 	call   556ac0 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>
 	jmp    572d87 <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedSliceOp, fbgemm_gpu::(anonymous namespace)::JaggedSliceOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedSliceOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<long const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedSliceOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedSliceOp, at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&>(at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&)+0xa07>
 	lea    -0x280(%rbp),%rsi
 	call   556ac0 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>
 	jmp    572e1b <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedSliceOp, fbgemm_gpu::(anonymous namespace)::JaggedSliceOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedSliceOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<long const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedSliceOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedSliceOp, at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&>(at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&)+0xa9b>
 	mov    0x5bcd14(%rip),%rax        
-	cmpb   $0x0,0xfa0(%rax)
+	cmpb   $0x0,0xfa8(%rax)
 	je     572f5b <std::enable_if<std::is_same<fbgemm_gpu::(anonymous namespace)::JaggedSliceOp, fbgemm_gpu::(anonymous namespace)::JaggedSliceOp>::value, decltype (fbgemm_gpu::(anonymous namespace)::JaggedSliceOp::forward(decltype(nullptr), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<at::Tensor const&>)(), (declval<long const&>)()))>::type torch::autograd::Function<fbgemm_gpu::(anonymous namespace)::JaggedSliceOp>::apply<fbgemm_gpu::(anonymous namespace)::JaggedSliceOp, at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&>(at::Tensor const&, at::Tensor const&, at::Tensor const&, long const&)+0xbdb>
 	sub    $0x8,%rsp
 	mov    %rbx,%r8
 	mov    %r13,%rcx
 	mov    -0x2b0(%rbp),%r9
 	push   $0x0
 	mov    -0x2c0(%rbp),%rdi
@@ -982486,15 +982486,15 @@
 	mov    %rbp,%rcx
 	mov    %rbx,%rdi
 	lea    0x4e5d15(%rip),%rax        # a5a648 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedSliceOp>*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>+0xba8>
 	mov    %rax,0x10(%rsp)
 	call   1448c0 <c10::detail::_str_wrapper<char const*, c10::OperatorName const&, char const*>::call(char const* const&, c10::OperatorName const&, char const* const&)@plt>
 	mov    %rbx,%r8
 	lea    0x4e5d21(%rip),%rcx        # a5a668 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedSliceOp>*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>+0xbc8>
-	mov    $0x50,%edx
+	mov    $0x51,%edx
 	lea    0x4e5de5(%rip),%rsi        # a5a738 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedSliceOp>*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>+0xc98>
 	lea    0x4e5e54(%rip),%rdi        # a5a7ae <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::(anonymous namespace)::JaggedSliceOp>*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>+0xd0e>
 	call   1485f0 <c10::detail::torchInternalAssertFail(char const*, char const*, unsigned int, char const*, std::string const&)@plt>
 	mov    %rax,%r12
 	mov    0x8(%rsp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    0x5ae7ee(%rip),%rdi
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -11884,15 +11884,15 @@
   0x00a5a690 45442061 7420222f 67697468 75622f68 ED at "/github/h
   0x00a5a6a0 6f6d652f 6d696e69 636f6e64 612f656e ome/miniconda/en
   0x00a5a6b0 76732f62 75696c64 5f62696e 6172792f vs/build_binary/
   0x00a5a6c0 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x00a5a6d0 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00a5a6e0 682f696e 636c7564 652f4154 656e2f63 h/include/ATen/c
   0x00a5a6f0 6f72652f 64697370 61746368 2f4f7065 ore/dispatch/Ope
-  0x00a5a700 7261746f 72456e74 72792e68 223a3830 ratorEntry.h":80
+  0x00a5a700 7261746f 72456e74 72792e68 223a3831 ratorEntry.h":81
   0x00a5a710 2c20706c 65617365 20726570 6f727420 , please report 
   0x00a5a720 61206275 6720746f 20507954 6f726368 a bug to PyTorch
   0x00a5a730 2e200000 00000000 2f676974 6875622f . ....../github/
   0x00a5a740 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00a5a750 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
   0x00a5a760 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
   0x00a5a770 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
```

## Comparing `fbgemm_gpu_nightly_cpu-2023.5.16.dist-info/METADATA` & `fbgemm_gpu_nightly_cpu-2023.5.17.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbgemm-gpu-nightly-cpu
-Version: 2023.5.16
+Version: 2023.5.17
 Home-page: https://github.com/pytorch/fbgemm
 Author: FBGEMM Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: PyTorch,Recommendation Models,High Performance Computing,GPU,CUDA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `fbgemm_gpu_nightly_cpu-2023.5.16.dist-info/RECORD` & `fbgemm_gpu_nightly_cpu-2023.5.17.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 fbgemm_gpu/__init__.py,sha256=hyPNE6QvlwUNM4PlyfKee7j7agkOF2SNoT3EQXJ-pe0,567
 fbgemm_gpu/_fbgemm_gpu_docs.py,sha256=d1eWCuXlA6GFuwZ4fZZ_2b7rLec6dqoD91BhRdY19Ys,14800
 fbgemm_gpu/batched_unary_embeddings_ops.py,sha256=rc49BZwtZuu8qsO5MENAlHeswgPUn35aM8Cgr3XtBE0,2747
 fbgemm_gpu/enums.py,sha256=Tg1pBJrcfSIWmWec2WCZkRuMwmCnepKrcACi3ZijZmk,818
-fbgemm_gpu/fbgemm_gpu_py.so,sha256=7Yu0bvRwkrx1vWj565-WfdfPVV9nYJ1u8DupaNKs6PI,13704384
+fbgemm_gpu/fbgemm_gpu_py.so,sha256=P_d9F4d24P7CbEC1jWPdibs8LJXOXM3npMk5LP1JQ4E,13704384
 fbgemm_gpu/metrics.py,sha256=e5VnTatZjFqcgOfipH7Eqk5lsAkuxY2qsbil3Csy_yk,5648
 fbgemm_gpu/permute_pooled_embedding_modules.py,sha256=n80gTkNwSA9k0dvJeZhVjzXC08c74o0G-u4MnKs7rek,2339
 fbgemm_gpu/permute_pooled_embedding_modules_split.py,sha256=9MWBghoy5eajS4yleFWAMdi0LWV0nNbcIgCkqdkRP5g,2477
 fbgemm_gpu/quantize_comm.py,sha256=qONCevOTVA89K7vFJe-Bcc903lHsKDg6s661pTHCF2k,7682
 fbgemm_gpu/quantize_utils.py,sha256=pnZCkIeYxPnvwkIVsRdfPeGBLVXSpEdSsFLH2Ygk7D0,4005
 fbgemm_gpu/split_embedding_configs.py,sha256=o5RUPVwuuQx75T4QsvXKjMKAMQ915EXso8Wpyjgrhvg,5727
 fbgemm_gpu/split_embedding_inference_converter.py,sha256=ruYOwgdI_6ZPR2_YoJ1UBzVeUQt9yRWFWhBnkhx6u_A,8738
@@ -27,11 +27,11 @@
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py,sha256=fBw0hDYHVaob9Pc2IC_XnpQ0jRStbG9R-IZqBnMywRM,4964
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py,sha256=z_INEdVlMxPi-rrq4W7oma6YnJF6EqHFIJeD1VdJNh0,4964
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py,sha256=YO8izH_FCVjxnhlf-Rx3uwTYrKJeERYEGki-QwnWmag,4451
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py,sha256=5NeEd5Vx-cEpJMLTXFbJqlUtbKptFtx6lFpTSrd6xKA,6460
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py,sha256=aL3HeCkQw88kBm685hn1QQJpEtQvKha_XAki6GtzpUU,4487
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py,sha256=qOeMzSHbEm74uOWD4W5r5UPZ1NpBqZefvYZS41_9kbE,4407
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py,sha256=IjeKrN7_9l5SZppuc2WbOR8sv6JtRew5geHKKRIRexY,3696
-fbgemm_gpu_nightly_cpu-2023.5.16.dist-info/METADATA,sha256=QoFgFimpPeZwR-B6PGV4wB1FYhb5RtfiY2CgvOK3q4U,2934
-fbgemm_gpu_nightly_cpu-2023.5.16.dist-info/WHEEL,sha256=7fnRuWrgVZ-We1c67_7QZCYn_AQfJ-Z7mCmVro0eJMM,102
-fbgemm_gpu_nightly_cpu-2023.5.16.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
-fbgemm_gpu_nightly_cpu-2023.5.16.dist-info/RECORD,,
+fbgemm_gpu_nightly_cpu-2023.5.17.dist-info/METADATA,sha256=7xNy2XezQNGdS65oaoHu0vGK-Kg_vrxKJTtMxet753U,2934
+fbgemm_gpu_nightly_cpu-2023.5.17.dist-info/WHEEL,sha256=7fnRuWrgVZ-We1c67_7QZCYn_AQfJ-Z7mCmVro0eJMM,102
+fbgemm_gpu_nightly_cpu-2023.5.17.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
+fbgemm_gpu_nightly_cpu-2023.5.17.dist-info/RECORD,,
```

