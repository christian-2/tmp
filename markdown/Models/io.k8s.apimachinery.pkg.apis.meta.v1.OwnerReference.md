# io.k8s.apimachinery.pkg.apis.meta.v1.OwnerReference
## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
| **apiVersion** | **String** | API version of the referent. | [default to ] |
| **blockOwnerDeletion** | **Boolean** | If true, AND if the owner has the \&quot;foregroundDeletion\&quot; finalizer, then the owner cannot be deleted from the key-value store until this reference is removed. See https://kubernetes.io/docs/concepts/architecture/garbage-collection/#foreground-deletion for how the garbage collector interacts with this field and enforces the foreground deletion. Defaults to false. To set this field, a user needs \&quot;delete\&quot; permission of the owner, otherwise 422 (Unprocessable Entity) will be returned. | [optional] [default to null] |
| **controller** | **Boolean** | If true, this reference points to the managing controller. | [optional] [default to null] |
| **kind** | **String** | Kind of the referent. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds | [default to ] |
| **name** | **String** | Name of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names#names | [default to ] |
| **uid** | **String** | UID of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names#uids | [default to ] |

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

