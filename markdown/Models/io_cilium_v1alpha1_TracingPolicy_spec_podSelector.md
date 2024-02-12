# io_cilium_v1alpha1_TracingPolicy_spec_podSelector
## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
| **matchExpressions** | [**List**](io_cilium_v1alpha1_TracingPolicy_spec_podSelector_matchExpressions_inner.md) | matchExpressions is a list of label selector requirements. The requirements are ANDed. | [optional] [default to null] |
| **matchLabels** | **Map** | matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \&quot;key\&quot;, the operator is \&quot;In\&quot;, and the values array contains only \&quot;value\&quot;. The requirements are ANDed. | [optional] [default to null] |

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

