# io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner
## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
| **args** | [**List**](io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_args_inner.md) | A list of function arguments to include in the trace output. | [optional] [default to null] |
| **call** | **String** | Name of the function to apply the kprobe spec to. | [default to null] |
| **return** | **Boolean** | Indicates whether to collect return value of the traced function. | [optional] [default to false] |
| **returnArg** | [**io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_returnArg**](io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_returnArg.md) |  | [optional] [default to null] |
| **returnArgAction** | **String** | An action to perform on the return argument. Available actions are: Post;TrackSock;UntrackSock | [optional] [default to null] |
| **selectors** | [**List**](io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_selectors_inner.md) | Selectors to apply before producing trace output. Selectors are ORed. | [optional] [default to null] |
| **syscall** | **Boolean** | Indicates whether the traced function is a syscall. | [optional] [default to true] |

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

