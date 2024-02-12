# Documentation for Kubernetes CRD Swagger

<a name="documentation-for-api-endpoints"></a>
## Documentation for API Endpoints

All URIs are relative to *http://localhost*

| Class | Method | HTTP request | Description |
|------------ | ------------- | ------------- | -------------|
| *CiliumIoV1alpha1Api* | [**createCiliumIoV1alpha1NamespacedTracingPolicyNamespaced**](Apis/CiliumIoV1alpha1Api.md#createciliumiov1alpha1namespacedtracingpolicynamespaced) | **POST** /apis/cilium.io/v1alpha1/namespaces/{namespace}/tracingpoliciesnamespaced | create a TracingPolicyNamespaced |
*CiliumIoV1alpha1Api* | [**createCiliumIoV1alpha1TracingPolicy**](Apis/CiliumIoV1alpha1Api.md#createciliumiov1alpha1tracingpolicy) | **POST** /apis/cilium.io/v1alpha1/tracingpolicies | create a TracingPolicy |
*CiliumIoV1alpha1Api* | [**deleteCiliumIoV1alpha1CollectionNamespacedTracingPolicyNamespaced**](Apis/CiliumIoV1alpha1Api.md#deleteciliumiov1alpha1collectionnamespacedtracingpolicynamespaced) | **DELETE** /apis/cilium.io/v1alpha1/namespaces/{namespace}/tracingpoliciesnamespaced | delete collection of TracingPolicyNamespaced |
*CiliumIoV1alpha1Api* | [**deleteCiliumIoV1alpha1CollectionTracingPolicy**](Apis/CiliumIoV1alpha1Api.md#deleteciliumiov1alpha1collectiontracingpolicy) | **DELETE** /apis/cilium.io/v1alpha1/tracingpolicies | delete collection of TracingPolicy |
*CiliumIoV1alpha1Api* | [**deleteCiliumIoV1alpha1NamespacedTracingPolicyNamespaced**](Apis/CiliumIoV1alpha1Api.md#deleteciliumiov1alpha1namespacedtracingpolicynamespaced) | **DELETE** /apis/cilium.io/v1alpha1/namespaces/{namespace}/tracingpoliciesnamespaced/{name} | delete a TracingPolicyNamespaced |
*CiliumIoV1alpha1Api* | [**deleteCiliumIoV1alpha1TracingPolicy**](Apis/CiliumIoV1alpha1Api.md#deleteciliumiov1alpha1tracingpolicy) | **DELETE** /apis/cilium.io/v1alpha1/tracingpolicies/{name} | delete a TracingPolicy |
*CiliumIoV1alpha1Api* | [**listCiliumIoV1alpha1NamespacedTracingPolicyNamespaced**](Apis/CiliumIoV1alpha1Api.md#listciliumiov1alpha1namespacedtracingpolicynamespaced) | **GET** /apis/cilium.io/v1alpha1/namespaces/{namespace}/tracingpoliciesnamespaced | list objects of kind TracingPolicyNamespaced |
*CiliumIoV1alpha1Api* | [**listCiliumIoV1alpha1TracingPolicy**](Apis/CiliumIoV1alpha1Api.md#listciliumiov1alpha1tracingpolicy) | **GET** /apis/cilium.io/v1alpha1/tracingpolicies | list objects of kind TracingPolicy |
*CiliumIoV1alpha1Api* | [**listCiliumIoV1alpha1TracingPolicyNamespacedForAllNamespaces**](Apis/CiliumIoV1alpha1Api.md#listciliumiov1alpha1tracingpolicynamespacedforallnamespaces) | **GET** /apis/cilium.io/v1alpha1/tracingpoliciesnamespaced | list objects of kind TracingPolicyNamespaced |
*CiliumIoV1alpha1Api* | [**patchCiliumIoV1alpha1NamespacedTracingPolicyNamespaced**](Apis/CiliumIoV1alpha1Api.md#patchciliumiov1alpha1namespacedtracingpolicynamespaced) | **PATCH** /apis/cilium.io/v1alpha1/namespaces/{namespace}/tracingpoliciesnamespaced/{name} | partially update the specified TracingPolicyNamespaced |
*CiliumIoV1alpha1Api* | [**patchCiliumIoV1alpha1TracingPolicy**](Apis/CiliumIoV1alpha1Api.md#patchciliumiov1alpha1tracingpolicy) | **PATCH** /apis/cilium.io/v1alpha1/tracingpolicies/{name} | partially update the specified TracingPolicy |
*CiliumIoV1alpha1Api* | [**readCiliumIoV1alpha1NamespacedTracingPolicyNamespaced**](Apis/CiliumIoV1alpha1Api.md#readciliumiov1alpha1namespacedtracingpolicynamespaced) | **GET** /apis/cilium.io/v1alpha1/namespaces/{namespace}/tracingpoliciesnamespaced/{name} | read the specified TracingPolicyNamespaced |
*CiliumIoV1alpha1Api* | [**readCiliumIoV1alpha1TracingPolicy**](Apis/CiliumIoV1alpha1Api.md#readciliumiov1alpha1tracingpolicy) | **GET** /apis/cilium.io/v1alpha1/tracingpolicies/{name} | read the specified TracingPolicy |
*CiliumIoV1alpha1Api* | [**replaceCiliumIoV1alpha1NamespacedTracingPolicyNamespaced**](Apis/CiliumIoV1alpha1Api.md#replaceciliumiov1alpha1namespacedtracingpolicynamespaced) | **PUT** /apis/cilium.io/v1alpha1/namespaces/{namespace}/tracingpoliciesnamespaced/{name} | replace the specified TracingPolicyNamespaced |
*CiliumIoV1alpha1Api* | [**replaceCiliumIoV1alpha1TracingPolicy**](Apis/CiliumIoV1alpha1Api.md#replaceciliumiov1alpha1tracingpolicy) | **PUT** /apis/cilium.io/v1alpha1/tracingpolicies/{name} | replace the specified TracingPolicy |


<a name="documentation-for-models"></a>
## Documentation for Models

 - [io.cilium.v1alpha1.TracingPolicy](./Models/io.cilium.v1alpha1.TracingPolicy.md)
 - [io.cilium.v1alpha1.TracingPolicyList](./Models/io.cilium.v1alpha1.TracingPolicyList.md)
 - [io.cilium.v1alpha1.TracingPolicyNamespaced](./Models/io.cilium.v1alpha1.TracingPolicyNamespaced.md)
 - [io.cilium.v1alpha1.TracingPolicyNamespacedList](./Models/io.cilium.v1alpha1.TracingPolicyNamespacedList.md)
 - [io.k8s.apimachinery.pkg.apis.meta.v1.DeleteOptions](./Models/io.k8s.apimachinery.pkg.apis.meta.v1.DeleteOptions.md)
 - [io.k8s.apimachinery.pkg.apis.meta.v1.ListMeta](./Models/io.k8s.apimachinery.pkg.apis.meta.v1.ListMeta.md)
 - [io.k8s.apimachinery.pkg.apis.meta.v1.ManagedFieldsEntry](./Models/io.k8s.apimachinery.pkg.apis.meta.v1.ManagedFieldsEntry.md)
 - [io.k8s.apimachinery.pkg.apis.meta.v1.ObjectMeta](./Models/io.k8s.apimachinery.pkg.apis.meta.v1.ObjectMeta.md)
 - [io.k8s.apimachinery.pkg.apis.meta.v1.OwnerReference](./Models/io.k8s.apimachinery.pkg.apis.meta.v1.OwnerReference.md)
 - [io.k8s.apimachinery.pkg.apis.meta.v1.Preconditions](./Models/io.k8s.apimachinery.pkg.apis.meta.v1.Preconditions.md)
 - [io.k8s.apimachinery.pkg.apis.meta.v1.Status](./Models/io.k8s.apimachinery.pkg.apis.meta.v1.Status.md)
 - [io.k8s.apimachinery.pkg.apis.meta.v1.StatusCause](./Models/io.k8s.apimachinery.pkg.apis.meta.v1.StatusCause.md)
 - [io.k8s.apimachinery.pkg.apis.meta.v1.StatusDetails](./Models/io.k8s.apimachinery.pkg.apis.meta.v1.StatusDetails.md)
 - [io_cilium_v1alpha1_TracingPolicy_spec](./Models/io_cilium_v1alpha1_TracingPolicy_spec.md)
 - [io_cilium_v1alpha1_TracingPolicy_spec_killers_inner](./Models/io_cilium_v1alpha1_TracingPolicy_spec_killers_inner.md)
 - [io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner](./Models/io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner.md)
 - [io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_args_inner](./Models/io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_args_inner.md)
 - [io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_returnArg](./Models/io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_returnArg.md)
 - [io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_selectors_inner](./Models/io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_selectors_inner.md)
 - [io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_selectors_inner_matchActions_inner](./Models/io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_selectors_inner_matchActions_inner.md)
 - [io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_selectors_inner_matchArgs_inner](./Models/io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_selectors_inner_matchArgs_inner.md)
 - [io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_selectors_inner_matchBinaries_inner](./Models/io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_selectors_inner_matchBinaries_inner.md)
 - [io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_selectors_inner_matchCapabilities_inner](./Models/io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_selectors_inner_matchCapabilities_inner.md)
 - [io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_selectors_inner_matchNamespaceChanges_inner](./Models/io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_selectors_inner_matchNamespaceChanges_inner.md)
 - [io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_selectors_inner_matchNamespaces_inner](./Models/io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_selectors_inner_matchNamespaces_inner.md)
 - [io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_selectors_inner_matchPIDs_inner](./Models/io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_selectors_inner_matchPIDs_inner.md)
 - [io_cilium_v1alpha1_TracingPolicy_spec_lists_inner](./Models/io_cilium_v1alpha1_TracingPolicy_spec_lists_inner.md)
 - [io_cilium_v1alpha1_TracingPolicy_spec_options_inner](./Models/io_cilium_v1alpha1_TracingPolicy_spec_options_inner.md)
 - [io_cilium_v1alpha1_TracingPolicy_spec_podSelector](./Models/io_cilium_v1alpha1_TracingPolicy_spec_podSelector.md)
 - [io_cilium_v1alpha1_TracingPolicy_spec_podSelector_matchExpressions_inner](./Models/io_cilium_v1alpha1_TracingPolicy_spec_podSelector_matchExpressions_inner.md)
 - [io_cilium_v1alpha1_TracingPolicy_spec_tracepoints_inner](./Models/io_cilium_v1alpha1_TracingPolicy_spec_tracepoints_inner.md)
 - [io_cilium_v1alpha1_TracingPolicy_spec_uprobes_inner](./Models/io_cilium_v1alpha1_TracingPolicy_spec_uprobes_inner.md)


<a name="documentation-for-authorization"></a>
## Documentation for Authorization

All endpoints do not require authorization.
