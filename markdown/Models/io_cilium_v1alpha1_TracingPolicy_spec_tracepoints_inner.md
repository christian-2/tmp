# io_cilium_v1alpha1_TracingPolicy_spec_tracepoints_inner
## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
| **args** | [**List**](io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_args_inner.md) | A list of function arguments to include in the trace output. | [optional] [default to null] |
| **event** | **String** | Tracepoint event | [default to null] |
| **selectors** | [**List**](io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_selectors_inner.md) | Selectors to apply before producing trace output. Selectors are ORed. | [optional] [default to null] |
| **subsystem** | **String** | Tracepoint subsystem | [default to null] |

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

