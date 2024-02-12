# io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_returnArg
## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
| **index** | **Integer** | Position of the argument. | [default to null] |
| **label** | **String** | Label to output in the JSON | [optional] [default to null] |
| **maxData** | **Boolean** | Read maximum possible data (currently 327360). This field is only used for char_buff data. When this value is false (default), the bpf program will fetch at most 4096 bytes. In later kernels (&gt;&#x3D;5.4) tetragon supports fetching up to 327360 bytes if this flag is turned on | [optional] [default to false] |
| **returnCopy** | **Boolean** | This field is used only for char_buf and char_iovec types. It indicates that this argument should be read later (when the kretprobe for the symbol is triggered) because it might not be populated when the kprobe is triggered at the entrance of the function. For example, a buffer supplied to read(2) won&#39;t have content until kretprobe is triggered. | [optional] [default to false] |
| **sizeArgIndex** | **Integer** | Specifies the position of the corresponding size argument for this argument. This field is used only for char_buf and char_iovec types. | [optional] [default to null] |
| **type** | **String** | Argument type. | [default to auto] |

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

