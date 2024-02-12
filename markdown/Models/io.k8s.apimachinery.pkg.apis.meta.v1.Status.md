# io.k8s.apimachinery.pkg.apis.meta.v1.Status
## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
| **apiVersion** | **String** | APIVersion defines the versioned schema of this representation of an object. Servers should convert recognized schemas to the latest internal value, and may reject unrecognized values. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources | [optional] [default to null] |
| **code** | **Integer** | Suggested HTTP return code for this status, 0 if not set. | [optional] [default to null] |
| **details** | [**io.k8s.apimachinery.pkg.apis.meta.v1.StatusDetails**](io.k8s.apimachinery.pkg.apis.meta.v1.StatusDetails.md) | Extended data associated with the reason.  Each reason may define its own extended details. This field is optional and the data returned is not guaranteed to conform to any schema except that defined by the reason type. | [optional] [default to null] |
| **kind** | **String** | Kind is a string value representing the REST resource this object represents. Servers may infer this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds | [optional] [default to null] |
| **message** | **String** | A human-readable description of the status of this operation. | [optional] [default to null] |
| **metadata** | [**io.k8s.apimachinery.pkg.apis.meta.v1.ListMeta**](io.k8s.apimachinery.pkg.apis.meta.v1.ListMeta.md) | Standard list metadata. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds | [optional] [default to {}] |
| **reason** | **String** | A machine-readable description of why this operation is in the \&quot;Failure\&quot; status. If this value is empty there is no information available. A Reason clarifies an HTTP status code but does not override it. | [optional] [default to null] |
| **status** | **String** | Status of the operation. One of: \&quot;Success\&quot; or \&quot;Failure\&quot;. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#spec-and-status | [optional] [default to null] |

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

